# Comparing `tmp/agsi-1.0.2.tar.gz` & `tmp/agsi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.0.2.tar", last modified: Wed May 17 09:25:16 2023, max compression
+gzip compressed data, was "agsi-1.0.3.tar", last modified: Wed May 17 09:28:46 2023, max compression
```

## Comparing `agsi-1.0.2.tar` & `agsi-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:25:16.378291 agsi-1.0.2/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       46 2023-05-17 09:19:08.000000 agsi-1.0.2/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-17 09:25:16.378291 agsi-1.0.2/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.2/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:25:16.378291 agsi-1.0.2/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.2/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:25:16.378291 agsi-1.0.2/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    12789 2023-05-17 09:25:00.000000 agsi-1.0.2/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.2/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.2/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.2/agsi/main.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:25:16.378291 agsi-1.0.2/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-17 09:25:16.000000 agsi-1.0.2/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      261 2023-05-17 09:25:16.000000 agsi-1.0.2/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 09:25:16.000000 agsi-1.0.2/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 09:25:16.000000 agsi-1.0.2/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-17 09:25:16.000000 agsi-1.0.2/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 09:25:16.378291 agsi-1.0.2/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-17 09:25:14.000000 agsi-1.0.2/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       46 2023-05-17 09:19:08.000000 agsi-1.0.3/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-17 09:28:46.762694 agsi-1.0.3/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.3/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.3/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    12758 2023-05-17 09:27:46.000000 agsi-1.0.3/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.3/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.3/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.3/agsi/main.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      261 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 09:28:46.762694 agsi-1.0.3/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-17 09:28:43.000000 agsi-1.0.3/setup.py
```

### Comparing `agsi-1.0.2/README.md` & `agsi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `agsi-1.0.2/agsi/data/FarmData.py` & `agsi-1.0.3/agsi/data/FarmData.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import geopandas as gpd
 import sys
 import os 
 import csv
 from descartes import PolygonPatch
 import copy
 import matplotlib as mpl
-from .utils import convert_pat
 
 from .utils import *
   
 class FarmData():
 
   """
     A utility class that provides access to farm data and related functionalities.
```

### Comparing `agsi-1.0.2/agsi/data/utils.py` & `agsi-1.0.3/agsi/data/utils.py`

 * *Files identical despite different names*

