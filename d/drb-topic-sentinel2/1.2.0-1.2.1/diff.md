# Comparing `tmp/drb-topic-sentinel2-1.2.0.tar.gz` & `tmp/drb-topic-sentinel2-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-sentinel2-1.2.0.tar", last modified: Tue May 16 13:28:20 2023, max compression
+gzip compressed data, was "drb-topic-sentinel2-1.2.1.tar", last modified: Wed May 17 15:45:05 2023, max compression
```

## Comparing `drb-topic-sentinel2-1.2.0.tar` & `drb-topic-sentinel2-1.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:45:26.000000 drb-topic-sentinel2-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6040 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5572 2022-07-25 14:59:39.000000 drb-topic-sentinel2-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.738412 drb-topic-sentinel2-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.738412 drb-topic-sentinel2-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4448 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2171 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5290 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5030 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3875 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6040 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      788 2022-07-06 15:33:55.000000 drb-topic-sentinel2-1.2.0/tests/test_sentinel2_topics.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:45:26.000000 drb-topic-sentinel2-1.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5572 2022-07-25 14:59:39.000000 drb-topic-sentinel2-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.441566 drb-topic-sentinel2-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.441566 drb-topic-sentinel2-1.2.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.449566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.449566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2217 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5168 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3875 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 15:45:04.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2022-07-06 15:33:55.000000 drb-topic-sentinel2-1.2.1/tests/test_sentinel2_topics.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/versioneer.py
```

### Comparing `drb-topic-sentinel2-1.2.0/LICENCE.txt` & `drb-topic-sentinel2-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.0/PKG-INFO` & `drb-topic-sentinel2-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel2
-Version: 1.2.0
+Version: 1.2.1
 Summary: Sentinel-2 topic for DRB Python
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel2
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `drb-topic-sentinel2-1.2.0/README.md` & `drb-topic-sentinel2-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/cortex.yml` & `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/cortex.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 signatures:
   - name: S2[A|B|_]_...._(AUX|GIP)_.*
 ---
 ###############################################################################
 # Sentinel-2 AUX SAD product
 ###############################################################################
 id: be45c266-f23d-11ec-b939-0242ac120002
-subClassOf: 02318e52-fd2d-11ec-b939-0242ac120002
+subClassOf:
+  id: 02318e52-fd2d-11ec-b939-0242ac120002
+  override: true
 label: Sentinel-2 Auxiliary SAD PDI
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._AUX_SADATA_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}_......._.._..\.tar
 ---
 ###############################################################################
 # Sentinel-2 AUX ECMWFD & UT1UTC product
 ###############################################################################
 id: 0cacd114-0c20-11ed-861d-0242ac120002
-subClassOf: 02318e52-fd2d-11ec-b939-0242ac120002
+subClassOf:
+  id: 02318e52-fd2d-11ec-b939-0242ac120002
+  override: true
 label: Sentinel-2 Auxiliary ECMWFD and UT1UTC product
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB_]_...._AUX_(ECMWFD|UT1UTC)_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.TGZ
 ---
 ###############################################################################
@@ -50,15 +54,17 @@
 signatures:
   - name: S2[AB_]_...._AUX_UT1UTC_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.TGZ
 ---
 ###############################################################################
 # Sentinel-2 AUX RESORB & PREORB
 ###############################################################################
 id: 8bc2ca58-0c25-11ed-861d-0242ac120002
-subClassOf: 02318e52-fd2d-11ec-b939-0242ac120002
+subClassOf:
+  id: 02318e52-fd2d-11ec-b939-0242ac120002
+  override: true
 factory: xml
 label: Sentinel-2 EOF RESORB & PREORB
 category: FORMATTING
 signatures:
   - name: S2(A|B)_...._AUX_RESORB_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.EOF
 ---
 ###############################################################################
@@ -81,15 +87,17 @@
 signatures:
   - name: S2(A|B)_...._AUX_PREORB_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.EOF
 ---
 ###############################################################################
 # Sentinel-2 AUX GIP product
 ###############################################################################
 id: 7de4ab0c-fd40-11ec-b939-0242ac120002
-subClassOf: 02318e52-fd2d-11ec-b939-0242ac120002
+subClassOf:
+  id: 02318e52-fd2d-11ec-b939-0242ac120002
+  override: true
 label: Sentinel-2 Auxiliary GIP
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB_]_...._GIP_......_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}_...\.TGZ
 ---
 ###############################################################################
```

### Comparing `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/cortex.yml` & `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/cortex.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 signatures:
   - name: S2[AB]_...._MSI_L0__LT.*_N[0-9]{2}\.[0-9]{2}.*
 ---
 ###############################################################################
 # Sentinel-2 PDI Level-1C TCI
 ###############################################################################
 id: ff9720b6-f2f1-11ec-b939-0242ac120002
-subClassOf: 172f47a2-f307-11ec-b939-0242ac120002
 label: Sentinel-2 Level-1C Tile Image File
+subClassOf:
+  id: 172f47a2-f307-11ec-b939-0242ac120002
+  override: true
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L1C_TC.*_N[0-9]{2}\.[0-9]{2}\.tar$
 ---
 ###############################################################################
 # Sentinel-2 PDI Level-1C TCI (exotic product)
@@ -39,13 +41,15 @@
 signatures:
   - name: S2[AB]_...._MSI_L1C_TC.*_N[0-9]{2}\.[0-9]{2}\.jp2
 ---
 ###############################################################################
 # Sentinel-2 HKTM Level-0
 ###############################################################################
 id: 3f43fa3e-f2f9-11ec-b939-0242ac120002
-subClassOf: 329762ec-e1a8-11ec-8fea-0242ac120002
+subClassOf:
+  id: 329762ec-e1a8-11ec-8fea-0242ac120002
+  override: true
 label: Sentinel-2 Level-0 HKTM
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._PRD_HKTM___[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}_[0-9]{4}\.tar
```

### Comparing `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/cortex.yml` & `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/cortex.yml`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 signatures:
   - name: S2[AB]_...._MSI_L0__DS.*_N[0-9]{2}\.[0-9]{2}$
 ---
 ###############################################################################
 # Sentinel-2 Level-0 Tar Datastrip
 ###############################################################################
 id: 746dc578-0bf4-11ed-861d-0242ac120002
-subClassOf: fad132d2-f2fc-11ec-b939-0242ac120002
+subClassOf:
+  id: fad132d2-f2fc-11ec-b939-0242ac120002
+  override: true
 factory: tar
 label: Sentinel-2 Level-0 Datastrip tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L0__DS.*_N[0-9]{2}\.[0-9]{2}\.tar
 ---
 ###############################################################################
@@ -39,15 +41,17 @@
 signatures:
   - name: S2[AB]_...._MSI_L1A_DS.*_N[0-9]{2}\.[0-9]{2}$
 ---
 ###############################################################################
 # Sentinel-2 Level-1A tar Datastrip
 ###############################################################################
 id: 3f1ab53c-0bf6-11ed-861d-0242ac120002
-subClassOf: fad132d2-f2fc-11ec-b939-0242ac120002
+subClassOf:
+  id: fad132d2-f2fc-11ec-b939-0242ac120002
+  override: true
 factory: tar
 label: Sentinel-2 Level-1A Datastrip tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L1A_DS.*_N[0-9]{2}\.[0-9]{2}\.tar
 ---
 ###############################################################################
@@ -60,15 +64,17 @@
 signatures:
   - name: S2[AB]_...._MSI_L1B_DS.*_N[0-9]{2}\.[0-9]{2}$
 ---
 ###############################################################################
 # Sentinel-2 Level-1B tar Datastrip
 ###############################################################################
 id: 4784eb66-0bf6-11ed-861d-0242ac120002
-subClassOf: fad132d2-f2fc-11ec-b939-0242ac120002
+subClassOf:
+  id: fad132d2-f2fc-11ec-b939-0242ac120002
+  override: true
 factory: tar
 label: Sentinel-2 Level-1B Datastrip tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L1B_DS.*_N[0-9]{2}\.[0-9]{2}\.tar
 ---
 ###############################################################################
@@ -81,15 +87,17 @@
 signatures:
   - name: S2[AB]_...._MSI_L1C_DS.*_N[0-9]{2}\.[0-9]{2}$|DS_...._[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]_S[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]$
 ---
 ###############################################################################
 # Sentinel-2 Level-1C tar Datastrip
 ###############################################################################
 id: 50448cde-0bf6-11ed-861d-0242ac120002
-subClassOf: fad132d2-f2fc-11ec-b939-0242ac120002
+subClassOf:
+  id: fad132d2-f2fc-11ec-b939-0242ac120002
+  override: true
 label: Sentinel-2 Level-1C Datastrip
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L1C_DS.*_N[0-9]{2}\.[0-9]{2}\.tar|DS_...._[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]_S[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]\.tar
 ---
 ###############################################################################
@@ -102,13 +110,15 @@
 signatures:
   - name: S2[AB]_...._MSI_L2A_DS.*_N[0-9]{2}\.[0-9]{2}$|DS_...._[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]_S[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]$
 ---
 ###############################################################################
 # Sentinel-2 Level-2A tar Datastrip
 ###############################################################################
 id: 564d3d42-0bf6-11ed-861d-0242ac120002
-subClassOf: fad132d2-f2fc-11ec-b939-0242ac120002
+subClassOf:
+  id: fad132d2-f2fc-11ec-b939-0242ac120002
+  override: true
 label: Sentinel-2 Level-2A Datastrip
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L2A_DS.*_N[0-9]{2}\.[0-9]{2}\.tar|DS_...._[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]_S[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]\.tar
```

### Comparing `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/cortex.yml` & `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/cortex.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,37 +18,43 @@
 signatures:
   - name: S2[AB]_...._MSI_L0__GR.*_N[0-9]{2}\.[0-9]{2}$
 ---
 ###############################################################################
 # Sentinel-2 Level-0 tar Granule
 ###############################################################################
 id: aed3f1e8-0bf8-11ed-861d-0242ac120002
-subClassOf: c6da0d68-f23a-11ec-b939-0242ac120002
 label: Sentinel-2 Level-0 Granule tar
+subClassOf:
+  id: c6da0d68-f23a-11ec-b939-0242ac120002
+  override: true
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L0__GR.*_N[0-9]{2}\.[0-9]{2}\.tar
 ---
 ###############################################################################
 # Sentinel-2 Level-1a Granule
 ###############################################################################
 id: beadaaac-f2f6-11ec-b939-0242ac120002
-subClassOf: c6da0d68-f23a-11ec-b939-0242ac120002
+subClassOf:
+  id: c6da0d68-f23a-11ec-b939-0242ac120002
+  override: true
 label: Sentinel-2 Level-1A Granule
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L1A_GR.*_N[0-9]{2}\.[0-9]{2}$
 ---
 ###############################################################################
 # Sentinel-2 Level-1a tar Granule
 ###############################################################################
 id: bec4dfb8-0bf8-11ed-861d-0242ac120002
-subClassOf: c6da0d68-f23a-11ec-b939-0242ac120002
 label: Sentinel-2 Level-1A Granule tar
+subClassOf:
+  id: c6da0d68-f23a-11ec-b939-0242ac120002
+  override: true
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L1A_GR.*_N[0-9]{2}\.[0-9]{2}\.tar
 ---
 ###############################################################################
 # Sentinel-2 Level-1b Granule
@@ -60,16 +66,18 @@
 signatures:
   - name: S2[AB]_...._MSI_L1B_GR.*_N[0-9]{2}\.[0-9]{2}$
 ---
 ###############################################################################
 # Sentinel-2 Level-1b tar Granule
 ###############################################################################
 id: defc1e86-0bf8-11ed-861d-0242ac120002
-subClassOf: c6da0d68-f23a-11ec-b939-0242ac120002
 label: Sentinel-2 Level-1B Granule tar
+subClassOf:
+  id: c6da0d68-f23a-11ec-b939-0242ac120002
+  override: true
 factory: tar
 category: CONTAINER
 signatures:
   - name: S2[AB]_...._MSI_L1B_GR.*_N[0-9]{2}\.[0-9]{2}\.tar
 ---
 ###############################################################################
 # Sentinel-2 Level-1c Granule
@@ -81,16 +89,18 @@
 signatures:
   - name: (S2[AB]_...._MSI_L1C_TL.*_N[0-9]{2}\.[0-9]{2}$|L1C_T....._A[0-9]{6}_[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]$)
 ---
 ###############################################################################
 # Sentinel-2 Level-1c tar Granule
 ###############################################################################
 id: e9d52d0c-0bf8-11ed-861d-0242ac120002
-subClassOf: c6da0d68-f23a-11ec-b939-0242ac120002
 label: Sentinel-2 Level-1C Granule tar
+subClassOf:
+  id: c6da0d68-f23a-11ec-b939-0242ac120002
+  override: true
 factory: tar
 category: CONTAINER
 signatures:
   - name: (S2[AB]_...._MSI_L1C_TL.*_N[0-9]{2}\.[0-9]{2}\.tar|L1C_T....._A[0-9]{6}_[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]\.tar)
 ---
 ###############################################################################
 # Sentinel-2 Level-2a Granule
@@ -102,13 +112,15 @@
 signatures:
   - name: (S2[AB]_...._MSI_L2A_TL.*_N[0-9]{2}\.[0-9]{2}$|L2A_T....._A[0-9]{6}_[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]$)
 ---
 ###############################################################################
 # Sentinel-2 Level-2a tar Granule
 ###############################################################################
 id: 116c5804-0bf9-11ed-861d-0242ac120002
-subClassOf: c6da0d68-f23a-11ec-b939-0242ac120002
 label: Sentinel-2 Level-2A Granule tar
+subClassOf:
+  id: c6da0d68-f23a-11ec-b939-0242ac120002
+  override: true
 factory: tar
 category: CONTAINER
 signatures:
   - name: (S2[AB]_...._MSI_L2A_TL.*_N[0-9]{2}\.[0-9]{2}\.tar|L2A_T....._A[0-9]{6}_[0-9]{4}[0-1][0-9][0-3][0-9]T[0-2][0-9][0-6][0-9][0-6][0-9]\.tar)
```

### Comparing `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/cortex.yml` & `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/PKG-INFO` & `drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel2
-Version: 1.2.0
+Version: 1.2.1
 Summary: Sentinel-2 topic for DRB Python
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel2
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/SOURCES.txt` & `drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.0/setup.cfg` & `drb-topic-sentinel2-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.0/tests/test_sentinel2_topics.py` & `drb-topic-sentinel2-1.2.1/tests/test_sentinel2_topics.py`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.0/versioneer.py` & `drb-topic-sentinel2-1.2.1/versioneer.py`

 * *Files identical despite different names*

