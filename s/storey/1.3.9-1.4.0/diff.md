# Comparing `tmp/storey-1.3.9.tar.gz` & `tmp/storey-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-ww2czogr/storey-1.3.9.tar", last modified: Thu Feb 16 15:38:36 2023, max compression
+gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-2ly22aqa/storey-1.4.0.tar", last modified: Wed May 17 08:28:59 2023, max compression
```

## Comparing `storey-1.3.9.tar` & `storey-1.4.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-16 15:32:21.000000 storey-1.3.9/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-16 15:32:21.000000 storey-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-16 15:32:21.000000 storey-1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-16 15:38:36.000000 storey-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-02-16 15:32:21.000000 storey-1.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-16 15:32:21.000000 storey-1.3.9/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-16 15:32:21.000000 storey-1.3.9/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-02-16 15:32:21.000000 storey-1.3.9/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-02-16 15:32:21.000000 storey-1.3.9/integration/integration_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_aggregation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_filesystems_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    43061 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_flow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_kafka_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_redis_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-16 15:32:21.000000 storey-1.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-16 15:38:36.000000 storey-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-16 15:32:21.000000 storey-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-02-16 15:38:31.000000 storey-1.3.9/storey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-02-16 15:32:21.000000 storey-1.3.9/storey/aggregation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-02-16 15:32:21.000000 storey-1.3.9/storey/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-02-16 15:32:21.000000 storey-1.3.9/storey/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-02-16 15:32:21.000000 storey-1.3.9/storey/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-02-16 15:32:21.000000 storey-1.3.9/storey/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    50623 2023-02-16 15:32:21.000000 storey-1.3.9/storey/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-16 15:32:21.000000 storey-1.3.9/storey/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    26785 2023-02-16 15:32:21.000000 storey-1.3.9/storey/redis_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    41331 2023-02-16 15:32:21.000000 storey-1.3.9/storey/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-02-16 15:32:21.000000 storey-1.3.9/storey/sql_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    79845 2023-02-16 15:32:21.000000 storey-1.3.9/storey/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    50736 2023-02-16 15:32:21.000000 storey-1.3.9/storey/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-16 15:32:21.000000 storey-1.3.9/storey/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-02-16 15:32:21.000000 storey-1.3.9/storey/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-02-16 15:32:21.000000 storey-1.3.9/storey/windowed_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-16 15:32:21.000000 storey-1.3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_aggregate_by_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_aggregate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   117320 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_v3io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:28:59.000000 storey-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 08:23:55.000000 storey-1.4.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 08:23:55.000000 storey-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-17 08:23:55.000000 storey-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-17 08:28:59.000000 storey-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-17 08:23:55.000000 storey-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-17 08:23:55.000000 storey-1.4.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:28:59.000000 storey-1.4.0/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-17 08:23:55.000000 storey-1.4.0/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-05-17 08:23:55.000000 storey-1.4.0/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-17 08:23:55.000000 storey-1.4.0/integration/integration_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-05-17 08:23:55.000000 storey-1.4.0/integration/test_aggregation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-05-17 08:23:55.000000 storey-1.4.0/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-05-17 08:23:55.000000 storey-1.4.0/integration/test_filesystems_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-05-17 08:23:55.000000 storey-1.4.0/integration/test_flow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-17 08:23:55.000000 storey-1.4.0/integration/test_kafka_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-17 08:23:55.000000 storey-1.4.0/integration/test_redis_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-17 08:23:55.000000 storey-1.4.0/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-17 08:23:55.000000 storey-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 08:28:59.000000 storey-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-17 08:23:55.000000 storey-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:28:59.000000 storey-1.4.0/storey/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-17 08:28:52.000000 storey-1.4.0/storey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-17 08:23:55.000000 storey-1.4.0/storey/aggregation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-17 08:23:55.000000 storey-1.4.0/storey/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-17 08:23:55.000000 storey-1.4.0/storey/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-05-17 08:23:55.000000 storey-1.4.0/storey/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-05-17 08:23:55.000000 storey-1.4.0/storey/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50623 2023-05-17 08:23:55.000000 storey-1.4.0/storey/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-17 08:23:55.000000 storey-1.4.0/storey/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-05-17 08:23:55.000000 storey-1.4.0/storey/redis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37701 2023-05-17 08:23:55.000000 storey-1.4.0/storey/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-17 08:23:55.000000 storey-1.4.0/storey/sql_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:28:59.000000 storey-1.4.0/storey/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-17 08:23:55.000000 storey-1.4.0/storey/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-17 08:23:55.000000 storey-1.4.0/storey/steps/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-17 08:23:55.000000 storey-1.4.0/storey/steps/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-17 08:23:55.000000 storey-1.4.0/storey/steps/foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-17 08:23:55.000000 storey-1.4.0/storey/steps/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-17 08:23:55.000000 storey-1.4.0/storey/steps/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-05-17 08:23:55.000000 storey-1.4.0/storey/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50747 2023-05-17 08:23:55.000000 storey-1.4.0/storey/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:28:59.000000 storey-1.4.0/storey/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-17 08:23:55.000000 storey-1.4.0/storey/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-17 08:23:55.000000 storey-1.4.0/storey/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-05-17 08:23:55.000000 storey-1.4.0/storey/windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:28:59.000000 storey-1.4.0/storey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-17 08:28:59.000000 storey-1.4.0/storey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 08:28:59.000000 storey-1.4.0/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:28:59.000000 storey-1.4.0/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-17 08:28:59.000000 storey-1.4.0/storey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 08:28:59.000000 storey-1.4.0/storey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:28:59.000000 storey-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-17 08:23:55.000000 storey-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-05-17 08:23:55.000000 storey-1.4.0/tests/test_aggregate_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-17 08:23:55.000000 storey-1.4.0/tests/test_aggregate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124056 2023-05-17 08:23:55.000000 storey-1.4.0/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-05-17 08:23:55.000000 storey-1.4.0/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 08:23:55.000000 storey-1.4.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-17 08:23:55.000000 storey-1.4.0/tests/test_v3io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-17 08:23:55.000000 storey-1.4.0/tests/test_windowed_store.py
```

### Comparing `storey-1.3.9/LICENSE` & `storey-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/PKG-INFO` & `storey-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.3.9
+Version: 1.4.0
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.3.9/README.md` & `storey-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/integration/__init__.py` & `storey-1.4.0/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/integration/conftest.py` & `storey-1.4.0/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/integration/integration_test_utils.py` & `storey-1.4.0/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/integration/test_aggregation_integration.py` & `storey-1.4.0/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/integration/test_azure_filesystem_integration.py` & `storey-1.4.0/integration/test_azure_filesystem_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 
 @pytest.mark.skipif(not has_azure_credentials, reason="No azure credentials found")
 def test_csv_reader_from_azure(azure_create_csv):
     controller = build_flow(
         [
             CSVSource(
                 f"az:///{azure_create_csv}",
-                header=True,
                 storage_options=storage_options,
             ),
             FlatMap(lambda x: x),
             Map(lambda x: int(x)),
             Reduce(0, lambda acc, x: acc + x),
         ]
     ).run()
@@ -122,15 +121,14 @@
 
 @pytest.mark.skipif(not has_azure_credentials, reason="No azure credentials found")
 def test_csv_reader_from_azure_error_on_file_not_found():
     controller = build_flow(
         [
             CSVSource(
                 f'az:///{os.getenv("AZURE_BLOB_STORE")}/idontexist.csv',
-                header=True,
                 storage_options=storage_options,
             ),
         ]
     ).run()
 
     with pytest.raises(FileNotFoundError):
         controller.await_termination()
```

### Comparing `storey-1.3.9/integration/test_filesystems_integration.py` & `storey-1.4.0/integration/test_filesystems_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import asyncio
 import datetime
-import os
 import random as rand
 import sys
 import uuid
 
 import aiohttp
 import pandas as pd
 import pytest
@@ -31,15 +30,14 @@
     CSVTarget,
     DataframeSource,
     FlatMap,
     Map,
     ParquetSource,
     ParquetTarget,
     Reduce,
-    ReduceToDataFrame,
     SyncEmitSource,
     build_flow,
 )
 from storey.dtypes import V3ioError
 from storey.utils import get_remaining_path
 
 
@@ -101,34 +99,34 @@
     finally:
         await client_session.close()
 
 
 def test_csv_reader_from_v3io(v3io_create_csv):
     controller = build_flow(
         [
-            CSVSource(f"v3io:///{v3io_create_csv}", header=True),
+            CSVSource(f"v3io:///{v3io_create_csv}"),
             FlatMap(lambda x: x),
             Map(lambda x: int(x)),
             Reduce(0, lambda acc, x: acc + x),
         ]
     ).run()
 
     termination_result = controller.await_termination()
     assert termination_result == 495
 
 
 def test_csv_reader_from_v3io_error_on_file_not_found():
     controller = build_flow(
         [
-            CSVSource("v3io:///bigdatra/tests/idontexist.csv", header=True),
+            CSVSource("v3io:///bigdata/tests/idontexist.csv"),
         ]
-    ).run()
+    )
 
     with pytest.raises(FileNotFoundError):
-        controller.await_termination()
+        controller.run()
 
 
 async def async_test_write_csv_to_v3io(v3io_teardown_csv):
     controller = build_flow(
         [
             AsyncEmitSource(),
             CSVTarget(f"v3io:///{v3io_teardown_csv}", columns=["n", "n*10"], header=True),
@@ -418,29 +416,29 @@
             ["hello", pd.Timestamp("2019-01-26 14:52:37")],
             ["world", pd.Timestamp("2020-05-11 13:52:37")],
         ],
         columns=columns,
     )
     df.set_index("my_string")
 
-    out_file = f"v3io:///{setup_teardown_test.table_name}/before_after_non_partioned/"
+    out_file = f"v3io:///{setup_teardown_test.table_name}/before_after_non_partitioned/"
     controller = build_flow(
         [
             DataframeSource(df),
             ParquetTarget(out_file, columns=columns, partition_cols=[]),
         ]
     ).run()
     controller.await_termination()
 
     before = pd.Timestamp("2019-12-01 00:00:00")
     after = pd.Timestamp("2019-01-01 23:59:59.999999")
 
     controller = build_flow(
         [
-            ParquetSource(out_file, end_filter=before, start_filter=after, filter_column="my_time"),
+            ParquetSource(out_file, start_filter=after, end_filter=before, filter_column="my_time"),
             Reduce([], append_and_return),
         ]
     ).run()
     read_back_result = controller.await_termination()
     expected = [{"my_string": "hello", "my_time": pd.Timestamp("2019-01-26 14:52:37")}]
 
     assert read_back_result == expected, f"{read_back_result}\n!=\n{expected}"
@@ -504,31 +502,31 @@
 
     controller.await_termination()
 
     controller = build_flow(
         [
             ParquetSource(
                 out_file,
-                end_filter=high_limit,
                 start_filter=middle_limit,
+                end_filter=high_limit,
                 filter_column="datetime",
             ),
             Reduce([], append_and_return),
         ]
     ).run()
     read_back_result = controller.await_termination()
     print("expecting " + str(10 - number_below_middle_limit) + " to be above middle limit")
     assert (len(read_back_result)) == 10 - number_below_middle_limit
 
     controller = build_flow(
         [
             ParquetSource(
                 out_file,
-                end_filter=middle_limit,
                 start_filter=low_limit,
+                end_filter=middle_limit,
                 filter_column="datetime",
             ),
             Reduce([], append_and_return),
         ]
     ).run()
     read_back_result = controller.await_termination()
     print("expecting " + str(number_below_middle_limit) + " to be below middle limit")
@@ -567,16 +565,16 @@
     before = pd.Timestamp("2020-12-31 14:00:00")
     after = pd.Timestamp("2019-07-01 00:00:00")
 
     controller = build_flow(
         [
             ParquetSource(
                 out_file,
-                end_filter=before,
                 start_filter=after,
+                end_filter=before,
                 filter_column="my_time",
                 columns=columns,
             ),
             Reduce([], append_and_return),
         ]
     ).run()
     read_back_result = controller.await_termination()
@@ -665,84 +663,12 @@
             "my_city": "ramat gan",
         },
     ]
 
     assert read_back_result == expected, f"{read_back_result}\n!=\n{expected}"
 
 
-def test_filter_by_time_non_partioned(setup_teardown_test):
-    columns = ["my_string", "my_time", "my_city"]
-
-    df = pd.DataFrame(
-        [
-            ["dina", pd.Timestamp("2019-07-01 00:00:00"), "tel aviv"],
-            ["uri", pd.Timestamp("2018-12-30 09:00:00"), "tel aviv"],
-            ["katya", pd.Timestamp("2020-12-31 14:00:00"), "hod hasharon"],
-        ],
-        columns=columns,
-    )
-    df.set_index("my_string")
-    path = "/tmp/test_filter_by_time_non_partioned.parquet"
-    df.to_parquet(path)
-    start = pd.Timestamp("2019-07-01 00:00:00")
-    end = pd.Timestamp("2020-12-31 14:00:00")
-
-    controller = build_flow(
-        [
-            ParquetSource(path, end_filter=end, start_filter=start, filter_column="my_time"),
-            Reduce([], append_and_return),
-        ]
-    ).run()
-
-    read_back_result = controller.await_termination()
-
-    expected = [
-        {
-            "my_string": "katya",
-            "my_time": pd.Timestamp("2020-12-31 14:00:00"),
-            "my_city": "hod hasharon",
-        }
-    ]
-
-    try:
-        assert read_back_result == expected, f"{read_back_result}\n!=\n{expected}"
-    finally:
-        os.remove(path)
-
-
-def test_empty_filter_result(setup_teardown_test):
-    columns = ["my_string", "my_time", "my_city"]
-
-    df = pd.DataFrame(
-        [
-            ["dina", pd.Timestamp("2019-07-01 00:00:00"), "tel aviv"],
-            ["uri", pd.Timestamp("2018-12-30 09:00:00"), "tel aviv"],
-            ["katya", pd.Timestamp("2020-12-31 14:00:00"), "hod hasharon"],
-        ],
-        columns=columns,
-    )
-    df.set_index("my_string")
-    path = "/tmp/test_filter_by_time_non_partioned.parquet"
-    df.to_parquet(path)
-    start = pd.Timestamp("2022-07-01 00:00:00")
-    end = pd.Timestamp("2022-12-31 14:00:00")
-
-    controller = build_flow(
-        [
-            ParquetSource(path, end_filter=end, start_filter=start, filter_column="my_time"),
-            ReduceToDataFrame(index=["my_string"], insert_key_column_as=["my_string"]),
-        ]
-    ).run()
-
-    read_back_result = controller.await_termination()
-
-    try:
-        pd.testing.assert_frame_equal(read_back_result, pd.DataFrame({}))
-    finally:
-        os.remove(path)
-
-
 def test_get_path_utils():
     url = "wasbs://mycontainer@myaccount.blob.core.windows.net/path/to/object.csv"
     schema, path = get_remaining_path(url)
     assert path == "mycontainer/path/to/object.csv"
     assert schema == "wasbs"
```

### Comparing `storey-1.3.9/integration/test_flow_integration.py` & `storey-1.4.0/integration/test_flow_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,29 +131,21 @@
     metadata = db.MetaData()
     sql_table = db.Table(
         table_name,
         metadata,
         autoload=True,
         autoload_with=engine,
     )
-
-    where_statement = ""
     if isinstance(key, str):
         key = key.split(".")
-    if isinstance(key, list):
-        for i in range(len(key_name)):
-            if i != 0:
-                where_statement += " and "
-            if sql_table.columns[key_name[i]].type.python_type == str:
-                where_statement += f'{key_name[i]}="{key[i]}"'
-            else:
-                where_statement += f"{key_name[i]}={key[i]}"
-    query = f"SELECT * FROM {sql_table} where ({where_statement})"
+    select_object = db.select(sql_table).where(
+        db.and_(getattr(sql_table.c, key_name[i]) == key[i] for i in range(len(key_name)))
+    )
     with engine.connect() as conn:
-        return pd.read_sql(query, con=conn, parse_dates=time_fields).to_dict(orient="records")[0]
+        return pd.read_sql(select_object, con=conn, parse_dates=time_fields).to_dict(orient="records")[0]
 
 
 def get_key_all_attrs_test_helper(
     setup_teardown_test: ContextForTests,
     key: Union[str, List[str]],
     key_name: Union[str, List[str]] = None,
     time_fields: List[str] = None,
@@ -692,20 +684,20 @@
     expected = [{"col1": 9, "age": 1}]
     controller.terminate()
     termination_result = controller.await_termination()
     assert termination_result == expected
 
 
 def test_write_table_specific_columns(setup_teardown_test):
-    keys = ["my_key"]
+    keys = ["index"]
     time_fields = ["sometime", "first_activity", "last_event"]
     table = _get_table(
         setup_teardown_test,
         {
-            "my_key": str,
+            "index": str,
             "color": str,
             "age": int,
             "iss": bool,
             "sometime": pd.Timestamp,
             "first_activity": pd.Timestamp,
             "last_event": pd.Timestamp,
             "total_activities": int,
@@ -739,15 +731,15 @@
         return event, state
 
     controller = build_flow(
         [
             SyncEmitSource(),
             MapWithState(table, enrich, group_by_key=True),
             DropColumns("sometime"),
-            NoSqlTarget(table, columns=["twice_total_activities", "my_key=$key"]),
+            NoSqlTarget(table, columns=["twice_total_activities", "index=$key"]),
             Reduce([], lambda acc, x: append_return(acc, x)),
         ]
     ).run()
 
     items_in_ingest_batch = 10
     for i in range(items_in_ingest_batch):
         data = {"col1": i, "sometime": test_base_time + timedelta(minutes=25 * i)}
@@ -829,29 +821,29 @@
         "sometime": test_base_time,
         "first_activity": test_base_time,
         "last_event": test_base_time + timedelta(minutes=25 * (items_in_ingest_batch - 1)),
         "total_activities": 10,
         "twice_total_activities": 20,
         "min": 1,
         "Avg": 3,
-        "my_key": "tal",
+        "index": "tal",
     }
 
     actual_cache = get_key_all_attrs_test_helper(setup_teardown_test, "tal", keys, time_fields)
     assert expected_cache == actual_cache
 
     # delete cache - testing load__by_key from driver
     table = Table(setup_teardown_test.table_name, table._storage)
 
     controller = build_flow(
         [
             SyncEmitSource(),
             MapWithState(table, enrich, group_by_key=True),
             DropColumns("sometime"),
-            NoSqlTarget(table, columns=["twice_total_activities", "my_key=$key"]),
+            NoSqlTarget(table, columns=["twice_total_activities", "index=$key"]),
             Reduce([], lambda acc, x: append_return(acc, x)),
         ]
     ).run()
 
     items_in_ingest_batch = 10
     for i in range(items_in_ingest_batch):
         data = {"col1": i, "sometime": test_base_time + timedelta(minutes=25 * i)}
@@ -1210,15 +1202,15 @@
 
 
 def test_write_multiple_keys_from_csv(setup_teardown_test):
     keys = ["n1", "n2"]
     table = _get_table(setup_teardown_test, {"n1": int, "n2": int, "n3": int}, keys)
     controller = build_flow(
         [
-            CSVSource("tests/test.csv", header=True, key_field=["n1", "n2"], build_dict=True),
+            CSVSource("tests/test.csv", key_field=["n1", "n2"], build_dict=True),
             NoSqlTarget(table),
         ]
     ).run()
     controller.await_termination()
 
     expected = {"n1": 1, "n2": 2, "n3": 3}
     actual = get_key_all_attrs_test_helper(setup_teardown_test, "1.2", ["n1", "n2"])
```

### Comparing `storey-1.3.9/integration/test_kafka_integration.py` & `storey-1.4.0/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/integration/test_redis_specific.py` & `storey-1.4.0/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/integration/test_s3_filesystem_integration.py` & `storey-1.4.0/integration/test_s3_filesystem_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,30 +111,30 @@
     s3_fs.rm(path, True)
 
 
 @pytest.mark.skipif(not has_s3_credentials, reason="No s3 credentials found")
 def test_csv_reader_from_s3(s3_create_csv):
     controller = build_flow(
         [
-            CSVSource(f"s3://{s3_create_csv}", header=True),
+            CSVSource(f"s3://{s3_create_csv}"),
             FlatMap(lambda x: x),
             Map(lambda x: int(x)),
             Reduce(0, lambda acc, x: acc + x),
         ]
     ).run()
 
     termination_result = controller.await_termination()
     assert termination_result == 495
 
 
 @pytest.mark.skipif(not has_s3_credentials, reason="No s3 credentials found")
 def test_csv_reader_from_s3_error_on_file_not_found():
     controller = build_flow(
         [
-            CSVSource(f's3://{os.getenv("AWS_BUCKET")}/idontexist.csv', header=True),
+            CSVSource(f's3://{os.getenv("AWS_BUCKET")}/idontexist.csv'),
         ]
     ).run()
 
     with pytest.raises(FileNotFoundError):
         controller.await_termination()
```

### Comparing `storey-1.3.9/setup.py` & `storey-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def version():
     with open("storey/__init__.py") as fp:
         for line in fp:
             if line.startswith("__version__"):
                 _, version = line.split("=")
-                return version.replace("'", "").strip()
+                return version.replace('"', "").strip()
 
 
 def load_deps(file_name):
     """Load dependencies from requirements file"""
     deps = []
     with open(file_name) as fp:
         for line in fp:
```

### Comparing `storey-1.3.9/storey/__init__.py` & `storey-1.4.0/storey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = '1.3.9'
+__version__ = "1.4.0"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.3.9/storey/aggregation_utils.py` & `storey-1.4.0/storey/aggregation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,7 +136,11 @@
                     raw_aggregates[dependant_aggr] = True
 
     return raw_aggregates
 
 
 def get_all_raw_aggregates(aggregates):
     return set(get_all_raw_aggregates_with_hidden(aggregates).keys())
+
+
+def is_aggregation_name(name: str):
+    return name in _all_aggregates_by_name
```

### Comparing `storey-1.3.9/storey/aggregations.py` & `storey-1.4.0/storey/aggregations.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import re
 import time
 from datetime import datetime
 from typing import Callable, Dict, List, Optional, Union
 
 import pandas as pd
 
+from .aggregation_utils import is_aggregation_name
 from .dtypes import (
     EmitAfterMaxEvent,
     EmitAfterPeriod,
     EmitAfterWindow,
     EmitEveryEvent,
     EmitPolicy,
     FieldAggregator,
@@ -305,22 +306,21 @@
     """
     Query features by name
 
     :param features: List of features to get.
     :param table: A Table object or name for persistence of aggregations.
         If a table name is provided, it will be looked up in the context object passed in kwargs.
     :param key_field: Key field to query by, accepts either a string representing the key field or a key
-        extracting function. Defaults to the key in the event's metadata. (Optional)
+        extracting function. Defaults to the key in the event's metadata. Can be list of keys (Optional)
     :param time_field: Time field to query by, accepts either a string representing the time field or a time
         extracting function. Defaults to the processing time in the event's metadata. (Optional)
-     Defaults to the key in the event's metadata. (Optional). Can be list of keys
     :param augmentation_fn: Function that augments the features into the event's body.
         Defaults to updating a dict. (Optional)
     :param aliases: Dictionary specifying aliases for enriched or aggregate columns, of the
-     format `{'col_name': 'new_col_name'}`. (Optional)
+        format `{'col_name': 'new_col_name'}`. (Optional)
     :param options: Enum flags specifying query options. (Optional)
     """
 
     def __init__(
         self,
         features: List[str],
         table: Union[Table, str],
@@ -335,15 +335,16 @@
         self._enrich_cols = []
         resolved_aggrs = {}
         if isinstance(table, str):
             if "context" not in kwargs:
                 raise TypeError("Table can not be string if no context was provided to the step")
             table = kwargs["context"].get_table(table)
         for feature in features:
-            if table.supports_aggregations() and re.match(r".*_[a-z]+_[0-9]+[smhd]$", feature):
+            match = re.match(r".*_([a-z]+)_[0-9]+[smhd]$", feature) if table.supports_aggregations() else None
+            if match and is_aggregation_name(match.group(1)):
                 name, window = feature.rsplit("_", 1)
                 if name in resolved_aggrs:
                     resolved_aggrs[name].append(window)
                 else:
                     resolved_aggrs[name] = [window]
             else:
                 self._enrich_cols.append(feature)
```

### Comparing `storey-1.3.9/storey/dataframe.py` & `storey-1.4.0/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/drivers.py` & `storey-1.4.0/storey/drivers.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/dtypes.py` & `storey-1.4.0/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/flow.py` & `storey-1.4.0/storey/flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/queue.py` & `storey-1.4.0/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/redis_driver.py` & `storey-1.4.0/storey/redis_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 
 class RedisDriver(NeedsRedisAccess, Driver):
     REDIS_TIMEOUT = 5  # Seconds
     REDIS_WATCH_INTERVAL = 1  # Seconds
     DATETIME_FIELD_PREFIX = "_dt:"
     TIMEDELTA_FIELD_PREFIX = "_td:"
     DEFAULT_KEY_PREFIX = "storey:"
-    AGGREGATION_ATTRIBUTE_PREFIX = "aggr_"
+    AGGREGATION_ATTRIBUTE_PREFIX = "moving_windows"
     AGGREGATION_TIME_ATTRIBUTE_PREFIX = "_"
-    AGGREGATION_PREFIXES = (AGGREGATION_ATTRIBUTE_PREFIX, AGGREGATION_TIME_ATTRIBUTE_PREFIX)
+    AGGREGATION_PREFIXES = AGGREGATION_TIME_ATTRIBUTE_PREFIX
 
     def __init__(
         self,
         redis_client: Optional[Union[redis.Redis, redis.cluster.RedisCluster]] = None,
         key_prefix: str = None,
         redis_url: Optional[str] = None,
         use_parallel_operations: bool = True,  # unused
@@ -251,29 +251,40 @@
                     )
                 else:
                     additional_data_lua_script = (
                         f'{additional_data_lua_script}redis.call("HDEL",additional_data_key, "{name}");\n'
                     )
 
         lua_script = additional_data_lua_script
+        list_attribute_key_aggr = self._list_key(redis_key_prefix, RedisDriver.AGGREGATION_ATTRIBUTE_PREFIX)
 
         if aggregation_element:
             times_updates = {}
             new_cached_times = {}
             initialized_attributes = {}
             if partitioned_by_key:
                 condition_expression = aggregation_element.storage_specific_cache.get(self._mtime_name, None)
             lua_tonum_function = (
                 'local function tonum(str) if str == "inf" then return math.huge elseif str == "-inf" then '
-                'return -math.huge elseif str == "nan" then return 0/0 end return tonumber(str) end'
+                'return -math.huge elseif str == "nan" then return 0/0 end return tonumber(str) end;\n'
+            )
+            lua_strToArr_funct = (
+                "local function strToArr(input)\n"
+                "    local result = {}\n"
+                "    if input == nil or input == false then return {} end\n"
+                '    for value in string.gmatch(input, "([^,]+)") do\n'
+                "        table.insert(result, value)\n"
+                "    end\n"
+                "    return result\n"
+                "end\n"
             )
             lua_script = (
-                f'{lua_script}local len;local redis_key_prefix="{redis_key_prefix}";local list_attribute_key;\n'
+                f"{lua_script}local old_value;local attr_name;\n" f'local aggr_key="{list_attribute_key_aggr}";\n'
             )
-            lua_script = f"{lua_script}{lua_tonum_function}\n"
+            lua_script = f"{lua_script}{lua_tonum_function}{lua_strToArr_funct}\n"
             for name, bucket in aggregation_element.aggregation_buckets.items():
                 # Only save raw aggregates, not virtual
                 if bucket.should_persist:
                     # In case we have pending data that spreads over more than 2 windows, discard the old ones.
                     pending_updates[name] = self._discard_old_pending_items(
                         bucket.get_and_flush_pending(), bucket.max_window_millis
                     )
@@ -288,69 +299,67 @@
 
                         cached_time = bucket.storage_specific_cache.get(array_time_attribute_key, -1)
 
                         expected_time = int(bucket_start_time / bucket.max_window_millis) * bucket.max_window_millis
                         expected_time_expr = self._convert_python_obj_to_lua_value(
                             datetime.fromtimestamp(expected_time / 1000)
                         )
-                        index_to_update = int((bucket_start_time - expected_time) / bucket.period_millis)
+                        lua_index_to_update = 1 + int((bucket_start_time - expected_time) / bucket.period_millis)
 
                         for (
                             aggregation,
                             aggregation_value,
                         ) in aggregation_values.items():
-                            list_attribute_name = (
-                                f"{RedisDriver.AGGREGATION_ATTRIBUTE_PREFIX}{name}_{aggregation}_{feature_attr}"
-                            )
-                            list_attribute_key = self._list_key(redis_key_prefix, list_attribute_name)
-                            if list_attribute_key not in redis_keys_involved:
-                                redis_keys_involved.append(list_attribute_key)
-                            lua_script = f'{lua_script}list_attribute_key="{list_attribute_key}";\n'
+                            list_attribute_name = f"{name}_{aggregation}_{feature_attr}"
+                            if list_attribute_key_aggr not in redis_keys_involved:
+                                redis_keys_involved.append(list_attribute_key_aggr)
+                            lua_script = f'{lua_script}attr_name="{list_attribute_name}";\n'
 
                             if cached_time < expected_time:
+                                list_attribute_key = self._list_key(redis_key_prefix, list_attribute_name)
                                 if not initialized_attributes.get(list_attribute_key, -1) == expected_time:
                                     initialized_attributes[list_attribute_key] = expected_time
                                     lua_script = (
                                         f'{lua_script}local t=redis.call("GET","{array_time_attribute_key}");\n'
                                         f'if (type(t)~="boolean" and (tonumber(t) < {expected_time})) then '
-                                        f'redis.call("DEL",list_attribute_key); end;\n'
+                                        f'redis.call("HDEL",aggr_key, attr_name); end;\n'
                                     )
                                     default_value = self._convert_python_obj_to_redis_value(
                                         aggregation_value.default_value
                                     )
                                     lua_script = (
-                                        f'{lua_script}len=redis.call("LLEN",list_attribute_key);\n'
-                                        f"for i=1,({bucket.total_number_of_buckets}-len) do "
-                                        f'redis.call("RPUSH",list_attribute_key,{default_value}) end;\n'
+                                        f'{lua_script}local curr_agg=redis.call("HGET",aggr_key, attr_name)\n'
+                                        "local arr=strToArr(curr_agg);\n"
+                                        f"local org_arr_len=#arr\n"
+                                        f"for i=1,({bucket.total_number_of_buckets}-org_arr_len) \
+                                            do arr[#arr+1]={default_value};end;\n"
+                                        f'if org_arr_len ~= #arr then redis.call("HSET", aggr_key, attr_name,\
+                                            table.concat(arr, ",")) end;\n'
                                     )
                                 if array_time_attribute_key not in times_updates:
                                     times_updates[array_time_attribute_key] = expected_time_expr
                                 new_cached_times[name] = (
                                     array_time_attribute_key,
                                     expected_time,
                                 )
 
                             # Updating the specific cells
                             if cached_time <= expected_time:
-                                lua_script = (
-                                    f"{lua_script}local old_value=redis.call("
-                                    f'"LINDEX",list_attribute_key,{index_to_update});\n'
-                                )
-                                lua_script = f"{lua_script}old_value=tonum(old_value)\n"
                                 new_value_expression = aggregation_value.aggregate_lua_script(
                                     "old_value", aggregation_value.value
                                 )
                                 lua_script = (
-                                    f'{lua_script}redis.call("LSET", list_attribute_key, {index_to_update}, '
-                                    f"{new_value_expression});\n"
+                                    f'{lua_script}arr=strToArr(redis.call("HGET",aggr_key, attr_name))\n'
+                                    f"old_value=tonum(arr[{lua_index_to_update}]);\n"
+                                    f'arr[{lua_index_to_update}]=string.format("%.17f",{new_value_expression});\n'
+                                    'redis.call("HSET", aggr_key, attr_name, table.concat(arr, ","))\n'
                                 )
 
                         redis_keys_involved.append(array_time_attribute_key)
                         lua_script = f'{lua_script}redis.call("SET","{array_time_attribute_key}",{expected_time}); \n'
-
         return lua_script, condition_expression, pending_updates, redis_keys_involved
 
     async def _save_key(self, container, table_path, key, aggr_item, partitioned_by_key, additional_data):
         redis_key_prefix = self._make_key(container, table_path, key)
         (
             update_expression,
             mtime_condition,
@@ -392,14 +401,15 @@
                 redis_keys_involved,
             ) = self._build_feature_store_lua_update_script(redis_key_prefix, aggr_item, False, additional_data)
             update_expression = (
                 f"{update_expression}redis.call("
                 f'"HSET","{redis_key_prefix}","{self._mtime_name}",{current_time});return 1;'
             )
             redis_keys_involved.append(redis_key_prefix)
+
             update_ok = await RedisDriver.asyncify(self.redis.eval)(
                 update_expression, len(redis_keys_involved), *redis_keys_involved
             )
             if update_ok and aggr_item:
                 await self._fetch_state_by_key(aggr_item, container, table_path, key)
 
     async def _get_all_fields(self, redis_key: str):
@@ -477,29 +487,32 @@
         }
         """
         redis_key_prefix = self._make_key(container, table_path, key)
         additional_data = await self._get_all_fields(self._static_data_key(redis_key_prefix))
         aggregations = {}
         # Aggregation Redis keys start with the Redis key prefix for this Storey container, table
         # path, and "key," followed by ":aggr_"
+        redis_key_prefix = self._make_key(container, table_path, key)
         aggr_key_prefix = f"{redis_key_prefix}:{RedisDriver.AGGREGATION_ATTRIBUTE_PREFIX}"
-        # We can't use `async for` here...
-        for aggr_key in self.redis.scan_iter(f"{aggr_key_prefix}*"):
+        all_aggr_keys = self.redis.hkeys(aggr_key_prefix)
+        for aggr_key in all_aggr_keys:
             aggr_key = RedisDriver.convert_to_str(aggr_key)
-            value = await RedisDriver.asyncify(self.redis.lrange)(aggr_key, 0, -1)
+            value = await RedisDriver.asyncify(self.redis.hget)(aggr_key_prefix, aggr_key)
             # Build an attribute for this aggregation in the format that Storey
             # expects to receive from this method. The feature and aggregation
             # name are embedded in the Redis key. Also, drop the "_a" or "_b"
             # portion of the key, which is "the relevant attribute out of the 2
             # feature attributes," according to comments in the V3IO driver.
-            feature_and_aggr_name = aggr_key[len(aggr_key_prefix) : -2]
+            value = RedisDriver.convert_to_str(value)
+            value = value.split(",")
+            feature_and_aggr_name = aggr_key[:-2]
 
             # To get the associated time, we need the aggregation name and the relevant
             # attribute (a or b), so we take a second form of the string for that purpose.
-            aggr_name_with_relevant_attribute = aggr_key[len(aggr_key_prefix) :]
+            aggr_name_with_relevant_attribute = aggr_key
             associated_time_attr, time_in_millis = await self._get_associated_time_attr(
                 redis_key_prefix, aggr_name_with_relevant_attribute
             )
             if feature_and_aggr_name not in aggregations:
                 aggregations[feature_and_aggr_name] = {}
             aggregations[feature_and_aggr_name][time_in_millis] = [
                 float(RedisDriver.convert_redis_value_to_python_obj(v)) for v in value
@@ -516,28 +529,31 @@
         key = str(key)
         # Aggregation Redis keys start with the Redis key prefix for this Storey container, table
         # path, and "key," followed by ":aggr_"
         aggregations = {}
 
         redis_key_prefix = self._make_key(container, table_path, key)
         aggr_key_prefix = f"{redis_key_prefix}:{RedisDriver.AGGREGATION_ATTRIBUTE_PREFIX}"
-        # We can't use `async for` here...
-        for aggr_key in self.redis.scan_iter(f"{aggr_key_prefix}*"):
+        all_aggr_keys = self.redis.hkeys(aggr_key_prefix)
+        for aggr_key in all_aggr_keys:
             aggr_key = RedisDriver.convert_to_str(aggr_key)
-            value = await RedisDriver.asyncify(self.redis.lrange)(aggr_key, 0, -1)
+            value = await RedisDriver.asyncify(self.redis.hget)(aggr_key_prefix, aggr_key)
             # Build an attribute for this aggregation in the format that Storey
             # expects to receive from this method. The feature and aggregation
             # name are embedded in the Redis key. Also, drop the "_a" or "_b"
             # portion of the key, which is "the relevant attribute out of the 2
             # feature attributes," according to comments in the V3IO driver.
-            feature_and_aggr_name = aggr_key[len(aggr_key_prefix) : -2]
+            value = RedisDriver.convert_to_str(value)
+            value = value.split(",")
+
+            feature_and_aggr_name = aggr_key[:-2]
 
             # To get the associated time, we need the aggregation name and the relevant
             # attribute (a or b), so we take a second form of the string for that purpose.
-            aggr_name_with_relevant_attribute = aggr_key[len(aggr_key_prefix) :]
+            aggr_name_with_relevant_attribute = aggr_key
             associated_time_attr, time_in_millis = await self._get_associated_time_attr(
                 redis_key_prefix, aggr_name_with_relevant_attribute
             )
             if feature_and_aggr_name not in aggregations:
                 aggregations[feature_and_aggr_name] = {}
             aggregations[feature_and_aggr_name][time_in_millis] = [
                 float(RedisDriver.convert_redis_value_to_python_obj(v)) for v in value
```

### Comparing `storey-1.3.9/storey/sources.py` & `storey-1.4.0/storey/sources.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import asyncio
 import copy
-import csv
-import math
 import queue
 import threading
 import uuid
 import warnings
 from datetime import datetime, timezone
 from typing import Callable, Coroutine, Iterable, List, Optional, Union
 
 import pandas
+import pandas as pd
+import pyarrow
 import pytz
 
 from .dtypes import Event, _termination_obj
 from .flow import Complete, Flow
 from .utils import find_filters, find_partitions, url_to_file_system
 
 
@@ -176,19 +176,18 @@
         return_awaitable_result: Optional[bool] = None,
         expected_number_of_results: Optional[int] = None,
     ):
         """Emits an event into the associated flow.
 
         :param element: The event data, or payload. To set metadata as well, pass an Event object.
         :param key: The event key(s) (optional) #add to async
-        :param return_awaitable_result: Deprecated! An awaitable result object will be returned if a Complete step
+        :param return_awaitable_result: Deprecated. An awaitable result object will be returned if a Complete step
             appears in the flow.
         :param expected_number_of_results: Number of times the event will have to pass through a Complete step to be
-            completed (for graph
-        flows).
+            completed (for graph flows).
 
         :returns: AsyncAwaitableResult if a Complete appears in the flow. None otherwise.
         """
         if return_awaitable_result is not None:
             warnings.warn(
                 "return_awaitable_result is deprecated. An awaitable result object will be returned if a Complete step "
                 "appears in the flow.",
@@ -411,15 +410,15 @@
     ) -> object:
         """Emits an event into the associated flow.
 
         :param element: The event data, or payload. To set metadata as well, pass an Event object.
         :param key: The event key(s) (optional)
         :param await_result: Deprecated. Will await a result if a Complete step appears in the flow.
         :param expected_number_of_results: Number of times the event will have to pass through a Complete step to be
-        completed (for graph flows).
+            completed (for graph flows).
 
         :returns: The result received from the flow if a Complete step appears in the flow. None otherwise.
         """
         if await_result is not None:
             warnings.warn(
                 "await_result is deprecated. An awaitable result object will be returned if a Complete step appears "
                 "in the flow.",
@@ -591,341 +590,228 @@
         return FlowAwaiter(raise_error_or_return_termination_result)
 
     async def run_async(self):
         self._closeables = super().run()
         return await self._run_loop()
 
 
-class CSVSource(_IterableSource, WithUUID):
+class DataframeSource(_IterableSource, WithUUID):
+    """Use pandas dataframe as input source for a flow.
+
+    :param dfs: A pandas dataframe, or dataframes, to be used as input source for the flow.
+    :param key_field: column to be used as key for events. can be list of columns
+    :param id_field: column to be used as ID for events.
+
+    for additional params, see documentation of  :class:`~storey.flow.Flow`
+    """
+
+    def __init__(
+        self,
+        dfs: Union[pandas.DataFrame, Iterable[pandas.DataFrame]],
+        key_field: Optional[Union[str, List[str]]] = None,
+        id_field: Optional[str] = None,
+        **kwargs,
+    ):
+        if key_field is not None:
+            kwargs["key_field"] = key_field
+        if id_field is not None:
+            kwargs["id_field"] = id_field
+        _IterableSource.__init__(self, **kwargs)
+        WithUUID.__init__(self)
+        #  in order to raise exception also for key_field=0
+        if key_field is not None:
+            key_fields = [key_field] if not isinstance(key_field, list) else key_field
+            if any([not isinstance(single_key_field, str) for single_key_field in key_fields]):
+                raise ValueError("key_field must be a string or list of strings")
+        if id_field and not isinstance(id_field, str):
+            raise ValueError("id_field must be a string")
+        self._key_field = key_field
+        self._id_field = id_field
+        if isinstance(dfs, pandas.DataFrame):
+            dfs = [dfs]
+        if dfs:
+            for df in dfs:
+                self._validate_fields(df)
+        self._dfs = dfs
+
+    def _get_keys(self, body: dict):
+        keys = []
+        if self._key_field:
+            if isinstance(self._key_field, list):
+                for key_field in self._key_field:
+                    single_key = body[key_field]
+                    keys.append(single_key)
+            else:
+                keys.append(body[self._key_field])
+        return keys
+
+    async def _run_loop(self):
+        for df in self._dfs:
+            columns = list(df.columns)
+            is_df_index_nonempty = not df.index.empty and not (len(df.index.names) == 1 and df.index.names[0] is None)
+            if is_df_index_nonempty:
+                df = df.reset_index(drop=False)
+            for body in df.to_dict("records"):
+                keys = self._get_keys(body)
+                key_fields = self._key_field if isinstance(self._key_field, list) else [self._key_field]
+                none_keys = [key for key, value in zip(key_fields, keys) if pd.isna(value)]
+                if none_keys:
+                    if self.context:
+                        self.context.logger.error(
+                            f"Encountered null values in the following key fields:"
+                            f" {', '.join(none_keys)}, in line: {body}."
+                        )
+                else:
+                    if self._id_field:
+                        line_id = body[self._id_field]
+                    else:
+                        line_id = self._get_uuid()
+                    element = self._get_element(body, columns)
+                    keys = keys[0] if len(keys) == 1 else (None if not keys else keys)
+                    event = Event(element, keys, id=line_id)
+                    await self._do_downstream(event)
+        return await self._do_downstream(_termination_obj)
+
+    def _validate_fields(self, df, path=""):
+        path_message = f" File path: {path}." if path else ""
+        df = df.reset_index()
+        if self._key_field:
+            key_fields = [self._key_field] if not isinstance(self._key_field, list) else self._key_field
+            missing_keys = [key_field for key_field in key_fields if key_field not in df.columns]
+            if missing_keys:
+                if len(missing_keys) > 1:
+                    missing_keys_message = f"key columns {missing_keys} are"
+                else:
+                    missing_keys_message = f"key column '{missing_keys[0]}' is"
+                raise ValueError(f"{missing_keys_message} missing from dataframe.{path_message}")
+
+        if self._id_field and self._id_field not in df.columns:
+            raise ValueError(f"id column '{self._id_field}' is missing from dataframe.{path_message}")
+
+    def _get_element(self, body: dict, columns):
+        return body
+
+
+class CSVSource(DataframeSource):
     """
     Reads CSV files as input source for a flow.
 
     :parameter paths: paths to CSV files
-    :parameter header: whether CSV files have a header or not. Defaults to False.
+    :parameter header: Deprecated. whether CSV files have a header or not. Defaults to False.
     :parameter build_dict: whether to format each record produced from the input file as a dictionary (as opposed to a
         list). Default to False.
     :parameter key_field: the CSV field to be used as the key for events. May be an int (field index) or string (field
         name) if with_header is True. Defaults to None (no key). Can be a list of keys
     :parameter time_field: the CSV field to be parsed as the timestamp for events. May be an int (field index) or string
         (field name) if with_header is True. Defaults to None (no timestamp field).
     :parameter timestamp_format: timestamp format as defined in datetime.strptime(). Default to ISO-8601 as defined in
         datetime.fromisoformat().
     :parameter id_field: the CSV field to be used as the ID for events. May be an int (field index) or string (field
         name) if with_header is True. Defaults to None (random ID will be generated per event).
-    :parameter type_inference: Whether to infer data types from the data (when True), or read all fields in as strings
-        (when False). Defaults to True.
+    :parameter type_inference: Deprecated. Whether to infer data types from the data (when True), or read all fields in
+     as strings (when False). Defaults to True.
     :parameter parse_dates: list of columns (names or integers) that will be attempted to parse as date column
 
     for additional params, see documentation of  :class:`~storey.flow.Flow`
     """
 
     def __init__(
         self,
         paths: Union[List[str], str],
-        header: bool = False,
+        header: bool = True,
         build_dict: bool = False,
         key_field: Union[int, str, List[int], List[str], None] = None,
         time_field: Union[int, str, None] = None,
         timestamp_format: Optional[str] = None,
         id_field: Union[str, int, None] = None,
         type_inference: bool = True,
         parse_dates: Optional[Union[int, str, List[int], List[str]]] = None,
         **kwargs,
     ):
+
         kwargs["paths"] = paths
+        if isinstance(paths, str):
+            paths = [paths]
+        self._paths = paths
+        self._build_dict = build_dict
+        if header is False:
+            warnings.warn(
+                "header=False is deprecated, will be treated as header=True."
+                " The parameter will be removed in a future version.",
+                DeprecationWarning,
+            )
+        if type_inference is False:
+            warnings.warn(
+                "type_inference is deprecated, will be treated as type_inference=True."
+                " The parameter will be removed in a future version.",
+                DeprecationWarning,
+            )
         kwargs["header"] = header
         kwargs["build_dict"] = build_dict
         if key_field is not None:
             kwargs["key_field"] = key_field
         if time_field is not None:
             kwargs["time_field"] = time_field
         if id_field is not None:
             kwargs["id_field"] = id_field
         if timestamp_format is not None:
             kwargs["timestamp_format"] = timestamp_format
         kwargs["type_inference"] = type_inference
-        _IterableSource.__init__(self, **kwargs)
-        WithUUID.__init__(self)
-        if isinstance(paths, str):
-            paths = [paths]
+        self._storage_options = kwargs.get("storage_options")
         self._paths = paths
-        self._with_header = header
-        self._build_dict = build_dict
         self._key_field = key_field
         self._time_field = time_field
         self._timestamp_format = timestamp_format
         self._id_field = id_field
         self._type_inference = type_inference
         self._storage_options = kwargs.get("storage_options")
         self._parse_dates = parse_dates
         self._dates_indices = []
         if parse_dates:
             if not isinstance(parse_dates, List):
                 parse_dates = [parse_dates]
-            if isinstance(parse_dates, List):
-                if self._with_header and any([isinstance(f, int) for f in self._parse_dates]):
-                    raise ValueError("parse_dates can be list of int only when there is no header")
-                if not self._with_header and all([isinstance(f, int) for f in self._parse_dates]):
-                    self._dates_indices = parse_dates
-        if isinstance(self._time_field, int):
-            if self._with_header:
-                raise ValueError("time field can be int only when there is no header")
-            self._dates_indices.append(self._time_field)
-
-        if not header and isinstance(key_field, str):
-            raise ValueError("key_field can only be set to an integer when with_header is false")
-        if not header and isinstance(time_field, str):
-            raise ValueError("time_field can only be set to an integer when with_header is false")
+            self._dates_indices.extend(parse_dates)
+        if time_field is not None:
+            self._dates_indices.append(time_field)
+
+        super().__init__([], **kwargs)
 
     def _init(self):
         super()._init()
-        self._event_buffer = queue.Queue(1024)
-        self._types = []
-        self._none_columns = set()
-
-    def _infer_type(self, value):
-        lowercase = value.lower()
-        if lowercase == "true" or lowercase == "false":
-            return "b"
-
-        try:
-            int(value)
-            return "i"
-        except ValueError:
-            pass
-
-        try:
-            float(value)
-            return "f"
-        except ValueError:
-            pass
-
-        if value == "":
-            return "n"
-
-        return "s"
-
-    def _parse_field(self, field, index):
-        typ = self._types[index]
-        if typ == "s":
-            if field == "":
-                return None
-            return field
-        if typ == "f":
-            return float(field) if field != "" else math.nan
-        if typ == "i":
-            return int(field) if field != "" else math.nan
-        if typ == "b":
-            lowercase = field.lower()
-            if lowercase == "true":
-                return True
-            if lowercase == "false":
-                return False
-            if lowercase == "":
-                return None
-            raise TypeError(f"Expected boolean, got {field}")
-        if typ == "t":
-            if field == "":
-                return None
-            return self._datetime_from_timestamp(field)
-        if typ == "n":
-            return None
-        raise TypeError(f"Unknown type: {typ}")
+        self._dfs = []
+        for path in self._paths:
+            df = pandas.read_csv(
+                path,
+                header=0,
+                parse_dates=self._dates_indices,
+                date_parser=self._datetime_from_timestamp,
+                storage_options=self._storage_options,
+            )
+            self._validate_fields(df, path)
+            self._dfs.append(df)
 
     def _datetime_from_timestamp(self, timestamp):
+        if timestamp == "" or timestamp is None:
+            return None
         if self._timestamp_format:
             return pandas.to_datetime(timestamp, format=self._timestamp_format).floor("u").to_pydatetime()
         else:
             return datetime.fromisoformat(timestamp)
 
-    def _blocking_io_loop(self):
-        try:
-
-            for path in self._paths:
-                fs, file_path = url_to_file_system(path, self._storage_options)
-                with fs.open(file_path, mode="r") as f:
-                    header = None
-                    field_name_to_index = None
-                    if self._with_header:
-                        line = f.readline()
-                        header = next(csv.reader([line]))
-                        field_name_to_index = {}
-                        for i in range(len(header)):
-                            field_name_to_index[header[i]] = i
-                            if header[i] == self._time_field or (self._parse_dates and header[i] in self._parse_dates):
-                                self._dates_indices.append(i)
-                    for line in f:
-                        create_event = True
-                        parsed_line = next(csv.reader([line]))
-                        if self._type_inference:
-                            if not self._types:
-                                for index, field in enumerate(parsed_line):
-                                    if index in self._dates_indices:
-                                        self._types.append("t")
-                                    else:
-                                        type_field = self._infer_type(field)
-                                        self._types.append(type_field)
-                                        if type_field == "n":
-                                            self._none_columns.add(index)
-                            else:
-                                for index in copy.copy(self._none_columns):
-                                    type_field = self._infer_type(parsed_line[index])
-                                    if type_field != "n":
-                                        self._types[index] = type_field
-                                        self._none_columns.remove(index)
-                            for i in range(len(parsed_line)):
-                                parsed_line[i] = self._parse_field(parsed_line[i], i)
-                        element = parsed_line
-                        key = None
-                        if header:
-                            if len(parsed_line) != len(header):
-                                raise ValueError(
-                                    f"CSV line with {len(parsed_line)} fields did not match header "
-                                    f"with {len(header)} fields"
-                                )
-                            if self._build_dict:
-                                element = {}
-                                for i in range(len(parsed_line)):
-                                    element[header[i]] = parsed_line[i]
-                        if self._key_field:
-                            if isinstance(self._key_field, list):
-                                key = []
-                                for single_key_field in self._key_field:
-                                    if self._with_header and isinstance(single_key_field, str):
-                                        single_key_field_index = field_name_to_index[single_key_field]
-                                    else:
-                                        single_key_field_index = single_key_field
-                                    if parsed_line[single_key_field_index] is None:
-                                        create_event = False
-                                        break
-                                    key.append(parsed_line[single_key_field_index])
-                            else:
-                                single_key_field = self._key_field
-                                if self._with_header and isinstance(single_key_field, str):
-                                    single_key_field_index = field_name_to_index[single_key_field]
-                                else:
-                                    single_key_field_index = single_key_field
-                                key = parsed_line[single_key_field_index]
-                                if key is None:
-                                    create_event = False
-                        if create_event:
-                            if self._id_field:
-                                id_field = self._id_field
-                                if self._with_header and isinstance(id_field, str):
-                                    id_field = field_name_to_index[id_field]
-                                id = parsed_line[id_field]
-                            else:
-                                id = self._get_uuid()
-                            event = Event(element, key=key, id=id)
-                            self._event_buffer.put(event)
-                        else:
-                            if self.context:
-                                self.context.logger.error(f"For {parsed_line} value of key {single_key_field} is None")
-                if self._with_header:
-                    self._dates_indices = []
-
-        except BaseException as ex:
-            self._event_buffer.put(ex)
-        self._event_buffer.put(_termination_obj)
-
-    def _get_event(self):
-        event = self._event_buffer.get()
-        if isinstance(event, BaseException):
-            raise event
-        return event
-
-    async def _run_loop(self):
-        asyncio.get_running_loop().run_in_executor(None, self._blocking_io_loop)
-
-        def get_multiple():
-            events = [self._get_event()]
-            while not self._event_buffer.empty() and len(events) < 128:
-                events.append(self._get_event())
-            return events
-
-        while True:
-            events = await asyncio.get_running_loop().run_in_executor(None, get_multiple)
-            for event in events:
-                res = await self._do_downstream(event)
-                if event is _termination_obj:
-                    return res
-
-
-class DataframeSource(_IterableSource, WithUUID):
-    """Use pandas dataframe as input source for a flow.
-
-    :param dfs: A pandas dataframe, or dataframes, to be used as input source for the flow.
-    :param key_field: column to be used as key for events. can be list of columns
-    :param id_field: column to be used as ID for events.
-
-    for additional params, see documentation of  :class:`~storey.flow.Flow`
-    """
-
-    def __init__(
-        self,
-        dfs: Union[pandas.DataFrame, Iterable[pandas.DataFrame]],
-        key_field: Optional[Union[str, List[str]]] = None,
-        id_field: Optional[str] = None,
-        **kwargs,
-    ):
-        if key_field is not None:
-            kwargs["key_field"] = key_field
-        if id_field is not None:
-            kwargs["id_field"] = id_field
-        _IterableSource.__init__(self, **kwargs)
-        WithUUID.__init__(self)
-        if isinstance(dfs, pandas.DataFrame):
-            dfs = [dfs]
-        self._dfs = dfs
-        self._key_field = key_field
-        self._id_field = id_field
-
-    async def _run_loop(self):
-        for df in self._dfs:
-            for namedtuple in df.itertuples():
-                create_event = True
-                body = namedtuple._asdict()
-                index = body.pop("Index")
-                if len(df.index.names) > 1:
-                    for i, index_column in enumerate(df.index.names):
-                        body[index_column] = index[i]
-                elif df.index.names[0] is not None:
-                    body[df.index.names[0]] = index
-
-                key = None
-                if self._key_field:
-                    if isinstance(self._key_field, list):
-                        key = []
-                        for key_field in self._key_field:
-                            if key_field not in body or pandas.isna(body[key_field]):
-                                create_event = False
-                                break
-                            key.append(body[key_field])
-                    else:
-                        key = body[self._key_field]
-                        if key is None:
-                            create_event = False
-                if create_event:
-                    if self._id_field:
-                        id = body[self._id_field]
-                    else:
-                        id = self._get_uuid()
-                    event = Event(body, key=key, id=id)
-                    await self._do_downstream(event)
-                else:
-                    if self.context:
-                        self.context.logger.error(f"For {body} value of key {key_field} is None")
-        return await self._do_downstream(_termination_obj)
+    def _get_element(self, body: dict, columns: List[str]):
+        if self._build_dict:
+            return body
+        return [body[column] for column in columns]
 
 
 class ParquetSource(DataframeSource):
     """Reads Parquet files as input source for a flow.
 
     :parameter paths: paths to Parquet files
-    :parameter columns : list, default=None. If not None, only these columns will be read from the file.
+    :parameter columns: list, default=None. If not None, only these columns will be read from the file.
     :parameter start_filter: datetime. If not None, the results will be filtered by partitions and
         'filter_column' > start_filter. Default is None.
     :parameter end_filter: datetime. If not None, the results will be filtered by partitions
         'filter_column' <= end_filter. Default is None.
     :parameter filter_column: Optional. if not None, the results will be filtered by this column and before and/or after
     :param key_field: column to be used as key for events. can be list of columns
     :param id_field: column to be used as ID for events.
@@ -936,17 +822,26 @@
         paths: Union[str, Iterable[str]],
         columns=None,
         start_filter: Optional[datetime] = None,
         end_filter: Optional[datetime] = None,
         filter_column: Optional[str] = None,
         **kwargs,
     ):
-        if end_filter or start_filter:
-            start_filter = datetime.min if start_filter is None else start_filter
-            end_filter = datetime.max if end_filter is None else end_filter
+        if start_filter or end_filter:
+            if start_filter is None:
+                start_filter = datetime.min
+                if end_filter.tzinfo:
+                    start_filter = start_filter.replace(tzinfo=pytz.utc)
+            if end_filter is None:
+                end_filter = datetime.max
+                if start_filter.tzinfo:
+                    end_filter = end_filter.replace(tzinfo=pytz.utc)
+            if (start_filter.tzinfo is None) ^ (end_filter.tzinfo is None):
+                raise ValueError("Start and end filters must either both have a time zone or both be naive timestamps")
+
             if filter_column is None:
                 raise TypeError("Filter column is required when passing start/end filters")
 
         self._paths = paths
         if isinstance(paths, str):
             self._paths = [paths]
         self._columns = columns
@@ -964,29 +859,57 @@
         find_filters(
             partitions_time_attributes,
             self._start_filter,
             self._end_filter,
             filters,
             self._filter_column,
         )
-        return pandas.read_parquet(
-            path,
-            columns=self._columns,
-            filters=filters,
-            storage_options=self._storage_options,
-        )
+        try:
+            return pandas.read_parquet(
+                path,
+                columns=self._columns,
+                filters=filters,
+                storage_options=self._storage_options,
+            )
+        except pyarrow.lib.ArrowInvalid as ex:
+            if not str(ex).startswith("Cannot compare timestamp with timezone to timestamp without timezone"):
+                raise ex
+
+            if self._start_filter.tzinfo:
+                start_filter = self._start_filter.replace(tzinfo=None)
+                end_filter = self._end_filter.replace(tzinfo=None)
+            else:
+                start_filter = self._start_filter.replace(tzinfo=pytz.utc)
+                end_filter = self._end_filter.replace(tzinfo=pytz.utc)
+
+            filters = []
+            find_filters(
+                partitions_time_attributes,
+                start_filter,
+                end_filter,
+                filters,
+                self._filter_column,
+            )
+
+            return pandas.read_parquet(
+                path,
+                columns=self._columns,
+                filters=filters,
+                storage_options=self._storage_options,
+            )
 
     def _init(self):
         super()._init()
         self._dfs = []
         for path in self._paths:
             if self._start_filter or self._end_filter:
                 df = self._read_filtered_parquet(path)
             else:
                 df = pandas.read_parquet(path, columns=self._columns, storage_options=self._storage_options)
+            self._validate_fields(df, path)
             self._dfs.append(df)
 
 
 class SQLSource(_IterableSource, WithUUID):
     """Use SQL table as input source for a flow.
 
     :parameter key_field: the primary key of the table.
@@ -1021,16 +944,24 @@
         self._id_field = id_field
 
     async def _run_loop(self):
         import sqlalchemy as db
 
         engine = db.create_engine(self.db_path)
         with engine.connect() as conn:
-            query = f"SELECT * FROM {self.table_name}"
-            cursor = pandas.read_sql(query, con=conn, parse_dates=self.time_fields, chunksize=100)
+            metadata = db.MetaData()
+
+            table = db.Table(
+                self.table_name,
+                metadata,
+                autoload=True,
+                autoload_with=engine,
+            )
+            select_object = db.select(table)
+            cursor = pandas.read_sql(select_object, con=conn, parse_dates=self.time_fields, chunksize=100)
 
             for df in cursor:
                 for row in df.itertuples(index=False):
                     body = dict(row._asdict())
                     key = None
                     if self._key_field:
                         if isinstance(self._key_field, list):
```

### Comparing `storey-1.3.9/storey/steps/__init__.py` & `storey-1.4.0/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/steps/assertion.py` & `storey-1.4.0/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/steps/flatten.py` & `storey-1.4.0/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/steps/foreach.py` & `storey-1.4.0/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/steps/partition.py` & `storey-1.4.0/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/steps/sample.py` & `storey-1.4.0/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/table.py` & `storey-1.4.0/storey/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,23 +1327,23 @@
                 feature_name = key[:separator_index]
                 aggr = key[separator_index + 1 :]
                 if feature_name not in initial_data_by_feature:
                     initial_data_by_feature[feature_name] = {}
                 initial_data_by_feature[feature_name][aggr] = value
 
         for aggregation_metadata in aggregates:
-            explicit_raw_aggregates = set()
-            hidden_raw_aggregates = set()
+            explicit_raw_aggregates = []
+            hidden_raw_aggregates = []
             virtual_aggregates = []
             for aggregation in aggregation_metadata.aggregations:
                 if is_raw_aggregate(aggregation):
-                    explicit_raw_aggregates.add(aggregation)
+                    explicit_raw_aggregates.append(aggregation)
                 else:
                     dependant_aggregate_names = get_implied_aggregates(aggregation)
-                    hidden_raw_aggregates.update(dependant_aggregate_names)
+                    hidden_raw_aggregates.extend(dependant_aggregate_names)
                     virtual_aggregates.append(VirtualAggregation(aggregation, dependant_aggregate_names))
             initial_column_data = None
             if initial_data_by_feature and aggregation_metadata.name in initial_data_by_feature:
                 initial_column_data = initial_data_by_feature[aggregation_metadata.name]
             self.aggregation_buckets[aggregation_metadata.name] = AggregationBuckets(
                 aggregation_metadata.name,
                 explicit_raw_aggregates,
@@ -1400,17 +1400,18 @@
         initial_data=None,
         persist_func=None,
     ):
         self.key = key
         self.name = name
         self._explicit_raw_aggregations = explicit_raw_aggregations
         self._hidden_raw_aggregations = hidden_raw_aggregations
-        self._all_raw_aggregates = set()
-        self._all_raw_aggregates.update(self._explicit_raw_aggregations)
-        self._all_raw_aggregates.update(self._hidden_raw_aggregations)
+        self._all_raw_aggregates = self._explicit_raw_aggregations.copy()
+        for hidden_aggr in self._hidden_raw_aggregations:
+            if hidden_aggr not in self._all_raw_aggregates:
+                self._all_raw_aggregates.append(hidden_aggr)
         self._virtual_aggregations = virtual_aggregations
         self.explicit_windows = explicit_windows
         self.max_value = max_value
         self.buckets = []
         self.should_persist = True
         self.pending_aggr = {}
         self.storage_specific_cache = {}
```

### Comparing `storey-1.3.9/storey/targets.py` & `storey-1.4.0/storey/targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,16 +172,16 @@
                 else:
                     self._non_partition_columns.append(col)
                     if self._column_types:
                         self._non_partition_column_types.append(self._column_types[index])
 
     def _get_event_time(self, event):
         event_time = event.processing_time
-        if self._time_field is not None:
-            time_field = self._time_field
+        time_field = self._time_field
+        if time_field is not None and time_field != "":
             if isinstance(event.body, list) and isinstance(time_field, str):
                 time_field = self._col_to_index[time_field]
             event_time = event.body[time_field]
             if isinstance(event_time, str):
                 if self._time_format:
                     event_time = datetime.datetime.strptime(event_time, self._time_format)
                 else:
```

### Comparing `storey-1.3.9/storey/transformations/__init__.py` & `storey-1.4.0/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/utils.py` & `storey-1.4.0/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey/windowed_store.py` & `storey-1.4.0/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/storey.egg-info/PKG-INFO` & `storey-1.4.0/storey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.3.9
+Version: 1.4.0
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.3.9/storey.egg-info/SOURCES.txt` & `storey-1.4.0/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/tests/__init__.py` & `storey-1.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/tests/test_aggregate_by_key.py` & `storey-1.4.0/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/tests/test_aggregate_store.py` & `storey-1.4.0/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/tests/test_flow.py` & `storey-1.4.0/tests/test_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,40 +224,41 @@
     expected = pd.DataFrame([["hello", t]], columns=["salutation", "mytime"])
     assert termination_result.equals(expected)
 
 
 def test_csv_reader():
     controller = build_flow(
         [
-            CSVSource("tests/test.csv", header=True),
+            CSVSource("tests/test.csv"),
             FlatMap(lambda x: x),
             Map(lambda x: int(x)),
             Reduce(0, lambda acc, x: acc + x),
         ]
     ).run()
 
     termination_result = controller.await_termination()
     assert termination_result == 21
 
 
 def test_csv_reader_error_on_file_not_found():
-    controller = build_flow(
+    flow = build_flow(
         [
-            CSVSource("tests/idontexist.csv", header=True),
+            CSVSource("tests/idontexist.csv"),
         ]
-    ).run()
-
-    with pytest.raises(FileNotFoundError):
-        controller.await_termination()
+    )
+    with pytest.raises(
+        FileNotFoundError,
+    ):
+        flow.run()
 
 
 def test_csv_reader_as_dict():
     controller = build_flow(
         [
-            CSVSource("tests/test.csv", header=True, build_dict=True),
+            CSVSource("tests/test.csv", build_dict=True),
             FlatMap(lambda x: [x["n1"], x["n2"], x["n3"]]),
             Map(lambda x: int(x)),
             Reduce(0, lambda acc, x: acc + x),
         ]
     ).run()
 
     termination_result = controller.await_termination()
@@ -355,42 +356,89 @@
     assert len(termination_result) == 2
     assert termination_result[0].key == "m1"
     assert termination_result[0].body == ["m1", datetime(2020, 2, 15, 2, 0), 8, True]
     assert termination_result[1].key == "m2"
     assert termination_result[1].body == ["m2", datetime(2020, 2, 16, 2, 0), 14, False]
 
 
-def test_csv_reader_as_dict_no_header():
-    controller = build_flow(
-        [
-            CSVSource("tests/test-no-header.csv", header=False, build_dict=True),
-            FlatMap(lambda x: [x[0], x[1], x[2]]),
-            Map(lambda x: int(x)),
-            Reduce(0, lambda acc, x: acc + x),
-        ]
-    ).run()
+@pytest.mark.parametrize(
+    "csv_source_kwargs", [{"parse_dates": ["t", "non_existent_column"]}, {"time_field": "non_existent_column"}]
+)
+def test_parse_dates_key_error(csv_source_kwargs):
+    with pytest.raises(ValueError) as value_error:
+        controller = build_flow(
+            [
+                CSVSource(
+                    "tests/test-with-timestamp.csv",
+                    header=True,
+                    key_field="t",
+                    timestamp_format="%d/%m/%Y %H:%M:%S",
+                    **csv_source_kwargs,
+                )
+            ]
+        ).run()
+        controller.await_termination()
+    assert str(value_error.value) == "Missing column provided to 'parse_dates': 'non_existent_column'"
 
-    termination_result = controller.await_termination()
-    assert termination_result == 21
+
+@pytest.mark.parametrize("csv_source_kwargs", [{"parse_dates": ["t", 10]}, {"time_field": 10}])
+def test_parse_dates_index_error(csv_source_kwargs):
+    with pytest.raises(IndexError):
+        controller = build_flow(
+            [
+                CSVSource(
+                    "tests/test-with-timestamp.csv",
+                    header=True,
+                    key_field="k",
+                    timestamp_format="%d/%m/%Y %H:%M:%S",
+                    **csv_source_kwargs,
+                )
+            ]
+        ).run()
+        controller.await_termination()
 
 
 def test_csv_reader_none_in_keyfield_should_send_error_log():
     logger = MockLogger()
     context = MockContext(logger, True)
 
     controller = build_flow(
         [
-            CSVSource("tests/test-none-in-keyfield.csv", header=True, key_field="k", context=context),
+            CSVSource("tests/test-none-in-keyfield.csv", key_field="k", context=context),
         ]
     ).run()
 
     controller.await_termination()
 
     assert "error" == logger.logs[0][0]
-    assert "value of key k is None" in logger.logs[0][1][0]
+    assert "Encountered null values in the following key fields: k" in logger.logs[0][1][0]
+
+
+def test_csv_source_key_error():
+    with pytest.raises(ValueError) as value_error:
+        controller = build_flow(
+            [
+                CSVSource("tests/test.csv", key_field="not_exist"),
+            ]
+        ).run()
+
+        controller.await_termination()
+    assert str(value_error.value) == "key column 'not_exist' is missing from dataframe. File path: tests/test.csv."
+
+
+def test_csv_reader_id_key_error():
+    with pytest.raises(ValueError) as value_error:
+        controller = build_flow(
+            [
+                CSVSource("tests/test.csv", id_field="not_exist"),
+            ]
+        ).run()
+
+        controller.await_termination()
+    assert str(value_error.value) == "id column 'not_exist' is missing from dataframe. File path: tests/test.csv."
 
 
 def test_dataframe_source():
     df = pd.DataFrame([["hello", 1, 1.5], ["world", 2, 2.5]], columns=["string", "int", "float"])
     controller = build_flow(
         [
             DataframeSource(df),
@@ -784,14 +832,40 @@
         controller.emit(i)
 
     controller.terminate()
     result = controller.await_termination()
     assert result == 55
 
 
+def test_read_space_in_header_csv():
+    controller = build_flow(
+        [
+            CSVSource("tests/test_space_in_header.csv", build_dict=True),
+            Reduce([], append_and_return),
+        ]
+    ).run()
+
+    termination_result = controller.await_termination()
+    expected = [{"header with space": 1, "n2": 2, "n3": 3}, {"header with space": 4, "n2": 5, "n3": 6}]
+    assert termination_result == expected
+
+
+def test_read_space_in_header_parquet():
+    controller = build_flow(
+        [
+            ParquetSource("tests/test_space_in_header.parquet"),
+            Reduce([], append_and_return),
+        ]
+    ).run()
+
+    termination_result = controller.await_termination()
+    expected = [{"header with space": 1, "n2": 2, "n3": 3}, {"header with space": 4, "n2": 5, "n3": 6}]
+    assert termination_result == expected
+
+
 def test_error_specific_recovery():
     reduce = Reduce(0, lambda acc, x: acc + x)
     controller = build_flow(
         [
             SyncEmitSource(),
             Map(lambda x: x + 1),
             Map(RaiseEx(5).raise_ex, recovery_step={ATestException: reduce}),
@@ -2173,15 +2247,16 @@
         ("my_int", "int"),
         ("my_string", "str"),
         ("my_datetime", "datetime"),
     ]
     controller = build_flow(
         [
             SyncEmitSource(),
-            ParquetTarget(out_dir, partition_cols=[], columns=columns_with_type, max_events=1),
+            # set time_field="" to test for ML-3544 regression
+            ParquetTarget(out_dir, partition_cols=[], columns=columns_with_type, time_field="", max_events=1),
         ]
     ).run()
 
     my_time = datetime(2020, 2, 15)
 
     expected = []
     for i in range(10):
@@ -3276,15 +3351,15 @@
 
 
 def test_reader_writer_to_code():
     flow = build_flow([CSVSource("mycsv.csv"), ParquetTarget("mypq")])
 
     reconstructed_code = flow.to_code()
     print(reconstructed_code)
-    expected = """c_s_v_source0 = CSVSource(paths='mycsv.csv', header=False, build_dict=False, type_inference=True)
+    expected = """c_s_v_source0 = CSVSource(paths='mycsv.csv', header=True, build_dict=False, type_inference=True)
 parquet_target0 = ParquetTarget(path='mypq', max_events=10000, flush_after_seconds=60)
 
 c_s_v_source0.to(parquet_target0)
 """
     assert reconstructed_code == expected
 
 
@@ -3378,41 +3453,57 @@
     controller.terminate()
     controller.await_termination()
 
 
 # ML-2257
 def test_query_by_key_edge_case_field_name():
     table = Table("table", NoopDriver())
-    QueryByKey(["my_color_5sec"], table, key_field="name"),
+    QueryByKey(["my_color_5sec"], table, key_field="name")
+
+
+# ML-3782
+def test_query_by_key_non_aggregate():
+    table = Table("table", NoopDriver())
+    query_by_key = QueryByKey(["my_color_5h"], table, key_field="name")
+    assert query_by_key._aggrs == []
+    assert query_by_key._enrich_cols == ["my_color_5h"]
 
 
 def test_csv_source_with_none_values():
     controller = build_flow(
         [
-            CSVSource("tests/test-with-none-values.csv", header=True, key_field="string"),
+            CSVSource("tests/test-with-none-values.csv", key_field="string"),
             Reduce([], append_and_return, full_event=True),
         ]
     ).run()
 
     termination_result = controller.await_termination()
 
-    print(termination_result)
-
     assert len(termination_result) == 2
     assert termination_result[0].key == "a"
     assert termination_result[0].body == [
         "a",
         True,
         False,
         1,
         2.3,
         "2021-04-21 15:56:53.385444",
     ]
     assert termination_result[1].key == "b"
-    assert termination_result[1].body == ["b", True, None, math.nan, math.nan, None]
+    excepted_result = ["b", True, math.nan, math.nan, math.nan, math.nan]
+    assert len(termination_result[1].body) == len(excepted_result)
+    for x, y in zip(termination_result[1].body, excepted_result):
+        if isinstance(x, float):
+            assert isinstance(y, float)
+            if math.isnan(x):
+                assert math.isnan(y)
+            else:
+                assert x == y
+        else:
+            assert x == y
 
 
 def test_csv_source_event_metadata():
     controller = build_flow(
         [
             CSVSource(
                 "tests/test-with-timestamp.csv",
@@ -3481,14 +3572,42 @@
     ).run()
     result = controller.await_termination()
     expected = [{"index": 10, "some_data": 1}, {"index": 20, "some_data": 3}]
 
     assert result == expected
 
 
+def test_dataframe_source_missing_key_column():
+    with pytest.raises(ValueError) as value_error:
+        data = pd.DataFrame({"id": [1, 2, 3], "some_data": ["data", "random_data", "my_data"]})
+
+        controller = build_flow(
+            [
+                DataframeSource(dfs=data, key_field="non_existent_column"),
+            ]
+        ).run()
+        controller.await_termination()
+
+    assert str(value_error.value) == "key column 'non_existent_column' is missing from dataframe."
+
+
+def test_dataframe_source_missing_id_column():
+    with pytest.raises(ValueError) as value_error:
+        data = pd.DataFrame({"id": [1, 2, 3], "some_data": ["data", "random_data", "my_data"]})
+
+        controller = build_flow(
+            [
+                DataframeSource(dfs=data, id_field="non_existent_column"),
+            ]
+        ).run()
+        controller.await_termination()
+
+    assert str(value_error.value) == "id column 'non_existent_column' is missing from dataframe."
+
+
 def test_none_key_date_is_not_written():
     data = pd.DataFrame(
         {
             "index": [
                 datetime(2020, 6, 27, 10, 23, 8, 420581),
                 None,
                 datetime(2020, 6, 28, 10, 23, 8, 420581),
@@ -3509,14 +3628,25 @@
         {"index": datetime(2020, 6, 27, 10, 23, 8, 420581), "some_data": 1},
         {"index": datetime(2020, 6, 28, 10, 23, 8, 420581), "some_data": 3},
     ]
 
     assert result == expected
 
 
+def test_not_string_key_field():
+    with pytest.raises(ValueError) as value_error:
+        build_flow(
+            [
+                CSVSource("tests/test.csv", key_field=0),
+            ]
+        ).run()
+
+    assert str(value_error.value) == "key_field must be a string or list of strings"
+
+
 def test_csv_none_value_first_row(tmpdir):
     out_file_par = f"{tmpdir}/test_csv_none_value_first_row_{uuid.uuid4().hex}.parquet"
     out_file_csv = f"{tmpdir}/test_csv_none_value_first_row_{uuid.uuid4().hex}.csv"
 
     columns = ["first_name", "bid", "bool", "time"]
     data = pd.DataFrame(
         [
@@ -3525,15 +3655,15 @@
         ],
         columns=columns,
     )
     data.to_csv(out_file_csv)
 
     controller = build_flow(
         [
-            CSVSource(out_file_csv, header=True, key_field="first_name", build_dict=True),
+            CSVSource(out_file_csv, key_field="first_name", build_dict=True),
             ParquetTarget(out_file_par),
         ]
     ).run()
 
     controller.await_termination()
     read_back_df = pd.read_parquet(out_file_par)
 
@@ -3551,15 +3681,15 @@
 
     columns = ["first_name", "str"]
     data = pd.DataFrame([["katya", "strrrr"], ["dina", None]], columns=columns)
     data.to_csv(out_file_csv)
 
     controller = build_flow(
         [
-            CSVSource(out_file_csv, header=True, key_field="first_name", build_dict=True),
+            CSVSource(out_file_csv, key_field="first_name", build_dict=True),
             ParquetTarget(out_file_par),
         ]
     ).run()
 
     controller.await_termination()
     read_back_df = pd.read_parquet(out_file_par)
 
@@ -3567,28 +3697,14 @@
     u.to_parquet(out_file_par)
     r2 = pd.read_parquet(out_file_par)
 
     assert r2["str"].compare(read_back_df["str"]).empty
 
 
 def test_csv_multiple_time_columns(tmpdir):
-    with pytest.raises(ValueError):
-        controller = build_flow(
-            [
-                CSVSource(
-                    "tests/test-multiple-time-columns.csv",
-                    header=True,
-                    time_field="t1",
-                    parse_dates=[2],
-                ),
-                Reduce([], append_and_return),
-            ]
-        ).run()
-
-    # now do it correctly
     controller = build_flow(
         [
             CSVSource(
                 "tests/test-multiple-time-columns.csv",
                 header=True,
                 time_field="t1",
                 parse_dates=["t2"],
@@ -3987,33 +4103,114 @@
     controller.emit({"a": 1, "b": 2, "c": 3, "d": 4, "e": 5})
     controller.terminate()
     termination_result = controller.await_termination()
     assert termination_result == [{"b": 1, "c": 3, "e": 5}]
 
 
 def test_read_sql_db():
+    # using `table_1; DROP DATABASE test;` as the table name for testing injection
     import sqlalchemy as db
 
     engine = db.create_engine(integration.conftest.SQLITE_DB)
     with engine.connect() as conn:
         origin_df = pd.DataFrame(
             {
                 "string": ["hello", "world"],
                 "int": [1, 2],
                 "float": [1.5, 2.5],
                 "time": [pd.Timestamp(2017, 1, 1, 12), pd.Timestamp(2017, 1, 1, 12)],
             }
         )
-        origin_df.to_sql("table_1", conn, if_exists="replace", index=False)
+        origin_df.to_sql("table_1; DROP DATABASE test;", conn, if_exists="replace", index=False)
     controller = build_flow(
         [
-            SQLSource("sqlite:///test.db", "table_1", "string", id_field="int", time_fields=["time"]),
+            SQLSource(
+                "sqlite:///test.db", "table_1; DROP DATABASE test;", "string", id_field="int", time_fields=["time"]
+            ),
             Reduce([], append_and_return),
         ]
     ).run()
 
     actual = controller.await_termination()
     expected = [
         {"string": "hello", "int": 1, "float": 1.5, "time": pd.Timestamp(2017, 1, 1, 12)},
         {"string": "world", "int": 2, "float": 2.5, "time": pd.Timestamp(2017, 1, 1, 12)},
     ]
     assert actual == expected
+
+
+# Time zone related parameterization is to test for ML-3566
+@pytest.mark.parametrize(
+    ["data_with_timezone", "filter_with_timezone"], [[True, True], [True, False], [False, True], [False, False]]
+)
+def test_filter_by_time_non_partitioned(data_with_timezone, filter_with_timezone):
+    columns = ["my_string", "my_time", "my_city"]
+
+    data_timezone_suffix = "Z" if data_with_timezone else ""
+
+    df = pd.DataFrame(
+        [
+            ["dina", pd.Timestamp(f"2019-07-01 00:00:00{data_timezone_suffix}"), "tel aviv"],
+            ["uri", pd.Timestamp(f"2018-12-30 09:00:00{data_timezone_suffix}"), "tel aviv"],
+            ["katya", pd.Timestamp(f"2020-12-31 14:00:00{data_timezone_suffix}"), "hod hasharon"],
+        ],
+        columns=columns,
+    )
+    df.set_index("my_string")
+    path = "/tmp/test_filter_by_time_non_partitioned.parquet"
+    df.to_parquet(path)
+    start = datetime.fromisoformat("2019-07-01 00:00:00" + ("+00:00" if data_with_timezone else ""))
+    end = pd.Timestamp("2020-12-31 14:00:00" + ("Z" if data_with_timezone else ""))
+
+    controller = build_flow(
+        [
+            ParquetSource(path, start_filter=start, end_filter=end, filter_column="my_time"),
+            Reduce([], append_and_return),
+        ]
+    ).run()
+
+    read_back_result = controller.await_termination()
+
+    expected = [
+        {
+            "my_string": "katya",
+            "my_time": pd.Timestamp(f"2020-12-31 14:00:00{data_timezone_suffix}"),
+            "my_city": "hod hasharon",
+        }
+    ]
+
+    try:
+        assert read_back_result == expected, f"{read_back_result}\n!=\n{expected}"
+    finally:
+        os.remove(path)
+
+
+def test_empty_filter_result():
+    columns = ["my_string", "my_time", "my_city"]
+
+    df = pd.DataFrame(
+        [
+            ["dina", pd.Timestamp("2019-07-01 00:00:00"), "tel aviv"],
+            ["uri", pd.Timestamp("2018-12-30 09:00:00"), "tel aviv"],
+            ["katya", pd.Timestamp("2020-12-31 14:00:00"), "hod hasharon"],
+        ],
+        columns=columns,
+    )
+    df.set_index("my_string")
+    path = "/tmp/test_empty_filter_result.parquet"
+    df.to_parquet(path)
+    start = pd.Timestamp("2022-07-01 00:00:00")
+    end = pd.Timestamp("2022-12-31 14:00:00")
+
+    controller = build_flow(
+        [
+            ParquetSource(path, start_filter=start, end_filter=end, filter_column="my_time"),
+            ReduceToDataFrame(index=["my_string"], insert_key_column_as=["my_string"]),
+        ]
+    ).run()
+
+    read_back_result = controller.await_termination()
+
+    try:
+        pd.testing.assert_frame_equal(read_back_result, pd.DataFrame({}))
+    finally:
+        os.remove(path)
```

### Comparing `storey-1.3.9/tests/test_steps.py` & `storey-1.4.0/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/tests/test_types.py` & `storey-1.4.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/tests/test_v3io.py` & `storey-1.4.0/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.9/tests/test_windowed_store.py` & `storey-1.4.0/tests/test_windowed_store.py`

 * *Files identical despite different names*

