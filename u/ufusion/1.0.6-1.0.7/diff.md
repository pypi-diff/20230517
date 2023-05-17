# Comparing `tmp/ufusion-1.0.6.tar.gz` & `tmp/ufusion-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufusion-1.0.6.tar", last modified: Wed May 17 02:46:16 2023, max compression
+gzip compressed data, was "ufusion-1.0.7.tar", last modified: Wed May 17 02:49:47 2023, max compression
```

## Comparing `ufusion-1.0.6.tar` & `ufusion-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:46:16.614983 ufusion-1.0.6/
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:46:16.612596 ufusion-1.0.6/Fusion/
--rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 02:34:12.000000 ufusion-1.0.6/Fusion/Fusion.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:46:16.612802 ufusion-1.0.6/Fusion/Packages/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.0.6/Fusion/Packages/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     1938 2023-05-16 12:37:58.000000 ufusion-1.0.6/Fusion/Packages/packager.py
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.0.6/Fusion/__init__.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:46:16.613161 ufusion-1.0.6/Fusion/download/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:34:58.000000 ufusion-1.0.6/Fusion/download/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     2346 2023-05-16 11:52:47.000000 ufusion-1.0.6/Fusion/download/downloader.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:46:16.613497 ufusion-1.0.6/Fusion/ui/
--rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:48:11.000000 ufusion-1.0.6/Fusion/ui/__init__.py
--rw-r--r--   0 fostn.     (501) staff       (20)     3482 2023-05-16 12:54:54.000000 ufusion-1.0.6/Fusion/ui/menu.py
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:46:16.614807 ufusion-1.0.6/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 02:46:16.615044 ufusion-1.0.6/setup.cfg
--rw-r--r--   0 fostn.     (501) staff       (20)      371 2023-05-17 02:46:11.000000 ufusion-1.0.6/setup.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:46:16.614583 ufusion-1.0.6/ufusion.egg-info/
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:46:16.000000 ufusion-1.0.6/ufusion.egg-info/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)      386 2023-05-17 02:46:16.000000 ufusion-1.0.6/ufusion.egg-info/SOURCES.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:46:16.000000 ufusion-1.0.6/ufusion.egg-info/dependency_links.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 02:46:16.000000 ufusion-1.0.6/ufusion.egg-info/entry_points.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 02:46:16.000000 ufusion-1.0.6/ufusion.egg-info/requires.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 02:46:16.000000 ufusion-1.0.6/ufusion.egg-info/top_level.txt
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:49:47.503834 ufusion-1.0.7/
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:49:47.501433 ufusion-1.0.7/Fusion/
+-rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 02:34:12.000000 ufusion-1.0.7/Fusion/Fusion.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:49:47.501647 ufusion-1.0.7/Fusion/Packages/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.0.7/Fusion/Packages/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     1938 2023-05-16 12:37:58.000000 ufusion-1.0.7/Fusion/Packages/packager.py
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:35:02.000000 ufusion-1.0.7/Fusion/__init__.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:49:47.502086 ufusion-1.0.7/Fusion/download/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:34:58.000000 ufusion-1.0.7/Fusion/download/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     2346 2023-05-16 11:52:47.000000 ufusion-1.0.7/Fusion/download/downloader.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:49:47.502493 ufusion-1.0.7/Fusion/ui/
+-rw-r--r--   0 fostn.     (501) staff       (20)        0 2023-05-14 22:48:11.000000 ufusion-1.0.7/Fusion/ui/__init__.py
+-rw-r--r--   0 fostn.     (501) staff       (20)     3482 2023-05-16 12:54:54.000000 ufusion-1.0.7/Fusion/ui/menu.py
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:49:47.503676 ufusion-1.0.7/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 02:49:47.503895 ufusion-1.0.7/setup.cfg
+-rw-r--r--   0 fostn.     (501) staff       (20)      379 2023-05-17 02:49:44.000000 ufusion-1.0.7/setup.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:49:47.503466 ufusion-1.0.7/ufusion.egg-info/
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:49:47.000000 ufusion-1.0.7/ufusion.egg-info/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)      386 2023-05-17 02:49:47.000000 ufusion-1.0.7/ufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:49:47.000000 ufusion-1.0.7/ufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       54 2023-05-17 02:49:47.000000 ufusion-1.0.7/ufusion.egg-info/entry_points.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 02:49:47.000000 ufusion-1.0.7/ufusion.egg-info/requires.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 02:49:47.000000 ufusion-1.0.7/ufusion.egg-info/top_level.txt
```

### Comparing `ufusion-1.0.6/Fusion/Fusion.py` & `ufusion-1.0.7/Fusion/Fusion.py`

 * *Files identical despite different names*

### Comparing `ufusion-1.0.6/Fusion/Packages/packager.py` & `ufusion-1.0.7/Fusion/Packages/packager.py`

 * *Files identical despite different names*

### Comparing `ufusion-1.0.6/Fusion/download/downloader.py` & `ufusion-1.0.7/Fusion/download/downloader.py`

 * *Files identical despite different names*

### Comparing `ufusion-1.0.6/Fusion/ui/menu.py` & `ufusion-1.0.7/Fusion/ui/menu.py`

 * *Files identical despite different names*

