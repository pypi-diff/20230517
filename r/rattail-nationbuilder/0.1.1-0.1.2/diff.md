# Comparing `tmp/rattail-nationbuilder-0.1.1.tar.gz` & `tmp/rattail-nationbuilder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/rattail-nationbuilder/dist/.tmp-7o5gr9q5/rattail-nationbuilder-0.1.1.tar", last modified: Thu May 11 20:25:42 2023, max compression
+gzip compressed data, was "/home/lance/src/rattail-nationbuilder/dist/.tmp-qbjl5toy/rattail-nationbuilder-0.1.2.tar", last modified: Wed May 17 12:02:10 2023, max compression
```

## Comparing `rattail-nationbuilder-0.1.1.tar` & `rattail-nationbuilder-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/
--rw-r--r--   0 lance     (1000) lance     (1000)      484 2023-05-11 20:25:13.000000 rattail-nationbuilder-0.1.1/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.1/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.1/README.md
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-11 20:25:19.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4578 2023-05-09 23:33:43.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/webapi.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      429 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     2268 2023-05-05 19:43:42.000000 rattail-nationbuilder-0.1.1/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/
+-rw-r--r--   0 lance     (1000) lance     (1000)      569 2023-05-17 12:01:36.000000 rattail-nationbuilder-0.1.2/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.2/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.2/README.md
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-17 12:01:39.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4578 2023-05-09 23:33:43.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/webapi.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      439 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      794 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1017 2023-05-17 12:01:08.000000 rattail-nationbuilder-0.1.2/setup.py
```

### Comparing `rattail-nationbuilder-0.1.1/PKG-INFO` & `rattail-nationbuilder-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.1
+Version: 0.1.2
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-nationbuilder-0.1.1/rattail_nationbuilder/__init__.py` & `rattail-nationbuilder-0.1.2/rattail_nationbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/webapi.py` & `rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/webapi.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/PKG-INFO` & `rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.1
+Version: 0.1.2
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

