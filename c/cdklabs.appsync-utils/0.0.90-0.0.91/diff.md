# Comparing `tmp/cdklabs.appsync-utils-0.0.90.tar.gz` & `tmp/cdklabs.appsync-utils-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.appsync-utils-0.0.90.tar", last modified: Tue May 16 00:17:17 2023, max compression
+gzip compressed data, was "cdklabs.appsync-utils-0.0.91.tar", last modified: Wed May 17 00:18:38 2023, max compression
```

## Comparing `cdklabs.appsync-utils-0.0.90.tar` & `cdklabs.appsync-utils-0.0.91.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:17:17.551891 cdklabs.appsync-utils-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-16 00:17:17.551891 cdklabs.appsync-utils-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:17:17.551891 cdklabs.appsync-utils-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:17:17.547891 cdklabs.appsync-utils-0.0.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:17:17.547891 cdklabs.appsync-utils-0.0.90/src/awscdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:17:17.547891 cdklabs.appsync-utils-0.0.90/src/awscdk/appsync_utils/
--rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/src/awscdk/appsync_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:17:17.547891 cdklabs.appsync-utils-0.0.90/src/awscdk/appsync_utils/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/src/awscdk/appsync_utils/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82442 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.90.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:17:04.000000 cdklabs.appsync-utils-0.0.90/src/awscdk/appsync_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:17:17.551891 cdklabs.appsync-utils-0.0.90/src/cdklabs.appsync_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-16 00:17:17.000000 cdklabs.appsync-utils-0.0.90/src/cdklabs.appsync_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 00:17:17.000000 cdklabs.appsync-utils-0.0.90/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:17:17.000000 cdklabs.appsync-utils-0.0.90/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 00:17:17.000000 cdklabs.appsync-utils-0.0.90/src/cdklabs.appsync_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 00:17:17.000000 cdklabs.appsync-utils-0.0.90/src/cdklabs.appsync_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:18:38.638947 cdklabs.appsync-utils-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-17 00:18:38.634946 cdklabs.appsync-utils-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:18:38.638947 cdklabs.appsync-utils-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:18:38.634946 cdklabs.appsync-utils-0.0.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:18:38.630946 cdklabs.appsync-utils-0.0.91/src/awscdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:18:38.634946 cdklabs.appsync-utils-0.0.91/src/awscdk/appsync_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   134850 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/src/awscdk/appsync_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:18:38.634946 cdklabs.appsync-utils-0.0.91/src/awscdk/appsync_utils/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/src/awscdk/appsync_utils/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82442 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/src/awscdk/appsync_utils/_jsii/awscdk-appsync-utils@0.0.91.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:18:23.000000 cdklabs.appsync-utils-0.0.91/src/awscdk/appsync_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:18:38.634946 cdklabs.appsync-utils-0.0.91/src/cdklabs.appsync_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-05-17 00:18:38.000000 cdklabs.appsync-utils-0.0.91/src/cdklabs.appsync_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-17 00:18:38.000000 cdklabs.appsync-utils-0.0.91/src/cdklabs.appsync_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:18:38.000000 cdklabs.appsync-utils-0.0.91/src/cdklabs.appsync_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 00:18:38.000000 cdklabs.appsync-utils-0.0.91/src/cdklabs.appsync_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 00:18:38.000000 cdklabs.appsync-utils-0.0.91/src/cdklabs.appsync_utils.egg-info/top_level.txt
```

### Comparing `cdklabs.appsync-utils-0.0.90/LICENSE` & `cdklabs.appsync-utils-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.90/PKG-INFO` & `cdklabs.appsync-utils-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.90
+Version: 0.0.91
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.appsync-utils-0.0.90/README.md` & `cdklabs.appsync-utils-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.90/setup.py` & `cdklabs.appsync-utils-0.0.91/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.appsync-utils",
-    "version": "0.0.90",
+    "version": "0.0.91",
     "description": "Utilities for creating appsync apis using aws-cdk",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/awscdk-appsync-utils.git",
     "long_description_content_type": "text/markdown",
     "author": "Mitchell Valine<mitchellvaline@yahoo.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "awscdk.appsync_utils",
         "awscdk.appsync_utils._jsii"
     ],
     "package_data": {
         "awscdk.appsync_utils._jsii": [
-            "awscdk-appsync-utils@0.0.90.jsii.tgz"
+            "awscdk-appsync-utils@0.0.91.jsii.tgz"
         ],
         "awscdk.appsync_utils": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdklabs.appsync-utils-0.0.90/src/awscdk/appsync_utils/__init__.py` & `cdklabs.appsync-utils-0.0.91/src/awscdk/appsync_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.appsync-utils-0.0.90/src/cdklabs.appsync_utils.egg-info/PKG-INFO` & `cdklabs.appsync-utils-0.0.91/src/cdklabs.appsync_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.appsync-utils
-Version: 0.0.90
+Version: 0.0.91
 Summary: Utilities for creating appsync apis using aws-cdk
 Home-page: https://github.com/cdklabs/awscdk-appsync-utils.git
 Author: Mitchell Valine<mitchellvaline@yahoo.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/awscdk-appsync-utils.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

