# Comparing `tmp/macrometa-source-mssql-0.0.2.tar.gz` & `tmp/macrometa-source-mssql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mssql-0.0.2.tar", max compression
+gzip compressed data, was "macrometa-source-mssql-0.0.3.tar", max compression
```

## Comparing `macrometa-source-mssql-0.0.2.tar` & `macrometa-source-mssql-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11899 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/LICENSE
--rw-r--r--   0        0        0    34757 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/__init__.py
--rwxr-xr-x   0        0        0     1483 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/connection.py
--rw-r--r--   0        0        0     2287 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sample_data.py
--rwxr-xr-x   0        0        0        0 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8025 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2206 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/full_table.py
--rw-r--r--   0        0        0    14533 2023-05-17 06:39:29.627656 macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1557 2023-05-17 06:39:29.883655 macrometa-source-mssql-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.2/setup.py
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/LICENSE
+-rw-r--r--   0        0        0    34455 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1483 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/connection.py
+-rw-r--r--   0        0        0     2287 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sample_data.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     8025 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2206 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    14533 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1557 2023-05-17 07:48:02.210661 macrometa-source-mssql-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.3/setup.py
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.3/PKG-INFO
```

### Comparing `macrometa-source-mssql-0.0.2/LICENSE` & `macrometa-source-mssql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.2/macrometa_source_mssql/__init__.py` & `macrometa-source-mssql-0.0.3/macrometa_source_mssql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 REQUIRED_CONFIG_KEYS = [
     'host',
     'port',
     'user',
     'password',
     'database',
-    'filter_dbs',
-    'filter_table'
+    'source_schema',
+    'source_table'
 ]
 
 
 class MicrosoftSQLServerConnector(C8Connector):
     """MicrosoftSQLServerConnector's C8Connector impl."""
 
     def name(self) -> str:
@@ -167,17 +167,17 @@
                            description='Microsoft SQL Server port.', default_value='1433'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='Microsoft SQL Server user.', default_value='admin'),
             ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='Microsoft SQL Server password.', placeholder_value='password'),
             ConfigProperty('database', 'Database Name', ConfigAttributeType.STRING, True, True,
                            description='Microsoft SQL Server database name.', default_value='master'),
-            ConfigProperty('filter_dbs', 'Source Schema', ConfigAttributeType.STRING, True, True,
+            ConfigProperty('source_schema', 'Source Schema', ConfigAttributeType.STRING, True, True,
                            description='Source Schema to scan.', placeholder_value='my_schema'),
-            ConfigProperty('filter_table', 'Source Table', ConfigAttributeType.STRING, True, True,
+            ConfigProperty('source_table', 'Source Table', ConfigAttributeType.STRING, True, True,
                            description='Source Table to scan.', placeholder_value='my_table'),
             ConfigProperty('default_replication_method', 'Replication Method', ConfigAttributeType.STRING, True, True,
                            description='Choose from LOG_BASED, FULL_TABLE.', default_value='FULL_TABLE'),
             ConfigProperty('characterset', 'Character Set', ConfigAttributeType.STRING, False, False,
                            description='The characterset of the Microsoft SQL Server database.', default_value='utf8'),
             ConfigProperty('tds_version', 'TDS Version', ConfigAttributeType.STRING, False, False,
                            description='Set the version of TDS to use when communicating with MS SQL Server.',
@@ -199,16 +199,16 @@
             return {
                 # Required config keys
                 'host': integration['host'],
                 'port': integration['port'],
                 'user': integration['user'],
                 'password': integration['password'],
                 'database': integration['database'],
-                'filter_dbs': integration['filter_dbs'],
-                'filter_table': integration['filter_table'],
+                'source_schema': integration['source_schema'],
+                'source_table': integration['source_table'],
 
                 # Optional config keys
                 'characterset': integration.get('characterset', "utf8"),
                 'tds_version': integration.get('tds_version', "7.3"),
                 'use_date_datatype': integration.get('use_date_datatype', False),
                 'default_replication_method': integration.get('default_replication_method', "FULL_TABLE")
             }
@@ -339,33 +339,20 @@
 
     return metadata.to_list(mdata)
 
 
 def discover_catalog(mssql_conn, config):
     """Returns a Catalog describing the structure of the database."""
     LOGGER.info("Preparing Catalog")
-    mssql_conn = MSSQLConnection(config)
-    filter_dbs_config = config.get("filter_dbs")
-
-    if filter_dbs_config:
-        filter_dbs_clause = ",".join(["'{}'".format(db) for db in filter_dbs_config.split(",")])
-
-        table_schema_clause = "WHERE c.table_schema IN ({})".format(filter_dbs_clause)
-    else:
-        table_schema_clause = """
-        WHERE c.table_schema NOT IN (
-        'information_schema',
-        'INFORMATION_SCHEMA',
-        'performance_schema',
-        'sys'
-        )"""
+    source_schema = config.get("source_schema")
+    source_table = config.get("source_table")
+    table_schema_clause = "WHERE c.table_schema = '{}' AND c.table_name='{}'".format(source_schema, source_table)
 
     with connect_with_backoff(mssql_conn) as open_conn:
         cur = open_conn.cursor()
-        LOGGER.info("Fetching tables")
         cur.execute(
             """SELECT table_schema,
                 table_name,
                 table_type
             FROM INFORMATION_SCHEMA.tables c
             {}
         """.format(
@@ -373,17 +360,17 @@
             )
         )
         table_info = {}
 
         for (db, table, table_type) in cur.fetchall():
             if db not in table_info:
                 table_info[db] = {}
-
             table_info[db][table] = {"row_count": None, "is_view": table_type == "VIEW"}
-        LOGGER.info("Tables fetched, fetching columns")
+
+        LOGGER.info("Source table information fetched, fetching columns")
         cur.execute(
             """with constraint_columns as (
                 select c.table_schema
                 , c.table_name
                 , c.column_name
 
                 from INFORMATION_SCHEMA.constraint_column_usage c
```

### Comparing `macrometa-source-mssql-0.0.2/macrometa_source_mssql/connection.py` & `macrometa-source-mssql-0.0.3/macrometa_source_mssql/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sample_data.py` & `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/common.py` & `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/full_table.py` & `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.2/macrometa_source_mssql/sync_strategies/log_based.py` & `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.2/pyproject.toml` & `macrometa-source-mssql-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mssql"
-version='0.0.2'
+version='0.0.3'
 description = "Macrometa Source for extracting data from Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mssql-0.0.2/setup.py` & `macrometa-source-mssql-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'pymssql>=2.2.1']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mssql = macrometa_source_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mssql',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Macrometa Source for extracting data from Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mssql-0.0.2/PKG-INFO` & `macrometa-source-mssql-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mssql
-Version: 0.0.2
+Version: 0.0.3
 Summary: Macrometa Source for extracting data from Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MSSQL,Microsoft SQL Server,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

