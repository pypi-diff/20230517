# Comparing `tmp/threedi-modelchecker-2.2.1.tar.gz` & `tmp/threedi-modelchecker-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-modelchecker-2.2.1.tar", last modified: Tue May 16 09:59:38 2023, max compression
+gzip compressed data, was "threedi-modelchecker-2.2.2.tar", last modified: Wed May 17 09:27:55 2023, max compression
```

## Comparing `threedi-modelchecker-2.2.1.tar` & `threedi-modelchecker-2.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:38.939534 threedi-modelchecker-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-16 09:59:38.939534 threedi-modelchecker-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 09:59:38.939534 threedi-modelchecker-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:38.935534 threedi-modelchecker-2.2.1/threedi_modelchecker/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:38.935534 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/geo_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/checks/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    94471 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:38.935534 threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/raster_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/raster_interface_gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/raster_interface_rasterio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/model_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:38.939534 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:38.939534 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/data/empty_v4.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_other.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-16 09:59:35.000000 threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_model_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:59:38.935534 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-16 09:59:38.000000 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-16 09:59:38.000000 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:59:38.000000 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 09:59:38.000000 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:59:38.000000 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 09:59:38.000000 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 09:59:38.000000 threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    20124 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.770960 threedi-modelchecker-2.2.2/threedi_modelchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.774960 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/geo_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/checks/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94471 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.774960 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_rasterio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.778960 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:46.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/data/empty_v4.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-17 09:27:47.000000 threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_model_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:27:55.770960 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 09:27:55.000000 threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/top_level.txt
```

### Comparing `threedi-modelchecker-2.2.1/CHANGES.rst` & `threedi-modelchecker-2.2.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changelog of threedi-modelchecker
 =================================
 
 
+2.2.2 (2023-05-17)
+------------------
+
+- Rewrite release workflow to use a supported github action for github release.
+- Build the release with the build package instead of setuptools.
+
+
+
 2.2.1 (2023-05-16)
 ------------------
 
 - Fixed incorrect units in pumpstation check 66.
 
 
 2.2.0 (2023-05-15)
```

### Comparing `threedi-modelchecker-2.2.1/LICENSE` & `threedi-modelchecker-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/PKG-INFO` & `threedi-modelchecker-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.2.1
+Version: 2.2.2
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.2.1/README.rst` & `threedi-modelchecker-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/setup.py` & `threedi-modelchecker-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/checks/base.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/checks/cross_section_definitions.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/checks/factories.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/checks/geo_query.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/geo_query.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/checks/other.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/other.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/checks/raster.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/checks/timeseries.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/checks/timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/config.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/config.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/exporters.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/raster_interface.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/raster_interface_gdal.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_gdal.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/interfaces/raster_interface_rasterio.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/interfaces/raster_interface_rasterio.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/model_checks.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/scripts.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/conftest.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/factories.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_base.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_cross_section_definitions.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_factories.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_other.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_other.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_raster.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_checks_timeseries.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_checks_timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_exporters.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker/tests/test_model_checks.py` & `threedi-modelchecker-2.2.2/threedi_modelchecker/tests/test_model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/PKG-INFO` & `threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.2.1
+Version: 2.2.2
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.2.1/threedi_modelchecker.egg-info/SOURCES.txt` & `threedi-modelchecker-2.2.2/threedi_modelchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

