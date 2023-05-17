# Comparing `tmp/rdapy-1.0.0.tar.gz` & `tmp/rdapy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdapy-1.0.0.tar", last modified: Wed May 17 15:46:51 2023, max compression
+gzip compressed data, was "rdapy-1.0.1.tar", last modified: Wed May 17 16:05:38 2023, max compression
```

## Comparing `rdapy-1.0.0.tar` & `rdapy-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,64 @@
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 15:46:51.730052 rdapy-1.0.0/
--rw-r--r--   0 alecramsay   (501) staff       (20)     1067 2023-05-15 21:02:16.000000 rdapy-1.0.0/LICENSE
--rw-r--r--   0 alecramsay   (501) staff       (20)     1492 2023-05-17 15:46:51.729907 rdapy-1.0.0/PKG-INFO
--rw-r--r--   0 alecramsay   (501) staff       (20)      913 2023-05-15 21:02:16.000000 rdapy-1.0.0/README.md
--rw-r--r--   0 alecramsay   (501) staff       (20)      576 2023-05-17 15:46:07.000000 rdapy-1.0.0/pyproject.toml
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 15:46:51.725757 rdapy-1.0.0/rdapy/
--rw-r--r--   0 alecramsay   (501) staff       (20)     1250 2023-05-15 21:02:16.000000 rdapy-1.0.0/rdapy/__init__.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 15:46:51.726858 rdapy-1.0.0/rdapy.egg-info/
--rw-r--r--   0 alecramsay   (501) staff       (20)     1492 2023-05-17 15:46:51.000000 rdapy-1.0.0/rdapy.egg-info/PKG-INFO
--rw-r--r--   0 alecramsay   (501) staff       (20)      464 2023-05-17 15:46:51.000000 rdapy-1.0.0/rdapy.egg-info/SOURCES.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 15:46:51.000000 rdapy-1.0.0/rdapy.egg-info/dependency_links.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 14:22:22.000000 rdapy-1.0.0/rdapy.egg-info/not-zip-safe
--rw-r--r--   0 alecramsay   (501) staff       (20)      161 2023-05-17 15:46:51.000000 rdapy-1.0.0/rdapy.egg-info/requires.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)        6 2023-05-17 15:46:51.000000 rdapy-1.0.0/rdapy.egg-info/top_level.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)       38 2023-05-17 15:46:51.730099 rdapy-1.0.0/setup.cfg
--rw-r--r--   0 alecramsay   (501) staff       (20)      792 2023-05-17 15:01:42.000000 rdapy-1.0.0/setup.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 15:46:51.729621 rdapy-1.0.0/test/
--rw-r--r--   0 alecramsay   (501) staff       (20)      982 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_bias.py
--rw-r--r--   0 alecramsay   (501) staff       (20)      593 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_coi_splitting.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1518 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_compactness.py
--rw-r--r--   0 alecramsay   (501) staff       (20)    20846 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_county_splitting.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     4689 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_graph.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1987 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_kiwysi.py
--rw-r--r--   0 alecramsay   (501) staff       (20)    29281 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_method.py
--rw-r--r--   0 alecramsay   (501) staff       (20)    32227 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_partisan.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1315 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_population.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     3073 2023-05-15 21:02:16.000000 rdapy-1.0.0/test/test_responsiveness.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.809479 rdapy-1.0.1/
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1067 2023-05-15 21:02:16.000000 rdapy-1.0.1/LICENSE
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1519 2023-05-17 16:05:38.809342 rdapy-1.0.1/PKG-INFO
+-rw-r--r--   0 alecramsay   (501) staff       (20)      940 2023-05-17 15:57:58.000000 rdapy-1.0.1/README.md
+-rw-r--r--   0 alecramsay   (501) staff       (20)      576 2023-05-17 16:05:24.000000 rdapy-1.0.1/pyproject.toml
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.802790 rdapy-1.0.1/rdapy/
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1250 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/__init__.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.804192 rdapy-1.0.1/rdapy/compactness/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      128 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1351 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/compactness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     7701 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/features.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     2651 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/kiwysi.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.805011 rdapy-1.0.1/rdapy/compactness/pypoly/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      360 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     2299 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/miniumareaboundingrectangle.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3605 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/polygonattributes.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3357 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/polygoncoordinates.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)      684 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/project.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     4916 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/smallestenclosingcircle.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.805290 rdapy-1.0.1/rdapy/equal/
+-rw-r--r--   0 alecramsay   (501) staff       (20)       69 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/equal/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)      300 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/equal/population.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.805809 rdapy-1.0.1/rdapy/graph/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      117 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1132 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/connected.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)       98 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/constants.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1429 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/embedded.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.806752 rdapy-1.0.1/rdapy/partisan/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      145 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/__init__.py
+-rwxr-xr-x   0 alecramsay   (501) staff       (20)     8599 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/bias.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)       83 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/constants.py
+-rwxr-xr-x   0 alecramsay   (501) staff       (20)     4532 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/method.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3571 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/partisan.py
+-rwxr-xr-x   0 alecramsay   (501) staff       (20)     3165 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/responsiveness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1420 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/utils.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.807128 rdapy-1.0.1/rdapy/splitting/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      268 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/splitting/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1362 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/splitting/coi.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     7959 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/splitting/county.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.803644 rdapy-1.0.1/rdapy.egg-info/
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1519 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/PKG-INFO
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1360 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/SOURCES.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/dependency_links.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 14:22:22.000000 rdapy-1.0.1/rdapy.egg-info/not-zip-safe
+-rw-r--r--   0 alecramsay   (501) staff       (20)      161 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/requires.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)       16 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/top_level.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)       38 2023-05-17 16:05:38.809532 rdapy-1.0.1/setup.cfg
+-rw-r--r--   0 alecramsay   (501) staff       (20)      839 2023-05-17 16:02:31.000000 rdapy-1.0.1/setup.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.808638 rdapy-1.0.1/test/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      982 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_bias.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)      593 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_coi_splitting.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1518 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_compactness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)    20846 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_county_splitting.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     4689 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_graph.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1987 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_kiwysi.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)    29281 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_method.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)    32227 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_partisan.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1315 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_population.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3073 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_responsiveness.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.809170 rdapy-1.0.1/testutils/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      156 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1194 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/compactness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1652 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/equal.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     6371 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/readwrite.py
```

### Comparing `rdapy-1.0.0/LICENSE` & `rdapy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/PKG-INFO` & `rdapy-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdapy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Redistricting analytics in Python
 Home-page: https://github.com/dra2020/rdapy
 Author: alecramsay
 Author-email: Alec Ramsay <alec@davesredistricting.org>
 License: MIT
 Project-URL: Homepage, https://github.com/dra2020/rdapy
 Project-URL: Bug Tracker, https://github.com/dra2020/rdapy/issues
@@ -32,12 +32,12 @@
 - [Equal](./docs/equal.md): Population deviation
 - [Graph](./docs/graph.md): Checks for contiguity & embeddedness
 - [Partisan](./docs/partisan.md): Various measures of partisan bias & responsiveness, as well as support for rank-vote graphs and seats-votes curves
 - [Splitting](./docs/splitting.md): County- & district-splitting and COI splitting
 
 ## Installation
 
-TODO
+Use pip to install the package:
 
 ```bash
 pip install rdapy
 ```
```

### Comparing `rdapy-1.0.0/README.md` & `rdapy-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 - [Equal](./docs/equal.md): Population deviation
 - [Graph](./docs/graph.md): Checks for contiguity & embeddedness
 - [Partisan](./docs/partisan.md): Various measures of partisan bias & responsiveness, as well as support for rank-vote graphs and seats-votes curves
 - [Splitting](./docs/splitting.md): County- & district-splitting and COI splitting
 
 ## Installation
 
-TODO
+Use pip to install the package:
 
 ```bash
 pip install rdapy
 ```
```

### Comparing `rdapy-1.0.0/pyproject.toml` & `rdapy-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rdapy"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Alec Ramsay", email="alec@davesredistricting.org" },
 ]
 description = "Redistricting analytics in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rdapy-1.0.0/rdapy/__init__.py` & `rdapy-1.0.1/rdapy/__init__.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/rdapy.egg-info/PKG-INFO` & `rdapy-1.0.1/rdapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdapy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Redistricting analytics in Python
 Home-page: https://github.com/dra2020/rdapy
 Author: alecramsay
 Author-email: Alec Ramsay <alec@davesredistricting.org>
 License: MIT
 Project-URL: Homepage, https://github.com/dra2020/rdapy
 Project-URL: Bug Tracker, https://github.com/dra2020/rdapy/issues
@@ -32,12 +32,12 @@
 - [Equal](./docs/equal.md): Population deviation
 - [Graph](./docs/graph.md): Checks for contiguity & embeddedness
 - [Partisan](./docs/partisan.md): Various measures of partisan bias & responsiveness, as well as support for rank-vote graphs and seats-votes curves
 - [Splitting](./docs/splitting.md): County- & district-splitting and COI splitting
 
 ## Installation
 
-TODO
+Use pip to install the package:
 
 ```bash
 pip install rdapy
 ```
```

### Comparing `rdapy-1.0.0/setup.py` & `rdapy-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 """
 python setup.py register
 python setup.py register sdist upload
 """
 
 setup(
     name="rdapy",
     version="1.0",
     description="Redistricting analytics in Python",
     url="https://github.com/dra2020/rdapy",
     author="alecramsay",
     author_email="alec@davesredistricting.org",
     license="MIT",
-    packages=["rdapy"],
+    packages=find_packages(),
+    # packages=["rdapy"],
     install_requires=[
         "attrs",
         "certifi",
         "click",
         "click-plugins",
         "cligj",
         "exceptiongroup",
```

### Comparing `rdapy-1.0.0/test/test_bias.py` & `rdapy-1.0.1/test/test_bias.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_coi_splitting.py` & `rdapy-1.0.1/test/test_coi_splitting.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_compactness.py` & `rdapy-1.0.1/test/test_compactness.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_county_splitting.py` & `rdapy-1.0.1/test/test_county_splitting.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_graph.py` & `rdapy-1.0.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_kiwysi.py` & `rdapy-1.0.1/test/test_kiwysi.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_method.py` & `rdapy-1.0.1/test/test_method.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_partisan.py` & `rdapy-1.0.1/test/test_partisan.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_population.py` & `rdapy-1.0.1/test/test_population.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.0/test/test_responsiveness.py` & `rdapy-1.0.1/test/test_responsiveness.py`

 * *Files identical despite different names*

