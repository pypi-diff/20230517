# Comparing `tmp/upsolver_sdk_python-0.1.8.tar.gz` & `tmp/upsolver_sdk_python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsolver_sdk_python-0.1.8.tar", max compression
+gzip compressed data, was "upsolver_sdk_python-0.1.9.tar", max compression
```

## Comparing `upsolver_sdk_python-0.1.8.tar` & `upsolver_sdk_python-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     5071 2023-05-16 16:28:08.085060 upsolver_sdk_python-0.1.8/README.md
--rw-r--r--   0        0        0      651 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       97 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/__init__.py
--rw-r--r--   0        0        0      825 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/auth_filler.py
--rw-r--r--   0        0        0     3673 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/exceptions.py
--rw-r--r--   0        0        0     4428 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/poller.py
--rw-r--r--   0        0        0     1185 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/query.py
--rw-r--r--   0        0        0     4204 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/requester.py
--rw-r--r--   0        0        0     1108 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/response.py
--rw-r--r--   0        0        0      938 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/README.md
--rw-r--r--   0        0        0      131 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/__init__.py
--rw-r--r--   0        0        0     2222 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/connection.py
--rw-r--r--   0        0        0     7851 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/cursor.py
--rw-r--r--   0        0        0     2172 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/examples.py
--rw-r--r--   0        0        0     1423 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/type_constructors.py
--rw-r--r--   0        0        0     1609 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/types_definitions.py
--rw-r--r--   0        0        0     3463 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/utils.py
--rw-r--r--   0        0        0        0 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/sdk/__init__.py
--rw-r--r--   0        0        0     1309 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/sdk/client.py
--rw-r--r--   0        0        0      454 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/sdk/utils.py
--rw-r--r--   0        0        0     2557 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/utils.py
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 upsolver_sdk_python-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5071 2023-05-17 10:29:51.746295 upsolver_sdk_python-0.1.9/README.md
+-rw-r--r--   0        0        0      651 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/client/__init__.py
+-rw-r--r--   0        0        0      825 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/client/auth_filler.py
+-rw-r--r--   0        0        0     3673 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/client/exceptions.py
+-rw-r--r--   0        0        0     4437 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/client/poller.py
+-rw-r--r--   0        0        0     1185 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/client/query.py
+-rw-r--r--   0        0        0     4204 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/client/requester.py
+-rw-r--r--   0        0        0     1108 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/client/response.py
+-rw-r--r--   0        0        0      938 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/README.md
+-rw-r--r--   0        0        0      131 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/__init__.py
+-rw-r--r--   0        0        0     2222 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/connection.py
+-rw-r--r--   0        0        0     7851 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/cursor.py
+-rw-r--r--   0        0        0     2172 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/examples.py
+-rw-r--r--   0        0        0     1423 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/type_constructors.py
+-rw-r--r--   0        0        0     1609 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/types_definitions.py
+-rw-r--r--   0        0        0     3472 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/dbapi/utils.py
+-rw-r--r--   0        0        0        0 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/sdk/__init__.py
+-rw-r--r--   0        0        0     1309 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/sdk/client.py
+-rw-r--r--   0        0        0      454 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/sdk/utils.py
+-rw-r--r--   0        0        0     2557 2023-05-17 10:29:51.758295 upsolver_sdk_python-0.1.9/upsolver/utils.py
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 upsolver_sdk_python-0.1.9/PKG-INFO
```

### Comparing `upsolver_sdk_python-0.1.8/README.md` & `upsolver_sdk_python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/pyproject.toml` & `upsolver_sdk_python-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upsolver-sdk-python"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python SDK for Upsolver"
 authors = ["Upsolver Team <info@upsolver.com>"]
 
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "upsolver/__init__.py"},
```

### Comparing `upsolver_sdk_python-0.1.8/upsolver/client/auth_filler.py` & `upsolver_sdk_python-0.1.9/upsolver/client/auth_filler.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/client/exceptions.py` & `upsolver_sdk_python-0.1.9/upsolver/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/client/poller.py` & `upsolver_sdk_python-0.1.9/upsolver/client/poller.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             )
 
         if 'result' in rjson:
             result = rjson['result']
             if rjson['kind'] == 'upsolver_scalar_query_response':
                 scalar = result['scalar']
                 column_name = [scalar['valueType']]
-                data_w_columns: ExecutionResult = [dict(zip([column_name], [scalar]))]
+                data_w_columns: ExecutionResult = [dict(zip([column_name], [scalar['value']]))]
             else:
                 grid = result['grid']  # columns, data, ...
                 column_name = [c['name'] for c in grid['columns']]
                 data_w_columns: ExecutionResult = [dict(zip(column_name, row)) for row in grid['data']]
 
             return data_w_columns, result.get('next')
         else:
```

### Comparing `upsolver_sdk_python-0.1.8/upsolver/client/query.py` & `upsolver_sdk_python-0.1.9/upsolver/client/query.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/client/requester.py` & `upsolver_sdk_python-0.1.9/upsolver/client/requester.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/client/response.py` & `upsolver_sdk_python-0.1.9/upsolver/client/response.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/dbapi/README.md` & `upsolver_sdk_python-0.1.9/upsolver/dbapi/README.md`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/dbapi/connection.py` & `upsolver_sdk_python-0.1.9/upsolver/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/dbapi/cursor.py` & `upsolver_sdk_python-0.1.9/upsolver/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/dbapi/examples.py` & `upsolver_sdk_python-0.1.9/upsolver/dbapi/examples.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/dbapi/type_constructors.py` & `upsolver_sdk_python-0.1.9/upsolver/dbapi/type_constructors.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/dbapi/types_definitions.py` & `upsolver_sdk_python-0.1.9/upsolver/dbapi/types_definitions.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/dbapi/utils.py` & `upsolver_sdk_python-0.1.9/upsolver/dbapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,13 +82,13 @@
             )
 
         if 'result' in rjson:
             result = rjson['result']
             if rjson['kind'] == 'upsolver_scalar_query_response':
                 scalar = result['scalar']
                 columns = [{'name': scalar['valueType'], 'columnType': {'clazz': 'StringColumnType'}}]
-                return {'columns': columns, 'data': [scalar]}, result.get('next')
+                return {'columns': columns, 'data': [scalar['value']]}, result.get('next')
             else:
                 result['grid']['has_next_page'] = result.get('next') is not None
                 return result['grid'], result.get('next')
         else:
             return rjson, None
```

### Comparing `upsolver_sdk_python-0.1.8/upsolver/sdk/client.py` & `upsolver_sdk_python-0.1.9/upsolver/sdk/client.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/upsolver/utils.py` & `upsolver_sdk_python-0.1.9/upsolver/utils.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.8/PKG-INFO` & `upsolver_sdk_python-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsolver-sdk-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for Upsolver
 License: MIT
 Author: Upsolver Team
 Author-email: info@upsolver.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

