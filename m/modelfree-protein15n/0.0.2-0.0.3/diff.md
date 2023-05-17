# Comparing `tmp/modelfree-protein15n-0.0.2.tar.gz` & `tmp/modelfree-protein15n-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelfree-protein15n-0.0.2.tar", last modified: Tue May 16 15:00:32 2023, max compression
+gzip compressed data, was "modelfree-protein15n-0.0.3.tar", last modified: Tue May 16 15:09:47 2023, max compression
```

## Comparing `modelfree-protein15n-0.0.2.tar` & `modelfree-protein15n-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:00:32.112038 modelfree-protein15n-0.0.2/
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/LICENSE
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/MANIFEST.in
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3586 2023-05-16 15:00:32.111029 modelfree-protein15n-0.0.2/PKG-INFO
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2621 2023-05-15 21:35:59.000000 modelfree-protein15n-0.0.2/README.md
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:00:32.081463 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3586 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/PKG-INFO
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      573 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/SOURCES.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/dependency_links.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/entry_points.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       40 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/requires.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/top_level.txt
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:00:32.108854 modelfree-protein15n-0.0.2/modfree/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/__init__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/__main__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1736 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/analysis.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      719 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/constants_functions.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/data_format.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6461 2023-05-16 14:24:26.000000 modelfree-protein15n-0.0.2/modfree/generator.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2327 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/inputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14130 2023-05-16 14:28:18.000000 modelfree-protein15n-0.0.2/modfree/mf_standard.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5842 2023-05-16 14:21:36.000000 modelfree-protein15n-0.0.2/modfree/modfree.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3667 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/outputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2481 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/parser.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5079 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/ploter.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2912 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/run_fit.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-16 15:00:32.112741 modelfree-protein15n-0.0.2/setup.cfg
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1075 2023-05-16 14:16:51.000000 modelfree-protein15n-0.0.2/setup.py
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:09:47.781730 modelfree-protein15n-0.0.3/
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/LICENSE
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/MANIFEST.in
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3586 2023-05-16 15:09:47.780732 modelfree-protein15n-0.0.3/PKG-INFO
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2621 2023-05-15 21:35:59.000000 modelfree-protein15n-0.0.3/README.md
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:09:47.747317 modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3586 2023-05-16 15:09:47.000000 modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/PKG-INFO
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      573 2023-05-16 15:09:47.000000 modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/SOURCES.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-16 15:09:47.000000 modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/dependency_links.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-16 15:09:47.000000 modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/entry_points.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       48 2023-05-16 15:09:47.000000 modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/requires.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-16 15:09:47.000000 modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/top_level.txt
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:09:47.778730 modelfree-protein15n-0.0.3/modfree/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/__init__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/__main__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1736 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/analysis.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      719 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/constants_functions.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/data_format.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6461 2023-05-16 14:24:26.000000 modelfree-protein15n-0.0.3/modfree/generator.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2327 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/inputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14130 2023-05-16 14:28:18.000000 modelfree-protein15n-0.0.3/modfree/mf_standard.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5842 2023-05-16 15:07:38.000000 modelfree-protein15n-0.0.3/modfree/modfree.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3667 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/outputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2481 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/parser.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5079 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/ploter.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2912 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.3/modfree/run_fit.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-16 15:09:47.782184 modelfree-protein15n-0.0.3/setup.cfg
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1094 2023-05-16 15:06:21.000000 modelfree-protein15n-0.0.3/setup.py
```

### Comparing `modelfree-protein15n-0.0.2/LICENSE` & `modelfree-protein15n-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/PKG-INFO` & `modelfree-protein15n-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.2
+Version: 0.0.3
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Simple flexible model free analysis framework for protein backbone amide 15N NMR spin relaxation rates
```

### Comparing `modelfree-protein15n-0.0.2/README.md` & `modelfree-protein15n-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/PKG-INFO` & `modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.2
+Version: 0.0.3
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Simple flexible model free analysis framework for protein backbone amide 15N NMR spin relaxation rates
```

### Comparing `modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/SOURCES.txt` & `modelfree-protein15n-0.0.3/modelfree_protein15n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/analysis.py` & `modelfree-protein15n-0.0.3/modfree/analysis.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/constants_functions.py` & `modelfree-protein15n-0.0.3/modfree/constants_functions.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/data_format.py` & `modelfree-protein15n-0.0.3/modfree/data_format.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/generator.py` & `modelfree-protein15n-0.0.3/modfree/generator.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/inputs.py` & `modelfree-protein15n-0.0.3/modfree/inputs.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/mf_standard.py` & `modelfree-protein15n-0.0.3/modfree/mf_standard.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/modfree.py` & `modelfree-protein15n-0.0.3/modfree/modfree.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import modfree.inputs as inputs
 import modfree.outputs as outputs
 import modfree.run_fit as run_fit
 import modfree.ploter as ploter
 import modfree.generator as generator
 
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 console = Console()
 
 
 header = "\n".join(
 [
```

### Comparing `modelfree-protein15n-0.0.2/modfree/outputs.py` & `modelfree-protein15n-0.0.3/modfree/outputs.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/parser.py` & `modelfree-protein15n-0.0.3/modfree/parser.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/ploter.py` & `modelfree-protein15n-0.0.3/modfree/ploter.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/modfree/run_fit.py` & `modelfree-protein15n-0.0.3/modfree/run_fit.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.2/setup.py` & `modelfree-protein15n-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     install_requires = [
         'numpy',
         'scipy',
         'lmfit',
         'matplotlib',
         'rich',
         'tomli',
+        'seaborn',
     ],
     classifiers = [
         "Programming Language :: Python :: 3",
         ],
     extras_requires = {
         "dev": [
             "pytest>=3.7",
```

