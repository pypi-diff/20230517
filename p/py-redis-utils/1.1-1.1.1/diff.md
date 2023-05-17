# Comparing `tmp/py-redis-utils-1.1.tar.gz` & `tmp/py-redis-utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-1.1.tar", last modified: Wed May 17 10:33:45 2023, max compression
+gzip compressed data, was "py-redis-utils-1.1.1.tar", last modified: Wed May 17 10:57:17 2023, max compression
```

## Comparing `py-redis-utils-1.1.tar` & `py-redis-utils-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:33:45.370864 py-redis-utils-1.1/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-05-17 10:33:45.370864 py-redis-utils-1.1/PKG-INFO
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.1/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:33:45.370864 py-redis-utils-1.1/py_redis_utils.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      286 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       63 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       13 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:33:45.370864 py-redis-utils-1.1/pyredisutils/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       65 2023-05-17 09:03:25.000000 py-redis-utils-1.1/pyredisutils/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     8167 2023-05-17 10:33:37.000000 py-redis-utils-1.1/pyredisutils/_decorators.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)    14305 2023-05-17 09:03:25.000000 py-redis-utils-1.1/pyredisutils/_settings.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-05-17 10:33:45.370864 py-redis-utils-1.1/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      784 2023-05-17 10:33:37.000000 py-redis-utils-1.1/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:57:17.800864 py-redis-utils-1.1.1/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      416 2023-05-17 10:57:17.800864 py-redis-utils-1.1.1/PKG-INFO
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.1.1/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:57:17.800864 py-redis-utils-1.1.1/py_redis_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      416 2023-05-17 10:57:17.000000 py-redis-utils-1.1.1/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      286 2023-05-17 10:57:17.000000 py-redis-utils-1.1.1/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-05-17 10:57:17.000000 py-redis-utils-1.1.1/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       63 2023-05-17 10:57:17.000000 py-redis-utils-1.1.1/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       13 2023-05-17 10:57:17.000000 py-redis-utils-1.1.1/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:57:17.800864 py-redis-utils-1.1.1/pyredisutils/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       65 2023-05-17 09:03:25.000000 py-redis-utils-1.1.1/pyredisutils/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     8535 2023-05-17 10:56:48.000000 py-redis-utils-1.1.1/pyredisutils/_decorators.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)    14363 2023-05-17 10:56:48.000000 py-redis-utils-1.1.1/pyredisutils/_settings.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-05-17 10:57:17.800864 py-redis-utils-1.1.1/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      786 2023-05-17 10:57:15.000000 py-redis-utils-1.1.1/setup.py
```

### Comparing `py-redis-utils-1.1/README.md` & `py-redis-utils-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.1/pyredisutils/_decorators.py` & `py-redis-utils-1.1.1/pyredisutils/_decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import logging
 from functools import wraps
 from typing import List, Tuple, Any
 
 import redis
 
 from pyredisutils._settings import Settings
@@ -36,34 +37,39 @@
     "SECOND", as well as will look for value "ABC" and will change it to the "QWE". In that way, your list should contain lists with two parameters, where first
     is the old value that should be changed, and the second is the value to which it will be changed.
     :return: Returns nothing if Redis returned Successful message, and will return Flask Response *Any | Tuple[Any, int]* if Any error occurred.
     """
     def funct_decorator(org_function):
         @wraps(org_function)
         def authorize(*args, **kwargs):
+
             settings = Settings(
                 redis_instance,
                 channel_name,
-                publish_template,
-                response_template,
-                publish_changes,
-                response_changes,
+                copy.deepcopy(publish_template),
+                copy.deepcopy(response_template),
+                copy.deepcopy(publish_changes),
+                copy.deepcopy(response_changes),
             )
-            print(settings)
+
             # Applies all necessary settings
             settings.get_token()
             settings.generate_id()
             settings.update_publish_replaces()
             settings.update_response_replaces()
             settings.transform_publish_template()
             settings.transform_response_template()
 
             # Publishes message to Redis
             if settings.publish_message_to_redis():
+                settings.publish_template = None
+                settings.response_template = None
                 return org_function(*args, **kwargs)
+            settings.publish_template = None
+            settings.response_template = None
             logging.info("Redis response - Token is not valid")
             return settings.make_response("Unauthorized", 401)
 
         return authorize
 
     return funct_decorator
 
@@ -94,26 +100,27 @@
     is the old value that should be changed, and the second is the value to which it will be changed.
     :param response_changes: Field that contains custom replaceable values for response message. It should be List of Lists *List[List]*.
     For example, you should pass this kind of list -  [["FIRST", "SECOND"], ["ABC", "QWE"]], and the decorator will look for value "FIRST" and change it to the
     "SECOND", as well as will look for value "ABC" and will change it to the "QWE". In that way, your list should contain lists with two parameters, where first
     is the old value that should be changed, and the second is the value to which it will be changed.
     :return: Returns nothing if Redis returned Successful message, and will return Flask Response *Any | Tuple[Any, int]* if Any error occurred.
     """
-    settings = Settings(
-        redis_instance,
-        channel_name,
-        publish_template,
-        response_template,
-        publish_changes,
-        response_changes,
-    )
-
     def wrapper(org_function):
         @wraps(org_function)
         def check(*args, **kwargs):
+
+            settings = Settings(
+                redis_instance,
+                channel_name,
+                copy.deepcopy(publish_template),
+                copy.deepcopy(response_template),
+                copy.deepcopy(publish_changes),
+                copy.deepcopy(response_changes),
+            )
+
             # Applies all necessary settings
             settings.get_token()
             settings.get_user_id_from_token()
             settings.get_roles_from_token()
             settings.generate_id()
             settings.update_publish_replaces()
             settings.update_response_replaces()
```

### Comparing `py-redis-utils-1.1/pyredisutils/_settings.py` & `py-redis-utils-1.1.1/pyredisutils/_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,14 +390,15 @@
         For example, you should pass this kind of list -  [["FIRST", "SECOND"], ["ABC", "QWE"]],
         and the decorator will look for value "FIRST" and change it to the
         "SECOND", as well as will look for value "ABC" and will change it to the "QWE".
         In that way, your list should contain lists with two parameters, where first
         is the old value that should be changed, and the second is the value to which it will be changed.
         :return: Transformed dictionary
         """
+        # working_dict = copy.deepcopy(data)
         for key, value in data.items():
             if isinstance(value, dict):
                 data[key] = cls._transform_dict(value, change_fields)
             for change_field in change_fields:
                 if change_field[0] == value:
                     data[key] = change_field[1]
         return data
@@ -416,15 +417,15 @@
             for key, value in loaded_d.items():
                 loaded_d[key] = cls._transform_redis_response(value)
         except (JSONDecodeError, TypeError):
             return data.decode("utf-8") if isinstance(data, bytes) else data
         return loaded_d
 
     @classmethod
-    def make_response(cls, message: str, status_code: int) -> Response:
+    def make_response(cls, message: str, status_code: int) -> Tuple[Response, int]:
         """
         Method to make a Flask response and return it back.
         This response will contain JSON body with 2 parameters - `message`
         (response message, answer) and `status_code` (integer value of HTTP response code).
         :param message: Message on the response
         :param status_code:
         :return: Flask Response
```

### Comparing `py-redis-utils-1.1/setup.py` & `py-redis-utils-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.1"
+VERSION = "1.1.1"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
```

