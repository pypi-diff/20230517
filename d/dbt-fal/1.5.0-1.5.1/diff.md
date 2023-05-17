# Comparing `tmp/dbt-fal-1.5.0.tar.gz` & `tmp/dbt_fal-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fal-1.5.0.tar", max compression
+gzip compressed data, was "dbt_fal-1.5.1.tar", max compression
```

## Comparing `dbt-fal-1.5.0.tar` & `dbt_fal-1.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     3009 2023-04-28 00:56:53.124588 dbt-fal-1.5.0/README.md
--rw-r--r--   0        0        0     1581 2023-04-28 00:57:00.832545 dbt-fal-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      303 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal/__init__.py
--rw-r--r--   0        0        0       18 2023-04-28 00:57:01.324544 dbt-fal-1.5.0/src/dbt/adapters/fal/__version__.py
--rw-r--r--   0        0        0      392 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal/connections.py
--rw-r--r--   0        0        0     3369 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal/impl.py
--rw-r--r--   0        0        0     2734 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal/load_db_profile.py
--rw-r--r--   0        0        0     4091 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal/wrappers.py
--rw-r--r--   0        0        0      344 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/__init__.py
--rw-r--r--   0        0        0       18 2023-04-28 00:57:01.324544 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/__version__.py
--rw-r--r--   0        0        0     4820 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/adapter.py
--rw-r--r--   0        0        0     8364 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/adapter_support.py
--rw-r--r--   0        0        0     1627 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/connections.py
--rw-r--r--   0        0        0     8714 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/impl.py
--rw-r--r--   0        0        0     3192 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/athena.py
--rw-r--r--   0        0        0     2686 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/bigquery.py
--rw-r--r--   0        0        0      980 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/duckdb.py
--rw-r--r--   0        0        0     2977 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/postgres.py
--rw-r--r--   0        0        0     2781 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/snowflake.py
--rw-r--r--   0        0        0      821 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/trino.py
--rw-r--r--   0        0        0       25 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/telemetry/__init__.py
--rw-r--r--   0        0        0    10763 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
--rw-r--r--   0        0        0     6572 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport.py
--rw-r--r--   0        0        0     1153 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
--rw-r--r--   0        0        0     4719 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
--rw-r--r--   0        0        0     2972 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
--rw-r--r--   0        0        0     1256 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/utils/__init__.py
--rw-r--r--   0        0        0     9804 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/utils/environments.py
--rw-r--r--   0        0        0     1970 2023-04-28 00:56:53.128588 dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
--rw-r--r--   0        0        0      208 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/fal/adapters/python/__init__.py
--rw-r--r--   0        0        0    11898 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/fal/adapters/python/connections.py
--rw-r--r--   0        0        0    10015 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/fal/adapters/python/impl.py
--rw-r--r--   0        0        0      181 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/fal/adapters/teleport/__init__.py
--rw-r--r--   0        0        0     3498 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/fal/adapters/teleport/impl.py
--rw-r--r--   0        0        0     2310 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/fal/adapters/teleport/info.py
--rw-r--r--   0        0        0       52 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal/__init__.py
--rw-r--r--   0        0        0       70 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal/dbt_project.yml
--rw-r--r--   0        0        0     1213 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal/macros/materializations/table.sql
--rw-r--r--   0        0        0      265 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal/macros/teleport_duckdb.sql
--rw-r--r--   0        0        0      921 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal/macros/teleport_snowflake.sql
--rw-r--r--   0        0        0       52 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal_experimental/__init__.py
--rw-r--r--   0        0        0       83 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal_experimental/dbt_project.yml
--rw-r--r--   0        0        0      989 2023-04-28 00:56:53.132588 dbt-fal-1.5.0/src/dbt/include/fal_experimental/macros/materializations/table.sql
--rw-r--r--   0        0        0     4844 2023-04-28 00:57:02.194341 dbt-fal-1.5.0/setup.py
--rw-r--r--   0        0        0     4577 2023-04-28 00:57:02.194809 dbt-fal-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3009 2023-05-17 17:25:16.234837 dbt_fal-1.5.1/README.md
+-rw-r--r--   0        0        0     1607 2023-05-17 17:25:27.635055 dbt_fal-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      639 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal/__init__.py
+-rw-r--r--   0        0        0       18 2023-05-17 17:25:28.131064 dbt_fal-1.5.1/src/dbt/adapters/fal/__version__.py
+-rw-r--r--   0        0        0      392 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal/connections.py
+-rw-r--r--   0        0        0     3369 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal/impl.py
+-rw-r--r--   0        0        0     2768 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal/load_db_profile.py
+-rw-r--r--   0        0        0     4091 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal/wrappers.py
+-rw-r--r--   0        0        0      344 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       18 2023-05-17 17:25:28.131064 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/__version__.py
+-rw-r--r--   0        0        0     4820 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/adapter.py
+-rw-r--r--   0        0        0     8381 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/adapter_support.py
+-rw-r--r--   0        0        0     1627 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/connections.py
+-rw-r--r--   0        0        0     8714 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/impl.py
+-rw-r--r--   0        0        0     3192 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/athena.py
+-rw-r--r--   0        0        0     2686 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/bigquery.py
+-rw-r--r--   0        0        0      980 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/duckdb.py
+-rw-r--r--   0        0        0     2977 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/postgres.py
+-rw-r--r--   0        0        0     1633 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/redshift.py
+-rw-r--r--   0        0        0     2781 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/snowflake.py
+-rw-r--r--   0        0        0      821 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/trino.py
+-rw-r--r--   0        0        0       25 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/telemetry/__init__.py
+-rw-r--r--   0        0        0    10763 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
+-rw-r--r--   0        0        0     6572 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport.py
+-rw-r--r--   0        0        0     1153 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
+-rw-r--r--   0        0        0     4719 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
+-rw-r--r--   0        0        0     2972 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
+-rw-r--r--   0        0        0     1256 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/utils/__init__.py
+-rw-r--r--   0        0        0     9804 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/utils/environments.py
+-rw-r--r--   0        0        0     1970 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
+-rw-r--r--   0        0        0      208 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/fal/adapters/python/__init__.py
+-rw-r--r--   0        0        0    11898 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/fal/adapters/python/connections.py
+-rw-r--r--   0        0        0    10015 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/fal/adapters/python/impl.py
+-rw-r--r--   0        0        0      181 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/fal/adapters/teleport/__init__.py
+-rw-r--r--   0        0        0     3498 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/fal/adapters/teleport/impl.py
+-rw-r--r--   0        0        0     2310 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/fal/adapters/teleport/info.py
+-rw-r--r--   0        0        0       52 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal/dbt_project.yml
+-rw-r--r--   0        0        0     1213 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal/macros/materializations/table.sql
+-rw-r--r--   0        0        0      265 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal/macros/teleport_duckdb.sql
+-rw-r--r--   0        0        0      921 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal/macros/teleport_snowflake.sql
+-rw-r--r--   0        0        0       52 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal_experimental/dbt_project.yml
+-rw-r--r--   0        0        0      989 2023-05-17 17:25:16.238837 dbt_fal-1.5.1/src/dbt/include/fal_experimental/macros/materializations/table.sql
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 dbt_fal-1.5.1/PKG-INFO
```

### Comparing `dbt-fal-1.5.0/README.md` & `dbt_fal-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/pyproject.toml` & `dbt_fal-1.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-fal"
-version = "1.5.0"
+version = "1.5.1"
 description = "Simplest way to run dbt python models."
 readme = "README.md"
 homepage = "https://github.com/fal-ai/fal/blob/-/projects/adapter"
 repository = "https://github.com/fal-ai/fal"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
     { include = "dbt", from = "src" }
@@ -29,15 +29,15 @@
 snowflake-connector-python = { version = "~=3.0", extras = ["pandas"], optional = true }
 
 ## bigquery
 ### version defined by dbt-bigquery, installs pyarrow<8
 google-cloud-bigquery = { version = "~3.5.0", extras = ["pandas"], optional = true }
 
 ## redshift
-sqlalchemy-redshift = { version = "^0.8.9", optional = true }
+awswrangler = { version = ">=3.0.0", extras = ["redshift"], optional = true, python = ">=3.8" }
 
 ## trino
 trino = { version = "~0.321.0", extras = ["sqlalchemy"], optional = true }
 
 # teleport
 s3fs = { version = ">=2022.8.2", optional = true }
 
@@ -50,15 +50,15 @@
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.extras]
 postgres = []
 snowflake = ["snowflake-connector-python"]
 bigquery = ["google-cloud-bigquery"]
-redshift = ["sqlalchemy-redshift"]
+redshift = ["awswrangler"]
 duckdb = []
 athena = []
 trino = ["trino"]
 teleport = ["s3fs"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal/impl.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal/load_db_profile.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal/load_db_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     return target_name
 
 
 def load_profiles_info_1_5() -> Tuple[Profile, Dict[str, Any]]:
     flags: Namespace = get_flags()
 
-    profile_renderer = ProfileRenderer(flags.VARS)
+    profile_renderer = ProfileRenderer(getattr(flags, "VARS", {}))
 
     profile_name = find_profile_name(flags.PROFILE, flags.PROJECT_DIR, profile_renderer)
 
     raw_profiles = read_profile(flags.PROFILES_DIR)
     raw_profile = raw_profiles[profile_name]
 
     target_name = find_target_name(flags.TARGET, raw_profile, profile_renderer)
@@ -70,11 +70,11 @@
         )
     except RecursionError as error:
         raise AttributeError(
             "Did you wrap a type 'fal' profile with another type 'fal' profile?"
         ) from error
 
     override_properties = {
-        "threads": flags.THREADS or fal_dict.get("threads") or db_profile.threads,
+        "threads": getattr(flags, "THREADS", None) or fal_dict.get("threads") or db_profile.threads,
     }
 
     return db_profile, override_properties
```

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal/wrappers.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal/wrappers.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/adapter.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/adapter_support.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/adapter_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from dbt.config import RuntimeConfig
 from dbt.parser.manifest import MacroManifest, Manifest
 from dbt.flags import Namespace
 
 from dbt.adapters import factory
 
 _SQLALCHEMY_DIALECTS = {
-    "redshift": "redshift+psycopg2",
     "sqlserver": "mssql+pyodbc",
 }
 
 
 def _get_alchemy_engine(adapter: BaseAdapter, connection: Connection) -> Any:
     # The following code heavily depends on the implementation
     # details of the known adapters, hence it can't work for
@@ -28,20 +27,14 @@
     format_url = lambda url: url
 
     if adapter_type == "trino":
         import dbt.adapters.fal_experimental.support.trino as support_trino
 
         return support_trino.create_engine(adapter)
 
-    if adapter_type == "redshift":
-        # If the given adapter supports the DBAPI (PEP 249), we can
-        # use its connection directly for the engine.
-        sqlalchemy_kwargs["creator"] = lambda *args, **kwargs: connection.handle
-        url = _SQLALCHEMY_DIALECTS.get(adapter_type, adapter_type) + "://"
-        url = format_url(url)
     elif adapter_type == "sqlserver":
         sqlalchemy_kwargs["creator"] = lambda *args, **kwargs: connection.handle
         url = _SQLALCHEMY_DIALECTS.get(adapter_type, adapter_type) + "://"
         url = format_url(url)
     else:
         message = (
             f"dbt-fal does not support {adapter_type} adapter. ",
@@ -96,14 +89,18 @@
         return support_postgres.write_df_to_relation(adapter, dataframe, relation)
     elif adapter.type() == "athena":
         import dbt.adapters.fal_experimental.support.athena as support_athena
 
         return support_athena.write_df_to_relation(
             adapter, dataframe, relation, if_exists
         )
+    elif adapter_type == "redshift":
+        import dbt.adapters.fal_experimental.support.redshift as support_redshift
+
+        return support_redshift.write_df_to_relation(adapter, dataframe, relation)
 
     else:
         with new_connection(adapter, "fal:write_df_to_relation") as connection:
             # TODO: this should probably live in the materialization macro.
             temp_relation = relation.replace_path(
                 identifier=f"__dbt_fal_temp_{relation.identifier}"
             )
@@ -156,14 +153,19 @@
         return support_postgres.read_relation_as_df(adapter, relation)
 
     elif adapter.type() == "athena":
         import dbt.adapters.fal_experimental.support.athena as support_athena
 
         return support_athena.read_relation_as_df(adapter, relation)
 
+    elif adapter.type() == "redshift":
+        import dbt.adapters.fal_experimental.support.redshift as support_redshift
+
+        return support_redshift.read_relation_as_df(adapter, relation)
+
     else:
         with new_connection(adapter, "fal:read_relation_as_df") as connection:
             alchemy_engine = _get_alchemy_engine(adapter, connection)
 
             return pd.read_sql_table(
                 con=alchemy_engine,
                 table_name=relation.identifier,
```

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/connections.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/impl.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/athena.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/athena.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/bigquery.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/bigquery.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/duckdb.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/postgres.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/snowflake.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/support/trino.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/support/trino.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/telemetry/telemetry.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport_adapter_support.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport_adapter_support.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/utils/__init__.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/utils/environments.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/utils/environments.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/adapters/fal_experimental/utils/yaml_helper.py` & `dbt_fal-1.5.1/src/dbt/adapters/fal_experimental/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/fal/adapters/python/connections.py` & `dbt_fal-1.5.1/src/dbt/fal/adapters/python/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/fal/adapters/python/impl.py` & `dbt_fal-1.5.1/src/dbt/fal/adapters/python/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/fal/adapters/teleport/impl.py` & `dbt_fal-1.5.1/src/dbt/fal/adapters/teleport/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/fal/adapters/teleport/info.py` & `dbt_fal-1.5.1/src/dbt/fal/adapters/teleport/info.py`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/include/fal/macros/materializations/table.sql` & `dbt_fal-1.5.1/src/dbt/include/fal/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/include/fal/macros/teleport_snowflake.sql` & `dbt_fal-1.5.1/src/dbt/include/fal/macros/teleport_snowflake.sql`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/src/dbt/include/fal_experimental/macros/materializations/table.sql` & `dbt_fal-1.5.1/src/dbt/include/fal_experimental/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-fal-1.5.0/PKG-INFO` & `dbt_fal-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: dbt-fal
-Version: 1.5.0
+Version: 1.5.1
 Summary: Simplest way to run dbt python models.
 Home-page: https://github.com/fal-ai/fal/blob/-/projects/adapter
 Keywords: dbt,pandas,fal,runtime
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7.2,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: athena
 Provides-Extra: bigquery
 Provides-Extra: duckdb
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: teleport
 Provides-Extra: trino
+Requires-Dist: awswrangler[redshift] (>=3.0.0) ; (python_version >= "3.8") and (extra == "redshift")
 Requires-Dist: backports.functools_lru_cache (>=1.6.4,<2.0.0)
 Requires-Dist: dbt-core (>=1.5.0,<1.6)
 Requires-Dist: dill (>=0.3.5.1)
 Requires-Dist: fal-serverless (>=0.6.28,<0.7.0)
-Requires-Dist: google-cloud-bigquery[pandas] (>=3.5.0,<3.6.0); extra == "bigquery"
+Requires-Dist: google-cloud-bigquery[pandas] (>=3.5.0,<3.6.0) ; extra == "bigquery"
 Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
 Requires-Dist: packaging (>=23)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: posthog (>=1.4.5,<2.0.0)
-Requires-Dist: s3fs (>=2022.8.2); extra == "teleport"
-Requires-Dist: snowflake-connector-python[pandas] (>=3.0,<4.0); extra == "snowflake"
+Requires-Dist: s3fs (>=2022.8.2) ; extra == "teleport"
+Requires-Dist: snowflake-connector-python[pandas] (>=3.0,<4.0) ; extra == "snowflake"
 Requires-Dist: sqlalchemy (>=1.4.41,<2.0.0)
-Requires-Dist: sqlalchemy-redshift (>=0.8.9,<0.9.0); extra == "redshift"
-Requires-Dist: trino[sqlalchemy] (>=0.321.0,<0.322.0); extra == "trino"
+Requires-Dist: trino[sqlalchemy] (>=0.321.0,<0.322.0) ; extra == "trino"
 Project-URL: Repository, https://github.com/fal-ai/fal
 Description-Content-Type: text/markdown
 
 <!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/adapter/" target="_blank" /> -->
 
 # Welcome to dbt-fal 👋
```

