# Comparing `tmp/ufusion-1.0.0.tar.gz` & `tmp/ufusion-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufusion-1.0.0.tar", last modified: Wed May 17 01:50:46 2023, max compression
+gzip compressed data, was "ufusion-1.0.1.tar", last modified: Wed May 17 02:09:38 2023, max compression
```

## Comparing `ufusion-1.0.0.tar` & `ufusion-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:50:46.538072 ufusion-1.0.0/
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:50:46.536878 ufusion-1.0.0/Fusion/
--rw-r--r--   0 fostn.     (501) staff       (20)     1032 2023-05-17 01:22:47.000000 ufusion-1.0.0/Fusion/Fusion.py
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 01:50:46.537919 ufusion-1.0.0/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 01:50:46.538130 ufusion-1.0.0/setup.cfg
--rw-r--r--   0 fostn.     (501) staff       (20)      351 2023-05-17 01:49:08.000000 ufusion-1.0.0/setup.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:50:46.537734 ufusion-1.0.0/ufusion.egg-info/
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 01:50:46.000000 ufusion-1.0.0/ufusion.egg-info/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)      213 2023-05-17 01:50:46.000000 ufusion-1.0.0/ufusion.egg-info/SOURCES.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 01:50:46.000000 ufusion-1.0.0/ufusion.egg-info/dependency_links.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 01:50:46.000000 ufusion-1.0.0/ufusion.egg-info/entry_points.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 01:50:46.000000 ufusion-1.0.0/ufusion.egg-info/requires.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 01:50:46.000000 ufusion-1.0.0/ufusion.egg-info/top_level.txt
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:09:38.858451 ufusion-1.0.1/
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:09:38.857236 ufusion-1.0.1/Fusion/
+-rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 01:57:45.000000 ufusion-1.0.1/Fusion/Fusion.py
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:09:38.858299 ufusion-1.0.1/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 02:09:38.858505 ufusion-1.0.1/setup.cfg
+-rw-r--r--   0 fostn.     (501) staff       (20)      371 2023-05-17 02:09:20.000000 ufusion-1.0.1/setup.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:09:38.858113 ufusion-1.0.1/ufusion.egg-info/
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:09:38.000000 ufusion-1.0.1/ufusion.egg-info/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)      213 2023-05-17 02:09:38.000000 ufusion-1.0.1/ufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:09:38.000000 ufusion-1.0.1/ufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 02:09:38.000000 ufusion-1.0.1/ufusion.egg-info/entry_points.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 02:09:38.000000 ufusion-1.0.1/ufusion.egg-info/requires.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:09:38.000000 ufusion-1.0.1/ufusion.egg-info/top_level.txt
```

### Comparing `ufusion-1.0.0/Fusion/Fusion.py` & `ufusion-1.0.1/Fusion/Fusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from Fusion.ui.menu import Menu
-from Fusion.download.downloader import Downloader
-from Fusion.Packages.packager import Packager
+from ui.menu import Menu
+from download.downloader import Downloader
+from Packages.packager import Packager
 import json
 class Fusion:
     def __init__(self):
         version = self.get_version()
         logo = f"""
        ______           _                
       / ____/_  _______(_)___  ____
```

