# Comparing `tmp/moredata-0.2.2.tar.gz` & `tmp/moredata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moredata-0.2.2.tar", last modified: Wed May 17 01:16:20 2023, max compression
+gzip compressed data, was "moredata-0.2.3.tar", last modified: Wed May 17 01:55:22 2023, max compression
```

## Comparing `moredata-0.2.2.tar` & `moredata-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.2.2/LICENSE.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 01:16:20.413640 moredata-0.2.2/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1892 2023-05-16 15:16:10.000000 moredata-0.2.2/README.md
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.409654 moredata-0.2.2/moredata/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2023-05-17 01:09:13.000000 moredata-0.2.2/moredata/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.409654 moredata-0.2.2/moredata/datasets/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      667 2023-05-16 15:16:10.000000 moredata-0.2.2/moredata/datasets/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.409654 moredata-0.2.2/moredata/enricher/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.2.2/moredata/enricher/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.409654 moredata-0.2.2/moredata/enricher/api_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.2.2/moredata/enricher/api_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.2.2/moredata/enricher/api_connector/api_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/moredata/enricher/elasticsearch_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.2.2/moredata/enricher/elasticsearch_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.2.2/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.2.2/moredata/enricher/elasticsearch_connector/index_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.2.2/moredata/enricher/elasticsearch_connector/pipeline_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.2.2/moredata/enricher/elasticsearch_connector/policy_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.2.2/moredata/enricher/enricher.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2340 2023-05-16 15:16:10.000000 moredata-0.2.2/moredata/enricher/enricher_builder.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/moredata/enricher/osm/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.2.2/moredata/enricher/osm/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5807 2023-05-16 15:16:10.000000 moredata-0.2.2/moredata/enricher/osm/functional_region_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     7398 2023-05-16 15:16:10.000000 moredata-0.2.2/moredata/enricher/osm/osm_places_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/moredata/enricher/sql_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.2.2/moredata/enricher/sql_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.2.2/moredata/enricher/sql_connector/sql_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/moredata/models/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.2.2/moredata/models/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1807 2023-05-16 15:16:10.000000 moredata-0.2.2/moredata/models/data.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/moredata/parser/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1168 2023-05-16 15:16:10.000000 moredata-0.2.2/moredata/parser/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/moredata/tests/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.2.2/moredata/tests/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.2.2/moredata/tests/test_datasets.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.413640 moredata-0.2.2/moredata/utils/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2023-05-16 14:22:23.000000 moredata-0.2.2/moredata/utils/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2023-05-16 14:22:23.000000 moredata-0.2.2/moredata/utils/osm_downloader.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:16:20.409654 moredata-0.2.2/moredata.egg-info/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 01:16:20.000000 moredata-0.2.2/moredata.egg-info/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1170 2023-05-17 01:16:20.000000 moredata-0.2.2/moredata.egg-info/SOURCES.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2023-05-17 01:16:20.000000 moredata-0.2.2/moredata.egg-info/dependency_links.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      225 2023-05-17 01:16:20.000000 moredata-0.2.2/moredata.egg-info/requires.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2023-05-17 01:16:20.000000 moredata-0.2.2/moredata.egg-info/top_level.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2023-05-17 01:16:20.413640 moredata-0.2.2/setup.cfg
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1888 2023-05-17 01:16:18.000000 moredata-0.2.2/setup.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.109209 moredata-0.2.3/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.2.3/LICENSE.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 01:55:22.109209 moredata-0.2.3/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1892 2023-05-16 15:16:10.000000 moredata-0.2.3/README.md
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.105210 moredata-0.2.3/moredata/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2023-05-17 01:09:13.000000 moredata-0.2.3/moredata/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.105210 moredata-0.2.3/moredata/datasets/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      667 2023-05-16 15:16:10.000000 moredata-0.2.3/moredata/datasets/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.105210 moredata-0.2.3/moredata/enricher/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.2.3/moredata/enricher/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.105210 moredata-0.2.3/moredata/enricher/api_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.2.3/moredata/enricher/api_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.2.3/moredata/enricher/api_connector/api_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.105210 moredata-0.2.3/moredata/enricher/elasticsearch_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.2.3/moredata/enricher/elasticsearch_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.2.3/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.2.3/moredata/enricher/elasticsearch_connector/index_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.2.3/moredata/enricher/elasticsearch_connector/pipeline_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.2.3/moredata/enricher/elasticsearch_connector/policy_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.2.3/moredata/enricher/enricher.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2340 2023-05-16 15:16:10.000000 moredata-0.2.3/moredata/enricher/enricher_builder.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.109209 moredata-0.2.3/moredata/enricher/osm/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.2.3/moredata/enricher/osm/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5807 2023-05-16 15:16:10.000000 moredata-0.2.3/moredata/enricher/osm/functional_region_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     7422 2023-05-17 01:54:53.000000 moredata-0.2.3/moredata/enricher/osm/osm_places_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.109209 moredata-0.2.3/moredata/enricher/sql_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.2.3/moredata/enricher/sql_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.2.3/moredata/enricher/sql_connector/sql_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.109209 moredata-0.2.3/moredata/models/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.2.3/moredata/models/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1807 2023-05-16 15:16:10.000000 moredata-0.2.3/moredata/models/data.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.109209 moredata-0.2.3/moredata/parser/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1168 2023-05-16 15:16:10.000000 moredata-0.2.3/moredata/parser/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.109209 moredata-0.2.3/moredata/tests/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.2.3/moredata/tests/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.2.3/moredata/tests/test_datasets.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.109209 moredata-0.2.3/moredata/utils/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2023-05-16 14:22:23.000000 moredata-0.2.3/moredata/utils/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2023-05-16 14:22:23.000000 moredata-0.2.3/moredata/utils/osm_downloader.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-17 01:55:22.105210 moredata-0.2.3/moredata.egg-info/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      296 2023-05-17 01:55:22.000000 moredata-0.2.3/moredata.egg-info/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1170 2023-05-17 01:55:22.000000 moredata-0.2.3/moredata.egg-info/SOURCES.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2023-05-17 01:55:22.000000 moredata-0.2.3/moredata.egg-info/dependency_links.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      225 2023-05-17 01:55:22.000000 moredata-0.2.3/moredata.egg-info/requires.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2023-05-17 01:55:22.000000 moredata-0.2.3/moredata.egg-info/top_level.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2023-05-17 01:55:22.109209 moredata-0.2.3/setup.cfg
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1888 2023-05-17 01:55:21.000000 moredata-0.2.3/setup.py
```

### Comparing `moredata-0.2.2/LICENSE.txt` & `moredata-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/README.md` & `moredata-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/__init__.py` & `moredata-0.2.3/moredata/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/datasets/__init__.py` & `moredata-0.2.3/moredata/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/api_connector/api_connector.py` & `moredata-0.2.3/moredata/enricher/api_connector/api_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py` & `moredata-0.2.3/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/elasticsearch_connector/index_handler.py` & `moredata-0.2.3/moredata/enricher/elasticsearch_connector/index_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/elasticsearch_connector/pipeline_handler.py` & `moredata-0.2.3/moredata/enricher/elasticsearch_connector/pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/elasticsearch_connector/policy_handler.py` & `moredata-0.2.3/moredata/enricher/elasticsearch_connector/policy_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/enricher.py` & `moredata-0.2.3/moredata/enricher/enricher.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/enricher_builder.py` & `moredata-0.2.3/moredata/enricher/enricher_builder.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/osm/functional_region_connector.py` & `moredata-0.2.3/moredata/enricher/osm/functional_region_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/enricher/osm/osm_places_connector.py` & `moredata-0.2.3/moredata/enricher/osm/osm_places_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         return data
 
     def enrich_geopandas_data(self, data, **kwargs):
         data = self._buffer_with_crs(data, kwargs.get("new_crs", None))
 
         self._df = self._df.set_crs("EPSG:4326")
 
-        sj = geopandas.sjoin(data, self._df, how="left", predicate="intersects")
+        sj = geopandas.sjoin(data, self._df, how=kwargs.get("join_how", "left"), predicate="intersects")
 
         sj["geometry"] = sj["geometry_not_buffered"]
         sj.drop(columns=["geometry_not_buffered"], inplace=True)
 
         return GeopandasData.from_geodataframe(sj)
 
     def enrich_dask_geopandas_data(self, data, **kwargs):
```

### Comparing `moredata-0.2.2/moredata/enricher/sql_connector/sql_connector.py` & `moredata-0.2.3/moredata/enricher/sql_connector/sql_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/models/data.py` & `moredata-0.2.3/moredata/models/data.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/parser/__init__.py` & `moredata-0.2.3/moredata/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/utils/__init__.py` & `moredata-0.2.3/moredata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata/utils/osm_downloader.py` & `moredata-0.2.3/moredata/utils/osm_downloader.py`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/moredata.egg-info/SOURCES.txt` & `moredata-0.2.3/moredata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moredata-0.2.2/setup.py` & `moredata-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         "jinja2==2.11.1",
         "sphinxcontrib-napoleon==0.7",
     ]
 
 setup(
     name="moredata",
     url="https://https://github.com/NESPEDUFV/more-data",
-    download_url="https://github.com/NESPEDUFV/more-data/archive/v0.2.2.tar.gz",
-    version="0.2.2",
+    download_url="https://github.com/NESPEDUFV/more-data/archive/v0.2.3.tar.gz",
+    version="0.2.3",
     packages=find_packages(where="."),
     python_requires=">=3.8",
     install_requires=dependencies + elasticsearch + sql + json + osm,
     # extras_require={
     #     "complete": dependencies + elasticsearch + sql + json + osm,
     #     "osm": dependencies + osm,
     #     "elasticsearch": dependencies + elasticsearch,
```

