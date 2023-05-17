# Comparing `tmp/moredata-0.2.0.tar.gz` & `tmp/moredata-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moredata-0.2.0.tar", last modified: Tue May 16 15:07:30 2023, max compression
+gzip compressed data, was "moredata-0.2.1.tar", last modified: Wed May 17 01:10:59 2023, max compression
```

## Comparing `moredata-0.2.0.tar` & `moredata-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.2.0/LICENSE.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      457 2023-05-16 15:07:30.247055 moredata-0.2.0/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1892 2023-05-16 14:20:50.000000 moredata-0.2.0/README.md
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/datasets/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      633 2022-08-10 22:04:01.000000 moredata-0.2.0/moredata/datasets/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/enricher/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/enricher/api_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.2.0/moredata/enricher/api_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.2.0/moredata/enricher/api_connector/api_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/enricher/elasticsearch_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/index_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/pipeline_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/policy_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.2.0/moredata/enricher/enricher.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2340 2023-03-24 00:39:22.000000 moredata-0.2.0/moredata/enricher/enricher_builder.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/enricher/osm/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/osm/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5807 2023-05-16 14:15:55.000000 moredata-0.2.0/moredata/enricher/osm/functional_region_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     7398 2023-05-16 14:22:06.000000 moredata-0.2.0/moredata/enricher/osm/osm_places_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/enricher/sql_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/sql_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.2.0/moredata/enricher/sql_connector/sql_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/models/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/models/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1807 2023-05-16 14:17:33.000000 moredata-0.2.0/moredata/models/data.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/parser/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1168 2023-05-16 14:27:49.000000 moredata-0.2.0/moredata/parser/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/tests/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.2.0/moredata/tests/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/tests/test_datasets.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/utils/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2023-05-16 14:22:23.000000 moredata-0.2.0/moredata/utils/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2023-05-16 14:22:23.000000 moredata-0.2.0/moredata/utils/osm_downloader.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata.egg-info/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      457 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1170 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/SOURCES.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/dependency_links.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1299 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/requires.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/top_level.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2023-05-16 15:07:30.247055 moredata-0.2.0/setup.cfg
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1546 2023-05-16 15:00:39.000000 moredata-0.2.0/setup.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.823390 moredata-0.2.1/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.2.1/LICENSE.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 01:10:59.823390 moredata-0.2.1/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1892 2023-05-16 15:16:10.000000 moredata-0.2.1/README.md
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.819390 moredata-0.2.1/moredata/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2023-05-17 01:09:13.000000 moredata-0.2.1/moredata/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.819390 moredata-0.2.1/moredata/datasets/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      667 2023-05-16 15:16:10.000000 moredata-0.2.1/moredata/datasets/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.819390 moredata-0.2.1/moredata/enricher/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.2.1/moredata/enricher/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.819390 moredata-0.2.1/moredata/enricher/api_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.2.1/moredata/enricher/api_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.2.1/moredata/enricher/api_connector/api_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.819390 moredata-0.2.1/moredata/enricher/elasticsearch_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.2.1/moredata/enricher/elasticsearch_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.2.1/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.2.1/moredata/enricher/elasticsearch_connector/index_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.2.1/moredata/enricher/elasticsearch_connector/pipeline_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.2.1/moredata/enricher/elasticsearch_connector/policy_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.2.1/moredata/enricher/enricher.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2340 2023-05-16 15:16:10.000000 moredata-0.2.1/moredata/enricher/enricher_builder.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.823390 moredata-0.2.1/moredata/enricher/osm/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.2.1/moredata/enricher/osm/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5807 2023-05-16 15:16:10.000000 moredata-0.2.1/moredata/enricher/osm/functional_region_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     7398 2023-05-16 15:16:10.000000 moredata-0.2.1/moredata/enricher/osm/osm_places_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.823390 moredata-0.2.1/moredata/enricher/sql_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.2.1/moredata/enricher/sql_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.2.1/moredata/enricher/sql_connector/sql_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.823390 moredata-0.2.1/moredata/models/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.2.1/moredata/models/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1807 2023-05-16 15:16:10.000000 moredata-0.2.1/moredata/models/data.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.823390 moredata-0.2.1/moredata/parser/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1168 2023-05-16 15:16:10.000000 moredata-0.2.1/moredata/parser/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.823390 moredata-0.2.1/moredata/tests/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.2.1/moredata/tests/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.2.1/moredata/tests/test_datasets.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.823390 moredata-0.2.1/moredata/utils/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2023-05-16 14:22:23.000000 moredata-0.2.1/moredata/utils/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2023-05-16 14:22:23.000000 moredata-0.2.1/moredata/utils/osm_downloader.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:10:59.819390 moredata-0.2.1/moredata.egg-info/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 01:10:59.000000 moredata-0.2.1/moredata.egg-info/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1170 2023-05-17 01:10:59.000000 moredata-0.2.1/moredata.egg-info/SOURCES.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2023-05-17 01:10:59.000000 moredata-0.2.1/moredata.egg-info/dependency_links.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      225 2023-05-17 01:10:59.000000 moredata-0.2.1/moredata.egg-info/requires.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2023-05-17 01:10:59.000000 moredata-0.2.1/moredata.egg-info/top_level.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2023-05-17 01:10:59.823390 moredata-0.2.1/setup.cfg
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1888 2023-05-17 01:10:44.000000 moredata-0.2.1/setup.py
```

### Comparing `moredata-0.2.0/LICENSE.txt` & `moredata-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/README.md` & `moredata-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/__init__.py` & `moredata-0.2.1/moredata/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/datasets/__init__.py` & `moredata-0.2.1/moredata/datasets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 
 __all__ = ["available", "get_path"]
 
 _module_path = os.path.dirname(__file__)
 _available_csv = {
-    "airbnb-berlin-main": "airbnb-berlin-main.csv",
-    "airbnb-berlin-host": "airbnb-berlin-host.csv",
-    "airbnb-berlin-extra": "airbnb-berlin-extra.csv",
+    "airbnb-berlin-main": "./airbnb/airbnb-berlin-main.csv",
+    "airbnb-berlin-host": "./airbnb/airbnb-berlin-host.csv",
+    "airbnb-berlin-extra": "./airbnb/airbnb-berlin-extra.csv",
 }
 available = list(_available_csv.keys())
 
 
 def get_path(dataset):
     if dataset in _available_csv:
-        return os.path.abspath(os.path.join(_module_path, dataset + ".csv"))
+        return os.path.abspath(os.path.join(_module_path, _available_csv[dataset]))
     else:
         msg = "The dataset '{data}' is not available. ".format(data=dataset)
         msg += "Available datasets are {}".format(", ".join(available))
         raise ValueError(msg)
```

### Comparing `moredata-0.2.0/moredata/enricher/api_connector/api_connector.py` & `moredata-0.2.1/moredata/enricher/api_connector/api_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py` & `moredata-0.2.1/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/elasticsearch_connector/index_handler.py` & `moredata-0.2.1/moredata/enricher/elasticsearch_connector/index_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/elasticsearch_connector/pipeline_handler.py` & `moredata-0.2.1/moredata/enricher/elasticsearch_connector/pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/elasticsearch_connector/policy_handler.py` & `moredata-0.2.1/moredata/enricher/elasticsearch_connector/policy_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/enricher.py` & `moredata-0.2.1/moredata/enricher/enricher.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/enricher_builder.py` & `moredata-0.2.1/moredata/enricher/enricher_builder.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/osm/functional_region_connector.py` & `moredata-0.2.1/moredata/enricher/osm/functional_region_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/osm/osm_places_connector.py` & `moredata-0.2.1/moredata/enricher/osm/osm_places_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/enricher/sql_connector/sql_connector.py` & `moredata-0.2.1/moredata/enricher/sql_connector/sql_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/models/data.py` & `moredata-0.2.1/moredata/models/data.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/parser/__init__.py` & `moredata-0.2.1/moredata/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/utils/__init__.py` & `moredata-0.2.1/moredata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata/utils/osm_downloader.py` & `moredata-0.2.1/moredata/utils/osm_downloader.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.0/moredata.egg-info/SOURCES.txt` & `moredata-0.2.1/moredata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

