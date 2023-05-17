# Comparing `tmp/elemento-cli-0.1.1.tar.gz` & `tmp/elemento-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elemento-cli-0.1.1.tar", last modified: Mon Apr 24 10:44:38 2023, max compression
+gzip compressed data, was "elemento-cli-0.1.3.tar", last modified: Wed May 17 12:25:44 2023, max compression
```

## Comparing `elemento-cli-0.1.1.tar` & `elemento-cli-0.1.3.tar`

### file list

```diff
@@ -1,80 +1,89 @@
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.954412 elemento-cli-0.1.1/
--rw-r--r--   0 filippovalle   (501) staff       (20)     3550 2023-04-24 10:44:38.954280 elemento-cli-0.1.1/PKG-INFO
--rw-r--r--   0 filippovalle   (501) staff       (20)     3286 2023-04-24 10:43:54.000000 elemento-cli-0.1.1/README.md
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.942877 elemento-cli-0.1.1/common/
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.942989 elemento-cli-0.1.1/common/lib/
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.943103 elemento-cli-0.1.1/common/lib/components/
--rw-r--r--   0 filippovalle   (501) staff       (20)       94 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.945349 elemento-cli-0.1.1/common/lib/components/cpu/
--rw-r--r--   0 filippovalle   (501) staff       (20)      174 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      127 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/common.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1824 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/cpudescriptor.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    88145 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/cpuinfo.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      647 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/cpumatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1443 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/cpurequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    12275 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/cpustatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.946638 elemento-cli-0.1.1/common/lib/components/cpu/tests/
--rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/tests/__init__.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     5890 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/tests/test_coresstatus.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     7412 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/tests/test_corestatus.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      959 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/tests/test_cpudescriptor.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2694 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/tests/test_cpumatcher.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2105 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/cpu/tests/test_cpustatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.947451 elemento-cli-0.1.1/common/lib/components/memory/
--rw-r--r--   0 filippovalle   (501) staff       (20)      134 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/memory/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      788 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/memory/memdescriptor.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/memory/memmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      615 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/memory/memrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     2405 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/memory/memstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.948159 elemento-cli-0.1.1/common/lib/components/misc/
--rw-r--r--   0 filippovalle   (501) staff       (20)       65 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/misc/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      461 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/misc/miscmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      609 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/misc/miscrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1525 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/misc/miscstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.949024 elemento-cli-0.1.1/common/lib/components/net/
--rw-r--r--   0 filippovalle   (501) staff       (20)       88 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/net/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      449 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/net/netmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     2016 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/net/netrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1909 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/net/netspeed.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     7668 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/net/netstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.949687 elemento-cli-0.1.1/common/lib/components/pcidev/
--rw-r--r--   0 filippovalle   (501) staff       (20)       68 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/pcimatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      940 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/pcirequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     7024 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/pcistatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.950807 elemento-cli-0.1.1/common/lib/components/pcidev/tests/
--rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/tests/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1037 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pciaddress.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      747 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcidevice.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      785 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcimatcher.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      682 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcirequirements.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      793 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pciscanner.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2481 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcistatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.951550 elemento-cli-0.1.1/common/lib/system/
--rw-r--r--   0 filippovalle   (501) staff       (20)      108 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/system/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      565 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/system/systemmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1416 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/system/systemrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6528 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/common/lib/system/systemstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.952148 elemento-cli-0.1.1/ecd/
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/ecd/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/ecd/networking.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/ecd/restkeys.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      148 2022-11-10 10:08:31.000000 elemento-cli-0.1.1/ecd/test.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.952773 elemento-cli-0.1.1/elemento_cli.egg-info/
--rw-r--r--   0 filippovalle   (501) staff       (20)     3550 2023-04-24 10:44:38.000000 elemento-cli-0.1.1/elemento_cli.egg-info/PKG-INFO
--rw-r--r--   0 filippovalle   (501) staff       (20)     2321 2023-04-24 10:44:38.000000 elemento-cli-0.1.1/elemento_cli.egg-info/SOURCES.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)        1 2023-04-24 10:44:38.000000 elemento-cli-0.1.1/elemento_cli.egg-info/dependency_links.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)       68 2023-04-24 10:44:38.000000 elemento-cli-0.1.1/elemento_cli.egg-info/requires.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)       20 2023-04-24 10:44:38.000000 elemento-cli-0.1.1/elemento_cli.egg-info/top_level.txt
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-04-24 10:44:38.953968 elemento-cli-0.1.1/handlers/
--rw-r--r--   0 filippovalle   (501) staff       (20)     2168 2023-03-17 11:00:12.000000 elemento-cli-0.1.1/handlers/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6781 2023-03-17 11:00:12.000000 elemento-cli-0.1.1/handlers/account.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     3261 2023-03-17 11:00:12.000000 elemento-cli-0.1.1/handlers/iso.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6871 2023-03-17 11:00:12.000000 elemento-cli-0.1.1/handlers/login.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6950 2023-03-17 11:00:12.000000 elemento-cli-0.1.1/handlers/network.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    13109 2023-04-18 10:37:58.000000 elemento-cli-0.1.1/handlers/vm.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     9321 2023-04-13 08:13:05.000000 elemento-cli-0.1.1/handlers/volumes.py
--rw-r--r--   0 filippovalle   (501) staff       (20)       38 2023-04-24 10:44:38.954451 elemento-cli-0.1.1/setup.cfg
--rw-r--r--   0 filippovalle   (501) staff       (20)     2730 2023-04-24 10:44:35.000000 elemento-cli-0.1.1/setup.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.408244 elemento-cli-0.1.3/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3532 2023-05-17 12:25:44.407985 elemento-cli-0.1.3/PKG-INFO
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3286 2023-04-24 10:43:54.000000 elemento-cli-0.1.3/README.md
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2772 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/betterprinttable.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.396889 elemento-cli-0.1.3/common/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      558 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/README.md
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.397139 elemento-cli-0.1.3/common/lib/
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.397243 elemento-cli-0.1.3/common/lib/components/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       94 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.399080 elemento-cli-0.1.3/common/lib/components/cpu/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      174 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      127 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/common.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1824 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpudescriptor.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    88145 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpuinfo.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      647 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpumatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1443 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpurequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    12275 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpustatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.400287 elemento-cli-0.1.3/common/lib/components/cpu/tests/
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/__init__.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5890 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_coresstatus.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     7412 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_corestatus.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      959 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpudescriptor.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2694 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpumatcher.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2105 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpustatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.401055 elemento-cli-0.1.3/common/lib/components/memory/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      134 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      788 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memdescriptor.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      615 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2405 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.401688 elemento-cli-0.1.3/common/lib/components/misc/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       65 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      461 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/miscmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      609 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/miscrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1525 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/miscstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.402427 elemento-cli-0.1.3/common/lib/components/net/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       88 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      449 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2016 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1909 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netspeed.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     7668 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.403039 elemento-cli-0.1.3/common/lib/components/pcidev/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       68 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/pcimatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      940 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/pcirequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     7024 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/pcistatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.404096 elemento-cli-0.1.3/common/lib/components/pcidev/tests/
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1037 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciaddress.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      747 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcidevice.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      785 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcimatcher.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      682 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcirequirements.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      793 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciscanner.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2481 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcistatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.404747 elemento-cli-0.1.3/common/lib/system/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      108 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      565 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/systemmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1416 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/systemrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6528 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/systemstatus.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      106 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/requirements.txt
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      167 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/run_tests.sh
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.405660 elemento-cli-0.1.3/ecd/
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      677 2022-11-25 10:13:55.000000 elemento-cli-0.1.3/ecd/networking.json
+-rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/networking.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1104 2022-11-25 10:13:32.000000 elemento-cli-0.1.3/ecd/restkeys.json
+-rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/restkeys.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      148 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/test.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/elemento
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/elemento.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.406243 elemento-cli-0.1.3/elemento_cli.egg-info/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3532 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/PKG-INFO
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2472 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)        1 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)       84 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/requires.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)       20 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/top_level.txt
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.407644 elemento-cli-0.1.3/handlers/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2168 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6781 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/account.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3261 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/iso.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6871 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/login.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6950 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/network.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    13109 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/handlers/vm.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     9321 2023-04-13 08:13:05.000000 elemento-cli-0.1.3/handlers/volumes.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3880 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/headers.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)       38 2023-05-17 12:25:44.408287 elemento-cli-0.1.3/setup.cfg
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2972 2023-05-17 12:25:37.000000 elemento-cli-0.1.3/setup.py
```

### Comparing `elemento-cli-0.1.1/PKG-INFO` & `elemento-cli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: elemento-cli
-Version: 0.1.1
+Version: 0.1.3
 Summary: CLI for Elemento
-Home-page: https://hackmd.io/qLIyWjTDRWiGeeCvQbj2yQ
+Home-page: https://elemento.cloud
 Author: Elemento
 Author-email: hello@elemento.cloud
 License: GPL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <br/>
```

### Comparing `elemento-cli-0.1.1/README.md` & `elemento-cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/cpudescriptor.py` & `elemento-cli-0.1.3/common/lib/components/cpu/cpudescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/cpuinfo.py` & `elemento-cli-0.1.3/common/lib/components/cpu/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/cpumatcher.py` & `elemento-cli-0.1.3/common/lib/components/cpu/cpumatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/cpurequirements.py` & `elemento-cli-0.1.3/common/lib/components/cpu/cpurequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/cpustatus.py` & `elemento-cli-0.1.3/common/lib/components/cpu/cpustatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/tests/test_coresstatus.py` & `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_coresstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/tests/test_corestatus.py` & `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_corestatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/tests/test_cpudescriptor.py` & `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpudescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/tests/test_cpumatcher.py` & `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpumatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/cpu/tests/test_cpustatus.py` & `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpustatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/memory/memdescriptor.py` & `elemento-cli-0.1.3/common/lib/components/memory/memdescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/memory/memrequirements.py` & `elemento-cli-0.1.3/common/lib/components/memory/memrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/memory/memstatus.py` & `elemento-cli-0.1.3/common/lib/components/memory/memstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/misc/miscrequirements.py` & `elemento-cli-0.1.3/common/lib/components/misc/miscrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/misc/miscstatus.py` & `elemento-cli-0.1.3/common/lib/components/misc/miscstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/net/netrequirements.py` & `elemento-cli-0.1.3/common/lib/components/net/netrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/net/netspeed.py` & `elemento-cli-0.1.3/common/lib/components/net/netspeed.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/net/netstatus.py` & `elemento-cli-0.1.3/common/lib/components/net/netstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/pcirequirements.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/pcirequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/pcistatus.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/pcistatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pciaddress.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciaddress.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcidevice.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcidevice.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcimatcher.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcimatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcirequirements.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcirequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pciscanner.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciscanner.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/components/pcidev/tests/test_pcistatus.py` & `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcistatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/system/systemmatcher.py` & `elemento-cli-0.1.3/common/lib/system/systemmatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/system/systemrequirements.py` & `elemento-cli-0.1.3/common/lib/system/systemrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/common/lib/system/systemstatus.py` & `elemento-cli-0.1.3/common/lib/system/systemstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/elemento_cli.egg-info/PKG-INFO` & `elemento-cli-0.1.3/elemento_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: elemento-cli
-Version: 0.1.1
+Version: 0.1.3
 Summary: CLI for Elemento
-Home-page: https://hackmd.io/qLIyWjTDRWiGeeCvQbj2yQ
+Home-page: https://elemento.cloud
 Author: Elemento
 Author-email: hello@elemento.cloud
 License: GPL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <br/>
```

### Comparing `elemento-cli-0.1.1/elemento_cli.egg-info/SOURCES.txt` & `elemento-cli-0.1.3/elemento_cli.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 README.md
+betterprinttable.py
+elemento
+elemento.py
+headers.py
 setup.py
+common/README.md
 common/__init__.py
+common/requirements.txt
+common/run_tests.sh
 common/lib/__init__.py
 common/lib/components/__init__.py
 common/lib/components/cpu/__init__.py
 common/lib/components/cpu/common.py
 common/lib/components/cpu/cpudescriptor.py
 common/lib/components/cpu/cpuinfo.py
 common/lib/components/cpu/cpumatcher.py
@@ -42,15 +49,17 @@
 common/lib/components/pcidev/tests/test_pciscanner.py
 common/lib/components/pcidev/tests/test_pcistatus.py
 common/lib/system/__init__.py
 common/lib/system/systemmatcher.py
 common/lib/system/systemrequirements.py
 common/lib/system/systemstatus.py
 ecd/__init__.py
+ecd/networking.json
 ecd/networking.py
+ecd/restkeys.json
 ecd/restkeys.py
 ecd/test.py
 elemento_cli.egg-info/PKG-INFO
 elemento_cli.egg-info/SOURCES.txt
 elemento_cli.egg-info/dependency_links.txt
 elemento_cli.egg-info/requires.txt
 elemento_cli.egg-info/top_level.txt
```

### Comparing `elemento-cli-0.1.1/handlers/__init__.py` & `elemento-cli-0.1.3/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/handlers/account.py` & `elemento-cli-0.1.3/handlers/account.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/handlers/iso.py` & `elemento-cli-0.1.3/handlers/iso.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/handlers/login.py` & `elemento-cli-0.1.3/handlers/login.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/handlers/network.py` & `elemento-cli-0.1.3/handlers/network.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/handlers/vm.py` & `elemento-cli-0.1.3/handlers/vm.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/handlers/volumes.py` & `elemento-cli-0.1.3/handlers/volumes.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.1/setup.py` & `elemento-cli-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,25 +29,33 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="elemento-cli",
-    version="0.1.1",
+    version="0.1.3",
     author="Elemento",
     author_email="hello@elemento.cloud",
     description="CLI for Elemento",
     license="GPL",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://hackmd.io/qLIyWjTDRWiGeeCvQbj2yQ",
+    url="https://elemento.cloud",
     packages=setuptools.find_packages(),
+    include_package_data=True,
+    scripts=['elemento.py', 'elemento', "headers.py", "betterprinttable.py"],
+    package_data={
+        ".":["headers.py"],
+        "ecd":["*"],
+        "common": ["*"],
+        "handlers": ["*.py"]},
     install_requires = ["argparse", 
         "argcomplete", 
         "tabulate", 
         "si_prefix",
         "jsonpickle",
         "requests",
-        "pwinput"],
+        "pwinput",
+        "urllib3==1.26.6"],
     python_requires='>=3.9',
 )
```

