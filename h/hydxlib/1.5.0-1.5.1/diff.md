# Comparing `tmp/hydxlib-1.5.0.tar.gz` & `tmp/hydxlib-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydxlib-1.5.0.tar", last modified: Wed Apr 12 07:20:37 2023, max compression
+gzip compressed data, was "hydxlib-1.5.1.tar", last modified: Wed May 17 13:14:54 2023, max compression
```

## Comparing `hydxlib-1.5.0.tar` & `hydxlib-1.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.335319 hydxlib-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-12 07:20:34.000000 hydxlib-1.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-12 07:20:34.000000 hydxlib-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 07:20:34.000000 hydxlib-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-12 07:20:37.335319 hydxlib-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 07:20:34.000000 hydxlib-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.331319 hydxlib-1.5.0/hydxlib/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/hydx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.335319 hydxlib-1.5.0/hydxlib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_hydx.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/tests/test_threedi.py
--rw-r--r--   0 runner    (1001) docker     (123)    31610 2023-04-12 07:20:34.000000 hydxlib-1.5.0/hydxlib/threedi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:20:37.335319 hydxlib-1.5.0/hydxlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 07:20:37.000000 hydxlib-1.5.0/hydxlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 07:20:37.335319 hydxlib-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-12 07:20:34.000000 hydxlib-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:54.760274 hydxlib-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-17 13:14:51.000000 hydxlib-1.5.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-17 13:14:51.000000 hydxlib-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-17 13:14:51.000000 hydxlib-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-17 13:14:54.760274 hydxlib-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-17 13:14:51.000000 hydxlib-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:54.752274 hydxlib-1.5.1/hydxlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/hydx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:54.760274 hydxlib-1.5.1/hydxlib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/tests/test_hydx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/tests/test_threedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31610 2023-05-17 13:14:51.000000 hydxlib-1.5.1/hydxlib/threedi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:54.756274 hydxlib-1.5.1/hydxlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-17 13:14:54.000000 hydxlib-1.5.1/hydxlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 13:14:54.000000 hydxlib-1.5.1/hydxlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:14:54.000000 hydxlib-1.5.1/hydxlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 13:14:54.000000 hydxlib-1.5.1/hydxlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:14:54.000000 hydxlib-1.5.1/hydxlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 13:14:54.000000 hydxlib-1.5.1/hydxlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 13:14:54.000000 hydxlib-1.5.1/hydxlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 13:14:54.760274 hydxlib-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-17 13:14:51.000000 hydxlib-1.5.1/setup.py
```

### Comparing `hydxlib-1.5.0/CHANGES.rst` & `hydxlib-1.5.1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog of hydxlib
 ===================================================
 
+1.5.1 (2023-05-17)
+------------------
+
+- Updated required threedi-schema version to 0.217.*
+
+
 1.5.0 (2023-04-12)
 ------------------
 
 - Extra release to signal updated requirements.
 
 
 1.4.5 (2023-03-31)
```

### Comparing `hydxlib-1.5.0/LICENSE` & `hydxlib-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/PKG-INFO` & `hydxlib-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydxlib
-Version: 1.5.0
+Version: 1.5.1
 Summary: Importer and Exporter for GWSW
 Home-page: https://github.com/nens/hydxlib
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
@@ -83,14 +83,20 @@
 
   $ pre-commit install
 
 
 Changelog of hydxlib
 ===================================================
 
+1.5.1 (2023-05-17)
+------------------
+
+- Updated required threedi-schema version to 0.217.*
+
+
 1.5.0 (2023-04-12)
 ------------------
 
 - Extra release to signal updated requirements.
 
 
 1.4.5 (2023-03-31)
```

### Comparing `hydxlib-1.5.0/README.rst` & `hydxlib-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/exporter.py` & `hydxlib-1.5.1/hydxlib/exporter.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/hydx.py` & `hydxlib-1.5.1/hydxlib/hydx.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/importer.py` & `hydxlib-1.5.1/hydxlib/importer.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/scripts.py` & `hydxlib-1.5.1/hydxlib/scripts.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/tests/conftest.py` & `hydxlib-1.5.1/hydxlib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/tests/test_exporter.py` & `hydxlib-1.5.1/hydxlib/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/tests/test_hydx.py` & `hydxlib-1.5.1/hydxlib/tests/test_hydx.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/tests/test_importer.py` & `hydxlib-1.5.1/hydxlib/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/tests/test_scripts.py` & `hydxlib-1.5.1/hydxlib/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/tests/test_threedi.py` & `hydxlib-1.5.1/hydxlib/tests/test_threedi.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib/threedi.py` & `hydxlib-1.5.1/hydxlib/threedi.py`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/hydxlib.egg-info/PKG-INFO` & `hydxlib-1.5.1/hydxlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydxlib
-Version: 1.5.0
+Version: 1.5.1
 Summary: Importer and Exporter for GWSW
 Home-page: https://github.com/nens/hydxlib
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
@@ -83,14 +83,20 @@
 
   $ pre-commit install
 
 
 Changelog of hydxlib
 ===================================================
 
+1.5.1 (2023-05-17)
+------------------
+
+- Updated required threedi-schema version to 0.217.*
+
+
 1.5.0 (2023-04-12)
 ------------------
 
 - Extra release to signal updated requirements.
 
 
 1.4.5 (2023-03-31)
```

### Comparing `hydxlib-1.5.0/hydxlib.egg-info/SOURCES.txt` & `hydxlib-1.5.1/hydxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydxlib-1.5.0/setup.py` & `hydxlib-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 install_requires = [
     "sqlalchemy",
-    "threedi-schema==0.216.*",
+    "threedi-schema==0.217.*",
     "pyproj>=3",
 ]
 
 tests_require = ["pytest", "pytest-cov"]
 
 setup(
     name="hydxlib",
```

