# Comparing `tmp/gettestmail-1.0.0.tar.gz` & `tmp/gettestmail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gettestmail-1.0.0.tar", last modified: Thu Apr 13 11:24:43 2023, max compression
+gzip compressed data, was "gettestmail-1.0.1.tar", last modified: Wed May 17 13:06:35 2023, max compression
```

## Comparing `gettestmail-1.0.0.tar` & `gettestmail-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bdonchev   (501) staff       (20)        0 2023-04-13 11:24:43.397825 gettestmail-1.0.0/
--rw-r--r--   0 bdonchev   (501) staff       (20)     1068 2023-04-13 10:48:10.000000 gettestmail-1.0.0/LICENSE
--rw-r--r--   0 bdonchev   (501) staff       (20)     1481 2023-04-13 11:24:43.397686 gettestmail-1.0.0/PKG-INFO
--rw-r--r--   0 bdonchev   (501) staff       (20)      735 2023-04-13 11:16:34.000000 gettestmail-1.0.0/README.md
-drwxr-xr-x   0 bdonchev   (501) staff       (20)        0 2023-04-13 11:24:43.396944 gettestmail-1.0.0/gettestmail/
--rw-r--r--   0 bdonchev   (501) staff       (20)       38 2023-04-13 11:03:18.000000 gettestmail-1.0.0/gettestmail/__init__.py
--rw-r--r--   0 bdonchev   (501) staff       (20)     1383 2023-04-13 11:01:54.000000 gettestmail-1.0.0/gettestmail/client.py
--rw-r--r--   0 bdonchev   (501) staff       (20)      498 2023-04-13 10:54:18.000000 gettestmail-1.0.0/gettestmail/models.py
-drwxr-xr-x   0 bdonchev   (501) staff       (20)        0 2023-04-13 11:24:43.397525 gettestmail-1.0.0/gettestmail.egg-info/
--rw-r--r--   0 bdonchev   (501) staff       (20)     1481 2023-04-13 11:24:43.000000 gettestmail-1.0.0/gettestmail.egg-info/PKG-INFO
--rw-r--r--   0 bdonchev   (501) staff       (20)      268 2023-04-13 11:24:43.000000 gettestmail-1.0.0/gettestmail.egg-info/SOURCES.txt
--rw-r--r--   0 bdonchev   (501) staff       (20)        1 2023-04-13 11:24:43.000000 gettestmail-1.0.0/gettestmail.egg-info/dependency_links.txt
--rw-r--r--   0 bdonchev   (501) staff       (20)        9 2023-04-13 11:24:43.000000 gettestmail-1.0.0/gettestmail.egg-info/requires.txt
--rw-r--r--   0 bdonchev   (501) staff       (20)       12 2023-04-13 11:24:43.000000 gettestmail-1.0.0/gettestmail.egg-info/top_level.txt
--rw-r--r--   0 bdonchev   (501) staff       (20)       38 2023-04-13 11:24:43.397860 gettestmail-1.0.0/setup.cfg
--rw-r--r--   0 bdonchev   (501) staff       (20)     1026 2023-04-13 11:12:09.000000 gettestmail-1.0.0/setup.py
+drwxr-xr-x   0 bdonchev   (501) staff       (20)        0 2023-05-17 13:06:35.932109 gettestmail-1.0.1/
+-rw-r--r--   0 bdonchev   (501) staff       (20)     1068 2023-04-13 10:48:10.000000 gettestmail-1.0.1/LICENSE
+-rw-r--r--   0 bdonchev   (501) staff       (20)     2572 2023-05-17 13:06:35.932001 gettestmail-1.0.1/PKG-INFO
+-rw-r--r--   0 bdonchev   (501) staff       (20)     1826 2023-05-17 11:32:09.000000 gettestmail-1.0.1/README.md
+drwxr-xr-x   0 bdonchev   (501) staff       (20)        0 2023-05-17 13:06:35.931310 gettestmail-1.0.1/gettestmail/
+-rw-r--r--   0 bdonchev   (501) staff       (20)       38 2023-04-13 11:03:18.000000 gettestmail-1.0.1/gettestmail/__init__.py
+-rw-r--r--   0 bdonchev   (501) staff       (20)     1371 2023-05-17 13:03:04.000000 gettestmail-1.0.1/gettestmail/client.py
+-rw-r--r--   0 bdonchev   (501) staff       (20)      510 2023-05-17 11:25:50.000000 gettestmail-1.0.1/gettestmail/models.py
+drwxr-xr-x   0 bdonchev   (501) staff       (20)        0 2023-05-17 13:06:35.931849 gettestmail-1.0.1/gettestmail.egg-info/
+-rw-r--r--   0 bdonchev   (501) staff       (20)     2572 2023-05-17 13:06:35.000000 gettestmail-1.0.1/gettestmail.egg-info/PKG-INFO
+-rw-r--r--   0 bdonchev   (501) staff       (20)      268 2023-05-17 13:06:35.000000 gettestmail-1.0.1/gettestmail.egg-info/SOURCES.txt
+-rw-r--r--   0 bdonchev   (501) staff       (20)        1 2023-05-17 13:06:35.000000 gettestmail-1.0.1/gettestmail.egg-info/dependency_links.txt
+-rw-r--r--   0 bdonchev   (501) staff       (20)        9 2023-05-17 13:06:35.000000 gettestmail-1.0.1/gettestmail.egg-info/requires.txt
+-rw-r--r--   0 bdonchev   (501) staff       (20)       12 2023-05-17 13:06:35.000000 gettestmail-1.0.1/gettestmail.egg-info/top_level.txt
+-rw-r--r--   0 bdonchev   (501) staff       (20)       38 2023-05-17 13:06:35.932141 gettestmail-1.0.1/setup.cfg
+-rw-r--r--   0 bdonchev   (501) staff       (20)     1026 2023-05-17 13:06:17.000000 gettestmail-1.0.1/setup.py
```

### Comparing `gettestmail-1.0.0/LICENSE` & `gettestmail-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gettestmail-1.0.0/gettestmail/client.py` & `gettestmail-1.0.1/gettestmail/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import requests
 from gettestmail.models import GetTestMail, Problem
 from typing import Optional
 
 
 class APIException(Exception):
     def __init__(self, problem: Problem):
```

### Comparing `gettestmail-1.0.0/setup.py` & `gettestmail-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gettestmail",
-    version="1.0.0",
+    version="1.0.1",
     author="Bobby Donchev",
     author_email="support@gettestmail.com",
     description="A Python client library for the GetTestMail API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gettestmail/python-sdk",
     packages=find_packages(),
```

