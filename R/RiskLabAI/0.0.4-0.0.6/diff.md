# Comparing `tmp/RiskLabAI-0.0.4.tar.gz` & `tmp/RiskLabAI-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLabAI-0.0.4.tar", last modified: Wed May 17 13:40:23 2023, max compression
+gzip compressed data, was "RiskLabAI-0.0.6.tar", last modified: Wed May 17 14:23:52 2023, max compression
```

## Comparing `RiskLabAI-0.0.4.tar` & `RiskLabAI-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/data/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/data/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/hedging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/infomation_driven_bars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/standard_bars.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/RiskLabAI/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/utils/smoothing_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:52.066944 RiskLabAI-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 14:23:52.066944 RiskLabAI-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:52.062944 RiskLabAI-0.0.6/RiskLabAI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:52.062944 RiskLabAI-0.0.6/RiskLabAI/RiskLabAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 14:23:52.000000 RiskLabAI-0.0.6/RiskLabAI/RiskLabAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-17 14:23:52.000000 RiskLabAI-0.0.6/RiskLabAI/RiskLabAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:23:52.000000 RiskLabAI-0.0.6/RiskLabAI/RiskLabAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 14:23:52.000000 RiskLabAI-0.0.6/RiskLabAI/RiskLabAI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 14:23:52.000000 RiskLabAI-0.0.6/RiskLabAI/RiskLabAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:52.066944 RiskLabAI-0.0.6/RiskLabAI/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:52.066944 RiskLabAI-0.0.6/RiskLabAI/data/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/data/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/data/structures/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/data/structures/hedging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/data/structures/infomation_driven_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/data/structures/standard_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/data/structures/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:52.066944 RiskLabAI-0.0.6/RiskLabAI/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/RiskLabAI/utils/smoothing_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 14:23:30.000000 RiskLabAI-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 14:23:52.066944 RiskLabAI-0.0.6/setup.cfg
```

### Comparing `RiskLabAI-0.0.4/LICENSE` & `RiskLabAI-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/PKG-INFO` & `RiskLabAI-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskLabAI
-Version: 0.0.4
+Version: 0.0.6
 Summary: Financial AI using Python.
 Home-page: https://github.com/RiskLabAI/RiskLabAI.py
 Author: RiskLab
 Author-email: research@risklab.ai
 Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
 Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/PKG-INFO` & `RiskLabAI-0.0.6/RiskLabAI/RiskLabAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskLabAI
-Version: 0.0.4
+Version: 0.0.6
 Summary: Financial AI using Python.
 Home-page: https://github.com/RiskLabAI/RiskLabAI.py
 Author: RiskLab
 Author-email: research@risklab.ai
 Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
 Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RiskLabAI-0.0.4/RiskLabAI/data/structures/filtering.py` & `RiskLabAI-0.0.6/RiskLabAI/data/structures/filtering.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/RiskLabAI/data/structures/hedging.py` & `RiskLabAI-0.0.6/RiskLabAI/data/structures/hedging.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/RiskLabAI/data/structures/infomation_driven_bars.py` & `RiskLabAI-0.0.6/RiskLabAI/data/structures/infomation_driven_bars.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/RiskLabAI/data/structures/standard_bars.py` & `RiskLabAI-0.0.6/RiskLabAI/data/structures/standard_bars.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/RiskLabAI/data/structures/utilities.py` & `RiskLabAI-0.0.6/RiskLabAI/data/structures/utilities.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/RiskLabAI/utils/progress.py` & `RiskLabAI-0.0.6/RiskLabAI/utils/progress.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/RiskLabAI/utils/smoothing_average.py` & `RiskLabAI-0.0.6/RiskLabAI/utils/smoothing_average.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.4/setup.cfg` & `RiskLabAI-0.0.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = RiskLabAI
-version = 0.0.4
+version = 0.0.6
 author = RiskLab
 author_email = research@risklab.ai
 description = Financial AI using Python.
 long_description_content_type = text/markdown
 url = https://github.com/RiskLabAI/RiskLabAI.py
 project_urls = 
 	Bug Tracker = https://github.com/RiskLabAI/RiskLabAI.py/issues
```

