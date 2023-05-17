# Comparing `tmp/amazon-ec2-best-instance-2.5.0.tar.gz` & `tmp/amazon-ec2-best-instance-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/alexey/PycharmProjects/kankou-aliaksei/amazon-ec2-best-instance/dist/.tmp-7ajvglzd/amazon-ec2-best-instance-2.5.0.tar", last modified: Sun May 14 14:58:51 2023, max compression
+gzip compressed data, was "/Users/alexey/PycharmProjects/kankou-aliaksei/amazon-ec2-best-instance/dist/.tmp-9cuibstj/amazon-ec2-best-instance-3.0.0.tar", last modified: Wed May 17 10:57:13 2023, max compression
```

## Comparing `amazon-ec2-best-instance-2.5.0.tar` & `amazon-ec2-best-instance-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/
--rw-r--r--   0 alexey     (501) staff       (20)     7353 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)     6789 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-2.5.0/README.md
--rw-r--r--   0 alexey     (501) staff       (20)        0 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/pyproject.toml
--rw-r--r--   0 alexey     (501) staff       (20)      812 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)      214 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-2.5.0/setup.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance/
--rw-r--r--   0 alexey     (501) staff       (20)     1677 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance/SpotUtils.py
--rw-r--r--   0 alexey     (501) staff       (20)       67 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    21824 2023-05-14 14:58:38.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     7353 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      792 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)       58 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       25 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/top_level.txt
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-14 14:58:51.000000 amazon-ec2-best-instance-2.5.0/test/
--rw-r--r--   0 alexey     (501) staff       (20)      914 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test.py
--rw-r--r--   0 alexey     (501) staff       (20)     1822 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test1.py
--rw-r--r--   0 alexey     (501) staff       (20)      870 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test10.py
--rw-r--r--   0 alexey     (501) staff       (20)     1008 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test11.py
--rw-r--r--   0 alexey     (501) staff       (20)     1250 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test2.py
--rw-r--r--   0 alexey     (501) staff       (20)      242 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1257 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1397 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test5.py
--rw-r--r--   0 alexey     (501) staff       (20)      804 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test6.py
--rw-r--r--   0 alexey     (501) staff       (20)     1720 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test7.py
--rw-r--r--   0 alexey     (501) staff       (20)     1154 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test8.py
--rw-r--r--   0 alexey     (501) staff       (20)      517 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test9.py
--rw-r--r--   0 alexey     (501) staff       (20)     1086 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test_azs.py
--rw-r--r--   0 alexey     (501) staff       (20)     1996 2023-05-13 17:39:20.000000 amazon-ec2-best-instance-2.5.0/test/test_cache.py
--rw-r--r--   0 alexey     (501) staff       (20)     1869 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test_cache_2.py
--rw-r--r--   0 alexey     (501) staff       (20)      938 2023-05-13 17:42:39.000000 amazon-ec2-best-instance-2.5.0/test/test_cache_3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1040 2023-05-13 17:54:23.000000 amazon-ec2-best-instance-2.5.0/test/test_cache_4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1028 2023-05-13 17:55:02.000000 amazon-ec2-best-instance-2.5.0/test/test_cache_5.py
--rw-r--r--   0 alexey     (501) staff       (20)      638 2023-05-13 18:06:28.000000 amazon-ec2-best-instance-2.5.0/test/test_cache_6.py
--rw-r--r--   0 alexey     (501) staff       (20)      599 2023-05-13 18:07:20.000000 amazon-ec2-best-instance-2.5.0/test/test_cache_7.py
--rw-r--r--   0 alexey     (501) staff       (20)     2138 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-2.5.0/test/test_clients.py
--rw-r--r--   0 alexey     (501) staff       (20)     2145 2023-05-14 14:57:55.000000 amazon-ec2-best-instance-2.5.0/test/test_fast.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/
+-rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)     6791 2023-05-17 10:53:19.000000 amazon-ec2-best-instance-3.0.0/README.md
+-rw-r--r--   0 alexey     (501) staff       (20)        0 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/pyproject.toml
+-rw-r--r--   0 alexey     (501) staff       (20)      812 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)      214 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-3.0.0/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/
+-rw-r--r--   0 alexey     (501) staff       (20)     1677 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/SpotUtils.py
+-rw-r--r--   0 alexey     (501) staff       (20)       67 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/__init__.py
+-rw-r--r--   0 alexey     (501) staff       (20)    22676 2023-05-17 08:51:37.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      809 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       58 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       25 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/top_level.txt
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/test/
+-rw-r--r--   0 alexey     (501) staff       (20)      914 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1822 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test1.py
+-rw-r--r--   0 alexey     (501) staff       (20)      870 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test10.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1008 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test11.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1250 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test2.py
+-rw-r--r--   0 alexey     (501) staff       (20)      242 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test3.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1257 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test4.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1397 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test5.py
+-rw-r--r--   0 alexey     (501) staff       (20)      804 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test6.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1720 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test7.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1154 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test8.py
+-rw-r--r--   0 alexey     (501) staff       (20)      517 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test9.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1086 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test_azs.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1996 2023-05-13 17:39:20.000000 amazon-ec2-best-instance-3.0.0/test/test_cache.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1869 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_2.py
+-rw-r--r--   0 alexey     (501) staff       (20)      938 2023-05-13 17:42:39.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_3.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1040 2023-05-13 17:54:23.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_4.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1028 2023-05-13 17:55:02.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_5.py
+-rw-r--r--   0 alexey     (501) staff       (20)      638 2023-05-13 18:06:28.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_6.py
+-rw-r--r--   0 alexey     (501) staff       (20)      599 2023-05-13 18:07:20.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_7.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2138 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test_clients.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2145 2023-05-14 14:57:55.000000 amazon-ec2-best-instance-3.0.0/test/test_fast.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2191 2023-05-17 08:52:19.000000 amazon-ec2-best-instance-3.0.0/test/test_gpu.py
```

### Comparing `amazon-ec2-best-instance-2.5.0/PKG-INFO` & `amazon-ec2-best-instance-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ec2-best-instance
-Version: 2.5.0
+Version: 3.0.0
 Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
@@ -28,15 +28,16 @@
 * **vcpu** Required. Float. Describes the vCPU configurations for the instance type.
 * **memory_gb** Required. Float. Describes the memory for the instance type in GiB.
 * **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand. Default: 'on-demand'. Values: 'spot'|'on-demand'.
 * **burstable** Optional. Boolean. Indicates whether the instance type is a burstable performance instance type.
 * **architecture** Optional. String. The architectures supported by the instance type. Default: 'x86_64'. Values: 'i386'|'x86_64'|'arm64'|'x86_64_mac'
 * **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Default: ['Linux/UNIX']. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
 * **is_current_generation** Optional. Boolean. Use the latest generation or not.
-* **is_best_price** Optional. Boolean. Indicate if you need to get an instance type with the best price. If this flag is specified, the "get_best_instance_types" method returns a list of instance types sorted by price in ascending order.
+* **has_gpu** Optional. Boolean. Indicating whether the instance is equipped with a GPU. Default: None
+* **gpu_memory** Optional. Integer. Amount of GPU Memory in Gigabytes (GiB). Only activated when 'has_gpu' is set to True. Default: None
 * **is_instance_storage_supported** Optional. Boolean. Use instance types with instance store support
 * **max_interruption_frequency** Optional. Integer (%). Max spot instance frequency interruption in percent. Note: If you specify >=21, then the '>20%' rate is applied. It is used only if 'usage_class' == 'spot' and 'is_best_price' == True
 * **availability_zones** Optional. List<String>. Availability zones. E.g. ['us-east-1a', 'us-east-1b']
 * **final_spot_price_determination_strategy** Optional. String. Default: "min". Valid values: "min"|"max"|"average"
 
 # Usage
```

### Comparing `amazon-ec2-best-instance-2.5.0/README.md` & `amazon-ec2-best-instance-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 * **vcpu** Required. Float. Describes the vCPU configurations for the instance type.
 * **memory_gb** Required. Float. Describes the memory for the instance type in GiB.
 * **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand. Default: 'on-demand'. Values: 'spot'|'on-demand'.
 * **burstable** Optional. Boolean. Indicates whether the instance type is a burstable performance instance type.
 * **architecture** Optional. String. The architectures supported by the instance type. Default: 'x86_64'. Values: 'i386'|'x86_64'|'arm64'|'x86_64_mac'
 * **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Default: ['Linux/UNIX']. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
 * **is_current_generation** Optional. Boolean. Use the latest generation or not.
-* **is_best_price** Optional. Boolean. Indicate if you need to get an instance type with the best price. If this flag is specified, the "get_best_instance_types" method returns a list of instance types sorted by price in ascending order.
+* **has_gpu** Optional. Boolean. Indicating whether the instance is equipped with a GPU. Default: None
+* **gpu_memory** Optional. Integer. Amount of GPU Memory in Gigabytes (GiB). Only activated when 'has_gpu' is set to True. Default: None
 * **is_instance_storage_supported** Optional. Boolean. Use instance types with instance store support
 * **max_interruption_frequency** Optional. Integer (%). Max spot instance frequency interruption in percent. Note: If you specify >=21, then the '>20%' rate is applied. It is used only if 'usage_class' == 'spot' and 'is_best_price' == True
 * **availability_zones** Optional. List<String>. Availability zones. E.g. ['us-east-1a', 'us-east-1b']
 * **final_spot_price_determination_strategy** Optional. String. Default: "min". Valid values: "min"|"max"|"average"
 
 # Usage
```

### Comparing `amazon-ec2-best-instance-2.5.0/setup.cfg` & `amazon-ec2-best-instance-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amazon-ec2-best-instance
-version = 2.5.0
+version = 3.0.0
 author = Aliaksei Kankou
 author_email = aliaksei.kankou@gmail.com
 description = Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 project_urls =
```

### Comparing `amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance/SpotUtils.py` & `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/SpotUtils.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance/main.py` & `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import boto3
 import json
 import logging
 import os
 import operator
 import hashlib
 from datetime import datetime
+from typing import Optional, Dict, Any
+from multiprocessing.pool import ThreadPool
+from lambda_thread_pool import LambdaThreadPool
 from .SpotUtils import SpotUtils
 
 
 class Ec2BestInstance:
     __DESCRIBE_SPOT_PRICE_HISTORY_CONCURRENCY = 10
     __DESCRIBE_ON_DEMAND_PRICE_CONCURRENCY = 10
     __CACHE_TTL_IN_MINUTES = 120
@@ -45,40 +48,27 @@
         'Windows': 'Windows',
         'Linux/UNIX (Amazon VPC)': 'Linux',
         'Red Hat Enterprise Linux (Amazon VPC)': 'RHEL',
         'SUSE Linux (Amazon VPC)': 'SUSE',
         'Windows (Amazon VPC)': 'Windows'
     }
 
-    def __init__(self, options={}, logger=None):
-        self.__CACHE_TTL_IN_MINUTES = options.get('cache_ttl_in_minutes', self.__CACHE_TTL_IN_MINUTES)
+    def __init__(self, options: Optional[Dict[str, Any]] = None, logger: Optional[logging.Logger] = None):
+        if options is None:
+            options = {}
 
-        if os.environ.get('AWS_LAMBDA_FUNCTION_NAME') is None:
-            from multiprocessing.pool import ThreadPool as Pool
-            self.__Pool = Pool
-        else:
-            from lambda_thread_pool import LambdaThreadPool
-            self.__Pool = LambdaThreadPool
-        self.__region = 'us-east-1'
-        self.__describe_spot_price_history_concurrency = self.__DESCRIBE_SPOT_PRICE_HISTORY_CONCURRENCY
-        self.__describe_on_demand_price_concurrency = self.__DESCRIBE_ON_DEMAND_PRICE_CONCURRENCY
-        if options.get('region'):
-            self.__region = options['region']
-        if options.get('describe_spot_price_history_concurrency'):
-            self.__describe_spot_price_history_concurrency = options.get('describe_spot_price_history_concurrency')
-        if options.get('describe_on_demand_price_concurrency'):
-            self.__describe_on_demand_price_concurrency = options.get('describe_on_demand_price_concurrency')
-        if options.get('clients') is not None and options['clients'].get('ec2') is not None:
-            self.__ec2_client = options['clients']['ec2']
-        else:
-            self.__ec2_client = boto3.session.Session().client('ec2', region_name=self.__region)
-        if options.get('clients') is not None and options['clients'].get('pricing') is not None:
-            self.__pricing_client = options['clients']['pricing']
-        else:
-            self.__pricing_client = boto3.session.Session().client('pricing', region_name='us-east-1')
+        self.__CACHE_TTL_IN_MINUTES = options.get('cache_ttl_in_minutes', self.__CACHE_TTL_IN_MINUTES)
+        self.__Pool = self.__get_pool()
+        self.__region = options.get('region', 'us-east-1')
+        self.__describe_spot_price_history_concurrency = options.get('describe_spot_price_history_concurrency',
+                                                                     self.__DESCRIBE_SPOT_PRICE_HISTORY_CONCURRENCY)
+        self.__describe_on_demand_price_concurrency = options.get('describe_on_demand_price_concurrency',
+                                                                  self.__DESCRIBE_ON_DEMAND_PRICE_CONCURRENCY)
+        self.__ec2_client = self.__get_client(options, 'ec2', self.__region)
+        self.__pricing_client = self.__get_client(options, 'pricing', 'us-east-1')
         self.__logger = logger if logger is not None else logging.getLogger()
 
     def get_best_instance_types(self, options={}):
         hash_digest = self.get_hash(options)
         if self.__cache.get(hash_digest) is not None:
             cache_datetime = self.__cache[hash_digest]['datetime']
             now = datetime.now()
@@ -105,51 +95,52 @@
 
         usage_class = options.get('usage_class', 'on-demand')
         burstable = options.get('burstable')
         architecture = options.get('architecture', 'x86_64')
         availability_zones = options.get('availability_zones')
         final_spot_price_determination_strategy = options.get('final_spot_price_determination_strategy', 'min')
 
+        has_gpu = options.get('has_gpu')
+        gpu_memory = options.get('gpu_memory')
+
         valid_product_descriptions = [
             'Linux/UNIX',
             'Red Hat Enterprise Linux',
             'SUSE Linux',
             'Windows',
             'Linux/UNIX (Amazon VPC)',
             'Red Hat Enterprise Linux (Amazon VPC)',
             'SUSE Linux (Amazon VPC)',
             'Windows (Amazon VPC)'
         ]
-        product_descriptions = options.get('product_descriptions', ['Linux/UNIX'])
-        for product_description in product_descriptions:
-            if product_description not in valid_product_descriptions:
-                raise Exception(f'The product description {product_description} is not supported')
+        product_description = options.get('product_description', 'Linux/UNIX')
+        if product_description not in valid_product_descriptions:
+            raise Exception(f'The product description {product_description} is not supported')
         is_current_generation = None
-        is_best_price = options.get('is_best_price', False)
+        is_best_price = True
         is_instance_storage_supported = options.get('is_instance_storage_supported')
         max_interruption_frequency = options.get('max_interruption_frequency')
-        operating_systems = self.__get_operating_systems_by_product_descriptions(product_descriptions)
-        if len(operating_systems) > 1:
-            raise Exception('You must specify products that are compatible with only one operating system')
-        operating_system = operating_systems[0]
+        operating_system = self.__get_operating_system_by_product_description(product_description)
 
         if options.get('is_current_generation') is not None:
             is_current_generation = 'true' if options['is_current_generation'] == True else 'false'
 
         instances = self.__describe_instance_types({
             'is_current_generation': is_current_generation,
             'is_instance_storage_supported': is_instance_storage_supported
         })
 
         filtered_instances = self.__filter_ec2_instances(instances, {
             'cpu': cpu,
             'memory_gb': memory_gb,
             'usage_class': usage_class,
             'burstable': burstable,
-            'architecture': architecture
+            'architecture': architecture,
+            'has_gpu': has_gpu,
+            'gpu_memory': gpu_memory
         })
 
         self.__logger.debug(f'Instance types number before filtering: {str(len(instances))}')
 
         if usage_class == 'spot' and max_interruption_frequency is not None:
             spot_utils = SpotUtils(self.__region)
 
@@ -180,15 +171,15 @@
 
         self.__logger.debug(f'Instance types number after filtering: {str(len(filtered_instances))}')
 
         if is_best_price:
             if usage_class == 'on-demand':
                 result = self.__sort_on_demand_instances_by_price(filtered_instances, operating_system)
             elif usage_class == 'spot':
-                result = self.__sort_spot_instances_by_price(filtered_instances, product_descriptions,
+                result = self.__sort_spot_instances_by_price(filtered_instances, product_description,
                                                              availability_zones,
                                                              final_spot_price_determination_strategy)
             else:
                 raise Exception(f'The usage_class: {usage_class} does not exist')
         else:
             result = list(map(lambda ec2_instance: {'instance_type': ec2_instance['InstanceType']}, filtered_instances))
 
@@ -290,25 +281,37 @@
                 filter(lambda ec2_instance: options.get('burstable') == ec2_instance['BurstablePerformanceSupported'],
                        filtered_instances))
         if options.get('architecture') is not None:
             filtered_instances = list(
                 filter(lambda ec2_instance: options.get('architecture') in ec2_instance['ProcessorInfo'][
                     'SupportedArchitectures'],
                        filtered_instances))
+        if options.get('has_gpu') is not None:
+            if options['has_gpu']:
+                filtered_instances = list(
+                    filter(lambda ec2_instance: ec2_instance.get('GpuInfo') is not None, filtered_instances))
+                if options.get('gpu_memory') is not None:
+                    filtered_instances = list(
+                        filter(
+                            lambda ec2_instance: int(ec2_instance['GpuInfo']['TotalGpuMemoryInMiB'] / 1024) >= options[
+                                'gpu_memory'], filtered_instances))
+            else:
+                filtered_instances = list(
+                    filter(lambda ec2_instance: ec2_instance.get('GpuInfo') is None, filtered_instances))
 
         return filtered_instances
 
-    def __ec2_instance_price_loop(self, ec2_instance, product_descriptions, availability_zones,
+    def __ec2_instance_price_loop(self, ec2_instance, product_description, availability_zones,
                                   final_spot_price_determination_strategy):
         instance_type = ec2_instance['InstanceType']
 
         filters = [
             {
                 'Name': 'product-description',
-                'Values': product_descriptions
+                'Values': [product_description]
             }
         ]
 
         if availability_zones:
             filters.append({
                 'Name': 'availability-zone',
                 'Values': availability_zones
@@ -351,23 +354,23 @@
 
         return {
             'price': spot_price,
             'ec2_instance': ec2_instance,
             'az_price': az_price
         }
 
-    def __sort_spot_instances_by_price(self, filtered_instances, product_descriptions, availability_zones,
+    def __sort_spot_instances_by_price(self, filtered_instances, product_description, availability_zones,
                                        final_spot_price_determination_strategy):
         pool = self.__Pool(self.__describe_spot_price_history_concurrency)
 
         results = []
 
         for ec2_instance in filtered_instances:
             result = pool.apply_async(self.__ec2_instance_price_loop,
-                                      (ec2_instance, product_descriptions, availability_zones,
+                                      (ec2_instance, product_description, availability_zones,
                                        final_spot_price_determination_strategy))
             results.append(result)
 
         pool.close()
         pool.join()
 
         ec2_instances = [result.get() for result in results]
@@ -386,14 +389,17 @@
                 'vcpu': ec2_instance['ec2_instance']['VCpuInfo']['DefaultVCpus'],
                 'memory': int(ec2_instance['ec2_instance']['MemoryInfo']['SizeInMiB'] / 1024),
                 'network_performance': ec2_instance['ec2_instance']['NetworkInfo']['NetworkPerformance'],
                 'storage': ec2_instance['ec2_instance'].get('InstanceStorageInfo').get('Disks') if ec2_instance[
                     'ec2_instance'].get('InstanceStorageInfo') else 'EBS Only'
             }
 
+            if ec2_instance['ec2_instance'].get('GpuInfo') is not None:
+                entry['gpu_memory'] = int(ec2_instance['ec2_instance']['GpuInfo']['TotalGpuMemoryInMiB'] / 1024)
+
             if interruption_frequency:
                 entry['interruption_frequency'] = interruption_frequency
 
             enriched_instances.append(entry)
 
         return enriched_instances
 
@@ -401,23 +407,28 @@
         ec2_prices = self.__get_ec2_price(operating_system)
         ec2_instances = []
 
         for ec2_instance_input in ec2_instances_input:
             instance_type = ec2_instance_input['InstanceType']
             price = ec2_prices.get(instance_type)
             if price is not None:
-                ec2_instances.append({
+                entry = {
                     'price': ec2_prices[instance_type]['instance_price'],
                     'instance_type': instance_type,
                     'vcpu': ec2_instance_input['VCpuInfo']['DefaultVCpus'],
                     'memory': int(ec2_instance_input['MemoryInfo']['SizeInMiB'] / 1024),
                     'network_performance': ec2_instance_input['NetworkInfo']['NetworkPerformance'],
                     'storage': ec2_instance_input.get('InstanceStorageInfo').get('Disks') if ec2_instance_input.get(
                         'InstanceStorageInfo') else 'EBS Only'
-                })
+                }
+
+                if ec2_instance_input.get('GpuInfo') is not None:
+                    entry['gpu_memory'] = int(ec2_instance_input['GpuInfo']['TotalGpuMemoryInMiB'] / 1024)
+
+                ec2_instances.append(entry)
             else:
                 self.__logger.warning(f'Price for the {instance_type} instance type not found')
 
         ec2_instances.sort(key=operator.itemgetter('price'))
 
         return ec2_instances
 
@@ -460,18 +471,17 @@
                     'vcpu': vcpu,
                     'memory': memory,
                     'os': os,
                     'instance_price': instance_price
                 }
         return records
 
-    def __get_operating_systems_by_product_descriptions(self, product_descriptions):
-        operating_systems = [self.__OS_PRODUCT_DESCRIPTION_MAP[product_description] for product_description in
-                             product_descriptions]
-        return Ec2BestInstance.unique(operating_systems)
+    def __get_operating_system_by_product_description(self, product_description):
+        operating_system = self.__OS_PRODUCT_DESCRIPTION_MAP[product_description]
+        return operating_system
 
     def get_hash(self, dictionary):
         dictionary_copy = dictionary.copy()
         dictionary_copy['region'] = self.__region
         dict_string = json.dumps(dictionary_copy)
         hash_object = hashlib.md5(dict_string.encode())
         return hash_object.hexdigest()
@@ -489,7 +499,21 @@
         return availability_zones
 
     @staticmethod
     def unique(list1):
         list_set = set(list1)
         unique_list = (list(list_set))
         return unique_list
+
+    @staticmethod
+    def __get_pool() -> Any:
+        if os.environ.get('AWS_LAMBDA_FUNCTION_NAME') is None:
+            return ThreadPool()
+        else:
+            return LambdaThreadPool()
+
+    @staticmethod
+    def __get_client(options: Dict[str, Any], service: str, region: str) -> Any:
+        if options.get('clients') is not None and options['clients'].get(service) is not None:
+            return options['clients'][service]
+        else:
+            return boto3.session.Session().client(service, region_name=region)
```

### Comparing `amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/PKG-INFO` & `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ec2-best-instance
-Version: 2.5.0
+Version: 3.0.0
 Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
@@ -28,15 +28,16 @@
 * **vcpu** Required. Float. Describes the vCPU configurations for the instance type.
 * **memory_gb** Required. Float. Describes the memory for the instance type in GiB.
 * **usage_class** Optional. String. Indicates whether the instance type is offered for spot or On-Demand. Default: 'on-demand'. Values: 'spot'|'on-demand'.
 * **burstable** Optional. Boolean. Indicates whether the instance type is a burstable performance instance type.
 * **architecture** Optional. String. The architectures supported by the instance type. Default: 'x86_64'. Values: 'i386'|'x86_64'|'arm64'|'x86_64_mac'
 * **product_descriptions** Optional. List<String>. The operating system that you will use on the virtual machine. Default: ['Linux/UNIX']. Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
 * **is_current_generation** Optional. Boolean. Use the latest generation or not.
-* **is_best_price** Optional. Boolean. Indicate if you need to get an instance type with the best price. If this flag is specified, the "get_best_instance_types" method returns a list of instance types sorted by price in ascending order.
+* **has_gpu** Optional. Boolean. Indicating whether the instance is equipped with a GPU. Default: None
+* **gpu_memory** Optional. Integer. Amount of GPU Memory in Gigabytes (GiB). Only activated when 'has_gpu' is set to True. Default: None
 * **is_instance_storage_supported** Optional. Boolean. Use instance types with instance store support
 * **max_interruption_frequency** Optional. Integer (%). Max spot instance frequency interruption in percent. Note: If you specify >=21, then the '>20%' rate is applied. It is used only if 'usage_class' == 'spot' and 'is_best_price' == True
 * **availability_zones** Optional. List<String>. Availability zones. E.g. ['us-east-1a', 'us-east-1b']
 * **final_spot_price_determination_strategy** Optional. String. Default: "min". Valid values: "min"|"max"|"average"
 
 # Usage
```

### Comparing `amazon-ec2-best-instance-2.5.0/src/amazon_ec2_best_instance.egg-info/SOURCES.txt` & `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 test/test_cache_2.py
 test/test_cache_3.py
 test/test_cache_4.py
 test/test_cache_5.py
 test/test_cache_6.py
 test/test_cache_7.py
 test/test_clients.py
-test/test_fast.py
+test/test_fast.py
+test/test_gpu.py
```

### Comparing `amazon-ec2-best-instance-2.5.0/test/test.py` & `amazon-ec2-best-instance-3.0.0/test/test.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test1.py` & `amazon-ec2-best-instance-3.0.0/test/test1.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test10.py` & `amazon-ec2-best-instance-3.0.0/test/test10.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test11.py` & `amazon-ec2-best-instance-3.0.0/test/test11.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test2.py` & `amazon-ec2-best-instance-3.0.0/test/test2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test4.py` & `amazon-ec2-best-instance-3.0.0/test/test4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test5.py` & `amazon-ec2-best-instance-3.0.0/test/test5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test6.py` & `amazon-ec2-best-instance-3.0.0/test/test6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test7.py` & `amazon-ec2-best-instance-3.0.0/test/test7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test8.py` & `amazon-ec2-best-instance-3.0.0/test/test8.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test9.py` & `amazon-ec2-best-instance-3.0.0/test/test9.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_azs.py` & `amazon-ec2-best-instance-3.0.0/test/test_azs.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_cache.py` & `amazon-ec2-best-instance-3.0.0/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_cache_2.py` & `amazon-ec2-best-instance-3.0.0/test/test_cache_2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_cache_3.py` & `amazon-ec2-best-instance-3.0.0/test/test_cache_3.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_cache_4.py` & `amazon-ec2-best-instance-3.0.0/test/test_cache_4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_cache_5.py` & `amazon-ec2-best-instance-3.0.0/test/test_cache_5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_cache_6.py` & `amazon-ec2-best-instance-3.0.0/test/test_cache_6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_cache_7.py` & `amazon-ec2-best-instance-3.0.0/test/test_cache_7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_clients.py` & `amazon-ec2-best-instance-3.0.0/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-2.5.0/test/test_fast.py` & `amazon-ec2-best-instance-3.0.0/test/test_fast.py`

 * *Files identical despite different names*

