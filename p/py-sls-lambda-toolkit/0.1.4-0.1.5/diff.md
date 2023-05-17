# Comparing `tmp/py-sls-lambda-toolkit-0.1.4.tar.gz` & `tmp/py-sls-lambda-toolkit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sls-lambda-toolkit-0.1.4.tar", last modified: Wed May 17 02:13:26 2023, max compression
+gzip compressed data, was "py-sls-lambda-toolkit-0.1.5.tar", last modified: Wed May 17 03:23:11 2023, max compression
```

## Comparing `py-sls-lambda-toolkit-0.1.4.tar` & `py-sls-lambda-toolkit-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-17 02:13:26.186224 py-sls-lambda-toolkit-0.1.4/
--rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.1.4/LICENSE
--rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.1.4/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-17 02:13:26.186224 py-sls-lambda-toolkit-0.1.4/PKG-INFO
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-17 02:13:26.186224 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/
--rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/dynamodb_shortcuts.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/http_event.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1228 2023-05-17 02:11:54.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/http_response.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      604 2023-05-03 19:42:23.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/jwt.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/logger.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      646 2023-04-28 06:49:01.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/mappers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/parsers.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      584 2023-05-03 16:03:44.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/password.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     3086 2023-04-23 20:42:46.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/scan_filter_builder.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/status_code.py
--rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/validators.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-17 02:13:26.186224 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-17 02:13:25.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      700 2023-05-17 02:13:26.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-05-17 02:13:26.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       71 2023-05-17 02:13:26.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-05-17 02:13:26.000000 py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.1.4/pyproject.toml
--rw-rw-r--   0 julio     (1000) julio     (1000)      966 2023-05-17 02:13:26.186224 py-sls-lambda-toolkit-0.1.4/setup.cfg
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-17 03:23:11.855736 py-sls-lambda-toolkit-0.1.5/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1069 2023-04-23 17:34:15.000000 py-sls-lambda-toolkit-0.1.5/LICENSE
+-rw-rw-r--   0 julio     (1000) julio     (1000)       34 2023-04-23 18:05:48.000000 py-sls-lambda-toolkit-0.1.5/MANIFEST.in
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-17 03:23:11.855736 py-sls-lambda-toolkit-0.1.5/PKG-INFO
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-17 03:23:11.855736 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/
+-rw-rw-r--   0 julio     (1000) julio     (1000)        0 2023-04-23 17:11:35.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/__init__.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1370 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/dynamodb_shortcuts.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1651 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/http_event.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1369 2023-05-17 03:22:25.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/http_response.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      604 2023-05-03 19:42:23.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/jwt.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      112 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/logger.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      646 2023-04-28 06:49:01.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/mappers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      757 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/parsers.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      584 2023-05-03 16:03:44.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/password.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3086 2023-04-23 20:42:46.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/scan_filter_builder.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1255 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/status_code.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)      863 2023-04-23 17:11:56.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/validators.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-05-17 03:23:11.855736 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/
+-rw-rw-r--   0 julio     (1000) julio     (1000)      762 2023-05-17 03:23:11.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)      700 2023-05-17 03:23:11.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-05-17 03:23:11.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       71 2023-05-17 03:23:11.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       22 2023-05-17 03:23:11.000000 py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       94 2023-04-23 17:31:48.000000 py-sls-lambda-toolkit-0.1.5/pyproject.toml
+-rw-rw-r--   0 julio     (1000) julio     (1000)      966 2023-05-17 03:23:11.855736 py-sls-lambda-toolkit-0.1.5/setup.cfg
```

### Comparing `py-sls-lambda-toolkit-0.1.4/LICENSE` & `py-sls-lambda-toolkit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/PKG-INFO` & `py-sls-lambda-toolkit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/dynamodb_shortcuts.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/dynamodb_shortcuts.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/http_event.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/http_event.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/http_response.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/http_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import json
+import numbers
 from .parsers import SnakeToCamelConverter
 
+def default(obj):
+    if isinstance(obj, numbers.Number):
+        return str(obj)
+    return json.JSONEncoder.default(obj)
 
 def create_response(response, status_code=200, headers=None, content_type='application/json'):
     """
         Creates an HTTP response object.
 
         Parameters:
             response (dict): The response body.
@@ -20,14 +25,14 @@
         'Access-Control-Allow-Origin': '*',
         'Access-Control-Allow-Credentials': True,
         'Content-Type': content_type,
         'Access-Control-Allow-Methods': 'GET, POST, OPTIONS, PUT, PATCH, DELETE',
         'Access-Control-Allow-Headers': 'Origin, X-Requested-With, Content-Type, Accept, X-API-AUTH, X-Amz-Date, X-Api-Key, X-Amz-Security-Token, X-Amz-User-Agent',
     }
 
-    # body = SnakeToCamelConverter.convert(response)
+    body = SnakeToCamelConverter.convert(response)
 
     return {
         'statusCode': status_code,
         'headers': headers,
-        'body': json.dumps(response)
+        'body': json.dumps(body, default)
     }
```

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/jwt.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/jwt.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/mappers.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/mappers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/parsers.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/parsers.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/password.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/password.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/scan_filter_builder.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/scan_filter_builder.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/status_code.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/status_code.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit/validators.py` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/PKG-INFO` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sls-lambda-toolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-sls-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit
 Classifier: Development Status :: 1 - Planning
```

### Comparing `py-sls-lambda-toolkit-0.1.4/py_sls_lambda_toolkit.egg-info/SOURCES.txt` & `py-sls-lambda-toolkit-0.1.5/py_sls_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-sls-lambda-toolkit-0.1.4/setup.cfg` & `py-sls-lambda-toolkit-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-sls-lambda-toolkit
-version = 0.1.4
+version = 0.1.5
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0riion/py-sls-lambda-toolkit
```

