# Comparing `tmp/latch_postgres-0.1.6.tar.gz` & `tmp/latch_postgres-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_postgres-0.1.6.tar", max compression
+gzip compressed data, was "latch_postgres-0.1.7.tar", max compression
```

## Comparing `latch_postgres-0.1.6.tar` & `latch_postgres-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.6/LICENSE
--rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.6/latch_postgres/__init__.py
--rw-r--r--   0        0        0    24177 2023-05-10 17:24:58.509088 latch_postgres-0.1.6/latch_postgres/postgres.py
--rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.6/latch_postgres/py.typed
--rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.6/latch_postgres/retries.py
--rw-r--r--   0        0        0     1018 2023-05-10 17:24:55.837956 latch_postgres-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.6/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.7/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.7/latch_postgres/__init__.py
+-rw-r--r--   0        0        0    24469 2023-05-17 01:55:18.986327 latch_postgres-0.1.7/latch_postgres/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.7/latch_postgres/py.typed
+-rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.7/latch_postgres/retries.py
+-rw-r--r--   0        0        0     1018 2023-05-17 01:55:35.995411 latch_postgres-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.7/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.7/PKG-INFO
```

### Comparing `latch_postgres-0.1.6/LICENSE` & `latch_postgres-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.6/latch_postgres/postgres.py` & `latch_postgres-0.1.7/latch_postgres/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Iterable,
     ParamSpec,
     TypeVar,
     cast,
 )
 
 import psycopg.sql as sql
-from latch_config.config import DatabaseConfig
+from latch_config.config import PostgresConnectionConfig
 from latch_data_validation.data_validation import JsonObject, validate
 from latch_o11y.o11y import dict_to_attrs, trace_function
 from opentelemetry.sdk.resources import Attributes
 from opentelemetry.trace import SpanKind, get_tracer
 from psycopg import AsyncConnection, AsyncCursor, IsolationLevel
 from psycopg.abc import AdaptContext, Params, Query
 from psycopg.conninfo import conninfo_to_dict, make_conninfo
@@ -63,14 +63,15 @@
 
 from latch_postgres.retries import CABackoff
 
 T = TypeVar("T")
 
 tracer = get_tracer(__name__)
 
+
 # todo(maximsmol): switch all the tracing attributes to otel spec
 # del span.type
 # in event names postgres -> postgresql (or to psycopg)?
 # out.host -> net.peer.name
 # out.port -> net.peer.port
 # sql.query -> db.statement
 # del resource.name
@@ -210,14 +211,19 @@
             return None
 
         if len(results) > 1:
             raise RuntimeError(f"received too many rows: '{len(results)}' > 1")
 
         return results[0]
 
+    async def query_void(
+        self, query: sql.SQL, **kwargs: Any
+    ) -> None:
+        await self.queryn(type(None), query, **kwargs)
+
 
 @dataclass(frozen=True)
 class EnumInfoQueryResponse:
     nspname: str
     name: str
     oid: int
     array_oid: int
@@ -479,15 +485,15 @@
         "type": type(x).__name__,
     }
 
 
 def with_conn_retry(
     f: Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]],
     pool: AsyncConnectionPool,
-    db_config: DatabaseConfig,
+    db_config: PostgresConnectionConfig,
 ) -> Callable[P, Awaitable[T]]:
     @functools.wraps(f)
     async def inner(*args: P.args, **kwargs: P.kwargs):
         with tracer.start_as_current_span("database session") as s:
             try:
                 retries = 0
                 accum_retry_time = 0
@@ -603,53 +609,55 @@
 
                 raise e
 
     return inner
 
 
 def get_with_conn_retry(
-    pool: AsyncConnectionPool, db_config: DatabaseConfig
+    pool: AsyncConnectionPool, db_config: PostgresConnectionConfig
 ) -> Callable[
     [Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]]],
     Callable[P, Awaitable[T]],
 ]:
     return functools.partial(with_conn_retry, pool=pool, db_config=db_config)
 
 
 def sqlq(x: str):
     return sql.SQL(dedent(x))
 
 
 # todo(maximsmol): conn resets appear in the startup span and make it last forever
 @trace_function(tracer)
-async def reset_conn(x: AsyncConnection[object]):
+async def reset_conn(x: AsyncConnection[object], read_only: bool = False):
     x.prepare_threshold = 0
 
-    if not x.read_only:
-        await x.set_read_only(True)
+    if x.read_only != read_only:
+        await x.set_read_only(read_only)
 
     if x.isolation_level != IsolationLevel.SERIALIZABLE:
         await x.set_isolation_level(IsolationLevel.SERIALIZABLE)
 
 
 # fixme(maximsmol): use autocommit transactions
 def get_pool(
-    config: DatabaseConfig, application_name: str
+    config: PostgresConnectionConfig,
+    application_name: str,
+    read_only: bool = True,
 ) -> TracedAsyncConnectionPool:
     conn_str = make_conninfo(
         host=config.host,
         port=config.port,
         dbname=config.dbname,
         user=config.user,
         password=config.password,
         application_name=application_name,
     )
     return TracedAsyncConnectionPool(
         conn_str,
         min_size=1,
         max_size=config.pool_size,
         timeout=timedelta(seconds=5) / timedelta(seconds=1),
-        open=False,  # tied into the server lifecycle instead
-        configure=reset_conn,
-        reset=reset_conn,
+        open=False,
+        configure=functools.partial(reset_conn, read_only=read_only),
+        reset=functools.partial(reset_conn, read_only=read_only),
         connection_class=LatchAsyncConnection,
     )
```

### Comparing `latch_postgres-0.1.6/latch_postgres/retries.py` & `latch_postgres-0.1.7/latch_postgres/retries.py`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.6/pyproject.toml` & `latch_postgres-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "latch-postgres"
-version = "0.1.6"
+version = "0.1.7"
 description = "Postges wrapper for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_postgres"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typing-extensions = "^4.4.0"
 psycopg = { extras = ["pool", "binary"], version = "^3.1.8" }
-latch-config = "^0.1.5"
+latch-config = "^0.1.6"
 latch-data-validation = "^0.1.3"
 latch-o11y = "^0.1.4"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
```

### Comparing `latch_postgres-0.1.6/setup.py` & `latch_postgres-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['latch_postgres']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['latch-config>=0.1.5,<0.2.0',
+['latch-config>=0.1.6,<0.2.0',
  'latch-data-validation>=0.1.3,<0.2.0',
  'latch-o11y>=0.1.4,<0.2.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'latch-postgres',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Postges wrapper for latch python backend services',
     'long_description': '# python-postgres\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_postgres-0.1.6/PKG-INFO` & `latch_postgres-0.1.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: latch-postgres
-Version: 0.1.6
+Version: 0.1.7
 Summary: Postges wrapper for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: latch-config (>=0.1.5,<0.2.0)
+Requires-Dist: latch-config (>=0.1.6,<0.2.0)
 Requires-Dist: latch-data-validation (>=0.1.3,<0.2.0)
 Requires-Dist: latch-o11y (>=0.1.4,<0.2.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.8,<4.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Description-Content-Type: text/markdown
```

