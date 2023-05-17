# Comparing `tmp/flattenpy-0.1.tar.gz` & `tmp/flattenpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/iovcharenko/work/intetics/firemap/codebase/flattenpy/dist/.tmp-ikdfhtgf/flattenpy-0.1.tar", last modified: Wed May 17 14:12:17 2023, max compression
+gzip compressed data, was "/Users/iovcharenko/work/intetics/firemap/codebase/flattenpy/dist/.tmp-dyz6zmxn/flattenpy-0.2.tar", last modified: Wed May 17 14:59:56 2023, max compression
```

## Comparing `flattenpy-0.1.tar` & `flattenpy-0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 iovcharenko   (502) staff       (20)        0 2023-05-17 14:12:17.000000 flattenpy-0.1/
--rw-r--r--   0 iovcharenko   (502) staff       (20)      192 2023-05-17 14:12:17.000000 flattenpy-0.1/PKG-INFO
-drwxr-xr-x   0 iovcharenko   (502) staff       (20)        0 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy/
--rw-r--r--   0 iovcharenko   (502) staff       (20)     6709 2023-05-17 13:59:35.000000 flattenpy-0.1/flattenpy/__init__.py
--rw-r--r--   0 iovcharenko   (502) staff       (20)       33 2023-05-17 13:58:53.000000 flattenpy-0.1/flattenpy/__main__.py
-drwxr-xr-x   0 iovcharenko   (502) staff       (20)        0 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy.egg-info/
--rw-r--r--   0 iovcharenko   (502) staff       (20)      192 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy.egg-info/PKG-INFO
--rw-r--r--   0 iovcharenko   (502) staff       (20)      252 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy.egg-info/SOURCES.txt
--rw-r--r--   0 iovcharenko   (502) staff       (20)        1 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy.egg-info/dependency_links.txt
--rw-r--r--   0 iovcharenko   (502) staff       (20)       44 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy.egg-info/entry_points.txt
--rw-r--r--   0 iovcharenko   (502) staff       (20)       48 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy.egg-info/requires.txt
--rw-r--r--   0 iovcharenko   (502) staff       (20)       10 2023-05-17 14:12:17.000000 flattenpy-0.1/flattenpy.egg-info/top_level.txt
--rw-r--r--   0 iovcharenko   (502) staff       (20)       38 2023-05-17 14:12:17.000000 flattenpy-0.1/setup.cfg
--rw-r--r--   0 iovcharenko   (502) staff       (20)      543 2023-05-17 13:51:01.000000 flattenpy-0.1/setup.py
+drwxr-xr-x   0 iovcharenko   (502) staff       (20)        0 2023-05-17 14:59:56.000000 flattenpy-0.2/
+-rw-r--r--   0 iovcharenko   (502) staff       (20)       30 2023-05-17 14:56:33.000000 flattenpy-0.2/MANIFEST.in
+-rw-r--r--   0 iovcharenko   (502) staff       (20)      192 2023-05-17 14:59:56.000000 flattenpy-0.2/PKG-INFO
+drwxr-xr-x   0 iovcharenko   (502) staff       (20)        0 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy/
+-rw-r--r--   0 iovcharenko   (502) staff       (20)     6709 2023-05-17 13:59:35.000000 flattenpy-0.2/flattenpy/__init__.py
+-rw-r--r--   0 iovcharenko   (502) staff       (20)       33 2023-05-17 13:58:53.000000 flattenpy-0.2/flattenpy/__main__.py
+drwxr-xr-x   0 iovcharenko   (502) staff       (20)        0 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy.egg-info/
+-rw-r--r--   0 iovcharenko   (502) staff       (20)      192 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy.egg-info/PKG-INFO
+-rw-r--r--   0 iovcharenko   (502) staff       (20)      291 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 iovcharenko   (502) staff       (20)        1 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 iovcharenko   (502) staff       (20)       44 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy.egg-info/entry_points.txt
+-rw-r--r--   0 iovcharenko   (502) staff       (20)       48 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy.egg-info/requires.txt
+-rw-r--r--   0 iovcharenko   (502) staff       (20)       10 2023-05-17 14:59:56.000000 flattenpy-0.2/flattenpy.egg-info/top_level.txt
+-rw-r--r--   0 iovcharenko   (502) staff       (20)        0 2023-05-17 13:03:57.000000 flattenpy-0.2/readme.md
+-rw-r--r--   0 iovcharenko   (502) staff       (20)       48 2023-05-17 13:16:09.000000 flattenpy-0.2/requirements.txt
+-rw-r--r--   0 iovcharenko   (502) staff       (20)       38 2023-05-17 14:59:56.000000 flattenpy-0.2/setup.cfg
+-rw-r--r--   0 iovcharenko   (502) staff       (20)      543 2023-05-17 14:58:24.000000 flattenpy-0.2/setup.py
```

### Comparing `flattenpy-0.1/flattenpy/__init__.py` & `flattenpy-0.2/flattenpy/__init__.py`

 * *Files identical despite different names*

### Comparing `flattenpy-0.1/setup.py` & `flattenpy-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = 0.1
+version = 0.2
 
 try:
     with open("requirements.txt", "r") as f:
         required = f.read().split("\n")
 except FileNotFoundError:
     required = []
```

