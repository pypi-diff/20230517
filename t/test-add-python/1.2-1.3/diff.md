# Comparing `tmp/test_add_python-1.2.tar.gz` & `tmp/test_add_python-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_add_python-1.2.tar", last modified: Wed May 17 16:12:33 2023, max compression
+gzip compressed data, was "test_add_python-1.3.tar", last modified: Wed May 17 16:16:33 2023, max compression
```

## Comparing `test_add_python-1.2.tar` & `test_add_python-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:12:33.415500 test_add_python-1.2/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-1.2/MANIFEST.in
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2325 2023-05-17 16:12:33.415500 test_add_python-1.2/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-1.2/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-1.2/pyproject.toml
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 16:12:33.415500 test_add_python-1.2/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7224 2023-05-17 16:12:25.000000 test_add_python-1.2/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:12:33.415500 test_add_python-1.2/src/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-1.2/src/test_add.cu
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-1.2/src/test_add.hh
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-1.2/src/test_add_cpu.cpp
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-1.2/src/test_add_cpu.hpp
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:12:33.415500 test_add_python-1.2/test_add_python.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2325 2023-05-17 16:12:33.000000 test_add_python-1.2/test_add_python.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 16:12:33.000000 test_add_python-1.2/test_add_python.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 16:12:33.000000 test_add_python-1.2/test_add_python.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-1.2/test_add_python.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 16:12:33.000000 test_add_python-1.2/test_add_python.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-1.2/test_add_wrapper.pyx
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:16:33.286856 test_add_python-1.3/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-1.3/MANIFEST.in
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2325 2023-05-17 16:16:33.286856 test_add_python-1.3/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-1.3/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-1.3/pyproject.toml
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 16:16:33.286856 test_add_python-1.3/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7287 2023-05-17 16:16:21.000000 test_add_python-1.3/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:16:33.286856 test_add_python-1.3/src/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-1.3/src/test_add.cu
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-1.3/src/test_add.hh
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-1.3/src/test_add_cpu.cpp
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-1.3/src/test_add_cpu.hpp
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:16:33.286856 test_add_python-1.3/test_add_python.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2325 2023-05-17 16:16:33.000000 test_add_python-1.3/test_add_python.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 16:16:33.000000 test_add_python-1.3/test_add_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 16:16:33.000000 test_add_python-1.3/test_add_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-1.3/test_add_python.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 16:16:33.000000 test_add_python-1.3/test_add_python.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-1.3/test_add_wrapper.pyx
```

### Comparing `test_add_python-1.2/PKG-INFO` & `test_add_python-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_add_python
-Version: 1.2
+Version: 1.3
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
 $$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}) |\Delta_{AUC_{ij}}|$$
```

### Comparing `test_add_python-1.2/README.md` & `test_add_python-1.3/README.md`

 * *Files identical despite different names*

### Comparing `test_add_python-1.2/setup.py` & `test_add_python-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,16 @@
 Discovery in Databases. (2007)
 
 """
 
 setup(name = 'test_add_python',
       # Random metadata. there's more you can supply
       author = 'Dmitry Michaylin',
-      version = '1.2',
-      
+      version = '1.3',
+      short_description = "RocAuc Pairwise Loss, GPU implementation",
       long_description=long_description,
       long_description_content_type='text/markdown',
       
       ext_modules = [ext],
 
       # Inject our custom trigger
       cmdclass = {'build_ext': custom_build_ext},
```

### Comparing `test_add_python-1.2/src/test_add.cu` & `test_add_python-1.3/src/test_add.cu`

 * *Files identical despite different names*

### Comparing `test_add_python-1.2/src/test_add_cpu.cpp` & `test_add_python-1.3/src/test_add_cpu.cpp`

 * *Files identical despite different names*

### Comparing `test_add_python-1.2/test_add_python.egg-info/PKG-INFO` & `test_add_python-1.3/test_add_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-add-python
-Version: 1.2
+Version: 1.3
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
 $$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}) |\Delta_{AUC_{ij}}|$$
```

### Comparing `test_add_python-1.2/test_add_wrapper.pyx` & `test_add_python-1.3/test_add_wrapper.pyx`

 * *Files identical despite different names*

