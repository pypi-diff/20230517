# Comparing `tmp/test_add_python-0.7.tar.gz` & `tmp/test_add_python-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_add_python-0.7.tar", last modified: Wed May 17 15:55:22 2023, max compression
+gzip compressed data, was "test_add_python-0.8.tar", last modified: Wed May 17 15:59:26 2023, max compression
```

## Comparing `test_add_python-0.7.tar` & `test_add_python-0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:55:22.363115 test_add_python-0.7/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.7/MANIFEST.in
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2451 2023-05-17 15:55:22.363115 test_add_python-0.7/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.7/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.7/pyproject.toml
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:55:22.363115 test_add_python-0.7/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7359 2023-05-17 15:55:03.000000 test_add_python-0.7/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:55:22.363115 test_add_python-0.7/src/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.7/src/test_add.cu
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.7/src/test_add.hh
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.7/src/test_add_cpu.cpp
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.7/src/test_add_cpu.hpp
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:55:22.363115 test_add_python-0.7/test_add_python.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2451 2023-05-17 15:55:22.000000 test_add_python-0.7/test_add_python.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:55:22.000000 test_add_python-0.7/test_add_python.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:55:22.000000 test_add_python-0.7/test_add_python.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.7/test_add_python.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:55:22.000000 test_add_python-0.7/test_add_python.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.7/test_add_wrapper.pyx
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:59:26.195514 test_add_python-0.8/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.8/MANIFEST.in
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2404 2023-05-17 15:59:26.195514 test_add_python-0.8/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.8/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.8/pyproject.toml
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:59:26.195514 test_add_python-0.8/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     7311 2023-05-17 15:59:18.000000 test_add_python-0.8/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:59:26.195514 test_add_python-0.8/src/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.8/src/test_add.cu
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.8/src/test_add.hh
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.8/src/test_add_cpu.cpp
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.8/src/test_add_cpu.hpp
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:59:26.195514 test_add_python-0.8/test_add_python.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2404 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.8/test_add_python.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:59:26.000000 test_add_python-0.8/test_add_python.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.8/test_add_wrapper.pyx
```

### Comparing `test_add_python-0.7/PKG-INFO` & `test_add_python-0.8/test_add_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
-Name: test_add_python
-Version: 0.7
+Name: test-add-python
+Version: 0.8
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC_{ij}}ert$$
-Where:
-$$P_{ij} = rac{1}{1 + e^{-(x_i - x_j)}} $$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC_{ij}}vert$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}ert$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}vert$$
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{exact}_{ij}}ert$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{exact}_{ij}}vert$$
 4. **RocAuc Pairwise Loss Exact Smoothened** (GPU or CPU implementations). This loss allows you to incorporate information about equal instances. Because $\Delta_{AUC_{ij}} = 0$ if $y_i = y_j$. So we just add small $\epsilon > 0$ in equation.
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)(\epsilon + \lvert \Delta_{AUC^{exact}_{ij}}ert)$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)(\epsilon + \lvert \Delta_{AUC^{exact}_{ij}}vert)$$
 
 ### For more information 
 - You can see [GitHub repository](https://github.com/DmitryAsdre/rocauc_pairwise).
 - Or you can use example notebook on [Google Colab](https://colab.research.google.com/drive/1w7BN0XGjB5vgFp2pbiCaejabc91xWmI0?usp=sharing)
 - Or you can use example notebook on [Kaggle](https://www.kaggle.com/code/michailindmitry/gradient-boosting-roc-auc-pairwise-example-ipynb)
 
 ## References
```

### Comparing `test_add_python-0.7/README.md` & `test_add_python-0.8/README.md`

 * *Files identical despite different names*

### Comparing `test_add_python-0.7/setup.py` & `test_add_python-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,28 +126,26 @@
             include_dirs = [numpy_include, CUDA['include'], 'src']
         )
 
 
 long_description = """
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC_{ij}}\vert$$
-Where:
-$$P_{ij} = \frac{1}{1 + e^{-(x_i - x_j)}} $$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC_{ij}}\rvert$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. \
 Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC^{approx}_{ij}}\vert$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC^{approx}_{ij}}\rvert$$
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC^{exact}_{ij}}\vert$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)\lvert \Delta_{AUC^{exact}_{ij}}\rvert$$
 4. **RocAuc Pairwise Loss Exact Smoothened** (GPU or CPU implementations). This loss allows you to incorporate information about equal instances. Because $\Delta_{AUC_{ij}} = 0$ if $y_i = y_j$. So we just add small $\epsilon > 0$ in equation.
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)(\epsilon + \lvert \Delta_{AUC^{exact}_{ij}}\vert)$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}\right)(\epsilon + \lvert \Delta_{AUC^{exact}_{ij}}\rvert)$$
 
 ### For more information 
 - You can see [GitHub repository](https://github.com/DmitryAsdre/rocauc_pairwise).
 - Or you can use example notebook on [Google Colab](https://colab.research.google.com/drive/1w7BN0XGjB5vgFp2pbiCaejabc91xWmI0?usp=sharing)
 - Or you can use example notebook on [Kaggle](https://www.kaggle.com/code/michailindmitry/gradient-boosting-roc-auc-pairwise-example-ipynb)
 
 ## References
@@ -157,15 +155,15 @@
 Discovery in Databases. (2007)
 
 """
 
 setup(name = 'test_add_python',
       # Random metadata. there's more you can supply
       author = 'Dmitry Michaylin',
-      version = '0.7',
+      version = '0.8',
       
       long_description=long_description,
       long_description_content_type='text/markdown',
       
       ext_modules = [ext],
 
       # Inject our custom trigger
```

### Comparing `test_add_python-0.7/src/test_add.cu` & `test_add_python-0.8/src/test_add.cu`

 * *Files identical despite different names*

### Comparing `test_add_python-0.7/src/test_add_cpu.cpp` & `test_add_python-0.8/src/test_add_cpu.cpp`

 * *Files identical despite different names*

### Comparing `test_add_python-0.7/test_add_python.egg-info/PKG-INFO` & `test_add_python-0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
-Name: test-add-python
-Version: 0.7
+Name: test_add_python
+Version: 0.8
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
  This is gpu implementation of rocauc pairwise loss:
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC_{ij}}ert$$
-Where:
-$$P_{ij} = rac{1}{1 + e^{-(x_i - x_j)}} $$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC_{ij}}vert$$
 This package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
 $$L = \sum_{i, j}\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}ert$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{approx}_{ij}}vert$$
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{exact}_{ij}}ert$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)\lvert \Delta_{AUC^{exact}_{ij}}vert$$
 4. **RocAuc Pairwise Loss Exact Smoothened** (GPU or CPU implementations). This loss allows you to incorporate information about equal instances. Because $\Delta_{AUC_{ij}} = 0$ if $y_i = y_j$. So we just add small $\epsilon > 0$ in equation.
-$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)(\epsilon + \lvert \Delta_{AUC^{exact}_{ij}}ert)$$
+$$L = \sum_{i, j} \left(\hat P_{ij}\log{P_{ij}} + (1 - \hat P_{ij})\log{(1 - P_{ij})}ight)(\epsilon + \lvert \Delta_{AUC^{exact}_{ij}}vert)$$
 
 ### For more information 
 - You can see [GitHub repository](https://github.com/DmitryAsdre/rocauc_pairwise).
 - Or you can use example notebook on [Google Colab](https://colab.research.google.com/drive/1w7BN0XGjB5vgFp2pbiCaejabc91xWmI0?usp=sharing)
 - Or you can use example notebook on [Kaggle](https://www.kaggle.com/code/michailindmitry/gradient-boosting-roc-auc-pairwise-example-ipynb)
 
 ## References
```

### Comparing `test_add_python-0.7/test_add_wrapper.pyx` & `test_add_python-0.8/test_add_wrapper.pyx`

 * *Files identical despite different names*

