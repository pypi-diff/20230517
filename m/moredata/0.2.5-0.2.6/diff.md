# Comparing `tmp/moredata-0.2.5.tar.gz` & `tmp/moredata-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moredata-0.2.5.tar", last modified: Wed May 17 03:02:18 2023, max compression
+gzip compressed data, was "moredata-0.2.6.tar", last modified: Wed May 17 16:36:44 2023, max compression
```

## Comparing `moredata-0.2.5.tar` & `moredata-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.599662 moredata-0.2.5/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.2.5/LICENSE.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 03:02:18.599662 moredata-0.2.5/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1892 2023-05-16 15:16:10.000000 moredata-0.2.5/README.md
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.595662 moredata-0.2.5/moredata/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2023-05-17 01:09:13.000000 moredata-0.2.5/moredata/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.595662 moredata-0.2.5/moredata/datasets/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      667 2023-05-16 15:16:10.000000 moredata-0.2.5/moredata/datasets/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.595662 moredata-0.2.5/moredata/enricher/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.2.5/moredata/enricher/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.595662 moredata-0.2.5/moredata/enricher/api_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.2.5/moredata/enricher/api_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.2.5/moredata/enricher/api_connector/api_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.595662 moredata-0.2.5/moredata/enricher/elasticsearch_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.2.5/moredata/enricher/elasticsearch_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.2.5/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.2.5/moredata/enricher/elasticsearch_connector/index_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.2.5/moredata/enricher/elasticsearch_connector/pipeline_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.2.5/moredata/enricher/elasticsearch_connector/policy_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.2.5/moredata/enricher/enricher.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2340 2023-05-16 15:16:10.000000 moredata-0.2.5/moredata/enricher/enricher_builder.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.599662 moredata-0.2.5/moredata/enricher/osm/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.2.5/moredata/enricher/osm/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5807 2023-05-16 15:16:10.000000 moredata-0.2.5/moredata/enricher/osm/functional_region_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     7763 2023-05-17 03:01:52.000000 moredata-0.2.5/moredata/enricher/osm/osm_places_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.599662 moredata-0.2.5/moredata/enricher/sql_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.2.5/moredata/enricher/sql_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.2.5/moredata/enricher/sql_connector/sql_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.599662 moredata-0.2.5/moredata/models/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.2.5/moredata/models/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1807 2023-05-16 15:16:10.000000 moredata-0.2.5/moredata/models/data.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.599662 moredata-0.2.5/moredata/parser/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1168 2023-05-16 15:16:10.000000 moredata-0.2.5/moredata/parser/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.599662 moredata-0.2.5/moredata/tests/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.2.5/moredata/tests/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.2.5/moredata/tests/test_datasets.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.599662 moredata-0.2.5/moredata/utils/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2023-05-16 14:22:23.000000 moredata-0.2.5/moredata/utils/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2023-05-16 14:22:23.000000 moredata-0.2.5/moredata/utils/osm_downloader.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 03:02:18.595662 moredata-0.2.5/moredata.egg-info/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 03:02:18.000000 moredata-0.2.5/moredata.egg-info/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1170 2023-05-17 03:02:18.000000 moredata-0.2.5/moredata.egg-info/SOURCES.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2023-05-17 03:02:18.000000 moredata-0.2.5/moredata.egg-info/dependency_links.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      225 2023-05-17 03:02:18.000000 moredata-0.2.5/moredata.egg-info/requires.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2023-05-17 03:02:18.000000 moredata-0.2.5/moredata.egg-info/top_level.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2023-05-17 03:02:18.599662 moredata-0.2.5/setup.cfg
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1888 2023-05-17 03:02:16.000000 moredata-0.2.5/setup.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.531571 moredata-0.2.6/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.2.6/LICENSE.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 16:36:44.531571 moredata-0.2.6/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1892 2023-05-16 15:16:10.000000 moredata-0.2.6/README.md
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2023-05-17 01:09:13.000000 moredata-0.2.6/moredata/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/datasets/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      667 2023-05-16 15:16:10.000000 moredata-0.2.6/moredata/datasets/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/enricher/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.2.6/moredata/enricher/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/enricher/api_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.2.6/moredata/enricher/api_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.2.6/moredata/enricher/api_connector/api_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/enricher/elasticsearch_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.2.6/moredata/enricher/elasticsearch_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.2.6/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.2.6/moredata/enricher/elasticsearch_connector/index_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.2.6/moredata/enricher/elasticsearch_connector/pipeline_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.2.6/moredata/enricher/elasticsearch_connector/policy_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.2.6/moredata/enricher/enricher.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2340 2023-05-16 15:16:10.000000 moredata-0.2.6/moredata/enricher/enricher_builder.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/enricher/osm/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.2.6/moredata/enricher/osm/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5807 2023-05-16 15:16:10.000000 moredata-0.2.6/moredata/enricher/osm/functional_region_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     7764 2023-05-17 16:36:23.000000 moredata-0.2.6/moredata/enricher/osm/osm_places_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/enricher/sql_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.2.6/moredata/enricher/sql_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.2.6/moredata/enricher/sql_connector/sql_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/models/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.2.6/moredata/models/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1807 2023-05-16 15:16:10.000000 moredata-0.2.6/moredata/models/data.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/parser/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1168 2023-05-16 15:16:10.000000 moredata-0.2.6/moredata/parser/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata/tests/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.2.6/moredata/tests/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.2.6/moredata/tests/test_datasets.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.531571 moredata-0.2.6/moredata/utils/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2023-05-16 14:22:23.000000 moredata-0.2.6/moredata/utils/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2023-05-16 14:22:23.000000 moredata-0.2.6/moredata/utils/osm_downloader.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 16:36:44.527571 moredata-0.2.6/moredata.egg-info/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 16:36:44.000000 moredata-0.2.6/moredata.egg-info/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1170 2023-05-17 16:36:44.000000 moredata-0.2.6/moredata.egg-info/SOURCES.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2023-05-17 16:36:44.000000 moredata-0.2.6/moredata.egg-info/dependency_links.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      225 2023-05-17 16:36:44.000000 moredata-0.2.6/moredata.egg-info/requires.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2023-05-17 16:36:44.000000 moredata-0.2.6/moredata.egg-info/top_level.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2023-05-17 16:36:44.531571 moredata-0.2.6/setup.cfg
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1888 2023-05-17 16:36:34.000000 moredata-0.2.6/setup.py
```

### Comparing `moredata-0.2.5/LICENSE.txt` & `moredata-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/README.md` & `moredata-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/__init__.py` & `moredata-0.2.6/moredata/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/datasets/__init__.py` & `moredata-0.2.6/moredata/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/api_connector/api_connector.py` & `moredata-0.2.6/moredata/enricher/api_connector/api_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py` & `moredata-0.2.6/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/elasticsearch_connector/index_handler.py` & `moredata-0.2.6/moredata/enricher/elasticsearch_connector/index_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/elasticsearch_connector/pipeline_handler.py` & `moredata-0.2.6/moredata/enricher/elasticsearch_connector/pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/elasticsearch_connector/policy_handler.py` & `moredata-0.2.6/moredata/enricher/elasticsearch_connector/policy_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/enricher.py` & `moredata-0.2.6/moredata/enricher/enricher.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/enricher_builder.py` & `moredata-0.2.6/moredata/enricher/enricher_builder.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/osm/functional_region_connector.py` & `moredata-0.2.6/moredata/enricher/osm/functional_region_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/enricher/osm/osm_places_connector.py` & `moredata-0.2.6/moredata/enricher/osm/osm_places_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
         sj["geometry"] = sj["geometry_not_buffered"]
         sj = sj.drop(columns=["geometry_not_buffered"])
 
         for column in ['index_left', 'index_right']:
             try:
                 sj = sj.drop(column, axis=1)
-            except KeyError:
+            except Exception:
                 pass
 
         return DaskGeopandasData.from_dask_geodataframe(sj)
 
     def enrich(self, data, **kwargs):
         """Method overrided of interface. This method do enrichment using OSM data as a enricher. It walk through the keys to reach at the data that will be used to intersect the polygons. It uses a R tree to index polygons and search faster. If the radius attribute is passed the algorithm returns all polygons that intersect the point buffered with this radius else the algorithm returns all polygons that contains the point.
```

### Comparing `moredata-0.2.5/moredata/enricher/sql_connector/sql_connector.py` & `moredata-0.2.6/moredata/enricher/sql_connector/sql_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/models/data.py` & `moredata-0.2.6/moredata/models/data.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/parser/__init__.py` & `moredata-0.2.6/moredata/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/utils/__init__.py` & `moredata-0.2.6/moredata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata/utils/osm_downloader.py` & `moredata-0.2.6/moredata/utils/osm_downloader.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/moredata.egg-info/SOURCES.txt` & `moredata-0.2.6/moredata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moredata-0.2.5/setup.py` & `moredata-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         "jinja2==2.11.1",
         "sphinxcontrib-napoleon==0.7",
     ]
 
 setup(
     name="moredata",
     url="https://https://github.com/NESPEDUFV/more-data",
-    download_url="https://github.com/NESPEDUFV/more-data/archive/v0.2.5.tar.gz",
-    version="0.2.5",
+    download_url="https://github.com/NESPEDUFV/more-data/archive/v0.2.6.tar.gz",
+    version="0.2.6",
     packages=find_packages(where="."),
     python_requires=">=3.8",
     install_requires=dependencies + elasticsearch + sql + json + osm,
     # extras_require={
     #     "complete": dependencies + elasticsearch + sql + json + osm,
     #     "osm": dependencies + osm,
     #     "elasticsearch": dependencies + elasticsearch,
```

