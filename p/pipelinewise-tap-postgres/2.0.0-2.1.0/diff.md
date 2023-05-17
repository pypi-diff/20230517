# Comparing `tmp/pipelinewise-tap-postgres-2.0.0.tar.gz` & `tmp/pipelinewise-tap-postgres-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinewise-tap-postgres-2.0.0.tar", last modified: Thu Nov  3 07:24:15 2022, max compression
+gzip compressed data, was "pipelinewise-tap-postgres-2.1.0.tar", last modified: Wed May 17 10:31:33 2023, max compression
```

## Comparing `pipelinewise-tap-postgres-2.0.0.tar` & `pipelinewise-tap-postgres-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 07:24:15.830905 pipelinewise-tap-postgres-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    32393 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9345 2022-11-03 07:24:15.830905 pipelinewise-tap-postgres-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8863 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 07:24:15.830905 pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9345 2022-11-03 07:24:15.000000 pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-11-03 07:24:15.000000 pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 07:24:15.000000 pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-03 07:24:15.000000 pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-03 07:24:15.000000 pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-03 07:24:15.000000 pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 07:24:15.830905 pipelinewise-tap-postgres-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 07:24:15.830905 pipelinewise-tap-postgres-2.0.0/tap_postgres/
--rw-r--r--   0 runner    (1001) docker     (121)    17935 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9923 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/db.py
--rw-r--r--   0 runner    (1001) docker     (121)    18145 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/discovery_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 07:24:15.830905 pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     7865 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/incremental.py
--rw-r--r--   0 runner    (1001) docker     (121)    29963 2022-11-03 07:24:04.000000 pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/logical_replication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:31:33.606834 pipelinewise-tap-postgres-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-17 10:31:33.606834 pipelinewise-tap-postgres-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:31:33.606834 pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-17 10:31:33.000000 pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-17 10:31:33.000000 pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:31:33.000000 pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 10:31:33.000000 pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-17 10:31:33.000000 pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 10:31:33.000000 pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:31:33.606834 pipelinewise-tap-postgres-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:31:33.606834 pipelinewise-tap-postgres-2.1.0/tap_postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18145 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/discovery_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:31:33.606834 pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/full_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/incremental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29963 2023-05-17 10:31:23.000000 pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/logical_replication.py
```

### Comparing `pipelinewise-tap-postgres-2.0.0/LICENSE` & `pipelinewise-tap-postgres-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-postgres-2.0.0/PKG-INFO` & `pipelinewise-tap-postgres-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-postgres
-Version: 2.0.0
+Version: 2.1.0
 Summary: Singer.io tap for extracting data from PostgresSQL - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-postgres
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
@@ -59,33 +59,34 @@
 }
 ```
 
 These are the same basic configuration properties used by the PostgreSQL command-line client (`psql`).
 
 Full list of options in `config.json`:
 
-| Property                            | Type    | Required?  | Description                                                   |
-|-------------------------------------|---------|------------|---------------------------------------------------------------|
-| host                                | String  | Yes        | PostgreSQL host                                               |
-| port                                | Integer | Yes        | PostgreSQL port                                               |
-| user                                | String  | Yes        | PostgreSQL user                                               |
-| password                            | String  | Yes        | PostgreSQL password                                           |
-| dbname                              | String  | Yes        | PostgreSQL database name                                      |
-| filter_schemas                      | String  | No         | Comma separated schema names to scan only the required schemas to improve the performance of data extraction. (Default: None) |
-| ssl                                 | String  | No         | If set to `"true"` then use SSL via postgres sslmode `require` option. If the server does not accept SSL connections or the client certificate is not recognized the connection will fail. (Default: None) |
-| logical_poll_total_seconds          | Integer | No         | Stop running the tap when no data received from wal after certain number of seconds. (Default: 10800) |
-| break_at_end_lsn                    | Boolean | No         | Stop running the tap if the newly received lsn is after the max lsn that was detected when the tap started. (Default: true) |
-| max_run_seconds                     | Integer | No         | Stop running the tap after certain number of seconds. (Default: 43200) |
-| debug_lsn                           | String  | No         | If set to `"true"` then add `_sdc_lsn` property to the singer messages to debug postgres LSN position in the WAL stream. (Default: None) |
-| tap_id                              | String  | No         | ID of the pipeline/tap (Default: None) |
-| itersize                            | Integer | No         | Size of PG cursor iterator when doing INCREMENTAL or FULL_TABLE  (Default: 20000) |
-| default_replication_method          | String  | No         | Default replication method to use when no one is provided in the catalog (Values: `LOG_BASED`, `INCREMENTAL` or `FULL_TABLE`)  (Default: None) |
-| use_secondary                       | Boolean | No         | Use a database replica for `INCREMENTAL` and `FULL_TABLE` replication (Default : False) |
-| secondary_host                      | String  | No         | PostgreSQL Replica host (required if `use_secondary` is `True`) |
-| secondary_port                      | Integer | No         | PostgreSQL Replica port (required if `use_secondary` is `True`) |
+| Property                   | Type    | Required? | Default | Description                                                                                                                                                                                |
+|----------------------------|---------|----------|---------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| host                       | String  | Yes      | -       | PostgreSQL host                                                                                                                                                                            |
+| port                       | Integer | Yes      | -       | PostgreSQL port                                                                                                                                                                            |
+| user                       | String  | Yes      | -       | PostgreSQL user                                                                                                                                                                            |
+| password                   | String  | Yes      | -       | PostgreSQL password                                                                                                                                                                        |
+| dbname                     | String  | Yes      | -       | PostgreSQL database name                                                                                                                                                                   |
+| filter_schemas             | String  | No       | None    | Comma separated schema names to scan only the required schemas to improve the performance of data extraction.                                                                              |
+| ssl                        | String  | No       | None    | If set to `"true"` then use SSL via postgres sslmode `require` option. If the server does not accept SSL connections or the client certificate is not recognized the connection will fail. |
+| logical_poll_total_seconds | Integer | No       | 10800   | Stop running the tap when no data received from wal after certain number of seconds.                                                                                                       |
+| break_at_end_lsn           | Boolean | No       | true    | Stop running the tap if the newly received lsn is after the max lsn that was detected when the tap started.                                                                                |
+| max_run_seconds            | Integer | No       | 43200   | Stop running the tap after certain number of seconds.                                                                                                                                      |
+| debug_lsn                  | String  | No       | None    | If set to `"true"` then add `_sdc_lsn` property to the singer messages to debug postgres LSN position in the WAL stream.                                                                   |
+| tap_id                     | String  | No       | None    | ID of the pipeline/tap                                                                                                                                                                     |
+| itersize                   | Integer | No       | 20000   | Size of PG cursor iterator when doing INCREMENTAL or FULL_TABLE                                                                                                                            |
+| default_replication_method | String  | No       | None    | Default replication method to use when no one is provided in the catalog (Values: `LOG_BASED`, `INCREMENTAL` or `FULL_TABLE`)                                                              |
+| use_secondary              | Boolean | No       | False   | Use a database replica for `INCREMENTAL` and `FULL_TABLE` replication                                                                                                                      |
+| secondary_host             | String  | No       | -       | PostgreSQL Replica host (required if `use_secondary` is `True`)                                                                                                                            |
+| secondary_port             | Integer | No       | -       | PostgreSQL Replica port (required if `use_secondary` is `True`)                                                                                                                            |
+| limit                      | Integer | No       | None    | Adds a limit to INCREMENTAL queries to limit the number of records returns per run                                                                                                         |
 
 
 ### Run the tap in Discovery Mode
 
 ```
 tap-postgres --config config.json --discover                # Should dump a Catalog to stdout
 tap-postgres --config config.json --discover > catalog.json # Capture the Catalog
```

### Comparing `pipelinewise-tap-postgres-2.0.0/README.md` & `pipelinewise-tap-postgres-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -46,33 +46,34 @@
 }
 ```
 
 These are the same basic configuration properties used by the PostgreSQL command-line client (`psql`).
 
 Full list of options in `config.json`:
 
-| Property                            | Type    | Required?  | Description                                                   |
-|-------------------------------------|---------|------------|---------------------------------------------------------------|
-| host                                | String  | Yes        | PostgreSQL host                                               |
-| port                                | Integer | Yes        | PostgreSQL port                                               |
-| user                                | String  | Yes        | PostgreSQL user                                               |
-| password                            | String  | Yes        | PostgreSQL password                                           |
-| dbname                              | String  | Yes        | PostgreSQL database name                                      |
-| filter_schemas                      | String  | No         | Comma separated schema names to scan only the required schemas to improve the performance of data extraction. (Default: None) |
-| ssl                                 | String  | No         | If set to `"true"` then use SSL via postgres sslmode `require` option. If the server does not accept SSL connections or the client certificate is not recognized the connection will fail. (Default: None) |
-| logical_poll_total_seconds          | Integer | No         | Stop running the tap when no data received from wal after certain number of seconds. (Default: 10800) |
-| break_at_end_lsn                    | Boolean | No         | Stop running the tap if the newly received lsn is after the max lsn that was detected when the tap started. (Default: true) |
-| max_run_seconds                     | Integer | No         | Stop running the tap after certain number of seconds. (Default: 43200) |
-| debug_lsn                           | String  | No         | If set to `"true"` then add `_sdc_lsn` property to the singer messages to debug postgres LSN position in the WAL stream. (Default: None) |
-| tap_id                              | String  | No         | ID of the pipeline/tap (Default: None) |
-| itersize                            | Integer | No         | Size of PG cursor iterator when doing INCREMENTAL or FULL_TABLE  (Default: 20000) |
-| default_replication_method          | String  | No         | Default replication method to use when no one is provided in the catalog (Values: `LOG_BASED`, `INCREMENTAL` or `FULL_TABLE`)  (Default: None) |
-| use_secondary                       | Boolean | No         | Use a database replica for `INCREMENTAL` and `FULL_TABLE` replication (Default : False) |
-| secondary_host                      | String  | No         | PostgreSQL Replica host (required if `use_secondary` is `True`) |
-| secondary_port                      | Integer | No         | PostgreSQL Replica port (required if `use_secondary` is `True`) |
+| Property                   | Type    | Required? | Default | Description                                                                                                                                                                                |
+|----------------------------|---------|----------|---------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| host                       | String  | Yes      | -       | PostgreSQL host                                                                                                                                                                            |
+| port                       | Integer | Yes      | -       | PostgreSQL port                                                                                                                                                                            |
+| user                       | String  | Yes      | -       | PostgreSQL user                                                                                                                                                                            |
+| password                   | String  | Yes      | -       | PostgreSQL password                                                                                                                                                                        |
+| dbname                     | String  | Yes      | -       | PostgreSQL database name                                                                                                                                                                   |
+| filter_schemas             | String  | No       | None    | Comma separated schema names to scan only the required schemas to improve the performance of data extraction.                                                                              |
+| ssl                        | String  | No       | None    | If set to `"true"` then use SSL via postgres sslmode `require` option. If the server does not accept SSL connections or the client certificate is not recognized the connection will fail. |
+| logical_poll_total_seconds | Integer | No       | 10800   | Stop running the tap when no data received from wal after certain number of seconds.                                                                                                       |
+| break_at_end_lsn           | Boolean | No       | true    | Stop running the tap if the newly received lsn is after the max lsn that was detected when the tap started.                                                                                |
+| max_run_seconds            | Integer | No       | 43200   | Stop running the tap after certain number of seconds.                                                                                                                                      |
+| debug_lsn                  | String  | No       | None    | If set to `"true"` then add `_sdc_lsn` property to the singer messages to debug postgres LSN position in the WAL stream.                                                                   |
+| tap_id                     | String  | No       | None    | ID of the pipeline/tap                                                                                                                                                                     |
+| itersize                   | Integer | No       | 20000   | Size of PG cursor iterator when doing INCREMENTAL or FULL_TABLE                                                                                                                            |
+| default_replication_method | String  | No       | None    | Default replication method to use when no one is provided in the catalog (Values: `LOG_BASED`, `INCREMENTAL` or `FULL_TABLE`)                                                              |
+| use_secondary              | Boolean | No       | False   | Use a database replica for `INCREMENTAL` and `FULL_TABLE` replication                                                                                                                      |
+| secondary_host             | String  | No       | -       | PostgreSQL Replica host (required if `use_secondary` is `True`)                                                                                                                            |
+| secondary_port             | Integer | No       | -       | PostgreSQL Replica port (required if `use_secondary` is `True`)                                                                                                                            |
+| limit                      | Integer | No       | None    | Adds a limit to INCREMENTAL queries to limit the number of records returns per run                                                                                                         |
 
 
 ### Run the tap in Discovery Mode
 
 ```
 tap-postgres --config config.json --discover                # Should dump a Catalog to stdout
 tap-postgres --config config.json --discover > catalog.json # Capture the Catalog
```

### Comparing `pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/PKG-INFO` & `pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-postgres
-Version: 2.0.0
+Version: 2.1.0
 Summary: Singer.io tap for extracting data from PostgresSQL - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-postgres
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
@@ -59,33 +59,34 @@
 }
 ```
 
 These are the same basic configuration properties used by the PostgreSQL command-line client (`psql`).
 
 Full list of options in `config.json`:
 
-| Property                            | Type    | Required?  | Description                                                   |
-|-------------------------------------|---------|------------|---------------------------------------------------------------|
-| host                                | String  | Yes        | PostgreSQL host                                               |
-| port                                | Integer | Yes        | PostgreSQL port                                               |
-| user                                | String  | Yes        | PostgreSQL user                                               |
-| password                            | String  | Yes        | PostgreSQL password                                           |
-| dbname                              | String  | Yes        | PostgreSQL database name                                      |
-| filter_schemas                      | String  | No         | Comma separated schema names to scan only the required schemas to improve the performance of data extraction. (Default: None) |
-| ssl                                 | String  | No         | If set to `"true"` then use SSL via postgres sslmode `require` option. If the server does not accept SSL connections or the client certificate is not recognized the connection will fail. (Default: None) |
-| logical_poll_total_seconds          | Integer | No         | Stop running the tap when no data received from wal after certain number of seconds. (Default: 10800) |
-| break_at_end_lsn                    | Boolean | No         | Stop running the tap if the newly received lsn is after the max lsn that was detected when the tap started. (Default: true) |
-| max_run_seconds                     | Integer | No         | Stop running the tap after certain number of seconds. (Default: 43200) |
-| debug_lsn                           | String  | No         | If set to `"true"` then add `_sdc_lsn` property to the singer messages to debug postgres LSN position in the WAL stream. (Default: None) |
-| tap_id                              | String  | No         | ID of the pipeline/tap (Default: None) |
-| itersize                            | Integer | No         | Size of PG cursor iterator when doing INCREMENTAL or FULL_TABLE  (Default: 20000) |
-| default_replication_method          | String  | No         | Default replication method to use when no one is provided in the catalog (Values: `LOG_BASED`, `INCREMENTAL` or `FULL_TABLE`)  (Default: None) |
-| use_secondary                       | Boolean | No         | Use a database replica for `INCREMENTAL` and `FULL_TABLE` replication (Default : False) |
-| secondary_host                      | String  | No         | PostgreSQL Replica host (required if `use_secondary` is `True`) |
-| secondary_port                      | Integer | No         | PostgreSQL Replica port (required if `use_secondary` is `True`) |
+| Property                   | Type    | Required? | Default | Description                                                                                                                                                                                |
+|----------------------------|---------|----------|---------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| host                       | String  | Yes      | -       | PostgreSQL host                                                                                                                                                                            |
+| port                       | Integer | Yes      | -       | PostgreSQL port                                                                                                                                                                            |
+| user                       | String  | Yes      | -       | PostgreSQL user                                                                                                                                                                            |
+| password                   | String  | Yes      | -       | PostgreSQL password                                                                                                                                                                        |
+| dbname                     | String  | Yes      | -       | PostgreSQL database name                                                                                                                                                                   |
+| filter_schemas             | String  | No       | None    | Comma separated schema names to scan only the required schemas to improve the performance of data extraction.                                                                              |
+| ssl                        | String  | No       | None    | If set to `"true"` then use SSL via postgres sslmode `require` option. If the server does not accept SSL connections or the client certificate is not recognized the connection will fail. |
+| logical_poll_total_seconds | Integer | No       | 10800   | Stop running the tap when no data received from wal after certain number of seconds.                                                                                                       |
+| break_at_end_lsn           | Boolean | No       | true    | Stop running the tap if the newly received lsn is after the max lsn that was detected when the tap started.                                                                                |
+| max_run_seconds            | Integer | No       | 43200   | Stop running the tap after certain number of seconds.                                                                                                                                      |
+| debug_lsn                  | String  | No       | None    | If set to `"true"` then add `_sdc_lsn` property to the singer messages to debug postgres LSN position in the WAL stream.                                                                   |
+| tap_id                     | String  | No       | None    | ID of the pipeline/tap                                                                                                                                                                     |
+| itersize                   | Integer | No       | 20000   | Size of PG cursor iterator when doing INCREMENTAL or FULL_TABLE                                                                                                                            |
+| default_replication_method | String  | No       | None    | Default replication method to use when no one is provided in the catalog (Values: `LOG_BASED`, `INCREMENTAL` or `FULL_TABLE`)                                                              |
+| use_secondary              | Boolean | No       | False   | Use a database replica for `INCREMENTAL` and `FULL_TABLE` replication                                                                                                                      |
+| secondary_host             | String  | No       | -       | PostgreSQL Replica host (required if `use_secondary` is `True`)                                                                                                                            |
+| secondary_port             | Integer | No       | -       | PostgreSQL Replica port (required if `use_secondary` is `True`)                                                                                                                            |
+| limit                      | Integer | No       | None    | Adds a limit to INCREMENTAL queries to limit the number of records returns per run                                                                                                         |
 
 
 ### Run the tap in Discovery Mode
 
 ```
 tap-postgres --config config.json --discover                # Should dump a Catalog to stdout
 tap-postgres --config config.json --discover > catalog.json # Capture the Catalog
```

### Comparing `pipelinewise-tap-postgres-2.0.0/pipelinewise_tap_postgres.egg-info/SOURCES.txt` & `pipelinewise-tap-postgres-2.1.0/pipelinewise_tap_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-postgres-2.0.0/setup.py` & `pipelinewise-tap-postgres-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='pipelinewise-tap-postgres',
-      version='2.0.0',
+      version='2.1.0',
       description='Singer.io tap for extracting data from PostgresSQL - PipelineWise compatible',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Wise',
       url='https://github.com/transferwise/pipelinewise-tap-postgres',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3',
@@ -20,15 +20,15 @@
       install_requires=[
           'pipelinewise-singer-python==1.*',
           'psycopg2-binary==2.9.5',
           'strict-rfc3339==0.7',
       ],
       extras_require={
           "test": [
-              'pytest==7.2.0',
+              'pytest==7.2.2',
               'pylint==2.12.*',
               'pytest-cov==4.0.0'
           ]
       },
       entry_points='''
           [console_scripts]
           tap-postgres=tap_postgres:main
```

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/__init__.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,16 @@
 
 
 def main_impl():
     """
     Main method
     """
     args = parse_args(REQUIRED_CONFIG_KEYS)
+
+    limit = args.config.get('limit')
     conn_config = {
         # Required config keys
         'host': args.config['host'],
         'user': args.config['user'],
         'password': args.config['password'],
         'port': args.config['port'],
         'dbname': args.config['dbname'],
@@ -403,14 +405,15 @@
         'tap_id': args.config.get('tap_id'),
         'filter_schemas': args.config.get('filter_schemas'),
         'debug_lsn': args.config.get('debug_lsn') == 'true',
         'max_run_seconds': args.config.get('max_run_seconds', 43200),
         'break_at_end_lsn': args.config.get('break_at_end_lsn', True),
         'logical_poll_total_seconds': float(args.config.get('logical_poll_total_seconds', 0)),
         'use_secondary': args.config.get('use_secondary', False),
+        'limit': int(limit) if limit else None
     }
 
     if conn_config['use_secondary']:
         try:
             conn_config.update({
                 # Host and Port are mandatory.
                 'secondary_host': args.config['secondary_host'],
```

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/db.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/db.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/discovery_utils.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/discovery_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/stream_utils.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/stream_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/common.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/full_table.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/incremental.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/incremental.py`

 * *Files 13% similar despite different names*

```diff
@@ -82,15 +82,17 @@
                 cur.itersize = post_db.CURSOR_ITER_SIZE
                 LOGGER.info("Beginning new incremental replication sync %s", stream_version)
                 select_sql = _get_select_sql({"escaped_columns": escaped_columns,
                                               "replication_key": replication_key,
                                               "replication_key_sql_datatype": replication_key_sql_datatype,
                                               "replication_key_value": replication_key_value,
                                               "schema_name": schema_name,
-                                              "stream": stream})
+                                              "table_name": stream['table_name'],
+                                              "limit": conn_info['limit']
+                                              })
                 LOGGER.info('select statement: %s with itersize %s', select_sql, cur.itersize)
                 cur.execute(select_sql)
 
                 rows_saved = 0
 
                 for rec in cur:
                     record_message = post_db.selected_row_to_singer_message(stream,
@@ -107,39 +109,37 @@
                     #event worse would be allowing the NULL value to enter into the state
                     if record_message.record[replication_key] is not None:
                         state = singer.write_bookmark(state,
                                                       stream['tap_stream_id'],
                                                       'replication_key_value',
                                                       record_message.record[replication_key])
 
-
                     if rows_saved % UPDATE_BOOKMARK_PERIOD == 0:
                         singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
                     counter.increment()
 
     return state
 
 
 def _get_select_sql(params):
     escaped_columns = params['escaped_columns']
-    replication_key = params['replication_key']
+    replication_key = post_db.prepare_columns_sql(params['replication_key'])
     replication_key_sql_datatype = params['replication_key_sql_datatype']
     replication_key_value = params['replication_key_value']
     schema_name = params['schema_name']
-    stream = params['stream']
-    if replication_key_value:
-        select_sql = f"""
-        SELECT {','.join(escaped_columns)}
-        FROM (
-            SELECT *
-            FROM {post_db.fully_qualified_table_name(schema_name, stream['table_name'])}
-            WHERE {post_db.prepare_columns_sql(replication_key)} >= '{replication_key_value}'::{replication_key_sql_datatype}
-            ORDER BY {post_db.prepare_columns_sql(replication_key)} ASC
-        ) pg_speedup_trick"""
-    else:
-        # if not replication_key_value
-        select_sql = f"""
-        SELECT {','.join(escaped_columns)}
-        FROM {post_db.fully_qualified_table_name(schema_name, stream['table_name'])}
-        """
+    table_name = params['table_name']
+
+    limit_statement = f'LIMIT {params["limit"]}' if params["limit"] else ''
+    where_statement = f"WHERE {replication_key} >= '{replication_key_value}'::{replication_key_sql_datatype}" \
+        if replication_key_value else ""
+
+    select_sql = f"""
+    SELECT {','.join(escaped_columns)}
+    FROM (
+        SELECT *
+        FROM {post_db.fully_qualified_table_name(schema_name, table_name)} 
+        {where_statement}
+        ORDER BY {replication_key} ASC {limit_statement}
+    ) pg_speedup_trick;"""
+
     return select_sql
```

### Comparing `pipelinewise-tap-postgres-2.0.0/tap_postgres/sync_strategies/logical_replication.py` & `pipelinewise-tap-postgres-2.1.0/tap_postgres/sync_strategies/logical_replication.py`

 * *Files identical despite different names*

