# Comparing `tmp/ufusion-1.0.8.tar.gz` & `tmp/ufusion-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufusion-1.0.8.tar", last modified: Wed May 17 02:54:49 2023, max compression
+gzip compressed data, was "ufusion-1.1.0.tar", last modified: Wed May 17 03:02:37 2023, max compression
```

## Comparing `ufusion-1.0.8.tar` & `ufusion-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:54:49.601274 ufusion-1.0.8/
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:54:49.598815 ufusion-1.0.8/Fusion/
--rw-r--r--   0 fostn.     (501) staff       (20)     1032 2023-05-17 02:51:20.000000 ufusion-1.0.8/Fusion/Fusion.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:54:49.599034 ufusion-1.0.8/Fusion/Packages/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.0.8/Fusion/Packages/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     1938 2023-05-16 12:37:58.000000 ufusion-1.0.8/Fusion/Packages/packager.py
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.0.8/Fusion/__init__.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:54:49.599420 ufusion-1.0.8/Fusion/download/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:34:58.000000 ufusion-1.0.8/Fusion/download/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     2346 2023-05-16 11:52:47.000000 ufusion-1.0.8/Fusion/download/downloader.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:54:49.599850 ufusion-1.0.8/Fusion/ui/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:48:11.000000 ufusion-1.0.8/Fusion/ui/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     3482 2023-05-16 12:54:54.000000 ufusion-1.0.8/Fusion/ui/menu.py
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:54:49.601097 ufusion-1.0.8/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 02:54:49.601787 ufusion-1.0.8/setup.cfg
--rw-r--r--   0 fostn.     (501) staff       (20)      371 2023-05-17 02:54:45.000000 ufusion-1.0.8/setup.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:54:49.600879 ufusion-1.0.8/ufusion.egg-info/
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:54:49.000000 ufusion-1.0.8/ufusion.egg-info/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)      386 2023-05-17 02:54:49.000000 ufusion-1.0.8/ufusion.egg-info/SOURCES.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:54:49.000000 ufusion-1.0.8/ufusion.egg-info/dependency_links.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 02:54:49.000000 ufusion-1.0.8/ufusion.egg-info/entry_points.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 02:54:49.000000 ufusion-1.0.8/ufusion.egg-info/requires.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 02:54:49.000000 ufusion-1.0.8/ufusion.egg-info/top_level.txt
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:02:37.650800 ufusion-1.1.0/
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:02:37.648410 ufusion-1.1.0/Fusion/
+-rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 02:58:02.000000 ufusion-1.1.0/Fusion/Fusion.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:02:37.648677 ufusion-1.1.0/Fusion/Packages/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.1.0/Fusion/Packages/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     1938 2023-05-16 12:37:58.000000 ufusion-1.1.0/Fusion/Packages/packager.py
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.1.0/Fusion/__init__.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:02:37.649091 ufusion-1.1.0/Fusion/download/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:34:58.000000 ufusion-1.1.0/Fusion/download/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     2346 2023-05-16 11:52:47.000000 ufusion-1.1.0/Fusion/download/downloader.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:02:37.649418 ufusion-1.1.0/Fusion/ui/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:48:11.000000 ufusion-1.1.0/Fusion/ui/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     3482 2023-05-16 12:54:54.000000 ufusion-1.1.0/Fusion/ui/menu.py
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 03:02:37.650628 ufusion-1.1.0/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 03:02:37.650861 ufusion-1.1.0/setup.cfg
+-rw-r--r--   0 fostn.     (501) staff       (20)      417 2023-05-17 03:02:29.000000 ufusion-1.1.0/setup.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:02:37.650412 ufusion-1.1.0/ufusion.egg-info/
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 03:02:37.000000 ufusion-1.1.0/ufusion.egg-info/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)      386 2023-05-17 03:02:37.000000 ufusion-1.1.0/ufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 03:02:37.000000 ufusion-1.1.0/ufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 03:02:37.000000 ufusion-1.1.0/ufusion.egg-info/entry_points.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 03:02:37.000000 ufusion-1.1.0/ufusion.egg-info/requires.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 03:02:37.000000 ufusion-1.1.0/ufusion.egg-info/top_level.txt
```

### Comparing `ufusion-1.0.8/Fusion/Fusion.py` & `ufusion-1.1.0/Fusion/Fusion.py`

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

### Comparing `ufusion-1.0.8/Fusion/Packages/packager.py` & `ufusion-1.1.0/Fusion/Packages/packager.py`

 * *Files identical despite different names*

### Comparing `ufusion-1.0.8/Fusion/download/downloader.py` & `ufusion-1.1.0/Fusion/download/downloader.py`

 * *Files identical despite different names*

### Comparing `ufusion-1.0.8/Fusion/ui/menu.py` & `ufusion-1.1.0/Fusion/ui/menu.py`

 * *Files identical despite different names*

