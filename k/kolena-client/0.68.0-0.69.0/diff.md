# Comparing `tmp/kolena_client-0.68.0.tar.gz` & `tmp/kolena_client-0.69.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.68.0.tar", max compression
+gzip compressed data, was "kolena_client-0.69.0.tar", max compression
```

## Comparing `kolena_client-0.68.0.tar` & `kolena_client-0.69.0.tar`

### file list

```diff
@@ -1,105 +1,102 @@
--rw-r--r--   0        0        0    11346 2023-05-09 21:48:51.859365 kolena_client-0.68.0/LICENSE
--rw-r--r--   0        0        0      556 2023-05-09 21:48:51.859365 kolena_client-0.68.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1405 2023-05-09 21:48:51.859365 kolena_client-0.68.0/README.md
--rw-r--r--   0        0        0     1356 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1725 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     7594 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7480 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5507 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      690 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/samples.py
--rw-r--r--   0        0        0      833 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0      784 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/_consts.py
--rw-r--r--   0        0        0     1604 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     7115 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1260 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/futures.py
--rw-r--r--   0        0        0     1183 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2646 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4866 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/log.py
--rw-r--r--   0        0        0      997 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     4768 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     6672 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/stratification.py
--rw-r--r--   0        0        0     1942 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3005 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    14914 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3578 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     2645 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4138 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8540 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13501 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    12954 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     4707 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0      689 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/_consts.py
--rw-r--r--   0        0        0    20512 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9301 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14447 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12177 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    17008 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15282 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     4134 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/initialize.py
--rw-r--r--   0        0        0     4550 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6052 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     7794 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    15849 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0     9312 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3359 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3433 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      760 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     7762 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7571 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13233 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22814 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     9155 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    11542 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9293 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     1925 2023-05-09 21:49:11.668943 kolena_client-0.68.0/pyproject.toml
--rw-r--r--   0        0        0     2973 1970-01-01 00:00:00.000000 kolena_client-0.68.0/setup.py
--rw-r--r--   0        0        0     3275 1970-01-01 00:00:00.000000 kolena_client-0.68.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-17 01:43:54.191003 kolena_client-0.69.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-05-17 01:43:54.191003 kolena_client-0.69.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1546 2023-05-17 01:43:54.191003 kolena_client-0.69.0/README.md
+-rw-r--r--   0        0        0     1356 2023-05-17 01:54:04.798995 kolena_client-0.69.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-17 01:43:54.191003 kolena_client-0.69.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-17 01:43:54.191003 kolena_client-0.69.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-05-17 01:43:54.191003 kolena_client-0.69.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-05-17 01:43:54.191003 kolena_client-0.69.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     8201 2023-05-17 01:43:54.191003 kolena_client-0.69.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-05-17 01:43:54.191003 kolena_client-0.69.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-05-17 01:43:54.191003 kolena_client-0.69.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5540 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      783 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4970 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5481 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3235 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15591 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3578 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     2645 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4138 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8572 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13515 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12407 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    12957 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     4716 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-05-17 01:43:54.195003 kolena_client-0.69.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20512 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9319 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14479 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12196 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16929 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15301 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3544 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4550 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6052 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     7794 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    15849 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0     9318 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3359 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3433 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      846 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0    14420 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7592 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13372 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22779 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     9155 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    14458 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9326 2023-05-17 01:43:54.199003 kolena_client-0.69.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     2560 2023-05-17 01:54:04.798995 kolena_client-0.69.0/pyproject.toml
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 kolena_client-0.69.0/setup.py
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 kolena_client-0.69.0/PKG-INFO
```

### Comparing `kolena_client-0.68.0/LICENSE` & `kolena_client-0.69.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/LICENSE_HEADER` & `kolena_client-0.69.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/README.md` & `kolena_client-0.69.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 <p align="center">
   <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />
 </p>
 
 <p align='center'>
-  <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>
-  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>
-  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>
-  <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>
+  <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena" /></a>
+  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena" /></a>
+  <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk" /></a>
+  <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1"/></a>
+  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/resource-docs-6434c1" /></a>
 </p>
 
 ---
 
 [Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden
 model behaviors and take the mystery out of model development. Kolena helps you:
 
 - Perform high-resolution model evaluation
 - Understand and track behavioral improvements and regressions
 - Meaningfully communicate model capabilities
 - Automate model testing and deployment workflows
 
-`kolena-client` is the Python client library for programmatic interaction with Kolena.
+This `kolena` package contains the Python client library for programmatic interaction with the Kolena ML testing
+platform.
 
 ## Documentation
 
 Visit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the
-[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena-client` typing and
+[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena` typing and
 function documentation.
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
                                    [Kolena]
- [https://img.shields.io/pypi/v/kolena-client] [https://img.shields.io/pypi/l/
-   kolena-client] [https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-
-      6434c1] [https://img.shields.io/badge/docs-API%20Reference-6434c1]
+[https://img.shields.io/pypi/v/kolena] [https://img.shields.io/pypi/l/kolena]
+ [https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk] [https://
+ codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1]
+              [https://img.shields.io/badge/resource-docs-6434c1]
 --- [Kolena](https://www.kolena.io) is a comprehensive machine learning testing
 and debugging platform to surface hidden model behaviors and take the mystery
 out of model development. Kolena helps you: - Perform high-resolution model
 evaluation - Understand and track behavioral improvements and regressions -
 Meaningfully communicate model capabilities - Automate model testing and
-deployment workflows `kolena-client` is the Python client library for
-programmatic interaction with Kolena. ## Documentation Visit [docs.kolena.io]
-(https://docs.kolena.io/) for tutorial and usage documentation and the [API
-Reference](https://app.kolena.io/api/developer/docs/html/index.html) for
-detailed `kolena-client` typing and function documentation.
+deployment workflows This `kolena` package contains the Python client library
+for programmatic interaction with the Kolena ML testing platform. ##
+Documentation Visit [docs.kolena.io](https://docs.kolena.io/) for tutorial and
+usage documentation and the [API Reference](https://app.kolena.io/api/
+developer/docs/html/index.html) for detailed `kolena` typing and function
+documentation.
```

### Comparing `kolena_client-0.68.0/kolena/__init__.py` & `kolena_client-0.69.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_api/__init__.py` & `kolena_client-0.69.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_api/v1/__init__.py` & `kolena_client-0.69.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.69.0/kolena/_api/v1/batched_load.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         INIT_UPLOAD = "/batched-load/upload/init"
         COMPLETE_DOWNLOAD = "/batched-load/download/complete"
         UPLOAD_SIGNED_URL_STUB = "/batched-load/upload/signed-url"
         DOWNLOAD_BY_PATH_STUB = "/batched-load/download/by-path"
 
         @classmethod
         def upload_signed_url(cls, load_uuid: str) -> str:
-            return f"{cls.UPLOAD_SIGNED_URL_STUB}/{load_uuid}"
+            return f"{cls.UPLOAD_SIGNED_URL_STUB.value}/{load_uuid}"
 
         @classmethod
         def download_by_path(cls, path: str) -> str:
-            return f"{cls.DOWNLOAD_BY_PATH_STUB}/{path}"
+            return f"{cls.DOWNLOAD_BY_PATH_STUB.value}/{path}"
 
     @dataclass(frozen=True)
     class WithLoadUUID:
         uuid: str
 
     @dataclass(frozen=True)
     class SignedURL:
```

### Comparing `kolena_client-0.68.0/kolena/_api/v1/client_log.py` & `kolena_client-0.69.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_api/v1/core.py` & `kolena_client-0.69.0/kolena/_api/v1/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         workflow: str
         compute_metrics_where_possible: bool = False
         compute_metrics_models: Optional[List[int]] = None
 
     @dataclass(frozen=True)
     class CreateFromExistingResponse:
         test_case_id: int
-        test_suite_id: int
+        test_suite_id: int  # newly created version ID
 
     @dataclass(frozen=True)
     class LoadByNameRequest:
         name: str
         version: Optional[int] = None
 
     @dataclass(frozen=True)
@@ -122,54 +122,69 @@
         test_case_names: List[str]
         uuids: List[str]
         compute_metrics_where_possible: bool = False
         compute_metrics_models: Optional[List[int]] = None
 
     @dataclass(frozen=True)
     class BulkCreateFromExistingResult:
-        test_suite_id: int
+        test_suite_id: int  # ID of specific version
         test_suite_name: str
         test_suite_description: Optional[str]
         test_cases: List[TestCaseInfo]
 
 
 class TestSuite:
     @dataclass(frozen=True)
     class CreateRequest:
         name: str
         description: str
         workflow: str
+        tags: Optional[List[str]] = None
 
     @dataclass(frozen=True)
     class LoadByNameRequest:
         name: str
         version: Optional[int] = None
 
     @dataclass(frozen=True)
+    class LoadAllRequest:
+        workflow: str
+        tags: Optional[List[str]] = None
+
+    @dataclass(frozen=True)
     class EntityData:
         id: int
         name: str
         version: int
         description: str
         test_cases: List[TestCase.EntityData]
         workflow: str
+        tags: List[str]
+
+    @dataclass(frozen=True)
+    class LoadAllResponse:
+        test_suites: List["TestSuite.EntityData"]
 
     @dataclass(frozen=True)
     class EditRequest:
-        test_suite_id: int
+        test_suite_id: int  # ID of version being edited
         current_version: int
         name: str
         description: str
         test_case_ids: List[int]
+        tags: Optional[List[str]] = None  # unique set -- list used to preserve ordering
 
     @dataclass(frozen=True)
     class DeleteRequest:
         test_suite_id: int
 
 
+TestSuite.LoadAllResponse.__pydantic_model__.update_forward_refs()
+
+
 class TestRun:
     @dataclass(frozen=True)
     class MarkCrashedRequest:
         test_run_id: int
 
 
 CATEGORICAL = "categorical"
@@ -178,18 +193,18 @@
 
 @dataclass(frozen=True)
 class Dimension:
     column: Literal["test_sample", "test_sample_metadata", "ground_truth"]
     field: str
     datatype: Literal["categorical", "numeric"]
 
-    def is_categorical(self):
+    def is_categorical(self) -> bool:
         return self.datatype == CATEGORICAL
 
-    def is_numeric(self):
+    def is_numeric(self) -> bool:
         return self.datatype == NUMERIC
 
 
 @dataclass(frozen=True)
 class CategoricalBucket:
     values: Union[List[StrictStr], List[StrictBool]]
 
@@ -209,15 +224,15 @@
 @dataclass(frozen=True)
 class DimensionSpec:
     # arbitrarily selected max_length for sanity reason
     name: constr(min_length=1, max_length=100)
     columns: conlist(Dimension, min_items=1, max_items=3)
     buckets: Dict[str, List[Union[CategoricalBucket, NumericBucket]]]
 
-    def __post_init_post_parse__(self):
+    def __post_init_post_parse__(self) -> None:
         n_cols = len(self.columns)
         # auto-stratification only supported for single categorical field
         if not self.buckets and not self.should_auto_stratify():
             raise ValueError("Empty bucket.")
 
         check_duplicate_fields(self.columns)
 
@@ -227,44 +242,44 @@
 
             for dimension, filter in zip(self.columns, filters):
                 if (dimension.is_categorical() and not isinstance(filter, CategoricalBucket)) or (
                     dimension.is_numeric() and not isinstance(filter, NumericBucket)
                 ):
                     raise ValueError(f"Column {dimension} has incompatible filter.")
 
-    def should_auto_stratify(self):
+    def should_auto_stratify(self) -> bool:
         return not self.buckets and len(self.columns) == 1 and self.columns[0].is_categorical()
 
 
 @dataclass(frozen=True)
 class BaseStratifyRequest:
     workflow: str
     test_case_id: int
     test_suite_name: constr(strict=True, min_length=1)
     # stratification should be non-empty, and currently restrict to max 3 cross-dimension
     strata: conlist(DimensionSpec, min_items=1, max_items=3)
 
-    def __post_init_post_parse__(self):
+    def __post_init_post_parse__(self) -> None:
         unique_names = {s.name for s in self.strata}
         if len(unique_names) != len(self.strata):
             raise ValueError("Duplicate stratification name")
 
         check_duplicate_fields([stratum for s in self.strata for stratum in s.columns])
 
 
 @dataclass(frozen=True)
 class StratifyResponse:
-    test_suite_id: int
+    test_suite_id: int  # newly created version ID
     test_suite_name: str
     test_suite_description: str
     base_test_case: TestCaseInfo
     stratified_test_cases: List[TestCaseInfo]
 
 
-def check_duplicate_fields(strata: List[Dimension]):
+def check_duplicate_fields(strata: List[Dimension]) -> None:
     field_set = set()
     for stratum in strata:
         field = (stratum.column, stratum.field)
         # prevent self-cross stratification, i.e. one field can only be used once
         if field in field_set:
             raise ValueError(f"{field} is already used for stratification.")
         field_set.add(field)
```

### Comparing `kolena_client-0.68.0/kolena/_api/v1/detection.py` & `kolena_client-0.69.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_api/v1/fr.py` & `kolena_client-0.69.0/kolena/_api/v1/fr.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 class TestRun:
     class Path(str, Enum):
         CREATE_OR_RETRIEVE = "/fr/test-run/create-or-retrieve"
         INIT_LOAD_REMAINING_IMAGES = "/fr/test-run/load-remaining-images/init"
         COMPLETE_UPLOAD_IMAGE_RESULTS = "/fr/test-run/upload-image-results/complete"
         INIT_LOAD_REMAINING_PAIRS = "/fr/test-run/load-remaining-pairs/init"
         COMPLETE_UPLOAD_PAIR_RESULTS = "/fr/test-run/upload-pair-results/complete"
+        MARK_CRASHED = "/fr/test-run/mark-crashed"
 
     @dataclass(frozen=True)
     class CreateOrRetrieveRequest:
         model_id: int
         test_suite_ids: List[int]
         reset: bool = False
```

### Comparing `kolena_client-0.68.0/kolena/_api/v1/generic.py` & `kolena_client-0.69.0/kolena/_api/v1/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         COMPLETE_EDIT = "/generic/test-case/edit"
 
 
 class TestSuite:
     class Path(str, Enum):
         CREATE = "/generic/test-suite/create"
         LOAD = "/generic/test-suite/load"
+        LOAD_ALL = "/generic/test-suite/load-all"
         EDIT = "/generic/test-suite/edit"
         DELETE = "/generic/test-suite/delete"
         INIT_LOAD_TEST_SAMPLES = "/generic/test-suite/load-test-samples"
 
     @dataclass(frozen=True)
     class LoadTestSamplesRequest(BatchedLoad.BaseInitDownloadRequest):
         test_suite_id: int
@@ -111,15 +112,15 @@
         test_run_id: int
         test_case_id: Optional[int]
         configuration: Optional["TestRun.EvaluatorConfiguration"]
 
     @dataclass(frozen=True)
     class UpdateMetricsStatusRequest:
         test_run_id: int
-        progress: Optional[float] = None
+        progress: float
         message: str = ""
 
     @dataclass(frozen=True)
     class UploadAggregateMetricsRequest(BatchedLoad.WithLoadUUID):
         test_run_id: int
         test_suite_id: int
```

### Comparing `kolena_client-0.68.0/kolena/_api/v1/repository.py` & `kolena_client-0.69.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_api/v1/samples.py` & `kolena_client-0.69.0/kolena/_api/v1/workflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,10 +10,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
 
 
-class SampleType(str, Enum):
-    LOCATOR = "LOCATOR"
-    LOCATOR_TEXT = "LOCATOR_TEXT"
+class WorkflowType(str, Enum):
+    FR = "FR"
+    CLASSIFICATION = "CLASSIFICATION"
+    DETECTION = "DETECTION"
+    UNKNOWN = "UNKNOWN"
```

### Comparing `kolena_client-0.68.0/kolena/_api/v1/token.py` & `kolena_client-0.69.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_api/v1/workflow.py` & `kolena_client-0.69.0/kolena/detection/_internal/ground_truth.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,12 +10,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
 
 
-class WorkflowType(str, Enum):
-    FR = "FR"
-    CLASSIFICATION = "CLASSIFICATION"
-    DETECTION = "DETECTION"
-    UNKNOWN = "UNKNOWN"
+class GroundTruthType(str, Enum):
+    CLASSIFICATION_LABEL = "CLASSIFICATION_LABEL"
+    BOUNDING_BOX = "BOUNDING_BOX"
+    SEGMENTATION_MASK = "SEGMENTATION_MASK"
```

### Comparing `kolena_client-0.68.0/kolena/_utils/__init__.py` & `kolena_client-0.69.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/_consts.py` & `kolena_client-0.69.0/kolena/_utils/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
 
 
-class _BatchSize(int, Enum):
-    UPLOAD_CHIPS = 5_000
+class BatchSize(int, Enum):
+    UPLOAD_CHIPS = 1_000
     UPLOAD_RECORDS = 10_000_000
     UPLOAD_RESULTS = 1_000_000
 
     LOAD_RECORDS = UPLOAD_RECORDS
     LOAD_SAMPLES = 1_000_000
```

### Comparing `kolena_client-0.68.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.69.0/kolena/_utils/asset_path_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,13 +26,14 @@
 
     def absolute_locator(self, test_run_id: int, load_uuid: str, image_id: int, key: str) -> str:
         return self._absolute_locator(self.relative_locator(self.path_stub(test_run_id, load_uuid, image_id, key)))
 
     def relative_locator(self, path_stub: str) -> str:
         return f"{self.prefix}/{path_stub}"
 
-    def path_stub(self, test_run_id: int, load_uuid: str, image_id: int, key: str) -> str:
+    @staticmethod
+    def path_stub(test_run_id: int, load_uuid: str, image_id: int, key: str) -> str:
         return f"{test_run_id}/{image_id}/{key}-{load_uuid}.png"
 
     def _absolute_locator(self, relative_locator: str) -> str:
         relative_locator_stripped = relative_locator.strip("/")
         return f"s3://{self.bucket}/{relative_locator_stripped}"
```

### Comparing `kolena_client-0.68.0/kolena/_utils/batched_load.py` & `kolena_client-0.69.0/kolena/_utils/batched_load.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,47 +22,39 @@
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 import numpy as np
 import pandas as pd
 import requests
-from PIL import Image
-from requests_toolbelt import MultipartEncoder
 from retrying import retry
 
 from kolena._api.v1.batched_load import BatchedLoad as API
-from kolena._api.v1.fr import Asset as AssetAPI
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils.asset_path_mapper import AssetPathMapper
 from kolena._utils.datatypes import LoadableDataFrame
 from kolena._utils.serde import from_dict
-from kolena.fr._consts import _BatchSize
-from kolena.fr.datatypes import _ImageChipsDataFrame
 
 VALIDATION_COUNT_LIMIT = 100
-MAX_FILE_UPLOAD_SIZE = 1_000
 STAGE_STATUS__LOADED = "LOADED"
 
 
 def init_upload() -> API.InitiateUploadResponse:
-    init_res = krequests.put(endpoint_path=API.Path.INIT_UPLOAD)
+    init_res = krequests.put(endpoint_path=API.Path.INIT_UPLOAD.value)
     krequests.raise_for_status(init_res)
     init_response = from_dict(data_class=API.InitiateUploadResponse, data=init_res.json())
     return init_response
 
 
 def upload_data_frame(df: pd.DataFrame, batch_size: int, load_uuid: str) -> None:
     num_chunks = math.ceil(len(df) / batch_size)
     chunk_iter = np.array_split(df, num_chunks) if num_chunks > 0 else []
 
     # only display progress bar if there are multiple chunks to upload
     chunk_iter_logged = log.progress_bar(chunk_iter) if num_chunks > 1 else chunk_iter
-
     for df_chunk in chunk_iter_logged:
         upload_data_frame_chunk(df_chunk, load_uuid)
 
 
 @retry(stop_max_attempt_number=3)
 def upload_data_frame_chunk(df_chunk: pd.DataFrame, load_uuid: str) -> None:
     # We use a file-like object here so that requests chunks the file upload
@@ -78,59 +70,14 @@
         data=df_chunk_buffer,
         headers={"Content-Type": "application/octet-stream"},
         **krequests.get_connection_args(),
     )
     krequests.raise_for_status(upload_response)
 
 
-def upload_image_chips(
-    df: _ImageChipsDataFrame,
-    path_mapper: AssetPathMapper,
-    batch_size: int = _BatchSize.UPLOAD_CHIPS,
-) -> None:
-    def upload_batch(df_batch: _ImageChipsDataFrame) -> None:
-        df_batch = df_batch.reset_index(drop=True)  # reset indices so we match the signed_url indices
-
-        def as_buffer(image_raw: np.ndarray) -> io.BytesIO:
-            pil_image = Image.fromarray(image_raw).convert("RGB")
-            buf = io.BytesIO()
-            pil_image.save(buf, "png")
-            buf.seek(0)
-            return buf
-
-        data = MultipartEncoder(
-            fields=[
-                (
-                    "files",
-                    (
-                        path_mapper.path_stub(row["test_run_id"], row["uuid"], row["image_id"], row["key"]),
-                        as_buffer(row["image"]),
-                    ),
-                )
-                for _, row in df_batch.iterrows()
-            ],
-        )
-        upload_response = krequests.put(
-            endpoint_path=AssetAPI.Path.BULK_UPLOAD,
-            data=data,
-            headers={"Content-Type": data.content_type},
-        )
-        krequests.raise_for_status(upload_response)
-
-    batch_size = min(batch_size, MAX_FILE_UPLOAD_SIZE)
-    num_chunks = math.ceil(len(df) / batch_size)
-    chunk_iter = np.array_split(df, num_chunks) if len(df) > 0 else []
-    for df_chunk in chunk_iter:
-        upload_batch(df_chunk)
-
-
-def sanitize_uuid(load_uuid: str) -> str:
-    return load_uuid.replace("-", "_")
-
-
 DFType = TypeVar("DFType", bound=LoadableDataFrame)
 
 
 class _BatchedLoader(Generic[DFType]):
     @staticmethod
     def load_path(path: str, df_class: Type[DFType]) -> DFType:
         with tempfile.TemporaryFile() as tmp:
@@ -162,15 +109,15 @@
 
     @staticmethod
     def complete_load(uuid: Optional[str]) -> None:
         if uuid is None:
             return
         complete_request = API.CompleteDownloadRequest(uuid=uuid)
         complete_res = krequests.put(
-            endpoint_path=API.Path.COMPLETE_DOWNLOAD,
+            endpoint_path=API.Path.COMPLETE_DOWNLOAD.value,
             data=json.dumps(dataclasses.asdict(complete_request)),
         )
         krequests.raise_for_status(complete_res)
 
     @staticmethod
     def iter_data(
         init_request: API.BaseInitDownloadRequest,
```

### Comparing `kolena_client-0.68.0/kolena/_utils/cli.py` & `kolena_client-0.69.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.69.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.69.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/datatypes.py` & `kolena_client-0.69.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/endpoints.py` & `kolena_client-0.69.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/frozen.py` & `kolena_client-0.69.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/futures.py` & `kolena_client-0.69.0/kolena/_utils/serializable.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,33 +7,21 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import concurrent.futures
-from concurrent.futures import Future
-from dataclasses import dataclass
-from typing import Generic
-from typing import List
-from typing import TypeVar
+import json
+from abc import ABCMeta
+from abc import abstractmethod
+from typing import Any
+from typing import Dict
 
-T = TypeVar("T")
 
+class Serializable(metaclass=ABCMeta):
+    @abstractmethod
+    def _to_dict(self) -> Dict[str, Any]:
+        ...
 
-class CombinedFutureError(RuntimeError):
-    ...
-
-
-@dataclass(frozen=True)
-class CombinedFuture(Generic[T]):
-    futures: List[Future]
-
-    def wait(self) -> List[T]:
-        results = []
-        for future in concurrent.futures.as_completed(self.futures):
-            try:
-                results.append(future.result(timeout=1))
-            except Exception as e:
-                raise CombinedFutureError(f"future failed with error: {type(e).__name__}({e})")
-        return results
+    def __hash__(self) -> int:
+        return hash(json.dumps(self._to_dict()))
```

### Comparing `kolena_client-0.68.0/kolena/_utils/geometry.py` & `kolena_client-0.69.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/inference_validators.py` & `kolena_client-0.69.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/instrumentation.py` & `kolena_client-0.69.0/kolena/_utils/instrumentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import dataclasses
 import datetime
 import functools
 import inspect
+import json
 import traceback as tb
 from abc import ABCMeta
 from enum import Enum
 from typing import Any
 from typing import Callable
 
 import kolena
 from kolena._api.v1.client_log import ClientLog as API
+from kolena._api.v1.core import TestRun as CoreAPI
 from kolena._utils import krequests
 from kolena._utils.state import _client_state
 
 
 class DatadogLogLevels(str, Enum):
     ERROR = "error"
 
@@ -48,23 +50,23 @@
 def upload_log(message: str, status: str) -> None:
     request = API.UploadLogRequest(
         client_version=kolena.__version__,
         timestamp=str(datetime.datetime.now()),
         message=message,
         status=status,
     )
-    krequests.post(endpoint_path=API.Path.UPLOAD, json=dataclasses.asdict(request))
+    krequests.post(endpoint_path=API.Path.UPLOAD.value, json=dataclasses.asdict(request))
 
 
 def log_telemetry(e: BaseException) -> None:
     try:
         stack = tb.format_stack()
         exc_format = tb.format_exception(None, e, e.__traceback__)
         combined = stack + exc_format
-        upload_log("".join(combined), DatadogLogLevels.ERROR)
+        upload_log("".join(combined), DatadogLogLevels.ERROR.value)
     except BaseException:
         """
         Attempting to upload the telemetry is best-effort. We don't want to have exceptions in that
         process be thrown to the customer--instead they should get their original stacktrace.
         """
         ...
 
@@ -75,7 +77,13 @@
     """
 
     def __init_subclass__(cls) -> None:
         for key, value in cls.__dict__.items():
             if key.startswith("_") and not key == "__init__" or not callable(value) or inspect.isclass(value):
                 continue
             setattr(cls, key, telemetry(value))
+
+
+def report_crash(id: int, endpoint_path: str):
+    request = CoreAPI.MarkCrashedRequest(test_run_id=id)
+    # note no krequests.raise_for_status -- already in crashed state
+    krequests.post(endpoint_path=endpoint_path, data=json.dumps(dataclasses.asdict(request)))
```

### Comparing `kolena_client-0.68.0/kolena/_utils/krequests.py` & `kolena_client-0.69.0/kolena/_utils/krequests.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 # limitations under the License.
 import uuid
 from typing import Any
 from typing import Dict
 
 import requests
 from requests import HTTPError
+from requests_toolbelt import user_agent
 from requests_toolbelt.adapters import socket_options
 from urllib3.util import Retry
 
-from kolena import __version__ as version
+from kolena import __name__ as client_name
+from kolena import __version__ as client_version
 from kolena._utils.endpoints import get_endpoint
 from kolena._utils.state import get_client_state
 from kolena._utils.state import kolena_initialized
 from kolena.errors import NameConflictError
 from kolena.errors import NotFoundError
 from kolena.errors import RemoteError
 from kolena.errors import UnauthenticatedError
@@ -60,15 +62,15 @@
         "timeout": (CONNECTION_CONNECT_TIMEOUT, CONNECTION_READ_TIMEOUT),
         "proxies": client_state.proxies,
     }
     default_headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {client_state.jwt_token}",
         "X-Request-ID": uuid.uuid4().hex,
-        "User-Agent": f"kolena-client/{version}",
+        "User-Agent": user_agent(client_name, client_version),
     }
     return {
         **default_kwargs,
         **kwargs,
         "headers": {**default_headers, **kwargs.get("headers", {})},
     }
```

### Comparing `kolena_client-0.68.0/kolena/_utils/log.py` & `kolena_client-0.69.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/repository.py` & `kolena_client-0.69.0/kolena/_utils/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 from kolena._api.v1.repository import CreateRepositoryRequest
 from kolena._api.v1.repository import Path
 from kolena._utils import krequests
 
 
 def create(repository: str) -> None:
     response = krequests.post(
-        endpoint_path=Path.CREATE,
+        endpoint_path=Path.CREATE.value,
         data=json.dumps(dataclasses.asdict(CreateRepositoryRequest(repository=repository))),
     )
     krequests.raise_for_status(response)
```

### Comparing `kolena_client-0.68.0/kolena/_utils/serde.py` & `kolena_client-0.69.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/serializable.py` & `kolena_client-0.69.0/kolena/detection/_internal/inference.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,21 +7,32 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
 from abc import ABCMeta
 from abc import abstractmethod
-from typing import Any
-from typing import Dict
+from enum import Enum
 
+from kolena._utils.frozen import Frozen
+from kolena._utils.serializable import Serializable
+
+
+class InferenceType(str, Enum):
+    CLASSIFICATION_LABEL = "CLASSIFICATION_LABEL"
+    BOUNDING_BOX = "BOUNDING_BOX"
+    SEGMENTATION_MASK = "SEGMENTATION_MASK"
+
+
+class Inference(Serializable, Frozen, metaclass=ABCMeta):
+    """
+    Base class for an inference associated with an image.
+
+    See concrete implementations :class:`kolena.detection.inference.ClassificationLabel`,
+    :class:`kolena.detection.inference.BoundingBox`, :class:`kolena.detection.inference.SegmentationMask`, for details.
+    """
 
-class Serializable(metaclass=ABCMeta):
     @abstractmethod
-    def _to_dict(self) -> Dict[str, Any]:
+    def __init__(self) -> None:
         ...
-
-    def __hash__(self) -> int:
-        return hash(json.dumps(self._to_dict()))
```

### Comparing `kolena_client-0.68.0/kolena/_utils/state.py` & `kolena_client-0.69.0/kolena/_utils/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import contextlib
 import contextvars
+import dataclasses
 import functools
 import os
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import Optional
 
 import requests
 
+import kolena
 import kolena._api.v1.token as API
+from kolena._utils import krequests
 from kolena._utils.serde import from_dict
 from kolena.errors import InvalidClientStateError
+from kolena.errors import InvalidTokenError
+from kolena.errors import UnauthenticatedError
 from kolena.errors import UninitializedError
 
 API_VERSION = "v1"
 API_BASE_URL = "https://api.kolena.io"
 API_BASE_URL_ENV_VAR = "KOLENA_CLIENT_BASE_URL"
 CLIENT_STATE = contextvars.ContextVar("client_state")
 
@@ -93,16 +98,19 @@
         self.api_token = None
         self.jwt_token = None
         self.tenant = None
         self.verbose = False
         self.telemetry = False
 
 
-_client_base_url = os.environ.get(API_BASE_URL_ENV_VAR, API_BASE_URL)
-_client_state = _ClientState(base_url=_client_base_url)
+def _get_api_base_url() -> str:
+    return os.environ.get(API_BASE_URL_ENV_VAR, API_BASE_URL)
+
+
+_client_state = _ClientState(base_url=_get_api_base_url())
 
 
 def get_client_state() -> _ClientState:
     return CLIENT_STATE.get(_client_state)
 
 
 def is_client_initialized() -> bool:
@@ -125,22 +133,39 @@
     return wrapper
 
 
 def get_endpoint_with_baseurl(base_url: str, endpoint_path: str) -> str:
     return f"{base_url}/{API_VERSION}/{endpoint_path.lstrip('/')}"
 
 
-@contextlib.contextmanager
-def kolena_session(base_url: str, api_token: str) -> Iterator[_ClientState]:
+def get_token(
+    api_token: str,
+    base_url: Optional[str] = None,
+    proxies: Optional[Dict[str, str]] = None,
+) -> API.ValidateResponse:
+    base_url = base_url or get_client_state().base_url
+    request = API.ValidateRequest(api_token=api_token, version=kolena.__version__)
     r = requests.put(
         get_endpoint_with_baseurl(base_url, "token/login"),
-        json={"api_token": api_token, "version": API_VERSION},
+        json=dataclasses.asdict(request),
+        proxies=proxies,
     )
-    r.raise_for_status()
+    try:
+        krequests.raise_for_status(r)
+    except UnauthenticatedError as e:
+        raise InvalidTokenError(e)
+
     init_response = from_dict(data_class=API.ValidateResponse, data=r.json())
+    return init_response
+
+
+@contextlib.contextmanager
+def kolena_session(api_token: str, base_url: Optional[str] = None) -> Iterator[_ClientState]:
+    base_url = base_url or _get_api_base_url()
+    init_response = get_token(api_token, base_url)
     client_state = _ClientState(
         base_url=base_url,
         api_token=api_token,
         jwt_token=init_response.access_token,
         tenant=init_response.tenant,
     )
     token = CLIENT_STATE.set(client_state)
```

### Comparing `kolena_client-0.68.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.69.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/_utils/validators.py` & `kolena_client-0.69.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/__init__.py` & `kolena_client-0.69.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/metadata.py` & `kolena_client-0.69.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/model.py` & `kolena_client-0.69.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.69.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.69.0/kolena/classification/multiclass/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
+from typing import Optional
 from typing import Tuple
 
 import numpy as np
 
 from kolena._utils import log
 from kolena.classification.multiclass import InferenceLabel
 
@@ -50,32 +51,38 @@
         tps = tps[optimal_indices]
 
     fps = np.r_[0, fps]
     tps = np.r_[0, tps]
 
     # Map cumulative sums to tpr and fpr
     if fps[-1] <= 0:
-        log.warn("No negative samples in y_true, false positive value should be meaningless")
+        # No negative samples in y_true, false positive value should be meaningless
         fpr = []
     else:
         fpr = fps / fps[-1]
         fpr = fpr.tolist()
     if tps[-1] <= 0:
-        log.warn("No positive samples in y_true, true positive value should be meaningless")
+        # No positive samples in y_true, true positive value should be meaningless
         tpr = []
     else:
         tpr = tps / tps[-1]
         tpr = tpr.tolist()
 
     return fpr, tpr
 
 
-def get_histogram_range(scores: List[float]) -> Tuple[float, float, int]:  # min, max, num_buckets
-    bin_range_options = np.linspace(0, 1, 51)
+def get_histogram_range(scores: List[float]) -> Optional[Tuple[float, float, int]]:  # min, max, num_buckets
     min_score, max_score = min(scores), max(scores)
+    if min_score < 0.0 or max_score > 1.0:
+        log.warn(
+            f"scores out of range for confidence histograms: expecting [0, 1], got [{min_score:.3f}, {max_score:.3f}]",
+        )
+        return None
+
+    bin_range_options = np.linspace(0, 1, 51)
     min_range, max_range, bucket_fenceposts = 0, 1, 0
     for option in bin_range_options:
         if min_score >= option > min_range:
             min_range = option
         if max_score <= option < max_range:
             max_range = option
     for option in bin_range_options:
```

### Comparing `kolena_client-0.68.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.69.0/kolena/classification/multiclass/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,27 +82,31 @@
     )
 
 
 def _as_class_metric_plot(
     metric_name: str,
     metrics_by_label: Dict[str, AggregatedMetrics],
     labels: List[str],
-) -> BarPlot:
+) -> Optional[BarPlot]:
     if metric_name == "Recall":
         title = f"{metric_name} (TPR) vs. Class"
     else:
         title = f"{metric_name} vs. Class"
 
-    return BarPlot(
-        title=title,
-        x_label="Class",
-        y_label=metric_name,
-        labels=labels,
-        values=[getattr(metrics_by_label[label], metric_name) for label in labels],
-    )
+    values = [getattr(metrics_by_label[label], metric_name) for label in labels]
+    valid_pairs = [(label, value) for label, value in zip(labels, values) if value != 0.0]
+    if len(valid_pairs) > 0:
+        return BarPlot(
+            title=title,
+            x_label="Class",
+            y_label=metric_name,
+            labels=[label for label, _ in valid_pairs],
+            values=[value for _, value in valid_pairs],
+        )
+    return None
 
 
 def _as_confidence_histogram(
     title: str,
     confidence_scores: List[float],
     confidence_range: Tuple[float, float, int] = (0, 1, 25),
 ) -> Histogram:
@@ -117,52 +121,63 @@
         x_label="Confidence",
         y_label="Count",
         buckets=list(bins),
         frequency=list(hist),
     )
 
 
-def _compute_test_case_plots(
+def _compute_confidence_histograms(
     test_case_name: str,
-    labels: List[str],
-    ground_truths: List[GroundTruth],
-    inferences: List[Inference],
     metrics: List[TestSampleMetrics],
-    metrics_by_label: Dict[str, AggregatedMetrics],
-    confidence_range: Tuple[float, float, int],
-) -> List[Plot]:
+    confidence_range: Optional[Tuple[float, float, int]],
+) -> List[Histogram]:
+    if confidence_range is None:
+        log.warn(
+            f"skipping confidence histograms for {test_case_name}: unsupported confidence range",
+        )
+        return []
+
     confidence_all = [mts.classification.confidence for mts in metrics if mts.classification is not None]
     confidence_correct = [
         mts.classification.confidence for mts in metrics if mts.classification is not None and mts.is_correct
     ]
     confidence_incorrect = [
         mts.classification.confidence for mts in metrics if mts.classification is not None and not mts.is_correct
     ]
 
+    plots = [
+        _as_confidence_histogram("Confidence Distribution (All)", confidence_all, confidence_range),
+        _as_confidence_histogram("Confidence Distribution (Correct)", confidence_correct, confidence_range),
+        _as_confidence_histogram("Confidence Distribution (Incorrect)", confidence_incorrect, confidence_range),
+    ]
+    return plots
+
+
+def _compute_test_case_plots(
+    test_case_name: str,
+    labels: List[str],
+    ground_truths: List[GroundTruth],
+    inferences: List[Inference],
+    metrics: List[TestSampleMetrics],
+    metrics_by_label: Dict[str, AggregatedMetrics],
+    confidence_range: Optional[Tuple[float, float, int]],
+) -> List[Plot]:
     gt_labels = {gt.classification.label for gt in ground_truths}
-    class_metric_plots = [
+    plots = [
         _as_class_metric_plot(field.name, metrics_by_label, labels)
         for field in dataclasses.fields(AggregatedMetrics)
         if len(gt_labels) > 2
         or field.name not in ["Precision", "Recall"]  # Omit single-class TC from precision and recall plots
     ]
 
-    plots = [
-        *class_metric_plots,
-        _as_confidence_histogram("Confidence Distribution (All)", confidence_all, confidence_range),
-        _as_confidence_histogram("Confidence Distribution (Correct)", confidence_correct, confidence_range),
-        _as_confidence_histogram("Confidence Distribution (Incorrect)", confidence_incorrect, confidence_range),
-    ]
+    plots.extend(_compute_confidence_histograms(test_case_name, metrics, confidence_range))
+    plots.append(_compute_test_case_ovr_roc_curve(test_case_name, labels, ground_truths, inferences))
+    plots.append(_compute_test_case_confusion_matrix(test_case_name, ground_truths, metrics))
+    plots = list(filter(lambda plot: plot is not None, plots))
 
-    roc_curve_plot = _compute_test_case_ovr_roc_curve(labels, ground_truths, inferences)
-    if roc_curve_plot:
-        plots.append(roc_curve_plot)
-    confusion_matrix = _compute_test_case_confusion_matrix(test_case_name, ground_truths, metrics)
-    if confusion_matrix:
-        plots.append(confusion_matrix)
     return plots
 
 
 def _compute_test_case_confusion_matrix(
     test_case_name: str,
     ground_truths: List[GroundTruth],
     metrics: List[TestSampleMetrics],
@@ -180,41 +195,42 @@
         confusion_matrix[actual_label][predicted_label] += 1
 
     if len(gt_labels) < 2:
         log.warn(f"skipping confusion matrix for {test_case_name}: single label test case")
         return None
 
     labels: Set[str] = {*gt_labels, *pred_labels}
-    if len(labels) > 10:
-        log.warn(f"skipping confusion matrix for {test_case_name}: too many labels")
-        return None
-
     contains_none = none_label in labels
     sortable_labels = [label for label in labels if label != none_label]
     ordered_labels = sorted(sortable_labels) if not contains_none else [*sorted(sortable_labels), none_label]
     matrix = []
     for actual_label in ordered_labels:
         matrix.append([confusion_matrix[actual_label][predicted_label] for predicted_label in ordered_labels])
     return ConfusionMatrix(title="Label Confusion Matrix", labels=ordered_labels, matrix=matrix)
 
 
 def _compute_test_case_ovr_roc_curve(
+    test_case_name: str,
     labels: List[str],
     ground_truths: List[GroundTruth],
     inferences: List[Inference],
 ) -> Optional[Plot]:
     curves = []
     for label in labels:
         y_true = [1 if gt.classification.label == label else 0 for gt in ground_truths]
         y_score = [get_label_confidence(label, inf.inferences) for inf in inferences]
         fpr_values, tpr_values = roc_curve(y_true, y_score)
         if len(fpr_values) > 0 and len(tpr_values) > 0:
             curves.append(Curve(x=fpr_values, y=tpr_values, label=label))
 
     if len(curves) > 0:
+        if len(curves) > 10:
+            log.warn(f"skipping one-vs-rest ROC curve for {test_case_name}: too many labels")
+            return None
+
         return CurvePlot(
             title="Receiver Operating Characteristic (One-vs-Rest)",
             x_label="False Positive Rate (FPR)",
             y_label="True Positive Rate (TPR)",
             curves=curves,
         )
     return None
```

### Comparing `kolena_client-0.68.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.69.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.69.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/test_case.py` & `kolena_client-0.69.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/test_config.py` & `kolena_client-0.69.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/test_image.py` & `kolena_client-0.69.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/test_run.py` & `kolena_client-0.69.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/classification/test_suite.py` & `kolena_client-0.69.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/__init__.py` & `kolena_client-0.69.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/_datatypes.py` & `kolena_client-0.69.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.69.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.69.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.69.0/kolena/workflow/metrics/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from enum import Enum
+from ._geometry import InferenceMatches
+from ._geometry import iou
+from ._geometry import match_inferences
+from ._geometry import match_inferences_multiclass
 
-
-class GroundTruthType(str, Enum):
-    CLASSIFICATION_LABEL = "CLASSIFICATION_LABEL"
-    BOUNDING_BOX = "BOUNDING_BOX"
-    SEGMENTATION_MASK = "SEGMENTATION_MASK"
+__all__ = [
+    "InferenceMatches",
+    "iou",
+    "match_inferences",
+    "match_inferences_multiclass",
+]
```

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.69.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/model.py` & `kolena_client-0.69.0/kolena/detection/_internal/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 from pydantic import validate_arguments
 
 from kolena._api.v1.core import Model as CoreAPI
 from kolena._api.v1.detection import Model as API
 from kolena._api.v1.workflow import WorkflowType
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import DFType
+from kolena._utils.consts import BatchSize
 from kolena._utils.endpoints import get_model_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseTestCase
 from kolena.detection._internal import BaseTestImage
@@ -89,25 +89,25 @@
         self._workflow = WorkflowType(loaded.workflow)
         self._freeze()
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _create(cls, workflow: WorkflowType, name: str, metadata: Dict[str, Any]) -> CoreAPI.EntityData:
         request = CoreAPI.CreateRequest(name=name, metadata=metadata, workflow=workflow.value)
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         log.info(f"created model '{name}' ({get_model_url(obj.id)})")
         return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str) -> CoreAPI.EntityData:
         request = CoreAPI.LoadByNameRequest(name=name)
-        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         log.info(f"loaded model '{name}' ({get_model_url(obj.id)})")
         return obj
 
     @validate_arguments(config=ValidatorConfig)
     def load_inferences(
@@ -130,27 +130,27 @@
         for df_batch in self._iter_inference_batch_for_reference(test_object):
             yield from (self._inferences_from_record(record) for record in df_batch.itertuples())
 
     @validate_arguments(config=ValidatorConfig)
     def _iter_inference_batch_for_reference(
         self,
         test_object: Union[_TestCaseClass, _TestSuiteClass],
-        batch_size: int = _BatchSize.LOAD_SAMPLES,
+        batch_size: int = BatchSize.LOAD_SAMPLES.value,
     ) -> Iterator[_LoadInferencesDataFrameClass]:
         if batch_size <= 0:
             raise InputValidationError(f"invalid batch_size '{batch_size}': expected positive integer")
         test_object_display_type = "test case" if isinstance(test_object, self._TestCaseClass) else "test suite"
         test_object_display_name = f"{test_object_display_type} '{test_object.name}'"
         log.info(f"loading inferences from model '{self.name}' on {test_object_display_name}")
         test_id_key = "test_case_id" if isinstance(test_object, self._TestCaseClass) else "test_suite_id"
         params = dict(model_id=self._id, batch_size=batch_size, **{test_id_key: test_object._id})
         init_request = API.InitLoadInferencesRequest(**params)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_INFERENCES,
+            endpoint_path=API.Path.INIT_LOAD_INFERENCES.value,
             df_class=self._LoadInferencesDataFrameClass,
         )
         log.success(f"loaded inferences from model '{self.name}' on {test_object_display_name}")
 
     @validate_arguments(config=ValidatorConfig)
     def load_inferences_by_test_case(
         self,
@@ -165,24 +165,24 @@
         df_by_testcase = df.groupby("test_case_id")["test_sample"].agg(list).to_dict()
         return df_by_testcase
 
     @validate_arguments(config=ValidatorConfig)
     def _iter_inference_batch_for_test_suite(
         self,
         test_suite: _TestSuiteClass,
-        batch_size: int = _BatchSize.LOAD_SAMPLES,
+        batch_size: int = BatchSize.LOAD_SAMPLES.value,
     ) -> Iterator[_LoadInferencesDataFrameClass]:
         if batch_size <= 0:
             raise InputValidationError(f"invalid batch_size '{batch_size}': expected positive integer")
         log.info(f"loading inferences from model '{self.name}' on test suite '{test_suite.name}'")
         params = dict(model_id=self._id, batch_size=batch_size, test_suite_id=test_suite._id)
         init_request = API.InitLoadInferencesByTestCaseRequest(**params)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_INFERENCES_BY_TEST_CASE,
+            endpoint_path=API.Path.INIT_LOAD_INFERENCES_BY_TEST_CASE.value,
             df_class=self._LoadInferencesDataFrameClass,
         )
         log.success(f"loaded inferences from model '{self.name}' on test suite '{test_suite.name}'")
 
     @abstractmethod
     def _inferences_from_record(self, record: Any) -> Tuple[_TestImageClass, Optional[List[_InferenceClass]]]:
         ...
```

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.69.0/kolena/detection/_internal/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 from pydantic import validate_arguments
 
 from kolena._api.v1.core import TestCase as CoreAPI
 from kolena._api.v1.detection import TestCase as API
 from kolena._api.v1.workflow import WorkflowType
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import DFType
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
+from kolena._utils.consts import BatchSize
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseTestImage
 from kolena.errors import NotFoundError
@@ -123,42 +123,42 @@
         workflow: WorkflowType,
         name: str,
         description: Optional[str] = None,
         images: Optional[List[_TestImageClass]] = None,
     ) -> "BaseTestCase":
         """Create a new test case with the provided name."""
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=workflow.value)
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if images is not None:
             obj._hydrate(images)
         log.info(f"created test case '{name}'")
         return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> CoreAPI.EntityData:
         """Load an existing test case with the provided name."""
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
-        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         log.info(f"loaded test case '{name}'")
         return from_dict(data_class=CoreAPI.EntityData, data=res.json())
 
     @validate_arguments(config=ValidatorConfig)
     def _hydrate(self, images: List[_TestImageClass], description: Optional[str] = None) -> None:
         if len(images) == 0:
             log.warn("no images provided, unable to populate test case")
             return
         with self.edit(reset=True) as editor:
             if description is not None:
                 editor.description(description)
-            for image in log.progress_bar(images):
+            for image in images:
                 editor.add(image)
 
     @classmethod
     def _create_from_data(cls, data: CoreAPI.EntityData) -> "BaseTestCase":
         assert_workflows_match(cls._workflow, data.workflow)
         return cls._from(data)
 
@@ -167,18 +167,18 @@
         """Load all test images with their associated ground truths in this test case."""
         return list(self.iter_images())
 
     @validate_arguments(config=ValidatorConfig)
     def iter_images(self) -> Iterator[_TestImageClass]:
         """Iterate through all images with their associated ground truths in this test case."""
         log.info(f"loading test images for test case '{self.name}'")
-        init_request = CoreAPI.InitLoadContentsRequest(batch_size=_BatchSize.LOAD_SAMPLES, test_case_id=self._id)
+        init_request = CoreAPI.InitLoadContentsRequest(batch_size=BatchSize.LOAD_SAMPLES.value, test_case_id=self._id)
         for df in _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_IMAGES,
+            endpoint_path=API.Path.INIT_LOAD_IMAGES.value,
             df_class=self._TestImageDataFrameClass,
         ):
             for record in df.itertuples():
                 yield self._TestImageClass._from_record(record)
         log.success(f"loaded test images for test case '{self.name}'")
 
     @classmethod
@@ -306,24 +306,24 @@
         if not editor._edited:
             return
 
         log.info(f"editing test case '{self.name}'")
         init_response = init_upload()
         df = self._to_data_frame(list(editor._images.values()))
         df_serialized = df.as_serializable()
-        upload_data_frame(df=df_serialized, batch_size=_BatchSize.UPLOAD_RECORDS, load_uuid=init_response.uuid)
+        upload_data_frame(df=df_serialized, batch_size=BatchSize.UPLOAD_RECORDS.value, load_uuid=init_response.uuid)
 
         request = CoreAPI.CompleteEditRequest(
             test_case_id=self._id,
             current_version=self.version,
             description=editor._description,
             reset=editor._reset,
             uuid=init_response.uuid,
         )
         complete_res = krequests.put(
-            endpoint_path=API.Path.COMPLETE_EDIT,
+            endpoint_path=API.Path.COMPLETE_EDIT.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=CoreAPI.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
         log.success(f"edited test case '{self.name}'")
```

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.69.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.69.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.69.0/kolena/detection/_internal/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import pandera as pa
 from pydantic import validate_arguments
 
-from kolena._api.v1.core import TestRun as CoreAPI
 from kolena._api.v1.detection import CustomMetrics
 from kolena._api.v1.detection import Metrics
 from kolena._api.v1.detection import TestRun as API
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import DFType
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame_chunk
+from kolena._utils.consts import BatchSize
 from kolena._utils.datatypes import LoadableDataFrame
 from kolena._utils.frozen import Frozen
+from kolena._utils.instrumentation import report_crash
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseModel
 from kolena.detection._internal import BaseTestImage
 from kolena.detection._internal import BaseTestSuite
 from kolena.detection._internal import Inference
@@ -93,15 +93,18 @@
             log.info("reset flag is disabled. update existing inferences by enabling the reset flag")
 
         request = API.CreateOrRetrieveRequest(
             model_id=model._id,
             test_suite_ids=[test_suite._id],
             config=config,
         )
-        res = krequests.post(endpoint_path=API.Path.CREATE_OR_RETRIEVE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(
+            endpoint_path=API.Path.CREATE_OR_RETRIEVE.value,
+            data=json.dumps(dataclasses.asdict(request)),
+        )
         krequests.raise_for_status(res)
         response = from_dict(data_class=API.CreateOrRetrieveResponse, data=res.json())
         self._id = response.test_run_id
         self._model = model
         self._test_suite = test_suite
         self._locator_to_image_id: Dict[str, int] = {}
         self._inferences: Dict[int, List[Optional[Inference]]] = OrderedDict()
@@ -124,16 +127,15 @@
         exc_tb: Optional[TracebackType],
     ) -> None:
         self._upload_chunk()
         self._finalize_upload()
         self._submit_custom_metrics()
         self._active = False
         if exc_type is not None:
-            request = CoreAPI.MarkCrashedRequest(test_run_id=self._id)
-            krequests.post(endpoint_path=API.Path.MARK_CRASHED, data=json.dumps(dataclasses.asdict(request)))
+            report_crash(self._id, API.Path.MARK_CRASHED.value)
 
     @validate_arguments(config=ValidatorConfig)
     def add_inferences(self, image: _TestImageClass, inferences: Optional[List[_InferenceClass]]) -> None:
         """
         Adds inferences for a test image to the test run results.
 
         :param image: the image that inferences are evaluated on
@@ -157,15 +159,15 @@
                 self._n_inferences += 1
             else:
                 context_image_inferences.extend(inferences)
                 self._n_inferences += len(inferences)
 
             self._inferences[image_id] = context_image_inferences
 
-        if self._n_inferences >= _BatchSize.UPLOAD_RESULTS:
+        if self._n_inferences >= BatchSize.UPLOAD_RESULTS.value:
             log.info(f"uploading batch of '{self._n_inferences}' inference results")
             self._upload_chunk()
             log.success(f"uploaded batch of '{self._n_inferences}' inference results")
 
     @validate_arguments(config=ValidatorConfig)
     def iter_images(self) -> Iterator[_TestImageClass]:
         """
@@ -173,15 +175,15 @@
         """
         self._assert_active()
         for df_image_batch in self._iter_image_batch():
             for record in df_image_batch.itertuples():
                 yield self._image_from_load_image_record(record)
 
     @validate_arguments(config=ValidatorConfig)
-    def load_images(self, batch_size: int = _BatchSize.LOAD_SAMPLES) -> List[_TestImageClass]:
+    def load_images(self, batch_size: int = BatchSize.LOAD_SAMPLES.value) -> List[_TestImageClass]:
         """
         Returns a list of images that still need inferences evaluated, bounded in count
         by batch_size. Note that image ground truths will be excluded from the returned
         batch of images.
 
         :param batch_size: the maximum number of images to retrieve
         """
@@ -192,25 +194,28 @@
         except StopIteration:
             # no more images
             return []
         log.success("loaded batch of images for test run")
         return [self._image_from_load_image_record(record) for record in df_image_batch.itertuples()]
 
     @validate_arguments(config=ValidatorConfig)
-    def _iter_image_batch(self, batch_size: int = _BatchSize.LOAD_SAMPLES) -> Iterator[_LoadTestImagesDataFrameClass]:
+    def _iter_image_batch(
+        self,
+        batch_size: int = BatchSize.LOAD_SAMPLES.value,
+    ) -> Iterator[_LoadTestImagesDataFrameClass]:
         if batch_size <= 0:
             raise InputValidationError(f"invalid batch_size '{batch_size}': expected positive integer")
         init_request = API.InitLoadRemainingImagesRequest(
             test_run_id=self._id,
             batch_size=batch_size,
             load_all=self._reset,
         )
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_REMAINING_IMAGES,
+            endpoint_path=API.Path.INIT_LOAD_REMAINING_IMAGES.value,
             df_class=self._LoadTestImagesDataFrameClass,
         )
 
     @validate_arguments(config=ValidatorConfig)
     def _upload_chunk(self) -> None:
         if self._n_inferences == 0:
             # Bail if this happens to being run by fencepost immediately after being run by add_inference
@@ -236,15 +241,15 @@
         if self._upload_uuid is None:
             # nothing was uploaded
             return
 
         log.info("finalizing inference upload for test run")
         request = API.UploadImageResultsRequest(uuid=self._upload_uuid, test_run_id=self._id, reset=self._reset)
         finalize_res = krequests.put(
-            endpoint_path=API.Path.UPLOAD_IMAGE_RESULTS,
+            endpoint_path=API.Path.UPLOAD_IMAGE_RESULTS.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(finalize_res)
         log.success("finalized inference upload for test run")
 
     def _assert_active(self) -> None:
         if not self._active:
@@ -286,10 +291,13 @@
     def _submit_custom_metrics(self) -> None:
         if self._custom_metrics_callback is None:
             return
 
         log.info("submitting custom metrics for test run")
         custom_metrics = self._compute_custom_metrics()
         request = API.UpdateCustomMetricsRequest(model_id=self._model._id, metrics=custom_metrics)
-        res = krequests.put(endpoint_path=API.Path.UPLOAD_CUSTOM_METRICS, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(
+            endpoint_path=API.Path.UPLOAD_CUSTOM_METRICS.value,
+            data=json.dumps(dataclasses.asdict(request)),
+        )
         krequests.raise_for_status(res)
         log.success("submitted custom metrics for test run")
```

### Comparing `kolena_client-0.68.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.69.0/kolena/detection/_internal/test_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,41 +108,41 @@
         workflow: WorkflowType,
         name: str,
         description: Optional[str] = None,
         test_cases: Optional[List[BaseTestCase]] = None,
     ) -> "BaseTestSuite":
         """Create a new test suite with the provided name."""
         request = CoreAPI.TestSuite.CreateRequest(name=name, description=description or "", workflow=workflow.value)
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_cases is not None:
             obj._hydrate(test_cases)
         log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> CoreAPI.TestSuite.EntityData:
         """Retrieve the existing test suite with the provided name."""
         request = CoreAPI.TestSuite.LoadByNameRequest(name=name, version=version)
         data = json.dumps(dataclasses.asdict(request))
-        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=data)
+        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=data)
         krequests.raise_for_status(res)
         return from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
 
     @validate_arguments(config=ValidatorConfig)
     def _hydrate(self, test_cases: List[BaseTestCase], description: Optional[str] = None) -> None:
         """Convenience method to hydrate an empty test suite with the provided test cases"""
         with self.edit(reset=True) as editor:
             if description is not None:
                 editor.description(description)
-            if len(test_cases):
-                for test_case in log.progress_bar(test_cases):
+            if len(test_cases) > 0:
+                for test_case in test_cases:
                     editor.add(test_case)
 
     @classmethod
     def _create_from_data(cls, data: CoreAPI.TestSuite.EntityData) -> "BaseTestSuite":
         assert_workflows_match(cls._workflow, data.workflow)
         obj = cls.__new__(cls)
         obj._id = data.id
@@ -285,24 +285,24 @@
 
         yield editor
 
         if not editor._edited():
             log.info("no op: nothing edited")
             return
 
-        log.info(f"editing test suite '{self.name}'")
+        log.info(f"edited test suite '{self.name}'")
         request = CoreAPI.TestSuite.EditRequest(
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             test_case_ids=list(editor._test_cases.values()),
         )
         data = json.dumps(dataclasses.asdict(request))
-        res = krequests.post(endpoint_path=API.Path.EDIT, data=data)
+        res = krequests.post(endpoint_path=API.Path.EDIT.value, data=data)
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
         log.success(f"edited test suite '{self.name}' ({get_test_suite_url(test_suite_data.id)})")
         with self._unfrozen():
             self.version = test_suite_data.version
             self.description = test_suite_data.description
             self.test_cases = [self._test_case_from(tc) for tc in test_suite_data.test_cases]
```

### Comparing `kolena_client-0.68.0/kolena/detection/ground_truth.py` & `kolena_client-0.69.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/inference.py` & `kolena_client-0.69.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/metadata.py` & `kolena_client-0.69.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/model.py` & `kolena_client-0.69.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/test_case.py` & `kolena_client-0.69.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/test_config.py` & `kolena_client-0.69.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/test_image.py` & `kolena_client-0.69.0/kolena/detection/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from typing import Optional
 from typing import Tuple
 
 from deprecation import deprecated
 from pydantic import validate_arguments
 
 from kolena._api.v1.detection import TestImage as API
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
+from kolena._utils.consts import BatchSize
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._datatypes import TestImageDataFrame
 from kolena.detection._internal import BaseTestImage
 from kolena.detection._internal.metadata import _from_dict
 from kolena.detection._internal.metadata import _to_dict
 from kolena.detection._internal.metadata import MetadataElement
 from kolena.detection.ground_truth import GroundTruth
@@ -99,15 +99,15 @@
     """
     Return iterator over :class:`kolena.detection.TestImage` samples registered in the Kolena platform. Images are
     lazily loaded in chunks to facilitate working with large datasets that are cumbersome to hold in memory.
 
     :param dataset: optionally specify the single dataset to be retrieved. By default, images from all
         datasets are returned
     """
-    init_request = API.InitLoadImagesRequest(dataset=dataset, batch_size=_BatchSize.LOAD_RECORDS)
+    init_request = API.InitLoadImagesRequest(dataset=dataset, batch_size=BatchSize.LOAD_RECORDS.value)
     for df in _BatchedLoader.iter_data(
         init_request=init_request,
-        endpoint_path=API.Path.INIT_LOAD_IMAGES,
+        endpoint_path=API.Path.INIT_LOAD_IMAGES.value,
         df_class=TestImageDataFrame,
     ):
         for record in df.itertuples():
             yield TestImage._from_record(record)
```

### Comparing `kolena_client-0.68.0/kolena/detection/test_run.py` & `kolena_client-0.69.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/detection/test_suite.py` & `kolena_client-0.69.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/errors.py` & `kolena_client-0.69.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/fr/__init__.py` & `kolena_client-0.69.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/fr/datatypes.py` & `kolena_client-0.69.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/fr/model.py` & `kolena_client-0.69.0/kolena/fr/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         :param name: unique name of the new model to create
         :param metadata: unstructured metadata to associate with the model
         :return: the created model
         :raises ValueError: if a model by the provided name already exists
         """
         request = API.CreateRequest(name=name, metadata=metadata)
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
         log.info(f"created model '{name}' ({get_model_url(obj.data.id)})")
         return obj
 
     @classmethod
     def load_by_name(cls, name: str) -> "Model":
@@ -70,15 +70,15 @@
         Retrieve the existing model with the provided name.
 
         :param name: name of the model to retrieve
         :return: the retrieved model
         :raises KeyError: if no model with the provided name exists
         """
         request = API.LoadByNameRequest(name=name)
-        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
         log.info(f"loaded model '{name}' ({get_model_url(obj.data.id)})")
         return obj
 
     def _get_load_pair_results_request(
         self,
@@ -143,15 +143,15 @@
         display_name = test_object.data.name if isinstance(test_object, (TestCase, TestSuite)) else test_object.name
         test_object_display_name = f"{display_type} '{display_name}'"
         log.info(f"loading pair results from model '{self.data.name}' on {test_object_display_name}")
         base_load_request = dataclasses.asdict(self._get_load_pair_results_request(test_object))
         init_request = API.InitLoadPairResultsRequest(batch_size=batch_size, **base_load_request)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_PAIR_RESULTS,
+            endpoint_path=API.Path.INIT_LOAD_PAIR_RESULTS.value,
             df_class=LoadedPairResultDataFrame,
         )
         log.success(f"loaded pair results from model '{self.data.name}' on {test_object_display_name}")
 
 
 class InferenceModel(Model):
     """
```

### Comparing `kolena_client-0.68.0/kolena/fr/test_case.py` & `kolena_client-0.69.0/kolena/fr/test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 
 from kolena._api.v1.fr import TestCase as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
+from kolena._utils.consts import BatchSize
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
-from kolena.fr._consts import _BatchSize
 from kolena.fr.datatypes import TEST_CASE_COLUMNS
 from kolena.fr.datatypes import TestCaseDataFrame
 from kolena.fr.datatypes import TestCaseDataFrameSchema
 from kolena.fr.datatypes import TestCaseRecord
 
 
 class TestCase(ABC, Frozen, WithTelemetry):
@@ -121,15 +121,15 @@
 
         :param name: the name of the new test case to create.
         :param description: optional free-form description of the test case to create.
         :param test_samples: optionally specify a set of test samples to populate the test case.
         :return: the newly created test case.
         """
         request = API.CreateRequest(name=name, description=description or "")
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_samples is not None:
             obj._hydrate(test_samples)
         log.info(f"created test case '{name}'")
         return obj
@@ -158,15 +158,15 @@
         :return: the loaded test case
         """
         return cls.load(name, version)
 
     @classmethod
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> "TestCase":
         request = API.LoadByNameRequest(name=name, version=version)
-        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         log.info(f"loaded test case '{name}'")
         return cls._create_from_data(data)
 
     def load_data(self) -> TestCaseDataFrame:
         """
@@ -205,15 +205,15 @@
             self._id = other._id
             self.name = other.name
             self.version = other.version
             self.description = other.description
             self.image_count = other.image_count
             self.pair_count_genuine = other.pair_count_genuine
             self.pair_count_imposter = other.pair_count_imposter
-            self.data = other.data
+            self.data = other._data
 
     class Editor:
         _samples: Dict[str, TestCaseRecord]
         _reset: bool
         _description: str
         _initial_description: str
         _initial_samples: Optional[Dict[str, TestCaseRecord]] = None
@@ -313,24 +313,24 @@
             return
 
         log.info(f"editing test case '{self.name}'")
         init_response = init_upload()
         df = pd.DataFrame(editor._samples.values(), columns=TEST_CASE_COLUMNS)
         df_validated = validate_df_schema(df, TestCaseDataFrameSchema)
 
-        upload_data_frame(df=df_validated, batch_size=_BatchSize.UPLOAD_RECORDS, load_uuid=init_response.uuid)
+        upload_data_frame(df=df_validated, batch_size=BatchSize.UPLOAD_RECORDS.value, load_uuid=init_response.uuid)
         request = API.CompleteEditRequest(
             test_case_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             uuid=init_response.uuid,
         )
         complete_res = krequests.post(
-            endpoint_path=API.Path.COMPLETE_EDIT,
+            endpoint_path=API.Path.COMPLETE_EDIT.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=API.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
         log.success(f"edited test case '{self.name}'")
 
@@ -342,11 +342,11 @@
         :param batch_size: optionally specify maximum number of rows to be returned in a single DataFrame. By default,
             limits row count to 10_000_000.
         """
         log.info(f"loading image pairs in test case '{self.name}'")
         init_request = API.InitLoadDataRequest(batch_size=batch_size, test_case_id=self._id)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_DATA,
+            endpoint_path=API.Path.INIT_LOAD_DATA.value,
             df_class=TestCaseDataFrame,
         )
         log.success(f"loaded image pairs in test case '{self.name}'")
```

### Comparing `kolena_client-0.68.0/kolena/fr/test_images.py` & `kolena_client-0.69.0/kolena/fr/test_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 from kolena._api.v1.batched_load import BatchedLoad as LoadAPI
 from kolena._api.v1.fr import TestImages as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
+from kolena._utils.consts import BatchSize
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.uninstantiable import Uninstantiable
 from kolena._utils.validators import ValidatorConfig
 from kolena.fr import TestCase
 from kolena.fr import TestSuite
-from kolena.fr._consts import _BatchSize
 from kolena.fr.datatypes import TEST_IMAGE_COLUMNS
 from kolena.fr.datatypes import TestImageDataFrame
 from kolena.fr.datatypes import TestImageDataFrameSchema
 from kolena.fr.datatypes import TestImageRecord
 
 
 class TestImages(Uninstantiable[None]):
@@ -180,18 +180,18 @@
 
         init_response = init_upload()
         df = pd.DataFrame(registrar.data.records, columns=TEST_IMAGE_COLUMNS)
         df["image_id"] = -1
         df_validated = TestImageDataFrame(validate_df_schema(df, TestImageDataFrameSchema))
         df_serializable = df_validated.as_serializable()
 
-        upload_data_frame(df=df_serializable, batch_size=_BatchSize.UPLOAD_RECORDS, load_uuid=init_response.uuid)
+        upload_data_frame(df=df_serializable, batch_size=BatchSize.UPLOAD_RECORDS.value, load_uuid=init_response.uuid)
         request = LoadAPI.WithLoadUUID(uuid=init_response.uuid)
         finalize_res = krequests.put(
-            endpoint_path=API.Path.COMPLETE_REGISTER,
+            endpoint_path=API.Path.COMPLETE_REGISTER.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(finalize_res)
         log.success("registered test images")
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
@@ -224,15 +224,15 @@
             data_source=data_source if isinstance(data_source, str) else None,
             test_suite_id=test_suite_id,
             test_case_id=test_case_id,
             batch_size=batch_size,
         )
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_REQUEST,
+            endpoint_path=API.Path.INIT_LOAD_REQUEST.value,
             df_class=TestImageDataFrame,
         )
         log.success(f"loaded test images{from_extra}")
 
     @staticmethod
     def _data_source_display_name(
         data_source: Optional[Union[str, TestSuite, TestSuite.Data, TestCase, TestCase.Data]],
```

### Comparing `kolena_client-0.68.0/kolena/fr/test_run.py` & `kolena_client-0.69.0/kolena/fr/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,27 @@
 from kolena._api.v1.fr import TestRun as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.asset_path_mapper import AssetPathMapper
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
-from kolena._utils.batched_load import upload_image_chips
+from kolena._utils.consts import BatchSize
 from kolena._utils.dataframes.validators import validate_df_record_count
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.frozen import Frozen
+from kolena._utils.instrumentation import report_crash
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import InputValidationError
 from kolena.fr import InferenceModel
 from kolena.fr import Model
 from kolena.fr import TestSuite
-from kolena.fr._consts import _BatchSize
+from kolena.fr._utils import upload_image_chips
 from kolena.fr.datatypes import _ImageChipsDataFrame
 from kolena.fr.datatypes import _ResultStageFrame
 from kolena.fr.datatypes import EmbeddingDataFrame
 from kolena.fr.datatypes import ImageDataFrame
 from kolena.fr.datatypes import ImageResultDataFrame
 from kolena.fr.datatypes import ImageResultDataFrameSchema
 from kolena.fr.datatypes import PairDataFrame
@@ -77,15 +78,18 @@
     def __init__(self, model: Model, test_suite: TestSuite, reset: bool = False):
         if reset:
             log.warn("overwriting existing inferences from this model (reset=True)")
         else:
             log.info("reset flag is disabled. update existing inferences by enabling the reset flag")
 
         request = API.CreateOrRetrieveRequest(model_id=model.data.id, test_suite_ids=[test_suite._id], reset=reset)
-        res = krequests.post(endpoint_path=API.Path.CREATE_OR_RETRIEVE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(
+            endpoint_path=API.Path.CREATE_OR_RETRIEVE.value,
+            data=json.dumps(dataclasses.asdict(request)),
+        )
         krequests.raise_for_status(res)
         response = from_dict(data_class=TestRun.Data, data=res.json())
 
         self.data = response
         self._id = response.id
         self._model = model
         self._test_suite = test_suite
@@ -122,15 +126,15 @@
         log.info("loading remaining images for test run")
         init_request = API.InitLoadRemainingImagesRequest(
             test_run_id=self.data.id,
             batch_size=batch_size,
             load_all=self._reset,
         )
         with krequests.put(
-            endpoint_path=API.Path.INIT_LOAD_REMAINING_IMAGES,
+            endpoint_path=API.Path.INIT_LOAD_REMAINING_IMAGES.value,
             data=json.dumps(dataclasses.asdict(init_request)),
             stream=True,
         ) as init_res:
             krequests.raise_for_status(init_res)
 
             load_uuid = None
             try:
@@ -160,38 +164,38 @@
         :return: number of records successfully uploaded.
         :raises TypeValidationError: if the DataFrame failed type validation.
         :raises RemoteError: if the DataFrame was unable to be successfully ingested for any reason.
         """
         log.info("uploading inference results for test run")
         init_response = init_upload()
 
-        asset_config_res = krequests.get(endpoint_path=AssetAPI.Path.CONFIG)
+        asset_config_res = krequests.get(endpoint_path=AssetAPI.Path.CONFIG.value)
         krequests.raise_for_status(asset_config_res)
         asset_config = from_dict(data_class=AssetAPI.Config, data=asset_config_res.json())
         asset_path_mapper = AssetPathMapper(asset_config)
 
         df_validated = ImageResultDataFrame(validate_df_schema(df_image_result, ImageResultDataFrameSchema))
         validate_df_record_count(df_validated)
         df_image_chips = _ImageChipsDataFrame.from_image_result_data_frame(
             test_run_id=self.data.id,
             load_uuid=init_response.uuid,
             df=df_validated,
         )
-        upload_image_chips(df_image_chips, asset_path_mapper)
+        upload_image_chips(df_image_chips)
         df_result_stage = _ResultStageFrame.from_image_result_data_frame(
             test_run_id=self.data.id,
             load_uuid=init_response.uuid,
             df=df_validated,
             path_mapper=asset_path_mapper,
         )
-        upload_data_frame(df_result_stage, _BatchSize.UPLOAD_RECORDS, init_response.uuid)
+        upload_data_frame(df_result_stage, BatchSize.UPLOAD_RECORDS.value, init_response.uuid)
 
         request = API.UploadImageResultsRequest(uuid=init_response.uuid, test_run_id=self.data.id, reset=self._reset)
         finalize_res = krequests.put(
-            endpoint_path=API.Path.COMPLETE_UPLOAD_IMAGE_RESULTS,
+            endpoint_path=API.Path.COMPLETE_UPLOAD_IMAGE_RESULTS.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(finalize_res)
         response = from_dict(data_class=API.UploadImageResultsResponse, data=finalize_res.json())
         log.success("uploaded inference results for test run")
         return response.n_uploaded
 
@@ -218,15 +222,15 @@
         log.info("loading batch of image pairs for test run")
         init_request = API.InitLoadRemainingPairsRequest(
             test_run_id=self.data.id,
             batch_size=batch_size,
             load_all=self._reset,
         )
         with krequests.put(
-            endpoint_path=API.Path.INIT_LOAD_REMAINING_PAIRS,
+            endpoint_path=API.Path.INIT_LOAD_REMAINING_PAIRS.value,
             data=json.dumps(dataclasses.asdict(init_request)),
             stream=True,
         ) as init_res:
             krequests.raise_for_status(init_res)
 
             load_uuid_embedding = None
             load_uuid_pair = None
@@ -275,19 +279,19 @@
         :raises RemoteError: if the DataFrame was unable to be successfully ingested for any reason.
         """
         log.info("uploading pair results for test run")
         init_response = init_upload()
 
         df_validated = validate_df_schema(df_pair_result, PairResultDataFrameSchema)
         validate_df_record_count(df_validated)
-        upload_data_frame(df_validated, _BatchSize.UPLOAD_RECORDS, init_response.uuid)
+        upload_data_frame(df_validated, BatchSize.UPLOAD_RECORDS.value, init_response.uuid)
 
         request = API.UploadPairResultsRequest(uuid=init_response.uuid, test_run_id=self.data.id, reset=self._reset)
         finalize_res = krequests.put(
-            endpoint_path=API.Path.COMPLETE_UPLOAD_PAIR_RESULTS,
+            endpoint_path=API.Path.COMPLETE_UPLOAD_PAIR_RESULTS.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(finalize_res)
         log.success("uploaded pair results for test run")
         response = from_dict(data_class=API.UploadPairResultsResponse, data=finalize_res.json())
         return response.n_uploaded
 
@@ -334,11 +338,9 @@
         ]
         df_pair_result = df_pair[["image_pair_id", "similarity"]]
         if len(df_pair_result) > 0:
             test_run.upload_pair_results(df_pair_result)
         log.success("completed test run")
 
     except Exception as e:
-        request = API.MarkCrashedRequest(test_run_id=test_run.data.id)
-        # note no krequests.raise_for_status -- already in crashed state
-        krequests.post(endpoint_path="/fr/test-run/mark-crashed", data=json.dumps(dataclasses.asdict(request)))
+        report_crash(test_run.data.id, API.Path.MARK_CRASHED.value)
         raise e
```

### Comparing `kolena_client-0.68.0/kolena/fr/test_suite.py` & `kolena_client-0.69.0/kolena/fr/test_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
         :param name: the name of the new test suite to create.
         :param description: optional free-form description of the test suite to create.
         :param test_cases: optionally specify a set of test cases to populate the test suite.
         :return: the newly created test suite.
         """
         request = API.CreateRequest(name=name, description=description or "")
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         obj._hydrate(baseline_test_cases, non_baseline_test_cases)
         log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
@@ -157,15 +157,15 @@
         :raises NotFoundError: if the test suite with the provided name doesn't exist.
         """
         return cls.load(name, version)
 
     @classmethod
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         request = API.LoadByNameRequest(name=name, version=version)
-        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = cls._create_from_data(from_dict(data_class=API.EntityData, data=res.json()))
         log.info(f"loaded test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
     def _populate_from_other(self, other: "TestSuite") -> None:
         with self._unfrozen():
@@ -174,15 +174,15 @@
             self.version = other.version
             self.description = other.description
             self.baseline_test_cases = other.baseline_test_cases
             self.non_baseline_test_cases = other.non_baseline_test_cases
             self.baseline_image_count = other.baseline_image_count
             self.baseline_pair_count_genuine = other.baseline_pair_count_genuine
             self.baseline_pair_count_imposter = other.baseline_pair_count_imposter
-            self.data = other.data
+            self.data = other._data
 
     @classmethod
     def _create_from_data(cls, data: API.EntityData) -> "TestSuite":
         obj = cls.__new__(cls)
         obj._id = data.id
         obj.name = data.name
         obj.version = data.version
@@ -332,12 +332,12 @@
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             baseline_test_case_ids=list(editor._baseline_test_cases.values()),
             non_baseline_test_case_ids=list(editor._non_baseline_test_cases.values()),
         )
-        res = krequests.post(endpoint_path=API.Path.EDIT, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.EDIT.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=API.EntityData, data=res.json())
         self._populate_from_other(self._create_from_data(test_suite_data))
         log.success(f"edited test suite '{self.name}' ({get_test_suite_url(self._id)})")
```

### Comparing `kolena_client-0.68.0/kolena/initialize.py` & `kolena_client-0.69.0/kolena/initialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,35 +7,27 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import dataclasses
 import warnings
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 import pandas as pd
-import requests
 
-import kolena
-import kolena._api.v1.token as API
-from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils.endpoints import get_endpoint
+from kolena._utils import state
 from kolena._utils.endpoints import get_platform_url
 from kolena._utils.instrumentation import upload_log
-from kolena._utils.serde import from_dict
 from kolena._utils.state import _client_state
 from kolena.errors import InputValidationError
-from kolena.errors import InvalidTokenError
-from kolena.errors import UnauthenticatedError
 
 
 def initialize(
     api_token: str,
     *args: Any,
     verbose: bool = False,
     proxies: Optional[Dict[str, str]] = None,
@@ -70,23 +62,15 @@
         used_deprecated_signature = True
         warnings.warn(
             "The signature initialize(entity, token) is deprecated. Please update to initialize(token).",
             category=DeprecationWarning,
             stacklevel=2,
         )
 
-    request = API.ValidateRequest(api_token=api_token, version=kolena.__version__)
-    r = requests.put(get_endpoint("token/login"), json=dataclasses.asdict(request), proxies=proxies)
-
-    try:
-        krequests.raise_for_status(r)
-    except UnauthenticatedError as e:
-        raise InvalidTokenError(e)
-
-    init_response = from_dict(data_class=API.ValidateResponse, data=r.json())
+    init_response = state.get_token(api_token, proxies=proxies)
     derived_telemetry = init_response.tenant_telemetry
     _client_state.update(
         api_token=api_token,
         jwt_token=init_response.access_token,
         tenant=init_response.tenant,
         verbose=verbose,
         telemetry=derived_telemetry,
```

### Comparing `kolena_client-0.68.0/kolena/workflow/__init__.py` & `kolena_client-0.69.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/_datatypes.py` & `kolena_client-0.69.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/_helpers.py` & `kolena_client-0.69.0/kolena/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/_validators.py` & `kolena_client-0.69.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/annotation.py` & `kolena_client-0.69.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/asset.py` & `kolena_client-0.69.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/evaluator.py` & `kolena_client-0.69.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.69.0/kolena/workflow/evaluator_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         log.info(message)
         request = API.UpdateMetricsStatusRequest(
             test_run_id=self._test_run_id,
             progress=progress,
             message=message,
         )
         res = krequests.put(
-            endpoint_path=API.Path.UPDATE_METRICS_STATUS,
+            endpoint_path=API.Path.UPDATE_METRICS_STATUS.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(res)
 
     def _set_configuration(self, configuration: Optional[EvaluatorConfiguration]) -> None:
         self._wip_configuration = configuration
         config_description = (
```

### Comparing `kolena_client-0.68.0/kolena/workflow/ground_truth.py` & `kolena_client-0.69.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/inference.py` & `kolena_client-0.69.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/model.py` & `kolena_client-0.69.0/kolena/workflow/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 from pydantic import validate_arguments
 
 from kolena._api.v1.core import Model as CoreAPI
 from kolena._api.v1.generic import Model as API
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
+from kolena._utils.consts import BatchSize
 from kolena._utils.endpoints import get_model_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
@@ -110,30 +110,30 @@
         :param name: the unique name of the new model to create.
         :param infer: optional inference function for this model.
         :param metadata: optional unstructured metadata to store with this model.
         :return: the newly created model.
         """
         metadata = metadata or {}
         request = CoreAPI.CreateRequest(name=name, metadata=metadata, workflow=cls.workflow.name)
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
         log.info(f"created model '{name}' ({get_model_url(obj._id)})")
         return obj
 
     @classmethod
     def load(cls, name: str, infer: Optional[Callable[[TestSample], Inference]] = None) -> "Model":
         """
         Load an existing model.
 
         :param name: the name of the model to load.
         :param infer: optional inference function for this model.
         """
         request = CoreAPI.LoadByNameRequest(name=name)
-        res = krequests.put(endpoint_path=API.Path.LOAD, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.LOAD.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
         log.info(f"loaded model '{name}' ({get_model_url(obj._id)})")
         return obj
 
     @validate_arguments(config=ValidatorConfig)
     def load_inferences(self, test_case: TestCase) -> List[Tuple[TestSample, GroundTruth, Inference]]:
@@ -155,17 +155,17 @@
         """
         log.info(f"loading inferences from model '{self.name}' on test case '{test_case.name}'")
         assert_workflows_match(self.workflow.name, test_case.workflow.name)
         for df_batch in _BatchedLoader.iter_data(
             init_request=API.LoadInferencesRequest(
                 model_id=self._id,
                 test_case_id=test_case._id,
-                batch_size=_BatchSize.LOAD_SAMPLES,
+                batch_size=BatchSize.LOAD_SAMPLES.value,
             ),
-            endpoint_path=API.Path.LOAD_INFERENCES,
+            endpoint_path=API.Path.LOAD_INFERENCES.value,
             df_class=TestSampleDataFrame,
         ):
             for record in df_batch.itertuples():
                 test_sample = self.workflow.test_sample_type._from_dict(record.test_sample)
                 ground_truth = self.workflow.ground_truth_type._from_dict(record.ground_truth)
                 inference = self.workflow.inference_type._from_dict(record.inference)
                 yield test_sample, ground_truth, inference
```

### Comparing `kolena_client-0.68.0/kolena/workflow/test_case.py` & `kolena_client-0.69.0/kolena/workflow/test_case.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 from pydantic import validate_arguments
 from pydantic.dataclasses import dataclass
 
 from kolena._api.v1.core import TestCase as CoreAPI
 from kolena._api.v1.generic import TestCase as API
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
+from kolena._utils.consts import BatchSize
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
@@ -153,62 +153,62 @@
         :param name: the name of the new test case to create.
         :param description: optional free-form description of the test case to create.
         :param test_samples: optionally specify a set of test samples and ground truths to populate the test case.
         :return: the newly created test case.
         """
         cls._validate_test_samples(test_samples)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name)
-        res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_samples is not None:
             obj._hydrate(test_samples)
-        log.info(f"created test case '{name}'")
+        log.info(f"created test case '{name}' (v{obj.version})")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
         Load an existing test case with the provided name.
 
         :param name: the name of the test case to load.
         :param version: optionally specify a particular version of the test case to load. Defaults to the latest version
             when unset.
         :return: the loaded test case.
         """
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
-        res = krequests.put(endpoint_path=API.Path.LOAD, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.LOAD.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
-        log.info(f"loaded test case '{name}'")
+        log.info(f"loaded test case '{name}' (v{data.version})")
         return cls._create_from_data(data)
 
     def load_test_samples(self) -> List[Tuple[TestSample, GroundTruth]]:
         """Load all test samples and ground truths in this test case."""
         return list(self.iter_test_samples())
 
     def iter_test_samples(self) -> Iterator[Tuple[TestSample, GroundTruth]]:
         """Iterate through all test samples and ground truths in this test case."""
-        log.info(f"loading test samples in test case '{self.name}'")
+        log.info(f"loading test samples in test case '{self.name}' (v{self.version})")
         test_sample_type = self.workflow.test_sample_type
         ground_truth_type = self.workflow.ground_truth_type
-        init_request = CoreAPI.InitLoadContentsRequest(batch_size=_BatchSize.LOAD_SAMPLES, test_case_id=self._id)
+        init_request = CoreAPI.InitLoadContentsRequest(batch_size=BatchSize.LOAD_SAMPLES.value, test_case_id=self._id)
         for df in _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.INIT_LOAD_TEST_SAMPLES,
+            endpoint_path=API.Path.INIT_LOAD_TEST_SAMPLES.value,
             df_class=TestSampleDataFrame,
         ):
             has_metadata = "test_sample_metadata" in df.columns
             for record in df.itertuples():
                 metadata_field = record.test_sample_metadata if has_metadata else {}
                 test_sample = test_sample_type._from_dict({**record.test_sample, "metadata": metadata_field})
                 ground_truth = ground_truth_type._from_dict(record.ground_truth)
                 yield test_sample, ground_truth
-        log.success(f"loaded test samples in test case '{self.name}'")
+        log.success(f"loaded test samples in test case '{self.name}' (v{self.version})")
 
     class Editor:
         @dataclass(frozen=True)
         class _Edit:
             test_sample: TestSample
             ground_truth: Optional[GroundTruth] = None
             remove: bool = False
@@ -287,27 +287,27 @@
         editor = self.Editor(self.description, reset)
 
         yield editor
 
         if not editor._edited():
             return
 
-        log.info(f"editing test case '{self.name}'")
+        log.info(f"editing test case '{self.name}' (v{self.version})")
         init_response = init_upload()
         df_serialized = editor._to_data_frame().as_serializable()
-        upload_data_frame(df=df_serialized, batch_size=_BatchSize.UPLOAD_RECORDS, load_uuid=init_response.uuid)
+        upload_data_frame(df=df_serialized, batch_size=BatchSize.UPLOAD_RECORDS.value, load_uuid=init_response.uuid)
 
         request = CoreAPI.CompleteEditRequest(
             test_case_id=self._id,
             current_version=self.version,
             description=editor._description,
             reset=editor._reset,
             uuid=init_response.uuid,
         )
         complete_res = krequests.put(
-            endpoint_path=API.Path.COMPLETE_EDIT,
+            endpoint_path=API.Path.COMPLETE_EDIT.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=CoreAPI.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
-        log.success(f"edited test case '{self.name}'")
+        log.success(f"edited test case '{self.name}' (v{self.version})")
```

### Comparing `kolena_client-0.68.0/kolena/workflow/test_run.py` & `kolena_client-0.69.0/kolena/workflow/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import pandas as pd
 from pydantic import validate_arguments
 
-from kolena._api.v1.core import TestRun as CoreAPI
 from kolena._api.v1.generic import TestRun as API
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame_chunk
+from kolena._utils.consts import BatchSize
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.endpoints import get_results_url
 from kolena._utils.frozen import Frozen
+from kolena._utils.instrumentation import report_crash
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import InputValidationError
 from kolena.errors import WorkflowMismatchError
 from kolena.workflow import Evaluator
 from kolena.workflow import EvaluatorConfiguration
@@ -146,15 +146,18 @@
 
         request = API.CreateOrRetrieveRequest(
             model_id=model._id,
             test_suite_id=test_suite._id,
             evaluator=evaluator_display_name,
             configurations=api_configurations,
         )
-        res = krequests.put(endpoint_path=API.Path.CREATE_OR_RETRIEVE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(
+            endpoint_path=API.Path.CREATE_OR_RETRIEVE.value,
+            data=json.dumps(dataclasses.asdict(request)),
+        )
         krequests.raise_for_status(res)
         response = from_dict(data_class=API.CreateOrRetrieveResponse, data=res.json())
         self._id = response.test_run_id
         self._freeze()
 
     def run(self) -> None:
         """
@@ -171,17 +174,15 @@
             if len(inferences) > 0:
                 log.success(f"performed inference on {len(inferences)} test samples")
                 log.info("uploading inferences")
                 self.upload_inferences(inferences)
 
             self.evaluate()
         except Exception as e:
-            request = CoreAPI.MarkCrashedRequest(test_run_id=self._id)
-            # note no krequests.raise_for_status -- already in crashed state
-            krequests.post(endpoint_path=API.Path.MARK_CRASHED, data=json.dumps(dataclasses.asdict(request)))
+            report_crash(self._id, API.Path.MARK_CRASHED.value)
             raise e
 
     def load_test_samples(self) -> List[TestSample]:
         """
         Load the test samples in the test suite that do not yet have inferences uploaded.
 
         :return: a list of all test samples in the test suite still requiring inferences.
@@ -205,17 +206,17 @@
 
         :return: an iterator exposing the ground truths and inferences for all test samples in the test run.
         """
         log.info(f"loading inferences from model '{self.model.name}' on test suite '{self.test_suite.name}'")
         for df_batch in _BatchedLoader.iter_data(
             init_request=API.LoadTestSampleInferencesRequest(
                 test_run_id=self._id,
-                batch_size=_BatchSize.LOAD_SAMPLES,
+                batch_size=BatchSize.LOAD_SAMPLES.value,
             ),
-            endpoint_path=API.Path.LOAD_INFERENCES,
+            endpoint_path=API.Path.LOAD_INFERENCES.value,
             df_class=TestSampleDataFrame,
         ):
             for record in df_batch.itertuples():
                 test_sample = self.test_suite.workflow.test_sample_type._from_dict(record.test_sample)
                 ground_truth = self.test_suite.workflow.ground_truth_type._from_dict(record.ground_truth)
                 inference = self.test_suite.workflow.inference_type._from_dict(record.inference)
                 yield test_sample, ground_truth, inference
@@ -236,15 +237,18 @@
         df_validated = TestSampleDataFrame(validate_df_schema(df, TestSampleDataFrameSchema, trusted=True))
         df_serializable = df_validated.as_serializable()
 
         init_response = init_upload()
         upload_data_frame_chunk(df_serializable, init_response.uuid)
 
         request = API.UploadInferencesRequest(uuid=init_response.uuid, test_run_id=self._id, reset=self.reset)
-        res = krequests.put(endpoint_path=API.Path.UPLOAD_INFERENCES, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(
+            endpoint_path=API.Path.UPLOAD_INFERENCES.value,
+            data=json.dumps(dataclasses.asdict(request)),
+        )
         krequests.raise_for_status(res)
 
     def evaluate(self) -> None:
         """
         Perform evaluation by computing metrics for individual test samples, in aggregate across test cases, and across
         the complete test suite at each :class:`kolena.workflow.EvaluatorConfiguration`.
         """
@@ -372,25 +376,28 @@
         log.info("uploading test case metrics")
         self._upload_test_case_metrics(test_case_metrics)
         log.info("uploading test case plots")
         self._upload_test_case_plots(test_case_plots)
         log.info("uploading test suite metrics")
         self._upload_test_suite_metrics(test_suite_metrics)
 
-    def _iter_test_samples_batch(self, batch_size: int = _BatchSize.LOAD_SAMPLES) -> Iterator[TestSampleDataFrame]:
+    def _iter_test_samples_batch(
+        self,
+        batch_size: int = BatchSize.LOAD_SAMPLES.value,
+    ) -> Iterator[TestSampleDataFrame]:
         if batch_size <= 0:
             raise InputValidationError(f"invalid batch_size '{batch_size}': expected positive integer")
         init_request = API.LoadRemainingTestSamplesRequest(
             test_run_id=self._id,
             batch_size=batch_size,
             load_all=self.reset,
         )
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
-            endpoint_path=API.Path.LOAD_TEST_SAMPLES,
+            endpoint_path=API.Path.LOAD_TEST_SAMPLES.value,
             df_class=TestSampleDataFrame,
         )
 
     @validate_arguments(config=ValidatorConfig)
     def _upload_test_sample_metrics(
         self,
         test_case: Optional[TestCase],
@@ -408,55 +415,55 @@
         request = API.UploadTestSampleMetricsRequest(
             uuid=init_response.uuid,
             test_run_id=self._id,
             test_case_id=test_case._id if test_case is not None else None,
             configuration=_maybe_evaluator_configuration_to_api(configuration),
         )
         res = krequests.put(
-            endpoint_path=API.Path.UPLOAD_TEST_SAMPLE_METRICS,
+            endpoint_path=API.Path.UPLOAD_TEST_SAMPLE_METRICS.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(res)
 
     def _upload_test_case_metrics(
         self,
         metrics: Dict[int, Dict[Optional[EvaluatorConfiguration], MetricsTestCase]],
     ) -> None:
         records = [
             (test_case_id, _maybe_display_name(config), tc_metrics._to_dict())
             for test_case_id, tc_metrics_by_config in metrics.items()
             for config, tc_metrics in tc_metrics_by_config.items()
         ]
         df = pd.DataFrame(records, columns=["test_case_id", "configuration_display_name", "metrics"])
-        return self._upload_aggregate_metrics(API.Path.UPLOAD_TEST_CASE_METRICS, df)
+        return self._upload_aggregate_metrics(API.Path.UPLOAD_TEST_CASE_METRICS.value, df)
 
     def _upload_test_case_plots(
         self,
         plots: Dict[int, Dict[Optional[EvaluatorConfiguration], Optional[List[Plot]]]],
     ) -> None:
         records = [
             (test_case_id, _maybe_display_name(config), tc_plot._to_dict())
             for test_case_id, tc_plots_by_config in plots.items()
             for config, tc_plots in tc_plots_by_config.items()
             for tc_plot in tc_plots or []
         ]
         df = pd.DataFrame(records, columns=["test_case_id", "configuration_display_name", "metrics"])
-        return self._upload_aggregate_metrics(API.Path.UPLOAD_TEST_CASE_PLOTS, df)
+        return self._upload_aggregate_metrics(API.Path.UPLOAD_TEST_CASE_PLOTS.value, df)
 
     def _upload_test_suite_metrics(
         self,
         metrics: Dict[Optional[EvaluatorConfiguration], Optional[MetricsTestSuite]],
     ) -> None:
         records: List[Tuple[Optional[str], Dict[str, Any]]] = [
             (_maybe_display_name(config), ts_metrics._to_dict())
             for config, ts_metrics in metrics.items()
             if ts_metrics is not None
         ]
         df = pd.DataFrame(records, columns=["configuration_display_name", "metrics"])
-        return self._upload_aggregate_metrics(API.Path.UPLOAD_TEST_SUITE_METRICS, df)
+        return self._upload_aggregate_metrics(API.Path.UPLOAD_TEST_SUITE_METRICS.value, df)
 
     def _upload_aggregate_metrics(self, endpoint_path: str, df: pd.DataFrame) -> None:
         df_validated = MetricsDataFrame(validate_df_schema(df, MetricsDataFrameSchema, trusted=True))
         df_serializable = df_validated.as_serializable()
 
         init_response = init_upload()
         upload_data_frame_chunk(df_serializable, init_response.uuid)
@@ -467,15 +474,15 @@
             test_suite_id=self.test_suite._id,
         )
         res = krequests.put(endpoint_path=endpoint_path, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
 
     def _start_server_side_evaluation(self) -> None:
         request = API.EvaluateRequest(test_run_id=self._id)
-        res = krequests.put(endpoint_path=API.Path.EVALUATE, data=json.dumps(dataclasses.asdict(request)))
+        res = krequests.put(endpoint_path=API.Path.EVALUATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
 
 
 @validate_arguments(config=ValidatorConfig)
 def test(
     model: Model,
     test_suite: TestSuite,
```

### Comparing `kolena_client-0.68.0/kolena/workflow/test_sample.py` & `kolena_client-0.69.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.68.0/kolena/workflow/test_suite.py` & `kolena_client-0.69.0/kolena/workflow/test_suite.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,31 +16,33 @@
 from abc import ABCMeta
 from collections import defaultdict
 from contextlib import contextmanager
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Optional
+from typing import Set
 from typing import Tuple
 from typing import Type
 
 from pydantic import validate_arguments
 
 from kolena._api.v1.core import TestSuite as CoreAPI
 from kolena._api.v1.generic import TestSuite as API
 from kolena._utils import krequests
 from kolena._utils import log
-from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
+from kolena._utils.consts import BatchSize
 from kolena._utils.endpoints import get_test_suite_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
+from kolena.errors import IncorrectUsageError
 from kolena.errors import NotFoundError
 from kolena.workflow import TestSample
 from kolena.workflow._datatypes import TestSuiteTestSamplesDataFrame
 from kolena.workflow._validators import assert_workflows_match
 from kolena.workflow.test_case import TestCase
 from kolena.workflow.workflow import Workflow
 
@@ -66,14 +68,17 @@
 
     #: Free-form, human-readable description of this test suite. Can be edited at any time via :meth:`TestSuite.edit`.
     description: str
 
     #: The :class:`kolena.workflow.TestCase` objects belonging to this test suite.
     test_cases: List[TestCase]
 
+    #: The tags associated with this test suite.
+    tags: Set[str]
+
     @telemetry
     def __init_subclass__(cls) -> None:
         if not hasattr(cls, "workflow"):
             raise NotImplementedError(f"{cls.__name__} must implement class attribute 'workflow'")
         if not hasattr(cls, "_test_case_type"):
             raise NotImplementedError(f"{cls.__name__} must implement class attribute '_test_case_type'")
         super().__init_subclass__()
@@ -82,123 +87,177 @@
     def __init__(
         self,
         name: str,
         version: Optional[int] = None,
         description: Optional[str] = None,
         test_cases: Optional[List[TestCase]] = None,
         reset: bool = False,
+        tags: Optional[Set[str]] = None,
     ):
-        if type(self) == TestSuite:
-            raise Exception("<TestSuite> must be subclassed.")
+        self._validate_workflow()
         self._validate_test_cases(test_cases)
 
         try:
-            self._populate_from_other(self.load(name, version))
-            if description is not None and self.description != description and not reset:
-                log.warn("test suite already exists, not updating description when reset=False")
-            if test_cases is not None:
-                if self.version > 0 and not reset:
-                    log.warn("test suite already exists, not updating test cases when reset=False")
-                else:
-                    self._hydrate(test_cases, description)
+            other = self.load(name, version)
         except NotFoundError:
-            self._populate_from_other(self.create(name, description, test_cases))
+            other = self.create(name, description, test_cases, tags)
+        self._populate_from_other(other)
+
+        should_update_test_cases = test_cases is not None and test_cases != self.test_cases
+        can_update_test_cases = reset or self.version == 0
+        if should_update_test_cases and not can_update_test_cases:
+            log.warn(f"reset=False, not updating test cases on test suite '{self.name}' (v{self.version})")
+        to_update = [
+            *(["test cases"] if should_update_test_cases and can_update_test_cases else []),
+            *(["description"] if description is not None and description != self.description else []),
+            *(["tags"] if tags is not None and tags != self.tags else []),
+        ]
+        if len(to_update) > 0:
+            log.info(f"updating {', '.join(to_update)} on test suite '{self.name}' (v{self.version})")
+            updated_test_cases = test_cases or self.test_cases if can_update_test_cases else self.test_cases
+            self._hydrate(updated_test_cases, description=description, tags=tags)
+
         self._freeze()
 
     @classmethod
     def _validate_test_cases(cls, test_cases: Optional[List[TestCase]] = None) -> None:
         if test_cases:
             if any(cls.workflow != testcase.workflow for testcase in test_cases):
                 raise TypeError("test case workflow does not match test suite's")
 
+    @classmethod
+    def _validate_workflow(cls) -> None:
+        if cls == TestSuite:
+            raise IncorrectUsageError("<TestSuite> must be subclassed. See `kolena.workflow.define_workflow`")
+
     def _populate_from_other(self, other: "TestSuite") -> None:
         with self._unfrozen():
             self._id = other._id
             self.name = other.name
             self.version = other.version
             self.description = other.description
             self.test_cases = other.test_cases
+            self.tags = other.tags
 
     @classmethod
     def _create_from_data(cls, data: CoreAPI.EntityData) -> "TestSuite":
         assert_workflows_match(cls.workflow.name, data.workflow)
         obj = cls.__new__(cls)
         obj._id = data.id
         obj.name = data.name
         obj.version = data.version
         obj.description = data.description
         obj.test_cases = [cls._test_case_type._create_from_data(tc) for tc in data.test_cases]
+        obj.tags = set(data.tags)
         obj._freeze()
         return obj
 
-    def _hydrate(self, test_cases: List[TestCase], description: Optional[str] = None) -> None:
+    def _hydrate(
+        self,
+        test_cases: List[TestCase],
+        description: Optional[str] = None,
+        tags: Optional[Set[str]] = None,
+    ) -> None:
         with self.edit(reset=True) as editor:
             if description is not None:
                 editor.description(description)
             for test_case in test_cases:
                 editor.add(test_case)
+            if tags is not None:
+                editor.tags = tags
 
     @classmethod
     def create(
         cls,
         name: str,
         description: Optional[str] = None,
         test_cases: Optional[List[TestCase]] = None,
+        tags: Optional[Set[str]] = None,
     ) -> "TestSuite":
         """
         Create a new test suite with the provided name.
 
         :param name: the name of the new test suite to create.
         :param description: optional free-form description of the test suite to create.
-        :param test_cases: optionally specify a set of test cases to populate the test suite.
+        :param test_cases: optionally specify a list of test cases to populate the test suite.
+        :param tags: optionally specify a set of tags to attach to the test suite.
         :return: the newly created test suite.
         """
+        cls._validate_workflow()
         cls._validate_test_cases(test_cases)
-        request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name)
+        request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name, tags=tags)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_cases is not None:
             obj._hydrate(test_cases)
-        log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
+        log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         """
         Load an existing test suite with the provided name.
 
         :param name: the name of the test suite to load.
         :param version: optionally specify a particular version of the test suite to load. Defaults to the latest
             version when unset.
         :return: the loaded test suite.
         """
+        cls._validate_workflow()
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
-        log.info(f"loaded test suite '{name}' ({get_test_suite_url(obj._id)})")
+        log.info(f"loaded test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         return obj
 
+    @classmethod
+    def load_all(cls, *, tags: Optional[Set[str]] = None) -> List["TestSuite"]:
+        """
+        Load the latest version of all non-archived test suites with this workflow.
+
+        :param tags: optionally specify a set of tags to apply as a filter. The loaded test suites will include only
+            test suites with tags matching each of these specified tags, i.e.
+            ``test_suite.tags.intersection(tags) == tags``.
+        :return: the latest version of all non-archived test suites, with matching tags when specified.
+        """
+        cls._validate_workflow()
+        request = CoreAPI.LoadAllRequest(workflow=cls.workflow.name, tags=tags)
+        res = krequests.put(endpoint_path=API.Path.LOAD_ALL.value, data=json.dumps(dataclasses.asdict(request)))
+        krequests.raise_for_status(res)
+        data = from_dict(data_class=CoreAPI.LoadAllResponse, data=res.json())
+        objs = [cls._create_from_data(test_suite) for test_suite in data.test_suites]
+        tags_quoted = {f"'{t}'" for t in tags or {}}
+        tags_message = f" with tag{'s' if len(tags) > 1 else ''} {', '.join(tags_quoted)}" if tags else ""
+        log.info(f"loaded {len(objs)} '{cls.workflow.name}' test suites{tags_message}")
+        return objs
+
     class Editor:
         _test_cases: List[TestCase]
         _reset: bool
         _description: str
         _initial_test_case_ids: List[int]
         _initial_description: str
+        _initial_tags: Set[str]
+
+        #: The tags associated with this test suite. Modify this list directly to edit this test suite's tags.
+        tags: Set[str]
 
         @validate_arguments(config=ValidatorConfig)
-        def __init__(self, test_cases: List[TestCase], description: str, reset: bool):
+        def __init__(self, test_cases: List[TestCase], description: str, tags: Set[str], reset: bool):
             self._test_cases = test_cases if not reset else []
             self._reset = reset
             self._description = description
             self._initial_test_case_ids = [tc._id for tc in test_cases]
             self._initial_description = description
+            self._initial_tags = tags
+            self.tags = tags
 
         @validate_arguments(config=ValidatorConfig)
         def description(self, description: str) -> None:
             """Update the description of the test suite."""
             self._description = description
 
         @validate_arguments(config=ValidatorConfig)
@@ -217,16 +276,19 @@
             Remove a test case from this test suite. Does nothing if the test case is not in the test suite.
 
             :param test_case: the test case to remove.
             """
             self._test_cases = [tc for tc in self._test_cases if tc.name != test_case.name]
 
         def _edited(self) -> bool:
-            test_case_ids = [tc._id for tc in self._test_cases]
-            return self._description != self._initial_description or self._initial_test_case_ids != test_case_ids
+            return (
+                self._description != self._initial_description
+                or self._initial_test_case_ids != [tc._id for tc in self._test_cases]
+                or self._initial_tags != self.tags
+            )
 
     @contextmanager
     def edit(self, reset: bool = False) -> Iterator[Editor]:
         """
         Edit this test suite in a context:
 
         .. code-block:: python
@@ -236,41 +298,42 @@
                 editor.add(...)
                 editor.remove(...)
 
         Changes are committed to the Kolena platform when the context is exited.
 
         :param reset: clear any and all test cases currently in the test suite.
         """
-        editor = self.Editor(self.test_cases, self.description, reset)
+        editor = self.Editor(self.test_cases, self.description, self.tags, reset)
 
         yield editor
 
         if not editor._edited():
             return
 
-        log.info(f"editing test suite '{self.name}'")
+        log.info(f"editing test suite '{self.name}' (v{self.version})")
         request = CoreAPI.EditRequest(
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             test_case_ids=[tc._id for tc in editor._test_cases],
+            tags=list(editor.tags),
         )
         res = krequests.post(endpoint_path=API.Path.EDIT, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         self._populate_from_other(self._create_from_data(test_suite_data))
-        log.success(f"edited test suite '{self.name}' ({get_test_suite_url(self._id)})")
+        log.success(f"edited test suite '{self.name}' (v{self.version}) ({get_test_suite_url(self._id)})")
 
     def load_test_samples(self) -> List[Tuple[TestCase, List[TestSample]]]:
         test_case_id_to_samples: Dict[int, List[TestSample]] = defaultdict(list)
         for df_batch in _BatchedLoader.iter_data(
             init_request=API.LoadTestSamplesRequest(
                 test_suite_id=self._id,
-                batch_size=_BatchSize.LOAD_SAMPLES,
+                batch_size=BatchSize.LOAD_SAMPLES,
             ),
             endpoint_path=API.Path.INIT_LOAD_TEST_SAMPLES,
             df_class=TestSuiteTestSamplesDataFrame,
         ):
             for record in df_batch.itertuples():
                 test_sample = self.workflow.test_sample_type._from_dict(record.test_sample)
                 test_case_id_to_samples[record.test_case_id].append(test_sample)
```

### Comparing `kolena_client-0.68.0/kolena/workflow/workflow.py` & `kolena_client-0.69.0/kolena/workflow/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     :param image: fully qualified docker image name, i.e. <repository-url>/<image>:<tag>
     :param secret: sensitive data in string format
     :param aws_assume_role: AWS role that the evaluator would use to access AWS APIs
     :return: registered evaluator data
     """
 
     response = krequests.post(
-        API.Path.EVALUATOR,
+        API.Path.EVALUATOR.value,
         json=dict(workflow=workflow, image=image, name=evaluator_name, secret=secret, aws_assume_role=aws_assume_role),
     )
     krequests.raise_for_status(response)
 
     log.info(f"Image {image} successfully registered for evaluator {evaluator_name}.")
 
     result = dacite.from_dict(API.EvaluatorResponse, response.json())
@@ -218,15 +218,15 @@
     """
     List all evaluators registered for a given workflow.
 
     :param workflow: workflow name
     :return: list of registered evaluators
     """
 
-    response = krequests.get(f"{API.Path.EVALUATOR}/{quote(workflow)}")
+    response = krequests.get(f"{API.Path.EVALUATOR.value}/{quote(workflow)}")
     krequests.raise_for_status(response)
 
     return [
         RemoteEvaluator(workflow=workflow, name=evaluator.name, image=evaluator.image, created=evaluator.created)
         for evaluator in dacite.from_dict(API.ListEvaluatorsResponse, response.json()).evaluators
     ]
 
@@ -239,14 +239,14 @@
     :param workflow: workflow name
     :param evaluator_name: evaluator name
     :param include_secret: retrieve secret registered with the evaluator or not
     :return: remote evaluator
     """
 
     response = krequests.get(
-        f"{API.Path.EVALUATOR}/{quote(workflow)}/{quote(evaluator_name)}",
-        params={"include_secret": include_secret},
+        endpoint_path=f"{API.Path.EVALUATOR.value}/{quote(workflow)}/{quote(evaluator_name)}",
+        params=dict(include_secret=include_secret),
     )
     krequests.raise_for_status(response)
 
     result = dacite.from_dict(API.EvaluatorResponse, response.json())
     return RemoteEvaluator._from_api_response(workflow, result)
```

### Comparing `kolena_client-0.68.0/setup.py` & `kolena_client-0.69.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,45 +20,46 @@
 
 install_requires = \
 ['Pillow>=9.1.1,<10.0.0',
  'Shapely>=1.8.5,<2.0.0',
  'click>=8.1.3,<9.0.0',
  'dacite>=1.6',
  'deprecation>=2.1.0,<3.0.0',
- 'numpy>=1.19',
- 'pandas>=1.1,<1.6',
  'pandera>=0.9.0',
  'pyarrow>=8',
  'pydantic>=1.8',
- 'requests-toolbelt>=1.0.0,<2.0.0',
- 'requests>=2.20',
+ 'requests-toolbelt',
+ 'requests>=2.20,<2.30',
  'retrying>=1.3.3,<2.0.0',
  'termcolor>=1.1.0,<2.0.0',
  'tqdm>=4,<5']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata<5.0',
-                             'typing-extensions>=4.5.0,<5.0.0']}
+                             'typing-extensions>=4.5.0,<5.0.0'],
+ ':python_version >= "3.11"': ['numpy>=1.23', 'pandas>=1.5,<1.6'],
+ ':python_version >= "3.7" and python_version < "3.11"': ['numpy>=1.19',
+                                                          'pandas>=1.1,<1.6']}
 
 entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']}
 
 setup_kwargs = {
     'name': 'kolena-client',
-    'version': '0.68.0',
+    'version': '0.69.0',
     'description': "Client for Kolena's machine learning (ML) testing and debugging platform.",
-    'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>\n  <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\n`kolena-client` is the Python client library for programmatic interaction with Kolena.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena-client` typing and\nfunction documentation.\n',
+    'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena" /></a>\n  <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk" /></a>\n  <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1"/></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/resource-docs-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\nThis `kolena` package contains the Python client library for programmatic interaction with the Kolena ML testing\nplatform.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena` typing and\nfunction documentation.\n',
     'author': 'Kolena Engineering',
     'author_email': 'eng@kolena.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kolena.io',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.11',
+    'python_requires': '>=3.7.1,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,37 +1,40 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['kolena',
 'kolena._api', 'kolena._api.v1', 'kolena._utils', 'kolena._utils.dataframes',
 'kolena.classification', 'kolena.classification.multiclass',
 'kolena.detection', 'kolena.detection._internal', 'kolena.fr',
 'kolena.workflow', 'kolena.workflow.metrics'] package_data = \ {'': ['*']}
 install_requires = \ ['Pillow>=9.1.1,<10.0.0', 'Shapely>=1.8.5,<2.0.0',
 'click>=8.1.3,<9.0.0', 'dacite>=1.6', 'deprecation>=2.1.0,<3.0.0',
-'numpy>=1.19', 'pandas>=1.1,<1.6', 'pandera>=0.9.0', 'pyarrow>=8',
-'pydantic>=1.8', 'requests-toolbelt>=1.0.0,<2.0.0', 'requests>=2.20',
-'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0', 'tqdm>=4,<5']
-extras_require = \ {':python_version < "3.8"': ['importlib-metadata<5.0',
-'typing-extensions>=4.5.0,<5.0.0']} entry_points = \ {'console_scripts':
-['kolena = kolena._utils.cli:run']} setup_kwargs = { 'name': 'kolena-client',
-'version': '0.68.0', 'description': "Client for Kolena's machine learning (ML)
-testing and debugging platform.", 'long_description': '
+'pandera>=0.9.0', 'pyarrow>=8', 'pydantic>=1.8', 'requests-toolbelt',
+'requests>=2.20,<2.30', 'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0',
+'tqdm>=4,<5'] extras_require = \ {':python_version < "3.8"': ['importlib-
+metadata<5.0', 'typing-extensions>=4.5.0,<5.0.0'], ':python_version >= "3.11"':
+['numpy>=1.23', 'pandas>=1.5,<1.6'], ':python_version >= "3.7" and
+python_version < "3.11"': ['numpy>=1.19', 'pandas>=1.1,<1.6']} entry_points = \
+{'console_scripts': ['kolena = kolena._utils.cli:run']} setup_kwargs =
+{ 'name': 'kolena-client', 'version': '0.69.0', 'description': "Client for
+Kolena's machine learning (ML) testing and debugging platform.",
+'long_description': '
                                  \n [Kolena]\n
 \n\n
-\n [https://img.shields.io/pypi/v/kolena-client]\n [https://img.shields.io/
-pypi/l/kolena-client]\n [https://img.shields.io/badge/docs-
-Tutorial%20%26%20Usage-6434c1]\n [https://img.shields.io/badge/docs-
-API%20Reference-6434c1]\n
+\n [https://img.shields.io/pypi/v/kolena]\n [https://img.shields.io/pypi/l/
+kolena]\n [https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk]\n
+[https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/
+badge.svg?token=8WOY5I8SF1]\n [https://img.shields.io/badge/resource-docs-
+6434c1]\n
 \n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning
 testing and debugging platform to surface hidden\nmodel behaviors and take the
 mystery out of model development. Kolena helps you:\n\n- Perform high-
 resolution model evaluation\n- Understand and track behavioral improvements and
 regressions\n- Meaningfully communicate model capabilities\n- Automate model
-testing and deployment workflows\n\n`kolena-client` is the Python client
-library for programmatic interaction with Kolena.\n\n## Documentation\n\nVisit
-[docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation
-and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/
-index.html) for detailed `kolena-client` typing and\nfunction
-documentation.\n', 'author': 'Kolena Engineering', 'author_email':
-'eng@kolena.io', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://kolena.io', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'entry_points': entry_points, 'python_requires': '>=3.7.1,<3.11', } setup
-(**setup_kwargs)
+testing and deployment workflows\n\nThis `kolena` package contains the Python
+client library for programmatic interaction with the Kolena ML
+testing\nplatform.\n\n## Documentation\n\nVisit [docs.kolena.io](https://
+docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference]
+(https://app.kolena.io/api/developer/docs/html/index.html) for detailed
+`kolena` typing and\nfunction documentation.\n', 'author': 'Kolena
+Engineering', 'author_email': 'eng@kolena.io', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://kolena.io', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'extras_require': extras_require, 'entry_points': entry_points,
+'python_requires': '>=3.7.1,<3.12', } setup(**setup_kwargs)
```

### Comparing `kolena_client-0.68.0/PKG-INFO` & `kolena_client-0.69.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.68.0
+Version: 0.69.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.7.1,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
 Requires-Dist: Pillow (>=9.1.1,<10.0.0)
 Requires-Dist: Shapely (>=1.8.5,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dacite (>=1.6)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: importlib-metadata (<5.0); python_version < "3.8"
-Requires-Dist: numpy (>=1.19)
-Requires-Dist: pandas (>=1.1,<1.6)
+Requires-Dist: numpy (>=1.19); python_version >= "3.7" and python_version < "3.11"
+Requires-Dist: numpy (>=1.23); python_version >= "3.11"
+Requires-Dist: pandas (>=1.1,<1.6); python_version >= "3.7" and python_version < "3.11"
+Requires-Dist: pandas (>=1.5,<1.6); python_version >= "3.11"
 Requires-Dist: pandera (>=0.9.0)
 Requires-Dist: pyarrow (>=8)
 Requires-Dist: pydantic (>=1.8)
-Requires-Dist: requests (>=2.20)
-Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.20,<2.30)
+Requires-Dist: requests-toolbelt
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0); python_version < "3.8"
 Project-URL: Documentation, https://docs.kolena.io
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />
 </p>
 
 <p align='center'>
-  <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>
-  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>
-  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>
-  <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>
+  <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena" /></a>
+  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena" /></a>
+  <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk" /></a>
+  <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1"/></a>
+  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/resource-docs-6434c1" /></a>
 </p>
 
 ---
 
 [Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden
 model behaviors and take the mystery out of model development. Kolena helps you:
 
 - Perform high-resolution model evaluation
 - Understand and track behavioral improvements and regressions
 - Meaningfully communicate model capabilities
 - Automate model testing and deployment workflows
 
-`kolena-client` is the Python client library for programmatic interaction with Kolena.
+This `kolena` package contains the Python client library for programmatic interaction with the Kolena ML testing
+platform.
 
 ## Documentation
 
 Visit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the
-[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena-client` typing and
+[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena` typing and
 function documentation.
```

#### html2text {}

```diff
@@ -1,39 +1,45 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.68.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.69.0 Summary: Client for
 Kolena's machine learning (ML) testing and debugging platform. Home-page:
 https://kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author:
-Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.11
+Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Visualization Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Software
-Development :: Quality Assurance Classifier: Topic :: Software Development ::
-Testing Classifier: Typing :: Typed Requires-Dist: Pillow (>=9.1.1,<10.0.0)
-Requires-Dist: Shapely (>=1.8.5,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: dacite (>=1.6) Requires-Dist: deprecation (>=2.1.0,<3.0.0)
-Requires-Dist: importlib-metadata (<5.0); python_version < "3.8" Requires-Dist:
-numpy (>=1.19) Requires-Dist: pandas (>=1.1,<1.6) Requires-Dist: pandera
-(>=0.9.0) Requires-Dist: pyarrow (>=8) Requires-Dist: pydantic (>=1.8)
-Requires-Dist: requests (>=2.20) Requires-Dist: requests-toolbelt
-(>=1.0.0,<2.0.0) Requires-Dist: retrying (>=1.3.3,<2.0.0) Requires-Dist:
-termcolor (>=1.1.0,<2.0.0) Requires-Dist: tqdm (>=4,<5) Requires-Dist: typing-
-extensions (>=4.5.0,<5.0.0); python_version < "3.8" Project-URL: Documentation,
-https://docs.kolena.io Description-Content-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
+Engineering :: Visualization Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Quality Assurance Classifier: Topic :: Software Development :: Testing
+Classifier: Typing :: Typed Requires-Dist: Pillow (>=9.1.1,<10.0.0) Requires-
+Dist: Shapely (>=1.8.5,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-
+Dist: dacite (>=1.6) Requires-Dist: deprecation (>=2.1.0,<3.0.0) Requires-Dist:
+importlib-metadata (<5.0); python_version < "3.8" Requires-Dist: numpy
+(>=1.19); python_version >= "3.7" and python_version < "3.11" Requires-Dist:
+numpy (>=1.23); python_version >= "3.11" Requires-Dist: pandas (>=1.1,<1.6);
+python_version >= "3.7" and python_version < "3.11" Requires-Dist: pandas
+(>=1.5,<1.6); python_version >= "3.11" Requires-Dist: pandera (>=0.9.0)
+Requires-Dist: pyarrow (>=8) Requires-Dist: pydantic (>=1.8) Requires-Dist:
+requests (>=2.20,<2.30) Requires-Dist: requests-toolbelt Requires-Dist:
+retrying (>=1.3.3,<2.0.0) Requires-Dist: termcolor (>=1.1.0,<2.0.0) Requires-
+Dist: tqdm (>=4,<5) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0);
+python_version < "3.8" Project-URL: Documentation, https://docs.kolena.io
+Description-Content-Type: text/markdown
                                    [Kolena]
- [https://img.shields.io/pypi/v/kolena-client] [https://img.shields.io/pypi/l/
-   kolena-client] [https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-
-      6434c1] [https://img.shields.io/badge/docs-API%20Reference-6434c1]
+[https://img.shields.io/pypi/v/kolena] [https://img.shields.io/pypi/l/kolena]
+ [https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk] [https://
+ codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1]
+              [https://img.shields.io/badge/resource-docs-6434c1]
 --- [Kolena](https://www.kolena.io) is a comprehensive machine learning testing
 and debugging platform to surface hidden model behaviors and take the mystery
 out of model development. Kolena helps you: - Perform high-resolution model
 evaluation - Understand and track behavioral improvements and regressions -
 Meaningfully communicate model capabilities - Automate model testing and
-deployment workflows `kolena-client` is the Python client library for
-programmatic interaction with Kolena. ## Documentation Visit [docs.kolena.io]
-(https://docs.kolena.io/) for tutorial and usage documentation and the [API
-Reference](https://app.kolena.io/api/developer/docs/html/index.html) for
-detailed `kolena-client` typing and function documentation.
+deployment workflows This `kolena` package contains the Python client library
+for programmatic interaction with the Kolena ML testing platform. ##
+Documentation Visit [docs.kolena.io](https://docs.kolena.io/) for tutorial and
+usage documentation and the [API Reference](https://app.kolena.io/api/
+developer/docs/html/index.html) for detailed `kolena` typing and function
+documentation.
```

