# Comparing `tmp/discovery-connectors-1.4.3.tar.gz` & `tmp/discovery-connectors-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-connectors-1.4.3.tar", last modified: Wed Apr 26 14:53:22 2023, max compression
+gzip compressed data, was "discovery-connectors-1.4.4.tar", last modified: Wed May 17 12:34:59 2023, max compression
```

## Comparing `discovery-connectors-1.4.3.tar` & `discovery-connectors-1.4.4.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.413227 discovery-connectors-1.4.3/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-26 14:53:22.413481 discovery-connectors-1.4.3/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.399489 discovery-connectors-1.4.3/discovery_connectors.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-26 14:53:22.000000 discovery-connectors-1.4.3/discovery_connectors.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)      981 2023-04-26 14:53:22.000000 discovery-connectors-1.4.3/discovery_connectors.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-04-26 14:53:22.000000 discovery-connectors-1.4.3/discovery_connectors.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      197 2023-04-26 14:53:22.000000 discovery-connectors-1.4.3/discovery_connectors.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-04-26 14:53:22.000000 discovery-connectors-1.4.3/discovery_connectors.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.400212 discovery-connectors-1.4.3/ds_connectors/
--rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-04-25 21:49:25.000000 discovery-connectors-1.4.3/ds_connectors/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.405331 discovery-connectors-1.4.3/ds_connectors/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/ds_connectors/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.4.3/ds_connectors/handlers/cortex_helpers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/ds_connectors/handlers/hive_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.4.3/ds_connectors/handlers/mc_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5089 2023-04-24 14:03:48.000000 discovery-connectors-1.4.3/ds_connectors/handlers/mongodb_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5754 2023-04-08 20:31:43.000000 discovery-connectors-1.4.3/ds_connectors/handlers/mysql_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/ds_connectors/handlers/postgres_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/ds_connectors/handlers/redis_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.406599 discovery-connectors-1.4.3/ds_connectors/parsers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/ds_connectors/parsers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/ds_connectors/parsers/dsv.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-04-26 14:53:22.414557 discovery-connectors-1.4.3/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2354 2023-04-24 14:03:48.000000 discovery-connectors-1.4.3/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.393597 discovery-connectors-1.4.3/tests/
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.407894 discovery-connectors-1.4.3/tests/aws/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/tests/aws/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/tests/aws/s3_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.408507 discovery-connectors-1.4.3/tests/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.3/tests/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.409104 discovery-connectors-1.4.3/tests/managed_content/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.4.3/tests/managed_content/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.4.3/tests/managed_content/mc_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.410317 discovery-connectors-1.4.3/tests/mongodb/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-24 14:02:30.000000 discovery-connectors-1.4.3/tests/mongodb/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8334 2023-04-24 14:02:17.000000 discovery-connectors-1.4.3/tests/mongodb/mongodb_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.411706 discovery-connectors-1.4.3/tests/mysql/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.3/tests/mysql/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8825 2023-04-24 14:02:30.000000 discovery-connectors-1.4.3/tests/mysql/mysql_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-26 14:53:22.412689 discovery-connectors-1.4.3/tests/po1/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.4.3/tests/po1/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.319429 discovery-connectors-1.4.4/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-05-17 12:34:59.319754 discovery-connectors-1.4.4/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.262804 discovery-connectors-1.4.4/discovery_connectors.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-05-17 12:34:58.000000 discovery-connectors-1.4.4/discovery_connectors.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1023 2023-05-17 12:34:59.000000 discovery-connectors-1.4.4/discovery_connectors.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-05-17 12:34:58.000000 discovery-connectors-1.4.4/discovery_connectors.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      197 2023-05-17 12:34:58.000000 discovery-connectors-1.4.4/discovery_connectors.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-05-17 12:34:58.000000 discovery-connectors-1.4.4/discovery_connectors.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.263725 discovery-connectors-1.4.4/ds_connectors/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-05-15 13:51:03.000000 discovery-connectors-1.4.4/ds_connectors/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.306110 discovery-connectors-1.4.4/ds_connectors/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/ds_connectors/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.4.4/ds_connectors/handlers/cortex_helpers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/ds_connectors/handlers/hive_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.4.4/ds_connectors/handlers/mc_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5089 2023-04-24 14:03:48.000000 discovery-connectors-1.4.4/ds_connectors/handlers/mongodb_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5754 2023-04-08 20:31:43.000000 discovery-connectors-1.4.4/ds_connectors/handlers/mysql_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7002 2023-05-15 13:53:46.000000 discovery-connectors-1.4.4/ds_connectors/handlers/oracle_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/ds_connectors/handlers/postgres_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/ds_connectors/handlers/redis_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.308567 discovery-connectors-1.4.4/ds_connectors/parsers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/ds_connectors/parsers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/ds_connectors/parsers/dsv.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-05-17 12:34:59.321199 discovery-connectors-1.4.4/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2354 2023-04-24 14:03:48.000000 discovery-connectors-1.4.4/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.253270 discovery-connectors-1.4.4/tests/
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.310697 discovery-connectors-1.4.4/tests/aws/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/tests/aws/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/tests/aws/s3_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.311801 discovery-connectors-1.4.4/tests/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.4/tests/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.312939 discovery-connectors-1.4.4/tests/managed_content/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.4.4/tests/managed_content/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.4.4/tests/managed_content/mc_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.315113 discovery-connectors-1.4.4/tests/mongodb/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-24 14:02:30.000000 discovery-connectors-1.4.4/tests/mongodb/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8334 2023-04-24 14:02:17.000000 discovery-connectors-1.4.4/tests/mongodb/mongodb_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.317436 discovery-connectors-1.4.4/tests/mysql/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.4/tests/mysql/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8825 2023-04-24 14:02:30.000000 discovery-connectors-1.4.4/tests/mysql/mysql_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-05-17 12:34:59.318656 discovery-connectors-1.4.4/tests/po1/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.4.4/tests/po1/__init__.py
```

### Comparing `discovery-connectors-1.4.3/LICENSE.txt` & `discovery-connectors-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/PKG-INFO` & `discovery-connectors-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.4.3
+Version: 1.4.4
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-connectors-1.4.3/discovery_connectors.egg-info/PKG-INFO` & `discovery-connectors-1.4.4/discovery_connectors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.4.3
+Version: 1.4.4
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-connectors-1.4.3/discovery_connectors.egg-info/SOURCES.txt` & `discovery-connectors-1.4.4/discovery_connectors.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ds_connectors/__init__.py
 ds_connectors/handlers/__init__.py
 ds_connectors/handlers/cortex_helpers.py
 ds_connectors/handlers/hive_handlers.py
 ds_connectors/handlers/mc_handlers.py
 ds_connectors/handlers/mongodb_handlers.py
 ds_connectors/handlers/mysql_handlers.py
+ds_connectors/handlers/oracle_handlers.py
 ds_connectors/handlers/postgres_handlers.py
 ds_connectors/handlers/redis_handlers.py
 ds_connectors/parsers/__init__.py
 ds_connectors/parsers/dsv.py
 tests/aws/__init__.py
 tests/aws/s3_handler_test.py
 tests/handlers/__init__.py
```

### Comparing `discovery-connectors-1.4.3/ds_connectors/handlers/cortex_helpers.py` & `discovery-connectors-1.4.4/ds_connectors/handlers/cortex_helpers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/ds_connectors/handlers/hive_handlers.py` & `discovery-connectors-1.4.4/ds_connectors/handlers/hive_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/ds_connectors/handlers/mc_handlers.py` & `discovery-connectors-1.4.4/ds_connectors/handlers/mc_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/ds_connectors/handlers/mongodb_handlers.py` & `discovery-connectors-1.4.4/ds_connectors/handlers/mongodb_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/ds_connectors/handlers/mysql_handlers.py` & `discovery-connectors-1.4.4/ds_connectors/handlers/mysql_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/ds_connectors/handlers/postgres_handlers.py` & `discovery-connectors-1.4.4/ds_connectors/handlers/postgres_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/ds_connectors/handlers/redis_handlers.py` & `discovery-connectors-1.4.4/ds_connectors/handlers/redis_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/ds_connectors/parsers/dsv.py` & `discovery-connectors-1.4.4/ds_connectors/parsers/dsv.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/setup.py` & `discovery-connectors-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/tests/aws/s3_handler_test.py` & `discovery-connectors-1.4.4/tests/aws/s3_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/tests/managed_content/mc_handler_test.py` & `discovery-connectors-1.4.4/tests/managed_content/mc_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/tests/mongodb/mongodb_handler_test.py` & `discovery-connectors-1.4.4/tests/mongodb/mongodb_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.3/tests/mysql/mysql_handler_test.py` & `discovery-connectors-1.4.4/tests/mysql/mysql_handler_test.py`

 * *Files identical despite different names*

