# Comparing `tmp/BunkerSync-0.0.11.tar.gz` & `tmp/BunkerSync-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BunkerSync-0.0.11.tar", last modified: Wed May 17 15:05:34 2023, max compression
+gzip compressed data, was "BunkerSync-0.0.12.tar", last modified: Wed May 17 15:09:15 2023, max compression
```

## Comparing `BunkerSync-0.0.11.tar` & `BunkerSync-0.0.12.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 okashal   (1000) okashal   (1000)        0 2023-05-17 15:05:34.724074 BunkerSync-0.0.11/
--rw-rw-r--   0 okashal   (1000) okashal   (1000)    11345 2023-05-17 14:37:31.000000 BunkerSync-0.0.11/LICENSE
--rw-rw-r--   0 okashal   (1000) okashal   (1000)     5793 2023-05-17 15:05:34.724074 BunkerSync-0.0.11/PKG-INFO
-drwxrwxr-x   0 okashal   (1000) okashal   (1000)        0 2023-05-17 15:05:34.720073 BunkerSync-0.0.11/app/
-drwxrwxr-x   0 okashal   (1000) okashal   (1000)        0 2023-05-17 15:05:34.724074 BunkerSync-0.0.11/app/BunkerSync.egg-info/
--rw-rw-r--   0 okashal   (1000) okashal   (1000)     5793 2023-05-17 15:05:34.000000 BunkerSync-0.0.11/app/BunkerSync.egg-info/PKG-INFO
--rw-rw-r--   0 okashal   (1000) okashal   (1000)      205 2023-05-17 15:05:34.000000 BunkerSync-0.0.11/app/BunkerSync.egg-info/SOURCES.txt
--rw-rw-r--   0 okashal   (1000) okashal   (1000)        1 2023-05-17 15:05:34.000000 BunkerSync-0.0.11/app/BunkerSync.egg-info/dependency_links.txt
--rw-rw-r--   0 okashal   (1000) okashal   (1000)       12 2023-05-17 15:05:34.000000 BunkerSync-0.0.11/app/BunkerSync.egg-info/requires.txt
--rw-rw-r--   0 okashal   (1000) okashal   (1000)        1 2023-05-17 15:05:34.000000 BunkerSync-0.0.11/app/BunkerSync.egg-info/top_level.txt
--rw-rw-r--   0 okashal   (1000) okashal   (1000)       38 2023-05-17 15:05:34.724074 BunkerSync-0.0.11/setup.cfg
--rw-rw-r--   0 okashal   (1000) okashal   (1000)     1027 2023-05-17 15:03:57.000000 BunkerSync-0.0.11/setup.py
+drwxrwxr-x   0 okashal   (1000) okashal   (1000)        0 2023-05-17 15:09:15.540082 BunkerSync-0.0.12/
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)    11345 2023-05-17 14:37:31.000000 BunkerSync-0.0.12/LICENSE
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)     5937 2023-05-17 15:09:15.540082 BunkerSync-0.0.12/PKG-INFO
+drwxrwxr-x   0 okashal   (1000) okashal   (1000)        0 2023-05-17 15:09:15.536082 BunkerSync-0.0.12/app/
+drwxrwxr-x   0 okashal   (1000) okashal   (1000)        0 2023-05-17 15:09:15.540082 BunkerSync-0.0.12/app/BunkerSync.egg-info/
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)     5937 2023-05-17 15:09:15.000000 BunkerSync-0.0.12/app/BunkerSync.egg-info/PKG-INFO
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)      205 2023-05-17 15:09:15.000000 BunkerSync-0.0.12/app/BunkerSync.egg-info/SOURCES.txt
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)        1 2023-05-17 15:09:15.000000 BunkerSync-0.0.12/app/BunkerSync.egg-info/dependency_links.txt
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)       12 2023-05-17 15:09:15.000000 BunkerSync-0.0.12/app/BunkerSync.egg-info/requires.txt
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)        1 2023-05-17 15:09:15.000000 BunkerSync-0.0.12/app/BunkerSync.egg-info/top_level.txt
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)       38 2023-05-17 15:09:15.540082 BunkerSync-0.0.12/setup.cfg
+-rw-rw-r--   0 okashal   (1000) okashal   (1000)      987 2023-05-17 15:08:24.000000 BunkerSync-0.0.12/setup.py
```

### Comparing `BunkerSync-0.0.11/LICENSE` & `BunkerSync-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `BunkerSync-0.0.11/PKG-INFO` & `BunkerSync-0.0.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BunkerSync
-Version: 0.0.11
-Summary: BunkerSync simplifies Git repository syncing. 
+Version: 0.0.12
+Summary: BunkerSync simplifies Git repository syncing. Sync internal and external repositories with branch filtering and automatic syncing. Ideal for developers who need to keep repositories in sync.
 Home-page: https://github.com/okashaluai/BunkerSync.git
 Author: Luai Okasha
 Author-email: LuaiOkasha@gmail.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `BunkerSync-0.0.11/app/BunkerSync.egg-info/PKG-INFO` & `BunkerSync-0.0.12/app/BunkerSync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BunkerSync
-Version: 0.0.11
-Summary: BunkerSync simplifies Git repository syncing. 
+Version: 0.0.12
+Summary: BunkerSync simplifies Git repository syncing. Sync internal and external repositories with branch filtering and automatic syncing. Ideal for developers who need to keep repositories in sync.
 Home-page: https://github.com/okashaluai/BunkerSync.git
 Author: Luai Okasha
 Author-email: LuaiOkasha@gmail.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `BunkerSync-0.0.11/setup.py` & `BunkerSync-0.0.12/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="BunkerSync",
-    version="0.0.11",
-    description="""BunkerSync simplifies Git repository syncing. 
-                   Sync internal and external repositories with branch filtering and automatic syncing. 
-                   Ideal for developers who need to keep repositories in sync.""",
+    version="0.0.12",
+    description="""BunkerSync simplifies Git repository syncing. Sync internal and external repositories with branch filtering and automatic syncing. Ideal for developers who need to keep repositories in sync.""",
     package_dir={"": "app"},
     packages= find_packages(where="app"),
     long_description= long_description ,
     long_description_content_type = "text/markdown",
     url= "https://github.com/okashaluai/BunkerSync.git",
     author= "Luai Okasha",
     author_email= "LuaiOkasha@gmail.com",
```

