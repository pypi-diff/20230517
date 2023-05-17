# Comparing `tmp/Log_Api-0.0.3.tar.gz` & `tmp/Log_Api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Log_Api-0.0.3.tar", last modified: Mon May 15 20:09:32 2023, max compression
+gzip compressed data, was "Log_Api-0.0.4.tar", last modified: Wed May 17 17:23:59 2023, max compression
```

## Comparing `Log_Api-0.0.3.tar` & `Log_Api-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:09:32.784393 Log_Api-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-15 20:09:32.730027 Log_Api-0.0.3/Log_Api/
-drwxrwxrwx   0        0        0        0 2023-05-15 20:09:32.773424 Log_Api-0.0.3/Log_Api/Class/
--rw-rw-rw-   0        0        0     2068 2023-05-15 16:56:09.000000 Log_Api-0.0.3/Log_Api/Class/Database.py
--rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.3/Log_Api/Class/LogAPI.py
--rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.3/Log_Api/Class/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.3/Log_Api/Class/response..py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:09:32.776414 Log_Api-0.0.3/Log_Api/Models/
--rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.3/Log_Api/Models/LogAPI.py
--rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.3/Log_Api/Models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:09:32.782398 Log_Api-0.0.3/Log_Api/Utils/
--rw-rw-rw-   0        0        0     7535 2023-05-15 19:52:53.000000 Log_Api-0.0.3/Log_Api/Utils/Aws.py
--rw-rw-rw-   0        0        0     3492 2023-05-15 18:44:49.000000 Log_Api-0.0.3/Log_Api/Utils/ModelsType.py
--rw-rw-rw-   0        0        0     4008 2023-05-15 19:54:00.000000 Log_Api-0.0.3/Log_Api/Utils/Response.py
--rw-rw-rw-   0        0        0     1183 2023-05-15 19:59:43.000000 Log_Api-0.0.3/Log_Api/Utils/Template.py
--rw-rw-rw-   0        0        0       47 2023-05-15 16:56:09.000000 Log_Api-0.0.3/Log_Api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:09:32.765443 Log_Api-0.0.3/Log_Api.egg-info/
--rw-rw-rw-   0        0        0      284 2023-05-15 20:09:32.000000 Log_Api-0.0.3/Log_Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-15 20:09:32.000000 Log_Api-0.0.3/Log_Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:09:32.000000 Log_Api-0.0.3/Log_Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.3/Log_Api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2023-05-15 20:09:32.000000 Log_Api-0.0.3/Log_Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-15 20:09:32.000000 Log_Api-0.0.3/Log_Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2023-05-15 20:09:32.783396 Log_Api-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.3/README.md
--rw-rw-rw-   0        0        0    14467 2023-05-15 20:09:20.000000 Log_Api-0.0.3/aws_handler_decorators.py
--rw-rw-rw-   0        0        0       42 2023-05-15 20:09:32.784393 Log_Api-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-05-15 19:52:55.000000 Log_Api-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.714095 Log_Api-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.665373 Log_Api-0.0.4/Log_Api/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.700279 Log_Api-0.0.4/Log_Api/Class/
+-rw-rw-rw-   0        0        0     2050 2023-05-16 21:33:41.000000 Log_Api-0.0.4/Log_Api/Class/Database.py
+-rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Class/LogAPI.py
+-rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Class/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Class/response..py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.703271 Log_Api-0.0.4/Log_Api/Models/
+-rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Models/LogAPI.py
+-rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.710104 Log_Api-0.0.4/Log_Api/Utils/
+-rw-rw-rw-   0        0        0     7535 2023-05-15 21:16:39.000000 Log_Api-0.0.4/Log_Api/Utils/Aws.py
+-rw-rw-rw-   0        0        0     3494 2023-05-15 20:49:03.000000 Log_Api-0.0.4/Log_Api/Utils/ModelsType.py
+-rw-rw-rw-   0        0        0     4008 2023-05-15 19:54:00.000000 Log_Api-0.0.4/Log_Api/Utils/Response.py
+-rw-rw-rw-   0        0        0     1181 2023-05-15 20:49:32.000000 Log_Api-0.0.4/Log_Api/Utils/Template.py
+-rw-rw-rw-   0        0        0      117 2023-05-15 20:43:57.000000 Log_Api-0.0.4/Log_Api/Utils/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-15 20:44:12.000000 Log_Api-0.0.4/Log_Api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.694296 Log_Api-0.0.4/Log_Api.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.4/Log_Api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-05-17 17:23:59.713098 Log_Api-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.4/README.md
+-rw-rw-rw-   0        0        0    14639 2023-05-17 17:23:50.000000 Log_Api-0.0.4/aws_handler_decorators.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:23:59.714095 Log_Api-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-05-17 17:23:19.000000 Log_Api-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.711101 Log_Api-0.0.4/test/
+-rw-rw-rw-   0        0        0       29 2023-05-17 16:29:27.000000 Log_Api-0.0.4/test/test_utils.py
```

### Comparing `Log_Api-0.0.3/Log_Api/Class/Database.py` & `Log_Api-0.0.4/Log_Api/Class/Database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
+import os
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.pool import QueuePool, NullPool
-# from utils.Secrets import Secretos
-from Utils.Aws import Aws
-import json
+
+from ..Utils import Aws
 
 #Excepciones
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm.exc import FlushError
 
 base_class = declarative_base()  # Extend class for models
 
-
 class Database():
-
+    
     # Mode can be:
     # dbr: Mode Read
     # dbw: Mode Write
     def __init__(self, mode):
         if mode is None or (mode != "dbw" and mode != "dbr"):
             raise Warning("El modo de uso de base de datos no es válido.")
 
         try:
-            connection_data = Aws.get_secret(f'{mode}-fcc')
+            connection_data = Aws(f'{mode}{os.getenv("APP", "")}').get_secret()
 
             # Get connections strings from secret manager
             __connection_strings = self.__get_connection_strings(
                 connection_data)
 
             # Create a engine DB
             self.__engine = create_engine(
```

### Comparing `Log_Api-0.0.3/Log_Api/Class/LogAPI.py` & `Log_Api-0.0.4/Log_Api/Class/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.3/Log_Api/Class/response..py` & `Log_Api-0.0.4/Log_Api/Class/response..py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.3/Log_Api/Models/LogAPI.py` & `Log_Api-0.0.4/Log_Api/Models/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.3/Log_Api/Utils/Aws.py` & `Log_Api-0.0.4/Log_Api/Utils/Aws.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.3/Log_Api/Utils/ModelsType.py` & `Log_Api-0.0.4/Log_Api/Utils/ModelsType.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from sqlalchemy import Column, Integer, String, sql
-from Class.Database import declarative_base as BASE
+from ..Class.Database import declarative_base as BASE
 
 class Model:
     """
     Clase para generar los modelos de la base de datos de tipo detalle
     """
     @classmethod
     def create(cls, table_name):
```

### Comparing `Log_Api-0.0.3/Log_Api/Utils/Response.py` & `Log_Api-0.0.4/Log_Api/Utils/Response.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.3/Log_Api/Utils/Template.py` & `Log_Api-0.0.4/Log_Api/Utils/Template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Utils.Aws import Aws
+from ..Utils import Aws
 
 class Template:
     
     def __init__(self, template_name, bucket_secret_name: str):
         __s3 = Aws(bucket_secret_name).get_secret()
         self.template_name = template_name
         self.template_path = f"Templates/{self.template_name}"
```

### Comparing `Log_Api-0.0.3/README.md` & `Log_Api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.3/aws_handler_decorators.py` & `Log_Api-0.0.4/aws_handler_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     basestring
 except NameError:
     basestring = str
 
 logger = logging.getLogger(__name__)
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 class AwsHandlerDecorator(object):
     def __init__(self, func):
         update_wrapper(self, func)
         self.func = func
 
     def __call__(self, event, context):
@@ -252,14 +252,16 @@
         if isinstance(event.get("queryStringParameters"), str):
             try:
                 event["queryStringParameters"] = ast.literal_eval(event["queryStringParameters"])
                 if isObject(event["queryStringParameters"]):
                     event["queryStringParameters"] = evaluate_items(event["queryStringParameters"])
             except Exception as exception:
                 return {"statusCode": 400, "body": str(exception)}
+        elif isinstance(event.get("queryStringParameters"), dict) and event.get("body") in [None, {}]:
+            event["body"] = event.get("queryStringParameters", {})
         return handler(event, context)
     return wrapper
 
 def json_schema_validator(request_schema=None, document=None, body=True):
     """
     Decorator to validate the request for a API Gateway event.
     Validate the request against the schema passed as `request_schema` parameter
```

### Comparing `Log_Api-0.0.3/setup.py` & `Log_Api-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from setuptools import setup
-# import sys
-# sys.path.append('Log_Api')
-# from Log_Api.Class.LogAPI import log_resquest_response
 import aws_handler_decorators
-# from Log_Api.Class.LogAPI import log_resquest_response
 
 setup(name='Log_Api',
       version=aws_handler_decorators.__version__,
       description='Paquete para el manejo de logs de apis aws lambda serverles con sqlalchemy',
       url='https://github.com/1kagro/serverless-sqlalchemy-logapi',
       author='Fabian Lozano',
       author_email='fabianlozano044@gmail.com',
```

