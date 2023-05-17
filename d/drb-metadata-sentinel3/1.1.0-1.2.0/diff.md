# Comparing `tmp/drb-metadata-sentinel3-1.1.0.tar.gz` & `tmp/drb-metadata-sentinel3-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-metadata-sentinel3-1.1.0.tar", last modified: Thu Jan  5 10:08:45 2023, max compression
+gzip compressed data, was "drb-metadata-sentinel3-1.2.0.tar", last modified: Wed May 17 14:35:59 2023, max compression
```

## Comparing `drb-metadata-sentinel3-1.1.0.tar` & `drb-metadata-sentinel3-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:08:45.780936 drb-metadata-sentinel3-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     6805 2023-01-05 10:08:45.780936 drb-metadata-sentinel3-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6428 2022-09-21 15:37:00.000000 drb-metadata-sentinel3-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:08:45.776936 drb-metadata-sentinel3-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:08:45.776936 drb-metadata-sentinel3-1.1.0/drb/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:08:45.776936 drb-metadata-sentinel3-1.1.0/drb/addons/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:08:45.784936 drb-metadata-sentinel3-1.1.0/drb/addons/metadata/sentinel3/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-04 16:01:25.000000 drb-metadata-sentinel3-1.1.0/drb/addons/metadata/sentinel3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-05 10:08:45.784936 drb-metadata-sentinel3-1.1.0/drb/addons/metadata/sentinel3/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    16337 2023-01-04 16:01:25.000000 drb-metadata-sentinel3-1.1.0/drb/addons/metadata/sentinel3/cortex.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 10:08:45.780936 drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6805 2023-01-05 10:08:45.000000 drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      463 2023-01-05 10:08:45.000000 drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-05 10:08:45.000000 drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-01-05 10:08:45.000000 drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-01-05 10:08:45.000000 drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-05 10:08:45.000000 drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-01-04 16:01:25.000000 drb-metadata-sentinel3-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-01-05 10:08:45.784936 drb-metadata-sentinel3-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-01-04 16:01:25.000000 drb-metadata-sentinel3-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-09-21 15:37:00.000000 drb-metadata-sentinel3-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:35:59.350916 drb-metadata-sentinel3-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     6914 2023-05-17 14:35:59.350916 drb-metadata-sentinel3-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6428 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:35:59.338915 drb-metadata-sentinel3-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:35:59.338915 drb-metadata-sentinel3-1.2.0/drb/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:35:59.338915 drb-metadata-sentinel3-1.2.0/drb/addons/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:35:59.350916 drb-metadata-sentinel3-1.2.0/drb/addons/metadata/sentinel3/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/drb/addons/metadata/sentinel3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 14:35:59.350916 drb-metadata-sentinel3-1.2.0/drb/addons/metadata/sentinel3/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    16337 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/drb/addons/metadata/sentinel3/cortex.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:35:59.350916 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6914 2023-05-17 14:35:59.000000 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-17 14:35:59.000000 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:35:59.000000 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-17 14:35:59.000000 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:35:58.000000 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-17 14:35:59.000000 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 14:35:59.000000 drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-17 14:35:59.350916 drb-metadata-sentinel3-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:35:59.350916 drb-metadata-sentinel3-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5552 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/tests/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-17 09:31:17.000000 drb-metadata-sentinel3-1.2.0/versioneer.py
```

### Comparing `drb-metadata-sentinel3-1.1.0/PKG-INFO` & `drb-metadata-sentinel3-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel3
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sentinel-3 Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-3
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # DRB Metadata Sentinel 3
 This DRB addon allowing to extract metadata of *Sentinel-3* products.
 
 see:
  - [Sentinel-3](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-3)
  - [drb-topic-sentinel3](https://gitlab.com/drb-python/topics/sentinel3)
@@ -127,8 +128,7 @@
 | processorName            |
 | processorVersion         |
 | beginningDateTime        |
 | endingDateTime           |
 | productType              |
 | timeliness               |
 | baselineCollection       |
-
```

### Comparing `drb-metadata-sentinel3-1.1.0/README.md` & `drb-metadata-sentinel3-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel3-1.1.0/drb/addons/metadata/sentinel3/cortex.yaml` & `drb-metadata-sentinel3-1.2.0/drb/addons/metadata/sentinel3/cortex.yaml`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel3-1.1.0/drb_metadata_sentinel3.egg-info/PKG-INFO` & `drb-metadata-sentinel3-1.2.0/drb_metadata_sentinel3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel3
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sentinel-3 Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-3
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # DRB Metadata Sentinel 3
 This DRB addon allowing to extract metadata of *Sentinel-3* products.
 
 see:
  - [Sentinel-3](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-3)
  - [drb-topic-sentinel3](https://gitlab.com/drb-python/topics/sentinel3)
@@ -127,8 +128,7 @@
 | processorName            |
 | processorVersion         |
 | beginningDateTime        |
 | endingDateTime           |
 | productType              |
 | timeliness               |
 | baselineCollection       |
-
```

### Comparing `drb-metadata-sentinel3-1.1.0/versioneer.py` & `drb-metadata-sentinel3-1.2.0/versioneer.py`

 * *Files identical despite different names*

