# Comparing `tmp/drb-metadata-sentinel1-1.1.0.tar.gz` & `tmp/drb-metadata-sentinel1-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-metadata-sentinel1-1.1.0.tar", last modified: Thu Jan  5 10:01:08 2023, max compression
+gzip compressed data, was "drb-metadata-sentinel1-1.2.0.tar", last modified: Wed May 17 14:30:43 2023, max compression
```

## Comparing `drb-metadata-sentinel1-1.1.0.tar` & `drb-metadata-sentinel1-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:01:08.116411 drb-metadata-sentinel1-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-01-04 15:00:09.000000 drb-metadata-sentinel1-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2712 2023-01-05 10:01:08.116411 drb-metadata-sentinel1-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2335 2022-07-29 09:06:17.000000 drb-metadata-sentinel1-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:01:08.108410 drb-metadata-sentinel1-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:01:08.108410 drb-metadata-sentinel1-1.1.0/drb/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:01:08.108410 drb-metadata-sentinel1-1.1.0/drb/addons/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:01:08.120411 drb-metadata-sentinel1-1.1.0/drb/addons/metadata/sentinel1/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-04 15:00:09.000000 drb-metadata-sentinel1-1.1.0/drb/addons/metadata/sentinel1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-05 10:01:08.120411 drb-metadata-sentinel1-1.1.0/drb/addons/metadata/sentinel1/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    16423 2023-01-04 15:00:09.000000 drb-metadata-sentinel1-1.1.0/drb/addons/metadata/sentinel1/cortex.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:01:08.116411 drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2712 2023-01-05 10:01:08.000000 drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      475 2023-01-05 10:01:08.000000 drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-05 10:01:08.000000 drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-01-05 10:01:08.000000 drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-01-05 10:01:08.000000 drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-05 10:01:08.000000 drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-01-04 15:00:09.000000 drb-metadata-sentinel1-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-01-05 10:01:08.120411 drb-metadata-sentinel1-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      997 2023-01-04 15:00:09.000000 drb-metadata-sentinel1-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    81180 2022-07-29 09:06:17.000000 drb-metadata-sentinel1-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:30:43.701150 drb-metadata-sentinel1-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-05-17 14:30:43.701150 drb-metadata-sentinel1-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:30:43.685150 drb-metadata-sentinel1-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:30:43.685150 drb-metadata-sentinel1-1.2.0/drb/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:30:43.685150 drb-metadata-sentinel1-1.2.0/drb/addons/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:30:43.705150 drb-metadata-sentinel1-1.2.0/drb/addons/metadata/sentinel1/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/drb/addons/metadata/sentinel1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 14:30:43.705150 drb-metadata-sentinel1-1.2.0/drb/addons/metadata/sentinel1/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    16423 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/drb/addons/metadata/sentinel1/cortex.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:30:43.697150 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-05-17 14:30:43.000000 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-17 14:30:43.000000 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:30:43.000000 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-17 14:30:43.000000 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:30:43.000000 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-17 14:30:43.000000 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 14:30:43.000000 drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-17 14:30:43.701150 drb-metadata-sentinel1-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-17 09:27:27.000000 drb-metadata-sentinel1-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:30:43.697150 drb-metadata-sentinel1-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/tests/test_sentinel1_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2023-05-17 08:34:51.000000 drb-metadata-sentinel1-1.2.0/versioneer.py
```

### Comparing `drb-metadata-sentinel1-1.1.0/PKG-INFO` & `drb-metadata-sentinel1-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel1
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sentinel-1 Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-1
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-1
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # DRB Sentinel-1 Metadata AddOn
 This addon allowing to enrich the `Sentinel-1 Product` topic with its metadata
 derivative topics also. 
 
 
 Defined metadata:
@@ -82,8 +83,7 @@
 | PlatformSerialIdentifier         |
 | ProcessingDate                   |
 | ProcessingCenter                 |
 | ProcessorVersion                 |
 | beginningDateTime                |
 | endingDateTime                   |
 | productType                      |
-
```

### Comparing `drb-metadata-sentinel1-1.1.0/README.md` & `drb-metadata-sentinel1-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel1-1.1.0/drb/addons/metadata/sentinel1/cortex.yaml` & `drb-metadata-sentinel1-1.2.0/drb/addons/metadata/sentinel1/cortex.yaml`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel1-1.1.0/drb_metadata_sentinel1.egg-info/PKG-INFO` & `drb-metadata-sentinel1-1.2.0/drb_metadata_sentinel1.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel1
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sentinel-1 Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-1
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-1
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # DRB Sentinel-1 Metadata AddOn
 This addon allowing to enrich the `Sentinel-1 Product` topic with its metadata
 derivative topics also. 
 
 
 Defined metadata:
@@ -82,8 +83,7 @@
 | PlatformSerialIdentifier         |
 | ProcessingDate                   |
 | ProcessingCenter                 |
 | ProcessorVersion                 |
 | beginningDateTime                |
 | endingDateTime                   |
 | productType                      |
-
```

### Comparing `drb-metadata-sentinel1-1.1.0/versioneer.py` & `drb-metadata-sentinel1-1.2.0/versioneer.py`

 * *Files identical despite different names*

