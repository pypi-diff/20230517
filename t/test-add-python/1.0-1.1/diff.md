# Comparing `tmp/test_add_python-1.0.tar.gz` & `tmp/test_add_python-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_add_python-1.0.tar", last modified: Wed May 17 16:05:30 2023, max compression
+gzip compressed data, was "test_add_python-1.1.tar", last modified: Wed May 17 16:08:00 2023, max compression
```

## Comparing `test_add_python-1.0.tar` & `test_add_python-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:05:30.449333 test_add_python-1.0/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-1.0/MANIFEST.in
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2395 2023-05-17 16:05:30.449333 test_add_python-1.0/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-1.0/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-1.0/pyproject.toml
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 16:05:30.449333 test_add_python-1.0/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7301 2023-05-17 16:04:56.000000 test_add_python-1.0/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:05:30.449333 test_add_python-1.0/src/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-1.0/src/test_add.cu
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-1.0/src/test_add.hh
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-1.0/src/test_add_cpu.cpp
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-1.0/src/test_add_cpu.hpp
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:05:30.449333 test_add_python-1.0/test_add_python.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2395 2023-05-17 16:05:30.000000 test_add_python-1.0/test_add_python.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 16:05:30.000000 test_add_python-1.0/test_add_python.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 16:05:30.000000 test_add_python-1.0/test_add_python.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-1.0/test_add_python.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 16:05:30.000000 test_add_python-1.0/test_add_python.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-1.0/test_add_wrapper.pyx
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:08:00.631573 test_add_python-1.1/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-1.1/MANIFEST.in
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2385 2023-05-17 16:08:00.631573 test_add_python-1.1/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-1.1/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-1.1/pyproject.toml
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 16:08:00.631573 test_add_python-1.1/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7290 2023-05-17 16:07:48.000000 test_add_python-1.1/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:08:00.631573 test_add_python-1.1/src/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-1.1/src/test_add.cu
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-1.1/src/test_add.hh
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-1.1/src/test_add_cpu.cpp
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-1.1/src/test_add_cpu.hpp
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:08:00.631573 test_add_python-1.1/test_add_python.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2385 2023-05-17 16:08:00.000000 test_add_python-1.1/test_add_python.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 16:08:00.000000 test_add_python-1.1/test_add_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 16:08:00.000000 test_add_python-1.1/test_add_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-1.1/test_add_python.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 16:08:00.000000 test_add_python-1.1/test_add_python.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-1.1/test_add_wrapper.pyx
```

### Comparing `test_add_python-1.0/PKG-INFO` & `test_add_python-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: test_add_python
-Version: 1.0
+Version: 1.1
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})})\lvert \Delta_{AUC_{ij}} vert$$
+$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}) |\Delta_{AUC_{ij}}|$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 $$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}vert$$
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
```

### Comparing `test_add_python-1.0/README.md` & `test_add_python-1.1/README.md`

 * *Files identical despite different names*

### Comparing `test_add_python-1.0/setup.py` & `test_add_python-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             include_dirs = [numpy_include, CUDA['include'], 'src']
         )
 
 
 long_description = """
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})})\lvert \Delta_{AUC_{ij}} \rvert$$
+$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}) |\Delta_{AUC_{ij}}|$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. \
 Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 $$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC^{approx}_{ij}}\rvert$$
@@ -155,15 +155,15 @@
 Discovery in Databases. (2007)
 
 """
 
 setup(name = 'test_add_python',
       # Random metadata. there's more you can supply
       author = 'Dmitry Michaylin',
-      version = '1.0',
+      version = '1.1',
       
       long_description=long_description,
       long_description_content_type='text/markdown',
       
       ext_modules = [ext],
 
       # Inject our custom trigger
```

### Comparing `test_add_python-1.0/src/test_add.cu` & `test_add_python-1.1/src/test_add.cu`

 * *Files identical despite different names*

### Comparing `test_add_python-1.0/src/test_add_cpu.cpp` & `test_add_python-1.1/src/test_add_cpu.cpp`

 * *Files identical despite different names*

### Comparing `test_add_python-1.0/test_add_python.egg-info/PKG-INFO` & `test_add_python-1.1/test_add_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: test-add-python
-Version: 1.0
+Version: 1.1
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})})\lvert \Delta_{AUC_{ij}} vert$$
+$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}) |\Delta_{AUC_{ij}}|$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 $$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}vert$$
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
```

### Comparing `test_add_python-1.0/test_add_wrapper.pyx` & `test_add_python-1.1/test_add_wrapper.pyx`

 * *Files identical despite different names*

