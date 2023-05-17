# Comparing `tmp/macrometa-source-mongo-0.0.39.tar.gz` & `tmp/macrometa-source-mongo-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.39.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.40.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.39.tar` & `macrometa-source-mongo-0.0.40.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/LICENSE
--rw-r--r--   0        0        0    20533 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7271 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-05-12 12:47:36.766087 macrometa-source-mongo-0.0.39/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.39/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.39/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/LICENSE
+-rw-r--r--   0        0        0    20738 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6470 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-05-17 06:36:07.144934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7271 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-05-17 06:36:07.148934 macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-05-17 06:36:07.384932 macrometa-source-mongo-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.40/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.40/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.39/LICENSE` & `macrometa-source-mongo-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,18 @@
         config (Dict): A dictionary containing database configuration parameters.
     """
     if config['database'] not in get_user_databases(client, config):
         raise NoReadPrivilegeException(config['user'], config['database'])
 
     database = client[config['database']]
     collection_name = config['source_collection']
+    # Check if collection exists
+    if collection_name not in database.list_collection_names():
+        raise Exception(f'Collection "{collection_name}" not found in the database {config["database"]}.')
+
     collection = database[collection_name]
     is_view = collection.options().get('viewOn') is not None
 
     if is_view:
         raise KeyError('The connector does not support views.')
 
     LOGGER.info("Retrieving collection information for database '%s', collection '%s'", database.name, collection_name)
```

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.40/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.39/pyproject.toml` & `macrometa-source-mongo-0.0.40/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.39'
+version='0.0.40'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.39/setup.py` & `macrometa-source-mongo-0.0.40/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.39',
+    'version': '0.0.40',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.39/PKG-INFO` & `macrometa-source-mongo-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.39
+Version: 0.0.40
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

