# Comparing `tmp/collecting_faces-0.0.1.tar.gz` & `tmp/collecting_faces-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collecting_faces-0.0.1.tar", last modified: Wed May 17 08:42:33 2023, max compression
+gzip compressed data, was "dist/collecting_faces-1.0.0.tar", last modified: Wed May 17 08:42:33 2023, max compression
```

## Comparing `collecting_faces-0.0.1.tar` & `collecting_faces-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/
--rw-rw-r--   0 hail      (1000) hail      (1000)        0 2023-05-17 03:12:16.000000 collecting_faces-0.0.1/LICENSE
--rw-rw-r--   0 hail      (1000) hail      (1000)      518 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/PKG-INFO
--rw-rw-r--   0 hail      (1000) hail      (1000)       38 2023-05-17 03:23:25.000000 collecting_faces-0.0.1/README.md
-drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/collecting_faces/
--rw-rw-r--   0 hail      (1000) hail      (1000)        0 2023-05-17 08:31:17.000000 collecting_faces-0.0.1/collecting_faces/__init__.py
--rw-rw-r--   0 hail      (1000) hail      (1000)     2016 2023-05-17 08:41:48.000000 collecting_faces-0.0.1/collecting_faces/collect_faces.py
-drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/collecting_faces/preprocess/
--rw-rw-r--   0 hail      (1000) hail      (1000)        0 2023-05-16 14:03:13.000000 collecting_faces-0.0.1/collecting_faces/preprocess/__init__.py
--rwxrwxr-x   0 hail      (1000) hail      (1000)     3115 2023-05-17 08:30:32.000000 collecting_faces-0.0.1/collecting_faces/preprocess/align_images.py
--rw-rw-r--   0 hail      (1000) hail      (1000)     4532 2023-05-16 14:03:13.000000 collecting_faces-0.0.1/collecting_faces/preprocess/face_alignment.py
--rw-rw-r--   0 hail      (1000) hail      (1000)      894 2023-05-16 14:03:13.000000 collecting_faces-0.0.1/collecting_faces/preprocess/landmarks_detector.py
--rw-rw-r--   0 hail      (1000) hail      (1000)      185 2023-05-17 08:41:48.000000 collecting_faces-0.0.1/collecting_faces/preprocess/unpack_bz2.py
-drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/collecting_faces.egg-info/
--rw-rw-r--   0 hail      (1000) hail      (1000)      518 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/collecting_faces.egg-info/PKG-INFO
--rw-rw-r--   0 hail      (1000) hail      (1000)      471 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/collecting_faces.egg-info/SOURCES.txt
--rw-rw-r--   0 hail      (1000) hail      (1000)        1 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/collecting_faces.egg-info/dependency_links.txt
--rw-rw-r--   0 hail      (1000) hail      (1000)       17 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/collecting_faces.egg-info/top_level.txt
--rw-rw-r--   0 hail      (1000) hail      (1000)       38 2023-05-17 08:42:33.000000 collecting_faces-0.0.1/setup.cfg
--rw-rw-r--   0 hail      (1000) hail      (1000)     1343 2023-05-17 08:28:07.000000 collecting_faces-0.0.1/setup.py
+drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/
+-rw-rw-r--   0 hail      (1000) hail      (1000)        0 2023-05-17 03:12:16.000000 collecting_faces-1.0.0/LICENSE
+-rw-rw-r--   0 hail      (1000) hail      (1000)      372 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/PKG-INFO
+-rw-rw-r--   0 hail      (1000) hail      (1000)       38 2023-05-17 03:23:25.000000 collecting_faces-1.0.0/README.md
+drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces/
+-rw-rw-r--   0 hail      (1000) hail      (1000)        0 2023-05-17 08:31:17.000000 collecting_faces-1.0.0/collecting_faces/__init__.py
+-rw-rw-r--   0 hail      (1000) hail      (1000)     2016 2023-05-17 08:41:48.000000 collecting_faces-1.0.0/collecting_faces/collect_faces.py
+drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces/preprocess/
+-rw-rw-r--   0 hail      (1000) hail      (1000)        0 2023-05-16 14:03:13.000000 collecting_faces-1.0.0/collecting_faces/preprocess/__init__.py
+-rwxrwxr-x   0 hail      (1000) hail      (1000)     3115 2023-05-17 08:30:32.000000 collecting_faces-1.0.0/collecting_faces/preprocess/align_images.py
+-rw-rw-r--   0 hail      (1000) hail      (1000)     4532 2023-05-16 14:03:13.000000 collecting_faces-1.0.0/collecting_faces/preprocess/face_alignment.py
+-rw-rw-r--   0 hail      (1000) hail      (1000)      894 2023-05-16 14:03:13.000000 collecting_faces-1.0.0/collecting_faces/preprocess/landmarks_detector.py
+-rw-rw-r--   0 hail      (1000) hail      (1000)      185 2023-05-17 08:41:48.000000 collecting_faces-1.0.0/collecting_faces/preprocess/unpack_bz2.py
+drwxrwxr-x   0 hail      (1000) hail      (1000)        0 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces.egg-info/
+-rw-rw-r--   0 hail      (1000) hail      (1000)      372 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces.egg-info/PKG-INFO
+-rw-rw-r--   0 hail      (1000) hail      (1000)      549 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces.egg-info/SOURCES.txt
+-rw-rw-r--   0 hail      (1000) hail      (1000)        1 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces.egg-info/dependency_links.txt
+-rw-rw-r--   0 hail      (1000) hail      (1000)        1 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces.egg-info/not-zip-safe
+-rw-rw-r--   0 hail      (1000) hail      (1000)       43 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces.egg-info/requires.txt
+-rw-rw-r--   0 hail      (1000) hail      (1000)       17 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/collecting_faces.egg-info/top_level.txt
+-rw-rw-r--   0 hail      (1000) hail      (1000)       38 2023-05-17 08:42:33.000000 collecting_faces-1.0.0/setup.cfg
+-rw-rw-r--   0 hail      (1000) hail      (1000)     1343 2023-05-17 08:28:07.000000 collecting_faces-1.0.0/setup.py
```

### Comparing `collecting_faces-0.0.1/collecting_faces/collect_faces.py` & `collecting_faces-1.0.0/collecting_faces/collect_faces.py`

 * *Files identical despite different names*

### Comparing `collecting_faces-0.0.1/collecting_faces/preprocess/align_images.py` & `collecting_faces-1.0.0/collecting_faces/preprocess/align_images.py`

 * *Files identical despite different names*

### Comparing `collecting_faces-0.0.1/collecting_faces/preprocess/face_alignment.py` & `collecting_faces-1.0.0/collecting_faces/preprocess/face_alignment.py`

 * *Files identical despite different names*

### Comparing `collecting_faces-0.0.1/collecting_faces/preprocess/landmarks_detector.py` & `collecting_faces-1.0.0/collecting_faces/preprocess/landmarks_detector.py`

 * *Files identical despite different names*

### Comparing `collecting_faces-0.0.1/setup.py` & `collecting_faces-1.0.0/setup.py`

 * *Files identical despite different names*

