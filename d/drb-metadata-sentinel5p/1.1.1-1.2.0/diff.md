# Comparing `tmp/drb-metadata-sentinel5p-1.1.1.tar.gz` & `tmp/drb-metadata-sentinel5p-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-metadata-sentinel5p-1.1.1.tar", last modified: Wed Mar 15 16:20:44 2023, max compression
+gzip compressed data, was "drb-metadata-sentinel5p-1.2.0.tar", last modified: Wed May 17 13:23:42 2023, max compression
```

## Comparing `drb-metadata-sentinel5p-1.1.1.tar` & `drb-metadata-sentinel5p-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:20:44.040446 drb-metadata-sentinel5p-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 16:19:25.000000 drb-metadata-sentinel5p-1.1.1/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-04 17:15:53.000000 drb-metadata-sentinel5p-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-15 16:20:44.040446 drb-metadata-sentinel5p-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1097 2022-09-15 15:23:25.000000 drb-metadata-sentinel5p-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:20:44.020445 drb-metadata-sentinel5p-1.1.1/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:20:44.020445 drb-metadata-sentinel5p-1.1.1/drb/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:20:44.020445 drb-metadata-sentinel5p-1.1.1/drb/addons/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:20:44.040446 drb-metadata-sentinel5p-1.1.1/drb/addons/metadata/sentinel5p/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-04 17:15:53.000000 drb-metadata-sentinel5p-1.1.1/drb/addons/metadata/sentinel5p/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-15 16:20:44.040446 drb-metadata-sentinel5p-1.1.1/drb/addons/metadata/sentinel5p/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    20397 2023-01-04 17:16:00.000000 drb-metadata-sentinel5p-1.1.1/drb/addons/metadata/sentinel5p/cortex.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:20:44.040446 drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-15 16:20:43.000000 drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-03-15 16:20:43.000000 drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 16:20:43.000000 drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-15 16:20:43.000000 drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-03-15 16:20:43.000000 drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-15 16:20:43.000000 drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-03-15 13:54:59.000000 drb-metadata-sentinel5p-1.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-03-15 16:20:44.040446 drb-metadata-sentinel5p-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-03-10 09:44:02.000000 drb-metadata-sentinel5p-1.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    81180 2022-09-15 15:23:26.000000 drb-metadata-sentinel5p-1.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:23:42.415332 drb-metadata-sentinel5p-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-05-17 13:23:42.415332 drb-metadata-sentinel5p-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:23:42.291330 drb-metadata-sentinel5p-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:23:42.291330 drb-metadata-sentinel5p-1.2.0/drb/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:23:42.291330 drb-metadata-sentinel5p-1.2.0/drb/addons/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:23:42.419332 drb-metadata-sentinel5p-1.2.0/drb/addons/metadata/sentinel5p/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/drb/addons/metadata/sentinel5p/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 13:23:42.419332 drb-metadata-sentinel5p-1.2.0/drb/addons/metadata/sentinel5p/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    20397 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/drb/addons/metadata/sentinel5p/cortex.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:23:42.355331 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-05-17 13:23:42.000000 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      591 2023-05-17 13:23:42.000000 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 13:23:42.000000 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-17 13:23:42.000000 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 13:23:41.000000 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-17 13:23:42.000000 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 13:23:42.000000 drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-05-17 13:23:42.419332 drb-metadata-sentinel5p-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-17 11:54:42.000000 drb-metadata-sentinel5p-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:23:42.355331 drb-metadata-sentinel5p-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-17 11:54:46.000000 drb-metadata-sentinel5p-1.2.0/tests/test_sentinel5p_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2023-05-17 11:54:46.000000 drb-metadata-sentinel5p-1.2.0/versioneer.py
```

### Comparing `drb-metadata-sentinel5p-1.1.1/LICENCE.txt` & `drb-metadata-sentinel5p-1.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel5p-1.1.1/PKG-INFO` & `drb-metadata-sentinel5p-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel5p
-Version: 1.1.1
+Version: 1.2.0
 Summary: Sentinel-5P Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-5p
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-5p
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # DRB Sentinel-5P Metadata AddOn
 This addon allowing to enrich the `Sentinel-5P Product` topic with its metadata
 derivative topics also. 
@@ -45,9 +43,7 @@
 |--------------------------------------------------|
 | platformShortName                                |
 | instrumentShortName                              |
 | processingLevel                                  |
 | endingDateTime                                   |
 | beginningDateTime                                |
 | productType                                      |
-
-
```

### Comparing `drb-metadata-sentinel5p-1.1.1/README.md` & `drb-metadata-sentinel5p-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel5p-1.1.1/drb/addons/metadata/sentinel5p/cortex.yaml` & `drb-metadata-sentinel5p-1.2.0/drb/addons/metadata/sentinel5p/cortex.yaml`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel5p-1.1.1/drb_metadata_sentinel5p.egg-info/PKG-INFO` & `drb-metadata-sentinel5p-1.2.0/drb_metadata_sentinel5p.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel5p
-Version: 1.1.1
+Version: 1.2.0
 Summary: Sentinel-5P Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-5p
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-5p
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # DRB Sentinel-5P Metadata AddOn
 This addon allowing to enrich the `Sentinel-5P Product` topic with its metadata
 derivative topics also. 
@@ -45,9 +43,7 @@
 |--------------------------------------------------|
 | platformShortName                                |
 | instrumentShortName                              |
 | processingLevel                                  |
 | endingDateTime                                   |
 | beginningDateTime                                |
 | productType                                      |
-
-
```

### Comparing `drb-metadata-sentinel5p-1.1.1/versioneer.py` & `drb-metadata-sentinel5p-1.2.0/versioneer.py`

 * *Files identical despite different names*

