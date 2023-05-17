# Comparing `tmp/test_add_python-0.8.tar.gz` & `tmp/test_add_python-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_add_python-0.8.tar", last modified: Wed May 17 15:59:26 2023, max compression
+gzip compressed data, was "test_add_python-0.9.tar", last modified: Wed May 17 16:02:31 2023, max compression
```

## Comparing `test_add_python-0.8.tar` & `test_add_python-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:59:26.195514 test_add_python-0.8/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.8/MANIFEST.in
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2404 2023-05-17 15:59:26.195514 test_add_python-0.8/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.8/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.8/pyproject.toml
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:59:26.195514 test_add_python-0.8/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7311 2023-05-17 15:59:18.000000 test_add_python-0.8/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:59:26.195514 test_add_python-0.8/src/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.8/src/test_add.cu
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.8/src/test_add.hh
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.8/src/test_add_cpu.cpp
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.8/src/test_add_cpu.hpp
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:59:26.195514 test_add_python-0.8/test_add_python.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2404 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.8/test_add_python.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.8/test_add_wrapper.pyx
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:02:31.250554 test_add_python-0.9/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.9/MANIFEST.in
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2394 2023-05-17 16:02:31.250554 test_add_python-0.9/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.9/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.9/pyproject.toml
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 16:02:31.250554 test_add_python-0.9/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7300 2023-05-17 16:02:04.000000 test_add_python-0.9/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:02:31.250554 test_add_python-0.9/src/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.9/src/test_add.cu
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.9/src/test_add.hh
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.9/src/test_add_cpu.cpp
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.9/src/test_add_cpu.hpp
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 16:02:31.250554 test_add_python-0.9/test_add_python.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2394 2023-05-17 16:02:31.000000 test_add_python-0.9/test_add_python.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 16:02:31.000000 test_add_python-0.9/test_add_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 16:02:31.000000 test_add_python-0.9/test_add_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.9/test_add_python.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 16:02:31.000000 test_add_python-0.9/test_add_python.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.9/test_add_wrapper.pyx
```

### Comparing `test_add_python-0.8/PKG-INFO` & `test_add_python-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: test_add_python
-Version: 0.8
+Version: 0.9
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC_{ij}}vert$$
+$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})})\lvert \Delta_{AUC_{ij}}vert$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 $$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}vert$$
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
```

### Comparing `test_add_python-0.8/README.md` & `test_add_python-0.9/README.md`

 * *Files identical despite different names*

### Comparing `test_add_python-0.8/setup.py` & `test_add_python-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             include_dirs = [numpy_include, CUDA['include'], 'src']
         )
 
 
 long_description = """
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC_{ij}}\rvert$$
+$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})})\lvert \Delta_{AUC_{ij}}\rvert$$
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
-      version = '0.8',
+      version = '0.9',
       
       long_description=long_description,
       long_description_content_type='text/markdown',
       
       ext_modules = [ext],
 
       # Inject our custom trigger
```

### Comparing `test_add_python-0.8/src/test_add.cu` & `test_add_python-0.9/src/test_add.cu`

 * *Files identical despite different names*

### Comparing `test_add_python-0.8/src/test_add_cpu.cpp` & `test_add_python-0.9/src/test_add_cpu.cpp`

 * *Files identical despite different names*

### Comparing `test_add_python-0.8/test_add_python.egg-info/PKG-INFO` & `test_add_python-0.9/test_add_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: test-add-python
-Version: 0.8
+Version: 0.9
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC_{ij}}vert$$
+$$L = \sum_{i, j} (\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})})\lvert \Delta_{AUC_{ij}}vert$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 $$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}vert$$
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
```

### Comparing `test_add_python-0.8/test_add_wrapper.pyx` & `test_add_python-0.9/test_add_wrapper.pyx`

 * *Files identical despite different names*

