# Comparing `tmp/pyathena-3.0.1.tar.gz` & `tmp/pyathena-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyathena-3.0.1.tar", max compression
+gzip compressed data, was "pyathena-3.0.2.tar", max compression
```

## Comparing `pyathena-3.0.1.tar` & `pyathena-3.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1055 2023-05-14 14:29:12.112188 pyathena-3.0.1/LICENSE
--rw-r--r--   0        0        0    70055 2023-05-14 14:29:12.116188 pyathena-3.0.1/README.rst
--rw-r--r--   0        0        0     1923 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/__init__.py
--rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     5157 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2554 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     7250 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9755 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2421 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/util.py
--rw-r--r--   0        0        0     5373 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/async_cursor.py
--rw-r--r--   0        0        0    21136 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/common.py
--rw-r--r--   0        0        0    10416 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/connection.py
--rw-r--r--   0        0        0     4209 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/converter.py
--rw-r--r--   0        0        0     5722 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/cursor.py
--rw-r--r--   0        0        0      660 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/error.py
--rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2439 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    20474 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0     1216 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0     6571 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/formatter.py
--rw-r--r--   0        0        0    17085 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/model.py
--rw-r--r--   0        0        0      220 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5829 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1830 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     8327 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13589 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0     9822 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/util.py
--rw-r--r--   0        0        0        0 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/py.typed
--rw-r--r--   0        0        0    24537 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/result_set.py
--rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      661 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    36892 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      884 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2638 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1210 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0     1948 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/util.py
--rw-r--r--   0        0        0     3482 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyproject.toml
--rw-r--r--   0        0        0    71494 1970-01-01 00:00:00.000000 pyathena-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-05-17 14:43:32.683209 pyathena-3.0.2/LICENSE
+-rw-r--r--   0        0        0    70055 2023-05-17 14:43:32.683209 pyathena-3.0.2/README.rst
+-rw-r--r--   0        0        0     1923 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     5157 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2554 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     7250 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9755 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2421 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/arrow/util.py
+-rw-r--r--   0        0        0     5373 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    21170 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/common.py
+-rw-r--r--   0        0        0    10416 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/connection.py
+-rw-r--r--   0        0        0     4209 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/converter.py
+-rw-r--r--   0        0        0     5835 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/cursor.py
+-rw-r--r--   0        0        0      660 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/error.py
+-rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2439 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    20474 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0     1216 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0     6571 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/formatter.py
+-rw-r--r--   0        0        0    17085 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/model.py
+-rw-r--r--   0        0        0      220 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5829 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1830 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     8327 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13589 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0     9822 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/pandas/util.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/py.typed
+-rw-r--r--   0        0        0    25104 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/result_set.py
+-rw-r--r--   0        0        0       24 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      661 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    36892 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      884 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2638 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1210 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0     1948 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyathena/util.py
+-rw-r--r--   0        0        0     3482 2023-05-17 14:43:32.687209 pyathena-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0    71494 1970-01-01 00:00:00.000000 pyathena-3.0.2/PKG-INFO
```

### Comparing `pyathena-3.0.1/LICENSE` & `pyathena-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/README.rst` & `pyathena-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/__init__.py` & `pyathena-3.0.2/pyathena/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, FrozenSet, Type
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
-__version__: str = "3.0.1"
+__version__: str = "3.0.2"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.0.1/pyathena/arrow/async_cursor.py` & `pyathena-3.0.2/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/arrow/converter.py` & `pyathena-3.0.2/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/arrow/cursor.py` & `pyathena-3.0.2/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/arrow/result_set.py` & `pyathena-3.0.2/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/arrow/util.py` & `pyathena-3.0.2/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/async_cursor.py` & `pyathena-3.0.2/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/common.py` & `pyathena-3.0.2/pyathena/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     # that Athena should consider for reuse. The default is 60.
     DEFAULT_RESULT_REUSE_MINUTES = 60
 
     def __init__(self, **kwargs) -> None:
         super(CursorIterator, self).__init__()
         self.arraysize: int = kwargs.get("arraysize", self.DEFAULT_FETCH_SIZE)
         self._rownumber: Optional[int] = None
+        self._rowcount: int = -1  # By default, return -1 to indicate that this is not supported.
 
     @property
     def arraysize(self) -> int:
         return self._arraysize
 
     @arraysize.setter
     def arraysize(self, value: int) -> None:
@@ -46,16 +47,15 @@
 
     @property
     def rownumber(self) -> Optional[int]:
         return self._rownumber
 
     @property
     def rowcount(self) -> int:
-        """By default, return -1 to indicate that this is not supported."""
-        return -1
+        return self._rowcount
 
     @abstractmethod
     def fetchone(self):
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def fetchmany(self):
```

### Comparing `pyathena-3.0.1/pyathena/connection.py` & `pyathena-3.0.2/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/converter.py` & `pyathena-3.0.2/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/cursor.py` & `pyathena-3.0.2/pyathena/cursor.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,18 @@
     def query_id(self, val) -> None:
         self._query_id = val
 
     @property
     def rownumber(self) -> Optional[int]:
         return self.result_set.rownumber if self.result_set else None
 
+    @property
+    def rowcount(self) -> int:
+        return self.result_set.rowcount if self.result_set else -1
+
     def close(self) -> None:
         if self.result_set and not self.result_set.is_closed:
             self.result_set.close()
 
     def execute(
         self,
         operation: str,
```

### Comparing `pyathena-3.0.1/pyathena/error.py` & `pyathena-3.0.2/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/fastparquet/util.py` & `pyathena-3.0.2/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/filesystem/s3.py` & `pyathena-3.0.2/pyathena/filesystem/s3.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/filesystem/s3_object.py` & `pyathena-3.0.2/pyathena/filesystem/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/formatter.py` & `pyathena-3.0.2/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/model.py` & `pyathena-3.0.2/pyathena/model.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/pandas/async_cursor.py` & `pyathena-3.0.2/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/pandas/converter.py` & `pyathena-3.0.2/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/pandas/cursor.py` & `pyathena-3.0.2/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/pandas/result_set.py` & `pyathena-3.0.2/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/pandas/util.py` & `pyathena-3.0.2/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/result_set.py` & `pyathena-3.0.2/pyathena/result_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,15 @@
             raise ProgrammingError("NextToken is none or empty.")
         response = self.__fetch(self._next_token)
         self._process_rows(response)
 
     def _pre_fetch(self) -> None:
         response = self.__fetch()
         self._process_metadata(response)
+        self._process_update_count(response)
         self._process_rows(response)
 
     def fetchone(
         self,
     ) -> Optional[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self._rows and self._next_token:
             self._fetch()
@@ -367,14 +368,30 @@
         if not metadata:
             raise DataError("KeyError `ResultSetMetadata`")
         column_info = metadata.get("ColumnInfo", None)
         if column_info is None:
             raise DataError("KeyError `ColumnInfo`")
         self._metadata = tuple(column_info)
 
+    def _process_update_count(self, response: Dict[str, Any]) -> None:
+        update_count = response.get("UpdateCount", None)
+        if (
+            update_count is not None
+            and self.substatement_type
+            and self.substatement_type.upper()
+            in (
+                "INSERT",
+                "UPDATE",
+                "DELETE",
+                "MERGE",
+                "CREATE_TABLE_AS_SELECT",
+            )
+        ):
+            self._rowcount = update_count
+
     def _get_rows(
         self, offset: int, metadata: Tuple[Any, ...], rows: List[Dict[str, Any]]
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         return [
             tuple(
                 [
                     self._converter.convert(meta.get("Type", None), row.get("VarCharValue", None))
@@ -451,14 +468,15 @@
     def close(self) -> None:
         self._connection = None
         self._query_execution = None
         self._metadata = None
         self._rows.clear()
         self._next_token = None
         self._rownumber = None
+        self._rowcount = -1
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
```

### Comparing `pyathena-3.0.1/pyathena/sqlalchemy/arrow.py` & `pyathena-3.0.2/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/sqlalchemy/base.py` & `pyathena-3.0.2/pyathena/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/sqlalchemy/pandas.py` & `pyathena-3.0.2/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/sqlalchemy/requirements.py` & `pyathena-3.0.2/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/sqlalchemy/types.py` & `pyathena-3.0.2/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyathena/util.py` & `pyathena-3.0.2/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.1/pyproject.toml` & `pyathena-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyAthena"
-version = "3.0.1"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
+version = "3.0.2"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
 description = "Python DB API 2.0 (PEP 249) client for Amazon Athena"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyathena-3.0.1/PKG-INFO` & `pyathena-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyathena
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Home-page: https://github.com/laughingman7743/PyAthena/
 License: MIT
 Author: laughingman7743
 Author-email: laughingman7743@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

