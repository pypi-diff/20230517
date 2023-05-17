# Comparing `tmp/chailie-0.3.0.tar.gz` & `tmp/chailie-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chailie-0.3.0.tar", last modified: Tue May 16 06:20:58 2023, max compression
+gzip compressed data, was "chailie-0.3.1.tar", last modified: Wed May 17 06:54:01 2023, max compression
```

## Comparing `chailie-0.3.0.tar` & `chailie-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 06:20:58.197236 chailie-0.3.0/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 chailie-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 chailie-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-05-16 06:20:58.198237 chailie-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 chailie-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 06:20:58.161238 chailie-0.3.0/chailie/
-drwxrwxrwx   0        0        0        0 2023-05-16 06:20:58.186238 chailie-0.3.0/chailie/Function/
--rw-rw-rw-   0        0        0        0 2023-05-03 10:04:28.000000 chailie-0.3.0/chailie/Function/__init__.py
--rw-rw-rw-   0        0        0    69120 2023-05-05 07:36:40.000000 chailie-0.3.0/chailie/Function/optionDb.pyd
--rw-rw-rw-   0        0        0        0 2023-05-03 10:04:20.000000 chailie-0.3.0/chailie/__init__.py
--rw-rw-rw-   0        0        0    99328 2023-05-12 07:40:55.000000 chailie-0.3.0/chailie/chailie.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 06:20:58.194310 chailie-0.3.0/chailie/database/
--rw-rw-rw-   0        0        0        0 2023-05-03 10:04:34.000000 chailie-0.3.0/chailie/database/__init__.py
--rw-rw-rw-   0        0        0     8192 2023-05-03 07:44:24.000000 chailie-0.3.0/chailie/database/userOption.db
-drwxrwxrwx   0        0        0        0 2023-05-16 06:20:58.179235 chailie-0.3.0/chailie.egg-info/
--rw-rw-rw-   0        0        0      408 2023-05-16 06:20:58.000000 chailie-0.3.0/chailie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-05-16 06:20:58.000000 chailie-0.3.0/chailie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 06:20:58.000000 chailie-0.3.0/chailie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 06:20:58.000000 chailie-0.3.0/chailie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-05-16 06:20:58.200237 chailie-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-05-16 06:17:40.000000 chailie-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:01.226288 chailie-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 chailie-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 chailie-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-05-17 06:54:01.227290 chailie-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 chailie-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:01.180288 chailie-0.3.1/chailie/
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:01.206290 chailie-0.3.1/chailie/Function/
+-rw-rw-rw-   0        0        0        0 2023-05-03 10:04:28.000000 chailie-0.3.1/chailie/Function/__init__.py
+-rw-rw-rw-   0        0        0    69120 2023-05-05 07:36:40.000000 chailie-0.3.1/chailie/Function/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:01.213288 chailie-0.3.1/chailie/Ui/
+-rw-rw-rw-   0        0        0        0 2023-05-03 10:04:28.000000 chailie-0.3.1/chailie/Ui/__init__.py
+-rw-rw-rw-   0        0        0    72192 2023-05-05 07:36:28.000000 chailie-0.3.1/chailie/Ui/chailieUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-05-03 10:04:20.000000 chailie-0.3.1/chailie/__init__.py
+-rw-rw-rw-   0        0        0    99328 2023-05-12 07:40:55.000000 chailie-0.3.1/chailie/chailie.pyd
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:01.223290 chailie-0.3.1/chailie/database/
+-rw-rw-rw-   0        0        0        0 2023-05-03 10:04:34.000000 chailie-0.3.1/chailie/database/__init__.py
+-rw-rw-rw-   0        0        0     8192 2023-05-03 07:44:24.000000 chailie-0.3.1/chailie/database/userOption.db
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:01.197287 chailie-0.3.1/chailie.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-05-17 06:54:01.000000 chailie-0.3.1/chailie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-17 06:54:01.000000 chailie-0.3.1/chailie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:54:01.000000 chailie-0.3.1/chailie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 06:54:01.000000 chailie-0.3.1/chailie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-05-17 06:54:01.228292 chailie-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-05-17 06:53:15.000000 chailie-0.3.1/setup.py
```

### Comparing `chailie-0.3.0/LICENSE.txt` & `chailie-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chailie-0.3.0/chailie/database/userOption.db` & `chailie-0.3.1/chailie/database/userOption.db`

 * *Files identical despite different names*

### Comparing `chailie-0.3.0/setup.py` & `chailie-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 0
+PATCH = 1
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "chailie",
```

