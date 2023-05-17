# Comparing `tmp/duckdb_engine-0.7.1.tar.gz` & `tmp/duckdb_engine-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdb_engine-0.7.1.tar", max compression
+gzip compressed data, was "duckdb_engine-0.7.2.tar", max compression
```

## Comparing `duckdb_engine-0.7.1.tar` & `duckdb_engine-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-05-09 16:12:04.584668 duckdb_engine-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     5953 2023-05-09 16:12:04.584668 duckdb_engine-0.7.1/README.md
--rw-r--r--   0        0        0        4 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
--rw-r--r--   0        0        0        1 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
--rw-r--r--   0        0        0    20688 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
--rw-r--r--   0        0        0    11514 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/__init__.py
--rw-r--r--   0        0        0      985 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/config.py
--rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/conftest.py
--rw-r--r--   0        0        0     1707 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/datatypes.py
--rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/py.typed
--rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      338 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/snapshots/snap_test_basic.py
--rw-r--r--   0        0        0    10426 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_basic.py
--rw-r--r--   0        0        0     2351 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_datatypes.py
--rw-r--r--   0        0        0      948 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_ibis.py
--rw-r--r--   0        0        0      455 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_integration.py
--rw-r--r--   0        0        0     3946 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_pandas.py
--rw-r--r--   0        0        0      257 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/util.py
--rw-r--r--   0        0        0     1370 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     5953 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/README.md
+-rw-r--r--   0        0        0        4 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
+-rw-r--r--   0        0        0        1 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
+-rw-r--r--   0        0        0    20688 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
+-rw-r--r--   0        0        0    11629 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/config.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/conftest.py
+-rw-r--r--   0        0        0     2291 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/datatypes.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/py.typed
+-rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/snapshots/snap_test_basic.py
+-rw-r--r--   0        0        0    10426 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_basic.py
+-rw-r--r--   0        0        0     3015 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_datatypes.py
+-rw-r--r--   0        0        0      948 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_ibis.py
+-rw-r--r--   0        0        0      455 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_integration.py
+-rw-r--r--   0        0        0     3946 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_pandas.py
+-rw-r--r--   0        0        0      257 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/util.py
+-rw-r--r--   0        0        0     1370 2023-05-17 10:30:48.307976 duckdb_engine-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.7.2/PKG-INFO
```

### Comparing `duckdb_engine-0.7.1/LICENSE.txt` & `duckdb_engine-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/README.md` & `duckdb_engine-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz` & `duckdb_engine-0.7.2/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/duckdb_engine/__init__.py` & `duckdb_engine-0.7.2/duckdb_engine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.dialects.postgresql.base import PGDialect, PGInspector
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.url import URL
 
 from .config import apply_config, get_core_config
-from .datatypes import register_extension_types
+from .datatypes import ISCHEMA_NAMES, register_extension_types
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 if TYPE_CHECKING:
     from sqlalchemy.base import Connection
     from sqlalchemy.engine.interfaces import _IndexDict
 
 
 register_extension_types()
@@ -180,14 +180,18 @@
             # postgres type_codes (such as 701 for float) that duckdb doesn't have
             sqltypes.Numeric: sqltypes.Numeric,
             sqltypes.Interval: sqltypes.Interval,
             sqltypes.JSON: sqltypes.JSON,
             UUID: UUID,
         },
     )
+    ischema_names = util.update_copy(
+        PGDialect.ischema_names,
+        ISCHEMA_NAMES,
+    )
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["use_native_hstore"] = False
         super().__init__(*args, **kwargs)
 
     def connect(self, *cargs: Any, **cparams: Any) -> "Connection":
         core_keys = get_core_config()
```

### Comparing `duckdb_engine-0.7.1/duckdb_engine/config.py` & `duckdb_engine-0.7.2/duckdb_engine/config.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/duckdb_engine/datatypes.py` & `duckdb_engine-0.7.2/duckdb_engine/datatypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 ```
 """
 
 from typing import Any
 
 from sqlalchemy.dialects.postgresql.base import PGTypeCompiler
 from sqlalchemy.ext.compiler import compiles
+from sqlalchemy.sql import sqltypes
+from sqlalchemy.sql.type_api import TypeEngine
 from sqlalchemy.types import BigInteger, Integer, SmallInteger
 
 # INTEGER	INT4, INT, SIGNED	-2147483648	2147483647
 # SMALLINT	INT2, SHORT	-32768	32767
 # BIGINT	INT8, LONG	-9223372036854775808	9223372036854775807
 (BigInteger, SmallInteger)  # pure reexport
 
@@ -79,10 +81,35 @@
     subclass
     for subclass in Integer.__subclasses__()
     if subclass.__module__ == UInt64.__module__
 ]
 assert types
 
 
+class Struct(TypeEngine):
+    pass
+
+
+class Map(TypeEngine):
+    pass
+
+
+ISCHEMA_NAMES = {
+    "hugeint": HugeInteger,
+    "tinyint": TinyInteger,
+    "utinyint": UTinyInteger,
+    "usmallint": USmallInteger,
+    "uinteger": UInt8,
+    "ubigint": UBigInteger,
+    "timestamp_s": sqltypes.TIMESTAMP,
+    "timestamp_ms": sqltypes.TIMESTAMP,
+    "timestamp_ns": sqltypes.TIMESTAMP,
+    "enum": sqltypes.Enum,
+    "list": lambda: sqltypes.ARRAY(sqltypes.NULLTYPE),
+    "struct": Struct,
+    "map": Map,
+}
+
+
 def register_extension_types() -> None:
     for subclass in types:
         compiles(subclass, "duckdb")(compile_uint)
```

### Comparing `duckdb_engine-0.7.1/duckdb_engine/tests/conftest.py` & `duckdb_engine-0.7.2/duckdb_engine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/duckdb_engine/tests/test_basic.py` & `duckdb_engine-0.7.2/duckdb_engine/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/duckdb_engine/tests/test_datatypes.py` & `duckdb_engine-0.7.2/duckdb_engine/tests/test_datatypes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import warnings
 from typing import Type
 from uuid import uuid4
 
+import duckdb
 from pytest import importorskip, mark
 from sqlalchemy import Column, Integer, MetaData, Table, inspect, text
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session
+from sqlalchemy.sql import sqltypes
 from sqlalchemy.types import JSON
 
 from ..datatypes import types
 
 
 @mark.parametrize("coltype", types)
 def test_unsigned_integer_type(
@@ -89,7 +92,21 @@
 
     md = MetaData()
 
     t = Table("t", md, autoload_with=engine)
 
     with engine.begin() as con:
         con.execute(t.select())
+
+
+def test_all_types_reflection(engine: Engine) -> None:
+    importorskip("sqlalchemy", "1.4.0")
+    importorskip("duckdb", "0.5.1")
+
+    with warnings.catch_warnings() as capture, engine.connect() as conn:
+        conn.execute(text("create table t2 as select * from test_all_types()"))
+        table = Table("t2", MetaData(), autoload_with=conn)
+        for col in table.columns:
+            if col.name.endswith("_enum") and duckdb.__version__ < "0.7.1":  # type: ignore[attr-defined]
+                continue
+            assert col.type != sqltypes.NULLTYPE, col.name
+        assert not capture
```

### Comparing `duckdb_engine-0.7.1/duckdb_engine/tests/test_ibis.py` & `duckdb_engine-0.7.2/duckdb_engine/tests/test_ibis.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/duckdb_engine/tests/test_pandas.py` & `duckdb_engine-0.7.2/duckdb_engine/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.1/pyproject.toml` & `duckdb_engine-0.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duckdb_engine"
-version = "0.7.1"
+version = "0.7.2"
 description = "SQLAlchemy driver for duckdb"
 authors = ["Elliana <me@mause.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Mause/duckdb_engine"
 
 [tool.poetry.urls]
@@ -17,15 +17,15 @@
 sqlalchemy = ">=1.3.22"
 numpy = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pre-commit = "^2.21.0"
 pdbpp = "^0.10.3"
-mypy = "^1.1"
+mypy = "^1.3"
 hypothesis = "^6.75.2"
 pandas = "^1"
 jupysql = "^0.7.4"
 sqlalchemy = {version="^1.3.19", extras=['mypy']}
 pytest-cov = {extras = ["coverage"], version = "^4.0.0"}
 snapshottest = "^0.6.0"
```

### Comparing `duckdb_engine-0.7.1/PKG-INFO` & `duckdb_engine-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb-engine
-Version: 0.7.1
+Version: 0.7.2
 Summary: SQLAlchemy driver for duckdb
 Home-page: https://github.com/Mause/duckdb_engine
 License: MIT
 Author: Elliana
 Author-email: me@mause.me
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

