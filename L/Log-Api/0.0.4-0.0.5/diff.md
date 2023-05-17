# Comparing `tmp/Log_Api-0.0.4.tar.gz` & `tmp/Log_Api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Log_Api-0.0.4.tar", last modified: Wed May 17 17:23:59 2023, max compression
+gzip compressed data, was "Log_Api-0.0.5.tar", last modified: Wed May 17 21:01:45 2023, max compression
```

## Comparing `Log_Api-0.0.4.tar` & `Log_Api-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.714095 Log_Api-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.665373 Log_Api-0.0.4/Log_Api/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.700279 Log_Api-0.0.4/Log_Api/Class/
--rw-rw-rw-   0        0        0     2050 2023-05-16 21:33:41.000000 Log_Api-0.0.4/Log_Api/Class/Database.py
--rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Class/LogAPI.py
--rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Class/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Class/response..py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.703271 Log_Api-0.0.4/Log_Api/Models/
--rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Models/LogAPI.py
--rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.4/Log_Api/Models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.710104 Log_Api-0.0.4/Log_Api/Utils/
--rw-rw-rw-   0        0        0     7535 2023-05-15 21:16:39.000000 Log_Api-0.0.4/Log_Api/Utils/Aws.py
--rw-rw-rw-   0        0        0     3494 2023-05-15 20:49:03.000000 Log_Api-0.0.4/Log_Api/Utils/ModelsType.py
--rw-rw-rw-   0        0        0     4008 2023-05-15 19:54:00.000000 Log_Api-0.0.4/Log_Api/Utils/Response.py
--rw-rw-rw-   0        0        0     1181 2023-05-15 20:49:32.000000 Log_Api-0.0.4/Log_Api/Utils/Template.py
--rw-rw-rw-   0        0        0      117 2023-05-15 20:43:57.000000 Log_Api-0.0.4/Log_Api/Utils/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-15 20:44:12.000000 Log_Api-0.0.4/Log_Api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.694296 Log_Api-0.0.4/Log_Api.egg-info/
--rw-rw-rw-   0        0        0      284 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.4/Log_Api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-17 17:23:59.000000 Log_Api-0.0.4/Log_Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2023-05-17 17:23:59.713098 Log_Api-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.4/README.md
--rw-rw-rw-   0        0        0    14639 2023-05-17 17:23:50.000000 Log_Api-0.0.4/aws_handler_decorators.py
--rw-rw-rw-   0        0        0       42 2023-05-17 17:23:59.714095 Log_Api-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-05-17 17:23:19.000000 Log_Api-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:23:59.711101 Log_Api-0.0.4/test/
--rw-rw-rw-   0        0        0       29 2023-05-17 16:29:27.000000 Log_Api-0.0.4/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 21:01:45.023326 Log_Api-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.955503 Log_Api-0.0.5/Log_Api/
+drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.994403 Log_Api-0.0.5/Log_Api/Class/
+-rw-rw-rw-   0        0        0     2050 2023-05-16 21:33:41.000000 Log_Api-0.0.5/Log_Api/Class/Database.py
+-rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Class/LogAPI.py
+-rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Class/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Class/response..py
+drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.997394 Log_Api-0.0.5/Log_Api/Models/
+-rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Models/LogAPI.py
+-rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 21:01:45.020333 Log_Api-0.0.5/Log_Api/Utils/
+-rw-rw-rw-   0        0        0     7752 2023-05-17 21:00:18.000000 Log_Api-0.0.5/Log_Api/Utils/Aws.py
+-rw-rw-rw-   0        0        0     3494 2023-05-15 20:49:03.000000 Log_Api-0.0.5/Log_Api/Utils/ModelsType.py
+-rw-rw-rw-   0        0        0     4008 2023-05-15 19:54:00.000000 Log_Api-0.0.5/Log_Api/Utils/Response.py
+-rw-rw-rw-   0        0        0     1181 2023-05-15 20:49:32.000000 Log_Api-0.0.5/Log_Api/Utils/Template.py
+-rw-rw-rw-   0        0        0      117 2023-05-15 20:43:57.000000 Log_Api-0.0.5/Log_Api/Utils/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-15 20:44:12.000000 Log_Api-0.0.5/Log_Api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.986454 Log_Api-0.0.5/Log_Api.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.5/Log_Api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-05-17 21:01:45.022328 Log_Api-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.5/README.md
+-rw-rw-rw-   0        0        0    14763 2023-05-17 21:01:41.000000 Log_Api-0.0.5/aws_handler_decorators.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 21:01:45.023326 Log_Api-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-05-17 17:23:19.000000 Log_Api-0.0.5/setup.py
```

### Comparing `Log_Api-0.0.4/Log_Api/Class/Database.py` & `Log_Api-0.0.5/Log_Api/Class/Database.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/Log_Api/Class/LogAPI.py` & `Log_Api-0.0.5/Log_Api/Class/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/Log_Api/Class/response..py` & `Log_Api-0.0.5/Log_Api/Class/response..py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/Log_Api/Models/LogAPI.py` & `Log_Api-0.0.5/Log_Api/Models/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/Log_Api/Utils/Aws.py` & `Log_Api-0.0.5/Log_Api/Utils/Aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,26 +96,31 @@
             LogType='Tail',
             InvocationType=inv_type
         )
 
         return response
 
     @classmethod
-    def funciton_name(cls, function: str, service: str, stage=os.getenv('STAGE'), app=os.getenv('APP', '')):
+    def function_name(cls, function: str, service: str='', stage=os.getenv('STAGE'), ext_app=False):
         """
         Crea nombre de función lambda
         :param: function
             nombre de la función
         :param: stage
             nombre del stage
-        :param: app
-            nombre de la aplicación
+        :param: ext_app
+            si es una aplicación externa
         :return: function_name
         """
-        return f"{app}-{service}-{stage}-{function}"
+        if ext_app == False:
+            service = os.getenv('SERVICE', '')
+        
+        if service == '':
+            raise Exception("No se ha definido el nombre del servicio en la variable de entorno SERVICE")
+        return f"{service}-{stage}-{function}"
     
     def put_in_s3(self, file_name: str, file_path: str):
         """
         Subir archivo a S3
         :param: file_name
             nombre del archivo, debe tener esta estructura:
                 carpeta/nombre_archivo.extension
```

### Comparing `Log_Api-0.0.4/Log_Api/Utils/ModelsType.py` & `Log_Api-0.0.5/Log_Api/Utils/ModelsType.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/Log_Api/Utils/Response.py` & `Log_Api-0.0.5/Log_Api/Utils/Response.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/Log_Api/Utils/Template.py` & `Log_Api-0.0.5/Log_Api/Utils/Template.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/Log_Api.egg-info/SOURCES.txt` & `Log_Api-0.0.5/Log_Api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 Log_Api/Class/response..py
 Log_Api/Models/LogAPI.py
 Log_Api/Models/__init__.py
 Log_Api/Utils/Aws.py
 Log_Api/Utils/ModelsType.py
 Log_Api/Utils/Response.py
 Log_Api/Utils/Template.py
-Log_Api/Utils/__init__.py
-test/test_utils.py
+Log_Api/Utils/__init__.py
```

### Comparing `Log_Api-0.0.4/README.md` & `Log_Api-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.4/aws_handler_decorators.py` & `Log_Api-0.0.5/aws_handler_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     basestring
 except NameError:
     basestring = str
 
 logger = logging.getLogger(__name__)
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 class AwsHandlerDecorator(object):
     def __init__(self, func):
         update_wrapper(self, func)
         self.func = func
 
     def __call__(self, event, context):
@@ -257,15 +257,15 @@
             except Exception as exception:
                 return {"statusCode": 400, "body": str(exception)}
         elif isinstance(event.get("queryStringParameters"), dict) and event.get("body") in [None, {}]:
             event["body"] = event.get("queryStringParameters", {})
         return handler(event, context)
     return wrapper
 
-def json_schema_validator(request_schema=None, document=None, body=True):
+def json_schema_validator(request_schema=None, document=None, body=True, in_file=False):
     """
     Decorator to validate the request for a API Gateway event.
     Validate the request against the schema passed as `request_schema` parameter
     """
     def wrapper_wrapper(handler):
         @wraps(handler)
         def wrapper(event, context):
@@ -274,15 +274,17 @@
                     try:
                         with open(request_schema) as lfile:
                             schema_data = load(lfile)
                             if document is None:
                                 document_name = handler.__name__
                             else:
                                 document_name = document
-                            validate(request_data, schema_data[document_name])
+                            if in_file == False:
+                                schema_data = schema_data[document_name]
+                            validate(request_data, schema_data)
                     except ValidationError as ex:
                         error_path = ".".join(str(path) for path in ex.path)
                         error_message = f"Validation error at field '{error_path}': {ex.message}"
                         logging.error(error_message)
                         return {
                             "statusCode": 400,
                             "body": error_message
```

### Comparing `Log_Api-0.0.4/setup.py` & `Log_Api-0.0.5/setup.py`

 * *Files identical despite different names*

