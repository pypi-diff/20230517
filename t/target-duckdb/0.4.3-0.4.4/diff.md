# Comparing `tmp/target-duckdb-0.4.3.tar.gz` & `tmp/target-duckdb-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-duckdb-0.4.3.tar", last modified: Mon Oct 31 16:01:01 2022, max compression
+gzip compressed data, was "target-duckdb-0.4.4.tar", last modified: Tue Jan 24 22:42:51 2023, max compression
```

## Comparing `target-duckdb-0.4.3.tar` & `target-duckdb-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2022-10-31 16:01:01.949961 target-duckdb-0.4.3/
--rw-r--r--   0 jwills     (501) staff       (20)    10409 2022-04-04 16:17:07.000000 target-duckdb-0.4.3/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)     5627 2022-10-31 16:01:01.949553 target-duckdb-0.4.3/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     5240 2022-10-31 15:59:49.000000 target-duckdb-0.4.3/README.md
--rw-r--r--   0 jwills     (501) staff       (20)       38 2022-10-31 16:01:01.950072 target-duckdb-0.4.3/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1046 2022-10-31 16:00:31.000000 target-duckdb-0.4.3/setup.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2022-10-31 16:01:01.945815 target-duckdb-0.4.3/target_duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)    15202 2022-10-28 18:21:28.000000 target-duckdb-0.4.3/target_duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)    21429 2022-10-28 18:21:28.000000 target-duckdb-0.4.3/target_duckdb/db_sync.py
--rw-r--r--   0 jwills     (501) staff       (20)      685 2022-10-31 16:00:13.000000 target-duckdb-0.4.3/target_duckdb/logger.py
--rw-r--r--   0 jwills     (501) staff       (20)      370 2022-10-28 18:21:28.000000 target-duckdb-0.4.3/target_duckdb/logging.conf
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2022-10-31 16:01:01.948979 target-duckdb-0.4.3/target_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)     5627 2022-10-31 16:01:01.000000 target-duckdb-0.4.3/target_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      352 2022-10-31 16:01:01.000000 target-duckdb-0.4.3/target_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2022-10-31 16:01:01.000000 target-duckdb-0.4.3/target_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       53 2022-10-31 16:01:01.000000 target-duckdb-0.4.3/target_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 jwills     (501) staff       (20)       65 2022-10-31 16:01:01.000000 target-duckdb-0.4.3/target_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)       14 2022-10-31 16:01:01.000000 target-duckdb-0.4.3/target_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-24 22:42:51.636423 target-duckdb-0.4.4/
+-rw-r--r--   0 jwills     (501) staff       (20)    10409 2022-12-17 04:32:30.000000 target-duckdb-0.4.4/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)     5627 2023-01-24 22:42:51.636310 target-duckdb-0.4.4/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     5240 2022-12-17 04:32:30.000000 target-duckdb-0.4.4/README.md
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-01-24 22:42:51.636456 target-duckdb-0.4.4/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1010 2023-01-24 22:42:31.000000 target-duckdb-0.4.4/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-24 22:42:51.635542 target-duckdb-0.4.4/target_duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)    15202 2022-12-17 04:32:30.000000 target-duckdb-0.4.4/target_duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)    21717 2023-01-24 22:42:31.000000 target-duckdb-0.4.4/target_duckdb/db_sync.py
+-rw-r--r--   0 jwills     (501) staff       (20)      685 2023-01-24 22:42:31.000000 target-duckdb-0.4.4/target_duckdb/logger.py
+-rw-r--r--   0 jwills     (501) staff       (20)      370 2022-12-17 04:32:30.000000 target-duckdb-0.4.4/target_duckdb/logging.conf
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-01-24 22:42:51.636175 target-duckdb-0.4.4/target_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)     5627 2023-01-24 22:42:51.000000 target-duckdb-0.4.4/target_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      352 2023-01-24 22:42:51.000000 target-duckdb-0.4.4/target_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-01-24 22:42:51.000000 target-duckdb-0.4.4/target_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-24 22:42:51.000000 target-duckdb-0.4.4/target_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       65 2023-01-24 22:42:51.000000 target-duckdb-0.4.4/target_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       14 2023-01-24 22:42:51.000000 target-duckdb-0.4.4/target_duckdb.egg-info/top_level.txt
```

### Comparing `target-duckdb-0.4.3/LICENSE` & `target-duckdb-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.4.3/PKG-INFO` & `target-duckdb-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-duckdb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Singer.io target for loading data into DuckDB
 Home-page: https://github.com/jwills/target-duckdb
 Author: TransferWise
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `target-duckdb-0.4.3/README.md` & `target-duckdb-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.4.3/setup.py` & `target-duckdb-0.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="target-duckdb",
-    version="0.4.3",
+    version="0.4.4",
     description="Singer.io target for loading data into DuckDB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TransferWise",
     url="https://github.com/jwills/target-duckdb",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
@@ -30,14 +30,10 @@
         ]
     },
     entry_points="""
           [console_scripts]
           target-duckdb=target_duckdb:main
       """,
     packages=["target_duckdb"],
-    package_data={
-        "target_duckdb": [
-            "logging.conf"
-        ]
-    },
+    package_data={"target_duckdb": ["logging.conf"]},
     include_package_data=True,
 )
```

### Comparing `target-duckdb-0.4.3/target_duckdb/__init__.py` & `target-duckdb-0.4.4/target_duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.4.3/target_duckdb/db_sync.py` & `target-duckdb-0.4.4/target_duckdb/db_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,22 @@
                         sep=sep,
                         level=level + 1,
                         max_level=max_level,
                     ).items()
                 )
             else:
                 items.append((new_key, v))
+        elif "anyOf" in v.keys():
+            llv = v["anyOf"]
+            i, entry = 0, llv[0]
+            while entry["type"] == "null":
+                i += 1
+                entry = llv[i]
+            entry["type"] = ["null", entry["type"]]
+            items.append((new_key, entry))
         else:
             if len(v.values()) > 0:
                 if list(v.values())[0][0]["type"] == "string":
                     list(v.values())[0][0]["type"] = ["null", "string"]
                     items.append((new_key, list(v.values())[0][0]))
                 elif list(v.values())[0][0]["type"] == "array":
                     list(v.values())[0][0]["type"] = ["null", "array"]
```

### Comparing `target-duckdb-0.4.3/target_duckdb/logger.py` & `target-duckdb-0.4.4/target_duckdb/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import logging.config
 import os
 
 
-def get_logger(name='singer'):
+def get_logger(name="singer"):
     """Return a Logger instance to use in singer."""
     # Use custom logging config provided by environment variable
-    if 'LOGGING_CONF_FILE' in os.environ and os.environ['LOGGING_CONF_FILE']:
-        path = os.environ['LOGGING_CONF_FILE']
+    if "LOGGING_CONF_FILE" in os.environ and os.environ["LOGGING_CONF_FILE"]:
+        path = os.environ["LOGGING_CONF_FILE"]
         logging.config.fileConfig(path, disable_existing_loggers=False)
     # Use the default logging conf that meets the singer specs criteria
     else:
         this_dir, _ = os.path.split(__file__)
-        path = os.path.join(this_dir, 'logging.conf')
+        path = os.path.join(this_dir, "logging.conf")
         logging.config.fileConfig(path, disable_existing_loggers=False)
 
     return logging.getLogger(name)
```

### Comparing `target-duckdb-0.4.3/target_duckdb.egg-info/PKG-INFO` & `target-duckdb-0.4.4/target_duckdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-duckdb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Singer.io target for loading data into DuckDB
 Home-page: https://github.com/jwills/target-duckdb
 Author: TransferWise
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

