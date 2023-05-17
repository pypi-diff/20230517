# Comparing `tmp/voltha-protos-5.4.2.tar.gz` & `tmp/voltha-protos-5.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/voltha-protos-5.4.2.tar", last modified: Thu Mar 16 08:16:10 2023, max compression
+gzip compressed data, was "dist/voltha-protos-5.4.3.tar", last modified: Wed May 17 20:37:55 2023, max compression
```

## Comparing `voltha-protos-5.4.2.tar` & `voltha-protos-5.4.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/PKG-INFO
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     2885 2023-03-16 08:15:42.000000 voltha-protos-5.4.2/README.md
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1663 2023-03-16 08:15:42.000000 voltha-protos-5.4.2/setup.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/setup.cfg
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)       17 2023-03-16 08:15:42.000000 voltha-protos-5.4.2/MANIFEST.in
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/voltha_protos/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/ietf_interfaces_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19060 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/omci_alarm_db_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25293 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/inter_adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    64403 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/events_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19758 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/ext_config_pb2.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-03-16 08:15:42.000000 voltha-protos-5.4.2/python/voltha_protos/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    59478 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13326 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/logical_device_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/core_adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    48518 2023-03-16 08:16:04.000000 voltha-protos-5.4.2/python/voltha_protos/voltha_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/device_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   108159 2023-03-16 08:16:04.000000 voltha-protos-5.4.2/python/voltha_protos/voltha_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/omci_test_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4572 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/core_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/omci_mib_db_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4295 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/extensions_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16809 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/ietf_interfaces_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5050 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/omci_test_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/logical_device_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5344 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/onu_inter_adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/common_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:00.000000 voltha-protos-5.4.2/python/voltha_protos/adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   421230 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/openflow_13_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   106603 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/device_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/ext_config_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    49438 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/core_adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/inter_adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40916 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/core_services_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4707 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/health_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    96862 2023-03-16 08:16:04.000000 voltha-protos-5.4.2/python/voltha_protos/tech_profile_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4435 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/olt_inter_adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/core_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/events_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16961 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/common_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19653 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13096 2023-03-16 08:16:01.000000 voltha-protos-5.4.2/python/voltha_protos/core_services_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/openflow_13_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8405 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9978 2023-03-16 08:16:00.000000 voltha-protos-5.4.2/python/voltha_protos/adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   162370 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/extensions_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    50853 2023-03-16 08:16:04.000000 voltha-protos-5.4.2/python/voltha_protos/openolt_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2588 2023-03-16 08:16:02.000000 voltha-protos-5.4.2/python/voltha_protos/health_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18434 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/omci_mib_db_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11674 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   249696 2023-03-16 08:16:04.000000 voltha-protos-5.4.2/python/voltha_protos/openolt_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:04.000000 voltha-protos-5.4.2/python/voltha_protos/tech_profile_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-03-16 08:16:03.000000 voltha-protos-5.4.2/python/voltha_protos/omci_alarm_db_pb2_grpc.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/test/
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-03-16 08:15:42.000000 voltha-protos-5.4.2/python/test/__init__.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1007 2023-03-16 08:15:42.000000 voltha-protos-5.4.2/python/test/test_protos.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/voltha_protos.egg-info/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/voltha_protos.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/voltha_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2302 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/voltha_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       86 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/voltha_protos.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       19 2023-03-16 08:16:10.000000 voltha-protos-5.4.2/python/voltha_protos.egg-info/top_level.txt
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        6 2023-03-16 08:15:42.000000 voltha-protos-5.4.2/VERSION
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/PKG-INFO
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3151 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/README.md
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1663 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/setup.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/setup.cfg
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)       17 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/MANIFEST.in
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/ietf_interfaces_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19060 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_alarm_db_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25293 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/inter_adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    64403 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/events_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19758 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/ext_config_pb2.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/python/voltha_protos/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    59478 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13326 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/logical_device_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    48518 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/voltha_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/device_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   108159 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/voltha_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_test_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4572 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_mib_db_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4295 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/extensions_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16809 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/ietf_interfaces_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5050 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_test_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/logical_device_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5344 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/common_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   421230 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/openflow_13_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   106603 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/device_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/ext_config_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    49438 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/inter_adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40916 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_services_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4707 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/health_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    96862 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/tech_profile_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4435 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/events_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16961 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/common_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19653 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13096 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_services_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/openflow_13_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8405 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9978 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   162370 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/extensions_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52525 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/openolt_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2588 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/health_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18434 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_mib_db_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11674 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   247532 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/openolt_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/tech_profile_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_alarm_db_pb2_grpc.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/test/
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/python/test/__init__.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1007 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/python/test/test_protos.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2302 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       86 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       19 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/top_level.txt
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        6 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/VERSION
```

### Comparing `voltha-protos-5.4.2/PKG-INFO` & `voltha-protos-5.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: voltha-protos
-Version: 5.4.2
+Version: 5.4.3
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/gitweb?p=voltha-protos.git
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf voltha
```

### Comparing `voltha-protos-5.4.2/README.md` & `voltha-protos-5.4.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -99,7 +99,10 @@
 
 To use the libraries, import protos with the root path github.com/opencord/voltha-protos/v2/go/
 
 ## Testing
 
 `make test` will run tests for all languages.
 
+## Miscelaneous
+
+[setup.py](https://gerrit.opencord.org/plugins/gitiles/voltha-protos/+/refs/heads/master/setup.py) and [requirements.txt](https://gerrit.opencord.org/plugins/gitiles/voltha-protos/+/refs/heads/master/requirements.txt) versions must be kept in sync.
```

### Comparing `voltha-protos-5.4.2/setup.py` & `voltha-protos-5.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/omci_alarm_db_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/omci_alarm_db_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/inter_adapter_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/inter_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/events_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/events_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/ext_config_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/ext_config_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/__init__.py` & `voltha-protos-5.4.3/python/voltha_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/adapter_service_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/logical_device_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/logical_device_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/voltha_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/voltha_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/voltha_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/voltha_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/core_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/core_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/extensions_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/extensions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/ietf_interfaces_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/ietf_interfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/omci_test_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/omci_test_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/onu_inter_adapter_service_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/openflow_13_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/openflow_13_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/device_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/device_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/core_adapter_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/core_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/core_services_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/core_services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/health_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/health_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/tech_profile_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/tech_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/olt_inter_adapter_service_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/common_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/common_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/adapter_service_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/core_services_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/core_services_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/adapter_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/extensions_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/openolt_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/openolt_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,18 +163,23 @@
                 response_deserializer=voltha__protos_dot_openolt__pb2.OnuLogicalDistance.FromString,
                 )
         self.GetPonRxPower = channel.unary_unary(
                 '/openolt.Openolt/GetPonRxPower',
                 request_serializer=voltha__protos_dot_openolt__pb2.Onu.SerializeToString,
                 response_deserializer=voltha__protos_dot_openolt__pb2.PonRxPowerData.FromString,
                 )
-        self.GetObject = channel.unary_unary(
-                '/openolt.Openolt/GetObject',
-                request_serializer=voltha__protos_dot_openolt__pb2.ObjectDataRequest.SerializeToString,
-                response_deserializer=voltha__protos_dot_openolt__pb2.ObjectDataResponse.FromString,
+        self.GetOnuInfo = channel.unary_unary(
+                '/openolt.Openolt/GetOnuInfo',
+                request_serializer=voltha__protos_dot_openolt__pb2.Onu.SerializeToString,
+                response_deserializer=voltha__protos_dot_openolt__pb2.OnuInfo.FromString,
+                )
+        self.GetPonInterfaceInfo = channel.unary_unary(
+                '/openolt.Openolt/GetPonInterfaceInfo',
+                request_serializer=voltha__protos_dot_openolt__pb2.Interface.SerializeToString,
+                response_deserializer=voltha__protos_dot_openolt__pb2.PonIntfInfo.FromString,
                 )
 
 
 class OpenoltServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def DisableOlt(self, request, context):
@@ -353,18 +358,27 @@
 
     def GetPonRxPower(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetObject(self, request, context):
+    def GetOnuInfo(self, request, context):
         """
-        GetObjects gets takes in type of the object and request details as argument.
-        Returns the Object from the device.
+        GetOnuInfo takes Onu id, serialnumber, and pon interface as argument from the onu structure.
+        Returns the Onu info from the device.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetPonInterfaceInfo(self, request, context):
+        """
+        GetPonInterfaceInfo takes the pon intf id as argument.
+        Returns the pon interface information from the device.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_OpenoltServicer_to_server(servicer, server):
@@ -515,18 +529,23 @@
                     response_serializer=voltha__protos_dot_openolt__pb2.OnuLogicalDistance.SerializeToString,
             ),
             'GetPonRxPower': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPonRxPower,
                     request_deserializer=voltha__protos_dot_openolt__pb2.Onu.FromString,
                     response_serializer=voltha__protos_dot_openolt__pb2.PonRxPowerData.SerializeToString,
             ),
-            'GetObject': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetObject,
-                    request_deserializer=voltha__protos_dot_openolt__pb2.ObjectDataRequest.FromString,
-                    response_serializer=voltha__protos_dot_openolt__pb2.ObjectDataResponse.SerializeToString,
+            'GetOnuInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetOnuInfo,
+                    request_deserializer=voltha__protos_dot_openolt__pb2.Onu.FromString,
+                    response_serializer=voltha__protos_dot_openolt__pb2.OnuInfo.SerializeToString,
+            ),
+            'GetPonInterfaceInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPonInterfaceInfo,
+                    request_deserializer=voltha__protos_dot_openolt__pb2.Interface.FromString,
+                    response_serializer=voltha__protos_dot_openolt__pb2.PonIntfInfo.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'openolt.Openolt', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -1041,22 +1060,39 @@
         return grpc.experimental.unary_unary(request, target, '/openolt.Openolt/GetPonRxPower',
             voltha__protos_dot_openolt__pb2.Onu.SerializeToString,
             voltha__protos_dot_openolt__pb2.PonRxPowerData.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetObject(request,
+    def GetOnuInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/openolt.Openolt/GetOnuInfo',
+            voltha__protos_dot_openolt__pb2.Onu.SerializeToString,
+            voltha__protos_dot_openolt__pb2.OnuInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetPonInterfaceInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/openolt.Openolt/GetObject',
-            voltha__protos_dot_openolt__pb2.ObjectDataRequest.SerializeToString,
-            voltha__protos_dot_openolt__pb2.ObjectDataResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/openolt.Openolt/GetPonInterfaceInfo',
+            voltha__protos_dot_openolt__pb2.Interface.SerializeToString,
+            voltha__protos_dot_openolt__pb2.PonIntfInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `voltha-protos-5.4.2/python/voltha_protos/health_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/omci_mib_db_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/omci_mib_db_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py` & `voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos/openolt_pb2.py` & `voltha-protos-5.4.3/python/voltha_protos/openolt_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='voltha_protos/openolt.proto',
   package='openolt',
   syntax='proto3',
   serialized_options=b'\n\033org.opencord.voltha.openoltB\rVolthaOpenOLTZ/github.com/opencord/voltha-protos/v5/go/openolt',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1bvoltha_protos/openolt.proto\x12\x07openolt\x1a\x1cgoogle/api/annotations.proto\x1a voltha_protos/tech_profile.proto\x1a\x1evoltha_protos/ext_config.proto\x1a\x1evoltha_protos/extensions.proto\"\xe9\x03\n\nIndication\x12)\n\x07olt_ind\x18\x01 \x01(\x0b\x32\x16.openolt.OltIndicationH\x00\x12+\n\x08intf_ind\x18\x02 \x01(\x0b\x32\x17.openolt.IntfIndicationH\x00\x12\x34\n\rintf_oper_ind\x18\x03 \x01(\x0b\x32\x1b.openolt.IntfOperIndicationH\x00\x12\x32\n\x0conu_disc_ind\x18\x04 \x01(\x0b\x32\x1a.openolt.OnuDiscIndicationH\x00\x12)\n\x07onu_ind\x18\x05 \x01(\x0b\x32\x16.openolt.OnuIndicationH\x00\x12+\n\x08omci_ind\x18\x06 \x01(\x0b\x32\x17.openolt.OmciIndicationH\x00\x12,\n\x07pkt_ind\x18\x07 \x01(\x0b\x32\x19.openolt.PacketIndicationH\x00\x12-\n\nport_stats\x18\x08 \x01(\x0b\x32\x17.openolt.PortStatisticsH\x00\x12-\n\nflow_stats\x18\t \x01(\x0b\x32\x17.openolt.FlowStatisticsH\x00\x12-\n\talarm_ind\x18\n \x01(\x0b\x32\x18.openolt.AlarmIndicationH\x00\x42\x06\n\x04\x64\x61ta\"\xf5\n\n\x0f\x41larmIndication\x12)\n\x07los_ind\x18\x01 \x01(\x0b\x32\x16.openolt.LosIndicationH\x00\x12\x36\n\x0e\x64ying_gasp_ind\x18\x02 \x01(\x0b\x32\x1c.openolt.DyingGaspIndicationH\x00\x12\x34\n\ronu_alarm_ind\x18\x03 \x01(\x0b\x32\x1b.openolt.OnuAlarmIndicationH\x00\x12\x44\n\x14onu_startup_fail_ind\x18\x04 \x01(\x0b\x32$.openolt.OnuStartupFailureIndicationH\x00\x12\x45\n\x16onu_signal_degrade_ind\x18\x05 \x01(\x0b\x32#.openolt.OnuSignalDegradeIndicationH\x00\x12\x46\n\x17onu_drift_of_window_ind\x18\x06 \x01(\x0b\x32#.openolt.OnuDriftOfWindowIndicationH\x00\x12\x44\n\x11onu_loss_omci_ind\x18\x07 \x01(\x0b\x32\'.openolt.OnuLossOfOmciChannelIndicationH\x00\x12\x44\n\x14onu_signals_fail_ind\x18\x08 \x01(\x0b\x32$.openolt.OnuSignalsFailureIndicationH\x00\x12\x43\n\x0conu_tiwi_ind\x18\t \x01(\x0b\x32+.openolt.OnuTransmissionInterferenceWarningH\x00\x12J\n\x17onu_activation_fail_ind\x18\n \x01(\x0b\x32\'.openolt.OnuActivationFailureIndicationH\x00\x12I\n\x18onu_processing_error_ind\x18\x0b \x01(\x0b\x32%.openolt.OnuProcessingErrorIndicationH\x00\x12O\n\x19onu_loss_of_sync_fail_ind\x18\x0c \x01(\x0b\x32*.openolt.OnuLossOfKeySyncFailureIndicationH\x00\x12\x42\n\x15onu_itu_pon_stats_ind\x18\r \x01(\x0b\x32!.openolt.OnuItuPonStatsIndicationH\x00\x12Q\n\x1conu_deactivation_failure_ind\x18\x0e \x01(\x0b\x32).openolt.OnuDeactivationFailureIndicationH\x00\x12\x43\n\x15onu_remote_defect_ind\x18\x0f \x01(\x0b\x32\".openolt.OnuRemoteDefectIndicationH\x00\x12Y\n\x1conu_loss_gem_delineation_ind\x18\x10 \x01(\x0b\x32\x31.openolt.OnuLossOfGEMChannelDelineationIndicationH\x00\x12X\n onu_physical_equipment_error_ind\x18\x11 \x01(\x0b\x32,.openolt.OnuPhysicalEquipmentErrorIndicationH\x00\x12J\n\x13onu_loss_of_ack_ind\x18\x12 \x01(\x0b\x32+.openolt.OnuLossOfAcknowledgementIndicationH\x00\x12V\n\x1bonu_diff_reach_exceeded_ind\x18\x13 \x01(\x0b\x32/.openolt.OnuDifferentialReachExceededIndicationH\x00\x42\x06\n\x04\x64\x61ta\"#\n\rOltIndication\x12\x12\n\noper_state\x18\x01 \x01(\t\"5\n\x0eIntfIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x12\n\noper_state\x18\x02 \x01(\t\"R\n\x11OnuDiscIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12,\n\rserial_number\x18\x02 \x01(\x0b\x32\x15.openolt.SerialNumber\"\xd3\x03\n\rOnuIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x12\n\noper_state\x18\x03 \x01(\t\x12\x13\n\x0b\x61\x64min_state\x18\x05 \x01(\t\x12,\n\rserial_number\x18\x04 \x01(\x0b\x32\x15.openolt.SerialNumber\x12@\n\x0b\x66\x61il_reason\x18\x06 \x01(\x0e\x32+.openolt.OnuIndication.ActivationFailReason\"\x87\x02\n\x14\x41\x63tivationFailReason\x12#\n\x1fONU_ACTIVATION_FAIL_REASON_NONE\x10\x00\x12&\n\"ONU_ACTIVATION_FAIL_REASON_RANGING\x10\x01\x12\x36\n2ONU_ACTIVATION_FAIL_REASON_PASSWORD_AUTHENTICATION\x10\x02\x12\"\n\x1eONU_ACTIVATION_FAIL_REASON_LOS\x10\x03\x12!\n\x1dONU_ACTIVATION_FAIL_ONU_ALARM\x10\x04\x12#\n\x1fONU_ACTIVATION_FAIL_SWITCH_OVER\x10\x05\"\xb5\x03\n\x12IntfOperIndication\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07intf_id\x18\x02 \x01(\x07\x12\x12\n\noper_state\x18\x03 \x01(\t\x12\r\n\x05speed\x18\x04 \x01(\x07\x12\x12\n\ntechnology\x18\x05 \x01(\t\x12=\n\x06ranges\x18\x06 \x01(\x0b\x32-.openolt.IntfOperIndication.PONResourceRanges\x1a\x89\x02\n\x11PONResourceRanges\x12\x41\n\x05pools\x18\x03 \x03(\x0b\x32\x32.openolt.IntfOperIndication.PONResourceRanges.Pool\x1a\xb0\x01\n\x04Pool\x12I\n\x04type\x18\x01 \x01(\x0e\x32;.openolt.IntfOperIndication.PONResourceRanges.Pool.PoolType\x12\r\n\x05start\x18\x03 \x01(\x07\x12\x0b\n\x03\x65nd\x18\x04 \x01(\x07\"A\n\x08PoolType\x12\n\n\x06ONU_ID\x10\x00\x12\x0c\n\x08\x41LLOC_ID\x10\x01\x12\x0e\n\nGEMPORT_ID\x10\x02\x12\x0b\n\x07\x46LOW_ID\x10\x03\">\n\x0eOmciIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0b\n\x03pkt\x18\x03 \x01(\x0c\"\xa9\x01\n\x10PacketIndication\x12\x11\n\tintf_type\x18\x05 \x01(\t\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x08 \x01(\x07\x12\x0e\n\x06uni_id\x18\t \x01(\x07\x12\x12\n\ngemport_id\x18\x02 \x01(\x07\x12\x0f\n\x07\x66low_id\x18\x03 \x01(\x07\x12\x0f\n\x07port_no\x18\x06 \x01(\x07\x12\x0e\n\x06\x63ookie\x18\x07 \x01(\x06\x12\x0b\n\x03pkt\x18\x04 \x01(\x0c\"\x1c\n\tInterface\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\"(\n\tHeartbeat\x12\x1b\n\x13heartbeat_signature\x18\x01 \x01(\x07\"z\n\x03Onu\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12,\n\rserial_number\x18\x03 \x01(\x0b\x32\x15.openolt.SerialNumber\x12\x0b\n\x03pir\x18\x04 \x01(\x07\x12\x17\n\x0fomcc_encryption\x18\x05 \x01(\x08\"v\n\x12OnuLogicalDistance\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12!\n\x19logical_onu_distance_zero\x18\x03 \x01(\x07\x12\x1c\n\x14logical_onu_distance\x18\x04 \x01(\x07\"7\n\x07OmciMsg\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0b\n\x03pkt\x18\x03 \x01(\x0c\"^\n\tOnuPacket\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0f\n\x07port_no\x18\x04 \x01(\x07\x12\x12\n\ngemport_id\x18\x05 \x01(\x07\x12\x0b\n\x03pkt\x18\x03 \x01(\x0c\",\n\x0cUplinkPacket\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0b\n\x03pkt\x18\x02 \x01(\x0c\"\xee\x05\n\nDeviceInfo\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\r\n\x05model\x18\x02 \x01(\t\x12\x18\n\x10hardware_version\x18\x03 \x01(\t\x12\x18\n\x10\x66irmware_version\x18\x04 \x01(\t\x12\x11\n\tdevice_id\x18\x10 \x01(\t\x12\x1c\n\x14\x64\x65vice_serial_number\x18\x11 \x01(\t\x12\x1c\n\x14previously_connected\x18\x13 \x01(\x08\x12\x11\n\tpon_ports\x18\x0c \x01(\x07\x12\x38\n\x06ranges\x18\x0f \x03(\x0b\x32(.openolt.DeviceInfo.DeviceResourceRanges\x1a\xde\x03\n\x14\x44\x65viceResourceRanges\x12\x10\n\x08intf_ids\x18\x01 \x03(\x07\x12\x12\n\ntechnology\x18\x02 \x01(\t\x12<\n\x05pools\x18\x03 \x03(\x0b\x32-.openolt.DeviceInfo.DeviceResourceRanges.Pool\x1a\xe1\x02\n\x04Pool\x12\x44\n\x04type\x18\x01 \x01(\x0e\x32\x36.openolt.DeviceInfo.DeviceResourceRanges.Pool.PoolType\x12J\n\x07sharing\x18\x02 \x01(\x0e\x32\x39.openolt.DeviceInfo.DeviceResourceRanges.Pool.SharingType\x12\r\n\x05start\x18\x03 \x01(\x07\x12\x0b\n\x03\x65nd\x18\x04 \x01(\x07\"A\n\x08PoolType\x12\n\n\x06ONU_ID\x10\x00\x12\x0c\n\x08\x41LLOC_ID\x10\x01\x12\x0e\n\nGEMPORT_ID\x10\x02\x12\x0b\n\x07\x46LOW_ID\x10\x03\"h\n\x0bSharingType\x12\x16\n\x12\x44\x45\x44ICATED_PER_INTF\x10\x00\x12\x1f\n\x1bSHARED_BY_ALL_INTF_ALL_TECH\x10\x01\x12 \n\x1cSHARED_BY_ALL_INTF_SAME_TECH\x10\x02J\x04\x08\x05\x10\x0cJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\x8c\x02\n\nClassifier\x12\x0e\n\x06o_tpid\x18\x01 \x01(\x07\x12\r\n\x05o_vid\x18\x02 \x01(\x07\x12\x0e\n\x06i_tpid\x18\x03 \x01(\x07\x12\r\n\x05i_vid\x18\x04 \x01(\x07\x12\x0f\n\x07o_pbits\x18\x05 \x01(\x07\x12\x0f\n\x07i_pbits\x18\x06 \x01(\x07\x12\x10\n\x08\x65th_type\x18\x07 \x01(\x07\x12\x0f\n\x07\x64st_mac\x18\x08 \x01(\x0c\x12\x0f\n\x07src_mac\x18\t \x01(\x0c\x12\x10\n\x08ip_proto\x18\n \x01(\x07\x12\x0e\n\x06\x64st_ip\x18\x0b \x01(\x07\x12\x0e\n\x06src_ip\x18\x0c \x01(\x07\x12\x10\n\x08src_port\x18\r \x01(\x07\x12\x10\n\x08\x64st_port\x18\x0e \x01(\x07\x12\x14\n\x0cpkt_tag_type\x18\x0f \x01(\t\"\xf5\x01\n\tActionCmd\x12\x15\n\radd_outer_tag\x18\x01 \x01(\x08\x12\x18\n\x10remove_outer_tag\x18\x02 \x01(\x08\x12\x14\n\x0ctrap_to_host\x18\x03 \x01(\x08\x12\x1a\n\x12remark_outer_pbits\x18\x04 \x01(\x08\x12\x1a\n\x12remark_inner_pbits\x18\x05 \x01(\x08\x12\x15\n\radd_inner_tag\x18\x06 \x01(\x08\x12\x18\n\x10remove_inner_tag\x18\x07 \x01(\x08\x12\x1b\n\x13translate_inner_tag\x18\x08 \x01(\x08\x12\x1b\n\x13translate_outer_tag\x18\t \x01(\x08\"\x89\x01\n\x06\x41\x63tion\x12\x1f\n\x03\x63md\x18\x01 \x01(\x0b\x32\x12.openolt.ActionCmd\x12\r\n\x05o_vid\x18\x02 \x01(\x07\x12\x0f\n\x07o_pbits\x18\x03 \x01(\x07\x12\x0e\n\x06o_tpid\x18\x04 \x01(\x07\x12\r\n\x05i_vid\x18\x05 \x01(\x07\x12\x0f\n\x07i_pbits\x18\x06 \x01(\x07\x12\x0e\n\x06i_tpid\x18\x07 \x01(\x07\"\xdb\x04\n\x04\x46low\x12\x16\n\x0e\x61\x63\x63\x65ss_intf_id\x18\x01 \x01(\x0f\x12\x0e\n\x06onu_id\x18\x02 \x01(\x0f\x12\x0e\n\x06uni_id\x18\x0b \x01(\x0f\x12\x0f\n\x07\x66low_id\x18\x03 \x01(\x06\x12\x19\n\x11symmetric_flow_id\x18\x12 \x01(\x06\x12\x11\n\tflow_type\x18\x04 \x01(\t\x12\x10\n\x08\x61lloc_id\x18\n \x01(\x0f\x12\x17\n\x0fnetwork_intf_id\x18\x05 \x01(\x0f\x12\x12\n\ngemport_id\x18\x06 \x01(\x0f\x12\'\n\nclassifier\x18\x07 \x01(\x0b\x32\x13.openolt.Classifier\x12\x1f\n\x06\x61\x63tion\x18\x08 \x01(\x0b\x32\x0f.openolt.Action\x12\x10\n\x08priority\x18\t \x01(\x0f\x12\x0e\n\x06\x63ookie\x18\x0c \x01(\x06\x12\x0f\n\x07port_no\x18\r \x01(\x07\x12\x10\n\x08group_id\x18\x0e \x01(\x07\x12\x17\n\x0ftech_profile_id\x18\x0f \x01(\x07\x12\x16\n\x0ereplicate_flow\x18\x10 \x01(\x08\x12\x39\n\x0fpbit_to_gemport\x18\x11 \x03(\x0b\x32 .openolt.Flow.PbitToGemportEntry\x12\x37\n\x0egemport_to_aes\x18\x13 \x03(\x0b\x32\x1f.openolt.Flow.GemportToAesEntry\x1a\x34\n\x12PbitToGemportEntry\x12\x0b\n\x03key\x18\x01 \x01(\x07\x12\r\n\x05value\x18\x02 \x01(\x07:\x02\x38\x01\x1a\x33\n\x11GemportToAesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x07\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\":\n\x0cSerialNumber\x12\x11\n\tvendor_id\x18\x01 \x01(\x0c\x12\x17\n\x0fvendor_specific\x18\x02 \x01(\x0c\"\xc9\x07\n\x0ePortStatistics\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x10\n\x08rx_bytes\x18\x02 \x01(\x06\x12\x12\n\nrx_packets\x18\x03 \x01(\x06\x12\x18\n\x10rx_ucast_packets\x18\x04 \x01(\x06\x12\x18\n\x10rx_mcast_packets\x18\x05 \x01(\x06\x12\x18\n\x10rx_bcast_packets\x18\x06 \x01(\x06\x12\x18\n\x10rx_error_packets\x18\x07 \x01(\x06\x12\x11\n\trx_frames\x18\x11 \x01(\x06\x12\x14\n\x0crx_frames_64\x18\x12 \x01(\x06\x12\x18\n\x10rx_frames_65_127\x18\x13 \x01(\x06\x12\x19\n\x11rx_frames_128_255\x18\x14 \x01(\x06\x12\x19\n\x11rx_frames_256_511\x18\x15 \x01(\x06\x12\x1a\n\x12rx_frames_512_1023\x18\x16 \x01(\x06\x12\x1b\n\x13rx_frames_1024_1518\x18\x17 \x01(\x06\x12\x1b\n\x13rx_frames_1519_2047\x18\x18 \x01(\x06\x12\x1b\n\x13rx_frames_2048_4095\x18\x19 \x01(\x06\x12\x1b\n\x13rx_frames_4096_9216\x18\x1a \x01(\x06\x12\x1c\n\x14rx_frames_9217_16383\x18\x1b \x01(\x06\x12\x15\n\rrx_crc_errors\x18\x0e \x01(\x06\x12\x10\n\x08tx_bytes\x18\x08 \x01(\x06\x12\x12\n\ntx_packets\x18\t \x01(\x06\x12\x18\n\x10tx_ucast_packets\x18\n \x01(\x06\x12\x18\n\x10tx_mcast_packets\x18\x0b \x01(\x06\x12\x18\n\x10tx_bcast_packets\x18\x0c \x01(\x06\x12\x18\n\x10tx_error_packets\x18\r \x01(\x06\x12\x11\n\ttx_frames\x18\x1c \x01(\x06\x12\x14\n\x0ctx_frames_64\x18\x1d \x01(\x06\x12\x18\n\x10tx_frames_65_127\x18\x1e \x01(\x06\x12\x19\n\x11tx_frames_128_255\x18\x1f \x01(\x06\x12\x19\n\x11tx_frames_256_511\x18  \x01(\x06\x12\x1a\n\x12tx_frames_512_1023\x18! \x01(\x06\x12\x1b\n\x13tx_frames_1024_1518\x18\" \x01(\x06\x12\x1b\n\x13tx_frames_1519_2047\x18# \x01(\x06\x12\x1b\n\x13tx_frames_2048_4095\x18$ \x01(\x06\x12\x1b\n\x13tx_frames_4096_9216\x18% \x01(\x06\x12\x1c\n\x14tx_frames_9217_16383\x18& \x01(\x06\x12\x12\n\nbip_errors\x18\x0f \x01(\x06\x12\x11\n\ttimestamp\x18\x10 \x01(\x07\"\xf5\x04\n\rOnuStatistics\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x16\n\x0epositive_drift\x18\x03 \x01(\x06\x12\x16\n\x0enegative_drift\x18\x04 \x01(\x06\x12 \n\x18\x64\x65limiter_miss_detection\x18\x05 \x01(\x06\x12\x12\n\nbip_errors\x18\x06 \x01(\x06\x12\x11\n\tbip_units\x18\x07 \x01(\x06\x12\x1d\n\x15\x66\x65\x63_corrected_symbols\x18\x08 \x01(\x06\x12\x1f\n\x17\x66\x65\x63_codewords_corrected\x18\t \x01(\x06\x12#\n\x1b\x66\x65\x63_codewords_uncorrectable\x18\n \x01(\x06\x12\x15\n\rfec_codewords\x18\x0b \x01(\x06\x12\x1b\n\x13\x66\x65\x63_corrected_units\x18\x0c \x01(\x06\x12\x17\n\x0fxgem_key_errors\x18\r \x01(\x06\x12\x11\n\txgem_loss\x18\x0e \x01(\x06\x12\x17\n\x0frx_ploams_error\x18\x0f \x01(\x06\x12\x1a\n\x12rx_ploams_non_idle\x18\x10 \x01(\x06\x12\x0f\n\x07rx_omci\x18\x11 \x01(\x06\x12!\n\x19rx_omci_packets_crc_error\x18\x12 \x01(\x06\x12\x10\n\x08rx_bytes\x18\x13 \x01(\x06\x12\x12\n\nrx_packets\x18\x14 \x01(\x06\x12\x10\n\x08tx_bytes\x18\x15 \x01(\x06\x12\x12\n\ntx_packets\x18\x16 \x01(\x06\x12\x14\n\x0c\x62\x65r_reported\x18\x17 \x01(\x06\x12\x13\n\x0blcdg_errors\x18\x18 \x01(\x06\x12\x12\n\nrdi_errors\x18\x19 \x01(\x06\x12\x11\n\ttimestamp\x18\x1a \x01(\x07\"\x97\x01\n\x11GemPortStatistics\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x12\n\ngemport_id\x18\x02 \x01(\x07\x12\x12\n\nrx_packets\x18\x03 \x01(\x06\x12\x10\n\x08rx_bytes\x18\x04 \x01(\x06\x12\x12\n\ntx_packets\x18\x05 \x01(\x06\x12\x10\n\x08tx_bytes\x18\x06 \x01(\x06\x12\x11\n\ttimestamp\x18\x1a \x01(\x07\"\x80\x01\n\x0e\x46lowStatistics\x12\x0f\n\x07\x66low_id\x18\x01 \x01(\x07\x12\x10\n\x08rx_bytes\x18\x02 \x01(\x06\x12\x12\n\nrx_packets\x18\x03 \x01(\x06\x12\x10\n\x08tx_bytes\x18\x08 \x01(\x06\x12\x12\n\ntx_packets\x18\t \x01(\x06\x12\x11\n\ttimestamp\x18\x10 \x01(\x07\"0\n\rLosIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06status\x18\x02 \x01(\t\"F\n\x13\x44yingGaspIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"\xc1\x01\n\x12OnuAlarmIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x12\n\nlos_status\x18\x03 \x01(\t\x12\x12\n\nlob_status\x18\x04 \x01(\t\x12\x18\n\x10lopc_miss_status\x18\x05 \x01(\t\x12\x1d\n\x15lopc_mic_error_status\x18\x06 \x01(\t\x12\x13\n\x0blofi_status\x18\x07 \x01(\t\x12\x14\n\x0cloami_status\x18\x08 \x01(\t\"N\n\x1bOnuStartupFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"m\n\x1aOnuSignalDegradeIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x1e\n\x16inverse_bit_error_rate\x18\x04 \x01(\x07\"m\n\x1aOnuDriftOfWindowIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05\x64rift\x18\x04 \x01(\x07\x12\x0f\n\x07new_eqd\x18\x05 \x01(\x07\"Q\n\x1eOnuLossOfOmciChannelIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"n\n\x1bOnuSignalsFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x1e\n\x16inverse_bit_error_rate\x18\x04 \x01(\x07\"d\n\"OnuTransmissionInterferenceWarning\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05\x64rift\x18\x04 \x01(\x07\"V\n\x1eOnuActivationFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x13\n\x0b\x66\x61il_reason\x18\x03 \x01(\x07\"T\n!OnuLossOfKeySyncFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"=\n\x12RdiErrorIndication\x12\x17\n\x0frdi_error_count\x18\x01 \x01(\x06\x12\x0e\n\x06status\x18\x02 \x01(\t\"z\n\x18OnuItuPonStatsIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x34\n\rrdi_error_ind\x18\x03 \x01(\x0b\x32\x1b.openolt.RdiErrorIndicationH\x00\x42\x07\n\x05stats\"?\n\x1cOnuProcessingErrorIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\"S\n OnuDeactivationFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"P\n\x19OnuRemoteDefectIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x12\n\nrdi_errors\x18\x03 \x01(\x06\"w\n(OnuLossOfGEMChannelDelineationIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65lineation_errors\x18\x04 \x01(\x07\"V\n#OnuPhysicalEquipmentErrorIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"U\n\"OnuLossOfAcknowledgementIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"k\n&OnuDifferentialReachExceededIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x10\n\x08\x64istance\x18\x04 \x01(\x07\"\xc5\x01\n\x0bGroupMember\x12\x14\n\x0cinterface_id\x18\x01 \x01(\r\x12:\n\x0einterface_type\x18\x02 \x01(\x0e\x32\".openolt.GroupMember.InterfaceType\x12\x13\n\x0bgem_port_id\x18\x03 \x01(\r\x12\x10\n\x08priority\x18\x04 \x01(\r\"=\n\rInterfaceType\x12\x07\n\x03PON\x10\x00\x12\x10\n\x0c\x45PON_1G_PATH\x10\x01\x12\x11\n\rEPON_10G_PATH\x10\x02\"\xe3\x01\n\x05Group\x12\x10\n\x08group_id\x18\x01 \x01(\r\x12\x33\n\x07\x63ommand\x18\x02 \x01(\x0e\x32\".openolt.Group.GroupMembersCommand\x12%\n\x07members\x18\x03 \x03(\x0b\x32\x14.openolt.GroupMember\x12\x1f\n\x06\x61\x63tion\x18\x04 \x01(\x0b\x32\x0f.openolt.Action\"K\n\x13GroupMembersCommand\x12\x0f\n\x0b\x41\x44\x44_MEMBERS\x10\x00\x12\x12\n\x0eREMOVE_MEMBERS\x10\x01\x12\x0f\n\x0bSET_MEMBERS\x10\x02\"Q\n\nValueParam\x12\x19\n\x03onu\x18\x01 \x01(\x0b\x32\x0c.openolt.Onu\x12(\n\x05value\x18\x02 \x01(\x0e\x32\x19.extension.ValueType.Type\"\x90\x02\n\x0ePonRxPowerData\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x46\n\x0b\x66\x61il_reason\x18\x04 \x01(\x0e\x32\x31.openolt.PonRxPowerData.RssiMeasurementFailReason\x12\x19\n\x11rx_power_mean_dbm\x18\x05 \x01(\x01\"j\n\x19RssiMeasurementFailReason\x12\x14\n\x10\x46\x41IL_REASON_NONE\x10\x00\x12\x1c\n\x18\x46\x41IL_REASON_NO_DELIMITER\x10\x01\x12\x19\n\x15\x46\x41IL_REASON_NO_ACCESS\x10\x02\"\xd5\x01\n\rOnuObjectData\x12\x0e\n\x06onu_id\x18\x01 \x01(\x07\x12\x31\n\x05state\x18\x02 \x01(\x0e\x32\".openolt.OnuObjectData.OnuObjState\x12!\n\x04losi\x18\x03 \x01(\x0e\x32\x13.openolt.AlarmState\x12!\n\x04lofi\x18\x04 \x01(\x0e\x32\x13.openolt.AlarmState\";\n\x0bOnuObjState\x12\x12\n\x0eNOT_CONFIGURED\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0c\n\x08INACTIVE\x10\x02\"C\n\x0eIntfObjectData\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12 \n\x03los\x18\x02 \x01(\x0e\x32\x13.openolt.AlarmState\"\x84\x01\n\x12ObjectDataResponse\x12\x31\n\x0fonu_object_data\x18\x02 \x01(\x0b\x32\x16.openolt.OnuObjectDataH\x00\x12\x33\n\x10intf_object_data\x18\x03 \x01(\x0b\x32\x17.openolt.IntfObjectDataH\x00\x42\x06\n\x04\x64\x61ta\"s\n\x11ObjectDataRequest\x12\'\n\x0fonu_object_data\x18\x01 \x01(\x0b\x32\x0c.openolt.OnuH\x00\x12-\n\x0fint_object_data\x18\x02 \x01(\x0b\x32\x12.openolt.InterfaceH\x00\x42\x06\n\x04\x64\x61ta\"\x07\n\x05\x45mpty*\x1d\n\nAlarmState\x12\x07\n\x03OFF\x10\x00\x12\x06\n\x02ON\x10\x01\x32\xff\x14\n\x07Openolt\x12\x44\n\nDisableOlt\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0b/v1/Disable:\x01*\x12\x46\n\x0bReenableOlt\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v1/Reenable:\x01*\x12\x45\n\x0b\x41\x63tivateOnu\x12\x0c.openolt.Onu\x1a\x0e.openolt.Empty\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v1/EnableOnu:\x01*\x12H\n\rDeactivateOnu\x12\x0c.openolt.Onu\x1a\x0e.openolt.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/DisableOnu:\x01*\x12\x43\n\tDeleteOnu\x12\x0c.openolt.Onu\x1a\x0e.openolt.Empty\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v1/DeleteOnu:\x01*\x12I\n\nOmciMsgOut\x12\x10.openolt.OmciMsg\x1a\x0e.openolt.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/OmciMsgOut:\x01*\x12O\n\x0cOnuPacketOut\x12\x12.openolt.OnuPacket\x1a\x0e.openolt.Empty\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x10/v1/OnuPacketOut:\x01*\x12X\n\x0fUplinkPacketOut\x12\x15.openolt.UplinkPacket\x1a\x0e.openolt.Empty\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/v1/UplinkPacketOut:\x01*\x12@\n\x07\x46lowAdd\x12\r.openolt.Flow\x1a\x0e.openolt.Empty\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0b/v1/FlowAdd:\x01*\x12\x46\n\nFlowRemove\x12\r.openolt.Flow\x1a\x0e.openolt.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/FlowRemove:\x01*\x12S\n\x0eHeartbeatCheck\x12\x0e.openolt.Empty\x1a\x12.openolt.Heartbeat\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1/HeartbeatCheck:\x01*\x12M\n\x0b\x45nablePonIf\x12\x12.openolt.Interface\x1a\x0e.openolt.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/EnablePonIf:\x01*\x12O\n\x0c\x44isablePonIf\x12\x12.openolt.Interface\x1a\x0e.openolt.Empty\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x10/v1/DisablePonIf:\x01*\x12R\n\rGetDeviceInfo\x12\x0e.openolt.Empty\x1a\x13.openolt.DeviceInfo\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/v1/GetDeviceInfo:\x01*\x12?\n\x06Reboot\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\"\x15\x82\xd3\xe4\x93\x02\x0f\"\n/v1/Reboot:\x01*\x12U\n\x11\x43ollectStatistics\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\" \x82\xd3\xe4\x93\x02\x1a\"\x15/v1/CollectStatistics:\x01*\x12Y\n\x10GetOnuStatistics\x12\x0c.openolt.Onu\x1a\x16.openolt.OnuStatistics\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/v1/GetOnuStatistics:\x01*\x12k\n\x14GetGemPortStatistics\x12\x12.openolt.OnuPacket\x1a\x1a.openolt.GemPortStatistics\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/v1/GetGemPortStatistics:\x01*\x12r\n\x17\x43reateTrafficSchedulers\x12\x1f.tech_profile.TrafficSchedulers\x1a\x0e.openolt.Empty\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/CreateTrafficSchedulers:\x01*\x12r\n\x17RemoveTrafficSchedulers\x12\x1f.tech_profile.TrafficSchedulers\x1a\x0e.openolt.Empty\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/RemoveTrafficSchedulers:\x01*\x12\x66\n\x13\x43reateTrafficQueues\x12\x1b.tech_profile.TrafficQueues\x1a\x0e.openolt.Empty\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/v1/CreateTrafficQueues:\x01*\x12\x66\n\x13RemoveTrafficQueues\x12\x1b.tech_profile.TrafficQueues\x1a\x0e.openolt.Empty\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/v1/RemoveTrafficQueues:\x01*\x12;\n\x10\x45nableIndication\x12\x0e.openolt.Empty\x1a\x13.openolt.Indication\"\x00\x30\x01\x12]\n\x15PerformGroupOperation\x12\x0e.openolt.Group\x1a\x0e.openolt.Empty\"$\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/PerformGroupOperation:\x01*\x12I\n\x0b\x44\x65leteGroup\x12\x0e.openolt.Group\x1a\x0e.openolt.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/DeleteGroup:\x01*\x12W\n\x0bGetExtValue\x12\x13.openolt.ValueParam\x1a\x17.extension.ReturnValues\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/GetExtValue:\x01*\x12]\n\x11OnuItuPonAlarmSet\x12\x16.config.OnuItuPonAlarm\x1a\x0e.openolt.Empty\" \x82\xd3\xe4\x93\x02\x1a\"\x15/v1/OnuItuPonAlarmSet:\x01*\x12p\n\x19GetLogicalOnuDistanceZero\x12\x0c.openolt.Onu\x1a\x1b.openolt.OnuLogicalDistance\"(\x82\xd3\xe4\x93\x02\"\"\x1d/v1/GetLogicalOnuDistanceZero:\x01*\x12h\n\x15GetLogicalOnuDistance\x12\x0c.openolt.Onu\x1a\x1b.openolt.OnuLogicalDistance\"$\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/GetLogicalOnuDistance:\x01*\x12T\n\rGetPonRxPower\x12\x0c.openolt.Onu\x1a\x17.openolt.PonRxPowerData\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/v1/GetPonRxPower:\x01*\x12^\n\tGetObject\x12\x1a.openolt.ObjectDataRequest\x1a\x1b.openolt.ObjectDataResponse\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v1/GetObject:\x01*B]\n\x1borg.opencord.voltha.openoltB\rVolthaOpenOLTZ/github.com/opencord/voltha-protos/v5/go/openoltb\x06proto3'
+  serialized_pb=b'\n\x1bvoltha_protos/openolt.proto\x12\x07openolt\x1a\x1cgoogle/api/annotations.proto\x1a voltha_protos/tech_profile.proto\x1a\x1evoltha_protos/ext_config.proto\x1a\x1evoltha_protos/extensions.proto\"\xe9\x03\n\nIndication\x12)\n\x07olt_ind\x18\x01 \x01(\x0b\x32\x16.openolt.OltIndicationH\x00\x12+\n\x08intf_ind\x18\x02 \x01(\x0b\x32\x17.openolt.IntfIndicationH\x00\x12\x34\n\rintf_oper_ind\x18\x03 \x01(\x0b\x32\x1b.openolt.IntfOperIndicationH\x00\x12\x32\n\x0conu_disc_ind\x18\x04 \x01(\x0b\x32\x1a.openolt.OnuDiscIndicationH\x00\x12)\n\x07onu_ind\x18\x05 \x01(\x0b\x32\x16.openolt.OnuIndicationH\x00\x12+\n\x08omci_ind\x18\x06 \x01(\x0b\x32\x17.openolt.OmciIndicationH\x00\x12,\n\x07pkt_ind\x18\x07 \x01(\x0b\x32\x19.openolt.PacketIndicationH\x00\x12-\n\nport_stats\x18\x08 \x01(\x0b\x32\x17.openolt.PortStatisticsH\x00\x12-\n\nflow_stats\x18\t \x01(\x0b\x32\x17.openolt.FlowStatisticsH\x00\x12-\n\talarm_ind\x18\n \x01(\x0b\x32\x18.openolt.AlarmIndicationH\x00\x42\x06\n\x04\x64\x61ta\"\xf5\n\n\x0f\x41larmIndication\x12)\n\x07los_ind\x18\x01 \x01(\x0b\x32\x16.openolt.LosIndicationH\x00\x12\x36\n\x0e\x64ying_gasp_ind\x18\x02 \x01(\x0b\x32\x1c.openolt.DyingGaspIndicationH\x00\x12\x34\n\ronu_alarm_ind\x18\x03 \x01(\x0b\x32\x1b.openolt.OnuAlarmIndicationH\x00\x12\x44\n\x14onu_startup_fail_ind\x18\x04 \x01(\x0b\x32$.openolt.OnuStartupFailureIndicationH\x00\x12\x45\n\x16onu_signal_degrade_ind\x18\x05 \x01(\x0b\x32#.openolt.OnuSignalDegradeIndicationH\x00\x12\x46\n\x17onu_drift_of_window_ind\x18\x06 \x01(\x0b\x32#.openolt.OnuDriftOfWindowIndicationH\x00\x12\x44\n\x11onu_loss_omci_ind\x18\x07 \x01(\x0b\x32\'.openolt.OnuLossOfOmciChannelIndicationH\x00\x12\x44\n\x14onu_signals_fail_ind\x18\x08 \x01(\x0b\x32$.openolt.OnuSignalsFailureIndicationH\x00\x12\x43\n\x0conu_tiwi_ind\x18\t \x01(\x0b\x32+.openolt.OnuTransmissionInterferenceWarningH\x00\x12J\n\x17onu_activation_fail_ind\x18\n \x01(\x0b\x32\'.openolt.OnuActivationFailureIndicationH\x00\x12I\n\x18onu_processing_error_ind\x18\x0b \x01(\x0b\x32%.openolt.OnuProcessingErrorIndicationH\x00\x12O\n\x19onu_loss_of_sync_fail_ind\x18\x0c \x01(\x0b\x32*.openolt.OnuLossOfKeySyncFailureIndicationH\x00\x12\x42\n\x15onu_itu_pon_stats_ind\x18\r \x01(\x0b\x32!.openolt.OnuItuPonStatsIndicationH\x00\x12Q\n\x1conu_deactivation_failure_ind\x18\x0e \x01(\x0b\x32).openolt.OnuDeactivationFailureIndicationH\x00\x12\x43\n\x15onu_remote_defect_ind\x18\x0f \x01(\x0b\x32\".openolt.OnuRemoteDefectIndicationH\x00\x12Y\n\x1conu_loss_gem_delineation_ind\x18\x10 \x01(\x0b\x32\x31.openolt.OnuLossOfGEMChannelDelineationIndicationH\x00\x12X\n onu_physical_equipment_error_ind\x18\x11 \x01(\x0b\x32,.openolt.OnuPhysicalEquipmentErrorIndicationH\x00\x12J\n\x13onu_loss_of_ack_ind\x18\x12 \x01(\x0b\x32+.openolt.OnuLossOfAcknowledgementIndicationH\x00\x12V\n\x1bonu_diff_reach_exceeded_ind\x18\x13 \x01(\x0b\x32/.openolt.OnuDifferentialReachExceededIndicationH\x00\x42\x06\n\x04\x64\x61ta\"#\n\rOltIndication\x12\x12\n\noper_state\x18\x01 \x01(\t\"5\n\x0eIntfIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x12\n\noper_state\x18\x02 \x01(\t\"R\n\x11OnuDiscIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12,\n\rserial_number\x18\x02 \x01(\x0b\x32\x15.openolt.SerialNumber\"\xd3\x03\n\rOnuIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x12\n\noper_state\x18\x03 \x01(\t\x12\x13\n\x0b\x61\x64min_state\x18\x05 \x01(\t\x12,\n\rserial_number\x18\x04 \x01(\x0b\x32\x15.openolt.SerialNumber\x12@\n\x0b\x66\x61il_reason\x18\x06 \x01(\x0e\x32+.openolt.OnuIndication.ActivationFailReason\"\x87\x02\n\x14\x41\x63tivationFailReason\x12#\n\x1fONU_ACTIVATION_FAIL_REASON_NONE\x10\x00\x12&\n\"ONU_ACTIVATION_FAIL_REASON_RANGING\x10\x01\x12\x36\n2ONU_ACTIVATION_FAIL_REASON_PASSWORD_AUTHENTICATION\x10\x02\x12\"\n\x1eONU_ACTIVATION_FAIL_REASON_LOS\x10\x03\x12!\n\x1dONU_ACTIVATION_FAIL_ONU_ALARM\x10\x04\x12#\n\x1fONU_ACTIVATION_FAIL_SWITCH_OVER\x10\x05\"\xb5\x03\n\x12IntfOperIndication\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07intf_id\x18\x02 \x01(\x07\x12\x12\n\noper_state\x18\x03 \x01(\t\x12\r\n\x05speed\x18\x04 \x01(\x07\x12\x12\n\ntechnology\x18\x05 \x01(\t\x12=\n\x06ranges\x18\x06 \x01(\x0b\x32-.openolt.IntfOperIndication.PONResourceRanges\x1a\x89\x02\n\x11PONResourceRanges\x12\x41\n\x05pools\x18\x03 \x03(\x0b\x32\x32.openolt.IntfOperIndication.PONResourceRanges.Pool\x1a\xb0\x01\n\x04Pool\x12I\n\x04type\x18\x01 \x01(\x0e\x32;.openolt.IntfOperIndication.PONResourceRanges.Pool.PoolType\x12\r\n\x05start\x18\x03 \x01(\x07\x12\x0b\n\x03\x65nd\x18\x04 \x01(\x07\"A\n\x08PoolType\x12\n\n\x06ONU_ID\x10\x00\x12\x0c\n\x08\x41LLOC_ID\x10\x01\x12\x0e\n\nGEMPORT_ID\x10\x02\x12\x0b\n\x07\x46LOW_ID\x10\x03\">\n\x0eOmciIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0b\n\x03pkt\x18\x03 \x01(\x0c\"\xa9\x01\n\x10PacketIndication\x12\x11\n\tintf_type\x18\x05 \x01(\t\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x08 \x01(\x07\x12\x0e\n\x06uni_id\x18\t \x01(\x07\x12\x12\n\ngemport_id\x18\x02 \x01(\x07\x12\x0f\n\x07\x66low_id\x18\x03 \x01(\x07\x12\x0f\n\x07port_no\x18\x06 \x01(\x07\x12\x0e\n\x06\x63ookie\x18\x07 \x01(\x06\x12\x0b\n\x03pkt\x18\x04 \x01(\x0c\"\x1c\n\tInterface\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\"(\n\tHeartbeat\x12\x1b\n\x13heartbeat_signature\x18\x01 \x01(\x07\"z\n\x03Onu\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12,\n\rserial_number\x18\x03 \x01(\x0b\x32\x15.openolt.SerialNumber\x12\x0b\n\x03pir\x18\x04 \x01(\x07\x12\x17\n\x0fomcc_encryption\x18\x05 \x01(\x08\"v\n\x12OnuLogicalDistance\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12!\n\x19logical_onu_distance_zero\x18\x03 \x01(\x07\x12\x1c\n\x14logical_onu_distance\x18\x04 \x01(\x07\"7\n\x07OmciMsg\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0b\n\x03pkt\x18\x03 \x01(\x0c\"^\n\tOnuPacket\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0f\n\x07port_no\x18\x04 \x01(\x07\x12\x12\n\ngemport_id\x18\x05 \x01(\x07\x12\x0b\n\x03pkt\x18\x03 \x01(\x0c\",\n\x0cUplinkPacket\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0b\n\x03pkt\x18\x02 \x01(\x0c\"\xee\x05\n\nDeviceInfo\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\r\n\x05model\x18\x02 \x01(\t\x12\x18\n\x10hardware_version\x18\x03 \x01(\t\x12\x18\n\x10\x66irmware_version\x18\x04 \x01(\t\x12\x11\n\tdevice_id\x18\x10 \x01(\t\x12\x1c\n\x14\x64\x65vice_serial_number\x18\x11 \x01(\t\x12\x1c\n\x14previously_connected\x18\x13 \x01(\x08\x12\x11\n\tpon_ports\x18\x0c \x01(\x07\x12\x38\n\x06ranges\x18\x0f \x03(\x0b\x32(.openolt.DeviceInfo.DeviceResourceRanges\x1a\xde\x03\n\x14\x44\x65viceResourceRanges\x12\x10\n\x08intf_ids\x18\x01 \x03(\x07\x12\x12\n\ntechnology\x18\x02 \x01(\t\x12<\n\x05pools\x18\x03 \x03(\x0b\x32-.openolt.DeviceInfo.DeviceResourceRanges.Pool\x1a\xe1\x02\n\x04Pool\x12\x44\n\x04type\x18\x01 \x01(\x0e\x32\x36.openolt.DeviceInfo.DeviceResourceRanges.Pool.PoolType\x12J\n\x07sharing\x18\x02 \x01(\x0e\x32\x39.openolt.DeviceInfo.DeviceResourceRanges.Pool.SharingType\x12\r\n\x05start\x18\x03 \x01(\x07\x12\x0b\n\x03\x65nd\x18\x04 \x01(\x07\"A\n\x08PoolType\x12\n\n\x06ONU_ID\x10\x00\x12\x0c\n\x08\x41LLOC_ID\x10\x01\x12\x0e\n\nGEMPORT_ID\x10\x02\x12\x0b\n\x07\x46LOW_ID\x10\x03\"h\n\x0bSharingType\x12\x16\n\x12\x44\x45\x44ICATED_PER_INTF\x10\x00\x12\x1f\n\x1bSHARED_BY_ALL_INTF_ALL_TECH\x10\x01\x12 \n\x1cSHARED_BY_ALL_INTF_SAME_TECH\x10\x02J\x04\x08\x05\x10\x0cJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\x8c\x02\n\nClassifier\x12\x0e\n\x06o_tpid\x18\x01 \x01(\x07\x12\r\n\x05o_vid\x18\x02 \x01(\x07\x12\x0e\n\x06i_tpid\x18\x03 \x01(\x07\x12\r\n\x05i_vid\x18\x04 \x01(\x07\x12\x0f\n\x07o_pbits\x18\x05 \x01(\x07\x12\x0f\n\x07i_pbits\x18\x06 \x01(\x07\x12\x10\n\x08\x65th_type\x18\x07 \x01(\x07\x12\x0f\n\x07\x64st_mac\x18\x08 \x01(\x0c\x12\x0f\n\x07src_mac\x18\t \x01(\x0c\x12\x10\n\x08ip_proto\x18\n \x01(\x07\x12\x0e\n\x06\x64st_ip\x18\x0b \x01(\x07\x12\x0e\n\x06src_ip\x18\x0c \x01(\x07\x12\x10\n\x08src_port\x18\r \x01(\x07\x12\x10\n\x08\x64st_port\x18\x0e \x01(\x07\x12\x14\n\x0cpkt_tag_type\x18\x0f \x01(\t\"\xf5\x01\n\tActionCmd\x12\x15\n\radd_outer_tag\x18\x01 \x01(\x08\x12\x18\n\x10remove_outer_tag\x18\x02 \x01(\x08\x12\x14\n\x0ctrap_to_host\x18\x03 \x01(\x08\x12\x1a\n\x12remark_outer_pbits\x18\x04 \x01(\x08\x12\x1a\n\x12remark_inner_pbits\x18\x05 \x01(\x08\x12\x15\n\radd_inner_tag\x18\x06 \x01(\x08\x12\x18\n\x10remove_inner_tag\x18\x07 \x01(\x08\x12\x1b\n\x13translate_inner_tag\x18\x08 \x01(\x08\x12\x1b\n\x13translate_outer_tag\x18\t \x01(\x08\"\x89\x01\n\x06\x41\x63tion\x12\x1f\n\x03\x63md\x18\x01 \x01(\x0b\x32\x12.openolt.ActionCmd\x12\r\n\x05o_vid\x18\x02 \x01(\x07\x12\x0f\n\x07o_pbits\x18\x03 \x01(\x07\x12\x0e\n\x06o_tpid\x18\x04 \x01(\x07\x12\r\n\x05i_vid\x18\x05 \x01(\x07\x12\x0f\n\x07i_pbits\x18\x06 \x01(\x07\x12\x0e\n\x06i_tpid\x18\x07 \x01(\x07\"\xdb\x04\n\x04\x46low\x12\x16\n\x0e\x61\x63\x63\x65ss_intf_id\x18\x01 \x01(\x0f\x12\x0e\n\x06onu_id\x18\x02 \x01(\x0f\x12\x0e\n\x06uni_id\x18\x0b \x01(\x0f\x12\x0f\n\x07\x66low_id\x18\x03 \x01(\x06\x12\x19\n\x11symmetric_flow_id\x18\x12 \x01(\x06\x12\x11\n\tflow_type\x18\x04 \x01(\t\x12\x10\n\x08\x61lloc_id\x18\n \x01(\x0f\x12\x17\n\x0fnetwork_intf_id\x18\x05 \x01(\x0f\x12\x12\n\ngemport_id\x18\x06 \x01(\x0f\x12\'\n\nclassifier\x18\x07 \x01(\x0b\x32\x13.openolt.Classifier\x12\x1f\n\x06\x61\x63tion\x18\x08 \x01(\x0b\x32\x0f.openolt.Action\x12\x10\n\x08priority\x18\t \x01(\x0f\x12\x0e\n\x06\x63ookie\x18\x0c \x01(\x06\x12\x0f\n\x07port_no\x18\r \x01(\x07\x12\x10\n\x08group_id\x18\x0e \x01(\x07\x12\x17\n\x0ftech_profile_id\x18\x0f \x01(\x07\x12\x16\n\x0ereplicate_flow\x18\x10 \x01(\x08\x12\x39\n\x0fpbit_to_gemport\x18\x11 \x03(\x0b\x32 .openolt.Flow.PbitToGemportEntry\x12\x37\n\x0egemport_to_aes\x18\x13 \x03(\x0b\x32\x1f.openolt.Flow.GemportToAesEntry\x1a\x34\n\x12PbitToGemportEntry\x12\x0b\n\x03key\x18\x01 \x01(\x07\x12\r\n\x05value\x18\x02 \x01(\x07:\x02\x38\x01\x1a\x33\n\x11GemportToAesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x07\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\":\n\x0cSerialNumber\x12\x11\n\tvendor_id\x18\x01 \x01(\x0c\x12\x17\n\x0fvendor_specific\x18\x02 \x01(\x0c\"\xc9\x07\n\x0ePortStatistics\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x10\n\x08rx_bytes\x18\x02 \x01(\x06\x12\x12\n\nrx_packets\x18\x03 \x01(\x06\x12\x18\n\x10rx_ucast_packets\x18\x04 \x01(\x06\x12\x18\n\x10rx_mcast_packets\x18\x05 \x01(\x06\x12\x18\n\x10rx_bcast_packets\x18\x06 \x01(\x06\x12\x18\n\x10rx_error_packets\x18\x07 \x01(\x06\x12\x11\n\trx_frames\x18\x11 \x01(\x06\x12\x14\n\x0crx_frames_64\x18\x12 \x01(\x06\x12\x18\n\x10rx_frames_65_127\x18\x13 \x01(\x06\x12\x19\n\x11rx_frames_128_255\x18\x14 \x01(\x06\x12\x19\n\x11rx_frames_256_511\x18\x15 \x01(\x06\x12\x1a\n\x12rx_frames_512_1023\x18\x16 \x01(\x06\x12\x1b\n\x13rx_frames_1024_1518\x18\x17 \x01(\x06\x12\x1b\n\x13rx_frames_1519_2047\x18\x18 \x01(\x06\x12\x1b\n\x13rx_frames_2048_4095\x18\x19 \x01(\x06\x12\x1b\n\x13rx_frames_4096_9216\x18\x1a \x01(\x06\x12\x1c\n\x14rx_frames_9217_16383\x18\x1b \x01(\x06\x12\x15\n\rrx_crc_errors\x18\x0e \x01(\x06\x12\x10\n\x08tx_bytes\x18\x08 \x01(\x06\x12\x12\n\ntx_packets\x18\t \x01(\x06\x12\x18\n\x10tx_ucast_packets\x18\n \x01(\x06\x12\x18\n\x10tx_mcast_packets\x18\x0b \x01(\x06\x12\x18\n\x10tx_bcast_packets\x18\x0c \x01(\x06\x12\x18\n\x10tx_error_packets\x18\r \x01(\x06\x12\x11\n\ttx_frames\x18\x1c \x01(\x06\x12\x14\n\x0ctx_frames_64\x18\x1d \x01(\x06\x12\x18\n\x10tx_frames_65_127\x18\x1e \x01(\x06\x12\x19\n\x11tx_frames_128_255\x18\x1f \x01(\x06\x12\x19\n\x11tx_frames_256_511\x18  \x01(\x06\x12\x1a\n\x12tx_frames_512_1023\x18! \x01(\x06\x12\x1b\n\x13tx_frames_1024_1518\x18\" \x01(\x06\x12\x1b\n\x13tx_frames_1519_2047\x18# \x01(\x06\x12\x1b\n\x13tx_frames_2048_4095\x18$ \x01(\x06\x12\x1b\n\x13tx_frames_4096_9216\x18% \x01(\x06\x12\x1c\n\x14tx_frames_9217_16383\x18& \x01(\x06\x12\x12\n\nbip_errors\x18\x0f \x01(\x06\x12\x11\n\ttimestamp\x18\x10 \x01(\x07\"\xf5\x04\n\rOnuStatistics\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x16\n\x0epositive_drift\x18\x03 \x01(\x06\x12\x16\n\x0enegative_drift\x18\x04 \x01(\x06\x12 \n\x18\x64\x65limiter_miss_detection\x18\x05 \x01(\x06\x12\x12\n\nbip_errors\x18\x06 \x01(\x06\x12\x11\n\tbip_units\x18\x07 \x01(\x06\x12\x1d\n\x15\x66\x65\x63_corrected_symbols\x18\x08 \x01(\x06\x12\x1f\n\x17\x66\x65\x63_codewords_corrected\x18\t \x01(\x06\x12#\n\x1b\x66\x65\x63_codewords_uncorrectable\x18\n \x01(\x06\x12\x15\n\rfec_codewords\x18\x0b \x01(\x06\x12\x1b\n\x13\x66\x65\x63_corrected_units\x18\x0c \x01(\x06\x12\x17\n\x0fxgem_key_errors\x18\r \x01(\x06\x12\x11\n\txgem_loss\x18\x0e \x01(\x06\x12\x17\n\x0frx_ploams_error\x18\x0f \x01(\x06\x12\x1a\n\x12rx_ploams_non_idle\x18\x10 \x01(\x06\x12\x0f\n\x07rx_omci\x18\x11 \x01(\x06\x12!\n\x19rx_omci_packets_crc_error\x18\x12 \x01(\x06\x12\x10\n\x08rx_bytes\x18\x13 \x01(\x06\x12\x12\n\nrx_packets\x18\x14 \x01(\x06\x12\x10\n\x08tx_bytes\x18\x15 \x01(\x06\x12\x12\n\ntx_packets\x18\x16 \x01(\x06\x12\x14\n\x0c\x62\x65r_reported\x18\x17 \x01(\x06\x12\x13\n\x0blcdg_errors\x18\x18 \x01(\x06\x12\x12\n\nrdi_errors\x18\x19 \x01(\x06\x12\x11\n\ttimestamp\x18\x1a \x01(\x07\"\x97\x01\n\x11GemPortStatistics\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x12\n\ngemport_id\x18\x02 \x01(\x07\x12\x12\n\nrx_packets\x18\x03 \x01(\x06\x12\x10\n\x08rx_bytes\x18\x04 \x01(\x06\x12\x12\n\ntx_packets\x18\x05 \x01(\x06\x12\x10\n\x08tx_bytes\x18\x06 \x01(\x06\x12\x11\n\ttimestamp\x18\x1a \x01(\x07\"\x80\x01\n\x0e\x46lowStatistics\x12\x0f\n\x07\x66low_id\x18\x01 \x01(\x07\x12\x10\n\x08rx_bytes\x18\x02 \x01(\x06\x12\x12\n\nrx_packets\x18\x03 \x01(\x06\x12\x10\n\x08tx_bytes\x18\x08 \x01(\x06\x12\x12\n\ntx_packets\x18\t \x01(\x06\x12\x11\n\ttimestamp\x18\x10 \x01(\x07\"0\n\rLosIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06status\x18\x02 \x01(\t\"F\n\x13\x44yingGaspIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"\xc1\x01\n\x12OnuAlarmIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x12\n\nlos_status\x18\x03 \x01(\t\x12\x12\n\nlob_status\x18\x04 \x01(\t\x12\x18\n\x10lopc_miss_status\x18\x05 \x01(\t\x12\x1d\n\x15lopc_mic_error_status\x18\x06 \x01(\t\x12\x13\n\x0blofi_status\x18\x07 \x01(\t\x12\x14\n\x0cloami_status\x18\x08 \x01(\t\"N\n\x1bOnuStartupFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"m\n\x1aOnuSignalDegradeIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x1e\n\x16inverse_bit_error_rate\x18\x04 \x01(\x07\"m\n\x1aOnuDriftOfWindowIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05\x64rift\x18\x04 \x01(\x07\x12\x0f\n\x07new_eqd\x18\x05 \x01(\x07\"Q\n\x1eOnuLossOfOmciChannelIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"n\n\x1bOnuSignalsFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x1e\n\x16inverse_bit_error_rate\x18\x04 \x01(\x07\"d\n\"OnuTransmissionInterferenceWarning\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05\x64rift\x18\x04 \x01(\x07\"V\n\x1eOnuActivationFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x13\n\x0b\x66\x61il_reason\x18\x03 \x01(\x07\"T\n!OnuLossOfKeySyncFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"=\n\x12RdiErrorIndication\x12\x17\n\x0frdi_error_count\x18\x01 \x01(\x06\x12\x0e\n\x06status\x18\x02 \x01(\t\"z\n\x18OnuItuPonStatsIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x34\n\rrdi_error_ind\x18\x03 \x01(\x0b\x32\x1b.openolt.RdiErrorIndicationH\x00\x42\x07\n\x05stats\"?\n\x1cOnuProcessingErrorIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\"S\n OnuDeactivationFailureIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"P\n\x19OnuRemoteDefectIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x12\n\nrdi_errors\x18\x03 \x01(\x06\"w\n(OnuLossOfGEMChannelDelineationIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65lineation_errors\x18\x04 \x01(\x07\"V\n#OnuPhysicalEquipmentErrorIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"U\n\"OnuLossOfAcknowledgementIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\"k\n&OnuDifferentialReachExceededIndication\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x10\n\x08\x64istance\x18\x04 \x01(\x07\"\xc5\x01\n\x0bGroupMember\x12\x14\n\x0cinterface_id\x18\x01 \x01(\r\x12:\n\x0einterface_type\x18\x02 \x01(\x0e\x32\".openolt.GroupMember.InterfaceType\x12\x13\n\x0bgem_port_id\x18\x03 \x01(\r\x12\x10\n\x08priority\x18\x04 \x01(\r\"=\n\rInterfaceType\x12\x07\n\x03PON\x10\x00\x12\x10\n\x0c\x45PON_1G_PATH\x10\x01\x12\x11\n\rEPON_10G_PATH\x10\x02\"\xe3\x01\n\x05Group\x12\x10\n\x08group_id\x18\x01 \x01(\r\x12\x33\n\x07\x63ommand\x18\x02 \x01(\x0e\x32\".openolt.Group.GroupMembersCommand\x12%\n\x07members\x18\x03 \x03(\x0b\x32\x14.openolt.GroupMember\x12\x1f\n\x06\x61\x63tion\x18\x04 \x01(\x0b\x32\x0f.openolt.Action\"K\n\x13GroupMembersCommand\x12\x0f\n\x0b\x41\x44\x44_MEMBERS\x10\x00\x12\x12\n\x0eREMOVE_MEMBERS\x10\x01\x12\x0f\n\x0bSET_MEMBERS\x10\x02\"Q\n\nValueParam\x12\x19\n\x03onu\x18\x01 \x01(\x0b\x32\x0c.openolt.Onu\x12(\n\x05value\x18\x02 \x01(\x0e\x32\x19.extension.ValueType.Type\"\x90\x02\n\x0ePonRxPowerData\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x0e\n\x06onu_id\x18\x02 \x01(\x07\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x46\n\x0b\x66\x61il_reason\x18\x04 \x01(\x0e\x32\x31.openolt.PonRxPowerData.RssiMeasurementFailReason\x12\x19\n\x11rx_power_mean_dbm\x18\x05 \x01(\x01\"j\n\x19RssiMeasurementFailReason\x12\x14\n\x10\x46\x41IL_REASON_NONE\x10\x00\x12\x1c\n\x18\x46\x41IL_REASON_NO_DELIMITER\x10\x01\x12\x19\n\x15\x46\x41IL_REASON_NO_ACCESS\x10\x02\"\x82\x02\n\x07OnuInfo\x12\x0e\n\x06onu_id\x18\x01 \x01(\x07\x12(\n\x05state\x18\x02 \x01(\x0e\x32\x19.openolt.OnuInfo.OnuState\x12!\n\x04losi\x18\x03 \x01(\x0e\x32\x13.openolt.AlarmState\x12!\n\x04lofi\x18\x04 \x01(\x0e\x32\x13.openolt.AlarmState\x12\"\n\x05loami\x18\x05 \x01(\x0e\x32\x13.openolt.AlarmState\"S\n\x08OnuState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x12\n\x0eNOT_CONFIGURED\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08INACTIVE\x10\x03\x12\x0c\n\x08\x44ISABLED\x10\x04\"\xd3\x01\n\x0bPonIntfInfo\x12\x0f\n\x07intf_id\x18\x01 \x01(\x07\x12\x30\n\x05state\x18\x03 \x01(\x0e\x32!.openolt.PonIntfInfo.PonIntfState\x12 \n\x03los\x18\x04 \x01(\x0e\x32\x13.openolt.AlarmState\"_\n\x0cPonIntfState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x12\n\x0e\x41\x43TIVE_WORKING\x10\x01\x12\x12\n\x0e\x41\x43TIVE_STANDBY\x10\x02\x12\x0c\n\x08INACTIVE\x10\x03\x12\x0c\n\x08\x44ISABLED\x10\x04\"\x07\n\x05\x45mpty*\x1d\n\nAlarmState\x12\x07\n\x03OFF\x10\x00\x12\x06\n\x02ON\x10\x01\x32\xca\x15\n\x07Openolt\x12\x44\n\nDisableOlt\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0b/v1/Disable:\x01*\x12\x46\n\x0bReenableOlt\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v1/Reenable:\x01*\x12\x45\n\x0b\x41\x63tivateOnu\x12\x0c.openolt.Onu\x1a\x0e.openolt.Empty\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v1/EnableOnu:\x01*\x12H\n\rDeactivateOnu\x12\x0c.openolt.Onu\x1a\x0e.openolt.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/DisableOnu:\x01*\x12\x43\n\tDeleteOnu\x12\x0c.openolt.Onu\x1a\x0e.openolt.Empty\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/v1/DeleteOnu:\x01*\x12I\n\nOmciMsgOut\x12\x10.openolt.OmciMsg\x1a\x0e.openolt.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/OmciMsgOut:\x01*\x12O\n\x0cOnuPacketOut\x12\x12.openolt.OnuPacket\x1a\x0e.openolt.Empty\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x10/v1/OnuPacketOut:\x01*\x12X\n\x0fUplinkPacketOut\x12\x15.openolt.UplinkPacket\x1a\x0e.openolt.Empty\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/v1/UplinkPacketOut:\x01*\x12@\n\x07\x46lowAdd\x12\r.openolt.Flow\x1a\x0e.openolt.Empty\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0b/v1/FlowAdd:\x01*\x12\x46\n\nFlowRemove\x12\r.openolt.Flow\x1a\x0e.openolt.Empty\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/FlowRemove:\x01*\x12S\n\x0eHeartbeatCheck\x12\x0e.openolt.Empty\x1a\x12.openolt.Heartbeat\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1/HeartbeatCheck:\x01*\x12M\n\x0b\x45nablePonIf\x12\x12.openolt.Interface\x1a\x0e.openolt.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/EnablePonIf:\x01*\x12O\n\x0c\x44isablePonIf\x12\x12.openolt.Interface\x1a\x0e.openolt.Empty\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x10/v1/DisablePonIf:\x01*\x12R\n\rGetDeviceInfo\x12\x0e.openolt.Empty\x1a\x13.openolt.DeviceInfo\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/v1/GetDeviceInfo:\x01*\x12?\n\x06Reboot\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\"\x15\x82\xd3\xe4\x93\x02\x0f\"\n/v1/Reboot:\x01*\x12U\n\x11\x43ollectStatistics\x12\x0e.openolt.Empty\x1a\x0e.openolt.Empty\" \x82\xd3\xe4\x93\x02\x1a\"\x15/v1/CollectStatistics:\x01*\x12Y\n\x10GetOnuStatistics\x12\x0c.openolt.Onu\x1a\x16.openolt.OnuStatistics\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/v1/GetOnuStatistics:\x01*\x12k\n\x14GetGemPortStatistics\x12\x12.openolt.OnuPacket\x1a\x1a.openolt.GemPortStatistics\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/v1/GetGemPortStatistics:\x01*\x12r\n\x17\x43reateTrafficSchedulers\x12\x1f.tech_profile.TrafficSchedulers\x1a\x0e.openolt.Empty\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/CreateTrafficSchedulers:\x01*\x12r\n\x17RemoveTrafficSchedulers\x12\x1f.tech_profile.TrafficSchedulers\x1a\x0e.openolt.Empty\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/RemoveTrafficSchedulers:\x01*\x12\x66\n\x13\x43reateTrafficQueues\x12\x1b.tech_profile.TrafficQueues\x1a\x0e.openolt.Empty\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/v1/CreateTrafficQueues:\x01*\x12\x66\n\x13RemoveTrafficQueues\x12\x1b.tech_profile.TrafficQueues\x1a\x0e.openolt.Empty\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/v1/RemoveTrafficQueues:\x01*\x12;\n\x10\x45nableIndication\x12\x0e.openolt.Empty\x1a\x13.openolt.Indication\"\x00\x30\x01\x12]\n\x15PerformGroupOperation\x12\x0e.openolt.Group\x1a\x0e.openolt.Empty\"$\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/PerformGroupOperation:\x01*\x12I\n\x0b\x44\x65leteGroup\x12\x0e.openolt.Group\x1a\x0e.openolt.Empty\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/DeleteGroup:\x01*\x12W\n\x0bGetExtValue\x12\x13.openolt.ValueParam\x1a\x17.extension.ReturnValues\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/GetExtValue:\x01*\x12]\n\x11OnuItuPonAlarmSet\x12\x16.config.OnuItuPonAlarm\x1a\x0e.openolt.Empty\" \x82\xd3\xe4\x93\x02\x1a\"\x15/v1/OnuItuPonAlarmSet:\x01*\x12p\n\x19GetLogicalOnuDistanceZero\x12\x0c.openolt.Onu\x1a\x1b.openolt.OnuLogicalDistance\"(\x82\xd3\xe4\x93\x02\"\"\x1d/v1/GetLogicalOnuDistanceZero:\x01*\x12h\n\x15GetLogicalOnuDistance\x12\x0c.openolt.Onu\x1a\x1b.openolt.OnuLogicalDistance\"$\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/GetLogicalOnuDistance:\x01*\x12T\n\rGetPonRxPower\x12\x0c.openolt.Onu\x1a\x17.openolt.PonRxPowerData\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/v1/GetPonRxPower:\x01*\x12G\n\nGetOnuInfo\x12\x0c.openolt.Onu\x1a\x10.openolt.OnuInfo\"\x19\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/GetOnuInfo:\x01*\x12`\n\x13GetPonInterfaceInfo\x12\x12.openolt.Interface\x1a\x14.openolt.PonIntfInfo\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/v1/GetInterfaceInfo:\x01*B]\n\x1borg.opencord.voltha.openoltB\rVolthaOpenOLTZ/github.com/opencord/voltha-protos/v5/go/openoltb\x06proto3'
   ,
   dependencies=[google_dot_api_dot_annotations__pb2.DESCRIPTOR,voltha__protos_dot_tech__profile__pb2.DESCRIPTOR,voltha__protos_dot_ext__config__pb2.DESCRIPTOR,voltha__protos_dot_extensions__pb2.DESCRIPTOR,])
 
 _ALARMSTATE = _descriptor.EnumDescriptor(
   name='AlarmState',
   full_name='openolt.AlarmState',
   filename=None,
@@ -44,16 +44,16 @@
       name='ON', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=11113,
-  serialized_end=11142,
+  serialized_start=11051,
+  serialized_end=11080,
 )
 _sym_db.RegisterEnumDescriptor(_ALARMSTATE)
 
 AlarmState = enum_type_wrapper.EnumTypeWrapper(_ALARMSTATE)
 OFF = 0
 ON = 1
 
@@ -289,43 +289,93 @@
   containing_type=None,
   serialized_options=None,
   serialized_start=10459,
   serialized_end=10565,
 )
 _sym_db.RegisterEnumDescriptor(_PONRXPOWERDATA_RSSIMEASUREMENTFAILREASON)
 
-_ONUOBJECTDATA_ONUOBJSTATE = _descriptor.EnumDescriptor(
-  name='OnuObjState',
-  full_name='openolt.OnuObjectData.OnuObjState',
+_ONUINFO_ONUSTATE = _descriptor.EnumDescriptor(
+  name='OnuState',
+  full_name='openolt.OnuInfo.OnuState',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='NOT_CONFIGURED', index=0, number=0,
+      name='UNKNOWN', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='ACTIVE', index=1, number=1,
+      name='NOT_CONFIGURED', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='INACTIVE', index=2, number=2,
+      name='ACTIVE', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='INACTIVE', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DISABLED', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=10743,
+  serialized_end=10826,
+)
+_sym_db.RegisterEnumDescriptor(_ONUINFO_ONUSTATE)
+
+_PONINTFINFO_PONINTFSTATE = _descriptor.EnumDescriptor(
+  name='PonIntfState',
+  full_name='openolt.PonIntfInfo.PonIntfState',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='UNKNOWN', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='ACTIVE_WORKING', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='ACTIVE_STANDBY', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='INACTIVE', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DISABLED', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=10722,
-  serialized_end=10781,
+  serialized_start=10945,
+  serialized_end=11040,
 )
-_sym_db.RegisterEnumDescriptor(_ONUOBJECTDATA_ONUOBJSTATE)
+_sym_db.RegisterEnumDescriptor(_PONINTFINFO_PONINTFSTATE)
 
 
 _INDICATION = _descriptor.Descriptor(
   name='Indication',
   full_name='openolt.Indication',
   filename=None,
   file=DESCRIPTOR,
@@ -3948,192 +3998,119 @@
   oneofs=[
   ],
   serialized_start=10293,
   serialized_end=10565,
 )
 
 
-_ONUOBJECTDATA = _descriptor.Descriptor(
-  name='OnuObjectData',
-  full_name='openolt.OnuObjectData',
+_ONUINFO = _descriptor.Descriptor(
+  name='OnuInfo',
+  full_name='openolt.OnuInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='onu_id', full_name='openolt.OnuObjectData.onu_id', index=0,
+      name='onu_id', full_name='openolt.OnuInfo.onu_id', index=0,
       number=1, type=7, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='state', full_name='openolt.OnuObjectData.state', index=1,
+      name='state', full_name='openolt.OnuInfo.state', index=1,
       number=2, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='losi', full_name='openolt.OnuObjectData.losi', index=2,
+      name='losi', full_name='openolt.OnuInfo.losi', index=2,
       number=3, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='lofi', full_name='openolt.OnuObjectData.lofi', index=3,
+      name='lofi', full_name='openolt.OnuInfo.lofi', index=3,
       number=4, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-    _ONUOBJECTDATA_ONUOBJSTATE,
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=10568,
-  serialized_end=10781,
-)
-
-
-_INTFOBJECTDATA = _descriptor.Descriptor(
-  name='IntfObjectData',
-  full_name='openolt.IntfObjectData',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='intf_id', full_name='openolt.IntfObjectData.intf_id', index=0,
-      number=1, type=7, cpp_type=3, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='los', full_name='openolt.IntfObjectData.los', index=1,
-      number=2, type=14, cpp_type=8, label=1,
+      name='loami', full_name='openolt.OnuInfo.loami', index=4,
+      number=5, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
+    _ONUINFO_ONUSTATE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10783,
-  serialized_end=10850,
+  serialized_start=10568,
+  serialized_end=10826,
 )
 
 
-_OBJECTDATARESPONSE = _descriptor.Descriptor(
-  name='ObjectDataResponse',
-  full_name='openolt.ObjectDataResponse',
+_PONINTFINFO = _descriptor.Descriptor(
+  name='PonIntfInfo',
+  full_name='openolt.PonIntfInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='onu_object_data', full_name='openolt.ObjectDataResponse.onu_object_data', index=0,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='intf_object_data', full_name='openolt.ObjectDataResponse.intf_object_data', index=1,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='intf_id', full_name='openolt.PonIntfInfo.intf_id', index=0,
+      number=1, type=7, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-    _descriptor.OneofDescriptor(
-      name='data', full_name='openolt.ObjectDataResponse.data',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-  ],
-  serialized_start=10853,
-  serialized_end=10985,
-)
-
-
-_OBJECTDATAREQUEST = _descriptor.Descriptor(
-  name='ObjectDataRequest',
-  full_name='openolt.ObjectDataRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='onu_object_data', full_name='openolt.ObjectDataRequest.onu_object_data', index=0,
-      number=1, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='state', full_name='openolt.PonIntfInfo.state', index=1,
+      number=3, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='int_object_data', full_name='openolt.ObjectDataRequest.int_object_data', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='los', full_name='openolt.PonIntfInfo.los', index=2,
+      number=4, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
+    _PONINTFINFO_PONINTFSTATE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
-    _descriptor.OneofDescriptor(
-      name='data', full_name='openolt.ObjectDataRequest.data',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
   ],
-  serialized_start=10987,
-  serialized_end=11102,
+  serialized_start=10829,
+  serialized_end=11040,
 )
 
 
 _EMPTY = _descriptor.Descriptor(
   name='Empty',
   full_name='openolt.Empty',
   filename=None,
@@ -4149,16 +4126,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11104,
-  serialized_end=11111,
+  serialized_start=11042,
+  serialized_end=11049,
 )
 
 _INDICATION.fields_by_name['olt_ind'].message_type = _OLTINDICATION
 _INDICATION.fields_by_name['intf_ind'].message_type = _INTFINDICATION
 _INDICATION.fields_by_name['intf_oper_ind'].message_type = _INTFOPERINDICATION
 _INDICATION.fields_by_name['onu_disc_ind'].message_type = _ONUDISCINDICATION
 _INDICATION.fields_by_name['onu_ind'].message_type = _ONUINDICATION
@@ -4309,35 +4286,22 @@
 _GROUP.fields_by_name['members'].message_type = _GROUPMEMBER
 _GROUP.fields_by_name['action'].message_type = _ACTION
 _GROUP_GROUPMEMBERSCOMMAND.containing_type = _GROUP
 _VALUEPARAM.fields_by_name['onu'].message_type = _ONU
 _VALUEPARAM.fields_by_name['value'].enum_type = voltha__protos_dot_extensions__pb2._VALUETYPE_TYPE
 _PONRXPOWERDATA.fields_by_name['fail_reason'].enum_type = _PONRXPOWERDATA_RSSIMEASUREMENTFAILREASON
 _PONRXPOWERDATA_RSSIMEASUREMENTFAILREASON.containing_type = _PONRXPOWERDATA
-_ONUOBJECTDATA.fields_by_name['state'].enum_type = _ONUOBJECTDATA_ONUOBJSTATE
-_ONUOBJECTDATA.fields_by_name['losi'].enum_type = _ALARMSTATE
-_ONUOBJECTDATA.fields_by_name['lofi'].enum_type = _ALARMSTATE
-_ONUOBJECTDATA_ONUOBJSTATE.containing_type = _ONUOBJECTDATA
-_INTFOBJECTDATA.fields_by_name['los'].enum_type = _ALARMSTATE
-_OBJECTDATARESPONSE.fields_by_name['onu_object_data'].message_type = _ONUOBJECTDATA
-_OBJECTDATARESPONSE.fields_by_name['intf_object_data'].message_type = _INTFOBJECTDATA
-_OBJECTDATARESPONSE.oneofs_by_name['data'].fields.append(
-  _OBJECTDATARESPONSE.fields_by_name['onu_object_data'])
-_OBJECTDATARESPONSE.fields_by_name['onu_object_data'].containing_oneof = _OBJECTDATARESPONSE.oneofs_by_name['data']
-_OBJECTDATARESPONSE.oneofs_by_name['data'].fields.append(
-  _OBJECTDATARESPONSE.fields_by_name['intf_object_data'])
-_OBJECTDATARESPONSE.fields_by_name['intf_object_data'].containing_oneof = _OBJECTDATARESPONSE.oneofs_by_name['data']
-_OBJECTDATAREQUEST.fields_by_name['onu_object_data'].message_type = _ONU
-_OBJECTDATAREQUEST.fields_by_name['int_object_data'].message_type = _INTERFACE
-_OBJECTDATAREQUEST.oneofs_by_name['data'].fields.append(
-  _OBJECTDATAREQUEST.fields_by_name['onu_object_data'])
-_OBJECTDATAREQUEST.fields_by_name['onu_object_data'].containing_oneof = _OBJECTDATAREQUEST.oneofs_by_name['data']
-_OBJECTDATAREQUEST.oneofs_by_name['data'].fields.append(
-  _OBJECTDATAREQUEST.fields_by_name['int_object_data'])
-_OBJECTDATAREQUEST.fields_by_name['int_object_data'].containing_oneof = _OBJECTDATAREQUEST.oneofs_by_name['data']
+_ONUINFO.fields_by_name['state'].enum_type = _ONUINFO_ONUSTATE
+_ONUINFO.fields_by_name['losi'].enum_type = _ALARMSTATE
+_ONUINFO.fields_by_name['lofi'].enum_type = _ALARMSTATE
+_ONUINFO.fields_by_name['loami'].enum_type = _ALARMSTATE
+_ONUINFO_ONUSTATE.containing_type = _ONUINFO
+_PONINTFINFO.fields_by_name['state'].enum_type = _PONINTFINFO_PONINTFSTATE
+_PONINTFINFO.fields_by_name['los'].enum_type = _ALARMSTATE
+_PONINTFINFO_PONINTFSTATE.containing_type = _PONINTFINFO
 DESCRIPTOR.message_types_by_name['Indication'] = _INDICATION
 DESCRIPTOR.message_types_by_name['AlarmIndication'] = _ALARMINDICATION
 DESCRIPTOR.message_types_by_name['OltIndication'] = _OLTINDICATION
 DESCRIPTOR.message_types_by_name['IntfIndication'] = _INTFINDICATION
 DESCRIPTOR.message_types_by_name['OnuDiscIndication'] = _ONUDISCINDICATION
 DESCRIPTOR.message_types_by_name['OnuIndication'] = _ONUINDICATION
 DESCRIPTOR.message_types_by_name['IntfOperIndication'] = _INTFOPERINDICATION
@@ -4380,18 +4344,16 @@
 DESCRIPTOR.message_types_by_name['OnuPhysicalEquipmentErrorIndication'] = _ONUPHYSICALEQUIPMENTERRORINDICATION
 DESCRIPTOR.message_types_by_name['OnuLossOfAcknowledgementIndication'] = _ONULOSSOFACKNOWLEDGEMENTINDICATION
 DESCRIPTOR.message_types_by_name['OnuDifferentialReachExceededIndication'] = _ONUDIFFERENTIALREACHEXCEEDEDINDICATION
 DESCRIPTOR.message_types_by_name['GroupMember'] = _GROUPMEMBER
 DESCRIPTOR.message_types_by_name['Group'] = _GROUP
 DESCRIPTOR.message_types_by_name['ValueParam'] = _VALUEPARAM
 DESCRIPTOR.message_types_by_name['PonRxPowerData'] = _PONRXPOWERDATA
-DESCRIPTOR.message_types_by_name['OnuObjectData'] = _ONUOBJECTDATA
-DESCRIPTOR.message_types_by_name['IntfObjectData'] = _INTFOBJECTDATA
-DESCRIPTOR.message_types_by_name['ObjectDataResponse'] = _OBJECTDATARESPONSE
-DESCRIPTOR.message_types_by_name['ObjectDataRequest'] = _OBJECTDATAREQUEST
+DESCRIPTOR.message_types_by_name['OnuInfo'] = _ONUINFO
+DESCRIPTOR.message_types_by_name['PonIntfInfo'] = _PONINTFINFO
 DESCRIPTOR.message_types_by_name['Empty'] = _EMPTY
 DESCRIPTOR.enum_types_by_name['AlarmState'] = _ALARMSTATE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Indication = _reflection.GeneratedProtocolMessageType('Indication', (_message.Message,), {
   'DESCRIPTOR' : _INDICATION,
   '__module__' : 'voltha_protos.openolt_pb2'
@@ -4786,41 +4748,27 @@
 PonRxPowerData = _reflection.GeneratedProtocolMessageType('PonRxPowerData', (_message.Message,), {
   'DESCRIPTOR' : _PONRXPOWERDATA,
   '__module__' : 'voltha_protos.openolt_pb2'
   # @@protoc_insertion_point(class_scope:openolt.PonRxPowerData)
   })
 _sym_db.RegisterMessage(PonRxPowerData)
 
-OnuObjectData = _reflection.GeneratedProtocolMessageType('OnuObjectData', (_message.Message,), {
-  'DESCRIPTOR' : _ONUOBJECTDATA,
-  '__module__' : 'voltha_protos.openolt_pb2'
-  # @@protoc_insertion_point(class_scope:openolt.OnuObjectData)
-  })
-_sym_db.RegisterMessage(OnuObjectData)
-
-IntfObjectData = _reflection.GeneratedProtocolMessageType('IntfObjectData', (_message.Message,), {
-  'DESCRIPTOR' : _INTFOBJECTDATA,
+OnuInfo = _reflection.GeneratedProtocolMessageType('OnuInfo', (_message.Message,), {
+  'DESCRIPTOR' : _ONUINFO,
   '__module__' : 'voltha_protos.openolt_pb2'
-  # @@protoc_insertion_point(class_scope:openolt.IntfObjectData)
+  # @@protoc_insertion_point(class_scope:openolt.OnuInfo)
   })
-_sym_db.RegisterMessage(IntfObjectData)
+_sym_db.RegisterMessage(OnuInfo)
 
-ObjectDataResponse = _reflection.GeneratedProtocolMessageType('ObjectDataResponse', (_message.Message,), {
-  'DESCRIPTOR' : _OBJECTDATARESPONSE,
+PonIntfInfo = _reflection.GeneratedProtocolMessageType('PonIntfInfo', (_message.Message,), {
+  'DESCRIPTOR' : _PONINTFINFO,
   '__module__' : 'voltha_protos.openolt_pb2'
-  # @@protoc_insertion_point(class_scope:openolt.ObjectDataResponse)
+  # @@protoc_insertion_point(class_scope:openolt.PonIntfInfo)
   })
-_sym_db.RegisterMessage(ObjectDataResponse)
-
-ObjectDataRequest = _reflection.GeneratedProtocolMessageType('ObjectDataRequest', (_message.Message,), {
-  'DESCRIPTOR' : _OBJECTDATAREQUEST,
-  '__module__' : 'voltha_protos.openolt_pb2'
-  # @@protoc_insertion_point(class_scope:openolt.ObjectDataRequest)
-  })
-_sym_db.RegisterMessage(ObjectDataRequest)
+_sym_db.RegisterMessage(PonIntfInfo)
 
 Empty = _reflection.GeneratedProtocolMessageType('Empty', (_message.Message,), {
   'DESCRIPTOR' : _EMPTY,
   '__module__' : 'voltha_protos.openolt_pb2'
   # @@protoc_insertion_point(class_scope:openolt.Empty)
   })
 _sym_db.RegisterMessage(Empty)
@@ -4833,16 +4781,16 @@
 _OPENOLT = _descriptor.ServiceDescriptor(
   name='Openolt',
   full_name='openolt.Openolt',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=11145,
-  serialized_end=13832,
+  serialized_start=11083,
+  serialized_end=13845,
   methods=[
   _descriptor.MethodDescriptor(
     name='DisableOlt',
     full_name='openolt.Openolt.DisableOlt',
     index=0,
     containing_service=None,
     input_type=_EMPTY,
@@ -5137,21 +5085,31 @@
     containing_service=None,
     input_type=_ONU,
     output_type=_PONRXPOWERDATA,
     serialized_options=b'\202\323\344\223\002\026\"\021/v1/GetPonRxPower:\001*',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
-    name='GetObject',
-    full_name='openolt.Openolt.GetObject',
+    name='GetOnuInfo',
+    full_name='openolt.Openolt.GetOnuInfo',
     index=30,
     containing_service=None,
-    input_type=_OBJECTDATAREQUEST,
-    output_type=_OBJECTDATARESPONSE,
-    serialized_options=b'\202\323\344\223\002\022\"\r/v1/GetObject:\001*',
+    input_type=_ONU,
+    output_type=_ONUINFO,
+    serialized_options=b'\202\323\344\223\002\023\"\016/v1/GetOnuInfo:\001*',
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetPonInterfaceInfo',
+    full_name='openolt.Openolt.GetPonInterfaceInfo',
+    index=31,
+    containing_service=None,
+    input_type=_INTERFACE,
+    output_type=_PONINTFINFO,
+    serialized_options=b'\202\323\344\223\002\031\"\024/v1/GetInterfaceInfo:\001*',
     create_key=_descriptor._internal_create_key,
   ),
 ])
 _sym_db.RegisterServiceDescriptor(_OPENOLT)
 
 DESCRIPTOR.services_by_name['Openolt'] = _OPENOLT
```

### Comparing `voltha-protos-5.4.2/python/test/__init__.py` & `voltha-protos-5.4.3/python/test/__init__.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/test/test_protos.py` & `voltha-protos-5.4.3/python/test/test_protos.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.2/python/voltha_protos.egg-info/PKG-INFO` & `voltha-protos-5.4.3/python/voltha_protos.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: voltha-protos
-Version: 5.4.2
+Version: 5.4.3
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/gitweb?p=voltha-protos.git
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf voltha
```

### Comparing `voltha-protos-5.4.2/python/voltha_protos.egg-info/SOURCES.txt` & `voltha-protos-5.4.3/python/voltha_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

