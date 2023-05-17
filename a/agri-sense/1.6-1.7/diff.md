# Comparing `tmp/agri_sense-1.6.tar.gz` & `tmp/agri_sense-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agri_sense-1.6.tar", last modified: Wed May 17 08:40:41 2023, max compression
+gzip compressed data, was "agri_sense-1.7.tar", last modified: Wed May 17 08:44:32 2023, max compression
```

## Comparing `agri_sense-1.6.tar` & `agri_sense-1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:40:41.793759 agri_sense-1.6/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.6/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:40:41.793759 agri_sense-1.6/PKG-INFO
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:40:41.793759 agri_sense-1.6/agri_sense/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 08:40:18.000000 agri_sense-1.6/agri_sense/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:40:41.793759 agri_sense-1.6/agri_sense/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    12691 2023-05-17 07:35:55.000000 agri_sense-1.6/agri_sense/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:10:02.000000 agri_sense-1.6/agri_sense/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5760 2023-05-16 08:13:32.000000 agri_sense-1.6/agri_sense/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.6/agri_sense/main.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:40:41.793759 agri_sense-1.6/agri_sense.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:40:41.000000 agri_sense-1.6/agri_sense.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      328 2023-05-17 08:40:41.000000 agri_sense-1.6/agri_sense.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 08:40:41.000000 agri_sense-1.6/agri_sense.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 08:40:41.000000 agri_sense-1.6/agri_sense.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 08:40:41.000000 agri_sense-1.6/agri_sense.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 08:09:59.000000 agri_sense-1.6/requirements.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 08:40:41.793759 agri_sense-1.6/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      373 2023-05-17 08:40:34.000000 agri_sense-1.6/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:44:32.359736 agri_sense-1.7/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.7/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:44:32.355736 agri_sense-1.7/PKG-INFO
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:44:32.355736 agri_sense-1.7/agri_sense/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 08:40:18.000000 agri_sense-1.7/agri_sense/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:44:32.355736 agri_sense-1.7/agri_sense/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    12640 2023-05-17 08:44:16.000000 agri_sense-1.7/agri_sense/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:10:02.000000 agri_sense-1.7/agri_sense/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5760 2023-05-16 08:13:32.000000 agri_sense-1.7/agri_sense/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.7/agri_sense/main.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:44:32.355736 agri_sense-1.7/agri_sense.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:44:32.000000 agri_sense-1.7/agri_sense.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      328 2023-05-17 08:44:32.000000 agri_sense-1.7/agri_sense.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 08:44:32.000000 agri_sense-1.7/agri_sense.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 08:44:32.000000 agri_sense-1.7/agri_sense.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 08:44:32.000000 agri_sense-1.7/agri_sense.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 08:09:59.000000 agri_sense-1.7/requirements.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 08:44:32.359736 agri_sense-1.7/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      373 2023-05-17 08:44:26.000000 agri_sense-1.7/setup.py
```

### Comparing `agri_sense-1.6/agri_sense/data/FarmData.py` & `agri_sense-1.7/agri_sense/data/FarmData.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 import geopandas as gpd
 import sys
 import os 
 import csv
 from descartes import PolygonPatch
 import copy
 import matplotlib as mpl
-
-sys.path.append(os.path.realpath(__file__))
-
-from data.utils import *
+from utils import *
   
 class FarmData():
 
   """
     A utility class that provides access to farm data and related functionalities.
 
     Attributes:
```

### Comparing `agri_sense-1.6/agri_sense/data/utils.py` & `agri_sense-1.7/agri_sense/data/utils.py`

 * *Files identical despite different names*

