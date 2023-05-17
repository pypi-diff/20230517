# Comparing `tmp/aqueduct-sdk-0.3.2.tar.gz` & `tmp/aqueduct-sdk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-sdk-0.3.2.tar", last modified: Wed May 10 18:31:38 2023, max compression
+gzip compressed data, was "aqueduct-sdk-0.3.3.tar", last modified: Wed May 17 16:03:38 2023, max compression
```

## Comparing `aqueduct-sdk-0.3.2.tar` & `aqueduct-sdk-0.3.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.157794 aqueduct-sdk-0.3.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-10 18:31:38.157794 aqueduct-sdk-0.3.2/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.145794 aqueduct-sdk-0.3.2/aqueduct/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.145794 aqueduct-sdk-0.3.2/aqueduct/artifacts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/base_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/bool_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/generic_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/numeric_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/preview.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/system_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/table_artifact.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24525 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/backend/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/backend/response_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35841 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/constants/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6596 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/exports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/decorator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/flow_run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/github.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/globals/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/llm_wrapper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/dag_rules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/execution_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7640 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/operators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9747 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/response_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/airflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/aws.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/aws_lambda.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/connect_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/databricks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/dynamic_k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/ecr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/google_sheets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9035 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/salesforce.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3199 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/save.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/spark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12027 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/schedule.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/connect_config_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/dag_delta_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/dag_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/decorator_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/decorators_with_without_parentheses_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/enum_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/flow_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/helpers_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/metric_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/naming_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/serialization_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/python_function.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/test_dependency_folder/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/type_annotations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10504 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/dag_deltas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/describe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/format.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/function_packaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/integration_validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/local_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/naming.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16432 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/type_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8505 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-10.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-7.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-8.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-9.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-10 18:31:38.157794 aqueduct-sdk-0.3.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-09 23:19:59.000000 aqueduct-sdk-0.3.2/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/artifacts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/base_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/bool_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/generic_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/numeric_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/preview.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/system_metric.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/artifacts/table_artifact.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/backend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/backend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24525 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/backend/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/backend/response_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35831 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/constants/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6626 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/exports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/constants/metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/decorator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/error.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/flow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/flow_run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/github.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/globals/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/globals/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/llm_wrapper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.500865 aqueduct-sdk-0.3.3/aqueduct/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/dag_rules.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/execution_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7786 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/operators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12714 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/response_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/models/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/airflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/aws.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/aws_lambda.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/connect_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/databricks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/dynamic_k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/ecr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/google_sheets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9035 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/salesforce.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3528 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/save.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/spark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13374 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      738 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/resources/validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/schedule.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/connect_config_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/dag_delta_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/dag_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/decorator_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/decorators_with_without_parentheses_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/enum_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/flow_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/helpers_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/metric_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/naming_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/serialization_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/python_function.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.504865 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/test_dependency_folder/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/tests/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/type_annotations.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/aqueduct/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10726 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/dag_deltas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/describe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/format.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/function_packaging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/integration_validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/local_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/naming.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16574 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/type_inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8505 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/aqueduct/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7716 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-17 16:03:38.000000 aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/requirements/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-10.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-7.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-8.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/requirements/python-3-9.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 16:03:38.508865 aqueduct-sdk-0.3.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-17 00:29:47.000000 aqueduct-sdk-0.3.3/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-17 01:51:34.000000 aqueduct-sdk-0.3.3/version
```

### Comparing `aqueduct-sdk-0.3.2/PKG-INFO` & `aqueduct-sdk-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
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

### Comparing `aqueduct-sdk-0.3.2/aqueduct/__init__.py` & `aqueduct-sdk-0.3.3/aqueduct/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/_create.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/_create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/base_artifact.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/bool_artifact.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/bool_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/create.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/generic_artifact.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/generic_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/numeric_artifact.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/numeric_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/preview.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/preview.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/system_metric.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/system_metric.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/artifacts/table_artifact.py` & `aqueduct-sdk-0.3.3/aqueduct/artifacts/table_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/backend/api_client.py` & `aqueduct-sdk-0.3.3/aqueduct/backend/api_client.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/backend/response_helpers.py` & `aqueduct-sdk-0.3.3/aqueduct/backend/response_helpers.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/client.py` & `aqueduct-sdk-0.3.3/aqueduct/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,16 +282,16 @@
 
         if isinstance(config, dict):
             config = convert_dict_to_integration_connect_config(service, config)
         assert isinstance(config, BaseConnectionConfig)
 
         config = prepare_integration_config(service, config)
 
+        logger().info("Connecting to new %s integration `%s`..." % (service, name))
         globals.__GLOBAL_API_CLIENT__.connect_integration(name, service, config)
-        logger().info("Successfully connected to new %s integration `%s`." % (service, name))
 
     def delete_integration(
         self,
         name: str,
     ) -> None:
         """Deprecated. Use `client.delete_resource()` instead."""
         logger().warning(
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/constants/enums.py` & `aqueduct-sdk-0.3.3/aqueduct/constants/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     AQUEDUCT_ENGINE = "Aqueduct"
     DATABRICKS = "Databricks"
     EMAIL = "Email"
     SLACK = "Slack"
     SPARK = "Spark"
     AWS = "AWS"
     ECR = "ECR"
+    FILESYSTEM = "Filesystem"
 
 
 class RelationalDBServices(str, Enum, metaclass=MetaEnum):
     """Must match the corresponding entries in `ServiceType` exactly."""
 
     POSTGRES = "Postgres"
     SNOWFLAKE = "Snowflake"
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/decorator.py` & `aqueduct-sdk-0.3.3/aqueduct/decorator.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/error.py` & `aqueduct-sdk-0.3.3/aqueduct/error.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/flow.py` & `aqueduct-sdk-0.3.3/aqueduct/flow.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/flow_run.py` & `aqueduct-sdk-0.3.3/aqueduct/flow_run.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/github.py` & `aqueduct-sdk-0.3.3/aqueduct/github.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/llm_wrapper.py` & `aqueduct-sdk-0.3.3/aqueduct/llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/artifact.py` & `aqueduct-sdk-0.3.3/aqueduct/models/artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/config.py` & `aqueduct-sdk-0.3.3/aqueduct/models/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/dag.py` & `aqueduct-sdk-0.3.3/aqueduct/models/dag.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/dag_rules.py` & `aqueduct-sdk-0.3.3/aqueduct/models/dag_rules.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/execution_state.py` & `aqueduct-sdk-0.3.3/aqueduct/models/execution_state.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/integration.py` & `aqueduct-sdk-0.3.3/aqueduct/models/integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/operators.py` & `aqueduct-sdk-0.3.3/aqueduct/models/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 class ExtractSpec(BaseModel):
     service: ServiceType
     integration_id: uuid.UUID
     parameters: UnionExtractParams
 
 
 class RelationalDBLoadParams(BaseModel):
+    # If this field is parameterized, then it is expected to be empty.
+    # Instead, we will feed the parameter artifact into the save operator.
     table: str
     update_mode: LoadUpdateMode
 
 
 class SalesforceLoadParams(BaseModel):
     object: str
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/models/response_models.py` & `aqueduct-sdk-0.3.3/aqueduct/models/response_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 from datetime import datetime
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from aqueduct.constants.enums import (
     ArtifactType,
     ExecutionStatus,
     K8sClusterStatusType,
     SerializationType,
 )
@@ -18,14 +18,132 @@
 
 class ArtifactResult(BaseModel):
     serialization_type: SerializationType
     artifact_type: ArtifactType
     content: bytes
 
 
+# V2 Responses
+class GetDagResultResponse(BaseModel):
+    """Represents the result of a single workflow run.
+
+    Attributes:
+        id:
+            The id of the workflow run. This is the same id users can use to fetch
+            FlowRuns.
+        dag_id:
+            This id can be used to find the corresponding workflow dag version.
+        exec_state:
+            The execution state of the run result.
+
+    """
+
+    id: uuid.UUID
+    dag_id: uuid.UUID
+    exec_state: ExecutionState
+
+
+class GetOperatorResultResponse(BaseModel):
+    """Represents the result of a single operator in a workflow run.
+
+    Attributes:
+        id:
+            The id of the operator node result.
+        exec_state:
+            The execution state of the run result.
+    """
+
+    id: uuid.UUID
+    exec_state: ExecutionState
+
+
+class GetArtifactResultResponse(BaseModel):
+    """Represents the result of a single artifact in a workflow run.
+
+    Attributes:
+        id:
+            The id of the artifact node result.
+        serialization_type:
+            What is being serialized.
+        content_path:
+            Path to get content.
+        content_serialized:
+            If the content is too big, none. Otherwise, the content.
+        exec_state:
+            The execution state of the run result.
+    """
+
+    id: uuid.UUID
+    serialization_type: SerializationType
+    content_path: str
+    content_serialized: Optional[str]
+    exec_state: ExecutionState
+
+
+class GetNodeOperatorResponse(BaseModel):
+    """Represents a single operator in a workflow run.
+
+    Attributes:
+        id:
+            The id of the operator node.
+        dag_id:
+            This id can be used to find the corresponding workflow dag version.
+        name:
+            The name of the operator.
+        description:
+            The description of the operator.
+        spec:
+            The operator spec.
+        inputs:
+            The id(s) of the input artifact(s) of the operator.
+        outputs:
+            The id(s) of the output artifact(s) of the operator.
+
+    """
+
+    id: uuid.UUID
+    dag_id: uuid.UUID
+    name: str
+    description: str
+    spec: OperatorSpec
+    inputs: List[uuid.UUID]
+    outputs: List[uuid.UUID]
+
+
+class GetNodeArtifactResponse(BaseModel):
+    """Represents a single artifact in a workflow run.
+
+    Attributes:
+        id:
+            The id of the artifact node.
+        dag_id:
+            This id can be used to find the corresponding workflow dag version.
+        name:
+            The name of the artifact.
+        description:
+            The description of the artifact.
+        type:
+            The artifact type.
+        input:
+            The id of the input operator.
+        outputs:
+            The id(s) of the operator(s) that take this artifact as input.
+
+    """
+
+    id: uuid.UUID
+    dag_id: uuid.UUID
+    name: str
+    description: str
+    type: ArtifactType
+    input: uuid.UUID
+    outputs: List[uuid.UUID]
+
+
+# V1 Responses
 class PreviewResponse(BaseModel):
     """This is the response object returned by api_client.preview().
 
     Attributes:
         status:
             The execution state of preview.
         operator_results:
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/aws.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/aws.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/connect_config.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/connect_config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/dynamic_k8s.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/dynamic_k8s.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/ecr.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/ecr.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/google_sheets.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/google_sheets.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/mongodb.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/parameters.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/s3.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/salesforce.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/salesforce.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/save.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/save.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from typing import List
+from typing import List, Union
 
 from aqueduct.constants.enums import OperatorType
 from aqueduct.error import InvalidIntegrationException
 from aqueduct.globals import __GLOBAL_API_CLIENT__ as global_api_client
 from aqueduct.models.dag import DAG
 from aqueduct.models.integration import ResourceInfo
 from aqueduct.models.operators import LoadSpec, Operator, OperatorSpec, UnionLoadParams
@@ -13,24 +13,25 @@
     RemoveOperatorDelta,
     apply_deltas_to_dag,
 )
 from aqueduct.utils.utils import generate_uuid
 
 
 def _save_artifact(
-    artifact_id: uuid.UUID,
+    artifact_ids: Union[uuid.UUID, List[uuid.UUID]],
     dag: DAG,
     integration_info: ResourceInfo,
     save_params: UnionLoadParams,
 ) -> None:
     """Configures the given artifact to be written to a specific integration after it's computed in a published flow.
 
     Args:
-        artifact_id:
-            The artifact who's contents will be saved.
+        artifact_ids:
+            Can either be a single ID, or any number of IDs. In the latter case, that means that the first n-1 artifacts
+            are parameters to the save operators. The nth artifact is the one that will be saved.
         dag:
             The dag object that we will attach the load operator to.
         integration_info:
             Config info for the destination integration.
         save_params:
             Save configuration info (eg. table name, update mode).
 
@@ -39,31 +40,35 @@
             An error occurred because the requested integration could not be
             found.
         InvalidUserActionException:
             An error occurred because you are trying to load non-relational data into a relational integration.
         InvalidUserArgumentException:
             An error occurred because some necessary fields are missing in the SaveParams.
     """
+    if not isinstance(artifact_ids, list):
+        artifact_ids = [artifact_ids]
 
     integrations_map = global_api_client.list_resources()
     if integration_info.name not in integrations_map:
         raise InvalidIntegrationException(
             "Not connected to integration %s!" % integration_info.name
         )
 
     # We currently do not allow multiple save operators on the same artifact to the same integration.
     # We do allow multiple artifacts to write to the same integration, as well as a single artifact
     # to write to multiple integrations.
     save_op_name = "save to %s" % integration_info.name
 
     # Replace any existing save operator on this artifact that goes to the same integration.
+    artifact_id_to_save = artifact_ids[-1]
+
     deltas: List[DAGDelta] = []
     existing_save_ops = dag.list_operators(
         filter_to=[OperatorType.LOAD],
-        on_artifact_id=artifact_id,
+        on_artifact_id=artifact_id_to_save,
     )
     for op in existing_save_ops:
         assert op.spec.load is not None
         if op.spec.load.integration_id == integration_info.id:
             deltas.append(RemoveOperatorDelta(op.id))
 
     deltas.append(
@@ -75,15 +80,15 @@
                 spec=OperatorSpec(
                     load=LoadSpec(
                         service=integration_info.service,
                         integration_id=integration_info.id,
                         parameters=save_params,
                     )
                 ),
-                inputs=[artifact_id],
+                inputs=artifact_ids,
             ),
             output_artifacts=[],
         )
     )
 
     apply_deltas_to_dag(
         dag,
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/sql.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/sql.py`

 * *Files 7% similar despite different names*

```diff
@@ -233,41 +233,72 @@
             assert isinstance(artifact, TableArtifact)
             return artifact
         else:
             # We are in lazy mode.
             return TableArtifact(self._dag, sql_output_artifact_id)
 
     @validate_is_connected()
-    def save(self, artifact: BaseArtifact, table_name: str, update_mode: LoadUpdateMode) -> None:
+    def save(
+        self,
+        artifact: BaseArtifact,
+        table_name: Union[str, BaseArtifact],
+        update_mode: LoadUpdateMode,
+    ) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
 
         Args:
             artifact:
                 The artifact to save into this sql integration.
             table_name:
-                The table to save the artifact to.
+                The table to save the artifact to. You can also parameterize this field by passing
+                a string parameter here. When this save is parameterized, the table name parameter
+                will always be ordered before the artifact in the save operator's input list.
             update_mode:
                 Defines the semantics of the save if a table already exists.
                 Options are "replace", "append" (row-wise), or "fail" (if table already exists).
         """
         if self.type() == ServiceType.ATHENA:
             raise InvalidUserActionException(
                 "Save operation not supported for %s." % self.type().value
             )
+
+        if not isinstance(table_name, str) and not isinstance(table_name, BaseArtifact):
+            raise InvalidUserArgumentException(
+                "`table_name` must either be a string or a string parameter artifact."
+            )
+
+        table_name_str = table_name
+        artifact_ids = [artifact.id()]
+        if isinstance(table_name, BaseArtifact):
+            table_name_artifact = table_name
+            if table_name_artifact.type() != ArtifactType.STRING:
+                raise InvalidUserArgumentException(
+                    "A parameter value for `table_name` must be of string type."
+                )
+
+            # This is unset in the LoadParams, since we're parameterizing it.
+            table_name_str = ""
+
+            # Assumption: All parameter artifacts are prepended to the operator's input list.
+            artifact_ids = [table_name_artifact.id()] + artifact_ids
+        else:
+            if table_name_str == "":
+                raise InvalidUserArgumentException("Cannot save to an empty table name.")
+
         # Non-tabular data cannot be saved into relational data stores.
         if artifact.type() not in [ArtifactType.UNTYPED, ArtifactType.TABLE]:
             raise InvalidUserActionException(
                 "Unable to save non-relational data into relational data store `%s`." % self.name()
             )
 
         _save_artifact(
-            artifact.id(),
+            artifact_ids,
             self._dag,
             self._metadata,
-            save_params=RelationalDBLoadParams(table=table_name, update_mode=update_mode),
+            save_params=RelationalDBLoadParams(table=table_name_str, update_mode=update_mode),
         )
 
     def describe(self) -> None:
         """
         Prints out a human-readable description of the SQL integration.
         """
         print("==================== SQL Resource =============================")
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/resources/validation.py` & `aqueduct-sdk-0.3.3/aqueduct/resources/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from functools import wraps
 from typing import Any, Callable
 
 from aqueduct.utils.integration_validation import validate_integration_is_connected
 
 AnyFunc = Callable[..., Any]
 
 
 def validate_is_connected() -> Callable[[AnyFunc], AnyFunc]:
     """This decorator, which must be used on a Resource class method,
     ensures that the integration is connected before allowing the method to be called."""
 
     def decorator(method: AnyFunc) -> Callable[[AnyFunc], AnyFunc]:
+        @wraps(method)
         def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
             validate_integration_is_connected(self.name(), self._metadata.exec_state)
             return method(self, *args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/schedule.py` & `aqueduct-sdk-0.3.3/aqueduct/schedule.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/dag_delta_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/dag_delta_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/dag_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/dag_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/decorator_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/decorator_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/decorators_with_without_parentheses_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/decorators_with_without_parentheses_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/flow_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/helpers_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/metric_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/metric_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/serialization_test.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/tests/utils.py` & `aqueduct-sdk-0.3.3/aqueduct/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/dag_deltas.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/dag_deltas.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,18 @@
             # If requested, keep load operators on all artifacts along the way.
             if self.include_saves:
                 load_ops = dag.list_operators(
                     filter_to=[OperatorType.LOAD], on_artifact_id=curr_artifact_id
                 )
                 load_operator_ids.extend([op.id for op in load_ops])
 
+                # These load operators may also have input parameters, so we'll need to fetch those too.
+                for load_op in load_ops:
+                    upstream_artifact_ids.update(set(load_op.inputs[:-1]))
+
             # The operator who's output is the current artifact.
             curr_op = dag.must_get_operator(with_output_artifact_id=curr_artifact_id)
             candidate_next_artifact_ids = copy.copy(curr_op.inputs)
 
             implicit_types_to_include = []
             if self.include_checks:
                 implicit_types_to_include.append(OperatorType.CHECK)
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/describe.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/describe.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/function_packaging.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/function_packaging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/integration_validation.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/integration_validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/local_data.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/naming.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/naming.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/serialization.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,17 @@
 
 
 def _write_bytes_output(output: bytes) -> bytes:
     return output
 
 
 def _write_pickle_output(output: Any) -> bytes:
-    return bytes(pickle.dumps(output))
+    # Setting the protocol to pickle.DEFAULT_PROTOCOL is necessary for
+    # compatibility with Python 3.7.
+    return bytes(pickle.dumps(output, protocol=pickle.DEFAULT_PROTOCOL))
 
 
 def _write_json_output(output: Any) -> bytes:
     return json.dumps(output).encode(DEFAULT_ENCODING)
 
 
 def _write_tf_keras_model(output: Any) -> bytes:
```

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/type_inference.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/type_inference.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct/utils/utils.py` & `aqueduct-sdk-0.3.3/aqueduct/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/PKG-INFO` & `aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
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

### Comparing `aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/SOURCES.txt` & `aqueduct-sdk-0.3.3/aqueduct_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.2/setup.py` & `aqueduct-sdk-0.3.3/setup.py`

 * *Files identical despite different names*

