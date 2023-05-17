# Comparing `tmp/eswrap-0.4.5.tar.gz` & `tmp/eswrap-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.4.5.tar", last modified: Fri May 12 12:11:42 2023, max compression
+gzip compressed data, was "eswrap-0.4.6.tar", last modified: Wed May 17 10:50:49 2023, max compression
```

## Comparing `eswrap-0.4.5.tar` & `eswrap-0.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-12 12:11:42.501857 eswrap-0.4.5/
--rw-rw-r--   0 paul      (1000) paul      (1000)      566 2023-05-12 12:11:42.501857 eswrap-0.4.5/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)        8 2023-05-08 12:59:52.000000 eswrap-0.4.5/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-12 12:11:42.501857 eswrap-0.4.5/eswrap/
--rw-rw-r--   0 paul      (1000) paul      (1000)    34509 2023-05-08 12:59:52.000000 eswrap-0.4.5/eswrap/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)        5 2023-05-12 12:11:42.000000 eswrap-0.4.5/eswrap/VERSION
--rw-rw-r--   0 paul      (1000) paul      (1000)     2664 2023-05-08 13:05:11.000000 eswrap-0.4.5/eswrap/__init__.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-12 12:11:42.501857 eswrap-0.4.5/eswrap/common/
--rw-rw-r--   0 paul      (1000) paul      (1000)     7447 2023-05-12 11:59:03.000000 eswrap-0.4.5/eswrap/common/EsHandler.py
--rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-05-08 12:59:52.000000 eswrap-0.4.5/eswrap/common/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     3877 2023-05-12 06:02:39.000000 eswrap-0.4.5/eswrap/main.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-12 12:11:42.501857 eswrap-0.4.5/eswrap.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)      566 2023-05-12 12:11:42.000000 eswrap-0.4.5/eswrap.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      284 2023-05-12 12:11:42.000000 eswrap-0.4.5/eswrap.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-05-12 12:11:42.000000 eswrap-0.4.5/eswrap.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       21 2023-05-12 12:11:42.000000 eswrap-0.4.5/eswrap.egg-info/requires.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        7 2023-05-12 12:11:42.000000 eswrap-0.4.5/eswrap.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-05-12 12:11:42.501857 eswrap-0.4.5/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)     1233 2023-05-12 06:02:39.000000 eswrap-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:50:49.460035 eswrap-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-17 10:50:49.460035 eswrap-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 10:50:31.000000 eswrap-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:50:49.456035 eswrap-0.4.6/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-17 10:50:31.000000 eswrap-0.4.6/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 10:50:49.000000 eswrap-0.4.6/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-17 10:50:31.000000 eswrap-0.4.6/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:50:49.460035 eswrap-0.4.6/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-17 10:50:31.000000 eswrap-0.4.6/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:50:31.000000 eswrap-0.4.6/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-17 10:50:31.000000 eswrap-0.4.6/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:50:49.456035 eswrap-0.4.6/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-17 10:50:49.000000 eswrap-0.4.6/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 10:50:49.000000 eswrap-0.4.6/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:50:49.000000 eswrap-0.4.6/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 10:50:49.000000 eswrap-0.4.6/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 10:50:49.000000 eswrap-0.4.6/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:50:49.460035 eswrap-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-17 10:50:31.000000 eswrap-0.4.6/setup.py
```

### Comparing `eswrap-0.4.5/PKG-INFO` & `eswrap-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.5/eswrap/LICENSE` & `eswrap-0.4.6/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.5/eswrap/__init__.py` & `eswrap-0.4.6/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.5/eswrap/common/EsHandler.py` & `eswrap-0.4.6/eswrap/common/EsHandler.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.5/eswrap/main.py` & `eswrap-0.4.6/eswrap/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,13 +119,38 @@
                 f"The index {index_name} cannot not be deleted; reason -> {ret_val}"
             )
         except Exception as err:
             self.logger.error(f"Uncaught exception encountered: {err}")
 
         return False
 
+    def create_index(self, index_name: str):
+
+        ret_val = self.es_client.options(ignore_status=[400, 404]).indices.create(
+            index=index_name
+        )
+
+        try:
+            if ret_val["acknowledged"]:
+                if not hasattr(self, index_name):
+                    setattr(
+                        self,
+                        index_name,
+                        EsHandler(es_connection=self.__es_client, index=index_name),
+                    )
+                return True
+        except KeyError:
+            # failed somehow, assuming the given index does not exist
+            self.logger.warning(
+                f"The index {index_name} cannot not be created; reason -> {ret_val}"
+            )
+        except Exception as err:
+            self.logger.error(f"Uncaught exception encountered: {err}")
+
+        return False
+
     def __del__(self):
         self.__es_client.close()
 
     def __repr__(self):
         """String representation of object"""
         return "<< EsWrap:{} >>".format(self.version)
```

### Comparing `eswrap-0.4.5/eswrap.egg-info/PKG-INFO` & `eswrap-0.4.6/eswrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.5/setup.py` & `eswrap-0.4.6/setup.py`

 * *Files identical despite different names*

