# Comparing `tmp/alibabacloud_hologram20220601-1.0.2.tar.gz` & `tmp/alibabacloud_hologram20220601-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.2.tar", last modified: Wed Apr 26 09:32:29 2023, max compression
+gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.3.tar", last modified: Wed May 17 03:56:22 2023, max compression
```

## Comparing `alibabacloud_hologram20220601-1.0.2.tar` & `alibabacloud_hologram20220601-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21836 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/client.py
--rw-r--r--   0 root         (0) root         (0)    47357 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-26 09:32:29.000000 alibabacloud_hologram20220601-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-04-26 09:32:28.000000 alibabacloud_hologram20220601-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21136 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/client.py
+-rw-r--r--   0 root         (0) root         (0)    47585 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/setup.py
```

### Comparing `alibabacloud_hologram20220601-1.0.2/LICENSE` & `alibabacloud_hologram20220601-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.2/PKG-INFO` & `alibabacloud_hologram20220601-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_hologram20220601
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.2/README-CN.md` & `alibabacloud_hologram20220601-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.2/README.md` & `alibabacloud_hologram20220601-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/client.py` & `alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Dict
 from Tea.core import TeaCore
 
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_endpoint_util.client import Client as EndpointUtilClient
-from alibabacloud_hologram20220601 import models as hologram_20220601_models
 from alibabacloud_tea_util import models as util_models
+from alibabacloud_hologram20220601 import models as hologram_20220601_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
     """
@@ -40,25 +40,19 @@
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def get_instance_with_options(
         self,
         instance_id: str,
-        request: hologram_20220601_models.GetInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.GetInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='GetInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}',
             method='GET',
@@ -71,25 +65,19 @@
             hologram_20220601_models.GetInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def get_instance_with_options_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.GetInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.GetInstanceResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
+            headers=headers
         )
         params = open_api_models.Params(
             action='GetInstance',
             version='2022-06-01',
             protocol='HTTPS',
             pathname=f'/api/v1/instances/{OpenApiUtilClient.get_encode_param(instance_id)}',
             method='GET',
@@ -102,28 +90,26 @@
             hologram_20220601_models.GetInstanceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def get_instance(
         self,
         instance_id: str,
-        request: hologram_20220601_models.GetInstanceRequest,
     ) -> hologram_20220601_models.GetInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_instance_with_options(instance_id, request, headers, runtime)
+        return self.get_instance_with_options(instance_id, headers, runtime)
 
     async def get_instance_async(
         self,
         instance_id: str,
-        request: hologram_20220601_models.GetInstanceRequest,
     ) -> hologram_20220601_models.GetInstanceResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_instance_with_options_async(instance_id, request, headers, runtime)
+        return await self.get_instance_with_options_async(instance_id, headers, runtime)
 
     def list_instances_with_options(
         self,
         request: hologram_20220601_models.ListInstancesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> hologram_20220601_models.ListInstancesResponse:
```

### Comparing `alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601/models.py` & `alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,13 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import List, Dict
 
 
-class GetInstanceRequest(TeaModel):
-    def __init__(
-        self,
-        region_id: str = None,
-    ):
-        self.region_id = region_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
 class GetInstanceResponseBodyInstanceEndpoints(TeaModel):
     def __init__(
         self,
         alternative_endpoints: str = None,
         enabled: bool = None,
         endpoint: str = None,
         type: str = None,
@@ -137,14 +110,17 @@
         compute_node_count: int = None,
         cpu: int = None,
         creation_time: str = None,
         disk: str = None,
         enable_hive_access: str = None,
         endpoints: List[GetInstanceResponseBodyInstanceEndpoints] = None,
         expiration_time: str = None,
+        gateway_count: int = None,
+        gateway_cpu: int = None,
+        gateway_memory: int = None,
         instance_charge_type: str = None,
         instance_id: str = None,
         instance_name: str = None,
         instance_owner: str = None,
         instance_status: str = None,
         instance_type: str = None,
         leader_instance_id: str = None,
@@ -161,14 +137,17 @@
         self.compute_node_count = compute_node_count
         self.cpu = cpu
         self.creation_time = creation_time
         self.disk = disk
         self.enable_hive_access = enable_hive_access
         self.endpoints = endpoints
         self.expiration_time = expiration_time
+        self.gateway_count = gateway_count
+        self.gateway_cpu = gateway_cpu
+        self.gateway_memory = gateway_memory
         self.instance_charge_type = instance_charge_type
         self.instance_id = instance_id
         self.instance_name = instance_name
         self.instance_owner = instance_owner
         self.instance_status = instance_status
         self.instance_type = instance_type
         self.leader_instance_id = leader_instance_id
@@ -213,14 +192,20 @@
             result['EnableHiveAccess'] = self.enable_hive_access
         result['Endpoints'] = []
         if self.endpoints is not None:
             for k in self.endpoints:
                 result['Endpoints'].append(k.to_map() if k else None)
         if self.expiration_time is not None:
             result['ExpirationTime'] = self.expiration_time
+        if self.gateway_count is not None:
+            result['GatewayCount'] = self.gateway_count
+        if self.gateway_cpu is not None:
+            result['GatewayCpu'] = self.gateway_cpu
+        if self.gateway_memory is not None:
+            result['GatewayMemory'] = self.gateway_memory
         if self.instance_charge_type is not None:
             result['InstanceChargeType'] = self.instance_charge_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.instance_name is not None:
             result['InstanceName'] = self.instance_name
         if self.instance_owner is not None:
@@ -268,14 +253,20 @@
         self.endpoints = []
         if m.get('Endpoints') is not None:
             for k in m.get('Endpoints'):
                 temp_model = GetInstanceResponseBodyInstanceEndpoints()
                 self.endpoints.append(temp_model.from_map(k))
         if m.get('ExpirationTime') is not None:
             self.expiration_time = m.get('ExpirationTime')
+        if m.get('GatewayCount') is not None:
+            self.gateway_count = m.get('GatewayCount')
+        if m.get('GatewayCpu') is not None:
+            self.gateway_cpu = m.get('GatewayCpu')
+        if m.get('GatewayMemory') is not None:
+            self.gateway_memory = m.get('GatewayMemory')
         if m.get('InstanceChargeType') is not None:
             self.instance_charge_type = m.get('InstanceChargeType')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('InstanceName') is not None:
             self.instance_name = m.get('InstanceName')
         if m.get('InstanceOwner') is not None:
```

### Comparing `alibabacloud_hologram20220601-1.0.2/alibabacloud_hologram20220601.egg-info/PKG-INFO` & `alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-hologram20220601
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.2/setup.py` & `alibabacloud_hologram20220601-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_hologram20220601.
 
-Created on 26/04/2023
+Created on 17/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_hologram20220601"
 NAME = "alibabacloud_hologram20220601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Hologres (20220601) SDK Library for Python"
```

