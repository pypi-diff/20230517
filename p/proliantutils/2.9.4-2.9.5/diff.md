# Comparing `tmp/proliantutils-2.9.4.tar.gz` & `tmp/proliantutils-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/proliantutils-2.9.4.tar", last modified: Mon Feb 24 05:50:43 2020, max compression
+gzip compressed data, was "dist/proliantutils-2.9.5.tar", last modified: Thu Jul 30 10:18:06 2020, max compression
```

## Comparing `proliantutils-2.9.4.tar` & `proliantutils-2.9.5.tar`

### file list

```diff
@@ -1,236 +1,241 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-02-24 05:49:58.000000 proliantutils-2.9.4/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11323 2020-02-24 05:49:58.000000 proliantutils-2.9.4/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2020-02-24 05:49:58.000000 proliantutils-2.9.4/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9498 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2020-02-24 05:50:43.000000 proliantutils-2.9.4/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2020-02-24 05:49:58.000000 proliantutils-2.9.4/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2020-02-24 05:49:58.000000 proliantutils-2.9.4/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2020-02-24 05:49:58.000000 proliantutils-2.9.4/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/doc/hpssa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2216 2020-02-24 05:49:58.000000 proliantutils-2.9.4/doc/hpssa/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6724 2020-02-24 05:49:58.000000 proliantutils-2.9.4/doc/make.bat
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2020-02-24 05:49:58.000000 proliantutils-2.9.4/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8192 2020-02-24 05:49:58.000000 proliantutils-2.9.4/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6799 2020-02-24 05:49:58.000000 proliantutils-2.9.4/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2020-02-24 05:50:43.000000 proliantutils-2.9.4/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/ipa_hw_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ipa_hw_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4915 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ipa_hw_manager/hardware_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6991 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/hpssa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5640 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/hpssa/disk_allocator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3453 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/hpssa/raid_config_schema.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/hpssa/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27208 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/hpssa/objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16136 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/hpssa/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/hpssa/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/sum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8658 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/sum/sum_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/sum/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/redfish/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4531 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2667 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    54896 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/redfish.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/redfish/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/redfish/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/manager/mapping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/manager/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/manager/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4055 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/manager/virtual_media.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6413 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/update_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4606 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/secure_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1944 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/pci_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2232 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/memory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/mappings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2508 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/ethernet_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8614 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/bios.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/logical_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5548 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/mappings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1922 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/simple_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4478 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/physical_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3002 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/smart_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1490 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7282 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5337 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/array_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8696 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/smart_storage_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28204 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/system.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2477 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/system/iscsi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/redfish/resources/account_service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/account_service/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1621 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/account_service/account.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/account_service/account_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/resources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/redfish/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/test_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/ipa_hw_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4187 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ipa_hw_manager/test_hardware_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ipa_hw_manager/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/hpssa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11776 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/hpssa/test_disk_allocator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31042 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/hpssa/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    72627 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/hpssa/raid_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29233 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/hpssa/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/hpssa/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/sum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16045 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/sum/test_sum_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/sum/sum_sample_output.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/sum/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/redfish/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    92376 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/test_redfish.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4485 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/test_connector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3376 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/manager/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5958 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/manager/test_virtual_media.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5426 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20132 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_bios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_memory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58195 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_system.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11926 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_smart_storage_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4793 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_pci_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4596 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_secure_boot.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8738 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_physical_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1813 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5032 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_logical_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3821 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12114 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12738 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_array_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4523 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_simple_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8910 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_smart_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6530 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5812 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_ethernet_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12256 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/test_update_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/account_service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/account_service/test_account_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2622 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/account_service/test_account.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/account_service/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/resources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4450 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/test_main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/volume_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6645 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/manager.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/pci_device1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18649 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_failed.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/secure_boot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/account_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4024 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/vmedia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/array_controller_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2856 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_mappings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/account_service.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/ethernet_interface_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10769 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_boot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9054 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_base_configs.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/array_controller.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2001 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/logical_nvdimm.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/vmedia_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/logical_drive_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2204 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/ethernet_interface.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/pci_device_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2730 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/smart_storage_config.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/drive.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/pci_device.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4884 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/disk_drive.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/update_service.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/simple_storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/memory_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/simple_storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15329 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/system.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/root.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/account.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/disk_drive_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/smart_storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17919 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/iscsi_settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5944 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/iscsi.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2227 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/logical_drive.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4546 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/redfish/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/rest/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8647 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/rest/rest_sample_outputs.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9649 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/rest/test_v1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/rest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/test_exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/ilo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25283 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/test_firmware_controller.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)   144070 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/test_ris.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    68231 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   923805 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/ribcl_sample_outputs.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)   157068 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/ris_sample_outputs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4780 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/ipmi_sample_outputs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/tests/ilo/snmp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2217 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/snmp/snmp_sample_output.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/snmp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3223 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/snmp/test_snmp_cpqdisk_sizes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51229 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/test_ribcl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10593 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/test_operations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8190 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/ilo/test_ipmi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13570 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/tests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/functests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4867 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/functests/test_hpssa.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/functests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/rest/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10553 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/rest/v1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/rest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/ilo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15821 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/firmware_controller.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    85247 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/ris.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5624 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/ipmi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/mappings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22017 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/operations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49395 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/ribcl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:50:43.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39444 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/CPQHOST-MIB.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   127453 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/CPQIDA-MIB.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/RFC1215-MIB.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7719 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/IANAifType-MIB.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81329 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/CPQSCSI-MIB.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/IF-MIB.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9238 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/snmp_cpqdisk_sizes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/snmp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35629 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9837 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/ilo/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6954 2020-02-24 05:49:58.000000 proliantutils-2.9.4/proliantutils/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2020-02-24 05:50:43.000000 proliantutils-2.9.4/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2020-02-24 05:49:58.000000 proliantutils-2.9.4/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12712 2020-02-24 05:50:43.000000 proliantutils-2.9.4/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2020-02-24 05:49:58.000000 proliantutils-2.9.4/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2020-02-24 05:49:58.000000 proliantutils-2.9.4/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2020-07-30 10:18:06.000000 proliantutils-2.9.5/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2020-07-30 10:16:54.000000 proliantutils-2.9.5/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2020-07-30 10:16:54.000000 proliantutils-2.9.5/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-07-30 10:16:54.000000 proliantutils-2.9.5/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2020-07-30 10:16:54.000000 proliantutils-2.9.5/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2020-07-30 10:16:54.000000 proliantutils-2.9.5/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9792 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils.egg-info/SOURCES.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/redfish/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59912 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/redfish.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2667 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4423 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/redfish/resources/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/redfish/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/manager/virtual_media.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/manager/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/manager/mapping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/manager/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6411 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/update_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2484 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/ethernet_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1969 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/tls_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2233 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/memory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/mappings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8696 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/smart_storage_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28246 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/system.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4606 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/secure_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2477 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9146 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/bios.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7282 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1490 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5548 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2014 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/logical_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3002 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/smart_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4477 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/physical_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/mappings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1922 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/simple_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5338 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/array_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1944 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/system/pci_device.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/redfish/resources/account_service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1621 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/account_service/account.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/account_service/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/redfish/resources/account_service/account_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/sum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8788 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/sum/sum_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/sum/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/functests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/functests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4867 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/functests/test_hpssa.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/redfish/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4546 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4450 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   100392 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/test_redfish.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/drive.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/pci_device1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5944 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/iscsi.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/update_service.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/iscsi_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/tls_config_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9054 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_base_configs.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/simple_storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/simple_storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/vmedia_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4884 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/disk_drive.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2001 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/logical_nvdimm.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/certfile.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/logical_drive_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/memory_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/pci_device_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/disk_drive_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18649 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_failed.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2227 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/logical_drive.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6645 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/manager.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4024 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/vmedia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/pci_device.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2730 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/smart_storage_config.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/ethernet_interface_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2204 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/ethernet_interface.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17944 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/array_controller.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10769 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_boot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/volume_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/account_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/smart_storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2856 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_mappings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/root.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15329 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/system.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/account.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/secure_boot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/account_service.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/array_controller_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/tls_config.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4485 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/test_connector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12257 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/test_update_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5957 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/manager/test_virtual_media.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3377 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/manager/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5426 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20927 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_bios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5812 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_ethernet_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4825 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_tls_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_memory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11926 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_smart_storage_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4793 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_pci_device.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12114 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6530 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3821 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1813 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4523 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_simple_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8910 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_smart_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5032 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_logical_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12738 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_array_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8738 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_physical_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58181 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_system.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4596 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_secure_boot.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/account_service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2622 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/account_service/test_account.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/account_service/test_account_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/redfish/resources/account_service/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13570 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/sum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17324 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/sum/test_sum_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/sum/sum_sample_output.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/sum/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/test_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/ipa_hw_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ipa_hw_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ipa_hw_manager/test_hardware_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/hpssa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31042 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/hpssa/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11776 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/hpssa/test_disk_allocator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/hpssa/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29247 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/hpssa/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    72627 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/hpssa/raid_constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/rest/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9649 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/rest/test_v1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/rest/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8647 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/rest/rest_sample_outputs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/ilo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10593 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/test_common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/tests/ilo/snmp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2217 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/snmp/snmp_sample_output.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/snmp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/snmp/test_snmp_cpqdisk_sizes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    68223 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/test_client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)   144064 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/test_ris.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8190 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/test_ipmi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/test_operations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   923805 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/ribcl_sample_outputs.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)   157012 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/ris_sample_outputs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51697 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/test_ribcl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25283 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/test_firmware_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4780 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/tests/ilo/ipmi_sample_outputs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/ipa_hw_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ipa_hw_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10572 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ipa_hw_manager/hardware_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/hpssa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27119 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/hpssa/objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16136 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/hpssa/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/hpssa/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3453 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/hpssa/raid_config_schema.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5640 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/hpssa/disk_allocator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/hpssa/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/rest/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10553 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/rest/v1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/rest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6924 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/ilo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36199 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5624 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/ipmi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9833 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9211 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/snmp_cpqdisk_sizes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39444 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/CPQHOST-MIB.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/IF-MIB.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81329 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/CPQSCSI-MIB.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/RFC1215-MIB.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7719 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/IANAifType-MIB.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   127453 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/CPQIDA-MIB.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22807 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/operations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15825 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/firmware_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/mappings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49395 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/ribcl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/constants.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    85222 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/ilo/ris.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6954 2020-07-30 10:16:54.000000 proliantutils-2.9.5/proliantutils/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11323 2020-07-30 10:16:54.000000 proliantutils-2.9.5/LICENSE
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6724 2020-07-30 10:16:54.000000 proliantutils-2.9.5/doc/make.bat
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2020-07-30 10:16:54.000000 proliantutils-2.9.5/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8192 2020-07-30 10:16:54.000000 proliantutils-2.9.5/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6799 2020-07-30 10:16:54.000000 proliantutils-2.9.5/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-30 10:18:06.000000 proliantutils-2.9.5/doc/hpssa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2216 2020-07-30 10:16:54.000000 proliantutils-2.9.5/doc/hpssa/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12978 2020-07-30 10:18:06.000000 proliantutils-2.9.5/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2020-07-30 10:18:06.000000 proliantutils-2.9.5/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2020-07-30 10:16:54.000000 proliantutils-2.9.5/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2020-07-30 10:18:06.000000 proliantutils-2.9.5/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2020-07-30 10:16:54.000000 proliantutils-2.9.5/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2020-07-30 10:16:54.000000 proliantutils-2.9.5/README.md
```

### Comparing `proliantutils-2.9.4/LICENSE` & `proliantutils-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils.egg-info/SOURCES.txt` & `proliantutils-2.9.5/proliantutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 proliantutils/redfish/resources/system/iscsi.py
 proliantutils/redfish/resources/system/mappings.py
 proliantutils/redfish/resources/system/memory.py
 proliantutils/redfish/resources/system/pci_device.py
 proliantutils/redfish/resources/system/secure_boot.py
 proliantutils/redfish/resources/system/smart_storage_config.py
 proliantutils/redfish/resources/system/system.py
+proliantutils/redfish/resources/system/tls_config.py
 proliantutils/redfish/resources/system/storage/__init__.py
 proliantutils/redfish/resources/system/storage/array_controller.py
 proliantutils/redfish/resources/system/storage/common.py
 proliantutils/redfish/resources/system/storage/constants.py
 proliantutils/redfish/resources/system/storage/drive.py
 proliantutils/redfish/resources/system/storage/logical_drive.py
 proliantutils/redfish/resources/system/storage/mappings.py
@@ -133,14 +134,15 @@
 proliantutils/tests/redfish/json_samples/array_controller.json
 proliantutils/tests/redfish/json_samples/array_controller_collection.json
 proliantutils/tests/redfish/json_samples/bios.json
 proliantutils/tests/redfish/json_samples/bios_base_configs.json
 proliantutils/tests/redfish/json_samples/bios_boot.json
 proliantutils/tests/redfish/json_samples/bios_failed.json
 proliantutils/tests/redfish/json_samples/bios_mappings.json
+proliantutils/tests/redfish/json_samples/certfile.crt
 proliantutils/tests/redfish/json_samples/disk_drive.json
 proliantutils/tests/redfish/json_samples/disk_drive_collection.json
 proliantutils/tests/redfish/json_samples/drive.json
 proliantutils/tests/redfish/json_samples/ethernet_interface.json
 proliantutils/tests/redfish/json_samples/ethernet_interface_collection.json
 proliantutils/tests/redfish/json_samples/iscsi.json
 proliantutils/tests/redfish/json_samples/iscsi_settings.json
@@ -157,14 +159,16 @@
 proliantutils/tests/redfish/json_samples/simple_storage.json
 proliantutils/tests/redfish/json_samples/simple_storage_collection.json
 proliantutils/tests/redfish/json_samples/smart_storage.json
 proliantutils/tests/redfish/json_samples/smart_storage_config.json
 proliantutils/tests/redfish/json_samples/storage.json
 proliantutils/tests/redfish/json_samples/storage_collection.json
 proliantutils/tests/redfish/json_samples/system.json
+proliantutils/tests/redfish/json_samples/tls_config.json
+proliantutils/tests/redfish/json_samples/tls_config_settings.json
 proliantutils/tests/redfish/json_samples/update_service.json
 proliantutils/tests/redfish/json_samples/vmedia.json
 proliantutils/tests/redfish/json_samples/vmedia_collection.json
 proliantutils/tests/redfish/json_samples/volume.json
 proliantutils/tests/redfish/json_samples/volume_collection.json
 proliantutils/tests/redfish/resources/__init__.py
 proliantutils/tests/redfish/resources/test_update_service.py
@@ -179,14 +183,15 @@
 proliantutils/tests/redfish/resources/system/test_ethernet_interface.py
 proliantutils/tests/redfish/resources/system/test_iscsi.py
 proliantutils/tests/redfish/resources/system/test_memory.py
 proliantutils/tests/redfish/resources/system/test_pci_device.py
 proliantutils/tests/redfish/resources/system/test_secure_boot.py
 proliantutils/tests/redfish/resources/system/test_smart_storage_config.py
 proliantutils/tests/redfish/resources/system/test_system.py
+proliantutils/tests/redfish/resources/system/test_tls_config.py
 proliantutils/tests/redfish/resources/system/storage/__init__.py
 proliantutils/tests/redfish/resources/system/storage/test_array_controller.py
 proliantutils/tests/redfish/resources/system/storage/test_common.py
 proliantutils/tests/redfish/resources/system/storage/test_drive.py
 proliantutils/tests/redfish/resources/system/storage/test_logical_drive.py
 proliantutils/tests/redfish/resources/system/storage/test_physical_drive.py
 proliantutils/tests/redfish/resources/system/storage/test_simple_storage.py
```

### Comparing `proliantutils-2.9.4/proliantutils.egg-info/PKG-INFO` & `proliantutils-2.9.5/proliantutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: proliantutils
-Version: 2.9.4
+Version: 2.9.5
 Summary: Client Library for interfacing with various devices in HP Proliant Servers.
-Home-page: https://github.com/openstack/proliantutils
+Home-page: https://opendev.org/x/proliantutils
 Author: Hewlett Packard Enterprise
 Author-email: proliantutils@gmail.com
 License: Apache License, Version 2.0
 Description: proliantutils
         =============
         
         **proliantutils** is a set of utility libraries for interfacing and managing
@@ -53,13 +53,13 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
```

### Comparing `proliantutils-2.9.4/PKG-INFO` & `proliantutils-2.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: proliantutils
-Version: 2.9.4
+Version: 2.9.5
 Summary: Client Library for interfacing with various devices in HP Proliant Servers.
-Home-page: https://github.com/openstack/proliantutils
+Home-page: https://opendev.org/x/proliantutils
 Author: Hewlett Packard Enterprise
 Author-email: proliantutils@gmail.com
 License: Apache License, Version 2.0
 Description: proliantutils
         =============
         
         **proliantutils** is a set of utility libraries for interfacing and managing
@@ -53,13 +53,13 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
```

### Comparing `proliantutils-2.9.4/README.rst` & `proliantutils-2.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/doc/hpssa/index.rst` & `proliantutils-2.9.5/doc/hpssa/index.rst`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/doc/make.bat` & `proliantutils-2.9.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/doc/source/index.rst` & `proliantutils-2.9.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/doc/source/conf.py` & `proliantutils-2.9.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/doc/Makefile` & `proliantutils-2.9.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/AUTHORS` & `proliantutils-2.9.5/AUTHORS`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Dirk Mueller <dirk@dmllr.de>
 Ilya Etingof <etingof@gmail.com>
 Jim Mankovich <jmank@hp.com>
 Mark Goddard <mark@stackhpc.com>
 Nisha Agarwal <agarwalnisha1980@gmail.com>
 Pratyusha <pratyusha957@gmail.com>
 Ramakrishnan G <rameshg87@gmail.com>
+Riccardo Pittau <elfosardo@gmail.com>
 Shivanand Tendulker <shivanand.tendulker@hpe.com>
 Shivanand Tendulker <stendulker@gmail.com>
 ankit <ankit.dhn31@gmail.com>
 hpproliant <proliantutils@gmail.com>
 kesper <paresh.h.sao@gmail.com>
 kesper <paresh.sao@hpe.com>
 mallikarjuna.kolagatla <mallikarjuna.reddy@hpe.com>
```

### Comparing `proliantutils-2.9.4/proliantutils/log.py` & `proliantutils-2.9.5/proliantutils/log.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/utils.py` & `proliantutils-2.9.5/proliantutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     raw_fw_file_path, is_extracted = fw_img_extractor.extract()
 
     # Note(deray): Need to check if this processing is for RIS or RIBCL
     # based systems. For Gen9 machines (RIS based) the firmware file needs
     # to be on a http store, and hence requires the upload to happen for the
     # firmware file.
     to_upload = False
-    m = re.search('Gen(\d+)', ilo_object.model)
+    m = re.search(r"Gen(\d+)", ilo_object.model)
     if int(m.group(1)) > 8:
         to_upload = True
 
     LOG.debug('Extracting firmware file: %s ... done', compact_firmware_file)
     msg = ('Firmware file %(fw_file)s is %(msg)s. Need hosting (on an http '
            'store): %(yes_or_no)s' %
            {'fw_file': compact_firmware_file,
@@ -132,32 +132,32 @@
                {'image': image_location, 'checksum': expected_checksum,
                 'actual_checksum': actual_checksum})
         raise exception.ImageRefValidationFailed(image_href=image_location,
                                                  reason=msg)
 
 
 def validate_href(image_href):
-        """Validate HTTP image reference.
+    """Validate HTTP image reference.
 
-        :param image_href: Image reference.
-        :raises: exception.ImageRefValidationFailed if HEAD request failed or
-            returned response code not equal to 200.
-        :returns: Response to HEAD request.
-        """
-        try:
-            response = requests.head(image_href)
-            if response.status_code != http_client.OK:
-                raise exception.ImageRefValidationFailed(
-                    image_href=image_href,
-                    reason=("Got HTTP code %s instead of 200 in response to "
-                            "HEAD request." % response.status_code))
-        except requests.RequestException as e:
-            raise exception.ImageRefValidationFailed(image_href=image_href,
-                                                     reason=e)
-        return response
+    :param image_href: Image reference.
+    :raises: exception.ImageRefValidationFailed if HEAD request failed or
+        returned response code not equal to 200.
+    :returns: Response to HEAD request.
+    """
+    try:
+        response = requests.head(image_href)
+        if response.status_code != http_client.OK:
+            raise exception.ImageRefValidationFailed(
+                image_href=image_href,
+                reason=("Got HTTP code %s instead of 200 in response to "
+                        "HEAD request." % response.status_code))
+    except requests.RequestException as e:
+        raise exception.ImageRefValidationFailed(image_href=image_href,
+                                                 reason=e)
+    return response
 
 
 def apply_bios_properties_filter(settings, filter_to_be_applied):
     """Applies the filter to return the dict of filtered BIOS properties.
 
     :param settings: dict of BIOS settings on which filter to be applied.
     :param filter_to_be_applied: list of keys to be applied as filter.
```

### Comparing `proliantutils-2.9.4/proliantutils/hpssa/disk_allocator.py` & `proliantutils-2.9.5/proliantutils/hpssa/disk_allocator.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             return
 
     # We didn't find physical disks to create an independent array.
     # Check if we can get some shared arrays.
     if share_physical_disks:
         sharable_disk_wwns = []
         for sharable_logical_disk in raid_config['logical_disks']:
-            if (sharable_logical_disk.get('share_physical_disks', False) and
-                    'root_device_hint' in sharable_logical_disk):
+            if (sharable_logical_disk.get('share_physical_disks', False)
+                    and 'root_device_hint' in sharable_logical_disk):
                 wwn = sharable_logical_disk['root_device_hint']['wwn']
                 sharable_disk_wwns.append(wwn)
 
         for controller in server.controllers:
             sharable_arrays = [x for x in controller.raid_arrays if
                                x.logical_drives[0].wwn in sharable_disk_wwns]
```

### Comparing `proliantutils-2.9.4/proliantutils/hpssa/raid_config_schema.json` & `proliantutils-2.9.5/proliantutils/hpssa/raid_config_schema.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/hpssa/objects.py` & `proliantutils-2.9.5/proliantutils/hpssa/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,29 +72,30 @@
     while i < len(lines):
 
         current_line = lines[i]
         current_line_indentation = _get_indentation(current_line)
 
         # Check for multi-level returns
         if current_line_indentation < indentation:
-            return info, i-1
+            return info, i - 1
 
         if current_line_indentation == indentation:
             current_item = current_line.lstrip(' ')
             info[current_item] = {}
             i = i + 1
             continue
 
         if i < len(lines) - 1:
-            next_line_indentation = _get_indentation(lines[i+1])
+            next_line_indentation = _get_indentation(lines[i + 1])
         else:
             next_line_indentation = current_line_indentation
 
         if next_line_indentation > current_line_indentation:
-            ret_dict, i = _get_dict(lines, i, current_line_indentation, deep+1)
+            ret_dict, i = _get_dict(lines, i,
+                                    current_line_indentation, deep + 1)
             for key in ret_dict.keys():
                 if key in info[current_item]:
                     info[current_item][key].update(ret_dict[key])
                 else:
                     info[current_item][key] = ret_dict[key]
         else:
             key, value = _get_key_value(current_line)
@@ -550,15 +551,15 @@
             else:
                 raise exception.HPSSAOperationError(reason=ex)
         except Exception as ex:
             raise exception.HPSSAOperationError(reason=ex)
 
         # TODO(rameshg87): This always returns in MB, but confirm with
         # HPSSA folks.
-        match = re.search('Max: (\d+)', stdout)
+        match = re.search(r"Max: (\d+)", stdout)
         if not match:
             return False
 
         max_size_gb = int(match.group(1)) / 1024
         return desired_disk_size <= max_size_gb
 
 
@@ -576,17 +577,16 @@
         # (like 500MB, 25GB) unit of storage space to bytes (Integer value).
         # It requires space to be stripped.
         try:
             size = self.properties['Size'].replace(' ', '')
             # TODO(rameshg87): Reduce the disk size by 1 to make sure Ironic
             # has enough space to write a config drive. Remove this when
             # Ironic doesn't need it.
-            self.size_gb = int(strutils.string_to_bytes(size,
-                                                        return_int=True) /
-                               (1024*1024*1024)) - 1
+            self.size_gb = int(strutils.string_to_bytes(
+                size, return_int=True) / (1024 * 1024 * 1024)) - 1
         except KeyError:
             msg = ("Can't get 'Size' parameter from ssacli output for logical "
                    "disk '%(logical_disk)s' of RAID array '%(array)s' in "
                    "controller '%(controller)s'." %
                    {'logical_disk': self.id,
                     'array': self.parent.id,
                     'controller': self.parent.parent.id})
@@ -645,17 +645,16 @@
         self.id = id[14:]
 
         # 'string_to_bytes' takes care of converting any returned
         # (like 500MB, 25GB) unit of storage space to bytes (Integer value).
         # It requires space to be stripped.
         try:
             size = self.properties['Size'].replace(' ', '')
-            self.size_gb = int(strutils.string_to_bytes(size,
-                                                        return_int=True) /
-                               (1024*1024*1024))
+            self.size_gb = int(strutils.string_to_bytes(
+                size, return_int=True) / (1024 * 1024 * 1024))
         except KeyError:
             msg = ("Can't get 'Size' parameter from ssacli output for "
                    "physical disk '%(physical_disk)s' of controller "
                    "'%(controller)s'." %
                    {'physical_disk': self.id,
                     'controller': self.parent.parent.id})
             raise exception.HPSSAOperationError(reason=msg)
```

### Comparing `proliantutils-2.9.4/proliantutils/hpssa/manager.py` & `proliantutils-2.9.5/proliantutils/hpssa/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
         no_of_disks_specified = None
         if 'number_of_physical_disks' in logical_disk:
             no_of_disks_specified = logical_disk['number_of_physical_disks']
         elif 'physical_disks' in logical_disk:
             no_of_disks_specified = len(logical_disk['physical_disks'])
 
-        if (no_of_disks_specified and
-                no_of_disks_specified < min_disks_reqd):
+        if (no_of_disks_specified
+                and no_of_disks_specified < min_disks_reqd):
             msg = ("RAID level %(raid_level)s requires at least %(number)s "
                    "disks." % {'raid_level': raid_level,
                                'number': min_disks_reqd})
             raise exception.InvalidInputError(msg)
 
 
 def _select_controllers_by(server, select_condition, msg):
@@ -141,16 +141,16 @@
     #
     # Also make sure we create the MAX logical_disks the last to make sure
     # we allot only the remaining space available.
     logical_disks_sorted = (
         sorted((x for x in raid_config['logical_disks']
                 if x['size_gb'] != "MAX"),
                reverse=True,
-               key=lambda x: x['size_gb']) +
-        [x for x in raid_config['logical_disks'] if x['size_gb'] == "MAX"])
+               key=lambda x: x['size_gb'])
+        + [x for x in raid_config['logical_disks'] if x['size_gb'] == "MAX"])
 
     if any(logical_disk['share_physical_disks']
             for logical_disk in logical_disks_sorted
             if 'share_physical_disks' in logical_disk):
         logical_disks_sorted = _sort_shared_logical_disks(logical_disks_sorted)
 
     # We figure out the new disk created by recording the wwns
@@ -231,16 +231,16 @@
 
     And RAID 1+0 can share only when the logical volume with even number of
     disks.
     :param logical_disks: 'logical_disks' to be sorted for shared logical
     disks.
     :returns: the logical disks sorted based the above conditions.
     """
-    is_shared = (lambda x: True if ('share_physical_disks' in x and
-                                    x['share_physical_disks']) else False)
+    is_shared = (lambda x: True if ('share_physical_disks' in x
+                                    and x['share_physical_disks']) else False)
     num_of_disks = (lambda x: x['number_of_physical_disks']
                     if 'number_of_physical_disks' in x else
                     constants.RAID_LEVEL_MIN_DISKS[x['raid_level']])
 
     # Separate logical disks based on share_physical_disks value.
     # 'logical_disks_shared' when share_physical_disks is True and
     # 'logical_disks_nonshared' when share_physical_disks is False
@@ -287,17 +287,17 @@
             logical_disks_shared.insert(0, x)
             check = True
 
     # Final 'logical_disks_sorted' list should have non shared logical disks
     # first, followed by shared logical disks with RAID 1, and finally by the
     # shared logical disks sorted based on number of disks and RAID 1+0
     # condition.
-    logical_disks_sorted = (logical_disks_nonshared +
-                            logical_disks_shared_raid1 +
-                            logical_disks_shared)
+    logical_disks_sorted = (logical_disks_nonshared
+                            + logical_disks_shared_raid1
+                            + logical_disks_shared)
     return logical_disks_sorted
 
 
 def delete_configuration():
     """Delete a RAID configuration on this server.
 
     :returns: the current RAID configuration after deleting all
```

### Comparing `proliantutils-2.9.4/proliantutils/hpssa/constants.py` & `proliantutils-2.9.5/proliantutils/hpssa/constants.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/sum/sum_controller.py` & `proliantutils-2.9.5/proliantutils/sum/sum_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 EXIT_CODE_TO_STRING = {
     0: "The smart component was installed successfully.",
     1: ("The smart component was installed successfully, but the system "
         "must be restarted."),
     3: ("The smart component was not installed. Node is already "
         "up-to-date."),
     253: "The installation of the component failed."
-    }
+}
 
 
 def _execute_sum(sum_file_path, mount_point, components=None):
     """Executes the SUM based firmware update command.
 
     This method executes the SUM based firmware update command to update the
     components specified, if not, it performs update on all the firmware
@@ -125,16 +125,16 @@
         return "Summary: %s" % EXIT_CODE_TO_STRING.get(exit_code)
 
     if exit_code in (0, 1, 253):
         if os.path.exists(OUTPUT_FILES[0]):
             with open(OUTPUT_FILES[0], 'r') as f:
                 output_data = f.read()
 
-            ret_data = output_data[(output_data.find('Deployed Components:') +
-                                    len('Deployed Components:')):
+            ret_data = output_data[(output_data.find('Deployed Components:')
+                                    + len('Deployed Components:')):
                                    output_data.find('Exit status:')]
 
             failed = 0
             success = 0
             for line in re.split('\n\n', ret_data):
                 if line:
                     if 'Success' not in line:
@@ -151,53 +151,55 @@
                      'failed': failed}),
                 'Log Data': _get_log_file_data_as_encoded_content()
             }
 
         return "UPDATE STATUS: UNKNOWN"
 
 
-def update_firmware(node):
+def update_firmware(node, url, checksum, components=None):
     """Performs SUM based firmware update on the node.
 
     This method performs SUM firmware update by mounting the
     SPP ISO on the node. It performs firmware update on all or
     some of the firmware components.
 
-    :param node: A node object of type dict.
+    :param node: A dictionary of the node object.
+    :param url: URL of SPP (Service Pack for Proliant) ISO.
+    :param checksum: MD5 checksum of SPP ISO to verify the image.
+    :param components: List of filenames of the firmware components to be
+        flashed. If not provided, the firmware update is performed on all
+        the firmware components.
     :returns: Operation Status string.
     :raises: SUMOperationError, when the vmedia device is not found or
         when the mount operation fails or when the image validation fails.
     :raises: IloConnectionError, when the iLO connection fails.
     :raises: IloError, when vmedia eject or insert operation fails.
     """
-    sum_update_iso = node['clean_step']['args'].get('url')
-
     # Validates the http image reference for SUM update ISO.
     try:
-        utils.validate_href(sum_update_iso)
+        utils.validate_href(url)
     except exception.ImageRefValidationFailed as e:
         raise exception.SUMOperationError(reason=e)
 
     # Waits for the OS to detect the disk and update the label file. SPP ISO
     # is identified by matching its label.
     time.sleep(WAIT_TIME_DISK_LABEL_TO_BE_VISIBLE)
     vmedia_device_dir = "/dev/disk/by-label/"
-    for file in os.listdir(vmedia_device_dir):
-        if fnmatch.fnmatch(file, 'SPP*'):
-            vmedia_device_file = os.path.join(vmedia_device_dir, file)
+    for fname in os.listdir(vmedia_device_dir):
+        if fnmatch.fnmatch(fname, 'SPP*'):
+            vmedia_device_file = os.path.join(vmedia_device_dir, fname)
 
     if not os.path.exists(vmedia_device_file):
         msg = "Unable to find the virtual media device for SUM"
         raise exception.SUMOperationError(reason=msg)
 
     # Validates the SPP ISO image for any file corruption using the checksum
     # of the ISO file.
-    expected_checksum = node['clean_step']['args'].get('checksum')
     try:
-        utils.verify_image_checksum(vmedia_device_file, expected_checksum)
+        utils.verify_image_checksum(vmedia_device_file, checksum)
     except exception.ImageRefValidationFailed as e:
         raise exception.SUMOperationError(reason=e)
 
     # Mounts SPP ISO on a temporary directory.
     vmedia_mount_point = tempfile.mkdtemp()
     try:
         try:
@@ -211,15 +213,14 @@
         # Executes the SUM based firmware update by passing the 'smartupdate'
         # executable path if exists else 'hpsum' executable path and the
         # components specified (if any).
         sum_file_path = os.path.join(vmedia_mount_point, SUM_LOCATION)
         if not os.path.exists(sum_file_path):
             sum_file_path = os.path.join(vmedia_mount_point, HPSUM_LOCATION)
 
-        components = node['clean_step']['args'].get('components')
         result = _execute_sum(sum_file_path, vmedia_mount_point,
                               components=components)
 
         processutils.trycmd("umount", vmedia_mount_point)
     finally:
         shutil.rmtree(vmedia_mount_point, ignore_errors=True)
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/utils.py` & `proliantutils-2.9.5/proliantutils/redfish/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,53 +49,50 @@
 
     if not body:
         raise exception.MissingAttributeError(
             attribute='/'.join(subresource_path), resource=resource.path)
 
     if '@odata.id' not in body:
         raise exception.MissingAttributeError(
-            attribute='/'.join(subresource_path)+'/@odata.id',
+            attribute='/'.join(subresource_path) + '/@odata.id',
             resource=resource.path)
 
     return body['@odata.id']
 
 
 def get_supported_boot_mode(supported_boot_mode):
-        """Return bios and uefi support.
+    """Return bios and uefi support.
 
-        :param supported_boot_mode: Supported boot modes
-        :return: A tuple of 'true'/'false' based on bios and uefi
-            support respectively.
-        """
-        boot_mode_bios = 'false'
-        boot_mode_uefi = 'false'
-        if (supported_boot_mode ==
-                sys_cons.SUPPORTED_LEGACY_BIOS_ONLY):
-            boot_mode_bios = 'true'
-        elif (supported_boot_mode ==
-                sys_cons.SUPPORTED_UEFI_ONLY):
-            boot_mode_uefi = 'true'
-        elif (supported_boot_mode ==
-                sys_cons.SUPPORTED_LEGACY_BIOS_AND_UEFI):
-            boot_mode_bios = 'true'
-            boot_mode_uefi = 'true'
+    :param supported_boot_mode: Supported boot modes
+    :return: A tuple of 'true'/'false' based on bios and uefi
+        support respectively.
+    """
+    boot_mode_bios = 'false'
+    boot_mode_uefi = 'false'
+    if (supported_boot_mode == sys_cons.SUPPORTED_LEGACY_BIOS_ONLY):
+        boot_mode_bios = 'true'
+    elif (supported_boot_mode == sys_cons.SUPPORTED_UEFI_ONLY):
+        boot_mode_uefi = 'true'
+    elif (supported_boot_mode == sys_cons.SUPPORTED_LEGACY_BIOS_AND_UEFI):
+        boot_mode_bios = 'true'
+        boot_mode_uefi = 'true'
 
-        return SupportedBootModes(boot_mode_bios=boot_mode_bios,
-                                  boot_mode_uefi=boot_mode_uefi)
+    return SupportedBootModes(boot_mode_bios=boot_mode_bios,
+                              boot_mode_uefi=boot_mode_uefi)
 
 
-def get_allowed_operations(resource, subresouce_path):
+def get_allowed_operations(resource, subresource_path):
     """Helper function to get the HTTP allowed methods.
 
     :param resource: ResourceBase instance from which the path is loaded.
     :param subresource_path: JSON field to fetch the value from.
             Either a string, or a list of strings in case of a nested field.
     :returns: A list of allowed HTTP methods.
     """
-    uri = get_subresource_path_by(resource, subresouce_path)
+    uri = get_subresource_path_by(resource, subresource_path)
     response = resource._conn.get(path=uri)
     return response.headers['Allow']
 
 
 def is_operation_allowed(method, resource, subresouce_path):
     """Checks whether the operation is allowed for the resource.
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/connector.py` & `proliantutils-2.9.5/proliantutils/redfish/connector.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/redfish.py` & `proliantutils-2.9.5/proliantutils/redfish/redfish.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 __author__ = 'HPE'
 
 import json
+import re
 
 from six.moves.urllib import parse
 import sushy
 from sushy.resources.system import mappings as sushy_map
 from sushy import utils
 
 from proliantutils import exception
@@ -51,14 +52,15 @@
 }
 
 DEVICE_COMMON_TO_REDFISH = {
     'NETWORK': sushy.BOOT_SOURCE_TARGET_PXE,
     'HDD': sushy.BOOT_SOURCE_TARGET_HDD,
     'CDROM': sushy.BOOT_SOURCE_TARGET_CD,
     'ISCSI': sushy.BOOT_SOURCE_TARGET_UEFI_TARGET,
+    'UEFIHTTP': sushy.BOOT_SOURCE_TARGET_UEFI_HTTP,
     'NONE': sushy.BOOT_SOURCE_TARGET_NONE
 }
 
 DEVICE_REDFISH_TO_COMMON = {v: k for k, v in DEVICE_COMMON_TO_REDFISH.items()}
 
 BOOT_MODE_MAP = {
     sys_cons.BIOS_BOOT_MODE_LEGACY_BIOS: 'LEGACY',
@@ -69,14 +71,15 @@
     utils.revert_dictionary(BOOT_MODE_MAP))
 
 PERSISTENT_BOOT_MAP = {
     sushy.BOOT_SOURCE_TARGET_PXE: 'NETWORK',
     sushy.BOOT_SOURCE_TARGET_HDD: 'HDD',
     sushy.BOOT_SOURCE_TARGET_CD: 'CDROM',
     sushy.BOOT_SOURCE_TARGET_UEFI_TARGET: 'NETWORK',
+    sushy.BOOT_SOURCE_TARGET_UEFI_HTTP: 'UEFIHTTP',
     sushy.BOOT_SOURCE_TARGET_NONE: 'NONE'
 }
 
 GET_SECUREBOOT_CURRENT_BOOT_MAP = {
     sys_cons.SECUREBOOT_CURRENT_BOOT_ENABLED: True,
     sys_cons.SECUREBOOT_CURRENT_BOOT_DISABLED: False
 }
@@ -564,15 +567,15 @@
         :raises: IloInvalidInputError, if the given input is not valid.
         """
         sushy_system = self._get_sushy_system(PROLIANT_SYSTEM_ID)
         # Check if the input is valid
         for item in devices:
             if item.upper() not in DEVICE_COMMON_TO_REDFISH:
                 msg = (self._('Invalid input "%(device)s". Valid devices: '
-                              'NETWORK, HDD, ISCSI or CDROM.') %
+                              'NETWORK, HDD, ISCSI, UEFIHTTP or CDROM.') %
                        {'device': item})
                 raise exception.IloInvalidInputError(msg)
 
         try:
             sushy_system.update_persistent_boot(
                 devices, persistent=True)
         except sushy.exceptions.SushyError as e:
@@ -590,15 +593,15 @@
         :raises: IloError, on an error from iLO.
         :raises: IloInvalidInputError, if the given input is not valid.
         """
         sushy_system = self._get_sushy_system(PROLIANT_SYSTEM_ID)
         # Check if the input is valid
         if device.upper() not in DEVICE_COMMON_TO_REDFISH:
             msg = (self._('Invalid input "%(device)s". Valid devices: '
-                          'NETWORK, HDD, ISCSI or CDROM.') %
+                          'NETWORK, HDD, ISCSI, UEFIHTTP or CDROM.') %
                    {'device': device})
             raise exception.IloInvalidInputError(msg)
 
         try:
             sushy_system.update_persistent_boot(
                 [device], persistent=False)
         except sushy.exceptions.SushyError as e:
@@ -692,15 +695,15 @@
                      members_identities) > 0),
                 ('has_ssd',
                  common_storage.has_ssd(sushy_system)),
                 ('has_rotational',
                  common_storage.has_rotational(sushy_system)),
                 ('has_nvme_ssd',
                  common_storage.has_nvme_ssd(sushy_system))
-                ]
+            ]
 
             all_key_to_value_expression_tuples += (
                 [('logical_raid_level_' + x, True)
                  for x in sushy_system.smart_storage.logical_raid_levels])
 
             all_key_to_value_expression_tuples += (
                 [('drive_rotational_' + str(x) + '_rpm', True)
@@ -1272,7 +1275,125 @@
         """Get the list of all disk type available in server
 
         :returns: A list containing disk types
         :raises: IloError, on an error from iLO.
         """
         sushy_system = self._get_sushy_system(PROLIANT_SYSTEM_ID)
         return sushy_system.get_disk_types()
+
+    def get_http_boot_url(self):
+        """Sets current BIOS settings to the provided data.
+
+        :raises: IloError, on an error from iLO.
+        :return: Returns the setting 'UrlBootFile' if set previously.
+        """
+        sushy_system = self._get_sushy_system(PROLIANT_SYSTEM_ID)
+        url = None
+        try:
+            settings = sushy_system.bios_settings.json
+            attributes = settings.get('Attributes')
+            url = attributes.get('UrlBootFile')
+        except sushy.exceptions.SushyError as e:
+            msg = (self._('The attribute "UrlBootFile" not found.'
+                          ' Error %(error)s') %
+                   {'error': str(e)})
+            LOG.debug(msg)
+            raise exception.IloError(msg)
+        return url
+
+    def set_http_boot_url(self, url, is_dhcp_enabled=True):
+        """Sets HTTP boot URL to boot from it.
+
+        :param: url: HTTP URL of the image to be booted on the iLO.
+        :param: is_dhcp_enabled: True if no static IP is set on the node and
+                preferred to use DHCP service running in the network.
+                If False, the MAC is expected to be configured with static IP.
+        :raises: IloError, on an error from iLO.
+        """
+        if not url:
+            raise exception.IloError("Could not set http url with"
+                                     " empty URL")
+        data = {
+            'PreBootNetwork': 'Auto',
+            'UrlBootFile': url,
+            'Dhcpv4': 'Enabled' if is_dhcp_enabled else 'Disabled'
+        }
+
+        sushy_system = self._get_sushy_system(PROLIANT_SYSTEM_ID)
+        try:
+            settings_required = sushy_system.bios_settings.pending_settings
+            settings_required.update_bios_data_by_post(data)
+        except sushy.exceptions.SushyError as e:
+            msg = (self._('Could not set HTTPS URL on the iLO.'
+                          ' Error %(error)s') %
+                   {'error': str(e)})
+            LOG.debug(msg)
+            raise exception.IloError(msg)
+
+    def add_tls_certificate(self, cert_file_list):
+        """Adds the TLS certificates to the iLO.
+
+        :param cert_file_list: List of TLS certificate files
+
+        :raises: IloError, on an error from iLO.
+        :raises: IloCommandNotSupportedError, if the command is
+                 not supported on the server.
+        """
+        sushy_system = self._get_sushy_system(PROLIANT_SYSTEM_ID)
+        if(self._is_boot_mode_uefi()):
+            cert_list = []
+            for cert_file in cert_file_list:
+                with open(cert_file, 'r') as f:
+                    data = json.dumps(f.read())
+                p = re.sub(r"\"", "", data)
+                q = re.sub(r"\\n", "\r\n", p)
+                r = q.rstrip()
+                cert = {}
+                cert['X509Certificate'] = r
+                cert_list.append(cert)
+
+            cert_dict = {}
+            cert_dict['NewCertificates'] = cert_list
+            try:
+                (sushy_system.bios_settings.tls_config.
+                 tls_config_settings.add_tls_certificate(cert_dict))
+            except sushy.exceptions.SushyError as e:
+                msg = (self._("The Redfish controller has failed to upload "
+                              "TLS certificate. Error %(error)s") %
+                       {'error': str(e)})
+                LOG.debug(msg)
+                raise exception.IloError(msg)
+        else:
+            msg = 'TLS certificate cannot be upload in BIOS boot mode'
+            raise exception.IloCommandNotSupportedInBiosError(msg)
+
+    def remove_tls_certificate(self, fp_list):
+        """Removes the TLS certificate from the iLO.
+
+        :param fp_list: List of finger prints of the TLS certificates
+
+        :raises: IloError, on an error from iLO.
+        :raises: IloCommandNotSupportedError, if the command is
+                 not supported on the server.
+        """
+        sushy_system = self._get_sushy_system(PROLIANT_SYSTEM_ID)
+        if(self._is_boot_mode_uefi()):
+            cert = {}
+            del_cert_list = []
+            for fp in fp_list:
+                cert_fp = {
+                    "FingerPrint": fp
+                }
+                del_cert_list.append(cert_fp)
+            cert.update({"DeleteCertificates": del_cert_list})
+            try:
+                (sushy_system.bios_settings.tls_config.
+                 tls_config_settings.remove_tls_certificate(cert))
+            except sushy.exceptions.SushyError as e:
+                msg = (self._("The Redfish controller has failed to remove "
+                              "TLS certificate. Error %(error)s") %
+                       {'error': str(e)})
+                LOG.debug(msg)
+                raise exception.IloError(msg)
+        else:
+            msg = 'TLS certificate cannot be removed in BIOS boot mode'
+            raise exception.IloCommandNotSupportedInBiosError(msg)
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/manager/mapping.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/manager/mapping.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/manager/manager.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/manager/manager.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/manager/constants.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/manager/constants.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/manager/virtual_media.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/manager/virtual_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,17 @@
         :param boot_on_next_reset: boolean value
         :raises: SushyError, on an error from iLO.
         """
         data = {
             "Oem": {
                 "Hpe": {
                     "BootOnNextServerReset": boot_on_next_reset
-                    }
                 }
             }
+        }
         self._conn.patch(self.path, data=data)
 
 
 class VirtualMediaCollection(base.ResourceCollectionBase):
 
     @property
     def _resource_type(self):
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/update_service.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/update_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 __author__ = 'HPE'
 
 import sushy
-
 from sushy.resources import base
 from sushy.resources import common as sushy_common
 
 from proliantutils import exception
 from proliantutils.ilo import common
 from proliantutils import log
 
@@ -51,15 +50,15 @@
         fw_update_action = self._actions.update_firmware
         if not fw_update_action:
             raise (sushy.exceptions.
                    MissingActionError(action='#UpdateService.SimpleUpdate',
                                       resource=self._path))
         return fw_update_action
 
-    def flash_firmware(self, redfish_inst,  file_url):
+    def flash_firmware(self, redfish_inst, file_url):
         """Perform firmware flashing on a redfish system
 
         :param file_url: url to firmware bits.
         :param redfish_inst: redfish instance
         :raises: IloError, on an error from iLO.
         """
         action_data = {
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/secure_boot.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/secure_boot.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/pci_device.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/pci_device.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/memory.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+import collections
+
 from sushy.resources import base
 
-import collections
 from proliantutils.redfish.resources.system import constants as sys_cons
 from proliantutils.redfish.resources.system import mappings
 
 MemoryData = collections.namedtuple(
     'MemoryData', ['has_persistent_memory',
                    'has_nvdimm_n',
                    'has_logical_nvdimm_n'])
@@ -51,15 +52,15 @@
         persistent_memory = False
         nvdimm_n = False
         logical_nvdimm_n = False
         for mem in self.get_members():
             if mem.memory_type == sys_cons.MEMORY_TYPE_NVDIMM_N:
                 persistent_memory = True
                 nvdimm_n = True
-                if (mem.memory_device_type ==
-                        sys_cons.MEMORY_DEVICE_TYPE_LOGICAL):
+                if (mem.memory_device_type
+                        == sys_cons.MEMORY_DEVICE_TYPE_LOGICAL):
                     logical_nvdimm_n = True
                     break
 
         return MemoryData(has_persistent_memory=persistent_memory,
                           has_nvdimm_n=nvdimm_n,
                           has_logical_nvdimm_n=logical_nvdimm_n)
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/mappings.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/mappings.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/ethernet_interface.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/ethernet_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,17 @@
         {'Port 1': 'aa:bb:cc:dd:ee:ff'} and ironic ilo drivers inspection
         consumes the data in this format.
         Note: 'Id' is referred to as "Port number".
         """
         mac_dict = {}
         for eth in self.get_members():
             if eth.mac_address is not None:
-                if (eth.status is not None and
-                        eth.status.health == sys_cons.HEALTH_OK
-                        and eth.status.state ==
-                        sys_cons.HEALTH_STATE_ENABLED):
+                if (eth.status is not None
+                        and eth.status.health == sys_cons.HEALTH_OK
+                        and eth.status.state == sys_cons.HEALTH_STATE_ENABLED):
                     mac_dict.update(
                         {'Port ' + eth.identity: eth.mac_address})
         return mac_dict
 
     def get_uefi_device_path_by_mac(self, mac):
         """Return uefi device path of mac"""
         for nic in self.get_members():
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/bios.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/bios.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from sushy import utils as sushy_utils
 
 from proliantutils import exception
 from proliantutils import log
 from proliantutils.redfish.resources.system import constants as sys_cons
 from proliantutils.redfish.resources.system import iscsi
 from proliantutils.redfish.resources.system import mappings
+from proliantutils.redfish.resources.system import tls_config
 from proliantutils.redfish import utils
 
 LOG = log.get_logger(__name__)
 
 BOOT_SOURCE_TARGET_TO_PARTIAL_STRING_MAP = {
     sushy.BOOT_SOURCE_TARGET_CD: ('HPE Virtual CD-ROM',),
     sushy.BOOT_SOURCE_TARGET_PXE: ('NIC', 'PXE'),
@@ -92,14 +93,27 @@
         return iscsi.ISCSIResource(
             self._conn, utils.get_subresource_path_by(
                 self, ["Oem", "Hpe", "Links", "iScsi"]),
             redfish_version=self.redfish_version)
 
     @property
     @sushy_utils.cache_it
+    def tls_config(self):
+        """Property to provide reference to BIOS TLS configuration instance
+
+        It is calculated once when the first time it is queried. On refresh,
+        this property gets reset.
+        """
+        return tls_config.TLSConfig(
+            self._conn, utils.get_subresource_path_by(
+                self, ["Oem", "Hpe", "Links", "TlsConfig"]),
+            redfish_version=self.redfish_version)
+
+    @property
+    @sushy_utils.cache_it
     def bios_mappings(self):
         """Property to provide reference to bios mappings instance
 
         It is calculated once when the first time it is queried. On refresh,
         this property gets reset.
         """
         return BIOSMappings(
@@ -187,16 +201,16 @@
             msg = ('Boot sources or persistent boot config order not found')
             LOG.debug(msg)
             raise exception.IloError(msg)
 
         preferred_boot_device = self.persistent_boot_config_order[0]
         for boot_source in self.boot_sources:
             if ((boot_source.get("StructuredBootString") is not None) and (
-                    preferred_boot_device ==
-                    boot_source.get("StructuredBootString"))):
+                    preferred_boot_device
+                    == boot_source.get("StructuredBootString"))):
                 boot_string = boot_source["BootString"]
                 break
         else:
             msg = (('Persistent boot device failed, as no matched boot '
                     'sources found for device: %(persistent_boot_device)s')
                    % {'persistent_boot_device': preferred_boot_device})
             LOG.debug(msg)
@@ -217,16 +231,16 @@
         boot_sources = self.boot_sources
         if not boot_sources:
             msg = ('Boot sources are not found')
             LOG.debug(msg)
             raise exception.IloError(msg)
 
         for boot_source in boot_sources:
-            if (mac.upper() in boot_source['UEFIDevicePath'] and
-                    'iSCSI' in boot_source['UEFIDevicePath']):
+            if (mac.upper() in boot_source['UEFIDevicePath']
+                    and 'iSCSI' in boot_source['UEFIDevicePath']):
                 return boot_source['StructuredBootString']
         else:
             msg = ('MAC provided "%s" is Invalid' % mac)
             raise exception.IloInvalidInputError(msg)
 
 
 class BIOSMappings(base.ResourceBase):
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/logical_drive.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/logical_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from sushy.resources import base
 from sushy import utils as sushy_utils
 
-from proliantutils.redfish import utils
-
 from proliantutils.redfish.resources.system.storage import mappings
+from proliantutils.redfish import utils
 
 
 class HPELogicalDrive(base.ResourceBase):
     """This class represents the LogicalDrives resource"""
 
     identity = base.Field('Id')
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/storage.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         return False
 
     @property
     @sushy_utils.cache_it
     def has_nvme_ssd(self):
         """Return True if the drive is SSD and protocol is NVMe"""
         for member in self._drives_list():
-            if (member.media_type == constants.MEDIA_TYPE_SSD and
-                    member.protocol == constants.PROTOCOL_NVMe):
+            if (member.media_type == constants.MEDIA_TYPE_SSD
+                    and member.protocol == constants.PROTOCOL_NVMe):
                 return True
         return False
 
     @property
     @sushy_utils.cache_it
     def drive_rotational_speed_rpm(self):
         """Gets set of rotational speed of the disks"""
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/mappings.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/mappings.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/simple_storage.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/simple_storage.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/physical_drive.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/physical_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from sushy.resources import base
 from sushy import utils as sushy_utils
 
-from proliantutils.redfish import utils
-
 from proliantutils.redfish.resources.system.storage import constants
 from proliantutils.redfish.resources.system.storage import mappings
+from proliantutils.redfish import utils
 
 
 class HPEPhysicalDrive(base.ResourceBase):
     """This class represents the HPEPhysicalDrives resource"""
 
     identity = base.Field('Id', required=True)
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/smart_storage.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/smart_storage.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/volume.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/volume.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/drive.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/drive.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-# There is no explicit collection for Drives. That said, a URI link as
-# "/redfish/v1/Systems/1/Storage/1/Drives" will be an invalid URI.
+"""
+There is no explicit collection for Drives. That said, a URI link as
+"/redfish/v1/Systems/1/Storage/1/Drives" will be an invalid URI.
+"""
 
+from sushy.resources import base
 
 from proliantutils.redfish.resources.system.storage import mappings
 
-from sushy.resources import base
-
 
 class Drive(base.ResourceBase):
     """This class represents the Drive resource"""
 
     capacity_bytes = base.Field('CapacityBytes', adapter=int)
     """The size in bytes of this Drive"""
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/common.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/common.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/constants.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/constants.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/storage/array_controller.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/storage/array_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import logging
 
+from sushy.resources import base
 from sushy import utils as sushy_utils
 
 from proliantutils.redfish.resources.system.storage import logical_drive
 from proliantutils.redfish.resources.system.storage import physical_drive
 from proliantutils.redfish import utils
-from sushy.resources import base
+
 
 LOG = logging.getLogger(__name__)
 
 
 class HPEArrayController(base.ResourceBase):
     """This class represents the HPEArrayControllers resource"""
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/smart_storage_config.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/smart_storage_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from proliantutils import exception
-from proliantutils import log
 from sushy.resources import base
 
+from proliantutils import exception
 from proliantutils.hpssa import constants
 from proliantutils.hpssa import manager
+from proliantutils import log
 from proliantutils.redfish.resources.system.storage import \
     constants as storage_const
 from proliantutils.redfish.resources.system.storage import \
     mappings as storage_map
 
 
 LOG = log.get_logger(__name__)
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/system.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 __author__ = 'HPE'
 
 import re
+
 import sushy
 from sushy.resources import base
 from sushy.resources.system import system
 from sushy import utils as sushy_utils
 
 from proliantutils import exception
 from proliantutils import log
@@ -34,25 +35,25 @@
     constants as storage_const
 from proliantutils.redfish.resources.system.storage import \
     mappings as storage_map
 from proliantutils.redfish.resources.system.storage import simple_storage
 from proliantutils.redfish.resources.system.storage import \
     smart_storage as hpe_smart_storage
 from proliantutils.redfish.resources.system.storage import storage
-
 from proliantutils.redfish import utils
 
 
 LOG = log.get_logger(__name__)
 
 PERSISTENT_BOOT_DEVICE_MAP = {
     'CDROM': sushy.BOOT_SOURCE_TARGET_CD,
     'NETWORK': sushy.BOOT_SOURCE_TARGET_PXE,
     'ISCSI': sushy.BOOT_SOURCE_TARGET_UEFI_TARGET,
-    'HDD': sushy.BOOT_SOURCE_TARGET_HDD
+    'HDD': sushy.BOOT_SOURCE_TARGET_HDD,
+    'UEFIHTTP': sushy.BOOT_SOURCE_TARGET_UEFI_HTTP
 }
 
 
 class PowerButtonActionField(base.CompositeField):
     allowed_values = base.Field('PushType@Redfish.AllowableValues',
                                 adapter=list)
 
@@ -311,15 +312,15 @@
         self.check_smart_storage_config_ids()
         any_exceptions = []
         ld_exc_count = 0
         for config_id in self.smart_storage_config_identities:
             try:
                 ssc_obj = self.get_smart_storage_config(config_id)
                 ssc_obj.delete_raid()
-            except exception.IloLogicalDriveNotFoundError as e:
+            except exception.IloLogicalDriveNotFoundError:
                 ld_exc_count += 1
             except sushy.exceptions.SushyError as e:
                 any_exceptions.append((config_id, str(e)))
 
         if any_exceptions:
             msg = ('The Redfish controller failed to delete the '
                    'raid configuration in one or more controllers with '
@@ -530,15 +531,15 @@
             try:
                 ssc_obj = (
                     self._get_smart_storage_config_by_controller_model(
                         controller))
                 if ssc_obj:
                     result = ssc_obj.read_raid(controller=controller)
                     config['logical_disks'].extend(result['logical_disks'])
-            except exception.IloLogicalDriveNotFoundError as e:
+            except exception.IloLogicalDriveNotFoundError:
                 ld_exc_count += 1
             except sushy.exceptions.SushyError as e:
                 any_exceptions.append((controller, str(e)))
 
         if ld_exc_count == len(controllers):
             msg = 'No logical drives are found in any controllers.'
             raise exception.IloLogicalDriveNotFoundError(msg)
```

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/constants.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/constants.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/system/iscsi.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/system/iscsi.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/account_service/account.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/account_service/account.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/resources/account_service/account_service.py` & `proliantutils-2.9.5/proliantutils/redfish/resources/account_service/account_service.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/redfish/main.py` & `proliantutils-2.9.5/proliantutils/redfish/main.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/test_log.py` & `proliantutils-2.9.5/proliantutils/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/ipa_hw_manager/__init__.py` & `proliantutils-2.9.5/proliantutils/tests/ipa_hw_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-import six
 import sys
 
 import mock
 from oslo_utils import importutils
+import six
+
 
 ironic_python_agent = importutils.try_import('ironic_python_agent')
 if not ironic_python_agent:
     ipa_mock = mock.MagicMock()
     sys.modules['ironic_python_agent'] = ipa_mock
     sys.modules['ironic_python_agent.errors'] = ipa_mock.errors
     sys.modules['ironic_python_agent.hardware'] = ipa_mock.hardware
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/hpssa/test_disk_allocator.py` & `proliantutils-2.9.5/proliantutils/tests/hpssa/test_disk_allocator.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/hpssa/test_objects.py` & `proliantutils-2.9.5/proliantutils/tests/hpssa/test_objects.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/hpssa/raid_constants.py` & `proliantutils-2.9.5/proliantutils/tests/hpssa/raid_constants.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/hpssa/test_manager.py` & `proliantutils-2.9.5/proliantutils/tests/hpssa/test_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+import time
+
 import mock
 import testtools
-import time
 
 from proliantutils import exception
 from proliantutils.hpssa import manager
 from proliantutils.hpssa import objects
 from proliantutils.tests.hpssa import raid_constants
 
 
@@ -46,22 +47,22 @@
 
         ld1_drives = '5I:1:1,5I:1:2'
         ld2_drives = '5I:1:3,5I:1:4,6I:1:5'
         controller_exec_cmd_mock.assert_any_call("create",
                                                  "type=logicaldrive",
                                                  "drives=%s" % ld2_drives,
                                                  "raid=5",
-                                                 "size=%d" % (100*1024),
+                                                 "size=%d" % (100 * 1024),
                                                  process_input='y')
         # Verify that we created the 50GB disk the last.
         controller_exec_cmd_mock.assert_called_with("create",
                                                     "type=logicaldrive",
                                                     "drives=%s" % ld1_drives,
                                                     "raid=1",
-                                                    "size=%d" % (50*1024),
+                                                    "size=%d" % (50 * 1024),
                                                     process_input='y')
 
         ld1_ret = [x for x in current_config['logical_disks']
                    if x['raid_level'] == '1'][0]
         ld2_ret = [x for x in current_config['logical_disks']
                    if x['raid_level'] == '5'][0]
 
@@ -144,22 +145,22 @@
                                        {'size_gb': 100,
                                         'raid_level': '5'}]}
         current_config = manager.create_configuration(raid_info)
         controller_exec_cmd_mock.assert_any_call("create",
                                                  "type=logicaldrive",
                                                  mock.ANY,
                                                  "raid=5",
-                                                 "size=%d" % (100*1024),
+                                                 "size=%d" % (100 * 1024),
                                                  process_input='y')
         # Verify that we created the 50GB disk the last.
         controller_exec_cmd_mock.assert_called_with("create",
                                                     "type=logicaldrive",
                                                     mock.ANY,
                                                     "raid=1",
-                                                    "size=%d" % (50*1024),
+                                                    "size=%d" % (50 * 1024),
                                                     process_input='y')
 
         ld1_ret = [x for x in current_config['logical_disks']
                    if x['raid_level'] == '1'][0]
         ld2_ret = [x for x in current_config['logical_disks']
                    if x['raid_level'] == '5'][0]
         self.assertEqual('0x600508b1001cc42c',
@@ -547,15 +548,16 @@
         controller_exec_cmd_mock.return_value = value
         expt_ret = {
             'Smart Array P440 in Slot 2': {
                 '1I:2:1': 'Erase Complete. Reenable Before Using.',
                 'Summary': ('Drives overwritten with zeros because '
                             'sanitize erase is not supported on the '
                             'controller.')
-                }}
+            }
+        }
 
         ret = manager.erase_devices()
         self.assertEqual(expt_ret, ret)
         self.assertTrue(controller_exec_cmd_mock.called)
         self.assertTrue(sleep_mock.called)
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/sum/test_sum_controller.py` & `proliantutils-2.9.5/proliantutils/tests/sum/test_sum_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import os
 import shutil
 import tarfile
 import tempfile
+import time
 
 import mock
 from oslo_concurrency import processutils
 from oslo_serialization import base64
 import testtools
 
 from proliantutils import exception
@@ -57,15 +58,15 @@
         execute_mock.side_effect = processutils.ProcessExecutionError(
             stdout=value, stderr=None, exit_code=0)
         ret_value = {
             'Log Data': 'aaabbbcccdddd',
             'Summary': ("The smart component was installed successfully."
                         " Status of updated components: Total: 2 Success: 2 "
                         "Failed: 0.")
-            }
+        }
 
         stdout = sum_controller._execute_sum("hpsum", "/tmp/hpsum",
                                              components=None)
 
         self.assertEqual(ret_value, stdout)
         execute_mock.assert_called_once_with('hpsum', '--s', '--romonly', '')
 
@@ -99,15 +100,15 @@
         exists_mock.return_value = True
         log_mock.return_value = "aaabbbcccdddd"
         ret = {
             'Log Data': 'aaabbbcccdddd',
             'Summary': ("The installation of the component failed. Status "
                         "of updated components: Total: 2 Success: 1 "
                         "Failed: 1.")
-            }
+        }
         value = ("hpsum_service_x64 started successfully. Sending Shutdown "
                  "request to engine. Successfully shutdown the service.")
         execute_mock.side_effect = processutils.ProcessExecutionError(
             stdout=value, stderr=None, exit_code=253)
 
         stdout = sum_controller._execute_sum("hpsum", "/tmp/hpsum",
                                              components=None)
@@ -148,72 +149,81 @@
 
         with tarfile.open(name=tar_file.name) as tar:
             f = tar.extractfile(file_object.name.lstrip('/'))
             self.assertEqual(log_file_content, f.read())
         os.remove(file_object.name)
         os.remove(tar_file.name)
 
+    @mock.patch.object(time, 'sleep')
     @mock.patch.object(utils, 'validate_href')
     @mock.patch.object(utils, 'verify_image_checksum')
     @mock.patch.object(sum_controller, '_execute_sum')
     @mock.patch.object(os, 'listdir')
     @mock.patch.object(shutil, 'rmtree', autospec=True)
     @mock.patch.object(tempfile, 'mkdtemp', autospec=True)
     @mock.patch.object(os.path, 'exists')
     @mock.patch.object(os, 'mkdir')
     @mock.patch.object(processutils, 'execute')
     def test_update_firmware(self, execute_mock, mkdir_mock,
                              exists_mock, mkdtemp_mock, rmtree_mock,
                              listdir_mock, execute_sum_mock,
-                             verify_image_mock, validate_mock):
+                             verify_image_mock, validate_mock, sleep_mock):
         execute_sum_mock.return_value = 'SUCCESS'
         listdir_mock.return_value = ['SPP_LABEL']
         mkdtemp_mock.return_value = "/tempdir"
         null_output = ["", ""]
         exists_mock.side_effect = [True, False]
         execute_mock.side_effect = [null_output, null_output]
-
-        ret_val = sum_controller.update_firmware(self.node)
+        url = "http://a.b.c.d/spp.iso"
+        checksum = "12345678"
+        components = ['abc', 'pqr']
+        ret_val = sum_controller.update_firmware(self.node, url, checksum,
+                                                 components)
 
         execute_mock.assert_any_call('mount', "/dev/disk/by-label/SPP_LABEL",
                                      "/tempdir")
         execute_sum_mock.assert_any_call('/tempdir/hp/swpackages/hpsum',
-                                         '/tempdir',
-                                         components=None)
+                                         '/tempdir', components=components)
         calls = [mock.call("/dev/disk/by-label/SPP_LABEL"),
                  mock.call("/tempdir/packages/smartupdate")]
         exists_mock.assert_has_calls(calls, any_order=False)
         execute_mock.assert_any_call('umount', "/tempdir")
         mkdtemp_mock.assert_called_once_with()
         rmtree_mock.assert_called_once_with("/tempdir", ignore_errors=True)
         self.assertEqual('SUCCESS', ret_val)
 
+    @mock.patch.object(time, 'sleep')
     @mock.patch.object(utils, 'validate_href')
     @mock.patch.object(utils, 'verify_image_checksum')
     @mock.patch.object(sum_controller, '_execute_sum')
     @mock.patch.object(os, 'listdir')
     @mock.patch.object(shutil, 'rmtree', autospec=True)
     @mock.patch.object(tempfile, 'mkdtemp', autospec=True)
     @mock.patch.object(os.path, 'exists')
     @mock.patch.object(os, 'mkdir')
     @mock.patch.object(processutils, 'execute')
     def test_update_firmware_sum(self, execute_mock, mkdir_mock,
                                  exists_mock, mkdtemp_mock, rmtree_mock,
                                  listdir_mock, execute_sum_mock,
-                                 verify_image_mock, validate_mock):
+                                 verify_image_mock, validate_mock, sleep_mock):
         execute_sum_mock.return_value = 'SUCCESS'
         listdir_mock.return_value = ['SPP_LABEL']
         mkdtemp_mock.return_value = "/tempdir"
         null_output = ["", ""]
-        exists_mock.side_effect = [True, True]
-        execute_mock.side_effect = [null_output, null_output]
+        exists_mock.side_effect = [True, True, True, True]
+        execute_mock.side_effect = [null_output, null_output,
+                                    null_output, null_output]
+        url = "http://a.b.c.d/spp.iso"
+        checksum = "12345678"
 
-        ret_val = sum_controller.update_firmware(self.node)
+        ret_val = sum_controller.update_firmware(
+            self.node, url, checksum)
 
-        execute_mock.assert_any_call('mount', "/dev/disk/by-label/SPP_LABEL",
+        execute_mock.assert_any_call('mount',
+                                     "/dev/disk/by-label/SPP_LABEL",
                                      "/tempdir")
         execute_sum_mock.assert_any_call('/tempdir/packages/smartupdate',
                                          '/tempdir',
                                          components=None)
         calls = [mock.call("/dev/disk/by-label/SPP_LABEL"),
                  mock.call("/tempdir/packages/smartupdate")]
         exists_mock.assert_has_calls(calls, any_order=False)
@@ -222,84 +232,103 @@
         rmtree_mock.assert_called_once_with("/tempdir", ignore_errors=True)
         self.assertEqual('SUCCESS', ret_val)
 
     @mock.patch.object(utils, 'validate_href')
     def test_update_firmware_throws_for_nonexistent_file(self,
                                                          validate_href_mock):
         invalid_file_path = '/some/invalid/file/path'
+        url = "http://a.b.c.d/spp.iso"
+        checksum = "12345678"
+        components = ['abc', 'pqr']
         value = ("Got HTTP code 503 instead of 200 in response to "
                  "HEAD request.")
         validate_href_mock.side_effect = exception.ImageRefValidationFailed(
             reason=value, image_href=invalid_file_path)
 
         exc = self.assertRaises(exception.SUMOperationError,
-                                sum_controller.update_firmware, self.node)
+                                sum_controller.update_firmware, self.node,
+                                url, checksum, components)
         self.assertIn(value, str(exc))
 
+    @mock.patch.object(time, 'sleep')
     @mock.patch.object(utils, 'validate_href')
     @mock.patch.object(os.path, 'exists')
     @mock.patch.object(os, 'listdir')
     def test_update_firmware_device_file_not_found(self,
                                                    listdir_mock, exists_mock,
-                                                   validate_mock):
+                                                   validate_mock, sleep_mock):
         listdir_mock.return_value = ['SPP_LABEL']
         exists_mock.return_value = False
+        url = "http://a.b.c.d/spp.iso"
+        checksum = "12345678"
+        components = ['abc', 'pqr']
 
         msg = ("An error occurred while performing SUM based firmware "
                "update, reason: Unable to find the virtual media device "
                "for SUM")
         exc = self.assertRaises(exception.SUMOperationError,
-                                sum_controller.update_firmware, self.node)
+                                sum_controller.update_firmware, self.node,
+                                url, checksum, components=components)
         self.assertEqual(msg, str(exc))
         exists_mock.assert_called_once_with("/dev/disk/by-label/SPP_LABEL")
 
+    @mock.patch.object(time, 'sleep')
     @mock.patch.object(utils, 'validate_href')
     @mock.patch.object(utils, 'verify_image_checksum')
     @mock.patch.object(os, 'listdir')
     @mock.patch.object(os.path, 'exists')
     def test_update_firmware_invalid_checksum(self, exists_mock,
                                               listdir_mock, verify_image_mock,
-                                              validate_mock):
+                                              validate_mock, sleep_mock):
         listdir_mock.return_value = ['SPP_LABEL']
         exists_mock.side_effect = [True, False]
+        url = "http://1.2.3.4/SPP.iso"
+        checksum = "1234567890"
+        components = ['abc', 'pqr']
 
         value = ("Error verifying image checksum. Image "
                  "http://1.2.3.4/SPP.iso failed to verify against checksum "
                  "123456789. Actual checksum is: xxxxxxxx")
 
         verify_image_mock.side_effect = exception.ImageRefValidationFailed(
             reason=value, image_href='http://1.2.3.4/SPP.iso')
 
         self.assertRaisesRegex(exception.SUMOperationError, value,
-                               sum_controller.update_firmware, self.node)
+                               sum_controller.update_firmware, self.node,
+                               url, checksum, components=components)
 
         verify_image_mock.assert_called_once_with(
             '/dev/disk/by-label/SPP_LABEL', '1234567890')
         exists_mock.assert_called_once_with("/dev/disk/by-label/SPP_LABEL")
 
+    @mock.patch.object(time, 'sleep')
     @mock.patch.object(utils, 'validate_href')
     @mock.patch.object(utils, 'verify_image_checksum')
     @mock.patch.object(processutils, 'execute')
     @mock.patch.object(tempfile, 'mkdtemp', autospec=True)
     @mock.patch.object(os, 'mkdir')
     @mock.patch.object(os.path, 'exists')
     @mock.patch.object(os, 'listdir')
     def test_update_firmware_mount_fails(self, listdir_mock,
                                          exists_mock, mkdir_mock,
                                          mkdtemp_mock, execute_mock,
-                                         verify_image_mock, validate_mock):
+                                         verify_image_mock, validate_mock,
+                                         sleep_mock):
         listdir_mock.return_value = ['SPP_LABEL']
         exists_mock.return_value = True
         mkdtemp_mock.return_value = "/tempdir"
         execute_mock.side_effect = processutils.ProcessExecutionError
+        url = "http://a.b.c.d/spp.iso"
+        checksum = "12345678"
 
         msg = ("Unable to mount virtual media device "
                "/dev/disk/by-label/SPP_LABEL")
         exc = self.assertRaises(exception.SUMOperationError,
-                                sum_controller.update_firmware, self.node)
+                                sum_controller.update_firmware, self.node,
+                                url, checksum)
         self.assertIn(msg, str(exc))
         exists_mock.assert_called_once_with("/dev/disk/by-label/SPP_LABEL")
 
     @mock.patch.object(sum_controller,
                        '_get_log_file_data_as_encoded_content')
     @mock.patch.object(sum_controller, 'open',
                        mock.mock_open(read_data=constants.SUM_OUTPUT_DATA))
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/sum/sum_sample_output.py` & `proliantutils-2.9.5/proliantutils/tests/sum/sum_sample_output.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/test_redfish.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/test_redfish.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import collections
+import json
 
 import ddt
-import json
 import mock
 import sushy
-import testtools
-
 from sushy.resources.system import system
+import testtools
 
 from proliantutils import exception
 from proliantutils.ilo import constants as ilo_cons
 from proliantutils.redfish import main
 from proliantutils.redfish import redfish
 from proliantutils.redfish.resources.account_service import account
 from proliantutils.redfish.resources.account_service import account_service
@@ -552,15 +551,15 @@
         (get_system_mock.return_value.update_persistent_boot.
          assert_called_once_with(['NETWORK'], persistent=True))
 
     def test_update_persistent_boot_invalid_input(self):
         self.assertRaisesRegex(
             exception.IloInvalidInputError,
             ('Invalid input "test". Valid devices: NETWORK, '
-             'HDD, ISCSI or CDROM.'),
+             'HDD, ISCSI, UEFIHTTP or CDROM.'),
             self.rf_client.update_persistent_boot, ['test'])
 
     @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
     def test_update_persistent_boot_fail(self, get_system_mock):
         get_system_mock.return_value.update_persistent_boot.side_effect = (
             sushy.exceptions.SushyError)
         self.assertRaisesRegex(
@@ -575,15 +574,15 @@
         (get_system_mock.return_value.update_persistent_boot.
          assert_called_once_with(['CDROM'], persistent=False))
 
     def test_set_one_time_boot_invalid_input(self):
         self.assertRaisesRegex(
             exception.IloInvalidInputError,
             ('Invalid input "test". Valid devices: NETWORK, '
-             'HDD, ISCSI or CDROM.'),
+             'HDD, ISCSI, UEFIHTTP or CDROM.'),
             self.rf_client.set_one_time_boot, 'test')
 
     @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
     def test_set_one_time_boot_fail(self, get_system_mock):
         get_system_mock.return_value.update_persistent_boot.side_effect = (
             sushy.exceptions.SushyError)
         self.assertRaisesRegex(
@@ -1336,15 +1335,15 @@
             self, get_system_mock):
         msg = ("Given macs: %(macs)s not found in the system"
                % {'macs': str(['12:44:6A:3B:04:15'])})
         get_system_mock.return_value.validate_macs.side_effect = (
             exception.InvalidInputError(msg))
         self.assertRaisesRegex(
             exception.InvalidInputError,
-            "Given macs: \['12:44:6A:3B:04:15'\] not found in the system",
+            r"Given macs: \['12:44:6A:3B:04:15'\] not found in the system",
             self.rf_client._change_iscsi_target_settings, {},
             ['12:44:6A:3B:04:15'])
 
     @mock.patch.object(iscsi.ISCSISettings, 'update_iscsi_settings')
     @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
     def test__change_iscsi_target_settings_update_failed(
             self, get_system_mock, update_iscsi_settings_mock):
@@ -1910,7 +1909,198 @@
 
     @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
     def test_get_available_disk_types(self, get_system_mock):
         get_system_mock.return_value.get_disk_types.return_value = ['HDD',
                                                                     'SSD']
         self.assertEqual(
             ['HDD', 'SSD'], self.rf_client.get_available_disk_types())
+
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_get_http_boot_url(self, get_system_mock):
+        with open('proliantutils/tests/redfish/'
+                  'json_samples/bios.json', 'r') as f:
+            jsonval = json.loads(f.read()).get("Default")
+        type(
+            get_system_mock.return_value.bios_settings).json = (
+                mock.PropertyMock(return_value=jsonval))
+        settings = jsonval.get('Attributes')
+        expected_url_boot_file = settings.get('UrlBootFile')
+
+        actual_url_boot_file = self.rf_client.get_http_boot_url()
+        self.assertEqual(expected_url_boot_file, actual_url_boot_file)
+
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_get_http_boot_url_fail(self, get_system_mock):
+        bios_mock = mock.PropertyMock(
+            side_effect=sushy.exceptions.SushyError)
+        type(get_system_mock.return_value).bios_settings = bios_mock
+        self.assertRaisesRegex(
+            exception.IloError,
+            'The attribute "UrlBootFile" not found.',
+            self.rf_client.get_http_boot_url)
+
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_set_http_boot_url_dhcp_default(self, system_mock):
+        bios_ps_mock = mock.MagicMock(spec=bios.BIOSPendingSettings)
+        pending_settings_mock = mock.PropertyMock(return_value=bios_ps_mock)
+        type(system_mock.return_value.bios_settings).pending_settings = (
+            pending_settings_mock)
+
+        url = 'a.b.c'
+        expected_parameter = {
+            'PreBootNetwork': 'Auto',
+            'UrlBootFile': 'a.b.c',
+            'Dhcpv4': 'Enabled'
+        }
+        self.rf_client.set_http_boot_url(url)
+
+        bios_ps_mock.update_bios_data_by_post.assert_called_once_with(
+            expected_parameter)
+
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_set_http_boot_url_dhcp_enabled(self, system_mock):
+        bios_ps_mock = mock.MagicMock(spec=bios.BIOSPendingSettings)
+        pending_settings_mock = mock.PropertyMock(return_value=bios_ps_mock)
+        type(system_mock.return_value.bios_settings).pending_settings = (
+            pending_settings_mock)
+
+        dhcp_enabled = True
+        url = 'a.b.c'
+        expected_parameter = {
+            'PreBootNetwork': 'Auto',
+            'UrlBootFile': 'a.b.c',
+            'Dhcpv4': 'Enabled'
+        }
+        self.rf_client.set_http_boot_url(url, dhcp_enabled)
+
+        bios_ps_mock.update_bios_data_by_post.assert_called_once_with(
+            expected_parameter)
+
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_set_http_boot_url_dhcp_disabled(self, system_mock):
+        bios_ps_mock = mock.MagicMock(spec=bios.BIOSPendingSettings)
+        pending_settings_mock = mock.PropertyMock(return_value=bios_ps_mock)
+        type(system_mock.return_value.bios_settings).pending_settings = (
+            pending_settings_mock)
+
+        dhcp_enabled = False
+        url = 'a.b.c'
+        expected_parameter = {
+            'PreBootNetwork': 'Auto',
+            'UrlBootFile': 'a.b.c',
+            'Dhcpv4': 'Disabled'
+        }
+        self.rf_client.set_http_boot_url(url, dhcp_enabled)
+
+        bios_ps_mock.update_bios_data_by_post.assert_called_once_with(
+            expected_parameter)
+
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_set_http_boot_url_raises_exception(self, system_mock):
+        pending_settings_mock = mock.PropertyMock(
+            side_effect=sushy.exceptions.SushyError)
+
+        type(system_mock.return_value.bios_settings).pending_settings = (
+            pending_settings_mock)
+
+        dhcp_enabled = True
+        url = 'a.b.c'
+        self.assertRaisesRegex(
+            exception.IloError,
+            'Could not set HTTPS URL on the iLO.',
+            self.rf_client.set_http_boot_url, url, dhcp_enabled)
+
+    @mock.patch.object(redfish.RedfishOperations, '_is_boot_mode_uefi')
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_add_tls_certificate_bios(self, get_sushy_system_mock,
+                                      _uefi_boot_mode_mock):
+        _uefi_boot_mode_mock.return_value = False
+        data = {
+            "NewCertificates": [
+                {
+                    "X509Certificate": "Some data"
+                }
+            ]
+        }
+
+        self.assertRaisesRegex(
+            exception.IloCommandNotSupportedInBiosError,
+            'TLS certificate cannot be upload in BIOS boot mode',
+            self.rf_client.add_tls_certificate,
+            data)
+
+    @mock.patch.object(redfish.RedfishOperations, '_is_boot_mode_uefi')
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_add_tls_certificate(self, get_sushy_system_mock,
+                                 _uefi_boot_mode_mock):
+        _uefi_boot_mode_mock.return_value = True
+        cert_file = 'proliantutils/tests/redfish/json_samples/certfile.crt'
+        with open('proliantutils/tests/redfish/'
+                  'json_samples/certfile.crt', 'r') as f:
+            cert_data = f.read()
+
+        import re
+        cert_data = cert_data.rstrip()
+        ref_data = re.sub(r"\n", "\r\n", cert_data)
+
+        data = {
+            "NewCertificates": [
+                {
+                    "X509Certificate": ref_data
+                }
+            ]
+        }
+        self.rf_client.add_tls_certificate([cert_file])
+
+        (get_sushy_system_mock.return_value.
+         bios_settings.tls_config.tls_config_settings.
+         add_tls_certificate.assert_called_once_with(data))
+
+    @mock.patch.object(redfish.RedfishOperations, '_is_boot_mode_uefi')
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_add_tls_certificate_raises_ilo_error(self, get_sushy_system_mock,
+                                                  _uefi_boot_mode_mock):
+        _uefi_boot_mode_mock.return_value = True
+        cert_file = 'proliantutils/tests/redfish/json_samples/certfile.crt'
+        (get_sushy_system_mock.return_value.
+         bios_settings.tls_config.tls_config_settings.
+         add_tls_certificate.side_effect) = (
+             sushy.exceptions.SushyError)
+
+        self.assertRaisesRegex(
+            exception.IloError,
+            'The Redfish controller has failed to upload TLS certificate.',
+            self.rf_client.add_tls_certificate, [cert_file])
+
+    @mock.patch.object(redfish.RedfishOperations, '_is_boot_mode_uefi')
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_remove_tls_certificate(self, get_sushy_system_mock,
+                                    _uefi_boot_mode_mock):
+        _uefi_boot_mode_mock.return_value = True
+        fp = ('FA:3A:68:C7:7E:ED:90:21:D2:FA:3E:54:6B:0C:14:D3:'
+              '2F:8D:43:50:F7:05:A7:0F:1C:68:35:DB:5C:D2:53:28')
+
+        cert = {}
+        del_cert_list = []
+        cert_fp = {
+            "FingerPrint": fp
+        }
+        del_cert_list.append(cert_fp)
+        cert.update({"DeleteCertificates": del_cert_list})
+        self.rf_client.remove_tls_certificate([fp])
+
+        (get_sushy_system_mock.return_value.
+         bios_settings.tls_config.tls_config_settings.
+         remove_tls_certificate.assert_called_once_with(cert))
+
+    @mock.patch.object(redfish.RedfishOperations, '_is_boot_mode_uefi')
+    @mock.patch.object(redfish.RedfishOperations, '_get_sushy_system')
+    def test_remove_tls_certificate_bios(self, get_sushy_system_mock,
+                                         _uefi_boot_mode_mock):
+        _uefi_boot_mode_mock.return_value = False
+        fp = ('FA:3A:68:C7:7E:ED:90:21:D2:FA:3E:54:6B:0C:14:D3:'
+              '2F:8D:43:50:F7:05:A7:0F:1C:68:35:DB:5C:D2:53:28')
+
+        self.assertRaisesRegex(
+            exception.IloCommandNotSupportedInBiosError,
+            'TLS certificate cannot be removed in BIOS boot mode',
+            self.rf_client.remove_tls_certificate, fp)
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/test_connector.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/test_connector.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/manager/test_manager.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/manager/test_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import json
+
 import mock
 import testtools
 
 from proliantutils.redfish.resources.manager import manager
 from proliantutils.redfish.resources.manager import virtual_media
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/manager/test_virtual_media.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/manager/test_virtual_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # under the License.
 
 __author__ = 'HPE'
 
 import json
 
 import mock
-import testtools
-
 from sushy import exceptions
 from sushy.resources.manager import virtual_media as sushy_virt_media
+import testtools
 
 from proliantutils import exception
 from proliantutils.redfish.resources.manager import constants
 from proliantutils.redfish.resources.manager import virtual_media
 
 
 class VirtualMediaCollectionTestCase(testtools.TestCase):
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_iscsi.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_iscsi.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_bios.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_bios.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import sushy
 import testtools
 
 from proliantutils import exception
 from proliantutils.redfish.resources.system import bios
 from proliantutils.redfish.resources.system import constants as sys_cons
 from proliantutils.redfish.resources.system import iscsi
+from proliantutils.redfish.resources.system import tls_config
 
 
 class BIOSSettingsTestCase(testtools.TestCase):
 
     def setUp(self):
         super(BIOSSettingsTestCase, self).setUp()
         self.conn = mock.MagicMock()
@@ -107,14 +108,30 @@
         self.conn.get.return_value.json.assert_called_once_with()
         # reset mock
         self.conn.get.return_value.json.reset_mock()
         self.assertIs(actual_settings,
                       self.bios_inst.iscsi_resource)
         self.conn.get.return_value.json.assert_not_called()
 
+    def test_tls_config(self):
+        self.conn.get.return_value.json.reset_mock()
+        with open('proliantutils/tests/redfish/'
+                  'json_samples/tls_config.json', 'r') as f:
+            self.conn.get.return_value.json.return_value = (
+                json.loads(f.read()))
+        actual_settings = self.bios_inst.tls_config
+        self.assertIsInstance(actual_settings,
+                              tls_config.TLSConfig)
+        self.conn.get.return_value.json.assert_called_once_with()
+        # reset mock
+        self.conn.get.return_value.json.reset_mock()
+        self.assertIs(actual_settings,
+                      self.bios_inst.tls_config)
+        self.conn.get.return_value.json.assert_not_called()
+
     def test__get_base_configs(self):
         with open('proliantutils/tests/redfish/'
                   'json_samples/bios_base_configs.json', 'r') as f:
             self.conn.get.return_value.json.return_value = json.loads(f.read())
         default_settings = self.bios_inst._get_base_configs()
         self.assertIsInstance(default_settings, bios.BIOSBaseConfigs)
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_memory.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_memory.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_system.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import json
 
 import mock
 import sushy
+from sushy.resources.system import system as sushy_system
 import testtools
 
 from proliantutils import exception
 from proliantutils.redfish.resources.system import bios
 from proliantutils.redfish.resources.system import constants as sys_cons
 from proliantutils.redfish.resources.system import ethernet_interface
 from proliantutils.redfish.resources.system import memory
@@ -28,15 +29,14 @@
 from proliantutils.redfish.resources.system import smart_storage_config
 from proliantutils.redfish.resources.system.storage import array_controller
 from proliantutils.redfish.resources.system.storage import simple_storage
 from proliantutils.redfish.resources.system.storage import smart_storage
 from proliantutils.redfish.resources.system.storage import storage
 from proliantutils.redfish.resources.system import system
 from proliantutils.redfish import utils
-from sushy.resources.system import system as sushy_system
 
 
 class HPESystemTestCase(testtools.TestCase):
 
     def setUp(self):
         super(HPESystemTestCase, self).setUp()
         self.conn = mock.MagicMock()
@@ -1171,11 +1171,10 @@
         with open(path, 'r') as f:
             eth_coll = json.loads(f.read())
         self.conn.get.return_value.json.side_effect = [eth_coll]
         get_all_macs_mock.return_value = [
             '12:44:6a:3b:04:11', '13:44:6a:3b:04:13']
         self.assertRaisesRegex(
             exception.InvalidInputError,
-            "Given macs: \['14:23:AD:3B:4C:78'\] "
-            "not found in the system",
+            r"Given macs: \['14:23:AD:3B:4C:78'\] not found in the system",
             self.sys_inst.validate_macs,
             ['12:44:6a:3b:04:11', '14:23:AD:3B:4C:78'])
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_smart_storage_config.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_smart_storage_config.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_pci_device.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_pci_device.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_secure_boot.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_secure_boot.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_physical_drive.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_physical_drive.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_drive.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_drive.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_logical_drive.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_logical_drive.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_volume.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_volume.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_storage.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_array_controller.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_array_controller.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_simple_storage.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_simple_storage.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_smart_storage.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_smart_storage.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/storage/test_common.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/storage/test_common.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/system/test_ethernet_interface.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/system/test_ethernet_interface.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/test_update_service.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/test_update_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import json
+import time
+
 import mock
 import sushy
 import testtools
-import time
 
 from proliantutils import exception
 from proliantutils.ilo import common
 from proliantutils.redfish import main
 from proliantutils.redfish import redfish
 from proliantutils.redfish.resources import update_service
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/account_service/test_account_service.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/account_service/test_account_service.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/resources/account_service/test_account.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/resources/account_service/test_account.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/test_main.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/test_main.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/manager.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/manager.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/pci_device1.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/pci_device1.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_failed.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_failed.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/secure_boot.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/secure_boot.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/storage.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/storage.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/vmedia.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/vmedia.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/array_controller_collection.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/array_controller_collection.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_mappings.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_mappings.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/volume.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/volume.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/account_service.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/account_service.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/ethernet_interface_collection.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/ethernet_interface_collection.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_boot.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_boot.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios_base_configs.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios_base_configs.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/array_controller.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/array_controller.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/logical_nvdimm.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/logical_nvdimm.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/logical_drive_collection.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/logical_drive_collection.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/ethernet_interface.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/ethernet_interface.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/smart_storage_config.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/smart_storage_config.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/drive.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/drive.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/pci_device.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/pci_device.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/disk_drive.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/disk_drive.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/update_service.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/update_service.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/memory_collection.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/memory_collection.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/simple_storage.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/simple_storage.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/system.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/system.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/root.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/root.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/account.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/account.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/disk_drive_collection.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/disk_drive_collection.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/smart_storage.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/smart_storage.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/bios.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/bios.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999748592115849%*

 * *Differences: {"'Default'": "{'Attributes': {'UrlBootFile': 'http://w.x.y.z/ironic.iso'}}"}*

```diff
@@ -452,15 +452,15 @@
             "UefiShellScriptVerification": "Disabled",
             "UefiShellStartup": "Disabled",
             "UefiShellStartupLocation": "Auto",
             "UefiShellStartupUrl": "",
             "UefiShellStartupUrlFromDhcp": "Disabled",
             "UncoreFreqScaling": "Auto",
             "UpiPrefetcher": "Enabled",
-            "UrlBootFile": "",
+            "UrlBootFile": "http://w.x.y.z/ironic.iso",
             "UrlBootFile2": "",
             "UrlBootFile3": "",
             "UrlBootFile4": "",
             "UsbBoot": "Enabled",
             "UsbControl": "UsbEnabled",
             "UserDefaultsState": "Disabled",
             "UtilityLang": "English",
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/iscsi_settings.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/iscsi_settings.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/iscsi.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/iscsi.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/json_samples/logical_drive.json` & `proliantutils-2.9.5/proliantutils/tests/redfish/json_samples/logical_drive.json`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/redfish/test_utils.py` & `proliantutils-2.9.5/proliantutils/tests/redfish/test_utils.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/rest/rest_sample_outputs.py` & `proliantutils-2.9.5/proliantutils/tests/rest/rest_sample_outputs.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/rest/test_v1.py` & `proliantutils-2.9.5/proliantutils/tests/rest/test_v1.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/test_exception.py` & `proliantutils-2.9.5/proliantutils/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/test_firmware_controller.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/test_firmware_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,17 +334,17 @@
         '_ilo', '.bin', '.xml', '.TXT', '.hpsetup', '.cpq_package.inc'
     ]
 
     if format == 'scexe':
         fw_files_dir = temp_dir
     elif format == 'rpm':
         fw_files_dir = os.path.join(
-            temp_dir +
-            '/please_remove_rpm_file_extracts/usr/lib/i386-linux-gnu/' +
-            'hp-firmware-iloX-xxxx'
+            temp_dir
+            + '/please_remove_rpm_file_extracts/usr/lib/i386-linux-gnu/'
+            + 'hp-firmware-iloX-xxxx'
         )
     else:
         fw_files_dir = temp_dir
 
     if not os.path.exists(fw_files_dir):
         os.makedirs(fw_files_dir)
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/test_ris.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/test_ris.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,26 +72,26 @@
                                     get_bios_settings_mock):
         get_bios_settings_mock.return_value = ris_outputs.HTTP_BOOT_URL
         _uefi_boot_mode_mock.return_value = True
         result = self.client.get_http_boot_url()
         _uefi_boot_mode_mock.assert_called_once_with()
         self.assertEqual(
             'http://10.10.1.30:8081/startup.nsh', result['UefiShellStartupUrl']
-            )
+        )
 
     @mock.patch.object(ris.RISOperations, '_change_bios_setting')
     @mock.patch.object(ris.RISOperations, '_is_boot_mode_uefi')
     def test_set_http_boot_url_uefi(self, _uefi_boot_mode_mock,
                                     change_bios_setting_mock):
         _uefi_boot_mode_mock.return_value = True
         self.client.set_http_boot_url('http://10.10.1.30:8081/startup.nsh')
         _uefi_boot_mode_mock.assert_called_once_with()
         change_bios_setting_mock.assert_called_once_with({
             "UefiShellStartupUrl": "http://10.10.1.30:8081/startup.nsh"
-            })
+        })
 
     @mock.patch.object(ris.RISOperations, '_is_boot_mode_uefi')
     def test_get_http_boot_url_bios(self, _uefi_boot_mode_mock):
         _uefi_boot_mode_mock.return_value = False
         self.assertRaises(exception.IloCommandNotSupportedInBiosError,
                           self.client.get_http_boot_url)
         _uefi_boot_mode_mock.assert_called_once_with()
@@ -1803,15 +1803,15 @@
 
     @mock.patch.object(ris.RISOperations, '_get_all_macs')
     def test_validate_macs_failed(self, get_all_macs_mock):
         get_all_macs_mock.return_value = [
             '12:44:6a:3b:04:11', '13:44:6a:3b:04:13']
         self.assertRaisesRegex(
             exception.InvalidInputError,
-            "Given macs: \['12:44:6A:3B:04:15'\] not found in the system",
+            r"Given macs: \['12:44:6A:3B:04:15'\] not found in the system",
             self.client._validate_macs, ['12:44:6A:3B:04:15'])
 
     @mock.patch.object(ris.RISOperations, '_get_collection')
     def test__get_uefi_device_path_by_mac(self, collection_mock):
         member_uri = '/rest/v1/Systems/1/NetworkAdapters'
         collection_item = json.loads(ris_outputs.RESP_NETWORK_ADAPTER)
         collection_mock.return_value = [(200, None, collection_item,
@@ -1879,15 +1879,15 @@
         iscsi_uri = '/rest/v1/systems/1/bios/iScsi/Settings'
         check_iscsi_mock.return_value = iscsi_uri
         msg = ("Given macs: %(macs)s not found in the system"
                % {'macs': str(['12:44:6A:3B:04:15'])})
         validate_macs_mock.side_effect = exception.InvalidInputError(msg)
         self.assertRaisesRegex(
             exception.InvalidInputError,
-            "Given macs: \['12:44:6A:3B:04:15'\] not found in the system",
+            r"Given macs: \['12:44:6A:3B:04:15'\] not found in the system",
             self.client._change_iscsi_settings, {}, ['12:44:6A:3B:04:15'])
 
     @mock.patch.object(ris.RISOperations, '_check_iscsi_rest_patch_allowed')
     @mock.patch.object(ris.RISOperations, '_get_bios_mappings_resource')
     @mock.patch.object(ris.RISOperations, '_check_bios_resource')
     def test__change_iscsi_settings_no_macs(
             self, check_bios_mock, mappings_mock, check_iscsi_mock):
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/test_client.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     @mock.patch.object(ris, 'RISOperations')
     def test_init(self, ris_mock, ribcl_mock):
         ribcl_obj_mock = mock.MagicMock()
         ribcl_mock.return_value = ribcl_obj_mock
         ribcl_obj_mock.get_product_name.return_value = 'product'
 
         c = client.IloClient.cls("1.2.3.4", "admin", "Admin",
-                                 timeout=120,  port=4430,
+                                 timeout=120, port=4430,
                                  bios_password='foo',
                                  cacert='/somewhere')
 
         ris_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", bios_password='foo',
             cacert='/somewhere')
         ribcl_mock.assert_called_once_with(
@@ -153,15 +153,15 @@
     @mock.patch.object(ris, 'RISOperations')
     def test_init_for_ipv6_link_address(self, ris_mock, ribcl_mock):
         ribcl_obj_mock = mock.MagicMock()
         ribcl_mock.return_value = ribcl_obj_mock
         ribcl_obj_mock.get_product_name.return_value = 'product'
 
         c = client.IloClient.cls("FE80::9AF2:B3FF:FEEE:F884%eth0", "admin",
-                                 "Admin", timeout=120,  port=4430,
+                                 "Admin", timeout=120, port=4430,
                                  bios_password='foo',
                                  cacert='/somewhere')
 
         ris_mock.assert_called_once_with(
             "[FE80::9AF2:B3FF:FEEE:F884%eth0]",
             "admin", "Admin", bios_password='foo',
             cacert='/somewhere')
@@ -178,15 +178,15 @@
     @mock.patch.object(ris, 'RISOperations')
     def test_init_for_ipv6_global_address(self, ris_mock, ribcl_mock):
         ribcl_obj_mock = mock.MagicMock()
         ribcl_mock.return_value = ribcl_obj_mock
         ribcl_obj_mock.get_product_name.return_value = 'product'
 
         c = client.IloClient.cls("2001:0db8:85a3::8a2e:0370:7334", "admin",
-                                 "Admin", timeout=120,  port=4430,
+                                 "Admin", timeout=120, port=4430,
                                  bios_password='foo',
                                  cacert='/somewhere')
 
         ris_mock.assert_called_once_with(
             "[2001:0db8:85a3::8a2e:0370:7334]",
             "admin", "Admin", bios_password='foo',
             cacert='/somewhere')
@@ -204,15 +204,15 @@
     def test_init_for_redfish_with_ribcl_enabled(
             self, redfish_mock, ribcl_mock):
         ribcl_obj_mock = mock.MagicMock()
         ribcl_mock.return_value = ribcl_obj_mock
         ribcl_obj_mock.get_product_name.return_value = 'ProLiant DL180 Gen10'
 
         c = client.IloClient.cls("1.2.3.4", "admin", "Admin",
-                                 timeout=120,  port=4430,
+                                 timeout=120, port=4430,
                                  bios_password='foo',
                                  cacert='/somewhere')
 
         ribcl_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", 120, 4430, cacert='/somewhere')
         redfish_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", bios_password='foo',
@@ -231,15 +231,15 @@
             self, redfish_mock, ribcl_mock):
         ribcl_obj_mock = mock.MagicMock()
         ribcl_mock.return_value = ribcl_obj_mock
         ribcl_obj_mock.get_product_name.side_effect = (
             exception.IloError('RIBCL is disabled'))
 
         c = client.IloClient.cls("1.2.3.4", "admin", "Admin",
-                                 timeout=120,  port=4430,
+                                 timeout=120, port=4430,
                                  bios_password='foo',
                                  cacert='/somewhere')
 
         ribcl_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", 120, 4430, cacert='/somewhere')
         redfish_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", bios_password='foo',
@@ -254,15 +254,15 @@
 
     @mock.patch.object(ribcl, 'RIBCLOperations')
     @mock.patch.object(redfish, 'RedfishOperations')
     def test_init_with_use_redfish_only_set(
             self, redfish_mock, ribcl_mock):
 
         c = client.IloClient.cls("1.2.3.4", "admin", "Admin",
-                                 timeout=120,  port=4430,
+                                 timeout=120, port=4430,
                                  bios_password='foo', cacert='/somewhere',
                                  use_redfish_only=True)
         ribcl_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", 120, 4430, cacert='/somewhere')
         redfish_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", bios_password='foo',
             cacert='/somewhere')
@@ -286,15 +286,15 @@
                             'auth_protocol': 'SHA',
                             'auth_prot_pp': '1234',
                             'priv_protocol': 'AES',
                             'auth_priv_pp': '4321',
                             'snmp_inspection': 'true'}
 
         c = client.IloClient.cls("1.2.3.4", "admin", "Admin",
-                                 timeout=120,  port=4430,
+                                 timeout=120, port=4430,
                                  bios_password='foo',
                                  cacert='/somewhere',
                                  snmp_credentials=snmp_credentials)
 
         ris_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", bios_password='foo',
             cacert='/somewhere')
@@ -317,15 +317,15 @@
         snmp_credentials = {'auth_user': 'user',
                             'auth_protocol': 'SHA',
                             'priv_protocol': 'AES',
                             'snmp_inspection': 'true'}
 
         self.assertRaises(exception.IloInvalidInputError, client.IloClient.cls,
                           "1.2.3.4", "admin", "Admin",
-                          timeout=120,  port=4430,
+                          timeout=120, port=4430,
                           bios_password='foo',
                           cacert='/somewhere',
                           snmp_credentials=snmp_credentials)
 
         ris_mock.assert_called_once_with(
             "1.2.3.4", "admin", "Admin", bios_password='foo',
             cacert='/somewhere')
@@ -1407,16 +1407,16 @@
                         eval('self.client.' + redfish_method_name)(
                             *method_args)
                     else:
                         eval('self.client.' + redfish_method_name)()
                     if redfish_method_name not in ('unset_iscsi_boot_info',
                                                    'set_iscsi_boot_info'):
                         self.assertTrue(eval(
-                            'self.redfish_mock.return_value.' +
-                            redfish_method_name).called)
+                            'self.redfish_mock.return_value.'
+                            + redfish_method_name).called)
                     validate_method_calls.no_test_cases += 1
                 except TypeError:
                     missed_ops.append(redfish_method_name)
 
         validate_method_calls.no_test_cases = 0
         missed_operations = []
         validate_method_calls(
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/ribcl_sample_outputs.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/ribcl_sample_outputs.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/ris_sample_outputs.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/ris_sample_outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # under the License.
 
 # Flake doesn't allow files without anything. Remove on first commit.
 MODULE = "RIS"
 
 HTTP_BOOT_URL = {
     "UefiShellStartupUrl": "http://10.10.1.30:8081/startup.nsh"
-    }
+}
 
 RESPONSE_BODY_FOR_REST_OP = """
 {
     "AssetTag": "",
     "AvailableActions": [
         {
             "Action": "Reset",
@@ -370,22 +370,20 @@
 REST_GET_SECURE_BOOT = {
     "Name": "SecureBoot",
     "ResetAllKeys": True,
     "ResetToDefaultKeys": True,
     "SecureBootCurrentState": False,
     "SecureBootEnable": True,
     "Type": "HpSecureBoot.0.9.5",
-    "links":
-        {
-            "self":
-                {
-                    "href": "/rest/v1/Systems/1/SecureBoot"
-                }
+    "links": {
+        "self": {
+            "href": "/rest/v1/Systems/1/SecureBoot"
         }
     }
+}
 
 REST_FAILURE_OUTPUT = {
     'Type': 'ExtendedError.1.0.0',
     'Messages': [{'MessageID': 'Base.0.0.FakeFailureMessage'}],
     'Name': 'Extended Error Information'
 }
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/ipmi_sample_outputs.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/ipmi_sample_outputs.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/snmp/snmp_sample_output.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/snmp/snmp_sample_output.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/snmp/test_snmp_cpqdisk_sizes.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/snmp/test_snmp_cpqdisk_sizes.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                           {'cpqDaPhyDrvSize': '286102'},
                           'SNMPv2-SMI::enterprises.232.3.2.5.1.1.45.2.2':
                           {'cpqDaPhyDrvSize': '572316'},
                           'SNMPv2-SMI::enterprises.232.3.2.5.1.1.45.2.3':
                           {'cpqDaPhyDrvSize': '286102'}}
         get_disk_mock.return_value = disk_snmp_data
         actual_size = snmp.get_local_gb(iLOIp, snmp_credentials)
-        expected_size = (572316/1024)
+        expected_size = (572316 / 1024)
         self.assertEqual(actual_size, expected_size)
         get_disk_mock.assert_called_once_with(iLOIp, snmp_credentials)
 
     @mock.patch.object(snmp, '_parse_mibs')
     def test__get_disksize_MiB(self, mib_mock):
         iLOIP = 'a.b.c.d'
         snmp_credentials = {'auth_user': 'user',
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/test_ribcl.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/test_ribcl.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import xml.etree.ElementTree as ET
 
 import ddt
 import mock
 import requests
 from requests.packages import urllib3
 from requests.packages.urllib3 import exceptions as urllib3_exceptions
+import xmltodict
 
 from proliantutils import exception
 from proliantutils.ilo import common
 from proliantutils.ilo import constants as cons
 from proliantutils.ilo import ribcl
 from proliantutils.tests.ilo import ribcl_sample_outputs as constants
 
@@ -98,14 +99,15 @@
 class IloRibclTestCase(unittest.TestCase):
 
     def setUp(self):
         super(IloRibclTestCase, self).setUp()
         self.ilo = ribcl.RIBCLOperations("x.x.x.x", "admin",
                                          "Admin", 60, 443)
         self.ilo.init_model_based_tags('ProLiant DL580 Gen8')
+        self.maxDiff = None
 
     def test_init_model_based_tags_gen7(self):
         self.ilo.init_model_based_tags('Proliant DL380 G7')
         self.assertEqual(self.ilo.MEMORY_SIZE_TAG, "MEMORY_SIZE")
         self.assertEqual(self.ilo.MEMORY_SIZE_NOT_PRESENT_TAG, "Not Installed")
         self.assertEqual(self.ilo.NIC_INFORMATION_TAG, "NIC_INFOMATION")
 
@@ -232,22 +234,22 @@
         result = self.ilo.get_host_power_status()
         self.assertIn('ON', result)
 
     def test_get_http_boot_url(self):
         self.assertRaises(
             exception.IloCommandNotSupportedError,
             self.ilo.get_http_boot_url
-            )
+        )
 
     def test_set_http_boot_url(self):
         self.assertRaises(
             exception.IloCommandNotSupportedError,
             self.ilo.set_http_boot_url,
             'http://10.10.1.30:8081/startup.nsh'
-            )
+        )
 
     @mock.patch.object(ribcl.RIBCLOperations, '_request_ilo')
     def test_reset_server(self, request_ilo_mock):
         request_ilo_mock.return_value = constants.RESET_SERVER_XML
         result = self.ilo.reset_server()
         self.assertIn('server being reset', result.lower())
 
@@ -824,23 +826,27 @@
         os_mock.path.getsize.return_value = 12345
         # | WHEN |
         self.ilo.update_firmware('raw_fw_file.bin', 'ilo')
         # | THEN |
         upload_file_to_mock.assert_called_once_with(
             (self.ilo.host, self.ilo.port), self.ilo.timeout)
 
-        root_xml_string = constants.UPDATE_ILO_FIRMWARE_INPUT_XML % (
+        ref_root_xml_string = constants.UPDATE_ILO_FIRMWARE_INPUT_XML % (
             self.ilo.password, self.ilo.login, 12345, 'raw_fw_file.bin')
-        root_xml_string = re.sub('\n\s*', '', root_xml_string)
+        ref_root_xml_string = re.sub(r"\n\s*", '', ref_root_xml_string)
+        ref_dict = xmltodict.parse(ref_root_xml_string)
+        ref_string = json.dumps(ref_dict, sort_keys=True)
 
         ((ribcl_obj, xml_elem), the_ext_header_dict) = (
             _request_ilo_mock.call_args)
 
-        self.assertEqual(root_xml_string,
-                         ET.tostring(xml_elem).decode('latin-1'))
+        actual_dict = xmltodict.parse(ET.tostring(xml_elem).decode('latin-1'))
+        actual_string = json.dumps(actual_dict, sort_keys=True)
+        self.assertEqual(ref_string, actual_string)
+
         self.assertDictEqual(the_ext_header_dict['extra_headers'],
                              {'Cookie': 'hickory-dickory-dock'})
 
         _parse_output_mock.assert_called_once_with(
             self.ilo, _request_ilo_mock.return_value)
 
     @mock.patch.object(
@@ -858,23 +864,27 @@
         os_mock.path.getsize.return_value = 12345
         # | WHEN |
         self.ilo.update_firmware('raw_fw_file.bin', 'power_pic')
         # | THEN |
         upload_file_to_mock.assert_called_once_with(
             (self.ilo.host, self.ilo.port), self.ilo.timeout)
 
-        root_xml_string = constants.UPDATE_NONILO_FIRMWARE_INPUT_XML % (
+        ref_root_xml_string = constants.UPDATE_NONILO_FIRMWARE_INPUT_XML % (
             self.ilo.password, self.ilo.login, 12345, 'raw_fw_file.bin')
-        root_xml_string = re.sub('\n\s*', '', root_xml_string)
+        ref_root_xml_string = re.sub(r"\n\s*", '', ref_root_xml_string)
+        ref_dict = xmltodict.parse(ref_root_xml_string)
+        ref_string = json.dumps(ref_dict, sort_keys=True)
 
         ((ribcl_obj, xml_elem), the_ext_header_dict) = (
             _request_ilo_mock.call_args)
 
-        self.assertEqual(root_xml_string,
-                         ET.tostring(xml_elem).decode('latin-1'))
+        actual_dict = xmltodict.parse(ET.tostring(xml_elem).decode('latin-1'))
+        actual_string = json.dumps(actual_dict, sort_keys=True)
+        self.assertEqual(ref_string, actual_string)
+
         self.assertDictEqual(the_ext_header_dict['extra_headers'],
                              {'Cookie': 'hickory-dickory-dock'})
 
         _parse_output_mock.assert_called_once_with(
             self.ilo, _request_ilo_mock.return_value)
 
     def test_update_firmware_throws_error_for_invalid_component(self):
@@ -1087,9 +1097,10 @@
     @mock.patch.object(ribcl.RIBCLOperations, 'get_product_name')
     def test_get_bios_settings_result(self, product_name_mock):
         product_name_mock.return_value = constants.GET_PRODUCT_NAME
         self.assertRaisesRegexp(exception.IloCommandNotSupportedError,
                                 'ProLiant DL380 G7',
                                 self.ilo.get_bios_settings_result)
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/test_common.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/test_common.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/test_operations.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/test_operations.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/ilo/test_ipmi.py` & `proliantutils-2.9.5/proliantutils/tests/ilo/test_ipmi.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/tests/test_utils.py` & `proliantutils-2.9.5/proliantutils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/functests/test_hpssa.py` & `proliantutils-2.9.5/proliantutils/functests/test_hpssa.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/rest/v1.py` & `proliantutils-2.9.5/proliantutils/rest/v1.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/firmware_controller.py` & `proliantutils-2.9.5/proliantutils/ilo/firmware_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,32 +131,32 @@
         """
         self.hostname, self.port = addressinfo
         self.timeout = timeout
         filename = self.fw_file
 
         firmware = open(filename, 'rb').read()
         # generate boundary
-        boundary = b('------hpiLO3t' +
-                     str(random.randint(100000, 1000000)) + 'z')
+        boundary = b('------hpiLO3t'
+                     + str(random.randint(100000, 1000000)) + 'z')
 
         while boundary in firmware:
-            boundary = b('------hpiLO3t' +
-                         str(random.randint(100000, 1000000)) + 'z')
+            boundary = b('------hpiLO3t'
+                         + str(random.randint(100000, 1000000)) + 'z')
         # generate body parts
         parts = [
             # body1
-            b("--") + boundary +
-            b("""\r\nContent-Disposition: form-data; """
-              """name="fileType"\r\n\r\n"""),
+            b("--") + boundary
+            + b("""\r\nContent-Disposition: form-data; """
+                """name="fileType"\r\n\r\n"""),
             # body2
-            b("\r\n--") + boundary +
-            b('''\r\nContent-Disposition: form-data; name="fwimgfile"; '''
-              '''filename="''') +
-            b(filename) +
-            b('''"\r\nContent-Type: application/octet-stream\r\n\r\n'''),
+            b("\r\n--") + boundary
+            + b('''\r\nContent-Disposition: form-data; name="fwimgfile"; '''
+                '''filename="''')
+            + b(filename)
+            + b('''"\r\nContent-Type: application/octet-stream\r\n\r\n'''),
             # firmware image
             firmware,
             # body3
             b("\r\n--") + boundary + b("--\r\n"),
         ]
         total_bytes = sum([len(x) for x in parts])
         sock = self._get_socket()
@@ -230,16 +230,16 @@
             raise err
 
         # wrapping the socket over ssl session
         try:
             return ssl.wrap_socket(sock, ssl_version=sslversion)
         except socket.sslerror:
             e = sys.exc_info()[1]
-            msg = (getattr(e, 'reason', None) or
-                   getattr(e, 'message', None))
+            msg = (getattr(e, 'reason', None)
+                   or getattr(e, 'message', None))
             # Some older iLO s don't support TLSv1, retry with SSLv3
             if ('wrong version number' in msg) and (
                     sslversion == ssl.PROTOCOL_TLSv1):
 
                 return self._get_socket(ssl.PROTOCOL_SSLv3)
 
             raise exception.IloConnectionError(
@@ -407,13 +407,13 @@
     #
     #    [TEMP_DIR]/xxx-xxx_actual_firmware_filename
     #
     # e.g. /tmp/77e8f689-f32c-4727-9fc3-a7dacefe67e4_ilo4_210.bin
     file_name, file_ext_with_dot = common.get_filename_and_extension_of(
         firmware_file_path)
     new_firmware_file_path = os.path.join(
-        tempfile.gettempdir(), str(uuid.uuid4()) + '_' +
-        file_name + file_ext_with_dot)
+        tempfile.gettempdir(), str(uuid.uuid4())
+        + '_' + file_name + file_ext_with_dot)
 
     # create a hard link to the raw firmware file
     os.link(firmware_file_path, new_firmware_file_path)
     return new_firmware_file_path
```

### Comparing `proliantutils-2.9.4/proliantutils/ilo/ris.py` & `proliantutils-2.9.5/proliantutils/ilo/ris.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 __author__ = 'HPE'
 
 import hashlib
+
 import retrying
 
 from proliantutils import exception
 from proliantutils.ilo import common
 from proliantutils.ilo import constants
 from proliantutils.ilo import firmware_controller
 from proliantutils.ilo import mappings
@@ -109,26 +110,26 @@
                     # supply that for convenience.
                     memberuri = None
                     if 'links' in item and 'self' in item['links']:
                         memberuri = item['links']['self']['href']
                     yield 200, None, item, memberuri
 
             # else walk the member links
-            elif ('links' in thecollection and
-                  'Member' in thecollection['links']):
+            elif ('links' in thecollection
+                  and 'Member' in thecollection['links']):
                 # iterate members
                 for memberuri in thecollection['links']['Member']:
                     # for each member return the resource indicated by the
                     # member link
                     status, headers, member = self._rest_get(memberuri['href'])
                     yield status, headers, member, memberuri['href']
 
             # page forward if there are more pages in the collection
-            if ('links' in thecollection and
-                    'NextPage' in thecollection['links']):
+            if ('links' in thecollection
+                    and 'NextPage' in thecollection['links']):
                 next_link_uri = (collection_uri + '?page=' + str(
                                  thecollection['links']['NextPage']['page']))
                 status, headers, thecollection = self._rest_get(next_link_uri)
 
             # else we are finished iterating the collection
             else:
                 break
@@ -155,16 +156,16 @@
         the with its own schema.  This function knows how to parse the
         ExtendedError object and, using any loaded message registries,
         render an array of plain language strings that represent
         the response.
         """
         messages = []
         if isinstance(extended_error, dict):
-            if ('Type' in extended_error and
-                    extended_error['Type'].startswith('ExtendedError.')):
+            if ('Type' in extended_error
+                    and extended_error['Type'].startswith('ExtendedError.')):
                 for msg in extended_error['Messages']:
                     message_id = msg['MessageID']
                     x = message_id.split('.')
                     registry = x[0]
                     msgkey = x[len(x) - 1]
 
                     # if the correct message registry is loaded,
@@ -172,20 +173,20 @@
                     if (registry in self.message_registries and msgkey in
                             self.message_registries[registry]['Messages']):
                         rmsgs = self.message_registries[registry]['Messages']
                         msg_dict = rmsgs[msgkey]
                         msg_str = message_id + ':  ' + msg_dict['Message']
 
                         for argn in range(0, msg_dict['NumberOfArgs']):
-                            subst = '%' + str(argn+1)
+                            subst = '%' + str(argn + 1)
                             m = str(msg['MessageArgs'][argn])
                             msg_str = msg_str.replace(subst, m)
 
-                        if ('Resolution' in msg_dict and
-                                msg_dict['Resolution'] != 'None'):
+                        if ('Resolution' in msg_dict
+                                and msg_dict['Resolution'] != 'None'):
                             msg_str += '  ' + msg_dict['Resolution']
 
                         messages.append(msg_str)
                     else:
                         # no message registry, simply return the msg object
                         # in string form
                         messages.append(str(message_id))
@@ -212,16 +213,16 @@
 
         return system
 
     def _check_bios_resource(self, properties=[]):
         """Check if the bios resource exists."""
 
         system = self._get_host_details()
-        if ('links' in system['Oem']['Hp'] and
-                'BIOS' in system['Oem']['Hp']['links']):
+        if ('links' in system['Oem']['Hp']
+                and 'BIOS' in system['Oem']['Hp']['links']):
             # Get the BIOS URI and Settings
             bios_uri = system['Oem']['Hp']['links']['BIOS']['href']
             status, headers, bios_settings = self._rest_get(bios_uri)
 
             if status >= 300:
                 msg = self._get_extended_error(bios_settings)
                 raise exception.IloError(msg)
@@ -247,16 +248,16 @@
         :returns: PCI devices list if the pci resource exist.
         :raises: IloCommandNotSupportedError if the PCI resource
             doesn't exist.
         :raises: IloError, on an error from iLO.
         """
 
         system = self._get_host_details()
-        if ('links' in system['Oem']['Hp'] and
-                'PCIDevices' in system['Oem']['Hp']['links']):
+        if ('links' in system['Oem']['Hp']
+                and 'PCIDevices' in system['Oem']['Hp']['links']):
             # Get the PCI URI and Settings
             pci_uri = system['Oem']['Hp']['links']['PCIDevices']['href']
             status, headers, pci_device_list = self._rest_get(pci_uri)
 
             if status >= 300:
                 msg = self._get_extended_error(pci_device_list)
                 raise exception.IloError(msg)
@@ -284,16 +285,16 @@
         """Gets the SmartStorage resource if exists.
 
         :raises: IloCommandNotSupportedError if the resource SmartStorage
             doesn't exist.
         :returns the tuple of SmartStorage URI, Headers and settings.
         """
         system = self._get_host_details()
-        if ('links' in system['Oem']['Hp'] and
-                'SmartStorage' in system['Oem']['Hp']['links']):
+        if ('links' in system['Oem']['Hp']
+                and 'SmartStorage' in system['Oem']['Hp']['links']):
             # Get the SmartStorage URI and Settings
             storage_uri = system['Oem']['Hp']['links']['SmartStorage']['href']
             status, headers, storage_settings = self._rest_get(storage_uri)
 
             if status >= 300:
                 msg = self._get_extended_error(storage_settings)
                 raise exception.IloError(msg)
@@ -311,16 +312,16 @@
             doesn't exist.
         :returns the tuple of SmartStorage URI, Headers and settings.
         """
         headers, storage_uri, storage_settings = self._get_storage_resource()
         # Do not raise exception if there is no ArrayControllers
         # as Storage can be zero at any point and if we raise
         # exception it might fail get_server_capabilities().
-        if ('links' in storage_settings and
-                'ArrayControllers' in storage_settings['links']):
+        if ('links' in storage_settings
+                and 'ArrayControllers' in storage_settings['links']):
             # Get the ArrayCOntrollers URI and Settings
             array_uri = storage_settings['links']['ArrayControllers']['href']
             status, headers, array_settings = self._rest_get(array_uri)
 
             if status >= 300:
                 msg = self._get_extended_error(array_settings)
                 raise exception.IloError(msg)
@@ -334,16 +335,16 @@
         """
         headers, array_uri, array_settings = (
             self._get_array_controller_resource())
         array_uri_links = []
         # Do not raise exception if there is no ArrayControllers
         # as Storage can be zero at any point and if we raise
         # exception it might fail get_server_capabilities().
-        if ('links' in array_settings and
-                'Member' in array_settings['links']):
+        if ('links' in array_settings
+                and 'Member' in array_settings['links']):
             array_uri_links = array_settings['links']['Member']
         return array_uri_links
 
     def _get_drive_type_and_speed(self):
         """Gets the disk drive type.
 
         :returns: A dictionary with the following keys:
@@ -395,21 +396,21 @@
         # Do not raise exception if there is no disk/logical drive
         # as Storage can be zero at any point and if we raise
         # exception it might fail get_server_capabilities().
         for array_link in array_uri_links:
             _, _, member_settings = (
                 self._rest_get(array_link['href']))
 
-            if ('links' in member_settings and
-                    drive_name in member_settings['links']):
+            if ('links' in member_settings
+                    and drive_name in member_settings['links']):
                 disk_uri = member_settings['links'][drive_name]['href']
                 headers, disk_member_uri, disk_mem = (
                     self._rest_get(disk_uri))
-                if ('links' in disk_mem and
-                        'Member' in disk_mem['links']):
+                if ('links' in disk_mem
+                        and 'Member' in disk_mem['links']):
                     for disk_link in disk_mem['links']['Member']:
                         diskdrive_uri = disk_link['href']
                         _, _, disk_details = (
                             self._rest_get(diskdrive_uri))
                         disk_details_list.append(disk_details)
         if disk_details_list:
             return disk_details_list
@@ -467,17 +468,16 @@
             raise exception.IloError(msg)
 
         return headers, bios_settings_uri, bios_settings
 
     def _validate_if_patch_supported(self, headers, uri):
         """Check if the PATCH Operation is allowed on the resource."""
         if not self._operation_allowed(headers, 'PATCH'):
-                msg = ('PATCH Operation not supported on the resource '
-                       '"%s"' % uri)
-                raise exception.IloError(msg)
+            msg = ('PATCH Operation not supported on the resource "%s"' % uri)
+            raise exception.IloError(msg)
 
     def _get_bios_setting(self, bios_property):
         """Retrieves bios settings of the server."""
         headers, bios_uri, bios_settings = self._check_bios_resource([
             bios_property])
         return bios_settings[bios_property]
 
@@ -708,16 +708,16 @@
             msg = self._get_extended_error(response)
             raise exception.IloError(msg)
 
     def _change_secure_boot_settings(self, property, value):
         """Change secure boot settings on the server."""
         system = self._get_host_details()
         # find the BIOS URI
-        if ('links' not in system['Oem']['Hp'] or
-           'SecureBoot' not in system['Oem']['Hp']['links']):
+        if ('links' not in system['Oem']['Hp']
+                or 'SecureBoot' not in system['Oem']['Hp']['links']):
             msg = (' "SecureBoot" resource or feature is not '
                    'supported on this system')
             raise exception.IloCommandNotSupportedError(msg)
 
         secure_boot_uri = system['Oem']['Hp']['links']['SecureBoot']['href']
 
         # Change the property required
@@ -731,15 +731,15 @@
         if status >= 300:
             msg = self._get_extended_error(response)
             raise exception.IloError(msg)
 
         # Change the bios setting as a workaround to enable secure boot
         # Can be removed when fixed for Gen9 snap2
         val = self._get_bios_setting('CustomPostMessage')
-        val = val.rstrip() if val.endswith(" ") else val+" "
+        val = val.rstrip() if val.endswith(" ") else val + " "
         self._change_bios_setting({'CustomPostMessage': val})
 
     def _is_boot_mode_uefi(self):
         """Checks if the system is in uefi boot mode.
 
         :return: 'True' if the boot mode is uefi else 'False'
         :raises: IloError, on an error from iLO.
@@ -767,16 +767,16 @@
         :returns: True, if enabled, else False
         :raises: IloError, on an error from iLO.
         :raises: IloCommandNotSupportedError, if the command is not supported
                  on the server.
         """
         system = self._get_host_details()
 
-        if ('links' not in system['Oem']['Hp'] or
-           'SecureBoot' not in system['Oem']['Hp']['links']):
+        if ('links' not in system['Oem']['Hp']
+                or 'SecureBoot' not in system['Oem']['Hp']['links']):
             msg = ('"SecureBoot" resource or feature is not supported'
                    ' on this system')
             raise exception.IloCommandNotSupportedError(msg)
 
         secure_boot_uri = system['Oem']['Hp']['links']['SecureBoot']['href']
 
         # get the Secure Boot object
@@ -1130,16 +1130,16 @@
             SUPPORTED_BOOT_MODE_LEGACY_BIOS_ONLY,
             SUPPORTED_BOOT_MODE_UEFI_ONLY,
             SUPPORTED_BOOT_MODE_LEGACY_BIOS_AND_UEFI
 
         """
         system = self._get_host_details()
         bios_uefi_class_val = 0  # value for bios_only boot mode
-        if ('Bios' in system['Oem']['Hp'] and
-                'UefiClass' in system['Oem']['Hp']['Bios']):
+        if ('Bios' in system['Oem']['Hp']
+                and 'UefiClass' in system['Oem']['Hp']['Bios']):
             bios_uefi_class_val = (system['Oem']['Hp']
                                          ['Bios']['UefiClass'])
         return mappings.GET_SUPPORTED_BOOT_MODE_RIS_MAP.get(
             bios_uefi_class_val)
 
     def reset_ilo_credential(self, password):
         """Resets the iLO password.
@@ -1357,36 +1357,36 @@
         # Perform POST to activate license
         status, headers, response = self._rest_post(lic_uri, None, lic_key)
 
         if status >= 300:
             msg = self._get_extended_error(response)
             raise exception.IloError(msg)
 
-    def _get_vm_device_status(self,  device='FLOPPY'):
+    def _get_vm_device_status(self, device='FLOPPY'):
         """Returns the given virtual media device status and device URI
 
         :param  device: virtual media device to be queried
         :returns json format virtual media device status and its URI
         :raises: IloError, on an error from iLO.
         :raises: IloCommandNotSupportedError, if the command is not supported
                  on the server.
         """
         valid_devices = {'FLOPPY': 'floppy',
                          'CDROM': 'cd'}
 
         # Check if the input is valid
         if device not in valid_devices:
-                raise exception.IloInvalidInputError(
-                    "Invalid device. Valid devices: FLOPPY or CDROM.")
+            raise exception.IloInvalidInputError(
+                "Invalid device. Valid devices: FLOPPY or CDROM.")
 
         manager, uri = self._get_ilo_details()
         try:
             vmedia_uri = manager['links']['VirtualMedia']['href']
         except KeyError:
-            msg = ('"VirtualMedia" section in Manager/links does not exist')
+            msg = '"VirtualMedia" section in Manager/links does not exist'
             raise exception.IloCommandNotSupportedError(msg)
 
         for status, hds, vmed, memberuri in self._get_collection(vmedia_uri):
             status, headers, response = self._rest_get(memberuri)
             if status != 200:
                 msg = self._get_extended_error(response)
                 raise exception.IloError(msg)
@@ -1443,16 +1443,16 @@
         else:
             response_data['VM_APPLET'] = 'CONNECTED'
 
         response_data['IMAGE_URL'] = response['Image']
         response_data['DEVICE'] = device
 
         # FLOPPY cannot be a boot device
-        if ((response_data['BOOT_OPTION'] == 'BOOT_ONCE') and
-           (response_data['DEVICE'] == 'FLOPPY')):
+        if ((response_data['BOOT_OPTION'] == 'BOOT_ONCE')
+                and (response_data['DEVICE'] == 'FLOPPY')):
             response_data['BOOT_OPTION'] = 'NO_BOOT'
 
         return response_data
 
     def set_vm_status(self, device='FLOPPY',
                       boot_option='BOOT_ONCE', write_protect='YES'):
         """Sets the Virtual Media drive status
@@ -1619,17 +1619,17 @@
         except KeyError as e:
             msg = "get_persistent_boot_device failed with the KeyError:%s"
             raise exception.IloError((msg) % e)
 
         if 'HP iLO Virtual USB CD' in boot_string:
             return 'CDROM'
 
-        elif ('NIC' in boot_string or
-              'PXE' in boot_string or
-              "iSCSI" in boot_string):
+        elif ('NIC' in boot_string
+              or 'PXE' in boot_string
+              or "iSCSI" in boot_string):
             return 'NETWORK'
 
         elif common.isDisk(boot_string):
             return 'HDD'
 
         else:
             return None
@@ -1653,15 +1653,15 @@
             new_device = DEVICE_COMMON_TO_RIS[device_type[0].upper()]
 
         if persistent:
             tenure = 'Continuous'
 
         systems_uri = "/rest/v1/Systems/1"
         # Need to set this option first if device is 'UefiTarget'
-        if new_device is 'UefiTarget':
+        if new_device == 'UefiTarget':
             system = self._get_host_details()
             uefi_devices = (
                 system['Boot']['UefiTargetBootSourceOverrideSupported'])
             iscsi_device = None
             for device in uefi_devices:
                 if device is not None and 'iSCSI' in device:
                     iscsi_device = device
```

### Comparing `proliantutils-2.9.4/proliantutils/ilo/ipmi.py` & `proliantutils-2.9.5/proliantutils/ilo/ipmi.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/mappings.py` & `proliantutils-2.9.5/proliantutils/ilo/mappings.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/operations.py` & `proliantutils-2.9.5/proliantutils/ilo/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -529,7 +529,27 @@
 
         :returns: List of disk types available in the server.
         :raises: IloError, on an error from iLO.
         :raises: IloCommandNotSupportedError, if the command is
                  not supported on the server.
         """
         raise exception.IloCommandNotSupportedError(ERRMSG)
+
+    def add_tls_certificate(self, cert_file_list):
+        """Adds the TLS certificate to the iLO
+
+        :param cert_file_list: List of TLS certificate files
+        :raises: IloError, on an error from iLO.
+        :raises: IloCommandNotSupportedError, if the command is
+                 not supported on the server.
+        """
+        raise exception.IloCommandNotSupportedError(ERRMSG)
+
+    def remove_tls_certificate(self, fp_list):
+        """Removes the TLS certificate from the iLO
+
+        :param fp_list: List of finger prints of the certificates
+        :raises: IloError, on an error from iLO.
+        :raises: IloCommandNotSupportedError, if the command is
+                 not supported on the server.
+        """
+        raise exception.IloCommandNotSupportedError(ERRMSG)
```

### Comparing `proliantutils-2.9.4/proliantutils/ilo/ribcl.py` & `proliantutils-2.9.5/proliantutils/ilo/ribcl.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,16 +312,16 @@
                             raise (exception.IloCommandNotSupportedError
                                    (msg, status))
                     else:
                         LOG.debug(self._("Got invalid response with "
                                          "message: '%(message)s'"),
                                   {'message': msg})
                         raise exception.IloClientInternalError(msg, status)
-                if (status in exception.IloLoginFailError.statuses or
-                        msg in exception.IloLoginFailError.messages):
+                if (status in exception.IloLoginFailError.statuses
+                        or msg in exception.IloLoginFailError.messages):
                     LOG.debug(self._("Got invalid response with "
                                      "message: '%(message)s'"),
                               {'message': msg})
                     raise exception.IloLoginFailError(msg, status)
 
                 LOG.debug(self._("Got invalid response with "
                                  "message: '%(message)s'"),
```

### Comparing `proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/CPQHOST-MIB.py` & `proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/CPQHOST-MIB.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/CPQIDA-MIB.py` & `proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/CPQIDA-MIB.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/RFC1215-MIB.py` & `proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/RFC1215-MIB.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/IANAifType-MIB.py` & `proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/IANAifType-MIB.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/CPQSCSI-MIB.py` & `proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/CPQSCSI-MIB.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/snmp/cpqdisk_mibs/IF-MIB.py` & `proliantutils-2.9.5/proliantutils/ilo/snmp/cpqdisk_mibs/IF-MIB.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/ilo/snmp/snmp_cpqdisk_sizes.py` & `proliantutils-2.9.5/proliantutils/ilo/snmp/snmp_cpqdisk_sizes.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 
 class MibBuilder(builder.MibBuilder):
     # NOTE(etingof): disable searching in `pysnmp_mibs` because it can
     # cause permission problems when opening files at relative path
     defaultMiscMibs = ''
 
+
 cpq_mibs_path = os.path.dirname(os.path.abspath(__file__))
 cpq_mibs_path = os.path.join(cpq_mibs_path, "cpqdisk_mibs")
 mBuilder = MibBuilder()
 mBuilder.addMibSources(builder.DirMibSource(cpq_mibs_path))
 mibBuilder = mBuilder.loadModules('CPQIDA-MIB', 'CPQSCSI-MIB')
 mibViewController = view.MibViewController(mibBuilder)
 
@@ -141,20 +142,18 @@
 
             if errorIndication:
                 LOG.error(errorIndication)
                 msg = "SNMP failed to traverse MIBs %s", errorIndication
                 raise exception.IloSNMPInvalidInputFailure(msg)
             else:
                 if errorStatus:
-                    msg = ('Parsing MIBs failed. %s at %s' % (
-                        errorStatus.prettyPrint(),
-                        errorIndex and varBinds[-1][int(errorIndex)-1]
-                        or '?'
-                        )
-                    )
+                    msg = ('Parsing MIBs failed. %s at %s'
+                           % (errorStatus.prettyPrint(),
+                              errorIndex and varBinds[-1][int(errorIndex) - 1]
+                              or '?'))
                     LOG.error(msg)
                     raise exception.IloSNMPInvalidInputFailure(msg)
                 else:
                     for varBindTableRow in varBinds:
                         name, val = tuple(varBindTableRow)
                         oid, label, suffix = (
                             mibViewController.getNodeName(name))
@@ -220,9 +219,9 @@
     """
     disk_sizes = _get_disksize_MiB(iLOIP, snmp_credentials)
     max_size = 0
     for uuid in disk_sizes:
         for key in disk_sizes[uuid]:
             if int(disk_sizes[uuid][key]) > max_size:
                 max_size = int(disk_sizes[uuid][key])
-    max_size_gb = max_size/1024
+    max_size_gb = max_size / 1024
     return max_size_gb
```

### Comparing `proliantutils-2.9.4/proliantutils/ilo/client.py` & `proliantutils-2.9.5/proliantutils/ilo/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,31 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
+
 """IloClient module"""
 
 import collections
+
 import netaddr
+
 from proliantutils import exception
 from proliantutils.ilo import ipmi
 from proliantutils.ilo import operations
 from proliantutils.ilo import ribcl
 from proliantutils.ilo import ris
 from proliantutils.ilo.snmp import snmp_cpqdisk_sizes as snmp
 from proliantutils import log
 from proliantutils.redfish import redfish
 
+
 SUPPORTED_RIS_METHODS = [
     'activate_license',
     'clear_secure_boot_keys',
     'create_raid_configuration',
     'delete_raid_configuration',
     'eject_virtual_media',
     'get_bios_settings_result',
@@ -65,15 +69,15 @@
     'set_iscsi_info',
     'unset_iscsi_info',
     'get_iscsi_initiator_info',
     'set_iscsi_initiator_info',
     'set_vm_status',
     'update_firmware',
     'update_persistent_boot',
-    ]
+]
 
 SUPPORTED_REDFISH_METHODS = [
     'create_raid_configuration',
     'delete_raid_configuration',
     'do_disk_erase',
     'has_disk_erase_completed',
     'get_product_name',
@@ -111,15 +115,19 @@
     'clear_secure_boot_keys',
     'get_server_capabilities',
     'get_supported_boot_mode',
     'get_essential_properties',
     'set_iscsi_info',
     'unset_iscsi_info',
     'get_iscsi_initiator_info',
-    'set_iscsi_initiator_info'
+    'set_iscsi_initiator_info',
+    'set_http_boot_url',
+    'get_http_boot_url',
+    'add_tls_certificate',
+    'remove_tls_certificate'
 ]
 
 LOG = log.get_logger(__name__)
 
 
 def cache_node(cache=True):
 
@@ -869,7 +877,21 @@
     def get_available_disk_types(self):
         """Get the list of all disk type available in server
 
         :returns: A list containing disk types.
         :raises: IloError, on an error from iLO.
         """
         return self._call_method('get_available_disk_types')
+
+    def add_tls_certificate(self, cert_file_list):
+        """Adds the TLS certificate to the iLO
+
+        :raises: IloError, on an error from iLO.
+        """
+        return self._call_method('add_tls_certificate', cert_file_list)
+
+    def remove_tls_certificate(self, fp_list):
+        """Removes the TLS certificate from the iLO
+
+        :raises: IloError, on an error from iLO.
+        """
+        return self._call_method('remove_tls_certificate', fp_list)
```

### Comparing `proliantutils-2.9.4/proliantutils/ilo/common.py` & `proliantutils-2.9.5/proliantutils/ilo/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,20 +235,20 @@
     :param supported_boot_mode_constant: supported boot_mode constant
     :returns: A namedtuple containing ``boot_mode_bios`` and
         ``boot_mode_uefi`` with 'true'/'false' set accordingly for
         legacy BIOS and UEFI boot modes.
     """
     boot_mode_bios = 'false'
     boot_mode_uefi = 'false'
-    if (supported_boot_mode_constant ==
-            constants.SUPPORTED_BOOT_MODE_LEGACY_BIOS_ONLY):
+    if (supported_boot_mode_constant
+            == constants.SUPPORTED_BOOT_MODE_LEGACY_BIOS_ONLY):
         boot_mode_bios = 'true'
-    elif (supported_boot_mode_constant ==
-            constants.SUPPORTED_BOOT_MODE_UEFI_ONLY):
+    elif (supported_boot_mode_constant
+          == constants.SUPPORTED_BOOT_MODE_UEFI_ONLY):
         boot_mode_uefi = 'true'
-    elif (supported_boot_mode_constant ==
-            constants.SUPPORTED_BOOT_MODE_LEGACY_BIOS_AND_UEFI):
+    elif (supported_boot_mode_constant
+          == constants.SUPPORTED_BOOT_MODE_LEGACY_BIOS_AND_UEFI):
         boot_mode_bios = 'true'
         boot_mode_uefi = 'true'
 
     return SupportedBootModes(boot_mode_bios=boot_mode_bios,
                               boot_mode_uefi=boot_mode_uefi)
```

### Comparing `proliantutils-2.9.4/proliantutils/ilo/constants.py` & `proliantutils-2.9.5/proliantutils/ilo/constants.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/proliantutils/exception.py` & `proliantutils-2.9.5/proliantutils/exception.py`

 * *Files identical despite different names*

### Comparing `proliantutils-2.9.4/setup.cfg` & `proliantutils-2.9.5/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 name = proliantutils
 summary = Client Library for interfacing with various devices in HP Proliant Servers.
 description-file = 
 	README.rst
 license = Apache License, Version 2.0
 author = Hewlett Packard Enterprise
 author-email = proliantutils@gmail.com
-home-page = https://github.com/openstack/proliantutils
+home-page = https://opendev.org/x/proliantutils
+python-requires = >=3.6
 classifier = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 2
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.5
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 
 [files]
 packages = 
 	proliantutils
 
 [entry_points]
 ironic_python_agent.hardware_managers =
```

### Comparing `proliantutils-2.9.4/ChangeLog` & `proliantutils-2.9.5/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+2.9.5
+-----
+
+* [Redfish] Provides APIs to add/remove TLS certificate
+* Redfish: Adds APIs to support boot from http url
+* Adds steps 'apply\_configuration' and 'flash\_firmware\_sum'
+* Enable check import order
+* Adds py3 to tox environment
+* Bump hacking to 3.0.0
+
 2.9.4
 -----
 
 * Updates mimimum version of sushy in requirements
 
 2.9.3
 -----
```

### Comparing `proliantutils-2.9.4/README.md` & `proliantutils-2.9.5/README.md`

 * *Files identical despite different names*

