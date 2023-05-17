# Comparing `tmp/minknow_api-5.4.0.tar.gz` & `tmp/minknow_api-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minknow_api-5.4.0.tar", last modified: Wed Feb  1 14:01:12 2023, max compression
+gzip compressed data, was "minknow_api-5.5.2.tar", last modified: Wed May 17 09:21:10 2023, max compression
```

## Comparing `minknow_api-5.4.0.tar` & `minknow_api-5.5.2.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 14:01:12.601487 minknow_api-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    14548 2023-02-01 14:01:12.601487 minknow_api-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14286 2023-02-01 14:01:02.000000 minknow_api-5.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 14:01:12.601487 minknow_api-5.4.0/minknow_api/
--rw-r--r--   0 runner    (1001) docker     (122)    19616 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/_support.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    59841 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/acquisition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    25816 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/acquisition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    38348 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/acquisition_service.py
--rw-r--r--   0 runner    (1001) docker     (122)   110009 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/analysis_configuration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    37700 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/analysis_configuration_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    54619 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/analysis_configuration_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    44113 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/basecaller_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    26230 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/basecaller_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    40149 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/basecaller_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/ca.crt
--rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    75802 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    28044 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    39259 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/data_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    79165 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    54269 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/device_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    67137 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/device_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 14:01:12.601487 minknow_api-5.4.0/minknow_api/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7071 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/examples/export_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/examples/extract_run_statistics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/examples/list_sequencing_positions.py
--rw-r--r--   0 runner    (1001) docker     (122)    14498 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/examples/load_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/examples/run_after_protocol.py
--rw-r--r--   0 runner    (1001) docker     (122)    22092 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/examples/start_protocol.py
--rw-r--r--   0 runner    (1001) docker     (122)    28033 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    18886 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/instance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    20779 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/instance_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    13608 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/keystore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    11607 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/keystore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    15100 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/keystore_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     9594 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     6377 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8935 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/log_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    22777 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    98102 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/manager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    61829 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/manager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    75988 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/manager_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    26154 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/minion_device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     6533 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/minion_device_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    23361 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/minion_device_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/post_processing_protocol_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    36210 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/promethion_device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    14303 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/promethion_device_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    20769 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/promethion_device_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    72191 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/protocol_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    49055 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/protocol_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    59523 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/protocol_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    12269 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/protocol_settings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/protocol_settings_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/protocol_settings_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/report_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/report_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/report_data_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/rpc_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    30270 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/run_until_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    35039 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/run_until_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    26189 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/run_until_service.py
--rw-r--r--   0 runner    (1001) docker     (122)    55921 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/statistics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    19968 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/statistics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    34751 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/statistics_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     9175 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 14:01:12.601487 minknow_api-5.4.0/minknow_api/tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15582 2023-02-01 14:01:02.000000 minknow_api-5.4.0/minknow_api/tools/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 14:01:12.601487 minknow_api-5.4.0/minknow_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14548 2023-02-01 14:01:12.000000 minknow_api-5.4.0/minknow_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-02-01 14:01:12.000000 minknow_api-5.4.0/minknow_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-01 14:01:12.000000 minknow_api-5.4.0/minknow_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-02-01 14:01:12.000000 minknow_api-5.4.0/minknow_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-01 14:01:12.000000 minknow_api-5.4.0/minknow_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-01 14:01:12.601487 minknow_api-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-02-01 14:01:02.000000 minknow_api-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:21:09.993781 minknow_api-5.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    14548 2023-05-17 09:21:09.993781 minknow_api-5.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14286 2023-05-17 09:20:59.000000 minknow_api-5.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:21:09.993781 minknow_api-5.5.2/minknow_api/
+-rw-r--r--   0 runner    (1001) docker     (122)    19793 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41104 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/acquisition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25816 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/acquisition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38348 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/acquisition_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74712 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/analysis_configuration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37700 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/analysis_configuration_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54619 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/analysis_configuration_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32426 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/basecaller_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26230 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/basecaller_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40149 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/basecaller_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/ca.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50659 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28044 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39259 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/data_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54186 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54406 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/device_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69791 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/device_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:21:09.993781 minknow_api-5.5.2/minknow_api/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7071 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/examples/export_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/examples/extract_run_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/examples/list_sequencing_positions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14503 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/examples/load_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/examples/run_after_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22311 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/examples/start_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17596 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18886 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/instance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20779 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/instance_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8751 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/keystore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11607 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/keystore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15100 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/keystore_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6107 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6377 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8935 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22777 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63973 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/manager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61829 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/manager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    76769 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/manager_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20793 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/minion_device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6533 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/minion_device_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23361 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/minion_device_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/post_processing_protocol_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24878 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/promethion_device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14303 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/promethion_device_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20850 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/promethion_device_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44096 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/protocol_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49055 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/protocol_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    59688 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/protocol_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9019 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/protocol_settings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/protocol_settings_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/protocol_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5840 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/report_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/report_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/report_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/rpc_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17803 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/run_until_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37760 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/run_until_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27474 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/run_until_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39520 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/statistics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22009 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/statistics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37254 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/statistics_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9175 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:21:09.993781 minknow_api-5.5.2/minknow_api/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/tools/any_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19003 2023-05-17 09:20:59.000000 minknow_api-5.5.2/minknow_api/tools/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:21:09.993781 minknow_api-5.5.2/minknow_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14548 2023-05-17 09:21:09.000000 minknow_api-5.5.2/minknow_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2437 2023-05-17 09:21:09.000000 minknow_api-5.5.2/minknow_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 09:21:09.000000 minknow_api-5.5.2/minknow_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-17 09:21:09.000000 minknow_api-5.5.2/minknow_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 09:21:09.000000 minknow_api-5.5.2/minknow_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 09:21:09.993781 minknow_api-5.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-05-17 09:20:59.000000 minknow_api-5.5.2/setup.py
```

### Comparing `minknow_api-5.4.0/PKG-INFO` & `minknow_api-5.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minknow_api
-Version: 5.4.0
+Version: 5.5.2
 Summary: MinKNOW RPC API bindings
 Home-page: https://github.com/nanoporetech/minknow_api
 Author: Oxford Nanopore Technologies PLC
 Author-email: info@nanoporetech.com
 Description-Content-Type: text/markdown
 
 ![.](docs/images/ONT_logo.png "Oxford Nanopore Technologies")
```

### Comparing `minknow_api-5.4.0/README.md` & `minknow_api-5.5.2/README.md`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/__init__.py` & `minknow_api-5.5.2/minknow_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,15 @@
     else:
         logger.debug("No protocol token found")
         return None
 
 
 def get_local_auth_token_credentials(manager_port):
     local_auth_path = get_local_authentication_token_file(port=manager_port)
+    logger.debug("Retrieving local token from file: '%s'", local_auth_path)
     if local_auth_path:
         if os.path.exists(local_auth_path):
             return grpc.metadata_call_credentials(
                 LocalAuthTokenCredentials(local_auth_path)
             )
         else:
             logger.warn(
@@ -422,15 +423,17 @@
     try:
         cache = grpc_credentials.cached_credentials
     except AttributeError:
         cache = dict()
         grpc_credentials.cached_credentials = cache
 
     try:
-        return cache[cache_key]
+        creds = cache[cache_key]
+        logger.debug("Using grpc credentials with cache key: (%s)", cache_key)
+        return creds
     except KeyError:
         pass
 
     creds = load_grpc_credentials(manager_port, developer_api_token, host)
     cache[cache_key] = creds
     return creds
```

### Comparing `minknow_api-5.4.0/minknow_api/_support.py` & `minknow_api-5.5.2/minknow_api/_support.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/acquisition_pb2.py` & `minknow_api-5.5.2/minknow_api/manager_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,982 +1,846 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: minknow_api/acquisition.proto
+# source: minknow_api/manager.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from minknow_api import run_until_pb2 as minknow__api_dot_run__until__pb2
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
+from minknow_api import device_pb2 as minknow__api_dot_device__pb2
+from minknow_api import instance_pb2 as minknow__api_dot_instance__pb2
+from minknow_api import protocol_settings_pb2 as minknow__api_dot_protocol__settings__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dminknow_api/acquisition.proto\x12\x17minknow_api.acquisition\x1a\x1bminknow_api/run_until.proto\x1a\x1dminknow_api/rpc_options.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd3\x03\n\x0cStartRequest\x12\"\n\x1a\x64ont_wait_for_device_ready\x18\x02 \x01(\x08\x12\x38\n\x0fgenerate_report\x18\x03 \x01(\x0e\x32\x1f.minknow_api.acquisition.Option\x12\x45\n\x1csend_sequencing_read_metrics\x18\x04 \x01(\x0e\x32\x1f.minknow_api.acquisition.Option\x12\x41\n\x18send_basecalling_metrics\x18\x05 \x01(\x0e\x32\x1f.minknow_api.acquisition.Option\x12\x31\n\x07purpose\x18\x06 \x01(\x0e\x32 .minknow_api.acquisition.Purpose\x12\x31\n\x08\x61nalysis\x18\x07 \x01(\x0e\x32\x1f.minknow_api.acquisition.Option\x12\x34\n\x0b\x66ile_output\x18\x08 \x01(\x0e\x32\x1f.minknow_api.acquisition.Option\x12?\n\x16generate_final_summary\x18\t \x01(\x0e\x32\x1f.minknow_api.acquisition.Option\"\x1f\n\rStartResponse\x12\x0e\n\x06run_id\x18\x01 \x01(\t\"\xe0\x01\n\x0bStopRequest\x12L\n\x13\x64\x61ta_action_on_stop\x18\x01 \x01(\x0e\x32/.minknow_api.acquisition.StopRequest.DataAction\x12\x18\n\x10wait_until_ready\x18\x02 \x01(\x08\x12\x15\n\rkeep_power_on\x18\x03 \x01(\x08\"R\n\nDataAction\x12\x10\n\x0cSTOP_DEFAULT\x10\x00\x12\x16\n\x12STOP_KEEP_ALL_DATA\x10\x01\x12\x1a\n\x16STOP_FINISH_PROCESSING\x10\x02\"\x0e\n\x0cStopResponse\"+\n\x1bWatchForStatusChangeRequest\x12\x0c\n\x04stop\x18\x01 \x01(\x08\"V\n\x1cWatchForStatusChangeResponse\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.minknow_api.acquisition.MinknowStatus\"\x16\n\x14\x43urrentStatusRequest\"O\n\x15\x43urrentStatusResponse\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.minknow_api.acquisition.MinknowStatus\"\x14\n\x12GetProgressRequest\"\xa0\x01\n\x13GetProgressResponse\x12S\n\x0fraw_per_channel\x18\x01 \x01(\x0b\x32:.minknow_api.acquisition.GetProgressResponse.RawPerChannel\x1a\x34\n\rRawPerChannel\x12\x10\n\x08\x61\x63quired\x18\x01 \x01(\x04\x12\x11\n\tprocessed\x18\x02 \x01(\x04\".\n\x1cGetAcquisitionRunInfoRequest\x12\x0e\n\x06run_id\x18\x01 \x01(\t\"\x96\x04\n\x17\x41\x63quisitionYieldSummary\x12\x12\n\nread_count\x18\x01 \x01(\x03\x12\x1b\n\x13\x66raction_basecalled\x18\x14 \x01(\x02\x12\x18\n\x10\x66raction_skipped\x18\x15 \x01(\x02\x12\"\n\x1a\x62\x61secalled_pass_read_count\x18\x03 \x01(\x03\x12\"\n\x1a\x62\x61secalled_fail_read_count\x18\x04 \x01(\x03\x12%\n\x1d\x62\x61secalled_skipped_read_count\x18\n \x01(\x03\x12\x1d\n\x15\x62\x61secalled_pass_bases\x18\x05 \x01(\x03\x12\x1d\n\x15\x62\x61secalled_fail_bases\x18\x12 \x01(\x03\x12\x1a\n\x12\x62\x61secalled_samples\x18\x06 \x01(\x03\x12\x1c\n\x14selected_raw_samples\x18\x07 \x01(\x03\x12\x17\n\x0fselected_events\x18\x08 \x01(\x03\x12 \n\x18\x65stimated_selected_bases\x18\t \x01(\x03\x12\x19\n\x11\x61lignment_matches\x18\x0e \x01(\x03\x12\x1c\n\x14\x61lignment_mismatches\x18\x0f \x01(\x03\x12\x1c\n\x14\x61lignment_insertions\x18\x10 \x01(\x03\x12\x1b\n\x13\x61lignment_deletions\x18\x11 \x01(\x03\x12\x1a\n\x12\x61lignment_coverage\x18\x13 \x01(\x02\"\x96\x01\n\x18\x41\x63quisitionWriterSummary\x12\x1f\n\x17\x62ytes_to_write_produced\x18\x02 \x01(\x03\x12\x1d\n\x15\x62ytes_to_write_failed\x18\x03 \x01(\x03\x12 \n\x18\x62ytes_to_write_completed\x18\x04 \x01(\x03J\x04\x08\x01\x10\x02R\x12written_read_count\"\xb0\x03\n\x10\x43hannelStateInfo\x12?\n\x06groups\x18\x01 \x03(\x0b\x32/.minknow_api.acquisition.ChannelStateInfo.Group\x1a;\n\x05Style\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06\x63olour\x18\x03 \x01(\t\x1a~\n\x0c\x43hannelState\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12>\n\x05style\x18\x03 \x01(\x0b\x32/.minknow_api.acquisition.ChannelStateInfo.Style\x12\x14\n\x0cglobal_order\x18\x04 \x01(\r\x1a\x9d\x01\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\x12>\n\x05style\x18\x02 \x01(\x0b\x32/.minknow_api.acquisition.ChannelStateInfo.Style\x12\x46\n\x06states\x18\x03 \x03(\x0b\x32\x36.minknow_api.acquisition.ChannelStateInfo.ChannelState\"\x9f\x05\n\x18\x41\x63quisitionConfigSummary\x12\x31\n\x07purpose\x18\x15 \x01(\x0e\x32 .minknow_api.acquisition.Purpose\x12\x1b\n\x13\x62\x61secalling_enabled\x18\x01 \x01(\x08\x12#\n\x1b\x62\x61secalling_config_filename\x18\x10 \x01(\t\x12\x19\n\x11\x62\x61rcoding_enabled\x18\r \x01(\x08\x12\x16\n\x0e\x62\x61rcoding_kits\x18\x11 \x03(\t\x12\x19\n\x11\x61lignment_enabled\x18\x0e \x01(\x08\x12!\n\x19\x61lignment_reference_files\x18\x12 \x03(\t\x12\x1a\n\x12\x61lignment_bed_file\x18\x13 \x01(\t\x12\x14\n\x0clamp_enabled\x18\x0f \x01(\x08\x12\x10\n\x08lamp_kit\x18\x14 \x01(\t\x12\x17\n\x0freads_directory\x18\x02 \x01(\t\x12\"\n\x1areads_fallback_directories\x18\x03 \x03(\t\x12\x1b\n\x13\x66\x61st5_reads_enabled\x18\x04 \x01(\x08\x12\x1b\n\x13\x66\x61stq_reads_enabled\x18\x05 \x01(\x08\x12\x1e\n\x16protobuf_reads_enabled\x18\x06 \x01(\x08\x12\x16\n\x0e\x62ulk_file_path\x18\x07 \x01(\t\x12\x19\n\x11\x62ulk_file_enabled\x18\x08 \x01(\x08\x12\x45\n\x12\x63hannel_state_info\x18\t \x01(\x0b\x32).minknow_api.acquisition.ChannelStateInfo\x12\x1c\n\x14\x65vents_to_base_ratio\x18\n \x01(\x02\x12\x13\n\x0bsample_rate\x18\x0b \x01(\r\x12\x15\n\rchannel_count\x18\x0c \x01(\r\"\xd6\x03\n\x0fMuxScanMetadata\x12\"\n\x1a\x61uto_mux_scan_period_hours\x18\x01 \x01(\x02\x12O\n\x0f\x63\x61tegory_groups\x18\x02 \x03(\x0b\x32\x36.minknow_api.acquisition.MuxScanMetadata.CategoryGroup\x1a;\n\x05Style\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06\x63olour\x18\x03 \x01(\t\x1am\n\x08\x43\x61tegory\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\x05style\x18\x02 \x01(\x0b\x32..minknow_api.acquisition.MuxScanMetadata.Style\x12\x14\n\x0cglobal_order\x18\x03 \x01(\r\x1a\xa1\x01\n\rCategoryGroup\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\x05style\x18\x02 \x01(\x0b\x32..minknow_api.acquisition.MuxScanMetadata.Style\x12\x43\n\x08\x63\x61tegory\x18\x03 \x03(\x0b\x32\x31.minknow_api.acquisition.MuxScanMetadata.Category\"\x9e\x01\n\rMuxScanResult\x12\x42\n\x06\x63ounts\x18\x01 \x03(\x0b\x32\x32.minknow_api.acquisition.MuxScanResult.CountsEntry\x12\x1a\n\x12mux_scan_timestamp\x18\x02 \x01(\x04\x1a-\n\x0b\x43ountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"\x93\x03\n\tBreamInfo\x12\x43\n\x11mux_scan_metadata\x18\x01 \x01(\x0b\x32(.minknow_api.acquisition.MuxScanMetadata\x12@\n\x10mux_scan_results\x18\x02 \x03(\x0b\x32&.minknow_api.acquisition.MuxScanResult\x12L\n\x1atarget_translocation_speed\x18\x03 \x01(\x0b\x32(.minknow_api.acquisition.BreamInfo.Range\x12@\n\x0etarget_q_score\x18\x04 \x01(\x0b\x32(.minknow_api.acquisition.BreamInfo.Range\x12\x44\n\x12target_temperature\x18\x05 \x01(\x0b\x32(.minknow_api.acquisition.BreamInfo.Range\x1a)\n\x05Range\x12\x0f\n\x07minimum\x18\x01 \x01(\x01\x12\x0f\n\x07maximum\x18\x02 \x01(\x01\"\x95\x01\n\x16TargetRunUntilCriteria\x12=\n\x0epause_criteria\x18\x01 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\x12<\n\rstop_criteria\x18\x02 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\"\xd1\x07\n\x12\x41\x63quisitionRunInfo\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12<\n\rstartup_state\x18\x0c \x01(\x0e\x32%.minknow_api.acquisition.StartupState\x12?\n\x1bstartup_state_estimated_end\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n(startup_state_estimated_percent_complete\x18\x0e \x01(\x02\x12\x38\n\x05state\x18\x02 \x01(\x0e\x32).minknow_api.acquisition.AcquisitionState\x12@\n\x0f\x66inishing_state\x18\n \x01(\x0e\x32\'.minknow_api.acquisition.FinishingState\x12\x43\n\x0bstop_reason\x18\x03 \x01(\x0e\x32..minknow_api.acquisition.AcquisitionStopReason\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x64\x61ta_read_start_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12\x64\x61ta_read_end_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12G\n\ryield_summary\x18\x08 \x01(\x0b\x32\x30.minknow_api.acquisition.AcquisitionYieldSummary\x12I\n\x0e\x63onfig_summary\x18\t \x01(\x0b\x32\x31.minknow_api.acquisition.AcquisitionConfigSummary\x12I\n\x0ewriter_summary\x18\x0b \x01(\x0b\x32\x31.minknow_api.acquisition.AcquisitionWriterSummary\x12\x36\n\nbream_info\x18\x0f \x01(\x0b\x32\".minknow_api.acquisition.BreamInfo\x12R\n\x19target_run_until_criteria\x18\x10 \x01(\x0b\x32/.minknow_api.acquisition.TargetRunUntilCriteria\"\x1c\n\x1aListAcquisitionRunsRequest\".\n\x1bListAcquisitionRunsResponse\x12\x0f\n\x07run_ids\x18\x01 \x03(\t\"!\n\x1fGetCurrentAcquisitionRunRequest\"#\n!WatchCurrentAcquisitionRunRequest\"\xdf\x02\n\x16SetSignalReaderRequest\x12V\n\x06reader\x18\x01 \x01(\x0e\x32@.minknow_api.acquisition.SetSignalReaderRequest.SignalReaderTypeB\x04\x88\xb5\x18\x01\x12\x12\n\nhdf_source\x18\x02 \x01(\t\x12P\n\x08hdf_mode\x18\x03 \x01(\x0e\x32>.minknow_api.acquisition.SetSignalReaderRequest.SourceFileMode\x12 \n\x18sample_rate_scale_factor\x18\x04 \x01(\x02\"(\n\x10SignalReaderType\x12\x08\n\x04HDF5\x10\x00\x12\n\n\x06\x44\x45VICE\x10\x01\";\n\x0eSourceFileMode\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nSINGLE_RUN\x10\x01\x12\x08\n\x04LOOP\x10\x02\"\x19\n\x17SetSignalReaderResponse\"g\n\x13SetBreamInfoRequest\x12\x30\n\x04info\x18\x01 \x01(\x0b\x32\".minknow_api.acquisition.BreamInfo\x12\x1e\n\x16overwrite_unset_fields\x18\x02 \x01(\x08\"\x16\n\x14SetBreamInfoResponse\"\x1d\n\x1b\x41ppendMuxScanResultResponse*Y\n\rMinknowStatus\x12\x10\n\x0c\x45RROR_STATUS\x10\x00\x12\t\n\x05READY\x10\x01\x12\x0c\n\x08STARTING\x10\x02\x12\x0e\n\nPROCESSING\x10\x03\x12\r\n\tFINISHING\x10\x04**\n\x06Option\x12\x08\n\x04\x41UTO\x10\x00\x12\x0b\n\x07\x44ISABLE\x10\x01\x12\t\n\x05\x46ORCE\x10\x02*=\n\x07Purpose\x12\x11\n\rOTHER_PURPOSE\x10\x00\x12\x0e\n\nSEQUENCING\x10\x02\x12\x0f\n\x0b\x43\x41LIBRATION\x10\x03*{\n\x10\x41\x63quisitionState\x12\x18\n\x14\x41\x43QUISITION_STARTING\x10\x00\x12\x17\n\x13\x41\x43QUISITION_RUNNING\x10\x01\x12\x19\n\x15\x41\x43QUISITION_FINISHING\x10\x02\x12\x19\n\x15\x41\x43QUISITION_COMPLETED\x10\x03*\xb2\x02\n\x15\x41\x63quisitionStopReason\x12\x13\n\x0fSTOPPED_NOT_SET\x10\x00\x12\x1a\n\x16STOPPED_USER_REQUESTED\x10\x01\x12\x19\n\x15STOPPED_NO_DISK_SPACE\x10\x02\x12&\n\"STOPPED_DEVICE_STOPPED_ACQUISITION\x10\x03\x12 \n\x1cSTOPPED_STARTING_ANOTHER_RUN\x10\x04\x12\x1a\n\x16STOPPED_PROTOCOL_ENDED\x10\x05\x12\x18\n\x14STOPPED_DEVICE_ERROR\x10\x06\x12\x1b\n\x17STOPPED_BAD_TEMPERATURE\x10\x07\x12\x14\n\x10STOPPED_SHUTDOWN\x10\x08\x12\x1a\n\x16STOPPED_INTERNAL_ERROR\x10\t*\x96\x02\n\x0cStartupState\x12\x13\n\x0fSTARTUP_UNKNOWN\x10\x00\x12\x1d\n\x19STARTUP_BUILDING_PIPELINE\x10\x02\x12#\n\x1fSTARTUP_INITIALISING_BASECALLER\x10\x03\x12-\n)STARTUP_INITIALISING_BASECALLER_ALIGNMENT\x10\x04\x12%\n!STARTUP_INITIALISING_DATA_WRITERS\x10\x05\x12\x32\n.STARTUP_INITIALISING_INTERMEDIATE_DATA_STORAGE\x10\x06\x12#\n\x1fSTARTUP_INITIALISING_STATISTICS\x10\x07*\x8b\x01\n\x0e\x46inishingState\x12\x15\n\x11\x46INISHING_UNKNOWN\x10\x00\x12&\n\"FINISHING_PROCESSING_DEVICE_SIGNAL\x10\x01\x12\x1f\n\x1b\x46INISHING_BASECALLING_READS\x10\x02\x12\x19\n\x15\x46INISHING_SAVING_DATA\x10\x03\x32\xd4\x0b\n\x12\x41\x63quisitionService\x12X\n\x05start\x12%.minknow_api.acquisition.StartRequest\x1a&.minknow_api.acquisition.StartResponse\"\x00\x12U\n\x04stop\x12$.minknow_api.acquisition.StopRequest\x1a%.minknow_api.acquisition.StopResponse\"\x00\x12\x8f\x01\n\x17watch_for_status_change\x12\x34.minknow_api.acquisition.WatchForStatusChangeRequest\x1a\x35.minknow_api.acquisition.WatchForStatusChangeResponse\"\x03\x90\x02\x01(\x01\x30\x01\x12\x8f\x01\n\x1dwatch_current_acquisition_run\x12:.minknow_api.acquisition.WatchCurrentAcquisitionRunRequest\x1a+.minknow_api.acquisition.AcquisitionRunInfo\"\x03\x90\x02\x01\x30\x01\x12t\n\x0e\x63urrent_status\x12-.minknow_api.acquisition.CurrentStatusRequest\x1a..minknow_api.acquisition.CurrentStatusResponse\"\x03\x90\x02\x01\x12n\n\x0cget_progress\x12+.minknow_api.acquisition.GetProgressRequest\x1a,.minknow_api.acquisition.GetProgressResponse\"\x03\x90\x02\x01\x12\x7f\n\x14get_acquisition_info\x12\x35.minknow_api.acquisition.GetAcquisitionRunInfoRequest\x1a+.minknow_api.acquisition.AcquisitionRunInfo\"\x03\x90\x02\x01\x12\x87\x01\n\x15list_acquisition_runs\x12\x33.minknow_api.acquisition.ListAcquisitionRunsRequest\x1a\x34.minknow_api.acquisition.ListAcquisitionRunsResponse\"\x03\x90\x02\x01\x12\x89\x01\n\x1bget_current_acquisition_run\x12\x38.minknow_api.acquisition.GetCurrentAcquisitionRunRequest\x1a+.minknow_api.acquisition.AcquisitionRunInfo\"\x03\x90\x02\x01\x12{\n\x11set_signal_reader\x12/.minknow_api.acquisition.SetSignalReaderRequest\x1a\x30.minknow_api.acquisition.SetSignalReaderResponse\"\x03\x90\x02\x02\x12r\n\x0eset_bream_info\x12,.minknow_api.acquisition.SetBreamInfoRequest\x1a-.minknow_api.acquisition.SetBreamInfoResponse\"\x03\x90\x02\x02\x12{\n\x16\x61ppend_mux_scan_result\x12&.minknow_api.acquisition.MuxScanResult\x1a\x34.minknow_api.acquisition.AppendMuxScanResultResponse\"\x03\x90\x02\x02\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19minknow_api/manager.proto\x12\x13minknow_api.manager\x1a\x1dminknow_api/rpc_options.proto\x1a\x18minknow_api/device.proto\x1a\x1aminknow_api/instance.proto\x1a#minknow_api/protocol_settings.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x15\n\x13\x44\x65scribeHostRequest\"\xad\x03\n\x14\x44\x65scribeHostResponse\x12\x14\n\x0cproduct_code\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06serial\x18\x03 \x01(\t\x12\x14\n\x0cnetwork_name\x18\x04 \x01(\t\x12\x19\n\x11needs_association\x18\x10 \x01(\x08\x12\x1c\n\x14\x63\x61n_sequence_offline\x18\x05 \x01(\x08\x12W\n\x0c\x63\x61n_basecall\x18\x06 \x01(\x0e\x32\x41.minknow_api.manager.DescribeHostResponse.BasecallingAvailability\"\xb1\x01\n\x17\x42\x61secallingAvailability\x12\x19\n\x15\x42\x41SECALLING_AVAILABLE\x10\x00\x12\x1b\n\x17\x42\x41SECALLING_UNAVAILABLE\x10\x01\x12-\n)BASECALLING_UNAVAILABLE_BAD_CONFIGURATION\x10\x02\x12/\n+BASECALLING_UNAVAILABLE_ATTEMPTING_RECOVERY\x10\x03\"\xf3\x06\n\x10\x46lowCellPosition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12@\n\x08location\x18\x02 \x01(\x0b\x32..minknow_api.manager.FlowCellPosition.Location\x12:\n\x05state\x18\x03 \x01(\x0e\x32+.minknow_api.manager.FlowCellPosition.State\x12\x41\n\trpc_ports\x18\x04 \x01(\x0b\x32..minknow_api.manager.FlowCellPosition.RpcPorts\x12\x12\n\nerror_info\x18\x05 \x01(\t\x12X\n\x15shared_hardware_group\x18\x06 \x01(\x0b\x32\x39.minknow_api.manager.FlowCellPosition.SharedHardwareGroup\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\x12\x1c\n\x14\x63\x61n_sequence_offline\x18\x08 \x01(\x08\x12@\n\x0eprotocol_state\x18\t \x01(\x0e\x32(.minknow_api.manager.SimpleProtocolState\x12\x14\n\x0cis_simulated\x18\n \x01(\x08\x12I\n\x0b\x64\x65vice_type\x18\x0b \x01(\x0e\x32\x34.minknow_api.device.GetDeviceInfoResponse.DeviceType\x12\x13\n\x0bparent_name\x18\x0c \x01(\t\x1a \n\x08Location\x12\t\n\x01x\x18\x01 \x01(\x05\x12\t\n\x01y\x18\x02 \x01(\x05\x1a\x33\n\x08RpcPorts\x12\x0e\n\x06secure\x18\x01 \x01(\r\x12\x17\n\x0fsecure_grpc_web\x18\x03 \x01(\r\x1a\'\n\x13SharedHardwareGroup\x12\x10\n\x08group_id\x18\x01 \x01(\r\"\xb4\x01\n\x05State\x12\x16\n\x12STATE_INITIALISING\x10\x00\x12\x11\n\rSTATE_RUNNING\x10\x01\x12\x13\n\x0fSTATE_RESETTING\x10\x02\x12\x1a\n\x16STATE_HARDWARE_REMOVED\x10\x03\x12\x18\n\x14STATE_HARDWARE_ERROR\x10\x04\x12\x18\n\x14STATE_SOFTWARE_ERROR\x10\x05\x12\x1b\n\x17STATE_NEEDS_ASSOCIATION\x10\x06\"\x1a\n\x18\x46lowCellPositionsRequest\"j\n\x19\x46lowCellPositionsResponse\x12\x13\n\x0btotal_count\x18\x01 \x01(\x05\x12\x38\n\tpositions\x18\x02 \x03(\x0b\x32%.minknow_api.manager.FlowCellPosition\"\x1f\n\x1dWatchFlowCellPositionsRequest\"\xa4\x01\n\x1eWatchFlowCellPositionsResponse\x12\x38\n\tadditions\x18\x01 \x03(\x0b\x32%.minknow_api.manager.FlowCellPosition\x12\x36\n\x07\x63hanges\x18\x02 \x03(\x0b\x32%.minknow_api.manager.FlowCellPosition\x12\x10\n\x08removals\x18\x03 \x03(\t\"8\n\x14ResetPositionRequest\x12\x11\n\tpositions\x18\x03 \x03(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\x17\n\x15ResetPositionResponse\"\x16\n\x14\x42\x61secallerApiRequest\"@\n\x15\x42\x61secallerApiResponse\x12\x0e\n\x06secure\x18\x01 \x01(\r\x12\x17\n\x0fsecure_grpc_web\x18\x03 \x01(\r\"\x15\n\x13GetGuppyInfoRequest\"^\n\x14GetGuppyInfoResponse\x12\x0e\n\x04port\x18\x01 \x01(\rH\x00\x12\x12\n\x08ipc_path\x18\x03 \x01(\tH\x00\x12\x0f\n\x07version\x18\x02 \x01(\tB\x11\n\x0f\x63onnection_type\"\x17\n\x15GetVersionInfoRequest\"1\n!ListProtocolOutputDirFilesRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\"\xf8\x01\n\"ListProtocolOutputDirFilesResponse\x12Z\n\x0b\x64irectories\x18\x01 \x03(\x0b\x32\x45.minknow_api.manager.ListProtocolOutputDirFilesResponse.DirectoryInfo\x12\r\n\x05\x66iles\x18\x02 \x03(\t\x12\x1b\n\x13\x63urrent_listed_path\x18\x03 \x01(\t\x1aJ\n\rDirectoryInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0f\x64irectory_count\x18\x02 \x01(\x05\x12\x12\n\nfile_count\x18\x03 \x01(\x05\";\n\x16\x43reateDirectoryRequest\x12\x13\n\x0bparent_path\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\'\n\x17\x43reateDirectoryResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\"\x87\x02\n\x17\x46ilesystemDiskSpaceInfo\x12\x15\n\rfilesystem_id\x18\x01 \x01(\t\x12\x17\n\x0f\x62ytes_available\x18\x02 \x01(\x04\x12\x16\n\x0e\x62ytes_capacity\x18\x03 \x01(\x04\x12\x19\n\x11\x66ile_types_stored\x18\x04 \x03(\t\x12\x1d\n\x15\x62ytes_to_stop_cleanly\x18\x05 \x01(\x04\x12\x1f\n\x17\x62ytes_when_alert_issued\x18\x06 \x01(\x04\x12\x17\n\x0frecommend_alert\x18\x07 \x01(\x08\x12\x16\n\x0erecommend_stop\x18\x08 \x01(\x08\x12\x18\n\x10\x62ytes_per_second\x18\t \x01(\x03\"\x19\n\x17GetDiskSpaceInfoRequest\",\n\x1aStreamDiskSpaceInfoRequest\x12\x0e\n\x06period\x18\x01 \x01(\r\"l\n\x18GetDiskSpaceInfoResponse\x12P\n\x1a\x66ilesystem_disk_space_info\x18\x01 \x03(\x0b\x32,.minknow_api.manager.FilesystemDiskSpaceInfo\"\x1a\n\x18GetBarcodeKitInfoRequest\"\xa8\x02\n\x19GetBarcodeKitInfoResponse\x12\\\n\x10\x62\x61rcode_kit_info\x18\x01 \x03(\x0b\x32\x42.minknow_api.manager.GetBarcodeKitInfoResponse.BarcodeKitInfoEntry\x1a\x37\n\x0e\x42\x61rcodeKitInfo\x12\x0f\n\x07is_dual\x18\x02 \x01(\x08\x12\x14\n\x0cis_both_ends\x18\x03 \x01(\x08\x1at\n\x13\x42\x61rcodeKitInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12L\n\x05value\x18\x02 \x01(\x0b\x32=.minknow_api.manager.GetBarcodeKitInfoResponse.BarcodeKitInfo:\x02\x38\x01\"\x17\n\x15GetLampKitInfoRequest\"+\n\x16GetLampKitInfoResponse\x12\x11\n\tlamp_kits\x18\x02 \x03(\t\"I\n\x15GetBarcodeKeysRequest\x12\x19\n\x11\x62\x61rcode_kit_names\x18\x01 \x03(\t\x12\x15\n\rlamp_kit_name\x18\x02 \x01(\t\"X\n\x16GetBarcodeKeysResponse\x12\x14\n\x0c\x62\x61rcode_keys\x18\x01 \x03(\t\x12\x11\n\tlamp_keys\x18\x02 \x03(\t\x12\x15\n\rcombined_keys\x18\x03 \x03(\t\"\x19\n\x17GetFlowCellTypesRequest\"\xdc\x01\n\x18GetFlowCellTypesResponse\x12\x41\n\x05types\x18\x01 \x03(\x0b\x32\x32.minknow_api.manager.GetFlowCellTypesResponse.Info\x1a}\n\x04Info\x12\x14\n\x0cproduct_code\x18\x01 \x01(\t\x12\x41\n\x0e\x63onnector_type\x18\x02 \x01(\x0e\x32).minknow_api.device.FlowCellConnectorType\x12\x1c\n\x14\x63\x61nnot_live_basecall\x18\x03 \x01(\x08\":\n\x18GetSequencingKitsRequest\x12\x1e\n\x16\x66low_cell_product_code\x18\x01 \x01(\t\"\xf2\x03\n\x19GetSequencingKitsResponse\x12@\n\x04kits\x18\x01 \x03(\x0b\x32\x32.minknow_api.manager.GetSequencingKitsResponse.Kit\x12\x66\n\x18\x62\x61rcoding_expansion_kits\x18\x02 \x03(\x0b\x32\x44.minknow_api.manager.GetSequencingKitsResponse.BarcodingExpansionKit\x1a\xfb\x01\n\x03Kit\x12\x14\n\x0cproduct_code\x18\x01 \x01(\t\x12 \n\x18\x62\x61rcoding_expansion_kits\x18\x02 \x03(\x05\x12\x1a\n\x12includes_barcoding\x18\x03 \x01(\x08\x12\x10\n\x08lamp_kit\x18\x10 \x01(\x08\x12\x1c\n\x14has_control_protocol\x18\x04 \x01(\x08\x12\x1e\n\x16no_sequencing_protocol\x18\x11 \x01(\x08\x12\x17\n\x0f\x66requently_used\x18\x12 \x01(\x08\x12\x0b\n\x03\x64na\x18\x05 \x01(\x08\x12\x0b\n\x03rna\x18\x06 \x01(\x08\x12\x0b\n\x03pcr\x18\x07 \x01(\x08\x12\x10\n\x08pcr_free\x18\x08 \x01(\x08\x1a-\n\x15\x42\x61rcodingExpansionKit\x12\x14\n\x0cproduct_code\x18\x01 \x01(\t\"m\n\x19\x41\x64\x64SimulatedDeviceRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12<\n\x04type\x18\x02 \x01(\x0e\x32(.minknow_api.manager.SimulatedDeviceTypeB\x04\x88\xb5\x18\x01\"\x1c\n\x1a\x41\x64\x64SimulatedDeviceResponse\"2\n\x1cRemoveSimulatedDeviceRequest\x12\x12\n\x04name\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"\x1f\n\x1dRemoveSimulatedDeviceResponse\"%\n#LocalAuthenticationTokenPathRequest\"4\n$LocalAuthenticationTokenPathResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\"7\n\'GetAlignmentReferenceInformationRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\"\x97\x01\n(GetAlignmentReferenceInformationResponse\x12#\n\x1b\x65stimated_load_time_seconds\x18\x01 \x01(\x02\x12&\n\x1e\x65stimated_reference_size_bases\x18\x02 \x01(\x04\x12\x1e\n\x16recommended_live_usage\x18\x03 \x01(\x08\"D\n\x1c\x41ssociationDeviceCodeRequest\x12\x15\n\rposition_name\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03R\x07offline\"-\n\x1d\x41ssociationDeviceCodeResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"V\n(ApplyOfflineAssociationUnlockCodeRequest\x12\x15\n\rposition_name\x18\x01 \x01(\t\x12\x13\n\x0bunlock_code\x18\x02 \x01(\t\"?\n)ApplyOfflineAssociationUnlockCodeResponse\x12\x12\n\nassociated\x18\x01 \x01(\x08\"\x1f\n\x1dListDeveloperApiTokensRequest\"\xd2\x01\n\x1eListDeveloperApiTokensResponse\x12U\n\x06tokens\x18\x01 \x03(\x0b\x32\x45.minknow_api.manager.ListDeveloperApiTokensResponse.DeveloperApiToken\x1aY\n\x11\x44\x65veloperApiToken\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12*\n\x06\x65xpiry\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"Z\n\x1e\x43reateDeveloperApiTokenRequest\x12\x0c\n\x04name\x18\x02 \x01(\t\x12*\n\x06\x65xpiry\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"<\n\x1f\x43reateDeveloperApiTokenResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\",\n\x1eRevokeDeveloperApiTokenRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\"\n RevokeDeveloperApiTokensResponse\"\x8c\x01\n\x14\x46indProtocolsRequest\x12\x1e\n\x16\x66low_cell_product_code\x18\x01 \x01(\t\x12\x16\n\x0esequencing_kit\x18\x02 \x01(\t\x12<\n\x0f\x65xperiment_type\x18\x03 \x01(\x0e\x32#.minknow_api.manager.ExperimentType\"\xc9\x01\n\x15\x46indProtocolsResponse\x12\x46\n\tprotocols\x18\x01 \x03(\x0b\x32\x33.minknow_api.manager.FindProtocolsResponse.Protocol\x1ah\n\x08Protocol\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\'\n\x1frequires_flow_cell_product_code\x18\x02 \x01(\x08\x12\x1f\n\x17requires_sequencing_kit\x18\x03 \x01(\x08\"\xee\x01\n\x1eListSettingsForProtocolRequest\x12\x14\n\nidentifier\x18\x01 \x01(\tH\x00\x12Q\n\ncomponents\x18\x02 \x01(\x0b\x32;.minknow_api.protocol_settings.ProtocolIdentifierComponentsH\x00\x12L\n\x13\x66low_cell_connector\x18\x03 \x01(\x0e\x32).minknow_api.device.FlowCellConnectorTypeB\x04\x88\xb5\x18\x01\x42\x15\n\x13protocol_identifier\"\xa3\"\n\x1fListSettingsForProtocolResponse\x12M\n\x08protocol\x18\x01 \x01(\x0b\x32;.minknow_api.protocol_settings.ProtocolIdentifierComponents\x12T\n\x0brun_options\x18\x02 \x01(\x0b\x32?.minknow_api.manager.ListSettingsForProtocolResponse.RunOptions\x12U\n\x0b\x62\x61secalling\x18\x03 \x01(\x0b\x32@.minknow_api.manager.ListSettingsForProtocolResponse.Basecalling\x12K\n\x06output\x18\x04 \x01(\x0b\x32;.minknow_api.manager.ListSettingsForProtocolResponse.Output\x12I\n\x11protocol_settings\x18\x05 \x03(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x1a\xd5\x06\n\nRunOptions\x12\x42\n\nrun_length\x18\x01 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12\x44\n\x0c\x62ias_voltage\x18\x02 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12J\n\x12read_until_enabled\x18\x03 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12K\n\x13read_until_ref_file\x18\x04 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12K\n\x13read_until_channels\x18\x05 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12S\n\x1bread_until_bed_file_enabled\x18\x06 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12K\n\x13read_until_bed_file\x18\x07 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12M\n\x15read_until_enrichment\x18\x08 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12P\n\x18\x61\x63tive_channel_selection\x18\t \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12G\n\x0fmux_scan_period\x18\n \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12K\n\x13group_change_period\x18\x0b \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x1a\x80\n\n\x0b\x42\x61secalling\x12K\n\x13\x62\x61secalling_enabled\x18\x01 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12I\n\x11\x62\x61rcoding_enabled\x18\x02 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12\x46\n\x0e\x62\x61rcoding_kits\x18\x03 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12\x46\n\x0e\x62\x61secall_model\x18\x04 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12M\n\x15trim_barcodes_enabled\x18\x05 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12R\n\x1arequire_barcodes_both_ends\x18\x06 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12R\n\x1a\x64\x65tect_mid_strand_barcodes\x18\x07 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12T\n\x1coverride_mid_barcoding_score\x18\x08 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12U\n\x1doverride_rear_barcoding_score\x18\t \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12K\n\x13min_barcoding_score\x18\n \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12P\n\x18min_barcoding_score_rear\x18\x0b \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12O\n\x17min_barcoding_score_mid\x18\x0c \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12I\n\x11\x61lignment_enabled\x18\r \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12J\n\x12\x61lignment_ref_file\x18\x0e \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12R\n\x1a\x61lignment_bed_file_enabled\x18\x0f \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12J\n\x12\x61lignment_bed_file\x18\x10 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x1a\x90\x0e\n\x06Output\x12G\n\x0foutput_location\x18\x01 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12\x46\n\x0e\x66\x61st_q_enabled\x18\x02 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12M\n\x15\x66\x61st_q_reads_per_file\x18\x03 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12O\n\x17\x66\x61st_q_data_compression\x18\x04 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12\x46\n\x0e\x66\x61st_5_enabled\x18\x05 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12M\n\x15\x66\x61st_5_reads_per_file\x18\x06 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12O\n\x17\x66\x61st_5_data_trace_table\x18\x07 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12N\n\x16\x66\x61st_5_data_move_table\x18\x08 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12J\n\x12\x66\x61st_5_data_fast_q\x18\t \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12G\n\x0f\x66\x61st_5_data_raw\x18\n \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12O\n\x17\x66\x61st_5_data_compression\x18\x0b \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12\x43\n\x0b\x62\x61m_enabled\x18\x0c \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12N\n\x16read_filtering_enabled\x18\r \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12Q\n\x19read_filtering_min_qscore\x18\x0e \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12V\n\x1eread_filtering_min_read_length\x18\x0f \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12V\n\x1eread_filtering_max_read_length\x18\x10 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12I\n\x11\x62ulk_file_enabled\x18\x11 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12\x45\n\rbulk_file_raw\x18\x12 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12H\n\x10\x62ulk_file_events\x18\x13 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12L\n\x14\x62ulk_file_read_table\x18\x14 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12M\n\x15\x62ulk_file_raw_enabled\x18\x15 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12P\n\x18\x62ulk_file_events_enabled\x18\x16 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\x12T\n\x1c\x62ulk_file_read_table_enabled\x18\x17 \x01(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\"\x1a\n\x07\x46\x65\x61ture\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\"\xe5\x01\n\x0b\x46\x65\x61tureList\x12\x33\n\rfeature_flags\x18\x03 \x01(\x0b\x32\x1c.minknow_api.manager.Feature\x12\x34\n\x0e\x65nrich_deplete\x18\x01 \x01(\x0b\x32\x1c.minknow_api.manager.Feature\x12\x37\n\x11\x62\x61rcode_balancing\x18\x02 \x01(\x0b\x32\x1c.minknow_api.manager.Feature\x12\x32\n\x0c\x64\x61ta_offload\x18\x04 \x01(\x0b\x32\x1c.minknow_api.manager.Feature\"\x14\n\x12GetFeaturesRequest\"\xde\x01\n\x13GetFeaturesResponse\x12=\n\x05state\x18\x01 \x01(\x0e\x32..minknow_api.manager.GetFeaturesResponse.State\x12\x32\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32 .minknow_api.manager.FeatureList\"T\n\x05State\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07NO_FILE\x10\x01\x12\x1b\n\x17\x45RROR_LOADING_FROM_FILE\x10\x02\x12\x14\n\x10LOADED_FROM_FILE\x10\x03\"H\n\x12SetFeaturesRequest\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32 .minknow_api.manager.FeatureList\"\x15\n\x13SetFeaturesResponse*\x88\x01\n\x13SimpleProtocolState\x12\x15\n\x11NO_PROTOCOL_STATE\x10\x00\x12\x14\n\x10PROTOCOL_RUNNING\x10\x01\x12\"\n\x1ePROTOCOL_FINISHED_SUCCESSFULLY\x10\x02\x12 \n\x1cPROTOCOL_FINISHED_WITH_ERROR\x10\x03*\x82\x01\n\x13SimulatedDeviceType\x12\x12\n\x0eSIMULATED_AUTO\x10\x00\x12\x14\n\x10SIMULATED_MINION\x10\x01\x12\x15\n\x11SIMULATED_TRAXION\x10\x02\x12\x18\n\x14SIMULATED_PROMETHION\x10\x03\x12\x10\n\x0cSIMULATED_P2\x10\x04*j\n\x0e\x45xperimentType\x12\x0e\n\nSEQUENCING\x10\x00\x12\x0b\n\x07\x43ONTROL\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x15\n\x11\x41LL_EXCEPT_HIDDEN\x10\x03\x12\x18\n\x14\x41LL_INCLUDING_HIDDEN\x10\x04\x32\xac\x1e\n\x0eManagerService\x12i\n\rdescribe_host\x12(.minknow_api.manager.DescribeHostRequest\x1a).minknow_api.manager.DescribeHostResponse\"\x03\x90\x02\x01\x12{\n\x13\x66low_cell_positions\x12-.minknow_api.manager.FlowCellPositionsRequest\x1a..minknow_api.manager.FlowCellPositionsResponse\"\x03\x90\x02\x01\x30\x01\x12\x8b\x01\n\x19watch_flow_cell_positions\x12\x32.minknow_api.manager.WatchFlowCellPositionsRequest\x1a\x33.minknow_api.manager.WatchFlowCellPositionsResponse\"\x03\x90\x02\x01\x30\x01\x12i\n\x0ereset_position\x12).minknow_api.manager.ResetPositionRequest\x1a*.minknow_api.manager.ResetPositionResponse\"\x00\x12l\n\x0e\x62\x61secaller_api\x12).minknow_api.manager.BasecallerApiRequest\x1a*.minknow_api.manager.BasecallerApiResponse\"\x03\x90\x02\x01\x12j\n\x0eget_guppy_info\x12(.minknow_api.manager.GetGuppyInfoRequest\x1a).minknow_api.manager.GetGuppyInfoResponse\"\x03\x90\x02\x01\x12q\n\x10get_version_info\x12*.minknow_api.manager.GetVersionInfoRequest\x1a,.minknow_api.instance.GetVersionInfoResponse\"\x03\x90\x02\x01\x12\x98\x01\n\x1elist_protocol_output_dir_files\x12\x36.minknow_api.manager.ListProtocolOutputDirFilesRequest\x1a\x37.minknow_api.manager.ListProtocolOutputDirFilesResponse\"\x03\x90\x02\x01\x30\x01\x12r\n\x10\x63reate_directory\x12+.minknow_api.manager.CreateDirectoryRequest\x1a,.minknow_api.manager.CreateDirectoryResponse\"\x03\x90\x02\x02\x12w\n\x13get_disk_space_info\x12,.minknow_api.manager.GetDiskSpaceInfoRequest\x1a-.minknow_api.manager.GetDiskSpaceInfoResponse\"\x03\x90\x02\x01\x12\x88\x01\n\x1eget_default_output_directories\x12\x38.minknow_api.instance.GetDefaultOutputDirectoriesRequest\x1a\'.minknow_api.instance.OutputDirectories\"\x03\x90\x02\x01\x12\x7f\n\x16stream_disk_space_info\x12/.minknow_api.manager.StreamDiskSpaceInfoRequest\x1a-.minknow_api.manager.GetDiskSpaceInfoResponse\"\x03\x90\x02\x01\x30\x01\x12z\n\x14get_barcode_kit_info\x12-.minknow_api.manager.GetBarcodeKitInfoRequest\x1a..minknow_api.manager.GetBarcodeKitInfoResponse\"\x03\x90\x02\x01\x12q\n\x11get_lamp_kit_info\x12*.minknow_api.manager.GetLampKitInfoRequest\x1a+.minknow_api.manager.GetLampKitInfoResponse\"\x03\x90\x02\x01\x12p\n\x10get_barcode_keys\x12*.minknow_api.manager.GetBarcodeKeysRequest\x1a+.minknow_api.manager.GetBarcodeKeysResponse\"\x03\x90\x02\x01\x12{\n\x13get_flow_cell_types\x12,.minknow_api.manager.GetFlowCellTypesRequest\x1a-.minknow_api.manager.GetFlowCellTypesResponse\"\x07\x90\x02\x01\x98\xb5\x18\x01\x12}\n\x13get_sequencing_kits\x12-.minknow_api.manager.GetSequencingKitsRequest\x1a..minknow_api.manager.GetSequencingKitsResponse\"\x07\x90\x02\x01\x98\xb5\x18\x01\x12y\n\x14\x61\x64\x64_simulated_device\x12..minknow_api.manager.AddSimulatedDeviceRequest\x1a/.minknow_api.manager.AddSimulatedDeviceResponse\"\x00\x12\x85\x01\n\x17remove_simulated_device\x12\x31.minknow_api.manager.RemoveSimulatedDeviceRequest\x1a\x32.minknow_api.manager.RemoveSimulatedDeviceResponse\"\x03\x90\x02\x02\x12\x9b\x01\n\x1flocal_authentication_token_path\x12\x38.minknow_api.manager.LocalAuthenticationTokenPathRequest\x1a\x39.minknow_api.manager.LocalAuthenticationTokenPathResponse\"\x03\x90\x02\x01\x12\xa7\x01\n#get_alignment_reference_information\x12<.minknow_api.manager.GetAlignmentReferenceInformationRequest\x1a=.minknow_api.manager.GetAlignmentReferenceInformationResponse\"\x03\x90\x02\x01\x12\x85\x01\n\x17\x61ssociation_device_code\x12\x31.minknow_api.manager.AssociationDeviceCodeRequest\x1a\x32.minknow_api.manager.AssociationDeviceCodeResponse\"\x03\x90\x02\x01\x12\xab\x01\n%apply_offline_association_unlock_code\x12=.minknow_api.manager.ApplyOfflineAssociationUnlockCodeRequest\x1a>.minknow_api.manager.ApplyOfflineAssociationUnlockCodeResponse\"\x03\x90\x02\x02\x12\x89\x01\n\x19list_developer_api_tokens\x12\x32.minknow_api.manager.ListDeveloperApiTokensRequest\x1a\x33.minknow_api.manager.ListDeveloperApiTokensResponse\"\x03\x90\x02\x02\x12\x89\x01\n\x1a\x63reate_developer_api_token\x12\x33.minknow_api.manager.CreateDeveloperApiTokenRequest\x1a\x34.minknow_api.manager.CreateDeveloperApiTokenResponse\"\x00\x12\x8a\x01\n\x1arevoke_developer_api_token\x12\x33.minknow_api.manager.RevokeDeveloperApiTokenRequest\x1a\x35.minknow_api.manager.RevokeDeveloperApiTokensResponse\"\x00\x12m\n\x0e\x66ind_protocols\x12).minknow_api.manager.FindProtocolsRequest\x1a*.minknow_api.manager.FindProtocolsResponse\"\x04\x98\xb5\x18\x01\x12\x90\x01\n\x1alist_settings_for_protocol\x12\x33.minknow_api.manager.ListSettingsForProtocolRequest\x1a\x34.minknow_api.manager.ListSettingsForProtocolResponse\"\x07\x90\x02\x01\x98\xb5\x18\x01\x12j\n\x0cget_features\x12\'.minknow_api.manager.GetFeaturesRequest\x1a(.minknow_api.manager.GetFeaturesResponse\"\x07\x90\x02\x01\x98\xb5\x18\x01\x12g\n\x0cset_features\x12\'.minknow_api.manager.SetFeaturesRequest\x1a(.minknow_api.manager.SetFeaturesResponse\"\x04\x98\xb5\x18\x01\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-_MINKNOWSTATUS = DESCRIPTOR.enum_types_by_name['MinknowStatus']
-MinknowStatus = enum_type_wrapper.EnumTypeWrapper(_MINKNOWSTATUS)
-_OPTION = DESCRIPTOR.enum_types_by_name['Option']
-Option = enum_type_wrapper.EnumTypeWrapper(_OPTION)
-_PURPOSE = DESCRIPTOR.enum_types_by_name['Purpose']
-Purpose = enum_type_wrapper.EnumTypeWrapper(_PURPOSE)
-_ACQUISITIONSTATE = DESCRIPTOR.enum_types_by_name['AcquisitionState']
-AcquisitionState = enum_type_wrapper.EnumTypeWrapper(_ACQUISITIONSTATE)
-_ACQUISITIONSTOPREASON = DESCRIPTOR.enum_types_by_name['AcquisitionStopReason']
-AcquisitionStopReason = enum_type_wrapper.EnumTypeWrapper(_ACQUISITIONSTOPREASON)
-_STARTUPSTATE = DESCRIPTOR.enum_types_by_name['StartupState']
-StartupState = enum_type_wrapper.EnumTypeWrapper(_STARTUPSTATE)
-_FINISHINGSTATE = DESCRIPTOR.enum_types_by_name['FinishingState']
-FinishingState = enum_type_wrapper.EnumTypeWrapper(_FINISHINGSTATE)
-ERROR_STATUS = 0
-READY = 1
-STARTING = 2
-PROCESSING = 3
-FINISHING = 4
-AUTO = 0
-DISABLE = 1
-FORCE = 2
-OTHER_PURPOSE = 0
-SEQUENCING = 2
-CALIBRATION = 3
-ACQUISITION_STARTING = 0
-ACQUISITION_RUNNING = 1
-ACQUISITION_FINISHING = 2
-ACQUISITION_COMPLETED = 3
-STOPPED_NOT_SET = 0
-STOPPED_USER_REQUESTED = 1
-STOPPED_NO_DISK_SPACE = 2
-STOPPED_DEVICE_STOPPED_ACQUISITION = 3
-STOPPED_STARTING_ANOTHER_RUN = 4
-STOPPED_PROTOCOL_ENDED = 5
-STOPPED_DEVICE_ERROR = 6
-STOPPED_BAD_TEMPERATURE = 7
-STOPPED_SHUTDOWN = 8
-STOPPED_INTERNAL_ERROR = 9
-STARTUP_UNKNOWN = 0
-STARTUP_BUILDING_PIPELINE = 2
-STARTUP_INITIALISING_BASECALLER = 3
-STARTUP_INITIALISING_BASECALLER_ALIGNMENT = 4
-STARTUP_INITIALISING_DATA_WRITERS = 5
-STARTUP_INITIALISING_INTERMEDIATE_DATA_STORAGE = 6
-STARTUP_INITIALISING_STATISTICS = 7
-FINISHING_UNKNOWN = 0
-FINISHING_PROCESSING_DEVICE_SIGNAL = 1
-FINISHING_BASECALLING_READS = 2
-FINISHING_SAVING_DATA = 3
-
-
-_STARTREQUEST = DESCRIPTOR.message_types_by_name['StartRequest']
-_STARTRESPONSE = DESCRIPTOR.message_types_by_name['StartResponse']
-_STOPREQUEST = DESCRIPTOR.message_types_by_name['StopRequest']
-_STOPRESPONSE = DESCRIPTOR.message_types_by_name['StopResponse']
-_WATCHFORSTATUSCHANGEREQUEST = DESCRIPTOR.message_types_by_name['WatchForStatusChangeRequest']
-_WATCHFORSTATUSCHANGERESPONSE = DESCRIPTOR.message_types_by_name['WatchForStatusChangeResponse']
-_CURRENTSTATUSREQUEST = DESCRIPTOR.message_types_by_name['CurrentStatusRequest']
-_CURRENTSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['CurrentStatusResponse']
-_GETPROGRESSREQUEST = DESCRIPTOR.message_types_by_name['GetProgressRequest']
-_GETPROGRESSRESPONSE = DESCRIPTOR.message_types_by_name['GetProgressResponse']
-_GETPROGRESSRESPONSE_RAWPERCHANNEL = _GETPROGRESSRESPONSE.nested_types_by_name['RawPerChannel']
-_GETACQUISITIONRUNINFOREQUEST = DESCRIPTOR.message_types_by_name['GetAcquisitionRunInfoRequest']
-_ACQUISITIONYIELDSUMMARY = DESCRIPTOR.message_types_by_name['AcquisitionYieldSummary']
-_ACQUISITIONWRITERSUMMARY = DESCRIPTOR.message_types_by_name['AcquisitionWriterSummary']
-_CHANNELSTATEINFO = DESCRIPTOR.message_types_by_name['ChannelStateInfo']
-_CHANNELSTATEINFO_STYLE = _CHANNELSTATEINFO.nested_types_by_name['Style']
-_CHANNELSTATEINFO_CHANNELSTATE = _CHANNELSTATEINFO.nested_types_by_name['ChannelState']
-_CHANNELSTATEINFO_GROUP = _CHANNELSTATEINFO.nested_types_by_name['Group']
-_ACQUISITIONCONFIGSUMMARY = DESCRIPTOR.message_types_by_name['AcquisitionConfigSummary']
-_MUXSCANMETADATA = DESCRIPTOR.message_types_by_name['MuxScanMetadata']
-_MUXSCANMETADATA_STYLE = _MUXSCANMETADATA.nested_types_by_name['Style']
-_MUXSCANMETADATA_CATEGORY = _MUXSCANMETADATA.nested_types_by_name['Category']
-_MUXSCANMETADATA_CATEGORYGROUP = _MUXSCANMETADATA.nested_types_by_name['CategoryGroup']
-_MUXSCANRESULT = DESCRIPTOR.message_types_by_name['MuxScanResult']
-_MUXSCANRESULT_COUNTSENTRY = _MUXSCANRESULT.nested_types_by_name['CountsEntry']
-_BREAMINFO = DESCRIPTOR.message_types_by_name['BreamInfo']
-_BREAMINFO_RANGE = _BREAMINFO.nested_types_by_name['Range']
-_TARGETRUNUNTILCRITERIA = DESCRIPTOR.message_types_by_name['TargetRunUntilCriteria']
-_ACQUISITIONRUNINFO = DESCRIPTOR.message_types_by_name['AcquisitionRunInfo']
-_LISTACQUISITIONRUNSREQUEST = DESCRIPTOR.message_types_by_name['ListAcquisitionRunsRequest']
-_LISTACQUISITIONRUNSRESPONSE = DESCRIPTOR.message_types_by_name['ListAcquisitionRunsResponse']
-_GETCURRENTACQUISITIONRUNREQUEST = DESCRIPTOR.message_types_by_name['GetCurrentAcquisitionRunRequest']
-_WATCHCURRENTACQUISITIONRUNREQUEST = DESCRIPTOR.message_types_by_name['WatchCurrentAcquisitionRunRequest']
-_SETSIGNALREADERREQUEST = DESCRIPTOR.message_types_by_name['SetSignalReaderRequest']
-_SETSIGNALREADERRESPONSE = DESCRIPTOR.message_types_by_name['SetSignalReaderResponse']
-_SETBREAMINFOREQUEST = DESCRIPTOR.message_types_by_name['SetBreamInfoRequest']
-_SETBREAMINFORESPONSE = DESCRIPTOR.message_types_by_name['SetBreamInfoResponse']
-_APPENDMUXSCANRESULTRESPONSE = DESCRIPTOR.message_types_by_name['AppendMuxScanResultResponse']
-_STOPREQUEST_DATAACTION = _STOPREQUEST.enum_types_by_name['DataAction']
-_SETSIGNALREADERREQUEST_SIGNALREADERTYPE = _SETSIGNALREADERREQUEST.enum_types_by_name['SignalReaderType']
-_SETSIGNALREADERREQUEST_SOURCEFILEMODE = _SETSIGNALREADERREQUEST.enum_types_by_name['SourceFileMode']
-StartRequest = _reflection.GeneratedProtocolMessageType('StartRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STARTREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """ Protobuf messages for input/output of RPC calls
-  
-  Attributes:
-      dont_wait_for_device_ready:
-          Prevent waiting until the device is ready before starting
-          acquisition.  Defaults to false.  By default, MinKNOW will
-          block in the start() call for the device and flow cell to be
-          ready for acquisition (which may take several seconds after
-          plugging in the flow cell on some devices). Setting this
-          option will cause the call to return with an error if the
-          device is not already prepared to acquire data.  Since 1.14
-      generate_report:
-          Generate duty time and throughput reports.  Note that this
-          setting will be ignored (and no reports will be generated) if
-          no protocol is running at the time acquisition is started.
-          The default setting (AUTO) will only generate reports if
-          purpose is set to SEQUENCING.  Since 3.0
-      send_sequencing_read_metrics:
-          Whether sequencing read metrics should be reported to Oxford
-          Nanopore.  These are performance metrics that are used to
-          improve the sequencing technology. They do not include any
-          actual sequencing data, only statistics about read lengths,
-          duty time and similar generic performance information.  The
-          default setting (AUTO) will only send metrics if purpose is
-          set to SEQUENCING.  Since 3.0
-      send_basecalling_metrics:
-          Whether basecalling metrics should be reported to Oxford
-          Nanopore.  These are performance metrics that are used to
-          improve the sequencing technology. They do not include any
-          actual sequencing data, only statistics about basecalling
-          performance.  The default setting (AUTO) will only send
-          metrics if purpose is set to SEQUENCING.  NB: this setting is
-          ignored if live basecalling is not enabled, since there will
-          be no metrics to send.  Since 3.2
-      purpose:
-          Specify the purpose of this acquisition period.  This affects
-          various defaults (see the Purpose enum documentation for more
-          details). It may also affect how the user interface presents
-          the state of the protocol.  Since 3.2
-      analysis:
-          Perform analysis for this acquisition period.  If this is
-          disabled, no reads, no events, no channel states and no
-          basecalls will be generated. Any RPCs that depend on any of
-          these will fail. No reads-based files will be produced at all,
-          regardless of any other settings.  This is mostly useful for
-          calibration (although you should normally use the purpose
-          field rather than setting this explicitly).  The default
-          setting (AUTO) will use the persistent setting from the
-          analysis_configuraiton service, unless the purpose is set to
-          CALIBRATION.  Since 3.2
-      file_output:
-          Allow file output for this acquisition period.  If this is
-          disabled, the file output settings will be ignored for this
-          acquisition period, and no data files will be produced. Note
-          that reports are NOT managed by this setting.  Note that
-          setting this to FORCE will simply make file output respect the
-          bulk and read writer configurations. If each file output type
-          is disabled, you will still get no file output.  This is
-          mostly useful for calibration (although you should normally
-          use the purpose field rather than setting this explicitly).
-          The default setting (AUTO) will only suppress file output if
-          purpose is set to CALIBRATION.  Since 3.2
-      generate_final_summary:
-          Write a final_summary.txt file.  If file_output is disabled,
-          the final_summary.txt file will not be written regardless of
-          this setting.  The default setting (AUTO) will only enable
-          writing a final_summary.txt file if the purpose is set to
-          SEQUENCING.  Since 3.5 (NB: in 3.3 and 3.4, final_summary.txt
-          was always written out if file_output was enabled).
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.StartRequest)
-  })
-_sym_db.RegisterMessage(StartRequest)
-
-StartResponse = _reflection.GeneratedProtocolMessageType('StartResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STARTRESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      run_id:
-          Globally-unique identifier generated when the acquisition is
-          started.  This is guaranteed to unique, including aross
-          sequencing devices.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.StartResponse)
-  })
-_sym_db.RegisterMessage(StartResponse)
-
-StopRequest = _reflection.GeneratedProtocolMessageType('StopRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STOPREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      wait_until_ready:
-          Defaults to false If false will return as soon as minknow
-          enters the FINISHING state. If true then returns as soon as
-          minknow enters the READY state.
-      keep_power_on:
-          Force the MinION/GridION ASIC power to be kept on after the
-          current acquisition finishes  Keeping the ASIC power on has
-          two main effects:       - The flow-cell will remain at the
-          correct operating temperature between acquisitions;
-          this allows following acquisition to be started more quickly.
-          - MinION/GridION flow cells may be damaged if they are removed
-          or plugged in while the        ASIC power is turned on.
-          Therefore, this option should be set to `true` if and only if
-          another acquisition will be performed using the same flow-
-          cell, soon after the acquisition that is being stopped.
-          Otherwise it should be set to `false` (or left unset) to
-          prevent potential damage to MinION/GridION flow-cells.  If
-          this option is set to `false` (or is left unset), then the
-          application configuration determines whether the power will be
-          left on when the acquisition finishes -- see the
-          `powered_when_idle` and `flongle_powered_when_idle`
-          configuration options for further details.  This option has no
-          effect on PromethIONs.  Since 1.15.2
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.StopRequest)
-  })
-_sym_db.RegisterMessage(StopRequest)
-
-StopResponse = _reflection.GeneratedProtocolMessageType('StopResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STOPRESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.StopResponse)
-  })
-_sym_db.RegisterMessage(StopResponse)
-
-WatchForStatusChangeRequest = _reflection.GeneratedProtocolMessageType('WatchForStatusChangeRequest', (_message.Message,), {
-  'DESCRIPTOR' : _WATCHFORSTATUSCHANGEREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.WatchForStatusChangeRequest)
-  })
-_sym_db.RegisterMessage(WatchForStatusChangeRequest)
-
-WatchForStatusChangeResponse = _reflection.GeneratedProtocolMessageType('WatchForStatusChangeResponse', (_message.Message,), {
-  'DESCRIPTOR' : _WATCHFORSTATUSCHANGERESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.WatchForStatusChangeResponse)
-  })
-_sym_db.RegisterMessage(WatchForStatusChangeResponse)
-
-CurrentStatusRequest = _reflection.GeneratedProtocolMessageType('CurrentStatusRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CURRENTSTATUSREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.CurrentStatusRequest)
-  })
-_sym_db.RegisterMessage(CurrentStatusRequest)
-
-CurrentStatusResponse = _reflection.GeneratedProtocolMessageType('CurrentStatusResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CURRENTSTATUSRESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.CurrentStatusResponse)
-  })
-_sym_db.RegisterMessage(CurrentStatusResponse)
-
-GetProgressRequest = _reflection.GeneratedProtocolMessageType('GetProgressRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETPROGRESSREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.GetProgressRequest)
-  })
-_sym_db.RegisterMessage(GetProgressRequest)
-
-GetProgressResponse = _reflection.GeneratedProtocolMessageType('GetProgressResponse', (_message.Message,), {
-
-  'RawPerChannel' : _reflection.GeneratedProtocolMessageType('RawPerChannel', (_message.Message,), {
-    'DESCRIPTOR' : _GETPROGRESSRESPONSE_RAWPERCHANNEL,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """Attributes:
-        acquired:
-            Number of samples (per channel) acquired from the device.
-        processed:
-            Number of samples (per channel) passed to the analysis
-            pipeline for processing.  This can be compared to acquired to
-            see how far behind the analysis is lagging.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.GetProgressResponse.RawPerChannel)
-    })
-  ,
-  'DESCRIPTOR' : _GETPROGRESSRESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      raw_per_channel:
-          The amount of raw data (per channel) that has been acquired
-          and processed.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.GetProgressResponse)
-  })
-_sym_db.RegisterMessage(GetProgressResponse)
-_sym_db.RegisterMessage(GetProgressResponse.RawPerChannel)
-
-GetAcquisitionRunInfoRequest = _reflection.GeneratedProtocolMessageType('GetAcquisitionRunInfoRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETACQUISITIONRUNINFOREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      run_id:
-          The acquisition period to get information about.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.GetAcquisitionRunInfoRequest)
-  })
-_sym_db.RegisterMessage(GetAcquisitionRunInfoRequest)
-
-AcquisitionYieldSummary = _reflection.GeneratedProtocolMessageType('AcquisitionYieldSummary', (_message.Message,), {
-  'DESCRIPTOR' : _ACQUISITIONYIELDSUMMARY,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      read_count:
-          Number of reads selected by analysis as good reads.  The reads
-          in this counter are completed, but not necessarily on disk
-          yet.
-      fraction_basecalled:
-          This is the fraction of whole reads that the base-caller has
-          finished with. The value should be in the range [0.0, 1.0]
-          When base-calling is enabled, it can be added to
-          fraction_skipped and multiplied by 100 to give the percentage
-          of reads processed and by implication, the percentage of reads
-          the user is waiting for the base-caller to process.  Since 5.0
-      fraction_skipped:
-          This is the fraction of whole reads that have been skipped.
-          The value should be in the range [0.0, 1.0]  Since 5.0
-      basecalled_pass_read_count:
-          Number of reads successfully basecalled.
-      basecalled_fail_read_count:
-          Number of reads which have failed to basecall.
-      basecalled_skipped_read_count:
-          Number of reads which have been skipped
-      basecalled_pass_bases:
-          Number of bases which have been called and classed as pass.
-      basecalled_fail_bases:
-          Number of bases which have been called and were classed as
-          fail.
-      basecalled_samples:
-          Number of raw samples which have been called.
-      selected_raw_samples:
-          Number of minknow raw samples which have been selected for
-          writing to disk as reads.
-      selected_events:
-          Number of minknow events which have been selected for writing
-          to disk as reads.
-      estimated_selected_bases:
-          Estimated number of bases MinKNOW has selected for writing.
-          This is estimated based on already called bases and samples.
-      alignment_matches:
-          Number of bases which have matched target reference.  Only
-          specified when running live alignment.  Since 4.0
-      alignment_mismatches:
-          Number of bases which have not matched target reference.  Only
-          specified when running live alignment.  Since 4.0
-      alignment_insertions:
-          Number of bases which were inserted into alignments that
-          matched the reference.  Only specified when running live
-          alignment.  Since 4.0
-      alignment_deletions:
-          Number of bases which were deleted from alignments that
-          matched the reference.  Only specified when running live
-          alignment.  Since 4.0
-      alignment_coverage:
-          Number of bases that match the target reference(s) expressed
-          as a fraction of the total size of the target reference(s).
-          eg: For a specified alignment-targets with 2000 and 3000
-          bases, if "alignment_matches" is 2500, then
-          "alignment_coverage" will be 0.5  Since 4.3
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.AcquisitionYieldSummary)
-  })
-_sym_db.RegisterMessage(AcquisitionYieldSummary)
-
-AcquisitionWriterSummary = _reflection.GeneratedProtocolMessageType('AcquisitionWriterSummary', (_message.Message,), {
-  'DESCRIPTOR' : _ACQUISITIONWRITERSUMMARY,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      bytes_to_write_produced:
-          Number of bytes which minknow needs to write in order to
-          finish the experiment.
-      bytes_to_write_failed:
-          Number of bytes which minknow has failed to write to final
-          location. These reads are instead contained in the
-          fallback/tmp locations.
-      bytes_to_write_completed:
-          Number of bytes which minknow has written to final location.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.AcquisitionWriterSummary)
-  })
-_sym_db.RegisterMessage(AcquisitionWriterSummary)
-
-ChannelStateInfo = _reflection.GeneratedProtocolMessageType('ChannelStateInfo', (_message.Message,), {
-
-  'Style' : _reflection.GeneratedProtocolMessageType('Style', (_message.Message,), {
-    'DESCRIPTOR' : _CHANNELSTATEINFO_STYLE,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """Attributes:
-        label:
-            The human-readable name to display when rendering this channel
-            state or group.
-        description:
-            A sentence describing the meaning of the channel state or
-            group.  This can be used as a tooltip, for example.
-        colour:
-            The colour to use when rendering this channel state or group.
-            This is a six-digit hex string describing an RGB colour (eg:
-            "ff00ff" for purple).
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.ChannelStateInfo.Style)
-    })
-  ,
-
-  'ChannelState' : _reflection.GeneratedProtocolMessageType('ChannelState', (_message.Message,), {
-    'DESCRIPTOR' : _CHANNELSTATEINFO_CHANNELSTATE,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """Attributes:
-        id:
-            The numeric identifier of the state.  This is what is reported
-            in any other APIs that return a channel state ID.
-        name:
-            The internal name of the state.  This is what is reported in
-            any other APIs that return a channel state name.
-        style:
-            How to render the channel state in a graphical user interface.
-            Note that the style may be missing from some channel states
-            (such as the ones that are built in to MinKNOW).
-        global_order:
-            An order ranking for the channel states when they are
-            ungrouped.  This can be used to order the channel states after
-            merging the groups.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.ChannelStateInfo.ChannelState)
-    })
-  ,
-
-  'Group' : _reflection.GeneratedProtocolMessageType('Group', (_message.Message,), {
-    'DESCRIPTOR' : _CHANNELSTATEINFO_GROUP,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """Attributes:
-        name:
-            The name of the group.
-        style:
-            How to render the group in a graphical user interface.  Note
-            that the style may be missing from some groups (such as the
-            ones that are built in to MinKNOW).
-        states:
-            The channel states contained in the group.  The groups are
-            ordered according to the "order" attribute of the channel
-            state style in the channel states configuration.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.ChannelStateInfo.Group)
-    })
-  ,
-  'DESCRIPTOR' : _CHANNELSTATEINFO,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      groups:
-          The groups of channel states.  The groups are ordered
-          according to the "order" attribute of the group style in the
-          channel states configuration.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.ChannelStateInfo)
-  })
-_sym_db.RegisterMessage(ChannelStateInfo)
-_sym_db.RegisterMessage(ChannelStateInfo.Style)
-_sym_db.RegisterMessage(ChannelStateInfo.ChannelState)
-_sym_db.RegisterMessage(ChannelStateInfo.Group)
-
-AcquisitionConfigSummary = _reflection.GeneratedProtocolMessageType('AcquisitionConfigSummary', (_message.Message,), {
-  'DESCRIPTOR' : _ACQUISITIONCONFIGSUMMARY,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      purpose:
-          The purpose, as supplied to `acquisition.start()`
-      basecalling_enabled:
-          Was basecalling enabled for the run.
-      basecalling_config_filename:
-          Basecalling configuration filename (if basecalling enabled)
-      barcoding_enabled:
-          Is barcoding enabled for the run
-      barcoding_kits:
-          / Barcoding kit(s) used (if barcoding enabled)
-      alignment_enabled:
-          Is alignment enabled for the run
-      alignment_reference_files:
-          Alignment reference file(s) used (if alignment enabled)
-      alignment_bed_file:
-          bed file used (if alignment enabled, and bed file specified)
-      lamp_enabled:
-          Is lamp enabled for the run
-      lamp_kit:
-          The LAMP kit used (if LAMP enabled)
-      reads_directory:
-          Root directory reads were written to for the run.  Empty if no
-          reads were enabled.
-      reads_fallback_directories:
-          Directories reads are written to if the reads_directory is on
-          the network and writes to it fail.  Empty if no reads were
-          enabled.
-      fast5_reads_enabled:
-          Determine if fast5 reads were enabled for the run.
-      fastq_reads_enabled:
-          Determine if fastq reads were enabled for the run.
-      protobuf_reads_enabled:
-          Determine if protobuf reads were enabled for the run.
-      bulk_file_path:
-          The path of the bulk file for the run.  Empty if no reads were
-          enabled.
-      bulk_file_enabled:
-          Find if the bulk writer was enabled for a run.
-      channel_state_info:
-          Channel state styling information
-      events_to_base_ratio:
-          Number of bases per event
-      sample_rate:
-          Sample rate for the acquisition.  Since 3.3
-      channel_count:
-          Channel count used in the acquisition.  Since 3.3
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.AcquisitionConfigSummary)
-  })
-_sym_db.RegisterMessage(AcquisitionConfigSummary)
-
-MuxScanMetadata = _reflection.GeneratedProtocolMessageType('MuxScanMetadata', (_message.Message,), {
-
-  'Style' : _reflection.GeneratedProtocolMessageType('Style', (_message.Message,), {
-    'DESCRIPTOR' : _MUXSCANMETADATA_STYLE,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """Presentation information for a category or group.
-    
-    Attributes:
-        label:
-            The human-readable name to display when rendering this
-            category or group.
-        description:
-            A sentence describing the meaning of the category or group.
-            This can be used as a tooltip, for example.
-        colour:
-            The colour to use when rendering this category or group.  This
-            is a six-digit hex string describing an RGB colour (eg:
-            "ff0000" for red).
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.MuxScanMetadata.Style)
-    })
-  ,
-
-  'Category' : _reflection.GeneratedProtocolMessageType('Category', (_message.Message,), {
-    'DESCRIPTOR' : _MUXSCANMETADATA_CATEGORY,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """A category that a channel mux can be assigned.
-    
-    Attributes:
-        name:
-            Name of the category.  This is the value that will be in the
-            `MuxScanResult.counts` field.  The user should not be shown
-            this. Instead, `style.label` should be displayed.
-        style:
-            How to render the category in a graphical user interface.
-        global_order:
-            An order ranking for the category when displaying them without
-            using groups.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.MuxScanMetadata.Category)
-    })
-  ,
-
-  'CategoryGroup' : _reflection.GeneratedProtocolMessageType('CategoryGroup', (_message.Message,), {
-    'DESCRIPTOR' : _MUXSCANMETADATA_CATEGORYGROUP,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """Attributes:
-        name:
-            The name of the group.
-        style:
-            How to render the group in a graphical user interface.
-        category:
-            The categories contained in the group.  Within this group,
-            categories should be presented in the order of this list.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.MuxScanMetadata.CategoryGroup)
-    })
-  ,
-  'DESCRIPTOR' : _MUXSCANMETADATA,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Provides information about how mux scans are configured.  This
-  primarily information to help present mux scan results to the user
-  (see `MuxScanResult`).
-  
-  Attributes:
-      auto_mux_scan_period_hours:
-          How frequently automatic scans are scheduled to occur.
-      category_groups:
-          Presentation information for categories.  Describes the
-          preferred way to present mux scan categories to users. Groups
-          should be presented in the order of this list.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.MuxScanMetadata)
-  })
-_sym_db.RegisterMessage(MuxScanMetadata)
-_sym_db.RegisterMessage(MuxScanMetadata.Style)
-_sym_db.RegisterMessage(MuxScanMetadata.Category)
-_sym_db.RegisterMessage(MuxScanMetadata.CategoryGroup)
-
-MuxScanResult = _reflection.GeneratedProtocolMessageType('MuxScanResult', (_message.Message,), {
-
-  'CountsEntry' : _reflection.GeneratedProtocolMessageType('CountsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _MUXSCANRESULT_COUNTSENTRY,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.MuxScanResult.CountsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _MUXSCANRESULT,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """A report of the states of channel muxes (wells) across the flow cell.
-  Every channel mux (well) is assigned to a specific category describing
-  its state (for example, is it expected to produce good results, and if
-  not why not?). This is a report of how many channel muxes are in each
-  category.
-  
-  Attributes:
-      counts:
-          How many channel muxes are in each category.  The sum of all
-          the values in this map should be the number of channels
-          multiplied by the number of muxes on each channel (eg:
-          512x4=2048 on a MinION Mk1B without a flongle adapter).  eg.
-          'sequencing': 1500
-      mux_scan_timestamp:
-          When this mux scan result was added (Seconds since the start
-          of the acquisition).
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.MuxScanResult)
-  })
-_sym_db.RegisterMessage(MuxScanResult)
-_sym_db.RegisterMessage(MuxScanResult.CountsEntry)
-
-BreamInfo = _reflection.GeneratedProtocolMessageType('BreamInfo', (_message.Message,), {
-
-  'Range' : _reflection.GeneratedProtocolMessageType('Range', (_message.Message,), {
-    'DESCRIPTOR' : _BREAMINFO_RANGE,
-    '__module__' : 'minknow_api.acquisition_pb2'
-    ,
-    '__doc__': """Represents a range of values.""",
-    # @@protoc_insertion_point(class_scope:minknow_api.acquisition.BreamInfo.Range)
-    })
-  ,
-  'DESCRIPTOR' : _BREAMINFO,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Information provided by Bream.  Note that this is provided by the
-  protocol, and some protocols may choose not to provide this.
-  
-  Attributes:
-      mux_scan_metadata:
-          Presentation information for mux scan results.
-      mux_scan_results:
-          Mux scan results.
-      target_translocation_speed:
-          The ideal translocation speed range.  This can be used to
-          provide context for speed graphs (see the statistics RPCs),
-          showing what range is considered "good".
-      target_q_score:
-          The ideal quality (Q) score range.  This can be used to
-          provide context for q-score graphs (see the statistics RPCs),
-          showing what range is considered "good".
-      target_temperature:
-          The ideal temperature range.  This can be used to provide
-          context for temperature (see the statistics RPCs), showing
-          what range is considered "good".  Note that a protocol may
-          request a different temperature range than this (eg: it might
-          request a tighter range, or it may adjust the temperature it
-          is requesting throughout the run). This intended only to
-          provide context when presenting data to users.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.BreamInfo)
-  })
-_sym_db.RegisterMessage(BreamInfo)
-_sym_db.RegisterMessage(BreamInfo.Range)
-
-TargetRunUntilCriteria = _reflection.GeneratedProtocolMessageType('TargetRunUntilCriteria', (_message.Message,), {
-  'DESCRIPTOR' : _TARGETRUNUNTILCRITERIA,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.TargetRunUntilCriteria)
-  })
-_sym_db.RegisterMessage(TargetRunUntilCriteria)
-
-AcquisitionRunInfo = _reflection.GeneratedProtocolMessageType('AcquisitionRunInfo', (_message.Message,), {
-  'DESCRIPTOR' : _ACQUISITIONRUNINFO,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      run_id:
-          The unique identifier assigned to this acquisition run.  This
-          is guaranteed to be made of ASCII characters, and at most 40
-          characters. It is globally unique across all acquisitions on
-          all MinKNOW instances.
-      startup_state:
-          Current startup task (or STARTUP_UNKNOWN if not starting up).
-      startup_state_estimated_end:
-          Estimated time for current startup state to end.  In some
-          cases this field is left unset, to indicate no estimation.
-      startup_state_estimated_percent_complete:
-          Estimate startup state completion percent (0 - 1).  In some
-          cases this field is left at 0, indicating no estimation.
-      state:
-          Indicates the current state of the acquisition.
-      finishing_state:
-          If the experiment is finishing, an extra piece of state
-          describing the current finishing state.
-      stop_reason:
-          The reason the acquisition period was ended.
-      start_time:
-          When the acquisition period was started (UTC).
-      data_read_start_time:
-          When MinKNOW began acquiring data (UTC).  Unset if the
-          acquisition is still starting up.
-      data_read_end_time:
-          When the MinKNOW stopped acquiring data (UTC).  Unset if the
-          acquisition is still acquiring.
-      end_time:
-          When the acquisition terminated (UTC).  Unset if the
-          acquisition period is still running.
-      yield_summary:
-          Summary of acquisition yields.  Since 1.12
-      config_summary:
-          Summary of the configuration settings for a run.  Since 1.14
-      writer_summary:
-          Summary of writer yields.  Since 4.0
-      bream_info:
-          Set information provided by the Bream toolkit.
-      target_run_until_criteria:
-          Target Run-Until Critiera, used to determine when the
-          acquisition should be paused or stopped.  Since 5.3
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.AcquisitionRunInfo)
-  })
-_sym_db.RegisterMessage(AcquisitionRunInfo)
-
-ListAcquisitionRunsRequest = _reflection.GeneratedProtocolMessageType('ListAcquisitionRunsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTACQUISITIONRUNSREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.ListAcquisitionRunsRequest)
-  })
-_sym_db.RegisterMessage(ListAcquisitionRunsRequest)
-
-ListAcquisitionRunsResponse = _reflection.GeneratedProtocolMessageType('ListAcquisitionRunsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LISTACQUISITIONRUNSRESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.ListAcquisitionRunsResponse)
-  })
-_sym_db.RegisterMessage(ListAcquisitionRunsResponse)
-
-GetCurrentAcquisitionRunRequest = _reflection.GeneratedProtocolMessageType('GetCurrentAcquisitionRunRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCURRENTACQUISITIONRUNREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.GetCurrentAcquisitionRunRequest)
-  })
-_sym_db.RegisterMessage(GetCurrentAcquisitionRunRequest)
-
-WatchCurrentAcquisitionRunRequest = _reflection.GeneratedProtocolMessageType('WatchCurrentAcquisitionRunRequest', (_message.Message,), {
-  'DESCRIPTOR' : _WATCHCURRENTACQUISITIONRUNREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.WatchCurrentAcquisitionRunRequest)
-  })
-_sym_db.RegisterMessage(WatchCurrentAcquisitionRunRequest)
-
-SetSignalReaderRequest = _reflection.GeneratedProtocolMessageType('SetSignalReaderRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETSIGNALREADERREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      reader:
-          The type of signal reader to use
-      hdf_source:
-          The following settings are optional, and only used when
-          setting the reader to hdf5
-      hdf_mode:
-           Defaults to UNSPECIFIED, since this setting is optional
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.SetSignalReaderRequest)
-  })
-_sym_db.RegisterMessage(SetSignalReaderRequest)
-
-SetSignalReaderResponse = _reflection.GeneratedProtocolMessageType('SetSignalReaderResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETSIGNALREADERRESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.SetSignalReaderResponse)
-  })
-_sym_db.RegisterMessage(SetSignalReaderResponse)
-
-SetBreamInfoRequest = _reflection.GeneratedProtocolMessageType('SetBreamInfoRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETBREAMINFOREQUEST,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  ,
-  '__doc__': """Attributes:
-      info:
-          The information to set.  Note that, other than treating the
-          top-level fields independently (see the other flags on this
-          request), MinKNOW Core will not do anything special to the
-          data. In particular, the caller must fill in the
-          `mux_scan_timestamp` field in `MuxScanResult` messages.
-      overwrite_unset_fields:
-          If any `BreamInfo` fields were set in a previous call, but are
-          unset in the `info` field of this call, then use the old value
-          for them.  For example, to just update the mux_scan_metadata
-          field, use a BreamInfo object with only the
-          `mux_scan_metadata` field set, and leave this as False. To
-          clear the entire BreamInfo structure, leave `info` empty and
-          set this to True.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.SetBreamInfoRequest)
-  })
-_sym_db.RegisterMessage(SetBreamInfoRequest)
-
-SetBreamInfoResponse = _reflection.GeneratedProtocolMessageType('SetBreamInfoResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETBREAMINFORESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.SetBreamInfoResponse)
-  })
-_sym_db.RegisterMessage(SetBreamInfoResponse)
-
-AppendMuxScanResultResponse = _reflection.GeneratedProtocolMessageType('AppendMuxScanResultResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPENDMUXSCANRESULTRESPONSE,
-  '__module__' : 'minknow_api.acquisition_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.acquisition.AppendMuxScanResultResponse)
-  })
-_sym_db.RegisterMessage(AppendMuxScanResultResponse)
-
-_ACQUISITIONSERVICE = DESCRIPTOR.services_by_name['AcquisitionService']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.manager_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
-  _MUXSCANRESULT_COUNTSENTRY._options = None
-  _MUXSCANRESULT_COUNTSENTRY._serialized_options = b'8\001'
-  _SETSIGNALREADERREQUEST.fields_by_name['reader']._options = None
-  _SETSIGNALREADERREQUEST.fields_by_name['reader']._serialized_options = b'\210\265\030\001'
-  _ACQUISITIONSERVICE.methods_by_name['watch_for_status_change']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['watch_for_status_change']._serialized_options = b'\220\002\001'
-  _ACQUISITIONSERVICE.methods_by_name['watch_current_acquisition_run']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['watch_current_acquisition_run']._serialized_options = b'\220\002\001'
-  _ACQUISITIONSERVICE.methods_by_name['current_status']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['current_status']._serialized_options = b'\220\002\001'
-  _ACQUISITIONSERVICE.methods_by_name['get_progress']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['get_progress']._serialized_options = b'\220\002\001'
-  _ACQUISITIONSERVICE.methods_by_name['get_acquisition_info']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['get_acquisition_info']._serialized_options = b'\220\002\001'
-  _ACQUISITIONSERVICE.methods_by_name['list_acquisition_runs']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['list_acquisition_runs']._serialized_options = b'\220\002\001'
-  _ACQUISITIONSERVICE.methods_by_name['get_current_acquisition_run']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['get_current_acquisition_run']._serialized_options = b'\220\002\001'
-  _ACQUISITIONSERVICE.methods_by_name['set_signal_reader']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['set_signal_reader']._serialized_options = b'\220\002\002'
-  _ACQUISITIONSERVICE.methods_by_name['set_bream_info']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['set_bream_info']._serialized_options = b'\220\002\002'
-  _ACQUISITIONSERVICE.methods_by_name['append_mux_scan_result']._options = None
-  _ACQUISITIONSERVICE.methods_by_name['append_mux_scan_result']._serialized_options = b'\220\002\002'
-  _MINKNOWSTATUS._serialized_start=6030
-  _MINKNOWSTATUS._serialized_end=6119
-  _OPTION._serialized_start=6121
-  _OPTION._serialized_end=6163
-  _PURPOSE._serialized_start=6165
-  _PURPOSE._serialized_end=6226
-  _ACQUISITIONSTATE._serialized_start=6228
-  _ACQUISITIONSTATE._serialized_end=6351
-  _ACQUISITIONSTOPREASON._serialized_start=6354
-  _ACQUISITIONSTOPREASON._serialized_end=6660
-  _STARTUPSTATE._serialized_start=6663
-  _STARTUPSTATE._serialized_end=6941
-  _FINISHINGSTATE._serialized_start=6944
-  _FINISHINGSTATE._serialized_end=7083
-  _STARTREQUEST._serialized_start=152
-  _STARTREQUEST._serialized_end=619
-  _STARTRESPONSE._serialized_start=621
-  _STARTRESPONSE._serialized_end=652
-  _STOPREQUEST._serialized_start=655
-  _STOPREQUEST._serialized_end=879
-  _STOPREQUEST_DATAACTION._serialized_start=797
-  _STOPREQUEST_DATAACTION._serialized_end=879
-  _STOPRESPONSE._serialized_start=881
-  _STOPRESPONSE._serialized_end=895
-  _WATCHFORSTATUSCHANGEREQUEST._serialized_start=897
-  _WATCHFORSTATUSCHANGEREQUEST._serialized_end=940
-  _WATCHFORSTATUSCHANGERESPONSE._serialized_start=942
-  _WATCHFORSTATUSCHANGERESPONSE._serialized_end=1028
-  _CURRENTSTATUSREQUEST._serialized_start=1030
-  _CURRENTSTATUSREQUEST._serialized_end=1052
-  _CURRENTSTATUSRESPONSE._serialized_start=1054
-  _CURRENTSTATUSRESPONSE._serialized_end=1133
-  _GETPROGRESSREQUEST._serialized_start=1135
-  _GETPROGRESSREQUEST._serialized_end=1155
-  _GETPROGRESSRESPONSE._serialized_start=1158
-  _GETPROGRESSRESPONSE._serialized_end=1318
-  _GETPROGRESSRESPONSE_RAWPERCHANNEL._serialized_start=1266
-  _GETPROGRESSRESPONSE_RAWPERCHANNEL._serialized_end=1318
-  _GETACQUISITIONRUNINFOREQUEST._serialized_start=1320
-  _GETACQUISITIONRUNINFOREQUEST._serialized_end=1366
-  _ACQUISITIONYIELDSUMMARY._serialized_start=1369
-  _ACQUISITIONYIELDSUMMARY._serialized_end=1903
-  _ACQUISITIONWRITERSUMMARY._serialized_start=1906
-  _ACQUISITIONWRITERSUMMARY._serialized_end=2056
-  _CHANNELSTATEINFO._serialized_start=2059
-  _CHANNELSTATEINFO._serialized_end=2491
-  _CHANNELSTATEINFO_STYLE._serialized_start=2144
-  _CHANNELSTATEINFO_STYLE._serialized_end=2203
-  _CHANNELSTATEINFO_CHANNELSTATE._serialized_start=2205
-  _CHANNELSTATEINFO_CHANNELSTATE._serialized_end=2331
-  _CHANNELSTATEINFO_GROUP._serialized_start=2334
-  _CHANNELSTATEINFO_GROUP._serialized_end=2491
-  _ACQUISITIONCONFIGSUMMARY._serialized_start=2494
-  _ACQUISITIONCONFIGSUMMARY._serialized_end=3165
-  _MUXSCANMETADATA._serialized_start=3168
-  _MUXSCANMETADATA._serialized_end=3638
-  _MUXSCANMETADATA_STYLE._serialized_start=2144
-  _MUXSCANMETADATA_STYLE._serialized_end=2203
-  _MUXSCANMETADATA_CATEGORY._serialized_start=3365
-  _MUXSCANMETADATA_CATEGORY._serialized_end=3474
-  _MUXSCANMETADATA_CATEGORYGROUP._serialized_start=3477
-  _MUXSCANMETADATA_CATEGORYGROUP._serialized_end=3638
-  _MUXSCANRESULT._serialized_start=3641
-  _MUXSCANRESULT._serialized_end=3799
-  _MUXSCANRESULT_COUNTSENTRY._serialized_start=3754
-  _MUXSCANRESULT_COUNTSENTRY._serialized_end=3799
-  _BREAMINFO._serialized_start=3802
-  _BREAMINFO._serialized_end=4205
-  _BREAMINFO_RANGE._serialized_start=4164
-  _BREAMINFO_RANGE._serialized_end=4205
-  _TARGETRUNUNTILCRITERIA._serialized_start=4208
-  _TARGETRUNUNTILCRITERIA._serialized_end=4357
-  _ACQUISITIONRUNINFO._serialized_start=4360
-  _ACQUISITIONRUNINFO._serialized_end=5337
-  _LISTACQUISITIONRUNSREQUEST._serialized_start=5339
-  _LISTACQUISITIONRUNSREQUEST._serialized_end=5367
-  _LISTACQUISITIONRUNSRESPONSE._serialized_start=5369
-  _LISTACQUISITIONRUNSRESPONSE._serialized_end=5415
-  _GETCURRENTACQUISITIONRUNREQUEST._serialized_start=5417
-  _GETCURRENTACQUISITIONRUNREQUEST._serialized_end=5450
-  _WATCHCURRENTACQUISITIONRUNREQUEST._serialized_start=5452
-  _WATCHCURRENTACQUISITIONRUNREQUEST._serialized_end=5487
-  _SETSIGNALREADERREQUEST._serialized_start=5490
-  _SETSIGNALREADERREQUEST._serialized_end=5841
-  _SETSIGNALREADERREQUEST_SIGNALREADERTYPE._serialized_start=5740
-  _SETSIGNALREADERREQUEST_SIGNALREADERTYPE._serialized_end=5780
-  _SETSIGNALREADERREQUEST_SOURCEFILEMODE._serialized_start=5782
-  _SETSIGNALREADERREQUEST_SOURCEFILEMODE._serialized_end=5841
-  _SETSIGNALREADERRESPONSE._serialized_start=5843
-  _SETSIGNALREADERRESPONSE._serialized_end=5868
-  _SETBREAMINFOREQUEST._serialized_start=5870
-  _SETBREAMINFOREQUEST._serialized_end=5973
-  _SETBREAMINFORESPONSE._serialized_start=5975
-  _SETBREAMINFORESPONSE._serialized_end=5997
-  _APPENDMUXSCANRESULTRESPONSE._serialized_start=5999
-  _APPENDMUXSCANRESULTRESPONSE._serialized_end=6028
-  _ACQUISITIONSERVICE._serialized_start=7086
-  _ACQUISITIONSERVICE._serialized_end=8578
+  _GETBARCODEKITINFORESPONSE_BARCODEKITINFOENTRY._options = None
+  _GETBARCODEKITINFORESPONSE_BARCODEKITINFOENTRY._serialized_options = b'8\001'
+  _ADDSIMULATEDDEVICEREQUEST.fields_by_name['name']._options = None
+  _ADDSIMULATEDDEVICEREQUEST.fields_by_name['name']._serialized_options = b'\210\265\030\001'
+  _ADDSIMULATEDDEVICEREQUEST.fields_by_name['type']._options = None
+  _ADDSIMULATEDDEVICEREQUEST.fields_by_name['type']._serialized_options = b'\210\265\030\001'
+  _REMOVESIMULATEDDEVICEREQUEST.fields_by_name['name']._options = None
+  _REMOVESIMULATEDDEVICEREQUEST.fields_by_name['name']._serialized_options = b'\210\265\030\001'
+  _LISTSETTINGSFORPROTOCOLREQUEST.fields_by_name['flow_cell_connector']._options = None
+  _LISTSETTINGSFORPROTOCOLREQUEST.fields_by_name['flow_cell_connector']._serialized_options = b'\210\265\030\001'
+  _MANAGERSERVICE.methods_by_name['describe_host']._options = None
+  _MANAGERSERVICE.methods_by_name['describe_host']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['flow_cell_positions']._options = None
+  _MANAGERSERVICE.methods_by_name['flow_cell_positions']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['watch_flow_cell_positions']._options = None
+  _MANAGERSERVICE.methods_by_name['watch_flow_cell_positions']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['basecaller_api']._options = None
+  _MANAGERSERVICE.methods_by_name['basecaller_api']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_guppy_info']._options = None
+  _MANAGERSERVICE.methods_by_name['get_guppy_info']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_version_info']._options = None
+  _MANAGERSERVICE.methods_by_name['get_version_info']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['list_protocol_output_dir_files']._options = None
+  _MANAGERSERVICE.methods_by_name['list_protocol_output_dir_files']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['create_directory']._options = None
+  _MANAGERSERVICE.methods_by_name['create_directory']._serialized_options = b'\220\002\002'
+  _MANAGERSERVICE.methods_by_name['get_disk_space_info']._options = None
+  _MANAGERSERVICE.methods_by_name['get_disk_space_info']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_default_output_directories']._options = None
+  _MANAGERSERVICE.methods_by_name['get_default_output_directories']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['stream_disk_space_info']._options = None
+  _MANAGERSERVICE.methods_by_name['stream_disk_space_info']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_barcode_kit_info']._options = None
+  _MANAGERSERVICE.methods_by_name['get_barcode_kit_info']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_lamp_kit_info']._options = None
+  _MANAGERSERVICE.methods_by_name['get_lamp_kit_info']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_barcode_keys']._options = None
+  _MANAGERSERVICE.methods_by_name['get_barcode_keys']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_flow_cell_types']._options = None
+  _MANAGERSERVICE.methods_by_name['get_flow_cell_types']._serialized_options = b'\220\002\001\230\265\030\001'
+  _MANAGERSERVICE.methods_by_name['get_sequencing_kits']._options = None
+  _MANAGERSERVICE.methods_by_name['get_sequencing_kits']._serialized_options = b'\220\002\001\230\265\030\001'
+  _MANAGERSERVICE.methods_by_name['remove_simulated_device']._options = None
+  _MANAGERSERVICE.methods_by_name['remove_simulated_device']._serialized_options = b'\220\002\002'
+  _MANAGERSERVICE.methods_by_name['local_authentication_token_path']._options = None
+  _MANAGERSERVICE.methods_by_name['local_authentication_token_path']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['get_alignment_reference_information']._options = None
+  _MANAGERSERVICE.methods_by_name['get_alignment_reference_information']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['association_device_code']._options = None
+  _MANAGERSERVICE.methods_by_name['association_device_code']._serialized_options = b'\220\002\001'
+  _MANAGERSERVICE.methods_by_name['apply_offline_association_unlock_code']._options = None
+  _MANAGERSERVICE.methods_by_name['apply_offline_association_unlock_code']._serialized_options = b'\220\002\002'
+  _MANAGERSERVICE.methods_by_name['list_developer_api_tokens']._options = None
+  _MANAGERSERVICE.methods_by_name['list_developer_api_tokens']._serialized_options = b'\220\002\002'
+  _MANAGERSERVICE.methods_by_name['find_protocols']._options = None
+  _MANAGERSERVICE.methods_by_name['find_protocols']._serialized_options = b'\230\265\030\001'
+  _MANAGERSERVICE.methods_by_name['list_settings_for_protocol']._options = None
+  _MANAGERSERVICE.methods_by_name['list_settings_for_protocol']._serialized_options = b'\220\002\001\230\265\030\001'
+  _MANAGERSERVICE.methods_by_name['get_features']._options = None
+  _MANAGERSERVICE.methods_by_name['get_features']._serialized_options = b'\220\002\001\230\265\030\001'
+  _MANAGERSERVICE.methods_by_name['set_features']._options = None
+  _MANAGERSERVICE.methods_by_name['set_features']._serialized_options = b'\230\265\030\001'
+  _SIMPLEPROTOCOLSTATE._serialized_start=11290
+  _SIMPLEPROTOCOLSTATE._serialized_end=11426
+  _SIMULATEDDEVICETYPE._serialized_start=11429
+  _SIMULATEDDEVICETYPE._serialized_end=11559
+  _EXPERIMENTTYPE._serialized_start=11561
+  _EXPERIMENTTYPE._serialized_end=11667
+  _DESCRIBEHOSTREQUEST._serialized_start=205
+  _DESCRIBEHOSTREQUEST._serialized_end=226
+  _DESCRIBEHOSTRESPONSE._serialized_start=229
+  _DESCRIBEHOSTRESPONSE._serialized_end=658
+  _DESCRIBEHOSTRESPONSE_BASECALLINGAVAILABILITY._serialized_start=481
+  _DESCRIBEHOSTRESPONSE_BASECALLINGAVAILABILITY._serialized_end=658
+  _FLOWCELLPOSITION._serialized_start=661
+  _FLOWCELLPOSITION._serialized_end=1544
+  _FLOWCELLPOSITION_LOCATION._serialized_start=1235
+  _FLOWCELLPOSITION_LOCATION._serialized_end=1267
+  _FLOWCELLPOSITION_RPCPORTS._serialized_start=1269
+  _FLOWCELLPOSITION_RPCPORTS._serialized_end=1320
+  _FLOWCELLPOSITION_SHAREDHARDWAREGROUP._serialized_start=1322
+  _FLOWCELLPOSITION_SHAREDHARDWAREGROUP._serialized_end=1361
+  _FLOWCELLPOSITION_STATE._serialized_start=1364
+  _FLOWCELLPOSITION_STATE._serialized_end=1544
+  _FLOWCELLPOSITIONSREQUEST._serialized_start=1546
+  _FLOWCELLPOSITIONSREQUEST._serialized_end=1572
+  _FLOWCELLPOSITIONSRESPONSE._serialized_start=1574
+  _FLOWCELLPOSITIONSRESPONSE._serialized_end=1680
+  _WATCHFLOWCELLPOSITIONSREQUEST._serialized_start=1682
+  _WATCHFLOWCELLPOSITIONSREQUEST._serialized_end=1713
+  _WATCHFLOWCELLPOSITIONSRESPONSE._serialized_start=1716
+  _WATCHFLOWCELLPOSITIONSRESPONSE._serialized_end=1880
+  _RESETPOSITIONREQUEST._serialized_start=1882
+  _RESETPOSITIONREQUEST._serialized_end=1938
+  _RESETPOSITIONRESPONSE._serialized_start=1940
+  _RESETPOSITIONRESPONSE._serialized_end=1963
+  _BASECALLERAPIREQUEST._serialized_start=1965
+  _BASECALLERAPIREQUEST._serialized_end=1987
+  _BASECALLERAPIRESPONSE._serialized_start=1989
+  _BASECALLERAPIRESPONSE._serialized_end=2053
+  _GETGUPPYINFOREQUEST._serialized_start=2055
+  _GETGUPPYINFOREQUEST._serialized_end=2076
+  _GETGUPPYINFORESPONSE._serialized_start=2078
+  _GETGUPPYINFORESPONSE._serialized_end=2172
+  _GETVERSIONINFOREQUEST._serialized_start=2174
+  _GETVERSIONINFOREQUEST._serialized_end=2197
+  _LISTPROTOCOLOUTPUTDIRFILESREQUEST._serialized_start=2199
+  _LISTPROTOCOLOUTPUTDIRFILESREQUEST._serialized_end=2248
+  _LISTPROTOCOLOUTPUTDIRFILESRESPONSE._serialized_start=2251
+  _LISTPROTOCOLOUTPUTDIRFILESRESPONSE._serialized_end=2499
+  _LISTPROTOCOLOUTPUTDIRFILESRESPONSE_DIRECTORYINFO._serialized_start=2425
+  _LISTPROTOCOLOUTPUTDIRFILESRESPONSE_DIRECTORYINFO._serialized_end=2499
+  _CREATEDIRECTORYREQUEST._serialized_start=2501
+  _CREATEDIRECTORYREQUEST._serialized_end=2560
+  _CREATEDIRECTORYRESPONSE._serialized_start=2562
+  _CREATEDIRECTORYRESPONSE._serialized_end=2601
+  _FILESYSTEMDISKSPACEINFO._serialized_start=2604
+  _FILESYSTEMDISKSPACEINFO._serialized_end=2867
+  _GETDISKSPACEINFOREQUEST._serialized_start=2869
+  _GETDISKSPACEINFOREQUEST._serialized_end=2894
+  _STREAMDISKSPACEINFOREQUEST._serialized_start=2896
+  _STREAMDISKSPACEINFOREQUEST._serialized_end=2940
+  _GETDISKSPACEINFORESPONSE._serialized_start=2942
+  _GETDISKSPACEINFORESPONSE._serialized_end=3050
+  _GETBARCODEKITINFOREQUEST._serialized_start=3052
+  _GETBARCODEKITINFOREQUEST._serialized_end=3078
+  _GETBARCODEKITINFORESPONSE._serialized_start=3081
+  _GETBARCODEKITINFORESPONSE._serialized_end=3377
+  _GETBARCODEKITINFORESPONSE_BARCODEKITINFO._serialized_start=3204
+  _GETBARCODEKITINFORESPONSE_BARCODEKITINFO._serialized_end=3259
+  _GETBARCODEKITINFORESPONSE_BARCODEKITINFOENTRY._serialized_start=3261
+  _GETBARCODEKITINFORESPONSE_BARCODEKITINFOENTRY._serialized_end=3377
+  _GETLAMPKITINFOREQUEST._serialized_start=3379
+  _GETLAMPKITINFOREQUEST._serialized_end=3402
+  _GETLAMPKITINFORESPONSE._serialized_start=3404
+  _GETLAMPKITINFORESPONSE._serialized_end=3447
+  _GETBARCODEKEYSREQUEST._serialized_start=3449
+  _GETBARCODEKEYSREQUEST._serialized_end=3522
+  _GETBARCODEKEYSRESPONSE._serialized_start=3524
+  _GETBARCODEKEYSRESPONSE._serialized_end=3612
+  _GETFLOWCELLTYPESREQUEST._serialized_start=3614
+  _GETFLOWCELLTYPESREQUEST._serialized_end=3639
+  _GETFLOWCELLTYPESRESPONSE._serialized_start=3642
+  _GETFLOWCELLTYPESRESPONSE._serialized_end=3862
+  _GETFLOWCELLTYPESRESPONSE_INFO._serialized_start=3737
+  _GETFLOWCELLTYPESRESPONSE_INFO._serialized_end=3862
+  _GETSEQUENCINGKITSREQUEST._serialized_start=3864
+  _GETSEQUENCINGKITSREQUEST._serialized_end=3922
+  _GETSEQUENCINGKITSRESPONSE._serialized_start=3925
+  _GETSEQUENCINGKITSRESPONSE._serialized_end=4423
+  _GETSEQUENCINGKITSRESPONSE_KIT._serialized_start=4125
+  _GETSEQUENCINGKITSRESPONSE_KIT._serialized_end=4376
+  _GETSEQUENCINGKITSRESPONSE_BARCODINGEXPANSIONKIT._serialized_start=4378
+  _GETSEQUENCINGKITSRESPONSE_BARCODINGEXPANSIONKIT._serialized_end=4423
+  _ADDSIMULATEDDEVICEREQUEST._serialized_start=4425
+  _ADDSIMULATEDDEVICEREQUEST._serialized_end=4534
+  _ADDSIMULATEDDEVICERESPONSE._serialized_start=4536
+  _ADDSIMULATEDDEVICERESPONSE._serialized_end=4564
+  _REMOVESIMULATEDDEVICEREQUEST._serialized_start=4566
+  _REMOVESIMULATEDDEVICEREQUEST._serialized_end=4616
+  _REMOVESIMULATEDDEVICERESPONSE._serialized_start=4618
+  _REMOVESIMULATEDDEVICERESPONSE._serialized_end=4649
+  _LOCALAUTHENTICATIONTOKENPATHREQUEST._serialized_start=4651
+  _LOCALAUTHENTICATIONTOKENPATHREQUEST._serialized_end=4688
+  _LOCALAUTHENTICATIONTOKENPATHRESPONSE._serialized_start=4690
+  _LOCALAUTHENTICATIONTOKENPATHRESPONSE._serialized_end=4742
+  _GETALIGNMENTREFERENCEINFORMATIONREQUEST._serialized_start=4744
+  _GETALIGNMENTREFERENCEINFORMATIONREQUEST._serialized_end=4799
+  _GETALIGNMENTREFERENCEINFORMATIONRESPONSE._serialized_start=4802
+  _GETALIGNMENTREFERENCEINFORMATIONRESPONSE._serialized_end=4953
+  _ASSOCIATIONDEVICECODEREQUEST._serialized_start=4955
+  _ASSOCIATIONDEVICECODEREQUEST._serialized_end=5023
+  _ASSOCIATIONDEVICECODERESPONSE._serialized_start=5025
+  _ASSOCIATIONDEVICECODERESPONSE._serialized_end=5070
+  _APPLYOFFLINEASSOCIATIONUNLOCKCODEREQUEST._serialized_start=5072
+  _APPLYOFFLINEASSOCIATIONUNLOCKCODEREQUEST._serialized_end=5158
+  _APPLYOFFLINEASSOCIATIONUNLOCKCODERESPONSE._serialized_start=5160
+  _APPLYOFFLINEASSOCIATIONUNLOCKCODERESPONSE._serialized_end=5223
+  _LISTDEVELOPERAPITOKENSREQUEST._serialized_start=5225
+  _LISTDEVELOPERAPITOKENSREQUEST._serialized_end=5256
+  _LISTDEVELOPERAPITOKENSRESPONSE._serialized_start=5259
+  _LISTDEVELOPERAPITOKENSRESPONSE._serialized_end=5469
+  _LISTDEVELOPERAPITOKENSRESPONSE_DEVELOPERAPITOKEN._serialized_start=5380
+  _LISTDEVELOPERAPITOKENSRESPONSE_DEVELOPERAPITOKEN._serialized_end=5469
+  _CREATEDEVELOPERAPITOKENREQUEST._serialized_start=5471
+  _CREATEDEVELOPERAPITOKENREQUEST._serialized_end=5561
+  _CREATEDEVELOPERAPITOKENRESPONSE._serialized_start=5563
+  _CREATEDEVELOPERAPITOKENRESPONSE._serialized_end=5623
+  _REVOKEDEVELOPERAPITOKENREQUEST._serialized_start=5625
+  _REVOKEDEVELOPERAPITOKENREQUEST._serialized_end=5669
+  _REVOKEDEVELOPERAPITOKENSRESPONSE._serialized_start=5671
+  _REVOKEDEVELOPERAPITOKENSRESPONSE._serialized_end=5705
+  _FINDPROTOCOLSREQUEST._serialized_start=5708
+  _FINDPROTOCOLSREQUEST._serialized_end=5848
+  _FINDPROTOCOLSRESPONSE._serialized_start=5851
+  _FINDPROTOCOLSRESPONSE._serialized_end=6052
+  _FINDPROTOCOLSRESPONSE_PROTOCOL._serialized_start=5948
+  _FINDPROTOCOLSRESPONSE_PROTOCOL._serialized_end=6052
+  _LISTSETTINGSFORPROTOCOLREQUEST._serialized_start=6055
+  _LISTSETTINGSFORPROTOCOLREQUEST._serialized_end=6293
+  _LISTSETTINGSFORPROTOCOLRESPONSE._serialized_start=6296
+  _LISTSETTINGSFORPROTOCOLRESPONSE._serialized_end=10683
+  _LISTSETTINGSFORPROTOCOLRESPONSE_RUNOPTIONS._serialized_start=6736
+  _LISTSETTINGSFORPROTOCOLRESPONSE_RUNOPTIONS._serialized_end=7589
+  _LISTSETTINGSFORPROTOCOLRESPONSE_BASECALLING._serialized_start=7592
+  _LISTSETTINGSFORPROTOCOLRESPONSE_BASECALLING._serialized_end=8872
+  _LISTSETTINGSFORPROTOCOLRESPONSE_OUTPUT._serialized_start=8875
+  _LISTSETTINGSFORPROTOCOLRESPONSE_OUTPUT._serialized_end=10683
+  _FEATURE._serialized_start=10685
+  _FEATURE._serialized_end=10711
+  _FEATURELIST._serialized_start=10714
+  _FEATURELIST._serialized_end=10943
+  _GETFEATURESREQUEST._serialized_start=10945
+  _GETFEATURESREQUEST._serialized_end=10965
+  _GETFEATURESRESPONSE._serialized_start=10968
+  _GETFEATURESRESPONSE._serialized_end=11190
+  _GETFEATURESRESPONSE_STATE._serialized_start=11106
+  _GETFEATURESRESPONSE_STATE._serialized_end=11190
+  _SETFEATURESREQUEST._serialized_start=11192
+  _SETFEATURESREQUEST._serialized_end=11264
+  _SETFEATURESRESPONSE._serialized_start=11266
+  _SETFEATURESRESPONSE._serialized_end=11287
+  _MANAGERSERVICE._serialized_start=11670
+  _MANAGERSERVICE._serialized_end=15554
+DescribeHostResponse.__doc__ = """Attributes:
+    product_code:
+        The product code for the host, if applicable.  If this is an
+        integrated Oxford Nanopore device, this will be the product
+        code of the device, or the part of the device that runs
+        MinKNOW (eg: several PromethION models have separate product
+        codes for the sequencing unit where the flow cells are
+        inserted and the compute unit - this would be the product code
+        for the compute unit).  Some example product codes:
+        ============  ================= Product Code  Name
+        ============  ================= GRD-X5B001    GridION X5
+        GRD-X5B002    GridION X5 GRD-X5B003    GridION X5 Mk1 MIN-101C
+        MinION Mk1C PRO-PRMC01    PromethION Beta PRO-PRC024
+        PromethION 24 PRO-PRC048    PromethION 48 ONT-314
+        PromethION (Production)  If MinKNOW is running on a machine
+        that is not provided by Oxford Nanopore (ie: their own laptop
+        or desktop machine with a MinION plugged in), this field will
+        be empty.
+    description:
+        A human-readable name for the type of host.  If `product_code`
+        is set, it will be the name of the model of instrument (see
+        the table in the `product_code` field). Otherwise it will be
+        empty.
+    serial:
+        The serial of Nanopore device.  If `product_code` is empty,
+        this will also be empty.  This uniquely identifies the device.
+        See also `network_name`.
+    network_name:
+        The network name of the host.  This is the name the host
+        system believes it has on the network. This can be useful if
+        an IP address was used to connect to the RPC system.  For
+        customer computers, this is the only available identfying
+        information for the system.
+    needs_association:
+        This device has not been associated with an account.
+        Association must be completed before using the device.  Note
+        that this will only ever be set for hosts that also have a
+        `product_code` and `serial`.  If this is true, all positions
+        will report as ``STATE_NEEDS_ASSOCIATION`` until the device is
+        associated. Even if this is false, however, removable
+        sequencing units (eg: the MinION Mk1B) may require their own
+        association (in which case they will individually report as
+        ``STATE_NEEDS_ASSOCIATION`` - see the `flow_cell_positions`
+        RPC).  Since 4.4
+    can_sequence_offline:
+        Whether the device can sequence while offline.  Not all
+        sequencing devices can sequence without an internet
+        connection. This indicates whether it is possible for the
+        integrated sequencing positions. Note that this will only be
+        set if `needs_association` is true.  Since 4.4
+    can_basecall:
+        Whether the device can currently provide basecalling
+"""
+FilesystemDiskSpaceInfo.__doc__ = """disk-usage information for one file-system
+
+Attributes:
+    filesystem_id:
+        The name of the file-system
+    bytes_available:
+        How much space is left on the file-system
+    bytes_capacity:
+        The total capacity of the file-system when empty.
+    what:
+        A list of what MinKNOW stores on this file-system, eg: reads,
+        logs, intermediate-files
+    bytes_to_stop_cleanly:
+        MinKNOW needs this much space to stop experiments. If
+        bytes_available goes below this number, data could be lost!
+    bytes_when_alert_issued:
+        The amount of space left on the file-system when
+        recommend_alert was set true.
+    recommend_alert:
+        MinKNOW recommends that you alert someone about the disk-usage
+    recommend_stop:
+        MinKNOW recommends that you stop experiments due to disk-usage
+        concerns
+    bytes_per_second:
+        Rate of change in bytes_available (per second) +'ve numbers
+        indicate that bytes_available is decreasing and space is being
+        used A value of 0 can indicate that this has not applicable or
+        not available.
+    file_types_stored:
+        A list of what types of file MinKNOW stores on this file-
+        system, eg: reads, logs, intermediate-files, etc.
+"""
+ListSettingsForProtocolResponse.RunOptions.__doc__ = """Run options
+
+Attributes:
+    active_channel_selection:
+         bool
+    mux_scan_period:
+         in hours
+"""
+FindProtocolsRequest.__doc__ = """Attributes:
+    flow_cell_product_code:
+        Find protocols that are compatible with this flow cell product
+        code.  Set to empty string to find protocols matching all flow
+        cell product codes.
+    sequencing_kit:
+        Limit to protocols that are compatible with this sequencing
+        kit.  Set to empty string to find protocols matching all kits.
+    experiment_type:
+        Limit response to certain protocol types.
+"""
+GetSequencingKitsResponse.BarcodingExpansionKit.__doc__ = """Information about a barcoding expansion kit.  In the future, this may
+include compatibility information for dual barcoding, for example.
+
+Attributes:
+    product_code:
+        The product code for the barcoding expansion kit.  This is the
+        user-visible name for the kit. It is the name used to order
+        kits, and is also displayed on the packaging.  While most
+        product codes are 10 characters, be aware that longer product
+        codes can exist.  Example: "EXP-NBD104".
+"""
+ApplyOfflineAssociationUnlockCodeResponse.__doc__ = """Attributes:
+    associated:
+        True if the association was successful (the unlock_code was
+        accepted), false otherwise.
+"""
+ResetPositionRequest.__doc__ = """Attributes:
+    positions:
+        The names of positions to restart.
+    force:
+        Force the software to be restarted even when it appears to be
+        in a healthy state (ie: STATE_RUNNING).
+"""
+Feature.__doc__ = """Attributes:
+    enabled:
+        Enable or disable the feature
+"""
+ApplyOfflineAssociationUnlockCodeRequest.__doc__ = """Attributes:
+    position_name:
+        The flow cell position to unlock.  This should be set (or not
+        set) to match the corresponding call to
+        `offline_association_device_code`.
+    unlock_code:
+        The unlock code provided by the user.  This the code given by
+        the customer support portal when the corresponding device code
+        is entered into the device association page.
+"""
+AssociationDeviceCodeRequest.__doc__ = """Offline association is now the default workflow  The following are
+therefore reserved/deprecated
+
+Attributes:
+    position_name:
+        The flow cell position to get the association code/key for.
+        If this is omitted, the code/key for the sequencing device as
+        a whole is returned.  Note that this cannot be omitted if
+        MinKNOW is installed on a PC (as opposed to a sequencing
+        device). It should be omitted if (and only if) the data
+        returned from `describe_host` has its ``needs_association``
+        field set to true.  Passing a integrated flow cell position
+        will return the code/key for the whole sequencing device.
+"""
+CreateDeveloperApiTokenResponse.__doc__ = """Attributes:
+    id:
+        Unique ID assigned to the token for identification purposes.
+        Not valid as an authentication token.
+    token:
+        Created token, available to be used with minknow API's
+        immediately.
+"""
+BasecallerApiResponse.__doc__ = """Attributes:
+    secure:
+        The port to use to access the minknow_api.basecaller API using
+        the standard gRPC protocol over TLS
+    secure_grpc_web:
+        The port to use to access the minknow_api.basecaller API using
+        the gRPC-Web protocol over TLS
+"""
+GetFlowCellTypesRequest.__doc__ = """Request message for `ManagerService.get_flow_cell_types`."""
+GetBarcodeKeysRequest.__doc__ = """Attributes:
+    barcode_kit_names:
+        Names of barcode kits to obtain barcode names for  Fails with
+        INVALID_ARGUMENT if any of the requested `barcode_kit_names`
+        are unavailable
+    lamp_kit_name:
+        Name of lamp kit to obtain barcode names for.  Fails with
+        INVALID_ARGUMENT if the requested `lamp_kit_name` is
+        unavailable.
+"""
+ListDeveloperApiTokensResponse.DeveloperApiToken.__doc__ = """Attributes:
+    id:
+        Unique ID assigned to the token.
+    name:
+        User facing name describing the token (guaranteed unique
+        across tokens).
+    expiry:
+        Optional expiry of the token.
+"""
+FindProtocolsResponse.__doc__ = """Attributes:
+    protocols:
+        Protocols available for starting.
+"""
+GetBarcodeKeysResponse.__doc__ = """Attributes:
+    barcode_keys:
+        Returned barcode keys.
+    lamp_keys:
+        Returned lamp barcode ids.
+    combined_keys:
+        Combined barcode and lamp keys.  Returned keys are joined
+        strings of all requested barcode kits, giving the caller a
+        unique string to identify each barcode pair.  eg. if both a
+        lamp kit + barcode kit are specified, NxM barcode keys are
+        returned:  - barcode01_lamp01  - barcode01_lamp02  -
+        barcode01_lamp03  - barcode02_lamp01  - barcode02_lamp02  -
+        barcode02_lamp03
+"""
+FlowCellPositionsResponse.__doc__ = """Attributes:
+    total_count:
+        How many positions are available in total.  This is the same
+        in every message returned from a single call, and allows the
+        caller to easily see how many further positions might be in
+        subsequent messages.
+    positions:
+        Known flow cell positions.  Note that not all positions listed
+        here are necessarily available. In particular, integrated flow
+        cell positions (eg: on GridIONs or PromethIONs) will always be
+        listed.
+"""
+FindProtocolsResponse.Protocol.__doc__ = """Attributes:
+    identifier:
+        An identifying string for protocol, of the form:
+        LOCATION:relative/path/to/protocol  The identifier uniquely
+        identifies the protocol.
+    requires_flow_cell_product_code:
+        Whether the protocol requires a flow cell product code in
+        order to start.
+    requires_sequencing_kit:
+        Whether the protocol requires a sequencing kit in order to
+        start.
+"""
+StreamDiskSpaceInfoRequest.__doc__ = """Attributes:
+    period:
+        Disk space information will be streamed with this value
+        determining the period in seconds between updates. A period of
+        0 is invalid
+"""
+GetAlignmentReferenceInformationResponse.__doc__ = """Attributes:
+    estimated_load_time_seconds:
+        Estimated load time of the reference in seconds.
+    estimated_reference_size_bases:
+        Estimated size of the reference file in bases.
+    recommended_live_usage:
+        Does the reference file fit within the recommended live usage
+        memory size?  This uses an estimate of how much memory a
+        reference may use when running in guppy and compares to the
+        amount of memory in the sequencer. It does not account for
+        whether the reference will run in real time.
+"""
+ListSettingsForProtocolRequest.__doc__ = """Attributes:
+    identifier:
+        specify the protocol with a string containing all the
+        protocol's identifying components, eg:
+        "sequencing/sequencing_MIN106_DNA:FLO-MIN106:SQK-RPB004"
+    components:
+        specify the protocol providing the identifying components
+        individually. All components are optional, if more than one
+        protocol matches given strings, information about the first
+        will be returned.
+    flow_cell_connector:
+        The flow-cell connector type identifies the type of hardware
+        and is used to identify the correct protocol. The flow-cell
+        connector types applicable to the device are listed by the
+        get_flow_cell_types rpc in this service and the
+        get_device_state rpc in the device service.
+"""
+WatchFlowCellPositionsResponse.__doc__ = """Each flow cell position will first be listed in `additions`. After
+that, it may appear in `changes` in zero or more messages. Then, it
+may appear in `removals` once, after which it will either never appear
+again, or appear in `additions` again (restarting the cycle).  No
+position will ever appear in more than one field in the same response
+message.
+
+Attributes:
+    additions:
+        Flow cell positions that are new (to this call).  Contains
+        flow cell positions that have not been seen before on this
+        call (or have re-appeared after being removed).  Note that a
+        flow cell position being listed here does not mean it is
+        available. In particular, integrated flow cell positions (eg:
+        on GridIONs or PromethIONs) will always be provided, so that
+        they can be positioned appropriately.
+    changes:
+        Flow cell positions that have changed state.  Every flow cell
+        position provided in this list will have previously been
+        provided in `additions`.
+    removals:
+        A flow cell position has been removed.  Note that this can
+        only happen with MinIONs - integrated flow cell positions are
+        never removed (if they become unavailable, this will be noted
+        in the `changes` field).
+"""
+AddSimulatedDeviceRequest.__doc__ = """Attributes:
+    name:
+        The name of the position, this must be unique and the correct
+        format:  For MinION Mk1B and Mk1C: "MS" followed by five
+        digits, eg: "MS12345". For GridION: "GS" followed by five
+        digits, eg: "GS12345". For P2 Solo: "P2S_" followed by five
+        digits, and then "-A" or "-B" eg: "P2S_12345-A".  PromethION
+        and P2 Solo position-names have no format restriction, but
+        must be unique. It is strongly recommended to follow standard
+        naming conventions:  For PromethION: start with "1A" and then
+        increase the number and/or the letter as you add more
+        positions. For P2 Solo: use "P2S_00000-A" and "P2S_00000-B"
+        (these fit the format of real P2 Solo devices, but do not
+        correspond to any real device).  Future versions might
+        constrain PromethION and P2 Solo device names. Using the above
+        suggestions should ensure that your code will continue to
+        work.  Note that MinKNOW Core 5.5 and earlier required the P2
+        Solo device name to be "P2S" followed by four digits. This is
+        no longer recommended.
+    type:
+        The type of the simulated device to create.  If left at
+        default (AUTO), then a sensible default device type is
+        selected.
+"""
+LocalAuthenticationTokenPathResponse.__doc__ = """Attributes:
+    path:
+        The full path of the local authentication token
+"""
+GetAlignmentReferenceInformationRequest.__doc__ = """Attributes:
+    path:
+        The full path of the alignment reference.  Should be a .fasta,
+        or .mmi file.
+"""
+GetLampKitInfoResponse.__doc__ = """Attributes:
+    lamp_kits:
+        Lamp kit names
+"""
+GetSequencingKitsResponse.Kit.__doc__ = """Information about a sequencing kit.
+
+Attributes:
+    product_code:
+        The product code for the sequencing kit.  This is the user-
+        visible name for the kit. It is the name used to order kits,
+        and is also displayed on the packaging.  While most product
+        codes are 10-15 characters, be aware that longer (or shorter)
+        product codes can exist.  Examples: "SQK-LSK109", "OND-SQK-
+        LP0096S".
+    barcoding_expansion_kits:
+        Compatible barcoding expansion kits.  These are indexes into
+        the GetSequencingKitsResponse.barcoding_expansion_kits list.
+        For example, 0 would indicate the first kit in that list. The
+        values are guaranteed to be unique and valid indexes for that
+        list.
+    includes_barcoding:
+        Whether barcoding support is part of the sequencing kit.  If
+        this is set, barcoding can be done without any expansion kits
+        (and, in fact, barcoding is an integral part of the kit).
+    lamp_kit:
+        Whether the kit can be used for LamPORE diagnostics.
+    has_control_protocol:
+        Whether there is a "control" protocol available for this kit.
+    no_sequencing_protocol:
+        Indicates there is no sequencing protocol available for this
+        kit.  This is an unusual situation. If a kit is known about,
+        it should generally have a sequencing protocol associated with
+        it, and it would be strange to have a control protocol
+        available but no sequencing protocol.
+    frequently_used:
+        Indicates that the sequencing kit is one of the most commonly
+        used ones.  This can be used to display such kits first, or
+        otherwise highlight them in some way.
+    dna:
+        The kit can be used with DNA samples.
+    rna:
+        The kit can be used with RNA samples.
+    pcr:
+        The kit can be used with samples that have had PCR applied to
+        them.
+    pcr_free:
+        The kit can be used without a PCR step.
+"""
+CreateDeveloperApiTokenRequest.__doc__ = """Attributes:
+    name:
+        User facing name describing the token.
+    expiry:
+        Optional expiry time for the token.
+"""
+GetGuppyInfoResponse.__doc__ = """Attributes:
+    port:
+        The port Guppy is listening on.
+    ipc_path:
+        The path to an ipc file Guppy is using. Use "ipc://<ipc_path>"
+        for a guppy connection string.
+    version:
+        The Guppy server version.
+"""
+FlowCellPosition.RpcPorts.__doc__ = """Attributes:
+    secure:
+        A port providing the standard gRPC protocol over TLS
+    secure_grpc_web:
+        A port providing the gRPC-Web protocol over TLS
+"""
+RevokeDeveloperApiTokenRequest.__doc__ = """Attributes:
+    id:
+        The id passed back from [CreateDeveloperApiTokenRequest] or
+        [DeveloperApiToken].
+"""
+GetSequencingKitsResponse.__doc__ = """Response message for `ManagerService.get_sequencing_kits`.
+
+Attributes:
+    kits:
+        The known sequencing kits.
+    barcoding_expansion_kits:
+        The possible barcoding expansion kits.  These are kits that
+        can be used in combination with certain sequencing kits to add
+        (or extend) barcoding functionality.
+"""
+CreateDirectoryResponse.__doc__ = """Attributes:
+    path:
+        The path to the created directory.
+"""
+CreateDirectoryRequest.__doc__ = """Attributes:
+    parent_path:
+        The path at which to create the directory.  This must exist,
+        be a directory, and be within the protocol output directory.
+        This can be determined via calls to
+        list_protocol_output_dir_files().
+    name:
+        The name of the directory to create.  This must be a single
+        path component (ie: it cannot contain '/' or '\'). There may
+        be other restrictions on valid characters, depending on the
+        operating system.
+"""
+ListProtocolOutputDirFilesRequest.__doc__ = """Attributes:
+    path:
+        Specify the root path to list files from. If the path is left
+        empty, then the base protocol output directory will be used.
+        Note that the path specified HAS to be a descendant of the
+        protocol output directory, otherwise a INVALID_ARGUMENT error
+        will be returned  If the path is left empty, and the path
+        specified in the user config doesn't exist, then the NOT_FOUND
+        error code will be returned
+"""
+GetFlowCellTypesResponse.Info.__doc__ = """Information about a flow cell type.
+
+Attributes:
+    product_code:
+        The product code for the flow cell type.  This is the user-
+        visible name for the flow cell type. It is the name used to
+        order flow cells, and is also displayed on the packaging.
+        While most product codes are 10 characters, be aware that
+        longer product codes can exist and have been used in the past.
+        Example: "FLO-MIN106".
+    connector_type:
+        The connector type of this flow cell type.  This determines
+        which flow cell positions it is possible to insert this flow
+        cell into. The connector type for a given flow cell position
+        can be determined using
+        `minknow_api.device.DeviceService.get_device_state`.  This
+        will never be ``FCCON_NOT_SET``.
+    cannot_live_basecall:
+        Indicates that live basecalling is not possible on the flow
+        cell.  Note that almost all flow cell types can be basecalled
+        on: that is why this indicates a negative (saving some bytes
+        on the wire by allowing the common case of basecalling being
+        possible to be omitted entirely).
+"""
+ListSettingsForProtocolResponse.__doc__ = """Attributes:
+    protocol_settings:
+        Any protocol settings not covered by the above structures, for
+        example those required for custom-scripts.
+"""
+ListProtocolOutputDirFilesResponse.__doc__ = """Attributes:
+    directories:
+        List of sub-directories in the directory specified
+    files:
+        List of files in the directory specified
+    current_listed_path:
+        The absolute directory that is being listed within this
+        response
+"""
+FeatureList.__doc__ = """Attributes:
+    feature_flags:
+        feature_flags is a special value  If false, turns off all
+        other feature flags If true, allows individual flags to be
+        enabled and disabled
+"""
+GetFlowCellTypesResponse.__doc__ = """Response message for `ManagerService.get_flow_cell_types`.
+
+Attributes:
+    types:
+        The flow cell types.
+"""
+FlowCellPosition.Location.__doc__ = """Attributes:
+    x:
+        The column (counting from 0, left-to-right) of the flow cell
+        position on the sequencing unit when viewed from above/in
+        front.
+    y:
+        The row (counting from 0, top-to-bottom) of the flow cell
+        position on the sequencing unit when viewed from above/in
+        front.
+"""
+RemoveSimulatedDeviceRequest.__doc__ = """Attributes:
+    name:
+        The name of the simulated device to be removed
+"""
+ListSettingsForProtocolResponse.Output.__doc__ = """Output"""
+GetSequencingKitsRequest.__doc__ = """Request message for `ManagerService.get_sequencing_kits`.
+
+Attributes:
+    flow_cell_product_code:
+        The product code of the flow cell that will be used for
+        sequencing.  Only kits compatible with this flow cell type
+        will be returned (currently, this means that there is at least
+        one (sequencing or control) protocol that is compatible with
+        both the kit and this flow cell product code).  This may also
+        affect the returned information about the kit. For example, if
+        it isn't possible to basecall on the flow cell, none of the
+        kits will claim to be barcoding capable (or compatible with
+        any barcoding expansion kits).
+"""
+GetBarcodeKitInfoResponse.__doc__ = """Attributes:
+    barcode_kit_info:
+        Map of barcode kit name to barcode kit info
+"""
+FlowCellPosition.__doc__ = """Attributes:
+    name:
+        The name of the position.  For MinIONs, this is the name of
+        the MinION (eg: MN12345). For integrated positions, this is
+        the label for the position on the sequencer (eg: X1 for
+        GridION, 1-A1-D1 for PromethION).
+    location:
+        For integrated flow cell positions, indicates where it is on
+        the sequencing unit.  This information is not provided for
+        MinIONs (except for the MinION Mk1C, in which case the
+        position is always 0, 0).
+    state:
+        The state of the flow cell position.  If the state is not
+        `STATE_RUNNING` or `STATE_INITIALISING`, the flow cell
+        position can be assumed to be unusable, and the `error_info`
+        field should be populated.
+    rpc_ports:
+        The ports the APIs for this flow cell position are provided
+        on.  Always provided if `state` is `STATE_RUNNING`. May also
+        be provided when `state` is one of the hardware errors if the
+        software is still running.
+    error_info:
+        Provides a textual description of error states.  When `state`
+        is not `STATE_INITIALISING`, `STATE_RUNNING` or
+        `STATE_RESETTING`, this provides some information (in English)
+        about the error. This will be a textual description of the
+        value in `state`, possibly with extra information about the
+        error (if available).  This can be useful for dealing with
+        (new) unknown states.
+    shared_hardware_group:
+        Some positions may share hardware. Positions that share
+        hardware will have the same group-id. If positions do share
+        hardware, to reset the hardware you will need to reset all
+        positions in the group at the same time.
+    is_integrated:
+        Indicates that this is an integrated flow cell position.  This
+        is true for the integrated positions on a PromethION, GridION
+        or MinION Mk1C, and false for a MinION Mk1B.  Integrated
+        positions are always listed, even if (due to some hardware
+        error) they can't be found. They are never in
+        STATE_HARDWARE_REMOVED, and they always report a location.
+        Additionally, integrated positions cannot be associated
+        independently - if they are in STATE_NEEDS_ASSOCIATION, then
+        the host as a whole needs associating. Likewise, either all
+        integrated positions can run offline, or none of them can.
+        Since 4.4
+    can_sequence_offline:
+        Indicates that this position can sequence offline.  For
+        integrated positions, this is the same as the corresponding
+        field returned from the describe_host RPC.
+    protocol_state:
+        Indicates the state of the last or current protocol on the
+        flow cell position.  Since 5.0.
+    is_simulated:
+        Whether the device is simulated.  If this is true, there is no
+        physical device - MinKNOW is simulating it. If it is false,
+        MinKNOW will be acquiring data from a real device.  Since 5.2
+    device_type:
+        The type of the device.  Since 5.2
+    parent_name:
+        The name of the device this flow cell position is part of.
+        For an integrated position, this will be the host serial, as
+        returned by describe_host().  For a MinION Mk1B, this will be
+        the same as the `name` field.  For a P2 Solo, this will be the
+        name of the P2 Solo unit.  Since 5.3
+"""
+AssociationDeviceCodeResponse.__doc__ = """Attributes:
+    code:
+        The code required to associate the device with an account.  If
+        the request had `offline` set, this code is suitable for use
+        in the customer portal offline association page. Otherwise, it
+        is suitable for the online association APIs.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/acquisition_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/acquisition_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/acquisition_service.py` & `minknow_api-5.5.2/minknow_api/acquisition_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/analysis_configuration_pb2.py` & `minknow_api-5.5.2/minknow_api/analysis_configuration_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1427 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: minknow_api/analysis_configuration.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(minknow_api/analysis_configuration.proto\x12\"minknow_api.analysis_configuration\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1dminknow_api/rpc_options.proto\"\xca\x01\n\x0e\x45ventDetection\x12\x13\n\x0bwindow_size\x18\x03 \x01(\r\x12\x11\n\tthreshold\x18\x05 \x01(\x01\x12\x13\n\x0bpeak_height\x18\t \x01(\x01\x12:\n\x14\x65vents_to_base_ratio\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x1c\n\x14\x62reak_on_mux_changes\x18\x11 \x01(\x08\x12!\n\x19max_mux_change_back_shift\x18\x12 \x01(\r\"\xf0\x04\n\x13ReadDetectionParams\x12W\n\x04mode\x18\x01 \x01(\x0e\x32I.minknow_api.analysis_configuration.ReadDetectionParams.ReadDetectionMode\x12\x1a\n\x12minimum_delta_mean\x18\x02 \x01(\x01\x12\x11\n\tlook_back\x18\x03 \x01(\r\x12>\n\x18\x62reak_reads_after_events\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12?\n\x19\x62reak_reads_after_seconds\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\"\n\x1a\x62reak_reads_on_mux_changes\x18\x06 \x01(\x08\x12\x33\n\ropen_pore_min\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\ropen_pore_max\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11open_pore_default\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12@\n\x1aopen_pore_seconds_required\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"G\n\x11ReadDetectionMode\x12\x08\n\x04none\x10\x00\x12\x0e\n\ntransition\x10\x01\x12\x0c\n\x08lookback\x10\x02\x12\n\n\x06minmax\x10\x03\"q\n\x0bReadFilters\x12\x17\n\x0fread_length_min\x18\x01 \x01(\r\x12\x17\n\x0fread_length_max\x18\x02 \x01(\r\x12\x17\n\x0f\x65vent_count_min\x18\x03 \x01(\r\x12\x17\n\x0f\x65vent_count_max\x18\x04 \x01(\r\"\xc9\x04\n\x18ReadClassificationParams\x12Z\n\rscheme_module\x18\x01 \x01(\x0e\x32\x43.minknow_api.analysis_configuration.ReadClassificationParams.Scheme\x12\x35\n\x0fmax_sample_size\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12 \n\x18selected_classifications\x18\x03 \x03(\t\x12!\n\x19open_pore_classifications\x18\x06 \x03(\t\x12;\n\x15open_pore_ewma_weight\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12J\n$open_pore_ignore_after_reset_seconds\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x1f\n\x17\x63lassification_strategy\x18\x04 \x01(\t\x12[\n\nparameters\x18\x05 \x01(\x0b\x32G.minknow_api.analysis_configuration.ReadClassificationParams.Parameters\x1a.\n\nParameters\x12 \n\x18rules_in_execution_order\x18\x02 \x03(\t\"\x1e\n\x06Scheme\x12\x08\n\x04none\x10\x00\x12\n\n\x06parsed\x10\x01\"\xdd\x07\n\rChannelStates\x12\x46\n\x05group\x18\x02 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Group\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x46\n\x05logic\x18\x03 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Logic\x12\x46\n\x05style\x18\x04 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Style\x1a\xaa\x04\n\x05Logic\x12\x10\n\x08\x63riteria\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x03 \x01(\x05\x12\x0f\n\x07pattern\x18\x04 \x01(\t\x12\x16\n\x0e\x63lassification\x18\x05 \x01(\t\x12N\n\x06ranges\x18\x06 \x01(\x0b\x32>.minknow_api.analysis_configuration.ChannelStates.Logic.Ranges\x12T\n\tbehaviour\x18\x07 \x01(\x0b\x32\x41.minknow_api.analysis_configuration.ChannelStates.Logic.Behaviour\x1a\xa4\x01\n\tBehaviour\x12\x1b\n\x13reset_on_mux_change\x18\x01 \x01(\x05\x12\x1c\n\x14reset_on_well_change\x18\x02 \x01(\x05\x12\r\n\x05latch\x18\x03 \x01(\x05\x12%\n\x1dreset_on_effective_mux_change\x18\x04 \x01(\x05\x12&\n\x1ereset_on_effective_well_change\x18\x05 \x01(\x05\x1a\x8a\x01\n\x06Ranges\x12S\n\x05range\x18\x01 \x01(\x0b\x32\x44.minknow_api.analysis_configuration.ChannelStates.Logic.Ranges.Range\x1a+\n\x05Range\x12\x10\n\x08lower_pa\x18\x01 \x01(\x05\x12\x10\n\x08upper_pa\x18\x02 \x01(\x05\x1aS\n\x05Style\x12+\n\x05order\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\r\n\x05label\x18\x02 \x01(\t\x12\x0e\n\x06\x63olour\x18\x03 \x01(\t\x1a]\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x46\n\x05style\x18\x02 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Style\"!\n\x1fGetAnalysisConfigurationRequest\"\x91\x03\n\x11ReadScalingParams\x12\x1a\n\x12quantile_locations\x18\x03 \x03(\x02\x12\x1e\n\x16quantile_weights_shift\x18\x01 \x03(\x02\x12\x1e\n\x16quantile_weights_scale\x18\x02 \x03(\x02\x12\x16\n\x0etracking_alpha\x18\x04 \x01(\x02\x12$\n\x1c\x61lpha_number_estimates_decay\x18\x05 \x01(\x02\x12\x18\n\x10quantile_maxdiff\x18\n \x01(\x02\x12\x1c\n\x14trust_limit_fraction\x18\x06 \x01(\x02\x12\x16\n\x0e\x64iff_threshold\x18\x07 \x01(\x02\x12\x1a\n\x12\x65mission_threshold\x18\x08 \x01(\x02\x12\x17\n\x0f\x64\x61\x63s_breakpoint\x18\t \x01(\x02\x12 \n\x18\x63onductance_factor_scale\x18\x0b \x01(\x02\x12 \n\x18\x63onductance_factor_shift\x18\x0c \x01(\x02\x12\x19\n\x11q90_q10_to_normal\x18\r \x01(\x02\"\xac\x04\n\x15\x41nalysisConfiguration\x12K\n\x0f\x65vent_detection\x18\x01 \x01(\x0b\x32\x32.minknow_api.analysis_configuration.EventDetection\x12O\n\x0eread_detection\x18\x02 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ReadDetectionParams\x12Y\n\x13read_classification\x18\x04 \x01(\x0b\x32<.minknow_api.analysis_configuration.ReadClassificationParams\x12\x64\n\x0e\x63hannel_states\x18\x07 \x03(\x0b\x32L.minknow_api.analysis_configuration.AnalysisConfiguration.ChannelStatesEntry\x12K\n\x0cread_scaling\x18\x08 \x01(\x0b\x32\x35.minknow_api.analysis_configuration.ReadScalingParams\x1ag\n\x12\x43hannelStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12@\n\x05value\x18\x02 \x01(\x0b\x32\x31.minknow_api.analysis_configuration.ChannelStates:\x02\x38\x01\"\"\n SetAnalysisConfigurationResponse\"#\n!ResetAnalysisConfigurationRequest\"$\n\"ResetAnalysisConfigurationResponse\"6\n\x1eSetAnalysisEnabledStateRequest\x12\x14\n\x06\x65nable\x18\x01 \x01(\x08\x42\x04\x88\xb5\x18\x01\"!\n\x1fSetAnalysisEnabledStateResponse\"\x1d\n\x1bGetChannelStatesDescRequest\"\x99\x04\n\x1cGetChannelStatesDescResponse\x12V\n\x06groups\x18\x01 \x03(\x0b\x32\x46.minknow_api.analysis_configuration.GetChannelStatesDescResponse.Group\x1a;\n\x05Style\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06\x63olour\x18\x03 \x01(\t\x1a\x95\x01\n\x0c\x43hannelState\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12U\n\x05style\x18\x03 \x01(\x0b\x32\x46.minknow_api.analysis_configuration.GetChannelStatesDescResponse.Style\x12\x14\n\x0cglobal_order\x18\x04 \x01(\r\x1a\xcb\x01\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\x12U\n\x05style\x18\x02 \x01(\x0b\x32\x46.minknow_api.analysis_configuration.GetChannelStatesDescResponse.Style\x12]\n\x06states\x18\x03 \x03(\x0b\x32M.minknow_api.analysis_configuration.GetChannelStatesDescResponse.ChannelState\"\x13\n\x11GetSummaryRequest\"K\n\x12GetSummaryResponse\x12\x18\n\x10\x61nalysis_enabled\x18\x01 \x01(\x08\x12\x1b\n\x13\x62\x61secalling_enabled\x18\x02 \x01(\x08\"\xdd\x02\n\x16\x42\x61rcodingConfiguration\x12\x16\n\x0e\x62\x61rcoding_kits\x18\x01 \x03(\t\x12\x15\n\rtrim_barcodes\x18\x02 \x01(\x08\x12\"\n\x1arequire_barcodes_both_ends\x18\x03 \x01(\x08\x12\"\n\x1a\x64\x65tect_mid_strand_barcodes\x18\x04 \x01(\x08\x12.\n\tmin_score\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x33\n\x0emin_score_rear\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x32\n\rmin_score_mid\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x33\n\x0emin_score_mask\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xae\x01\n\x16\x41lignmentConfiguration\x12\x17\n\x0freference_files\x18\x01 \x03(\t\x12\x10\n\x08\x62\x65\x64_file\x18\x02 \x01(\t\x12\x35\n\x10minimum_coverage\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x32\n*aggregate_statistics_for_multiple_bed_hits\x18\x04 \x01(\x08\"\xcc\x01\n\x11LampConfiguration\x12\x10\n\x08lamp_kit\x18\x01 \x01(\t\x12\x37\n\x12min_score_barcodes\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x34\n\x0fmin_score_masks\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x36\n\x11min_score_targets\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xfa\x08\n\x17\x42\x61secallerConfiguration\x12\x0e\n\x06\x65nable\x18\x02 \x01(\x08\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\x12\x14\n\x0c\x61lign_filter\x18\n \x01(\x08\x12\x61\n\x0eread_filtering\x18\x03 \x01(\x0b\x32I.minknow_api.analysis_configuration.BasecallerConfiguration.ReadFiltering\x12[\n\x17\x62\x61rcoding_configuration\x18\x04 \x01(\x0b\x32:.minknow_api.analysis_configuration.BarcodingConfiguration\x12\x65\n\x10target_filtering\x18\x05 \x01(\x0b\x32K.minknow_api.analysis_configuration.BasecallerConfiguration.TargetFiltering\x12[\n\x17\x61lignment_configuration\x18\x06 \x01(\x0b\x32:.minknow_api.analysis_configuration.AlignmentConfiguration\x12Q\n\x12lamp_configuration\x18\x07 \x01(\x0b\x32\x35.minknow_api.analysis_configuration.LampConfiguration\x12\x1d\n\x15\x65nable_read_splitting\x18\x08 \x01(\x08\x12=\n\x18min_score_read_splitting\x18\t \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x1a\xc2\x02\n\rReadFiltering\x12\x30\n\nmin_qscore\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0bmin_samples\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmax_samples\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12/\n\tmin_bases\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12/\n\tmax_bases\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x37\n\x11max_failed_chunks\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x1a\xa5\x01\n\x0fTargetFiltering\x12\x30\n\nmin_qscore\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12/\n\tmin_bases\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12/\n\tmax_bases\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\"w\n!SetBasecallerConfigurationRequest\x12R\n\x07\x63onfigs\x18\x01 \x01(\x0b\x32;.minknow_api.analysis_configuration.BasecallerConfigurationB\x04\x90\xb5\x18\x01\"$\n\"SetBasecallerConfigurationResponse\"#\n!GetBasecallerConfigurationRequest\"!\n\x1fGetPoreTypeConfigurationRequest\"\xab\x05\n\x15PoreTypeConfiguration\x12\x1a\n\x10global_pore_type\x18\x01 \x01(\tH\x00\x12~\n\x17\x63hannel_well_pore_types\x18\x02 \x01(\x0b\x32[.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurationsH\x00\x1a,\n\x0b\x43hannelWell\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\r\x12\x0c\n\x04well\x18\x02 \x01(\r\x1a\xb3\x03\n!ChannelWellPoreTypeConfigurations\x12~\n\npore_types\x18\x01 \x03(\x0b\x32j.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.PoreTypesEntry\x1an\n\x0f\x43hannelWellList\x12[\n\x0c\x63hannel_well\x18\x01 \x03(\x0b\x32\x45.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWell\x1a\x9d\x01\n\x0ePoreTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12z\n\x05value\x18\x02 \x01(\x0b\x32k.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.ChannelWellList:\x02\x38\x01\x42\x12\n\x10pore_type_config\"\"\n SetPoreTypeConfigurationResponse\"\x83#\n\x13WriterConfiguration\x12\x62\n\nread_fast5\x18\x02 \x01(\x0b\x32N.minknow_api.analysis_configuration.WriterConfiguration.ReadFast5Configuration\x12\x62\n\nread_fastq\x18\x03 \x01(\x0b\x32N.minknow_api.analysis_configuration.WriterConfiguration.ReadFastqConfiguration\x12^\n\x08read_bam\x18\x08 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ReadBamConfiguration\x12`\n\tread_pod5\x18\n \x01(\x0b\x32M.minknow_api.analysis_configuration.WriterConfiguration.ReadPod5Configuration\x12h\n\rread_protobuf\x18\x04 \x01(\x0b\x32Q.minknow_api.analysis_configuration.WriterConfiguration.ReadProtobufConfiguration\x12r\n\x12sequencing_summary\x18\x05 \x01(\x0b\x32V.minknow_api.analysis_configuration.WriterConfiguration.SequencingSummaryConfiguration\x12W\n\x04\x62ulk\x18\x06 \x01(\x0b\x32I.minknow_api.analysis_configuration.WriterConfiguration.BulkConfiguration\x12[\n\x06report\x18\x07 \x01(\x0b\x32K.minknow_api.analysis_configuration.WriterConfiguration.ReportConfiguration\x12\x45\n\x0cread_filters\x18\t \x01(\x0b\x32/.minknow_api.analysis_configuration.ReadFilters\x1a\xff\x03\n\x14\x43hannelConfiguration\x12\x16\n\x0c\x61ll_channels\x18\x01 \x01(\x08H\x00\x12u\n\x11specific_channels\x18\x02 \x01(\x0b\x32X.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelListH\x00\x12t\n\x0e\x63hannel_ranges\x18\x03 \x01(\x0b\x32Z.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelRangesH\x00\x1a\x1f\n\x0b\x43hannelList\x12\x10\n\x08\x63hannels\x18\x01 \x03(\x05\x1a\xb4\x01\n\rChannelRanges\x12w\n\x06ranges\x18\x01 \x03(\x0b\x32g.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelRanges.ChannelRange\x1a*\n\x0c\x43hannelRange\x12\r\n\x05start\x18\x01 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x05\x42\n\n\x08\x63hannels\x1a\xc0\x06\n\x16ReadFast5Configuration\x12\x19\n\x11\x63ompression_level\x18\x01 \x01(\x05\x12\x61\n\x10\x63ompression_type\x18\x0e \x01(\x0e\x32G.minknow_api.analysis_configuration.WriterConfiguration.CompressionType\x12Y\n\x03raw\x18\x02 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12[\n\x05\x66\x61stq\x18\x03 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x61\n\x0btrace_table\x18\x0b \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12`\n\nmove_table\x18\x0c \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12i\n\x13modifications_table\x18\r \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12$\n\x1c\x64isable_writing_passed_reads\x18\x05 \x01(\x08\x12$\n\x1c\x64isable_writing_failed_reads\x18\x06 \x01(\x08\x12+\n#disable_writing_force_skipped_reads\x18\x07 \x01(\x08\x12\x14\n\x0c\x66ile_pattern\x18\x08 \x01(\t\x12\x1c\n\x14\x66\x61stq_header_pattern\x18\t \x01(\t\x12\x13\n\x0b\x62\x61tch_count\x18\n \x01(\r\x1a\xce\x01\n\x16ReadFastqConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x16\n\x0eheader_pattern\x18\x03 \x01(\t\x12\x13\n\x0b\x62\x61tch_count\x18\x04 \x01(\r\x12\x13\n\x0b\x63ompression\x18\x05 \x01(\x08\x1a\xcc\x01\n\x14ReadBamConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x13\n\x0b\x62\x61tch_count\x18\x03 \x01(\r\x12+\n#disable_writing_multiple_alignments\x18\x04 \x01(\x08\x1a\x99\x02\n\x15ReadPod5Configuration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x13\n\x0b\x62\x61tch_count\x18\x03 \x01(\r\x12$\n\x1c\x64isable_writing_passed_reads\x18\x04 \x01(\x08\x12$\n\x1c\x64isable_writing_failed_reads\x18\x05 \x01(\x08\x12+\n#disable_writing_force_skipped_reads\x18\x06 \x01(\x08\x1a\xa4\x01\n\x19ReadProtobufConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x13\n\x0b\x62\x61tch_count\x18\x03 \x01(\r\x1a\x94\x01\n\x1eSequencingSummaryConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x1a\xd7\x05\n\x11\x42ulkConfiguration\x12\x19\n\x11\x63ompression_level\x18\x02 \x01(\x05\x12\x61\n\x10\x63ompression_type\x18\r \x01(\x0e\x32G.minknow_api.analysis_configuration.WriterConfiguration.CompressionType\x12\x14\n\x0c\x66ile_pattern\x18\x0e \x01(\t\x12Y\n\x03raw\x18\x03 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\\\n\x06\x65vents\x18\x04 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12[\n\x05reads\x18\x05 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12_\n\tmultiplex\x18\x06 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x64\n\x0e\x63hannel_states\x18\x07 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x17\n\x0f\x64\x65vice_metadata\x18\x0b \x01(\x08\x12\x17\n\x0f\x64\x65vice_commands\x18\x0c \x01(\x08\x12\x1f\n\x17\x64ynamic_analysis_config\x18\x0f \x01(\x08\x1a\x99\x03\n\x13ReportConfiguration\x12\x1f\n\x17pdf_report_file_pattern\x18\x01 \x01(\t\x12 \n\x18json_report_file_pattern\x18\x02 \x01(\t\x12 \n\x18html_report_file_pattern\x18\t \x01(\t\x12$\n\x1cmarkdown_report_file_pattern\x18\x08 \x01(\t\x12%\n\x1d\x64uty_time_report_file_pattern\x18\x03 \x01(\t\x12&\n\x1ethroughput_report_file_pattern\x18\x04 \x01(\t\x12)\n!final_summary_report_file_pattern\x18\x05 \x01(\t\x12-\n%barcode_alignment_report_file_pattern\x18\x06 \x01(\t\x12(\n sample_sheet_report_file_pattern\x18\n \x01(\t\x12$\n\x1c\x63ustom_report_suffix_pattern\x18\x07 \x01(\t\"R\n\x0f\x43ompressionType\x12\x16\n\x12\x44\x65\x66\x61ultCompression\x10\x00\x12\x13\n\x0fZlibCompression\x10\x01\x12\x12\n\x0eVbzCompression\x10\x02\" \n\x1eSetWriterConfigurationResponse\"\x1f\n\x1dGetWriterConfigurationRequest\"\x1f\n\x1dGetReadClassificationsRequest\"\xd7\x01\n\x1eGetReadClassificationsResponse\x12y\n\x14read_classifications\x18\x01 \x03(\x0b\x32[.minknow_api.analysis_configuration.GetReadClassificationsResponse.ReadClassificationsEntry\x1a:\n\x18ReadClassificationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xfc\x02\n\x1c\x44ynamicAnalysisConfiguration\x12o\n\x13read_scale_tracking\x18\x01 \x01(\x0b\x32R.minknow_api.analysis_configuration.DynamicAnalysisConfiguration.ReadScaleTracking\x1a\xea\x01\n\x11ReadScaleTracking\x12 \n\x18\x63onductance_scan_voltage\x18\x01 \x01(\x02\x12\x82\x01\n\x13\x63hannel_conductance\x18\x02 \x03(\x0b\x32\x65.minknow_api.analysis_configuration.DynamicAnalysisConfiguration.ReadScaleTracking.ChannelConductance\x1a.\n\x12\x43hannelConductance\x12\x18\n\x10well_conductance\x18\x01 \x03(\x02\"(\n&GetDynamicAnalysisConfigurationRequest\")\n\'SetDynamicAnalysisConfigurationResponse2\xac\x15\n\x1c\x41nalysisConfigurationService\x12\xa1\x01\n\x1aget_analysis_configuration\x12\x43.minknow_api.analysis_configuration.GetAnalysisConfigurationRequest\x1a\x39.minknow_api.analysis_configuration.AnalysisConfiguration\"\x03\x90\x02\x01\x12\xa2\x01\n\x1aset_analysis_configuration\x12\x39.minknow_api.analysis_configuration.AnalysisConfiguration\x1a\x44.minknow_api.analysis_configuration.SetAnalysisConfigurationResponse\"\x03\x90\x02\x02\x12\xb2\x01\n\x1creset_analysis_configuration\x12\x45.minknow_api.analysis_configuration.ResetAnalysisConfigurationRequest\x1a\x46.minknow_api.analysis_configuration.ResetAnalysisConfigurationResponse\"\x03\x90\x02\x02\x12\xaa\x01\n\x1aset_analysis_enabled_state\x12\x42.minknow_api.analysis_configuration.SetAnalysisEnabledStateRequest\x1a\x43.minknow_api.analysis_configuration.SetAnalysisEnabledStateResponse\"\x03\x90\x02\x02\x12\xa1\x01\n\x17get_channel_states_desc\x12?.minknow_api.analysis_configuration.GetChannelStatesDescRequest\x1a@.minknow_api.analysis_configuration.GetChannelStatesDescResponse\"\x03\x90\x02\x01\x12\x81\x01\n\x0bget_summary\x12\x35.minknow_api.analysis_configuration.GetSummaryRequest\x1a\x36.minknow_api.analysis_configuration.GetSummaryResponse\"\x03\x90\x02\x01\x12\xb2\x01\n\x1cset_basecaller_configuration\x12\x45.minknow_api.analysis_configuration.SetBasecallerConfigurationRequest\x1a\x46.minknow_api.analysis_configuration.SetBasecallerConfigurationResponse\"\x03\x90\x02\x02\x12\xb6\x01\n preload_basecaller_configuration\x12\x45.minknow_api.analysis_configuration.SetBasecallerConfigurationRequest\x1a\x46.minknow_api.analysis_configuration.SetBasecallerConfigurationResponse\"\x03\x90\x02\x02\x12\xa7\x01\n\x1cget_basecaller_configuration\x12\x45.minknow_api.analysis_configuration.GetBasecallerConfigurationRequest\x1a;.minknow_api.analysis_configuration.BasecallerConfiguration\"\x03\x90\x02\x01\x12\xa2\x01\n\x1bget_pore_type_configuration\x12\x43.minknow_api.analysis_configuration.GetPoreTypeConfigurationRequest\x1a\x39.minknow_api.analysis_configuration.PoreTypeConfiguration\"\x03\x90\x02\x01\x12\xa3\x01\n\x1bset_pore_type_configuration\x12\x39.minknow_api.analysis_configuration.PoreTypeConfiguration\x1a\x44.minknow_api.analysis_configuration.SetPoreTypeConfigurationResponse\"\x03\x90\x02\x02\x12\x9c\x01\n\x18set_writer_configuration\x12\x37.minknow_api.analysis_configuration.WriterConfiguration\x1a\x42.minknow_api.analysis_configuration.SetWriterConfigurationResponse\"\x03\x90\x02\x02\x12\x9b\x01\n\x18get_writer_configuration\x12\x41.minknow_api.analysis_configuration.GetWriterConfigurationRequest\x1a\x37.minknow_api.analysis_configuration.WriterConfiguration\"\x03\x90\x02\x01\x12\xa6\x01\n\x18get_read_classifications\x12\x41.minknow_api.analysis_configuration.GetReadClassificationsRequest\x1a\x42.minknow_api.analysis_configuration.GetReadClassificationsResponse\"\x03\x90\x02\x01\x12\xb7\x01\n\"get_dynamic_analysis_configuration\x12J.minknow_api.analysis_configuration.GetDynamicAnalysisConfigurationRequest\x1a@.minknow_api.analysis_configuration.DynamicAnalysisConfiguration\"\x03\x90\x02\x01\x12\xb5\x01\n\"set_dynamic_analysis_configuration\x12@.minknow_api.analysis_configuration.DynamicAnalysisConfiguration\x1aK.minknow_api.analysis_configuration.SetDynamicAnalysisConfigurationResponse\"\x00\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(minknow_api/analysis_configuration.proto\x12\"minknow_api.analysis_configuration\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1dminknow_api/rpc_options.proto\"\xca\x01\n\x0e\x45ventDetection\x12\x13\n\x0bwindow_size\x18\x03 \x01(\r\x12\x11\n\tthreshold\x18\x05 \x01(\x01\x12\x13\n\x0bpeak_height\x18\t \x01(\x01\x12:\n\x14\x65vents_to_base_ratio\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x1c\n\x14\x62reak_on_mux_changes\x18\x11 \x01(\x08\x12!\n\x19max_mux_change_back_shift\x18\x12 \x01(\r\"\xf0\x04\n\x13ReadDetectionParams\x12W\n\x04mode\x18\x01 \x01(\x0e\x32I.minknow_api.analysis_configuration.ReadDetectionParams.ReadDetectionMode\x12\x1a\n\x12minimum_delta_mean\x18\x02 \x01(\x01\x12\x11\n\tlook_back\x18\x03 \x01(\r\x12>\n\x18\x62reak_reads_after_events\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12?\n\x19\x62reak_reads_after_seconds\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\"\n\x1a\x62reak_reads_on_mux_changes\x18\x06 \x01(\x08\x12\x33\n\ropen_pore_min\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\ropen_pore_max\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11open_pore_default\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12@\n\x1aopen_pore_seconds_required\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"G\n\x11ReadDetectionMode\x12\x08\n\x04none\x10\x00\x12\x0e\n\ntransition\x10\x01\x12\x0c\n\x08lookback\x10\x02\x12\n\n\x06minmax\x10\x03\"q\n\x0bReadFilters\x12\x17\n\x0fread_length_min\x18\x01 \x01(\r\x12\x17\n\x0fread_length_max\x18\x02 \x01(\r\x12\x17\n\x0f\x65vent_count_min\x18\x03 \x01(\r\x12\x17\n\x0f\x65vent_count_max\x18\x04 \x01(\r\"\xc9\x04\n\x18ReadClassificationParams\x12Z\n\rscheme_module\x18\x01 \x01(\x0e\x32\x43.minknow_api.analysis_configuration.ReadClassificationParams.Scheme\x12\x35\n\x0fmax_sample_size\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12 \n\x18selected_classifications\x18\x03 \x03(\t\x12!\n\x19open_pore_classifications\x18\x06 \x03(\t\x12;\n\x15open_pore_ewma_weight\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12J\n$open_pore_ignore_after_reset_seconds\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x1f\n\x17\x63lassification_strategy\x18\x04 \x01(\t\x12[\n\nparameters\x18\x05 \x01(\x0b\x32G.minknow_api.analysis_configuration.ReadClassificationParams.Parameters\x1a.\n\nParameters\x12 \n\x18rules_in_execution_order\x18\x02 \x03(\t\"\x1e\n\x06Scheme\x12\x08\n\x04none\x10\x00\x12\n\n\x06parsed\x10\x01\"\xdd\x07\n\rChannelStates\x12\x46\n\x05group\x18\x02 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Group\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x46\n\x05logic\x18\x03 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Logic\x12\x46\n\x05style\x18\x04 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Style\x1a\xaa\x04\n\x05Logic\x12\x10\n\x08\x63riteria\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x03 \x01(\x05\x12\x0f\n\x07pattern\x18\x04 \x01(\t\x12\x16\n\x0e\x63lassification\x18\x05 \x01(\t\x12N\n\x06ranges\x18\x06 \x01(\x0b\x32>.minknow_api.analysis_configuration.ChannelStates.Logic.Ranges\x12T\n\tbehaviour\x18\x07 \x01(\x0b\x32\x41.minknow_api.analysis_configuration.ChannelStates.Logic.Behaviour\x1a\xa4\x01\n\tBehaviour\x12\x1b\n\x13reset_on_mux_change\x18\x01 \x01(\x05\x12\x1c\n\x14reset_on_well_change\x18\x02 \x01(\x05\x12\r\n\x05latch\x18\x03 \x01(\x05\x12%\n\x1dreset_on_effective_mux_change\x18\x04 \x01(\x05\x12&\n\x1ereset_on_effective_well_change\x18\x05 \x01(\x05\x1a\x8a\x01\n\x06Ranges\x12S\n\x05range\x18\x01 \x01(\x0b\x32\x44.minknow_api.analysis_configuration.ChannelStates.Logic.Ranges.Range\x1a+\n\x05Range\x12\x10\n\x08lower_pa\x18\x01 \x01(\x05\x12\x10\n\x08upper_pa\x18\x02 \x01(\x05\x1aS\n\x05Style\x12+\n\x05order\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\r\n\x05label\x18\x02 \x01(\t\x12\x0e\n\x06\x63olour\x18\x03 \x01(\t\x1a]\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x46\n\x05style\x18\x02 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ChannelStates.Style\"!\n\x1fGetAnalysisConfigurationRequest\"\x91\x03\n\x11ReadScalingParams\x12\x1a\n\x12quantile_locations\x18\x03 \x03(\x02\x12\x1e\n\x16quantile_weights_shift\x18\x01 \x03(\x02\x12\x1e\n\x16quantile_weights_scale\x18\x02 \x03(\x02\x12\x16\n\x0etracking_alpha\x18\x04 \x01(\x02\x12$\n\x1c\x61lpha_number_estimates_decay\x18\x05 \x01(\x02\x12\x18\n\x10quantile_maxdiff\x18\n \x01(\x02\x12\x1c\n\x14trust_limit_fraction\x18\x06 \x01(\x02\x12\x16\n\x0e\x64iff_threshold\x18\x07 \x01(\x02\x12\x1a\n\x12\x65mission_threshold\x18\x08 \x01(\x02\x12\x17\n\x0f\x64\x61\x63s_breakpoint\x18\t \x01(\x02\x12 \n\x18\x63onductance_factor_scale\x18\x0b \x01(\x02\x12 \n\x18\x63onductance_factor_shift\x18\x0c \x01(\x02\x12\x19\n\x11q90_q10_to_normal\x18\r \x01(\x02\"\xac\x04\n\x15\x41nalysisConfiguration\x12K\n\x0f\x65vent_detection\x18\x01 \x01(\x0b\x32\x32.minknow_api.analysis_configuration.EventDetection\x12O\n\x0eread_detection\x18\x02 \x01(\x0b\x32\x37.minknow_api.analysis_configuration.ReadDetectionParams\x12Y\n\x13read_classification\x18\x04 \x01(\x0b\x32<.minknow_api.analysis_configuration.ReadClassificationParams\x12\x64\n\x0e\x63hannel_states\x18\x07 \x03(\x0b\x32L.minknow_api.analysis_configuration.AnalysisConfiguration.ChannelStatesEntry\x12K\n\x0cread_scaling\x18\x08 \x01(\x0b\x32\x35.minknow_api.analysis_configuration.ReadScalingParams\x1ag\n\x12\x43hannelStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12@\n\x05value\x18\x02 \x01(\x0b\x32\x31.minknow_api.analysis_configuration.ChannelStates:\x02\x38\x01\"\"\n SetAnalysisConfigurationResponse\"#\n!ResetAnalysisConfigurationRequest\"$\n\"ResetAnalysisConfigurationResponse\"6\n\x1eSetAnalysisEnabledStateRequest\x12\x14\n\x06\x65nable\x18\x01 \x01(\x08\x42\x04\x88\xb5\x18\x01\"!\n\x1fSetAnalysisEnabledStateResponse\"\x1d\n\x1bGetChannelStatesDescRequest\"\x99\x04\n\x1cGetChannelStatesDescResponse\x12V\n\x06groups\x18\x01 \x03(\x0b\x32\x46.minknow_api.analysis_configuration.GetChannelStatesDescResponse.Group\x1a;\n\x05Style\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06\x63olour\x18\x03 \x01(\t\x1a\x95\x01\n\x0c\x43hannelState\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12U\n\x05style\x18\x03 \x01(\x0b\x32\x46.minknow_api.analysis_configuration.GetChannelStatesDescResponse.Style\x12\x14\n\x0cglobal_order\x18\x04 \x01(\r\x1a\xcb\x01\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\x12U\n\x05style\x18\x02 \x01(\x0b\x32\x46.minknow_api.analysis_configuration.GetChannelStatesDescResponse.Style\x12]\n\x06states\x18\x03 \x03(\x0b\x32M.minknow_api.analysis_configuration.GetChannelStatesDescResponse.ChannelState\"\x13\n\x11GetSummaryRequest\"K\n\x12GetSummaryResponse\x12\x18\n\x10\x61nalysis_enabled\x18\x01 \x01(\x08\x12\x1b\n\x13\x62\x61secalling_enabled\x18\x02 \x01(\x08\"\xdd\x02\n\x16\x42\x61rcodingConfiguration\x12\x16\n\x0e\x62\x61rcoding_kits\x18\x01 \x03(\t\x12\x15\n\rtrim_barcodes\x18\x02 \x01(\x08\x12\"\n\x1arequire_barcodes_both_ends\x18\x03 \x01(\x08\x12\"\n\x1a\x64\x65tect_mid_strand_barcodes\x18\x04 \x01(\x08\x12.\n\tmin_score\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x33\n\x0emin_score_rear\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x32\n\rmin_score_mid\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x33\n\x0emin_score_mask\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xae\x01\n\x16\x41lignmentConfiguration\x12\x17\n\x0freference_files\x18\x01 \x03(\t\x12\x10\n\x08\x62\x65\x64_file\x18\x02 \x01(\t\x12\x35\n\x10minimum_coverage\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x32\n*aggregate_statistics_for_multiple_bed_hits\x18\x04 \x01(\x08\"\xcc\x01\n\x11LampConfiguration\x12\x10\n\x08lamp_kit\x18\x01 \x01(\t\x12\x37\n\x12min_score_barcodes\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x34\n\x0fmin_score_masks\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x36\n\x11min_score_targets\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xfa\x08\n\x17\x42\x61secallerConfiguration\x12\x0e\n\x06\x65nable\x18\x02 \x01(\x08\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\x12\x14\n\x0c\x61lign_filter\x18\n \x01(\x08\x12\x61\n\x0eread_filtering\x18\x03 \x01(\x0b\x32I.minknow_api.analysis_configuration.BasecallerConfiguration.ReadFiltering\x12[\n\x17\x62\x61rcoding_configuration\x18\x04 \x01(\x0b\x32:.minknow_api.analysis_configuration.BarcodingConfiguration\x12\x65\n\x10target_filtering\x18\x05 \x01(\x0b\x32K.minknow_api.analysis_configuration.BasecallerConfiguration.TargetFiltering\x12[\n\x17\x61lignment_configuration\x18\x06 \x01(\x0b\x32:.minknow_api.analysis_configuration.AlignmentConfiguration\x12Q\n\x12lamp_configuration\x18\x07 \x01(\x0b\x32\x35.minknow_api.analysis_configuration.LampConfiguration\x12\x1d\n\x15\x65nable_read_splitting\x18\x08 \x01(\x08\x12=\n\x18min_score_read_splitting\x18\t \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x1a\xc2\x02\n\rReadFiltering\x12\x30\n\nmin_qscore\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0bmin_samples\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmax_samples\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12/\n\tmin_bases\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12/\n\tmax_bases\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x37\n\x11max_failed_chunks\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x1a\xa5\x01\n\x0fTargetFiltering\x12\x30\n\nmin_qscore\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12/\n\tmin_bases\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12/\n\tmax_bases\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\"w\n!SetBasecallerConfigurationRequest\x12R\n\x07\x63onfigs\x18\x01 \x01(\x0b\x32;.minknow_api.analysis_configuration.BasecallerConfigurationB\x04\x90\xb5\x18\x01\"$\n\"SetBasecallerConfigurationResponse\"#\n!GetBasecallerConfigurationRequest\"!\n\x1fGetPoreTypeConfigurationRequest\"\xab\x05\n\x15PoreTypeConfiguration\x12\x1a\n\x10global_pore_type\x18\x01 \x01(\tH\x00\x12~\n\x17\x63hannel_well_pore_types\x18\x02 \x01(\x0b\x32[.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurationsH\x00\x1a,\n\x0b\x43hannelWell\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\r\x12\x0c\n\x04well\x18\x02 \x01(\r\x1a\xb3\x03\n!ChannelWellPoreTypeConfigurations\x12~\n\npore_types\x18\x01 \x03(\x0b\x32j.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.PoreTypesEntry\x1an\n\x0f\x43hannelWellList\x12[\n\x0c\x63hannel_well\x18\x01 \x03(\x0b\x32\x45.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWell\x1a\x9d\x01\n\x0ePoreTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12z\n\x05value\x18\x02 \x01(\x0b\x32k.minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.ChannelWellList:\x02\x38\x01\x42\x12\n\x10pore_type_config\"\"\n SetPoreTypeConfigurationResponse\"\xda$\n\x13WriterConfiguration\x12\x62\n\nread_fast5\x18\x02 \x01(\x0b\x32N.minknow_api.analysis_configuration.WriterConfiguration.ReadFast5Configuration\x12\x62\n\nread_fastq\x18\x03 \x01(\x0b\x32N.minknow_api.analysis_configuration.WriterConfiguration.ReadFastqConfiguration\x12^\n\x08read_bam\x18\x08 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ReadBamConfiguration\x12`\n\tread_pod5\x18\n \x01(\x0b\x32M.minknow_api.analysis_configuration.WriterConfiguration.ReadPod5Configuration\x12h\n\rread_protobuf\x18\x04 \x01(\x0b\x32Q.minknow_api.analysis_configuration.WriterConfiguration.ReadProtobufConfiguration\x12r\n\x12sequencing_summary\x18\x05 \x01(\x0b\x32V.minknow_api.analysis_configuration.WriterConfiguration.SequencingSummaryConfiguration\x12W\n\x04\x62ulk\x18\x06 \x01(\x0b\x32I.minknow_api.analysis_configuration.WriterConfiguration.BulkConfiguration\x12[\n\x06report\x18\x07 \x01(\x0b\x32K.minknow_api.analysis_configuration.WriterConfiguration.ReportConfiguration\x12\x45\n\x0cread_filters\x18\t \x01(\x0b\x32/.minknow_api.analysis_configuration.ReadFilters\x1a\xff\x03\n\x14\x43hannelConfiguration\x12\x16\n\x0c\x61ll_channels\x18\x01 \x01(\x08H\x00\x12u\n\x11specific_channels\x18\x02 \x01(\x0b\x32X.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelListH\x00\x12t\n\x0e\x63hannel_ranges\x18\x03 \x01(\x0b\x32Z.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelRangesH\x00\x1a\x1f\n\x0b\x43hannelList\x12\x10\n\x08\x63hannels\x18\x01 \x03(\x05\x1a\xb4\x01\n\rChannelRanges\x12w\n\x06ranges\x18\x01 \x03(\x0b\x32g.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelRanges.ChannelRange\x1a*\n\x0c\x43hannelRange\x12\r\n\x05start\x18\x01 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x05\x42\n\n\x08\x63hannels\x1a\xeb\x06\n\x16ReadFast5Configuration\x12\x19\n\x11\x63ompression_level\x18\x01 \x01(\x05\x12\x61\n\x10\x63ompression_type\x18\x0e \x01(\x0e\x32G.minknow_api.analysis_configuration.WriterConfiguration.CompressionType\x12Y\n\x03raw\x18\x02 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12[\n\x05\x66\x61stq\x18\x03 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x61\n\x0btrace_table\x18\x0b \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12`\n\nmove_table\x18\x0c \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12i\n\x13modifications_table\x18\r \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12$\n\x1c\x64isable_writing_passed_reads\x18\x05 \x01(\x08\x12$\n\x1c\x64isable_writing_failed_reads\x18\x06 \x01(\x08\x12+\n#disable_writing_force_skipped_reads\x18\x07 \x01(\x08\x12\x14\n\x0c\x66ile_pattern\x18\x08 \x01(\t\x12\x1c\n\x14\x66\x61stq_header_pattern\x18\t \x01(\t\x12\x15\n\x0b\x62\x61tch_count\x18\n \x01(\rH\x00\x12\x19\n\x0f\x62\x61ses_per_batch\x18\x0f \x01(\x04H\x00\x42\x0c\n\nbatch_info\x1a\xf9\x01\n\x16ReadFastqConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x16\n\x0eheader_pattern\x18\x03 \x01(\t\x12\x15\n\x0b\x62\x61tch_count\x18\x04 \x01(\rH\x00\x12\x19\n\x0f\x62\x61ses_per_batch\x18\x06 \x01(\x04H\x00\x12\x13\n\x0b\x63ompression\x18\x05 \x01(\x08\x42\x0c\n\nbatch_info\x1a\xf7\x01\n\x14ReadBamConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x15\n\x0b\x62\x61tch_count\x18\x03 \x01(\rH\x00\x12\x19\n\x0f\x62\x61ses_per_batch\x18\x05 \x01(\x04H\x00\x12+\n#disable_writing_multiple_alignments\x18\x04 \x01(\x08\x42\x0c\n\nbatch_info\x1a\xc4\x02\n\x15ReadPod5Configuration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x15\n\x0b\x62\x61tch_count\x18\x03 \x01(\rH\x00\x12\x19\n\x0f\x62\x61ses_per_batch\x18\x07 \x01(\x04H\x00\x12$\n\x1c\x64isable_writing_passed_reads\x18\x04 \x01(\x08\x12$\n\x1c\x64isable_writing_failed_reads\x18\x05 \x01(\x08\x12+\n#disable_writing_force_skipped_reads\x18\x06 \x01(\x08\x42\x0c\n\nbatch_info\x1a\xcf\x01\n\x19ReadProtobufConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x12\x15\n\x0b\x62\x61tch_count\x18\x03 \x01(\rH\x00\x12\x19\n\x0f\x62\x61ses_per_batch\x18\x04 \x01(\x04H\x00\x42\x0c\n\nbatch_info\x1a\x94\x01\n\x1eSequencingSummaryConfiguration\x12\\\n\x06\x65nable\x18\x01 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x14\n\x0c\x66ile_pattern\x18\x02 \x01(\t\x1a\xd7\x05\n\x11\x42ulkConfiguration\x12\x19\n\x11\x63ompression_level\x18\x02 \x01(\x05\x12\x61\n\x10\x63ompression_type\x18\r \x01(\x0e\x32G.minknow_api.analysis_configuration.WriterConfiguration.CompressionType\x12\x14\n\x0c\x66ile_pattern\x18\x0e \x01(\t\x12Y\n\x03raw\x18\x03 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\\\n\x06\x65vents\x18\x04 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12[\n\x05reads\x18\x05 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12_\n\tmultiplex\x18\x06 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x64\n\x0e\x63hannel_states\x18\x07 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration\x12\x17\n\x0f\x64\x65vice_metadata\x18\x0b \x01(\x08\x12\x17\n\x0f\x64\x65vice_commands\x18\x0c \x01(\x08\x12\x1f\n\x17\x64ynamic_analysis_config\x18\x0f \x01(\x08\x1a\x99\x03\n\x13ReportConfiguration\x12\x1f\n\x17pdf_report_file_pattern\x18\x01 \x01(\t\x12 \n\x18json_report_file_pattern\x18\x02 \x01(\t\x12 \n\x18html_report_file_pattern\x18\t \x01(\t\x12$\n\x1cmarkdown_report_file_pattern\x18\x08 \x01(\t\x12%\n\x1d\x64uty_time_report_file_pattern\x18\x03 \x01(\t\x12&\n\x1ethroughput_report_file_pattern\x18\x04 \x01(\t\x12)\n!final_summary_report_file_pattern\x18\x05 \x01(\t\x12-\n%barcode_alignment_report_file_pattern\x18\x06 \x01(\t\x12(\n sample_sheet_report_file_pattern\x18\n \x01(\t\x12$\n\x1c\x63ustom_report_suffix_pattern\x18\x07 \x01(\t\"R\n\x0f\x43ompressionType\x12\x16\n\x12\x44\x65\x66\x61ultCompression\x10\x00\x12\x13\n\x0fZlibCompression\x10\x01\x12\x12\n\x0eVbzCompression\x10\x02\" \n\x1eSetWriterConfigurationResponse\"\x1f\n\x1dGetWriterConfigurationRequest\"\x1f\n\x1dGetReadClassificationsRequest\"\xd7\x01\n\x1eGetReadClassificationsResponse\x12y\n\x14read_classifications\x18\x01 \x03(\x0b\x32[.minknow_api.analysis_configuration.GetReadClassificationsResponse.ReadClassificationsEntry\x1a:\n\x18ReadClassificationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xfc\x02\n\x1c\x44ynamicAnalysisConfiguration\x12o\n\x13read_scale_tracking\x18\x01 \x01(\x0b\x32R.minknow_api.analysis_configuration.DynamicAnalysisConfiguration.ReadScaleTracking\x1a\xea\x01\n\x11ReadScaleTracking\x12 \n\x18\x63onductance_scan_voltage\x18\x01 \x01(\x02\x12\x82\x01\n\x13\x63hannel_conductance\x18\x02 \x03(\x0b\x32\x65.minknow_api.analysis_configuration.DynamicAnalysisConfiguration.ReadScaleTracking.ChannelConductance\x1a.\n\x12\x43hannelConductance\x12\x18\n\x10well_conductance\x18\x01 \x03(\x02\"(\n&GetDynamicAnalysisConfigurationRequest\")\n\'SetDynamicAnalysisConfigurationResponse2\xac\x15\n\x1c\x41nalysisConfigurationService\x12\xa1\x01\n\x1aget_analysis_configuration\x12\x43.minknow_api.analysis_configuration.GetAnalysisConfigurationRequest\x1a\x39.minknow_api.analysis_configuration.AnalysisConfiguration\"\x03\x90\x02\x01\x12\xa2\x01\n\x1aset_analysis_configuration\x12\x39.minknow_api.analysis_configuration.AnalysisConfiguration\x1a\x44.minknow_api.analysis_configuration.SetAnalysisConfigurationResponse\"\x03\x90\x02\x02\x12\xb2\x01\n\x1creset_analysis_configuration\x12\x45.minknow_api.analysis_configuration.ResetAnalysisConfigurationRequest\x1a\x46.minknow_api.analysis_configuration.ResetAnalysisConfigurationResponse\"\x03\x90\x02\x02\x12\xaa\x01\n\x1aset_analysis_enabled_state\x12\x42.minknow_api.analysis_configuration.SetAnalysisEnabledStateRequest\x1a\x43.minknow_api.analysis_configuration.SetAnalysisEnabledStateResponse\"\x03\x90\x02\x02\x12\xa1\x01\n\x17get_channel_states_desc\x12?.minknow_api.analysis_configuration.GetChannelStatesDescRequest\x1a@.minknow_api.analysis_configuration.GetChannelStatesDescResponse\"\x03\x90\x02\x01\x12\x81\x01\n\x0bget_summary\x12\x35.minknow_api.analysis_configuration.GetSummaryRequest\x1a\x36.minknow_api.analysis_configuration.GetSummaryResponse\"\x03\x90\x02\x01\x12\xb2\x01\n\x1cset_basecaller_configuration\x12\x45.minknow_api.analysis_configuration.SetBasecallerConfigurationRequest\x1a\x46.minknow_api.analysis_configuration.SetBasecallerConfigurationResponse\"\x03\x90\x02\x02\x12\xb6\x01\n preload_basecaller_configuration\x12\x45.minknow_api.analysis_configuration.SetBasecallerConfigurationRequest\x1a\x46.minknow_api.analysis_configuration.SetBasecallerConfigurationResponse\"\x03\x90\x02\x02\x12\xa7\x01\n\x1cget_basecaller_configuration\x12\x45.minknow_api.analysis_configuration.GetBasecallerConfigurationRequest\x1a;.minknow_api.analysis_configuration.BasecallerConfiguration\"\x03\x90\x02\x01\x12\xa2\x01\n\x1bget_pore_type_configuration\x12\x43.minknow_api.analysis_configuration.GetPoreTypeConfigurationRequest\x1a\x39.minknow_api.analysis_configuration.PoreTypeConfiguration\"\x03\x90\x02\x01\x12\xa3\x01\n\x1bset_pore_type_configuration\x12\x39.minknow_api.analysis_configuration.PoreTypeConfiguration\x1a\x44.minknow_api.analysis_configuration.SetPoreTypeConfigurationResponse\"\x03\x90\x02\x02\x12\x9c\x01\n\x18set_writer_configuration\x12\x37.minknow_api.analysis_configuration.WriterConfiguration\x1a\x42.minknow_api.analysis_configuration.SetWriterConfigurationResponse\"\x03\x90\x02\x02\x12\x9b\x01\n\x18get_writer_configuration\x12\x41.minknow_api.analysis_configuration.GetWriterConfigurationRequest\x1a\x37.minknow_api.analysis_configuration.WriterConfiguration\"\x03\x90\x02\x01\x12\xa6\x01\n\x18get_read_classifications\x12\x41.minknow_api.analysis_configuration.GetReadClassificationsRequest\x1a\x42.minknow_api.analysis_configuration.GetReadClassificationsResponse\"\x03\x90\x02\x01\x12\xb7\x01\n\"get_dynamic_analysis_configuration\x12J.minknow_api.analysis_configuration.GetDynamicAnalysisConfigurationRequest\x1a@.minknow_api.analysis_configuration.DynamicAnalysisConfiguration\"\x03\x90\x02\x01\x12\xb5\x01\n\"set_dynamic_analysis_configuration\x12@.minknow_api.analysis_configuration.DynamicAnalysisConfiguration\x1aK.minknow_api.analysis_configuration.SetDynamicAnalysisConfigurationResponse\"\x00\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-
-
-_EVENTDETECTION = DESCRIPTOR.message_types_by_name['EventDetection']
-_READDETECTIONPARAMS = DESCRIPTOR.message_types_by_name['ReadDetectionParams']
-_READFILTERS = DESCRIPTOR.message_types_by_name['ReadFilters']
-_READCLASSIFICATIONPARAMS = DESCRIPTOR.message_types_by_name['ReadClassificationParams']
-_READCLASSIFICATIONPARAMS_PARAMETERS = _READCLASSIFICATIONPARAMS.nested_types_by_name['Parameters']
-_CHANNELSTATES = DESCRIPTOR.message_types_by_name['ChannelStates']
-_CHANNELSTATES_LOGIC = _CHANNELSTATES.nested_types_by_name['Logic']
-_CHANNELSTATES_LOGIC_BEHAVIOUR = _CHANNELSTATES_LOGIC.nested_types_by_name['Behaviour']
-_CHANNELSTATES_LOGIC_RANGES = _CHANNELSTATES_LOGIC.nested_types_by_name['Ranges']
-_CHANNELSTATES_LOGIC_RANGES_RANGE = _CHANNELSTATES_LOGIC_RANGES.nested_types_by_name['Range']
-_CHANNELSTATES_STYLE = _CHANNELSTATES.nested_types_by_name['Style']
-_CHANNELSTATES_GROUP = _CHANNELSTATES.nested_types_by_name['Group']
-_GETANALYSISCONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['GetAnalysisConfigurationRequest']
-_READSCALINGPARAMS = DESCRIPTOR.message_types_by_name['ReadScalingParams']
-_ANALYSISCONFIGURATION = DESCRIPTOR.message_types_by_name['AnalysisConfiguration']
-_ANALYSISCONFIGURATION_CHANNELSTATESENTRY = _ANALYSISCONFIGURATION.nested_types_by_name['ChannelStatesEntry']
-_SETANALYSISCONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['SetAnalysisConfigurationResponse']
-_RESETANALYSISCONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['ResetAnalysisConfigurationRequest']
-_RESETANALYSISCONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['ResetAnalysisConfigurationResponse']
-_SETANALYSISENABLEDSTATEREQUEST = DESCRIPTOR.message_types_by_name['SetAnalysisEnabledStateRequest']
-_SETANALYSISENABLEDSTATERESPONSE = DESCRIPTOR.message_types_by_name['SetAnalysisEnabledStateResponse']
-_GETCHANNELSTATESDESCREQUEST = DESCRIPTOR.message_types_by_name['GetChannelStatesDescRequest']
-_GETCHANNELSTATESDESCRESPONSE = DESCRIPTOR.message_types_by_name['GetChannelStatesDescResponse']
-_GETCHANNELSTATESDESCRESPONSE_STYLE = _GETCHANNELSTATESDESCRESPONSE.nested_types_by_name['Style']
-_GETCHANNELSTATESDESCRESPONSE_CHANNELSTATE = _GETCHANNELSTATESDESCRESPONSE.nested_types_by_name['ChannelState']
-_GETCHANNELSTATESDESCRESPONSE_GROUP = _GETCHANNELSTATESDESCRESPONSE.nested_types_by_name['Group']
-_GETSUMMARYREQUEST = DESCRIPTOR.message_types_by_name['GetSummaryRequest']
-_GETSUMMARYRESPONSE = DESCRIPTOR.message_types_by_name['GetSummaryResponse']
-_BARCODINGCONFIGURATION = DESCRIPTOR.message_types_by_name['BarcodingConfiguration']
-_ALIGNMENTCONFIGURATION = DESCRIPTOR.message_types_by_name['AlignmentConfiguration']
-_LAMPCONFIGURATION = DESCRIPTOR.message_types_by_name['LampConfiguration']
-_BASECALLERCONFIGURATION = DESCRIPTOR.message_types_by_name['BasecallerConfiguration']
-_BASECALLERCONFIGURATION_READFILTERING = _BASECALLERCONFIGURATION.nested_types_by_name['ReadFiltering']
-_BASECALLERCONFIGURATION_TARGETFILTERING = _BASECALLERCONFIGURATION.nested_types_by_name['TargetFiltering']
-_SETBASECALLERCONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['SetBasecallerConfigurationRequest']
-_SETBASECALLERCONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['SetBasecallerConfigurationResponse']
-_GETBASECALLERCONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['GetBasecallerConfigurationRequest']
-_GETPORETYPECONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['GetPoreTypeConfigurationRequest']
-_PORETYPECONFIGURATION = DESCRIPTOR.message_types_by_name['PoreTypeConfiguration']
-_PORETYPECONFIGURATION_CHANNELWELL = _PORETYPECONFIGURATION.nested_types_by_name['ChannelWell']
-_PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS = _PORETYPECONFIGURATION.nested_types_by_name['ChannelWellPoreTypeConfigurations']
-_PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_CHANNELWELLLIST = _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS.nested_types_by_name['ChannelWellList']
-_PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_PORETYPESENTRY = _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS.nested_types_by_name['PoreTypesEntry']
-_SETPORETYPECONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['SetPoreTypeConfigurationResponse']
-_WRITERCONFIGURATION = DESCRIPTOR.message_types_by_name['WriterConfiguration']
-_WRITERCONFIGURATION_CHANNELCONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['ChannelConfiguration']
-_WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELLIST = _WRITERCONFIGURATION_CHANNELCONFIGURATION.nested_types_by_name['ChannelList']
-_WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES = _WRITERCONFIGURATION_CHANNELCONFIGURATION.nested_types_by_name['ChannelRanges']
-_WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES_CHANNELRANGE = _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES.nested_types_by_name['ChannelRange']
-_WRITERCONFIGURATION_READFAST5CONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['ReadFast5Configuration']
-_WRITERCONFIGURATION_READFASTQCONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['ReadFastqConfiguration']
-_WRITERCONFIGURATION_READBAMCONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['ReadBamConfiguration']
-_WRITERCONFIGURATION_READPOD5CONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['ReadPod5Configuration']
-_WRITERCONFIGURATION_READPROTOBUFCONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['ReadProtobufConfiguration']
-_WRITERCONFIGURATION_SEQUENCINGSUMMARYCONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['SequencingSummaryConfiguration']
-_WRITERCONFIGURATION_BULKCONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['BulkConfiguration']
-_WRITERCONFIGURATION_REPORTCONFIGURATION = _WRITERCONFIGURATION.nested_types_by_name['ReportConfiguration']
-_SETWRITERCONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['SetWriterConfigurationResponse']
-_GETWRITERCONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['GetWriterConfigurationRequest']
-_GETREADCLASSIFICATIONSREQUEST = DESCRIPTOR.message_types_by_name['GetReadClassificationsRequest']
-_GETREADCLASSIFICATIONSRESPONSE = DESCRIPTOR.message_types_by_name['GetReadClassificationsResponse']
-_GETREADCLASSIFICATIONSRESPONSE_READCLASSIFICATIONSENTRY = _GETREADCLASSIFICATIONSRESPONSE.nested_types_by_name['ReadClassificationsEntry']
-_DYNAMICANALYSISCONFIGURATION = DESCRIPTOR.message_types_by_name['DynamicAnalysisConfiguration']
-_DYNAMICANALYSISCONFIGURATION_READSCALETRACKING = _DYNAMICANALYSISCONFIGURATION.nested_types_by_name['ReadScaleTracking']
-_DYNAMICANALYSISCONFIGURATION_READSCALETRACKING_CHANNELCONDUCTANCE = _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING.nested_types_by_name['ChannelConductance']
-_GETDYNAMICANALYSISCONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['GetDynamicAnalysisConfigurationRequest']
-_SETDYNAMICANALYSISCONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['SetDynamicAnalysisConfigurationResponse']
-_READDETECTIONPARAMS_READDETECTIONMODE = _READDETECTIONPARAMS.enum_types_by_name['ReadDetectionMode']
-_READCLASSIFICATIONPARAMS_SCHEME = _READCLASSIFICATIONPARAMS.enum_types_by_name['Scheme']
-_WRITERCONFIGURATION_COMPRESSIONTYPE = _WRITERCONFIGURATION.enum_types_by_name['CompressionType']
-EventDetection = _reflection.GeneratedProtocolMessageType('EventDetection', (_message.Message,), {
-  'DESCRIPTOR' : _EVENTDETECTION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Attributes:
-      window_size:
-          The window size that the tstats are calculated from
-      threshold:
-          The peak detection must be above this threshold at a minimum
-          for it to be detected as an event.
-      peak_height:
-          When analysing the tstat peaks, if the jump between one value
-          and another is higher than than 'peak_height', then it will
-          "arm" the peak detector and move onto the next phase.  And
-          what goes up must come down. Once it has detected a peak going
-          up, it will also have to go down by 'peak_height' in order for
-          the peak to be classified as a found event
-      events_to_base_ratio:
-          Conversion factor used to convert from events to bases.  This
-          is used to estimate bases for various rpc feeds from minknow.
-      break_on_mux_changes:
-          Whether to break events on mux changes.  This will eliminate
-          "mux_uncertain" events and reads. Note that this will cause
-          starting or stopping unblocking to break events as well (even
-          though the mux does not normally change in this case).
-      max_mux_change_back_shift:
-          Control the number of samples MinKNOW will shift mux changes
-          back by in order to align mux changes with event boundaries.
-          When break on mux changes is enabled its possible that mux
-          changes recorded from the device and signal deltas caused by
-          the config changes will not align exactly (the signal delta
-          happen prior to the mux change due to the recorded sample
-          indicating the command is fully applied). Setting this value
-          to > 0 will allow minknow to record the mux change as active
-          up to this number of samples _before_ the device recorded the
-          change as active. Mux changes are never shifted forwards.  A
-          value of 0 will disable shifting of mux changes.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.EventDetection)
-  })
-_sym_db.RegisterMessage(EventDetection)
-
-ReadDetectionParams = _reflection.GeneratedProtocolMessageType('ReadDetectionParams', (_message.Message,), {
-  'DESCRIPTOR' : _READDETECTIONPARAMS,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Attributes:
-      open_pore_min:
-          The minimum level which is considered open pore (this value is
-          relative to open_pore_default or the tracked open_pore
-          section, if tracking is being used.)  This value must be <=
-          0.0 if tracking is being used.
-      open_pore_max:
-          The maximum level which is considered open pore (this value is
-          relative to open_pore_default or the tracked open_pore
-          section, if tracking is being used.)  This value must be >=
-          0.0 if tracking is being used.
-      open_pore_default:
-          The default value to use for open pore, either when tracking
-          isn't being used, or when open pore tracking has no value
-          currently.
-      open_pore_seconds_required:
-          Minimum number of seconds events must lie within the range of
-          open pore in order to allow a read to break.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ReadDetectionParams)
-  })
-_sym_db.RegisterMessage(ReadDetectionParams)
-
-ReadFilters = _reflection.GeneratedProtocolMessageType('ReadFilters', (_message.Message,), {
-  'DESCRIPTOR' : _READFILTERS,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Parameters for filtering out reads from being written.  The tests are
-  combined using a logical AND: if any given test fails, the read will
-  not be written. Only reads that pass all (non-zero) tests will be
-  written out.  Currently, it is only possible to filter on read length.
-  This can be given in samples or MinKNOW events.
-  
-  Attributes:
-      read_length_min:
-          Only write reads that contain at least this many samples.  The
-          default zero value will not exclude any reads.
-      read_length_max:
-          Only write reads that contain at most this many samples.  If
-          set to zero (the default), this test is not applied (as though
-          it had been set to a value longer than any possible read).
-      event_count_min:
-          Only write reads that contain at least this many MinKNOW
-          events.  The default zero value will not exclude any reads.
-      event_count_max:
-          Only write reads that contain at most this many MinKNOW
-          events.  If set to zero (the default), this test is not
-          applied (as though it had been set to a value longer than any
-          possible read).
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ReadFilters)
-  })
-_sym_db.RegisterMessage(ReadFilters)
-
-ReadClassificationParams = _reflection.GeneratedProtocolMessageType('ReadClassificationParams', (_message.Message,), {
-
-  'Parameters' : _reflection.GeneratedProtocolMessageType('Parameters', (_message.Message,), {
-    'DESCRIPTOR' : _READCLASSIFICATIONPARAMS_PARAMETERS,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        rules_in_execution_order:
-            An execution rule has the following format:  "pore =
-            (median,gt,185)&(median,lt,260)&(median_sd,lt,40)"  "median"
-            and "median_sd" are apart of a small subset of variable values
-            describing a read or read chunk, that are exposed to execution
-            rules. The full list of variable values and their descriptions
-            are documented here:
-            https://minknow.git.oxfordnanolabs.local/minknow-
-            core/analysis/reads.html  "gt" and "lt" describe how data can
-            be compared: gt: greater than lt: less than eq: equal ne: not
-            equal  Constant values like "185" or "260" can also be
-            specified. These can be real numbers also.  Note that
-            variables dont always have to be on the left and const values
-            on the right. The following sub rules are also valid:
-            (200,lt,median_sd) (median_before,gt,median) (5,lt,10)
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ReadClassificationParams.Parameters)
-    })
-  ,
-  'DESCRIPTOR' : _READCLASSIFICATIONPARAMS,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Attributes:
-      max_sample_size:
-          This tells minknow the maximum number of means to store in
-          memory before using a different strategy to calculate medians.
-          If the number of means goes over this size then the strategy
-          used may be less accurate, but will not use as much memory in
-          minknow
-      selected_classifications:
-          A list of classifications that are deemed interesting, and
-          will be marked to be written out to file
-      open_pore_classifications:
-          A set of classifications whose level should be tracked as the
-          level of open pore (fed back into read detection analysis).
-          Read chunks selected by this filter will be aggregated for use
-          in read detection.
-      open_pore_ewma_weight:
-          A weighting figure for the exponentially weighted moving
-          average given to the newest data. eg. 0.7 would weight new
-          data with 0.3 and all previous data with 0.7.  By default 0.5
-          is used.
-      open_pore_ignore_after_reset_seconds:
-          A number of seconds to ignore new chunks for after a reset
-          occurs on a channel this allows analysis to ignore spikes or
-          bad data on the channel for a small section of time.  By
-          default 0.0 is used - and chunks are accepted immediately.
-      classification_strategy:
-          Determine how to classify a whole read based on the strategy
-          'ultimate':      Chooses the last (ultimate) read chunk's
-          classification 'penultimate':   Chooses the second-to-last
-          read chunk's clasification 'modal':         Chooses the most
-          common classification out of the all read chunks
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ReadClassificationParams)
-  })
-_sym_db.RegisterMessage(ReadClassificationParams)
-_sym_db.RegisterMessage(ReadClassificationParams.Parameters)
-
-ChannelStates = _reflection.GeneratedProtocolMessageType('ChannelStates', (_message.Message,), {
-
-  'Logic' : _reflection.GeneratedProtocolMessageType('Logic', (_message.Message,), {
-
-    'Behaviour' : _reflection.GeneratedProtocolMessageType('Behaviour', (_message.Message,), {
-      'DESCRIPTOR' : _CHANNELSTATES_LOGIC_BEHAVIOUR,
-      '__module__' : 'minknow_api.analysis_configuration_pb2'
-      ,
-      '__doc__': """Attributes:
-          reset_on_mux_change:
-              TODO: MinKNOW 5: replace int32 with bool for these options
-              these are ints but act like bools
-          latch:
-              If the latch value is set to true, then when the criteria for
-              this channel state is active, then the latch will keep it
-              active until the channel state is reset.
-          reset_on_effective_mux_change:
-              An 'effective mux change' is any mux change apart from the one
-              triggered with the purpose of disconnecting a channel (turning
-              a channel off). For example, if a channel is in pore, and the
-              user changes the channel configuration to 'disconnected', that
-              mux change will not be an effective mux change. Any other mux
-              change is considered an 'effective mux change'. So if a
-              channel saturates, the mux change to disconnected is an
-              effective mux change. Similarly, a change from disconnected to
-              a pore is an effective mux change.  Use this reset mode to
-              make the channel state persist on non-effective mux changes.
-              For example, if a channel state is in 'multiple' and the user
-              triggers a channel configuration change to 'disconnected', the
-              state will remain in multiple if it has this option on. The
-              multiple state will be reset at all other mux changes (i.e.
-              effective mux changes).
-          reset_on_effective_well_change:
-              An 'effective well change' is any well change apart from the
-              one triggered with the purpose of disconnecting a channel
-              (turning a channel off). For example, if a channel is in
-              well_1, and the user changes the channel configuration to
-              'unblock_1', that change will not be an effective well change.
-              A change to disconnected is also not considered an effective
-              well change.  Use this reset mode to make the channel state
-              persist on non-effective well changes. For example, if a
-              channel state is in 'multiple' and the user triggers a channel
-              configuration change to 'disconnected', the state will remain
-              in multiple if it has this option on. The multiple state will
-              be reset then when the mux is set to a different setting.
-      """,
-      # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ChannelStates.Logic.Behaviour)
-      })
-    ,
-
-    'Ranges' : _reflection.GeneratedProtocolMessageType('Ranges', (_message.Message,), {
-
-      'Range' : _reflection.GeneratedProtocolMessageType('Range', (_message.Message,), {
-        'DESCRIPTOR' : _CHANNELSTATES_LOGIC_RANGES_RANGE,
-        '__module__' : 'minknow_api.analysis_configuration_pb2'
-        # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ChannelStates.Logic.Ranges.Range)
-        })
-      ,
-      'DESCRIPTOR' : _CHANNELSTATES_LOGIC_RANGES,
-      '__module__' : 'minknow_api.analysis_configuration_pb2'
-      ,
-      '__doc__': """Dont really like this way of doing it, but it has to match the old
-      way...""",
-      # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ChannelStates.Logic.Ranges)
-      })
-    ,
-    'DESCRIPTOR' : _CHANNELSTATES_LOGIC,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        rank:
-            Specifies the order in which channel state criteria will be
-            evaluated; the smaller the number, the earlier it will be
-            evaluated. The first criteria to match will be selected
-        pattern:
-            Note that this is a regex based pattern for describing a read
-            classification sequence. For example you can specify:
-            "unavailableunavailable" or:      "(unavailable)(unavailable)"
-            to recognise two consecutive read chunks classified as
-            unavailable.  You can also use "?" at the end of one of the
-            classifications in the sequence to indicate that it may or may
-            not be present at that point. For example:
-            "(pore)(transition)?(event)"  This will match both of the
-            sequences:      pore, transition, event      pore, event  The
-            technical documentation has more information on the range of
-            regex patterns you can apply.
-            https://minknow.git.oxfordnanolabs.local/minknow-
-            core/analysis/channel-states.html
-        ranges:
-            Range is [lower_pa, upper_pa)
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ChannelStates.Logic)
-    })
-  ,
-
-  'Style' : _reflection.GeneratedProtocolMessageType('Style', (_message.Message,), {
-    'DESCRIPTOR' : _CHANNELSTATES_STYLE,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ChannelStates.Style)
-    })
-  ,
-
-  'Group' : _reflection.GeneratedProtocolMessageType('Group', (_message.Message,), {
-    'DESCRIPTOR' : _CHANNELSTATES_GROUP,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ChannelStates.Group)
-    })
-  ,
-  'DESCRIPTOR' : _CHANNELSTATES,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ChannelStates)
-  })
-_sym_db.RegisterMessage(ChannelStates)
-_sym_db.RegisterMessage(ChannelStates.Logic)
-_sym_db.RegisterMessage(ChannelStates.Logic.Behaviour)
-_sym_db.RegisterMessage(ChannelStates.Logic.Ranges)
-_sym_db.RegisterMessage(ChannelStates.Logic.Ranges.Range)
-_sym_db.RegisterMessage(ChannelStates.Style)
-_sym_db.RegisterMessage(ChannelStates.Group)
-
-GetAnalysisConfigurationRequest = _reflection.GeneratedProtocolMessageType('GetAnalysisConfigurationRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETANALYSISCONFIGURATIONREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetAnalysisConfigurationRequest)
-  })
-_sym_db.RegisterMessage(GetAnalysisConfigurationRequest)
-
-ReadScalingParams = _reflection.GeneratedProtocolMessageType('ReadScalingParams', (_message.Message,), {
-  'DESCRIPTOR' : _READSCALINGPARAMS,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Since 5.3  Quantile Information:
-  
-  Attributes:
-      quantile_locations:
-          Position of quantiles in scaling data to use when computing
-          scale parameters.
-      quantile_weights_shift:
-          If present, must be the same length as quantile_locations.
-          Represents the coefficients that shall be multiplied with
-          measured quantiles to give a predicted_shift
-      quantile_weights_scale:
-          If present, must be the same length as quantile_locations.
-          Represents the coefficients that shall be multiplied with
-          measured quantiles to give a predicted_scale
-      tracking_alpha:
-          Alpha value to use in ewma calculation for scale and shift
-          tracking. 1 updates instantly. 0 does not update.
-      alpha_number_estimates_decay:
-          Alpha decay value to use. Higher values cause a more rapid
-          decay in greater trust of earlier numbers.
-      quantile_maxdiff:
-          Maximum difference in event quantiles which will be added into
-          trackers.  This is used to filter away cases where pore signal
-          is included in the read and thus cannot be trusted.
-      trust_limit_fraction:
-          Maximum fraction change between one tracked value and the next
-          which will be trusted. Higher values are not trusted.
-      diff_threshold:
-          The minimum difference between an event and the next to
-          include it in the subsampling
-      emission_threshold:
-          After how many cumulative pA is a new event emitted in the
-          subsampling
-      dacs_breakpoint:
-          Cumulative pA sum required to compute scaling. Any events
-          after this sum are not considered in scaling.
-      conductance_factor_scale:
-          Scale factor applied to conductance to produce a basic scale
-          estimate, also combined with q90_q10_to_normal.
-      conductance_factor_shift:
-          Scale factor applied to conductance to produce a basic shift
-          estimate.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ReadScalingParams)
-  })
-_sym_db.RegisterMessage(ReadScalingParams)
-
-AnalysisConfiguration = _reflection.GeneratedProtocolMessageType('AnalysisConfiguration', (_message.Message,), {
-
-  'ChannelStatesEntry' : _reflection.GeneratedProtocolMessageType('ChannelStatesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _ANALYSISCONFIGURATION_CHANNELSTATESENTRY,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.AnalysisConfiguration.ChannelStatesEntry)
-    })
-  ,
-  'DESCRIPTOR' : _ANALYSISCONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Attributes:
-      read_scaling:
-          Add read scale tracking to the pipeline. If this message is
-          unspecified, read scaling is not enabled.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.AnalysisConfiguration)
-  })
-_sym_db.RegisterMessage(AnalysisConfiguration)
-_sym_db.RegisterMessage(AnalysisConfiguration.ChannelStatesEntry)
-
-SetAnalysisConfigurationResponse = _reflection.GeneratedProtocolMessageType('SetAnalysisConfigurationResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETANALYSISCONFIGURATIONRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetAnalysisConfigurationResponse)
-  })
-_sym_db.RegisterMessage(SetAnalysisConfigurationResponse)
-
-ResetAnalysisConfigurationRequest = _reflection.GeneratedProtocolMessageType('ResetAnalysisConfigurationRequest', (_message.Message,), {
-  'DESCRIPTOR' : _RESETANALYSISCONFIGURATIONREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ResetAnalysisConfigurationRequest)
-  })
-_sym_db.RegisterMessage(ResetAnalysisConfigurationRequest)
-
-ResetAnalysisConfigurationResponse = _reflection.GeneratedProtocolMessageType('ResetAnalysisConfigurationResponse', (_message.Message,), {
-  'DESCRIPTOR' : _RESETANALYSISCONFIGURATIONRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.ResetAnalysisConfigurationResponse)
-  })
-_sym_db.RegisterMessage(ResetAnalysisConfigurationResponse)
-
-SetAnalysisEnabledStateRequest = _reflection.GeneratedProtocolMessageType('SetAnalysisEnabledStateRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETANALYSISENABLEDSTATEREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetAnalysisEnabledStateRequest)
-  })
-_sym_db.RegisterMessage(SetAnalysisEnabledStateRequest)
-
-SetAnalysisEnabledStateResponse = _reflection.GeneratedProtocolMessageType('SetAnalysisEnabledStateResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETANALYSISENABLEDSTATERESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetAnalysisEnabledStateResponse)
-  })
-_sym_db.RegisterMessage(SetAnalysisEnabledStateResponse)
-
-GetChannelStatesDescRequest = _reflection.GeneratedProtocolMessageType('GetChannelStatesDescRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCHANNELSTATESDESCREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetChannelStatesDescRequest)
-  })
-_sym_db.RegisterMessage(GetChannelStatesDescRequest)
-
-GetChannelStatesDescResponse = _reflection.GeneratedProtocolMessageType('GetChannelStatesDescResponse', (_message.Message,), {
-
-  'Style' : _reflection.GeneratedProtocolMessageType('Style', (_message.Message,), {
-    'DESCRIPTOR' : _GETCHANNELSTATESDESCRESPONSE_STYLE,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        label:
-            The human-readable name to display when rendering this channel
-            state or group.
-        description:
-            A sentence describing the meaning of the channel state or
-            group.  This can be used as a tooltip, for example.
-        colour:
-            The colour to use when rendering this channel state or group.
-            This is a six-digit hex string describing an RGB colour (eg:
-            "ff00ff" for purple).
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetChannelStatesDescResponse.Style)
-    })
-  ,
-
-  'ChannelState' : _reflection.GeneratedProtocolMessageType('ChannelState', (_message.Message,), {
-    'DESCRIPTOR' : _GETCHANNELSTATESDESCRESPONSE_CHANNELSTATE,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        id:
-            The numeric identifier of the state.  This is what is reported
-            in any other APIs that return a channel state ID.
-        name:
-            The internal name of the state.  This is what is reported in
-            any other APIs that return a channel state name.
-        style:
-            How to render the channel state in a graphical user interface.
-            Note that the style may be missing from some channel states
-            (such as the ones that are built in to MinKNOW).
-        global_order:
-            An order ranking for the channel states when they are
-            ungrouped.  This can be used to order the channel states after
-            merging the groups.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetChannelStatesDescResponse.ChannelState)
-    })
-  ,
-
-  'Group' : _reflection.GeneratedProtocolMessageType('Group', (_message.Message,), {
-    'DESCRIPTOR' : _GETCHANNELSTATESDESCRESPONSE_GROUP,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        name:
-            The name of the group.
-        style:
-            How to render the group in a graphical user interface.  Note
-            that the style may be missing from some groups (such as the
-            ones that are built in to MinKNOW).
-        states:
-            The channel states contained in the group.  The groups are
-            ordered according to the "order" attribute of the channel
-            state style in the channel states configuration.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetChannelStatesDescResponse.Group)
-    })
-  ,
-  'DESCRIPTOR' : _GETCHANNELSTATESDESCRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Attributes:
-      groups:
-          The groups of channel states.  The groups are ordered
-          according to the "order" attribute of the group style in the
-          channel states configuration.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetChannelStatesDescResponse)
-  })
-_sym_db.RegisterMessage(GetChannelStatesDescResponse)
-_sym_db.RegisterMessage(GetChannelStatesDescResponse.Style)
-_sym_db.RegisterMessage(GetChannelStatesDescResponse.ChannelState)
-_sym_db.RegisterMessage(GetChannelStatesDescResponse.Group)
-
-GetSummaryRequest = _reflection.GeneratedProtocolMessageType('GetSummaryRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETSUMMARYREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetSummaryRequest)
-  })
-_sym_db.RegisterMessage(GetSummaryRequest)
-
-GetSummaryResponse = _reflection.GeneratedProtocolMessageType('GetSummaryResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETSUMMARYRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Attributes:
-      analysis_enabled:
-          Whether any analysis is enabled.  If this is false, everything
-          else will be false as well.
-      basecalling_enabled:
-          Whether basecalling is enabled.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetSummaryResponse)
-  })
-_sym_db.RegisterMessage(GetSummaryResponse)
-
-BarcodingConfiguration = _reflection.GeneratedProtocolMessageType('BarcodingConfiguration', (_message.Message,), {
-  'DESCRIPTOR' : _BARCODINGCONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Since 3.5
-  
-  Attributes:
-      barcoding_kits:
-          The barcoding kits in use One entry per kit If no barcoding
-          kits are supplied, barcoding is disabled.
-      trim_barcodes:
-          Whether Guppy should trim barcodes If not specified, this
-          value defaults to false (not triming barcodes) If barcoding is
-          not enabled (e.g., because no barcoding kits are specified),
-          this parameter has no effect.
-      require_barcodes_both_ends:
-          Barcode is only classified if a barcode above `min_score` is
-          present at both ends of the basecalled read.
-      detect_mid_strand_barcodes:
-          Search for barcodes through the entire length of the read.  If
-          a barcode is found in the middle of a read the read is marked
-          as unclassified.
-      min_score:
-          Minimum alignment score to consider a valid barcode.  Maximum
-          value is 100, defaults to 60.
-      min_score_rear:
-          Minimum score to consider a valid barcode (overrides min_score
-          for rear barcodes).  Maximum value is 100, defaults to
-          min_score if not specified.
-      min_score_mid:
-          Minimum score to consider a valid mid barcode (only valid if
-          detect_mid_strand_barcodes is specified).  Maximum value is
-          100, defaults to 60.
-      min_score_mask:
-          The minimum score required for the barcode mask to be
-          detected.  Maximum value is 100, defaults to 40.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.BarcodingConfiguration)
-  })
-_sym_db.RegisterMessage(BarcodingConfiguration)
-
-AlignmentConfiguration = _reflection.GeneratedProtocolMessageType('AlignmentConfiguration', (_message.Message,), {
-  'DESCRIPTOR' : _ALIGNMENTCONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Since 4.0
-  
-  Attributes:
-      reference_files:
-          Provide an index to align reads against once basecalled.  Any
-          acceptable reference format to guppy can be passed here:   -
-          fasta reference file   - minimap index file
-      bed_file:
-          Provide a bed file for use indicating areas of interest in
-          alignment results.  Note: alignment_index must be provided for
-          this argument to be valid.
-      minimum_coverage:
-          Minimum coverage for guppy to accept an alignment.  If not
-          specified a default value is used.  Note: this option cannot
-          be used during live basecalling.
-      aggregate_statistics_for_multiple_bed_hits:
-          Control how statistics for bed results are aggregated.  If set
-          to false only the bed hit with the highest overlap is used
-          when computing heatmap/throughput graphs with bed hits.  If
-          set to true each bed hit is considered and bases for all hits
-          are counted. This may give more honest representation of
-          individual bed hit results but will skew read count statistics
-          - as each hit will be counted for every bed hit.  Note: this
-          option has no effect in offline basecalling.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.AlignmentConfiguration)
-  })
-_sym_db.RegisterMessage(AlignmentConfiguration)
-
-LampConfiguration = _reflection.GeneratedProtocolMessageType('LampConfiguration', (_message.Message,), {
-  'DESCRIPTOR' : _LAMPCONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Since 4.1
-  
-  Attributes:
-      lamp_kit:
-          Set the lamp kit being used.
-      min_score_barcodes:
-          Optionally specify a min score to detect a valid lamp barcode.
-      min_score_masks:
-          Optionally set the minimimum valid score for a lamp mask.
-      min_score_targets:
-          Optionally specify a minimum score for lamp targets.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.LampConfiguration)
-  })
-_sym_db.RegisterMessage(LampConfiguration)
-
-BasecallerConfiguration = _reflection.GeneratedProtocolMessageType('BasecallerConfiguration', (_message.Message,), {
-
-  'ReadFiltering' : _reflection.GeneratedProtocolMessageType('ReadFiltering', (_message.Message,), {
-    'DESCRIPTOR' : _BASECALLERCONFIGURATION_READFILTERING,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.BasecallerConfiguration.ReadFiltering)
-    })
-  ,
-
-  'TargetFiltering' : _reflection.GeneratedProtocolMessageType('TargetFiltering', (_message.Message,), {
-    'DESCRIPTOR' : _BASECALLERCONFIGURATION_TARGETFILTERING,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Since 3.7""",
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.BasecallerConfiguration.TargetFiltering)
-    })
-  ,
-  'DESCRIPTOR' : _BASECALLERCONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Since 3.0
-  
-  Attributes:
-      enable:
-          Choose if guppy is enabled or disabled.  If set to false then
-          no basecalling will take place, and the rest of the config is
-          ignored.
-      config_filename:
-          The Guppy cfg file with all the settings.  Filename can be
-          absolute, or a basename (eg dna_r9.4_450bps.cfg) which guppy
-          should locate (see guppy application config entry:
-          "data_path")
-      align_filter:
-          Enable or disable pass/fail filtering based on alignment.
-          When enabled, reads which do not align to any references will
-          be marked as "failed", and written to the folder specified in
-          MinKNOW configuration for failed reads.    The setting applies
-          to both regular read filtering and target filtering; if it is
-          enabled, then a read will not be marked as a target read if it
-          does not align to a reference.  Default setting is false, i.e.
-          disabled.  Since 5.4
-      read_filtering:
-          Control how read filtering is applied to output of basecaller.
-          These settings determine whether a read is marked as "passed"
-          or "failed".  Reads are written to different folders based on
-          the result of this filtering.  Those folders are specified in
-          MinKNOW configuration.  If no filtering parameters are
-          provided then reads will not be filtered.
-      barcoding_configuration:
-          Control the barcoding configuration. If no barcoding
-          configuration is supplied, barcoding is disabled.  Since 3.5
-      target_filtering:
-          Control how target filtering is applied to output of
-          basecaller. Reads which pass these filtering criteria will be
-          marked as "target" reads, and will be written to a separate
-          folder; this  folder is specified in MinKNOW configuration.
-          Reads which do  not pass these criteria will have the regular
-          read filtering applied to them, as specified by the `read-
-          filtering` settings above.  If no filtering parameters are
-          provided then reads will not be target-filtered.  Since 3.7
-      alignment_configuration:
-          Alignment configuration parameters. If no configuration is
-          specified alignment is disabled.  Since 4.0
-      lamp_configuration:
-          Lamp configuration parameters. If no configuration is
-          specified lamp is disabled.  Since 4.1
-      enable_read_splitting:
-          Enable read splitting in guppy.  Since 4.5
-      min_score_read_splitting:
-          Override score to use for guppy read splitting. If not
-          specified a default value is used from guppy.  Since 4.5
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.BasecallerConfiguration)
-  })
-_sym_db.RegisterMessage(BasecallerConfiguration)
-_sym_db.RegisterMessage(BasecallerConfiguration.ReadFiltering)
-_sym_db.RegisterMessage(BasecallerConfiguration.TargetFiltering)
-
-SetBasecallerConfigurationRequest = _reflection.GeneratedProtocolMessageType('SetBasecallerConfigurationRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETBASECALLERCONFIGURATIONREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetBasecallerConfigurationRequest)
-  })
-_sym_db.RegisterMessage(SetBasecallerConfigurationRequest)
-
-SetBasecallerConfigurationResponse = _reflection.GeneratedProtocolMessageType('SetBasecallerConfigurationResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETBASECALLERCONFIGURATIONRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetBasecallerConfigurationResponse)
-  })
-_sym_db.RegisterMessage(SetBasecallerConfigurationResponse)
-
-GetBasecallerConfigurationRequest = _reflection.GeneratedProtocolMessageType('GetBasecallerConfigurationRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETBASECALLERCONFIGURATIONREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetBasecallerConfigurationRequest)
-  })
-_sym_db.RegisterMessage(GetBasecallerConfigurationRequest)
-
-GetPoreTypeConfigurationRequest = _reflection.GeneratedProtocolMessageType('GetPoreTypeConfigurationRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETPORETYPECONFIGURATIONREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetPoreTypeConfigurationRequest)
-  })
-_sym_db.RegisterMessage(GetPoreTypeConfigurationRequest)
-
-PoreTypeConfiguration = _reflection.GeneratedProtocolMessageType('PoreTypeConfiguration', (_message.Message,), {
-
-  'ChannelWell' : _reflection.GeneratedProtocolMessageType('ChannelWell', (_message.Message,), {
-    'DESCRIPTOR' : _PORETYPECONFIGURATION_CHANNELWELL,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        channel:
-            Channel number to control pore type for.  Must be less than
-            channel count for the current platform
-        well:
-            Well to control pore type for.  Wells outside the available
-            wells on the flowcell are ignored.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWell)
-    })
-  ,
-
-  'ChannelWellPoreTypeConfigurations' : _reflection.GeneratedProtocolMessageType('ChannelWellPoreTypeConfigurations', (_message.Message,), {
-
-    'ChannelWellList' : _reflection.GeneratedProtocolMessageType('ChannelWellList', (_message.Message,), {
-      'DESCRIPTOR' : _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_CHANNELWELLLIST,
-      '__module__' : 'minknow_api.analysis_configuration_pb2'
-      # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.ChannelWellList)
-      })
-    ,
-
-    'PoreTypesEntry' : _reflection.GeneratedProtocolMessageType('PoreTypesEntry', (_message.Message,), {
-      'DESCRIPTOR' : _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_PORETYPESENTRY,
-      '__module__' : 'minknow_api.analysis_configuration_pb2'
-      # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.PoreTypesEntry)
-      })
-    ,
-    'DESCRIPTOR' : _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        pore_types:
-            Map with pore type as key, mapped to the list of wells to set
-            for.  It is undefined what will happen if one call sets the
-            pore type of a channel and well to two pore types.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.PoreTypeConfiguration.ChannelWellPoreTypeConfigurations)
-    })
-  ,
-  'DESCRIPTOR' : _PORETYPECONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """The pore type configuration  The ways of specifying a configuration
-  are as follows: - global_pore_type: all wells have a pore type of
-  global_pore_type. - channel_well_pore_types: channels are allowed
-  different values per channel/well   (allows a subset of channels to be
-  set).
-  
-  Attributes:
-      global_pore_type:
-          Set all channel/wells to one pore type.
-      channel_well_pore_types:
-          Set channel/wells to different pore types.  Pore types can be
-          created without being used by adding an empty entry.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.PoreTypeConfiguration)
-  })
-_sym_db.RegisterMessage(PoreTypeConfiguration)
-_sym_db.RegisterMessage(PoreTypeConfiguration.ChannelWell)
-_sym_db.RegisterMessage(PoreTypeConfiguration.ChannelWellPoreTypeConfigurations)
-_sym_db.RegisterMessage(PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.ChannelWellList)
-_sym_db.RegisterMessage(PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.PoreTypesEntry)
-
-SetPoreTypeConfigurationResponse = _reflection.GeneratedProtocolMessageType('SetPoreTypeConfigurationResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETPORETYPECONFIGURATIONRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetPoreTypeConfigurationResponse)
-  })
-_sym_db.RegisterMessage(SetPoreTypeConfigurationResponse)
-
-WriterConfiguration = _reflection.GeneratedProtocolMessageType('WriterConfiguration', (_message.Message,), {
-
-  'ChannelConfiguration' : _reflection.GeneratedProtocolMessageType('ChannelConfiguration', (_message.Message,), {
-
-    'ChannelList' : _reflection.GeneratedProtocolMessageType('ChannelList', (_message.Message,), {
-      'DESCRIPTOR' : _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELLIST,
-      '__module__' : 'minknow_api.analysis_configuration_pb2'
-      ,
-      '__doc__': """Attributes:
-          channels:
-              List of channel names (one based) which should be enabled for
-              writing.
-      """,
-      # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelList)
-      })
-    ,
-
-    'ChannelRanges' : _reflection.GeneratedProtocolMessageType('ChannelRanges', (_message.Message,), {
-
-      'ChannelRange' : _reflection.GeneratedProtocolMessageType('ChannelRange', (_message.Message,), {
-        'DESCRIPTOR' : _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES_CHANNELRANGE,
-        '__module__' : 'minknow_api.analysis_configuration_pb2'
-        # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelRanges.ChannelRange)
-        })
-      ,
-      'DESCRIPTOR' : _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES,
-      '__module__' : 'minknow_api.analysis_configuration_pb2'
-      ,
-      '__doc__': """Attributes:
-          ranges:
-              List of start/end paired channel numbers which should be
-              enabled for writing.  All channels in inclusive ranges should
-              be enabled.
-      """,
-      # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration.ChannelRanges)
-      })
-    ,
-    'DESCRIPTOR' : _WRITERCONFIGURATION_CHANNELCONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Used to control which channels for a specific data type emit data
-    
-    Attributes:
-        channels:
-            Control the way channels are enabled for this data type.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ChannelConfiguration)
-    })
-  ,
-
-  'ReadFast5Configuration' : _reflection.GeneratedProtocolMessageType('ReadFast5Configuration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_READFAST5CONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        compression_level:
-            Control the level of compression applied to read data.  0:
-            No compression will be applied to data. 1-9: Passed to zlib
-            compression, 1 is the fastest      compression, 9 is the
-            smallest possible output.
-        compression_type:
-            Control the type of compression applied to the read data.  By
-            default the vbz compressor is used (except in the single read
-            case).
-        raw:
-            Raw data, stored with calibration data, and read attributes.
-            Stored under /Raw/Reads_*/Signal
-        fastq:
-            Fastq data, stored as a string.  Stored under
-            /Analyses/Basecall_1D_*/BaseCalled_(template|complement)/Fastq
-        trace_table:
-            Trace table received from Guppy  Stored under
-            /Analyses/Basecall_1D_*/BaseCalled_template/Trace
-        move_table:
-            Move table received from Guppy  Stored under
-            /Analyses/Basecall_1D_*/BaseCalled_template/Move
-        modifications_table:
-            Base modification probability table  Store under
-            /Analyses/Basecall_1D_*/BaseCalled_template/ModBaseProbs
-        disable_writing_passed_reads:
-            Prevent reads which have successfully basecalled being written
-            to fast5.
-        disable_writing_failed_reads:
-            Prevent reads which have failed basecalling being written to
-            fast5.
-        disable_writing_force_skipped_reads:
-            disable writing reads which have been force skipped by the
-            basecaller.
-        file_pattern:
-            The pattern used to find a fast5 files name.  default: fast5{b
-            asecall_status}/{flow_cell_id}_{run_id}_{batch_number}.fast5
-            Where each {xxx} section is replaced with an attribute from
-            the minknow state when the file is written.  See file pattern
-            attributes above.
-        fastq_header_pattern:
-            The pattern used to find a fastq header.  default: {read_id}
-            runid={run_id} read={read_number} ch={channel_name}
-            start_time={read_start_time} Where each {xxx} section is
-            replaced with an attribute from the minknow state when the
-            fastq is generated.
-        batch_count:
-            How many reads are placed in each file (after batch_count
-            files {batch_number} is increased in the filename).
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ReadFast5Configuration)
-    })
-  ,
-
-  'ReadFastqConfiguration' : _reflection.GeneratedProtocolMessageType('ReadFastqConfiguration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_READFASTQCONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        enable:
-            Control if a fastq file should be generated per channel.
-        file_pattern:
-            The pattern used to find a fastq files name.  default: fastq{b
-            asecall_status}/{flow_cell_id}_{run_id}_{batch_number}.fastq
-            Where each {xxx} section is replaced with an attribute from
-            the minknow state when the file is written.  See file pattern
-            attributes above.
-        header_pattern:
-            The pattern used to find a fastq header.  default: {read_id}
-            runid={run_id} read={read_number} ch={channel_name}
-            start_time={read_start_time} Where each {xxx} section is
-            replaced with an attribute from the minknow state when the
-            fastq is generated.
-        batch_count:
-            How many files are placed in each batch (after batch_count
-            files {batch_number} is increased in the filename).
-        compression:
-            Compress fastq files with gzip compression. default: false
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ReadFastqConfiguration)
-    })
-  ,
-
-  'ReadBamConfiguration' : _reflection.GeneratedProtocolMessageType('ReadBamConfiguration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_READBAMCONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        enable:
-            Control if a BAM file should be generated per channel.
-        file_pattern:
-            The pattern used to find a BAM files name.  default: bam{basec
-            all_status}/{flow_cell_id}_{run_id}_{batch_number}.bam Where
-            each {xxx} section is replaced with an attribute from the
-            minknow state when the file is written.  See file pattern
-            attributes above.
-        batch_count:
-            How many files are placed in each batch (after batch_count
-            files {batch_number} is increased in the filename).
-        disable_writing_multiple_alignments:
-            If true minknow will only write the primary alignment for each
-            read.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ReadBamConfiguration)
-    })
-  ,
-
-  'ReadPod5Configuration' : _reflection.GeneratedProtocolMessageType('ReadPod5Configuration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_READPOD5CONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        enable:
-            Control if a POD5 file should be generated per channel.
-        file_pattern:
-            The pattern used to find a POD5 files name.  default: pod5{bas
-            ecall_status}/{flow_cell_id}_{run_id}_{batch_number}.pod5
-            Where each {xxx} section is replaced with an attribute from
-            the minknow state when the file is written.  See file pattern
-            attributes above.
-        batch_count:
-            How many files are placed in each batch (after batch_count
-            files {batch_number} is increased in the filename).  Set to
-            zero to disable batching.
-        disable_writing_passed_reads:
-            Prevent reads which have successfully basecalled being written
-            to pod5.
-        disable_writing_failed_reads:
-            Prevent reads which have failed basecalling being written to
-            pod5.
-        disable_writing_force_skipped_reads:
-            disable writing reads which have been force skipped by the
-            basecaller.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ReadPod5Configuration)
-    })
-  ,
-
-  'ReadProtobufConfiguration' : _reflection.GeneratedProtocolMessageType('ReadProtobufConfiguration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_READPROTOBUFCONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        enable:
-            Control if a protobuf file should be generated per channel.
-        file_pattern:
-            The pattern used to find a protobuf files name.  default: pbre
-            ad{basecall_status}/{batch_number}/{flow_cell_id}_{run_id}_ch_
-            {channel_name}_read_{read_number}.pbread Where each {xxx}
-            section is replaced with an attribute from the minknow state
-            when the file is written.  See file pattern attributes above.
-        batch_count:
-            How many files are placed in each batch (after batch_count
-            files {batch_number} is increased in the filename).
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ReadProtobufConfiguration)
-    })
-  ,
-
-  'SequencingSummaryConfiguration' : _reflection.GeneratedProtocolMessageType('SequencingSummaryConfiguration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_SEQUENCINGSUMMARYCONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        enable:
-            Should a sequencing summary file be generated
-        file_pattern:
-            The pattern used to find a summary files name.  default:
-            sequencing_summary_{flow_cell_id}_{short_run_id}.txt Where
-            each {xxx} section is replaced with an attribute from the
-            minknow state when the file is written.  See file pattern
-            attributes above.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.SequencingSummaryConfiguration)
-    })
-  ,
-
-  'BulkConfiguration' : _reflection.GeneratedProtocolMessageType('BulkConfiguration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_BULKCONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Control settings for the bulk writer
-    
-    Attributes:
-        compression_level:
-            Control the level of compression applied to read data.  0:
-            No compression will be applied to data. 1-9: Passed to zlib
-            compression, 1 is the fastest      compression, 9 is the
-            smallest possible output.
-        compression_type:
-            Control the type of compression applied to the read data.  By
-            default the vbz compressor is used (except in the single read
-            case).
-        file_pattern:
-            The pattern used to find a bulk files name. If left empty but
-            output is enabled a default pattern is used.  default:
-            {data_set}.fast5 Where each {xxx} section is replaced with an
-            attribute from the minknow state when the file is written.
-            See file pattern attributes above.
-        raw:
-            Raw data, stored with channel calibration data  Stored under
-            /Raw/Channel_*/Signal
-        events:
-            Minknow event data  Stored under
-            /IntermediateData/Channel_*/Events
-        reads:
-            Minknow read data  Stored under
-            /IntermediateData/Channel_*/Reads
-        multiplex:
-            Device multiplex data  Stored under
-            /MultiplexData/Channel_*/Multiplex
-        channel_states:
-            Channel state data  Stored under /StateData/Channel_*/States
-        device_metadata:
-            Device metadata (bias and temperature information)  Stored in
-            a per frame sequence in /Device/MetaData
-        device_commands:
-            Device commands  Stored with the frame commands take effect
-            sequence in /Device/AsicCommands
-        dynamic_analysis_config:
-            Dynamic analysis configuration  Stored with the frame config
-            took effect in /Meta/User/DynamicAnalysisConfiguration
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.BulkConfiguration)
-    })
-  ,
-
-  'ReportConfiguration' : _reflection.GeneratedProtocolMessageType('ReportConfiguration', (_message.Message,), {
-    'DESCRIPTOR' : _WRITERCONFIGURATION_REPORTCONFIGURATION,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Control settings for the report writer
-    
-    Attributes:
-        pdf_report_file_pattern:
-            DEPRECATED 6.0: As of 5.1 a pdf report is not generated at
-            all. This field will be removed in 6.0  The pattern used to
-            find the pdf report filename. If left empty but output is
-            enabled a default pattern is used.  default: report_{flow_cell
-            _id}_{daq_start_time}_{short_protocol_run_id}.pdf Where each
-            {xxx} section is replaced with an attribute from the minknow
-            state when the file is written.  See file pattern attributes
-            above.
-        json_report_file_pattern:
-            The pattern used to find the json report filename. If left
-            empty but output is enabled a default pattern is used.
-            default: report_{flow_cell_id}_{daq_start_time}_{short_protoco
-            l_run_id}.json Where each {xxx} section is replaced with an
-            attribute from the minknow state when the file is written.
-            See file pattern attributes above.
-        html_report_file_pattern:
-            The pattern used to find the html report filename. If left
-            empty but output is enabled a default pattern is used.
-            default: report_{flow_cell_id}_{daq_start_time}_{short_protoco
-            l_run_id}.html Where each {xxx} section is replaced with an
-            attribute from the minknow state when the file is written.
-            See file pattern attributes above.
-        markdown_report_file_pattern:
-            The pattern used to find the markdown report filename. If left
-            empty but output is enabled a default pattern is used.
-            default: report_{flow_cell_id}_{daq_start_time}_{short_protoco
-            l_run_id}.md Where each {xxx} section is replaced with an
-            attribute from the minknow state when the file is written.
-            See file pattern attributes above.
-        duty_time_report_file_pattern:
-            The pattern used to find the duty time csv report. If left
-            empty but output is enabled a default pattern is used.
-            default: duty_time_{flow_cell_id}_{short_run_id}.csv Where
-            each {xxx} section is replaced with an attribute from the
-            minknow state when the file is written.  See file pattern
-            attributes above.
-        throughput_report_file_pattern:
-            The pattern used to find the throughput csv report. If left
-            empty but output is enabled a default pattern is used.
-            default: throughput_{flow_cell_id}_{short_run_id}.csv Where
-            each {xxx} section is replaced with an attribute from the
-            minknow state when the file is written.  See file pattern
-            attributes above.
-        final_summary_report_file_pattern:
-            The pattern used to find the final summary report. If left
-            empty but output is enabled a default pattern is used.
-            default: final_summary_{flow_cell_id}_{short_run_id}.txt Where
-            each {xxx} section is replaced with an attribute from the
-            minknow state when the file is written.  See file pattern
-            attributes above.
-        barcode_alignment_report_file_pattern:
-            The pattern used to name the barcode-alignment report. If left
-            empty but output is enabled a default pattern is used.
-            default: barcode_alignment_{flow_cell_id}_{short_run_id}.tsv
-            Where each {xxx} section is replaced with an attribute from
-            the minknow state when the file is written.  See file pattern
-            attributes above.
-        sample_sheet_report_file_pattern:
-            The pattern used to name the sample sheet report. If left
-            empty but output is enabled a default pattern is used.
-            default: sample_sheet_{flow_cell_id}_{daq_start_time}_{short_p
-            rotocol_run_id}.csv Where each {xxx} section is replaced with
-            an attribute from the minknow state when the file is written.
-            See file pattern attributes above.
-        custom_report_suffix_pattern:
-            The pattern used to suffix custom reports.  default:
-            "_{flow_cell_id}_{short_run_id}" Where each {xxx} section is
-            replaced with an attribute from the minknow state when the
-            file is written.  Custom reports use this to build filenames:
-            - "custom_report{suffix}.txt"  See file pattern attributes
-            above.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration.ReportConfiguration)
-    })
-  ,
-  'DESCRIPTOR' : _WRITERCONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Configuration for the output writers for MinKNOWs analysis pipeline.
-  Each writer has its own section in this message, where individual data
-  elements can be enabled or disabled.  File pattern attributes
-  ----------------------- Writers have a 'file_pattern' field which
-  controls where individual files will be written to. The pattern is
-  expanded for each individual read, and then the read placed in the
-  required file. The tokens used to expand depend on the file type:
-  Read centric files (fastq, (multi-)fast5, protobuf):  -
-  read_classification:  The classification applied to the completed read
-  (eg. strand).  - batch_number:         The batch number of this read,
-  evaluated based on the destination file.  - read_id:
-  Unique read id for each read, formatted as a hash.  - read_number:
-  The read number (unique per channel, incrementing number assigned to
-  each read by MinKNOW).  - channel_name:         The name of the
-  channel which produced the read.  - read_start_time:      Read start
-  time formatted in rfc3339 format.  - basecall_status:      Basecalling
-  output status (derived from WriterDefaults section in analysis
-  config).  - pore_type:            Type of pore (as specified by
-  #set_pore_type_configuration).  General attributes:  - daq_start_time:
-  Data acquisition start time formatted as YYYYMMDD_hhmm.  -
-  protocol_start_time:  Time the current protocol was started.  -
-  run_id:               Acquisition run id formatted as hash.  -
-  short_run_id:         Shortened version of acquisition run id
-  formatted as hash.  - protocol_run_id:      Protocol run id formatted
-  as hash.  - short_protocol_run_id: Shortened protocol run id formatted
-  as hash.  - asic_id:              Integer id assigned to the asic in
-  the connected flow cell.  - flow_cell_id:         Flow cell integer as
-  read from eeprom.  - machine_id:           Name of the machine
-  (hostname or machine identifier depending on the sequencer type).  -
-  device_id:            Name of the connected sequencing device (eg.
-  MN12345).  - sample_id:            Sample id entered by the user when
-  starting a protocol.  - version_string:       Version string of the
-  running MinKNOW instance  - protocol_group_id:    Protocol group
-  entered by user when starting a protocol.  - protocol_purpose:
-  Prupose of protocol (see protocol.set_protocol_purpose())
-  
-  Attributes:
-      read_fast5:
-          Configuration for the fast5 writer.  If not specified, no
-          multi fast5 outputs are generated.
-      read_fastq:
-          Configuration for the fastq writer.  If not specified, no
-          fastq outputs are generated.
-      read_bam:
-          Configuration for the BAM writer.  If not specified, no BAM
-          outputs are generated.
-      read_pod5:
-          Configuration for the POD5 writer.  If not specified no POD5
-          outputs are generated.
-      read_protobuf:
-          Configuration for the protobuf writer.  If not specified, no
-          protobuf outputs are generated.
-      sequencing_summary:
-          Configuration for Sequencing Summary file  If not specified,
-          no summary file is generated.
-      bulk:
-          Configuration for the bulk writer.  If not specified, a basic
-          bulk output is generated.
-      report:
-          Configuration for the report writer  If
-          acquisition.StartRequest.generate_report is set for the
-          acquisition period, and empty paths (or no report config) are
-          supplied for reports default paths are used.
-      read_filters:
-          Parameters for filtering reads for writing.  If not present,
-          then no filtering will be applied, so no reads will be
-          excluded.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.WriterConfiguration)
-  })
-_sym_db.RegisterMessage(WriterConfiguration)
-_sym_db.RegisterMessage(WriterConfiguration.ChannelConfiguration)
-_sym_db.RegisterMessage(WriterConfiguration.ChannelConfiguration.ChannelList)
-_sym_db.RegisterMessage(WriterConfiguration.ChannelConfiguration.ChannelRanges)
-_sym_db.RegisterMessage(WriterConfiguration.ChannelConfiguration.ChannelRanges.ChannelRange)
-_sym_db.RegisterMessage(WriterConfiguration.ReadFast5Configuration)
-_sym_db.RegisterMessage(WriterConfiguration.ReadFastqConfiguration)
-_sym_db.RegisterMessage(WriterConfiguration.ReadBamConfiguration)
-_sym_db.RegisterMessage(WriterConfiguration.ReadPod5Configuration)
-_sym_db.RegisterMessage(WriterConfiguration.ReadProtobufConfiguration)
-_sym_db.RegisterMessage(WriterConfiguration.SequencingSummaryConfiguration)
-_sym_db.RegisterMessage(WriterConfiguration.BulkConfiguration)
-_sym_db.RegisterMessage(WriterConfiguration.ReportConfiguration)
-
-SetWriterConfigurationResponse = _reflection.GeneratedProtocolMessageType('SetWriterConfigurationResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETWRITERCONFIGURATIONRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetWriterConfigurationResponse)
-  })
-_sym_db.RegisterMessage(SetWriterConfigurationResponse)
-
-GetWriterConfigurationRequest = _reflection.GeneratedProtocolMessageType('GetWriterConfigurationRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETWRITERCONFIGURATIONREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetWriterConfigurationRequest)
-  })
-_sym_db.RegisterMessage(GetWriterConfigurationRequest)
-
-GetReadClassificationsRequest = _reflection.GeneratedProtocolMessageType('GetReadClassificationsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETREADCLASSIFICATIONSREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetReadClassificationsRequest)
-  })
-_sym_db.RegisterMessage(GetReadClassificationsRequest)
-
-GetReadClassificationsResponse = _reflection.GeneratedProtocolMessageType('GetReadClassificationsResponse', (_message.Message,), {
-
-  'ReadClassificationsEntry' : _reflection.GeneratedProtocolMessageType('ReadClassificationsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _GETREADCLASSIFICATIONSRESPONSE_READCLASSIFICATIONSENTRY,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetReadClassificationsResponse.ReadClassificationsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _GETREADCLASSIFICATIONSRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetReadClassificationsResponse)
-  })
-_sym_db.RegisterMessage(GetReadClassificationsResponse)
-_sym_db.RegisterMessage(GetReadClassificationsResponse.ReadClassificationsEntry)
-
-DynamicAnalysisConfiguration = _reflection.GeneratedProtocolMessageType('DynamicAnalysisConfiguration', (_message.Message,), {
-
-  'ReadScaleTracking' : _reflection.GeneratedProtocolMessageType('ReadScaleTracking', (_message.Message,), {
-
-    'ChannelConductance' : _reflection.GeneratedProtocolMessageType('ChannelConductance', (_message.Message,), {
-      'DESCRIPTOR' : _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING_CHANNELCONDUCTANCE,
-      '__module__' : 'minknow_api.analysis_configuration_pb2'
-      ,
-      '__doc__': """Attributes:
-          well_conductance:
-              Per well conductance values.
-      """,
-      # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.DynamicAnalysisConfiguration.ReadScaleTracking.ChannelConductance)
-      })
-    ,
-    'DESCRIPTOR' : _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING,
-    '__module__' : 'minknow_api.analysis_configuration_pb2'
-    ,
-    '__doc__': """Attributes:
-        conductance_scan_voltage:
-            Set the voltage the most recent conductance scan occured at.
-        channel_conductance:
-            Per channel/well conductance values
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.DynamicAnalysisConfiguration.ReadScaleTracking)
-    })
-  ,
-  'DESCRIPTOR' : _DYNAMICANALYSISCONFIGURATION,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  ,
-  '__doc__': """Attributes:
-      read_scale_tracking:
-          Parameters for read scale tracking:
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.DynamicAnalysisConfiguration)
-  })
-_sym_db.RegisterMessage(DynamicAnalysisConfiguration)
-_sym_db.RegisterMessage(DynamicAnalysisConfiguration.ReadScaleTracking)
-_sym_db.RegisterMessage(DynamicAnalysisConfiguration.ReadScaleTracking.ChannelConductance)
-
-GetDynamicAnalysisConfigurationRequest = _reflection.GeneratedProtocolMessageType('GetDynamicAnalysisConfigurationRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETDYNAMICANALYSISCONFIGURATIONREQUEST,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.GetDynamicAnalysisConfigurationRequest)
-  })
-_sym_db.RegisterMessage(GetDynamicAnalysisConfigurationRequest)
-
-SetDynamicAnalysisConfigurationResponse = _reflection.GeneratedProtocolMessageType('SetDynamicAnalysisConfigurationResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SETDYNAMICANALYSISCONFIGURATIONRESPONSE,
-  '__module__' : 'minknow_api.analysis_configuration_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.analysis_configuration.SetDynamicAnalysisConfigurationResponse)
-  })
-_sym_db.RegisterMessage(SetDynamicAnalysisConfigurationResponse)
-
-_ANALYSISCONFIGURATIONSERVICE = DESCRIPTOR.services_by_name['AnalysisConfigurationService']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.analysis_configuration_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
   _ANALYSISCONFIGURATION_CHANNELSTATESENTRY._options = None
   _ANALYSISCONFIGURATION_CHANNELSTATESENTRY._serialized_options = b'8\001'
   _SETANALYSISENABLEDSTATEREQUEST.fields_by_name['enable']._options = None
@@ -1551,57 +152,859 @@
   _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_CHANNELWELLLIST._serialized_start=7049
   _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_CHANNELWELLLIST._serialized_end=7159
   _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_PORETYPESENTRY._serialized_start=7162
   _PORETYPECONFIGURATION_CHANNELWELLPORETYPECONFIGURATIONS_PORETYPESENTRY._serialized_end=7319
   _SETPORETYPECONFIGURATIONRESPONSE._serialized_start=7341
   _SETPORETYPECONFIGURATIONRESPONSE._serialized_end=7375
   _WRITERCONFIGURATION._serialized_start=7378
-  _WRITERCONFIGURATION._serialized_end=11861
+  _WRITERCONFIGURATION._serialized_end=12076
   _WRITERCONFIGURATION_CHANNELCONFIGURATION._serialized_start=8271
   _WRITERCONFIGURATION_CHANNELCONFIGURATION._serialized_end=8782
   _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELLIST._serialized_start=8556
   _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELLIST._serialized_end=8587
   _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES._serialized_start=8590
   _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES._serialized_end=8770
   _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES_CHANNELRANGE._serialized_start=8728
   _WRITERCONFIGURATION_CHANNELCONFIGURATION_CHANNELRANGES_CHANNELRANGE._serialized_end=8770
   _WRITERCONFIGURATION_READFAST5CONFIGURATION._serialized_start=8785
-  _WRITERCONFIGURATION_READFAST5CONFIGURATION._serialized_end=9617
-  _WRITERCONFIGURATION_READFASTQCONFIGURATION._serialized_start=9620
-  _WRITERCONFIGURATION_READFASTQCONFIGURATION._serialized_end=9826
-  _WRITERCONFIGURATION_READBAMCONFIGURATION._serialized_start=9829
-  _WRITERCONFIGURATION_READBAMCONFIGURATION._serialized_end=10033
-  _WRITERCONFIGURATION_READPOD5CONFIGURATION._serialized_start=10036
-  _WRITERCONFIGURATION_READPOD5CONFIGURATION._serialized_end=10317
-  _WRITERCONFIGURATION_READPROTOBUFCONFIGURATION._serialized_start=10320
-  _WRITERCONFIGURATION_READPROTOBUFCONFIGURATION._serialized_end=10484
-  _WRITERCONFIGURATION_SEQUENCINGSUMMARYCONFIGURATION._serialized_start=10487
-  _WRITERCONFIGURATION_SEQUENCINGSUMMARYCONFIGURATION._serialized_end=10635
-  _WRITERCONFIGURATION_BULKCONFIGURATION._serialized_start=10638
-  _WRITERCONFIGURATION_BULKCONFIGURATION._serialized_end=11365
-  _WRITERCONFIGURATION_REPORTCONFIGURATION._serialized_start=11368
-  _WRITERCONFIGURATION_REPORTCONFIGURATION._serialized_end=11777
-  _WRITERCONFIGURATION_COMPRESSIONTYPE._serialized_start=11779
-  _WRITERCONFIGURATION_COMPRESSIONTYPE._serialized_end=11861
-  _SETWRITERCONFIGURATIONRESPONSE._serialized_start=11863
-  _SETWRITERCONFIGURATIONRESPONSE._serialized_end=11895
-  _GETWRITERCONFIGURATIONREQUEST._serialized_start=11897
-  _GETWRITERCONFIGURATIONREQUEST._serialized_end=11928
-  _GETREADCLASSIFICATIONSREQUEST._serialized_start=11930
-  _GETREADCLASSIFICATIONSREQUEST._serialized_end=11961
-  _GETREADCLASSIFICATIONSRESPONSE._serialized_start=11964
-  _GETREADCLASSIFICATIONSRESPONSE._serialized_end=12179
-  _GETREADCLASSIFICATIONSRESPONSE_READCLASSIFICATIONSENTRY._serialized_start=12121
-  _GETREADCLASSIFICATIONSRESPONSE_READCLASSIFICATIONSENTRY._serialized_end=12179
-  _DYNAMICANALYSISCONFIGURATION._serialized_start=12182
-  _DYNAMICANALYSISCONFIGURATION._serialized_end=12562
-  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING._serialized_start=12328
-  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING._serialized_end=12562
-  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING_CHANNELCONDUCTANCE._serialized_start=12516
-  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING_CHANNELCONDUCTANCE._serialized_end=12562
-  _GETDYNAMICANALYSISCONFIGURATIONREQUEST._serialized_start=12564
-  _GETDYNAMICANALYSISCONFIGURATIONREQUEST._serialized_end=12604
-  _SETDYNAMICANALYSISCONFIGURATIONRESPONSE._serialized_start=12606
-  _SETDYNAMICANALYSISCONFIGURATIONRESPONSE._serialized_end=12647
-  _ANALYSISCONFIGURATIONSERVICE._serialized_start=12650
-  _ANALYSISCONFIGURATIONSERVICE._serialized_end=15382
+  _WRITERCONFIGURATION_READFAST5CONFIGURATION._serialized_end=9660
+  _WRITERCONFIGURATION_READFASTQCONFIGURATION._serialized_start=9663
+  _WRITERCONFIGURATION_READFASTQCONFIGURATION._serialized_end=9912
+  _WRITERCONFIGURATION_READBAMCONFIGURATION._serialized_start=9915
+  _WRITERCONFIGURATION_READBAMCONFIGURATION._serialized_end=10162
+  _WRITERCONFIGURATION_READPOD5CONFIGURATION._serialized_start=10165
+  _WRITERCONFIGURATION_READPOD5CONFIGURATION._serialized_end=10489
+  _WRITERCONFIGURATION_READPROTOBUFCONFIGURATION._serialized_start=10492
+  _WRITERCONFIGURATION_READPROTOBUFCONFIGURATION._serialized_end=10699
+  _WRITERCONFIGURATION_SEQUENCINGSUMMARYCONFIGURATION._serialized_start=10702
+  _WRITERCONFIGURATION_SEQUENCINGSUMMARYCONFIGURATION._serialized_end=10850
+  _WRITERCONFIGURATION_BULKCONFIGURATION._serialized_start=10853
+  _WRITERCONFIGURATION_BULKCONFIGURATION._serialized_end=11580
+  _WRITERCONFIGURATION_REPORTCONFIGURATION._serialized_start=11583
+  _WRITERCONFIGURATION_REPORTCONFIGURATION._serialized_end=11992
+  _WRITERCONFIGURATION_COMPRESSIONTYPE._serialized_start=11994
+  _WRITERCONFIGURATION_COMPRESSIONTYPE._serialized_end=12076
+  _SETWRITERCONFIGURATIONRESPONSE._serialized_start=12078
+  _SETWRITERCONFIGURATIONRESPONSE._serialized_end=12110
+  _GETWRITERCONFIGURATIONREQUEST._serialized_start=12112
+  _GETWRITERCONFIGURATIONREQUEST._serialized_end=12143
+  _GETREADCLASSIFICATIONSREQUEST._serialized_start=12145
+  _GETREADCLASSIFICATIONSREQUEST._serialized_end=12176
+  _GETREADCLASSIFICATIONSRESPONSE._serialized_start=12179
+  _GETREADCLASSIFICATIONSRESPONSE._serialized_end=12394
+  _GETREADCLASSIFICATIONSRESPONSE_READCLASSIFICATIONSENTRY._serialized_start=12336
+  _GETREADCLASSIFICATIONSRESPONSE_READCLASSIFICATIONSENTRY._serialized_end=12394
+  _DYNAMICANALYSISCONFIGURATION._serialized_start=12397
+  _DYNAMICANALYSISCONFIGURATION._serialized_end=12777
+  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING._serialized_start=12543
+  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING._serialized_end=12777
+  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING_CHANNELCONDUCTANCE._serialized_start=12731
+  _DYNAMICANALYSISCONFIGURATION_READSCALETRACKING_CHANNELCONDUCTANCE._serialized_end=12777
+  _GETDYNAMICANALYSISCONFIGURATIONREQUEST._serialized_start=12779
+  _GETDYNAMICANALYSISCONFIGURATIONREQUEST._serialized_end=12819
+  _SETDYNAMICANALYSISCONFIGURATIONRESPONSE._serialized_start=12821
+  _SETDYNAMICANALYSISCONFIGURATIONRESPONSE._serialized_end=12862
+  _ANALYSISCONFIGURATIONSERVICE._serialized_start=12865
+  _ANALYSISCONFIGURATIONSERVICE._serialized_end=15597
+DynamicAnalysisConfiguration.ReadScaleTracking.__doc__ = """Attributes:
+    conductance_scan_voltage:
+        Set the voltage the most recent conductance scan occured at.
+    channel_conductance:
+        Per channel/well conductance values
+"""
+GetChannelStatesDescResponse.ChannelState.__doc__ = """Attributes:
+    id:
+        The numeric identifier of the state.  This is what is reported
+        in any other APIs that return a channel state ID.
+    name:
+        The internal name of the state.  This is what is reported in
+        any other APIs that return a channel state name.
+    style:
+        How to render the channel state in a graphical user interface.
+        Note that the style may be missing from some channel states
+        (such as the ones that are built in to MinKNOW).
+    global_order:
+        An order ranking for the channel states when they are
+        ungrouped.  This can be used to order the channel states after
+        merging the groups.
+"""
+ChannelStates.Logic.Behaviour.__doc__ = """Attributes:
+    reset_on_mux_change:
+        TODO: MinKNOW 5: replace int32 with bool for these options
+        these are ints but act like bools
+    latch:
+        If the latch value is set to true, then when the criteria for
+        this channel state is active, then the latch will keep it
+        active until the channel state is reset.
+    reset_on_effective_mux_change:
+        An 'effective mux change' is any mux change apart from the one
+        triggered with the purpose of disconnecting a channel (turning
+        a channel off). For example, if a channel is in pore, and the
+        user changes the channel configuration to 'disconnected', that
+        mux change will not be an effective mux change. Any other mux
+        change is considered an 'effective mux change'. So if a
+        channel saturates, the mux change to disconnected is an
+        effective mux change. Similarly, a change from disconnected to
+        a pore is an effective mux change.  Use this reset mode to
+        make the channel state persist on non-effective mux changes.
+        For example, if a channel state is in 'multiple' and the user
+        triggers a channel configuration change to 'disconnected', the
+        state will remain in multiple if it has this option on. The
+        multiple state will be reset at all other mux changes (i.e.
+        effective mux changes).
+    reset_on_effective_well_change:
+        An 'effective well change' is any well change apart from the
+        one triggered with the purpose of disconnecting a channel
+        (turning a channel off). For example, if a channel is in
+        well_1, and the user changes the channel configuration to
+        'unblock_1', that change will not be an effective well change.
+        A change to disconnected is also not considered an effective
+        well change.  Use this reset mode to make the channel state
+        persist on non-effective well changes. For example, if a
+        channel state is in 'multiple' and the user triggers a channel
+        configuration change to 'disconnected', the state will remain
+        in multiple if it has this option on. The multiple state will
+        be reset then when the mux is set to a different setting.
+"""
+BasecallerConfiguration.TargetFiltering.__doc__ = """Since 3.7"""
+ChannelStates.Logic.__doc__ = """Attributes:
+    rank:
+        Specifies the order in which channel state criteria will be
+        evaluated; the smaller the number, the earlier it will be
+        evaluated. The first criteria to match will be selected
+    pattern:
+        Note that this is a regex based pattern for describing a read
+        classification sequence. For example you can specify:
+        "unavailableunavailable" or:      "(unavailable)(unavailable)"
+        to recognise two consecutive read chunks classified as
+        unavailable.  You can also use "?" at the end of one of the
+        classifications in the sequence to indicate that it may or may
+        not be present at that point. For example:
+        "(pore)(transition)?(event)"  This will match both of the
+        sequences:      pore, transition, event      pore, event  The
+        technical documentation has more information on the range of
+        regex patterns you can apply.
+        https://minknow.git.oxfordnanolabs.local/minknow-
+        core/analysis/channel-states.html
+    ranges:
+        Range is [lower_pa, upper_pa)
+"""
+ReadClassificationParams.__doc__ = """Attributes:
+    max_sample_size:
+        This tells minknow the maximum number of means to store in
+        memory before using a different strategy to calculate medians.
+        If the number of means goes over this size then the strategy
+        used may be less accurate, but will not use as much memory in
+        minknow
+    selected_classifications:
+        A list of classifications that are deemed interesting, and
+        will be marked to be written out to file
+    open_pore_classifications:
+        A set of classifications whose level should be tracked as the
+        level of open pore (fed back into read detection analysis).
+        Read chunks selected by this filter will be aggregated for use
+        in read detection.
+    open_pore_ewma_weight:
+        A weighting figure for the exponentially weighted moving
+        average given to the newest data. eg. 0.7 would weight new
+        data with 0.3 and all previous data with 0.7.  By default 0.5
+        is used.
+    open_pore_ignore_after_reset_seconds:
+        A number of seconds to ignore new chunks for after a reset
+        occurs on a channel this allows analysis to ignore spikes or
+        bad data on the channel for a small section of time.  By
+        default 0.0 is used - and chunks are accepted immediately.
+    classification_strategy:
+        Determine how to classify a whole read based on the strategy
+        'ultimate':      Chooses the last (ultimate) read chunk's
+        classification 'penultimate':   Chooses the second-to-last
+        read chunk's clasification 'modal':         Chooses the most
+        common classification out of the all read chunks
+"""
+EventDetection.__doc__ = """Attributes:
+    window_size:
+        The window size that the tstats are calculated from
+    threshold:
+        The peak detection must be above this threshold at a minimum
+        for it to be detected as an event.
+    peak_height:
+        When analysing the tstat peaks, if the jump between one value
+        and another is higher than than 'peak_height', then it will
+        "arm" the peak detector and move onto the next phase.  And
+        what goes up must come down. Once it has detected a peak going
+        up, it will also have to go down by 'peak_height' in order for
+        the peak to be classified as a found event
+    events_to_base_ratio:
+        Conversion factor used to convert from events to bases.  This
+        is used to estimate bases for various rpc feeds from minknow.
+    break_on_mux_changes:
+        Whether to break events on mux changes.  This will eliminate
+        "mux_uncertain" events and reads. Note that this will cause
+        starting or stopping unblocking to break events as well (even
+        though the mux does not normally change in this case).
+    max_mux_change_back_shift:
+        Control the number of samples MinKNOW will shift mux changes
+        back by in order to align mux changes with event boundaries.
+        When break on mux changes is enabled its possible that mux
+        changes recorded from the device and signal deltas caused by
+        the config changes will not align exactly (the signal delta
+        happen prior to the mux change due to the recorded sample
+        indicating the command is fully applied). Setting this value
+        to > 0 will allow minknow to record the mux change as active
+        up to this number of samples _before_ the device recorded the
+        change as active. Mux changes are never shifted forwards.  A
+        value of 0 will disable shifting of mux changes.
+"""
+ReadScalingParams.__doc__ = """Since 5.3  Quantile Information:
+
+Attributes:
+    quantile_locations:
+        Position of quantiles in scaling data to use when computing
+        scale parameters.
+    quantile_weights_shift:
+        If present, must be the same length as quantile_locations.
+        Represents the coefficients that shall be multiplied with
+        measured quantiles to give a predicted_shift
+    quantile_weights_scale:
+        If present, must be the same length as quantile_locations.
+        Represents the coefficients that shall be multiplied with
+        measured quantiles to give a predicted_scale
+    tracking_alpha:
+        Alpha value to use in ewma calculation for scale and shift
+        tracking. 1 updates instantly. 0 does not update.
+    alpha_number_estimates_decay:
+        Alpha decay value to use. Higher values cause a more rapid
+        decay in greater trust of earlier numbers.
+    quantile_maxdiff:
+        Maximum difference in event quantiles which will be added into
+        trackers.  This is used to filter away cases where pore signal
+        is included in the read and thus cannot be trusted.
+    trust_limit_fraction:
+        Maximum fraction change between one tracked value and the next
+        which will be trusted. Higher values are not trusted.
+    diff_threshold:
+        The minimum difference between an event and the next to
+        include it in the subsampling
+    emission_threshold:
+        After how many cumulative pA is a new event emitted in the
+        subsampling
+    dacs_breakpoint:
+        Cumulative pA sum required to compute scaling. Any events
+        after this sum are not considered in scaling.
+    conductance_factor_scale:
+        Scale factor applied to conductance to produce a basic scale
+        estimate, also combined with q90_q10_to_normal.
+    conductance_factor_shift:
+        Scale factor applied to conductance to produce a basic shift
+        estimate.
+"""
+WriterConfiguration.ChannelConfiguration.__doc__ = """Used to control which channels for a specific data type emit data
+
+Attributes:
+    channels:
+        Control the way channels are enabled for this data type.
+"""
+WriterConfiguration.ReadBamConfiguration.__doc__ = """Attributes:
+    enable:
+        Control if a BAM file should be generated per channel.
+    file_pattern:
+        The pattern used to find a BAM files name.  default: bam{basec
+        all_status}/{flow_cell_id}_{run_id}_{batch_number}.bam Where
+        each {xxx} section is replaced with an attribute from the
+        minknow state when the file is written.  See file pattern
+        attributes above.
+    batch_count:
+        How many reads are placed in each batch (after batch_count
+        reads {batch_number} is increased in the pattern).
+    bases_per_batch:
+        Number of estimated bases within a batch before it rotates to
+        a new batch
+    disable_writing_multiple_alignments:
+        If true minknow will only write the primary alignment for each
+        read.
+"""
+AnalysisConfiguration.__doc__ = """Attributes:
+    read_scaling:
+        Add read scale tracking to the pipeline. If this message is
+        unspecified, read scaling is not enabled.
+"""
+PoreTypeConfiguration.__doc__ = """The pore type configuration  The ways of specifying a configuration
+are as follows: - global_pore_type: all wells have a pore type of
+global_pore_type. - channel_well_pore_types: channels are allowed
+different values per channel/well   (allows a subset of channels to be
+set).
+
+Attributes:
+    global_pore_type:
+        Set all channel/wells to one pore type.
+    channel_well_pore_types:
+        Set channel/wells to different pore types.  Pore types can be
+        created without being used by adding an empty entry.
+"""
+ReadClassificationParams.Parameters.__doc__ = """Attributes:
+    rules_in_execution_order:
+        An execution rule has the following format:  "pore =
+        (median,gt,185)&(median,lt,260)&(median_sd,lt,40)"  "median"
+        and "median_sd" are apart of a small subset of variable values
+        describing a read or read chunk, that are exposed to execution
+        rules. The full list of variable values and their descriptions
+        are documented here:
+        https://minknow.git.oxfordnanolabs.local/minknow-
+        core/analysis/reads.html  "gt" and "lt" describe how data can
+        be compared: gt: greater than lt: less than eq: equal ne: not
+        equal  Constant values like "185" or "260" can also be
+        specified. These can be real numbers also.  Note that
+        variables dont always have to be on the left and const values
+        on the right. The following sub rules are also valid:
+        (200,lt,median_sd) (median_before,gt,median) (5,lt,10)
+"""
+WriterConfiguration.__doc__ = """Configuration for the output writers for MinKNOWs analysis pipeline.
+Each writer has its own section in this message, where individual data
+elements can be enabled or disabled.  File pattern attributes
+----------------------- Writers have a 'file_pattern' field which
+controls where individual files will be written to. The pattern is
+expanded for each individual read, and then the read placed in the
+required file. The tokens used to expand depend on the file type:
+Read centric files (fastq, (multi-)fast5, protobuf):  -
+read_classification:  The classification applied to the completed read
+(eg. strand).  - batch_number:         The batch number of this read,
+evaluated based on the destination file.  - read_id:
+Unique read id for each read, formatted as a hash.  - read_number:
+The read number (unique per channel, incrementing number assigned to
+each read by MinKNOW).  - channel_name:         The name of the
+channel which produced the read.  - read_start_time:      Read start
+time formatted in rfc3339 format.  - basecall_status:      Basecalling
+output status (derived from WriterDefaults section in analysis
+config).  - pore_type:            Type of pore (as specified by
+#set_pore_type_configuration).  General attributes:  - daq_start_time:
+Data acquisition start time formatted as YYYYMMDD_hhmm.  -
+protocol_start_time:  Time the current protocol was started.  -
+run_id:               Acquisition run id formatted as hash.  -
+short_run_id:         Shortened version of acquisition run id
+formatted as hash.  - protocol_run_id:      Protocol run id formatted
+as hash.  - short_protocol_run_id: Shortened protocol run id formatted
+as hash.  - asic_id:              Integer id assigned to the asic in
+the connected flow cell.  - flow_cell_id:         Flow cell integer as
+read from eeprom.  - machine_id:           Name of the machine
+(hostname or machine identifier depending on the sequencer type).  -
+device_id:            Name of the connected sequencing device (eg.
+MN12345).  - sample_id:            Sample id entered by the user when
+starting a protocol.  - version_string:       Version string of the
+running MinKNOW instance  - protocol_group_id:    Protocol group
+entered by user when starting a protocol.  - protocol_purpose:
+Prupose of protocol (see protocol.set_protocol_purpose())
+
+Attributes:
+    read_fast5:
+        Configuration for the fast5 writer.  If not specified, no
+        multi fast5 outputs are generated.
+    read_fastq:
+        Configuration for the fastq writer.  If not specified, no
+        fastq outputs are generated.
+    read_bam:
+        Configuration for the BAM writer.  If not specified, no BAM
+        outputs are generated.
+    read_pod5:
+        Configuration for the POD5 writer.  If not specified no POD5
+        outputs are generated.
+    read_protobuf:
+        Configuration for the protobuf writer.  If not specified, no
+        protobuf outputs are generated.
+    sequencing_summary:
+        Configuration for Sequencing Summary file  If not specified,
+        no summary file is generated.
+    bulk:
+        Configuration for the bulk writer.  If not specified, a basic
+        bulk output is generated.
+    report:
+        Configuration for the report writer  If
+        acquisition.StartRequest.generate_report is set for the
+        acquisition period, and empty paths (or no report config) are
+        supplied for reports default paths are used.
+    read_filters:
+        Parameters for filtering reads for writing.  If not present,
+        then no filtering will be applied, so no reads will be
+        excluded.
+"""
+AlignmentConfiguration.__doc__ = """Since 4.0
+
+Attributes:
+    reference_files:
+        Provide an index to align reads against once basecalled.  Any
+        acceptable reference format to guppy can be passed here:   -
+        fasta reference file   - minimap index file
+    bed_file:
+        Provide a bed file for use indicating areas of interest in
+        alignment results.  Note: alignment_index must be provided for
+        this argument to be valid.
+    minimum_coverage:
+        Minimum coverage for guppy to accept an alignment.  If not
+        specified a default value is used.  Note: this option cannot
+        be used during live basecalling.
+    aggregate_statistics_for_multiple_bed_hits:
+        Control how statistics for bed results are aggregated.  If set
+        to false only the bed hit with the highest overlap is used
+        when computing heatmap/throughput graphs with bed hits.  If
+        set to true each bed hit is considered and bases for all hits
+        are counted. This may give more honest representation of
+        individual bed hit results but will skew read count statistics
+        - as each hit will be counted for every bed hit.  Note: this
+        option has no effect in offline basecalling.
+"""
+WriterConfiguration.ReadProtobufConfiguration.__doc__ = """Attributes:
+    enable:
+        Control if a protobuf file should be generated per channel.
+    file_pattern:
+        The pattern used to find a protobuf files name.  default: pbre
+        ad{basecall_status}/{batch_number}/{flow_cell_id}_{run_id}_ch_
+        {channel_name}_read_{read_number}.pbread Where each {xxx}
+        section is replaced with an attribute from the minknow state
+        when the file is written.  See file pattern attributes above.
+    batch_count:
+        How many reads are placed in each batch (after batch_count
+        reads {batch_number} is increased in the pattern).
+    bases_per_batch:
+        Number of estimated bases within a batch before it rotates to
+        a new batch
+"""
+GetSummaryResponse.__doc__ = """Attributes:
+    analysis_enabled:
+        Whether any analysis is enabled.  If this is false, everything
+        else will be false as well.
+    basecalling_enabled:
+        Whether basecalling is enabled.
+"""
+PoreTypeConfiguration.ChannelWell.__doc__ = """Attributes:
+    channel:
+        Channel number to control pore type for.  Must be less than
+        channel count for the current platform
+    well:
+        Well to control pore type for.  Wells outside the available
+        wells on the flowcell are ignored.
+"""
+LampConfiguration.__doc__ = """Since 4.1
+
+Attributes:
+    lamp_kit:
+        Set the lamp kit being used.
+    min_score_barcodes:
+        Optionally specify a min score to detect a valid lamp barcode.
+    min_score_masks:
+        Optionally set the minimimum valid score for a lamp mask.
+    min_score_targets:
+        Optionally specify a minimum score for lamp targets.
+"""
+ReadFilters.__doc__ = """Parameters for filtering out reads from being written.  The tests are
+combined using a logical AND: if any given test fails, the read will
+not be written. Only reads that pass all (non-zero) tests will be
+written out.  Currently, it is only possible to filter on read length.
+This can be given in samples or MinKNOW events.
+
+Attributes:
+    read_length_min:
+        Only write reads that contain at least this many samples.  The
+        default zero value will not exclude any reads.
+    read_length_max:
+        Only write reads that contain at most this many samples.  If
+        set to zero (the default), this test is not applied (as though
+        it had been set to a value longer than any possible read).
+    event_count_min:
+        Only write reads that contain at least this many MinKNOW
+        events.  The default zero value will not exclude any reads.
+    event_count_max:
+        Only write reads that contain at most this many MinKNOW
+        events.  If set to zero (the default), this test is not
+        applied (as though it had been set to a value longer than any
+        possible read).
+"""
+BasecallerConfiguration.__doc__ = """Since 3.0
+
+Attributes:
+    enable:
+        Choose if guppy is enabled or disabled.  If set to false then
+        no basecalling will take place, and the rest of the config is
+        ignored.
+    config_filename:
+        The Guppy cfg file with all the settings.  Filename can be
+        absolute, or a basename (eg dna_r9.4_450bps.cfg) which guppy
+        should locate (see guppy application config entry:
+        "data_path")
+    align_filter:
+        Enable or disable pass/fail filtering based on alignment.
+        When enabled, reads which do not align to any references will
+        be marked as "failed", and written to the folder specified in
+        MinKNOW configuration for failed reads.    The setting applies
+        to both regular read filtering and target filtering; if it is
+        enabled, then a read will not be marked as a target read if it
+        does not align to a reference.  Default setting is false, i.e.
+        disabled.  Since 5.4
+    read_filtering:
+        Control how read filtering is applied to output of basecaller.
+        These settings determine whether a read is marked as "passed"
+        or "failed".  Reads are written to different folders based on
+        the result of this filtering.  Those folders are specified in
+        MinKNOW configuration.  If no filtering parameters are
+        provided then reads will not be filtered.
+    barcoding_configuration:
+        Control the barcoding configuration. If no barcoding
+        configuration is supplied, barcoding is disabled.  Since 3.5
+    target_filtering:
+        Control how target filtering is applied to output of
+        basecaller. Reads which pass these filtering criteria will be
+        marked as "target" reads, and will be written to a separate
+        folder; this  folder is specified in MinKNOW configuration.
+        Reads which do  not pass these criteria will have the regular
+        read filtering applied to them, as specified by the `read-
+        filtering` settings above.  If no filtering parameters are
+        provided then reads will not be target-filtered.  Since 3.7
+    alignment_configuration:
+        Alignment configuration parameters. If no configuration is
+        specified alignment is disabled.  Since 4.0
+    lamp_configuration:
+        Lamp configuration parameters. If no configuration is
+        specified lamp is disabled.  Since 4.1
+    enable_read_splitting:
+        Enable read splitting in guppy.  Since 4.5
+    min_score_read_splitting:
+        Override score to use for guppy read splitting. If not
+        specified a default value is used from guppy.  Since 4.5
+"""
+WriterConfiguration.ChannelConfiguration.ChannelRanges.__doc__ = """Attributes:
+    ranges:
+        List of start/end paired channel numbers which should be
+        enabled for writing.  All channels in inclusive ranges should
+        be enabled.
+"""
+GetChannelStatesDescResponse.__doc__ = """Attributes:
+    groups:
+        The groups of channel states.  The groups are ordered
+        according to the "order" attribute of the group style in the
+        channel states configuration.
+"""
+DynamicAnalysisConfiguration.ReadScaleTracking.ChannelConductance.__doc__ = """Attributes:
+    well_conductance:
+        Per well conductance values.
+"""
+BarcodingConfiguration.__doc__ = """Since 3.5
+
+Attributes:
+    barcoding_kits:
+        The barcoding kits in use One entry per kit If no barcoding
+        kits are supplied, barcoding is disabled.
+    trim_barcodes:
+        Whether Guppy should trim barcodes If not specified, this
+        value defaults to false (not triming barcodes) If barcoding is
+        not enabled (e.g., because no barcoding kits are specified),
+        this parameter has no effect.
+    require_barcodes_both_ends:
+        Barcode is only classified if a barcode above `min_score` is
+        present at both ends of the basecalled read.
+    detect_mid_strand_barcodes:
+        Search for barcodes through the entire length of the read.  If
+        a barcode is found in the middle of a read the read is marked
+        as unclassified.
+    min_score:
+        Minimum alignment score to consider a valid barcode.  Maximum
+        value is 100, defaults to 60.
+    min_score_rear:
+        Minimum score to consider a valid barcode (overrides min_score
+        for rear barcodes).  Maximum value is 100, defaults to
+        min_score if not specified.
+    min_score_mid:
+        Minimum score to consider a valid mid barcode (only valid if
+        detect_mid_strand_barcodes is specified).  Maximum value is
+        100, defaults to 60.
+    min_score_mask:
+        The minimum score required for the barcode mask to be
+        detected.  Maximum value is 100, defaults to 40.
+"""
+WriterConfiguration.SequencingSummaryConfiguration.__doc__ = """Attributes:
+    enable:
+        Should a sequencing summary file be generated
+    file_pattern:
+        The pattern used to find a summary files name.  default:
+        sequencing_summary_{flow_cell_id}_{short_run_id}.txt Where
+        each {xxx} section is replaced with an attribute from the
+        minknow state when the file is written.  See file pattern
+        attributes above.
+"""
+ChannelStates.Logic.Ranges.__doc__ = """Dont really like this way of doing it, but it has to match the old
+way..."""
+PoreTypeConfiguration.ChannelWellPoreTypeConfigurations.__doc__ = """Attributes:
+    pore_types:
+        Map with pore type as key, mapped to the list of wells to set
+        for.  It is undefined what will happen if one call sets the
+        pore type of a channel and well to two pore types.
+"""
+DynamicAnalysisConfiguration.__doc__ = """Attributes:
+    read_scale_tracking:
+        Parameters for read scale tracking:
+"""
+WriterConfiguration.ReadFastqConfiguration.__doc__ = """Attributes:
+    enable:
+        Control if a fastq file should be generated per channel.
+    file_pattern:
+        The pattern used to find a fastq files name.  default: fastq{b
+        asecall_status}/{flow_cell_id}_{run_id}_{batch_number}.fastq
+        Where each {xxx} section is replaced with an attribute from
+        the minknow state when the file is written.  See file pattern
+        attributes above.
+    header_pattern:
+        The pattern used to find a fastq header.  default: {read_id}
+        runid={run_id} read={read_number} ch={channel_name}
+        start_time={read_start_time} Where each {xxx} section is
+        replaced with an attribute from the minknow state when the
+        fastq is generated.
+    batch_count:
+        How many reads are placed in each batch (after batch_count
+        reads {batch_number} is increased in the pattern).
+    bases_per_batch:
+        Number of estimated bases within a batch before it rotates to
+        a new batch
+    compression:
+        Compress fastq files with gzip compression. default: false
+"""
+WriterConfiguration.ReportConfiguration.__doc__ = """Control settings for the report writer
+
+Attributes:
+    pdf_report_file_pattern:
+        DEPRECATED 6.0: As of 5.1 a pdf report is not generated at
+        all. This field will be removed in 6.0  The pattern used to
+        find the pdf report filename. If left empty but output is
+        enabled a default pattern is used.  default: report_{flow_cell
+        _id}_{daq_start_time}_{short_protocol_run_id}.pdf Where each
+        {xxx} section is replaced with an attribute from the minknow
+        state when the file is written.  See file pattern attributes
+        above.
+    json_report_file_pattern:
+        The pattern used to find the json report filename. If left
+        empty but output is enabled a default pattern is used.
+        default: report_{flow_cell_id}_{daq_start_time}_{short_protoco
+        l_run_id}.json Where each {xxx} section is replaced with an
+        attribute from the minknow state when the file is written.
+        See file pattern attributes above.
+    html_report_file_pattern:
+        The pattern used to find the html report filename. If left
+        empty but output is enabled a default pattern is used.
+        default: report_{flow_cell_id}_{daq_start_time}_{short_protoco
+        l_run_id}.html Where each {xxx} section is replaced with an
+        attribute from the minknow state when the file is written.
+        See file pattern attributes above.
+    markdown_report_file_pattern:
+        The pattern used to find the markdown report filename. If left
+        empty but output is enabled a default pattern is used.
+        default: report_{flow_cell_id}_{daq_start_time}_{short_protoco
+        l_run_id}.md Where each {xxx} section is replaced with an
+        attribute from the minknow state when the file is written.
+        See file pattern attributes above.
+    duty_time_report_file_pattern:
+        The pattern used to find the duty time csv report. If left
+        empty but output is enabled a default pattern is used.
+        default: duty_time_{flow_cell_id}_{short_run_id}.csv Where
+        each {xxx} section is replaced with an attribute from the
+        minknow state when the file is written.  See file pattern
+        attributes above.
+    throughput_report_file_pattern:
+        The pattern used to find the throughput csv report. If left
+        empty but output is enabled a default pattern is used.
+        default: throughput_{flow_cell_id}_{short_run_id}.csv Where
+        each {xxx} section is replaced with an attribute from the
+        minknow state when the file is written.  See file pattern
+        attributes above.
+    final_summary_report_file_pattern:
+        The pattern used to find the final summary report. If left
+        empty but output is enabled a default pattern is used.
+        default: final_summary_{flow_cell_id}_{short_run_id}.txt Where
+        each {xxx} section is replaced with an attribute from the
+        minknow state when the file is written.  See file pattern
+        attributes above.
+    barcode_alignment_report_file_pattern:
+        The pattern used to name the barcode-alignment report. If left
+        empty but output is enabled a default pattern is used.
+        default: barcode_alignment_{flow_cell_id}_{short_run_id}.tsv
+        Where each {xxx} section is replaced with an attribute from
+        the minknow state when the file is written.  See file pattern
+        attributes above.
+    sample_sheet_report_file_pattern:
+        The pattern used to name the sample sheet report. If left
+        empty but output is enabled a default pattern is used.
+        default: sample_sheet_{flow_cell_id}_{daq_start_time}_{short_p
+        rotocol_run_id}.csv Where each {xxx} section is replaced with
+        an attribute from the minknow state when the file is written.
+        See file pattern attributes above.
+    custom_report_suffix_pattern:
+        The pattern used to suffix custom reports.  default:
+        "_{flow_cell_id}_{short_run_id}" Where each {xxx} section is
+        replaced with an attribute from the minknow state when the
+        file is written.  Custom reports use this to build filenames:
+        - "custom_report{suffix}.txt"  See file pattern attributes
+        above.
+"""
+GetChannelStatesDescResponse.Group.__doc__ = """Attributes:
+    name:
+        The name of the group.
+    style:
+        How to render the group in a graphical user interface.  Note
+        that the style may be missing from some groups (such as the
+        ones that are built in to MinKNOW).
+    states:
+        The channel states contained in the group.  The groups are
+        ordered according to the "order" attribute of the channel
+        state style in the channel states configuration.
+"""
+WriterConfiguration.ReadFast5Configuration.__doc__ = """Attributes:
+    compression_level:
+        Control the level of compression applied to read data.  0:
+        No compression will be applied to data. 1-9: Passed to zlib
+        compression, 1 is the fastest      compression, 9 is the
+        smallest possible output.
+    compression_type:
+        Control the type of compression applied to the read data.  By
+        default the vbz compressor is used (except in the single read
+        case).
+    raw:
+        Raw data, stored with calibration data, and read attributes.
+        Stored under /Raw/Reads_*/Signal
+    fastq:
+        Fastq data, stored as a string.  Stored under
+        /Analyses/Basecall_1D_*/BaseCalled_(template|complement)/Fastq
+    trace_table:
+        Trace table received from Guppy  Stored under
+        /Analyses/Basecall_1D_*/BaseCalled_template/Trace
+    move_table:
+        Move table received from Guppy  Stored under
+        /Analyses/Basecall_1D_*/BaseCalled_template/Move
+    modifications_table:
+        Base modification probability table  Store under
+        /Analyses/Basecall_1D_*/BaseCalled_template/ModBaseProbs
+    disable_writing_passed_reads:
+        Prevent reads which have successfully basecalled being written
+        to fast5.
+    disable_writing_failed_reads:
+        Prevent reads which have failed basecalling being written to
+        fast5.
+    disable_writing_force_skipped_reads:
+        disable writing reads which have been force skipped by the
+        basecaller.
+    file_pattern:
+        The pattern used to find a fast5 files name.  default: fast5{b
+        asecall_status}/{flow_cell_id}_{run_id}_{batch_number}.fast5
+        Where each {xxx} section is replaced with an attribute from
+        the minknow state when the file is written.  See file pattern
+        attributes above.
+    fastq_header_pattern:
+        The pattern used to find a fastq header.  default: {read_id}
+        runid={run_id} read={read_number} ch={channel_name}
+        start_time={read_start_time} Where each {xxx} section is
+        replaced with an attribute from the minknow state when the
+        fastq is generated.
+    batch_count:
+        How many reads are placed in each batch (after batch_count
+        reads {batch_number} is increased in the pattern).
+    bases_per_batch:
+        Number of estimated bases within a batch before it rotates to
+        a new batch
+"""
+WriterConfiguration.ReadPod5Configuration.__doc__ = """Attributes:
+    enable:
+        Control if a POD5 file should be generated per channel.
+    file_pattern:
+        The pattern used to find a POD5 files name.  default: pod5{bas
+        ecall_status}/{flow_cell_id}_{run_id}_{batch_number}.pod5
+        Where each {xxx} section is replaced with an attribute from
+        the minknow state when the file is written.  See file pattern
+        attributes above.
+    batch_count:
+        How many reads are placed in each batch (after batch_count
+        reads {batch_number} is increased in the pattern).
+    bases_per_batch:
+        Number of estimated bases within a batch before it rotates to
+        a new batch
+    disable_writing_passed_reads:
+        Prevent reads which have successfully basecalled being written
+        to pod5.
+    disable_writing_failed_reads:
+        Prevent reads which have failed basecalling being written to
+        pod5.
+    disable_writing_force_skipped_reads:
+        disable writing reads which have been force skipped by the
+        basecaller.
+"""
+WriterConfiguration.ChannelConfiguration.ChannelList.__doc__ = """Attributes:
+    channels:
+        List of channel names (one based) which should be enabled for
+        writing.
+"""
+WriterConfiguration.BulkConfiguration.__doc__ = """Control settings for the bulk writer
+
+Attributes:
+    compression_level:
+        Control the level of compression applied to read data.  0:
+        No compression will be applied to data. 1-9: Passed to zlib
+        compression, 1 is the fastest      compression, 9 is the
+        smallest possible output.
+    compression_type:
+        Control the type of compression applied to the read data.  By
+        default the vbz compressor is used (except in the single read
+        case).
+    file_pattern:
+        The pattern used to find a bulk files name. If left empty but
+        output is enabled a default pattern is used.  default:
+        {data_set}.fast5 Where each {xxx} section is replaced with an
+        attribute from the minknow state when the file is written.
+        See file pattern attributes above.
+    raw:
+        Raw data, stored with channel calibration data  Stored under
+        /Raw/Channel_*/Signal
+    events:
+        Minknow event data  Stored under
+        /IntermediateData/Channel_*/Events
+    reads:
+        Minknow read data  Stored under
+        /IntermediateData/Channel_*/Reads
+    multiplex:
+        Device multiplex data  Stored under
+        /MultiplexData/Channel_*/Multiplex
+    channel_states:
+        Channel state data  Stored under /StateData/Channel_*/States
+    device_metadata:
+        Device metadata (bias and temperature information)  Stored in
+        a per frame sequence in /Device/MetaData
+    device_commands:
+        Device commands  Stored with the frame commands take effect
+        sequence in /Device/AsicCommands
+    dynamic_analysis_config:
+        Dynamic analysis configuration  Stored with the frame config
+        took effect in /Meta/User/DynamicAnalysisConfiguration
+"""
+ReadDetectionParams.__doc__ = """Attributes:
+    open_pore_min:
+        The minimum level which is considered open pore (this value is
+        relative to open_pore_default or the tracked open_pore
+        section, if tracking is being used.)  This value must be <=
+        0.0 if tracking is being used.
+    open_pore_max:
+        The maximum level which is considered open pore (this value is
+        relative to open_pore_default or the tracked open_pore
+        section, if tracking is being used.)  This value must be >=
+        0.0 if tracking is being used.
+    open_pore_default:
+        The default value to use for open pore, either when tracking
+        isn't being used, or when open pore tracking has no value
+        currently.
+    open_pore_seconds_required:
+        Minimum number of seconds events must lie within the range of
+        open pore in order to allow a read to break.
+"""
+GetChannelStatesDescResponse.Style.__doc__ = """Attributes:
+    label:
+        The human-readable name to display when rendering this channel
+        state or group.
+    description:
+        A sentence describing the meaning of the channel state or
+        group.  This can be used as a tooltip, for example.
+    colour:
+        The colour to use when rendering this channel state or group.
+        This is a six-digit hex string describing an RGB colour (eg:
+        "ff00ff" for purple).
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/analysis_configuration_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/analysis_configuration_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/analysis_configuration_service.py` & `minknow_api-5.5.2/minknow_api/analysis_configuration_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/basecaller_pb2.py` & `minknow_api-5.5.2/minknow_api/basecaller_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: minknow_api/basecaller.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
@@ -18,625 +16,16 @@
 from minknow_api import analysis_configuration_pb2 as minknow__api_dot_analysis__configuration__pb2
 from minknow_api import protocol_settings_pb2 as minknow__api_dot_protocol__settings__pb2
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cminknow_api/basecaller.proto\x12\x16minknow_api.basecaller\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a(minknow_api/analysis_configuration.proto\x1a#minknow_api/protocol_settings.proto\x1a\x1dminknow_api/rpc_options.proto\"\x19\n\x17ListConfigsByKitRequest\"\xf4\x03\n\x18ListConfigsByKitResponse\x12`\n\x11\x66low_cell_configs\x18\x01 \x03(\x0b\x32\x45.minknow_api.basecaller.ListConfigsByKitResponse.FlowCellConfigsEntry\x1a\x1d\n\nConfigList\x12\x0f\n\x07\x63onfigs\x18\x01 \x03(\t\x1a\xe0\x01\n\x0bPerFlowCell\x12\x61\n\x0bkit_configs\x18\x01 \x03(\x0b\x32L.minknow_api.basecaller.ListConfigsByKitResponse.PerFlowCell.KitConfigsEntry\x1an\n\x0fKitConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12J\n\x05value\x18\x02 \x01(\x0b\x32;.minknow_api.basecaller.ListConfigsByKitResponse.ConfigList:\x02\x38\x01\x1at\n\x14\x46lowCellConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12K\n\x05value\x18\x02 \x01(\x0b\x32<.minknow_api.basecaller.ListConfigsByKitResponse.PerFlowCell:\x02\x38\x01\"\xed\x03\n\x17StartBasecallingRequest\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x1f\n\x17input_reads_directories\x18\x01 \x03(\t\x12\x1e\n\x16output_reads_directory\x18\x02 \x01(\t\x12\x15\n\rconfiguration\x18\x03 \x01(\t\x12\x11\n\tfast5_out\x18\x04 \x01(\x08\x12\x16\n\x0e\x63ompress_fastq\x18\x05 \x01(\x08\x12\x16\n\x0e\x64isable_events\x18\x06 \x01(\x08\x12\x11\n\trecursive\x18\x07 \x01(\x08\x12[\n\x17\x62\x61rcoding_configuration\x18\n \x01(\x0b\x32:.minknow_api.analysis_configuration.BarcodingConfiguration\x12[\n\x17\x61lignment_configuration\x18\x0b \x01(\x0b\x32:.minknow_api.analysis_configuration.AlignmentConfiguration\x12\x1d\n\x15\x65nable_read_splitting\x18\r \x01(\x08\x12=\n\x18min_score_read_splitting\x18\x0e \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"&\n\x18StartBasecallingResponse\x12\n\n\x02id\x18\x01 \x01(\t\"\xee\x01\n\x15StartBarcodingRequest\x12\x0c\n\x04name\x18\x0b \x01(\t\x12\x1f\n\x17input_reads_directories\x18\x01 \x03(\t\x12\x1e\n\x16output_reads_directory\x18\x02 \x01(\t\x12\x16\n\x0e\x63ompress_fastq\x18\x04 \x01(\x08\x12\x11\n\trecursive\x18\x05 \x01(\x08\x12[\n\x17\x62\x61rcoding_configuration\x18\n \x01(\x0b\x32:.minknow_api.analysis_configuration.BarcodingConfiguration\"$\n\x16StartBarcodingResponse\x12\n\n\x02id\x18\x01 \x01(\t\"\xd6\x01\n\x15StartAlignmentRequest\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x1f\n\x17input_reads_directories\x18\x01 \x03(\t\x12\x1e\n\x16output_reads_directory\x18\x02 \x01(\t\x12\x11\n\trecursive\x18\x04 \x01(\x08\x12[\n\x17\x61lignment_configuration\x18\x06 \x01(\x0b\x32:.minknow_api.analysis_configuration.AlignmentConfiguration\"$\n\x16StartAlignmentResponse\x12\n\n\x02id\x18\x01 \x01(\t\"\xce\x03\n\"StartPostProcessingProtocolRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\"\n\x1asequencing_protocol_run_id\x18\x07 \x01(\t\x12\x1d\n\x15input_fast5_directory\x18\x02 \x01(\t\x12\x1d\n\x15input_fastq_directory\x18\x03 \x01(\t\x12\x1b\n\x13input_bam_directory\x18\x04 \x01(\t\x12\x19\n\x11sample_sheet_path\x18\x08 \x01(\t\x12\x18\n\x10output_directory\x18\x05 \x01(\t\x12\x65\n\x0esetting_values\x18\x06 \x03(\x0b\x32M.minknow_api.basecaller.StartPostProcessingProtocolRequest.SettingValuesEntry\x1ay\n\x12SettingValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12R\n\x05value\x18\x02 \x01(\x0b\x32\x43.minknow_api.protocol_settings.ProtocolSetting.ProtocolSettingValue:\x02\x38\x01\"\x87\x03\n\x0cStartRequest\x12T\n\x19start_basecalling_request\x18\x02 \x01(\x0b\x32/.minknow_api.basecaller.StartBasecallingRequestH\x00\x12P\n\x17start_barcoding_request\x18\x03 \x01(\x0b\x32-.minknow_api.basecaller.StartBarcodingRequestH\x00\x12P\n\x17start_alignment_request\x18\x04 \x01(\x0b\x32-.minknow_api.basecaller.StartAlignmentRequestH\x00\x12l\n&start_post_processing_protocol_request\x18\x05 \x01(\x0b\x32:.minknow_api.basecaller.StartPostProcessingProtocolRequestH\x00\x42\x0f\n\rstart_request\"1\n#StartPostProcessingProtocolResponse\x12\n\n\x02id\x18\x01 \x01(\t\"\x1b\n\rCancelRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x10\n\x0e\x43\x61ncelResponse\"\xb4\x05\n\x07RunInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12T\n\x19start_basecalling_request\x18\x02 \x01(\x0b\x32/.minknow_api.basecaller.StartBasecallingRequestH\x00\x12P\n\x17start_barcoding_request\x18\x0b \x01(\x0b\x32-.minknow_api.basecaller.StartBarcodingRequestH\x00\x12P\n\x17start_alignment_request\x18\x0c \x01(\x0b\x32-.minknow_api.basecaller.StartAlignmentRequestH\x00\x12l\n&start_post_processing_protocol_request\x18\r \x01(\x0b\x32:.minknow_api.basecaller.StartPostProcessingProtocolRequestH\x00\x12,\n\x05state\x18\x03 \x01(\x0e\x32\x1d.minknow_api.basecaller.State\x12\x0e\n\x06\x65rrors\x18\x04 \x03(\t\x12\x18\n\x10\x66iles_discovered\x18\x05 \x01(\x05\x12\x18\n\x10progress_current\x18\x06 \x01(\x05\x12\x16\n\x0eprogress_total\x18\x07 \x01(\x05\x12.\n\nstart_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12\x65stimated_end_time\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x15\n\x13start_request_oneof\"\xbc\x01\n\x0eGetInfoRequest\x12\x39\n\x06preset\x18\x01 \x01(\x0e\x32\'.minknow_api.basecaller.SelectionPresetH\x00\x12\x0c\n\x02id\x18\x02 \x01(\tH\x00\x12=\n\x04list\x18\x03 \x01(\x0b\x32-.minknow_api.basecaller.GetInfoRequest.IdListH\x00\x1a\x15\n\x06IdList\x12\x0b\n\x03ids\x18\x01 \x03(\tB\x0b\n\tselection\"@\n\x0fGetInfoResponse\x12-\n\x04runs\x18\x01 \x03(\x0b\x32\x1f.minknow_api.basecaller.RunInfo\"*\n\x0cWatchRequest\x12\x1a\n\x12send_finished_runs\x18\x01 \x01(\x08\">\n\rWatchResponse\x12-\n\x04runs\x18\x01 \x03(\x0b\x32\x1f.minknow_api.basecaller.RunInfo\"^\n\x19MakeAlignmentIndexRequest\x12!\n\x19input_alignment_reference\x18\x01 \x01(\t\x12\x1e\n\x16output_alignment_index\x18\x02 \x01(\t\"\x1c\n\x1aMakeAlignmentIndexResponse\"$\n\"ListPostProcessingProtocolsRequest\"\xa6\x01\n\x1aPostProcessingProtocolInfo\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12@\n\x08provider\x18\x05 \x01(\x0e\x32..minknow_api.basecaller.PostProcessingProvider\"l\n#ListPostProcessingProtocolsResponse\x12\x45\n\tprotocols\x18\x01 \x03(\x0b\x32\x32.minknow_api.basecaller.PostProcessingProtocolInfo\"B\n,ListSettingsForPostProcessingProtocolRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\"\xd2\x01\n-ListSettingsForPostProcessingProtocolResponse\x12\x1c\n\x14requires_fast5_input\x18\x01 \x01(\x08\x12\x1c\n\x14requires_fastq_input\x18\x02 \x01(\x08\x12\x1a\n\x12requires_bam_input\x18\x03 \x01(\x08\x12I\n\x11protocol_settings\x18\x04 \x03(\x0b\x32..minknow_api.protocol_settings.ProtocolSetting\"5\n\x15UpdateProgressRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08progress\x18\x02 \x01(\x02\"\x18\n\x16UpdateProgressResponse\"*\n\x0fSendPingRequest\x12\x17\n\tping_data\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"\x12\n\x10SendPingResponse*S\n\x05State\x12\x11\n\rSTATE_RUNNING\x10\x00\x12\x11\n\rSTATE_SUCCESS\x10\x01\x12\x0f\n\x0bSTATE_ERROR\x10\x02\x12\x13\n\x0fSTATE_CANCELLED\x10\x03*[\n\x0fSelectionPreset\x12\x16\n\x12PRESET_ALL_RUNNING\x10\x00\x12 \n\x1cPRESET_MOST_RECENTLY_STARTED\x10\x01\x12\x0e\n\nPRESET_ALL\x10\x02*0\n\x16PostProcessingProvider\x12\n\n\x06SCRIPT\x10\x00\x12\n\n\x06\x45PI2ME\x10\x01\x32\xfd\x0c\n\nBasecaller\x12}\n\x13list_configs_by_kit\x12/.minknow_api.basecaller.ListConfigsByKitRequest\x1a\x30.minknow_api.basecaller.ListConfigsByKitResponse\"\x03\x90\x02\x01\x12x\n\x11start_basecalling\x12/.minknow_api.basecaller.StartBasecallingRequest\x1a\x30.minknow_api.basecaller.StartBasecallingResponse\"\x00\x12r\n\x0fstart_barcoding\x12-.minknow_api.basecaller.StartBarcodingRequest\x1a..minknow_api.basecaller.StartBarcodingResponse\"\x00\x12\x9b\x01\n\x1estart_post_processing_protocol\x12:.minknow_api.basecaller.StartPostProcessingProtocolRequest\x1a;.minknow_api.basecaller.StartPostProcessingProtocolResponse\"\x00\x12r\n\x0fstart_alignment\x12-.minknow_api.basecaller.StartAlignmentRequest\x1a..minknow_api.basecaller.StartAlignmentResponse\"\x00\x12\\\n\x06\x63\x61ncel\x12%.minknow_api.basecaller.CancelRequest\x1a&.minknow_api.basecaller.CancelResponse\"\x03\x90\x02\x02\x12\x62\n\x08get_info\x12&.minknow_api.basecaller.GetInfoRequest\x1a\'.minknow_api.basecaller.GetInfoResponse\"\x03\x90\x02\x01\x30\x01\x12[\n\x05watch\x12$.minknow_api.basecaller.WatchRequest\x1a%.minknow_api.basecaller.WatchResponse\"\x03\x90\x02\x01\x30\x01\x12\x7f\n\x14make_alignment_index\x12\x31.minknow_api.basecaller.MakeAlignmentIndexRequest\x1a\x32.minknow_api.basecaller.MakeAlignmentIndexResponse\"\x00\x12\x9e\x01\n\x1elist_post_processing_protocols\x12:.minknow_api.basecaller.ListPostProcessingProtocolsRequest\x1a;.minknow_api.basecaller.ListPostProcessingProtocolsResponse\"\x03\x90\x02\x02\x12\xbe\x01\n*list_settings_for_post_processing_protocol\x12\x44.minknow_api.basecaller.ListSettingsForPostProcessingProtocolRequest\x1a\x45.minknow_api.basecaller.ListSettingsForPostProcessingProtocolResponse\"\x03\x90\x02\x01\x12\x8b\x01\n(update_post_processing_protocol_progress\x12-.minknow_api.basecaller.UpdateProgressRequest\x1a..minknow_api.basecaller.UpdateProgressResponse\"\x00\x12`\n\tsend_ping\x12\'.minknow_api.basecaller.SendPingRequest\x1a(.minknow_api.basecaller.SendPingResponse\"\x00\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-_STATE = DESCRIPTOR.enum_types_by_name['State']
-State = enum_type_wrapper.EnumTypeWrapper(_STATE)
-_SELECTIONPRESET = DESCRIPTOR.enum_types_by_name['SelectionPreset']
-SelectionPreset = enum_type_wrapper.EnumTypeWrapper(_SELECTIONPRESET)
-_POSTPROCESSINGPROVIDER = DESCRIPTOR.enum_types_by_name['PostProcessingProvider']
-PostProcessingProvider = enum_type_wrapper.EnumTypeWrapper(_POSTPROCESSINGPROVIDER)
-STATE_RUNNING = 0
-STATE_SUCCESS = 1
-STATE_ERROR = 2
-STATE_CANCELLED = 3
-PRESET_ALL_RUNNING = 0
-PRESET_MOST_RECENTLY_STARTED = 1
-PRESET_ALL = 2
-SCRIPT = 0
-EPI2ME = 1
-
-
-_LISTCONFIGSBYKITREQUEST = DESCRIPTOR.message_types_by_name['ListConfigsByKitRequest']
-_LISTCONFIGSBYKITRESPONSE = DESCRIPTOR.message_types_by_name['ListConfigsByKitResponse']
-_LISTCONFIGSBYKITRESPONSE_CONFIGLIST = _LISTCONFIGSBYKITRESPONSE.nested_types_by_name['ConfigList']
-_LISTCONFIGSBYKITRESPONSE_PERFLOWCELL = _LISTCONFIGSBYKITRESPONSE.nested_types_by_name['PerFlowCell']
-_LISTCONFIGSBYKITRESPONSE_PERFLOWCELL_KITCONFIGSENTRY = _LISTCONFIGSBYKITRESPONSE_PERFLOWCELL.nested_types_by_name['KitConfigsEntry']
-_LISTCONFIGSBYKITRESPONSE_FLOWCELLCONFIGSENTRY = _LISTCONFIGSBYKITRESPONSE.nested_types_by_name['FlowCellConfigsEntry']
-_STARTBASECALLINGREQUEST = DESCRIPTOR.message_types_by_name['StartBasecallingRequest']
-_STARTBASECALLINGRESPONSE = DESCRIPTOR.message_types_by_name['StartBasecallingResponse']
-_STARTBARCODINGREQUEST = DESCRIPTOR.message_types_by_name['StartBarcodingRequest']
-_STARTBARCODINGRESPONSE = DESCRIPTOR.message_types_by_name['StartBarcodingResponse']
-_STARTALIGNMENTREQUEST = DESCRIPTOR.message_types_by_name['StartAlignmentRequest']
-_STARTALIGNMENTRESPONSE = DESCRIPTOR.message_types_by_name['StartAlignmentResponse']
-_STARTPOSTPROCESSINGPROTOCOLREQUEST = DESCRIPTOR.message_types_by_name['StartPostProcessingProtocolRequest']
-_STARTPOSTPROCESSINGPROTOCOLREQUEST_SETTINGVALUESENTRY = _STARTPOSTPROCESSINGPROTOCOLREQUEST.nested_types_by_name['SettingValuesEntry']
-_STARTREQUEST = DESCRIPTOR.message_types_by_name['StartRequest']
-_STARTPOSTPROCESSINGPROTOCOLRESPONSE = DESCRIPTOR.message_types_by_name['StartPostProcessingProtocolResponse']
-_CANCELREQUEST = DESCRIPTOR.message_types_by_name['CancelRequest']
-_CANCELRESPONSE = DESCRIPTOR.message_types_by_name['CancelResponse']
-_RUNINFO = DESCRIPTOR.message_types_by_name['RunInfo']
-_GETINFOREQUEST = DESCRIPTOR.message_types_by_name['GetInfoRequest']
-_GETINFOREQUEST_IDLIST = _GETINFOREQUEST.nested_types_by_name['IdList']
-_GETINFORESPONSE = DESCRIPTOR.message_types_by_name['GetInfoResponse']
-_WATCHREQUEST = DESCRIPTOR.message_types_by_name['WatchRequest']
-_WATCHRESPONSE = DESCRIPTOR.message_types_by_name['WatchResponse']
-_MAKEALIGNMENTINDEXREQUEST = DESCRIPTOR.message_types_by_name['MakeAlignmentIndexRequest']
-_MAKEALIGNMENTINDEXRESPONSE = DESCRIPTOR.message_types_by_name['MakeAlignmentIndexResponse']
-_LISTPOSTPROCESSINGPROTOCOLSREQUEST = DESCRIPTOR.message_types_by_name['ListPostProcessingProtocolsRequest']
-_POSTPROCESSINGPROTOCOLINFO = DESCRIPTOR.message_types_by_name['PostProcessingProtocolInfo']
-_LISTPOSTPROCESSINGPROTOCOLSRESPONSE = DESCRIPTOR.message_types_by_name['ListPostProcessingProtocolsResponse']
-_LISTSETTINGSFORPOSTPROCESSINGPROTOCOLREQUEST = DESCRIPTOR.message_types_by_name['ListSettingsForPostProcessingProtocolRequest']
-_LISTSETTINGSFORPOSTPROCESSINGPROTOCOLRESPONSE = DESCRIPTOR.message_types_by_name['ListSettingsForPostProcessingProtocolResponse']
-_UPDATEPROGRESSREQUEST = DESCRIPTOR.message_types_by_name['UpdateProgressRequest']
-_UPDATEPROGRESSRESPONSE = DESCRIPTOR.message_types_by_name['UpdateProgressResponse']
-_SENDPINGREQUEST = DESCRIPTOR.message_types_by_name['SendPingRequest']
-_SENDPINGRESPONSE = DESCRIPTOR.message_types_by_name['SendPingResponse']
-ListConfigsByKitRequest = _reflection.GeneratedProtocolMessageType('ListConfigsByKitRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTCONFIGSBYKITREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListConfigsByKitRequest)
-  })
-_sym_db.RegisterMessage(ListConfigsByKitRequest)
-
-ListConfigsByKitResponse = _reflection.GeneratedProtocolMessageType('ListConfigsByKitResponse', (_message.Message,), {
-
-  'ConfigList' : _reflection.GeneratedProtocolMessageType('ConfigList', (_message.Message,), {
-    'DESCRIPTOR' : _LISTCONFIGSBYKITRESPONSE_CONFIGLIST,
-    '__module__' : 'minknow_api.basecaller_pb2'
-    ,
-    '__doc__': """Attributes:
-        configs:
-            List of configuration names, to be used in
-            ``StartBasecallingRequest.configuration``
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListConfigsByKitResponse.ConfigList)
-    })
-  ,
-
-  'PerFlowCell' : _reflection.GeneratedProtocolMessageType('PerFlowCell', (_message.Message,), {
-
-    'KitConfigsEntry' : _reflection.GeneratedProtocolMessageType('KitConfigsEntry', (_message.Message,), {
-      'DESCRIPTOR' : _LISTCONFIGSBYKITRESPONSE_PERFLOWCELL_KITCONFIGSENTRY,
-      '__module__' : 'minknow_api.basecaller_pb2'
-      # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListConfigsByKitResponse.PerFlowCell.KitConfigsEntry)
-      })
-    ,
-    'DESCRIPTOR' : _LISTCONFIGSBYKITRESPONSE_PERFLOWCELL,
-    '__module__' : 'minknow_api.basecaller_pb2'
-    ,
-    '__doc__': """Attributes:
-        kit_configs:
-            Key: kit name (eg: "SQK-LSK109") Value: list of configuration
-            names
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListConfigsByKitResponse.PerFlowCell)
-    })
-  ,
-
-  'FlowCellConfigsEntry' : _reflection.GeneratedProtocolMessageType('FlowCellConfigsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _LISTCONFIGSBYKITRESPONSE_FLOWCELLCONFIGSENTRY,
-    '__module__' : 'minknow_api.basecaller_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListConfigsByKitResponse.FlowCellConfigsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _LISTCONFIGSBYKITRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      flow_cell_configs:
-          Key: flow cell type (eg: "FLO-MIN107") Value: FlowCellConfigs
-          describing configurations available for that flow cell.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListConfigsByKitResponse)
-  })
-_sym_db.RegisterMessage(ListConfigsByKitResponse)
-_sym_db.RegisterMessage(ListConfigsByKitResponse.ConfigList)
-_sym_db.RegisterMessage(ListConfigsByKitResponse.PerFlowCell)
-_sym_db.RegisterMessage(ListConfigsByKitResponse.PerFlowCell.KitConfigsEntry)
-_sym_db.RegisterMessage(ListConfigsByKitResponse.FlowCellConfigsEntry)
-
-StartBasecallingRequest = _reflection.GeneratedProtocolMessageType('StartBasecallingRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STARTBASECALLINGREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      name:
-          User specified name to identify the basecall run.
-      input_reads_directories:
-          Input directories to search for reads to be basecalled.
-          Currently, only one directory can be specified, but this
-          definition allows for multiple in the future without breaking
-          compatibility.
-      output_reads_directory:
-          Output directory where called reads will be placed.  Reads
-          will be sorted into subdirectories based on the sequencing run
-          they came from.
-      configuration:
-          The name of the basecalling configuration to use.
-      fast5_out:
-          Enable output of .fast5 files containing original raw reads,
-          event data/trace table from basecall and basecall result
-          sequence.  This causes .fast5 files to be output in addition
-          to FASTQ files.  DEPRECATED: This option does not have any
-          effect - the basecaller no longer has the ability to write
-          fast5 files.
-      compress_fastq:
-          Enable gzip compression of output FASTQ files.
-      disable_events:
-          Prevent events / trace tables being written to .fast5 files.
-          If event tables are not required for downstream processing
-          (eg: for 1d^2) then it is more efficient (and produces smaller
-          files) to disable them.  This has no effect if ``fast5_out``
-          is not enabled.
-      recursive:
-          Recursively find fast5 files to basecall in the
-          `input_reads_directories`.  If False, only the fast5 files
-          directly in one of the `input_reads_directories` will be
-          basecalled. If True, subdirectories of those directories will
-          also be searched recursively.
-      barcoding_configuration:
-          Options to control barcoding performed once basecalling reads
-          is complete.
-      alignment_configuration:
-          Options to control alignment performed once basecalling reads
-          is complete.
-      enable_read_splitting:
-          Enable read splitting in guppy
-      min_score_read_splitting:
-          Override score to use for guppy read splitting. If not
-          specified a default value is used from guppy.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartBasecallingRequest)
-  })
-_sym_db.RegisterMessage(StartBasecallingRequest)
-
-StartBasecallingResponse = _reflection.GeneratedProtocolMessageType('StartBasecallingResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STARTBASECALLINGRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      id:
-          An identifier for the basecalling run that was started. This
-          can be used to monitor or cancel the run.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartBasecallingResponse)
-  })
-_sym_db.RegisterMessage(StartBasecallingResponse)
-
-StartBarcodingRequest = _reflection.GeneratedProtocolMessageType('StartBarcodingRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STARTBARCODINGREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      name:
-          User specified name to identify the barcoding run.
-      input_reads_directories:
-          Input directories to search for reads to be basecalled.
-          Currently, only one directory can be specified, but this
-          definition allows for multiple in the future without breaking
-          compatibility.
-      output_reads_directory:
-          Output directory where called reads will be placed.  Reads
-          will be sorted into subdirectories based on the sequencing run
-          they came from.
-      compress_fastq:
-          Enable gzip compression of output FASTQ files.
-      recursive:
-          Recursively find fast5 files to basecall in the
-          `input_reads_directories`.  If False, only the fast5 files
-          directly in one of the `input_reads_directories` will be
-          basecalled. If True, subdirectories of those directories will
-          also be searched recursively.
-      barcoding_configuration:
-          Options to control barcoding performed once basecalling reads
-          is complete.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartBarcodingRequest)
-  })
-_sym_db.RegisterMessage(StartBarcodingRequest)
-
-StartBarcodingResponse = _reflection.GeneratedProtocolMessageType('StartBarcodingResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STARTBARCODINGRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      id:
-          An identifier for the basecalling run that was started. This
-          can be used to monitor or cancel the run.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartBarcodingResponse)
-  })
-_sym_db.RegisterMessage(StartBarcodingResponse)
-
-StartAlignmentRequest = _reflection.GeneratedProtocolMessageType('StartAlignmentRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STARTALIGNMENTREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      name:
-          User specified name to identify the alignment run.
-      input_reads_directories:
-          Input directories to search for reads to be aligned.
-          Currently, only one directory can be specified, but this
-          definition allows for multiple in the future without breaking
-          compatibility.
-      output_reads_directory:
-          Output directory where aligned reads will be placed.
-      recursive:
-          Recursively find fast5 files to align in the
-          `input_reads_directories`.  If False, only the fast5 files
-          directly in one of the `input_reads_directories` will be
-          aligned. If True, subdirectories of those directories will
-          also be searched recursively.
-      alignment_configuration:
-          Options to control alignment performed once basecalling reads
-          is complete.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartAlignmentRequest)
-  })
-_sym_db.RegisterMessage(StartAlignmentRequest)
-
-StartAlignmentResponse = _reflection.GeneratedProtocolMessageType('StartAlignmentResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STARTALIGNMENTRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      id:
-          An identifier for the alignment run that was started. This can
-          be used to monitor or cancel the run.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartAlignmentResponse)
-  })
-_sym_db.RegisterMessage(StartAlignmentResponse)
-
-StartPostProcessingProtocolRequest = _reflection.GeneratedProtocolMessageType('StartPostProcessingProtocolRequest', (_message.Message,), {
-
-  'SettingValuesEntry' : _reflection.GeneratedProtocolMessageType('SettingValuesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _STARTPOSTPROCESSINGPROTOCOLREQUEST_SETTINGVALUESENTRY,
-    '__module__' : 'minknow_api.basecaller_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartPostProcessingProtocolRequest.SettingValuesEntry)
-    })
-  ,
-  'DESCRIPTOR' : _STARTPOSTPROCESSINGPROTOCOLREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      identifier:
-          identifier value from a protocol returned from
-          list_post_processing_protocols.
-      sequencing_protocol_run_id:
-          Optionally specify a sequencing protocol that is linked with
-          this analysis.
-      input_fast5_directory:
-          Input directories for the protocol (omit those which the
-          protocol doesn't require).
-      sample_sheet_path:
-          Path to the sample sheet output by minknow
-      output_directory:
-          Output directory where the analysed output should be written.
-      setting_values:
-          Configured values for display settings for the protocol (see
-          basecaller.list_settings_for_protocol) keys missing from the
-          original protocol will cause errors.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartPostProcessingProtocolRequest)
-  })
-_sym_db.RegisterMessage(StartPostProcessingProtocolRequest)
-_sym_db.RegisterMessage(StartPostProcessingProtocolRequest.SettingValuesEntry)
-
-StartRequest = _reflection.GeneratedProtocolMessageType('StartRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STARTREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      start_request:
-          Start request that will be used to trigger analysis, used to
-          union over all the different types of analysis possible.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartRequest)
-  })
-_sym_db.RegisterMessage(StartRequest)
-
-StartPostProcessingProtocolResponse = _reflection.GeneratedProtocolMessageType('StartPostProcessingProtocolResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STARTPOSTPROCESSINGPROTOCOLRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      id:
-          An identifier for the protocol run that was started. This can
-          be used to monitor or cancel the run.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.StartPostProcessingProtocolResponse)
-  })
-_sym_db.RegisterMessage(StartPostProcessingProtocolResponse)
-
-CancelRequest = _reflection.GeneratedProtocolMessageType('CancelRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CANCELREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      id:
-          An identifier as returned from a call to start() or list().
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.CancelRequest)
-  })
-_sym_db.RegisterMessage(CancelRequest)
-
-CancelResponse = _reflection.GeneratedProtocolMessageType('CancelResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CANCELRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.CancelResponse)
-  })
-_sym_db.RegisterMessage(CancelResponse)
-
-RunInfo = _reflection.GeneratedProtocolMessageType('RunInfo', (_message.Message,), {
-  'DESCRIPTOR' : _RUNINFO,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      id:
-          The ID of the run, as returned by start().
-      start_request_oneof:
-          The original message used to start the run.
-      start_basecalling_request:
-          Set if basecalling reads
-      start_barcoding_request:
-          Set if barcoding reads
-      start_alignment_request:
-          Set if aligning reads
-      start_post_processing_protocol_request:
-          Set if aligning reads
-      state:
-          What state the run is in.  While the basecalling is running
-          the state field will be ``STATE_RUNNING``.
-      errors:
-          If state is STATE_ERROR, this will contain (some of) the
-          errors encountered.  Note that if there are a lot of errors,
-          only some may be returned.
-      files_discovered:
-          The number of files selected for input.
-      progress_current:
-          The current basecalling progress (with respect to
-          progress_total).  This is intended to be an estimate of how
-          close to completion the basecalling run is. The numbers have
-          no particular meaning other than as a proportion of
-          progress_total.  Note that this only really has useful meaning
-          while state is STATE_RUNNING. On STATE_SUCCESS, it will always
-          be the same as progress_total. On STATE_ERROR or
-          STATE_CANCELLED, it may give some indication of how far
-          through basecalling was when it failed or was cancelled.
-      progress_total:
-          The maximum value of progress_current.  (progress_current /
-          progress_total) * 100 will give a percentage completion.  If
-          this is 0, it should be interpreted as "unknown progress".
-      start_time:
-          When basecalling was started (UTC).
-      end_time:
-          When basecalling ended (UTC).  Unset if basecalling is still
-          running.
-      estimated_end_time:
-          An estimate for when basecalling will end (UTC).  Unset if
-          basecalling has finished, or if an estimate cannot be
-          calculated (eg: because the baescalling software does not
-          support it).  Since 3.6.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.RunInfo)
-  })
-_sym_db.RegisterMessage(RunInfo)
-
-GetInfoRequest = _reflection.GeneratedProtocolMessageType('GetInfoRequest', (_message.Message,), {
-
-  'IdList' : _reflection.GeneratedProtocolMessageType('IdList', (_message.Message,), {
-    'DESCRIPTOR' : _GETINFOREQUEST_IDLIST,
-    '__module__' : 'minknow_api.basecaller_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.basecaller.GetInfoRequest.IdList)
-    })
-  ,
-  'DESCRIPTOR' : _GETINFOREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      selection:
-          The selection of runs to return information about.  If no
-          selection is provided, the call will return all currently-
-          running basecall runs (as though PRESET_ALL_RUNNING were
-          selected).
-      preset:
-          A pre-determined selection of runs.
-      id:
-          An identifier, as returned by start().
-      list:
-          A list of identifiers, as returned by start().
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.GetInfoRequest)
-  })
-_sym_db.RegisterMessage(GetInfoRequest)
-_sym_db.RegisterMessage(GetInfoRequest.IdList)
-
-GetInfoResponse = _reflection.GeneratedProtocolMessageType('GetInfoResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETINFORESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      runs:
-          Information about the requested runs.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.GetInfoResponse)
-  })
-_sym_db.RegisterMessage(GetInfoResponse)
-
-WatchRequest = _reflection.GeneratedProtocolMessageType('WatchRequest', (_message.Message,), {
-  'DESCRIPTOR' : _WATCHREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      send_finished_runs:
-          By default, no information will be sent about runs that were
-          already finished when this call was made. Setting this to true
-          will cause the state of already-finished runs to be returned.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.WatchRequest)
-  })
-_sym_db.RegisterMessage(WatchRequest)
-
-WatchResponse = _reflection.GeneratedProtocolMessageType('WatchResponse', (_message.Message,), {
-  'DESCRIPTOR' : _WATCHRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      runs:
-          The current state of some of the runs.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.WatchResponse)
-  })
-_sym_db.RegisterMessage(WatchResponse)
-
-MakeAlignmentIndexRequest = _reflection.GeneratedProtocolMessageType('MakeAlignmentIndexRequest', (_message.Message,), {
-  'DESCRIPTOR' : _MAKEALIGNMENTINDEXREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      input_alignment_reference:
-          Input fasta reference to use for building the index.
-      output_alignment_index:
-          Output file path to write index (mmi file) to.  Must have a
-          ".mmi" extension, and the paths parent directory must exist.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.MakeAlignmentIndexRequest)
-  })
-_sym_db.RegisterMessage(MakeAlignmentIndexRequest)
-
-MakeAlignmentIndexResponse = _reflection.GeneratedProtocolMessageType('MakeAlignmentIndexResponse', (_message.Message,), {
-  'DESCRIPTOR' : _MAKEALIGNMENTINDEXRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.MakeAlignmentIndexResponse)
-  })
-_sym_db.RegisterMessage(MakeAlignmentIndexResponse)
-
-ListPostProcessingProtocolsRequest = _reflection.GeneratedProtocolMessageType('ListPostProcessingProtocolsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTPOSTPROCESSINGPROTOCOLSREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListPostProcessingProtocolsRequest)
-  })
-_sym_db.RegisterMessage(ListPostProcessingProtocolsRequest)
-
-PostProcessingProtocolInfo = _reflection.GeneratedProtocolMessageType('PostProcessingProtocolInfo', (_message.Message,), {
-  'DESCRIPTOR' : _POSTPROCESSINGPROTOCOLINFO,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      identifier:
-          System identifier for the protocol
-      name:
-          Readable name for the protocol (appropriate for use as a key
-          in translation database).  Note that this may not be unique:
-          in particular, the EPI2ME provider lists every version of a
-          workflow as a separate post-processing protocol.
-      version:
-          Protocol version.  This might not be set for all protocols or
-          all providers.
-      description:
-          A description of the protocol.
-      provider:
-          The source of the post-processing protocol.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.PostProcessingProtocolInfo)
-  })
-_sym_db.RegisterMessage(PostProcessingProtocolInfo)
-
-ListPostProcessingProtocolsResponse = _reflection.GeneratedProtocolMessageType('ListPostProcessingProtocolsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LISTPOSTPROCESSINGPROTOCOLSRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListPostProcessingProtocolsResponse)
-  })
-_sym_db.RegisterMessage(ListPostProcessingProtocolsResponse)
-
-ListSettingsForPostProcessingProtocolRequest = _reflection.GeneratedProtocolMessageType('ListSettingsForPostProcessingProtocolRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTSETTINGSFORPOSTPROCESSINGPROTOCOLREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      identifier:
-          specify the protocol with a string containing all the
-          protocol's identifying components, eg:
-          "SYSTEM:post_processing/artic"
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListSettingsForPostProcessingProtocolRequest)
-  })
-_sym_db.RegisterMessage(ListSettingsForPostProcessingProtocolRequest)
-
-ListSettingsForPostProcessingProtocolResponse = _reflection.GeneratedProtocolMessageType('ListSettingsForPostProcessingProtocolResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LISTSETTINGSFORPOSTPROCESSINGPROTOCOLRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      requires_fast5_input:
-          Does the protocol require fast5 files as input
-      requires_fastq_input:
-          Does the protocol require fastq files as input
-      requires_bam_input:
-          Does the protocol require bam files as input
-      protocol_settings:
-          List of protocol settings used by the post processing protocol
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.ListSettingsForPostProcessingProtocolResponse)
-  })
-_sym_db.RegisterMessage(ListSettingsForPostProcessingProtocolResponse)
-
-UpdateProgressRequest = _reflection.GeneratedProtocolMessageType('UpdateProgressRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATEPROGRESSREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Attributes:
-      id:
-          id of the protocol to update (stored in environment variable
-          for python process)
-      progress:
-          Progress indicator, 0-1.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.UpdateProgressRequest)
-  })
-_sym_db.RegisterMessage(UpdateProgressRequest)
-
-UpdateProgressResponse = _reflection.GeneratedProtocolMessageType('UpdateProgressResponse', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATEPROGRESSRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.UpdateProgressResponse)
-  })
-_sym_db.RegisterMessage(UpdateProgressResponse)
-
-SendPingRequest = _reflection.GeneratedProtocolMessageType('SendPingRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SENDPINGREQUEST,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Since 5.0
-  
-  Attributes:
-      ping_data:
-          The json data to send as a ping.  note: if this string is not
-          a valid json object, an error will be raised.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.SendPingRequest)
-  })
-_sym_db.RegisterMessage(SendPingRequest)
-
-SendPingResponse = _reflection.GeneratedProtocolMessageType('SendPingResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SENDPINGRESPONSE,
-  '__module__' : 'minknow_api.basecaller_pb2'
-  ,
-  '__doc__': """Since 5.0""",
-  # @@protoc_insertion_point(class_scope:minknow_api.basecaller.SendPingResponse)
-  })
-_sym_db.RegisterMessage(SendPingResponse)
-
-_BASECALLER = DESCRIPTOR.services_by_name['Basecaller']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.basecaller_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
   _LISTCONFIGSBYKITRESPONSE_PERFLOWCELL_KITCONFIGSENTRY._options = None
   _LISTCONFIGSBYKITRESPONSE_PERFLOWCELL_KITCONFIGSENTRY._serialized_options = b'8\001'
   _LISTCONFIGSBYKITRESPONSE_FLOWCELLCONFIGSENTRY._options = None
@@ -731,8 +120,372 @@
   _UPDATEPROGRESSRESPONSE._serialized_end=4651
   _SENDPINGREQUEST._serialized_start=4653
   _SENDPINGREQUEST._serialized_end=4695
   _SENDPINGRESPONSE._serialized_start=4697
   _SENDPINGRESPONSE._serialized_end=4715
   _BASECALLER._serialized_start=4946
   _BASECALLER._serialized_end=6607
+ListSettingsForPostProcessingProtocolRequest.__doc__ = """Attributes:
+    identifier:
+        specify the protocol with a string containing all the
+        protocol's identifying components, eg:
+        "SYSTEM:post_processing/artic"
+"""
+StartRequest.__doc__ = """ Protobuf messages for input/output of RPC calls
+
+Attributes:
+    dont_wait_for_device_ready:
+        Prevent waiting until the device is ready before starting
+        acquisition.  Defaults to false.  By default, MinKNOW will
+        block in the start() call for the device and flow cell to be
+        ready for acquisition (which may take several seconds after
+        plugging in the flow cell on some devices). Setting this
+        option will cause the call to return with an error if the
+        device is not already prepared to acquire data.  Since 1.14
+    generate_report:
+        Generate duty time and throughput reports.  Note that this
+        setting will be ignored (and no reports will be generated) if
+        no protocol is running at the time acquisition is started.
+        The default setting (AUTO) will only generate reports if
+        purpose is set to SEQUENCING.  Since 3.0
+    send_sequencing_read_metrics:
+        Whether sequencing read metrics should be reported to Oxford
+        Nanopore.  These are performance metrics that are used to
+        improve the sequencing technology. They do not include any
+        actual sequencing data, only statistics about read lengths,
+        duty time and similar generic performance information.  The
+        default setting (AUTO) will only send metrics if purpose is
+        set to SEQUENCING.  Since 3.0
+    send_basecalling_metrics:
+        Whether basecalling metrics should be reported to Oxford
+        Nanopore.  These are performance metrics that are used to
+        improve the sequencing technology. They do not include any
+        actual sequencing data, only statistics about basecalling
+        performance.  The default setting (AUTO) will only send
+        metrics if purpose is set to SEQUENCING.  NB: this setting is
+        ignored if live basecalling is not enabled, since there will
+        be no metrics to send.  Since 3.2
+    purpose:
+        Specify the purpose of this acquisition period.  This affects
+        various defaults (see the Purpose enum documentation for more
+        details). It may also affect how the user interface presents
+        the state of the protocol.  Since 3.2
+    analysis:
+        Perform analysis for this acquisition period.  If this is
+        disabled, no reads, no events, no channel states and no
+        basecalls will be generated. Any RPCs that depend on any of
+        these will fail. No reads-based files will be produced at all,
+        regardless of any other settings.  This is mostly useful for
+        calibration (although you should normally use the purpose
+        field rather than setting this explicitly).  The default
+        setting (AUTO) will use the persistent setting from the
+        analysis_configuraiton service, unless the purpose is set to
+        CALIBRATION.  Since 3.2
+    file_output:
+        Allow file output for this acquisition period.  If this is
+        disabled, the file output settings will be ignored for this
+        acquisition period, and no data files will be produced. Note
+        that reports are NOT managed by this setting.  Note that
+        setting this to FORCE will simply make file output respect the
+        bulk and read writer configurations. If each file output type
+        is disabled, you will still get no file output.  This is
+        mostly useful for calibration (although you should normally
+        use the purpose field rather than setting this explicitly).
+        The default setting (AUTO) will only suppress file output if
+        purpose is set to CALIBRATION.  Since 3.2
+    generate_final_summary:
+        Write a final_summary.txt file.  If file_output is disabled,
+        the final_summary.txt file will not be written regardless of
+        this setting.  The default setting (AUTO) will only enable
+        writing a final_summary.txt file if the purpose is set to
+        SEQUENCING.  Since 3.5 (NB: in 3.3 and 3.4, final_summary.txt
+        was always written out if file_output was enabled).
+    start_request:
+        Start request that will be used to trigger analysis, used to
+        union over all the different types of analysis possible.
+"""
+ListConfigsByKitResponse.PerFlowCell.__doc__ = """Attributes:
+    kit_configs:
+        Key: kit name (eg: "SQK-LSK109") Value: list of configuration
+        names
+"""
+ListSettingsForPostProcessingProtocolResponse.__doc__ = """Attributes:
+    requires_fast5_input:
+        Does the protocol require fast5 files as input
+    requires_fastq_input:
+        Does the protocol require fastq files as input
+    requires_bam_input:
+        Does the protocol require bam files as input
+    protocol_settings:
+        List of protocol settings used by the post processing protocol
+"""
+SendPingResponse.__doc__ = """Since 5.0"""
+GetInfoResponse.__doc__ = """Attributes:
+    runs:
+        Information about the requested runs.
+"""
+GetInfoRequest.__doc__ = """Attributes:
+    selection:
+        The selection of runs to return information about.  If no
+        selection is provided, the call will return all currently-
+        running basecall runs (as though PRESET_ALL_RUNNING were
+        selected).
+    preset:
+        A pre-determined selection of runs.
+    id:
+        An identifier, as returned by start().
+    list:
+        A list of identifiers, as returned by start().
+"""
+PostProcessingProtocolInfo.__doc__ = """Attributes:
+    identifier:
+        System identifier for the protocol
+    name:
+        Readable name for the protocol (appropriate for use as a key
+        in translation database).  Note that this may not be unique:
+        in particular, the EPI2ME provider lists every version of a
+        workflow as a separate post-processing protocol.
+    version:
+        Protocol version.  This might not be set for all protocols or
+        all providers.
+    description:
+        A description of the protocol.
+    provider:
+        The source of the post-processing protocol.
+"""
+MakeAlignmentIndexRequest.__doc__ = """Attributes:
+    input_alignment_reference:
+        Input fasta reference to use for building the index.
+    output_alignment_index:
+        Output file path to write index (mmi file) to.  Must have a
+        ".mmi" extension, and the paths parent directory must exist.
+"""
+StartBarcodingRequest.__doc__ = """Attributes:
+    name:
+        User specified name to identify the barcoding run.
+    input_reads_directories:
+        Input directories to search for reads to be basecalled.
+        Currently, only one directory can be specified, but this
+        definition allows for multiple in the future without breaking
+        compatibility.
+    output_reads_directory:
+        Output directory where called reads will be placed.  Reads
+        will be sorted into subdirectories based on the sequencing run
+        they came from.
+    compress_fastq:
+        Enable gzip compression of output FASTQ files.
+    recursive:
+        Recursively find fast5 files to basecall in the
+        `input_reads_directories`.  If False, only the fast5 files
+        directly in one of the `input_reads_directories` will be
+        basecalled. If True, subdirectories of those directories will
+        also be searched recursively.
+    barcoding_configuration:
+        Options to control barcoding performed once basecalling reads
+        is complete.
+"""
+StartBarcodingResponse.__doc__ = """Attributes:
+    id:
+        An identifier for the basecalling run that was started. This
+        can be used to monitor or cancel the run.
+"""
+UpdateProgressRequest.__doc__ = """Attributes:
+    id:
+        id of the protocol to update (stored in environment variable
+        for python process)
+    progress:
+        Progress indicator, 0-1.
+"""
+ListConfigsByKitResponse.__doc__ = """Attributes:
+    flow_cell_configs:
+        Key: flow cell type (eg: "FLO-MIN107") Value: FlowCellConfigs
+        describing configurations available for that flow cell.
+"""
+StartPostProcessingProtocolResponse.__doc__ = """Attributes:
+    id:
+        An identifier for the protocol run that was started. This can
+        be used to monitor or cancel the run.
+"""
+RunInfo.__doc__ = """Attributes:
+    id:
+        The ID of the run, as returned by start().
+    start_request_oneof:
+        The original message used to start the run.
+    start_basecalling_request:
+        Set if basecalling reads
+    start_barcoding_request:
+        Set if barcoding reads
+    start_alignment_request:
+        Set if aligning reads
+    start_post_processing_protocol_request:
+        Set if aligning reads
+    state:
+        What state the run is in.  While the basecalling is running
+        the state field will be ``STATE_RUNNING``.
+    errors:
+        If state is STATE_ERROR, this will contain (some of) the
+        errors encountered.  Note that if there are a lot of errors,
+        only some may be returned.
+    files_discovered:
+        The number of files selected for input.
+    progress_current:
+        The current basecalling progress (with respect to
+        progress_total).  This is intended to be an estimate of how
+        close to completion the basecalling run is. The numbers have
+        no particular meaning other than as a proportion of
+        progress_total.  Note that this only really has useful meaning
+        while state is STATE_RUNNING. On STATE_SUCCESS, it will always
+        be the same as progress_total. On STATE_ERROR or
+        STATE_CANCELLED, it may give some indication of how far
+        through basecalling was when it failed or was cancelled.
+    progress_total:
+        The maximum value of progress_current.  (progress_current /
+        progress_total) * 100 will give a percentage completion.  If
+        this is 0, it should be interpreted as "unknown progress".
+    start_time:
+        When basecalling was started (UTC).
+    end_time:
+        When basecalling ended (UTC).  Unset if basecalling is still
+        running.
+    estimated_end_time:
+        An estimate for when basecalling will end (UTC).  Unset if
+        basecalling has finished, or if an estimate cannot be
+        calculated (eg: because the baescalling software does not
+        support it).  Since 3.6.
+"""
+CancelRequest.__doc__ = """Attributes:
+    id:
+        An identifier as returned from a call to start() or list().
+"""
+StartBasecallingResponse.__doc__ = """Attributes:
+    id:
+        An identifier for the basecalling run that was started. This
+        can be used to monitor or cancel the run.
+"""
+StartPostProcessingProtocolRequest.__doc__ = """Attributes:
+    identifier:
+        identifier value from a protocol returned from
+        list_post_processing_protocols.
+    sequencing_protocol_run_id:
+        Optionally specify a sequencing protocol that is linked with
+        this analysis.
+    input_fast5_directory:
+        Input directories for the protocol (omit those which the
+        protocol doesn't require).
+    sample_sheet_path:
+        Path to the sample sheet output by minknow
+    output_directory:
+        Output directory where the analysed output should be written.
+    setting_values:
+        Configured values for display settings for the protocol (see
+        basecaller.list_settings_for_protocol) keys missing from the
+        original protocol will cause errors.
+"""
+ListConfigsByKitResponse.ConfigList.__doc__ = """Attributes:
+    configs:
+        List of configuration names, to be used in
+        ``StartBasecallingRequest.configuration``
+"""
+StartBasecallingRequest.__doc__ = """Attributes:
+    name:
+        User specified name to identify the basecall run.
+    input_reads_directories:
+        Input directories to search for reads to be basecalled.
+        Currently, only one directory can be specified, but this
+        definition allows for multiple in the future without breaking
+        compatibility.
+    output_reads_directory:
+        Output directory where called reads will be placed.  Reads
+        will be sorted into subdirectories based on the sequencing run
+        they came from.
+    configuration:
+        The name of the basecalling configuration to use.
+    fast5_out:
+        Enable output of .fast5 files containing original raw reads,
+        event data/trace table from basecall and basecall result
+        sequence.  This causes .fast5 files to be output in addition
+        to FASTQ files.  DEPRECATED: This option does not have any
+        effect - the basecaller no longer has the ability to write
+        fast5 files.
+    compress_fastq:
+        Enable gzip compression of output FASTQ files.
+    disable_events:
+        Prevent events / trace tables being written to .fast5 files.
+        If event tables are not required for downstream processing
+        (eg: for 1d^2) then it is more efficient (and produces smaller
+        files) to disable them.  This has no effect if ``fast5_out``
+        is not enabled.
+    recursive:
+        Recursively find fast5 files to basecall in the
+        `input_reads_directories`.  If False, only the fast5 files
+        directly in one of the `input_reads_directories` will be
+        basecalled. If True, subdirectories of those directories will
+        also be searched recursively.
+    barcoding_configuration:
+        Options to control barcoding performed once basecalling reads
+        is complete.
+    alignment_configuration:
+        Options to control alignment performed once basecalling reads
+        is complete.
+    enable_read_splitting:
+        Enable read splitting in guppy
+    min_score_read_splitting:
+        Override score to use for guppy read splitting. If not
+        specified a default value is used from guppy.
+"""
+WatchResponse.__doc__ = """Attributes:
+    runs:
+        The current state of some of the runs.
+    values:
+        The values that have changed.  The first received message will
+        contain the current state of all the watched values.
+        Subsequent messages will only contain the values that changed.
+    removed_values:
+        The values that have been removed.
+"""
+WatchRequest.__doc__ = """Attributes:
+    send_finished_runs:
+        By default, no information will be sent about runs that were
+        already finished when this call was made. Setting this to true
+        will cause the state of already-finished runs to be returned.
+    names:
+        The names of the values you wish to watch.
+    allow_missing:
+        Whether to allow missing values.  If set, names that are not
+        present in the store will be omitted from the first response,
+        but will still be watched. If and when they are added, a
+        message will be sent with the set values. Otherwise, missing
+        values will cause an immediate error.  Defaults to 'false'
+"""
+StartAlignmentRequest.__doc__ = """Attributes:
+    name:
+        User specified name to identify the alignment run.
+    input_reads_directories:
+        Input directories to search for reads to be aligned.
+        Currently, only one directory can be specified, but this
+        definition allows for multiple in the future without breaking
+        compatibility.
+    output_reads_directory:
+        Output directory where aligned reads will be placed.
+    recursive:
+        Recursively find fast5 files to align in the
+        `input_reads_directories`.  If False, only the fast5 files
+        directly in one of the `input_reads_directories` will be
+        aligned. If True, subdirectories of those directories will
+        also be searched recursively.
+    alignment_configuration:
+        Options to control alignment performed once basecalling reads
+        is complete.
+"""
+StartAlignmentResponse.__doc__ = """Attributes:
+    id:
+        An identifier for the alignment run that was started. This can
+        be used to monitor or cancel the run.
+"""
+SendPingRequest.__doc__ = """Since 5.0
+
+Attributes:
+    ping_data:
+        The json data to send as a ping.  note: if this string is not
+        a valid json object, an error will be raised.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/basecaller_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/basecaller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/basecaller_service.py` & `minknow_api-5.5.2/minknow_api/basecaller_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/ca.crt` & `minknow_api-5.5.2/minknow_api/ca.crt`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/data.py` & `minknow_api-5.5.2/minknow_api/data.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/data_pb2.py` & `minknow_api-5.5.2/minknow_api/data_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: minknow_api/data.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
@@ -17,950 +16,16 @@
 from minknow_api import statistics_pb2 as minknow__api_dot_statistics__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16minknow_api/data.proto\x12\x10minknow_api.data\x1a\x1dminknow_api/rpc_options.proto\x1a\x18minknow_api/device.proto\x1a\x1cminknow_api/statistics.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xd9\x01\n\x17GetChannelStatesRequest\x12\x1b\n\rfirst_channel\x18\x01 \x01(\rB\x04\x88\xb5\x18\x01\x12\x1a\n\x0clast_channel\x18\x02 \x01(\rB\x04\x88\xb5\x18\x01\x12:\n\x16use_channel_states_ids\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1b\n\x13wait_for_processing\x18\x04 \x01(\x08\x12,\n\theartbeat\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xdb\x02\n\x18GetChannelStatesResponse\x12S\n\x0e\x63hannel_states\x18\x01 \x03(\x0b\x32;.minknow_api.data.GetChannelStatesResponse.ChannelStateData\x1a\xe9\x01\n\x10\x43hannelStateData\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\r\x12\x12\n\x08state_id\x18\x02 \x01(\rH\x00\x12\x14\n\nstate_name\x18\x03 \x01(\tH\x00\x12\x1d\n\x15\x61\x63quisition_raw_index\x18\x04 \x01(\x04\x12\x1a\n\x12\x61nalysis_raw_index\x18\x05 \x01(\x04\x12\x14\n\x0ctrigger_time\x18\x07 \x01(\x04\x12@\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x30.minknow_api.device.ReturnedChannelConfigurationB\x07\n\x05state\"\x15\n\x13GetDataTypesRequest\"\xb1\x03\n\x14GetDataTypesResponse\x12L\n\x13uncalibrated_signal\x18\x01 \x01(\x0b\x32/.minknow_api.data.GetDataTypesResponse.DataType\x12J\n\x11\x63\x61librated_signal\x18\x02 \x01(\x0b\x32/.minknow_api.data.GetDataTypesResponse.DataType\x12\x46\n\rbias_voltages\x18\x03 \x01(\x0b\x32/.minknow_api.data.GetDataTypesResponse.DataType\x1a\xb6\x01\n\x08\x44\x61taType\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.minknow_api.data.GetDataTypesResponse.DataType.Type\x12\x12\n\nbig_endian\x18\x02 \x01(\x08\x12\x0c\n\x04size\x18\x03 \x01(\r\"D\n\x04Type\x12\x12\n\x0eSIGNED_INTEGER\x10\x00\x12\x14\n\x10UNSIGNED_INTEGER\x10\x01\x12\x12\n\x0e\x46LOATING_POINT\x10\x02\"\xf8\x01\n\x15GetSignalBytesRequest\x12\x11\n\x07seconds\x18\x01 \x01(\x02H\x00\x12\x11\n\x07samples\x18\x02 \x01(\rH\x00\x12\x1b\n\rfirst_channel\x18\x03 \x01(\rB\x04\x88\xb5\x18\x01\x12\x1a\n\x0clast_channel\x18\x04 \x01(\rB\x04\x88\xb5\x18\x01\x12\x1f\n\x17include_channel_configs\x18\x05 \x01(\x08\x12\x1d\n\x15include_bias_voltages\x18\x06 \x01(\x08\x12\x17\n\x0f\x63\x61librated_data\x18\x07 \x01(\x08\x12\x1d\n\x15return_when_listening\x18\x08 \x01(\x08\x42\x08\n\x06length\"\xa7\x03\n\x16GetSignalBytesResponse\x12\x1b\n\x13samples_since_start\x18\x01 \x01(\x04\x12\x1b\n\x13seconds_since_start\x18\x02 \x01(\x01\x12\x18\n\x10skipped_channels\x18\x03 \x01(\r\x12\x46\n\x08\x63hannels\x18\x04 \x03(\x0b\x32\x34.minknow_api.data.GetSignalBytesResponse.ChannelData\x12\x15\n\rbias_voltages\x18\x05 \x01(\x0c\x1ag\n\x13\x43hannelConfigChange\x12@\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x30.minknow_api.device.ReturnedChannelConfiguration\x12\x0e\n\x06offset\x18\x02 \x01(\x04\x1aq\n\x0b\x43hannelData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12T\n\x0e\x63onfig_changes\x18\x03 \x03(\x0b\x32<.minknow_api.data.GetSignalBytesResponse.ChannelConfigChange\"\x85\x01\n\x16GetSignalMinMaxRequest\x12\x1b\n\rfirst_channel\x18\x03 \x01(\rB\x04\x88\xb5\x18\x01\x12\x1a\n\x0clast_channel\x18\x04 \x01(\rB\x04\x88\xb5\x18\x01\x12\x19\n\x0bwindow_size\x18\x05 \x01(\rB\x04\x88\xb5\x18\x01\x12\x17\n\x0f\x63\x61librated_data\x18\x07 \x01(\x08\"\xa3\x02\n\x17GetSignalMinMaxResponse\x12\x1b\n\x13samples_since_start\x18\x01 \x01(\x04\x12\x1b\n\x13seconds_since_start\x18\x02 \x01(\x01\x12\x18\n\x10skipped_channels\x18\x03 \x01(\r\x12G\n\x08\x63hannels\x18\x04 \x03(\x0b\x32\x35.minknow_api.data.GetSignalMinMaxResponse.ChannelData\x1ak\n\x0b\x43hannelData\x12\x19\n\x11\x63\x61librated_minima\x18\x01 \x03(\x02\x12\x12\n\nraw_minima\x18\x02 \x03(\x05\x12\x19\n\x11\x63\x61librated_maxima\x18\x03 \x03(\x02\x12\x12\n\nraw_maxima\x18\x04 \x03(\x05\"\xb6\x07\n\x13GetLiveReadsRequest\x12\x42\n\x05setup\x18\x01 \x01(\x0b\x32\x31.minknow_api.data.GetLiveReadsRequest.StreamSetupH\x00\x12@\n\x07\x61\x63tions\x18\x02 \x01(\x0b\x32-.minknow_api.data.GetLiveReadsRequest.ActionsH\x00\x1a!\n\rUnblockAction\x12\x10\n\x08\x64uration\x18\x01 \x01(\x01\x1a\x11\n\x0fStopFurtherData\x1a\xfa\x01\n\x06\x41\x63tion\x12\x11\n\taction_id\x18\x01 \x01(\t\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\r\x12\x0c\n\x02id\x18\x03 \x01(\tH\x00\x12\x10\n\x06number\x18\x04 \x01(\rH\x00\x12\x46\n\x07unblock\x18\x05 \x01(\x0b\x32\x33.minknow_api.data.GetLiveReadsRequest.UnblockActionH\x01\x12R\n\x11stop_further_data\x18\x06 \x01(\x0b\x32\x35.minknow_api.data.GetLiveReadsRequest.StopFurtherDataH\x01\x42\x06\n\x04readB\x08\n\x06\x61\x63tion\x1a\xc6\x02\n\x0bStreamSetup\x12\x15\n\rfirst_channel\x18\x01 \x01(\r\x12\x14\n\x0clast_channel\x18\x02 \x01(\r\x12H\n\rraw_data_type\x18\x03 \x01(\x0e\x32\x31.minknow_api.data.GetLiveReadsRequest.RawDataType\x12!\n\x19sample_minimum_chunk_size\x18\x04 \x01(\x04\x12)\n\x1fmax_unblock_read_length_samples\x18\x05 \x01(\x04H\x00\x12)\n\x1fmax_unblock_read_length_seconds\x18\x06 \x01(\x01H\x00\x12,\n$accepted_first_chunk_classifications\x18\x07 \x03(\x05\x42\x19\n\x17max_unblock_read_length\x1aH\n\x07\x41\x63tions\x12=\n\x07\x61\x63tions\x18\x02 \x03(\x0b\x32,.minknow_api.data.GetLiveReadsRequest.Action\"H\n\x0bRawDataType\x12\r\n\tKEEP_LAST\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\x0e\n\nCALIBRATED\x10\x02\x12\x10\n\x0cUNCALIBRATED\x10\x03\x42\t\n\x07request\"\xc8\x06\n\x14GetLiveReadsResponse\x12\x1b\n\x13samples_since_start\x18\x01 \x01(\x04\x12\x1b\n\x13seconds_since_start\x18\x02 \x01(\x01\x12\x46\n\x08\x63hannels\x18\x04 \x03(\x0b\x32\x34.minknow_api.data.GetLiveReadsResponse.ChannelsEntry\x12O\n\x10\x61\x63tion_responses\x18\x05 \x03(\x0b\x32\x35.minknow_api.data.GetLiveReadsResponse.ActionResponse\x1a\xb5\x02\n\x08ReadData\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06number\x18\x02 \x01(\r\x12\x14\n\x0cstart_sample\x18\x03 \x01(\x04\x12\x1a\n\x12\x63hunk_start_sample\x18\x04 \x01(\x04\x12\x14\n\x0c\x63hunk_length\x18\x05 \x01(\x04\x12\x1d\n\x15\x63hunk_classifications\x18\x06 \x03(\x05\x12\x10\n\x08raw_data\x18\x07 \x01(\x0c\x12\x15\n\rmedian_before\x18\x08 \x01(\x02\x12\x0e\n\x06median\x18\t \x01(\x02\x12$\n\x1cprevious_read_classification\x18\n \x01(\x05\x12G\n\x18previous_read_end_reason\x18\x0b \x01(\x0e\x32%.minknow_api.statistics.ReadEndReason\x1a\xc2\x01\n\x0e\x41\x63tionResponse\x12\x11\n\taction_id\x18\x01 \x01(\t\x12P\n\x08response\x18\x02 \x01(\x0e\x32>.minknow_api.data.GetLiveReadsResponse.ActionResponse.Response\"K\n\x08Response\x12\x0b\n\x07SUCCESS\x10\x00\x12\x18\n\x14\x46\x41ILED_READ_FINISHED\x10\x01\x12\x18\n\x14\x46\x41ILED_READ_TOO_LONG\x10\x02\x1a`\n\rChannelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12>\n\x05value\x18\x02 \x01(\x0b\x32/.minknow_api.data.GetLiveReadsResponse.ReadData:\x02\x38\x01\"\x1b\n\x19ResetChannelStatesRequest\"\x1c\n\x1aResetChannelStatesResponse\"\xb8\x02\n\x18GetReadStatisticsRequest\x12\x10\n\x08\x63hannels\x18\x01 \x03(\r\x12\x11\n\x07seconds\x18\x02 \x01(\x02H\x00\x12\x11\n\x07samples\x18\x03 \x01(\x04H\x00\x12N\n\nread_split\x18\x04 \x01(\x0e\x32\x34.minknow_api.data.GetReadStatisticsRequest.ReadSplitB\x04\x88\xb5\x18\x01\x12\x1d\n\x15no_current_statistics\x18\x05 \x01(\x08\x12\x1b\n\x13no_chunk_statistics\x18\x06 \x01(\x08\x12 \n\x18required_classifications\x18\x07 \x03(\t\"*\n\tReadSplit\x12\t\n\x05\x43HUNK\x10\x00\x12\x12\n\x0e\x43OMPLETED_READ\x10\x01\x42\n\n\x08\x64uration\"\xe4\n\n\x19GetReadStatisticsResponse\x12L\n\x08\x63hannels\x18\x01 \x03(\x0b\x32:.minknow_api.data.GetReadStatisticsResponse.PerChannelData\x12\x1b\n\x13samples_since_start\x18\x02 \x01(\x04\x12\x1b\n\x13seconds_since_start\x18\x03 \x01(\x01\x1a\xa4\x01\n\nStatistics\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\x12\x0c\n\x04mean\x18\x03 \x01(\x01\x12\x0b\n\x03s_d\x18\x04 \x01(\x01\x12\x0e\n\x06median\x18\x06 \x01(\x01\x12\x0b\n\x03q_5\x18\x07 \x01(\x01\x12\x0c\n\x04q_10\x18\x08 \x01(\x01\x12\x0c\n\x04q_25\x18\t \x01(\x01\x12\x0c\n\x04q_75\x18\n \x01(\x01\x12\x0c\n\x04q_90\x18\x0b \x01(\x01\x12\x0c\n\x04q_95\x18\x0c \x01(\x01\x1a\x43\n\x0f\x43hunkStatistics\x12\x11\n\tmedian_sd\x18\x01 \x01(\x01\x12\x0e\n\x06median\x18\x02 \x01(\x01\x12\r\n\x05range\x18\x03 \x01(\x01\x1a\xcb\x02\n\x15PerClassificationData\x12S\n\x13\x64uration_statistics\x18\x01 \x01(\x0b\x32\x36.minknow_api.data.GetReadStatisticsResponse.Statistics\x12R\n\x12\x63urrent_statistics\x18\x02 \x01(\x0b\x32\x36.minknow_api.data.GetReadStatisticsResponse.Statistics\x12U\n\x10\x63hunk_statistics\x18\x06 \x01(\x0b\x32;.minknow_api.data.GetReadStatisticsResponse.ChunkStatistics\x12\x18\n\x10samples_duration\x18\x04 \x01(\x04\x12\x18\n\x10seconds_duration\x18\x05 \x01(\x01\x1a\xa9\x03\n\x14PerConfigurationData\x12O\n\x15\x63hannel_configuration\x18\x01 \x01(\x0b\x32\x30.minknow_api.device.ReturnedChannelConfiguration\x12n\n\x0f\x63lassifications\x18\x02 \x03(\x0b\x32U.minknow_api.data.GetReadStatisticsResponse.PerConfigurationData.ClassificationsEntry\x12U\n\nincomplete\x18\x03 \x01(\x0b\x32\x41.minknow_api.data.GetReadStatisticsResponse.PerClassificationData\x1ay\n\x14\x43lassificationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12P\n\x05value\x18\x02 \x01(\x0b\x32\x41.minknow_api.data.GetReadStatisticsResponse.PerClassificationData:\x02\x38\x01\x1a\xd8\x01\n\x0ePerChannelData\x12X\n\x0e\x63onfigurations\x18\x06 \x03(\x0b\x32@.minknow_api.data.GetReadStatisticsResponse.PerConfigurationData\x12\x1b\n\x13samples_since_start\x18\x02 \x01(\x04\x12\x1b\n\x13seconds_since_start\x18\x03 \x01(\x01\x12\x18\n\x10samples_duration\x18\x04 \x01(\x04\x12\x18\n\x10seconds_duration\x18\x05 \x01(\x01\"L\n\x18LockChannelStatesRequest\x12\x16\n\x08\x63hannels\x18\x01 \x03(\x04\x42\x04\x88\xb5\x18\x01\x12\x18\n\nstate_name\x18\x02 \x01(\tB\x04\x88\xb5\x18\x01\"\x1b\n\x19LockChannelStatesResponse\"4\n\x1aUnlockChannelStatesRequest\x12\x16\n\x08\x63hannels\x18\x01 \x03(\x04\x42\x04\x88\xb5\x18\x01\"\x1d\n\x1bUnlockChannelStatesResponse\"\x1f\n\x1dGetExperimentYieldInfoRequest\"\x84\x1c\n\x1eGetExperimentYieldInfoResponse\x12]\n\x12\x63omplete_read_info\x18\x01 \x01(\x0b\x32\x41.minknow_api.data.GetExperimentYieldInfoResponse.CompleteReadInfo\x12Z\n\x10\x61\x63quisition_info\x18\x02 \x01(\x0b\x32@.minknow_api.data.GetExperimentYieldInfoResponse.AcquisitionInfo\x12T\n\ranalyser_info\x18\x03 \x01(\x0b\x32=.minknow_api.data.GetExperimentYieldInfoResponse.AnalyserInfo\x12L\n\tbulk_info\x18\x04 \x01(\x0b\x32\x39.minknow_api.data.GetExperimentYieldInfoResponse.BulkInfo\x12W\n\x0fhdf_writer_info\x18\x05 \x01(\x0b\x32>.minknow_api.data.GetExperimentYieldInfoResponse.HdfWriterInfo\x12\x62\n\x15\x62\x61secaller_statistics\x18\x06 \x01(\x0b\x32\x43.minknow_api.data.GetExperimentYieldInfoResponse.BasecallStatistics\x12z\n\"hdf_multi_read_writing_statisitics\x18\x07 \x01(\x0b\x32N.minknow_api.data.GetExperimentYieldInfoResponse.HdfMultiReadWritingStatistics\x12r\n\x1d\x66\x61stq_read_writing_statistics\x18\x08 \x01(\x0b\x32K.minknow_api.data.GetExperimentYieldInfoResponse.FastqReadWritingStatistics\x12x\n protobuf_read_writing_statistics\x18\t \x01(\x0b\x32N.minknow_api.data.GetExperimentYieldInfoResponse.ProtobufReadWritingStatistics\x12r\n\x1d\x66ile_operation_queue_progress\x18\n \x01(\x0b\x32K.minknow_api.data.GetExperimentYieldInfoResponse.FileOperationQueueProgress\x1a\xa8\x04\n\x10\x43ompleteReadInfo\x12\x16\n\x0epending_chunks\x18\x01 \x01(\x04\x12\x1c\n\x14pending_memory_reads\x18\x02 \x01(\x04\x12\x1a\n\x12pending_disk_reads\x18\x0f \x01(\x04\x12 \n\x18pending_multi_disk_reads\x18\x03 \x01(\x04\x12\x1d\n\x15pending_skipped_reads\x18\x04 \x01(\x04\x12#\n\x1bpending_force_skipped_reads\x18\x05 \x01(\x04\x12\x1e\n\x16processed_memory_reads\x18\x06 \x01(\x04\x12\x1c\n\x14processed_disk_reads\x18\x07 \x01(\x04\x12\x1f\n\x17processed_skipped_reads\x18\x08 \x01(\x04\x12%\n\x1dprocessed_force_skipped_reads\x18\t \x01(\x04\x12!\n\x19stored_reads_bytes_memory\x18\n \x01(\x04\x12+\n#stored_read_supporting_bytes_memory\x18\x10 \x01(\x04\x12\x1f\n\x17stored_reads_bytes_disk\x18\x0b \x01(\x04\x12\x1d\n\x15\x64iscarded_error_bytes\x18\x0c \x01(\x04\x12 \n\x18\x63hannels_writing_to_disk\x18\r \x01(\x04\x12$\n\x1c\x63hannels_writing_to_disk_tmp\x18\x0e \x01(\x04\x1aI\n\x0f\x41\x63quisitionInfo\x12\x17\n\x0fraw_per_channel\x18\x01 \x01(\x04\x12\x1d\n\x15\x66rame_discontinuities\x18\x02 \x01(\x04\x1a\xe5\x01\n\x0c\x41nalyserInfo\x12\x17\n\x0fraw_per_channel\x18\x01 \x01(\x04\x12\x1a\n\x12total_selected_raw\x18\x02 \x01(\x04\x12\x1d\n\x15total_selected_events\x18\x03 \x01(\x04\x12\x14\n\x0ctotal_events\x18\x04 \x01(\x04\x12\x19\n\x11total_read_chunks\x18\x05 \x01(\x04\x12&\n\x1e\x63ompleted_selected_reads_count\x18\x06 \x01(\x04\x12(\n completed_unselected_reads_count\x18\x07 \x01(\x04\x1a\x33\n\x08\x42ulkInfo\x12\x11\n\ttotal_raw\x18\x01 \x01(\x04\x12\x14\n\x0ctotal_events\x18\x02 \x01(\x04\x1a\xa0\x01\n\rHdfWriterInfo\x12\x1c\n\x14pending_compressions\x18\x01 \x01(\x04\x12\x16\n\x0epending_writes\x18\x02 \x01(\x04\x12\x19\n\x11pending_hdf_tasks\x18\x03 \x01(\x04\x12\x18\n\x10\x63ompleted_writes\x18\x04 \x01(\x04\x12$\n\x1c\x64\x61taset_bytes_data_in_flight\x18\x05 \x01(\x04\x1a\xd9\x02\n\x12\x42\x61secallStatistics\x12\x19\n\x11reads_in_progress\x18\x01 \x01(\x04\x12\x17\n\x0freads_processed\x18\x02 \x01(\x04\x12\x15\n\rreads_skipped\x18\x03 \x01(\x04\x12\x1b\n\x13reads_force_skipped\x18\x04 \x01(\x04\x12%\n\x1dreads_failed_calling_filtered\x18\x05 \x01(\x04\x12\x1c\n\x14reads_failed_calling\x18\x06 \x01(\x04\x12\x14\n\x0creads_called\x18\x07 \x01(\x04\x12\x16\n\x0esamples_called\x18\x08 \x01(\x04\x12\x17\n\x0fsamples_skipped\x18\t \x01(\x04\x12\x1b\n\x13\x62\x61ses_passed_called\x18\n \x01(\x04\x12\x1b\n\x13\x62\x61ses_failed_called\x18\x0c \x01(\x04\x12\x15\n\revents_called\x18\x0b \x01(\x04\x1a\xf6\x01\n\x1dHdfMultiReadWritingStatistics\x12\x15\n\rreads_written\x18\x01 \x01(\x04\x12\x1c\n\x14passed_reads_written\x18\x02 \x01(\x04\x12\x1c\n\x14\x66\x61iled_reads_written\x18\x03 \x01(\x04\x12#\n\x1b\x66orce_skipped_reads_written\x18\x04 \x01(\x04\x12\x19\n\x11raw_bytes_written\x18\x05 \x01(\x04\x12\x1b\n\x13\x66\x61stq_bytes_written\x18\x06 \x01(\x04\x12%\n\x1d\x62\x61secall_events_bytes_written\x18\x07 \x01(\x04\x1a\xa7\x01\n\x1a\x46\x61stqReadWritingStatistics\x12\x1c\n\x14passed_reads_written\x18\x01 \x01(\x04\x12\x15\n\rskipped_reads\x18\x02 \x01(\x04\x12\x16\n\x0e\x66orced_skipped\x18\x03 \x01(\x04\x12\x1c\n\x14\x66\x61iled_reads_written\x18\x04 \x01(\x04\x12\x1e\n\x16\x66\x61iled_reads_discarded\x18\x05 \x01(\x04\x1a\x8b\x01\n\x1dProtobufReadWritingStatistics\x12\x1b\n\x13read_chunks_written\x18\x01 \x01(\x04\x12\x1d\n\x15read_chunks_discarded\x18\x02 \x01(\x04\x12\x15\n\rreads_written\x18\x03 \x01(\x04\x12\x17\n\x0freads_discarded\x18\x04 \x01(\x04\x1a\xa4\x04\n\x1a\x46ileOperationQueueProgress\x12\x1a\n\x12pending_operations\x18\x01 \x01(\x04\x12&\n\x1e\x63omplete_successful_operations\x18\x02 \x01(\x04\x12\"\n\x1a\x63omplete_failed_operations\x18\x03 \x01(\x04\x12\x1c\n\x14\x62ytes_to_move_posted\x18\x04 \x01(\x04\x12\x1c\n\x14\x62ytes_to_move_failed\x18\x05 \x01(\x04\x12\x1f\n\x17\x62ytes_to_move_completed\x18\x06 \x01(\x04\x12g\n\x05\x66\x61st5\x18\x07 \x01(\x0b\x32X.minknow_api.data.GetExperimentYieldInfoResponse.FileOperationQueueProgress.FileTypeInfo\x12g\n\x05\x66\x61stq\x18\x08 \x01(\x0b\x32X.minknow_api.data.GetExperimentYieldInfoResponse.FileOperationQueueProgress.FileTypeInfo\x1ao\n\x0c\x46ileTypeInfo\x12 \n\x18\x66iles_moved_successfully\x18\x01 \x01(\x04\x12\x1f\n\x17\x66iles_moved_to_fallback\x18\x02 \x01(\x04\x12\x1c\n\x14\x66iles_failed_to_move\x18\x03 \x01(\x04\x32\x8b\t\n\x0b\x44\x61taService\x12r\n\x12get_channel_states\x12).minknow_api.data.GetChannelStatesRequest\x1a*.minknow_api.data.GetChannelStatesResponse\"\x03\x90\x02\x01\x30\x01\x12\x64\n\x0eget_data_types\x12%.minknow_api.data.GetDataTypesRequest\x1a&.minknow_api.data.GetDataTypesResponse\"\x03\x90\x02\x01\x12l\n\x10get_signal_bytes\x12\'.minknow_api.data.GetSignalBytesRequest\x1a(.minknow_api.data.GetSignalBytesResponse\"\x03\x90\x02\x01\x30\x01\x12p\n\x12get_signal_min_max\x12(.minknow_api.data.GetSignalMinMaxRequest\x1a).minknow_api.data.GetSignalMinMaxResponse\"\x03\x90\x02\x01\x30\x01\x12s\n\x14reset_channel_states\x12+.minknow_api.data.ResetChannelStatesRequest\x1a,.minknow_api.data.ResetChannelStatesResponse\"\x00\x12p\n\x13lock_channel_states\x12*.minknow_api.data.LockChannelStatesRequest\x1a+.minknow_api.data.LockChannelStatesResponse\"\x00\x12v\n\x15unlock_channel_states\x12,.minknow_api.data.UnlockChannelStatesRequest\x1a-.minknow_api.data.UnlockChannelStatesResponse\"\x00\x12h\n\x0eget_live_reads\x12%.minknow_api.data.GetLiveReadsRequest\x1a&.minknow_api.data.GetLiveReadsResponse\"\x03\x90\x02\x01(\x01\x30\x01\x12s\n\x13get_read_statistics\x12*.minknow_api.data.GetReadStatisticsRequest\x1a+.minknow_api.data.GetReadStatisticsResponse\"\x03\x90\x02\x01\x12\x83\x01\n\x19get_experiment_yield_info\x12/.minknow_api.data.GetExperimentYieldInfoRequest\x1a\x30.minknow_api.data.GetExperimentYieldInfoResponse\"\x03\x90\x02\x01\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-
-
-_GETCHANNELSTATESREQUEST = DESCRIPTOR.message_types_by_name['GetChannelStatesRequest']
-_GETCHANNELSTATESRESPONSE = DESCRIPTOR.message_types_by_name['GetChannelStatesResponse']
-_GETCHANNELSTATESRESPONSE_CHANNELSTATEDATA = _GETCHANNELSTATESRESPONSE.nested_types_by_name['ChannelStateData']
-_GETDATATYPESREQUEST = DESCRIPTOR.message_types_by_name['GetDataTypesRequest']
-_GETDATATYPESRESPONSE = DESCRIPTOR.message_types_by_name['GetDataTypesResponse']
-_GETDATATYPESRESPONSE_DATATYPE = _GETDATATYPESRESPONSE.nested_types_by_name['DataType']
-_GETSIGNALBYTESREQUEST = DESCRIPTOR.message_types_by_name['GetSignalBytesRequest']
-_GETSIGNALBYTESRESPONSE = DESCRIPTOR.message_types_by_name['GetSignalBytesResponse']
-_GETSIGNALBYTESRESPONSE_CHANNELCONFIGCHANGE = _GETSIGNALBYTESRESPONSE.nested_types_by_name['ChannelConfigChange']
-_GETSIGNALBYTESRESPONSE_CHANNELDATA = _GETSIGNALBYTESRESPONSE.nested_types_by_name['ChannelData']
-_GETSIGNALMINMAXREQUEST = DESCRIPTOR.message_types_by_name['GetSignalMinMaxRequest']
-_GETSIGNALMINMAXRESPONSE = DESCRIPTOR.message_types_by_name['GetSignalMinMaxResponse']
-_GETSIGNALMINMAXRESPONSE_CHANNELDATA = _GETSIGNALMINMAXRESPONSE.nested_types_by_name['ChannelData']
-_GETLIVEREADSREQUEST = DESCRIPTOR.message_types_by_name['GetLiveReadsRequest']
-_GETLIVEREADSREQUEST_UNBLOCKACTION = _GETLIVEREADSREQUEST.nested_types_by_name['UnblockAction']
-_GETLIVEREADSREQUEST_STOPFURTHERDATA = _GETLIVEREADSREQUEST.nested_types_by_name['StopFurtherData']
-_GETLIVEREADSREQUEST_ACTION = _GETLIVEREADSREQUEST.nested_types_by_name['Action']
-_GETLIVEREADSREQUEST_STREAMSETUP = _GETLIVEREADSREQUEST.nested_types_by_name['StreamSetup']
-_GETLIVEREADSREQUEST_ACTIONS = _GETLIVEREADSREQUEST.nested_types_by_name['Actions']
-_GETLIVEREADSRESPONSE = DESCRIPTOR.message_types_by_name['GetLiveReadsResponse']
-_GETLIVEREADSRESPONSE_READDATA = _GETLIVEREADSRESPONSE.nested_types_by_name['ReadData']
-_GETLIVEREADSRESPONSE_ACTIONRESPONSE = _GETLIVEREADSRESPONSE.nested_types_by_name['ActionResponse']
-_GETLIVEREADSRESPONSE_CHANNELSENTRY = _GETLIVEREADSRESPONSE.nested_types_by_name['ChannelsEntry']
-_RESETCHANNELSTATESREQUEST = DESCRIPTOR.message_types_by_name['ResetChannelStatesRequest']
-_RESETCHANNELSTATESRESPONSE = DESCRIPTOR.message_types_by_name['ResetChannelStatesResponse']
-_GETREADSTATISTICSREQUEST = DESCRIPTOR.message_types_by_name['GetReadStatisticsRequest']
-_GETREADSTATISTICSRESPONSE = DESCRIPTOR.message_types_by_name['GetReadStatisticsResponse']
-_GETREADSTATISTICSRESPONSE_STATISTICS = _GETREADSTATISTICSRESPONSE.nested_types_by_name['Statistics']
-_GETREADSTATISTICSRESPONSE_CHUNKSTATISTICS = _GETREADSTATISTICSRESPONSE.nested_types_by_name['ChunkStatistics']
-_GETREADSTATISTICSRESPONSE_PERCLASSIFICATIONDATA = _GETREADSTATISTICSRESPONSE.nested_types_by_name['PerClassificationData']
-_GETREADSTATISTICSRESPONSE_PERCONFIGURATIONDATA = _GETREADSTATISTICSRESPONSE.nested_types_by_name['PerConfigurationData']
-_GETREADSTATISTICSRESPONSE_PERCONFIGURATIONDATA_CLASSIFICATIONSENTRY = _GETREADSTATISTICSRESPONSE_PERCONFIGURATIONDATA.nested_types_by_name['ClassificationsEntry']
-_GETREADSTATISTICSRESPONSE_PERCHANNELDATA = _GETREADSTATISTICSRESPONSE.nested_types_by_name['PerChannelData']
-_LOCKCHANNELSTATESREQUEST = DESCRIPTOR.message_types_by_name['LockChannelStatesRequest']
-_LOCKCHANNELSTATESRESPONSE = DESCRIPTOR.message_types_by_name['LockChannelStatesResponse']
-_UNLOCKCHANNELSTATESREQUEST = DESCRIPTOR.message_types_by_name['UnlockChannelStatesRequest']
-_UNLOCKCHANNELSTATESRESPONSE = DESCRIPTOR.message_types_by_name['UnlockChannelStatesResponse']
-_GETEXPERIMENTYIELDINFOREQUEST = DESCRIPTOR.message_types_by_name['GetExperimentYieldInfoRequest']
-_GETEXPERIMENTYIELDINFORESPONSE = DESCRIPTOR.message_types_by_name['GetExperimentYieldInfoResponse']
-_GETEXPERIMENTYIELDINFORESPONSE_COMPLETEREADINFO = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['CompleteReadInfo']
-_GETEXPERIMENTYIELDINFORESPONSE_ACQUISITIONINFO = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['AcquisitionInfo']
-_GETEXPERIMENTYIELDINFORESPONSE_ANALYSERINFO = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['AnalyserInfo']
-_GETEXPERIMENTYIELDINFORESPONSE_BULKINFO = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['BulkInfo']
-_GETEXPERIMENTYIELDINFORESPONSE_HDFWRITERINFO = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['HdfWriterInfo']
-_GETEXPERIMENTYIELDINFORESPONSE_BASECALLSTATISTICS = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['BasecallStatistics']
-_GETEXPERIMENTYIELDINFORESPONSE_HDFMULTIREADWRITINGSTATISTICS = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['HdfMultiReadWritingStatistics']
-_GETEXPERIMENTYIELDINFORESPONSE_FASTQREADWRITINGSTATISTICS = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['FastqReadWritingStatistics']
-_GETEXPERIMENTYIELDINFORESPONSE_PROTOBUFREADWRITINGSTATISTICS = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['ProtobufReadWritingStatistics']
-_GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS = _GETEXPERIMENTYIELDINFORESPONSE.nested_types_by_name['FileOperationQueueProgress']
-_GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS_FILETYPEINFO = _GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS.nested_types_by_name['FileTypeInfo']
-_GETDATATYPESRESPONSE_DATATYPE_TYPE = _GETDATATYPESRESPONSE_DATATYPE.enum_types_by_name['Type']
-_GETLIVEREADSREQUEST_RAWDATATYPE = _GETLIVEREADSREQUEST.enum_types_by_name['RawDataType']
-_GETLIVEREADSRESPONSE_ACTIONRESPONSE_RESPONSE = _GETLIVEREADSRESPONSE_ACTIONRESPONSE.enum_types_by_name['Response']
-_GETREADSTATISTICSREQUEST_READSPLIT = _GETREADSTATISTICSREQUEST.enum_types_by_name['ReadSplit']
-GetChannelStatesRequest = _reflection.GeneratedProtocolMessageType('GetChannelStatesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCHANNELSTATESREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      first_channel:
-          The first channel (inclusive) to return data for.  Note that
-          channel numbering starts at 1.
-      last_channel:
-          The last channel (inclusive) to return data for.  Note that
-          channel numbering starts at 1.
-      use_channel_states_ids:
-          If this is true, the returned messages will contain the
-          channel state id as opposed to the name. By default, the
-          response will contain channel states names.
-      wait_for_processing:
-          If `wait_for_processing` is true, then get_channel_states will
-          wait until minknow starts acquiring data instead of returning
-          with an error  Defaults to false
-      heartbeat:
-          Ensure the stream sends a message at least this often.  There
-          will usually be multiple channel updates a second, but in some
-          circumstances (eg: a flow cell with no sample loaded) there
-          can be long periods of time without updates.  Setting this
-          value will ensure that if this period of time passes without
-          there being any channel state changes to report, an empty
-          message will be sent. This can be useful to force a minimum
-          wakeup interval in the client code.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetChannelStatesRequest)
-  })
-_sym_db.RegisterMessage(GetChannelStatesRequest)
-
-GetChannelStatesResponse = _reflection.GeneratedProtocolMessageType('GetChannelStatesResponse', (_message.Message,), {
-
-  'ChannelStateData' : _reflection.GeneratedProtocolMessageType('ChannelStateData', (_message.Message,), {
-    'DESCRIPTOR' : _GETCHANNELSTATESRESPONSE_CHANNELSTATEDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        channel:
-            Represents the channel number, indexed from one. (i.e. what
-            channel did the channel state change happened on)
-        state:
-            depending on the channel state request, MinKNOW can fill in
-            either the name or the criteria id of the channel state. The
-            criteria id (or state_id) is the number passed in the channel
-            states configuration. Note that MinKNOW also has some default
-            channel states (like unclassified, pending mux change) which
-            receive unique ids - these are numbers bigger than 200.
-        acquisition_raw_index:
-            Indices of when the channel state was first seen. For example,
-            if a request is done half way through the experiment, the
-            first message will contain the current state on the requested
-            channels. The acquisition/analysis index of these would be
-            from when the channel states were set. These are exactly the
-            same numbers we see in the bulk file, in the 'states' table
-        config:
-            Channel config (mux state) the channel state was determined
-            on.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetChannelStatesResponse.ChannelStateData)
-    })
-  ,
-  'DESCRIPTOR' : _GETCHANNELSTATESRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      channel_states:
-          The streamed data for all channels will be appended to this
-          vector. After the request is made, all the channel state
-          changes are streamed through this array. This is implemented
-          in the idea of a sparse array because we can have channels
-          that remain in the same state for a long time.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetChannelStatesResponse)
-  })
-_sym_db.RegisterMessage(GetChannelStatesResponse)
-_sym_db.RegisterMessage(GetChannelStatesResponse.ChannelStateData)
-
-GetDataTypesRequest = _reflection.GeneratedProtocolMessageType('GetDataTypesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETDATATYPESREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetDataTypesRequest)
-  })
-_sym_db.RegisterMessage(GetDataTypesRequest)
-
-GetDataTypesResponse = _reflection.GeneratedProtocolMessageType('GetDataTypesResponse', (_message.Message,), {
-
-  'DataType' : _reflection.GeneratedProtocolMessageType('DataType', (_message.Message,), {
-    'DESCRIPTOR' : _GETDATATYPESRESPONSE_DATATYPE,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        type:
-            The basic type of the data item.
-        big_endian:
-            Whether the type is big-endian (high-byte first).  For numeric
-            data types, if this is not set, they are little-endian (low-
-            byte first).
-        size:
-            The size of the data type in bytes.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetDataTypesResponse.DataType)
-    })
-  ,
-  'DESCRIPTOR' : _GETDATATYPESRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      uncalibrated_signal:
-          The format of the uncalibrated (ADC) signal data returned by
-          get_raw_signal_bytes().  In the current release, this will
-          describe 16-bit little-endian integers.
-      calibrated_signal:
-          The format of the calibrated (picoamp) signal data returned by
-          get_raw_signal_bytes().  In the current release, this will
-          describe 32-bit IEEE 754 floating point values.
-      bias_voltages:
-          The format of the bias voltage data returned by
-          get_raw_signal_bytes().  In the current release, this will
-          describe 16-bit little-endian integers.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetDataTypesResponse)
-  })
-_sym_db.RegisterMessage(GetDataTypesResponse)
-_sym_db.RegisterMessage(GetDataTypesResponse.DataType)
-
-GetSignalBytesRequest = _reflection.GeneratedProtocolMessageType('GetSignalBytesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETSIGNALBYTESREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      length:
-          The amount of data to return.  If this is omitted, data will
-          be streamed until the call is cancelled.
-      seconds:
-          The amount of data to return in seconds.  The number of
-          samples returned will be just enough to cover this period of
-          time. Cannot be specified at the same time as ``samples``.
-      samples:
-          The amount of data to return in samples.  The result will
-          contain exactly this many samples. If this is not possible,
-          the call will fail. Cannot be specified at the same time as
-          ``seconds``.
-      first_channel:
-          The first channel (inclusive) to return data for.  Note that
-          channel numbering starts at 1.
-      last_channel:
-          The last channel (inclusive) to return data for.  Note that
-          channel numbering starts at 1.
-      include_channel_configs:
-          Whether to include channel configuration settings.
-      include_bias_voltages:
-          Whether to include bias voltage information.
-      calibrated_data:
-          Whether the data should be calibrated.
-      return_when_listening:
-          When this value is set to true, then an empty message will be
-          sent back to the client to indicate that the backend has
-          acknowleged the request, and that any calls made that will
-          affect the signal after that initial  response will be
-          reflected in the next messages
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetSignalBytesRequest)
-  })
-_sym_db.RegisterMessage(GetSignalBytesRequest)
-
-GetSignalBytesResponse = _reflection.GeneratedProtocolMessageType('GetSignalBytesResponse', (_message.Message,), {
-
-  'ChannelConfigChange' : _reflection.GeneratedProtocolMessageType('ChannelConfigChange', (_message.Message,), {
-    'DESCRIPTOR' : _GETSIGNALBYTESRESPONSE_CHANNELCONFIGCHANGE,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        config:
-            The new channel configuration.
-        offset:
-            The offset in the returned data where the change was applied.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetSignalBytesResponse.ChannelConfigChange)
-    })
-  ,
-
-  'ChannelData' : _reflection.GeneratedProtocolMessageType('ChannelData', (_message.Message,), {
-    'DESCRIPTOR' : _GETSIGNALBYTESRESPONSE_CHANNELDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        data:
-            The signal data.  This is the byte representation of a C-style
-            array of values. Values are stored in order and adjacent to
-            each other.  The type of the elements will depend on whether
-            calibrated data was chosen. The get_data_types() RPC call
-            should be used to determine the precise format of the data,
-            but in general terms, uncalibrated data will be signed
-            integers and calibrated data will be floating-point numbers.
-            Returning the data in this format allows it to be efficiently
-            processed in dynamic languages that can pass the data straight
-            down to a native runtime. For example, in Python, this data
-            can be intepreted directly into a numpy array using
-            numpy.fromstring().  Calibrated data is in picoamps.
-            Uncalibrated data is the raw values output by the device's ADC
-            (analogue-digital converter).
-        config_changes:
-            The configuration changes on the channel during data
-            collection.  If channel configuration changes were requested,
-            this will contain all the channel configuration changes that
-            affect the returned data. This will include at least one
-            element, with offset 0, that describes the configuration at
-            the time the first sample was taken.  Note that the offset is
-            the zero-based index into the adc or picoamps list.  The
-            changes will be ordered by offset.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetSignalBytesResponse.ChannelData)
-    })
-  ,
-  'DESCRIPTOR' : _GETSIGNALBYTESRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      samples_since_start:
-          The number of samples collected before the first sample
-          included in this response.  This gives the position of the
-          first data point on each channel in the overall stream of data
-          being acquired from the device (since this period of data
-          acquisition was started).
-      seconds_since_start:
-          The number of seconds elapsed since data acquisition started.
-          This is the same as ``samples_since_start``, but expressed in
-          seconds.
-      skipped_channels:
-          The number of channels omitted at the start of the
-          ``channels`` array.
-      channels:
-          The signal for each requested channel.  Note that
-          ``skipped_channels`` must be used to determine which channels
-          are given here, as not all channels will be included in every
-          message. The channels that are provided are contiguous and in
-          order, with the first channel being ``first_channel +
-          skipped_channels`` (where ``first_channel`` is from the
-          request message).
-      bias_voltages:
-          The bias voltages set for each sample.  If bias voltages were
-          requested, this will provide voltage data, one voltage per
-          sample. Note that not every message may include bias_voltages
-          (they will generally be included when ``skipped_channels`` is
-          0, but that is not guaranteed).  The get_data_types() RPC call
-          should be used to determine the format of the data.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetSignalBytesResponse)
-  })
-_sym_db.RegisterMessage(GetSignalBytesResponse)
-_sym_db.RegisterMessage(GetSignalBytesResponse.ChannelConfigChange)
-_sym_db.RegisterMessage(GetSignalBytesResponse.ChannelData)
-
-GetSignalMinMaxRequest = _reflection.GeneratedProtocolMessageType('GetSignalMinMaxRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETSIGNALMINMAXREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      first_channel:
-          The first channel (inclusive) to return data for.  Note that
-          channel numbering starts at 1.
-      last_channel:
-          The last channel (inclusive) to return data for.  Note that
-          channel numbering starts at 1.
-      window_size:
-          The size of window to summarise.  A value of zero will be
-          rejected; there is no default.
-      calibrated_data:
-          Whether the data should be calibrated.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetSignalMinMaxRequest)
-  })
-_sym_db.RegisterMessage(GetSignalMinMaxRequest)
-
-GetSignalMinMaxResponse = _reflection.GeneratedProtocolMessageType('GetSignalMinMaxResponse', (_message.Message,), {
-
-  'ChannelData' : _reflection.GeneratedProtocolMessageType('ChannelData', (_message.Message,), {
-    'DESCRIPTOR' : _GETSIGNALMINMAXRESPONSE_CHANNELDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        calibrated_minima:
-            The minimum value for each window.  The type of the elements
-            will depend on whether calibrated data was chosen.
-            Uncalibrated data will be signed integers and calibrated data
-            will be floating-point numbers.  It would be nice to use the
-            "oneof" enum-like type to capture this, but you can't have
-            repeated members in a oneof, and nor can you have a repeated
-            oneof field.  We can simply include message fields for both
-            types of data, as all fields are optional in proto3.  We will
-            rely on the code that constructs this message to guarantee
-            that we don't try and put both types of data into the same
-            message.  Calibrated data is in picoamps. Uncalibrated data is
-            the raw values output by the device's ADC (analogue-digital
-            converter).  This is guaranteed to be the same size as the
-            respective foo_maxima field.
-        calibrated_maxima:
-            The maximum value for each window.  See comments for the
-            "minima" fields above for details of calibrated and
-            uncalibrated data.  This is guaranteed to be the same size as
-            the respective foo_minima field.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetSignalMinMaxResponse.ChannelData)
-    })
-  ,
-  'DESCRIPTOR' : _GETSIGNALMINMAXRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      samples_since_start:
-          The number of samples collected before the first sample
-          included in this response.  This gives the position of the
-          first data point on each channel in the overall stream of data
-          being acquired from the device (since this period of data
-          acquisition was started).
-      seconds_since_start:
-          The number of seconds elapsed since data acquisition started.
-          This is the same as ``samples_since_start``, but expressed in
-          seconds.
-      skipped_channels:
-          The number of channels omitted at the start of the
-          ``channels`` array.
-      channels:
-          The window bounds for each requested channel.  Note that
-          ``skipped_channels`` must be used to determine which channels
-          are given here, as not all channels will be included in every
-          message. The channels that are provided are contiguous and in
-          order, with the first channel being ``first_channel +
-          skipped_channels`` (where ``first_channel`` is from the
-          request message).
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetSignalMinMaxResponse)
-  })
-_sym_db.RegisterMessage(GetSignalMinMaxResponse)
-_sym_db.RegisterMessage(GetSignalMinMaxResponse.ChannelData)
-
-GetLiveReadsRequest = _reflection.GeneratedProtocolMessageType('GetLiveReadsRequest', (_message.Message,), {
-
-  'UnblockAction' : _reflection.GeneratedProtocolMessageType('UnblockAction', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSREQUEST_UNBLOCKACTION,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        duration:
-            Duration of unblock in seconds.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsRequest.UnblockAction)
-    })
-  ,
-
-  'StopFurtherData' : _reflection.GeneratedProtocolMessageType('StopFurtherData', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSREQUEST_STOPFURTHERDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsRequest.StopFurtherData)
-    })
-  ,
-
-  'Action' : _reflection.GeneratedProtocolMessageType('Action', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSREQUEST_ACTION,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        channel:
-            Channel name to unblock
-        read:
-            Identifier for the read to act on.  If the read requested is
-            no longer in progress, the action fails.
-        unblock:
-            Unblock a read and skip further data from this read.
-        stop_further_data:
-            Skip further data from this read, doesn't affect the read
-            data.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsRequest.Action)
-    })
-  ,
-
-  'StreamSetup' : _reflection.GeneratedProtocolMessageType('StreamSetup', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSREQUEST_STREAMSETUP,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        first_channel:
-            The first channel (inclusive) to return data for.  Note that
-            channel numbering starts at 1.
-        last_channel:
-            The last channel (inclusive) to return data for.  Note that
-            channel numbering starts at 1.
-        raw_data_type:
-            Specify the type of raw data to retrieve
-        sample_minimum_chunk_size:
-            Minimum chunk size read data is returned in.
-        max_unblock_read_length:
-            Maximum read length MinKNOW will attempt to unblock reads
-            beyond this length will not be unblocked when Action's
-            request, instead minknow will skip any further data from the
-            read.
-        max_unblock_read_length_samples:
-            Maximum read length MinKNOW will attempt to unblock (in
-            samples).  A value of 0 will cause minknow to unblock reads of
-            any length.
-        max_unblock_read_length_seconds:
-            Maximum read length MinKNOW will attempt to unblock (in
-            seconds).  A value of 0.0 will cause minknow to unblock reads
-            of any length.
-        accepted_first_chunk_classifications:
-            A set of classification identifiers which the client is
-            interested in. If a read starts with a classification not
-            listed here the read is never sent to the client.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsRequest.StreamSetup)
-    })
-  ,
-
-  'Actions' : _reflection.GeneratedProtocolMessageType('Actions', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSREQUEST_ACTIONS,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsRequest.Actions)
-    })
-  ,
-  'DESCRIPTOR' : _GETLIVEREADSREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      setup:
-          Read setup request, initialises channel numbers and type of
-          data returned.  note: Must be specified in the first message
-          sent to MinKNOW. Once MinKNOW has the first setup message
-          reads are sent to the caller as requested. The user can then
-          resend a setup message as frequently as they need to in order
-          to reconfigure live reads - for example by changing if raw
-          data is sent with reads or not.
-      actions:
-          Actions to take given data returned to the user - can only be
-          sent once the setup message above has been sent.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsRequest)
-  })
-_sym_db.RegisterMessage(GetLiveReadsRequest)
-_sym_db.RegisterMessage(GetLiveReadsRequest.UnblockAction)
-_sym_db.RegisterMessage(GetLiveReadsRequest.StopFurtherData)
-_sym_db.RegisterMessage(GetLiveReadsRequest.Action)
-_sym_db.RegisterMessage(GetLiveReadsRequest.StreamSetup)
-_sym_db.RegisterMessage(GetLiveReadsRequest.Actions)
-
-GetLiveReadsResponse = _reflection.GeneratedProtocolMessageType('GetLiveReadsResponse', (_message.Message,), {
-
-  'ReadData' : _reflection.GeneratedProtocolMessageType('ReadData', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSRESPONSE_READDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        id:
-            The id of this read, this id is unique for every read ever
-            produced.
-        number:
-            The minknow assigned number of this read  Read numbers always
-            increment throughout the experiment, and are unique per
-            channel - however they are not necessarily contiguous.
-        start_sample:
-            Absolute start point of this read
-        chunk_start_sample:
-            Absolute start point through the experiment of this chunk
-        chunk_length:
-            Length of the chunk in samples
-        chunk_classifications:
-            All Classifications given to intermediate chunks by analysis
-            See analysis_configuration.get_read_classifications for how to
-            map these integers to names.
-        raw_data:
-            Any raw data selected by the request  The type of the elements
-            will depend on whether calibrated data was chosen. The
-            get_data_types() RPC call should be used to determine the
-            precise format of the data, but in general terms, uncalibrated
-            data will be signed integers and calibrated data will be
-            floating-point numbers.
-        median_before:
-            The median of the read previous to this read. intended to
-            allow querying of the approximate level of this read, comapred
-            to the last.  For example, a user could try to verify this is
-            a strand be ensuring the median of the current read is lower
-            than the median_before level.
-        median:
-            The media pA level of this read from all aggregated read
-            chunks so far.
-        previous_read_classification:
-            The classification of the chunk prior to this read starting.
-        previous_read_end_reason:
-            The classification of the chunk prior to this read starting.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsResponse.ReadData)
-    })
-  ,
-
-  'ActionResponse' : _reflection.GeneratedProtocolMessageType('ActionResponse', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSRESPONSE_ACTIONRESPONSE,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsResponse.ActionResponse)
-    })
-  ,
-
-  'ChannelsEntry' : _reflection.GeneratedProtocolMessageType('ChannelsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _GETLIVEREADSRESPONSE_CHANNELSENTRY,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsResponse.ChannelsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _GETLIVEREADSRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      samples_since_start:
-          The number of samples collected before the first sample
-          included in this response.  This gives the position of the
-          first data point on each channel in the overall stream of data
-          being acquired from the device (since this period of data
-          acquisition was started).
-      seconds_since_start:
-          The number of seconds elapsed since data acquisition started.
-          This is the same as ``samples_since_start``, but expressed in
-          seconds.
-      channels:
-          In progress reads for the requested channels.  Sparsely
-          populated as not all channels have new/incomplete reads.
-      action_responses:
-          List of responses to requested actions, informing the caller
-          of results to requested unblocks or discards of data.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetLiveReadsResponse)
-  })
-_sym_db.RegisterMessage(GetLiveReadsResponse)
-_sym_db.RegisterMessage(GetLiveReadsResponse.ReadData)
-_sym_db.RegisterMessage(GetLiveReadsResponse.ActionResponse)
-_sym_db.RegisterMessage(GetLiveReadsResponse.ChannelsEntry)
-
-ResetChannelStatesRequest = _reflection.GeneratedProtocolMessageType('ResetChannelStatesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _RESETCHANNELSTATESREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.data.ResetChannelStatesRequest)
-  })
-_sym_db.RegisterMessage(ResetChannelStatesRequest)
-
-ResetChannelStatesResponse = _reflection.GeneratedProtocolMessageType('ResetChannelStatesResponse', (_message.Message,), {
-  'DESCRIPTOR' : _RESETCHANNELSTATESRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.data.ResetChannelStatesResponse)
-  })
-_sym_db.RegisterMessage(ResetChannelStatesResponse)
-
-GetReadStatisticsRequest = _reflection.GeneratedProtocolMessageType('GetReadStatisticsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETREADSTATISTICSREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      channels:
-          List of channels required, indexed from 1.
-      duration:
-          How long to collect the statistics for
-      no_current_statistics:
-          Disable current_statistics results in returned data.  Intended
-          for use when the consumer doesn't need specific fields
-          allowing the implementation to be more efficient.
-      no_chunk_statistics:
-          Disable chunk_statistics results in returned data.  Intended
-          for use when the consumer doesn't need specific fields
-          allowing the implementation to be more efficient.
-      required_classifications:
-          Specify classifications which the user wants information
-          about.  The default behaviour (when empty) is to return
-          information on all classifications.  Specifying which
-          classifications the user needs information about may allow the
-          implementation to be more efficient.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsRequest)
-  })
-_sym_db.RegisterMessage(GetReadStatisticsRequest)
-
-GetReadStatisticsResponse = _reflection.GeneratedProtocolMessageType('GetReadStatisticsResponse', (_message.Message,), {
-
-  'Statistics' : _reflection.GeneratedProtocolMessageType('Statistics', (_message.Message,), {
-    'DESCRIPTOR' : _GETREADSTATISTICSRESPONSE_STATISTICS,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        q_5:
-             Quantiles (percentiles)
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsResponse.Statistics)
-    })
-  ,
-
-  'ChunkStatistics' : _reflection.GeneratedProtocolMessageType('ChunkStatistics', (_message.Message,), {
-    'DESCRIPTOR' : _GETREADSTATISTICSRESPONSE_CHUNKSTATISTICS,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        median_sd:
-            Aggregated median_sd value from all classified reads. Computed
-            as median(median_sd[...])
-        median:
-            Aggregated median_sd value from all classified reads.
-            Computed as median(median[...])
-        range:
-            Aggregated range value from all classified reads.  Computed as
-            median(q90[...] - q10[...])
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsResponse.ChunkStatistics)
-    })
-  ,
-
-  'PerClassificationData' : _reflection.GeneratedProtocolMessageType('PerClassificationData', (_message.Message,), {
-    'DESCRIPTOR' : _GETREADSTATISTICSRESPONSE_PERCLASSIFICATIONDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        duration_statistics:
-            Statistics of read (chunk) durations. These will be in the
-            same units as the requested duration (if you ask for X seconds
-            of data, you will get durations back in seconds, but if you
-            ask for X samples of data, you will get durations back in
-            samples).  NB: statistics may be estimates.
-        current_statistics:
-            Statistics for all current (signal) values for all reads under
-            this channel/configuration/classification combination.  NB:
-            Statistics are calculated from raw data.
-        chunk_statistics:
-            Statistics generated from the analysed read chunks (or
-            complete reads), rather than the raw signal.
-        samples_duration:
-            The number of samples seen with this classification on this
-            channel in this channel configuration.
-        seconds_duration:
-            The number of seconds spent in this classification on this
-            channel in this channel configuration.  This is the same as
-            ``samples_duration``, but expressed in seconds.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsResponse.PerClassificationData)
-    })
-  ,
-
-  'PerConfigurationData' : _reflection.GeneratedProtocolMessageType('PerConfigurationData', (_message.Message,), {
-
-    'ClassificationsEntry' : _reflection.GeneratedProtocolMessageType('ClassificationsEntry', (_message.Message,), {
-      'DESCRIPTOR' : _GETREADSTATISTICSRESPONSE_PERCONFIGURATIONDATA_CLASSIFICATIONSENTRY,
-      '__module__' : 'minknow_api.data_pb2'
-      # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsResponse.PerConfigurationData.ClassificationsEntry)
-      })
-    ,
-    'DESCRIPTOR' : _GETREADSTATISTICSRESPONSE_PERCONFIGURATIONDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        channel_configuration:
-            The channel configuration active during the reads these
-            statistics were gathered for.
-        classifications:
-            Map from classification names to statistics about read
-            (chunks) with that classification.
-        incomplete:
-            If statistics about complete reads were requested, this field
-            may contain data for a final, incomplete read (whose
-            classification is therefore unknown).  This field will not be
-            set if read chunks were requested, or if the data capture
-            happened to end at a complete read boundary.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsResponse.PerConfigurationData)
-    })
-  ,
-
-  'PerChannelData' : _reflection.GeneratedProtocolMessageType('PerChannelData', (_message.Message,), {
-    'DESCRIPTOR' : _GETREADSTATISTICSRESPONSE_PERCHANNELDATA,
-    '__module__' : 'minknow_api.data_pb2'
-    ,
-    '__doc__': """Attributes:
-        configurations:
-            Data for each channel configuration seen on this channel.
-            Note that each channel configuration will only appear once in
-            this list, and this list is *not* in any way ordered by time.
-            The only reason it is not a map is because of restrictions on
-            map key types.
-        samples_since_start:
-            The number of samples collected before this channel's first
-            sample.
-        seconds_since_start:
-            The number of seconds elapsed since data acquisition started.
-            This is the same as ``samples_since_start``, but expressed in
-            seconds.
-        samples_duration:
-            The number of samples collected for this channel.
-        seconds_duration:
-            The number of seconds of data captured for this session.  This
-            is the same as ``samples_duration``, but expressed in seconds.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsResponse.PerChannelData)
-    })
-  ,
-  'DESCRIPTOR' : _GETREADSTATISTICSRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      channels:
-          Data for each requested channel, in the same order as
-          requested.
-      samples_since_start:
-          The number of samples collected before the first sample
-          included in this response.  This gives the position of the
-          first data point which all channels share in the calculated
-          statistics. Each individual channel may have samples from read
-          chunks previous to this sample due to read boundaries not
-          being consistent across channels.
-      seconds_since_start:
-          The number of seconds elapsed before the first sample included
-          in this response.  This is the same as
-          ``samples_since_start``, but expressed in seconds.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetReadStatisticsResponse)
-  })
-_sym_db.RegisterMessage(GetReadStatisticsResponse)
-_sym_db.RegisterMessage(GetReadStatisticsResponse.Statistics)
-_sym_db.RegisterMessage(GetReadStatisticsResponse.ChunkStatistics)
-_sym_db.RegisterMessage(GetReadStatisticsResponse.PerClassificationData)
-_sym_db.RegisterMessage(GetReadStatisticsResponse.PerConfigurationData)
-_sym_db.RegisterMessage(GetReadStatisticsResponse.PerConfigurationData.ClassificationsEntry)
-_sym_db.RegisterMessage(GetReadStatisticsResponse.PerChannelData)
-
-LockChannelStatesRequest = _reflection.GeneratedProtocolMessageType('LockChannelStatesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LOCKCHANNELSTATESREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      channels:
-          The channels that we want to 'deactivate' = set them to the
-          given state until we re-activate them with
-          unlock_channel_states If the channels are already deactivated,
-          it will update the state to the new forced state given (if
-          different). Channels are indexed from 1.
-      state_name:
-          Channel state name as specified in the channel state
-          configuration. It HAS to be different to 'unclassified', which
-          denotes that the channel is active, but had not met any
-          successful criteria yet.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.LockChannelStatesRequest)
-  })
-_sym_db.RegisterMessage(LockChannelStatesRequest)
-
-LockChannelStatesResponse = _reflection.GeneratedProtocolMessageType('LockChannelStatesResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LOCKCHANNELSTATESRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.data.LockChannelStatesResponse)
-  })
-_sym_db.RegisterMessage(LockChannelStatesResponse)
-
-UnlockChannelStatesRequest = _reflection.GeneratedProtocolMessageType('UnlockChannelStatesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNLOCKCHANNELSTATESREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  ,
-  '__doc__': """Attributes:
-      channels:
-          The channels to activate (active = they will be considered for
-          channel state evaluation in the future). Channels are indexed
-          from 1.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.data.UnlockChannelStatesRequest)
-  })
-_sym_db.RegisterMessage(UnlockChannelStatesRequest)
-
-UnlockChannelStatesResponse = _reflection.GeneratedProtocolMessageType('UnlockChannelStatesResponse', (_message.Message,), {
-  'DESCRIPTOR' : _UNLOCKCHANNELSTATESRESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.data.UnlockChannelStatesResponse)
-  })
-_sym_db.RegisterMessage(UnlockChannelStatesResponse)
-
-GetExperimentYieldInfoRequest = _reflection.GeneratedProtocolMessageType('GetExperimentYieldInfoRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETEXPERIMENTYIELDINFOREQUEST,
-  '__module__' : 'minknow_api.data_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoRequest)
-  })
-_sym_db.RegisterMessage(GetExperimentYieldInfoRequest)
-
-GetExperimentYieldInfoResponse = _reflection.GeneratedProtocolMessageType('GetExperimentYieldInfoResponse', (_message.Message,), {
-
-  'CompleteReadInfo' : _reflection.GeneratedProtocolMessageType('CompleteReadInfo', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_COMPLETEREADINFO,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.CompleteReadInfo)
-    })
-  ,
-
-  'AcquisitionInfo' : _reflection.GeneratedProtocolMessageType('AcquisitionInfo', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_ACQUISITIONINFO,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.AcquisitionInfo)
-    })
-  ,
-
-  'AnalyserInfo' : _reflection.GeneratedProtocolMessageType('AnalyserInfo', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_ANALYSERINFO,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.AnalyserInfo)
-    })
-  ,
-
-  'BulkInfo' : _reflection.GeneratedProtocolMessageType('BulkInfo', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_BULKINFO,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.BulkInfo)
-    })
-  ,
-
-  'HdfWriterInfo' : _reflection.GeneratedProtocolMessageType('HdfWriterInfo', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_HDFWRITERINFO,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.HdfWriterInfo)
-    })
-  ,
-
-  'BasecallStatistics' : _reflection.GeneratedProtocolMessageType('BasecallStatistics', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_BASECALLSTATISTICS,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.BasecallStatistics)
-    })
-  ,
-
-  'HdfMultiReadWritingStatistics' : _reflection.GeneratedProtocolMessageType('HdfMultiReadWritingStatistics', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_HDFMULTIREADWRITINGSTATISTICS,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.HdfMultiReadWritingStatistics)
-    })
-  ,
-
-  'FastqReadWritingStatistics' : _reflection.GeneratedProtocolMessageType('FastqReadWritingStatistics', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_FASTQREADWRITINGSTATISTICS,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.FastqReadWritingStatistics)
-    })
-  ,
-
-  'ProtobufReadWritingStatistics' : _reflection.GeneratedProtocolMessageType('ProtobufReadWritingStatistics', (_message.Message,), {
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_PROTOBUFREADWRITINGSTATISTICS,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.ProtobufReadWritingStatistics)
-    })
-  ,
-
-  'FileOperationQueueProgress' : _reflection.GeneratedProtocolMessageType('FileOperationQueueProgress', (_message.Message,), {
-
-    'FileTypeInfo' : _reflection.GeneratedProtocolMessageType('FileTypeInfo', (_message.Message,), {
-      'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS_FILETYPEINFO,
-      '__module__' : 'minknow_api.data_pb2'
-      # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.FileOperationQueueProgress.FileTypeInfo)
-      })
-    ,
-    'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS,
-    '__module__' : 'minknow_api.data_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse.FileOperationQueueProgress)
-    })
-  ,
-  'DESCRIPTOR' : _GETEXPERIMENTYIELDINFORESPONSE,
-  '__module__' : 'minknow_api.data_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.data.GetExperimentYieldInfoResponse)
-  })
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.CompleteReadInfo)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.AcquisitionInfo)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.AnalyserInfo)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.BulkInfo)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.HdfWriterInfo)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.BasecallStatistics)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.HdfMultiReadWritingStatistics)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.FastqReadWritingStatistics)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.ProtobufReadWritingStatistics)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.FileOperationQueueProgress)
-_sym_db.RegisterMessage(GetExperimentYieldInfoResponse.FileOperationQueueProgress.FileTypeInfo)
-
-_DATASERVICE = DESCRIPTOR.services_by_name['DataService']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.data_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
   _GETCHANNELSTATESREQUEST.fields_by_name['first_channel']._options = None
   _GETCHANNELSTATESREQUEST.fields_by_name['first_channel']._serialized_options = b'\210\265\030\001'
   _GETCHANNELSTATESREQUEST.fields_by_name['last_channel']._options = None
@@ -1107,8 +172,480 @@
   _GETEXPERIMENTYIELDINFORESPONSE_PROTOBUFREADWRITINGSTATISTICS._serialized_end=9147
   _GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS._serialized_start=9150
   _GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS._serialized_end=9698
   _GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS_FILETYPEINFO._serialized_start=9587
   _GETEXPERIMENTYIELDINFORESPONSE_FILEOPERATIONQUEUEPROGRESS_FILETYPEINFO._serialized_end=9698
   _DATASERVICE._serialized_start=9701
   _DATASERVICE._serialized_end=10864
+GetLiveReadsRequest.UnblockAction.__doc__ = """Attributes:
+    duration:
+        Duration of unblock in seconds.
+"""
+LockChannelStatesRequest.__doc__ = """Attributes:
+    channels:
+        The channels that we want to 'deactivate' = set them to the
+        given state until we re-activate them with
+        unlock_channel_states If the channels are already deactivated,
+        it will update the state to the new forced state given (if
+        different). Channels are indexed from 1.
+    state_name:
+        Channel state name as specified in the channel state
+        configuration. It HAS to be different to 'unclassified', which
+        denotes that the channel is active, but had not met any
+        successful criteria yet.
+"""
+GetSignalMinMaxResponse.ChannelData.__doc__ = """Attributes:
+    calibrated_minima:
+        The minimum value for each window.  The type of the elements
+        will depend on whether calibrated data was chosen.
+        Uncalibrated data will be signed integers and calibrated data
+        will be floating-point numbers.  It would be nice to use the
+        "oneof" enum-like type to capture this, but you can't have
+        repeated members in a oneof, and nor can you have a repeated
+        oneof field.  We can simply include message fields for both
+        types of data, as all fields are optional in proto3.  We will
+        rely on the code that constructs this message to guarantee
+        that we don't try and put both types of data into the same
+        message.  Calibrated data is in picoamps. Uncalibrated data is
+        the raw values output by the device's ADC (analogue-digital
+        converter).  This is guaranteed to be the same size as the
+        respective foo_maxima field.
+    calibrated_maxima:
+        The maximum value for each window.  See comments for the
+        "minima" fields above for details of calibrated and
+        uncalibrated data.  This is guaranteed to be the same size as
+        the respective foo_minima field.
+"""
+GetReadStatisticsRequest.__doc__ = """Attributes:
+    channels:
+        List of channels required, indexed from 1.
+    duration:
+        How long to collect the statistics for
+    no_current_statistics:
+        Disable current_statistics results in returned data.  Intended
+        for use when the consumer doesn't need specific fields
+        allowing the implementation to be more efficient.
+    no_chunk_statistics:
+        Disable chunk_statistics results in returned data.  Intended
+        for use when the consumer doesn't need specific fields
+        allowing the implementation to be more efficient.
+    required_classifications:
+        Specify classifications which the user wants information
+        about.  The default behaviour (when empty) is to return
+        information on all classifications.  Specifying which
+        classifications the user needs information about may allow the
+        implementation to be more efficient.
+"""
+GetLiveReadsResponse.ReadData.__doc__ = """Attributes:
+    id:
+        The id of this read, this id is unique for every read ever
+        produced.
+    number:
+        The minknow assigned number of this read  Read numbers always
+        increment throughout the experiment, and are unique per
+        channel - however they are not necessarily contiguous.
+    start_sample:
+        Absolute start point of this read
+    chunk_start_sample:
+        Absolute start point through the experiment of this chunk
+    chunk_length:
+        Length of the chunk in samples
+    chunk_classifications:
+        All Classifications given to intermediate chunks by analysis
+        See analysis_configuration.get_read_classifications for how to
+        map these integers to names.
+    raw_data:
+        Any raw data selected by the request  The type of the elements
+        will depend on whether calibrated data was chosen. The
+        get_data_types() RPC call should be used to determine the
+        precise format of the data, but in general terms, uncalibrated
+        data will be signed integers and calibrated data will be
+        floating-point numbers.
+    median_before:
+        The median of the read previous to this read. intended to
+        allow querying of the approximate level of this read, comapred
+        to the last.  For example, a user could try to verify this is
+        a strand be ensuring the median of the current read is lower
+        than the median_before level.
+    median:
+        The media pA level of this read from all aggregated read
+        chunks so far.
+    previous_read_classification:
+        The classification of the chunk prior to this read starting.
+    previous_read_end_reason:
+        The classification of the chunk prior to this read starting.
+"""
+GetReadStatisticsResponse.ChunkStatistics.__doc__ = """Attributes:
+    median_sd:
+        Aggregated median_sd value from all classified reads. Computed
+        as median(median_sd[...])
+    median:
+        Aggregated median_sd value from all classified reads.
+        Computed as median(median[...])
+    range:
+        Aggregated range value from all classified reads.  Computed as
+        median(q90[...] - q10[...])
+"""
+GetReadStatisticsResponse.PerChannelData.__doc__ = """Attributes:
+    configurations:
+        Data for each channel configuration seen on this channel.
+        Note that each channel configuration will only appear once in
+        this list, and this list is *not* in any way ordered by time.
+        The only reason it is not a map is because of restrictions on
+        map key types.
+    samples_since_start:
+        The number of samples collected before this channel's first
+        sample.
+    seconds_since_start:
+        The number of seconds elapsed since data acquisition started.
+        This is the same as ``samples_since_start``, but expressed in
+        seconds.
+    samples_duration:
+        The number of samples collected for this channel.
+    seconds_duration:
+        The number of seconds of data captured for this session.  This
+        is the same as ``samples_duration``, but expressed in seconds.
+"""
+GetReadStatisticsResponse.__doc__ = """Attributes:
+    channels:
+        Data for each requested channel, in the same order as
+        requested.
+    samples_since_start:
+        The number of samples collected before the first sample
+        included in this response.  This gives the position of the
+        first data point which all channels share in the calculated
+        statistics. Each individual channel may have samples from read
+        chunks previous to this sample due to read boundaries not
+        being consistent across channels.
+    seconds_since_start:
+        The number of seconds elapsed before the first sample included
+        in this response.  This is the same as
+        ``samples_since_start``, but expressed in seconds.
+"""
+GetChannelStatesResponse.__doc__ = """Attributes:
+    channel_states:
+        The streamed data for all channels will be appended to this
+        vector. After the request is made, all the channel state
+        changes are streamed through this array. This is implemented
+        in the idea of a sparse array because we can have channels
+        that remain in the same state for a long time.
+"""
+GetDataTypesResponse.DataType.__doc__ = """Attributes:
+    type:
+        The basic type of the data item.
+    big_endian:
+        Whether the type is big-endian (high-byte first).  For numeric
+        data types, if this is not set, they are little-endian (low-
+        byte first).
+    size:
+        The size of the data type in bytes.
+"""
+GetReadStatisticsResponse.Statistics.__doc__ = """Attributes:
+    q_5:
+         Quantiles (percentiles)
+"""
+GetLiveReadsResponse.__doc__ = """Attributes:
+    samples_since_start:
+        The number of samples collected before the first sample
+        included in this response.  This gives the position of the
+        first data point on each channel in the overall stream of data
+        being acquired from the device (since this period of data
+        acquisition was started).
+    seconds_since_start:
+        The number of seconds elapsed since data acquisition started.
+        This is the same as ``samples_since_start``, but expressed in
+        seconds.
+    channels:
+        In progress reads for the requested channels.  Sparsely
+        populated as not all channels have new/incomplete reads.
+    action_responses:
+        List of responses to requested actions, informing the caller
+        of results to requested unblocks or discards of data.
+"""
+GetLiveReadsRequest.Action.__doc__ = """Attributes:
+    channel:
+        Channel name to unblock
+    read:
+        Identifier for the read to act on.  If the read requested is
+        no longer in progress, the action fails.
+    unblock:
+        Unblock a read and skip further data from this read.
+    stop_further_data:
+        Skip further data from this read, doesn't affect the read
+        data.
+"""
+GetReadStatisticsResponse.PerClassificationData.__doc__ = """Attributes:
+    duration_statistics:
+        Statistics of read (chunk) durations. These will be in the
+        same units as the requested duration (if you ask for X seconds
+        of data, you will get durations back in seconds, but if you
+        ask for X samples of data, you will get durations back in
+        samples).  NB: statistics may be estimates.
+    current_statistics:
+        Statistics for all current (signal) values for all reads under
+        this channel/configuration/classification combination.  NB:
+        Statistics are calculated from raw data.
+    chunk_statistics:
+        Statistics generated from the analysed read chunks (or
+        complete reads), rather than the raw signal.
+    samples_duration:
+        The number of samples seen with this classification on this
+        channel in this channel configuration.
+    seconds_duration:
+        The number of seconds spent in this classification on this
+        channel in this channel configuration.  This is the same as
+        ``samples_duration``, but expressed in seconds.
+"""
+GetDataTypesResponse.__doc__ = """Attributes:
+    uncalibrated_signal:
+        The format of the uncalibrated (ADC) signal data returned by
+        get_raw_signal_bytes().  In the current release, this will
+        describe 16-bit little-endian integers.
+    calibrated_signal:
+        The format of the calibrated (picoamp) signal data returned by
+        get_raw_signal_bytes().  In the current release, this will
+        describe 32-bit IEEE 754 floating point values.
+    bias_voltages:
+        The format of the bias voltage data returned by
+        get_raw_signal_bytes().  In the current release, this will
+        describe 16-bit little-endian integers.
+"""
+UnlockChannelStatesRequest.__doc__ = """Attributes:
+    channels:
+        The channels to activate (active = they will be considered for
+        channel state evaluation in the future). Channels are indexed
+        from 1.
+"""
+GetSignalBytesResponse.__doc__ = """Attributes:
+    samples_since_start:
+        The number of samples collected before the first sample
+        included in this response.  This gives the position of the
+        first data point on each channel in the overall stream of data
+        being acquired from the device (since this period of data
+        acquisition was started).
+    seconds_since_start:
+        The number of seconds elapsed since data acquisition started.
+        This is the same as ``samples_since_start``, but expressed in
+        seconds.
+    skipped_channels:
+        The number of channels omitted at the start of the
+        ``channels`` array.
+    channels:
+        The signal for each requested channel.  Note that
+        ``skipped_channels`` must be used to determine which channels
+        are given here, as not all channels will be included in every
+        message. The channels that are provided are contiguous and in
+        order, with the first channel being ``first_channel +
+        skipped_channels`` (where ``first_channel`` is from the
+        request message).
+    bias_voltages:
+        The bias voltages set for each sample.  If bias voltages were
+        requested, this will provide voltage data, one voltage per
+        sample. Note that not every message may include bias_voltages
+        (they will generally be included when ``skipped_channels`` is
+        0, but that is not guaranteed).  The get_data_types() RPC call
+        should be used to determine the format of the data.
+"""
+GetSignalMinMaxResponse.__doc__ = """Attributes:
+    samples_since_start:
+        The number of samples collected before the first sample
+        included in this response.  This gives the position of the
+        first data point on each channel in the overall stream of data
+        being acquired from the device (since this period of data
+        acquisition was started).
+    seconds_since_start:
+        The number of seconds elapsed since data acquisition started.
+        This is the same as ``samples_since_start``, but expressed in
+        seconds.
+    skipped_channels:
+        The number of channels omitted at the start of the
+        ``channels`` array.
+    channels:
+        The window bounds for each requested channel.  Note that
+        ``skipped_channels`` must be used to determine which channels
+        are given here, as not all channels will be included in every
+        message. The channels that are provided are contiguous and in
+        order, with the first channel being ``first_channel +
+        skipped_channels`` (where ``first_channel`` is from the
+        request message).
+"""
+GetSignalMinMaxRequest.__doc__ = """Attributes:
+    first_channel:
+        The first channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    last_channel:
+        The last channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    window_size:
+        The size of window to summarise.  A value of zero will be
+        rejected; there is no default.
+    calibrated_data:
+        Whether the data should be calibrated.
+"""
+GetLiveReadsRequest.__doc__ = """Attributes:
+    setup:
+        Read setup request, initialises channel numbers and type of
+        data returned.  note: Must be specified in the first message
+        sent to MinKNOW. Once MinKNOW has the first setup message
+        reads are sent to the caller as requested. The user can then
+        resend a setup message as frequently as they need to in order
+        to reconfigure live reads - for example by changing if raw
+        data is sent with reads or not.
+    actions:
+        Actions to take given data returned to the user - can only be
+        sent once the setup message above has been sent.
+"""
+GetSignalBytesRequest.__doc__ = """Attributes:
+    length:
+        The amount of data to return.  If this is omitted, data will
+        be streamed until the call is cancelled.
+    seconds:
+        The amount of data to return in seconds.  The number of
+        samples returned will be just enough to cover this period of
+        time. Cannot be specified at the same time as ``samples``.
+    samples:
+        The amount of data to return in samples.  The result will
+        contain exactly this many samples. If this is not possible,
+        the call will fail. Cannot be specified at the same time as
+        ``seconds``.
+    first_channel:
+        The first channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    last_channel:
+        The last channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    include_channel_configs:
+        Whether to include channel configuration settings.
+    include_bias_voltages:
+        Whether to include bias voltage information.
+    calibrated_data:
+        Whether the data should be calibrated.
+    return_when_listening:
+        When this value is set to true, then an empty message will be
+        sent back to the client to indicate that the backend has
+        acknowleged the request, and that any calls made that will
+        affect the signal after that initial  response will be
+        reflected in the next messages
+"""
+GetChannelStatesResponse.ChannelStateData.__doc__ = """Attributes:
+    channel:
+        Represents the channel number, indexed from one. (i.e. what
+        channel did the channel state change happened on)
+    state:
+        depending on the channel state request, MinKNOW can fill in
+        either the name or the criteria id of the channel state. The
+        criteria id (or state_id) is the number passed in the channel
+        states configuration. Note that MinKNOW also has some default
+        channel states (like unclassified, pending mux change) which
+        receive unique ids - these are numbers bigger than 200.
+    acquisition_raw_index:
+        Indices of when the channel state was first seen. For example,
+        if a request is done half way through the experiment, the
+        first message will contain the current state on the requested
+        channels. The acquisition/analysis index of these would be
+        from when the channel states were set. These are exactly the
+        same numbers we see in the bulk file, in the 'states' table
+    config:
+        Channel config (mux state) the channel state was determined
+        on.
+"""
+GetSignalBytesResponse.ChannelConfigChange.__doc__ = """Attributes:
+    config:
+        The new channel configuration.
+    offset:
+        The offset in the returned data where the change was applied.
+"""
+GetSignalBytesResponse.ChannelData.__doc__ = """Attributes:
+    data:
+        The signal data.  This is the byte representation of a C-style
+        array of values. Values are stored in order and adjacent to
+        each other.  The type of the elements will depend on whether
+        calibrated data was chosen. The get_data_types() RPC call
+        should be used to determine the precise format of the data,
+        but in general terms, uncalibrated data will be signed
+        integers and calibrated data will be floating-point numbers.
+        Returning the data in this format allows it to be efficiently
+        processed in dynamic languages that can pass the data straight
+        down to a native runtime. For example, in Python, this data
+        can be intepreted directly into a numpy array using
+        numpy.fromstring().  Calibrated data is in picoamps.
+        Uncalibrated data is the raw values output by the device's ADC
+        (analogue-digital converter).
+    config_changes:
+        The configuration changes on the channel during data
+        collection.  If channel configuration changes were requested,
+        this will contain all the channel configuration changes that
+        affect the returned data. This will include at least one
+        element, with offset 0, that describes the configuration at
+        the time the first sample was taken.  Note that the offset is
+        the zero-based index into the adc or picoamps list.  The
+        changes will be ordered by offset.
+"""
+GetChannelStatesRequest.__doc__ = """Attributes:
+    first_channel:
+        The first channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    last_channel:
+        The last channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    use_channel_states_ids:
+        If this is true, the returned messages will contain the
+        channel state id as opposed to the name. By default, the
+        response will contain channel states names.
+    wait_for_processing:
+        If `wait_for_processing` is true, then get_channel_states will
+        wait until minknow starts acquiring data instead of returning
+        with an error  Defaults to false
+    heartbeat:
+        Ensure the stream sends a message at least this often.  There
+        will usually be multiple channel updates a second, but in some
+        circumstances (eg: a flow cell with no sample loaded) there
+        can be long periods of time without updates.  Setting this
+        value will ensure that if this period of time passes without
+        there being any channel state changes to report, an empty
+        message will be sent. This can be useful to force a minimum
+        wakeup interval in the client code.
+"""
+GetReadStatisticsResponse.PerConfigurationData.__doc__ = """Attributes:
+    channel_configuration:
+        The channel configuration active during the reads these
+        statistics were gathered for.
+    classifications:
+        Map from classification names to statistics about read
+        (chunks) with that classification.
+    incomplete:
+        If statistics about complete reads were requested, this field
+        may contain data for a final, incomplete read (whose
+        classification is therefore unknown).  This field will not be
+        set if read chunks were requested, or if the data capture
+        happened to end at a complete read boundary.
+"""
+GetLiveReadsRequest.StreamSetup.__doc__ = """Attributes:
+    first_channel:
+        The first channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    last_channel:
+        The last channel (inclusive) to return data for.  Note that
+        channel numbering starts at 1.
+    raw_data_type:
+        Specify the type of raw data to retrieve
+    sample_minimum_chunk_size:
+        Minimum chunk size read data is returned in.
+    max_unblock_read_length:
+        Maximum read length MinKNOW will attempt to unblock reads
+        beyond this length will not be unblocked when Action's
+        request, instead minknow will skip any further data from the
+        read.
+    max_unblock_read_length_samples:
+        Maximum read length MinKNOW will attempt to unblock (in
+        samples).  A value of 0 will cause minknow to unblock reads of
+        any length.
+    max_unblock_read_length_seconds:
+        Maximum read length MinKNOW will attempt to unblock (in
+        seconds).  A value of 0.0 will cause minknow to unblock reads
+        of any length.
+    accepted_first_chunk_classifications:
+        A set of classification identifiers which the client is
+        interested in. If a read starts with a classification not
+        listed here the read is never sent to the client.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/data_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/data_service.py` & `minknow_api-5.5.2/minknow_api/data_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/device.py` & `minknow_api-5.5.2/minknow_api/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     """The type of device."""
 
     MINION = minknow_api.device_service.GetDeviceInfoResponse.MINION
     PROMETHION = minknow_api.device_service.GetDeviceInfoResponse.PROMETHION
     GRIDION = minknow_api.device_service.GetDeviceInfoResponse.GRIDION
     MINION_MK1C = minknow_api.device_service.GetDeviceInfoResponse.MINION_MK1C
     TRAXION = minknow_api.device_service.GetDeviceInfoResponse.TRAXION
+    P2_SOLO = minknow_api.device_service.GetDeviceInfoResponse.P2_SOLO
 
     def is_minion_like(self):
         """Whether the device acts like a MinION.
 
         Among other things, this means it can be used with the ``minion`` RPC service (see
         `minknow_api.minion_service`).
         """
@@ -38,15 +39,15 @@
 
     def is_promethion_like(self):
         """Whether the device acts like a PromethION.
 
         Among other things, this means it can be used with the ``promethion`` RPC service (see
         `minknow_api.prometion_service`).
         """
-        return self in [DeviceType.PROMETHION]
+        return self in [DeviceType.PROMETHION, DeviceType.P2_SOLO]
 
 
 def get_device_type(connection):
     """Get a `DeviceType` enum value from a connection to a flow cell position.
 
     Args:
         connection (minknow_api.Connection): Connection to a MinKNOW flow cell position.
```

### Comparing `minknow_api-5.4.0/minknow_api/device_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/device_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,16 +305,21 @@
         all offsets will be 0, and the pA ranges will be the same as the digitisation.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def set_temperature(self, request, context):
-        """If the device is capable (see GetDeviceInfoResponse.temperature_controllable)
-        then this sets the minimum and maximum temperatures of the flow-cell.
+        """Set the target primary device temperature
+
+        If the device is not temperature-controllable (see the fields
+        `device.GetDeviceInfoResponse.can_set_temperature` and
+        `minion_device.MinionDeviceSettings.enable_temperature_control`) then this call will have
+        no effect
+
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def get_temperature(self, request, context):
         """Get the current temperature of the device.
```

### Comparing `minknow_api-5.4.0/minknow_api/device_service.py` & `minknow_api-5.5.2/minknow_api/device_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -713,40 +713,80 @@
             raise ArgumentError("Unexpected keyword arguments to get_calibration: '{}'".format(", ".join(unused_args)))
 
         return run_with_retry(self._stub.get_calibration,
                               _message, _timeout,
                               [],
                               "minknow_api.device.DeviceService")
     def set_temperature(self, _message=None, _timeout=None, **kwargs):
-        """If the device is capable (see GetDeviceInfoResponse.temperature_controllable)
-        then this sets the minimum and maximum temperatures of the flow-cell.
+        """Set the target primary device temperature
+
+        If the device is not temperature-controllable (see the fields
+        `device.GetDeviceInfoResponse.can_set_temperature` and
+        `minion_device.MinionDeviceSettings.enable_temperature_control`) then this call will have
+        no effect
 
         This RPC is idempotent. It may change the state of the system, but if the requested
         change has already happened, it will not fail because of this, make any additional
         changes or return a different value.
 
         Args:
             _message (minknow_api.device_pb2.SetTemperatureRequest, optional): The message to send.
                 This can be passed instead of the keyword arguments.
             _timeout (float, optional): The call will be cancelled after this number of seconds
                 if it has not been completed.
             temperature (float, optional): The desired temperature in degrees Celsius.
 
                 If temperature control is supported and enabled, the device will attempt to keep its
-                temperature at this value. See the ``can_set_temperature`` field returned by the
-                DeviceService.get_device_info() RPC.
+                primary temperature at this value. The reading used as the "primary" temperature depends
+                on the device:
+                - For MinIONs, the primary temperature is the heatsink temperature
+                - For PromethIONs, the primary temperature is the flow cell temperature
+
+                (If temperature control is not supported or is not enabled, the call to `set_temperature`
+                will fail with `FAILED_PRECONDITION`)
             wait_for_temperature (minknow_api.device_pb2.SetTemperatureRequest.WaitForTemperatureSettings, optional): Settings which can be specified in order to wait for the temperature to be reached.
 
-                If this is not set at all, not waiting will be done. If it is set (even to an empty
-                WaitForTemperatureSettings object), the call will not return until either the temperature was
-                reached or the timeout was reached. In this case, on MinIONs and GridIONs, the ASIC power
-                will be enabled if it was not already. See acquisition.StopRequest.keep_power_on for more
-                details about the implications of this.
+                If this is not set at all, no waiting will be done. If it is set (even to an empty
+                WaitForTemperatureSettings object), the call will not return until either:
+                - The target temperature was reached, or
+                - The timeout was reached, or
+                - The secondary temperature limits were exceeded
+
+                If `wait_for_temperature` is supplied then, on MinIONs and GridIONs, the ASIC power will be
+                enabled if it was not already. See `acquisition.StopRequest.keep_power_on` for more details
+                about the implications of this.
 
                 Since 1.15
+            secondary_temperature_limits (minknow_api.device_pb2.SetTemperatureRequest.SecondaryTemperatureLimits, optional): Specify "secondary" temperature limits
+
+                This field allows limits to be placed on the "secondary" temperature, while waiting for
+                the primary temperature to reach its target value (as specified in the `temperature` field,
+                above).
+
+                The meaning of the "secondary" temperature depends on the device in question:
+                - For MinIONs, this is the ASIC temperature (i.e. flow cell or flow cell adapter
+                  temperature)
+                - For PromethIONs, this is the "chamber" temperature (which is derived from the measurements
+                  of the ASIC temperature)
+
+                These limits are intended to act as a safeguard against the case where the flow cell does
+                not have good thermal contact with temperature control hardware (e.g. if the flow cell was
+                not fully seated when it was inserted into the device). In such cases, the flow cell
+                temperature may rise high enough to damage the flow cell; these limits may be used to
+                mitigate the risk of the flow cell temperature rising high enough to cause damage to the
+                flow cell.
+
+                If the secondary temperature exceeds the specified limits while waiting for the target
+                temperature to be reached, then all temperature control settings are reset to the values
+                they had prior to the call to `set_temperature()` being made.
+
+                NB - These limits apply ONLY when waiting for the target temperature to be reached; once the
+                call to `set_temperature()` returns, these limits are no longer checked.
+
+                Since 5.5
 
         Returns:
             minknow_api.device_pb2.SetTemperatureResponse
 
         Note that the returned messages are actually wrapped in a type that collapses
         submessages for fields marked with ``[rpc_unwrap]``.
         """
@@ -766,14 +806,18 @@
             unused_args.remove("temperature")
             _message.temperature = kwargs['temperature']
 
         if "wait_for_temperature" in kwargs:
             unused_args.remove("wait_for_temperature")
             _message.wait_for_temperature.CopyFrom(kwargs['wait_for_temperature'])
 
+        if "secondary_temperature_limits" in kwargs:
+            unused_args.remove("secondary_temperature_limits")
+            _message.secondary_temperature_limits.CopyFrom(kwargs['secondary_temperature_limits'])
+
         if len(unused_args) > 0:
             raise ArgumentError("Unexpected keyword arguments to set_temperature: '{}'".format(", ".join(unused_args)))
 
         return run_with_retry(self._stub.set_temperature,
                               _message, _timeout,
                               [],
                               "minknow_api.device.DeviceService")
```

### Comparing `minknow_api-5.4.0/minknow_api/examples/export_to_csv.py` & `minknow_api-5.5.2/minknow_api/examples/export_to_csv.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/examples/extract_run_statistics.py` & `minknow_api-5.5.2/minknow_api/examples/extract_run_statistics.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/examples/list_sequencing_positions.py` & `minknow_api-5.5.2/minknow_api/examples/list_sequencing_positions.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/examples/load_sample_sheet.py` & `minknow_api-5.5.2/minknow_api/examples/load_sample_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,37 +254,37 @@
     # Handle the barcoding fields
     # Barcoding data is a map of `some barcode id` -> `alias / type`
 
     if "barcode_info" not in data:
         data["barcode_info"] = {}
 
     if "barcode" in record:
-        if not re.match("barcode(\d{2})", record["barcode"]):
+        if not re.match(r"barcode(\d{2})", record["barcode"]):
             raise SampleSheetParseError(
                 "Line {}: Bad 'barcode' name '{}'; ".format(line_num, record["barcode"])
                 + "expected a name like 'barcode01'"
             )
 
         barcode_name = record["barcode"]
         barcode_name_internal = None
         lamp_barcode_id = None
         barcode_key = barcode_name
 
     elif ("internal_barcode" in record) and ("external_barcode" in record):
         external_barcode = record["external_barcode"]
         internal_barcode = record["internal_barcode"]
 
-        if not re.match("internal(\d{2})", internal_barcode):
+        if not re.match(r"internal(\d{2})", internal_barcode):
             raise SampleSheetParseError(
                 "Line {}: Bad 'internal_barcode' name '{}'; ".format(
                     line_num, internal_barcode
                 )
                 + "expected a name like 'internal01'"
             )
-        if not re.match("external(\d{2})", external_barcode):
+        if not re.match(r"external(\d{2})", external_barcode):
             raise SampleSheetParseError(
                 "Line {}: Bad 'external_barcode' name '{}'; ".format(
                     line_num, external_barcode
                 )
                 + "expected a name like 'external01'"
             )
 
@@ -293,23 +293,23 @@
         lamp_barcode_id = None
         barcode_key = (external_barcode, internal_barcode)
 
     elif ("rapid_barcode" in record) and ("fip_barcode" in record):
         rapid_barcode = record["rapid_barcode"]
         fip_barcode = record["fip_barcode"]
 
-        if not re.match("barcode(\d{2})", rapid_barcode):
+        if not re.match(r"barcode(\d{2})", rapid_barcode):
             raise SampleSheetParseError(
                 "Line {}: Bad 'rapid_barcode' name '{}'; ".format(
                     line_num, rapid_barcode
                 )
                 + "expected a name like 'barcode01'"
             )
 
-        if not re.match("FIP(\d{2})", fip_barcode):
+        if not re.match(r"FIP(\d{2})", fip_barcode):
             raise SampleSheetParseError(
                 "Line {}: Bad 'fip_barcode' name '{}'; ".format(line_num, fip_barcode)
                 + "expected a name like 'FIP01'"
             )
 
         barcode_name = rapid_barcode
         barcode_name_internal = None
```

### Comparing `minknow_api-5.4.0/minknow_api/examples/run_after_protocol.py` & `minknow_api-5.5.2/minknow_api/examples/run_after_protocol.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/examples/start_protocol.py` & `minknow_api-5.5.2/minknow_api/examples/start_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import argparse
 import logging
 import sys
 
 # minknow_api.manager supplies "Manager" a wrapper around MinKNOW's Manager gRPC API with utilities
 # for querying sequencing positions + offline basecalling tools.
 from enum import Enum
-from typing import Optional, NamedTuple, Sequence
+from typing import Sequence
 
 from minknow_api.examples.load_sample_sheet import (
     load_sample_sheet_csv,
     SampleSheetParseError,
     ParsedSampleSheetEntry,
 )
 from minknow_api.manager import Manager, FlowCellPosition
@@ -617,29 +617,35 @@
 
         # Set up user specified product code if requested:
         if args.product_code:
             position_connection.device.set_user_specified_product_code(
                 code=args.product_code
             )
 
+        # Generate stop criteria for use by Run Until
+        # The `runtime` is in seconds, while the `experiment_duration` is in hours
+        stop_criteria = protocols.CriteriaValues(
+            runtime=int(args.experiment_duration * 60 * 60)
+        )
+
         run_id = protocols.start_protocol(
             position_connection,
             identifier=spec.protocol_id,
             sample_id=spec.entry.sample_id,
             experiment_group=spec.entry.experiment_id,
             barcode_info=spec.entry.barcode_info,
             basecalling=basecalling_args,
             read_until=read_until_args,
             fastq_arguments=fastq_arguments,
             fast5_arguments=fast5_arguments,
             pod5_arguments=pod5_arguments,
             bam_arguments=bam_arguments,
             disable_active_channel_selection=args.no_active_channel_selection,
             mux_scan_period=args.mux_scan_period,
-            experiment_duration=args.experiment_duration,
+            stop_criteria=stop_criteria,
             args=args.extra_args,  # Any extra args passed.
         )
 
         flow_cell_info = position_connection.device.get_flow_cell_info()
 
         print("Started protocol:")
         print("    run_id={}".format(run_id))
```

### Comparing `minknow_api-5.4.0/minknow_api/instance_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/instance_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/instance_service.py` & `minknow_api-5.5.2/minknow_api/instance_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/keystore_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/keystore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/keystore_service.py` & `minknow_api-5.5.2/minknow_api/keystore_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/log_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/log_service.py` & `minknow_api-5.5.2/minknow_api/log_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/manager.py` & `minknow_api-5.5.2/minknow_api/manager.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/manager_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/manager_service.py` & `minknow_api-5.5.2/minknow_api/manager_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -954,19 +954,31 @@
         Args:
             _message (minknow_api.manager_pb2.AddSimulatedDeviceRequest, optional): The message to send.
                 This can be passed instead of the keyword arguments.
             _timeout (float, optional): The call will be cancelled after this number of seconds
                 if it has not been completed.
             name (str): The name of the position, this must be unique and the correct format:
 
-                For MinIONs and MinION-mk1Cs, "MS" followed by five digits, eg: "MS12345".
-                For GridIONs, "GS" followed by five digits, eg: "GS12345".
-                For P2Solos, "P2S" followed by four digits, eg: "P2S1234".
+                For MinION Mk1B and Mk1C: "MS" followed by five digits, eg: "MS12345".
+                For GridION: "GS" followed by five digits, eg: "GS12345".
+                For P2 Solo: "P2S_" followed by five digits, and then "-A" or "-B" eg: "P2S_12345-A".
 
-                PromethIONs position-names have no format restriction, but must be unique
+                PromethION and P2 Solo position-names have no format restriction, but must be unique. It is
+                strongly recommended to follow standard naming conventions:
+
+                For PromethION: start with "1A" and then increase the number and/or the letter as you add
+                more positions.
+                For P2 Solo: use "P2S_00000-A" and "P2S_00000-B" (these fit the format of real P2 Solo devices,
+                but do not correspond to any real device).
+
+                Future versions might constrain PromethION and P2 Solo device names. Using the above
+                suggestions should ensure that your code will continue to work.
+
+                Note that MinKNOW Core 5.5 and earlier required the P2 Solo device name to be "P2S" followed
+                by four digits. This is no longer recommended.
             type (minknow_api.manager_pb2.SimulatedDeviceType): The type of the simulated device to create.
 
                 If left at default (AUTO), then a sensible default device type is selected.
 
         Returns:
             minknow_api.manager_pb2.AddSimulatedDeviceResponse
```

### Comparing `minknow_api-5.4.0/minknow_api/minion_device_pb2.py` & `minknow_api-5.5.2/minknow_api/minion_device_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,332 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: minknow_api/minion_device.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fminknow_api/minion_device.proto\x12\x19minknow_api.minion_device\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1dminknow_api/rpc_options.proto\",\n\x10TemperatureRange\x12\x0b\n\x03min\x18\x05 \x01(\x02\x12\x0b\n\x03max\x18\x06 \x01(\x02\"\x89\x02\n\x1bSamplingFrequencyParameters\x12\x15\n\rclock_divider\x18\x01 \x01(\r\x12\x18\n\x10integration_time\x18\x02 \x01(\r\x12V\n\x0b\x63lock_speed\x18\x03 \x01(\x0e\x32\x41.minknow_api.minion_device.SamplingFrequencyParameters.ClockSpeed\"a\n\nClockSpeed\x12\x10\n\x0c\x43LOCK_128MHz\x10\x00\x12\x0f\n\x0b\x43LOCK_64MHz\x10\x01\x12\x0f\n\x0b\x43LOCK_32MHz\x10\x02\x12\x0f\n\x0b\x43LOCK_16MHz\x10\x03\x12\x0e\n\nCLOCK_8MHz\x10\x04\"\x88\x16\n\x14MinionDeviceSettings\x12\x31\n\x0c\x62ias_voltage\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x38\n\x12sampling_frequency\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12Z\n\x0e\x63hannel_config\x18\x03 \x03(\x0b\x32\x42.minknow_api.minion_device.MinionDeviceSettings.ChannelConfigEntry\x12>\n\x1a\x65nable_temperature_control\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12G\n\x12temperature_target\x18\x05 \x01(\x0b\x32+.minknow_api.minion_device.TemperatureRange\x12[\n\rint_capacitor\x18\x06 \x01(\x0e\x32\x44.minknow_api.minion_device.MinionDeviceSettings.IntegrationCapacitor\x12\x32\n\x0ctest_current\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x34\n\x0funblock_voltage\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x35\n\x11overcurrent_limit\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x10samples_to_reset\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x45\n\x07th_gain\x18\x0c \x01(\x0e\x32\x34.minknow_api.minion_device.MinionDeviceSettings.Gain\x12\x30\n\nsinc_delay\x18\r \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x33\n\x0eth_sample_time\x18\x0e \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x33\n\x0eint_reset_time\x18\x0f \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12S\n\x0fsinc_decimation\x18\x10 \x01(\x0e\x32:.minknow_api.minion_device.MinionDeviceSettings.Decimation\x12V\n\x0flow_pass_filter\x18\x11 \x01(\x0e\x32=.minknow_api.minion_device.MinionDeviceSettings.LowPassFilter\x12Z\n\x11non_overlap_clock\x18\x12 \x01(\x0e\x32?.minknow_api.minion_device.MinionDeviceSettings.NonOverlapClock\x12\x32\n\x0c\x62ias_current\x18\x13 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12<\n\x16\x63ompensation_capacitor\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12Y\n\x19sampling_frequency_params\x18\x15 \x01(\x0b\x32\x36.minknow_api.minion_device.SamplingFrequencyParameters\x12\x35\n\x11\x65nable_asic_power\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12K\n\tfan_speed\x18\x17 \x01(\x0e\x32\x38.minknow_api.minion_device.MinionDeviceSettings.FanSpeed\x12\x37\n\x13\x61llow_full_fan_stop\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x43\n\x1f\x65nable_soft_temperature_control\x18\x19 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12>\n\x1a\x65nable_bias_voltage_lookup\x18\x1a \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12!\n\x19\x62ias_voltage_lookup_table\x18\x1b \x03(\x05\x1as\n\x12\x43hannelConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12L\n\x05value\x18\x02 \x01(\x0e\x32=.minknow_api.minion_device.MinionDeviceSettings.ChannelConfig:\x02\x38\x01\"-\n\x04Gain\x12\r\n\tGAIN_KEEP\x10\x00\x12\n\n\x06GAIN_1\x10\x01\x12\n\n\x06GAIN_5\x10\x02\"G\n\nDecimation\x12\x13\n\x0f\x44\x45\x43IMATION_KEEP\x10\x00\x12\x11\n\rDECIMATION_32\x10\x01\x12\x11\n\rDECIMATION_64\x10\x02\"y\n\rLowPassFilter\x12\x0c\n\x08LPF_KEEP\x10\x00\x12\x0c\n\x08LPF_5kHz\x10\x01\x12\r\n\tLPF_10kHz\x10\x02\x12\r\n\tLPF_20kHz\x10\x03\x12\r\n\tLPF_40kHz\x10\x04\x12\r\n\tLPF_80kHz\x10\x05\x12\x10\n\x0cLPF_DISABLED\x10\x06\"G\n\x0fNonOverlapClock\x12\x0c\n\x08NOC_KEEP\x10\x00\x12\x12\n\x0eNOC_1_HS_CLOCK\x10\x01\x12\x12\n\x0eNOC_2_HS_CLOCK\x10\x02\"q\n\x14IntegrationCapacitor\x12\x0f\n\x0bINTCAP_KEEP\x10\x00\x12\x11\n\rINTCAP_62_5fF\x10\x01\x12\x10\n\x0cINTCAP_250fF\x10\x02\x12\x0e\n\nINTCAP_1pF\x10\x03\x12\x13\n\x0fINTCAP_1_1875pF\x10\x04\"f\n\x08\x46\x61nSpeed\x12\x11\n\rFANSPEED_KEEP\x10\x00\x12\x10\n\x0c\x46\x41NSPEED_OFF\x10\x01\x12\x10\n\x0c\x46\x41NSPEED_LOW\x10\x02\x12\x11\n\rFANSPEED_HIGH\x10\x03\x12\x10\n\x0c\x46\x41NSPEED_MAX\x10\x04\"\xbd\x03\n\rChannelConfig\x12\x17\n\x13\x43HANNEL_CONFIG_KEEP\x10\x00\x12\x10\n\x0c\x44ISCONNECTED\x10\x01\x12\x17\n\x13WELL_1_BIAS_VOLTAGE\x10\x02\x12\x17\n\x13WELL_2_BIAS_VOLTAGE\x10\x03\x12\x17\n\x13WELL_3_BIAS_VOLTAGE\x10\x04\x12\x17\n\x13WELL_4_BIAS_VOLTAGE\x10\x05\x12\x10\n\x0cTEST_CURRENT\x10\x06\x12\x1a\n\x16WELL_1_UNBLOCK_VOLTAGE\x10\x07\x12\x1a\n\x16WELL_2_UNBLOCK_VOLTAGE\x10\x08\x12\x1a\n\x16WELL_3_UNBLOCK_VOLTAGE\x10\t\x12\x1a\n\x16WELL_4_UNBLOCK_VOLTAGE\x10\n\x12\x1b\n\x17TEST_CURRENT_VIA_WELL_1\x10\x0b\x12\x1b\n\x17TEST_CURRENT_VIA_WELL_2\x10\x0c\x12\x1b\n\x17TEST_CURRENT_VIA_WELL_3\x10\r\x12\x1b\n\x17TEST_CURRENT_VIA_WELL_4\x10\x0e\x12\x1b\n\x17GROUND_THROUGH_RESISTOR\x10\x0f\x12\n\n\x06GROUND\x10\x10\"\xbf\x01\n\x15\x43hangeSettingsRequest\x12G\n\x08settings\x18\x01 \x01(\x0b\x32/.minknow_api.minion_device.MinionDeviceSettingsB\x04\x90\xb5\x18\x01\x12]\n\x16\x63hannel_config_default\x18\x02 \x01(\x0e\x32=.minknow_api.minion_device.MinionDeviceSettings.ChannelConfig\"\x18\n\x16\x43hangeSettingsResponse\"\x14\n\x12GetSettingsRequest\"^\n\x13GetSettingsResponse\x12G\n\x08settings\x18\x01 \x01(\x0b\x32/.minknow_api.minion_device.MinionDeviceSettingsB\x04\x90\xb5\x18\x01\"\x14\n\x12GetFanSpeedRequest\"\"\n\x13GetFanSpeedResponse\x12\x0b\n\x03rpm\x18\x01 \x01(\r2\xfb\x02\n\x13MinionDeviceService\x12{\n\x0f\x63hange_settings\x12\x30.minknow_api.minion_device.ChangeSettingsRequest\x1a\x31.minknow_api.minion_device.ChangeSettingsResponse\"\x03\x90\x02\x02\x12r\n\x0cget_settings\x12-.minknow_api.minion_device.GetSettingsRequest\x1a..minknow_api.minion_device.GetSettingsResponse\"\x03\x90\x02\x01\x12s\n\rget_fan_speed\x12-.minknow_api.minion_device.GetFanSpeedRequest\x1a..minknow_api.minion_device.GetFanSpeedResponse\"\x03\x90\x02\x01\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-
-
-_TEMPERATURERANGE = DESCRIPTOR.message_types_by_name['TemperatureRange']
-_SAMPLINGFREQUENCYPARAMETERS = DESCRIPTOR.message_types_by_name['SamplingFrequencyParameters']
-_MINIONDEVICESETTINGS = DESCRIPTOR.message_types_by_name['MinionDeviceSettings']
-_MINIONDEVICESETTINGS_CHANNELCONFIGENTRY = _MINIONDEVICESETTINGS.nested_types_by_name['ChannelConfigEntry']
-_CHANGESETTINGSREQUEST = DESCRIPTOR.message_types_by_name['ChangeSettingsRequest']
-_CHANGESETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['ChangeSettingsResponse']
-_GETSETTINGSREQUEST = DESCRIPTOR.message_types_by_name['GetSettingsRequest']
-_GETSETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['GetSettingsResponse']
-_GETFANSPEEDREQUEST = DESCRIPTOR.message_types_by_name['GetFanSpeedRequest']
-_GETFANSPEEDRESPONSE = DESCRIPTOR.message_types_by_name['GetFanSpeedResponse']
-_SAMPLINGFREQUENCYPARAMETERS_CLOCKSPEED = _SAMPLINGFREQUENCYPARAMETERS.enum_types_by_name['ClockSpeed']
-_MINIONDEVICESETTINGS_GAIN = _MINIONDEVICESETTINGS.enum_types_by_name['Gain']
-_MINIONDEVICESETTINGS_DECIMATION = _MINIONDEVICESETTINGS.enum_types_by_name['Decimation']
-_MINIONDEVICESETTINGS_LOWPASSFILTER = _MINIONDEVICESETTINGS.enum_types_by_name['LowPassFilter']
-_MINIONDEVICESETTINGS_NONOVERLAPCLOCK = _MINIONDEVICESETTINGS.enum_types_by_name['NonOverlapClock']
-_MINIONDEVICESETTINGS_INTEGRATIONCAPACITOR = _MINIONDEVICESETTINGS.enum_types_by_name['IntegrationCapacitor']
-_MINIONDEVICESETTINGS_FANSPEED = _MINIONDEVICESETTINGS.enum_types_by_name['FanSpeed']
-_MINIONDEVICESETTINGS_CHANNELCONFIG = _MINIONDEVICESETTINGS.enum_types_by_name['ChannelConfig']
-TemperatureRange = _reflection.GeneratedProtocolMessageType('TemperatureRange', (_message.Message,), {
-  'DESCRIPTOR' : _TEMPERATURERANGE,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  ,
-  '__doc__': """Temperature range.
-  
-  Attributes:
-      min:
-          The minimum temperature in degrees Celsius.  If temperature
-          control is enabled, the device will attempt to keep its
-          temperature at or above this value.  Must be less than or
-          equal to max.  When soft temperature control is enabled, this
-          value is not used.
-      max:
-          The maximum temperature in degrees Celsius.  If temperature
-          control is enabled, the device will attempt to keep its
-          temperature at or below this value.  Must be less than or
-          equal to min.  When soft temperature control is enabled, this
-          is used as the target temperature, and ``min`` is not used.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.TemperatureRange)
-  })
-_sym_db.RegisterMessage(TemperatureRange)
-
-SamplingFrequencyParameters = _reflection.GeneratedProtocolMessageType('SamplingFrequencyParameters', (_message.Message,), {
-  'DESCRIPTOR' : _SAMPLINGFREQUENCYPARAMETERS,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  ,
-  '__doc__': """These values control the sampling frequency.
-  
-  Attributes:
-      clock_divider:
-          Clock divider.  Values over 31 cannot be set.
-      integration_time:
-          The time spent sampling a data point, in microseconds.  Must
-          be between 30 and 1023 (inclusive).  Note that setting the
-          integration_time to less than 50 will force the
-          sinc_decimation value to 32.
-      clock_speed:
-          The speed of the high-speed clock.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.SamplingFrequencyParameters)
-  })
-_sym_db.RegisterMessage(SamplingFrequencyParameters)
-
-MinionDeviceSettings = _reflection.GeneratedProtocolMessageType('MinionDeviceSettings', (_message.Message,), {
-
-  'ChannelConfigEntry' : _reflection.GeneratedProtocolMessageType('ChannelConfigEntry', (_message.Message,), {
-    'DESCRIPTOR' : _MINIONDEVICESETTINGS_CHANNELCONFIGENTRY,
-    '__module__' : 'minknow_api.minion_device_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.minion_device.MinionDeviceSettings.ChannelConfigEntry)
-    })
-  ,
-  'DESCRIPTOR' : _MINIONDEVICESETTINGS,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  ,
-  '__doc__': """Describes the MinION device settings.  Both unset structures and
-  *_KEEP values in enums indicate "no change". When changing settings,
-  these are the default values.
-  
-  Attributes:
-      bias_voltage:
-          The voltage potential to be applied across the wells (in
-          millivolts).  This voltage drives the process of forcing
-          molecules through the nanopores.  The range of possible values
-          is -1275 to 1275 inclusive, in 5mv steps.  When setting this
-          value, if the provided value is not a multiple of 5, an error
-          will be returned.
-      sampling_frequency:
-          The number of measurements to take each second.  This value is
-          derived from the sampling_frequency_params values, and so not
-          all values are possible.  When changing the sampling
-          frequency, either this value can be provided, or the values in
-          sampling_frequency_params can be provided (attempting to
-          provide both will cause the RPC to fail with an error). If
-          this value is provided, the nearest admissible value will be
-          used (eg: if 3000Hz is requested, 3012Hz will be applied).
-          This value cannot be changed during acquisition, and changing
-          it will invalidate the current calibration.  Note that setting
-          the sampling frequency to over 20000Hz (20KHz) will force the
-          sinc_decimation value to 32.
-      channel_config:
-          The per-channel configuration.  Each channel can be set to one
-          of 16 states, which specifies the set of electrical
-          connections to make. This includes which, if any, of the four
-          wells linked to the channel to use.  Note that channel names
-          start at 1. If you pass 0 as a key in this map, it will result
-          in an error.  When changing the device settings, any omitted
-          channels (or channels set to CHANNEL_CONFIG_KEEP) will use the
-          default value set in
-          ChangeSettingsRequest.channel_config_default.
-      enable_temperature_control:
-          Whether to enable temperature control.  If true, the device
-          will attempt to keep its temperature within the bounds given
-          by ``temperature_lower_bound`` and
-          ``temperature_upper_bound``. If false, it will not do any
-          temperature control.  Default is enabled.  It is recommended
-          that this is enabled. If temperature control is disabled, the
-          device may overheat. In this case, it will turn itself off,
-          and must be unplugged and allowed to cool before using again.
-      temperature_target:
-          The target temperature range for the device.  If
-          enable_temperature_control is set to true, the device will
-          attempt to keep its temperature between the min and max values
-          provided here.  Default is defined in application config.
-          Note that if soft temperature control is enabled, only the
-          ``max`` temperature is used.
-      int_capacitor:
-          Integration capacitor value.  This affects the sensitivity of
-          the measurement: lower capacitor values give more sensitive
-          measurements (but also more noise). Changing this will
-          invalidate the current calibration.  Default is 250.0
-      test_current:
-          The level of current used in the TEST_CURRENT channel
-          configuration.  This can be set in the range 0pA to 350pA in
-          50pA intervals, default is 100.0
-      unblock_voltage:
-          The unblock voltage potential (in millivolts).  When a channel
-          is set to one of the UNBLOCK configurations, the specified
-          well will have this voltage applied across it, rather than
-          bias_voltage.  The range of possible values is -372 to 0
-          inclusive, in 12mv steps,  default is 0.  When setting this
-          value, if the provided value is not a multiple of 12, an error
-          will be returned.
-      overcurrent_limit:
-          Whether to enable detection of excessive current.  The ADC
-          output of a channel that trips the overcurrent depends on what
-          track and hold gain has been set to.  Default is enabled.
-      samples_to_reset:
-          The the number of integrator resets per sample.  The range of
-          possible values is 0 to 255, default is 1
-      th_gain:
-          Track/Hold gain.  Default is 5.0
-      sinc_delay:
-          Delay from 2:1 mux switch to sinc filter enable in ADC clocks.
-          The range of possible values is 0 to 15, default is 4.0
-      th_sample_time:
-          Track/Hold sample time in microseconds (us).  The range of
-          possible values is 0.5us to 7.5us in steps of 0.5us, default
-          is 0.5.
-      int_reset_time:
-          Integrator reset time in microseconds (us).  This value forms
-          a part of the integration time specified in the sampling
-          frequency parameters.  The range of possible values is 1us to
-          16us in steps of 0.5us, default is 3.5.
-      sinc_decimation:
-          Decimation.  If the integration time is set to less than 50us
-          (or, equivalently, the sampling frequency is set to greater
-          than 20KHz), this value will be forced to 32.  Default is
-          64.0.
-      low_pass_filter:
-          Low pass filter that should be applied.  Default is 40kHz
-      non_overlap_clock:
-          Amount of non-overlap for non-overlapping clocks.  Default is
-          NOC_1_HS_CLOCK.
-      bias_current:
-          Bias current.  This can be set in the range 0 to 15 in
-          intervals of 5, default is 5.
-      compensation_capacitor:
-          Compensation capacitor value.  This can be set in the range 0
-          to 49 in intervals of 7, default is 14.
-      sampling_frequency_params:
-          Sampling frequency parameters.  The sampling_frequency value
-          is calculated from these settings.  When changing the sampling
-          frequency, either the values here can be provided, or a
-          sampling_frequency can be provided (attempting to provide both
-          will cause the RPC to fail with an error).  WARNING: This
-          should not be used in a change_settings call without
-          consulting the hardware documentation for permissible
-          combinations of values. MinKNOW will only do minimal checking
-          of the values given here; if you use invalid combinations of
-          settings, the device will be unable to acquire data, and may
-          even be permanently damaged.  This value cannot be changed
-          during acquisition.
-      enable_asic_power:
-          Enable ASIC analogue supply voltage.  This must be enabled to
-          heat and acquire data from the ASIC. It can be disabled to
-          save power, but doing so will allow the ASIC to cool down, and
-          it will take time to heat it up again.  Default is true.
-      fan_speed:
-          The speed of the fan when temperature control is off.  If
-          ``enable_temperature_control`` is false, this setting will be
-          ignored, as the temperature control routines on the device
-          will control the speed of the fan.  Note that this setting
-          does not apply to GridIONs.  Default is FANSPEED_MAX.
-      allow_full_fan_stop:
-          Whether to allow the fan to completely stop.  Allowing the fan
-          to stop causes issues on some old MinION models.  Note that
-          this setting does not apply to GridIONs.  Default is false.
-      enable_soft_temperature_control:
-          Enable soft temperature control.  "Soft" temperature control
-          is a more intelligent temperature control algorithm. It works
-          on a single target temperature, and dynamically adjusts the
-          fan speed to reach that temperature quickly, and then mainains
-          the target temperature with high precision.  If this is
-          disabled, "hard" temperature control is used instead. This is
-          a naive algorithm that simply turns the fan up when dropping
-          below the minimum temperature and turns it down when going
-          above the maximum temperature.  If
-          ``enable_temperature_control`` is false, this setting is
-          ignored.  It is recommended that this is enabled.  Default is
-          true.
-      enable_bias_voltage_lookup:
-          Use the bias voltage lookup table to set the bias voltage.  If
-          this is enabled, the bias voltage will be updated every
-          millisecond with each entry in the bias voltage lookup table
-          (see ``bias_voltage_lookup_table``) in turn, cycling through
-          when the end of the table is reached.  This has the effect of
-          producing a bias voltage waveform.  When enabling this, it is
-          required to either provide the lookup table entries at the
-          same time, or to have already provided them in a previous
-          call.  Default is false.
-      bias_voltage_lookup_table:
-          The bias voltage lookup table.  If no entries are provided,
-          the existing lookup table (if any) is preserved.  See
-          ``enable_bias_voltage_lookup``.  Up to 75 values can be
-          provided. The values have the same constraints as
-          ``bias_voltage``.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.MinionDeviceSettings)
-  })
-_sym_db.RegisterMessage(MinionDeviceSettings)
-_sym_db.RegisterMessage(MinionDeviceSettings.ChannelConfigEntry)
-
-ChangeSettingsRequest = _reflection.GeneratedProtocolMessageType('ChangeSettingsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CHANGESETTINGSREQUEST,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      settings:
-          MinION device settings
-      channel_config_default:
-          The default channel configuration.  This provides the default
-          configuration to apply to any channels not listed in
-          settings.channel_config.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.ChangeSettingsRequest)
-  })
-_sym_db.RegisterMessage(ChangeSettingsRequest)
-
-ChangeSettingsResponse = _reflection.GeneratedProtocolMessageType('ChangeSettingsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CHANGESETTINGSRESPONSE,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.ChangeSettingsResponse)
-  })
-_sym_db.RegisterMessage(ChangeSettingsResponse)
-
-GetSettingsRequest = _reflection.GeneratedProtocolMessageType('GetSettingsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETSETTINGSREQUEST,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  ,
-  '__doc__': """Request for MinionDeviceService.get_settings""",
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.GetSettingsRequest)
-  })
-_sym_db.RegisterMessage(GetSettingsRequest)
-
-GetSettingsResponse = _reflection.GeneratedProtocolMessageType('GetSettingsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETSETTINGSRESPONSE,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  ,
-  '__doc__': """Response for MinionDeviceService.get_settings
-  
-  Attributes:
-      settings:
-          MinION device settings
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.GetSettingsResponse)
-  })
-_sym_db.RegisterMessage(GetSettingsResponse)
-
-GetFanSpeedRequest = _reflection.GeneratedProtocolMessageType('GetFanSpeedRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETFANSPEEDREQUEST,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.GetFanSpeedRequest)
-  })
-_sym_db.RegisterMessage(GetFanSpeedRequest)
-
-GetFanSpeedResponse = _reflection.GeneratedProtocolMessageType('GetFanSpeedResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETFANSPEEDRESPONSE,
-  '__module__' : 'minknow_api.minion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.minion_device.GetFanSpeedResponse)
-  })
-_sym_db.RegisterMessage(GetFanSpeedResponse)
-
-_MINIONDEVICESERVICE = DESCRIPTOR.services_by_name['MinionDeviceService']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.minion_device_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
   _MINIONDEVICESETTINGS_CHANNELCONFIGENTRY._options = None
   _MINIONDEVICESETTINGS_CHANNELCONFIGENTRY._serialized_options = b'8\001'
   _CHANGESETTINGSREQUEST.fields_by_name['settings']._options = None
@@ -373,8 +69,215 @@
   _GETSETTINGSRESPONSE._serialized_end=3602
   _GETFANSPEEDREQUEST._serialized_start=3604
   _GETFANSPEEDREQUEST._serialized_end=3624
   _GETFANSPEEDRESPONSE._serialized_start=3626
   _GETFANSPEEDRESPONSE._serialized_end=3660
   _MINIONDEVICESERVICE._serialized_start=3663
   _MINIONDEVICESERVICE._serialized_end=4042
+GetSettingsRequest.__doc__ = """Request for MinionDeviceService.get_settings"""
+MinionDeviceSettings.__doc__ = """Describes the MinION device settings.  Both unset structures and
+*_KEEP values in enums indicate "no change". When changing settings,
+these are the default values.
+
+Attributes:
+    bias_voltage:
+        The voltage potential to be applied across the wells (in
+        millivolts).  This voltage drives the process of forcing
+        molecules through the nanopores.  The range of possible values
+        is -1275 to 1275 inclusive, in 5mv steps.  When setting this
+        value, if the provided value is not a multiple of 5, an error
+        will be returned.
+    sampling_frequency:
+        The number of measurements to take each second.  This value is
+        derived from the sampling_frequency_params values, and so not
+        all values are possible.  When changing the sampling
+        frequency, either this value can be provided, or the values in
+        sampling_frequency_params can be provided (attempting to
+        provide both will cause the RPC to fail with an error). If
+        this value is provided, the nearest admissible value will be
+        used (eg: if 3000Hz is requested, 3012Hz will be applied).
+        This value cannot be changed during acquisition, and changing
+        it will invalidate the current calibration.  Note that setting
+        the sampling frequency to over 20000Hz (20KHz) will force the
+        sinc_decimation value to 32.
+    channel_config:
+        The per-channel configuration.  Each channel can be set to one
+        of 16 states, which specifies the set of electrical
+        connections to make. This includes which, if any, of the four
+        wells linked to the channel to use.  Note that channel names
+        start at 1. If you pass 0 as a key in this map, it will result
+        in an error.  When changing the device settings, any omitted
+        channels (or channels set to CHANNEL_CONFIG_KEEP) will use the
+        default value set in
+        ChangeSettingsRequest.channel_config_default.
+    enable_temperature_control:
+        Whether to enable temperature control.  If true, the device
+        will attempt to keep its temperature within the bounds given
+        by ``temperature_lower_bound`` and
+        ``temperature_upper_bound``. If false, it will not do any
+        temperature control.  Default is enabled.  It is recommended
+        that this is enabled. If temperature control is disabled, the
+        device may overheat. In this case, it will turn itself off,
+        and must be unplugged and allowed to cool before using again.
+    temperature_target:
+        The target temperature range for the device.  If
+        enable_temperature_control is set to true, the device will
+        attempt to keep its temperature between the min and max values
+        provided here.  Default is defined in application config.
+        Note that if soft temperature control is enabled, only the
+        ``max`` temperature is used.
+    int_capacitor:
+        Integration capacitor value.  This affects the sensitivity of
+        the measurement: lower capacitor values give more sensitive
+        measurements (but also more noise). Changing this will
+        invalidate the current calibration.  Default is 250.0
+    test_current:
+        The level of current used in the TEST_CURRENT channel
+        configuration.  This can be set in the range 0pA to 350pA in
+        50pA intervals, default is 100.0
+    unblock_voltage:
+        The unblock voltage potential (in millivolts).  When a channel
+        is set to one of the UNBLOCK configurations, the specified
+        well will have this voltage applied across it, rather than
+        bias_voltage.  The range of possible values is -372 to 0
+        inclusive, in 12mv steps,  default is 0.  When setting this
+        value, if the provided value is not a multiple of 12, an error
+        will be returned.
+    overcurrent_limit:
+        Whether to enable detection of excessive current.  The ADC
+        output of a channel that trips the overcurrent depends on what
+        track and hold gain has been set to.  Default is enabled.
+    samples_to_reset:
+        The the number of integrator resets per sample.  The range of
+        possible values is 0 to 255, default is 1
+    th_gain:
+        Track/Hold gain.  Default is 5.0
+    sinc_delay:
+        Delay from 2:1 mux switch to sinc filter enable in ADC clocks.
+        The range of possible values is 0 to 15, default is 4.0
+    th_sample_time:
+        Track/Hold sample time in microseconds (us).  The range of
+        possible values is 0.5us to 7.5us in steps of 0.5us, default
+        is 0.5.
+    int_reset_time:
+        Integrator reset time in microseconds (us).  This value forms
+        a part of the integration time specified in the sampling
+        frequency parameters.  The range of possible values is 1us to
+        16us in steps of 0.5us, default is 3.5.
+    sinc_decimation:
+        Decimation.  If the integration time is set to less than 50us
+        (or, equivalently, the sampling frequency is set to greater
+        than 20KHz), this value will be forced to 32.  Default is
+        64.0.
+    low_pass_filter:
+        Low pass filter that should be applied.  Default is 40kHz
+    non_overlap_clock:
+        Amount of non-overlap for non-overlapping clocks.  Default is
+        NOC_1_HS_CLOCK.
+    bias_current:
+        Bias current.  This can be set in the range 0 to 15 in
+        intervals of 5, default is 5.
+    compensation_capacitor:
+        Compensation capacitor value.  This can be set in the range 0
+        to 49 in intervals of 7, default is 14.
+    sampling_frequency_params:
+        Sampling frequency parameters.  The sampling_frequency value
+        is calculated from these settings.  When changing the sampling
+        frequency, either the values here can be provided, or a
+        sampling_frequency can be provided (attempting to provide both
+        will cause the RPC to fail with an error).  WARNING: This
+        should not be used in a change_settings call without
+        consulting the hardware documentation for permissible
+        combinations of values. MinKNOW will only do minimal checking
+        of the values given here; if you use invalid combinations of
+        settings, the device will be unable to acquire data, and may
+        even be permanently damaged.  This value cannot be changed
+        during acquisition.
+    enable_asic_power:
+        Enable ASIC analogue supply voltage.  This must be enabled to
+        heat and acquire data from the ASIC. It can be disabled to
+        save power, but doing so will allow the ASIC to cool down, and
+        it will take time to heat it up again.  Default is true.
+    fan_speed:
+        The speed of the fan when temperature control is off.  If
+        ``enable_temperature_control`` is false, this setting will be
+        ignored, as the temperature control routines on the device
+        will control the speed of the fan.  Note that this setting
+        does not apply to GridIONs.  Default is FANSPEED_MAX.
+    allow_full_fan_stop:
+        Whether to allow the fan to completely stop.  Allowing the fan
+        to stop causes issues on some old MinION models.  Note that
+        this setting does not apply to GridIONs.  Default is false.
+    enable_soft_temperature_control:
+        Enable soft temperature control.  "Soft" temperature control
+        is a more intelligent temperature control algorithm. It works
+        on a single target temperature, and dynamically adjusts the
+        fan speed to reach that temperature quickly, and then mainains
+        the target temperature with high precision.  If this is
+        disabled, "hard" temperature control is used instead. This is
+        a naive algorithm that simply turns the fan up when dropping
+        below the minimum temperature and turns it down when going
+        above the maximum temperature.  If
+        ``enable_temperature_control`` is false, this setting is
+        ignored.  It is recommended that this is enabled.  Default is
+        true.
+    enable_bias_voltage_lookup:
+        Use the bias voltage lookup table to set the bias voltage.  If
+        this is enabled, the bias voltage will be updated every
+        millisecond with each entry in the bias voltage lookup table
+        (see ``bias_voltage_lookup_table``) in turn, cycling through
+        when the end of the table is reached.  This has the effect of
+        producing a bias voltage waveform.  When enabling this, it is
+        required to either provide the lookup table entries at the
+        same time, or to have already provided them in a previous
+        call.  Default is false.
+    bias_voltage_lookup_table:
+        The bias voltage lookup table.  If no entries are provided,
+        the existing lookup table (if any) is preserved.  See
+        ``enable_bias_voltage_lookup``.  Up to 75 values can be
+        provided. The values have the same constraints as
+        ``bias_voltage``.
+"""
+TemperatureRange.__doc__ = """Temperature range.
+
+Attributes:
+    min:
+        The minimum temperature in degrees Celsius.  If temperature
+        control is enabled, the device will attempt to keep its
+        temperature at or above this value.  Must be less than or
+        equal to max.  When soft temperature control is enabled, this
+        value is not used.
+    max:
+        The maximum temperature in degrees Celsius.  If temperature
+        control is enabled, the device will attempt to keep its
+        temperature at or below this value.  Must be less than or
+        equal to min.  When soft temperature control is enabled, this
+        is used as the target temperature, and ``min`` is not used.
+"""
+ChangeSettingsRequest.__doc__ = """Attributes:
+    settings:
+        MinION device settings
+    channel_config_default:
+        The default channel configuration.  This provides the default
+        configuration to apply to any channels not listed in
+        settings.channel_config.
+"""
+GetSettingsResponse.__doc__ = """Response for MinionDeviceService.get_settings
+
+Attributes:
+    settings:
+        MinION device settings
+"""
+SamplingFrequencyParameters.__doc__ = """These values control the sampling frequency.
+
+Attributes:
+    clock_divider:
+        Clock divider.  Values over 31 cannot be set.
+    integration_time:
+        The time spent sampling a data point, in microseconds.  Must
+        be between 30 and 1023 (inclusive).  Note that setting the
+        integration_time to less than 50 will force the
+        sinc_decimation value to 32.
+    clock_speed:
+        The speed of the high-speed clock.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/minion_device_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/minion_device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/minion_device_service.py` & `minknow_api-5.5.2/minknow_api/minion_device_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/post_processing_protocol_connection.py` & `minknow_api-5.5.2/minknow_api/post_processing_protocol_connection.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/promethion_device_pb2.py` & `minknow_api-5.5.2/minknow_api/promethion_device_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,436 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: minknow_api/promethion_device.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#minknow_api/promethion_device.proto\x12\x1dminknow_api.promethion_device\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1dminknow_api/rpc_options.proto\"7\n\x10WaveformSettings\x12\x10\n\x08voltages\x18\x01 \x03(\x01\x12\x11\n\tfrequency\x18\x02 \x01(\x01\"\xfb\x03\n\x0e\x44\x65viceSettings\x12\x37\n\x12sampling_frequency\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x32\n\x0cramp_voltage\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x16\n\x0c\x62ias_voltage\x18\x03 \x01(\x01H\x00\x12P\n\x15\x62ias_voltage_waveform\x18\x04 \x01(\x0b\x32/.minknow_api.promethion_device.WaveformSettingsH\x00\x12>\n\x1asaturation_control_enabled\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12<\n\x18\x66\x61st_calibration_enabled\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x37\n\x12temperature_target\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x43\n\x07timings\x18\x08 \x01(\x0b\x32\x32.minknow_api.promethion_device.TimingEnginePeriodsB\x16\n\x14\x62ias_voltage_setting\"\xf5\x04\n\x13TimingEnginePeriods\x12*\n\x04RST1\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12/\n\tRST1_CDS1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04\x43\x44S1\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12/\n\tCDS1_DATA\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04\x44\x41TA\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12/\n\tDATA_RST2\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04RST2\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12/\n\tRST2_CDS2\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04\x43\x44S2\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x07\x43\x44S2_SH\x18\n \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12(\n\x02SH\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x07SH_RST1\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x36\n\x12use_default_values\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\x8e\x01\n\x12PixelBlockSettings\x12\x41\n\x1bregen_current_voltage_clamp\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0funblock_voltage\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xaf\x11\n\rPixelSettings\x12\x45\n\x05input\x18\x01 \x01(\x0b\x32\x36.minknow_api.promethion_device.PixelSettings.InputWell\x12P\n\roverload_mode\x18\x02 \x01(\x0e\x32\x39.minknow_api.promethion_device.PixelSettings.OverloadMode\x12T\n\x10\x63utoff_frequency\x18\x03 \x01(\x0e\x32:.minknow_api.promethion_device.PixelSettings.LowPassFilter\x12T\n\x0fgain_multiplier\x18\x04 \x01(\x0e\x32;.minknow_api.promethion_device.PixelSettings.GainMultiplier\x12R\n\x0egain_capacitor\x18\x05 \x01(\x0e\x32:.minknow_api.promethion_device.PixelSettings.GainCapacitor\x12V\n\x10\x63\x61libration_mode\x18\x06 \x01(\x0e\x32<.minknow_api.promethion_device.PixelSettings.CalibrationMode\x12Q\n\x0funblock_voltage\x18\x07 \x01(\x0e\x32\x38.minknow_api.promethion_device.PixelSettings.UnblockMode\x12\x34\n\x10\x63urrent_inverted\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x1bmembrane_simulation_enabled\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12^\n\x14regeneration_current\x18\n \x01(\x0e\x32@.minknow_api.promethion_device.PixelSettings.RegenerationCurrent\x12\x45\n!regeneration_current_test_enabled\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12N\n\x0c\x62ias_current\x18\x0c \x01(\x0e\x32\x38.minknow_api.promethion_device.PixelSettings.BiasCurrent\x1a\x94\x02\n\tInputWell\x12V\n\ninput_well\x18\x01 \x01(\x0e\x32\x42.minknow_api.promethion_device.PixelSettings.InputWell.InputConfig\x12]\n\x11regeneration_well\x18\x02 \x01(\x0e\x32\x42.minknow_api.promethion_device.PixelSettings.InputWell.InputConfig\"P\n\x0bInputConfig\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06WELL_1\x10\x01\x12\n\n\x06WELL_2\x10\x02\x12\n\n\x06WELL_3\x10\x03\x12\n\n\x06WELL_4\x10\x04\x12\x07\n\x03\x41LL\x10\x05\"x\n\x0cOverloadMode\x12\x11\n\rOVERLOAD_KEEP\x10\x00\x12\x15\n\x11OVERLOAD_SET_FLAG\x10\x01\x12\x16\n\x12OVERLOAD_LATCH_OFF\x10\x02\x12\x12\n\x0eOVERLOAD_CLEAR\x10\x03\x12\x12\n\x0eOVERLOAD_LIMIT\x10\x04\"\x95\x01\n\rLowPassFilter\x12\x0c\n\x08LPF_KEEP\x10\x00\x12\r\n\tLPF_10kHz\x10\x01\x12\r\n\tLPF_20kHz\x10\x02\x12\r\n\tLPF_30kHz\x10\x03\x12\r\n\tLPF_40kHz\x10\x04\x12\r\n\tLPF_50kHz\x10\x05\x12\r\n\tLPF_60kHz\x10\x06\x12\r\n\tLPF_70kHz\x10\x07\x12\r\n\tLPF_80kHz\x10\x08\"@\n\x0eGainMultiplier\x12\x10\n\x0cINTGAIN_KEEP\x10\x00\x12\r\n\tINTGAIN_2\x10\x01\x12\r\n\tINTGAIN_4\x10\x02\"h\n\rGainCapacitor\x12\x0f\n\x0bINTCAP_KEEP\x10\x00\x12\x10\n\x0cINTCAP_100fF\x10\x01\x12\x10\n\x0cINTCAP_200fF\x10\x02\x12\x10\n\x0cINTCAP_500fF\x10\x03\x12\x10\n\x0cINTCAP_600fF\x10\x04\"A\n\x0f\x43\x61librationMode\x12\x0e\n\nCALIB_KEEP\x10\x00\x12\x0e\n\nCALIB_FAST\x10\x01\x12\x0e\n\nCALIB_SLOW\x10\x02\"@\n\x0bUnblockMode\x12\x10\n\x0cUNBLOCK_KEEP\x10\x00\x12\x0e\n\nUNBLOCK_ON\x10\x01\x12\x0f\n\x0bUNBLOCK_OFF\x10\x02\"\xb6\x02\n\x13RegenerationCurrent\x12\x0e\n\nREGEN_KEEP\x10\x00\x12\r\n\tREGEN_0pA\x10\x01\x12\x0e\n\nREGEN_50pA\x10\x02\x12\x0f\n\x0bREGEN_100pA\x10\x03\x12\x0f\n\x0bREGEN_150pA\x10\x04\x12\x0f\n\x0bREGEN_400pA\x10\x05\x12\x0f\n\x0bREGEN_450pA\x10\x06\x12\x0f\n\x0bREGEN_500pA\x10\x07\x12\x0f\n\x0bREGEN_550pA\x10\x08\x12\x0f\n\x0bREGEN_800pA\x10\t\x12\x0f\n\x0bREGEN_850pA\x10\n\x12\x0f\n\x0bREGEN_900pA\x10\x0b\x12\x0f\n\x0bREGEN_950pA\x10\x0c\x12\x10\n\x0cREGEN_1200pA\x10\r\x12\x10\n\x0cREGEN_1250pA\x10\x0e\x12\x10\n\x0cREGEN_1300pA\x10\x0f\x12\x10\n\x0cREGEN_1350pA\x10\x10\"Y\n\x0b\x42iasCurrent\x12\r\n\tBIAS_KEEP\x10\x00\x12\x0c\n\x08\x42IAS_OFF\x10\x01\x12\x0c\n\x08\x42IAS_LOW\x10\x02\x12\r\n\tBIAS_HIGH\x10\x03\x12\x10\n\x0c\x42IAS_NOMINAL\x10\x04\"d\n\x1b\x43hangeDeviceSettingsRequest\x12\x45\n\x08settings\x18\x01 \x01(\x0b\x32-.minknow_api.promethion_device.DeviceSettingsB\x04\x90\xb5\x18\x01\"\\\n\x1c\x43hangeDeviceSettingsResponse\x12<\n\x17real_sampling_frequency\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\"\x1a\n\x18GetDeviceSettingsRequest\"b\n\x19GetDeviceSettingsResponse\x12\x45\n\x08settings\x18\x01 \x01(\x0b\x32-.minknow_api.promethion_device.DeviceSettingsB\x04\x90\xb5\x18\x01\"\xbf\x02\n\x1f\x43hangePixelBlockSettingsRequest\x12\x65\n\x0cpixel_blocks\x18\x01 \x03(\x0b\x32O.minknow_api.promethion_device.ChangePixelBlockSettingsRequest.PixelBlocksEntry\x12N\n\x13pixel_block_default\x18\x02 \x01(\x0b\x32\x31.minknow_api.promethion_device.PixelBlockSettings\x1a\x65\n\x10PixelBlocksEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12@\n\x05value\x18\x02 \x01(\x0b\x32\x31.minknow_api.promethion_device.PixelBlockSettings:\x02\x38\x01\"\"\n ChangePixelBlockSettingsResponse\"\x1e\n\x1cGetPixelBlockSettingsRequest\"\xeb\x01\n\x1dGetPixelBlockSettingsResponse\x12\x63\n\x0cpixel_blocks\x18\x01 \x03(\x0b\x32M.minknow_api.promethion_device.GetPixelBlockSettingsResponse.PixelBlocksEntry\x1a\x65\n\x10PixelBlocksEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12@\n\x05value\x18\x02 \x01(\x0b\x32\x31.minknow_api.promethion_device.PixelBlockSettings:\x02\x38\x01\"\x95\x02\n\x1a\x43hangePixelSettingsRequest\x12U\n\x06pixels\x18\x01 \x03(\x0b\x32\x45.minknow_api.promethion_device.ChangePixelSettingsRequest.PixelsEntry\x12\x43\n\rpixel_default\x18\x02 \x01(\x0b\x32,.minknow_api.promethion_device.PixelSettings\x1a[\n\x0bPixelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.minknow_api.promethion_device.PixelSettings:\x02\x38\x01\"\x1d\n\x1b\x43hangePixelSettingsResponse\"/\n\x17GetPixelSettingsRequest\x12\x14\n\x06pixels\x18\x01 \x03(\rB\x04\x88\xb5\x18\x01\"X\n\x18GetPixelSettingsResponse\x12<\n\x06pixels\x18\x01 \x03(\x0b\x32,.minknow_api.promethion_device.PixelSettings\"2\n\x18StreamTemperatureRequest\x12\x16\n\x0eperiod_seconds\x18\x01 \x01(\r\"\x84\x02\n\x16GetTemperatureResponse\x12\x39\n\x14\x66lowcell_temperature\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x38\n\x13\x63hamber_temperature\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12<\n\x17pixel_block_temperature\x18\x03 \x03(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x37\n\x12target_temperature\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue2\xb6\x08\n\x17PromethionDeviceService\x12\x96\x01\n\x16\x63hange_device_settings\x12:.minknow_api.promethion_device.ChangeDeviceSettingsRequest\x1a;.minknow_api.promethion_device.ChangeDeviceSettingsResponse\"\x03\x90\x02\x02\x12\x8d\x01\n\x13get_device_settings\x12\x37.minknow_api.promethion_device.GetDeviceSettingsRequest\x1a\x38.minknow_api.promethion_device.GetDeviceSettingsResponse\"\x03\x90\x02\x01\x12\xa3\x01\n\x1b\x63hange_pixel_block_settings\x12>.minknow_api.promethion_device.ChangePixelBlockSettingsRequest\x1a?.minknow_api.promethion_device.ChangePixelBlockSettingsResponse\"\x03\x90\x02\x02\x12\x9a\x01\n\x18get_pixel_block_settings\x12;.minknow_api.promethion_device.GetPixelBlockSettingsRequest\x1a<.minknow_api.promethion_device.GetPixelBlockSettingsResponse\"\x03\x90\x02\x01\x12\x93\x01\n\x15\x63hange_pixel_settings\x12\x39.minknow_api.promethion_device.ChangePixelSettingsRequest\x1a:.minknow_api.promethion_device.ChangePixelSettingsResponse\"\x03\x90\x02\x02\x12\x8a\x01\n\x12get_pixel_settings\x12\x36.minknow_api.promethion_device.GetPixelSettingsRequest\x1a\x37.minknow_api.promethion_device.GetPixelSettingsResponse\"\x03\x90\x02\x01\x12\x8b\x01\n\x12stream_temperature\x12\x37.minknow_api.promethion_device.StreamTemperatureRequest\x1a\x35.minknow_api.promethion_device.GetTemperatureResponse\"\x03\x90\x02\x01\x30\x01\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-
-
-_WAVEFORMSETTINGS = DESCRIPTOR.message_types_by_name['WaveformSettings']
-_DEVICESETTINGS = DESCRIPTOR.message_types_by_name['DeviceSettings']
-_TIMINGENGINEPERIODS = DESCRIPTOR.message_types_by_name['TimingEnginePeriods']
-_PIXELBLOCKSETTINGS = DESCRIPTOR.message_types_by_name['PixelBlockSettings']
-_PIXELSETTINGS = DESCRIPTOR.message_types_by_name['PixelSettings']
-_PIXELSETTINGS_INPUTWELL = _PIXELSETTINGS.nested_types_by_name['InputWell']
-_CHANGEDEVICESETTINGSREQUEST = DESCRIPTOR.message_types_by_name['ChangeDeviceSettingsRequest']
-_CHANGEDEVICESETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['ChangeDeviceSettingsResponse']
-_GETDEVICESETTINGSREQUEST = DESCRIPTOR.message_types_by_name['GetDeviceSettingsRequest']
-_GETDEVICESETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['GetDeviceSettingsResponse']
-_CHANGEPIXELBLOCKSETTINGSREQUEST = DESCRIPTOR.message_types_by_name['ChangePixelBlockSettingsRequest']
-_CHANGEPIXELBLOCKSETTINGSREQUEST_PIXELBLOCKSENTRY = _CHANGEPIXELBLOCKSETTINGSREQUEST.nested_types_by_name['PixelBlocksEntry']
-_CHANGEPIXELBLOCKSETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['ChangePixelBlockSettingsResponse']
-_GETPIXELBLOCKSETTINGSREQUEST = DESCRIPTOR.message_types_by_name['GetPixelBlockSettingsRequest']
-_GETPIXELBLOCKSETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['GetPixelBlockSettingsResponse']
-_GETPIXELBLOCKSETTINGSRESPONSE_PIXELBLOCKSENTRY = _GETPIXELBLOCKSETTINGSRESPONSE.nested_types_by_name['PixelBlocksEntry']
-_CHANGEPIXELSETTINGSREQUEST = DESCRIPTOR.message_types_by_name['ChangePixelSettingsRequest']
-_CHANGEPIXELSETTINGSREQUEST_PIXELSENTRY = _CHANGEPIXELSETTINGSREQUEST.nested_types_by_name['PixelsEntry']
-_CHANGEPIXELSETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['ChangePixelSettingsResponse']
-_GETPIXELSETTINGSREQUEST = DESCRIPTOR.message_types_by_name['GetPixelSettingsRequest']
-_GETPIXELSETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['GetPixelSettingsResponse']
-_STREAMTEMPERATUREREQUEST = DESCRIPTOR.message_types_by_name['StreamTemperatureRequest']
-_GETTEMPERATURERESPONSE = DESCRIPTOR.message_types_by_name['GetTemperatureResponse']
-_PIXELSETTINGS_INPUTWELL_INPUTCONFIG = _PIXELSETTINGS_INPUTWELL.enum_types_by_name['InputConfig']
-_PIXELSETTINGS_OVERLOADMODE = _PIXELSETTINGS.enum_types_by_name['OverloadMode']
-_PIXELSETTINGS_LOWPASSFILTER = _PIXELSETTINGS.enum_types_by_name['LowPassFilter']
-_PIXELSETTINGS_GAINMULTIPLIER = _PIXELSETTINGS.enum_types_by_name['GainMultiplier']
-_PIXELSETTINGS_GAINCAPACITOR = _PIXELSETTINGS.enum_types_by_name['GainCapacitor']
-_PIXELSETTINGS_CALIBRATIONMODE = _PIXELSETTINGS.enum_types_by_name['CalibrationMode']
-_PIXELSETTINGS_UNBLOCKMODE = _PIXELSETTINGS.enum_types_by_name['UnblockMode']
-_PIXELSETTINGS_REGENERATIONCURRENT = _PIXELSETTINGS.enum_types_by_name['RegenerationCurrent']
-_PIXELSETTINGS_BIASCURRENT = _PIXELSETTINGS.enum_types_by_name['BiasCurrent']
-WaveformSettings = _reflection.GeneratedProtocolMessageType('WaveformSettings', (_message.Message,), {
-  'DESCRIPTOR' : _WAVEFORMSETTINGS,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      voltages:
-          The waveform data applied to the device (in millivolts)  Must
-          contain 32 values, in order to be a valid waveform.
-      frequency:
-          The frequency of the applied waveform, in Hz.  Valid values
-          are between 7.8125Hz and 500Hz.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.WaveformSettings)
-  })
-_sym_db.RegisterMessage(WaveformSettings)
-
-DeviceSettings = _reflection.GeneratedProtocolMessageType('DeviceSettings', (_message.Message,), {
-  'DESCRIPTOR' : _DEVICESETTINGS,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      sampling_frequency:
-          The number of measurements to take each second.  Possible
-          values are between 1000, and 10000. If the value is outside of
-          this range, it will be clamped within it  This value cannot be
-          changed during acquisition.
-      ramp_voltage:
-          The value to apply as the ramp voltage (in millivolts)  Valid
-          values are in the range -1250mv..1250mv
-      bias_voltage_setting:
-          Settings controlling the device bias voltage
-      bias_voltage:
-          The value to apply as the bias voltage (in millivolts)  Valid
-          values are in the range -1250mv..1250mv
-      bias_voltage_waveform:
-          The waveform settings
-      saturation_control_enabled:
-          Enables saturation control on the device
-      fast_calibration_enabled:
-          Enable use of the fast calibration mode across the device
-      temperature_target:
-          If the device is capable (see
-          device.get_device_info().temperature_controllable) then this
-          sets the minimum and maximum temperatures of the flow-cell.
-          These values must be between the limits specified in the
-          application config, see: min_user_setpoint_temperature_celsius
-          and max_user_setpoint_temperature_celsius
-      timings:
-          If specified, the device will adopt these timings to set how
-          long is spent at various stages of the current digitisation
-          processes. The message includes a way of returning to default
-          timings.  This value cannot be changed during acquisition
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.DeviceSettings)
-  })
-_sym_db.RegisterMessage(DeviceSettings)
-
-TimingEnginePeriods = _reflection.GeneratedProtocolMessageType('TimingEnginePeriods', (_message.Message,), {
-  'DESCRIPTOR' : _TIMINGENGINEPERIODS,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """ Timing-engine periods are specified in 5ns units. Some of the timing
-  mechanism can only achieve 10ns accuracy, so even numbers are
-  preferred.  Note: There is a timing feature in the ASIC that requires
-  the sum of the RST1 and DATA periods to be a multiple of 16
-  
-  Attributes:
-      RST1:
-          Reset1 phase  Note: Commands are written to the ASIC during
-          this period, to allow sufficient time to write the commands,
-          this should never be less than 1.2us or 240.
-      RST1_CDS1:
-          Reset1 to CDS1 transition
-      CDS1:
-          CDS1 phase (Correlated Double Sampling) sample-point 1
-      CDS1_DATA:
-          CDS1 to DATA transiton
-      DATA:
-          DATA transfer phase  NOTE: Setting this value has no effect,
-          MinKNOW will choose a value for DATA itself to acheive the
-          required frame-rate. Reading it will return the chosen DATA
-          period.
-      DATA_RST2:
-          DATA transfer to Reset2 transition. MinKNOW may increase this
-          value by small amounts so that when changing the DATA period,
-          the sum of the RST1 and DATA periods is a multiple of 16 and
-          the frame-rate and integration-period are maintained.
-      RST2:
-          Reset2
-      RST2_CDS2:
-          Reset2 to CDS2 transition
-      CDS2:
-          CDS2 Phase (sample-point 2)
-      CDS2_SH:
-          CDS2 to SH transition
-      SH:
-          SH phase (Sample and Hold)
-      SH_RST1:
-          SH to Reset1 transition
-      use_default_values:
-          If written true, other fields will be ignored and the hardware
-          will use default timings. When read will return true if
-          previously set true, it will not tell you if the timing
-          periods you previously entered are the same as the default
-          values.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.TimingEnginePeriods)
-  })
-_sym_db.RegisterMessage(TimingEnginePeriods)
-
-PixelBlockSettings = _reflection.GeneratedProtocolMessageType('PixelBlockSettings', (_message.Message,), {
-  'DESCRIPTOR' : _PIXELBLOCKSETTINGS,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      regen_current_voltage_clamp:
-          Voltage clamp for regeneration circuit (in millivolts)  The
-          voltage in the regeneration circuit is clamped under this
-          value, whilst applying the current specified in each pixel's
-          settings.  The acceptable input range is -1000..1000
-          (inclusive)
-      unblock_voltage:
-          The unblock voltage to apply when a pixel is unblocking.  The
-          acceptable input range is -1000..1000 (inclusive)
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.PixelBlockSettings)
-  })
-_sym_db.RegisterMessage(PixelBlockSettings)
-
-PixelSettings = _reflection.GeneratedProtocolMessageType('PixelSettings', (_message.Message,), {
-
-  'InputWell' : _reflection.GeneratedProtocolMessageType('InputWell', (_message.Message,), {
-    'DESCRIPTOR' : _PIXELSETTINGS_INPUTWELL,
-    '__module__' : 'minknow_api.promethion_device_pb2'
-    ,
-    '__doc__': """Attributes:
-        input_well:
-            Control which well is driving the adc minknow reads from.  ALL
-            is not a valid value here (other values are acceptable).
-        regeneration_well:
-            Control which wells are being regenerated (has the specified
-            regeneration current driven to it).  All possible Input values
-            are acceptable, as long as the input is not the active adc
-            input. For example, { input: 1, regeneration: all } is
-            invalid, as an well cannot be both input and regenerated.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.PixelSettings.InputWell)
-    })
-  ,
-  'DESCRIPTOR' : _PIXELSETTINGS,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      input:
-          The input driving the adv
-      overload_mode:
-          The mode the asic uses to handle currents that go above its
-          adc range.
-      cutoff_frequency:
-          Signal filter for input adc signal.
-      gain_multiplier:
-          Signal gain multiplier, applied to the integrator circuit.
-      gain_capacitor:
-          Gain capacitor, used in the integrtor circuit.
-      calibration_mode:
-          The calibration mode to use.
-      unblock_voltage:
-          Controls the application of the unblock voltage to the pixel.
-      current_inverted:
-          Inverts the current's polarity.
-      membrane_simulation_enabled:
-          Control the state of the membrane simulation.
-      regeneration_current:
-          Control the regeneration current used when regenerating
-          well's.
-      regeneration_current_test_enabled:
-          Control if the regeneration current test is enabled.  This
-          connects the regeneration current to the integration adc
-          circuit and the input well. and allows users to read regen
-          current via the channel adc value.
-      bias_current:
-          The bias current for the amplifier - this controls the level
-          of noise of the signal.  The higher the bias current, the
-          lower the noise, but the bigger the heat and power drawn by
-          the amplifier. If it is set to off, no signal readings can be
-          made.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.PixelSettings)
-  })
-_sym_db.RegisterMessage(PixelSettings)
-_sym_db.RegisterMessage(PixelSettings.InputWell)
-
-ChangeDeviceSettingsRequest = _reflection.GeneratedProtocolMessageType('ChangeDeviceSettingsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CHANGEDEVICESETTINGSREQUEST,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangeDeviceSettingsRequest)
-  })
-_sym_db.RegisterMessage(ChangeDeviceSettingsRequest)
-
-ChangeDeviceSettingsResponse = _reflection.GeneratedProtocolMessageType('ChangeDeviceSettingsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CHANGEDEVICESETTINGSRESPONSE,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      real_sampling_frequency:
-          The sampling frequency actually applied to the hardware, as
-          close as possible to the requested rate.  Note: only returned
-          if sampling rate was set as part of this call.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangeDeviceSettingsResponse)
-  })
-_sym_db.RegisterMessage(ChangeDeviceSettingsResponse)
-
-GetDeviceSettingsRequest = _reflection.GeneratedProtocolMessageType('GetDeviceSettingsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETDEVICESETTINGSREQUEST,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetDeviceSettingsRequest)
-  })
-_sym_db.RegisterMessage(GetDeviceSettingsRequest)
-
-GetDeviceSettingsResponse = _reflection.GeneratedProtocolMessageType('GetDeviceSettingsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETDEVICESETTINGSRESPONSE,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetDeviceSettingsResponse)
-  })
-_sym_db.RegisterMessage(GetDeviceSettingsResponse)
-
-ChangePixelBlockSettingsRequest = _reflection.GeneratedProtocolMessageType('ChangePixelBlockSettingsRequest', (_message.Message,), {
-
-  'PixelBlocksEntry' : _reflection.GeneratedProtocolMessageType('PixelBlocksEntry', (_message.Message,), {
-    'DESCRIPTOR' : _CHANGEPIXELBLOCKSETTINGSREQUEST_PIXELBLOCKSENTRY,
-    '__module__' : 'minknow_api.promethion_device_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangePixelBlockSettingsRequest.PixelBlocksEntry)
-    })
-  ,
-  'DESCRIPTOR' : _CHANGEPIXELBLOCKSETTINGSREQUEST,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      pixel_blocks:
-          1 based map of different pixel blocks settings, a sparse map
-          is accepted, keys should be integers between 1 and 12.
-      pixel_block_default:
-          If supplied, contains settings applied to every block before
-          then applying any specific settings in the per block settings.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangePixelBlockSettingsRequest)
-  })
-_sym_db.RegisterMessage(ChangePixelBlockSettingsRequest)
-_sym_db.RegisterMessage(ChangePixelBlockSettingsRequest.PixelBlocksEntry)
-
-ChangePixelBlockSettingsResponse = _reflection.GeneratedProtocolMessageType('ChangePixelBlockSettingsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CHANGEPIXELBLOCKSETTINGSRESPONSE,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangePixelBlockSettingsResponse)
-  })
-_sym_db.RegisterMessage(ChangePixelBlockSettingsResponse)
-
-GetPixelBlockSettingsRequest = _reflection.GeneratedProtocolMessageType('GetPixelBlockSettingsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETPIXELBLOCKSETTINGSREQUEST,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetPixelBlockSettingsRequest)
-  })
-_sym_db.RegisterMessage(GetPixelBlockSettingsRequest)
-
-GetPixelBlockSettingsResponse = _reflection.GeneratedProtocolMessageType('GetPixelBlockSettingsResponse', (_message.Message,), {
-
-  'PixelBlocksEntry' : _reflection.GeneratedProtocolMessageType('PixelBlocksEntry', (_message.Message,), {
-    'DESCRIPTOR' : _GETPIXELBLOCKSETTINGSRESPONSE_PIXELBLOCKSENTRY,
-    '__module__' : 'minknow_api.promethion_device_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetPixelBlockSettingsResponse.PixelBlocksEntry)
-    })
-  ,
-  'DESCRIPTOR' : _GETPIXELBLOCKSETTINGSRESPONSE,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      pixel_blocks:
-          1 based map of different pixel blocks settings, containing 12
-          entries.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetPixelBlockSettingsResponse)
-  })
-_sym_db.RegisterMessage(GetPixelBlockSettingsResponse)
-_sym_db.RegisterMessage(GetPixelBlockSettingsResponse.PixelBlocksEntry)
-
-ChangePixelSettingsRequest = _reflection.GeneratedProtocolMessageType('ChangePixelSettingsRequest', (_message.Message,), {
-
-  'PixelsEntry' : _reflection.GeneratedProtocolMessageType('PixelsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _CHANGEPIXELSETTINGSREQUEST_PIXELSENTRY,
-    '__module__' : 'minknow_api.promethion_device_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangePixelSettingsRequest.PixelsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _CHANGEPIXELSETTINGSREQUEST,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      pixels:
-          1 based map of up to 3000 different pixel settings
-      pixel_default:
-          If supplied, contains settings applied to every pixel before
-          then applying any specific settings in the per pixel settings.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangePixelSettingsRequest)
-  })
-_sym_db.RegisterMessage(ChangePixelSettingsRequest)
-_sym_db.RegisterMessage(ChangePixelSettingsRequest.PixelsEntry)
-
-ChangePixelSettingsResponse = _reflection.GeneratedProtocolMessageType('ChangePixelSettingsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CHANGEPIXELSETTINGSRESPONSE,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.ChangePixelSettingsResponse)
-  })
-_sym_db.RegisterMessage(ChangePixelSettingsResponse)
-
-GetPixelSettingsRequest = _reflection.GeneratedProtocolMessageType('GetPixelSettingsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETPIXELSETTINGSREQUEST,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      pixels:
-          The channels (one based) to return data for. A sparse map is
-          accepted
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetPixelSettingsRequest)
-  })
-_sym_db.RegisterMessage(GetPixelSettingsRequest)
-
-GetPixelSettingsResponse = _reflection.GeneratedProtocolMessageType('GetPixelSettingsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETPIXELSETTINGSRESPONSE,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      pixels:
-          List of all requested pixel settings, in the order requested.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetPixelSettingsResponse)
-  })
-_sym_db.RegisterMessage(GetPixelSettingsResponse)
-
-StreamTemperatureRequest = _reflection.GeneratedProtocolMessageType('StreamTemperatureRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMTEMPERATUREREQUEST,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      period_seconds:
-          How often temperature updates should be sent Defaults to a
-          period of 1 second, if not specified, or set to 0
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.StreamTemperatureRequest)
-  })
-_sym_db.RegisterMessage(StreamTemperatureRequest)
-
-GetTemperatureResponse = _reflection.GeneratedProtocolMessageType('GetTemperatureResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETTEMPERATURERESPONSE,
-  '__module__' : 'minknow_api.promethion_device_pb2'
-  ,
-  '__doc__': """Attributes:
-      flowcell_temperature:
-          Temperature as measured by thermistor TH2 on the P-Chip.
-      chamber_temperature:
-          Flow-cell chamber-temperature, calculated from the pixel-block
-          temperatures
-      pixel_block_temperature:
-          Temperature measured at each sensor in the ASIC, there are 12
-          sensors, one sensor per pixel-block
-      target_temperature:
-          Return the temperature target the device is aiming to reach.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.promethion_device.GetTemperatureResponse)
-  })
-_sym_db.RegisterMessage(GetTemperatureResponse)
-
-_PROMETHIONDEVICESERVICE = DESCRIPTOR.services_by_name['PromethionDeviceService']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.promethion_device_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
   _CHANGEDEVICESETTINGSREQUEST.fields_by_name['settings']._options = None
   _CHANGEDEVICESETTINGSREQUEST.fields_by_name['settings']._serialized_options = b'\220\265\030\001'
   _GETDEVICESETTINGSRESPONSE.fields_by_name['settings']._options = None
@@ -519,8 +111,210 @@
   _GETPIXELSETTINGSRESPONSE._serialized_end=5103
   _STREAMTEMPERATUREREQUEST._serialized_start=5105
   _STREAMTEMPERATUREREQUEST._serialized_end=5155
   _GETTEMPERATURERESPONSE._serialized_start=5158
   _GETTEMPERATURERESPONSE._serialized_end=5418
   _PROMETHIONDEVICESERVICE._serialized_start=5421
   _PROMETHIONDEVICESERVICE._serialized_end=6499
+ChangePixelBlockSettingsRequest.__doc__ = """Attributes:
+    pixel_blocks:
+        1 based map of different pixel blocks settings, a sparse map
+        is accepted, keys should be integers between 1 and 12.
+    pixel_block_default:
+        If supplied, contains settings applied to every block before
+        then applying any specific settings in the per block settings.
+"""
+WaveformSettings.__doc__ = """Attributes:
+    voltages:
+        The waveform data applied to the device (in millivolts)  Must
+        contain 32 values, in order to be a valid waveform.
+    frequency:
+        The frequency of the applied waveform, in Hz.  Valid values
+        are between 7.8125Hz and 500Hz.
+"""
+ChangeDeviceSettingsResponse.__doc__ = """Attributes:
+    real_sampling_frequency:
+        The sampling frequency actually applied to the hardware, as
+        close as possible to the requested rate.  Note: only returned
+        if sampling rate was set as part of this call.
+"""
+GetPixelBlockSettingsResponse.__doc__ = """Attributes:
+    pixel_blocks:
+        1 based map of different pixel blocks settings, containing 12
+        entries.
+"""
+DeviceSettings.__doc__ = """Attributes:
+    sampling_frequency:
+        The number of measurements to take each second.  Possible
+        values are between 1000, and 10000. If the value is outside of
+        this range, it will be clamped within it  This value cannot be
+        changed during acquisition.
+    ramp_voltage:
+        The value to apply as the ramp voltage (in millivolts)  Valid
+        values are in the range -1250mv..1250mv
+    bias_voltage_setting:
+        Settings controlling the device bias voltage
+    bias_voltage:
+        The value to apply as the bias voltage (in millivolts)  Valid
+        values are in the range -1250mv..1250mv
+    bias_voltage_waveform:
+        The waveform settings
+    saturation_control_enabled:
+        Enables saturation control on the device
+    fast_calibration_enabled:
+        Enable use of the fast calibration mode across the device
+        DEPRECATED since 5.5. This will be removed in a future
+        release.
+    temperature_target:
+        If the device is capable (see
+        device.get_device_info().temperature_controllable) then this
+        sets the minimum and maximum temperatures of the flow-cell.
+        These values must be between the limits specified in the
+        application config, see: min_user_setpoint_temperature_celsius
+        and max_user_setpoint_temperature_celsius
+    timings:
+        If specified, the device will adopt these timings to set how
+        long is spent at various stages of the current digitisation
+        processes. The message includes a way of returning to default
+        timings.  This value cannot be changed during acquisition
+"""
+GetPixelSettingsResponse.__doc__ = """Attributes:
+    pixels:
+        List of all requested pixel settings, in the order requested.
+"""
+GetPixelSettingsRequest.__doc__ = """Attributes:
+    pixels:
+        The channels (one based) to return data for. A sparse map is
+        accepted
+"""
+PixelSettings.__doc__ = """Attributes:
+    input:
+        The input driving the adv
+    overload_mode:
+        The mode the asic uses to handle currents that go above its
+        adc range.
+    cutoff_frequency:
+        Signal filter for input adc signal.
+    gain_multiplier:
+        Signal gain multiplier, applied to the integrator circuit.
+    gain_capacitor:
+        Gain capacitor, used in the integrtor circuit.
+    calibration_mode:
+        The calibration mode to use.
+    unblock_voltage:
+        Controls the application of the unblock voltage to the pixel.
+    current_inverted:
+        Inverts the current's polarity.
+    membrane_simulation_enabled:
+        Control the state of the membrane simulation.
+    regeneration_current:
+        Control the regeneration current used when regenerating
+        well's.
+    regeneration_current_test_enabled:
+        Control if the regeneration current test is enabled.  This
+        connects the regeneration current to the integration adc
+        circuit and the input well. and allows users to read regen
+        current via the channel adc value.
+    bias_current:
+        The bias current for the amplifier - this controls the level
+        of noise of the signal.  The higher the bias current, the
+        lower the noise, but the bigger the heat and power drawn by
+        the amplifier. If it is set to off, no signal readings can be
+        made.
+"""
+PixelSettings.InputWell.__doc__ = """Attributes:
+    input_well:
+        Control which well is driving the adc minknow reads from.  ALL
+        is not a valid value here (other values are acceptable).
+    regeneration_well:
+        Control which wells are being regenerated (has the specified
+        regeneration current driven to it).  All possible Input values
+        are acceptable, as long as the input is not the active adc
+        input. For example, { input: 1, regeneration: all } is
+        invalid, as an well cannot be both input and regenerated.
+"""
+ChangePixelSettingsRequest.__doc__ = """Attributes:
+    pixels:
+        1 based map of up to 3000 different pixel settings
+    pixel_default:
+        If supplied, contains settings applied to every pixel before
+        then applying any specific settings in the per pixel settings.
+"""
+StreamTemperatureRequest.__doc__ = """Attributes:
+    period_seconds:
+        How often temperature updates should be sent Defaults to a
+        period of 1 second, if not specified, or set to 0
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
+"""
+PixelBlockSettings.__doc__ = """Attributes:
+    regen_current_voltage_clamp:
+        Voltage clamp for regeneration circuit (in millivolts)  The
+        voltage in the regeneration circuit is clamped under this
+        value, whilst applying the current specified in each pixel's
+        settings.  The acceptable input range is -1000..1000
+        (inclusive)
+    unblock_voltage:
+        The unblock voltage to apply when a pixel is unblocking.  The
+        acceptable input range is -1000..1000 (inclusive)
+"""
+TimingEnginePeriods.__doc__ = """ Timing-engine periods are specified in 5ns units. Some of the timing
+mechanism can only achieve 10ns accuracy, so even numbers are
+preferred.  Note: There is a timing feature in the ASIC that requires
+the sum of the RST1 and DATA periods to be a multiple of 16
+
+Attributes:
+    RST1:
+        Reset1 phase  Note: Commands are written to the ASIC during
+        this period, to allow sufficient time to write the commands,
+        this should never be less than 1.2us or 240.
+    RST1_CDS1:
+        Reset1 to CDS1 transition
+    CDS1:
+        CDS1 phase (Correlated Double Sampling) sample-point 1
+    CDS1_DATA:
+        CDS1 to DATA transiton
+    DATA:
+        DATA transfer phase  NOTE: Setting this value has no effect,
+        MinKNOW will choose a value for DATA itself to acheive the
+        required frame-rate. Reading it will return the chosen DATA
+        period.
+    DATA_RST2:
+        DATA transfer to Reset2 transition. MinKNOW may increase this
+        value by small amounts so that when changing the DATA period,
+        the sum of the RST1 and DATA periods is a multiple of 16 and
+        the frame-rate and integration-period are maintained.
+    RST2:
+        Reset2
+    RST2_CDS2:
+        Reset2 to CDS2 transition
+    CDS2:
+        CDS2 Phase (sample-point 2)
+    CDS2_SH:
+        CDS2 to SH transition
+    SH:
+        SH phase (Sample and Hold)
+    SH_RST1:
+        SH to Reset1 transition
+    use_default_values:
+        If written true, other fields will be ignored and the hardware
+        will use default timings. When read will return true if
+        previously set true, it will not tell you if the timing
+        periods you previously entered are the same as the default
+        values.
+"""
+GetTemperatureResponse.__doc__ = """Attributes:
+    target_temperature:
+        Return the temperature target the device is aiming to reach.
+    flowcell_temperature:
+        Temperature as measured by thermistor TH2 on the P-Chip.
+    chamber_temperature:
+        Flow-cell chamber-temperature, calculated from the pixel-block
+        temperatures
+    pixel_block_temperature:
+        Temperature measured at each sensor in the ASIC, there are 12
+        sensors, one sensor per pixel-block
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/promethion_device_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/promethion_device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/promethion_device_service.py` & `minknow_api-5.5.2/minknow_api/promethion_device_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,16 @@
                 Valid values are in the range -1250mv..1250mv
             bias_voltage (float, optional): The value to apply as the bias voltage (in millivolts)
 
                 Valid values are in the range -1250mv..1250mv
             bias_voltage_waveform (minknow_api.promethion_device_pb2.WaveformSettings, optional): The waveform settings
             saturation_control_enabled (google.protobuf.wrappers_pb2.BoolValue, optional): Enables saturation control on the device
             fast_calibration_enabled (google.protobuf.wrappers_pb2.BoolValue, optional): Enable use of the fast calibration mode across the device
+
+                DEPRECATED since 5.5. This will be removed in a future release.
             temperature_target (google.protobuf.wrappers_pb2.FloatValue, optional): If the device is capable (see device.get_device_info().temperature_controllable)
                 then this sets the minimum and maximum temperatures of the flow-cell.
 
                 These values must be between the limits specified in the application config,
                 see: min_user_setpoint_temperature_celsius and max_user_setpoint_temperature_celsius
             timings (minknow_api.promethion_device_pb2.TimingEnginePeriods, optional): If specified, the device will adopt these timings to set how
                 long is spent at various stages of the current digitisation processes.
```

### Comparing `minknow_api-5.4.0/minknow_api/protocol_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/protocol_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/protocol_service.py` & `minknow_api-5.5.2/minknow_api/protocol_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "TriggerMuxScanRequest",
     "TriggerMuxScanResponse",
     "ListProtocolsRequest",
     "ProtocolInfo",
     "ListProtocolsResponse",
     "WaitForFinishedRequest",
     "GetRunInfoRequest",
+    "RequestOrigin",
     "Epi2meWorkflowReference",
     "AssociatedPostProcessingAnalysis",
     "PlatformQcResult",
     "ExternalOffload",
     "ProtocolRunInfo",
     "FilteringInfo",
     "ListProtocolRunsRequest",
@@ -73,25 +74,28 @@
     "PROTOCOL_WAITING_FOR_TEMPERATURE",
     "PROTOCOL_WAITING_FOR_ACQUISITION",
     "PROTOCOL_COMPLETED",
     "PROTOCOL_STOPPED_BY_USER",
     "PROTOCOL_FINISHED_WITH_ERROR",
     "PROTOCOL_FINISHED_WITH_DEVICE_ERROR",
     "PROTOCOL_FINISHED_UNABLE_TO_SEND_TELEMETRY",
+    "PROTOCOL_FINISHED_WITH_FLOW_CELL_DISCONNECT",
+    "PROTOCOL_FINISHED_WITH_DEVICE_DISCONNECT",
     "PROTOCOL_FINISHED_WITH_ERROR_CALIBRATION",
     "PROTOCOL_FINISHED_WITH_ERROR_BASECALL_SETTINGS",
     "PROTOCOL_FINISHED_WITH_ERROR_TEMPERATURE_REQUIRED",
     "ProtocolPhase",
     "PHASE_UNKNOWN",
     "PHASE_INITIALISING",
     "PHASE_SEQUENCING",
     "PHASE_PREPARING_FOR_MUX_SCAN",
     "PHASE_MUX_SCAN",
     "PHASE_PAUSED",
     "PHASE_PAUSING",
+    "PHASE_BAD_TEMPERATURE_AUTOMATIC_PAUSE",
     "PHASE_RESUMING",
     "Action",
     "ACTION_NONE",
     "ACTION_PAUSE",
     "ACTION_RESUME",
     "ACTION_TRIGGER_MUX_SCAN",
 ]
```

### Comparing `minknow_api-5.4.0/minknow_api/protocol_settings_pb2.py` & `minknow_api-5.5.2/minknow_api/protocol_settings_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,147 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: minknow_api/protocol_settings.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from minknow_api import analysis_configuration_pb2 as minknow__api_dot_analysis__configuration__pb2
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#minknow_api/protocol_settings.proto\x12\x1dminknow_api.protocol_settings\x1a(minknow_api/analysis_configuration.proto\x1a\x1dminknow_api/rpc_options.proto\"\x85\x02\n\x1cProtocolIdentifierComponents\x12V\n\x08location\x18\x01 \x01(\x0e\x32\x44.minknow_api.protocol_settings.ProtocolIdentifierComponents.Location\x12\x17\n\x0f\x65xperiment_type\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1e\n\x16\x66low_cell_product_code\x18\x04 \x01(\t\x12\x0b\n\x03kit\x18\x05 \x01(\t\"9\n\x08Location\x12\x07\n\x03\x41NY\x10\x00\x12\x12\n\x0eSYSTEM_SCRIPTS\x10\x01\x12\x10\n\x0cUSER_SCRIPTS\x10\x02\"\xca\r\n\x0fProtocolSetting\x12I\n\x08\x63\x61tegory\x18\x01 \x01(\x0e\x32\x37.minknow_api.protocol_settings.ProtocolSetting.Category\x12\x18\n\nidentifier\x18\x02 \x01(\tB\x04\x88\xb5\x18\x01\x12\x1a\n\x0c\x64isplay_name\x18\x03 \x01(\tB\x04\x88\xb5\x18\x01\x12\x0c\n\x04help\x18\x10 \x01(\t\x12\x41\n\x04unit\x18\x05 \x01(\x0e\x32\x33.minknow_api.protocol_settings.ProtocolSetting.Unit\x12Z\n\rdefault_value\x18\x06 \x01(\x0b\x32\x43.minknow_api.protocol_settings.ProtocolSetting.ProtocolSettingValue\x12N\n\x0b\x63onstraints\x18\x07 \x03(\x0b\x32\x39.minknow_api.protocol_settings.ProtocolSetting.Constraint\x12O\n\x0c\x64\x65pendencies\x18\x08 \x03(\x0b\x32\x39.minknow_api.protocol_settings.ProtocolSetting.Dependency\x12M\n\nvisibility\x18\t \x01(\x0e\x32\x39.minknow_api.protocol_settings.ProtocolSetting.Visibility\x12\x0f\n\x07\x63hoices\x18\x11 \x03(\t\x1a\x84\x03\n\x14ProtocolSettingValue\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x12\x15\n\x0b\x66loat_value\x18\x02 \x01(\x01H\x00\x12\x17\n\rinteger_value\x18\x03 \x01(\x03H\x00\x12\x14\n\nbool_value\x18\x04 \x01(\x08H\x00\x12\x66\n\x0e\x63hannels_value\x18\x05 \x01(\x0b\x32L.minknow_api.analysis_configuration.WriterConfiguration.ChannelConfigurationH\x00\x12m\n\x12multi_string_value\x18\x06 \x01(\x0b\x32O.minknow_api.protocol_settings.ProtocolSetting.ProtocolSettingValue.MultiStringH\x00\x1a\x1d\n\x0bMultiString\x12\x0e\n\x06values\x18\x01 \x03(\tB\x18\n\x16protocol_setting_value\x1a\xb9\x02\n\nConstraint\x12V\n\tcondition\x18\x01 \x01(\x0e\x32\x43.minknow_api.protocol_settings.ProtocolSetting.Constraint.Condition\x12R\n\x05value\x18\x02 \x01(\x0b\x32\x43.minknow_api.protocol_settings.ProtocolSetting.ProtocolSettingValue\"\x7f\n\tCondition\x12\t\n\x05\x45QUAL\x10\x00\x12\r\n\tNOT_EQUAL\x10\x01\x12\t\n\x05GT_EQ\x10\x02\x12\x06\n\x02GT\x10\x03\x12\t\n\x05LT_EQ\x10\x04\x12\x06\n\x02LT\x10\x05\x12\x06\n\x02IN\x10\x06\x12\n\n\x06NOT_IN\x10\x07\x12\r\n\tENDS_WITH\x10\x08\x12\x0f\n\x0bSTARTS_WITH\x10\t\x1ap\n\nDependency\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12N\n\x0b\x63onstraints\x18\x02 \x03(\x0b\x32\x39.minknow_api.protocol_settings.ProtocolSetting.Constraint\"C\n\x08\x43\x61tegory\x12\t\n\x05OTHER\x10\x00\x12\x0f\n\x0bRUN_OPTIONS\x10\x01\x12\x0f\n\x0b\x42\x41SECALLING\x10\x02\x12\n\n\x06OUTPUT\x10\x03\"\xcc\x01\n\x04Unit\x12\x0c\n\x08UNITLESS\x10\x00\x12\x0f\n\x0bUTF8_STRING\x10\x01\x12\x10\n\x0c\x41SCII_STRING\x10\x02\x12\x08\n\x04PATH\x10\x03\x12\x07\n\x03URL\x10\x04\x12\x12\n\x0ePRIVATE_STRING\x10\x05\x12\n\n\x06\x43HOICE\x10\x06\x12\x10\n\x0cMULTI_CHOICE\x10\x07\x12\n\n\x06SECOND\x10\x08\x12\x08\n\x04HOUR\x10\t\x12\x08\n\x04\x42\x41SE\x10\n\x12\t\n\x05KBASE\x10\x0b\x12\t\n\x05MBASE\x10\x0c\x12\t\n\x05GBASE\x10\r\x12\r\n\tMILLIVOLT\x10\x0e\"?\n\nVisibility\x12\x0c\n\x08\x45\x44ITABLE\x10\x00\x12\n\n\x06HIDDEN\x10\x01\x12\t\n\x05\x46IXED\x10\x02\x12\x0c\n\x08REQUIRED\x10\x03\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-
-
-_PROTOCOLIDENTIFIERCOMPONENTS = DESCRIPTOR.message_types_by_name['ProtocolIdentifierComponents']
-_PROTOCOLSETTING = DESCRIPTOR.message_types_by_name['ProtocolSetting']
-_PROTOCOLSETTING_PROTOCOLSETTINGVALUE = _PROTOCOLSETTING.nested_types_by_name['ProtocolSettingValue']
-_PROTOCOLSETTING_PROTOCOLSETTINGVALUE_MULTISTRING = _PROTOCOLSETTING_PROTOCOLSETTINGVALUE.nested_types_by_name['MultiString']
-_PROTOCOLSETTING_CONSTRAINT = _PROTOCOLSETTING.nested_types_by_name['Constraint']
-_PROTOCOLSETTING_DEPENDENCY = _PROTOCOLSETTING.nested_types_by_name['Dependency']
-_PROTOCOLIDENTIFIERCOMPONENTS_LOCATION = _PROTOCOLIDENTIFIERCOMPONENTS.enum_types_by_name['Location']
-_PROTOCOLSETTING_CONSTRAINT_CONDITION = _PROTOCOLSETTING_CONSTRAINT.enum_types_by_name['Condition']
-_PROTOCOLSETTING_CATEGORY = _PROTOCOLSETTING.enum_types_by_name['Category']
-_PROTOCOLSETTING_UNIT = _PROTOCOLSETTING.enum_types_by_name['Unit']
-_PROTOCOLSETTING_VISIBILITY = _PROTOCOLSETTING.enum_types_by_name['Visibility']
-ProtocolIdentifierComponents = _reflection.GeneratedProtocolMessageType('ProtocolIdentifierComponents', (_message.Message,), {
-  'DESCRIPTOR' : _PROTOCOLIDENTIFIERCOMPONENTS,
-  '__module__' : 'minknow_api.protocol_settings_pb2'
-  ,
-  '__doc__': """Attributes:
-      location:
-          If not specified, will default to "ANY"
-      experiment_type:
-          one of "custom", "sequencing", "control", "ctc", "platform qc"
-          or "flowcell_plugin"
-      name:
-          Name (or path) of the protocol, without the .toml extension
-          eg: "sequencing/sequencing_MIN106_DNA" this is relative to the
-          system or user protocol directory
-      flow_cell_product_code:
-          eg: "FLO-MIN106"
-      kit:
-          eg: "SQK-RPB004"
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.protocol_settings.ProtocolIdentifierComponents)
-  })
-_sym_db.RegisterMessage(ProtocolIdentifierComponents)
-
-ProtocolSetting = _reflection.GeneratedProtocolMessageType('ProtocolSetting', (_message.Message,), {
-
-  'ProtocolSettingValue' : _reflection.GeneratedProtocolMessageType('ProtocolSettingValue', (_message.Message,), {
-
-    'MultiString' : _reflection.GeneratedProtocolMessageType('MultiString', (_message.Message,), {
-      'DESCRIPTOR' : _PROTOCOLSETTING_PROTOCOLSETTINGVALUE_MULTISTRING,
-      '__module__' : 'minknow_api.protocol_settings_pb2'
-      # @@protoc_insertion_point(class_scope:minknow_api.protocol_settings.ProtocolSetting.ProtocolSettingValue.MultiString)
-      })
-    ,
-    'DESCRIPTOR' : _PROTOCOLSETTING_PROTOCOLSETTINGVALUE,
-    '__module__' : 'minknow_api.protocol_settings_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.protocol_settings.ProtocolSetting.ProtocolSettingValue)
-    })
-  ,
-
-  'Constraint' : _reflection.GeneratedProtocolMessageType('Constraint', (_message.Message,), {
-    'DESCRIPTOR' : _PROTOCOLSETTING_CONSTRAINT,
-    '__module__' : 'minknow_api.protocol_settings_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.protocol_settings.ProtocolSetting.Constraint)
-    })
-  ,
-
-  'Dependency' : _reflection.GeneratedProtocolMessageType('Dependency', (_message.Message,), {
-    'DESCRIPTOR' : _PROTOCOLSETTING_DEPENDENCY,
-    '__module__' : 'minknow_api.protocol_settings_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.protocol_settings.ProtocolSetting.Dependency)
-    })
-  ,
-  'DESCRIPTOR' : _PROTOCOLSETTING,
-  '__module__' : 'minknow_api.protocol_settings_pb2'
-  ,
-  '__doc__': """Attributes:
-      identifier:
-          Identifier is the unique primary-key for referring to
-          protocol-settings, dependencies refer to other settings via
-          their identifier.
-      help:
-          Optional additional help text for a setting that may be shown
-          to the user if required.
-      constraints:
-          All constraints must be met if this setting is to be
-          considered valid
-      dependencies:
-          If any of the dependencies matches it's constraints, this
-          setting should adopt the level of visibility specified in
-          "visibility". If none of the dependencies match their
-          constraints, then "visibility" should be ignored and the
-          option should be hidden from the user.  Some dependencies may
-          be specified multiple times, but with mutually exclusive
-          constraints, for example if the setting controls data
-          compression level, where there is a compression_algorithm
-          setting specified by a string that can have the values "X",
-          "Y" or "None". The setting may be dependent on
-          compression_algorithm equals "X" or compression_algorithm
-          equals "Y". If the compression_algorithm is "None" then none
-          of the dependency constraints will be met and the setting
-          should be hidden. A typical arrangement of fields in this case
-          would be: Dependency {   identifier: "compression_algorithm",
-          Constraint {     condition : EQUAL,     value: "X"   } }
-          Dependency {   identifier: "compression_algorithm",
-          Constraint {     condition : EQUAL,     value: "Y"   } } When
-          a dependency is specified with multiple constraints they must
-          all be met before the dependency is considered satisfied, for
-          example some other setting may be dependent on
-          compression_level being in a range (0,10] :  Dependency {
-          identifier: "compression_level",   Constraint {     condition
-          : GT,     value: 0   },   Constraint {     condition : LT_EQ,
-          value: 10   } }
-      visibility:
-          If any of the dependencies match their constraints, this level
-          of visibility should be adopted. It should also be adopted if
-          no dependencies are specified.
-      choices:
-          when unit is CHOICE, this defines the acceptable choices.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.protocol_settings.ProtocolSetting)
-  })
-_sym_db.RegisterMessage(ProtocolSetting)
-_sym_db.RegisterMessage(ProtocolSetting.ProtocolSettingValue)
-_sym_db.RegisterMessage(ProtocolSetting.ProtocolSettingValue.MultiString)
-_sym_db.RegisterMessage(ProtocolSetting.Constraint)
-_sym_db.RegisterMessage(ProtocolSetting.Dependency)
-
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.protocol_settings_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
   _PROTOCOLSETTING.fields_by_name['identifier']._options = None
   _PROTOCOLSETTING.fields_by_name['identifier']._serialized_options = b'\210\265\030\001'
   _PROTOCOLSETTING.fields_by_name['display_name']._options = None
@@ -164,8 +45,67 @@
   _PROTOCOLSETTING_DEPENDENCY._serialized_end=1805
   _PROTOCOLSETTING_CATEGORY._serialized_start=1807
   _PROTOCOLSETTING_CATEGORY._serialized_end=1874
   _PROTOCOLSETTING_UNIT._serialized_start=1877
   _PROTOCOLSETTING_UNIT._serialized_end=2081
   _PROTOCOLSETTING_VISIBILITY._serialized_start=2083
   _PROTOCOLSETTING_VISIBILITY._serialized_end=2146
+ProtocolIdentifierComponents.__doc__ = """Attributes:
+    location:
+        If not specified, will default to "ANY"
+    experiment_type:
+        one of "custom", "sequencing", "control", "ctc", "platform qc"
+        or "flowcell_plugin"
+    name:
+        Name (or path) of the protocol, without the .toml extension
+        eg: "sequencing/sequencing_MIN106_DNA" this is relative to the
+        system or user protocol directory
+    flow_cell_product_code:
+        eg: "FLO-MIN106"
+    kit:
+        eg: "SQK-RPB004"
+"""
+ProtocolSetting.__doc__ = """Attributes:
+    identifier:
+        Identifier is the unique primary-key for referring to
+        protocol-settings, dependencies refer to other settings via
+        their identifier.
+    help:
+        Optional additional help text for a setting that may be shown
+        to the user if required.
+    constraints:
+        All constraints must be met if this setting is to be
+        considered valid
+    dependencies:
+        If any of the dependencies matches it's constraints, this
+        setting should adopt the level of visibility specified in
+        "visibility". If none of the dependencies match their
+        constraints, then "visibility" should be ignored and the
+        option should be hidden from the user.  Some dependencies may
+        be specified multiple times, but with mutually exclusive
+        constraints, for example if the setting controls data
+        compression level, where there is a compression_algorithm
+        setting specified by a string that can have the values "X",
+        "Y" or "None". The setting may be dependent on
+        compression_algorithm equals "X" or compression_algorithm
+        equals "Y". If the compression_algorithm is "None" then none
+        of the dependency constraints will be met and the setting
+        should be hidden. A typical arrangement of fields in this case
+        would be: Dependency {   identifier: "compression_algorithm",
+        Constraint {     condition : EQUAL,     value: "X"   } }
+        Dependency {   identifier: "compression_algorithm",
+        Constraint {     condition : EQUAL,     value: "Y"   } } When
+        a dependency is specified with multiple constraints they must
+        all be met before the dependency is considered satisfied, for
+        example some other setting may be dependent on
+        compression_level being in a range (0,10] :  Dependency {
+        identifier: "compression_level",   Constraint {     condition
+        : GT,     value: 0   },   Constraint {     condition : LT_EQ,
+        value: 10   } }
+    visibility:
+        If any of the dependencies match their constraints, this level
+        of visibility should be adopted. It should also be adopted if
+        no dependencies are specified.
+    choices:
+        when unit is CHOICE, this defines the acceptable choices.
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/protocol_settings_service.py` & `minknow_api-5.5.2/minknow_api/protocol_settings_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/report_data_service.py` & `minknow_api-5.5.2/minknow_api/report_data_service.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/rpc_options_pb2.py` & `minknow_api-5.5.2/minknow_api/rpc_options_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: minknow_api/rpc_options.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dminknow_api/rpc_options.proto\x12\x0bminknow_api\x1a google/protobuf/descriptor.proto:5\n\x0crpc_required\x12\x1d.google.protobuf.FieldOptions\x18\xd1\x86\x03 \x01(\x08:3\n\nrpc_unwrap\x12\x1d.google.protobuf.FieldOptions\x18\xd2\x86\x03 \x01(\x08:6\n\x0c\x65xperimental\x12\x1e.google.protobuf.MethodOptions\x18\xd3\x86\x03 \x01(\x08\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-
-RPC_REQUIRED_FIELD_NUMBER = 50001
-rpc_required = DESCRIPTOR.extensions_by_name['rpc_required']
-RPC_UNWRAP_FIELD_NUMBER = 50002
-rpc_unwrap = DESCRIPTOR.extensions_by_name['rpc_unwrap']
-EXPERIMENTAL_FIELD_NUMBER = 50003
-experimental = DESCRIPTOR.extensions_by_name['experimental']
-
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.rpc_options_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(rpc_required)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(rpc_unwrap)
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(experimental)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
```

### Comparing `minknow_api-5.4.0/minknow_api/run_until_pb2.py` & `minknow_api-5.5.2/minknow_api/run_until_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,488 +1,583 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: minknow_api/run_until.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
-from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bminknow_api/run_until.proto\x12\x15minknow_api.run_until\x1a\x1dminknow_api/rpc_options.proto\x1a\x19google/protobuf/any.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x9e\x01\n\x0e\x43riteriaValues\x12\x45\n\x08\x63riteria\x18\x01 \x03(\x0b\x32\x33.minknow_api.run_until.CriteriaValues.CriteriaEntry\x1a\x45\n\rCriteriaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"\x1c\n\x1aGetStandardCriteriaRequest\"V\n\x1bGetStandardCriteriaResponse\x12\x37\n\x08\x63riteria\x18\x01 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\"\xbb\x01\n\x1aWriteTargetCriteriaRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12=\n\x0epause_criteria\x18\x02 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\x12<\n\rstop_criteria\x18\x03 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\"\x1d\n\x1bWriteTargetCriteriaResponse\"?\n\x1bStreamTargetCriteriaRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"\x9b\x01\n\x1cStreamTargetCriteriaResponse\x12=\n\x0epause_criteria\x18\x01 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\x12<\n\rstop_criteria\x18\x02 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\"~\n\x1aWriteCustomProgressRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12>\n\x0f\x63riteria_values\x18\x02 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\"\x1d\n\x1bWriteCustomProgressResponse\"9\n\x15StreamProgressRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"X\n\x16StreamProgressResponse\x12>\n\x0f\x63riteria_values\x18\x01 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\"\x98\x06\n\x1c\x45stimatedTimeRemainingUpdate\x12[\n\x0fpause_estimates\x18\x01 \x01(\x0b\x32\x42.minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedTimes\x12Z\n\x0estop_estimates\x18\x02 \x01(\x0b\x32\x42.minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedTimes\x1a\x0e\n\x0cNotEstimated\x1ag\n\tEstimated\x12,\n\x08min_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08max_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\xc7\x01\n\rEstimatedTime\x12Y\n\rnot_estimated\x18\x01 \x01(\x0b\x32@.minknow_api.run_until.EstimatedTimeRemainingUpdate.NotEstimatedH\x00\x12R\n\testimated\x18\x02 \x01(\x0b\x32=.minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedH\x00\x42\x07\n\x05value\x1a\xfb\x01\n\x0e\x45stimatedTimes\x12o\n\x0f\x65stimated_times\x18\x01 \x03(\x0b\x32V.minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedTimes.EstimatedTimesEntry\x1ax\n\x13\x45stimatedTimesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12P\n\x05value\x18\x02 \x01(\x0b\x32\x41.minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedTime:\x02\x38\x01\"\x88\x01\n\x0c\x41\x63tionUpdate\x12:\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32*.minknow_api.run_until.ActionUpdate.Action\"<\n\x06\x41\x63tion\x12\x0c\n\x08NoAction\x10\x00\x12\n\n\x06Paused\x10\x01\x12\x0b\n\x07Resumed\x10\x02\x12\x0b\n\x07Stopped\x10\x03\"\xb9\x01\n\x0cScriptUpdate\x12<\n\x07started\x18\x01 \x01(\x0b\x32+.minknow_api.run_until.ScriptUpdate.Started\x12M\n\x10\x63riteria_updated\x18\x02 \x01(\x0b\x32\x33.minknow_api.run_until.ScriptUpdate.CriteriaUpdated\x1a\t\n\x07Started\x1a\x11\n\x0f\x43riteriaUpdated\"\xec\x01\n\x0b\x45rrorUpdate\x12N\n\x10invalid_criteria\x18\x01 \x01(\x0b\x32\x32.minknow_api.run_until.ErrorUpdate.InvalidCriteriaH\x00\x12\x44\n\x0bother_error\x18\x0f \x01(\x0b\x32-.minknow_api.run_until.ErrorUpdate.OtherErrorH\x00\x1a\x1f\n\x0fInvalidCriteria\x12\x0c\n\x04name\x18\x01 \x03(\t\x1a\x1d\n\nOtherError\x12\x0f\n\x07message\x18\x01 \x01(\tB\x07\n\x05\x65rror\"\x85\x03\n\x06Update\x12\\\n\x1f\x65stimated_time_remaining_update\x18\x01 \x01(\x0b\x32\x33.minknow_api.run_until.EstimatedTimeRemainingUpdate\x12:\n\raction_update\x18\x02 \x01(\x0b\x32#.minknow_api.run_until.ActionUpdate\x12:\n\rscript_update\x18\x03 \x01(\x0b\x32#.minknow_api.run_until.ScriptUpdate\x12\x46\n\x17\x63urrent_progress_update\x18\x05 \x01(\x0b\x32%.minknow_api.run_until.CriteriaValues\x12\x38\n\x0c\x65rror_update\x18\x0e \x01(\x0b\x32\".minknow_api.run_until.ErrorUpdate\x12#\n\x05other\x18\x0f \x03(\x0b\x32\x14.google.protobuf.Any\"f\n\x13WriteUpdatesRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12-\n\x06update\x18\x02 \x01(\x0b\x32\x1d.minknow_api.run_until.Update\"\x16\n\x14WriteUpdatesResponse\"K\n\x14StreamUpdatesRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12\x11\n\tstart_idx\x18\x02 \x01(\x04\"}\n\x15StreamUpdatesResponse\x12\x0b\n\x03idx\x18\x01 \x01(\x04\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x06update\x18\x03 \x01(\x0b\x32\x1d.minknow_api.run_until.Update2\xfb\x06\n\x0fRunUntilService\x12\x80\x01\n\x15get_standard_criteria\x12\x31.minknow_api.run_until.GetStandardCriteriaRequest\x1a\x32.minknow_api.run_until.GetStandardCriteriaResponse\"\x00\x12\x80\x01\n\x15write_target_criteria\x12\x31.minknow_api.run_until.WriteTargetCriteriaRequest\x1a\x32.minknow_api.run_until.WriteTargetCriteriaResponse\"\x00\x12\x85\x01\n\x16stream_target_criteria\x12\x32.minknow_api.run_until.StreamTargetCriteriaRequest\x1a\x33.minknow_api.run_until.StreamTargetCriteriaResponse\"\x00\x30\x01\x12\x84\x01\n\x15write_custom_progress\x12\x31.minknow_api.run_until.WriteCustomProgressRequest\x1a\x32.minknow_api.run_until.WriteCustomProgressResponse\"\x04\x98\xb5\x18\x01\x12v\n\x0fstream_progress\x12,.minknow_api.run_until.StreamProgressRequest\x1a-.minknow_api.run_until.StreamProgressResponse\"\x04\x98\xb5\x18\x01\x30\x01\x12j\n\rwrite_updates\x12*.minknow_api.run_until.WriteUpdatesRequest\x1a+.minknow_api.run_until.WriteUpdatesResponse\"\x00\x12o\n\x0estream_updates\x12+.minknow_api.run_until.StreamUpdatesRequest\x1a,.minknow_api.run_until.StreamUpdatesResponse\"\x00\x30\x01\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
-
-
-
-_CRITERIAVALUES = DESCRIPTOR.message_types_by_name['CriteriaValues']
-_CRITERIAVALUES_CRITERIAENTRY = _CRITERIAVALUES.nested_types_by_name['CriteriaEntry']
-_GETSTANDARDCRITERIAREQUEST = DESCRIPTOR.message_types_by_name['GetStandardCriteriaRequest']
-_GETSTANDARDCRITERIARESPONSE = DESCRIPTOR.message_types_by_name['GetStandardCriteriaResponse']
-_WRITETARGETCRITERIAREQUEST = DESCRIPTOR.message_types_by_name['WriteTargetCriteriaRequest']
-_WRITETARGETCRITERIARESPONSE = DESCRIPTOR.message_types_by_name['WriteTargetCriteriaResponse']
-_STREAMTARGETCRITERIAREQUEST = DESCRIPTOR.message_types_by_name['StreamTargetCriteriaRequest']
-_STREAMTARGETCRITERIARESPONSE = DESCRIPTOR.message_types_by_name['StreamTargetCriteriaResponse']
-_WRITECUSTOMPROGRESSREQUEST = DESCRIPTOR.message_types_by_name['WriteCustomProgressRequest']
-_WRITECUSTOMPROGRESSRESPONSE = DESCRIPTOR.message_types_by_name['WriteCustomProgressResponse']
-_STREAMPROGRESSREQUEST = DESCRIPTOR.message_types_by_name['StreamProgressRequest']
-_STREAMPROGRESSRESPONSE = DESCRIPTOR.message_types_by_name['StreamProgressResponse']
-_ESTIMATEDTIMEREMAININGUPDATE = DESCRIPTOR.message_types_by_name['EstimatedTimeRemainingUpdate']
-_ESTIMATEDTIMEREMAININGUPDATE_NOTESTIMATED = _ESTIMATEDTIMEREMAININGUPDATE.nested_types_by_name['NotEstimated']
-_ESTIMATEDTIMEREMAININGUPDATE_ESTIMATED = _ESTIMATEDTIMEREMAININGUPDATE.nested_types_by_name['Estimated']
-_ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIME = _ESTIMATEDTIMEREMAININGUPDATE.nested_types_by_name['EstimatedTime']
-_ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES = _ESTIMATEDTIMEREMAININGUPDATE.nested_types_by_name['EstimatedTimes']
-_ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES_ESTIMATEDTIMESENTRY = _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES.nested_types_by_name['EstimatedTimesEntry']
-_ACTIONUPDATE = DESCRIPTOR.message_types_by_name['ActionUpdate']
-_SCRIPTUPDATE = DESCRIPTOR.message_types_by_name['ScriptUpdate']
-_SCRIPTUPDATE_STARTED = _SCRIPTUPDATE.nested_types_by_name['Started']
-_SCRIPTUPDATE_CRITERIAUPDATED = _SCRIPTUPDATE.nested_types_by_name['CriteriaUpdated']
-_ERRORUPDATE = DESCRIPTOR.message_types_by_name['ErrorUpdate']
-_ERRORUPDATE_INVALIDCRITERIA = _ERRORUPDATE.nested_types_by_name['InvalidCriteria']
-_ERRORUPDATE_OTHERERROR = _ERRORUPDATE.nested_types_by_name['OtherError']
-_UPDATE = DESCRIPTOR.message_types_by_name['Update']
-_WRITEUPDATESREQUEST = DESCRIPTOR.message_types_by_name['WriteUpdatesRequest']
-_WRITEUPDATESRESPONSE = DESCRIPTOR.message_types_by_name['WriteUpdatesResponse']
-_STREAMUPDATESREQUEST = DESCRIPTOR.message_types_by_name['StreamUpdatesRequest']
-_STREAMUPDATESRESPONSE = DESCRIPTOR.message_types_by_name['StreamUpdatesResponse']
-_ACTIONUPDATE_ACTION = _ACTIONUPDATE.enum_types_by_name['Action']
-CriteriaValues = _reflection.GeneratedProtocolMessageType('CriteriaValues', (_message.Message,), {
-
-  'CriteriaEntry' : _reflection.GeneratedProtocolMessageType('CriteriaEntry', (_message.Message,), {
-    'DESCRIPTOR' : _CRITERIAVALUES_CRITERIAENTRY,
-    '__module__' : 'minknow_api.run_until_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.CriteriaValues.CriteriaEntry)
-    })
-  ,
-  'DESCRIPTOR' : _CRITERIAVALUES,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """A map of criterion name -> value  This message is deliberately
-  flexible, to allow custom Run-Until Scripts to expand the range and
-  types of available criteria.""",
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.CriteriaValues)
-  })
-_sym_db.RegisterMessage(CriteriaValues)
-_sym_db.RegisterMessage(CriteriaValues.CriteriaEntry)
-
-GetStandardCriteriaRequest = _reflection.GeneratedProtocolMessageType('GetStandardCriteriaRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETSTANDARDCRITERIAREQUEST,
-  '__module__' : 'minknow_api.run_until_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.GetStandardCriteriaRequest)
-  })
-_sym_db.RegisterMessage(GetStandardCriteriaRequest)
-
-GetStandardCriteriaResponse = _reflection.GeneratedProtocolMessageType('GetStandardCriteriaResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETSTANDARDCRITERIARESPONSE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      criteria:
-          A list of valid criteria  An empty value is included for each
-          criterion, to indicate the required type of that criterion.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.GetStandardCriteriaResponse)
-  })
-_sym_db.RegisterMessage(GetStandardCriteriaResponse)
-
-WriteTargetCriteriaRequest = _reflection.GeneratedProtocolMessageType('WriteTargetCriteriaRequest', (_message.Message,), {
-  'DESCRIPTOR' : _WRITETARGETCRITERIAREQUEST,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition to set the Run-Until Criteria for
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.WriteTargetCriteriaRequest)
-  })
-_sym_db.RegisterMessage(WriteTargetCriteriaRequest)
-
-WriteTargetCriteriaResponse = _reflection.GeneratedProtocolMessageType('WriteTargetCriteriaResponse', (_message.Message,), {
-  'DESCRIPTOR' : _WRITETARGETCRITERIARESPONSE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.WriteTargetCriteriaResponse)
-  })
-_sym_db.RegisterMessage(WriteTargetCriteriaResponse)
-
-StreamTargetCriteriaRequest = _reflection.GeneratedProtocolMessageType('StreamTargetCriteriaRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMTARGETCRITERIAREQUEST,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition to obtain the Run-Until Criteria for
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.StreamTargetCriteriaRequest)
-  })
-_sym_db.RegisterMessage(StreamTargetCriteriaRequest)
-
-StreamTargetCriteriaResponse = _reflection.GeneratedProtocolMessageType('StreamTargetCriteriaResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMTARGETCRITERIARESPONSE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.StreamTargetCriteriaResponse)
-  })
-_sym_db.RegisterMessage(StreamTargetCriteriaResponse)
-
-WriteCustomProgressRequest = _reflection.GeneratedProtocolMessageType('WriteCustomProgressRequest', (_message.Message,), {
-  'DESCRIPTOR' : _WRITECUSTOMPROGRESSREQUEST,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition this Run-Until progress update relates to
-      criteria_values:
-          The current Run-Until criteria state  A Run-Until progress
-          update need not contain updates for all criteria.  It must not
-          contain updates for "standard" criteria
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.WriteCustomProgressRequest)
-  })
-_sym_db.RegisterMessage(WriteCustomProgressRequest)
-
-WriteCustomProgressResponse = _reflection.GeneratedProtocolMessageType('WriteCustomProgressResponse', (_message.Message,), {
-  'DESCRIPTOR' : _WRITECUSTOMPROGRESSRESPONSE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.WriteCustomProgressResponse)
-  })
-_sym_db.RegisterMessage(WriteCustomProgressResponse)
-
-StreamProgressRequest = _reflection.GeneratedProtocolMessageType('StreamProgressRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMPROGRESSREQUEST,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition to obtain the Run-Until progress updates for
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.StreamProgressRequest)
-  })
-_sym_db.RegisterMessage(StreamProgressRequest)
-
-StreamProgressResponse = _reflection.GeneratedProtocolMessageType('StreamProgressResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMPROGRESSRESPONSE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      criteria_values:
-          The run until criteria status  The criteria will always
-          contain the `runtime` field, which acts as a timestamp for the
-          message.  A Run-Until progress update need not contain updates
-          for all criteria.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.StreamProgressResponse)
-  })
-_sym_db.RegisterMessage(StreamProgressResponse)
-
-EstimatedTimeRemainingUpdate = _reflection.GeneratedProtocolMessageType('EstimatedTimeRemainingUpdate', (_message.Message,), {
-
-  'NotEstimated' : _reflection.GeneratedProtocolMessageType('NotEstimated', (_message.Message,), {
-    'DESCRIPTOR' : _ESTIMATEDTIMEREMAININGUPDATE_NOTESTIMATED,
-    '__module__' : 'minknow_api.run_until_pb2'
-    ,
-    '__doc__': """Indicates that a time is not estimated""",
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.EstimatedTimeRemainingUpdate.NotEstimated)
-    })
-  ,
-
-  'Estimated' : _reflection.GeneratedProtocolMessageType('Estimated', (_message.Message,), {
-    'DESCRIPTOR' : _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATED,
-    '__module__' : 'minknow_api.run_until_pb2'
-    ,
-    '__doc__': """ These times are estimates of the (UTC) time at which the condition
-    will be fulfilled  Some idea of the expected accuracy of this estimate
-    can be obtained by comparing `min_time` with `max_time`.  If the
-    estimated time is believed to be accurate (e.g. for a "runtime"
-    criterion), then `min_time` may be equal to `max_time`.  Otherwise, if
-    the estimate is believed to be inaccurate (e.g. for a "pore_scan"
-    criterion which is not close to being fulfilled), then `min_time` and
-    `max_time` may differ significantly.
-    
-    Attributes:
-        min_time:
-            Estimated lower bound on the time at which the condition will
-            occur (UTC)
-        max_time:
-            Estimated upper bound on the time at which the condition will
-            occur (UTC)
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.EstimatedTimeRemainingUpdate.Estimated)
-    })
-  ,
-
-  'EstimatedTime' : _reflection.GeneratedProtocolMessageType('EstimatedTime', (_message.Message,), {
-    'DESCRIPTOR' : _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIME,
-    '__module__' : 'minknow_api.run_until_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedTime)
-    })
-  ,
-
-  'EstimatedTimes' : _reflection.GeneratedProtocolMessageType('EstimatedTimes', (_message.Message,), {
-
-    'EstimatedTimesEntry' : _reflection.GeneratedProtocolMessageType('EstimatedTimesEntry', (_message.Message,), {
-      'DESCRIPTOR' : _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES_ESTIMATEDTIMESENTRY,
-      '__module__' : 'minknow_api.run_until_pb2'
-      # @@protoc_insertion_point(class_scope:minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedTimes.EstimatedTimesEntry)
-      })
-    ,
-    'DESCRIPTOR' : _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES,
-    '__module__' : 'minknow_api.run_until_pb2'
-    ,
-    '__doc__': """Map of Run-Until Criterion to `EstimatedTime` when the criterion will
-    be fulfilled  Only criteria for which an update is being provided are
-    contained in the map.""",
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.EstimatedTimeRemainingUpdate.EstimatedTimes)
-    })
-  ,
-  'DESCRIPTOR' : _ESTIMATEDTIMEREMAININGUPDATE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Indicates the estimated time remaining  An estimated time may be
-  provided for each Run-Until Criterion that is specified as an end-
-  point.""",
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.EstimatedTimeRemainingUpdate)
-  })
-_sym_db.RegisterMessage(EstimatedTimeRemainingUpdate)
-_sym_db.RegisterMessage(EstimatedTimeRemainingUpdate.NotEstimated)
-_sym_db.RegisterMessage(EstimatedTimeRemainingUpdate.Estimated)
-_sym_db.RegisterMessage(EstimatedTimeRemainingUpdate.EstimatedTime)
-_sym_db.RegisterMessage(EstimatedTimeRemainingUpdate.EstimatedTimes)
-_sym_db.RegisterMessage(EstimatedTimeRemainingUpdate.EstimatedTimes.EstimatedTimesEntry)
-
-ActionUpdate = _reflection.GeneratedProtocolMessageType('ActionUpdate', (_message.Message,), {
-  'DESCRIPTOR' : _ACTIONUPDATE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Indicates that an action has been performed  When a request is sent
-  using `write_updates()`, MinKNOW performs the specified action.""",
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.ActionUpdate)
-  })
-_sym_db.RegisterMessage(ActionUpdate)
-
-ScriptUpdate = _reflection.GeneratedProtocolMessageType('ScriptUpdate', (_message.Message,), {
-
-  'Started' : _reflection.GeneratedProtocolMessageType('Started', (_message.Message,), {
-    'DESCRIPTOR' : _SCRIPTUPDATE_STARTED,
-    '__module__' : 'minknow_api.run_until_pb2'
-    ,
-    '__doc__': """Indicates that the run-until script has started and is running""",
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.ScriptUpdate.Started)
-    })
-  ,
-
-  'CriteriaUpdated' : _reflection.GeneratedProtocolMessageType('CriteriaUpdated', (_message.Message,), {
-    'DESCRIPTOR' : _SCRIPTUPDATE_CRITERIAUPDATED,
-    '__module__' : 'minknow_api.run_until_pb2'
-    ,
-    '__doc__': """Indicates the the Run-Until Script has update its criteria in response
-    to receiving a `StreamTargetCriteriaResponse` message""",
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.ScriptUpdate.CriteriaUpdated)
-    })
-  ,
-  'DESCRIPTOR' : _SCRIPTUPDATE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.ScriptUpdate)
-  })
-_sym_db.RegisterMessage(ScriptUpdate)
-_sym_db.RegisterMessage(ScriptUpdate.Started)
-_sym_db.RegisterMessage(ScriptUpdate.CriteriaUpdated)
-
-ErrorUpdate = _reflection.GeneratedProtocolMessageType('ErrorUpdate', (_message.Message,), {
-
-  'InvalidCriteria' : _reflection.GeneratedProtocolMessageType('InvalidCriteria', (_message.Message,), {
-    'DESCRIPTOR' : _ERRORUPDATE_INVALIDCRITERIA,
-    '__module__' : 'minknow_api.run_until_pb2'
-    ,
-    '__doc__': """Indicates that one or more of the supplied target criteria is not
-    recognised by the  Run-Until Script.  Unrecognised target criteria
-    will not be used to pause or stop the run.""",
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.ErrorUpdate.InvalidCriteria)
-    })
-  ,
-
-  'OtherError' : _reflection.GeneratedProtocolMessageType('OtherError', (_message.Message,), {
-    'DESCRIPTOR' : _ERRORUPDATE_OTHERERROR,
-    '__module__' : 'minknow_api.run_until_pb2'
-    ,
-    '__doc__': """An error that is not covered by one of the other error types, above.""",
-    # @@protoc_insertion_point(class_scope:minknow_api.run_until.ErrorUpdate.OtherError)
-    })
-  ,
-  'DESCRIPTOR' : _ERRORUPDATE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Indicates that a problem has been encountered by the Run-Until Script""",
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.ErrorUpdate)
-  })
-_sym_db.RegisterMessage(ErrorUpdate)
-_sym_db.RegisterMessage(ErrorUpdate.InvalidCriteria)
-_sym_db.RegisterMessage(ErrorUpdate.OtherError)
-
-Update = _reflection.GeneratedProtocolMessageType('Update', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      current_progress_update:
-          Gives the current values of the criteria (Compare to
-          stream_target_criteria call to see %)
-      other:
-          Space for custom updates from custom Run-Until scripts
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.Update)
-  })
-_sym_db.RegisterMessage(Update)
-
-WriteUpdatesRequest = _reflection.GeneratedProtocolMessageType('WriteUpdatesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _WRITEUPDATESREQUEST,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition this Run-Until update applies to
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.WriteUpdatesRequest)
-  })
-_sym_db.RegisterMessage(WriteUpdatesRequest)
-
-WriteUpdatesResponse = _reflection.GeneratedProtocolMessageType('WriteUpdatesResponse', (_message.Message,), {
-  'DESCRIPTOR' : _WRITEUPDATESRESPONSE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.WriteUpdatesResponse)
-  })
-_sym_db.RegisterMessage(WriteUpdatesResponse)
-
-StreamUpdatesRequest = _reflection.GeneratedProtocolMessageType('StreamUpdatesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMUPDATESREQUEST,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition to stream Run-Until updates for
-      start_idx:
-          The index of the first update to send.  If an index is set
-          that is greater than the current greatest update index, no
-          past updates will be sent, but any future updates will be
-          sent.  This may mean that you receive updates with an `idx`
-          smaller than `start_idx`.  In order to receive only updates
-          that are sent after the call to `stream_updates()`, and no
-          historic updates, set `start_idx`` to `uint64_max`.  By
-          default, start_idx is `0`, which means that all updates from
-          the first update onwards will be sent.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.StreamUpdatesRequest)
-  })
-_sym_db.RegisterMessage(StreamUpdatesRequest)
-
-StreamUpdatesResponse = _reflection.GeneratedProtocolMessageType('StreamUpdatesResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMUPDATESRESPONSE,
-  '__module__' : 'minknow_api.run_until_pb2'
-  ,
-  '__doc__': """Attributes:
-      idx:
-          The index of this update All updates have a unique,
-          incrementing index that is assigned by MinKNOW
-      time:
-          The timestamp of this update (UTC)
-      update:
-          The update data itself
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.run_until.StreamUpdatesResponse)
-  })
-_sym_db.RegisterMessage(StreamUpdatesResponse)
-
-_RUNUNTILSERVICE = DESCRIPTOR.services_by_name['RunUntilService']
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
-  _CRITERIAVALUES_CRITERIAENTRY._options = None
-  _CRITERIAVALUES_CRITERIAENTRY._serialized_options = b'8\001'
-  _WRITETARGETCRITERIAREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _WRITETARGETCRITERIAREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMTARGETCRITERIAREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMTARGETCRITERIAREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _WRITECUSTOMPROGRESSREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _WRITECUSTOMPROGRESSREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMPROGRESSREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMPROGRESSREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES_ESTIMATEDTIMESENTRY._options = None
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES_ESTIMATEDTIMESENTRY._serialized_options = b'8\001'
-  _WRITEUPDATESREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _WRITEUPDATESREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMUPDATESREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMUPDATESREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _RUNUNTILSERVICE.methods_by_name['write_custom_progress']._options = None
-  _RUNUNTILSERVICE.methods_by_name['write_custom_progress']._serialized_options = b'\230\265\030\001'
-  _RUNUNTILSERVICE.methods_by_name['stream_progress']._options = None
-  _RUNUNTILSERVICE.methods_by_name['stream_progress']._serialized_options = b'\230\265\030\001'
-  _CRITERIAVALUES._serialized_start=146
-  _CRITERIAVALUES._serialized_end=304
-  _CRITERIAVALUES_CRITERIAENTRY._serialized_start=235
-  _CRITERIAVALUES_CRITERIAENTRY._serialized_end=304
-  _GETSTANDARDCRITERIAREQUEST._serialized_start=306
-  _GETSTANDARDCRITERIAREQUEST._serialized_end=334
-  _GETSTANDARDCRITERIARESPONSE._serialized_start=336
-  _GETSTANDARDCRITERIARESPONSE._serialized_end=422
-  _WRITETARGETCRITERIAREQUEST._serialized_start=425
-  _WRITETARGETCRITERIAREQUEST._serialized_end=612
-  _WRITETARGETCRITERIARESPONSE._serialized_start=614
-  _WRITETARGETCRITERIARESPONSE._serialized_end=643
-  _STREAMTARGETCRITERIAREQUEST._serialized_start=645
-  _STREAMTARGETCRITERIAREQUEST._serialized_end=708
-  _STREAMTARGETCRITERIARESPONSE._serialized_start=711
-  _STREAMTARGETCRITERIARESPONSE._serialized_end=866
-  _WRITECUSTOMPROGRESSREQUEST._serialized_start=868
-  _WRITECUSTOMPROGRESSREQUEST._serialized_end=994
-  _WRITECUSTOMPROGRESSRESPONSE._serialized_start=996
-  _WRITECUSTOMPROGRESSRESPONSE._serialized_end=1025
-  _STREAMPROGRESSREQUEST._serialized_start=1027
-  _STREAMPROGRESSREQUEST._serialized_end=1084
-  _STREAMPROGRESSRESPONSE._serialized_start=1086
-  _STREAMPROGRESSRESPONSE._serialized_end=1174
-  _ESTIMATEDTIMEREMAININGUPDATE._serialized_start=1177
-  _ESTIMATEDTIMEREMAININGUPDATE._serialized_end=1969
-  _ESTIMATEDTIMEREMAININGUPDATE_NOTESTIMATED._serialized_start=1394
-  _ESTIMATEDTIMEREMAININGUPDATE_NOTESTIMATED._serialized_end=1408
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATED._serialized_start=1410
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATED._serialized_end=1513
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIME._serialized_start=1516
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIME._serialized_end=1715
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES._serialized_start=1718
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES._serialized_end=1969
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES_ESTIMATEDTIMESENTRY._serialized_start=1849
-  _ESTIMATEDTIMEREMAININGUPDATE_ESTIMATEDTIMES_ESTIMATEDTIMESENTRY._serialized_end=1969
-  _ACTIONUPDATE._serialized_start=1972
-  _ACTIONUPDATE._serialized_end=2108
-  _ACTIONUPDATE_ACTION._serialized_start=2048
-  _ACTIONUPDATE_ACTION._serialized_end=2108
-  _SCRIPTUPDATE._serialized_start=2111
-  _SCRIPTUPDATE._serialized_end=2296
-  _SCRIPTUPDATE_STARTED._serialized_start=2268
-  _SCRIPTUPDATE_STARTED._serialized_end=2277
-  _SCRIPTUPDATE_CRITERIAUPDATED._serialized_start=2279
-  _SCRIPTUPDATE_CRITERIAUPDATED._serialized_end=2296
-  _ERRORUPDATE._serialized_start=2299
-  _ERRORUPDATE._serialized_end=2535
-  _ERRORUPDATE_INVALIDCRITERIA._serialized_start=2464
-  _ERRORUPDATE_INVALIDCRITERIA._serialized_end=2495
-  _ERRORUPDATE_OTHERERROR._serialized_start=2497
-  _ERRORUPDATE_OTHERERROR._serialized_end=2526
-  _UPDATE._serialized_start=2538
-  _UPDATE._serialized_end=2927
-  _WRITEUPDATESREQUEST._serialized_start=2929
-  _WRITEUPDATESREQUEST._serialized_end=3031
-  _WRITEUPDATESRESPONSE._serialized_start=3033
-  _WRITEUPDATESRESPONSE._serialized_end=3055
-  _STREAMUPDATESREQUEST._serialized_start=3057
-  _STREAMUPDATESREQUEST._serialized_end=3132
-  _STREAMUPDATESRESPONSE._serialized_start=3134
-  _STREAMUPDATESRESPONSE._serialized_end=3259
-  _RUNUNTILSERVICE._serialized_start=3262
-  _RUNUNTILSERVICE._serialized_end=4153
-# @@protoc_insertion_point(module_scope)
+### THIS FILE IS AUTOGENERATED. DO NOT EDIT THIS FILE DIRECTLY ###
+import minknow_api
+from minknow_api.run_until_pb2_grpc import *
+import minknow_api.run_until_pb2 as run_until_pb2
+from minknow_api.run_until_pb2 import *
+from minknow_api._support import MessageWrapper, ArgumentError
+import time
+import logging
+import sys
+
+__all__ = [
+    "RunUntilService",
+    "CriteriaValues",
+    "GetStandardCriteriaRequest",
+    "GetStandardCriteriaResponse",
+    "WriteTargetCriteriaRequest",
+    "WriteTargetCriteriaResponse",
+    "StreamTargetCriteriaRequest",
+    "StreamTargetCriteriaResponse",
+    "WriteCustomProgressRequest",
+    "WriteCustomProgressResponse",
+    "StreamProgressRequest",
+    "StreamProgressResponse",
+    "EstimatedTimeRemainingUpdate",
+    "ActionUpdate",
+    "ScriptUpdate",
+    "ErrorUpdate",
+    "Update",
+    "WriteUpdatesRequest",
+    "WriteUpdatesResponse",
+    "StreamUpdatesRequest",
+    "StreamUpdatesResponse",
+]
+
+def run_with_retry(method, message, timeout, unwraps, full_name):
+    retry_count = 20
+    error = None
+    for i in range(retry_count):
+        try:
+            result = MessageWrapper(method(message, timeout=timeout), unwraps=unwraps)
+            return result
+        except grpc.RpcError as e:
+            # Retrying unidentified grpc errors to keep clients from crashing
+            retryable_error = (e.code() == grpc.StatusCode.UNKNOWN and "Stream removed" in e.details() or \
+                                (e.code() == grpc.StatusCode.INTERNAL and "RST_STREAM" in e.details()))
+            if retryable_error:
+                logging.info('Bypassed ({}: {}) error for grpc: {}. Attempt {}.'.format(e.code(), e.details(), full_name, i))
+            else:
+                raise
+            error = e
+        time.sleep(1)
+    raise error
+
+
+class RunUntilService(object):
+    """Overview
+    ========
+
+    This service allows a user to set certain criteria (Target Run-Until Critera), which indicate
+    the conditions under which the experiment should be stopped or paused.  For example, the user
+    can specify that the experiment should be stopped after a certain time has elapsed, or paused
+    when the number of avaiable pores drops below a certain level.  This functionality is referred
+    to as "Run-Until", since it allows the user to specify that an experiment should "run until"
+    some condition has been fulfilled.
+
+    The Target Run-Until Criteria are the conditions that are used to determine whether an
+    experiment should be stopped or paused.  There is a "standard" set of Run-Until Criteria, which
+    can always be used.  Additional Run-Until Criteria may also be supported by custom Run-Until
+    Scripts (see below).
+
+    This service also provides updates about the Run-Until status.  These include updates about
+    the experiment's progress towards the Run-Until Criteria, as well as updates about the estimated
+    time remaining, and Run-Until actions (i.e. starting/stopping the experiment).
+
+    Finally, this service provides an API for Run-Until Scripts.  A Run-Until Script is responsible
+    for actually implementing the Run-Until functionality.  The Run-Until Script reads the Target 
+    Run-Until Criteria that are set by the user.  It then monitors the experiment's progress, and
+    pauses or stops the experiment when the Run-Until Criteria have been fulfilled.  There is a
+    "standard" ONT-provided run-until script, which supports the "standard" Run-Until Criteria. 
+    Custom Run-Until Scripts can be implemented which extend the "standard" Run-Until Script to
+    provide support for additional criteria.
+
+    Usage -- Users
+    ==============
+
+    Overview
+    --------
+
+    The user sets the initial target Run-Until Criteria when the protocol is started, supplying them
+    in the parameters passed to `start_protocol()` or `begin_protocol()`.
+
+    The user may update these criteria as the experiment progresses by calling
+    `write_target_criteria()` with the new criteria.
+
+    The user can determine progress towards these criteria by receiving message from
+    `stream_progress()`, which supplies updates of the current values of the Run-Until
+    Criteria.
+
+    The user can also obtain updates from the Run-Until Script by calling
+    `stream_updates()`.  The Run-Until Script may send "estimated time remaining"
+    information, or messages relating to the Run-Until status.
+
+    If a criterion is specified in `write_target_criteria()` that is not recognised by the
+    Run-Until Script, then the Run-Until Script will ignore that criterion.  It will also
+    report that it has encountered an unrecognised criterion through `stream_updates()`.
+
+
+    Standard Run-Until Criteria
+    ---------------------------
+
+    The Standard Run-Until Criteria are described below.  These criteria are always available for
+    use.
+
+    `runtime` (uint64)
+         Acquisition runtime, in seconds
+         Criterion is met if the runtime is greater than or equal to the specified value.
+
+    `available_pores` (float)
+         Pores marked available, following a mux scan.
+         Criterion is met if the percentage of available pores is less than the specified value.
+         An update will be supplied after each mux scan that is performed.
+
+    `estimated_bases` (uint64)
+         Estimated bases generated during the experiment.
+         Criterion is met if the number of estimated bases is greater than or equal to the specified
+         value.
+
+    `passed_basecalled_bases` (uint64)
+         Basecalled bases which pass filtering (following basecalling)
+         Criterion will never be met if basecalling is not enabled.
+         Updates will not be supplied if basecalling is not enabled.
+         Criterion is met if the number of basecalled bases which pass filtering is greater than or
+         equal to the specified value.
+
+
+    Additional Run-Until Criteria
+    -----------------------------
+
+    Custom Run-Until Scripts may support additional criteria (beyond the Standard Run-Until Criteria
+    described above).  The list of these criteria, and their meaning, will be supplied in the
+    documentation for the custom run-until script.
+
+
+    Usage -- Run-Until Scripts
+    ==========================
+
+    Overview
+    --------
+
+    The Run-Until Script is started as a custom script.
+
+    The script obtains the Run-Until Criteria from MinKNOW using `stream_target_criteria()`.  Any
+    updates to the Run-Until Criteria are also transmitted through this call.  If any of the
+    criteria specified are not support by the script, the script reports an error via
+    `write_updates()`.
+
+    The script receives experiment progress updates.  Updates for the "standard" Run-Until Criteria
+    are transmitted by MinKNOW over `stream_progress()`.  The "standard" Run-Until Criteria values
+    that MinKNOW transmits over `stream_progress()` are supplied as a convenience for Run-Until
+    Scripts; the same data is also available through other separate MinKNOW APIs.
+
+    A custom Run-Until Script can also determine additional custom Run-Until Criteria values using
+    any suitable method (e.g. reading another MinKNOW API).  Updates for custom Run-Until Criteria
+    can be transmitted to the user using the  the `write_custom_progress()` call. (Values for
+    "standard" Run-Until Criteria may not be transmitted from the script using the
+    `write_custom_progress()` call; the `write_custom_progress()` call will fail with an error if an
+    attempt is made to transmit such values.  The "standard" Run-Until Criteria can be obtained
+    using `get_standard_criteria()`.)
+
+    Finally, the Run-Until Script can perform actions and send updates to the user using the
+    `write_updates()` interface.  Actions include pausing, resuming and stopping the
+    acquisition.  Updates include estimated time remaining.
+
+    Update History
+    ==============
+
+    MinKNOW stores an "merged" history of updates that are receieved on the `write_updates()`
+    interface.  The history is calculated as MinKNOW receives updates on the `write_updates()`
+    stream as follows:
+
+     - When the protocol starts, an empty message is added to the history
+     - When an update is received on the `write_updates()` interface, the values of the 
+       `estimated_time_remaining_update` and `current_progress_update` fields are updated, by
+       "merging" the corresponding fields of the last message in the history.  "Merging" here means
+       copying keys/values which appear in the "previous" message, but which don't have
+       corresponding keys in the newly received message.
+     - Once the values in the update have been updated, the "merged" message is then added to the
+       history:
+         - If the previous message in the history has no fields set, besides the
+           `estimated_time_remaining_update` and/or `current_progress_update` fields, then the
+           previous message in the history is overwritten with the "merged" message
+         - Otherwise, the "merged" message is appended to the history.
+
+     After updating the history, the final entry in the history is sent to any open 
+     `stream_updates()` streams.  The `idx` in the `StreamUpdatesResponse` message is set equal to
+     the index of the entry in the history.  This means that the `stream_updates()` stream will
+     likely contain repeated `idx` values -- this will happen when the previous message in the
+     history is overwritten by the "merged" message.  The `time` in the `StreamUpdatesResponse`
+     message is set equal to the time at which the entry in the history was last updated."""
+    def __init__(self, channel):
+        self._stub = RunUntilServiceStub(channel)
+        self._pb = run_until_pb2
+    def get_standard_criteria(self, _message=None, _timeout=None, **kwargs):
+        """Get the standard Run-Until Criteria
+
+        Updates for these criteria will be provided by MinKNOW
+
+        
+
+        Args:
+            _message (minknow_api.run_until_pb2.GetStandardCriteriaRequest, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+
+        Returns:
+            minknow_api.run_until_pb2.GetStandardCriteriaResponse
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.get_standard_criteria,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.run_until.RunUntilService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = GetStandardCriteriaRequest()
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to get_standard_criteria: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.get_standard_criteria,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.run_until.RunUntilService")
+    def write_target_criteria(self, _message=None, _timeout=None, **kwargs):
+        """Write target run-until criteria
+
+        Updates to these criteria are forwarded to `stream_target_criteria()`.  When an update is
+        made, all existing criteria are replaced with those specified in the
+        WriteTargetCriteriaRequest
+
+        
+
+        Args:
+            _message (minknow_api.run_until_pb2.WriteTargetCriteriaRequest, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+            acquisition_run_id (str): The acquisition to set the Run-Until Criteria for
+            pause_criteria (minknow_api.run_until_pb2.CriteriaValues, optional): 
+            stop_criteria (minknow_api.run_until_pb2.CriteriaValues, optional): 
+
+        Returns:
+            minknow_api.run_until_pb2.WriteTargetCriteriaResponse
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.write_target_criteria,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.run_until.RunUntilService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = WriteTargetCriteriaRequest()
+
+        if "acquisition_run_id" in kwargs:
+            unused_args.remove("acquisition_run_id")
+            _message.acquisition_run_id = kwargs['acquisition_run_id']
+        else:
+            raise ArgumentError("write_target_criteria requires a 'acquisition_run_id' argument")
+
+        if "pause_criteria" in kwargs:
+            unused_args.remove("pause_criteria")
+            _message.pause_criteria.CopyFrom(kwargs['pause_criteria'])
+
+        if "stop_criteria" in kwargs:
+            unused_args.remove("stop_criteria")
+            _message.stop_criteria.CopyFrom(kwargs['stop_criteria'])
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to write_target_criteria: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.write_target_criteria,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.run_until.RunUntilService")
+    def stream_target_criteria(self, _message=None, _timeout=None, **kwargs):
+        """Obtain the current target run-until criteria, and listen for changes in the target
+        run-until criteria
+
+        When an update is received, it specifies the new target criteria, which should replace all
+        existing criteria.
+
+        
+
+        Args:
+            _message (minknow_api.run_until_pb2.StreamTargetCriteriaRequest, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+                Note that this is the time until the call ends, not the time between returned
+                messages.
+            acquisition_run_id (str): The acquisition to obtain the Run-Until Criteria for
+
+        Returns:
+            iter of minknow_api.run_until_pb2.StreamTargetCriteriaResponse
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.stream_target_criteria,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.run_until.RunUntilService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = StreamTargetCriteriaRequest()
+
+        if "acquisition_run_id" in kwargs:
+            unused_args.remove("acquisition_run_id")
+            _message.acquisition_run_id = kwargs['acquisition_run_id']
+        else:
+            raise ArgumentError("stream_target_criteria requires a 'acquisition_run_id' argument")
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to stream_target_criteria: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.stream_target_criteria,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.run_until.RunUntilService")
+    def write_custom_progress(self, _message=None, _timeout=None, **kwargs):
+        """Send a Custom Run-Until Progress update
+
+        Updates written here are forwarded on to `stream_progress()`.  The Run-Until Script can use
+        this to supply updates on "custom" Run-Until Criteria
+
+        
+
+        Note this API is experimental - it may be changed, revised or removed in future minor versions.
+
+        Args:
+            _message (minknow_api.run_until_pb2.WriteCustomProgressRequest, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+            acquisition_run_id (str): The acquisition this Run-Until progress update relates to
+            criteria_values (minknow_api.run_until_pb2.CriteriaValues, optional): The current Run-Until criteria state
+
+                A Run-Until progress update need not contain updates for all criteria. 
+                It must not contain updates for "standard" criteria
+
+        Returns:
+            minknow_api.run_until_pb2.WriteCustomProgressResponse
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        print("Warning: Method RunUntilService.write_custom_progress is experimental and may be changed, revised or removed in future minor versions.", file=sys.stderr)
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.write_custom_progress,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.run_until.RunUntilService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = WriteCustomProgressRequest()
+
+        if "acquisition_run_id" in kwargs:
+            unused_args.remove("acquisition_run_id")
+            _message.acquisition_run_id = kwargs['acquisition_run_id']
+        else:
+            raise ArgumentError("write_custom_progress requires a 'acquisition_run_id' argument")
+
+        if "criteria_values" in kwargs:
+            unused_args.remove("criteria_values")
+            _message.criteria_values.CopyFrom(kwargs['criteria_values'])
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to write_custom_progress: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.write_custom_progress,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.run_until.RunUntilService")
+    def stream_progress(self, _message=None, _timeout=None, **kwargs):
+        """Obtain Run-Until Progress updates
+
+        The Run-Until Script can use this data to determine progress towards the Run-Until endpoints.
+        The user can use this data to visualise progress towards the Run-Until endpoints.
+
+        This data may come from MinKNOW itself (for standard run-until criteria), or may come from
+        a call to `write_custom_progress` (for custom run-until criteria)
+
+        Note that streaming of progress updates for standard run-until has not yet been implemented
+        in MinKNOW.
+
+        
+
+        Note this API is experimental - it may be changed, revised or removed in future minor versions.
+
+        Args:
+            _message (minknow_api.run_until_pb2.StreamProgressRequest, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+                Note that this is the time until the call ends, not the time between returned
+                messages.
+            acquisition_run_id (str): The acquisition to obtain the Run-Until progress updates for
+
+        Returns:
+            iter of minknow_api.run_until_pb2.StreamProgressResponse
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        print("Warning: Method RunUntilService.stream_progress is experimental and may be changed, revised or removed in future minor versions.", file=sys.stderr)
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.stream_progress,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.run_until.RunUntilService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = StreamProgressRequest()
+
+        if "acquisition_run_id" in kwargs:
+            unused_args.remove("acquisition_run_id")
+            _message.acquisition_run_id = kwargs['acquisition_run_id']
+        else:
+            raise ArgumentError("stream_progress requires a 'acquisition_run_id' argument")
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to stream_progress: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.stream_progress,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.run_until.RunUntilService")
+    def write_updates(self, _message=None, _timeout=None, **kwargs):
+        """Send an update about the current Run-Until state
+
+        The Run-Until Script can use this to provide information about the expected time remaining
+        (as well as other information) to users of the Run-Until functionality
+
+        Updates written here are forwarded on to `stream_updates()`
+
+        
+
+        Args:
+            _message (minknow_api.run_until_pb2.WriteUpdatesRequest, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+            acquisition_run_id (str): The acquisition this Run-Until update applies to
+            update (minknow_api.run_until_pb2.Update, optional): 
+
+        Returns:
+            minknow_api.run_until_pb2.WriteUpdatesResponse
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.write_updates,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.run_until.RunUntilService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = WriteUpdatesRequest()
+
+        if "acquisition_run_id" in kwargs:
+            unused_args.remove("acquisition_run_id")
+            _message.acquisition_run_id = kwargs['acquisition_run_id']
+        else:
+            raise ArgumentError("write_updates requires a 'acquisition_run_id' argument")
+
+        if "update" in kwargs:
+            unused_args.remove("update")
+            _message.update.CopyFrom(kwargs['update'])
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to write_updates: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.write_updates,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.run_until.RunUntilService")
+    def stream_updates(self, _message=None, _timeout=None, **kwargs):
+        """Obtain updates about the current Run-Until state
+
+        The user can use this to obtain information about the expected time remaining (as well as
+        other information) from the Run-Until Script.
+
+        Updates are sent following writes to `write_updates()`
+
+        
+
+        Args:
+            _message (minknow_api.run_until_pb2.StreamUpdatesRequest, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+                Note that this is the time until the call ends, not the time between returned
+                messages.
+            acquisition_run_id (str): The acquisition to stream Run-Until updates for
+            start_idx (int, optional): The index of the first update to send.
+
+                If an index is set that is greater than the current greatest update index, no past updates
+                will be sent, but any future updates will be sent.  This may mean that you receive updates
+                with an `idx` smaller than `start_idx`.
+
+                In order to receive only updates that are sent after the call to `stream_updates()`, and no
+                historic updates, set `start_idx` to `int64_max`.
+
+                Setting `start_idx` to a negative number will be treated as an offset from the end of the
+                updates history. A `start_idx` of `-1` will cause the last update to be sent, and any future
+                updates to be streamed.  The negative value is clamped such that a "large" negative number
+                will be equivalent to setting a `start_idx` of `0`.
+
+                By default, `start_idx` is `0`, which means that all updates from the first update onwards
+                will be sent.
+
+        Returns:
+            iter of minknow_api.run_until_pb2.StreamUpdatesResponse
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.stream_updates,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.run_until.RunUntilService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = StreamUpdatesRequest()
+
+        if "acquisition_run_id" in kwargs:
+            unused_args.remove("acquisition_run_id")
+            _message.acquisition_run_id = kwargs['acquisition_run_id']
+        else:
+            raise ArgumentError("stream_updates requires a 'acquisition_run_id' argument")
+
+        if "start_idx" in kwargs:
+            unused_args.remove("start_idx")
+            _message.start_idx = kwargs['start_idx']
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to stream_updates: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.stream_updates,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.run_until.RunUntilService")
```

### Comparing `minknow_api-5.4.0/minknow_api/run_until_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/run_until_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,32 +74,14 @@
     An update will be supplied after each mux scan that is performed.
 
     `estimated_bases` (uint64)
     Estimated bases generated during the experiment.
     Criterion is met if the number of estimated bases is greater than or equal to the specified
     value.
 
-    `reads` (uint64)
-    Reads generated during the experiment.
-    Criterion is met if the number of reads is greater than or equal to the specified value.
-
-    `basecalled_bases` (uint64)
-    Basecalled bases generated during the experiment
-    Criterion will never be met if basecalling is not enabled.
-    Updates will not be supplied if basecalling is not enabled.
-    Criterion is met if the number of basecalled bases is greater than or equal to the
-    specified value.
-
-    `passed_reads` (uint64)
-    Reads which pass filtering (following basecalling)
-    Criterion will never be met if basecalling is not enabled.
-    Updates will not be supplied if basecalling is not enabled.
-    Criterion is met if the number of reads which pass filtering is greater than or equal to
-    the specified value.
-
     `passed_basecalled_bases` (uint64)
     Basecalled bases which pass filtering (following basecalling)
     Criterion will never be met if basecalling is not enabled.
     Updates will not be supplied if basecalling is not enabled.
     Criterion is met if the number of basecalled bases which pass filtering is greater than or
     equal to the specified value.
 
@@ -138,14 +120,42 @@
     attempt is made to transmit such values.  The "standard" Run-Until Criteria can be obtained
     using `get_standard_criteria()`.)
 
     Finally, the Run-Until Script can perform actions and send updates to the user using the
     `write_updates()` interface.  Actions include pausing, resuming and stopping the
     acquisition.  Updates include estimated time remaining.
 
+    Update History
+    ==============
+
+    MinKNOW stores an "merged" history of updates that are receieved on the `write_updates()`
+    interface.  The history is calculated as MinKNOW receives updates on the `write_updates()`
+    stream as follows:
+
+    - When the protocol starts, an empty message is added to the history
+    - When an update is received on the `write_updates()` interface, the values of the 
+    `estimated_time_remaining_update` and `current_progress_update` fields are updated, by
+    "merging" the corresponding fields of the last message in the history.  "Merging" here means
+    copying keys/values which appear in the "previous" message, but which don't have
+    corresponding keys in the newly received message.
+    - Once the values in the update have been updated, the "merged" message is then added to the
+    history:
+    - If the previous message in the history has no fields set, besides the
+    `estimated_time_remaining_update` and/or `current_progress_update` fields, then the
+    previous message in the history is overwritten with the "merged" message
+    - Otherwise, the "merged" message is appended to the history.
+
+    After updating the history, the final entry in the history is sent to any open 
+    `stream_updates()` streams.  The `idx` in the `StreamUpdatesResponse` message is set equal to
+    the index of the entry in the history.  This means that the `stream_updates()` stream will
+    likely contain repeated `idx` values -- this will happen when the previous message in the
+    history is overwritten by the "merged" message.  The `time` in the `StreamUpdatesResponse`
+    message is set equal to the time at which the entry in the history was last updated.
+
+
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -256,32 +266,14 @@
     An update will be supplied after each mux scan that is performed.
 
     `estimated_bases` (uint64)
     Estimated bases generated during the experiment.
     Criterion is met if the number of estimated bases is greater than or equal to the specified
     value.
 
-    `reads` (uint64)
-    Reads generated during the experiment.
-    Criterion is met if the number of reads is greater than or equal to the specified value.
-
-    `basecalled_bases` (uint64)
-    Basecalled bases generated during the experiment
-    Criterion will never be met if basecalling is not enabled.
-    Updates will not be supplied if basecalling is not enabled.
-    Criterion is met if the number of basecalled bases is greater than or equal to the
-    specified value.
-
-    `passed_reads` (uint64)
-    Reads which pass filtering (following basecalling)
-    Criterion will never be met if basecalling is not enabled.
-    Updates will not be supplied if basecalling is not enabled.
-    Criterion is met if the number of reads which pass filtering is greater than or equal to
-    the specified value.
-
     `passed_basecalled_bases` (uint64)
     Basecalled bases which pass filtering (following basecalling)
     Criterion will never be met if basecalling is not enabled.
     Updates will not be supplied if basecalling is not enabled.
     Criterion is met if the number of basecalled bases which pass filtering is greater than or
     equal to the specified value.
 
@@ -320,14 +312,42 @@
     attempt is made to transmit such values.  The "standard" Run-Until Criteria can be obtained
     using `get_standard_criteria()`.)
 
     Finally, the Run-Until Script can perform actions and send updates to the user using the
     `write_updates()` interface.  Actions include pausing, resuming and stopping the
     acquisition.  Updates include estimated time remaining.
 
+    Update History
+    ==============
+
+    MinKNOW stores an "merged" history of updates that are receieved on the `write_updates()`
+    interface.  The history is calculated as MinKNOW receives updates on the `write_updates()`
+    stream as follows:
+
+    - When the protocol starts, an empty message is added to the history
+    - When an update is received on the `write_updates()` interface, the values of the 
+    `estimated_time_remaining_update` and `current_progress_update` fields are updated, by
+    "merging" the corresponding fields of the last message in the history.  "Merging" here means
+    copying keys/values which appear in the "previous" message, but which don't have
+    corresponding keys in the newly received message.
+    - Once the values in the update have been updated, the "merged" message is then added to the
+    history:
+    - If the previous message in the history has no fields set, besides the
+    `estimated_time_remaining_update` and/or `current_progress_update` fields, then the
+    previous message in the history is overwritten with the "merged" message
+    - Otherwise, the "merged" message is appended to the history.
+
+    After updating the history, the final entry in the history is sent to any open 
+    `stream_updates()` streams.  The `idx` in the `StreamUpdatesResponse` message is set equal to
+    the index of the entry in the history.  This means that the `stream_updates()` stream will
+    likely contain repeated `idx` values -- this will happen when the previous message in the
+    history is overwritten by the "merged" message.  The `time` in the `StreamUpdatesResponse`
+    message is set equal to the time at which the entry in the history was last updated.
+
+
     """
 
     def get_standard_criteria(self, request, context):
         """Get the standard Run-Until Criteria
 
         Updates for these criteria will be provided by MinKNOW
         """
@@ -522,32 +542,14 @@
     An update will be supplied after each mux scan that is performed.
 
     `estimated_bases` (uint64)
     Estimated bases generated during the experiment.
     Criterion is met if the number of estimated bases is greater than or equal to the specified
     value.
 
-    `reads` (uint64)
-    Reads generated during the experiment.
-    Criterion is met if the number of reads is greater than or equal to the specified value.
-
-    `basecalled_bases` (uint64)
-    Basecalled bases generated during the experiment
-    Criterion will never be met if basecalling is not enabled.
-    Updates will not be supplied if basecalling is not enabled.
-    Criterion is met if the number of basecalled bases is greater than or equal to the
-    specified value.
-
-    `passed_reads` (uint64)
-    Reads which pass filtering (following basecalling)
-    Criterion will never be met if basecalling is not enabled.
-    Updates will not be supplied if basecalling is not enabled.
-    Criterion is met if the number of reads which pass filtering is greater than or equal to
-    the specified value.
-
     `passed_basecalled_bases` (uint64)
     Basecalled bases which pass filtering (following basecalling)
     Criterion will never be met if basecalling is not enabled.
     Updates will not be supplied if basecalling is not enabled.
     Criterion is met if the number of basecalled bases which pass filtering is greater than or
     equal to the specified value.
 
@@ -586,14 +588,42 @@
     attempt is made to transmit such values.  The "standard" Run-Until Criteria can be obtained
     using `get_standard_criteria()`.)
 
     Finally, the Run-Until Script can perform actions and send updates to the user using the
     `write_updates()` interface.  Actions include pausing, resuming and stopping the
     acquisition.  Updates include estimated time remaining.
 
+    Update History
+    ==============
+
+    MinKNOW stores an "merged" history of updates that are receieved on the `write_updates()`
+    interface.  The history is calculated as MinKNOW receives updates on the `write_updates()`
+    stream as follows:
+
+    - When the protocol starts, an empty message is added to the history
+    - When an update is received on the `write_updates()` interface, the values of the 
+    `estimated_time_remaining_update` and `current_progress_update` fields are updated, by
+    "merging" the corresponding fields of the last message in the history.  "Merging" here means
+    copying keys/values which appear in the "previous" message, but which don't have
+    corresponding keys in the newly received message.
+    - Once the values in the update have been updated, the "merged" message is then added to the
+    history:
+    - If the previous message in the history has no fields set, besides the
+    `estimated_time_remaining_update` and/or `current_progress_update` fields, then the
+    previous message in the history is overwritten with the "merged" message
+    - Otherwise, the "merged" message is appended to the history.
+
+    After updating the history, the final entry in the history is sent to any open 
+    `stream_updates()` streams.  The `idx` in the `StreamUpdatesResponse` message is set equal to
+    the index of the entry in the history.  This means that the `stream_updates()` stream will
+    likely contain repeated `idx` values -- this will happen when the previous message in the
+    history is overwritten by the "merged" message.  The `time` in the `StreamUpdatesResponse`
+    message is set equal to the time at which the entry in the history was last updated.
+
+
     """
 
     @staticmethod
     def get_standard_criteria(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `minknow_api-5.4.0/minknow_api/statistics_pb2.py` & `minknow_api-5.5.2/minknow_api/device_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,897 +1,753 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: minknow_api/statistics.proto
+# source: minknow_api/device.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from minknow_api import acquisition_pb2 as minknow__api_dot_acquisition__pb2
 from minknow_api import rpc_options_pb2 as minknow__api_dot_rpc__options__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cminknow_api/statistics.proto\x12\x16minknow_api.statistics\x1a\x1dminknow_api/acquisition.proto\x1a\x1dminknow_api/rpc_options.proto\"9\n\rDataSelection\x12\r\n\x05start\x18\x01 \x01(\x03\x12\x0c\n\x04step\x18\x02 \x01(\x04\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x03\"x\n\x15StreamDutyTimeRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12=\n\x0e\x64\x61ta_selection\x18\x02 \x01(\x0b\x32%.minknow_api.statistics.DataSelection\"\x91\x03\n\x16StreamDutyTimeResponse\x12Q\n\rbucket_ranges\x18\x01 \x03(\x0b\x32:.minknow_api.statistics.StreamDutyTimeResponse.BucketRange\x12Y\n\x0e\x63hannel_states\x18\x02 \x03(\x0b\x32\x41.minknow_api.statistics.StreamDutyTimeResponse.ChannelStatesEntry\x1a)\n\x0b\x42ucketRange\x12\r\n\x05start\x18\x01 \x01(\r\x12\x0b\n\x03\x65nd\x18\x02 \x01(\r\x1a\'\n\x10\x43hannelStateData\x12\x13\n\x0bstate_times\x18\x01 \x03(\x04\x1au\n\x12\x43hannelStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12N\n\x05value\x18\x02 \x01(\x0b\x32?.minknow_api.statistics.StreamDutyTimeResponse.ChannelStateData:\x02\x38\x01\"X\n\x16ReadLengthHistogramKey\x12>\n\x0fread_end_reason\x18\x01 \x01(\x0e\x32%.minknow_api.statistics.ReadEndReason\"3\n\x18ReadLengthHistogramSplit\x12\x17\n\x0fread_end_reason\x18\x01 \x01(\x08\"\xc9\x03\n StreamReadLengthHistogramRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12\x19\n\x11poll_time_seconds\x18\x02 \x01(\r\x12@\n\x10read_length_type\x18\x03 \x01(\x0e\x32&.minknow_api.statistics.ReadLengthType\x12=\n\x0e\x64\x61ta_selection\x18\x04 \x01(\x0b\x32%.minknow_api.statistics.DataSelection\x12\x42\n\x11\x62ucket_value_type\x18\x05 \x01(\x0e\x32\'.minknow_api.statistics.BucketValueType\x12\x1f\n\x17\x64iscard_outlier_percent\x18\x06 \x01(\x02\x12\x41\n\tfiltering\x18\x07 \x03(\x0b\x32..minknow_api.statistics.ReadLengthHistogramKey\x12?\n\x05split\x18\x08 \x01(\x0b\x32\x30.minknow_api.statistics.ReadLengthHistogramSplit\"\xb9\x04\n!StreamReadLengthHistogramResponse\x12@\n\x10read_length_type\x18\x01 \x01(\x0e\x32&.minknow_api.statistics.ReadLengthType\x12\\\n\rbucket_ranges\x18\x02 \x03(\x0b\x32\x45.minknow_api.statistics.StreamReadLengthHistogramResponse.BucketRange\x12\x17\n\x0fsource_data_end\x18\x05 \x01(\x04\x12\x42\n\x11\x62ucket_value_type\x18\x03 \x01(\x0e\x32\'.minknow_api.statistics.BucketValueType\x12i\n\x0ehistogram_data\x18\x04 \x03(\x0b\x32Q.minknow_api.statistics.StreamReadLengthHistogramResponse.ReadLengthHistogramData\x1a)\n\x0b\x42ucketRange\x12\r\n\x05start\x18\x01 \x01(\x04\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x04\x1a\x80\x01\n\x17ReadLengthHistogramData\x12\x41\n\tfiltering\x18\x03 \x03(\x0b\x32..minknow_api.statistics.ReadLengthHistogramKey\x12\x15\n\rbucket_values\x18\x01 \x03(\x04\x12\x0b\n\x03n50\x18\x02 \x01(\x02\"=\n\x19GetReadLengthTypesRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"]\n\x1aGetReadLengthTypesResponse\x12?\n\x0f\x61vailable_types\x18\x01 \x03(\x0e\x32&.minknow_api.statistics.ReadLengthType\"\x9c\x02\n\x14\x41\x63quisitionOutputKey\x12\x14\n\x0c\x62\x61rcode_name\x18\x01 \x01(\t\x12\x1b\n\x13\x61lignment_reference\x18\x02 \x01(\t\x12!\n\x19\x61lignment_bed_file_region\x18\x03 \x01(\t\x12&\n\x1e\x61lignment_bed_file_region_name\x18\x08 \x01(\t\x12\x17\n\x0flamp_barcode_id\x18\x04 \x01(\t\x12\x16\n\x0elamp_target_id\x18\x05 \x01(\t\x12\x15\n\rbarcode_alias\x18\x06 \x01(\t\x12>\n\x0fread_end_reason\x18\x07 \x01(\x0e\x32%.minknow_api.statistics.ReadEndReason\"\xb8\x01\n\x16\x41\x63quisitionOutputSplit\x12\x14\n\x0c\x62\x61rcode_name\x18\x01 \x01(\x08\x12\x1b\n\x13\x61lignment_reference\x18\x02 \x01(\x08\x12!\n\x19\x61lignment_bed_file_region\x18\x03 \x01(\x08\x12\x17\n\x0flamp_barcode_id\x18\x04 \x01(\x08\x12\x16\n\x0elamp_target_id\x18\x05 \x01(\x08\x12\x17\n\x0fread_end_reason\x18\x06 \x01(\x08\"\x81\x02\n\x1eStreamAcquisitionOutputRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12=\n\x0e\x64\x61ta_selection\x18\x02 \x01(\x0b\x32%.minknow_api.statistics.DataSelection\x12?\n\tfiltering\x18\x03 \x03(\x0b\x32,.minknow_api.statistics.AcquisitionOutputKey\x12=\n\x05split\x18\x04 \x01(\x0b\x32..minknow_api.statistics.AcquisitionOutputSplit\"u\n\x19\x41\x63quisitionOutputSnapshot\x12\x0f\n\x07seconds\x18\x01 \x01(\r\x12G\n\ryield_summary\x18\x02 \x01(\x0b\x32\x30.minknow_api.acquisition.AcquisitionYieldSummary\"\x9c\x02\n\x1fStreamAcquisitionOutputResponse\x12\\\n\tsnapshots\x18\x01 \x03(\x0b\x32I.minknow_api.statistics.StreamAcquisitionOutputResponse.FilteredSnapshots\x1a\x9a\x01\n\x11\x46ilteredSnapshots\x12?\n\tfiltering\x18\x01 \x03(\x0b\x32,.minknow_api.statistics.AcquisitionOutputKey\x12\x44\n\tsnapshots\x18\x02 \x03(\x0b\x32\x31.minknow_api.statistics.AcquisitionOutputSnapshot\"|\n\x19StreamWriterOutputRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12=\n\x0e\x64\x61ta_selection\x18\x02 \x01(\x0b\x32%.minknow_api.statistics.DataSelection\"q\n\x14WriterOutputSnapshot\x12\x0f\n\x07seconds\x18\x01 \x01(\r\x12H\n\rwriter_output\x18\x02 \x01(\x0b\x32\x31.minknow_api.acquisition.AcquisitionWriterSummary\"]\n\x1aStreamWriterOutputResponse\x12?\n\tsnapshots\x18\x01 \x03(\x0b\x32,.minknow_api.statistics.WriterOutputSnapshot\"Q\n-StreamEncounteredAcquisitionOutputKeysRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"\x7f\n.StreamEncounteredAcquisitionOutputKeysResponse\x12M\n\x17\x61\x63quisition_output_keys\x18\x01 \x03(\x0b\x32,.minknow_api.statistics.AcquisitionOutputKey\"{\n\x18StreamTemperatureRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12=\n\x0e\x64\x61ta_selection\x18\x02 \x01(\x0b\x32%.minknow_api.statistics.DataSelection\"\xe1\x03\n\x11TemperaturePacket\x12M\n\x06minion\x18\x01 \x01(\x0b\x32;.minknow_api.statistics.TemperaturePacket.MinIONTemperatureH\x00\x12U\n\npromethion\x18\x02 \x01(\x0b\x32?.minknow_api.statistics.TemperaturePacket.PromethIONTemperatureH\x00\x12K\n\x12target_temperature\x18\x03 \x01(\x0b\x32/.minknow_api.statistics.TemperaturePacket.Range\x1a)\n\x05Range\x12\x0f\n\x07minimum\x18\x01 \x01(\x02\x12\x0f\n\x07maximum\x18\x02 \x01(\x02\x1aK\n\x11MinIONTemperature\x12\x18\n\x10\x61sic_temperature\x18\x01 \x01(\x01\x12\x1c\n\x14heatsink_temperature\x18\x02 \x01(\x01\x1aR\n\x15PromethIONTemperature\x12\x1c\n\x14\x66lowcell_temperature\x18\x01 \x01(\x01\x12\x1b\n\x13\x63hamber_temperature\x18\x02 \x01(\x01\x42\r\n\x0btemperature\"\\\n\x19StreamTemperatureResponse\x12?\n\x0ctemperatures\x18\x01 \x03(\x0b\x32).minknow_api.statistics.TemperaturePacket\"Z\n\x11\x42iasVoltagePacket\x12\x19\n\x11\x61\x63quisition_index\x18\x01 \x01(\x04\x12\x14\n\x0c\x62ias_voltage\x18\x02 \x01(\x01\x12\x14\n\x0ctime_seconds\x18\x03 \x01(\x04\"=\n\x19StreamBiasVoltagesRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"^\n\x1aStreamBiasVoltagesResponse\x12@\n\rbias_voltages\x18\x01 \x03(\x0b\x32).minknow_api.statistics.BiasVoltagePacket\"\xee\x01\n\x14StreamBoxplotRequest\x12 \n\x12\x61\x63quisition_run_id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\x12K\n\tdata_type\x18\x02 \x01(\x0e\x32\x38.minknow_api.statistics.StreamBoxplotRequest.BoxplotType\x12\x15\n\rdataset_width\x18\x03 \x01(\r\x12\x11\n\tpoll_time\x18\x04 \x01(\r\"=\n\x0b\x42oxplotType\x12\n\n\x06QSCORE\x10\x00\x12\x14\n\x10\x42\x41SES_PER_SECOND\x10\x01\x12\x0c\n\x08\x41\x43\x43URACY\x10\x02\"\x9a\x02\n\x0f\x42oxplotResponse\x12H\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\x36.minknow_api.statistics.BoxplotResponse.BoxplotDataset\x1a\xbc\x01\n\x0e\x42oxplotDataset\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03q25\x18\x02 \x01(\x02\x12\x0b\n\x03q50\x18\x03 \x01(\x02\x12\x0b\n\x03q75\x18\x04 \x01(\x02\x12\x0b\n\x03max\x18\x05 \x01(\x02\x12\r\n\x05\x63ount\x18\x06 \x01(\x04\x12%\n\x1dlower_full_width_half_maximum\x18\x07 \x01(\x02\x12\x0c\n\x04mode\x18\x08 \x01(\x02\x12%\n\x1dupper_full_width_half_maximum\x18\t \x01(\x02*L\n\x0eReadLengthType\x12\x11\n\rMinknowEvents\x10\x00\x12\x12\n\x0e\x45stimatedBases\x10\x01\x12\x13\n\x0f\x42\x61secalledBases\x10\x02*2\n\x0f\x42ucketValueType\x12\x0e\n\nReadCounts\x10\x00\x12\x0f\n\x0bReadLengths\x10\x01*\xa0\x01\n\rReadEndReason\x12\x07\n\x03\x41ll\x10\x00\x12\x0b\n\x07Unknown\x10\x01\x12\x0b\n\x07Partial\x10\x02\x12\r\n\tMuxChange\x10\x03\x12\x14\n\x10UnblockMuxChange\x10\x04\x12\x12\n\x0eSignalPositive\x10\x05\x12\x12\n\x0eSignalNegative\x10\x06\x12\x1f\n\x1b\x44\x61taServiceUnblockMuxChange\x10\x07\x32\x96\n\n\x11StatisticsService\x12x\n\x10stream_duty_time\x12-.minknow_api.statistics.StreamDutyTimeRequest\x1a..minknow_api.statistics.StreamDutyTimeResponse\"\x03\x90\x02\x01\x30\x01\x12\x93\x01\n\x19stream_acquisition_output\x12\x36.minknow_api.statistics.StreamAcquisitionOutputRequest\x1a\x37.minknow_api.statistics.StreamAcquisitionOutputResponse\"\x03\x90\x02\x01\x30\x01\x12\x84\x01\n\x14stream_writer_output\x12\x31.minknow_api.statistics.StreamWriterOutputRequest\x1a\x32.minknow_api.statistics.StreamWriterOutputResponse\"\x03\x90\x02\x01\x30\x01\x12\xc2\x01\n*stream_encountered_acquisition_output_keys\x12\x45.minknow_api.statistics.StreamEncounteredAcquisitionOutputKeysRequest\x1a\x46.minknow_api.statistics.StreamEncounteredAcquisitionOutputKeysResponse\"\x03\x90\x02\x01\x30\x01\x12\x80\x01\n\x12stream_temperature\x12\x30.minknow_api.statistics.StreamTemperatureRequest\x1a\x31.minknow_api.statistics.StreamTemperatureResponse\"\x03\x90\x02\x01\x30\x01\x12\x84\x01\n\x14stream_bias_voltages\x12\x31.minknow_api.statistics.StreamBiasVoltagesRequest\x1a\x32.minknow_api.statistics.StreamBiasVoltagesResponse\"\x03\x90\x02\x01\x30\x01\x12\x9a\x01\n\x1cstream_read_length_histogram\x12\x38.minknow_api.statistics.StreamReadLengthHistogramRequest\x1a\x39.minknow_api.statistics.StreamReadLengthHistogramResponse\"\x03\x90\x02\x01\x30\x01\x12\x83\x01\n\x15get_read_length_types\x12\x31.minknow_api.statistics.GetReadLengthTypesRequest\x1a\x32.minknow_api.statistics.GetReadLengthTypesResponse\"\x03\x90\x02\x01\x12x\n\x18stream_basecall_boxplots\x12,.minknow_api.statistics.StreamBoxplotRequest\x1a\'.minknow_api.statistics.BoxplotResponse\"\x03\x90\x02\x01\x30\x01\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18minknow_api/device.proto\x12\x12minknow_api.device\x1a\x1dminknow_api/rpc_options.proto\x1a\x1egoogle/protobuf/wrappers.proto\":\n\x14\x43hannelConfiguration\x12\x0c\n\x04well\x18\x01 \x01(\r\x12\x14\n\x0ctest_current\x18\x02 \x01(\x08\"S\n\x1cReturnedChannelConfiguration\x12\x0c\n\x04well\x18\x01 \x01(\r\x12\x14\n\x0ctest_current\x18\x02 \x01(\x08\x12\x0f\n\x07unblock\x18\x04 \x01(\x08\"\x16\n\x14GetDeviceInfoRequest\"\xff\x03\n\x15GetDeviceInfoResponse\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12I\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x34.minknow_api.device.GetDeviceInfoResponse.DeviceType\x12\x14\n\x0cis_simulated\x18\x03 \x01(\x08\x12\x19\n\x11max_channel_count\x18\x04 \x01(\r\x12\x1d\n\x15max_wells_per_channel\x18\x05 \x01(\r\x12\x1b\n\x13\x63\x61n_set_temperature\x18\x06 \x01(\x08\x12\x14\n\x0c\x64igitisation\x18\x07 \x01(\r\x12T\n\x10\x66irmware_version\x18\n \x03(\x0b\x32:.minknow_api.device.GetDeviceInfoResponse.ComponentVersion\x1aM\n\x10\x43omponentVersion\x12\x11\n\tcomponent\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x15\n\rserial_number\x18\x03 \x01(\t\"`\n\nDeviceType\x12\n\n\x06MINION\x10\x00\x12\x0b\n\x07GRIDION\x10\x02\x12\x0e\n\nPROMETHION\x10\x03\x12\x0f\n\x0bMINION_MK1C\x10\x04\x12\x0b\n\x07TRAXION\x10\x05\x12\x0b\n\x07P2_SOLO\x10\x06\"\x17\n\x15GetDeviceStateRequest\"\xe8\x01\n\x16GetDeviceStateResponse\x12L\n\x0c\x64\x65vice_state\x18\x01 \x01(\x0e\x32\x36.minknow_api.device.GetDeviceStateResponse.DeviceState\x12\x46\n\x13\x66low_cell_connector\x18\x02 \x01(\x0e\x32).minknow_api.device.FlowCellConnectorType\"8\n\x0b\x44\x65viceState\x12\x17\n\x13\x44\x45VICE_DISCONNECTED\x10\x00\x12\x10\n\x0c\x44\x45VICE_READY\x10\x01\"\x1a\n\x18StreamDeviceStateRequest\"\x18\n\x16GetFlowCellInfoRequest\"\xb5\x03\n\x17GetFlowCellInfoResponse\x12\x15\n\rhas_flow_cell\x18\x01 \x01(\x08\x12\x15\n\rchannel_count\x18\x02 \x01(\r\x12\x19\n\x11wells_per_channel\x18\x03 \x01(\r\x12\x14\n\x0c\x66low_cell_id\x18\x04 \x01(\t\x12\x13\n\x0b\x61sic_id_str\x18\r \x01(\t\x12\x14\n\x0cproduct_code\x18\x06 \x01(\t\x12#\n\x1buser_specified_flow_cell_id\x18\x07 \x01(\t\x12#\n\x1buser_specified_product_code\x18\x08 \x01(\t\x12\x13\n\x0bhas_adapter\x18\t \x01(\x08\x12\x12\n\nadapter_id\x18\n \x01(\t\x12\x1c\n\x12temperature_offset\x18\x0b \x01(\x02H\x00\x12\x14\n\x0c\x61sic_version\x18\x0c \x01(\t\x12J\n\x17insertion_script_status\x18\x0e \x01(\x0e\x32).minknow_api.device.InsertionScriptStatusB\x1d\n\x1btemperature_offset_nullable\"\x1b\n\x19StreamFlowCellInfoRequest\"5\n!SetUserSpecifiedFlowCellIdRequest\x12\x10\n\x02id\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"$\n\"SetUserSpecifiedFlowCellIdResponse\"8\n\"SetUserSpecifiedProductCodeRequest\x12\x12\n\x04\x63ode\x18\x01 \x01(\tB\x04\x88\xb5\x18\x01\"%\n#SetUserSpecifiedProductCodeResponse\"\x1a\n\x18GetChannelsLayoutRequest\"W\n\x19GetChannelsLayoutResponse\x12:\n\x0f\x63hannel_records\x18\x01 \x03(\x0b\x32!.minknow_api.device.ChannelRecord\"\xa4\x01\n\rChannelRecord\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12@\n\x0bmux_records\x18\x03 \x03(\x0b\x32+.minknow_api.device.ChannelRecord.MuxRecord\x1a\x37\n\tMuxRecord\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0e\n\x06phys_x\x18\x02 \x01(\r\x12\x0e\n\x06phys_y\x18\x03 \x01(\r\"\x1c\n\x1aResetDeviceSettingsRequest\"\x1d\n\x1bResetDeviceSettingsResponse\"\x80\x01\n\x15SetCalibrationRequest\x12\x1b\n\rfirst_channel\x18\x01 \x01(\rB\x04\x88\xb5\x18\x01\x12\x1a\n\x0clast_channel\x18\x02 \x01(\rB\x04\x88\xb5\x18\x01\x12\x15\n\x07offsets\x18\x03 \x03(\x02\x42\x04\x88\xb5\x18\x01\x12\x17\n\tpa_ranges\x18\x04 \x03(\x02\x42\x04\x88\xb5\x18\x01\"\x18\n\x16SetCalibrationResponse\"\x19\n\x17\x43learCalibrationRequest\"\x1a\n\x18\x43learCalibrationResponse\"P\n\x15GetCalibrationRequest\x12\x1b\n\rfirst_channel\x18\x01 \x01(\rB\x04\x88\xb5\x18\x01\x12\x1a\n\x0clast_channel\x18\x02 \x01(\rB\x04\x88\xb5\x18\x01\"k\n\x16GetCalibrationResponse\x12\x14\n\x0c\x64igitisation\x18\x01 \x01(\r\x12\x0f\n\x07offsets\x18\x02 \x03(\x02\x12\x11\n\tpa_ranges\x18\x03 \x03(\x02\x12\x17\n\x0fhas_calibration\x18\x04 \x01(\x08\"\x93\x03\n\x15SetTemperatureRequest\x12\x13\n\x0btemperature\x18\x01 \x01(\x02\x12\x62\n\x14wait_for_temperature\x18\x02 \x01(\x0b\x32\x44.minknow_api.device.SetTemperatureRequest.WaitForTemperatureSettings\x12j\n\x1csecondary_temperature_limits\x18\x03 \x01(\x0b\x32\x44.minknow_api.device.SetTemperatureRequest.SecondaryTemperatureLimits\x1a]\n\x1aWaitForTemperatureSettings\x12\x0f\n\x07timeout\x18\x01 \x01(\r\x12\x1b\n\x13min_stable_duration\x18\x03 \x01(\r\x12\x11\n\ttolerance\x18\x02 \x01(\x02\x1a\x36\n\x1aSecondaryTemperatureLimits\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03max\x18\x02 \x01(\x02\"\xb4\x02\n\x16SetTemperatureResponse\x12)\n!timed_out_waiting_for_temperature\x18\x01 \x01(\x08\x12O\n\x06result\x18\x02 \x01(\x0e\x32?.minknow_api.device.SetTemperatureResponse.SetTemperatureResult\"\x9d\x01\n\x14SetTemperatureResult\x12\x1a\n\x16TARGET_TEMPERATURE_SET\x10\x00\x12\x17\n\x13REACHED_TEMPERATURE\x10\x01\x12%\n!TIMED_OUT_WAITING_FOR_TEMPERATURE\x10\x02\x12)\n%SECONDARY_TEMPERATURE_LIMITS_EXCEEDED\x10\x03\"\x17\n\x15GetTemperatureRequest\"\x9f\x04\n\x16GetTemperatureResponse\x12N\n\x06minion\x18\x01 \x01(\x0b\x32<.minknow_api.device.GetTemperatureResponse.MinIONTemperatureH\x00\x12V\n\npromethion\x18\x02 \x01(\x0b\x32@.minknow_api.device.GetTemperatureResponse.PromethIONTemperatureH\x00\x12\x37\n\x12target_temperature\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x1a\x85\x01\n\x11MinIONTemperature\x12\x35\n\x10\x61sic_temperature\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x39\n\x14heatsink_temperature\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x1a\x8c\x01\n\x15PromethIONTemperature\x12\x39\n\x14\x66lowcell_temperature\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x38\n\x13\x63hamber_temperature\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValueB\r\n\x0btemperature\"2\n\x18StreamTemperatureRequest\x12\x16\n\x0eperiod_seconds\x18\x01 \x01(\r\"q\n\x0eUnblockRequest\x12\x10\n\x08\x63hannels\x18\x01 \x03(\r\x12\x1d\n\x13\x64uration_in_seconds\x18\x02 \x01(\rH\x00\x12\"\n\x18\x64uration_in_milliseconds\x18\x03 \x01(\rH\x00\x42\n\n\x08\x64uration\"\x11\n\x0fUnblockResponse\"\x17\n\x15\x43\x61ncelUnblocksRequest\"4\n\x16\x43\x61ncelUnblocksResponse\x12\x1a\n\x12\x63\x61ncelled_unblocks\x18\x01 \x01(\r\"2\n\x1eGetChannelConfigurationRequest\x12\x10\n\x08\x63hannels\x18\x01 \x03(\r\"s\n\x1fGetChannelConfigurationResponse\x12P\n\x16\x63hannel_configurations\x18\x01 \x03(\x0b\x32\x30.minknow_api.device.ReturnedChannelConfiguration\"\xf7\x01\n\x1eSetChannelConfigurationRequest\x12m\n\x16\x63hannel_configurations\x18\x01 \x03(\x0b\x32M.minknow_api.device.SetChannelConfigurationRequest.ChannelConfigurationsEntry\x1a\x66\n\x1a\x43hannelConfigurationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\x37\n\x05value\x18\x02 \x01(\x0b\x32(.minknow_api.device.ChannelConfiguration:\x02\x38\x01\"!\n\x1fSetChannelConfigurationResponse\"r\n!SetChannelConfigurationAllRequest\x12M\n\x15\x63hannel_configuration\x18\x01 \x01(\x0b\x32(.minknow_api.device.ChannelConfigurationB\x04\x90\xb5\x18\x01\"$\n\"SetChannelConfigurationAllResponse\"\xc6\x06\n\x10SaturationConfig\x12\x43\n\nthresholds\x18\x01 \x01(\x0b\x32/.minknow_api.device.SaturationConfig.Thresholds\x12T\n\x13software_saturation\x18\x02 \x01(\x0b\x32\x37.minknow_api.device.SaturationConfig.SoftwareSaturation\x12_\n\x19user_threshold_saturation\x18\x03 \x01(\x0b\x32<.minknow_api.device.SaturationConfig.UserThresholdSaturation\x1a\xfa\x01\n\nThresholds\x12\x37\n\x11general_threshold\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x37\n\x11unblock_threshold\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12<\n\x16user_general_threshold\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12<\n\x16user_unblock_threshold\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x1a\x93\x01\n\x12SoftwareSaturation\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x35\n\x10software_min_adc\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x35\n\x10software_max_adc\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x1a\xa2\x01\n\x17UserThresholdSaturation\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12:\n\x15user_threshold_min_pa\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12:\n\x15user_threshold_max_pa\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"Z\n\x1aSetSaturationConfigRequest\x12<\n\x08settings\x18\x01 \x01(\x0b\x32$.minknow_api.device.SaturationConfigB\x04\x90\xb5\x18\x01\"\x1d\n\x1bSetSaturationConfigResponse\"\x1c\n\x1aGetSaturationConfigRequest\"[\n\x1bGetSaturationConfigResponse\x12<\n\x08settings\x18\x01 \x01(\x0b\x32$.minknow_api.device.SaturationConfigB\x04\x90\xb5\x18\x01\"\x16\n\x14GetSampleRateRequest\",\n\x15GetSampleRateResponse\x12\x13\n\x0bsample_rate\x18\x01 \x01(\r\"1\n\x14SetSampleRateRequest\x12\x19\n\x0bsample_rate\x18\x01 \x01(\rB\x04\x88\xb5\x18\x01\"1\n\x15SetSampleRateResponse\x12\x18\n\x10real_sample_rate\x18\x01 \x01(\r\"\x17\n\x15GetBiasVoltageRequest\".\n\x16GetBiasVoltageResponse\x12\x14\n\x0c\x62ias_voltage\x18\x01 \x01(\x01\"3\n\x15SetBiasVoltageRequest\x12\x1a\n\x0c\x62ias_voltage\x18\x01 \x01(\x01\x42\x04\x88\xb5\x18\x01\"\x18\n\x16SetBiasVoltageResponse\"\x12\n\x10\x44umpStateRequest\"\x13\n\x11\x44umpStateResponse*i\n\x15\x46lowCellConnectorType\x12\x11\n\rFCCON_NOT_SET\x10\x00\x12\x14\n\x10\x46\x43\x43ON_PROMETHION\x10\x01\x12\x14\n\x10\x46\x43\x43ON_MINION_MK1\x10\x02\x12\x11\n\rFCCON_FLONGLE\x10\x03*?\n\x15InsertionScriptStatus\x12\x0b\n\x07NOT_RUN\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\r\n\tSUCCEEDED\x10\x02*]\n\x0cSelectedWell\x12\r\n\tWELL_NONE\x10\x00\x12\n\n\x06WELL_1\x10\x01\x12\n\n\x06WELL_2\x10\x02\x12\n\n\x06WELL_3\x10\x03\x12\n\n\x06WELL_4\x10\x04\x12\x0e\n\nWELL_OTHER\x10\x05\x32\xa8\x19\n\rDeviceService\x12k\n\x0fget_device_info\x12(.minknow_api.device.GetDeviceInfoRequest\x1a).minknow_api.device.GetDeviceInfoResponse\"\x03\x90\x02\x01\x12n\n\x10get_device_state\x12).minknow_api.device.GetDeviceStateRequest\x1a*.minknow_api.device.GetDeviceStateResponse\"\x03\x90\x02\x01\x12v\n\x13stream_device_state\x12,.minknow_api.device.StreamDeviceStateRequest\x1a*.minknow_api.device.GetDeviceStateResponse\"\x03\x90\x02\x01\x30\x01\x12r\n\x12get_flow_cell_info\x12*.minknow_api.device.GetFlowCellInfoRequest\x1a+.minknow_api.device.GetFlowCellInfoResponse\"\x03\x90\x02\x01\x12z\n\x15stream_flow_cell_info\x12-.minknow_api.device.StreamFlowCellInfoRequest\x1a+.minknow_api.device.GetFlowCellInfoResponse\"\x03\x90\x02\x01\x30\x01\x12\x95\x01\n\x1fset_user_specified_flow_cell_id\x12\x35.minknow_api.device.SetUserSpecifiedFlowCellIdRequest\x1a\x36.minknow_api.device.SetUserSpecifiedFlowCellIdResponse\"\x03\x90\x02\x02\x12\x97\x01\n\x1fset_user_specified_product_code\x12\x36.minknow_api.device.SetUserSpecifiedProductCodeRequest\x1a\x37.minknow_api.device.SetUserSpecifiedProductCodeResponse\"\x03\x90\x02\x02\x12w\n\x13get_channels_layout\x12,.minknow_api.device.GetChannelsLayoutRequest\x1a-.minknow_api.device.GetChannelsLayoutResponse\"\x03\x90\x02\x01\x12}\n\x15reset_device_settings\x12..minknow_api.device.ResetDeviceSettingsRequest\x1a/.minknow_api.device.ResetDeviceSettingsResponse\"\x03\x90\x02\x02\x12m\n\x0fset_calibration\x12).minknow_api.device.SetCalibrationRequest\x1a*.minknow_api.device.SetCalibrationResponse\"\x03\x90\x02\x02\x12s\n\x11\x63lear_calibration\x12+.minknow_api.device.ClearCalibrationRequest\x1a,.minknow_api.device.ClearCalibrationResponse\"\x03\x90\x02\x02\x12m\n\x0fget_calibration\x12).minknow_api.device.GetCalibrationRequest\x1a*.minknow_api.device.GetCalibrationResponse\"\x03\x90\x02\x01\x12m\n\x0fset_temperature\x12).minknow_api.device.SetTemperatureRequest\x1a*.minknow_api.device.SetTemperatureResponse\"\x03\x90\x02\x02\x12m\n\x0fget_temperature\x12).minknow_api.device.GetTemperatureRequest\x1a*.minknow_api.device.GetTemperatureResponse\"\x03\x90\x02\x01\x12u\n\x12stream_temperature\x12,.minknow_api.device.StreamTemperatureRequest\x1a*.minknow_api.device.GetTemperatureResponse\"\x03\x90\x02\x01\x30\x01\x12T\n\x07unblock\x12\".minknow_api.device.UnblockRequest\x1a#.minknow_api.device.UnblockResponse\"\x00\x12j\n\x0f\x63\x61ncel_unblocks\x12).minknow_api.device.CancelUnblocksRequest\x1a*.minknow_api.device.CancelUnblocksResponse\"\x00\x12\x89\x01\n\x19get_channel_configuration\x12\x32.minknow_api.device.GetChannelConfigurationRequest\x1a\x33.minknow_api.device.GetChannelConfigurationResponse\"\x03\x90\x02\x01\x12\x89\x01\n\x19set_channel_configuration\x12\x32.minknow_api.device.SetChannelConfigurationRequest\x1a\x33.minknow_api.device.SetChannelConfigurationResponse\"\x03\x90\x02\x02\x12\x93\x01\n\x1dset_channel_configuration_all\x12\x35.minknow_api.device.SetChannelConfigurationAllRequest\x1a\x36.minknow_api.device.SetChannelConfigurationAllResponse\"\x03\x90\x02\x02\x12z\n\x15set_saturation_config\x12..minknow_api.device.SetSaturationConfigRequest\x1a/.minknow_api.device.SetSaturationConfigResponse\"\x00\x12}\n\x15get_saturation_config\x12..minknow_api.device.GetSaturationConfigRequest\x1a/.minknow_api.device.GetSaturationConfigResponse\"\x03\x90\x02\x01\x12k\n\x0fget_sample_rate\x12(.minknow_api.device.GetSampleRateRequest\x1a).minknow_api.device.GetSampleRateResponse\"\x03\x90\x02\x01\x12k\n\x0fset_sample_rate\x12(.minknow_api.device.SetSampleRateRequest\x1a).minknow_api.device.SetSampleRateResponse\"\x03\x90\x02\x02\x12n\n\x10get_bias_voltage\x12).minknow_api.device.GetBiasVoltageRequest\x1a*.minknow_api.device.GetBiasVoltageResponse\"\x03\x90\x02\x01\x12n\n\x10set_bias_voltage\x12).minknow_api.device.SetBiasVoltageRequest\x1a*.minknow_api.device.SetBiasVoltageResponse\"\x03\x90\x02\x02\x12[\n\ndump_state\x12$.minknow_api.device.DumpStateRequest\x1a%.minknow_api.device.DumpStateResponse\"\x00\x42&\n\x1c\x63om.nanoporetech.minknow_api\xa2\x02\x05MKAPIb\x06proto3')
 
-_READLENGTHTYPE = DESCRIPTOR.enum_types_by_name['ReadLengthType']
-ReadLengthType = enum_type_wrapper.EnumTypeWrapper(_READLENGTHTYPE)
-_BUCKETVALUETYPE = DESCRIPTOR.enum_types_by_name['BucketValueType']
-BucketValueType = enum_type_wrapper.EnumTypeWrapper(_BUCKETVALUETYPE)
-_READENDREASON = DESCRIPTOR.enum_types_by_name['ReadEndReason']
-ReadEndReason = enum_type_wrapper.EnumTypeWrapper(_READENDREASON)
-MinknowEvents = 0
-EstimatedBases = 1
-BasecalledBases = 2
-ReadCounts = 0
-ReadLengths = 1
-All = 0
-Unknown = 1
-Partial = 2
-MuxChange = 3
-UnblockMuxChange = 4
-SignalPositive = 5
-SignalNegative = 6
-DataServiceUnblockMuxChange = 7
-
-
-_DATASELECTION = DESCRIPTOR.message_types_by_name['DataSelection']
-_STREAMDUTYTIMEREQUEST = DESCRIPTOR.message_types_by_name['StreamDutyTimeRequest']
-_STREAMDUTYTIMERESPONSE = DESCRIPTOR.message_types_by_name['StreamDutyTimeResponse']
-_STREAMDUTYTIMERESPONSE_BUCKETRANGE = _STREAMDUTYTIMERESPONSE.nested_types_by_name['BucketRange']
-_STREAMDUTYTIMERESPONSE_CHANNELSTATEDATA = _STREAMDUTYTIMERESPONSE.nested_types_by_name['ChannelStateData']
-_STREAMDUTYTIMERESPONSE_CHANNELSTATESENTRY = _STREAMDUTYTIMERESPONSE.nested_types_by_name['ChannelStatesEntry']
-_READLENGTHHISTOGRAMKEY = DESCRIPTOR.message_types_by_name['ReadLengthHistogramKey']
-_READLENGTHHISTOGRAMSPLIT = DESCRIPTOR.message_types_by_name['ReadLengthHistogramSplit']
-_STREAMREADLENGTHHISTOGRAMREQUEST = DESCRIPTOR.message_types_by_name['StreamReadLengthHistogramRequest']
-_STREAMREADLENGTHHISTOGRAMRESPONSE = DESCRIPTOR.message_types_by_name['StreamReadLengthHistogramResponse']
-_STREAMREADLENGTHHISTOGRAMRESPONSE_BUCKETRANGE = _STREAMREADLENGTHHISTOGRAMRESPONSE.nested_types_by_name['BucketRange']
-_STREAMREADLENGTHHISTOGRAMRESPONSE_READLENGTHHISTOGRAMDATA = _STREAMREADLENGTHHISTOGRAMRESPONSE.nested_types_by_name['ReadLengthHistogramData']
-_GETREADLENGTHTYPESREQUEST = DESCRIPTOR.message_types_by_name['GetReadLengthTypesRequest']
-_GETREADLENGTHTYPESRESPONSE = DESCRIPTOR.message_types_by_name['GetReadLengthTypesResponse']
-_ACQUISITIONOUTPUTKEY = DESCRIPTOR.message_types_by_name['AcquisitionOutputKey']
-_ACQUISITIONOUTPUTSPLIT = DESCRIPTOR.message_types_by_name['AcquisitionOutputSplit']
-_STREAMACQUISITIONOUTPUTREQUEST = DESCRIPTOR.message_types_by_name['StreamAcquisitionOutputRequest']
-_ACQUISITIONOUTPUTSNAPSHOT = DESCRIPTOR.message_types_by_name['AcquisitionOutputSnapshot']
-_STREAMACQUISITIONOUTPUTRESPONSE = DESCRIPTOR.message_types_by_name['StreamAcquisitionOutputResponse']
-_STREAMACQUISITIONOUTPUTRESPONSE_FILTEREDSNAPSHOTS = _STREAMACQUISITIONOUTPUTRESPONSE.nested_types_by_name['FilteredSnapshots']
-_STREAMWRITEROUTPUTREQUEST = DESCRIPTOR.message_types_by_name['StreamWriterOutputRequest']
-_WRITEROUTPUTSNAPSHOT = DESCRIPTOR.message_types_by_name['WriterOutputSnapshot']
-_STREAMWRITEROUTPUTRESPONSE = DESCRIPTOR.message_types_by_name['StreamWriterOutputResponse']
-_STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSREQUEST = DESCRIPTOR.message_types_by_name['StreamEncounteredAcquisitionOutputKeysRequest']
-_STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSRESPONSE = DESCRIPTOR.message_types_by_name['StreamEncounteredAcquisitionOutputKeysResponse']
-_STREAMTEMPERATUREREQUEST = DESCRIPTOR.message_types_by_name['StreamTemperatureRequest']
-_TEMPERATUREPACKET = DESCRIPTOR.message_types_by_name['TemperaturePacket']
-_TEMPERATUREPACKET_RANGE = _TEMPERATUREPACKET.nested_types_by_name['Range']
-_TEMPERATUREPACKET_MINIONTEMPERATURE = _TEMPERATUREPACKET.nested_types_by_name['MinIONTemperature']
-_TEMPERATUREPACKET_PROMETHIONTEMPERATURE = _TEMPERATUREPACKET.nested_types_by_name['PromethIONTemperature']
-_STREAMTEMPERATURERESPONSE = DESCRIPTOR.message_types_by_name['StreamTemperatureResponse']
-_BIASVOLTAGEPACKET = DESCRIPTOR.message_types_by_name['BiasVoltagePacket']
-_STREAMBIASVOLTAGESREQUEST = DESCRIPTOR.message_types_by_name['StreamBiasVoltagesRequest']
-_STREAMBIASVOLTAGESRESPONSE = DESCRIPTOR.message_types_by_name['StreamBiasVoltagesResponse']
-_STREAMBOXPLOTREQUEST = DESCRIPTOR.message_types_by_name['StreamBoxplotRequest']
-_BOXPLOTRESPONSE = DESCRIPTOR.message_types_by_name['BoxplotResponse']
-_BOXPLOTRESPONSE_BOXPLOTDATASET = _BOXPLOTRESPONSE.nested_types_by_name['BoxplotDataset']
-_STREAMBOXPLOTREQUEST_BOXPLOTTYPE = _STREAMBOXPLOTREQUEST.enum_types_by_name['BoxplotType']
-DataSelection = _reflection.GeneratedProtocolMessageType('DataSelection', (_message.Message,), {
-  'DESCRIPTOR' : _DATASELECTION,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Specify a desired data selection.  Units for values are as specified
-  in the corresponding Request  The actual data selection used may
-  differ from the desired one.  They are adjusted in the following
-  sequence:   1. All values are set equal to the corresponding desired
-  value.  2. Negative `start` or `end` values are fixed up by adding the
-  current maximum value to the     specified value      - Negative start
-  and end values are only supported for certain requests; typically they
-  are        supported for time-series data      - If, after adding the
-  current bucket count, the `start` value is still negative, then the
-  start value is adjusted to `0`      - If, after adding the current
-  bucket count, the `end` value is still negative, or is zero,
-  then the data selection is empty      - If data collection is still
-  ongoing, then the current bucket count may change between rpc
-  calls as more data is collected.  3. Values which are not set, or
-  which are set at `0`, are then adjusted to a default value:      -
-  `start` and `step` will be set to the minimum valid value      - `end`
-  will be set to the maximum valid value  4. Values which are outside of
-  the valid range are clamped to the nearest valid value:      - Values
-  less than minimum valid value will be set equal to the minimum valid
-  value      - Values greater than the maximum valid value will be set
-  equal to the maximum valid value  5. Finally, all values are 'rounded'
-  to a nearby valid value      - `start` and `step` will be rounded down
-  to the first valid value less than or equal to        their current
-  values      - `end` will be rounded up to the first valid value that
-  is greater than or equal to its        current value      - This means
-  that the range that is specified after rounding includes the range
-  that was        specified prior to rounding  If (`end` - `start`) is
-  not an exact integer multiple of `step`, then the final bucket will
-  cover a smaller range than that specified by `step`.  Note also that
-  the maximum valid start and end value may not be known if data
-  collection is still ongoing -- for example, the maximum valid time for
-  time series data.  If this is the case, then the maximum valid value
-  will be determined when the experiment ends, and values in use will be
-  adjusted acordingly.""",
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.DataSelection)
-  })
-_sym_db.RegisterMessage(DataSelection)
-
-StreamDutyTimeRequest = _reflection.GeneratedProtocolMessageType('StreamDutyTimeRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMDUTYTIMEREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-      data_selection:
-          The desired data selection.  The units for all values are
-          `seconds since the start of the experiment`.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamDutyTimeRequest)
-  })
-_sym_db.RegisterMessage(StreamDutyTimeRequest)
-
-StreamDutyTimeResponse = _reflection.GeneratedProtocolMessageType('StreamDutyTimeResponse', (_message.Message,), {
-
-  'BucketRange' : _reflection.GeneratedProtocolMessageType('BucketRange', (_message.Message,), {
-    'DESCRIPTOR' : _STREAMDUTYTIMERESPONSE_BUCKETRANGE,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Attributes:
-        start:
-            The range covered by a bucket Values are in seconds  The range
-            [start, end) is half open (i.e. the start value is included,
-            the end value is not).
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamDutyTimeResponse.BucketRange)
-    })
-  ,
-
-  'ChannelStateData' : _reflection.GeneratedProtocolMessageType('ChannelStateData', (_message.Message,), {
-    'DESCRIPTOR' : _STREAMDUTYTIMERESPONSE_CHANNELSTATEDATA,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Attributes:
-        state_times:
-            How much time (in samples) spent in this channel state, for
-            each bucket
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamDutyTimeResponse.ChannelStateData)
-    })
-  ,
-
-  'ChannelStatesEntry' : _reflection.GeneratedProtocolMessageType('ChannelStatesEntry', (_message.Message,), {
-    'DESCRIPTOR' : _STREAMDUTYTIMERESPONSE_CHANNELSTATESENTRY,
-    '__module__' : 'minknow_api.statistics_pb2'
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamDutyTimeResponse.ChannelStatesEntry)
-    })
-  ,
-  'DESCRIPTOR' : _STREAMDUTYTIMERESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      bucket_ranges:
-          The range covered by each entry in state_times
-      channel_states:
-          Map between channel state names, and a list of bucketed duty
-          time data
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamDutyTimeResponse)
-  })
-_sym_db.RegisterMessage(StreamDutyTimeResponse)
-_sym_db.RegisterMessage(StreamDutyTimeResponse.BucketRange)
-_sym_db.RegisterMessage(StreamDutyTimeResponse.ChannelStateData)
-_sym_db.RegisterMessage(StreamDutyTimeResponse.ChannelStatesEntry)
-
-ReadLengthHistogramKey = _reflection.GeneratedProtocolMessageType('ReadLengthHistogramKey', (_message.Message,), {
-  'DESCRIPTOR' : _READLENGTHHISTOGRAMKEY,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      read_end_reason:
-          Only return data for the given ReadEndReason.  Special values:
-          - Specify `ReadEndReason::All` to return data for all read end
-          reasons  If unspecified all read end reasons are returned.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.ReadLengthHistogramKey)
-  })
-_sym_db.RegisterMessage(ReadLengthHistogramKey)
-
-ReadLengthHistogramSplit = _reflection.GeneratedProtocolMessageType('ReadLengthHistogramSplit', (_message.Message,), {
-  'DESCRIPTOR' : _READLENGTHHISTOGRAMSPLIT,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      read_end_reason:
-          Split returned data by read_end_reason
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.ReadLengthHistogramSplit)
-  })
-_sym_db.RegisterMessage(ReadLengthHistogramSplit)
-
-StreamReadLengthHistogramRequest = _reflection.GeneratedProtocolMessageType('StreamReadLengthHistogramRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMREADLENGTHHISTOGRAMREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The `acquisition_run_id` of the acquisition to obtain data for
-          If this is set to the `acquisition_run_id` of an acquisition
-          which is in-progress, then updates containing the latest
-          histogram data for that acquisition will be streamed regularly
-          until that acquisition finishes (see `poll_time_seconds`
-          below)  Otherwise, if this is set to the `acquisition_run_id`
-          of an acquisition which is finished, and for which final
-          histogram data is available, then the final histogram data for
-          that acquisition will be returned.  Final histogram data is
-          available until it is cleared.  Otherwise, if this parameter
-          is not set, or is set to a value which is neither the
-          `acquisition_run_id` of an acquisition which is in-progress,
-          nor the `acquisition_run_id` of an acquisition for which final
-          histogram data is available, then this call will fail with the
-          status `INVALID_ARGUMENT`.
-      poll_time_seconds:
-          How often to return new histogram data, in seconds  If not
-          specified, or set to `0`, then the poll time will be set to 60
-          seconds  If data is being returned for an acquisition which is
-          in progress, then one update will be sent when the call is
-          first performed, then subsequently every `poll_time` after
-          that, and then finally once again when the acquisition
-          finishes.  Otherwise, if final histogram data is being
-          returned for an acquisition that has already finished, this
-          parameter has no effect.  The final histogram data will be
-          returned, and the call will complete.
-      read_length_type:
-          The source of the read lengths in the histogram  If MinKNOW is
-          unable to supply data from the requested source (e.g. if the
-          user requests BasecalledBases, but basecalling is not
-          enabled), then this call will fail with the status
-          `FAILED_PRECONDITION`.  See `ReadLengthType` for further
-          information about the available options.
-      data_selection:
-          The desired read length range which histograms should cover.
-          Units are as set in `read_length_type`, above.
-      bucket_value_type:
-          What data to accumulate in the read length histogram buckets
-          See `BucketValueType` for further information about the
-          available options.
-      discard_outlier_percent:
-          If set greater than zero then discard some percent of data at
-          the upper end of the source data before producing histograms
-          and N50 values.  This is intended to assist in the case where
-          a small number of outliers with very long read lengths cause
-          the histogram axes and N50 to be skewed.  Defaults to 0 - no
-          data discarded. Values should be specified in percent - a
-          value of 0.05 will cause the top 5% of the data to be
-          discarded before producing outputs.  For histograms, the data
-          discarded depends on the bucket_value_type.  If `ReadCounts`,
-          then a percentage of the total number of reads reads will be
-          discarded; if `ReadLengths` then a percentage of the total
-          read lengths will be discarded.  For the N50 value,
-          `discard_outlier_percent` always causes a percentage of the
-          total read lengths to be discarded (since it is always
-          calculated from read length data)
-      filtering:
-          Define filtering parameters for streamed data.
-      split:
-          Define how results are split for returned data.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamReadLengthHistogramRequest)
-  })
-_sym_db.RegisterMessage(StreamReadLengthHistogramRequest)
-
-StreamReadLengthHistogramResponse = _reflection.GeneratedProtocolMessageType('StreamReadLengthHistogramResponse', (_message.Message,), {
-
-  'BucketRange' : _reflection.GeneratedProtocolMessageType('BucketRange', (_message.Message,), {
-    'DESCRIPTOR' : _STREAMREADLENGTHHISTOGRAMRESPONSE_BUCKETRANGE,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Attributes:
-        start:
-            The range covered by a bucket Units are as set in
-            `read_length_type`, above  The range [start, end) is half open
-            (i.e. the start value is included, the end value is not).
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamReadLengthHistogramResponse.BucketRange)
-    })
-  ,
-
-  'ReadLengthHistogramData' : _reflection.GeneratedProtocolMessageType('ReadLengthHistogramData', (_message.Message,), {
-    'DESCRIPTOR' : _STREAMREADLENGTHHISTOGRAMRESPONSE_READLENGTHHISTOGRAMDATA,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Attributes:
-        filtering:
-            The filtering parameters which contributed to this bucket.
-        bucket_values:
-            Counts for each histogram bucket  Units are as specified in
-            `read_length_type` The range covered by each bucket is as in
-            `bucket_ranges` The type of data accumulated in each bucket is
-            given by `bucket_value_type`
-        n50:
-            The N50 value for the read length data for the selected
-            `read_length_type` and `read_end_reasons`.  Units are as
-            specified by `read_length_type`.  Measured across all source
-            data, after excluding the reads specified by
-            `discard_outlier_percent` in the stream request.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamReadLengthHistogramResponse.ReadLengthHistogramData)
-    })
-  ,
-  'DESCRIPTOR' : _STREAMREADLENGTHHISTOGRAMRESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      read_length_type:
-          The data source for the histograms  Also specifies the units
-          for `data_selection` and `n50`  See `ReadLengthType` for
-          further information about the possible options.
-      bucket_ranges:
-          The range covered by each bucket in the histogram data
-      source_data_end:
-          The right hand edge of the last source bucket which contains
-          data  Measured across all source data, after excluding the
-          reads specified by `discard_outlier_percent` in the stream
-          request.
-      bucket_value_type:
-          The data accumulated in the read length histogram buckets  See
-          `BucketValueType` for further information about the possible
-          options.
-      histogram_data:
-          The histogram data
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamReadLengthHistogramResponse)
-  })
-_sym_db.RegisterMessage(StreamReadLengthHistogramResponse)
-_sym_db.RegisterMessage(StreamReadLengthHistogramResponse.BucketRange)
-_sym_db.RegisterMessage(StreamReadLengthHistogramResponse.ReadLengthHistogramData)
-
-GetReadLengthTypesRequest = _reflection.GeneratedProtocolMessageType('GetReadLengthTypesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETREADLENGTHTYPESREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.GetReadLengthTypesRequest)
-  })
-_sym_db.RegisterMessage(GetReadLengthTypesRequest)
-
-GetReadLengthTypesResponse = _reflection.GeneratedProtocolMessageType('GetReadLengthTypesResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETREADLENGTHTYPESRESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      available_types:
-          Array of the types of bucket for which a histogram is
-          currently available
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.GetReadLengthTypesResponse)
-  })
-_sym_db.RegisterMessage(GetReadLengthTypesResponse)
-
-AcquisitionOutputKey = _reflection.GeneratedProtocolMessageType('AcquisitionOutputKey', (_message.Message,), {
-  'DESCRIPTOR' : _ACQUISITIONOUTPUTKEY,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      barcode_name:
-          Only return data for the given barcode.  Special values:   -
-          Specify "unclassified" for data which does not have a barcode.
-          - Specify "classified" for all data which has a barcode.  If
-          unspecified all barcodes are returned.
-      alignment_reference:
-          Only return data for the given alignment reference.  Special
-          values:   - Specify "unaligned" for data which does not align
-          to a reference   - Specify "aligned" for all data which aligns
-          to a reference  If unspecified all alignment targets are
-          returned.
-      alignment_bed_file_region:
-          Only return data for the given target region.  Target regions
-          are defined in bed files.  The region is a string which
-          identifies an entry in the bed file.  Special values:   -
-          Specify "offtarget" for data which does not have a bed region.
-          - Specify "ontarget" for all data which has a bed region.  If
-          unspecified all alignment regions are returned.
-      alignment_bed_file_region_name:
-          An alias to `alignment_bed_file_region`  An optional name can
-          be used to identify a target region in the bed file
-      lamp_barcode_id:
-          Only return data for the given lamp barcode.  Special values:
-          - Specify "unclassified" for data which does not have a lamp
-          barcode.   - Specify "classified" for all data which has a
-          lamp barcode.  If unspecified all lamp barcodes are returned.
-      lamp_target_id:
-          Only return data for the given lamp target.  Special values:
-          - Specify "unclassified" for data which does not have a lamp
-          target.   - Specify "classified" for all data which has a lamp
-          target. Using barcode terms here as lamp is part of barcoding
-          pipeline  If unspecified all lamp target are returned.
-      barcode_alias:
-          The barcode alias corresponding to the `barcode_name` and
-          `lamp_barcode_id`
-      read_end_reason:
-          Only return data for the given ReadEndReason.  Special values:
-          - Specify `ReadEndReason::All` to return data for all read end
-          reasons  If unspecified all read end reasons are returned.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.AcquisitionOutputKey)
-  })
-_sym_db.RegisterMessage(AcquisitionOutputKey)
-
-AcquisitionOutputSplit = _reflection.GeneratedProtocolMessageType('AcquisitionOutputSplit', (_message.Message,), {
-  'DESCRIPTOR' : _ACQUISITIONOUTPUTSPLIT,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      barcode_name:
-          Split data for every individual barcode.
-      alignment_reference:
-          Split data for each individual alignment reference.
-          References are defined in alignment references.
-      alignment_bed_file_region:
-          Split data for each target region.  Target regions are defined
-          in bed files.
-      lamp_barcode_id:
-          Split data for each lamp barcode id.  Lamp barcodes are
-          defined by the active lamp kit.
-      lamp_target_id:
-          Split data for each lamp targets id.  Lamp targets are defined
-          by the active lamp kit.
-      read_end_reason:
-          Split returned data by read_end_reason
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.AcquisitionOutputSplit)
-  })
-_sym_db.RegisterMessage(AcquisitionOutputSplit)
-
-StreamAcquisitionOutputRequest = _reflection.GeneratedProtocolMessageType('StreamAcquisitionOutputRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMACQUISITIONOUTPUTREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-      data_selection:
-          The desired data selection.  The units for all values are
-          `seconds since the start of the experiment`.
-      filtering:
-          Define filtering parameters for streamed data.
-      split:
-          Define how results are split for returned data.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamAcquisitionOutputRequest)
-  })
-_sym_db.RegisterMessage(StreamAcquisitionOutputRequest)
-
-AcquisitionOutputSnapshot = _reflection.GeneratedProtocolMessageType('AcquisitionOutputSnapshot', (_message.Message,), {
-  'DESCRIPTOR' : _ACQUISITIONOUTPUTSNAPSHOT,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """A snapshot of acquisition output data, for a given set of filtering
-  criteria.
-  
-  Attributes:
-      seconds:
-          The time the snapshot was collected, in seconds.  Represents
-          the number of seconds since the start of the experiment Will
-          usually stream in minute chunks, so will first see 60, then
-          120 etc
-      yield_summary:
-          The yield summary data.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.AcquisitionOutputSnapshot)
-  })
-_sym_db.RegisterMessage(AcquisitionOutputSnapshot)
-
-StreamAcquisitionOutputResponse = _reflection.GeneratedProtocolMessageType('StreamAcquisitionOutputResponse', (_message.Message,), {
-
-  'FilteredSnapshots' : _reflection.GeneratedProtocolMessageType('FilteredSnapshots', (_message.Message,), {
-    'DESCRIPTOR' : _STREAMACQUISITIONOUTPUTRESPONSE_FILTEREDSNAPSHOTS,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Attributes:
-        filtering:
-            The filtering parameters which contributed to this bucket.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamAcquisitionOutputResponse.FilteredSnapshots)
-    })
-  ,
-  'DESCRIPTOR' : _STREAMACQUISITIONOUTPUTRESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      snapshots:
-          Snapshots split by requested filtering parameters.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamAcquisitionOutputResponse)
-  })
-_sym_db.RegisterMessage(StreamAcquisitionOutputResponse)
-_sym_db.RegisterMessage(StreamAcquisitionOutputResponse.FilteredSnapshots)
-
-StreamWriterOutputRequest = _reflection.GeneratedProtocolMessageType('StreamWriterOutputRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMWRITEROUTPUTREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-      data_selection:
-          The desired data selection.  The units for all values are
-          `seconds since the start of the experiment`.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamWriterOutputRequest)
-  })
-_sym_db.RegisterMessage(StreamWriterOutputRequest)
-
-WriterOutputSnapshot = _reflection.GeneratedProtocolMessageType('WriterOutputSnapshot', (_message.Message,), {
-  'DESCRIPTOR' : _WRITEROUTPUTSNAPSHOT,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """A snapshot of writer data.
-  
-  Attributes:
-      seconds:
-          The time the snapshot was collected, in seconds.  Represents
-          the number of seconds since the start of the experiment Will
-          usually stream in minute chunks, so will first see 60, then
-          120 etc
-      writer_output:
-          The writer data for this bucket.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.WriterOutputSnapshot)
-  })
-_sym_db.RegisterMessage(WriterOutputSnapshot)
-
-StreamWriterOutputResponse = _reflection.GeneratedProtocolMessageType('StreamWriterOutputResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMWRITEROUTPUTRESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamWriterOutputResponse)
-  })
-_sym_db.RegisterMessage(StreamWriterOutputResponse)
-
-StreamEncounteredAcquisitionOutputKeysRequest = _reflection.GeneratedProtocolMessageType('StreamEncounteredAcquisitionOutputKeysRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamEncounteredAcquisitionOutputKeysRequest)
-  })
-_sym_db.RegisterMessage(StreamEncounteredAcquisitionOutputKeysRequest)
-
-StreamEncounteredAcquisitionOutputKeysResponse = _reflection.GeneratedProtocolMessageType('StreamEncounteredAcquisitionOutputKeysResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSRESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamEncounteredAcquisitionOutputKeysResponse)
-  })
-_sym_db.RegisterMessage(StreamEncounteredAcquisitionOutputKeysResponse)
-
-StreamTemperatureRequest = _reflection.GeneratedProtocolMessageType('StreamTemperatureRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMTEMPERATUREREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-      data_selection:
-          The desired data selection.  The units for all values are
-          `seconds since the start of the experiment`.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamTemperatureRequest)
-  })
-_sym_db.RegisterMessage(StreamTemperatureRequest)
-
-TemperaturePacket = _reflection.GeneratedProtocolMessageType('TemperaturePacket', (_message.Message,), {
-
-  'Range' : _reflection.GeneratedProtocolMessageType('Range', (_message.Message,), {
-    'DESCRIPTOR' : _TEMPERATUREPACKET_RANGE,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Represents a range of values.""",
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.TemperaturePacket.Range)
-    })
-  ,
-
-  'MinIONTemperature' : _reflection.GeneratedProtocolMessageType('MinIONTemperature', (_message.Message,), {
-    'DESCRIPTOR' : _TEMPERATUREPACKET_MINIONTEMPERATURE,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Packet of temperatures appropriate for a MinION.
-    
-    Attributes:
-        asic_temperature:
-            Temperature as measured by the probe inside the asic.
-        heatsink_temperature:
-            Temperature as measured by the probe in the minion heatsink.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.TemperaturePacket.MinIONTemperature)
-    })
-  ,
-
-  'PromethIONTemperature' : _reflection.GeneratedProtocolMessageType('PromethIONTemperature', (_message.Message,), {
-    'DESCRIPTOR' : _TEMPERATUREPACKET_PROMETHIONTEMPERATURE,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Packet of temperatures appropriate for a PromethION.
-    
-    Attributes:
-        flowcell_temperature:
-            Temperature as measured by thermistor TH2 on the P-Chip.
-        chamber_temperature:
-            Mean of 12 pixel-blocks temperatures measured with sensors in
-            the ASIC.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.TemperaturePacket.PromethIONTemperature)
-    })
-  ,
-  'DESCRIPTOR' : _TEMPERATUREPACKET,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      target_temperature:
-          The range is based on the requested target temperature and
-          tolerance.  For example, if the target temperature is 35, and
-          the tolerance is 1 then target temperatures will return as
-          34(min) and 36(max).
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.TemperaturePacket)
-  })
-_sym_db.RegisterMessage(TemperaturePacket)
-_sym_db.RegisterMessage(TemperaturePacket.Range)
-_sym_db.RegisterMessage(TemperaturePacket.MinIONTemperature)
-_sym_db.RegisterMessage(TemperaturePacket.PromethIONTemperature)
-
-StreamTemperatureResponse = _reflection.GeneratedProtocolMessageType('StreamTemperatureResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMTEMPERATURERESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamTemperatureResponse)
-  })
-_sym_db.RegisterMessage(StreamTemperatureResponse)
-
-BiasVoltagePacket = _reflection.GeneratedProtocolMessageType('BiasVoltagePacket', (_message.Message,), {
-  'DESCRIPTOR' : _BIASVOLTAGEPACKET,
-  '__module__' : 'minknow_api.statistics_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.BiasVoltagePacket)
-  })
-_sym_db.RegisterMessage(BiasVoltagePacket)
-
-StreamBiasVoltagesRequest = _reflection.GeneratedProtocolMessageType('StreamBiasVoltagesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMBIASVOLTAGESREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamBiasVoltagesRequest)
-  })
-_sym_db.RegisterMessage(StreamBiasVoltagesRequest)
-
-StreamBiasVoltagesResponse = _reflection.GeneratedProtocolMessageType('StreamBiasVoltagesResponse', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMBIASVOLTAGESRESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamBiasVoltagesResponse)
-  })
-_sym_db.RegisterMessage(StreamBiasVoltagesResponse)
-
-StreamBoxplotRequest = _reflection.GeneratedProtocolMessageType('StreamBoxplotRequest', (_message.Message,), {
-  'DESCRIPTOR' : _STREAMBOXPLOTREQUEST,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      acquisition_run_id:
-          The acquisition id of the experiment.
-      data_type:
-          Type of boxplot data to return.
-      dataset_width:
-          Defines, in minutes, the width of each dataset. This is how
-          much time should each dataset (boxplot) cover. Note that
-          MinKNOW stores all stats at a default granularity (specified
-          in the config file, i.e. 10 min in MinKNOW 3.2). This
-          dataset_width HAS to be a multiple of the default granularity!
-          Note: When multiple buckets are aggregated into a single
-          dataset, the resulting dataset will contain the average of the
-          aggregated quantiles (with the exception of min/max)! This is
-          not the same as using a larger granularity in MinKNOW configs
-          - the values that MinKNOW stores are the true quantiles.
-          Averaging quantiles will give a rough approximation, but not a
-          quantile. If the finest granularity is not required, we
-          strongly suggest changing the time coverage in the config, not
-          the dataset_width in the rpc.
-      poll_time:
-          How often to return messages in this stream, specified in
-          seconds. Note that this stream will return results regardless
-          of the stats updates (because it always returns all the
-          datasets). poll_time should be larger than the basecalled
-          stats update rate in MinKNOW - please see
-          basecalled_stats_refresh_rate_seconds in the configs (set to 1
-          second in MinKNOW 3.2).  If unspecified, defaults to 1 minute.
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.StreamBoxplotRequest)
-  })
-_sym_db.RegisterMessage(StreamBoxplotRequest)
-
-BoxplotResponse = _reflection.GeneratedProtocolMessageType('BoxplotResponse', (_message.Message,), {
-
-  'BoxplotDataset' : _reflection.GeneratedProtocolMessageType('BoxplotDataset', (_message.Message,), {
-    'DESCRIPTOR' : _BOXPLOTRESPONSE_BOXPLOTDATASET,
-    '__module__' : 'minknow_api.statistics_pb2'
-    ,
-    '__doc__': """Attributes:
-        min:
-            Minimum value for any point in the dataset.
-        q25:
-            25th quartile value for all points in the dataset.
-        q50:
-            50th quartile or median value for all points in the dataset.
-        q75:
-            75th quartile value for all points in the dataset.
-        max:
-            Maximum value for any point in the dataset.
-        count:
-            Number of items in this box plot's stats.
-        lower_full_width_half_maximum:
-            Estimated lower value where there is half the data compared to
-            the mode. provides some estimate on the sharpness of the mode
-            peak.
-        mode:
-            Estimated mode for the dataset.
-        upper_full_width_half_maximum:
-            Estimated upper value where there is half the data compared to
-            the mode. provides some estimate on the sharpness of the mode
-            peak.
-    """,
-    # @@protoc_insertion_point(class_scope:minknow_api.statistics.BoxplotResponse.BoxplotDataset)
-    })
-  ,
-  'DESCRIPTOR' : _BOXPLOTRESPONSE,
-  '__module__' : 'minknow_api.statistics_pb2'
-  ,
-  '__doc__': """Attributes:
-      datasets:
-          Result boxplots are stored in this array. This is an overview
-          of the stored data from the START of the acquisition period.
-          This includes ALL the basecalled stats from MinKNOW, not just
-          updates since previous calls!
-  """,
-  # @@protoc_insertion_point(class_scope:minknow_api.statistics.BoxplotResponse)
-  })
-_sym_db.RegisterMessage(BoxplotResponse)
-_sym_db.RegisterMessage(BoxplotResponse.BoxplotDataset)
-
-_STATISTICSSERVICE = DESCRIPTOR.services_by_name['StatisticsService']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'minknow_api.device_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.nanoporetech.minknow_api\242\002\005MKAPI'
-  _STREAMDUTYTIMEREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMDUTYTIMEREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMDUTYTIMERESPONSE_CHANNELSTATESENTRY._options = None
-  _STREAMDUTYTIMERESPONSE_CHANNELSTATESENTRY._serialized_options = b'8\001'
-  _STREAMREADLENGTHHISTOGRAMREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMREADLENGTHHISTOGRAMREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _GETREADLENGTHTYPESREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _GETREADLENGTHTYPESREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMACQUISITIONOUTPUTREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMACQUISITIONOUTPUTREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMWRITEROUTPUTREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMWRITEROUTPUTREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMTEMPERATUREREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMTEMPERATUREREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMBIASVOLTAGESREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMBIASVOLTAGESREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STREAMBOXPLOTREQUEST.fields_by_name['acquisition_run_id']._options = None
-  _STREAMBOXPLOTREQUEST.fields_by_name['acquisition_run_id']._serialized_options = b'\210\265\030\001'
-  _STATISTICSSERVICE.methods_by_name['stream_duty_time']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_duty_time']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['stream_acquisition_output']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_acquisition_output']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['stream_writer_output']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_writer_output']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['stream_encountered_acquisition_output_keys']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_encountered_acquisition_output_keys']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['stream_temperature']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_temperature']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['stream_bias_voltages']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_bias_voltages']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['stream_read_length_histogram']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_read_length_histogram']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['get_read_length_types']._options = None
-  _STATISTICSSERVICE.methods_by_name['get_read_length_types']._serialized_options = b'\220\002\001'
-  _STATISTICSSERVICE.methods_by_name['stream_basecall_boxplots']._options = None
-  _STATISTICSSERVICE.methods_by_name['stream_basecall_boxplots']._serialized_options = b'\220\002\001'
-  _READLENGTHTYPE._serialized_start=5204
-  _READLENGTHTYPE._serialized_end=5280
-  _BUCKETVALUETYPE._serialized_start=5282
-  _BUCKETVALUETYPE._serialized_end=5332
-  _READENDREASON._serialized_start=5335
-  _READENDREASON._serialized_end=5495
-  _DATASELECTION._serialized_start=118
-  _DATASELECTION._serialized_end=175
-  _STREAMDUTYTIMEREQUEST._serialized_start=177
-  _STREAMDUTYTIMEREQUEST._serialized_end=297
-  _STREAMDUTYTIMERESPONSE._serialized_start=300
-  _STREAMDUTYTIMERESPONSE._serialized_end=701
-  _STREAMDUTYTIMERESPONSE_BUCKETRANGE._serialized_start=500
-  _STREAMDUTYTIMERESPONSE_BUCKETRANGE._serialized_end=541
-  _STREAMDUTYTIMERESPONSE_CHANNELSTATEDATA._serialized_start=543
-  _STREAMDUTYTIMERESPONSE_CHANNELSTATEDATA._serialized_end=582
-  _STREAMDUTYTIMERESPONSE_CHANNELSTATESENTRY._serialized_start=584
-  _STREAMDUTYTIMERESPONSE_CHANNELSTATESENTRY._serialized_end=701
-  _READLENGTHHISTOGRAMKEY._serialized_start=703
-  _READLENGTHHISTOGRAMKEY._serialized_end=791
-  _READLENGTHHISTOGRAMSPLIT._serialized_start=793
-  _READLENGTHHISTOGRAMSPLIT._serialized_end=844
-  _STREAMREADLENGTHHISTOGRAMREQUEST._serialized_start=847
-  _STREAMREADLENGTHHISTOGRAMREQUEST._serialized_end=1304
-  _STREAMREADLENGTHHISTOGRAMRESPONSE._serialized_start=1307
-  _STREAMREADLENGTHHISTOGRAMRESPONSE._serialized_end=1876
-  _STREAMREADLENGTHHISTOGRAMRESPONSE_BUCKETRANGE._serialized_start=1704
-  _STREAMREADLENGTHHISTOGRAMRESPONSE_BUCKETRANGE._serialized_end=1745
-  _STREAMREADLENGTHHISTOGRAMRESPONSE_READLENGTHHISTOGRAMDATA._serialized_start=1748
-  _STREAMREADLENGTHHISTOGRAMRESPONSE_READLENGTHHISTOGRAMDATA._serialized_end=1876
-  _GETREADLENGTHTYPESREQUEST._serialized_start=1878
-  _GETREADLENGTHTYPESREQUEST._serialized_end=1939
-  _GETREADLENGTHTYPESRESPONSE._serialized_start=1941
-  _GETREADLENGTHTYPESRESPONSE._serialized_end=2034
-  _ACQUISITIONOUTPUTKEY._serialized_start=2037
-  _ACQUISITIONOUTPUTKEY._serialized_end=2321
-  _ACQUISITIONOUTPUTSPLIT._serialized_start=2324
-  _ACQUISITIONOUTPUTSPLIT._serialized_end=2508
-  _STREAMACQUISITIONOUTPUTREQUEST._serialized_start=2511
-  _STREAMACQUISITIONOUTPUTREQUEST._serialized_end=2768
-  _ACQUISITIONOUTPUTSNAPSHOT._serialized_start=2770
-  _ACQUISITIONOUTPUTSNAPSHOT._serialized_end=2887
-  _STREAMACQUISITIONOUTPUTRESPONSE._serialized_start=2890
-  _STREAMACQUISITIONOUTPUTRESPONSE._serialized_end=3174
-  _STREAMACQUISITIONOUTPUTRESPONSE_FILTEREDSNAPSHOTS._serialized_start=3020
-  _STREAMACQUISITIONOUTPUTRESPONSE_FILTEREDSNAPSHOTS._serialized_end=3174
-  _STREAMWRITEROUTPUTREQUEST._serialized_start=3176
-  _STREAMWRITEROUTPUTREQUEST._serialized_end=3300
-  _WRITEROUTPUTSNAPSHOT._serialized_start=3302
-  _WRITEROUTPUTSNAPSHOT._serialized_end=3415
-  _STREAMWRITEROUTPUTRESPONSE._serialized_start=3417
-  _STREAMWRITEROUTPUTRESPONSE._serialized_end=3510
-  _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSREQUEST._serialized_start=3512
-  _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSREQUEST._serialized_end=3593
-  _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSRESPONSE._serialized_start=3595
-  _STREAMENCOUNTEREDACQUISITIONOUTPUTKEYSRESPONSE._serialized_end=3722
-  _STREAMTEMPERATUREREQUEST._serialized_start=3724
-  _STREAMTEMPERATUREREQUEST._serialized_end=3847
-  _TEMPERATUREPACKET._serialized_start=3850
-  _TEMPERATUREPACKET._serialized_end=4331
-  _TEMPERATUREPACKET_RANGE._serialized_start=4114
-  _TEMPERATUREPACKET_RANGE._serialized_end=4155
-  _TEMPERATUREPACKET_MINIONTEMPERATURE._serialized_start=4157
-  _TEMPERATUREPACKET_MINIONTEMPERATURE._serialized_end=4232
-  _TEMPERATUREPACKET_PROMETHIONTEMPERATURE._serialized_start=4234
-  _TEMPERATUREPACKET_PROMETHIONTEMPERATURE._serialized_end=4316
-  _STREAMTEMPERATURERESPONSE._serialized_start=4333
-  _STREAMTEMPERATURERESPONSE._serialized_end=4425
-  _BIASVOLTAGEPACKET._serialized_start=4427
-  _BIASVOLTAGEPACKET._serialized_end=4517
-  _STREAMBIASVOLTAGESREQUEST._serialized_start=4519
-  _STREAMBIASVOLTAGESREQUEST._serialized_end=4580
-  _STREAMBIASVOLTAGESRESPONSE._serialized_start=4582
-  _STREAMBIASVOLTAGESRESPONSE._serialized_end=4676
-  _STREAMBOXPLOTREQUEST._serialized_start=4679
-  _STREAMBOXPLOTREQUEST._serialized_end=4917
-  _STREAMBOXPLOTREQUEST_BOXPLOTTYPE._serialized_start=4856
-  _STREAMBOXPLOTREQUEST_BOXPLOTTYPE._serialized_end=4917
-  _BOXPLOTRESPONSE._serialized_start=4920
-  _BOXPLOTRESPONSE._serialized_end=5202
-  _BOXPLOTRESPONSE_BOXPLOTDATASET._serialized_start=5014
-  _BOXPLOTRESPONSE_BOXPLOTDATASET._serialized_end=5202
-  _STATISTICSSERVICE._serialized_start=5498
-  _STATISTICSSERVICE._serialized_end=6800
+  _SETUSERSPECIFIEDFLOWCELLIDREQUEST.fields_by_name['id']._options = None
+  _SETUSERSPECIFIEDFLOWCELLIDREQUEST.fields_by_name['id']._serialized_options = b'\210\265\030\001'
+  _SETUSERSPECIFIEDPRODUCTCODEREQUEST.fields_by_name['code']._options = None
+  _SETUSERSPECIFIEDPRODUCTCODEREQUEST.fields_by_name['code']._serialized_options = b'\210\265\030\001'
+  _SETCALIBRATIONREQUEST.fields_by_name['first_channel']._options = None
+  _SETCALIBRATIONREQUEST.fields_by_name['first_channel']._serialized_options = b'\210\265\030\001'
+  _SETCALIBRATIONREQUEST.fields_by_name['last_channel']._options = None
+  _SETCALIBRATIONREQUEST.fields_by_name['last_channel']._serialized_options = b'\210\265\030\001'
+  _SETCALIBRATIONREQUEST.fields_by_name['offsets']._options = None
+  _SETCALIBRATIONREQUEST.fields_by_name['offsets']._serialized_options = b'\210\265\030\001'
+  _SETCALIBRATIONREQUEST.fields_by_name['pa_ranges']._options = None
+  _SETCALIBRATIONREQUEST.fields_by_name['pa_ranges']._serialized_options = b'\210\265\030\001'
+  _GETCALIBRATIONREQUEST.fields_by_name['first_channel']._options = None
+  _GETCALIBRATIONREQUEST.fields_by_name['first_channel']._serialized_options = b'\210\265\030\001'
+  _GETCALIBRATIONREQUEST.fields_by_name['last_channel']._options = None
+  _GETCALIBRATIONREQUEST.fields_by_name['last_channel']._serialized_options = b'\210\265\030\001'
+  _SETCHANNELCONFIGURATIONREQUEST_CHANNELCONFIGURATIONSENTRY._options = None
+  _SETCHANNELCONFIGURATIONREQUEST_CHANNELCONFIGURATIONSENTRY._serialized_options = b'8\001'
+  _SETCHANNELCONFIGURATIONALLREQUEST.fields_by_name['channel_configuration']._options = None
+  _SETCHANNELCONFIGURATIONALLREQUEST.fields_by_name['channel_configuration']._serialized_options = b'\220\265\030\001'
+  _SETSATURATIONCONFIGREQUEST.fields_by_name['settings']._options = None
+  _SETSATURATIONCONFIGREQUEST.fields_by_name['settings']._serialized_options = b'\220\265\030\001'
+  _GETSATURATIONCONFIGRESPONSE.fields_by_name['settings']._options = None
+  _GETSATURATIONCONFIGRESPONSE.fields_by_name['settings']._serialized_options = b'\220\265\030\001'
+  _SETSAMPLERATEREQUEST.fields_by_name['sample_rate']._options = None
+  _SETSAMPLERATEREQUEST.fields_by_name['sample_rate']._serialized_options = b'\210\265\030\001'
+  _SETBIASVOLTAGEREQUEST.fields_by_name['bias_voltage']._options = None
+  _SETBIASVOLTAGEREQUEST.fields_by_name['bias_voltage']._serialized_options = b'\210\265\030\001'
+  _DEVICESERVICE.methods_by_name['get_device_info']._options = None
+  _DEVICESERVICE.methods_by_name['get_device_info']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['get_device_state']._options = None
+  _DEVICESERVICE.methods_by_name['get_device_state']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['stream_device_state']._options = None
+  _DEVICESERVICE.methods_by_name['stream_device_state']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['get_flow_cell_info']._options = None
+  _DEVICESERVICE.methods_by_name['get_flow_cell_info']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['stream_flow_cell_info']._options = None
+  _DEVICESERVICE.methods_by_name['stream_flow_cell_info']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['set_user_specified_flow_cell_id']._options = None
+  _DEVICESERVICE.methods_by_name['set_user_specified_flow_cell_id']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['set_user_specified_product_code']._options = None
+  _DEVICESERVICE.methods_by_name['set_user_specified_product_code']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['get_channels_layout']._options = None
+  _DEVICESERVICE.methods_by_name['get_channels_layout']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['reset_device_settings']._options = None
+  _DEVICESERVICE.methods_by_name['reset_device_settings']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['set_calibration']._options = None
+  _DEVICESERVICE.methods_by_name['set_calibration']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['clear_calibration']._options = None
+  _DEVICESERVICE.methods_by_name['clear_calibration']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['get_calibration']._options = None
+  _DEVICESERVICE.methods_by_name['get_calibration']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['set_temperature']._options = None
+  _DEVICESERVICE.methods_by_name['set_temperature']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['get_temperature']._options = None
+  _DEVICESERVICE.methods_by_name['get_temperature']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['stream_temperature']._options = None
+  _DEVICESERVICE.methods_by_name['stream_temperature']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['get_channel_configuration']._options = None
+  _DEVICESERVICE.methods_by_name['get_channel_configuration']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['set_channel_configuration']._options = None
+  _DEVICESERVICE.methods_by_name['set_channel_configuration']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['set_channel_configuration_all']._options = None
+  _DEVICESERVICE.methods_by_name['set_channel_configuration_all']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['get_saturation_config']._options = None
+  _DEVICESERVICE.methods_by_name['get_saturation_config']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['get_sample_rate']._options = None
+  _DEVICESERVICE.methods_by_name['get_sample_rate']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['set_sample_rate']._options = None
+  _DEVICESERVICE.methods_by_name['set_sample_rate']._serialized_options = b'\220\002\002'
+  _DEVICESERVICE.methods_by_name['get_bias_voltage']._options = None
+  _DEVICESERVICE.methods_by_name['get_bias_voltage']._serialized_options = b'\220\002\001'
+  _DEVICESERVICE.methods_by_name['set_bias_voltage']._options = None
+  _DEVICESERVICE.methods_by_name['set_bias_voltage']._serialized_options = b'\220\002\002'
+  _FLOWCELLCONNECTORTYPE._serialized_start=6128
+  _FLOWCELLCONNECTORTYPE._serialized_end=6233
+  _INSERTIONSCRIPTSTATUS._serialized_start=6235
+  _INSERTIONSCRIPTSTATUS._serialized_end=6298
+  _SELECTEDWELL._serialized_start=6300
+  _SELECTEDWELL._serialized_end=6393
+  _CHANNELCONFIGURATION._serialized_start=111
+  _CHANNELCONFIGURATION._serialized_end=169
+  _RETURNEDCHANNELCONFIGURATION._serialized_start=171
+  _RETURNEDCHANNELCONFIGURATION._serialized_end=254
+  _GETDEVICEINFOREQUEST._serialized_start=256
+  _GETDEVICEINFOREQUEST._serialized_end=278
+  _GETDEVICEINFORESPONSE._serialized_start=281
+  _GETDEVICEINFORESPONSE._serialized_end=792
+  _GETDEVICEINFORESPONSE_COMPONENTVERSION._serialized_start=617
+  _GETDEVICEINFORESPONSE_COMPONENTVERSION._serialized_end=694
+  _GETDEVICEINFORESPONSE_DEVICETYPE._serialized_start=696
+  _GETDEVICEINFORESPONSE_DEVICETYPE._serialized_end=792
+  _GETDEVICESTATEREQUEST._serialized_start=794
+  _GETDEVICESTATEREQUEST._serialized_end=817
+  _GETDEVICESTATERESPONSE._serialized_start=820
+  _GETDEVICESTATERESPONSE._serialized_end=1052
+  _GETDEVICESTATERESPONSE_DEVICESTATE._serialized_start=996
+  _GETDEVICESTATERESPONSE_DEVICESTATE._serialized_end=1052
+  _STREAMDEVICESTATEREQUEST._serialized_start=1054
+  _STREAMDEVICESTATEREQUEST._serialized_end=1080
+  _GETFLOWCELLINFOREQUEST._serialized_start=1082
+  _GETFLOWCELLINFOREQUEST._serialized_end=1106
+  _GETFLOWCELLINFORESPONSE._serialized_start=1109
+  _GETFLOWCELLINFORESPONSE._serialized_end=1546
+  _STREAMFLOWCELLINFOREQUEST._serialized_start=1548
+  _STREAMFLOWCELLINFOREQUEST._serialized_end=1575
+  _SETUSERSPECIFIEDFLOWCELLIDREQUEST._serialized_start=1577
+  _SETUSERSPECIFIEDFLOWCELLIDREQUEST._serialized_end=1630
+  _SETUSERSPECIFIEDFLOWCELLIDRESPONSE._serialized_start=1632
+  _SETUSERSPECIFIEDFLOWCELLIDRESPONSE._serialized_end=1668
+  _SETUSERSPECIFIEDPRODUCTCODEREQUEST._serialized_start=1670
+  _SETUSERSPECIFIEDPRODUCTCODEREQUEST._serialized_end=1726
+  _SETUSERSPECIFIEDPRODUCTCODERESPONSE._serialized_start=1728
+  _SETUSERSPECIFIEDPRODUCTCODERESPONSE._serialized_end=1765
+  _GETCHANNELSLAYOUTREQUEST._serialized_start=1767
+  _GETCHANNELSLAYOUTREQUEST._serialized_end=1793
+  _GETCHANNELSLAYOUTRESPONSE._serialized_start=1795
+  _GETCHANNELSLAYOUTRESPONSE._serialized_end=1882
+  _CHANNELRECORD._serialized_start=1885
+  _CHANNELRECORD._serialized_end=2049
+  _CHANNELRECORD_MUXRECORD._serialized_start=1994
+  _CHANNELRECORD_MUXRECORD._serialized_end=2049
+  _RESETDEVICESETTINGSREQUEST._serialized_start=2051
+  _RESETDEVICESETTINGSREQUEST._serialized_end=2079
+  _RESETDEVICESETTINGSRESPONSE._serialized_start=2081
+  _RESETDEVICESETTINGSRESPONSE._serialized_end=2110
+  _SETCALIBRATIONREQUEST._serialized_start=2113
+  _SETCALIBRATIONREQUEST._serialized_end=2241
+  _SETCALIBRATIONRESPONSE._serialized_start=2243
+  _SETCALIBRATIONRESPONSE._serialized_end=2267
+  _CLEARCALIBRATIONREQUEST._serialized_start=2269
+  _CLEARCALIBRATIONREQUEST._serialized_end=2294
+  _CLEARCALIBRATIONRESPONSE._serialized_start=2296
+  _CLEARCALIBRATIONRESPONSE._serialized_end=2322
+  _GETCALIBRATIONREQUEST._serialized_start=2324
+  _GETCALIBRATIONREQUEST._serialized_end=2404
+  _GETCALIBRATIONRESPONSE._serialized_start=2406
+  _GETCALIBRATIONRESPONSE._serialized_end=2513
+  _SETTEMPERATUREREQUEST._serialized_start=2516
+  _SETTEMPERATUREREQUEST._serialized_end=2919
+  _SETTEMPERATUREREQUEST_WAITFORTEMPERATURESETTINGS._serialized_start=2770
+  _SETTEMPERATUREREQUEST_WAITFORTEMPERATURESETTINGS._serialized_end=2863
+  _SETTEMPERATUREREQUEST_SECONDARYTEMPERATURELIMITS._serialized_start=2865
+  _SETTEMPERATUREREQUEST_SECONDARYTEMPERATURELIMITS._serialized_end=2919
+  _SETTEMPERATURERESPONSE._serialized_start=2922
+  _SETTEMPERATURERESPONSE._serialized_end=3230
+  _SETTEMPERATURERESPONSE_SETTEMPERATURERESULT._serialized_start=3073
+  _SETTEMPERATURERESPONSE_SETTEMPERATURERESULT._serialized_end=3230
+  _GETTEMPERATUREREQUEST._serialized_start=3232
+  _GETTEMPERATUREREQUEST._serialized_end=3255
+  _GETTEMPERATURERESPONSE._serialized_start=3258
+  _GETTEMPERATURERESPONSE._serialized_end=3801
+  _GETTEMPERATURERESPONSE_MINIONTEMPERATURE._serialized_start=3510
+  _GETTEMPERATURERESPONSE_MINIONTEMPERATURE._serialized_end=3643
+  _GETTEMPERATURERESPONSE_PROMETHIONTEMPERATURE._serialized_start=3646
+  _GETTEMPERATURERESPONSE_PROMETHIONTEMPERATURE._serialized_end=3786
+  _STREAMTEMPERATUREREQUEST._serialized_start=3803
+  _STREAMTEMPERATUREREQUEST._serialized_end=3853
+  _UNBLOCKREQUEST._serialized_start=3855
+  _UNBLOCKREQUEST._serialized_end=3968
+  _UNBLOCKRESPONSE._serialized_start=3970
+  _UNBLOCKRESPONSE._serialized_end=3987
+  _CANCELUNBLOCKSREQUEST._serialized_start=3989
+  _CANCELUNBLOCKSREQUEST._serialized_end=4012
+  _CANCELUNBLOCKSRESPONSE._serialized_start=4014
+  _CANCELUNBLOCKSRESPONSE._serialized_end=4066
+  _GETCHANNELCONFIGURATIONREQUEST._serialized_start=4068
+  _GETCHANNELCONFIGURATIONREQUEST._serialized_end=4118
+  _GETCHANNELCONFIGURATIONRESPONSE._serialized_start=4120
+  _GETCHANNELCONFIGURATIONRESPONSE._serialized_end=4235
+  _SETCHANNELCONFIGURATIONREQUEST._serialized_start=4238
+  _SETCHANNELCONFIGURATIONREQUEST._serialized_end=4485
+  _SETCHANNELCONFIGURATIONREQUEST_CHANNELCONFIGURATIONSENTRY._serialized_start=4383
+  _SETCHANNELCONFIGURATIONREQUEST_CHANNELCONFIGURATIONSENTRY._serialized_end=4485
+  _SETCHANNELCONFIGURATIONRESPONSE._serialized_start=4487
+  _SETCHANNELCONFIGURATIONRESPONSE._serialized_end=4520
+  _SETCHANNELCONFIGURATIONALLREQUEST._serialized_start=4522
+  _SETCHANNELCONFIGURATIONALLREQUEST._serialized_end=4636
+  _SETCHANNELCONFIGURATIONALLRESPONSE._serialized_start=4638
+  _SETCHANNELCONFIGURATIONALLRESPONSE._serialized_end=4674
+  _SATURATIONCONFIG._serialized_start=4677
+  _SATURATIONCONFIG._serialized_end=5515
+  _SATURATIONCONFIG_THRESHOLDS._serialized_start=4950
+  _SATURATIONCONFIG_THRESHOLDS._serialized_end=5200
+  _SATURATIONCONFIG_SOFTWARESATURATION._serialized_start=5203
+  _SATURATIONCONFIG_SOFTWARESATURATION._serialized_end=5350
+  _SATURATIONCONFIG_USERTHRESHOLDSATURATION._serialized_start=5353
+  _SATURATIONCONFIG_USERTHRESHOLDSATURATION._serialized_end=5515
+  _SETSATURATIONCONFIGREQUEST._serialized_start=5517
+  _SETSATURATIONCONFIGREQUEST._serialized_end=5607
+  _SETSATURATIONCONFIGRESPONSE._serialized_start=5609
+  _SETSATURATIONCONFIGRESPONSE._serialized_end=5638
+  _GETSATURATIONCONFIGREQUEST._serialized_start=5640
+  _GETSATURATIONCONFIGREQUEST._serialized_end=5668
+  _GETSATURATIONCONFIGRESPONSE._serialized_start=5670
+  _GETSATURATIONCONFIGRESPONSE._serialized_end=5761
+  _GETSAMPLERATEREQUEST._serialized_start=5763
+  _GETSAMPLERATEREQUEST._serialized_end=5785
+  _GETSAMPLERATERESPONSE._serialized_start=5787
+  _GETSAMPLERATERESPONSE._serialized_end=5831
+  _SETSAMPLERATEREQUEST._serialized_start=5833
+  _SETSAMPLERATEREQUEST._serialized_end=5882
+  _SETSAMPLERATERESPONSE._serialized_start=5884
+  _SETSAMPLERATERESPONSE._serialized_end=5933
+  _GETBIASVOLTAGEREQUEST._serialized_start=5935
+  _GETBIASVOLTAGEREQUEST._serialized_end=5958
+  _GETBIASVOLTAGERESPONSE._serialized_start=5960
+  _GETBIASVOLTAGERESPONSE._serialized_end=6006
+  _SETBIASVOLTAGEREQUEST._serialized_start=6008
+  _SETBIASVOLTAGEREQUEST._serialized_end=6059
+  _SETBIASVOLTAGERESPONSE._serialized_start=6061
+  _SETBIASVOLTAGERESPONSE._serialized_end=6085
+  _DUMPSTATEREQUEST._serialized_start=6087
+  _DUMPSTATEREQUEST._serialized_end=6105
+  _DUMPSTATERESPONSE._serialized_start=6107
+  _DUMPSTATERESPONSE._serialized_end=6126
+  _DEVICESERVICE._serialized_start=6396
+  _DEVICESERVICE._serialized_end=9636
+SetTemperatureRequest.__doc__ = """Attributes:
+    temperature:
+        The desired temperature in degrees Celsius.  If temperature
+        control is supported and enabled, the device will attempt to
+        keep its primary temperature at this value. The reading used
+        as the "primary" temperature depends on the device: - For
+        MinIONs, the primary temperature is the heatsink temperature -
+        For PromethIONs, the primary temperature is the flow cell
+        temperature  (If temperature control is not supported or is
+        not enabled, the call to `set_temperature` will fail with
+        `FAILED_PRECONDITION`)
+    wait_for_temperature:
+        Settings which can be specified in order to wait for the
+        temperature to be reached.  If this is not set at all, no
+        waiting will be done. If it is set (even to an empty
+        WaitForTemperatureSettings object), the call will not return
+        until either: - The target temperature was reached, or - The
+        timeout was reached, or - The secondary temperature limits
+        were exceeded  If `wait_for_temperature` is supplied then, on
+        MinIONs and GridIONs, the ASIC power will be enabled if it was
+        not already. See `acquisition.StopRequest.keep_power_on` for
+        more details about the implications of this.  Since 1.15
+    secondary_temperature_limits:
+        Specify "secondary" temperature limits  This field allows
+        limits to be placed on the "secondary" temperature, while
+        waiting for the primary temperature to reach its target value
+        (as specified in the `temperature` field, above).  The meaning
+        of the "secondary" temperature depends on the device in
+        question: - For MinIONs, this is the ASIC temperature (i.e.
+        flow cell or flow cell adapter   temperature) - For
+        PromethIONs, this is the "chamber" temperature (which is
+        derived from the measurements   of the ASIC temperature)
+        These limits are intended to act as a safeguard against the
+        case where the flow cell does not have good thermal contact
+        with temperature control hardware (e.g. if the flow cell was
+        not fully seated when it was inserted into the device). In
+        such cases, the flow cell temperature may rise high enough to
+        damage the flow cell; these limits may be used to mitigate the
+        risk of the flow cell temperature rising high enough to cause
+        damage to the flow cell.  If the secondary temperature exceeds
+        the specified limits while waiting for the target temperature
+        to be reached, then all temperature control settings are reset
+        to the values they had prior to the call to
+        `set_temperature()` being made.  NB - These limits apply ONLY
+        when waiting for the target temperature to be reached; once
+        the call to `set_temperature()` returns, these limits are no
+        longer checked.  Since 5.5
+"""
+SetTemperatureResponse.__doc__ = """Attributes:
+    timed_out_waiting_for_temperature:
+        Find if we hit a timeout waiting for the temperature to be
+        hit.  Deprecated since 5.5; in favour of the
+        `TIMED_OUT_WAITING_FOR_TEMPERATURE` result code.
+    result:
+        The result of setting the temperature  Since 5.5  NB - before
+        5.5, checking this field will always return a value of
+        `TARGET_TEMPERATURE_SET` The "real" value may be inferred as
+        follows:  - If `wait_for_temperature` was NOT specified, the
+        "real" result is    `TARGET_TEMPERATURE_SET`  - If
+        `wait_for_temperature` was specified, and
+        `timed_out_waiting_for_temperature` is    false, the "real"
+        result is `REACHED_TEMPERATURE`  - If `wait_for_temperature`
+        was specified, and `timed_out_waiting_for_temperature` is
+        true, the "real" result is `TIMED_OUT_WAITING_FOR_TEMPERATURE`
+        - Versions prior to 5.5 do not support setting the secondary
+        temperature limit, and so (for    these versions) the "real"
+        value can never be `SECONDARY_TEMPERATURE_LIMITS_EXCEEDED`
+"""
+SaturationConfig.__doc__ = """Attributes:
+    thresholds:
+        Settings for saturation count thresholds, this controls how
+        long a saturated value must be over limit before the channel
+        is turned off.  If not specified, the previous thresholds are
+        kept.
+    software_saturation:
+        Settings for software saturation, specified in adc units of
+        the device.  If not specified, the previous thresholds are
+        kept.
+    user_threshold_saturation:
+        Settings for user threshold saturation, specified in pA.  If
+        not specified, the previous thresholds are kept.
+"""
+GetDeviceInfoResponse.ComponentVersion.__doc__ = """Firmware versions and serial-numbers of components associated with
+this device  Depending on the hardware, there may be several
+components associated with this device, each with their own firmware
+version and serial-number. Not all components have serial-numbers.
+
+Attributes:
+    component:
+        Description of the component that has firmware
+    version:
+        The firmware version, if this cannot be determined for a
+        component where the firmware version would usually be
+        available, this will contain "Unknown"
+    serial_number:
+        The serial-number of a component. If this in not applicable to
+        the type of component or cannot be read at the current time,
+        then this field will be blank.
+"""
+SetChannelConfigurationRequest.__doc__ = """Attributes:
+    channel_configurations:
+        A map between <channel name, config to set>  Will return an
+        error if any of the key values (representing channel names)
+        are below 1, or above the channel count value returned from
+        :meth:`get_flow_cell_info`  The selected well cannot be set to
+        WELL_OTHER, and will error if it tries to do so  DEPRECATED:
+        Note that the type to set may change from 4.0 to enforce the
+        fact that unblock cannot be set through this call
+"""
+ReturnedChannelConfiguration.__doc__ = """Describes the configuration of a channel on the device.  Note that
+this is a lossy representation. The device-specific APIs provide more
+precise information. This only describes common configurations, and
+omits anything that doesn't impact the received signal.
+
+Attributes:
+    well:
+        The currently-connected well.  Wells are counted from 1. 0
+        indicates that no well is connected. 5 indicates some non-
+        generic configuration such as ground for a minion or
+        connecting all wells on promethion  Note that MinKNOW can
+        return channel configurations where the well number is larger
+        than the ``max_well_count`` value returned by
+        :meth:`DeviceService.get_device_info`. This indicates that
+        some other connection has been made (for example, PromethIONs
+        can simultaneously connect all wells, and MinIONs can connect
+        to ground).
+    test_current:
+        Whether the test current is connected to the integrator
+        (measurement circuit).  The signal will be a steady test
+        current produced on the device. This can be used for
+        calibration or to test the device integration circuits.
+    unblock:
+        Whether the unblock voltage is connected to the integrator
+        (measurement circuit).  Provides a reverse potential across
+        the connected well. This can be used to drive molecules back
+        out of the well.
+"""
+SaturationConfig.Thresholds.__doc__ = """The thresholds define how many over limit samples are required to
+trigger saturation on the device.  Each packet of frames minknow
+receive is delivered to the saturation check (in approx 64 frame
+chunks), only the first frame of each packet is inspected. The
+thresholds control how many _packets_ must be outside the valid range.
+ie. if general_threshold is set to 10, at least 640 frames are
+required to trigger saturation.  It is also possible to not define the
+value to never trigger saturation in this config.  Note: Setting a
+saturation threshold to 0 will prevent the threshold from triggering.
+
+Attributes:
+    general_threshold:
+        Threshold for software saturation on all non-unblock muxes
+    unblock_threshold:
+        Threshold for software saturation on unblock muxes
+    user_general_threshold:
+        Threshold for user threshold  saturation on all non-unblock
+        muxes
+    user_unblock_threshold:
+        Threshold for user threshold saturation on unblock muxes
+"""
+GetChannelConfigurationRequest.__doc__ = """Attributes:
+    channels:
+        A list of channel names (1-indexed) to specify what channels
+        to get channel configs for  Will return an error if any of the
+        channel names are below 1, or above the channel count value
+        returned from :meth:`get_flow_cell_info`
+"""
+SetUserSpecifiedFlowCellIdRequest.__doc__ = """Attributes:
+    id:
+        A unique identifier for the flow cell, which the user can
+        specify.  In the event a flow cell does not have an eeprom,
+        this field can be used by the user to record their
+        flow_cell_id.  Since 1.12
+"""
+CancelUnblocksResponse.__doc__ = """Attributes:
+    cancelled_unblocks:
+        The number of unblocks which have been cancelled as part of
+        this request.  Should return the total number of unblock
+        operations which have been cancelled.
+"""
+SetSampleRateResponse.__doc__ = """Attributes:
+    real_sample_rate:
+        The real sample rate is the actual sample rate that is set on
+        the device, which may be different from the actual value
+        passed into the rpc.  For example on promethion, when it is
+        given a sample rate, it will round to the nearest 1000. So
+        1499 becomes 1000 and 1500 becomes 2000 real sample rate  For
+        a minion, the actual sample rate is determined via 3 separate
+        values; clock speed, integration time and clock divider, and
+        so not all values are possible. e.g. setting 3000 will return
+        3012 real sample rate. See 'sampling_frequency' in
+        MinionDeviceService for a slightly more in depth explanation
+"""
+SetTemperatureRequest.WaitForTemperatureSettings.__doc__ = """Attributes:
+    timeout:
+        Maximum duration (in seconds) to wait for the device to reach
+        temperature.  Not specifying a value will wait for a maximum
+        of 5 minutes.
+    min_stable_duration:
+        Minimum duration (in seconds) that the reported temperature
+        must be continually within the target temperature range,
+        before the device is considered to have reached temperature.
+        A value of zero means that the device will be considered to
+        have reached temperature as soon as the reported temperature
+        is equal to the target temperature.  Not specifying a value is
+        equivalent to specifying a value of zero.  The
+        min_stable_duration must be less than or equal to the timeout
+        duration (if it were greater, then the temperature would never
+        be read as 'stable' before the time-out occurred).  Since 3.4
+    tolerance:
+        Specify an optional tolerance to apply to the wait.  For
+        example, if the target temperature is 35, and the tolerance is
+        1 any temperature in the range 34 - 36 will cause the request
+        to return.  Default is 0.5 degree tolerance.
+"""
+GetCalibrationRequest.__doc__ = """Attributes:
+    first_channel:
+        The first channel to get calibration data for.  This should
+        normally be 1.
+    last_channel:
+        The last channel included in calibration data.  This should
+        normally be the channel count returned by
+        :meth:`get_flow_cell_info`.
+"""
+GetDeviceInfoResponse.__doc__ = """Attributes:
+    device_id:
+        A unique identifier for the device.  This is the identifier of
+        the device MinKNOW was started for. It will only communicate
+        with this device.  Note that simulated device IDs are only
+        unique for this host, not globally.  This value will be set
+        even if the device is not currently connected (assuming
+        MinKNOW was started by the manager service).
+    device_type:
+        The type of the device.
+    is_simulated:
+        Whether the device is simulated.  If this is true, there is no
+        physical device - MinKNOW is simulating it. If it is false,
+        MinKNOW will be acquiring data from a real device.
+    max_channel_count:
+        The maximum number of channels supported by the device.  Each
+        channel provides a signal from the device. For example, a
+        MinION supports up to 512 channels, and so can provide 512
+        simultaneous streams of data.  This value is fixed for a given
+        device type. Note, however, that a flow cell might be attached
+        that has a smaller number of channels.
+    max_wells_per_channel:
+        The maximum number of wells connected to each channel.  A well
+        is a discrete location on the device where sensing can take
+        place. Normally, each well should have a single nanopore in
+        it.  For example, a MinION supports up to 4 wells per channel,
+        allowing for 2048 wells in total. So the value of this for a
+        MinION will be 4.  This value is fixed for a given device
+        type. Note, however, that a flow cell might be attached that
+        has a smaller number of wells on each channel.
+    can_set_temperature:
+        Whether the set_temperature() method can be expected to work.
+        On some systems, not all connected devices have the ability to
+        control their own temperature, as temperature controls are
+        managed in groups. If this field is true, this device can
+        control its own temperature. If it it false, it cannot, and
+        the temperature will be maintained at a pre-determined
+        temperature.
+    digitisation:
+        The range of uncalibrated data values.  This is the number of
+        distinct signal values that can be produced by the device's
+        analog to digital converter (ADC).
+"""
+SetCalibrationRequest.__doc__ = """Attributes:
+    first_channel:
+        The first channel included in calibration data.  This must
+        always be 1. This is required in order to make sure the client
+        and MinKNOW agree on what data is being provided.
+    last_channel:
+        The last channel included in calibration data.  This must
+        always be the same as the channel count returned by
+        :meth:`get_flow_cell_info`. This is required in order to make
+        sure the client and MinKNOW agree on what data is being
+        provided.
+    offsets:
+        The ADC value adjustment to reach 0pA on each channel.  This
+        is ``-x``, where ``x`` is the (mean) ADC value at 0pA.
+    pa_ranges:
+        The range of possible pA values that can be produced by the
+        device.
+"""
+GetFlowCellInfoResponse.__doc__ = """Attributes:
+    has_flow_cell:
+        Whether there is a flow cell present.  If both this and
+        has_adapter are false, none of the other fields will contain
+        useful information.
+    channel_count:
+        The number of channels currently supported by the device.
+        This may be smaller than the ``max_channel_count`` value
+        returned by get_device_info(), depending on the attached flow
+        cell.
+    wells_per_channel:
+        The number of wells currently supported by the device.  This
+        may be smaller than the ``max_wells_per_channel`` value
+        returned by get_device_info(), depending on the attached flow
+        cell.
+    flow_cell_id:
+        The unique identifier for the flow cell.  This should be same
+        as the value printed onto the flow cell casing. Not all flow
+        cells will have the flow cell ID recorded in a way that
+        MinKNOW can read. In those cases, this will be an empty
+        string, even though the user may be able to see a printed
+        identifier on the flow cell.
+    asic_id_str:
+        The unique identifier for the ASIC (formatted as string).
+        This is a value uniquely identifying the ASIC embedded in the
+        flow cell. It will always be set when a flow cell is present.
+        The intended use for this is to track the identity of the asic
+        in the flow cell, eg. for displaying to users during
+        production of chips.  Caveats:  * This value will not mean
+        anything to a customer. * There is no guarantee that this
+        field will contain the same identifier across   MinKNOW
+        versions, even with the same flow cell. * An ASIC can be
+        recycled into a new flow cell, so this identifier may be re-
+        used in the   future (although it can be considered unique for
+        the duration of a protocol run).
+    product_code:
+        The product code for the flow cell.  This should be the code
+        displayed in the shop where the flow cell was bought. Not all
+        flow cells will have the product code recorded in a way that
+        MinKNOW can read. In those cases, this will be an empty
+        string.
+    user_specified_flow_cell_id:
+        A unique identifier for the flow cell, which the user can
+        specify.  In the event a flow cell does not have an eeprom,
+        this field contains data input by the user using
+        set_flow_cell_info to record required data.  Only alpha-
+        numeric, space, dash and underscore characters are allowed in
+        this field.  Since 1.12
+    user_specified_product_code:
+        A product code for the flow cell, which the user can specify.
+        This should be the code displayed in the shop where the flow
+        cell was bought. Not all flow cells have an eeprom, in the
+        event they don't, the user can specify using this id using
+        set_flow_cell_info.  Since 1.12
+    has_adapter:
+        Whether there is a flongle adapter.  If this is true, the
+        adapter_id, channel_count and wells_per_channel fields should
+        all provide useful information, even if has_flow_cell is
+        false.
+    adapter_id:
+        The unique identifier of an attached flongle adapter.  This
+        should be same as the value printed onto the adapter casing.
+    temperature_offset_nullable:
+        Used to make the field nullable, since the null value is not
+        protobuf's default.
+    temperature_offset:
+        The temperature offset for the flow cell, returned as an
+        offset in degrees Celsius.  This offset specifies a correction
+        to be applied to ASIC temperature. If multiple ASIC
+        temperatures are available from the device, applies to the
+        mean temperature.  Since 1.14
+    asic_version:
+        The version of the ASIC contained in the flow cell (if
+        specified by the hardware).  This can be used to determine if
+        the hardware should support certain features added to only
+        newer ASICs.  Possible values include: "IA02C", "IA02D", or if
+        the value is not readable on the current hardware an empty
+        string is returned.  Since 1.14
+    insertion_script_status:
+        If the configuration specifies a script to run when a flow-
+        cell is inserted, this shows if it completed successfully.
+        Since 5.0
+"""
+GetTemperatureResponse.MinIONTemperature.__doc__ = """Packet of temperatures appropriate for a MinION.
+
+Attributes:
+    asic_temperature:
+        Temperature as measured by the probe inside the asic. This is
+        the "secondary" temperature
+    heatsink_temperature:
+        Temperature as measured by the probe in the minion heatsink.
+        This is the "primary" temperature
+"""
+GetTemperatureResponse.PromethIONTemperature.__doc__ = """Packet of temperatures appropriate for a PromethION.
+
+Attributes:
+    flowcell_temperature:
+        Temperature as measured by thermistor TH2 on the P-Chip. This
+        is the "primary" temperature
+    chamber_temperature:
+        Mean of 12 pixel-blocks temperatures measured with sensors in
+        the ASIC. This is the "secondary" temperature
+"""
+GetChannelConfigurationResponse.__doc__ = """Attributes:
+    channel_configurations:
+        A list of channel configurations  The order of channel
+        configurations matches the channel order specified by
+        :attribute:`channels` in the request message
+"""
+SaturationConfig.UserThresholdSaturation.__doc__ = """User threshold is specified in pico amps
+
+Attributes:
+    enabled:
+        Set to enable or disable software saturation.
+    user_threshold_min_pa:
+        The minimum pA value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+    user_threshold_max_pa:
+        The maximum pA value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+"""
+GetCalibrationResponse.__doc__ = """Attributes:
+    digitisation:
+        The range of possible ADC values that can be produced by the
+        device.  This is the same as the digitisation value returned
+        by the :meth:`DeviceService.get_device_info` RPC. It is
+        included here for convenience.
+    offsets:
+        The ADC value adjustment to reach 0pA on each channel.  This
+        is ``-x``, where ``x`` is the (mean) ADC value at 0pA.
+    pa_ranges:
+        The range of possible pA values that can be produced on each
+        channel.  The change in pA represented by a change of 1 ADC
+        can be calculated by dividing the digitisation by this value.
+    has_calibration:
+        Find if there is a stored calibration, or if the returned
+        response is empty.  Since 1.12
+"""
+UnblockRequest.__doc__ = """Attributes:
+    channels:
+        List of channels indexed from 1.
+    duration:
+        How long should an unblock last.
+"""
+GetDeviceStateResponse.__doc__ = """Attributes:
+    device_state:
+        Whether the physical hardware is present.  This is really only
+        relevant to MinIONs, which could be unplugged by the user at
+        any time.
+    flow_cell_connector:
+        Indicates what sort of flow cell can be inserted.  For
+        example, if the user needs to set or override the flow cell
+        product code, this can be used to limit the list of possible
+        flow cell product codes to choose from.  Since 4.1
+"""
+SetUserSpecifiedProductCodeRequest.__doc__ = """Attributes:
+    code:
+        A product code for the flow cell, which the user can specify.
+        In the event a flow cell does not have an eeprom, the user can
+        specify product code here.  Since 1.12
+"""
+ChannelConfiguration.__doc__ = """Describes the configuration of a channel on the device.  Note that
+this is a lossy representation. The device-specific APIs provide more
+precise information. This only describes common configurations, and
+omits anything that doesn't impact the received signal.
+
+Attributes:
+    well:
+        The currently-connected well.  Wells are counted from 1. 0
+        indicates that no well is connected. 5 indicates some non-
+        generic configuration such as ground for a minion or
+        connecting all wells on promethion  Note that MinKNOW can
+        return channel configurations where the well number is larger
+        than the ``max_well_count`` value returned by
+        :meth:`DeviceService.get_device_info`. This indicates that
+        some other connection has been made (for example, PromethIONs
+        can simultaneously connect all wells, and MinIONs can connect
+        to ground).
+    test_current:
+        Whether the test current is connected to the integrator
+        (measurement circuit).  The signal will be a steady test
+        current produced on the device. This can be used for
+        calibration or to test the device integration circuits.
+"""
+SaturationConfig.SoftwareSaturation.__doc__ = """The ranges specify the actual pA or ADC ranges which will trigger
+saturation. This range is checked against the first sample in each
+delivered packet.  software saturation is specified in adc units
+
+Attributes:
+    enabled:
+        Set to enable or disable software saturation.
+    software_min_adc:
+        The minimum adc value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+    software_max_adc:
+        The maximum adc value that is not a saturation.  If this value
+        is not specified, the previous value is kept.
+"""
+StreamTemperatureRequest.__doc__ = """Attributes:
+    period_seconds:
+        How often temperature updates should be sent Defaults to a
+        period of 1 second, if not specified, or set to 0
+    acquisition_run_id:
+        The acquisition id of the experiment.
+    data_selection:
+        The desired data selection.  The units for all values are
+        `seconds since the start of the experiment`.
+"""
+SetTemperatureRequest.SecondaryTemperatureLimits.__doc__ = """Attributes:
+    min:
+        The minimum permissible "secondary" temperature
+    max:
+        The maximum permissible "secondary" temperature
+"""
+GetTemperatureResponse.__doc__ = """Attributes:
+    target_temperature:
+        Return the temperature target the device is aiming to reach.
+    flowcell_temperature:
+        Temperature as measured by thermistor TH2 on the P-Chip.
+    chamber_temperature:
+        Flow-cell chamber-temperature, calculated from the pixel-block
+        temperatures
+    pixel_block_temperature:
+        Temperature measured at each sensor in the ASIC, there are 12
+        sensors, one sensor per pixel-block
+"""
 # @@protoc_insertion_point(module_scope)
```

### Comparing `minknow_api-5.4.0/minknow_api/statistics_pb2_grpc.py` & `minknow_api-5.5.2/minknow_api/statistics_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,19 @@
                 response_deserializer=minknow__api_dot_statistics__pb2.StreamBiasVoltagesResponse.FromString,
                 )
         self.stream_read_length_histogram = channel.unary_stream(
                 '/minknow_api.statistics.StatisticsService/stream_read_length_histogram',
                 request_serializer=minknow__api_dot_statistics__pb2.StreamReadLengthHistogramRequest.SerializeToString,
                 response_deserializer=minknow__api_dot_statistics__pb2.StreamReadLengthHistogramResponse.FromString,
                 )
+        self.read_length_n50 = channel.unary_unary(
+                '/minknow_api.statistics.StatisticsService/read_length_n50',
+                request_serializer=minknow__api_dot_statistics__pb2.ReadLengthN50Request.SerializeToString,
+                response_deserializer=minknow__api_dot_statistics__pb2.ReadLengthN50Response.FromString,
+                )
         self.get_read_length_types = channel.unary_unary(
                 '/minknow_api.statistics.StatisticsService/get_read_length_types',
                 request_serializer=minknow__api_dot_statistics__pb2.GetReadLengthTypesRequest.SerializeToString,
                 response_deserializer=minknow__api_dot_statistics__pb2.GetReadLengthTypesResponse.FromString,
                 )
         self.stream_basecall_boxplots = channel.unary_stream(
                 '/minknow_api.statistics.StatisticsService/stream_basecall_boxplots',
@@ -147,14 +152,32 @@
 
         Since 4.0
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def read_length_n50(self, request, context):
+        """Read lengths N50 value
+
+        Derived from RPC stream_read_length_histogram
+        Returns the same N50 data as you'd get from the stream_read_length_histogram RPC
+
+        Returns N50 value for estimated bases data
+
+        If no basecalling, one value will return as 0.0 exactly
+
+        No filtering, discarded outliers, or split
+
+        Since 5.5
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def get_read_length_types(self, request, context):
         """Gets a list of the types of read-length values for which a histogram is available
 
         Since 3.2
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -218,14 +241,19 @@
                     response_serializer=minknow__api_dot_statistics__pb2.StreamBiasVoltagesResponse.SerializeToString,
             ),
             'stream_read_length_histogram': grpc.unary_stream_rpc_method_handler(
                     servicer.stream_read_length_histogram,
                     request_deserializer=minknow__api_dot_statistics__pb2.StreamReadLengthHistogramRequest.FromString,
                     response_serializer=minknow__api_dot_statistics__pb2.StreamReadLengthHistogramResponse.SerializeToString,
             ),
+            'read_length_n50': grpc.unary_unary_rpc_method_handler(
+                    servicer.read_length_n50,
+                    request_deserializer=minknow__api_dot_statistics__pb2.ReadLengthN50Request.FromString,
+                    response_serializer=minknow__api_dot_statistics__pb2.ReadLengthN50Response.SerializeToString,
+            ),
             'get_read_length_types': grpc.unary_unary_rpc_method_handler(
                     servicer.get_read_length_types,
                     request_deserializer=minknow__api_dot_statistics__pb2.GetReadLengthTypesRequest.FromString,
                     response_serializer=minknow__api_dot_statistics__pb2.GetReadLengthTypesResponse.SerializeToString,
             ),
             'stream_basecall_boxplots': grpc.unary_stream_rpc_method_handler(
                     servicer.stream_basecall_boxplots,
@@ -358,14 +386,31 @@
         return grpc.experimental.unary_stream(request, target, '/minknow_api.statistics.StatisticsService/stream_read_length_histogram',
             minknow__api_dot_statistics__pb2.StreamReadLengthHistogramRequest.SerializeToString,
             minknow__api_dot_statistics__pb2.StreamReadLengthHistogramResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def read_length_n50(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/minknow_api.statistics.StatisticsService/read_length_n50',
+            minknow__api_dot_statistics__pb2.ReadLengthN50Request.SerializeToString,
+            minknow__api_dot_statistics__pb2.ReadLengthN50Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def get_read_length_types(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `minknow_api-5.4.0/minknow_api/statistics_service.py` & `minknow_api-5.5.2/minknow_api/statistics_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     "DataSelection",
     "StreamDutyTimeRequest",
     "StreamDutyTimeResponse",
     "ReadLengthHistogramKey",
     "ReadLengthHistogramSplit",
     "StreamReadLengthHistogramRequest",
     "StreamReadLengthHistogramResponse",
+    "ReadLengthN50Request",
+    "ReadLengthN50Response",
     "GetReadLengthTypesRequest",
     "GetReadLengthTypesResponse",
     "AcquisitionOutputKey",
     "AcquisitionOutputSplit",
     "StreamAcquisitionOutputRequest",
     "AcquisitionOutputSnapshot",
     "StreamAcquisitionOutputResponse",
@@ -562,14 +564,70 @@
         if len(unused_args) > 0:
             raise ArgumentError("Unexpected keyword arguments to stream_read_length_histogram: '{}'".format(", ".join(unused_args)))
 
         return run_with_retry(self._stub.stream_read_length_histogram,
                               _message, _timeout,
                               [],
                               "minknow_api.statistics.StatisticsService")
+    def read_length_n50(self, _message=None, _timeout=None, **kwargs):
+        """Read lengths N50 value
+
+        Derived from RPC stream_read_length_histogram
+        Returns the same N50 data as you'd get from the stream_read_length_histogram RPC
+
+        Returns N50 value for estimated bases data
+
+        If no basecalling, one value will return as 0.0 exactly
+
+        No filtering, discarded outliers, or split
+
+        Since 5.5
+
+        This RPC has no side effects. Calling it will have no effect on the state of the
+        system. It is safe to call repeatedly, or to retry on failure, although there is no
+        guarantee it will return the same information each time.
+
+        Args:
+            _message (minknow_api.statistics_pb2.ReadLengthN50Request, optional): The message to send.
+                This can be passed instead of the keyword arguments.
+            _timeout (float, optional): The call will be cancelled after this number of seconds
+                if it has not been completed.
+            acquisition_run_id (str): The `acquisition_run_id` of the acquisition to obtain data for
+
+        Returns:
+            minknow_api.statistics_pb2.ReadLengthN50Response
+
+        Note that the returned messages are actually wrapped in a type that collapses
+        submessages for fields marked with ``[rpc_unwrap]``.
+        """
+        if _message is not None:
+            if isinstance(_message, MessageWrapper):
+                _message = _message._message
+            return run_with_retry(self._stub.read_length_n50,
+                                  _message, _timeout,
+                                  [],
+                                  "minknow_api.statistics.StatisticsService")
+
+        unused_args = set(kwargs.keys())
+
+        _message = ReadLengthN50Request()
+
+        if "acquisition_run_id" in kwargs:
+            unused_args.remove("acquisition_run_id")
+            _message.acquisition_run_id = kwargs['acquisition_run_id']
+        else:
+            raise ArgumentError("read_length_n50 requires a 'acquisition_run_id' argument")
+
+        if len(unused_args) > 0:
+            raise ArgumentError("Unexpected keyword arguments to read_length_n50: '{}'".format(", ".join(unused_args)))
+
+        return run_with_retry(self._stub.read_length_n50,
+                              _message, _timeout,
+                              [],
+                              "minknow_api.statistics.StatisticsService")
     def get_read_length_types(self, _message=None, _timeout=None, **kwargs):
         """Gets a list of the types of read-length values for which a histogram is available
 
         Since 3.2
 
         This RPC has no side effects. Calling it will have no effect on the state of the
         system. It is safe to call repeatedly, or to retry on failure, although there is no
```

### Comparing `minknow_api-5.4.0/minknow_api/testutils.py` & `minknow_api-5.5.2/minknow_api/testutils.py`

 * *Files identical despite different names*

### Comparing `minknow_api-5.4.0/minknow_api/tools/protocols.py` & `minknow_api-5.5.2/minknow_api/tools/protocols.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """Tools for interacting with protocols in minknow"""
 
 import collections
 import logging
-import typing
 
 import grpc
 
-from minknow_api import protocol_pb2
+import dataclasses
+from typing import Optional, List, Sequence
+from minknow_api import protocol_pb2, run_until_pb2, acquisition_pb2
 from minknow_api.protocol_pb2 import BarcodeUserData
+from minknow_api.tools.any_helpers import make_float_any, make_uint64_any
 
 from .. import Connection
 
 LOGGER = logging.getLogger(__name__)
 
 
 def find_protocol(
     device_connection: Connection,
     product_code: str,
     kit: str,
     basecalling: bool = False,
-    basecall_config: typing.Optional[str] = None,
+    basecall_config: Optional[str] = None,
     barcoding: bool = False,
-    barcoding_kits: typing.Optional[typing.List[str]] = None,
+    barcoding_kits: Optional[List[str]] = None,
     force_reload: bool = False,
     experiment_type: str = "sequencing",
-) -> typing.Optional[str]:
+) -> Optional[str]:
     """Find a protocol identifier.
 
     This will fetch a list of protocols from the device-instance, then search through the protocols
     for one that supports the flow-cell type (product code) and all the specified options. It
     returns the first protocol it finds that matches.
 
     Args:
@@ -157,14 +159,48 @@
 )
 AlignmentArgs = collections.namedtuple("AlignmentArgs", ["reference_files", "bed_file"])
 BasecallingArgs = collections.namedtuple(
     "BasecallingArgs", ["config", "barcoding", "alignment"]
 )
 OutputArgs = collections.namedtuple("OutputArgs", ["reads_per_file"])
 
+
+@dataclasses.dataclass
+class CriteriaValues:
+    """
+    Python representation of a `minknow_api.run_until.CriteriaValues` message
+
+    See the `Standard Run-Until Criteria` in `run_until.proto` for further descriptions of the fields
+    """
+
+    # Runtime, in seconds
+    runtime: Optional[int] = None
+    # Estimated bases, in bases
+    estimated_bases: Optional[int] = None
+    # Passed basecalled bases, in seconds
+    passed_basecalled_bases: Optional[int] = None
+    # Available pores
+    available_pores: Optional[float] = None
+
+    def as_protobuf(self):
+        criteria_dict = {}
+        if self.runtime is not None:
+            criteria_dict["runtime"] = make_uint64_any(self.runtime)
+        if self.estimated_bases is not None:
+            criteria_dict["estimated_bases"] = make_uint64_any(self.estimated_bases)
+        if self.passed_basecalled_bases is not None:
+            criteria_dict["passed_basecalled_bases"] = make_uint64_any(
+                self.passed_basecalled_bases
+            )
+        if self.available_pores is not None:
+            criteria_dict["available_pores"] = make_float_any(self.available_pores)
+
+        return run_until_pb2.CriteriaValues(criteria=criteria_dict)
+
+
 ReadUntilArgs = collections.namedtuple(
     "ReadUntilArgs",
     [
         # "enrich", or "deplete"
         "filter_type",
         # List of reference files to pass to guppy for read until (only one file supported at the moment).
         "reference_files",
@@ -175,32 +211,30 @@
         # Last channel for read until to operate on.
         "last_channel",
     ],
 )
 
 
 def make_protocol_arguments(
-    experiment_duration: float = 72,
     basecalling: BasecallingArgs = None,
     read_until: ReadUntilArgs = None,
     fastq_arguments: OutputArgs = None,
     fast5_arguments: OutputArgs = None,
     pod5_arguments: OutputArgs = None,
     bam_arguments: OutputArgs = None,
     disable_active_channel_selection: bool = False,
     mux_scan_period: float = 1.5,
-    args: typing.Optional[typing.List[str]] = None,
+    args: Optional[List[str]] = None,
     is_flongle: bool = False,
-) -> typing.List[str]:
+) -> List[str]:
     """Build arguments to be used when starting a protocol.
 
     This will assemble the arguments passed to this script into arguments to pass to the protocol.
 
     Args:
-        experiment_duration(float):             Length of the experiment in hours.
         basecalling(:obj:`BasecallingArgs`):    Arguments to control basecalling.
         read_until(:obj:`ReadUntilArgs):        Arguments to control read until.
         fastq_arguments(:obj:`OutputArgs`):     Control fastq file generation.
         fast5_arguments(:obj:`OutputArgs`):     Control fast5 file generation.
         pod5_arguments(:obj:`OutputArgs`):      Control pod5 file generation.
         bam_arguments(:obj:`OutputArgs`):       Control bam file generation.
         disable_active_channel_selection(bool): Disable active channel selection
@@ -308,15 +342,14 @@
         if read_until.last_channel:
             read_until_args.append("last_channel={}".format(read_until.last_channel))
 
         # --read_until filter_type='enrich' reference_files=['/data/my-alignment-file'] bed_file='/data/bed_file.bed' first_channel=1 last_channel=512
         print(read_until_args)
         protocol_args.extend(["--read_until"] + read_until_args)
 
-    protocol_args.append("--experiment_time={}".format(experiment_duration))
     protocol_args.append("--fast5=" + on_off(fast5_arguments))
     if fast5_arguments:
         protocol_args.extend(
             ["--fast5_data", "trace_table", "fastq", "raw", "vbz_compress"]
         )
         protocol_args.append(
             "--fast5_reads_per_file={}".format(fast5_arguments.reads_per_file)
@@ -351,37 +384,87 @@
             protocol_args.append("--mux_scan_period={}".format(mux_scan_period))
 
     protocol_args.extend(args)
 
     return protocol_args
 
 
+def make_target_run_until_criteria(
+    stop_criteria: Optional[CriteriaValues] = None,
+    experiment_duration: Optional[float] = None,
+) -> acquisition_pb2.TargetRunUntilCriteria:
+    """Make an `acquisition.TargetRunUntilCriteria` message based on the supplied parameters
+
+    If `stop_criteria` is supplied, then the `stop_criteria` in the returned message are set to match the supplied
+    criteria.  Otherwise, if `experiment_duration` is supplied, then the "runtime" stop criterion in the returned
+    message is set to match the supplied `experiment_duration`.
+
+    If no arguments are supplied, the returned message will be empty.  If both arguments are supplied, a `ValueError`
+    is raised, since only one or the other argument may be supplied
+
+    Args:
+        stop_criteria(:obj:`CriteriaValues`):   Stop criteria to set.
+        experiment_duration(float):             Length of the experiment in hours.
+
+    Returns:
+        An `acquisition.TargetRunUntilCriteria` message with the specified criteria
+    """
+
+    if stop_criteria and experiment_duration:
+        raise ValueError(
+            "Can specify `stop_criteria` or `experiment_duration` but not both"
+        )
+
+    if experiment_duration:
+        # Case of having both is handled above
+        assert not stop_criteria
+
+        # `experiment_duration` is in hours
+        # `runtime` is in seconds
+        stop_criteria = CriteriaValues(runtime=int(experiment_duration * 60 * 60))
+
+    if stop_criteria:
+        return acquisition_pb2.TargetRunUntilCriteria(
+            stop_criteria=stop_criteria.as_protobuf()
+        )
+    else:
+        # Empty target criteria
+        return acquisition_pb2.TargetRunUntilCriteria()
+
+
 def start_protocol(
     device_connection: Connection,
     identifier: str,
     sample_id: str,
     experiment_group: str,
-    barcode_info: typing.Optional[typing.Sequence[BarcodeUserData]],
+    barcode_info: Optional[Sequence[BarcodeUserData]],
+    stop_criteria: Optional[CriteriaValues] = None,
+    experiment_duration: Optional[float] = None,
     *args,
-    **kwargs
+    **kwargs,
 ) -> str:
     """Start a protocol on the passed {device_connection}.
 
     Args:
         device_connection(:obj:`Connection`):   The device connection to start a protocol on.
         identifier(str):                        Protocol identifier to be started.
         sample_id(str):                         Sample id of protocol to start.
         experiment_group(str):                  Experiment group of protocol to start.
         barcode_info(Sequence[:obj:`BarcodeUserData`]):
                 Barcode user data (sample type and alias)
+        stop_criteria(::obj::`TargetCriteria`): When to stop the acquisition
+        experiment_duration(float):             Length of the experiment in hours.
         *args: Additional arguments forwarded to {make_protocol_arguments}
         **kwargs: Additional arguments forwarded to {make_protocol_arguments}
 
     Returns:
         The protocol_run_id of the started protocol.
+
+    Notes:
+        Only one of `stop_criteria` and `experiment_duration` may be specified
     """
 
     flow_cell_info = device_connection.device.get_flow_cell_info()
 
     protocol_arguments = make_protocol_arguments(
         *args, is_flongle=flow_cell_info.has_adapter, **kwargs
     )
@@ -391,12 +474,21 @@
     if sample_id:
         user_info.sample_id.value = sample_id
     if experiment_group:
         user_info.protocol_group_id.value = experiment_group
     if barcode_info:
         user_info.barcode_user_info.extend(barcode_info)
 
+    # Run until criteria
+    target_run_until_criteria = make_target_run_until_criteria(
+        stop_criteria=stop_criteria,
+        experiment_duration=experiment_duration,
+    )
+
     result = device_connection.protocol.start_protocol(
-        identifier=identifier, args=protocol_arguments, user_info=user_info
+        identifier=identifier,
+        args=protocol_arguments,
+        user_info=user_info,
+        target_run_until_criteria=target_run_until_criteria,
     )
 
     return result.run_id
```

### Comparing `minknow_api-5.4.0/minknow_api.egg-info/PKG-INFO` & `minknow_api-5.5.2/minknow_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minknow-api
-Version: 5.4.0
+Version: 5.5.2
 Summary: MinKNOW RPC API bindings
 Home-page: https://github.com/nanoporetech/minknow_api
 Author: Oxford Nanopore Technologies PLC
 Author-email: info@nanoporetech.com
 Description-Content-Type: text/markdown
 
 ![.](docs/images/ONT_logo.png "Oxford Nanopore Technologies")
```

### Comparing `minknow_api-5.4.0/minknow_api.egg-info/SOURCES.txt` & `minknow_api-5.5.2/minknow_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,8 +67,9 @@
 minknow_api/examples/export_to_csv.py
 minknow_api/examples/extract_run_statistics.py
 minknow_api/examples/list_sequencing_positions.py
 minknow_api/examples/load_sample_sheet.py
 minknow_api/examples/run_after_protocol.py
 minknow_api/examples/start_protocol.py
 minknow_api/tools/__init__.py
+minknow_api/tools/any_helpers.py
 minknow_api/tools/protocols.py
```

### Comparing `minknow_api-5.4.0/setup.py` & `minknow_api-5.5.2/setup.py`

 * *Files identical despite different names*

