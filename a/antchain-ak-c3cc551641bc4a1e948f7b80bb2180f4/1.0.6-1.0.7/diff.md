# Comparing `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6.tar.gz` & `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6.tar", last modified: Tue May 16 09:08:35 2023, max compression
+gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7.tar", last modified: Wed May 17 02:58:53 2023, max compression
```

## Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6.tar` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32882 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
--rw-r--r--   0 root         (0) root         (0)    28210 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 09:08:35.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 09:08:34.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
+-rw-r--r--   0 root         (0) root         (0)    28210 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-17 02:58:53.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/setup.py
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/LICENSE` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.6
+Version: 1.0.7
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/README-CN.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/README.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.6
+Version: 1.0.7
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.6',
+                    'sdk_version': '1.0.7',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
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
-                    'sdk_version': '1.0.6',
+                    'sdk_version': '1.0.7',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.6/setup.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.
 
-Created on 16/05/2023
+Created on 17/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4"
 NAME = "antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python"
```

