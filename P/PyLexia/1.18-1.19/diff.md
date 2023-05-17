# Comparing `tmp/PyLexia-1.18.tar.gz` & `tmp/PyLexia-1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLexia-1.18.tar", last modified: Wed May 17 09:58:17 2023, max compression
+gzip compressed data, was "PyLexia-1.19.tar", last modified: Wed May 17 11:36:28 2023, max compression
```

## Comparing `PyLexia-1.18.tar` & `PyLexia-1.19.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 09:58:17.803846 PyLexia-1.18/PKG-INFO
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/PyLexia/
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/PyLexia/PyLexia.egg-info/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 09:58:17.000000 PyLexia-1.18/PyLexia/PyLexia.egg-info/PKG-INFO
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      352 2023-05-17 09:58:17.000000 PyLexia-1.18/PyLexia/PyLexia.egg-info/SOURCES.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 09:58:17.000000 PyLexia-1.18/PyLexia/PyLexia.egg-info/dependency_links.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       81 2023-05-17 09:58:17.000000 PyLexia-1.18/PyLexia/PyLexia.egg-info/top_level.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.18/PyLexia/__init__.py
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/PyLexia/experimentals/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       59 2023-05-17 07:51:12.000000 PyLexia-1.18/PyLexia/experimentals/experimental1.py
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/PyLexia/inference/
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/PyLexia/inference/models/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:58:55.000000 PyLexia-1.18/PyLexia/inference/models/__init__.py
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      592 2023-05-16 14:22:15.000000 PyLexia-1.18/PyLexia/inference/models/cni.py
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/PyLexia/learning/
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:58:17.803846 PyLexia-1.18/PyLexia/learning/models/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)     2804 2023-05-16 14:10:09.000000 PyLexia-1.18/PyLexia/learning/models/cni.py
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.18/PyLexia/pylexia.py
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.18/README.md
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 09:58:17.803846 PyLexia-1.18/setup.cfg
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      243 2023-05-17 09:57:30.000000 PyLexia-1.18/setup.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 11:36:28.071118 PyLexia-1.19/PKG-INFO
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/PyLexia/
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/PyLexia/PyLexia.egg-info/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 11:36:28.000000 PyLexia-1.19/PyLexia/PyLexia.egg-info/PKG-INFO
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      390 2023-05-17 11:36:28.000000 PyLexia-1.19/PyLexia/PyLexia.egg-info/SOURCES.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 11:36:28.000000 PyLexia-1.19/PyLexia/PyLexia.egg-info/dependency_links.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      117 2023-05-17 11:36:28.000000 PyLexia-1.19/PyLexia/PyLexia.egg-info/requires.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       81 2023-05-17 11:36:28.000000 PyLexia-1.19/PyLexia/PyLexia.egg-info/top_level.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.19/PyLexia/__init__.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/PyLexia/experimentals/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       59 2023-05-17 07:51:12.000000 PyLexia-1.19/PyLexia/experimentals/experimental1.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/PyLexia/inference/
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/PyLexia/inference/models/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:58:55.000000 PyLexia-1.19/PyLexia/inference/models/__init__.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      592 2023-05-16 14:22:15.000000 PyLexia-1.19/PyLexia/inference/models/cni.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/PyLexia/learning/
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 11:36:28.071118 PyLexia-1.19/PyLexia/learning/models/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)     2804 2023-05-16 14:10:09.000000 PyLexia-1.19/PyLexia/learning/models/cni.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.19/PyLexia/pylexia.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.19/README.md
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 11:36:28.071118 PyLexia-1.19/setup.cfg
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      511 2023-05-17 11:36:11.000000 PyLexia-1.19/setup.py
```

### Comparing `PyLexia-1.18/PyLexia/inference/models/cni.py` & `PyLexia-1.19/PyLexia/inference/models/cni.py`

 * *Files identical despite different names*

### Comparing `PyLexia-1.18/PyLexia/learning/models/cni.py` & `PyLexia-1.19/PyLexia/learning/models/cni.py`

 * *Files identical despite different names*

