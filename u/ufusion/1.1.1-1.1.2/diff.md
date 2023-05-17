# Comparing `tmp/ufusion-1.1.1.tar.gz` & `tmp/ufusion-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufusion-1.1.1.tar", last modified: Wed May 17 03:06:01 2023, max compression
+gzip compressed data, was "ufusion-1.1.2.tar", last modified: Wed May 17 03:08:23 2023, max compression
```

## Comparing `ufusion-1.1.1.tar` & `ufusion-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:06:01.202577 ufusion-1.1.1/
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:06:01.200159 ufusion-1.1.1/Fusion/
--rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 02:58:02.000000 ufusion-1.1.1/Fusion/Fusion.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:06:01.200403 ufusion-1.1.1/Fusion/Packages/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.1.1/Fusion/Packages/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     1940 2023-05-17 03:05:37.000000 ufusion-1.1.1/Fusion/Packages/packager.py
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.1.1/Fusion/__init__.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:06:01.200824 ufusion-1.1.1/Fusion/download/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:34:58.000000 ufusion-1.1.1/Fusion/download/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     2348 2023-05-17 03:05:30.000000 ufusion-1.1.1/Fusion/download/downloader.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:06:01.201170 ufusion-1.1.1/Fusion/ui/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:48:11.000000 ufusion-1.1.1/Fusion/ui/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     3482 2023-05-16 12:54:54.000000 ufusion-1.1.1/Fusion/ui/menu.py
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 03:06:01.202343 ufusion-1.1.1/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 03:06:01.202639 ufusion-1.1.1/setup.cfg
--rw-r--r--   0 fostn.     (501) staff       (20)      417 2023-05-17 03:05:45.000000 ufusion-1.1.1/setup.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:06:01.202123 ufusion-1.1.1/ufusion.egg-info/
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 03:06:00.000000 ufusion-1.1.1/ufusion.egg-info/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)      386 2023-05-17 03:06:01.000000 ufusion-1.1.1/ufusion.egg-info/SOURCES.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 03:06:00.000000 ufusion-1.1.1/ufusion.egg-info/dependency_links.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 03:06:00.000000 ufusion-1.1.1/ufusion.egg-info/entry_points.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 03:06:01.000000 ufusion-1.1.1/ufusion.egg-info/requires.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 03:06:01.000000 ufusion-1.1.1/ufusion.egg-info/top_level.txt
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:08:23.052074 ufusion-1.1.2/
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:08:23.048683 ufusion-1.1.2/Fusion/
+-rw-r--r--   0 fostn.     (501) staff       (20)     1014 2023-05-17 03:08:00.000000 ufusion-1.1.2/Fusion/Fusion.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:08:23.048896 ufusion-1.1.2/Fusion/Packages/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.1.2/Fusion/Packages/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     1940 2023-05-17 03:05:37.000000 ufusion-1.1.2/Fusion/Packages/packager.py
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.1.2/Fusion/__init__.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:08:23.049268 ufusion-1.1.2/Fusion/download/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:34:58.000000 ufusion-1.1.2/Fusion/download/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     2348 2023-05-17 03:05:30.000000 ufusion-1.1.2/Fusion/download/downloader.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:08:23.050442 ufusion-1.1.2/Fusion/ui/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:48:11.000000 ufusion-1.1.2/Fusion/ui/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     3482 2023-05-16 12:54:54.000000 ufusion-1.1.2/Fusion/ui/menu.py
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 03:08:23.051884 ufusion-1.1.2/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 03:08:23.052136 ufusion-1.1.2/setup.cfg
+-rw-r--r--   0 fostn.     (501) staff       (20)      417 2023-05-17 03:08:08.000000 ufusion-1.1.2/setup.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 03:08:23.051575 ufusion-1.1.2/ufusion.egg-info/
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 03:08:22.000000 ufusion-1.1.2/ufusion.egg-info/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)      386 2023-05-17 03:08:23.000000 ufusion-1.1.2/ufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 03:08:22.000000 ufusion-1.1.2/ufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 03:08:22.000000 ufusion-1.1.2/ufusion.egg-info/entry_points.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 03:08:22.000000 ufusion-1.1.2/ufusion.egg-info/requires.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 03:08:22.000000 ufusion-1.1.2/ufusion.egg-info/top_level.txt
```

### Comparing `ufusion-1.1.1/Fusion/Fusion.py` & `ufusion-1.1.2/Fusion/Fusion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ui.menu import Menu
-from download.downloader import Downloader
-from Packages.packager import Packager
+from .ui.menu import Menu
+from .download.downloader import Downloader
+from .Packages.packager import Packager
 import json
 class Fusion:
     def __init__(self):
         version = self.get_version()
         logo = f"""
        ______           _                
       / ____/_  _______(_)___  ____
```

### Comparing `ufusion-1.1.1/Fusion/Packages/packager.py` & `ufusion-1.1.2/Fusion/Packages/packager.py`

 * *Files identical despite different names*

### Comparing `ufusion-1.1.1/Fusion/download/downloader.py` & `ufusion-1.1.2/Fusion/download/downloader.py`

 * *Files identical despite different names*

### Comparing `ufusion-1.1.1/Fusion/ui/menu.py` & `ufusion-1.1.2/Fusion/ui/menu.py`

 * *Files identical despite different names*

