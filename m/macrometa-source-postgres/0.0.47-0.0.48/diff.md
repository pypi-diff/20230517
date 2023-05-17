# Comparing `tmp/macrometa-source-postgres-0.0.47.tar.gz` & `tmp/macrometa-source-postgres-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.47.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.48.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.47.tar` & `macrometa-source-postgres-0.0.48.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/LICENSE
--rw-r--r--   0        0        0    34891 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    27687 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-05-15 03:01:57.485275 macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-05-15 03:01:57.725279 macrometa-source-postgres-0.0.47/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.47/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.47/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/LICENSE
+-rw-r--r--   0        0        0    35642 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     8974 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28329 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-05-17 03:54:10.974792 macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1512 2023-05-17 03:54:11.278795 macrometa-source-postgres-0.0.48/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.48/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.48/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.47/LICENSE` & `macrometa-source-postgres-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.47/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.48/macrometa_source_postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,25 +205,31 @@
             ConfigProperty('ssl_client_key', 'SSL Client Key', ConfigAttributeType.FILE, False, False,
                            description='Specific client key in PEM string format.',
                            placeholder_value="my_client_key"),
             ConfigProperty('ssl_client_password', 'SSL Client Password', ConfigAttributeType.PASSWORD, False, False,
                            description='If the private key contained in the SSL Client Key is encrypted, users can provide a '
                                        'password or passphrase to decrypt the encrypted private keys.',
                            placeholder_value="my_client_password"),
+            ConfigProperty('replication_slot', 'Replication Slot (LOG_BASED)', ConfigAttributeType.STRING, False, False,
+                           description='PostgreSQL replication slot name required for LOG_BASED replication method.'
+                                       ' This replication slot will be used to retrieve the required WAL files.'
+                                       'If no value is provided replication slot is set as `macrometa_dbname` '
+                                       '(dbname will be replaced by your database name).',
+                           placeholder_value='macrometa_dbname'),
             ConfigProperty('break_at_end_lsn', 'Break at End LSN', ConfigAttributeType.BOOLEAN, False, False,
                            description='Stop running if the newly received LSN is after the max LSN that was initially'
                                        ' detected.',
                            default_value='false'),
             ConfigProperty('wal_sender_timeout', 'WAL Sender Timeout (milliseconds)', ConfigAttributeType.INT, False, False,
                            description='Terminate replication connections that are inactive for longer than this amount of time.'
                                        ' This is useful for the sending server to detect a standby crash or network outage.'
                                        ' Unit is milliseconds. The default value is 3600000 ms.',
                            default_value='3600000'),
-            ConfigProperty('debug_lsn', 'Debug LSN', ConfigAttributeType.STRING, False, False,
-                           description='If set to "true" then add _sdc_lsn property to the singer messages '
+            ConfigProperty('debug_lsn', 'Debug LSN', ConfigAttributeType.BOOLEAN, False, False,
+                           description='If set to True then add _sdc_lsn property to the singer messages '
                                        'to debug postgres LSN position in the WAL stream.',
                            default_value='false'),
             ConfigProperty('itersize', 'Iterator Size', ConfigAttributeType.INT, False, False,
                            description='PG cursor size for FULL_TABLE.',
                            default_value='20000'),
             ConfigProperty('use_secondary', 'Use Secondary', ConfigAttributeType.BOOLEAN, False, False,
                            description='Use a database replica for FULL_TABLE replication.',
@@ -257,15 +263,16 @@
                 # Optional config keys
                 'ssl': integration.get('ssl', False),
                 'ssl_root_ca_cert': integration.get('ssl_root_ca_cert'),
                 'ssl_client_certificate': integration.get('ssl_client_certificate'),
                 'ssl_client_key': integration.get('ssl_client_key'),
                 'ssl_client_password': integration.get('ssl_client_password'),
                 'tap_id': integration.get('tap_id'),
-                'debug_lsn': integration.get('debug_lsn') == 'true',
+                'replication_slot': integration.get('replication_slot'),
+                'debug_lsn': integration.get('debug_lsn', False),
                 'wal_sender_timeout': integration.get('wal_sender_timeout', 3600000),
                 'break_at_end_lsn': integration.get('break_at_end_lsn', True),
                 'use_secondary': integration.get('use_secondary', False),
             }
         except KeyError as e:
             raise KeyError(f'Integration property `{e}` not found.') from e
 
@@ -727,15 +734,16 @@
         # Optional config keys
         'ssl': args.config.get('ssl', False),
         'ssl_root_ca_cert': args.config.get('ssl_root_ca_cert'),
         'ssl_client_certificate': args.config.get('ssl_client_certificate'),
         'ssl_client_key': args.config.get('ssl_client_key'),
         'ssl_client_password': args.config.get('ssl_client_password'),
         'tap_id': args.config.get('tap_id'),
-        'debug_lsn': args.config.get('debug_lsn') == 'true',
+        'replication_slot': args.config.get('replication_slot'),
+        'debug_lsn': args.config.get('debug_lsn', False),
         'wal_sender_timeout': args.config.get('wal_sender_timeout', 3600000),
         'break_at_end_lsn': args.config.get('break_at_end_lsn', True),
         'use_secondary': args.config.get('use_secondary', False),
     }
 
     if conn_config['use_secondary']:
         try:
```

### Comparing `macrometa-source-postgres-0.0.47/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.48/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.47/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.48/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,38 +433,48 @@
     # Combine prefix, dbname, and tap_id_suffix to form the initial slot name.
     slot_name = f'{prefix}_{dbname}{tap_id_suffix}'.lower()
 
     # Replace any invalid characters in the slot name to comply with Postgres naming specifications.
     return re.sub('[^a-z0-9_]', '_', slot_name)
 
 
-def locate_replication_slot_by_cur(cursor, dbname, tap_id=None):
-    slot_name_v15 = generate_replication_slot_name(dbname)
-    slot_name_v16 = generate_replication_slot_name(dbname, tap_id)
-
-    # Ensure backward compatibility: first attempt to locate the existing v15 slot (for PPW <= 0.15.0).
-    cursor.execute(f"SELECT * FROM pg_replication_slots WHERE slot_name = '{slot_name_v15}'")
-    if len(cursor.fetchall()) == 1:
-        LOGGER.info('Using replication slot %s from pg_replication_slots table.', slot_name_v15)
-        return slot_name_v15
-
-    # If the v15 replication slot is not found, attempt to locate the v16 replication slot.
-    cursor.execute(f"SELECT * FROM pg_replication_slots WHERE slot_name = '{slot_name_v16}'")
-    if len(cursor.fetchall()) == 1:
-        LOGGER.info('Using replication slot %s from pg_replication_slots table.', slot_name_v16)
-        return slot_name_v16
+def locate_replication_slot_by_cur(cursor, dbname, replication_slot=None, tap_id=None):
+    if replication_slot:
+        # If replication slot is provided use that
+        cursor.execute(f"SELECT * FROM pg_replication_slots WHERE slot_name = '{replication_slot}'")
+        if len(cursor.fetchall()) == 1:
+            LOGGER.info('Using replication slot %s from pg_replication_slots table.', replication_slot)
+            return replication_slot
+        raise ReplicationSlotNotFoundError(f'The replication slot {replication_slot} could not be found.')
+
+    else:
+        slot_name_v15 = generate_replication_slot_name(dbname)
+        slot_name_v16 = generate_replication_slot_name(dbname, tap_id)
+
+        # Ensure backward compatibility: first attempt to locate the existing v15 slot (for PPW <= 0.15.0).
+        cursor.execute(f"SELECT * FROM pg_replication_slots WHERE slot_name = '{slot_name_v15}'")
+        if len(cursor.fetchall()) == 1:
+            LOGGER.info('Using replication slot %s from pg_replication_slots table.', slot_name_v15)
+            return slot_name_v15
+
+        # If the v15 replication slot is not found, attempt to locate the v16 replication slot.
+        cursor.execute(f"SELECT * FROM pg_replication_slots WHERE slot_name = '{slot_name_v16}'")
+        if len(cursor.fetchall()) == 1:
+            LOGGER.info('Using replication slot %s from pg_replication_slots table.', slot_name_v16)
+            return slot_name_v16
 
-    raise ReplicationSlotNotFoundError(f'The replication slot {slot_name_v16} could not be found.')
+        raise ReplicationSlotNotFoundError(f'The replication slot {slot_name_v16} could not be found.')
 
 
 def locate_replication_slot(conn_info):
     with postgres.connect(conn_info, False, True) as conn:
         with conn.cursor() as cur:
             return locate_replication_slot_by_cur(
                 cur, conn_info['dbname'],
+                conn_info['replication_slot'] if 'replication_slot' in conn_info else None,
                 conn_info['tap_id'] if 'tap_id' in conn_info else None)
 
 
 def streams_to_wal2json_tables(streams):
     """
     Create a comma-separated, escaped list of table names that can be used with the wal2json plugin.
```

### Comparing `macrometa-source-postgres-0.0.47/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.48/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.47/pyproject.toml` & `macrometa-source-postgres-0.0.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.47'
+version='0.0.48'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-postgres-0.0.47/setup.py` & `macrometa-source-postgres-0.0.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.47',
+    'version': '0.0.48',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.47/PKG-INFO` & `macrometa-source-postgres-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.47
+Version: 0.0.48
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

