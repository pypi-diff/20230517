# Comparing `tmp/interpret-0.4.0.tar.gz` & `tmp/interpret-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpret-0.4.0.tar", last modified: Thu May 11 12:05:50 2023, max compression
+gzip compressed data, was "interpret-0.4.1.tar", last modified: Tue May 16 23:05:37 2023, max compression
```

## Comparing `interpret-0.4.0.tar` & `interpret-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:50.852062 interpret-0.4.0/
--rw-r--r--   0 vsts      (1001) docker     (122)      976 2023-05-11 12:05:50.848062 interpret-0.4.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 12:05:50.848062 interpret-0.4.0/interpret.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      976 2023-05-11 12:05:50.000000 interpret-0.4.0/interpret.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      172 2023-05-11 12:05:50.000000 interpret-0.4.0/interpret.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-11 12:05:50.000000 interpret-0.4.0/interpret.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-05-11 12:05:50.000000 interpret-0.4.0/interpret.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-11 12:05:50.000000 interpret-0.4.0/interpret.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-11 12:05:50.852062 interpret-0.4.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1662 2023-05-11 12:00:39.000000 interpret-0.4.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:37.985360 interpret-0.4.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)      976 2023-05-16 23:05:37.985360 interpret-0.4.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-16 23:05:37.981360 interpret-0.4.1/interpret.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      976 2023-05-16 23:05:37.000000 interpret-0.4.1/interpret.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      172 2023-05-16 23:05:37.000000 interpret-0.4.1/interpret.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-16 23:05:37.000000 interpret-0.4.1/interpret.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-05-16 23:05:37.000000 interpret-0.4.1/interpret.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-16 23:05:37.000000 interpret-0.4.1/interpret.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-16 23:05:37.985360 interpret-0.4.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1662 2023-05-16 23:00:07.000000 interpret-0.4.1/setup.py
```

### Comparing `interpret-0.4.0/PKG-INFO` & `interpret-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `interpret-0.4.0/interpret.egg-info/PKG-INFO` & `interpret-0.4.1/interpret.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `interpret-0.4.0/setup.py` & `interpret-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2023 The InterpretML Contributors
 # Distributed under the MIT software license
 
 from setuptools import setup, find_packages
 
 name = "interpret"
 # NOTE: Version is replaced by a regex script.
-version = "0.4.0"
+version = "0.4.1"
 long_description = """
 In the beginning machines learned in darkness, and data scientists struggled in the void to explain them.
 
 Let there be light.
 
 https://github.com/interpretml/interpret
 """
```

