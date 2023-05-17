# Comparing `tmp/ufusion-1.0.3.tar.gz` & `tmp/ufusion-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufusion-1.0.3.tar", last modified: Wed May 17 02:28:42 2023, max compression
+gzip compressed data, was "ufusion-1.0.4.tar", last modified: Wed May 17 02:35:53 2023, max compression
```

## Comparing `ufusion-1.0.3.tar` & `ufusion-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:28:42.535633 ufusion-1.0.3/
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:28:42.534416 ufusion-1.0.3/Fusion/
--rw-r--r--   0 fostn.     (501) staff       (20)     1011 2023-05-17 01:57:45.000000 ufusion-1.0.3/Fusion/Fusion.py
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:28:42.535482 ufusion-1.0.3/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 02:28:42.535688 ufusion-1.0.3/setup.cfg
--rw-r--r--   0 fostn.     (501) staff       (20)      371 2023-05-17 02:28:36.000000 ufusion-1.0.3/setup.py
-drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:28:42.535297 ufusion-1.0.3/ufusion.egg-info/
--rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:28:42.000000 ufusion-1.0.3/ufusion.egg-info/PKG-INFO
--rw-r--r--   0 fostn.     (501) staff       (20)      213 2023-05-17 02:28:42.000000 ufusion-1.0.3/ufusion.egg-info/SOURCES.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:28:42.000000 ufusion-1.0.3/ufusion.egg-info/dependency_links.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       46 2023-05-17 02:28:42.000000 ufusion-1.0.3/ufusion.egg-info/entry_points.txt
--rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 02:28:42.000000 ufusion-1.0.3/ufusion.egg-info/requires.txt
--rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:28:42.000000 ufusion-1.0.3/ufusion.egg-info/top_level.txt
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:35:53.217597 ufusion-1.0.4/
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:35:53.217441 ufusion-1.0.4/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)       38 2023-05-17 02:35:53.217653 ufusion-1.0.4/setup.cfg
+-rw-r--r--   0 fostn.     (501) staff       (20)      364 2023-05-17 02:35:47.000000 ufusion-1.0.4/setup.py
+drwxr-xr-x   0 fostn.     (501) staff       (20)        0 2023-05-17 02:35:53.217252 ufusion-1.0.4/ufusion.egg-info/
+-rw-r--r--   0 fostn.     (501) staff       (20)      164 2023-05-17 02:35:52.000000 ufusion-1.0.4/ufusion.egg-info/PKG-INFO
+-rw-r--r--   0 fostn.     (501) staff       (20)      196 2023-05-17 02:35:53.000000 ufusion-1.0.4/ufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:35:52.000000 ufusion-1.0.4/ufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       39 2023-05-17 02:35:53.000000 ufusion-1.0.4/ufusion.egg-info/entry_points.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)       26 2023-05-17 02:35:53.000000 ufusion-1.0.4/ufusion.egg-info/requires.txt
+-rw-r--r--   0 fostn.     (501) staff       (20)        1 2023-05-17 02:35:53.000000 ufusion-1.0.4/ufusion.egg-info/top_level.txt
```

