# Comparing `tmp/wds-client-0.2.80.tar.gz` & `tmp/wds-client-0.2.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds-client-0.2.80.tar", last modified: Mon May  8 19:30:41 2023, max compression
+gzip compressed data, was "wds-client-0.2.84.tar", last modified: Wed May 17 15:12:33 2023, max compression
```

## Comparing `wds-client-0.2.80.tar` & `wds-client-0.2.84.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.491436 wds-client-0.2.80/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 19:30:41.491436 wds-client-0.2.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-08 19:29:34.000000 wds-client-0.2.80/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 19:30:41.491436 wds-client-0.2.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 19:29:34.000000 wds-client-0.2.80/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.483436 wds-client-0.2.80/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.487436 wds-client-0.2.80/wds_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.487436 wds-client-0.2.80/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    61563 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19355 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26218 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.491436 wds-client-0.2.80/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.487436 wds-client-0.2.80/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.224681 wds-client-0.2.84/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 15:12:33.224681 wds-client-0.2.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-17 15:10:55.000000 wds-client-0.2.84/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 15:12:33.224681 wds-client-0.2.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-17 15:10:55.000000 wds-client-0.2.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.216681 wds-client-0.2.84/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 15:10:55.000000 wds-client-0.2.84/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.216681 wds-client-0.2.84/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.220681 wds-client-0.2.84/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61562 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26217 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.224681 wds-client-0.2.84/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-17 15:10:55.000000 wds-client-0.2.84/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:12:33.216681 wds-client-0.2.84/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 15:12:33.000000 wds-client-0.2.84/wds_client.egg-info/top_level.txt
```

### Comparing `wds-client-0.2.80/README.md` & `wds-client-0.2.84/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # wds-client
 This page lists current APIs.
-
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.2.80
+- Package version: 0.2.84
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -95,14 +94,15 @@
 *RecordsApi* | [**get_records_as_tsv**](docs/RecordsApi.md#get_records_as_tsv) | **GET** /{instanceid}/tsv/{v}/{type} | Retrieve all records in record type as tsv.
 *RecordsApi* | [**query_records**](docs/RecordsApi.md#query_records) | **POST** /{instanceid}/search/{v}/{type} | Query records
 *RecordsApi* | [**update_record**](docs/RecordsApi.md#update_record) | **PATCH** /{instanceid}/records/{v}/{type}/{id} | Update record
 *RecordsApi* | [**upload_tsv**](docs/RecordsApi.md#upload_tsv) | **POST** /{instanceid}/tsv/{v}/{type} | Import records to a record type from a tsv file
 *SchemaApi* | [**delete_record_type**](docs/SchemaApi.md#delete_record_type) | **DELETE** /{instanceid}/types/{v}/{type} | Delete record type
 *SchemaApi* | [**describe_all_record_types**](docs/SchemaApi.md#describe_all_record_types) | **GET** /{instanceid}/types/{v} | Describe all record types
 *SchemaApi* | [**describe_record_type**](docs/SchemaApi.md#describe_record_type) | **GET** /{instanceid}/types/{v}/{type} | Describe record type
+*SnapshotsApi* | [**import_snapshot**](docs/SnapshotsApi.md#import_snapshot) | **POST** /{instanceid}/snapshots/{v}/{snapshotid} | Import a snapshot from Terra Data Repo
 
 
 ## Documentation For Models
 
  - [AttributeSchema](docs/AttributeSchema.md)
  - [BatchOperation](docs/BatchOperation.md)
  - [BatchRecordRequest](docs/BatchRecordRequest.md)
```

### Comparing `wds-client-0.2.80/setup.py` & `wds-client-0.2.84/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.2.80"
+VERSION = "0.2.84"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -32,10 +32,10 @@
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "Workspace Data Service"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="BSD",
     long_description="""\
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
     """
 )
```

### Comparing `wds-client-0.2.80/test/test_attribute_schema.py` & `wds-client-0.2.84/test/test_attribute_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_batch_operation.py` & `wds-client-0.2.84/test/test_batch_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_batch_record_request.py` & `wds-client-0.2.84/test/test_batch_record_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_batch_response.py` & `wds-client-0.2.84/test/test_batch_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_build.py` & `wds-client-0.2.84/test/test_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_commit.py` & `wds-client-0.2.84/test/test_commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_component.py` & `wds-client-0.2.84/test/test_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_components.py` & `wds-client-0.2.84/test/test_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_db_component.py` & `wds-client-0.2.84/test/test_db_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_error_response.py` & `wds-client-0.2.84/test/test_error_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_general_wds_information_api.py` & `wds-client-0.2.84/test/test_general_wds_information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_git.py` & `wds-client-0.2.84/test/test_git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_inline_object.py` & `wds-client-0.2.84/test/test_inline_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_instances_api.py` & `wds-client-0.2.84/test/test_instances_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_record_attribute_definition.py` & `wds-client-0.2.84/test/test_record_attribute_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_record_query_response.py` & `wds-client-0.2.84/test/test_record_query_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_record_request.py` & `wds-client-0.2.84/test/test_record_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_record_response.py` & `wds-client-0.2.84/test/test_record_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_record_type_schema.py` & `wds-client-0.2.84/test/test_record_type_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_records_api.py` & `wds-client-0.2.84/test/test_records_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_request_body_search.py` & `wds-client-0.2.84/test/test_request_body_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_schema_api.py` & `wds-client-0.2.84/test/test_schema_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_search_operator.py` & `wds-client-0.2.84/test/test_search_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_search_request.py` & `wds-client-0.2.84/test/test_search_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_search_sort_direction.py` & `wds-client-0.2.84/test/test_search_sort_direction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_stack_trace_element.py` & `wds-client-0.2.84/test/test_stack_trace_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_status_response.py` & `wds-client-0.2.84/test/test_status_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_tsv_upload_response.py` & `wds-client-0.2.84/test/test_tsv_upload_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/test/test_version_response.py` & `wds-client-0.2.84/test/test_version_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/wds_client/__init__.py` & `wds-client-0.2.84/wds_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.80"
+__version__ = "0.2.84"
 
 # import apis into sdk package
 from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
 from wds_client.api.instances_api import InstancesApi
 from wds_client.api.records_api import RecordsApi
 from wds_client.api.schema_api import SchemaApi
+from wds_client.api.snapshots_api import SnapshotsApi
 
 # import ApiClient
 from wds_client.api_client import ApiClient
 from wds_client.configuration import Configuration
 from wds_client.exceptions import OpenApiException
 from wds_client.exceptions import ApiTypeError
 from wds_client.exceptions import ApiValueError
```

### Comparing `wds-client-0.2.80/wds_client/api/general_wds_information_api.py` & `wds-client-0.2.84/wds_client/api/general_wds_information_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/wds_client/api/instances_api.py` & `wds-client-0.2.84/wds_client/api/instances_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/wds_client/api/records_api.py` & `wds-client-0.2.84/wds_client/api/records_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/wds_client/api/schema_api.py` & `wds-client-0.2.84/wds_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/wds_client/api_client.py` & `wds-client-0.2.84/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.2.80/python'
+        self.user_agent = 'OpenAPI-Generator/0.2.84/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds-client-0.2.80/wds_client/configuration.py` & `wds-client-0.2.84/wds_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.2.80".\
+               "SDK Package Version: 0.2.84".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds-client-0.2.80/wds_client/exceptions.py` & `wds-client-0.2.84/wds_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `wds-client-0.2.80/wds_client/models/__init__.py` & `wds-client-0.2.84/wds_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/wds_client/models/attribute_schema.py` & `wds-client-0.2.84/wds_client/models/attribute_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/batch_operation.py` & `wds-client-0.2.84/wds_client/models/batch_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/batch_record_request.py` & `wds-client-0.2.84/wds_client/models/batch_record_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/batch_response.py` & `wds-client-0.2.84/wds_client/models/batch_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/build.py` & `wds-client-0.2.84/wds_client/models/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/commit.py` & `wds-client-0.2.84/wds_client/models/commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/component.py` & `wds-client-0.2.84/wds_client/models/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/components.py` & `wds-client-0.2.84/wds_client/models/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/db_component.py` & `wds-client-0.2.84/wds_client/models/db_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/error_response.py` & `wds-client-0.2.84/wds_client/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/git.py` & `wds-client-0.2.84/wds_client/models/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/inline_object.py` & `wds-client-0.2.84/wds_client/models/inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/record_attribute_definition.py` & `wds-client-0.2.84/wds_client/models/record_attribute_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/record_query_response.py` & `wds-client-0.2.84/wds_client/models/record_query_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/record_request.py` & `wds-client-0.2.84/wds_client/models/record_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/record_response.py` & `wds-client-0.2.84/wds_client/models/record_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/record_type_schema.py` & `wds-client-0.2.84/wds_client/models/record_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/request_body_search.py` & `wds-client-0.2.84/wds_client/models/request_body_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/search_operator.py` & `wds-client-0.2.84/wds_client/models/search_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/search_request.py` & `wds-client-0.2.84/wds_client/models/search_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/search_sort_direction.py` & `wds-client-0.2.84/wds_client/models/search_sort_direction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/stack_trace_element.py` & `wds-client-0.2.84/wds_client/models/stack_trace_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/status_response.py` & `wds-client-0.2.84/wds_client/models/status_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/tsv_upload_response.py` & `wds-client-0.2.84/wds_client/models/tsv_upload_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/models/version_response.py` & `wds-client-0.2.84/wds_client/models/version_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.80/wds_client/rest.py` & `wds-client-0.2.84/wds_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs. As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.80/wds_client.egg-info/SOURCES.txt` & `wds-client-0.2.84/wds_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 test/test_record_type_schema.py
 test/test_records_api.py
 test/test_request_body_search.py
 test/test_schema_api.py
 test/test_search_operator.py
 test/test_search_request.py
 test/test_search_sort_direction.py
+test/test_snapshots_api.py
 test/test_stack_trace_element.py
 test/test_status_response.py
 test/test_tsv_upload_response.py
 test/test_version_response.py
 wds_client/__init__.py
 wds_client/api_client.py
 wds_client/configuration.py
@@ -41,14 +42,15 @@
 wds_client.egg-info/requires.txt
 wds_client.egg-info/top_level.txt
 wds_client/api/__init__.py
 wds_client/api/general_wds_information_api.py
 wds_client/api/instances_api.py
 wds_client/api/records_api.py
 wds_client/api/schema_api.py
+wds_client/api/snapshots_api.py
 wds_client/models/__init__.py
 wds_client/models/attribute_schema.py
 wds_client/models/batch_operation.py
 wds_client/models/batch_record_request.py
 wds_client/models/batch_response.py
 wds_client/models/build.py
 wds_client/models/commit.py
```

