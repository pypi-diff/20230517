# Comparing `tmp/test_add_python-0.4.tar.gz` & `tmp/test_add_python-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_add_python-0.4.tar", last modified: Wed May 17 15:12:07 2023, max compression
+gzip compressed data, was "test_add_python-0.5.tar", last modified: Wed May 17 15:16:57 2023, max compression
```

## Comparing `test_add_python-0.4.tar` & `test_add_python-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:12:07.664661 test_add_python-0.4/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.4/MANIFEST.in
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1772 2023-05-17 15:12:07.664661 test_add_python-0.4/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.4/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.4/pyproject.toml
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:12:07.664661 test_add_python-0.4/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     6671 2023-05-17 15:11:49.000000 test_add_python-0.4/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:12:07.664661 test_add_python-0.4/src/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.4/src/test_add.cu
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.4/src/test_add.hh
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.4/src/test_add_cpu.cpp
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.4/src/test_add_cpu.hpp
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:12:07.664661 test_add_python-0.4/test_add_python.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1772 2023-05-17 15:12:07.000000 test_add_python-0.4/test_add_python.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:12:07.000000 test_add_python-0.4/test_add_python.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:12:07.000000 test_add_python-0.4/test_add_python.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.4/test_add_python.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:12:07.000000 test_add_python-0.4/test_add_python.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.4/test_add_wrapper.pyx
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:16:57.052092 test_add_python-0.5/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.5/MANIFEST.in
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1908 2023-05-17 15:16:57.052092 test_add_python-0.5/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.5/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.5/pyproject.toml
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:16:57.052092 test_add_python-0.5/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     6811 2023-05-17 15:16:22.000000 test_add_python-0.5/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:16:57.052092 test_add_python-0.5/src/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.5/src/test_add.cu
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.5/src/test_add.hh
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.5/src/test_add_cpu.cpp
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.5/src/test_add_cpu.hpp
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:16:57.052092 test_add_python-0.5/test_add_python.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1908 2023-05-17 15:16:57.000000 test_add_python-0.5/test_add_python.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:16:57.000000 test_add_python-0.5/test_add_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:16:57.000000 test_add_python-0.5/test_add_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.5/test_add_python.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:16:57.000000 test_add_python-0.5/test_add_python.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.5/test_add_wrapper.pyx
```

### Comparing `test_add_python-0.4/PKG-INFO` & `test_add_python-0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: test_add_python
-Version: 0.4
+Version: 0.5
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
-This is gpu implementation of rocauc pairwise loss:
+This is gpu implementation of rocauc pairwise loss.
 Package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
+$$ L = \sum_{i, j}\hat{P}_{ij}\log{P_{ij}} + (1 - \hat{P}_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
 4. **RocAuc Pairwise Loss Exact Smoothened** (GPU or CPU implementations). This loss allows you to incorporate information about equal instances. Because $\Delta_{AUC_{ij}} = 0$ if $y_i = y_j$. So we just add small $\epsilon > 0$ in equation.
 
 ### For more information 
-- You can see example notebook:
-```./examples/gradient_boosting_example.ipynb```
+- You can see example notebook on [GitHub](https://github.com/DmitryAsdre/rocauc_pairwise/blob/main/deltaauc_package_examples.ipynb)
 - Or you can use example notebook on [Google Colab]((https://colab.research.google.com/drive/1w7BN0XGjB5vgFp2pbiCaejabc91xWmI0?usp=sharing))
 - Or you can use example notebook on [Kaggle](https://www.kaggle.com/code/michailindmitry/gradient-boosting-roc-auc-pairwise-example-ipynb)
 
 ## References
-[1] Sean J. Welleck, Efficient AUC Optimization for Information Ranking Applications, IBM USA (2016)
-[2] Burges, C.J.: From ranknet to lambdarank to lambdamart: An overview. Learning (2010)
-[3] Calders, T., Jaroszewicz, S.: Efficient auc optimization for classification. Knowledge
+[1] Sean J. Welleck, Efficient AUC Optimization for Information Ranking Applications, IBM USA (2016) [2] Burges, C.J.: From ranknet to lambdarank to lambdamart: An overview. Learning (2010) [3] Calders, T., Jaroszewicz, S.: Efficient auc optimization for classification. Knowledge
 Discovery in Databases. (2007)
```

### Comparing `test_add_python-0.4/README.md` & `test_add_python-0.5/README.md`

 * *Files identical despite different names*

### Comparing `test_add_python-0.4/setup.py` & `test_add_python-0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,40 +125,40 @@
         extra_link_args= ['-fopenmp'],
             include_dirs = [numpy_include, CUDA['include'], 'src']
         )
 
 
 long_description = """
 # RocAuc Pairwise Loss
-This is gpu implementation of rocauc pairwise loss:
+This is gpu implementation of rocauc pairwise loss.
 Package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. \
 Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
+$$ L = \sum_{i, j}\hat{P}_{ij}\log{P_{ij}} + (1 - \hat{P}_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
 4. **RocAuc Pairwise Loss Exact Smoothened** (GPU or CPU implementations). This loss allows you to incorporate information about equal instances. Because $\Delta_{AUC_{ij}} = 0$ if $y_i = y_j$. So we just add small $\epsilon > 0$ in equation.
 
 ### For more information 
-- You can see example notebook:
-```./examples/gradient_boosting_example.ipynb```
+- You can see example notebook on [GitHub](https://github.com/DmitryAsdre/rocauc_pairwise/blob/main/deltaauc_package_examples.ipynb)
 - Or you can use example notebook on [Google Colab]((https://colab.research.google.com/drive/1w7BN0XGjB5vgFp2pbiCaejabc91xWmI0?usp=sharing))
 - Or you can use example notebook on [Kaggle](https://www.kaggle.com/code/michailindmitry/gradient-boosting-roc-auc-pairwise-example-ipynb)
 
 ## References
-[1] Sean J. Welleck, Efficient AUC Optimization for Information Ranking Applications, IBM USA (2016)
-[2] Burges, C.J.: From ranknet to lambdarank to lambdamart: An overview. Learning (2010)
+[1] Sean J. Welleck, Efficient AUC Optimization for Information Ranking Applications, IBM USA (2016) \
+[2] Burges, C.J.: From ranknet to lambdarank to lambdamart: An overview. Learning (2010) \
 [3] Calders, T., Jaroszewicz, S.: Efficient auc optimization for classification. Knowledge
 Discovery in Databases. (2007)
 """
 
 setup(name = 'test_add_python',
       # Random metadata. there's more you can supply
       author = 'Dmitry Michaylin',
-      version = '0.4',
+      version = '0.5',
       
       long_description=long_description,
       long_description_content_type='text/markdown',
       
       ext_modules = [ext],
 
       # Inject our custom trigger
```

### Comparing `test_add_python-0.4/src/test_add.cu` & `test_add_python-0.5/src/test_add.cu`

 * *Files identical despite different names*

### Comparing `test_add_python-0.4/src/test_add_cpu.cpp` & `test_add_python-0.5/src/test_add_cpu.cpp`

 * *Files identical despite different names*

### Comparing `test_add_python-0.4/test_add_python.egg-info/PKG-INFO` & `test_add_python-0.5/test_add_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: test-add-python
-Version: 0.4
+Version: 0.5
 Author: Dmitry Michaylin
 Description-Content-Type: text/markdown
 
 
 # RocAuc Pairwise Loss
-This is gpu implementation of rocauc pairwise loss:
+This is gpu implementation of rocauc pairwise loss.
 Package could be used to solve classification problems with relative small numbers of objects, where you need to improve rocauc score. Also there is cpu multithread implementation of this losses.
 ## Losses that are realized in this package
 1. **Sigmoid pairwise loss.** (GPU or CPU implementations)
+$$ L = \sum_{i, j}\hat{P}_{ij}\log{P_{ij}} + (1 - \hat{P}_{ij})\log{(1 - P_{ij})}$$
 2. **RocAuc Pairwise Loss** with approximate auc computation. (GPU or CPU implementations)
 3. **RocAuc Pairwise Loss Exact** (GPU or CPU implementations) with exact auc computation. This could be more compute intensive, but this loss might be helpfull for first boosting rounds (if you are using gradient boosting)
 4. **RocAuc Pairwise Loss Exact Smoothened** (GPU or CPU implementations). This loss allows you to incorporate information about equal instances. Because $\Delta_{AUC_{ij}} = 0$ if $y_i = y_j$. So we just add small $\epsilon > 0$ in equation.
 
 ### For more information 
-- You can see example notebook:
-```./examples/gradient_boosting_example.ipynb```
+- You can see example notebook on [GitHub](https://github.com/DmitryAsdre/rocauc_pairwise/blob/main/deltaauc_package_examples.ipynb)
 - Or you can use example notebook on [Google Colab]((https://colab.research.google.com/drive/1w7BN0XGjB5vgFp2pbiCaejabc91xWmI0?usp=sharing))
 - Or you can use example notebook on [Kaggle](https://www.kaggle.com/code/michailindmitry/gradient-boosting-roc-auc-pairwise-example-ipynb)
 
 ## References
-[1] Sean J. Welleck, Efficient AUC Optimization for Information Ranking Applications, IBM USA (2016)
-[2] Burges, C.J.: From ranknet to lambdarank to lambdamart: An overview. Learning (2010)
-[3] Calders, T., Jaroszewicz, S.: Efficient auc optimization for classification. Knowledge
+[1] Sean J. Welleck, Efficient AUC Optimization for Information Ranking Applications, IBM USA (2016) [2] Burges, C.J.: From ranknet to lambdarank to lambdamart: An overview. Learning (2010) [3] Calders, T., Jaroszewicz, S.: Efficient auc optimization for classification. Knowledge
 Discovery in Databases. (2007)
```

### Comparing `test_add_python-0.4/test_add_wrapper.pyx` & `test_add_python-0.5/test_add_wrapper.pyx`

 * *Files identical despite different names*

