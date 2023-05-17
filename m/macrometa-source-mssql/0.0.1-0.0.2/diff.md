# Comparing `tmp/macrometa-source-mssql-0.0.1.tar.gz` & `tmp/macrometa-source-mssql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mssql-0.0.1.tar", max compression
+gzip compressed data, was "macrometa-source-mssql-0.0.2.tar", max compression
```

## Comparing `macrometa-source-mssql-0.0.1.tar` & `macrometa-source-mssql-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11899 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/LICENSE
--rw-r--r--   0        0        0    34805 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/macrometa_source_mssql/__init__.py
--rwxr-xr-x   0        0        0     1483 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/macrometa_source_mssql/connection.py
--rw-r--r--   0        0        0     2296 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/macrometa_source_mssql/sample_data.py
--rwxr-xr-x   0        0        0        0 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/macrometa_source_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8025 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/macrometa_source_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2206 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/macrometa_source_mssql/sync_strategies/full_table.py
--rw-r--r--   0        0        0    14533 2023-05-17 06:07:21.591757 macrometa-source-mssql-0.0.1/macrometa_source_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1557 2023-05-17 06:07:21.915761 macrometa-source-mssql-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.1/setup.py
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/LICENSE
+-rw-r--r--   0        0        0    34757 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1483 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/connection.py
+-rw-r--r--   0        0        0     2287 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sample_data.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     8025 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2206 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    14533 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1557 2023-05-17 06:39:29.883655 macrometa-source-mssql-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.2/setup.py
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.2/PKG-INFO
```

### Comparing `macrometa-source-mssql-0.0.1/LICENSE` & `macrometa-source-mssql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.1/macrometa_source_mssql/__init__.py` & `macrometa-source-mssql-0.0.2/macrometa_source_mssql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,28 +86,28 @@
         try:
             config = self.get_config(integration)
             mssql_conn = MSSQLConnection(config)
             catalog = do_discover(mssql_conn, config)
             results = []
             for stream in catalog.streams:
                 s_attribs = []
-                s_schema = stream['schema']
+                s_schema = stream.schema
                 data = fetch_samples(mssql_conn, config, stream)[:10]
                 # Appending _ to keys for preserving values of reserved keys in source data
                 reserved_keys = ['_key', '_id', '_rev']
-                if stream['metadata'][0]['metadata'].get('table-key-properties'):
-                    key_properties = stream['metadata'][0]['metadata'].get('table-key-properties')
+                if stream.metadata[0]['metadata'].get('table-key-properties'):
+                    key_properties = stream.metadata[0]['metadata'].get('table-key-properties')
                     if key_properties[0] == '_key':
                         reserved_keys.remove('_key')
-                s_schema['properties'] = modify_reserved_keys(s_schema['properties'], reserved_keys)
+                s_schema.properties = modify_reserved_keys(s_schema.properties, reserved_keys)
 
-                for k, v in s_schema['properties'].items():
-                    t = v['type'][-1]
+                for k, v in s_schema.properties.items():
+                    t = v.type[-1]
                     s_attribs.append(SchemaAttribute(k, self.get_attribute_type(t)))
-                schema = Schema(stream['stream'], s_attribs)
+                schema = Schema(stream.stream, s_attribs)
                 results.append(Sample(
                     schema=schema,
                     data=data)
                 )
         except Exception as e:
             LOGGER.info("Exception raised: %s", e)
             raise e
@@ -118,28 +118,28 @@
         try:
             config = self.get_config(integration)
             mssql_conn = MSSQLConnection(config)
             catalog = do_discover(mssql_conn, config)
             results = []
             for stream in catalog.streams:
                 s_attribs = []
-                s_schema = stream['schema']
+                s_schema = stream.schema
 
                 # Appending _ to keys for preserving values of reserved keys in source data
                 reserved_keys = ['_key', '_id', '_rev']
-                if stream['metadata'][0]['metadata'].get('table-key-properties'):
-                    key_properties = stream['metadata'][0]['metadata'].get('table-key-properties')
+                if stream.metadata[0]['metadata'].get('table-key-properties'):
+                    key_properties = stream.metadata[0]['metadata'].get('table-key-properties')
                     if key_properties[0] == '_key':
                         reserved_keys.remove('_key')
-                s_schema['properties'] = modify_reserved_keys(s_schema['properties'], reserved_keys)
+                s_schema.properties = modify_reserved_keys(s_schema.properties, reserved_keys)
 
-                for k, v in s_schema['properties'].items():
-                    t = v['type'][-1]
+                for k, v in s_schema.properties.items():
+                    t = v.type[-1]
                     s_attribs.append(SchemaAttribute(k, self.get_attribute_type(t)))
-                results.append(Schema(stream['stream'], s_attribs))
+                results.append(Schema(stream.stream, s_attribs))
         except Exception as e:
             LOGGER.info("Exception raised: %s", e)
             raise e
         return results
 
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
```

### Comparing `macrometa-source-mssql-0.0.1/macrometa_source_mssql/connection.py` & `macrometa-source-mssql-0.0.2/macrometa_source_mssql/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.1/macrometa_source_mssql/sample_data.py` & `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sample_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     return samples
 
 
 def fetch_samples(mssql_conn, config, stream):
     """
     Fetch samples for the stream.
     """
-    md_map = metadata.to_map(stream['metadata'])
-    desired_columns = [c for c in stream['schema']['properties'].keys() if should_sync_column(md_map, c)]
+    md_map = metadata.to_map(stream.metadata)
+    desired_columns = [c for c in stream.schema.properties.keys() if should_sync_column(md_map, c)]
     desired_columns.sort()
     if not desired_columns:
         # There are no columns selected for stream. So, skipping it.
         return []
     state = fetch_table(mssql_conn, config, stream, desired_columns, limit=10)
 
     # Appending _ to keys for preserving values of reserved keys in source data
```

### Comparing `macrometa-source-mssql-0.0.1/macrometa_source_mssql/sync_strategies/common.py` & `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.1/macrometa_source_mssql/sync_strategies/full_table.py` & `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.1/macrometa_source_mssql/sync_strategies/log_based.py` & `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.1/pyproject.toml` & `macrometa-source-mssql-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mssql"
-version='0.0.1'
+version='0.0.2'
 description = "Macrometa Source for extracting data from Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mssql-0.0.1/setup.py` & `macrometa-source-mssql-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'pymssql>=2.2.1']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mssql = macrometa_source_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mssql',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Macrometa Source for extracting data from Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mssql-0.0.1/PKG-INFO` & `macrometa-source-mssql-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mssql
-Version: 0.0.1
+Version: 0.0.2
 Summary: Macrometa Source for extracting data from Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MSSQL,Microsoft SQL Server,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

