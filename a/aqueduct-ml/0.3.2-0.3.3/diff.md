# Comparing `tmp/aqueduct-ml-0.3.2.tar.gz` & `tmp/aqueduct-ml-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-ml-0.3.2.tar", last modified: Wed May 10 18:36:05 2023, max compression
+gzip compressed data, was "aqueduct-ml-0.3.3.tar", last modified: Wed May 17 17:21:29 2023, max compression
```

## Comparing `aqueduct-ml-0.3.2.tar` & `aqueduct-ml-0.3.3.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/operators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3010 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/athena.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3297 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/connector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15345 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6057 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/relational.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2023-05-09 23:16:09.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6878 2023-05-09 23:16:09.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5464 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/extract_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      435 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/timer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5737 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/bin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29290 2023-05-09 23:19:59.000000 aqueduct-ml-0.3.2/bin/aqueduct
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-09 23:19:59.000000 aqueduct-ml-0.3.2/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-09 23:19:59.000000 aqueduct-ml-0.3.2/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.632296 aqueduct-ml-0.3.3/aqueduct_executor/operators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/athena.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3990 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/connector.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16224 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6057 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/relational.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9602 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7001 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.636296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5478 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1276 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.640296 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/storage.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/timer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5737 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-17 17:21:29.000000 aqueduct-ml-0.3.3/aqueduct_ml.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/bin/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29290 2023-05-17 01:51:34.000000 aqueduct-ml-0.3.3/bin/aqueduct
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-17 01:51:34.000000 aqueduct-ml-0.3.3/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 17:21:29.644296 aqueduct-ml-0.3.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-17 00:29:47.000000 aqueduct-ml-0.3.3/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-17 01:51:34.000000 aqueduct-ml-0.3.3/version
```

### Comparing `aqueduct-ml-0.3.2/PKG-INFO` & `aqueduct-ml-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.2
+Version: 0.3.3
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -13,28 +13,28 @@
 
 
 <div align="center">
   <a href="https://aqueducthq.com">
     <img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width="40%" />
   </a>
   
-  <h2 style="border: 0px white;">The Python API to run machine learning in your cloud</h2>
+  <h2 style="border: 0px white;">Run LLMs and ML on any cloud infrastructure</h2>
 
 ### 📢 [Slack](https://slack.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🗺️ [Roadmap](https://roadmap.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🐞 [Report a bug](https://github.com/aqueducthq/aqueduct/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)&nbsp;&nbsp;|&nbsp;&nbsp;✍️ [Blog](https://blog.aqueducthq.com)
 
   
 [![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
 </div>
 
-**Aqueduct enables you to easily define, run, and manage AI & ML tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
+**Aqueduct is an MLOps framework that allows you to define and deploy machine learning and LLM workloads on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/867892/230214641-b0aec53b-4988-4581-84ed-134f97ed9276.png" width="80%" />
 </p>
 
 Aqueduct is an open-source MLOps framework that allows you to write code in vanilla Python, run that code on any cloud infrastructure you'd like to use, and gain visibility into the execution and performance of your models and predictions. **[See what infrastructure Aqueduct works with. →](https://aqueducthq.com/integrations/)**
 
@@ -49,31 +49,39 @@
 
 Aqueduct's Python native API allows you to define ML tasks in regular Python code. You can connect Aqueduct to your existing cloud infrastructure ([docs](https://docs.aqueducthq.com/integrations)), and Aqueduct will seamlessly move your code from your laptop to the cloud or between different cloud infrastructure layers. 
 
 <!--- TODO(vikram): Modify this once we add support for switching into/out of Databricks in a single workflow. --->
 For example, we can define a pipeline that trains a model on Kubernetes using a GPU and validates that model in AWS Lambda in a few lines of Python: 
 
 ```python
+# Use an existing LLM.
+vicuna = aq.llm_op('vicuna_7b', engine='eks-us-east-2')
+features = vicuna(
+    raw_logs,
+    { 
+        "prompt": 
+        "Turn this log entry into a CSV: {text}" 
+    }
+)
+
+# Or write a custom op on your favorite infrastructure!
 @op(
-  engine='eks-us-east-2', 
+  engine='kubernetes',
+  # Get a GPU.
   resources={'gpu_resource_name': 'nvidia.com/gpu'}
 )
-def train(features):
-  return model.train(features)
-
-@metric(engine='lambda-us-east-2')
-def validate(model):
-    return validation_test(model)
+def train(featurized_logs):
+  return model.train(features) # Train your model.
 
-validate(train(features))
+train(features)
 ```
 
 Once you publish this workflow to Aqueduct, you can see it on the UI: 
 
-![image](https://user-images.githubusercontent.com/867892/228295996-4ba3de23-3106-431d-93a9-afd8d77a707b.png)
+![image](https://github.com/aqueducthq/aqueduct/assets/867892/d0561772-8799-4046-92ae-3c975d70e47d)
 
 To see how to build your first workflow, check out our **[quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 ## Why Aqueduct?
 
 MLOps has become a [tangled mess of siloed infrastructure](https://aqueducthq.com/post/the-mlops-knot/). Most teams need to set up and operate many different cloud infrastructure tools to run ML effectively, but these tools have disparate APIs and interoperate poorly.
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `aqueduct-ml-0.3.3/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `aqueduct-ml-0.3.3/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 class Task:
     def __init__(self, task_id: str, spec: TaskSpec, alias: str):
         self.id = task_id
         self.spec = spec
         self.alias = alias
 
 
-def run(spec: spec.CompileAirflowSpec) -> None:
+def run(spec: spec.CompileAirflowSpec, version_tag: str) -> None:
     """
     Executes a compile airflow operator.
     """
     print("Started %s job: %s" % (spec.type, spec.name))
 
     storage = parse.parse_storage(spec.storage_config)
     exec_state = ExecutionState(user_logs=Logs())
 
     try:
-        dag_file = compile(spec)
+        dag_file = compile(spec, version_tag)
         utils.write_compile_airflow_output(storage, spec.output_content_path, dag_file)
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
     except Exception:
         traceback.print_exc()
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
         sys.exit(1)
 
 
-def compile(spec: spec.CompileAirflowSpec) -> bytes:
+def compile(spec: spec.CompileAirflowSpec, version_tag: str) -> bytes:
     """
     Takes a CompileAirflowSpec and generates an Airflow DAG specification Python file.
     It returns the DAG file.
     """
 
     schedule = None
     if spec.cron_schedule:
@@ -80,14 +80,15 @@
     r = template.render(
         workflow_dag_id=spec.workflow_dag_id,
         dag_id=spec.dag_id,
         schedule=schedule,
         tasks=tasks,
         edges=edges,
         task_to_alias=task_to_alias,
+        version_tag=version_tag,
     )
 
     return str.encode(r)
 
 
 def flatten_task_edges(edges: Dict[str, List[str]]) -> List[Tuple[str, str]]:
     """
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/spec.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/athena.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/bigquery.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pandas as pd
 from aqueduct_executor.operators.connectors.data import common, config, connector, extract, load
 from aqueduct_executor.operators.utils.enums import ArtifactType
 from aqueduct_executor.operators.utils.saved_object_delete import SavedObjectDelete
 from aqueduct_executor.operators.utils.utils import delete_object
 from google.cloud import bigquery
+from google.cloud.exceptions import NotFound
 from google.oauth2 import service_account
 
 
 class BigQueryConnector(connector.DataConnector):
     def __init__(self, config: config.BigQueryConfig):
         self.project_id = config.project_id
 
@@ -44,14 +45,32 @@
             results.append(delete_object(table, self._delete_object))
         return results
 
     def load(self, params: load.RelationalParams, df: Any, artifact_type: ArtifactType) -> None:
         if artifact_type != ArtifactType.TABLE:
             raise Exception("The data being loaded must be of type table, found %s" % artifact_type)
 
+        # The expected table name format is <DATASET>.<TABLE> so we try to parse
+        # just the dataset name here.
+        parts = params.table.split(".")
+        if len(parts) == 0:
+            raise Exception(
+                "Invalid name provided for BigQuery dataset and table: %s" % params.table
+            )
+
+        # Check if dataset actually exists
+        dataset_id = parts[0]
+        try:
+            self.client.get_dataset(dataset_id)
+        except NotFound:
+            raise Exception(
+                "The dataset %s does not exist. Please save to a dataset that already exists."
+                % dataset_id
+            )
+
         update_mode = params.update_mode
         write_disposition = bigquery.WriteDisposition.WRITE_TRUNCATE  # Default
         if update_mode == common.UpdateMode.APPEND:
             write_disposition = bigquery.WriteDisposition.WRITE_APPEND
         if update_mode == common.UpdateMode.REPLACE:
             write_disposition = bigquery.WriteDisposition.WRITE_TRUNCATE
         if update_mode == common.UpdateMode.FAIL:
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/common.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/config.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/connector.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import platform
 import sys
 from typing import Any
 
 from aqueduct_executor.operators.connectors.data import common, config, connector, extract
+from aqueduct_executor.operators.connectors.data.load import RelationalParams
 from aqueduct_executor.operators.connectors.data.spec import (
     AQUEDUCT_DEMO_NAME,
     AuthenticateSpec,
     DiscoverSpec,
     ExtractSpec,
     LoadSpec,
     LoadTableSpec,
@@ -261,27 +262,42 @@
     exec_state: ExecutionState,
     read_artifacts_func: Any,
     is_spark: bool,
     **kwargs: Any,
 ) -> None:
     inputs, input_types, _ = read_artifacts_func(
         storage=storage,
-        input_paths=[spec.input_content_path],
-        input_metadata_paths=[spec.input_metadata_path],
+        input_paths=spec.input_content_paths,
+        input_metadata_paths=spec.input_metadata_paths,
         **kwargs,
     )
-    if len(inputs) != 1:
-        raise Exception("Expected 1 input artifact, but got %d" % len(inputs))
+    if len(inputs) == 0:
+        raise Exception("Expected at least one input artifact!")
+    if len(inputs) > 2:
+        raise Exception("Unexpected number of inputs to save operator: %v.", len(inputs))
+
+    # Handle any parameterization of the save queries here. Currently, we only support
+    # the parameterization of the `table_name` for SQL connectors.
+    if len(inputs) > 1:
+        if not isinstance(spec.parameters, RelationalParams):
+            raise Exception("Only relational database resources support parameterized saves.")
+
+        assert (
+            len(spec.parameters.table) == 0
+        ), "A parameterized relational save spec should have an empty table name."
+        assert isinstance(inputs[0], str), "Relational saves can only have string parameters."
+        spec.parameters.table = inputs[0]
 
+    # Any parameters are expected to have been resolved by the time we get here.
     @exec_state.user_fn_redirected(failure_tip=TIP_LOAD)
     def _load() -> None:
         if is_spark:
-            op.load_spark(spec.parameters, inputs[0], input_types[0])  # type: ignore
+            op.load_spark(spec.parameters, inputs[-1], input_types[-1])  # type: ignore
         else:
-            op.load(spec.parameters, inputs[0], input_types[0])
+            op.load(spec.parameters, inputs[-1], input_types[-1])
 
     _load()
 
 
 def run_load_table(
     spec: LoadTableSpec,
     op: connector.DataConnector,
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/extract.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/gcs.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/main.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,36 @@
 import argparse
 import base64
+import sys
 
-from aqueduct_executor.operators.connectors.data import execute
-from aqueduct_executor.operators.connectors.data.spec import parse_spec
-from aqueduct_executor.operators.utils.utils import time_it
+from aqueduct_executor.operators.system_metric_executor import execute
+from aqueduct_executor.operators.system_metric_executor.spec import parse_spec
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("-s", "--spec", required=True)
+    parser.add_argument("-v", "--version-tag", default="")
     args = parser.parse_args()
+    if args.version_tag:
+        import subprocess
+
+        install_process = subprocess.run(
+            [
+                sys.executable,
+                "-m",
+                "pip",
+                "install",
+                "--index-url",
+                "https://test.pypi.org/simple/",
+                "--extra-index-url",  # allows dependencies from pypi
+                "https://pypi.org/simple",
+                f"aqueduct-ml=={args.version_tag}",
+            ]
+        )
+        print(install_process.stderr)
+        print(install_process.stdout)
+        install_process.check_returncode()
 
     spec_json = base64.b64decode(args.spec)
     spec = parse_spec(spec_json)
 
-    time_it(job_name=spec.name, job_type=spec.type.value, step="Running Connector")(execute.run)(
-        spec
-    )
+    execute.run(spec)
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/models.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mongodb.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mysql.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/postgres.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/relational.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
+from http import HTTPStatus
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 import pandas as pd
 from aqueduct.utils.serialization import deserialize
 from aqueduct_executor.operators.connectors.data import connector, extract, load
 from aqueduct_executor.operators.connectors.data.config import S3Config
 from aqueduct_executor.operators.connectors.data.s3_serialization import (
+    S3InsufficientPermissionsException,
+    S3RootFolderCreationException,
     S3UnknownFileFormatException,
     S3UnsupportedArtifactTypeException,
     _s3_deserialization_function_mapping,
     artifact_type_to_s3_serialization_type,
     serialize_val_for_s3,
 )
 from aqueduct_executor.operators.connectors.data.utils import construct_boto_session
@@ -34,21 +37,35 @@
             self.s3.meta.client.head_bucket(Bucket=self.bucket)
         except ClientError as e:
             raise Exception(
                 "Bucket does not exist or you do not have permission to access the bucket: %s."
                 % str(e)
             )
 
-        # Check that any user-supplied root directory exists.
-        if self.root_dir != "":
-            # If nothing is returned by this filter call, then the directory does not exist.
-            if len(list(self.s3.Bucket(self.bucket).objects.filter(Prefix=self.root_dir))) == 0:
-                raise Exception(
-                    "Supplied root directory `%s` does not exist in bucket %s."
-                    % (self.root_dir, self.bucket)
+        # Check that any user-supplied root directory exists. If the object key name does not exist,
+        # create a new one.
+        try:
+            if self.root_dir != "":
+                # If nothing is returned by this filter call, then the directory does not exist.
+                if len(list(self.s3.Bucket(self.bucket).objects.filter(Prefix=self.root_dir))) == 0:
+                    if not self.root_dir.endswith("/"):
+                        self.root_dir = self.root_dir + "/"
+                    bucket = self.s3.Bucket(self.bucket)
+                    bucket.put_object(Bucket=self.bucket, Key=self.root_dir)
+        except ClientError as e:
+            status_code = e.response["ResponseMetadata"]["HTTPStatusCode"]
+            if status_code == HTTPStatus.FORBIDDEN:
+                raise S3InsufficientPermissionsException(
+                    "The specified root folder {} does not exist and you do not have permission to modify the bucket {} to create the folder.".format(
+                        self.root_dir, self.bucket
+                    )
+                )
+            else:
+                raise S3RootFolderCreationException(
+                    "Failed to create root folder in bucket {} with {}".format(self.bucket, str(e))
                 )
 
     def discover(self) -> List[str]:
         raise Exception("Discover is not supported for S3.")
 
     def fetch_object(self, key: str, params: extract.S3Params) -> Any:
         response = self.s3.Object(self.bucket, key).get()
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,22 @@
     pass
 
 
 class S3UnknownFileFormatException(Exception):
     pass
 
 
+class S3InsufficientPermissionsException(Exception):
+    pass
+
+
+class S3RootFolderCreationException(Exception):
+    pass
+
+
 def artifact_type_to_s3_serialization_type(
     artifact_type: ArtifactType,
     format: Optional[S3TableFormat],
     ignore_format_requirement: bool = False,
 ) -> S3SerializationType:
     if artifact_type == ArtifactType.TABLE:
         if format is None:
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/snowflake.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/s3.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spec.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,16 @@
     name: str
     type: Literal[enums.JobType.LOAD]
     storage_config: sconfig.StorageConfig
     metadata_path: str
     connector_name: common.Name
     connector_config: config.Config
     parameters: load.Params
-    input_content_path: str
-    input_metadata_path: str
+    input_content_paths: List[str]
+    input_metadata_paths: List[str]
 
     # validators
     _unwrap_connector_config = validator("connector_config", allow_reuse=True, pre=True)(
         unwrap_connector_config
     )
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sql_server.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sqlite.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/utils.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/conf.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/utils.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/extract_function.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/get_extract_path.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/install_requirements.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/set_conda_version.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/spec.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/spec.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_data.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_function.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/execute_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/utils.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/execute.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/spec.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/enums.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/execution.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/config.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/file.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/gcs.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/parse.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/s3.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/timer.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/utils.py` & `aqueduct-ml-0.3.3/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/aqueduct_ml.egg-info/PKG-INFO` & `aqueduct-ml-0.3.3/aqueduct_ml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.2
+Version: 0.3.3
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -13,28 +13,28 @@
 
 
 <div align="center">
   <a href="https://aqueducthq.com">
     <img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width="40%" />
   </a>
   
-  <h2 style="border: 0px white;">The Python API to run machine learning in your cloud</h2>
+  <h2 style="border: 0px white;">Run LLMs and ML on any cloud infrastructure</h2>
 
 ### 📢 [Slack](https://slack.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🗺️ [Roadmap](https://roadmap.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🐞 [Report a bug](https://github.com/aqueducthq/aqueduct/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)&nbsp;&nbsp;|&nbsp;&nbsp;✍️ [Blog](https://blog.aqueducthq.com)
 
   
 [![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
 </div>
 
-**Aqueduct enables you to easily define, run, and manage AI & ML tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
+**Aqueduct is an MLOps framework that allows you to define and deploy machine learning and LLM workloads on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/867892/230214641-b0aec53b-4988-4581-84ed-134f97ed9276.png" width="80%" />
 </p>
 
 Aqueduct is an open-source MLOps framework that allows you to write code in vanilla Python, run that code on any cloud infrastructure you'd like to use, and gain visibility into the execution and performance of your models and predictions. **[See what infrastructure Aqueduct works with. →](https://aqueducthq.com/integrations/)**
 
@@ -49,31 +49,39 @@
 
 Aqueduct's Python native API allows you to define ML tasks in regular Python code. You can connect Aqueduct to your existing cloud infrastructure ([docs](https://docs.aqueducthq.com/integrations)), and Aqueduct will seamlessly move your code from your laptop to the cloud or between different cloud infrastructure layers. 
 
 <!--- TODO(vikram): Modify this once we add support for switching into/out of Databricks in a single workflow. --->
 For example, we can define a pipeline that trains a model on Kubernetes using a GPU and validates that model in AWS Lambda in a few lines of Python: 
 
 ```python
+# Use an existing LLM.
+vicuna = aq.llm_op('vicuna_7b', engine='eks-us-east-2')
+features = vicuna(
+    raw_logs,
+    { 
+        "prompt": 
+        "Turn this log entry into a CSV: {text}" 
+    }
+)
+
+# Or write a custom op on your favorite infrastructure!
 @op(
-  engine='eks-us-east-2', 
+  engine='kubernetes',
+  # Get a GPU.
   resources={'gpu_resource_name': 'nvidia.com/gpu'}
 )
-def train(features):
-  return model.train(features)
-
-@metric(engine='lambda-us-east-2')
-def validate(model):
-    return validation_test(model)
+def train(featurized_logs):
+  return model.train(features) # Train your model.
 
-validate(train(features))
+train(features)
 ```
 
 Once you publish this workflow to Aqueduct, you can see it on the UI: 
 
-![image](https://user-images.githubusercontent.com/867892/228295996-4ba3de23-3106-431d-93a9-afd8d77a707b.png)
+![image](https://github.com/aqueducthq/aqueduct/assets/867892/d0561772-8799-4046-92ae-3c975d70e47d)
 
 To see how to build your first workflow, check out our **[quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 ## Why Aqueduct?
 
 MLOps has become a [tangled mess of siloed infrastructure](https://aqueducthq.com/post/the-mlops-knot/). Most teams need to set up and operate many different cloud infrastructure tools to run ML effectively, but these tools have disparate APIs and interoperate poorly.
```

### Comparing `aqueduct-ml-0.3.2/aqueduct_ml.egg-info/SOURCES.txt` & `aqueduct-ml-0.3.3/aqueduct_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.2/bin/aqueduct` & `aqueduct-ml-0.3.3/bin/aqueduct`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
 PYODBC_VERSION_BOUND = "<=4.0.35"
 
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.3.2"
+package_version = "0.3.3"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
```

### Comparing `aqueduct-ml-0.3.2/setup.py` & `aqueduct-ml-0.3.3/setup.py`

 * *Files identical despite different names*

