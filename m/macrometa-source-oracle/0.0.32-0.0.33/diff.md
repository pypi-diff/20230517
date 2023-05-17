# Comparing `tmp/macrometa-source-oracle-0.0.32.tar.gz` & `tmp/macrometa-source-oracle-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-oracle-0.0.32.tar", max compression
+gzip compressed data, was "macrometa-source-oracle-0.0.33.tar", max compression
```

## Comparing `macrometa-source-oracle-0.0.32.tar` & `macrometa-source-oracle-0.0.33.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     9713 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/LICENSE
--rw-r--r--   0        0        0     1715 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/README.md
--rw-r--r--   0        0        0    42351 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/macrometa_source_oracle/__init__.py
--rwxr-xr-x   0        0        0     7417 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/macrometa_source_oracle/connection.py
--rwxr-xr-x   0        0        0        0 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/macrometa_source_oracle/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     4779 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/macrometa_source_oracle/sync_strategies/common.py
--rwxr-xr-x   0        0        0     4874 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/macrometa_source_oracle/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0    17662 2023-04-17 09:51:35.821352 macrometa-source-oracle-0.0.32/macrometa_source_oracle/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1563 2023-04-17 09:51:35.897353 macrometa-source-oracle-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.32/setup.py
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.32/PKG-INFO
+-rwxr-xr-x   0        0        0     9713 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/LICENSE
+-rw-r--r--   0        0        0     1715 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/README.md
+-rw-r--r--   0        0        0    42537 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/macrometa_source_oracle/__init__.py
+-rwxr-xr-x   0        0        0     7417 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/macrometa_source_oracle/connection.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/macrometa_source_oracle/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     4779 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/macrometa_source_oracle/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     4874 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/macrometa_source_oracle/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0    17662 2023-05-17 07:35:54.578404 macrometa-source-oracle-0.0.33/macrometa_source_oracle/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1563 2023-05-17 07:35:54.658404 macrometa-source-oracle-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.33/setup.py
+-rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.33/PKG-INFO
```

### Comparing `macrometa-source-oracle-0.0.32/LICENSE` & `macrometa-source-oracle-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.32/README.md` & `macrometa-source-oracle-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.32/macrometa_source_oracle/__init__.py` & `macrometa-source-oracle-0.0.33/macrometa_source_oracle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         If invalid, throw an exception with the cause.
         """
         config, filter_schema = self.get_config(integration)
         try:
             config = orc_db.create_wallet_file(config)
             do_discovery(config, [filter_schema], config['filter_table'])
         except Exception as e:
+            LOGGER.info('Exception raised: %s', e)
             orc_db.delete_wallet_file(config)
             raise e
         orc_db.delete_wallet_file(config)
 
     def schemas(self, integration: dict) -> list[C8Schema]:
         """Get supported schemas using the given configurations."""
         config, filter_schema = self.get_config(integration)
@@ -660,14 +661,17 @@
         if schema not in table_info:
             table_info[schema] = {}
 
         table_info[schema][view_name] = {
             'is_view': True
         }
 
+    if not table_info:
+        raise Exception(f'Table/view "{filter_table}" not found in the specified schema {filter_schemas[0]}.')
+
     for scheme in table_info:
         LOGGER.info(f"Schema {scheme} contains {len(table_info[scheme])} tables/views.")
 
     catalog = discover_columns(cur, table_info, filter_schemas, filter_table)
 
     dump_catalog(catalog)
     cur.close()
```

### Comparing `macrometa-source-oracle-0.0.32/macrometa_source_oracle/connection.py` & `macrometa-source-oracle-0.0.33/macrometa_source_oracle/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.32/macrometa_source_oracle/sync_strategies/common.py` & `macrometa-source-oracle-0.0.33/macrometa_source_oracle/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.32/macrometa_source_oracle/sync_strategies/full_table.py` & `macrometa-source-oracle-0.0.33/macrometa_source_oracle/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.32/macrometa_source_oracle/sync_strategies/log_based.py` & `macrometa-source-oracle-0.0.33/macrometa_source_oracle/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.32/pyproject.toml` & `macrometa-source-oracle-0.0.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-oracle"
-version='0.0.32'
+version='0.0.33'
 description = "Macrometa source oracle connector for reading from oracle databases."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 readme = "README.md"
 homepage = "https://www.macrometa.com/"
 keywords = [
     "ELT",
```

### Comparing `macrometa-source-oracle-0.0.32/setup.py` & `macrometa-source-oracle-0.0.33/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'strict-rfc3339>=0.7,<0.8']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-oracle = macrometa_source_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-oracle',
-    'version': '0.0.32',
+    'version': '0.0.33',
     'description': 'Macrometa source oracle connector for reading from oracle databases.',
     'long_description': '# macrometa-source-oracle\n\nMacrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).\n\n## How to use it\n\n### Install and Run\n\nFirst, make sure Python 3 is installed on your system or follow these\ninstallation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or\n[Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).\n\n\nIt\'s recommended to use a virtualenv:\n\n```bash\n  python3 -m venv venv\n  pip install macrometa-source-oracle\n```\n\nor from source using,\n1. Install poetry using https://python-poetry.org/docs/#installation\n2. Run \n    ```bash\n    poetry build\n    pip install dist/macrometa_source_oracle-<version>*.whl\n    ```\n\n### Configuration\n\nRunning the the macrometa source connector independently requires a `config.json` file. \n\nExample configuration:\n\n```json\n{\n  "host": "dev.oracledb.io",\n  "port": 1521,\n  "user": "C##HELLO",\n  "password": "password",\n  "service_name": "ORCLCDB",\n  "filter_schema": "C##HELLO",\n  "filter_table": "CUSTOMERS",\n  "default_replication_method": "LOG_BASED",\n  "pdb_name": "ORCLPDB1",\n  "multitenant": true,\n  "scn_window_size": 10\n}\n```\n\nYou can run a discover run using the previous `config.json` file to acquire all the tables definition\n \n```\nmacrometa-source-oracle --config /tmp/config.json --discover >> /tmp/catalog.json\n```\n\nThen use the catalog.json to run a full export:\n\n```\nmacrometa-source-oracle --config /tmp/config.json --catalog /tmp/catalog.json\n```\n\n',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.macrometa.com/',
```

### Comparing `macrometa-source-oracle-0.0.32/PKG-INFO` & `macrometa-source-oracle-0.0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-oracle
-Version: 0.0.32
+Version: 0.0.33
 Summary: Macrometa source oracle connector for reading from oracle databases.
 Home-page: https://www.macrometa.com/
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Oracle,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8
```

