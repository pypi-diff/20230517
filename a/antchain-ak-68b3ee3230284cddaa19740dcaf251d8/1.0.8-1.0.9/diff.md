# Comparing `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8.tar.gz` & `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8.tar", last modified: Tue May 16 03:58:19 2023, max compression
+gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9.tar", last modified: Wed May 17 06:08:54 2023, max compression
```

## Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8.tar` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31410 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
--rw-r--r--   0 root         (0) root         (0)    36763 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31330 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
+-rw-r--r--   0 root         (0) root         (0)    36709 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-17 06:08:54.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/setup.py
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/LICENSE` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README-CN.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8',
+                    'sdk_version': '1.0.9',
                     '_prod_code': 'ak_68b3ee3230284cddaa19740dcaf251d8',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8',
+                    'sdk_version': '1.0.9',
                     '_prod_code': 'ak_68b3ee3230284cddaa19740dcaf251d8',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -612,57 +612,57 @@
         )
 
     def query_antchain_saas_ability_businesscode(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 根据能力id查询能力信息
+        Summary: 根据能力id查询能力信息
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.query_antchain_saas_ability_businesscode_ex(request, headers, runtime)
 
     async def query_antchain_saas_ability_businesscode_async(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 根据能力id查询能力信息
+        Summary: 根据能力id查询能力信息
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.query_antchain_saas_ability_businesscode_ex_async(request, headers, runtime)
 
     def query_antchain_saas_ability_businesscode_ex(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 根据能力id查询能力信息
+        Summary: 根据能力id查询能力信息
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse(),
             self.do_request('1.0', 'antchain.saas.ability.businesscode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_antchain_saas_ability_businesscode_ex_async(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 根据能力id查询能力信息
+        Summary: 根据能力id查询能力信息
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse(),
             await self.do_request_async('1.0', 'antchain.saas.ability.businesscode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -953,47 +953,47 @@
 
 
 class QueryAntchainSaasAbilityBusinesscodeRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        business_code: str = None,
+        ability_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 商业产品编码，L5编码
-        self.business_code = business_code
+        # 能力id
+        self.ability_id = ability_id
 
     def validate(self):
-        self.validate_required(self.business_code, 'business_code')
+        self.validate_required(self.ability_id, 'ability_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.business_code is not None:
-            result['business_code'] = self.business_code
+        if self.ability_id is not None:
+            result['ability_id'] = self.ability_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('business_code') is not None:
-            self.business_code = m.get('business_code')
+        if m.get('ability_id') is not None:
+            self.ability_id = m.get('ability_id')
         return self
 
 
 class QueryAntchainSaasAbilityBusinesscodeResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/setup.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_68b3ee3230284cddaa19740dcaf251d8.
 
-Created on 16/05/2023
+Created on 17/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8"
 NAME = "antchain_ak_68b3ee3230284cddaa19740dcaf251d8" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python"
```

