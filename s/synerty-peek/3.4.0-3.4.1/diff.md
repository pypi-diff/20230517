# Comparing `tmp/synerty-peek-3.4.0.tar.gz` & `tmp/synerty-peek-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synerty-peek-3.4.0.tar", last modified: Wed Apr 12 11:05:38 2023, max compression
+gzip compressed data, was "synerty-peek-3.4.1.tar", last modified: Wed May 17 03:32:14 2023, max compression
```

## Comparing `synerty-peek-3.4.0.tar` & `synerty-peek-3.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:38.936204 synerty-peek-3.4.0/
--rw-r--r--   0 root         (0) root         (0)      462 2023-04-12 11:05:38.936204 synerty-peek-3.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2984 2023-04-12 11:03:19.000000 synerty-peek-3.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:38.936204 synerty-peek-3.4.0/peek/
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-12 11:03:19.000000 synerty-peek-3.4.0/peek/__init__.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 11:05:38.937204 synerty-peek-3.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2051 2023-04-12 11:05:38.000000 synerty-peek-3.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:38.936204 synerty-peek-3.4.0/synerty_peek.egg-info/
--rw-r--r--   0 root         (0) root         (0)      462 2023-04-12 11:05:38.000000 synerty-peek-3.4.0/synerty_peek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-12 11:05:38.000000 synerty-peek-3.4.0/synerty_peek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:38.000000 synerty-peek-3.4.0/synerty_peek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:38.000000 synerty-peek-3.4.0/synerty_peek.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      802 2023-04-12 11:05:38.000000 synerty-peek-3.4.0/synerty_peek.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-12 11:05:38.000000 synerty-peek-3.4.0/synerty_peek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:14.780430 synerty-peek-3.4.1/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-05-17 03:32:14.780430 synerty-peek-3.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-05-17 03:29:56.000000 synerty-peek-3.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:14.780430 synerty-peek-3.4.1/peek/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-17 03:29:56.000000 synerty-peek-3.4.1/peek/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-17 03:32:14.780430 synerty-peek-3.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-05-17 03:32:14.000000 synerty-peek-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:14.780430 synerty-peek-3.4.1/synerty_peek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-05-17 03:32:14.000000 synerty-peek-3.4.1/synerty_peek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-17 03:32:14.000000 synerty-peek-3.4.1/synerty_peek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:32:14.000000 synerty-peek-3.4.1/synerty_peek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:32:14.000000 synerty-peek-3.4.1/synerty_peek.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      802 2023-05-17 03:32:14.000000 synerty-peek-3.4.1/synerty_peek.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 03:32:14.000000 synerty-peek-3.4.1/synerty_peek.egg-info/top_level.txt
```

### Comparing `synerty-peek-3.4.0/README.rst` & `synerty-peek-3.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `synerty-peek-3.4.0/setup.py` & `synerty-peek-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 
 from setuptools import find_packages, setup
 
 pip_package_name = "synerty-peek"
-package_version = "3.4.0"
+package_version = "3.4.1"
 
 egg_info = "%s.egg-info" % pip_package_name
 if os.path.isdir(egg_info):
     shutil.rmtree(egg_info)
 
 if os.path.isfile("MANIFEST"):
     os.remove("MANIFEST")
```

### Comparing `synerty-peek-3.4.0/synerty_peek.egg-info/requires.txt` & `synerty-peek-3.4.1/synerty_peek.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-peek-admin-doc==3.4.*,>=3.4.0
-peek-admin-app==3.4.*,>=3.4.0
-peek-agent-service==3.4.*,>=3.4.0
-peek-core-device==3.4.*,>=3.4.0
-peek-core-docdb==3.4.*,>=3.4.0
-peek-core-email==3.4.*,>=3.4.0
-peek-core-search==3.4.*,>=3.4.0
-peek-core-user==3.4.*,>=3.4.0
-peek-core-screen==3.4.*,>=3.4.0
-peek-field-doc==3.4.*,>=3.4.0
-peek-field-app==3.4.*,>=3.4.0
-peek-field-service==3.4.*,>=3.4.0
-peek-logic-service==3.4.*,>=3.4.0
-peek-office-doc==3.4.*,>=3.4.0
-peek-office-app==3.4.*,>=3.4.0
-peek-office-service==3.4.*,>=3.4.0
-peek-platform==3.4.*,>=3.4.0
-peek-plugin-base==3.4.*,>=3.4.0
-peek-storage-service==3.4.*,>=3.4.0
-peek-worker-service==3.4.*,>=3.4.0
-peek-abstract-chunked-index==3.4.*,>=3.4.0
-peek-abstract-chunked-data-loader==3.4.*,>=3.4.0
+peek-admin-doc==3.4.*,>=3.4.1
+peek-admin-app==3.4.*,>=3.4.1
+peek-agent-service==3.4.*,>=3.4.1
+peek-core-device==3.4.*,>=3.4.1
+peek-core-docdb==3.4.*,>=3.4.1
+peek-core-email==3.4.*,>=3.4.1
+peek-core-search==3.4.*,>=3.4.1
+peek-core-user==3.4.*,>=3.4.1
+peek-core-screen==3.4.*,>=3.4.1
+peek-field-doc==3.4.*,>=3.4.1
+peek-field-app==3.4.*,>=3.4.1
+peek-field-service==3.4.*,>=3.4.1
+peek-logic-service==3.4.*,>=3.4.1
+peek-office-doc==3.4.*,>=3.4.1
+peek-office-app==3.4.*,>=3.4.1
+peek-office-service==3.4.*,>=3.4.1
+peek-platform==3.4.*,>=3.4.1
+peek-plugin-base==3.4.*,>=3.4.1
+peek-storage-service==3.4.*,>=3.4.1
+peek-worker-service==3.4.*,>=3.4.1
+peek-abstract-chunked-index==3.4.*,>=3.4.1
+peek-abstract-chunked-data-loader==3.4.*,>=3.4.1
 sphinx
 sphinx-rtd-theme
 sphinx-autobuild
 pytmpdir<1.1.0,>=1.0.2
 py-spy
```

