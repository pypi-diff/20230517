# Comparing `tmp/macrometa-source-mssql-0.0.3.tar.gz` & `tmp/macrometa-source-mssql-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mssql-0.0.3.tar", max compression
+gzip compressed data, was "macrometa-source-mssql-0.0.4.tar", max compression
```

## Comparing `macrometa-source-mssql-0.0.3.tar` & `macrometa-source-mssql-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11899 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/LICENSE
--rw-r--r--   0        0        0    34455 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/__init__.py
--rwxr-xr-x   0        0        0     1483 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/connection.py
--rw-r--r--   0        0        0     2287 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sample_data.py
--rwxr-xr-x   0        0        0        0 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8025 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2206 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/full_table.py
--rw-r--r--   0        0        0    14533 2023-05-17 07:48:01.962586 macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1557 2023-05-17 07:48:02.210661 macrometa-source-mssql-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.3/setup.py
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/LICENSE
+-rw-r--r--   0        0        0    34455 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/macrometa_source_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1476 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/macrometa_source_mssql/connection.py
+-rw-r--r--   0        0        0     2287 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/macrometa_source_mssql/sample_data.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/macrometa_source_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     8025 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/macrometa_source_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2206 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/macrometa_source_mssql/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    14533 2023-05-17 09:53:07.134505 macrometa-source-mssql-0.0.4/macrometa_source_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1537 2023-05-17 09:53:07.438513 macrometa-source-mssql-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.4/setup.py
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.4/PKG-INFO
```

### Comparing `macrometa-source-mssql-0.0.3/LICENSE` & `macrometa-source-mssql-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.3/macrometa_source_mssql/__init__.py` & `macrometa-source-mssql-0.0.4/macrometa_source_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.3/macrometa_source_mssql/connection.py` & `macrometa-source-mssql-0.0.4/macrometa_source_mssql/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 
-import backoff
 import pymssql
 import singer
 
 LOGGER = singer.get_logger('macrometa_source_mssql')
 
 
-@backoff.on_exception(backoff.expo, pymssql.Error, max_tries=5, factor=2)
+# TODO: @backoff.on_exception(backoff.expo, pymssql.Error, max_tries=5, factor=2)
 def connect_with_backoff(connection):
     warnings = []
     with connection.cursor():
         if warnings:
             LOGGER.info(
                 (
                     "Encountered non-fatal errors when configuring session that could "
```

### Comparing `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sample_data.py` & `macrometa-source-mssql-0.0.4/macrometa_source_mssql/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/common.py` & `macrometa-source-mssql-0.0.4/macrometa_source_mssql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/full_table.py` & `macrometa-source-mssql-0.0.4/macrometa_source_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.3/macrometa_source_mssql/sync_strategies/log_based.py` & `macrometa-source-mssql-0.0.4/macrometa_source_mssql/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.3/pyproject.toml` & `macrometa-source-mssql-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mssql"
-version='0.0.3'
+version='0.0.4'
 description = "Macrometa Source for extracting data from Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -29,15 +29,14 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
 c8connector = ">=0.0.20"
 attrs = ">=16.3.0"
 pendulum = ">=1.2.0"
 pymssql = ">=2.2.1"
-backoff = ">=1.8.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-source-mssql = 'macrometa_source_mssql:main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Macrometacorp/macrometa-source-mssql/issues"
```

### Comparing `macrometa-source-mssql-0.0.3/setup.py` & `macrometa-source-mssql-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,25 @@
  'sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=16.3.0',
- 'backoff>=1.8.0',
  'c8connector>=0.0.20',
  'pendulum>=1.2.0',
  'pipelinewise-singer-python==1.2.0',
  'pymssql>=2.2.1']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mssql = macrometa_source_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mssql',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Macrometa Source for extracting data from Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mssql-0.0.3/PKG-INFO` & `macrometa-source-mssql-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mssql
-Version: 0.0.3
+Version: 0.0.4
 Summary: Macrometa Source for extracting data from Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MSSQL,Microsoft SQL Server,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: attrs (>=16.3.0)
-Requires-Dist: backoff (>=1.8.0)
 Requires-Dist: c8connector (>=0.0.20)
 Requires-Dist: pendulum (>=1.2.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: pymssql (>=2.2.1)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-mssql/issues
```

