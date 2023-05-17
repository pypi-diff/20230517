# Comparing `tmp/nuclio_sdk-0.5.2.tar.gz` & `tmp/nuclio_sdk-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-jfy0923j/nuclio_sdk-0.5.2.tar", last modified: Mon May  1 08:30:35 2023, max compression
+gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-moulhhhn/nuclio_sdk-0.5.3.tar", last modified: Wed May 17 14:34:20 2023, max compression
```

## Comparing `nuclio_sdk-0.5.2.tar` & `nuclio_sdk-0.5.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/mock_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/mock_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/nuclio_sdk/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/nuclio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 14:34:20.000000 nuclio_sdk-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-17 14:33:45.000000 nuclio_sdk-0.5.3/setup.py
```

### Comparing `nuclio_sdk-0.5.2/LICENSE.txt` & `nuclio_sdk-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/PKG-INFO` & `nuclio_sdk-0.5.3/nuclio_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nuclio_sdk
-Version: 0.5.2
+Name: nuclio-sdk
+Version: 0.5.3
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.2/Pipfile` & `nuclio_sdk-0.5.3/Pipfile`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/Pipfile.lock` & `nuclio_sdk-0.5.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/__init__.py` & `nuclio_sdk-0.5.3/nuclio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/context.py` & `nuclio_sdk-0.5.3/nuclio_sdk/context.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/event.py` & `nuclio_sdk-0.5.3/nuclio_sdk/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             timestamp=datetime.datetime.utcfromtimestamp(parsed_data["timestamp"]),
             url=parsed_data["url"],
             shard_id=parsed_data["shard_id"],
             num_shards=parsed_data["num_shards"],
             _type=parsed_data["type"],
             type_version=parsed_data["type_version"],
             version=parsed_data["version"],
+            offset=parsed_data.get("offset", 0),
         )
 
     @staticmethod
     def _from_parsed_data_bytes(parsed_data, body):
         trigger = TriggerInfo(
             parsed_data[b"trigger"][b"kind"], parsed_data[b"trigger"][b"name"]
         )
@@ -80,14 +81,15 @@
             timestamp=datetime.datetime.utcfromtimestamp(parsed_data[b"timestamp"]),
             url=parsed_data[b"url"],
             shard_id=parsed_data[b"shard_id"],
             num_shards=parsed_data[b"num_shards"],
             _type=parsed_data[b"type"],
             type_version=parsed_data[b"type_version"],
             version=parsed_data[b"version"],
+            offset=parsed_data.get(b"offset", 0),
         )
 
 
 class _EventDeserializerMsgPack(_EventDeserializer):
     def __init__(self, raw=False):
 
         # return the concrete function that handled raw/decoded event messages
```

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/exceptions.py` & `nuclio_sdk-0.5.3/nuclio_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/helpers.py` & `nuclio_sdk-0.5.3/nuclio_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/json_encoder.py` & `nuclio_sdk-0.5.3/nuclio_sdk/json_encoder.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/logger.py` & `nuclio_sdk-0.5.3/nuclio_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/platform.py` & `nuclio_sdk-0.5.3/nuclio_sdk/platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/qualified_offset.py` & `nuclio_sdk-0.5.3/nuclio_sdk/qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/response.py` & `nuclio_sdk-0.5.3/nuclio_sdk/response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/test/__init__.py` & `nuclio_sdk-0.5.3/nuclio_sdk/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/test/mock_platform.py` & `nuclio_sdk-0.5.3/nuclio_sdk/test/mock_platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/test/test_case.py` & `nuclio_sdk-0.5.3/nuclio_sdk/test/test_case.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/test/test_event.py` & `nuclio_sdk-0.5.3/nuclio_sdk/test/test_event.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/test/test_logger.py` & `nuclio_sdk-0.5.3/nuclio_sdk/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/test/test_qualified_offset.py` & `nuclio_sdk-0.5.3/nuclio_sdk/test/test_qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk/test/test_response.py` & `nuclio_sdk-0.5.3/nuclio_sdk/test/test_response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk.egg-info/PKG-INFO` & `nuclio_sdk-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nuclio-sdk
-Version: 0.5.2
+Name: nuclio_sdk
+Version: 0.5.3
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.2/nuclio_sdk.egg-info/SOURCES.txt` & `nuclio_sdk-0.5.3/nuclio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.2/setup.py` & `nuclio_sdk-0.5.3/setup.py`

 * *Files identical despite different names*

