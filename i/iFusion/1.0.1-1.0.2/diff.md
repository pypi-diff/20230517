# Comparing `tmp/iFusion-1.0.1.tar.gz` & `tmp/iFusion-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iFusion-1.0.1.tar", last modified: Wed May 17 01:16:04 2023, max compression
+gzip compressed data, was "iFusion-1.0.2.tar", last modified: Wed May 17 01:19:23 2023, max compression
```

## Comparing `iFusion-1.0.1.tar` & `iFusion-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:16:04.307498 iFusion-1.0.1/
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:16:04.306293 iFusion-1.0.1/Fusion/
--rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 00:45:33.000000 iFusion-1.0.1/Fusion/Fusion.py
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 01:16:04.307350 iFusion-1.0.1/PKG-INFO
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:16:04.307167 iFusion-1.0.1/iFusion.egg-info/
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 01:16:03.000000 iFusion-1.0.1/iFusion.egg-info/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)      213 2023-05-17 01:16:04.000000 iFusion-1.0.1/iFusion.egg-info/SOURCES.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 01:16:03.000000 iFusion-1.0.1/iFusion.egg-info/dependency_links.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 01:16:04.000000 iFusion-1.0.1/iFusion.egg-info/entry_points.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 01:16:04.000000 iFusion-1.0.1/iFusion.egg-info/requires.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 01:16:04.000000 iFusion-1.0.1/iFusion.egg-info/top_level.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 01:16:04.307554 iFusion-1.0.1/setup.cfg
--rw-r--r--   0 fostn.     (501) staff       (20)      351 2023-05-17 01:15:55.000000 iFusion-1.0.1/setup.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:19:23.911549 iFusion-1.0.2/
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:19:23.910307 iFusion-1.0.2/Fusion/
+-rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 00:45:33.000000 iFusion-1.0.2/Fusion/Fusion.py
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 01:19:23.911400 iFusion-1.0.2/PKG-INFO
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 01:19:23.911198 iFusion-1.0.2/iFusion.egg-info/
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 01:19:23.000000 iFusion-1.0.2/iFusion.egg-info/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)      213 2023-05-17 01:19:23.000000 iFusion-1.0.2/iFusion.egg-info/SOURCES.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 01:19:23.000000 iFusion-1.0.2/iFusion.egg-info/dependency_links.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 01:19:23.000000 iFusion-1.0.2/iFusion.egg-info/entry_points.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 01:19:23.000000 iFusion-1.0.2/iFusion.egg-info/requires.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        7 2023-05-17 01:19:23.000000 iFusion-1.0.2/iFusion.egg-info/top_level.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 01:19:23.911609 iFusion-1.0.2/setup.cfg
+-rw-r--r--   0 fostn.     (501) staff       (20)      351 2023-05-17 01:19:07.000000 iFusion-1.0.2/setup.py
```

### Comparing `iFusion-1.0.1/Fusion/Fusion.py` & `iFusion-1.0.2/Fusion/Fusion.py`

 * *Files identical despite different names*

