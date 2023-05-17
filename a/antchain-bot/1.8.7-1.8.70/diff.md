# Comparing `tmp/antchain_bot-1.8.7.tar.gz` & `tmp/antchain_bot-1.8.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bot-1.8.7.tar", last modified: Tue Feb 28 07:21:50 2023, max compression
+gzip compressed data, was "dist/antchain_bot-1.8.70.tar", last modified: Wed May 17 06:30:00 2023, max compression
```

## Comparing `antchain_bot-1.8.7.tar` & `antchain_bot-1.8.70.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2162 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2162 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_sdk_bot/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_sdk_bot/__init__.py
--rw-r--r--   0 root         (0) root         (0)   371150 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_sdk_bot/client.py
--rw-r--r--   0 root         (0) root         (0)   961426 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/antchain_sdk_bot/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-02-28 07:21:50.000000 antchain_bot-1.8.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   423032 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/client.py
+-rw-r--r--   0 root         (0) root         (0)  1124816 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/setup.py
```

### Comparing `antchain_bot-1.8.7/LICENSE` & `antchain_bot-1.8.70/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.7/PKG-INFO` & `antchain_bot-1.8.70/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_bot
-Version: 1.8.7
+Version: 1.8.70
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.7/README-CN.md` & `antchain_bot-1.8.70/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.7/README.md` & `antchain_bot-1.8.70/README.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.7/antchain_bot.egg-info/PKG-INFO` & `antchain_bot-1.8.70/antchain_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-bot
-Version: 1.8.7
+Version: 1.8.70
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.7/antchain_sdk_bot/client.py` & `antchain_bot-1.8.70/antchain_sdk_bot/client.py`

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
-                    'sdk_version': '1.8.7',
+                    'sdk_version': '1.8.70',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
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
-                    'sdk_version': '1.8.7',
+                    'sdk_version': '1.8.70',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -607,14 +607,910 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.QueryLeaseRiskResponse(),
             await self.do_request_async('1.0', 'blockchain.bot.lease.risk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def create_xr_userticket(
+        self,
+        request: bot_models.CreateXrUserticketRequest,
+    ) -> bot_models.CreateXrUserticketResponse:
+        """
+        Description: aiot-创建用户通行证
+        Summary: aiot-创建用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_xr_userticket_ex(request, headers, runtime)
+
+    async def create_xr_userticket_async(
+        self,
+        request: bot_models.CreateXrUserticketRequest,
+    ) -> bot_models.CreateXrUserticketResponse:
+        """
+        Description: aiot-创建用户通行证
+        Summary: aiot-创建用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_xr_userticket_ex_async(request, headers, runtime)
+
+    def create_xr_userticket_ex(
+        self,
+        request: bot_models.CreateXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateXrUserticketResponse:
+        """
+        Description: aiot-创建用户通行证
+        Summary: aiot-创建用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateXrUserticketResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.userticket.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_xr_userticket_ex_async(
+        self,
+        request: bot_models.CreateXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateXrUserticketResponse:
+        """
+        Description: aiot-创建用户通行证
+        Summary: aiot-创建用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateXrUserticketResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.userticket.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def list_xr_xrticketpool(
+        self,
+        request: bot_models.ListXrXrticketpoolRequest,
+    ) -> bot_models.ListXrXrticketpoolResponse:
+        """
+        Description: aiot-获取通行证资源池列表
+        Summary: aiot-获取通行证资源池列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_xr_xrticketpool_ex(request, headers, runtime)
+
+    async def list_xr_xrticketpool_async(
+        self,
+        request: bot_models.ListXrXrticketpoolRequest,
+    ) -> bot_models.ListXrXrticketpoolResponse:
+        """
+        Description: aiot-获取通行证资源池列表
+        Summary: aiot-获取通行证资源池列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_xr_xrticketpool_ex_async(request, headers, runtime)
+
+    def list_xr_xrticketpool_ex(
+        self,
+        request: bot_models.ListXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ListXrXrticketpoolResponse:
+        """
+        Description: aiot-获取通行证资源池列表
+        Summary: aiot-获取通行证资源池列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ListXrXrticketpoolResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrticketpool.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_xr_xrticketpool_ex_async(
+        self,
+        request: bot_models.ListXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ListXrXrticketpoolResponse:
+        """
+        Description: aiot-获取通行证资源池列表
+        Summary: aiot-获取通行证资源池列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ListXrXrticketpoolResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrticketpool.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_xr_userticket(
+        self,
+        request: bot_models.PagequeryXrUserticketRequest,
+    ) -> bot_models.PagequeryXrUserticketResponse:
+        """
+        Description: aiot-分页查询用户通行证
+        Summary: aiot-分页查询用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_xr_userticket_ex(request, headers, runtime)
+
+    async def pagequery_xr_userticket_async(
+        self,
+        request: bot_models.PagequeryXrUserticketRequest,
+    ) -> bot_models.PagequeryXrUserticketResponse:
+        """
+        Description: aiot-分页查询用户通行证
+        Summary: aiot-分页查询用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_xr_userticket_ex_async(request, headers, runtime)
+
+    def pagequery_xr_userticket_ex(
+        self,
+        request: bot_models.PagequeryXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrUserticketResponse:
+        """
+        Description: aiot-分页查询用户通行证
+        Summary: aiot-分页查询用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrUserticketResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.userticket.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_xr_userticket_ex_async(
+        self,
+        request: bot_models.PagequeryXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrUserticketResponse:
+        """
+        Description: aiot-分页查询用户通行证
+        Summary: aiot-分页查询用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrUserticketResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.userticket.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_xr_userticket(
+        self,
+        request: bot_models.GetXrUserticketRequest,
+    ) -> bot_models.GetXrUserticketResponse:
+        """
+        Description: aiot-查询用户通行证
+        Summary: aiot-查询用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_xr_userticket_ex(request, headers, runtime)
+
+    async def get_xr_userticket_async(
+        self,
+        request: bot_models.GetXrUserticketRequest,
+    ) -> bot_models.GetXrUserticketResponse:
+        """
+        Description: aiot-查询用户通行证
+        Summary: aiot-查询用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_xr_userticket_ex_async(request, headers, runtime)
+
+    def get_xr_userticket_ex(
+        self,
+        request: bot_models.GetXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.GetXrUserticketResponse:
+        """
+        Description: aiot-查询用户通行证
+        Summary: aiot-查询用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.GetXrUserticketResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.userticket.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_xr_userticket_ex_async(
+        self,
+        request: bot_models.GetXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.GetXrUserticketResponse:
+        """
+        Description: aiot-查询用户通行证
+        Summary: aiot-查询用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.GetXrUserticketResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.userticket.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def operate_xr_userticket(
+        self,
+        request: bot_models.OperateXrUserticketRequest,
+    ) -> bot_models.OperateXrUserticketResponse:
+        """
+        Description: aiot-核销用户通行证
+        Summary: aiot-核销用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.operate_xr_userticket_ex(request, headers, runtime)
+
+    async def operate_xr_userticket_async(
+        self,
+        request: bot_models.OperateXrUserticketRequest,
+    ) -> bot_models.OperateXrUserticketResponse:
+        """
+        Description: aiot-核销用户通行证
+        Summary: aiot-核销用户通行证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.operate_xr_userticket_ex_async(request, headers, runtime)
+
+    def operate_xr_userticket_ex(
+        self,
+        request: bot_models.OperateXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.OperateXrUserticketResponse:
+        """
+        Description: aiot-核销用户通行证
+        Summary: aiot-核销用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.OperateXrUserticketResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.userticket.operate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def operate_xr_userticket_ex_async(
+        self,
+        request: bot_models.OperateXrUserticketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.OperateXrUserticketResponse:
+        """
+        Description: aiot-核销用户通行证
+        Summary: aiot-核销用户通行证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.OperateXrUserticketResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.userticket.operate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def list_xr_resource(
+        self,
+        request: bot_models.ListXrResourceRequest,
+    ) -> bot_models.ListXrResourceResponse:
+        """
+        Description: aiot-获取资源列表
+        Summary: aiot-获取资源列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_xr_resource_ex(request, headers, runtime)
+
+    async def list_xr_resource_async(
+        self,
+        request: bot_models.ListXrResourceRequest,
+    ) -> bot_models.ListXrResourceResponse:
+        """
+        Description: aiot-获取资源列表
+        Summary: aiot-获取资源列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_xr_resource_ex_async(request, headers, runtime)
+
+    def list_xr_resource_ex(
+        self,
+        request: bot_models.ListXrResourceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ListXrResourceResponse:
+        """
+        Description: aiot-获取资源列表
+        Summary: aiot-获取资源列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ListXrResourceResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.resource.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_xr_resource_ex_async(
+        self,
+        request: bot_models.ListXrResourceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ListXrResourceResponse:
+        """
+        Description: aiot-获取资源列表
+        Summary: aiot-获取资源列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ListXrResourceResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.resource.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_xr_xrverificationmodel(
+        self,
+        request: bot_models.PagequeryXrXrverificationmodelRequest,
+    ) -> bot_models.PagequeryXrXrverificationmodelResponse:
+        """
+        Description: aiot-核销实例分页查询
+        Summary: aiot-核销实例分页查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_xr_xrverificationmodel_ex(request, headers, runtime)
+
+    async def pagequery_xr_xrverificationmodel_async(
+        self,
+        request: bot_models.PagequeryXrXrverificationmodelRequest,
+    ) -> bot_models.PagequeryXrXrverificationmodelResponse:
+        """
+        Description: aiot-核销实例分页查询
+        Summary: aiot-核销实例分页查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_xr_xrverificationmodel_ex_async(request, headers, runtime)
+
+    def pagequery_xr_xrverificationmodel_ex(
+        self,
+        request: bot_models.PagequeryXrXrverificationmodelRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrXrverificationmodelResponse:
+        """
+        Description: aiot-核销实例分页查询
+        Summary: aiot-核销实例分页查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrXrverificationmodelResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrverificationmodel.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_xr_xrverificationmodel_ex_async(
+        self,
+        request: bot_models.PagequeryXrXrverificationmodelRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrXrverificationmodelResponse:
+        """
+        Description: aiot-核销实例分页查询
+        Summary: aiot-核销实例分页查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrXrverificationmodelResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrverificationmodel.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_xr_customerdevice(
+        self,
+        request: bot_models.PagequeryXrCustomerdeviceRequest,
+    ) -> bot_models.PagequeryXrCustomerdeviceResponse:
+        """
+        Description: aiot-客户对应设备分页查询
+        Summary: aiot-客户对应设备分页查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_xr_customerdevice_ex(request, headers, runtime)
+
+    async def pagequery_xr_customerdevice_async(
+        self,
+        request: bot_models.PagequeryXrCustomerdeviceRequest,
+    ) -> bot_models.PagequeryXrCustomerdeviceResponse:
+        """
+        Description: aiot-客户对应设备分页查询
+        Summary: aiot-客户对应设备分页查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_xr_customerdevice_ex_async(request, headers, runtime)
+
+    def pagequery_xr_customerdevice_ex(
+        self,
+        request: bot_models.PagequeryXrCustomerdeviceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrCustomerdeviceResponse:
+        """
+        Description: aiot-客户对应设备分页查询
+        Summary: aiot-客户对应设备分页查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrCustomerdeviceResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.customerdevice.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_xr_customerdevice_ex_async(
+        self,
+        request: bot_models.PagequeryXrCustomerdeviceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrCustomerdeviceResponse:
+        """
+        Description: aiot-客户对应设备分页查询
+        Summary: aiot-客户对应设备分页查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrCustomerdeviceResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.customerdevice.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_xr_xrticketpool(
+        self,
+        request: bot_models.CreateXrXrticketpoolRequest,
+    ) -> bot_models.CreateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证创建
+        Summary: aiot-xr通行证创建
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_xr_xrticketpool_ex(request, headers, runtime)
+
+    async def create_xr_xrticketpool_async(
+        self,
+        request: bot_models.CreateXrXrticketpoolRequest,
+    ) -> bot_models.CreateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证创建
+        Summary: aiot-xr通行证创建
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_xr_xrticketpool_ex_async(request, headers, runtime)
+
+    def create_xr_xrticketpool_ex(
+        self,
+        request: bot_models.CreateXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证创建
+        Summary: aiot-xr通行证创建
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateXrXrticketpoolResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrticketpool.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_xr_xrticketpool_ex_async(
+        self,
+        request: bot_models.CreateXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证创建
+        Summary: aiot-xr通行证创建
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateXrXrticketpoolResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrticketpool.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def update_xr_xrticketpool(
+        self,
+        request: bot_models.UpdateXrXrticketpoolRequest,
+    ) -> bot_models.UpdateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证修改
+        Summary: aiot-xr通行证修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_xr_xrticketpool_ex(request, headers, runtime)
+
+    async def update_xr_xrticketpool_async(
+        self,
+        request: bot_models.UpdateXrXrticketpoolRequest,
+    ) -> bot_models.UpdateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证修改
+        Summary: aiot-xr通行证修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_xr_xrticketpool_ex_async(request, headers, runtime)
+
+    def update_xr_xrticketpool_ex(
+        self,
+        request: bot_models.UpdateXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.UpdateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证修改
+        Summary: aiot-xr通行证修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.UpdateXrXrticketpoolResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrticketpool.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_xr_xrticketpool_ex_async(
+        self,
+        request: bot_models.UpdateXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.UpdateXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证修改
+        Summary: aiot-xr通行证修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.UpdateXrXrticketpoolResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrticketpool.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_xr_xrticketpool(
+        self,
+        request: bot_models.PagequeryXrXrticketpoolRequest,
+    ) -> bot_models.PagequeryXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证分页查询
+        Summary: aiot-xr通行证分页查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_xr_xrticketpool_ex(request, headers, runtime)
+
+    async def pagequery_xr_xrticketpool_async(
+        self,
+        request: bot_models.PagequeryXrXrticketpoolRequest,
+    ) -> bot_models.PagequeryXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证分页查询
+        Summary: aiot-xr通行证分页查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_xr_xrticketpool_ex_async(request, headers, runtime)
+
+    def pagequery_xr_xrticketpool_ex(
+        self,
+        request: bot_models.PagequeryXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证分页查询
+        Summary: aiot-xr通行证分页查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrXrticketpoolResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrticketpool.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_xr_xrticketpool_ex_async(
+        self,
+        request: bot_models.PagequeryXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.PagequeryXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证分页查询
+        Summary: aiot-xr通行证分页查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.PagequeryXrXrticketpoolResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrticketpool.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def sync_device_screenstatus(
+        self,
+        request: bot_models.SyncDeviceScreenstatusRequest,
+    ) -> bot_models.SyncDeviceScreenstatusResponse:
+        """
+        Description: aiot-同步设备屏幕状态
+        Summary: aiot-同步设备屏幕状态
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_device_screenstatus_ex(request, headers, runtime)
+
+    async def sync_device_screenstatus_async(
+        self,
+        request: bot_models.SyncDeviceScreenstatusRequest,
+    ) -> bot_models.SyncDeviceScreenstatusResponse:
+        """
+        Description: aiot-同步设备屏幕状态
+        Summary: aiot-同步设备屏幕状态
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_device_screenstatus_ex_async(request, headers, runtime)
+
+    def sync_device_screenstatus_ex(
+        self,
+        request: bot_models.SyncDeviceScreenstatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.SyncDeviceScreenstatusResponse:
+        """
+        Description: aiot-同步设备屏幕状态
+        Summary: aiot-同步设备屏幕状态
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.SyncDeviceScreenstatusResponse(),
+            self.do_request('1.0', 'blockchain.bot.device.screenstatus.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_device_screenstatus_ex_async(
+        self,
+        request: bot_models.SyncDeviceScreenstatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.SyncDeviceScreenstatusResponse:
+        """
+        Description: aiot-同步设备屏幕状态
+        Summary: aiot-同步设备屏幕状态
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.SyncDeviceScreenstatusResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.device.screenstatus.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def batchcreate_xr_xrticketpool(
+        self,
+        request: bot_models.BatchcreateXrXrticketpoolRequest,
+    ) -> bot_models.BatchcreateXrXrticketpoolResponse:
+        """
+        Description: xr通行证批量创建
+        Summary: xr通行证批量创建
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.batchcreate_xr_xrticketpool_ex(request, headers, runtime)
+
+    async def batchcreate_xr_xrticketpool_async(
+        self,
+        request: bot_models.BatchcreateXrXrticketpoolRequest,
+    ) -> bot_models.BatchcreateXrXrticketpoolResponse:
+        """
+        Description: xr通行证批量创建
+        Summary: xr通行证批量创建
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.batchcreate_xr_xrticketpool_ex_async(request, headers, runtime)
+
+    def batchcreate_xr_xrticketpool_ex(
+        self,
+        request: bot_models.BatchcreateXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.BatchcreateXrXrticketpoolResponse:
+        """
+        Description: xr通行证批量创建
+        Summary: xr通行证批量创建
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.BatchcreateXrXrticketpoolResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrticketpool.batchcreate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def batchcreate_xr_xrticketpool_ex_async(
+        self,
+        request: bot_models.BatchcreateXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.BatchcreateXrXrticketpoolResponse:
+        """
+        Description: xr通行证批量创建
+        Summary: xr通行证批量创建
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.BatchcreateXrXrticketpoolResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrticketpool.batchcreate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def list_xr_xrverificationmodelinstance(
+        self,
+        request: bot_models.ListXrXrverificationmodelinstanceRequest,
+    ) -> bot_models.ListXrXrverificationmodelinstanceResponse:
+        """
+        Description: aiot-获取资源实例列表
+        Summary: aiot-获取资源实例列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_xr_xrverificationmodelinstance_ex(request, headers, runtime)
+
+    async def list_xr_xrverificationmodelinstance_async(
+        self,
+        request: bot_models.ListXrXrverificationmodelinstanceRequest,
+    ) -> bot_models.ListXrXrverificationmodelinstanceResponse:
+        """
+        Description: aiot-获取资源实例列表
+        Summary: aiot-获取资源实例列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_xr_xrverificationmodelinstance_ex_async(request, headers, runtime)
+
+    def list_xr_xrverificationmodelinstance_ex(
+        self,
+        request: bot_models.ListXrXrverificationmodelinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ListXrXrverificationmodelinstanceResponse:
+        """
+        Description: aiot-获取资源实例列表
+        Summary: aiot-获取资源实例列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ListXrXrverificationmodelinstanceResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrverificationmodelinstance.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_xr_xrverificationmodelinstance_ex_async(
+        self,
+        request: bot_models.ListXrXrverificationmodelinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ListXrXrverificationmodelinstanceResponse:
+        """
+        Description: aiot-获取资源实例列表
+        Summary: aiot-获取资源实例列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ListXrXrverificationmodelinstanceResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrverificationmodelinstance.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def detail_xr_xrticketpool(
+        self,
+        request: bot_models.DetailXrXrticketpoolRequest,
+    ) -> bot_models.DetailXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证详情查询
+        Summary: aiot-xr通行证详情查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_xr_xrticketpool_ex(request, headers, runtime)
+
+    async def detail_xr_xrticketpool_async(
+        self,
+        request: bot_models.DetailXrXrticketpoolRequest,
+    ) -> bot_models.DetailXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证详情查询
+        Summary: aiot-xr通行证详情查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_xr_xrticketpool_ex_async(request, headers, runtime)
+
+    def detail_xr_xrticketpool_ex(
+        self,
+        request: bot_models.DetailXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.DetailXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证详情查询
+        Summary: aiot-xr通行证详情查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.DetailXrXrticketpoolResponse(),
+            self.do_request('1.0', 'blockchain.bot.xr.xrticketpool.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_xr_xrticketpool_ex_async(
+        self,
+        request: bot_models.DetailXrXrticketpoolRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.DetailXrXrticketpoolResponse:
+        """
+        Description: aiot-xr通行证详情查询
+        Summary: aiot-xr通行证详情查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.DetailXrXrticketpoolResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.xr.xrticketpool.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def operate_aiotnextbs_openapi(
+        self,
+        request: bot_models.OperateAiotnextbsOpenapiRequest,
+    ) -> bot_models.OperateAiotnextbsOpenapiResponse:
+        """
+        Description: aiotnextbs-openApi操作
+        Summary: aiotnextbs-openApi操作
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.operate_aiotnextbs_openapi_ex(request, headers, runtime)
+
+    async def operate_aiotnextbs_openapi_async(
+        self,
+        request: bot_models.OperateAiotnextbsOpenapiRequest,
+    ) -> bot_models.OperateAiotnextbsOpenapiResponse:
+        """
+        Description: aiotnextbs-openApi操作
+        Summary: aiotnextbs-openApi操作
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.operate_aiotnextbs_openapi_ex_async(request, headers, runtime)
+
+    def operate_aiotnextbs_openapi_ex(
+        self,
+        request: bot_models.OperateAiotnextbsOpenapiRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.OperateAiotnextbsOpenapiResponse:
+        """
+        Description: aiotnextbs-openApi操作
+        Summary: aiotnextbs-openApi操作
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.OperateAiotnextbsOpenapiResponse(),
+            self.do_request('1.0', 'blockchain.bot.aiotnextbs.openapi.operate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def operate_aiotnextbs_openapi_ex_async(
+        self,
+        request: bot_models.OperateAiotnextbsOpenapiRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.OperateAiotnextbsOpenapiResponse:
+        """
+        Description: aiotnextbs-openApi操作
+        Summary: aiotnextbs-openApi操作
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.OperateAiotnextbsOpenapiResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.aiotnextbs.openapi.operate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def finish_trace_config(
         self,
         request: bot_models.FinishTraceConfigRequest,
     ) -> bot_models.FinishTraceConfigResponse:
         """
         Description: 私有化配置推送回告API
         Summary: 私有化配置推送回告API
@@ -3503,41 +4399,41 @@
 
     def save_iotbasic_customer(
         self,
         request: bot_models.SaveIotbasicCustomerRequest,
     ) -> bot_models.SaveIotbasicCustomerResponse:
         """
         Description: IoT设备平台-客户新增
-        Summary: IoT设备平台-客户新增
+        Summary: IoT设备平台-中台签约客户同步
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.save_iotbasic_customer_ex(request, headers, runtime)
 
     async def save_iotbasic_customer_async(
         self,
         request: bot_models.SaveIotbasicCustomerRequest,
     ) -> bot_models.SaveIotbasicCustomerResponse:
         """
         Description: IoT设备平台-客户新增
-        Summary: IoT设备平台-客户新增
+        Summary: IoT设备平台-中台签约客户同步
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.save_iotbasic_customer_ex_async(request, headers, runtime)
 
     def save_iotbasic_customer_ex(
         self,
         request: bot_models.SaveIotbasicCustomerRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> bot_models.SaveIotbasicCustomerResponse:
         """
         Description: IoT设备平台-客户新增
-        Summary: IoT设备平台-客户新增
+        Summary: IoT设备平台-中台签约客户同步
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.SaveIotbasicCustomerResponse(),
             self.do_request('1.0', 'blockchain.bot.iotbasic.customer.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
@@ -3545,15 +4441,15 @@
         self,
         request: bot_models.SaveIotbasicCustomerRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> bot_models.SaveIotbasicCustomerResponse:
         """
         Description: IoT设备平台-客户新增
-        Summary: IoT设备平台-客户新增
+        Summary: IoT设备平台-中台签约客户同步
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.SaveIotbasicCustomerResponse(),
             await self.do_request_async('1.0', 'blockchain.bot.iotbasic.customer.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
@@ -8369,14 +9265,406 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.QueryThingmodelResponse(),
             await self.do_request_async('1.0', 'blockchain.bot.thingmodel.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def create_distributedevice_bydevicemul(
+        self,
+        request: bot_models.CreateDistributedeviceBydevicemulRequest,
+    ) -> bot_models.CreateDistributedeviceBydevicemulResponse:
+        """
+        Description: 通过设备异步批量发行设备
+        Summary: 通过设备异步批量发行设备
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_distributedevice_bydevicemul_ex(request, headers, runtime)
+
+    async def create_distributedevice_bydevicemul_async(
+        self,
+        request: bot_models.CreateDistributedeviceBydevicemulRequest,
+    ) -> bot_models.CreateDistributedeviceBydevicemulResponse:
+        """
+        Description: 通过设备异步批量发行设备
+        Summary: 通过设备异步批量发行设备
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_distributedevice_bydevicemul_ex_async(request, headers, runtime)
+
+    def create_distributedevice_bydevicemul_ex(
+        self,
+        request: bot_models.CreateDistributedeviceBydevicemulRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateDistributedeviceBydevicemulResponse:
+        """
+        Description: 通过设备异步批量发行设备
+        Summary: 通过设备异步批量发行设备
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateDistributedeviceBydevicemulResponse(),
+            self.do_request('1.0', 'blockchain.bot.distributedevice.bydevicemul.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_distributedevice_bydevicemul_ex_async(
+        self,
+        request: bot_models.CreateDistributedeviceBydevicemulRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateDistributedeviceBydevicemulResponse:
+        """
+        Description: 通过设备异步批量发行设备
+        Summary: 通过设备异步批量发行设备
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateDistributedeviceBydevicemulResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.distributedevice.bydevicemul.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_distributedevice_bydeviceidmul(
+        self,
+        request: bot_models.CreateDistributedeviceBydeviceidmulRequest,
+    ) -> bot_models.CreateDistributedeviceBydeviceidmulResponse:
+        """
+        Description: 通过设备ID异步批量发行设备
+        Summary: 通过设备ID异步批量发行设备
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_distributedevice_bydeviceidmul_ex(request, headers, runtime)
+
+    async def create_distributedevice_bydeviceidmul_async(
+        self,
+        request: bot_models.CreateDistributedeviceBydeviceidmulRequest,
+    ) -> bot_models.CreateDistributedeviceBydeviceidmulResponse:
+        """
+        Description: 通过设备ID异步批量发行设备
+        Summary: 通过设备ID异步批量发行设备
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_distributedevice_bydeviceidmul_ex_async(request, headers, runtime)
+
+    def create_distributedevice_bydeviceidmul_ex(
+        self,
+        request: bot_models.CreateDistributedeviceBydeviceidmulRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateDistributedeviceBydeviceidmulResponse:
+        """
+        Description: 通过设备ID异步批量发行设备
+        Summary: 通过设备ID异步批量发行设备
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateDistributedeviceBydeviceidmulResponse(),
+            self.do_request('1.0', 'blockchain.bot.distributedevice.bydeviceidmul.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_distributedevice_bydeviceidmul_ex_async(
+        self,
+        request: bot_models.CreateDistributedeviceBydeviceidmulRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateDistributedeviceBydeviceidmulResponse:
+        """
+        Description: 通过设备ID异步批量发行设备
+        Summary: 通过设备ID异步批量发行设备
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateDistributedeviceBydeviceidmulResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.distributedevice.bydeviceidmul.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def bind_entityrelation(
+        self,
+        request: bot_models.BindEntityrelationRequest,
+    ) -> bot_models.BindEntityrelationResponse:
+        """
+        Description: 绑定实体关系
+        Summary: 绑定实体关系
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.bind_entityrelation_ex(request, headers, runtime)
+
+    async def bind_entityrelation_async(
+        self,
+        request: bot_models.BindEntityrelationRequest,
+    ) -> bot_models.BindEntityrelationResponse:
+        """
+        Description: 绑定实体关系
+        Summary: 绑定实体关系
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.bind_entityrelation_ex_async(request, headers, runtime)
+
+    def bind_entityrelation_ex(
+        self,
+        request: bot_models.BindEntityrelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.BindEntityrelationResponse:
+        """
+        Description: 绑定实体关系
+        Summary: 绑定实体关系
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.BindEntityrelationResponse(),
+            self.do_request('1.0', 'blockchain.bot.entityrelation.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def bind_entityrelation_ex_async(
+        self,
+        request: bot_models.BindEntityrelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.BindEntityrelationResponse:
+        """
+        Description: 绑定实体关系
+        Summary: 绑定实体关系
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.BindEntityrelationResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.entityrelation.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def unbind_entityrelation(
+        self,
+        request: bot_models.UnbindEntityrelationRequest,
+    ) -> bot_models.UnbindEntityrelationResponse:
+        """
+        Description: 批量解绑实体关系
+        Summary: 批量解绑实体关系
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.unbind_entityrelation_ex(request, headers, runtime)
+
+    async def unbind_entityrelation_async(
+        self,
+        request: bot_models.UnbindEntityrelationRequest,
+    ) -> bot_models.UnbindEntityrelationResponse:
+        """
+        Description: 批量解绑实体关系
+        Summary: 批量解绑实体关系
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.unbind_entityrelation_ex_async(request, headers, runtime)
+
+    def unbind_entityrelation_ex(
+        self,
+        request: bot_models.UnbindEntityrelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.UnbindEntityrelationResponse:
+        """
+        Description: 批量解绑实体关系
+        Summary: 批量解绑实体关系
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.UnbindEntityrelationResponse(),
+            self.do_request('1.0', 'blockchain.bot.entityrelation.unbind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def unbind_entityrelation_ex_async(
+        self,
+        request: bot_models.UnbindEntityrelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.UnbindEntityrelationResponse:
+        """
+        Description: 批量解绑实体关系
+        Summary: 批量解绑实体关系
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.UnbindEntityrelationResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.entityrelation.unbind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def detail_thingmodel_device(
+        self,
+        request: bot_models.DetailThingmodelDeviceRequest,
+    ) -> bot_models.DetailThingmodelDeviceResponse:
+        """
+        Description: 查询物模型设备详情
+        Summary: 查询物模型设备详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_thingmodel_device_ex(request, headers, runtime)
+
+    async def detail_thingmodel_device_async(
+        self,
+        request: bot_models.DetailThingmodelDeviceRequest,
+    ) -> bot_models.DetailThingmodelDeviceResponse:
+        """
+        Description: 查询物模型设备详情
+        Summary: 查询物模型设备详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_thingmodel_device_ex_async(request, headers, runtime)
+
+    def detail_thingmodel_device_ex(
+        self,
+        request: bot_models.DetailThingmodelDeviceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.DetailThingmodelDeviceResponse:
+        """
+        Description: 查询物模型设备详情
+        Summary: 查询物模型设备详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.DetailThingmodelDeviceResponse(),
+            self.do_request('1.0', 'blockchain.bot.thingmodel.device.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_thingmodel_device_ex_async(
+        self,
+        request: bot_models.DetailThingmodelDeviceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.DetailThingmodelDeviceResponse:
+        """
+        Description: 查询物模型设备详情
+        Summary: 查询物模型设备详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.DetailThingmodelDeviceResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.thingmodel.device.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_collector_uploadfileurl(
+        self,
+        request: bot_models.CreateCollectorUploadfileurlRequest,
+    ) -> bot_models.CreateCollectorUploadfileurlResponse:
+        """
+        Description: 通过CSV文件上报数据时，需要先通过这个接口获取上报地址URL
+        Summary: 创建上传文件URL
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_collector_uploadfileurl_ex(request, headers, runtime)
+
+    async def create_collector_uploadfileurl_async(
+        self,
+        request: bot_models.CreateCollectorUploadfileurlRequest,
+    ) -> bot_models.CreateCollectorUploadfileurlResponse:
+        """
+        Description: 通过CSV文件上报数据时，需要先通过这个接口获取上报地址URL
+        Summary: 创建上传文件URL
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_collector_uploadfileurl_ex_async(request, headers, runtime)
+
+    def create_collector_uploadfileurl_ex(
+        self,
+        request: bot_models.CreateCollectorUploadfileurlRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateCollectorUploadfileurlResponse:
+        """
+        Description: 通过CSV文件上报数据时，需要先通过这个接口获取上报地址URL
+        Summary: 创建上传文件URL
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateCollectorUploadfileurlResponse(),
+            self.do_request('1.0', 'blockchain.bot.collector.uploadfileurl.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_collector_uploadfileurl_ex_async(
+        self,
+        request: bot_models.CreateCollectorUploadfileurlRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.CreateCollectorUploadfileurlResponse:
+        """
+        Description: 通过CSV文件上报数据时，需要先通过这个接口获取上报地址URL
+        Summary: 创建上传文件URL
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.CreateCollectorUploadfileurlResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.collector.uploadfileurl.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def confirm_collector_uploadfile(
+        self,
+        request: bot_models.ConfirmCollectorUploadfileRequest,
+    ) -> bot_models.ConfirmCollectorUploadfileResponse:
+        """
+        Description: 通过文件上报数据流程，先获取上报文件URL，然后向目标URL中上传文件，最后调用此接口进行确认
+        Summary: 通过文件上报数据，上传完毕后确认
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.confirm_collector_uploadfile_ex(request, headers, runtime)
+
+    async def confirm_collector_uploadfile_async(
+        self,
+        request: bot_models.ConfirmCollectorUploadfileRequest,
+    ) -> bot_models.ConfirmCollectorUploadfileResponse:
+        """
+        Description: 通过文件上报数据流程，先获取上报文件URL，然后向目标URL中上传文件，最后调用此接口进行确认
+        Summary: 通过文件上报数据，上传完毕后确认
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.confirm_collector_uploadfile_ex_async(request, headers, runtime)
+
+    def confirm_collector_uploadfile_ex(
+        self,
+        request: bot_models.ConfirmCollectorUploadfileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ConfirmCollectorUploadfileResponse:
+        """
+        Description: 通过文件上报数据流程，先获取上报文件URL，然后向目标URL中上传文件，最后调用此接口进行确认
+        Summary: 通过文件上报数据，上传完毕后确认
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ConfirmCollectorUploadfileResponse(),
+            self.do_request('1.0', 'blockchain.bot.collector.uploadfile.confirm', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def confirm_collector_uploadfile_ex_async(
+        self,
+        request: bot_models.ConfirmCollectorUploadfileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.ConfirmCollectorUploadfileResponse:
+        """
+        Description: 通过文件上报数据流程，先获取上报文件URL，然后向目标URL中上传文件，最后调用此接口进行确认
+        Summary: 通过文件上报数据，上传完毕后确认
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.ConfirmCollectorUploadfileResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.collector.uploadfile.confirm', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def exec_thingsdid_oneapi(
         self,
         request: bot_models.ExecThingsdidOneapiRequest,
     ) -> bot_models.ExecThingsdidOneapiResponse:
         """
         Description: 信物链oneapi
         Summary: 信物链oneapi
```

### Comparing `antchain_bot-1.8.7/antchain_sdk_bot/models.py` & `antchain_bot-1.8.70/antchain_sdk_bot/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1369,14 +1369,142 @@
         if m.get('checkin_date') is not None:
             self.checkin_date = m.get('checkin_date')
         if m.get('checkout_date') is not None:
             self.checkout_date = m.get('checkout_date')
         return self
 
 
+class RegByDeviceIdParm(TeaModel):
+    def __init__(
+        self,
+        device_id: str = None,
+        device_data_model_id: str = None,
+        device_feature: str = None,
+        with_exist_device_id: bool = None,
+        device_type_code: int = None,
+        initial_price: int = None,
+        factory_time: str = None,
+        release_time: str = None,
+        extra_info: str = None,
+        owner: str = None,
+        owner_name: str = None,
+        device_imei: str = None,
+        device_name: str = None,
+        corp_name: str = None,
+    ):
+        # 一般是业务上唯一的设备ID/资产编码
+        self.device_id = device_id
+        # 数据模型ID
+        self.device_data_model_id = device_data_model_id
+        # 固定填写RAW_DATA
+        self.device_feature = device_feature
+        # true : 设备ID已存在时返回存在的设备关联字段;
+        # false : 设备ID已存在时直接抛出异常；
+        self.with_exist_device_id = with_exist_device_id
+        # 设备类型编码，联系蚂蚁侧获取设备类型编码
+        self.device_type_code = device_type_code
+        # 设备单价 单位：分
+        self.initial_price = initial_price
+        # 出厂时间
+        self.factory_time = factory_time
+        # 投放时间
+        self.release_time = release_time
+        # 额外信息，联系蚂蚁侧获取参数格式
+        self.extra_info = extra_info
+        # 资产所有人标识（统一社会信用代码）
+        self.owner = owner
+        # 资产所有人名称
+        self.owner_name = owner_name
+        # 设备IMEI
+        self.device_imei = device_imei
+        # 设备名称/设备型号
+        self.device_name = device_name
+        # 生产厂商名
+        self.corp_name = corp_name
+
+    def validate(self):
+        self.validate_required(self.device_id, 'device_id')
+        self.validate_required(self.device_data_model_id, 'device_data_model_id')
+        self.validate_required(self.device_feature, 'device_feature')
+        self.validate_required(self.with_exist_device_id, 'with_exist_device_id')
+        self.validate_required(self.device_type_code, 'device_type_code')
+        if self.factory_time is not None:
+            self.validate_pattern(self.factory_time, 'factory_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+        if self.release_time is not None:
+            self.validate_pattern(self.release_time, 'release_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        if self.device_data_model_id is not None:
+            result['device_data_model_id'] = self.device_data_model_id
+        if self.device_feature is not None:
+            result['device_feature'] = self.device_feature
+        if self.with_exist_device_id is not None:
+            result['with_exist_device_id'] = self.with_exist_device_id
+        if self.device_type_code is not None:
+            result['device_type_code'] = self.device_type_code
+        if self.initial_price is not None:
+            result['initial_price'] = self.initial_price
+        if self.factory_time is not None:
+            result['factory_time'] = self.factory_time
+        if self.release_time is not None:
+            result['release_time'] = self.release_time
+        if self.extra_info is not None:
+            result['extra_info'] = self.extra_info
+        if self.owner is not None:
+            result['owner'] = self.owner
+        if self.owner_name is not None:
+            result['owner_name'] = self.owner_name
+        if self.device_imei is not None:
+            result['device_imei'] = self.device_imei
+        if self.device_name is not None:
+            result['device_name'] = self.device_name
+        if self.corp_name is not None:
+            result['corp_name'] = self.corp_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        if m.get('device_data_model_id') is not None:
+            self.device_data_model_id = m.get('device_data_model_id')
+        if m.get('device_feature') is not None:
+            self.device_feature = m.get('device_feature')
+        if m.get('with_exist_device_id') is not None:
+            self.with_exist_device_id = m.get('with_exist_device_id')
+        if m.get('device_type_code') is not None:
+            self.device_type_code = m.get('device_type_code')
+        if m.get('initial_price') is not None:
+            self.initial_price = m.get('initial_price')
+        if m.get('factory_time') is not None:
+            self.factory_time = m.get('factory_time')
+        if m.get('release_time') is not None:
+            self.release_time = m.get('release_time')
+        if m.get('extra_info') is not None:
+            self.extra_info = m.get('extra_info')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
+        if m.get('owner_name') is not None:
+            self.owner_name = m.get('owner_name')
+        if m.get('device_imei') is not None:
+            self.device_imei = m.get('device_imei')
+        if m.get('device_name') is not None:
+            self.device_name = m.get('device_name')
+        if m.get('corp_name') is not None:
+            self.corp_name = m.get('corp_name')
+        return self
+
+
 class SdkPageResponse(TeaModel):
     def __init__(
         self,
         page_index: int = None,
         page_size: int = None,
         total_size: int = None,
         total_pages: int = None,
@@ -1442,14 +1570,50 @@
         if m.get('page_data') is not None:
             for k in m.get('page_data'):
                 temp_model = SdkModel()
                 self.page_data.append(temp_model.from_map(k))
         return self
 
 
+class CodeListView(TeaModel):
+    def __init__(
+        self,
+        data_code: str = None,
+        data_name: str = None,
+    ):
+        # 数据code
+        self.data_code = data_code
+        # 数据名称
+        self.data_name = data_name
+
+    def validate(self):
+        self.validate_required(self.data_code, 'data_code')
+        self.validate_required(self.data_name, 'data_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_code is not None:
+            result['data_code'] = self.data_code
+        if self.data_name is not None:
+            result['data_name'] = self.data_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('data_code') is not None:
+            self.data_code = m.get('data_code')
+        if m.get('data_name') is not None:
+            self.data_name = m.get('data_name')
+        return self
+
+
 class IotBasicDeviceQueryResponse(TeaModel):
     def __init__(
         self,
         device_name: str = None,
         device_sn: str = None,
         device_category_name: str = None,
         device_model: str = None,
@@ -1724,14 +1888,50 @@
         if m.get('device_ext') is not None:
             self.device_ext = m.get('device_ext')
         if m.get('sec_id') is not None:
             self.sec_id = m.get('sec_id')
         return self
 
 
+class CustomEntityInfo(TeaModel):
+    def __init__(
+        self,
+        customer_entity_type: str = None,
+        customer_entity_content: str = None,
+    ):
+        # 客户自定义实体类型，默认为JSSDK_ACCOUNT
+        self.customer_entity_type = customer_entity_type
+        # 客户自定义实体内容
+        self.customer_entity_content = customer_entity_content
+
+    def validate(self):
+        self.validate_required(self.customer_entity_type, 'customer_entity_type')
+        self.validate_required(self.customer_entity_content, 'customer_entity_content')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.customer_entity_type is not None:
+            result['customer_entity_type'] = self.customer_entity_type
+        if self.customer_entity_content is not None:
+            result['customer_entity_content'] = self.customer_entity_content
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('customer_entity_type') is not None:
+            self.customer_entity_type = m.get('customer_entity_type')
+        if m.get('customer_entity_content') is not None:
+            self.customer_entity_content = m.get('customer_entity_content')
+        return self
+
+
 class BaiQrcodeComparisonReqData(TeaModel):
     def __init__(
         self,
         trace_id: str = None,
         query_image_location: BaiResourceLocation = None,
         gallery_image_location: BaiResourceLocation = None,
         downgrade: bool = None,
@@ -1784,14 +1984,63 @@
             temp_model = BaiResourceLocation()
             self.gallery_image_location = temp_model.from_map(m['gallery_image_location'])
         if m.get('downgrade') is not None:
             self.downgrade = m.get('downgrade')
         return self
 
 
+class XrUserTicketResultInfo(TeaModel):
+    def __init__(
+        self,
+        xr_ticket_pool_name: str = None,
+        count: int = None,
+        error_msg: str = None,
+        xr_ticket_code: str = None,
+    ):
+        # xr通行证资源池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 购买数量，失败列表有值
+        self.count = count
+        # 失败原因，失败列表有值
+        self.error_msg = error_msg
+        # 通行证编号，成功列表有值
+        self.xr_ticket_code = xr_ticket_code
+
+    def validate(self):
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.count is not None:
+            result['count'] = self.count
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.xr_ticket_code is not None:
+            result['xr_ticket_code'] = self.xr_ticket_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('count') is not None:
+            self.count = m.get('count')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('xr_ticket_code') is not None:
+            self.xr_ticket_code = m.get('xr_ticket_code')
+        return self
+
+
 class WarehouseReqModel(TeaModel):
     def __init__(
         self,
         address: str = None,
         area: int = None,
         elevation: int = None,
         height: int = None,
@@ -1982,14 +2231,50 @@
         if m.get('goods_id_and_count') is not None:
             for k in m.get('goods_id_and_count'):
                 temp_model = GoodsIdAndCount()
                 self.goods_id_and_count.append(temp_model.from_map(k))
         return self
 
 
+class InstanceInfo(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        instance_name: str = None,
+    ):
+        # 实例id
+        self.instance_id = instance_id
+        # 实例名称
+        self.instance_name = instance_name
+
+    def validate(self):
+        self.validate_required(self.instance_id, 'instance_id')
+        self.validate_required(self.instance_name, 'instance_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['instance_id'] = self.instance_id
+        if self.instance_name is not None:
+            result['instance_name'] = self.instance_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('instance_id') is not None:
+            self.instance_id = m.get('instance_id')
+        if m.get('instance_name') is not None:
+            self.instance_name = m.get('instance_name')
+        return self
+
+
 class DeviceDisableData(TeaModel):
     def __init__(
         self,
         device_sn: str = None,
         corp_name: str = None,
     ):
         # 设备sn号
@@ -2729,14 +3014,97 @@
         if m.get('detail_elec_money') is not None:
             self.detail_elec_money = m.get('detail_elec_money')
         if m.get('detail_service_money') is not None:
             self.detail_service_money = m.get('detail_service_money')
         return self
 
 
+class XrTicketPoolSuccessList(TeaModel):
+    def __init__(
+        self,
+        tenant_id: str = None,
+        resource_id: str = None,
+        valid_time: str = None,
+        test_time: int = None,
+        xr_apps: str = None,
+        max_pool_count: int = None,
+        xr_ticket_pool_name: str = None,
+        xr_verification_type: str = None,
+    ):
+        # 租户id
+        self.tenant_id = tenant_id
+        # 资源id
+        self.resource_id = resource_id
+        # 有效期
+        self.valid_time = valid_time
+        # 体验时长
+        self.test_time = test_time
+        # vr设备集合
+        self.xr_apps = xr_apps
+        # 券池最大数
+        self.max_pool_count = max_pool_count
+        # 券池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.valid_time, 'valid_time')
+        self.validate_required(self.test_time, 'test_time')
+        self.validate_required(self.max_pool_count, 'max_pool_count')
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.test_time is not None:
+            result['test_time'] = self.test_time
+        if self.xr_apps is not None:
+            result['xr_apps'] = self.xr_apps
+        if self.max_pool_count is not None:
+            result['max_pool_count'] = self.max_pool_count
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('test_time') is not None:
+            self.test_time = m.get('test_time')
+        if m.get('xr_apps') is not None:
+            self.xr_apps = m.get('xr_apps')
+        if m.get('max_pool_count') is not None:
+            self.max_pool_count = m.get('max_pool_count')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        return self
+
+
 class UpdateDeviceSpaceReq(TeaModel):
     def __init__(
         self,
         device_did: str = None,
         update_mode: int = None,
         device_space: List[str] = None,
     ):
@@ -3189,14 +3557,164 @@
         if m.get('device_no') is not None:
             self.device_no = m.get('device_no')
         if m.get('operation_date') is not None:
             self.operation_date = m.get('operation_date')
         return self
 
 
+class XrUserTicketDetail(TeaModel):
+    def __init__(
+        self,
+        biz_scene: str = None,
+        tenant_id: str = None,
+        xr_ticket_code: str = None,
+        xr_ticket_pool_name: str = None,
+        user_id: str = None,
+        resource_id: str = None,
+        resource_name: str = None,
+        status: str = None,
+        valid_time: str = None,
+        instance_id: str = None,
+        xr_verification_time: str = None,
+        sample_start_time: str = None,
+        sample_end_time: str = None,
+        xr_verification_type: str = None,
+        instance_name: str = None,
+        test_time: int = None,
+        xr_apps: str = None,
+    ):
+        # 业务类型
+        self.biz_scene = biz_scene
+        # 所属客户
+        self.tenant_id = tenant_id
+        # 用户通行证编码
+        self.xr_ticket_code = xr_ticket_code
+        # xr通行证资源池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 用户id
+        self.user_id = user_id
+        # 资源id
+        self.resource_id = resource_id
+        # 资源名称
+        self.resource_name = resource_name
+        # 用户通行证状态
+        self.status = status
+        # 有效期
+        self.valid_time = valid_time
+        # 实例id
+        self.instance_id = instance_id
+        # 核销时间
+        self.xr_verification_time = xr_verification_time
+        # 体验开始时间
+        self.sample_start_time = sample_start_time
+        # 体验结束时间
+        self.sample_end_time = sample_end_time
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+        # 实例名称
+        self.instance_name = instance_name
+        # 体验时长，分
+        self.test_time = test_time
+        # vr应用集合
+        self.xr_apps = xr_apps
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.xr_ticket_code, 'xr_ticket_code')
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.resource_name, 'resource_name')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.valid_time, 'valid_time')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+        self.validate_required(self.test_time, 'test_time')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.xr_ticket_code is not None:
+            result['xr_ticket_code'] = self.xr_ticket_code
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.resource_name is not None:
+            result['resource_name'] = self.resource_name
+        if self.status is not None:
+            result['status'] = self.status
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.instance_id is not None:
+            result['instance_id'] = self.instance_id
+        if self.xr_verification_time is not None:
+            result['xr_verification_time'] = self.xr_verification_time
+        if self.sample_start_time is not None:
+            result['sample_start_time'] = self.sample_start_time
+        if self.sample_end_time is not None:
+            result['sample_end_time'] = self.sample_end_time
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        if self.instance_name is not None:
+            result['instance_name'] = self.instance_name
+        if self.test_time is not None:
+            result['test_time'] = self.test_time
+        if self.xr_apps is not None:
+            result['xr_apps'] = self.xr_apps
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('xr_ticket_code') is not None:
+            self.xr_ticket_code = m.get('xr_ticket_code')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('resource_name') is not None:
+            self.resource_name = m.get('resource_name')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('instance_id') is not None:
+            self.instance_id = m.get('instance_id')
+        if m.get('xr_verification_time') is not None:
+            self.xr_verification_time = m.get('xr_verification_time')
+        if m.get('sample_start_time') is not None:
+            self.sample_start_time = m.get('sample_start_time')
+        if m.get('sample_end_time') is not None:
+            self.sample_end_time = m.get('sample_end_time')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        if m.get('instance_name') is not None:
+            self.instance_name = m.get('instance_name')
+        if m.get('test_time') is not None:
+            self.test_time = m.get('test_time')
+        if m.get('xr_apps') is not None:
+            self.xr_apps = m.get('xr_apps')
+        return self
+
+
 class DidBaseQueryReq(TeaModel):
     def __init__(
         self,
         data_filter: List[str] = None,
         on_chain: bool = None,
         things_did_list: List[str] = None,
     ):
@@ -3617,14 +4135,82 @@
         if m.get('distribute_device_id') is not None:
             self.distribute_device_id = m.get('distribute_device_id')
         if m.get('package_time') is not None:
             self.package_time = m.get('package_time')
         return self
 
 
+class XrTicketPoolFailList(TeaModel):
+    def __init__(
+        self,
+        xr_ticket_pool_name: str = None,
+        resource_id: str = None,
+        error_code: str = None,
+        tenant_id: str = None,
+        error_msg: str = None,
+        xr_verification_type: str = None,
+    ):
+        # 券名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 资源id
+        self.resource_id = resource_id
+        # 错误码
+        self.error_code = error_code
+        # 租户id
+        self.tenant_id = tenant_id
+        # 错误信息
+        self.error_msg = error_msg
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+
+    def validate(self):
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.error_code, 'error_code')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.error_msg, 'error_msg')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        return self
+
+
 class BaiOcrResponse(TeaModel):
     def __init__(
         self,
         data: str = None,
     ):
         # 返回的结果体
         self.data = data
@@ -3673,14 +4259,142 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('query_image_url') is not None:
             self.query_image_url = m.get('query_image_url')
         return self
 
 
+class XrVerificationModelVo(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        instance_name: str = None,
+        valid_time: str = None,
+        sevice_status: str = None,
+        device_status: str = None,
+        resource_id: str = None,
+        resource_name: str = None,
+        type: str = None,
+    ):
+        # 核销资源生成的实例，xr设备对应设备did
+        self.instance_id = instance_id
+        # 生成的实例名称，xr设备就的对应的具体设备sn
+        self.instance_name = instance_name
+        # 线下场有效期
+        self.valid_time = valid_time
+        # 服务状态：INIT初始化、SERVICING服务中、PAUSED已暂停、EXPIRED停用
+        self.sevice_status = sevice_status
+        # 设备状态：INIT 初始化、ONLINE 在线、OFFLINE 离线、FAULT 故障、ACTIVATED 激活
+        self.device_status = device_status
+        # 唯一ID，对应线下场code
+        self.resource_id = resource_id
+        # 对应线下场名称
+        self.resource_name = resource_name
+        # 核销类型
+        self.type = type
+
+    def validate(self):
+        self.validate_required(self.instance_id, 'instance_id')
+        self.validate_required(self.instance_name, 'instance_name')
+        self.validate_required(self.valid_time, 'valid_time')
+        self.validate_required(self.sevice_status, 'sevice_status')
+        self.validate_required(self.device_status, 'device_status')
+        self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.resource_name, 'resource_name')
+        self.validate_required(self.type, 'type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['instance_id'] = self.instance_id
+        if self.instance_name is not None:
+            result['instance_name'] = self.instance_name
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.sevice_status is not None:
+            result['sevice_status'] = self.sevice_status
+        if self.device_status is not None:
+            result['device_status'] = self.device_status
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.resource_name is not None:
+            result['resource_name'] = self.resource_name
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('instance_id') is not None:
+            self.instance_id = m.get('instance_id')
+        if m.get('instance_name') is not None:
+            self.instance_name = m.get('instance_name')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('sevice_status') is not None:
+            self.sevice_status = m.get('sevice_status')
+        if m.get('device_status') is not None:
+            self.device_status = m.get('device_status')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('resource_name') is not None:
+            self.resource_name = m.get('resource_name')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class BizStatusInfoOp(TeaModel):
+    def __init__(
+        self,
+        biz_type: str = None,
+        biz_status: str = None,
+        op_time: str = None,
+    ):
+        # 业务状态类型
+        self.biz_type = biz_type
+        # 业务状态
+        self.biz_status = biz_status
+        # 时间
+        self.op_time = op_time
+
+    def validate(self):
+        self.validate_required(self.biz_type, 'biz_type')
+        self.validate_required(self.biz_status, 'biz_status')
+        self.validate_required(self.op_time, 'op_time')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
+        if self.biz_status is not None:
+            result['biz_status'] = self.biz_status
+        if self.op_time is not None:
+            result['op_time'] = self.op_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        if m.get('biz_status') is not None:
+            self.biz_status = m.get('biz_status')
+        if m.get('op_time') is not None:
+            self.op_time = m.get('op_time')
+        return self
+
+
 class ThingsDidRegisterReq(TeaModel):
     def __init__(
         self,
         biz_type: str = None,
         owner_tenant_did: str = None,
         thing_extra_params: str = None,
         thing_origin_id: str = None,
@@ -4089,14 +4803,89 @@
         if m.get('p1') is not None:
             self.p_1 = m.get('p1')
         if m.get('p2') is not None:
             self.p_2 = m.get('p2')
         return self
 
 
+class XrTicketPoolBatchReq(TeaModel):
+    def __init__(
+        self,
+        resource_id: str = None,
+        valid_time: str = None,
+        test_time: int = None,
+        xr_apps: str = None,
+        max_pool_count: int = None,
+        xr_ticket_pool_name: str = None,
+        xr_verification_type: str = None,
+    ):
+        # 资源id
+        self.resource_id = resource_id
+        # 通行证有效期
+        self.valid_time = valid_time
+        # 体验时长
+        self.test_time = test_time
+        # vr设备集合
+        self.xr_apps = xr_apps
+        # 券池最大出票数
+        self.max_pool_count = max_pool_count
+        # 通行证名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+
+    def validate(self):
+        self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.valid_time, 'valid_time')
+        self.validate_required(self.test_time, 'test_time')
+        self.validate_required(self.max_pool_count, 'max_pool_count')
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.test_time is not None:
+            result['test_time'] = self.test_time
+        if self.xr_apps is not None:
+            result['xr_apps'] = self.xr_apps
+        if self.max_pool_count is not None:
+            result['max_pool_count'] = self.max_pool_count
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('test_time') is not None:
+            self.test_time = m.get('test_time')
+        if m.get('xr_apps') is not None:
+            self.xr_apps = m.get('xr_apps')
+        if m.get('max_pool_count') is not None:
+            self.max_pool_count = m.get('max_pool_count')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        return self
+
+
 class DeviceControlFail(TeaModel):
     def __init__(
         self,
         device_did: str = None,
         code: str = None,
         message: str = None,
     ):
@@ -4133,14 +4922,261 @@
         if m.get('code') is not None:
             self.code = m.get('code')
         if m.get('message') is not None:
             self.message = m.get('message')
         return self
 
 
+class RegByDeviceParm(TeaModel):
+    def __init__(
+        self,
+        device_id: str = None,
+        device_data_model_id: str = None,
+        device_reg_content: str = None,
+        device_reg_signature: str = None,
+        sdk_id: str = None,
+        device_type_code: int = None,
+        initial_price: int = None,
+        factory_time: str = None,
+        release_time: str = None,
+        extra_info: str = None,
+        owner: str = None,
+        owner_name: str = None,
+        device_name: str = None,
+    ):
+        # 一般是业务上唯一的设备ID/资产编码
+        # 
+        self.device_id = device_id
+        # 数据模型ID
+        self.device_data_model_id = device_data_model_id
+        # 设备端经过蚂蚁SDK或模组初始化得到的注册信息
+        self.device_reg_content = device_reg_content
+        # 蚂蚁侧SDK或模组对device_reg_content的签名
+        self.device_reg_signature = device_reg_signature
+        # sdk版本号，由蚂蚁侧提供
+        self.sdk_id = sdk_id
+        # 设备类型编码，联系蚂蚁侧获取设备类型编码
+        # 
+        self.device_type_code = device_type_code
+        # 设备单价 单位：分
+        # 
+        self.initial_price = initial_price
+        # 出厂时间
+        # 
+        self.factory_time = factory_time
+        # 投放时间
+        # 
+        self.release_time = release_time
+        # 额外信息，联系蚂蚁侧获取参数格式
+        # 
+        self.extra_info = extra_info
+        # 资产所有人标识（统一社会信用代码）
+        # 
+        self.owner = owner
+        # 资产所有人名称
+        self.owner_name = owner_name
+        # 设备名称/型号
+        self.device_name = device_name
+
+    def validate(self):
+        self.validate_required(self.device_id, 'device_id')
+        self.validate_required(self.device_data_model_id, 'device_data_model_id')
+        self.validate_required(self.device_reg_content, 'device_reg_content')
+        self.validate_required(self.device_reg_signature, 'device_reg_signature')
+        self.validate_required(self.sdk_id, 'sdk_id')
+        self.validate_required(self.device_type_code, 'device_type_code')
+        if self.factory_time is not None:
+            self.validate_pattern(self.factory_time, 'factory_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+        if self.release_time is not None:
+            self.validate_pattern(self.release_time, 'release_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        if self.device_data_model_id is not None:
+            result['device_data_model_id'] = self.device_data_model_id
+        if self.device_reg_content is not None:
+            result['device_reg_content'] = self.device_reg_content
+        if self.device_reg_signature is not None:
+            result['device_reg_signature'] = self.device_reg_signature
+        if self.sdk_id is not None:
+            result['sdk_id'] = self.sdk_id
+        if self.device_type_code is not None:
+            result['device_type_code'] = self.device_type_code
+        if self.initial_price is not None:
+            result['initial_price'] = self.initial_price
+        if self.factory_time is not None:
+            result['factory_time'] = self.factory_time
+        if self.release_time is not None:
+            result['release_time'] = self.release_time
+        if self.extra_info is not None:
+            result['extra_info'] = self.extra_info
+        if self.owner is not None:
+            result['owner'] = self.owner
+        if self.owner_name is not None:
+            result['owner_name'] = self.owner_name
+        if self.device_name is not None:
+            result['device_name'] = self.device_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        if m.get('device_data_model_id') is not None:
+            self.device_data_model_id = m.get('device_data_model_id')
+        if m.get('device_reg_content') is not None:
+            self.device_reg_content = m.get('device_reg_content')
+        if m.get('device_reg_signature') is not None:
+            self.device_reg_signature = m.get('device_reg_signature')
+        if m.get('sdk_id') is not None:
+            self.sdk_id = m.get('sdk_id')
+        if m.get('device_type_code') is not None:
+            self.device_type_code = m.get('device_type_code')
+        if m.get('initial_price') is not None:
+            self.initial_price = m.get('initial_price')
+        if m.get('factory_time') is not None:
+            self.factory_time = m.get('factory_time')
+        if m.get('release_time') is not None:
+            self.release_time = m.get('release_time')
+        if m.get('extra_info') is not None:
+            self.extra_info = m.get('extra_info')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
+        if m.get('owner_name') is not None:
+            self.owner_name = m.get('owner_name')
+        if m.get('device_name') is not None:
+            self.device_name = m.get('device_name')
+        return self
+
+
+class XrTicketPoolItem(TeaModel):
+    def __init__(
+        self,
+        biz_scene: str = None,
+        xr_ticket_pool_name: str = None,
+        resource_id: str = None,
+        valid_time: str = None,
+        test_time: int = None,
+        status: str = None,
+        use_status: str = None,
+        resource_name: str = None,
+        xr_apps: str = None,
+        max_pool_count: int = None,
+        tenant_id: str = None,
+        xr_verification_type: str = None,
+        surplus_count: int = None,
+        issued_count: int = None,
+    ):
+        # 业务类型
+        self.biz_scene = biz_scene
+        # 通行证名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 资源id
+        self.resource_id = resource_id
+        # 有效期
+        self.valid_time = valid_time
+        # 体验时长
+        self.test_time = test_time
+        # 通行证状态：EXPIRED：已过期  VALID：有效  SALED：已出售
+        self.status = status
+        # 判断已发放数量>0(USED：已使用)  判断已发放数量=0(NOT_USED：未使用)
+        self.use_status = use_status
+        # 资源名称
+        self.resource_name = resource_name
+        # 设备集合
+        self.xr_apps = xr_apps
+        # 券池最大票数
+        self.max_pool_count = max_pool_count
+        # 租户id
+        self.tenant_id = tenant_id
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+        # 剩余可用券数量
+        self.surplus_count = surplus_count
+        # 已发放数量 （总数-剩余数量）
+        self.issued_count = issued_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.test_time is not None:
+            result['test_time'] = self.test_time
+        if self.status is not None:
+            result['status'] = self.status
+        if self.use_status is not None:
+            result['use_status'] = self.use_status
+        if self.resource_name is not None:
+            result['resource_name'] = self.resource_name
+        if self.xr_apps is not None:
+            result['xr_apps'] = self.xr_apps
+        if self.max_pool_count is not None:
+            result['max_pool_count'] = self.max_pool_count
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        if self.surplus_count is not None:
+            result['surplus_count'] = self.surplus_count
+        if self.issued_count is not None:
+            result['issued_count'] = self.issued_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('test_time') is not None:
+            self.test_time = m.get('test_time')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('use_status') is not None:
+            self.use_status = m.get('use_status')
+        if m.get('resource_name') is not None:
+            self.resource_name = m.get('resource_name')
+        if m.get('xr_apps') is not None:
+            self.xr_apps = m.get('xr_apps')
+        if m.get('max_pool_count') is not None:
+            self.max_pool_count = m.get('max_pool_count')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        if m.get('surplus_count') is not None:
+            self.surplus_count = m.get('surplus_count')
+        if m.get('issued_count') is not None:
+            self.issued_count = m.get('issued_count')
+        return self
+
+
 class EvidenceBaseModel(TeaModel):
     def __init__(
         self,
         biz_data: str = None,
         hash: str = None,
         meta_json: str = None,
     ):
@@ -4951,14 +5987,50 @@
         if m.get('collect_id') is not None:
             self.collect_id = m.get('collect_id')
         if m.get('antchain_id') is not None:
             self.antchain_id = m.get('antchain_id')
         return self
 
 
+class TrustiotDeviceIdMap(TeaModel):
+    def __init__(
+        self,
+        trustiot_device_id: int = None,
+        device_id: str = None,
+    ):
+        # 可信设备ID
+        self.trustiot_device_id = trustiot_device_id
+        # 设备ID
+        self.device_id = device_id
+
+    def validate(self):
+        self.validate_required(self.trustiot_device_id, 'trustiot_device_id')
+        self.validate_required(self.device_id, 'device_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.trustiot_device_id is not None:
+            result['trustiot_device_id'] = self.trustiot_device_id
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('trustiot_device_id') is not None:
+            self.trustiot_device_id = m.get('trustiot_device_id')
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        return self
+
+
 class ProductKeyPageResponse(TeaModel):
     def __init__(
         self,
         page_index: int = None,
         page_size: int = None,
         total_size: int = None,
         total_pages: int = None,
@@ -5198,14 +6270,106 @@
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class XrUserTicketPageInfo(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+        xr_ticket_code: str = None,
+        xr_ticket_pool_name: str = None,
+        resource_name: str = None,
+        status: str = None,
+        valid_time: str = None,
+        biz_scene: str = None,
+        tenant_id: str = None,
+        xr_verification_type: str = None,
+    ):
+        # 用户id
+        self.user_id = user_id
+        # 用户通行证编码
+        self.xr_ticket_code = xr_ticket_code
+        # xr通行证资源池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 资源名称
+        self.resource_name = resource_name
+        # 用户通行证状态
+        self.status = status
+        # 有效期
+        self.valid_time = valid_time
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 租户id
+        self.tenant_id = tenant_id
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.xr_ticket_code, 'xr_ticket_code')
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.resource_name, 'resource_name')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.valid_time, 'valid_time')
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.xr_ticket_code is not None:
+            result['xr_ticket_code'] = self.xr_ticket_code
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.resource_name is not None:
+            result['resource_name'] = self.resource_name
+        if self.status is not None:
+            result['status'] = self.status
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('xr_ticket_code') is not None:
+            self.xr_ticket_code = m.get('xr_ticket_code')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('resource_name') is not None:
+            self.resource_name = m.get('resource_name')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        return self
+
+
 class LabelTrace(TeaModel):
     def __init__(
         self,
         content: str = None,
         tx_hash: str = None,
         tx_time: str = None,
         error_code: str = None,
@@ -5793,14 +6957,113 @@
         if m.get('page_data') is not None:
             for k in m.get('page_data'):
                 temp_model = SceneModel()
                 self.page_data.append(temp_model.from_map(k))
         return self
 
 
+class CustomerDeviceItem(TeaModel):
+    def __init__(
+        self,
+        id: int = None,
+        tenant_id: str = None,
+        account_id: str = None,
+        device_type: str = None,
+        device_sn: str = None,
+        device_did: str = None,
+        valide_time: str = None,
+        device_status: str = None,
+        service_status: str = None,
+        screen_status: str = None,
+    ):
+        # id
+        self.id = id
+        # 租户id
+        self.tenant_id = tenant_id
+        # 账号id
+        self.account_id = account_id
+        # 设备品类-型号-规格
+        self.device_type = device_type
+        # 设备sn
+        self.device_sn = device_sn
+        # 设备did
+        self.device_did = device_did
+        # 服务有效期
+        self.valide_time = valide_time
+        # 设备状态
+        self.device_status = device_status
+        # 服务状态
+        self.service_status = service_status
+        # 屏幕状态 开屏、锁屏
+        self.screen_status = screen_status
+
+    def validate(self):
+        self.validate_required(self.id, 'id')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.account_id, 'account_id')
+        self.validate_required(self.device_type, 'device_type')
+        self.validate_required(self.device_sn, 'device_sn')
+        self.validate_required(self.device_did, 'device_did')
+        self.validate_required(self.valide_time, 'valide_time')
+        self.validate_required(self.device_status, 'device_status')
+        self.validate_required(self.service_status, 'service_status')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['id'] = self.id
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.account_id is not None:
+            result['account_id'] = self.account_id
+        if self.device_type is not None:
+            result['device_type'] = self.device_type
+        if self.device_sn is not None:
+            result['device_sn'] = self.device_sn
+        if self.device_did is not None:
+            result['device_did'] = self.device_did
+        if self.valide_time is not None:
+            result['valide_time'] = self.valide_time
+        if self.device_status is not None:
+            result['device_status'] = self.device_status
+        if self.service_status is not None:
+            result['service_status'] = self.service_status
+        if self.screen_status is not None:
+            result['screen_status'] = self.screen_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('account_id') is not None:
+            self.account_id = m.get('account_id')
+        if m.get('device_type') is not None:
+            self.device_type = m.get('device_type')
+        if m.get('device_sn') is not None:
+            self.device_sn = m.get('device_sn')
+        if m.get('device_did') is not None:
+            self.device_did = m.get('device_did')
+        if m.get('valide_time') is not None:
+            self.valide_time = m.get('valide_time')
+        if m.get('device_status') is not None:
+            self.device_status = m.get('device_status')
+        if m.get('service_status') is not None:
+            self.service_status = m.get('service_status')
+        if m.get('screen_status') is not None:
+            self.screen_status = m.get('screen_status')
+        return self
+
+
 class DidBaseQueryResp(TeaModel):
     def __init__(
         self,
         auth_level: int = None,
         cert_public_key: str = None,
         cert_text: str = None,
         did_extension: str = None,
@@ -5949,14 +7212,50 @@
         if m.get('user_did_list') is not None:
             self.user_did_list = m.get('user_did_list')
         if m.get('did') is not None:
             self.did = m.get('did')
         return self
 
 
+class XrUserTicketInfo(TeaModel):
+    def __init__(
+        self,
+        xr_ticket_pool_name: str = None,
+        count: int = None,
+    ):
+        # xr通行证资源池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 购买数量
+        self.count = count
+
+    def validate(self):
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.count, 'count')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.count is not None:
+            result['count'] = self.count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('count') is not None:
+            self.count = m.get('count')
+        return self
+
+
 class IotBasicUserRequest(TeaModel):
     def __init__(
         self,
         tenant_id: str = None,
         cloud_user_id: str = None,
         login_name: str = None,
     ):
@@ -6713,14 +8012,50 @@
         if m.get('asset_data') is not None:
             self.asset_data = m.get('asset_data')
         if m.get('collect_id') is not None:
             self.collect_id = m.get('collect_id')
         return self
 
 
+class IdListView(TeaModel):
+    def __init__(
+        self,
+        data_id: int = None,
+        data_name: str = None,
+    ):
+        # 数据id
+        self.data_id = data_id
+        # 数据名称
+        self.data_name = data_name
+
+    def validate(self):
+        self.validate_required(self.data_id, 'data_id')
+        self.validate_required(self.data_name, 'data_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_id is not None:
+            result['data_id'] = self.data_id
+        if self.data_name is not None:
+            result['data_name'] = self.data_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('data_id') is not None:
+            self.data_id = m.get('data_id')
+        if m.get('data_name') is not None:
+            self.data_name = m.get('data_name')
+        return self
+
+
 class XNameValuePair(TeaModel):
     def __init__(
         self,
         name: str = None,
         value: str = None,
     ):
         # 键名
@@ -7450,14 +8785,2236 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('data') is not None:
             self.data = m.get('data')
         return self
 
 
+class CreateXrUserticketRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        user_id: str = None,
+        xr_user_ticket_list: List[XrUserTicketInfo] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 用户id
+        self.user_id = user_id
+        # 购买的通行证列表详情
+        self.xr_user_ticket_list = xr_user_ticket_list
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.xr_user_ticket_list, 'xr_user_ticket_list')
+        if self.xr_user_ticket_list:
+            for k in self.xr_user_ticket_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        result['xr_user_ticket_list'] = []
+        if self.xr_user_ticket_list is not None:
+            for k in self.xr_user_ticket_list:
+                result['xr_user_ticket_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        self.xr_user_ticket_list = []
+        if m.get('xr_user_ticket_list') is not None:
+            for k in m.get('xr_user_ticket_list'):
+                temp_model = XrUserTicketInfo()
+                self.xr_user_ticket_list.append(temp_model.from_map(k))
+        return self
+
+
+class CreateXrUserticketResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        success_list: List[XrUserTicketResultInfo] = None,
+        fail_list: List[XrUserTicketResultInfo] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 成功列表
+        self.success_list = success_list
+        # 失败列表
+        self.fail_list = fail_list
+
+    def validate(self):
+        if self.success_list:
+            for k in self.success_list:
+                if k:
+                    k.validate()
+        if self.fail_list:
+            for k in self.fail_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        result['success_list'] = []
+        if self.success_list is not None:
+            for k in self.success_list:
+                result['success_list'].append(k.to_map() if k else None)
+        result['fail_list'] = []
+        if self.fail_list is not None:
+            for k in self.fail_list:
+                result['fail_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        self.success_list = []
+        if m.get('success_list') is not None:
+            for k in m.get('success_list'):
+                temp_model = XrUserTicketResultInfo()
+                self.success_list.append(temp_model.from_map(k))
+        self.fail_list = []
+        if m.get('fail_list') is not None:
+            for k in m.get('fail_list'):
+                temp_model = XrUserTicketResultInfo()
+                self.fail_list.append(temp_model.from_map(k))
+        return self
+
+
+class ListXrXrticketpoolRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 所属业务
+        self.biz_scene = biz_scene
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        return self
+
+
+class ListXrXrticketpoolResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        xr_ticket_pool_list: List[IdListView] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 资源池列表
+        self.xr_ticket_pool_list = xr_ticket_pool_list
+
+    def validate(self):
+        if self.xr_ticket_pool_list:
+            for k in self.xr_ticket_pool_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        result['xr_ticket_pool_list'] = []
+        if self.xr_ticket_pool_list is not None:
+            for k in self.xr_ticket_pool_list:
+                result['xr_ticket_pool_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        self.xr_ticket_pool_list = []
+        if m.get('xr_ticket_pool_list') is not None:
+            for k in m.get('xr_ticket_pool_list'):
+                temp_model = IdListView()
+                self.xr_ticket_pool_list.append(temp_model.from_map(k))
+        return self
+
+
+class PagequeryXrUserticketRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        resource_id: str = None,
+        user_id: str = None,
+        status: str = None,
+        current: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 资源id
+        self.resource_id = resource_id
+        # 用户id
+        self.user_id = user_id
+        # 用户通行证状态，
+        # VALID：待核销
+        # WRITE_OFF：已核销
+        # EXPIRED：已过期
+        self.status = status
+        # 当前页
+        self.current = current
+        # 每页数量
+        self.page_size = page_size
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.current, 'current')
+        self.validate_required(self.page_size, 'page_size')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.status is not None:
+            result['status'] = self.status
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class PagequeryXrUserticketResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        xr_user_ticket_list: List[XrUserTicketPageInfo] = None,
+        current: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 用户通行证列表
+        self.xr_user_ticket_list = xr_user_ticket_list
+        # 当前页码
+        self.current = current
+        # 每页条数
+        self.page_size = page_size
+        # 总数量
+        self.total = total
+
+    def validate(self):
+        if self.xr_user_ticket_list:
+            for k in self.xr_user_ticket_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        result['xr_user_ticket_list'] = []
+        if self.xr_user_ticket_list is not None:
+            for k in self.xr_user_ticket_list:
+                result['xr_user_ticket_list'].append(k.to_map() if k else None)
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        self.xr_user_ticket_list = []
+        if m.get('xr_user_ticket_list') is not None:
+            for k in m.get('xr_user_ticket_list'):
+                temp_model = XrUserTicketPageInfo()
+                self.xr_user_ticket_list.append(temp_model.from_map(k))
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        return self
+
+
+class GetXrUserticketRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        xr_ticket_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 用户通行证编码
+        self.xr_ticket_code = xr_ticket_code
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.xr_ticket_code, 'xr_ticket_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.xr_ticket_code is not None:
+            result['xr_ticket_code'] = self.xr_ticket_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('xr_ticket_code') is not None:
+            self.xr_ticket_code = m.get('xr_ticket_code')
+        return self
+
+
+class GetXrUserticketResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        xr_user_ticket: XrUserTicketDetail = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 用户通行证详情
+        self.xr_user_ticket = xr_user_ticket
+
+    def validate(self):
+        if self.xr_user_ticket:
+            self.xr_user_ticket.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.xr_user_ticket is not None:
+            result['xr_user_ticket'] = self.xr_user_ticket.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('xr_user_ticket') is not None:
+            temp_model = XrUserTicketDetail()
+            self.xr_user_ticket = temp_model.from_map(m['xr_user_ticket'])
+        return self
+
+
+class OperateXrUserticketRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        xr_ticket_code: str = None,
+        user_id: str = None,
+        instance_id: str = None,
+        xr_verification_operate: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 用户通行证编码
+        self.xr_ticket_code = xr_ticket_code
+        # 用户id
+        self.user_id = user_id
+        # 实例id
+        self.instance_id = instance_id
+        # 核销动作
+        # open_screen（设备开屏）
+        self.xr_verification_operate = xr_verification_operate
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.xr_ticket_code, 'xr_ticket_code')
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.instance_id, 'instance_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.xr_ticket_code is not None:
+            result['xr_ticket_code'] = self.xr_ticket_code
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.instance_id is not None:
+            result['instance_id'] = self.instance_id
+        if self.xr_verification_operate is not None:
+            result['xr_verification_operate'] = self.xr_verification_operate
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('xr_ticket_code') is not None:
+            self.xr_ticket_code = m.get('xr_ticket_code')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('instance_id') is not None:
+            self.instance_id = m.get('instance_id')
+        if m.get('xr_verification_operate') is not None:
+            self.xr_verification_operate = m.get('xr_verification_operate')
+        return self
+
+
+class OperateXrUserticketResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class ListXrResourceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        xr_verification_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 核销资源类型
+        self.xr_verification_type = xr_verification_type
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        return self
+
+
+class ListXrResourceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        resource_list: List[CodeListView] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 资源列表
+        self.resource_list = resource_list
+
+    def validate(self):
+        if self.resource_list:
+            for k in self.resource_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        result['resource_list'] = []
+        if self.resource_list is not None:
+            for k in self.resource_list:
+                result['resource_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        self.resource_list = []
+        if m.get('resource_list') is not None:
+            for k in m.get('resource_list'):
+                temp_model = CodeListView()
+                self.resource_list.append(temp_model.from_map(k))
+        return self
+
+
+class PagequeryXrXrverificationmodelRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        resource_id: str = None,
+        resource_name: str = None,
+        instance_name: str = None,
+        instance_id: str = None,
+        current: int = None,
+        page_size: int = None,
+        biz_scene: str = None,
+        type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 唯一ID，对应线下场code
+        self.resource_id = resource_id
+        # 唯一ID，对应线下场名称
+        self.resource_name = resource_name
+        # 设备sn
+        self.instance_name = instance_name
+        # 设备did
+        self.instance_id = instance_id
+        # 当前页
+        self.current = current
+        # 每页大小
+        self.page_size = page_size
+        # 业务类型
+        self.biz_scene = biz_scene
+        # 核销类型
+        self.type = type
+
+    def validate(self):
+        self.validate_required(self.current, 'current')
+        self.validate_required(self.page_size, 'page_size')
+        self.validate_required(self.biz_scene, 'biz_scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.resource_name is not None:
+            result['resource_name'] = self.resource_name
+        if self.instance_name is not None:
+            result['instance_name'] = self.instance_name
+        if self.instance_id is not None:
+            result['instance_id'] = self.instance_id
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('resource_name') is not None:
+            self.resource_name = m.get('resource_name')
+        if m.get('instance_name') is not None:
+            self.instance_name = m.get('instance_name')
+        if m.get('instance_id') is not None:
+            self.instance_id = m.get('instance_id')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class PagequeryXrXrverificationmodelResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        xr_verification_model_list: List[XrVerificationModelVo] = None,
+        current: int = None,
+        page_size: int = None,
+        total: int = None,
+        total_page: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 核销实例列表
+        self.xr_verification_model_list = xr_verification_model_list
+        # 当前页
+        self.current = current
+        # 每页数据量
+        self.page_size = page_size
+        # 数据总条数
+        self.total = total
+        # 总页数
+        self.total_page = total_page
+
+    def validate(self):
+        if self.xr_verification_model_list:
+            for k in self.xr_verification_model_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        result['xr_verification_model_list'] = []
+        if self.xr_verification_model_list is not None:
+            for k in self.xr_verification_model_list:
+                result['xr_verification_model_list'].append(k.to_map() if k else None)
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        if self.total_page is not None:
+            result['total_page'] = self.total_page
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        self.xr_verification_model_list = []
+        if m.get('xr_verification_model_list') is not None:
+            for k in m.get('xr_verification_model_list'):
+                temp_model = XrVerificationModelVo()
+                self.xr_verification_model_list.append(temp_model.from_map(k))
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('total_page') is not None:
+            self.total_page = m.get('total_page')
+        return self
+
+
+class PagequeryXrCustomerdeviceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        device_sn: str = None,
+        service_status: str = None,
+        device_status: str = None,
+        device_type: str = None,
+        current: int = None,
+        page_size: int = None,
+        biz_scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 设备sn
+        self.device_sn = device_sn
+        # 服务状态
+        self.service_status = service_status
+        # 设备状态
+        self.device_status = device_status
+        # 设备品类-型号-规格
+        self.device_type = device_type
+        # 当前页
+        self.current = current
+        # 每页数据
+        self.page_size = page_size
+        # 业务类型
+        self.biz_scene = biz_scene
+
+    def validate(self):
+        self.validate_required(self.current, 'current')
+        self.validate_required(self.page_size, 'page_size')
+        self.validate_required(self.biz_scene, 'biz_scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.device_sn is not None:
+            result['device_sn'] = self.device_sn
+        if self.service_status is not None:
+            result['service_status'] = self.service_status
+        if self.device_status is not None:
+            result['device_status'] = self.device_status
+        if self.device_type is not None:
+            result['device_type'] = self.device_type
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('device_sn') is not None:
+            self.device_sn = m.get('device_sn')
+        if m.get('service_status') is not None:
+            self.service_status = m.get('service_status')
+        if m.get('device_status') is not None:
+            self.device_status = m.get('device_status')
+        if m.get('device_type') is not None:
+            self.device_type = m.get('device_type')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        return self
+
+
+class PagequeryXrCustomerdeviceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        current: int = None,
+        customer_device_list: List[CustomerDeviceItem] = None,
+        page_size: int = None,
+        total: int = None,
+        total_page: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 当前页
+        self.current = current
+        # 客户对应设备列表
+        self.customer_device_list = customer_device_list
+        # 每页数据
+        self.page_size = page_size
+        # 数据总条数
+        self.total = total
+        # 总页数
+        self.total_page = total_page
+
+    def validate(self):
+        if self.customer_device_list:
+            for k in self.customer_device_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.current is not None:
+            result['current'] = self.current
+        result['customer_device_list'] = []
+        if self.customer_device_list is not None:
+            for k in self.customer_device_list:
+                result['customer_device_list'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        if self.total_page is not None:
+            result['total_page'] = self.total_page
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        self.customer_device_list = []
+        if m.get('customer_device_list') is not None:
+            for k in m.get('customer_device_list'):
+                temp_model = CustomerDeviceItem()
+                self.customer_device_list.append(temp_model.from_map(k))
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('total_page') is not None:
+            self.total_page = m.get('total_page')
+        return self
+
+
+class CreateXrXrticketpoolRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        resource_id: str = None,
+        valid_time: str = None,
+        test_time: int = None,
+        xr_apps: str = None,
+        max_pool_count: int = None,
+        xr_ticket_pool_name: str = None,
+        xr_verification_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务类型
+        self.biz_scene = biz_scene
+        # 资源id
+        self.resource_id = resource_id
+        # 有效期
+        self.valid_time = valid_time
+        # 体验时长
+        self.test_time = test_time
+        # vr设备集合
+        self.xr_apps = xr_apps
+        # 券池数量，能发多少张券
+        self.max_pool_count = max_pool_count
+        # 券池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.valid_time, 'valid_time')
+        self.validate_required(self.test_time, 'test_time')
+        self.validate_required(self.max_pool_count, 'max_pool_count')
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.test_time is not None:
+            result['test_time'] = self.test_time
+        if self.xr_apps is not None:
+            result['xr_apps'] = self.xr_apps
+        if self.max_pool_count is not None:
+            result['max_pool_count'] = self.max_pool_count
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('test_time') is not None:
+            self.test_time = m.get('test_time')
+        if m.get('xr_apps') is not None:
+            self.xr_apps = m.get('xr_apps')
+        if m.get('max_pool_count') is not None:
+            self.max_pool_count = m.get('max_pool_count')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        return self
+
+
+class CreateXrXrticketpoolResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class UpdateXrXrticketpoolRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        xr_ticket_pool_name: str = None,
+        resource_id: str = None,
+        valid_time: str = None,
+        test_time: int = None,
+        xr_apps: str = None,
+        surplus_count: int = None,
+        xr_verification_type: str = None,
+        biz_scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 券池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 资源id
+        self.resource_id = resource_id
+        # 通行证有效期
+        self.valid_time = valid_time
+        # 体验时长
+        self.test_time = test_time
+        # vr设备集合
+        self.xr_apps = xr_apps
+        # 券池剩余数量
+        self.surplus_count = surplus_count
+        # 核销类型，资源id改变时必须有值
+        self.xr_verification_type = xr_verification_type
+        # 业务类型
+        self.biz_scene = biz_scene
+
+    def validate(self):
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+        self.validate_required(self.biz_scene, 'biz_scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.valid_time is not None:
+            result['valid_time'] = self.valid_time
+        if self.test_time is not None:
+            result['test_time'] = self.test_time
+        if self.xr_apps is not None:
+            result['xr_apps'] = self.xr_apps
+        if self.surplus_count is not None:
+            result['surplus_count'] = self.surplus_count
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('valid_time') is not None:
+            self.valid_time = m.get('valid_time')
+        if m.get('test_time') is not None:
+            self.test_time = m.get('test_time')
+        if m.get('xr_apps') is not None:
+            self.xr_apps = m.get('xr_apps')
+        if m.get('surplus_count') is not None:
+            self.surplus_count = m.get('surplus_count')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        return self
+
+
+class UpdateXrXrticketpoolResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class PagequeryXrXrticketpoolRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        resource_id: str = None,
+        xr_ticket_pool_name: str = None,
+        status: str = None,
+        current: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务类型
+        self.biz_scene = biz_scene
+        # 资源id
+        self.resource_id = resource_id
+        # 券池名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+        # 通行证状态，
+        # EXPIRED：已过期
+        # VALID：有效
+        # SALED：已出售
+        self.status = status
+        # 当前页
+        # 
+        self.current = current
+        # 每页大小
+        self.page_size = page_size
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.current, 'current')
+        self.validate_required(self.page_size, 'page_size')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        if self.status is not None:
+            result['status'] = self.status
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class PagequeryXrXrticketpoolResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        xr_ticket_pool_list: List[XrTicketPoolItem] = None,
+        success: bool = None,
+        current: int = None,
+        page_size: int = None,
+        total: int = None,
+        total_page: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 通行证列表
+        self.xr_ticket_pool_list = xr_ticket_pool_list
+        # 是否成功
+        self.success = success
+        # 当前页
+        self.current = current
+        # 每页数据条数
+        self.page_size = page_size
+        # 总数量
+        self.total = total
+        # 总页数
+        self.total_page = total_page
+
+    def validate(self):
+        if self.xr_ticket_pool_list:
+            for k in self.xr_ticket_pool_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['xr_ticket_pool_list'] = []
+        if self.xr_ticket_pool_list is not None:
+            for k in self.xr_ticket_pool_list:
+                result['xr_ticket_pool_list'].append(k.to_map() if k else None)
+        if self.success is not None:
+            result['success'] = self.success
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        if self.total_page is not None:
+            result['total_page'] = self.total_page
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.xr_ticket_pool_list = []
+        if m.get('xr_ticket_pool_list') is not None:
+            for k in m.get('xr_ticket_pool_list'):
+                temp_model = XrTicketPoolItem()
+                self.xr_ticket_pool_list.append(temp_model.from_map(k))
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('total_page') is not None:
+            self.total_page = m.get('total_page')
+        return self
+
+
+class SyncDeviceScreenstatusRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        device_did: str = None,
+        device_screen_status: str = None,
+        tenant_id: str = None,
+        status_change_time: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 所属业务
+        self.biz_scene = biz_scene
+        # 设备did
+        self.device_did = device_did
+        # 设备屏幕状态
+        self.device_screen_status = device_screen_status
+        # 租户id
+        self.tenant_id = tenant_id
+        # 状态改变时间
+        self.status_change_time = status_change_time
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.device_did, 'device_did')
+        self.validate_required(self.device_screen_status, 'device_screen_status')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.status_change_time, 'status_change_time')
+        if self.status_change_time is not None:
+            self.validate_pattern(self.status_change_time, 'status_change_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.device_did is not None:
+            result['device_did'] = self.device_did
+        if self.device_screen_status is not None:
+            result['device_screen_status'] = self.device_screen_status
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.status_change_time is not None:
+            result['status_change_time'] = self.status_change_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('device_did') is not None:
+            self.device_did = m.get('device_did')
+        if m.get('device_screen_status') is not None:
+            self.device_screen_status = m.get('device_screen_status')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('status_change_time') is not None:
+            self.status_change_time = m.get('status_change_time')
+        return self
+
+
+class SyncDeviceScreenstatusResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class BatchcreateXrXrticketpoolRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        xr_ticket_pool_reqs: List[XrTicketPoolBatchReq] = None,
+        biz_scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # xr通行证批量创建请求列表
+        self.xr_ticket_pool_reqs = xr_ticket_pool_reqs
+        # 业务类型
+        self.biz_scene = biz_scene
+
+    def validate(self):
+        self.validate_required(self.xr_ticket_pool_reqs, 'xr_ticket_pool_reqs')
+        if self.xr_ticket_pool_reqs:
+            for k in self.xr_ticket_pool_reqs:
+                if k:
+                    k.validate()
+        self.validate_required(self.biz_scene, 'biz_scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        result['xr_ticket_pool_reqs'] = []
+        if self.xr_ticket_pool_reqs is not None:
+            for k in self.xr_ticket_pool_reqs:
+                result['xr_ticket_pool_reqs'].append(k.to_map() if k else None)
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        self.xr_ticket_pool_reqs = []
+        if m.get('xr_ticket_pool_reqs') is not None:
+            for k in m.get('xr_ticket_pool_reqs'):
+                temp_model = XrTicketPoolBatchReq()
+                self.xr_ticket_pool_reqs.append(temp_model.from_map(k))
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        return self
+
+
+class BatchcreateXrXrticketpoolResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        success_list: List[XrTicketPoolSuccessList] = None,
+        fail_list: List[XrTicketPoolFailList] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # xr通行证创建成功列表
+        self.success_list = success_list
+        # xr通行证创建失败列表
+        self.fail_list = fail_list
+
+    def validate(self):
+        if self.success_list:
+            for k in self.success_list:
+                if k:
+                    k.validate()
+        if self.fail_list:
+            for k in self.fail_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        result['success_list'] = []
+        if self.success_list is not None:
+            for k in self.success_list:
+                result['success_list'].append(k.to_map() if k else None)
+        result['fail_list'] = []
+        if self.fail_list is not None:
+            for k in self.fail_list:
+                result['fail_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        self.success_list = []
+        if m.get('success_list') is not None:
+            for k in m.get('success_list'):
+                temp_model = XrTicketPoolSuccessList()
+                self.success_list.append(temp_model.from_map(k))
+        self.fail_list = []
+        if m.get('fail_list') is not None:
+            for k in m.get('fail_list'):
+                temp_model = XrTicketPoolFailList()
+                self.fail_list.append(temp_model.from_map(k))
+        return self
+
+
+class ListXrXrverificationmodelinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        resource_id: str = None,
+        xr_verification_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务类型
+        self.biz_scene = biz_scene
+        # 资源id
+        self.resource_id = resource_id
+        # 核销类型
+        self.xr_verification_type = xr_verification_type
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.xr_verification_type, 'xr_verification_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.xr_verification_type is not None:
+            result['xr_verification_type'] = self.xr_verification_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('xr_verification_type') is not None:
+            self.xr_verification_type = m.get('xr_verification_type')
+        return self
+
+
+class ListXrXrverificationmodelinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        instance_info_list: List[InstanceInfo] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 实例信息列表
+        self.instance_info_list = instance_info_list
+
+    def validate(self):
+        if self.instance_info_list:
+            for k in self.instance_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        result['instance_info_list'] = []
+        if self.instance_info_list is not None:
+            for k in self.instance_info_list:
+                result['instance_info_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        self.instance_info_list = []
+        if m.get('instance_info_list') is not None:
+            for k in m.get('instance_info_list'):
+                temp_model = InstanceInfo()
+                self.instance_info_list.append(temp_model.from_map(k))
+        return self
+
+
+class DetailXrXrticketpoolRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_scene: str = None,
+        xr_ticket_pool_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务类型
+        self.biz_scene = biz_scene
+        # 券名称
+        self.xr_ticket_pool_name = xr_ticket_pool_name
+
+    def validate(self):
+        self.validate_required(self.biz_scene, 'biz_scene')
+        self.validate_required(self.xr_ticket_pool_name, 'xr_ticket_pool_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        if self.xr_ticket_pool_name is not None:
+            result['xr_ticket_pool_name'] = self.xr_ticket_pool_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        if m.get('xr_ticket_pool_name') is not None:
+            self.xr_ticket_pool_name = m.get('xr_ticket_pool_name')
+        return self
+
+
+class DetailXrXrticketpoolResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        xr_ticket_pool_detail: XrTicketPoolItem = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 通行证对象
+        self.xr_ticket_pool_detail = xr_ticket_pool_detail
+
+    def validate(self):
+        if self.xr_ticket_pool_detail:
+            self.xr_ticket_pool_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.xr_ticket_pool_detail is not None:
+            result['xr_ticket_pool_detail'] = self.xr_ticket_pool_detail.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('xr_ticket_pool_detail') is not None:
+            temp_model = XrTicketPoolItem()
+            self.xr_ticket_pool_detail = temp_model.from_map(m['xr_ticket_pool_detail'])
+        return self
+
+
+class OperateAiotnextbsOpenapiRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        operate_type: str = None,
+        param_sign: str = None,
+        biz_type: str = None,
+        operator_id: str = None,
+        interface_name: str = None,
+        method_name: str = None,
+        param_class: str = None,
+        param_list: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 操作类型
+        self.operate_type = operate_type
+        # 参数签名
+        self.param_sign = param_sign
+        # 业务操作类型
+        self.biz_type = biz_type
+        # 操作人id
+        self.operator_id = operator_id
+        # 类名（实现类），首字母小写
+        self.interface_name = interface_name
+        # 方法名
+        self.method_name = method_name
+        # 参数类路径
+        self.param_class = param_class
+        # 参数数据
+        self.param_list = param_list
+
+    def validate(self):
+        self.validate_required(self.operate_type, 'operate_type')
+        self.validate_required(self.param_sign, 'param_sign')
+        self.validate_required(self.biz_type, 'biz_type')
+        self.validate_required(self.operator_id, 'operator_id')
+        self.validate_required(self.interface_name, 'interface_name')
+        self.validate_required(self.method_name, 'method_name')
+        self.validate_required(self.param_class, 'param_class')
+        self.validate_required(self.param_list, 'param_list')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.operate_type is not None:
+            result['operate_type'] = self.operate_type
+        if self.param_sign is not None:
+            result['param_sign'] = self.param_sign
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
+        if self.operator_id is not None:
+            result['operator_id'] = self.operator_id
+        if self.interface_name is not None:
+            result['interface_name'] = self.interface_name
+        if self.method_name is not None:
+            result['method_name'] = self.method_name
+        if self.param_class is not None:
+            result['param_class'] = self.param_class
+        if self.param_list is not None:
+            result['param_list'] = self.param_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('operate_type') is not None:
+            self.operate_type = m.get('operate_type')
+        if m.get('param_sign') is not None:
+            self.param_sign = m.get('param_sign')
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        if m.get('operator_id') is not None:
+            self.operator_id = m.get('operator_id')
+        if m.get('interface_name') is not None:
+            self.interface_name = m.get('interface_name')
+        if m.get('method_name') is not None:
+            self.method_name = m.get('method_name')
+        if m.get('param_class') is not None:
+            self.param_class = m.get('param_class')
+        if m.get('param_list') is not None:
+            self.param_list = m.get('param_list')
+        return self
+
+
+class OperateAiotnextbsOpenapiResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        result: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 操作是否成功
+        self.success = success
+        # 结果数据
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
 class FinishTraceConfigRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         success: bool = None,
         privated_tenant: str = None,
@@ -11458,29 +15015,33 @@
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         device_did: str = None,
         device_status: str = None,
         device_signature: str = None,
+        biz_status_info: BizStatusInfoOp = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 设备did
         self.device_did = device_did
         # 设备状态
         self.device_status = device_status
         # 设备签名
         self.device_signature = device_signature
+        # 业务状态
+        self.biz_status_info = biz_status_info
 
     def validate(self):
         self.validate_required(self.device_did, 'device_did')
-        self.validate_required(self.device_status, 'device_status')
         self.validate_required(self.device_signature, 'device_signature')
+        if self.biz_status_info:
+            self.biz_status_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -11490,28 +15051,33 @@
             result['product_instance_id'] = self.product_instance_id
         if self.device_did is not None:
             result['device_did'] = self.device_did
         if self.device_status is not None:
             result['device_status'] = self.device_status
         if self.device_signature is not None:
             result['device_signature'] = self.device_signature
+        if self.biz_status_info is not None:
+            result['biz_status_info'] = self.biz_status_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('device_did') is not None:
             self.device_did = m.get('device_did')
         if m.get('device_status') is not None:
             self.device_status = m.get('device_status')
         if m.get('device_signature') is not None:
             self.device_signature = m.get('device_signature')
+        if m.get('biz_status_info') is not None:
+            temp_model = BizStatusInfoOp()
+            self.biz_status_info = temp_model.from_map(m['biz_status_info'])
         return self
 
 
 class SyncIotbasicDevicestatusResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -13415,15 +16981,14 @@
 
     def validate(self):
         if self.device_operate_infos:
             for k in self.device_operate_infos:
                 if k:
                     k.validate()
         self.validate_required(self.device_operation, 'device_operation')
-        self.validate_required(self.user_id, 'user_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -15348,29 +18913,26 @@
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         data_model: str = None,
         data_model_name: str = None,
         biz_type: str = None,
         customer_version: str = None,
-        transform_thing_model: bool = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 数据模型
         self.data_model = data_model
         # 数据模型名称
         self.data_model_name = data_model_name
         # 数据模型类别
         self.biz_type = biz_type
         # 用户自定义版本
         self.customer_version = customer_version
-        # 是否转化为物模型，默认false
-        self.transform_thing_model = transform_thing_model
 
     def validate(self):
         self.validate_required(self.data_model, 'data_model')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -15385,16 +18947,14 @@
             result['data_model'] = self.data_model
         if self.data_model_name is not None:
             result['data_model_name'] = self.data_model_name
         if self.biz_type is not None:
             result['biz_type'] = self.biz_type
         if self.customer_version is not None:
             result['customer_version'] = self.customer_version
-        if self.transform_thing_model is not None:
-            result['transform_thing_model'] = self.transform_thing_model
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -15403,16 +18963,14 @@
             self.data_model = m.get('data_model')
         if m.get('data_model_name') is not None:
             self.data_model_name = m.get('data_model_name')
         if m.get('biz_type') is not None:
             self.biz_type = m.get('biz_type')
         if m.get('customer_version') is not None:
             self.customer_version = m.get('customer_version')
-        if m.get('transform_thing_model') is not None:
-            self.transform_thing_model = m.get('transform_thing_model')
         return self
 
 
 class CreateDeviceDatamodelResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -18691,14 +22249,15 @@
         device_type_code: int = None,
         initial_price: int = None,
         factory_time: str = None,
         release_time: str = None,
         device_name: str = None,
         owner: str = None,
         owner_name: str = None,
+        extra_info: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 设备Id
         # 
         self.device_id = device_id
@@ -18764,14 +22323,16 @@
         self.release_time = release_time
         # 设备型号
         self.device_name = device_name
         # 资产所有人标识（统一社会信用代码）
         self.owner = owner
         # 资产所有人名称
         self.owner_name = owner_name
+        # 额外信息
+        self.extra_info = extra_info
 
     def validate(self):
         self.validate_required(self.device_id, 'device_id')
         self.validate_required(self.data_model_id, 'data_model_id')
         self.validate_required(self.scene, 'scene')
         self.validate_required(self.content, 'content')
         self.validate_required(self.signature, 'signature')
@@ -18813,14 +22374,16 @@
             result['release_time'] = self.release_time
         if self.device_name is not None:
             result['device_name'] = self.device_name
         if self.owner is not None:
             result['owner'] = self.owner
         if self.owner_name is not None:
             result['owner_name'] = self.owner_name
+        if self.extra_info is not None:
+            result['extra_info'] = self.extra_info
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -18847,14 +22410,16 @@
             self.release_time = m.get('release_time')
         if m.get('device_name') is not None:
             self.device_name = m.get('device_name')
         if m.get('owner') is not None:
             self.owner = m.get('owner')
         if m.get('owner_name') is not None:
             self.owner_name = m.get('owner_name')
+        if m.get('extra_info') is not None:
+            self.extra_info = m.get('extra_info')
         return self
 
 
 class CreateDistributedeviceBydeviceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -25046,14 +28611,864 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('thing_model') is not None:
             self.thing_model = m.get('thing_model')
         return self
 
 
+class CreateDistributedeviceBydevicemulRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        scene: str = None,
+        device_param_list: List[RegByDeviceParm] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 场景码，由蚂蚁侧定义
+        self.scene = scene
+        # 设备注册信息集合, 数组长度不超过50
+        self.device_param_list = device_param_list
+
+    def validate(self):
+        self.validate_required(self.scene, 'scene')
+        self.validate_required(self.device_param_list, 'device_param_list')
+        if self.device_param_list:
+            for k in self.device_param_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.scene is not None:
+            result['scene'] = self.scene
+        result['device_param_list'] = []
+        if self.device_param_list is not None:
+            for k in self.device_param_list:
+                result['device_param_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        self.device_param_list = []
+        if m.get('device_param_list') is not None:
+            for k in m.get('device_param_list'):
+                temp_model = RegByDeviceParm()
+                self.device_param_list.append(temp_model.from_map(k))
+        return self
+
+
+class CreateDistributedeviceBydevicemulResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        trustiot_device_id_list: List[TrustiotDeviceIdMap] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 可信设备ID集合
+        self.trustiot_device_id_list = trustiot_device_id_list
+
+    def validate(self):
+        if self.trustiot_device_id_list:
+            for k in self.trustiot_device_id_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['trustiot_device_id_list'] = []
+        if self.trustiot_device_id_list is not None:
+            for k in self.trustiot_device_id_list:
+                result['trustiot_device_id_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.trustiot_device_id_list = []
+        if m.get('trustiot_device_id_list') is not None:
+            for k in m.get('trustiot_device_id_list'):
+                temp_model = TrustiotDeviceIdMap()
+                self.trustiot_device_id_list.append(temp_model.from_map(k))
+        return self
+
+
+class CreateDistributedeviceBydeviceidmulRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        scene: str = None,
+        device_param_list: List[RegByDeviceIdParm] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 场景码
+        self.scene = scene
+        # 设备注册信息集合
+        self.device_param_list = device_param_list
+
+    def validate(self):
+        self.validate_required(self.scene, 'scene')
+        self.validate_required(self.device_param_list, 'device_param_list')
+        if self.device_param_list:
+            for k in self.device_param_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.scene is not None:
+            result['scene'] = self.scene
+        result['device_param_list'] = []
+        if self.device_param_list is not None:
+            for k in self.device_param_list:
+                result['device_param_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        self.device_param_list = []
+        if m.get('device_param_list') is not None:
+            for k in m.get('device_param_list'):
+                temp_model = RegByDeviceIdParm()
+                self.device_param_list.append(temp_model.from_map(k))
+        return self
+
+
+class CreateDistributedeviceBydeviceidmulResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        trustiot_device_id_list: List[TrustiotDeviceIdMap] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 可信设备ID集合
+        # 
+        self.trustiot_device_id_list = trustiot_device_id_list
+
+    def validate(self):
+        if self.trustiot_device_id_list:
+            for k in self.trustiot_device_id_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['trustiot_device_id_list'] = []
+        if self.trustiot_device_id_list is not None:
+            for k in self.trustiot_device_id_list:
+                result['trustiot_device_id_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.trustiot_device_id_list = []
+        if m.get('trustiot_device_id_list') is not None:
+            for k in m.get('trustiot_device_id_list'):
+                temp_model = TrustiotDeviceIdMap()
+                self.trustiot_device_id_list.append(temp_model.from_map(k))
+        return self
+
+
+class BindEntityrelationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        subject_scene: str = None,
+        subject_entity_id: str = None,
+        subject_trustiot_id: int = None,
+        predicate: str = None,
+        object_entity_type: str = None,
+        object_scene: str = None,
+        object_entity_id: str = None,
+        object_trustiot_id: int = None,
+        upsert: bool = None,
+        remark: str = None,
+        custom_entity_info: CustomEntityInfo = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # [主]实体场景码
+        self.subject_scene = subject_scene
+        # [主]实体ID（当[主]实体平台唯一ID（subject_trustiot_id）为空时，此项不能为空）
+        self.subject_entity_id = subject_entity_id
+        # [主]实体平台唯一ID（当[主]实体ID（subject_entity_id）为空时，此项不能为空）
+        self.subject_trustiot_id = subject_trustiot_id
+        # 关系谓语, 取值范围：SUB_DEVICE、USER、LOCATION
+        self.predicate = predicate
+        # [宾]实体类型，取值范围：DEVICE、PERIPHERAL、LABEL、CUSTOMER_ENTITY
+        self.object_entity_type = object_entity_type
+        # [宾]场景码（当[宾]实体唯一ID为空时，此项必填）
+        self.object_scene = object_scene
+        # [宾]实体ID（当[宾]实体唯一ID为空时，此项必填）
+        self.object_entity_id = object_entity_id
+        # [宾]平台唯一ID，与[宾]实体场景码+[宾]实体ID（object_scene+object_entity_id）不能同时为空
+        self.object_trustiot_id = object_trustiot_id
+        # 绑定请求中，主语或宾语有历史关系，是否删除历史，写入新关系
+        # (只处理1对1关系，即生效的前提是{RelationProperty}的maxObjectCount=1 & maxSubjectCount=1)
+        self.upsert = upsert
+        # 备注
+        self.remark = remark
+        # 自定义实体信息（如果object_entity_type=CUSTOMER_ENTITY，则custom_entity_info必填）
+        self.custom_entity_info = custom_entity_info
+
+    def validate(self):
+        self.validate_required(self.subject_scene, 'subject_scene')
+        self.validate_required(self.predicate, 'predicate')
+        self.validate_required(self.object_entity_type, 'object_entity_type')
+        self.validate_required(self.upsert, 'upsert')
+        if self.custom_entity_info:
+            self.custom_entity_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.subject_scene is not None:
+            result['subject_scene'] = self.subject_scene
+        if self.subject_entity_id is not None:
+            result['subject_entity_id'] = self.subject_entity_id
+        if self.subject_trustiot_id is not None:
+            result['subject_trustiot_id'] = self.subject_trustiot_id
+        if self.predicate is not None:
+            result['predicate'] = self.predicate
+        if self.object_entity_type is not None:
+            result['object_entity_type'] = self.object_entity_type
+        if self.object_scene is not None:
+            result['object_scene'] = self.object_scene
+        if self.object_entity_id is not None:
+            result['object_entity_id'] = self.object_entity_id
+        if self.object_trustiot_id is not None:
+            result['object_trustiot_id'] = self.object_trustiot_id
+        if self.upsert is not None:
+            result['upsert'] = self.upsert
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.custom_entity_info is not None:
+            result['custom_entity_info'] = self.custom_entity_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('subject_scene') is not None:
+            self.subject_scene = m.get('subject_scene')
+        if m.get('subject_entity_id') is not None:
+            self.subject_entity_id = m.get('subject_entity_id')
+        if m.get('subject_trustiot_id') is not None:
+            self.subject_trustiot_id = m.get('subject_trustiot_id')
+        if m.get('predicate') is not None:
+            self.predicate = m.get('predicate')
+        if m.get('object_entity_type') is not None:
+            self.object_entity_type = m.get('object_entity_type')
+        if m.get('object_scene') is not None:
+            self.object_scene = m.get('object_scene')
+        if m.get('object_entity_id') is not None:
+            self.object_entity_id = m.get('object_entity_id')
+        if m.get('object_trustiot_id') is not None:
+            self.object_trustiot_id = m.get('object_trustiot_id')
+        if m.get('upsert') is not None:
+            self.upsert = m.get('upsert')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('custom_entity_info') is not None:
+            temp_model = CustomEntityInfo()
+            self.custom_entity_info = temp_model.from_map(m['custom_entity_info'])
+        return self
+
+
+class BindEntityrelationResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class UnbindEntityrelationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        subject_scene: str = None,
+        subject_entity_id: str = None,
+        subject_trustiot_id: int = None,
+        predicate: str = None,
+        object_entity_type: str = None,
+        object_scene: str = None,
+        object_entity_id_list: List[str] = None,
+        object_trustiotiot_id_list: List[int] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # [主]实体场景码
+        self.subject_scene = subject_scene
+        # [主]实体ID（当[主]实体平台唯一ID（subject_trustiot_id）为空时，此项不能为空）
+        self.subject_entity_id = subject_entity_id
+        # [主]实体平台唯一ID（当[主]实体ID（subject_entity_id）为空时，此项不能为空）
+        self.subject_trustiot_id = subject_trustiot_id
+        # 关系谓语, 取值范围：SUB_DEVICE、USER、LOCATION
+        self.predicate = predicate
+        # [宾]实体类型，取值范围：DEVICE、PERIPHERAL、LABEL、CUSTOMER_ENTITY
+        self.object_entity_type = object_entity_type
+        # [宾]场景码（当[宾]实体唯一ID列表(object_trustiotiot_id_list)为空时，此项必填）
+        self.object_scene = object_scene
+        # [宾]实体ID列表（当[宾]实体唯一ID列表(object_trustiotiot_id_list)为空时，此项必填）
+        # 
+        self.object_entity_id_list = object_entity_id_list
+        # [宾]实体唯一ID列表,与[宾]实体场景码+[宾]实体ID列表（object_scene+object_entity_id）不能同时为空
+        self.object_trustiotiot_id_list = object_trustiotiot_id_list
+
+    def validate(self):
+        self.validate_required(self.subject_scene, 'subject_scene')
+        self.validate_required(self.predicate, 'predicate')
+        self.validate_required(self.object_entity_type, 'object_entity_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.subject_scene is not None:
+            result['subject_scene'] = self.subject_scene
+        if self.subject_entity_id is not None:
+            result['subject_entity_id'] = self.subject_entity_id
+        if self.subject_trustiot_id is not None:
+            result['subject_trustiot_id'] = self.subject_trustiot_id
+        if self.predicate is not None:
+            result['predicate'] = self.predicate
+        if self.object_entity_type is not None:
+            result['object_entity_type'] = self.object_entity_type
+        if self.object_scene is not None:
+            result['object_scene'] = self.object_scene
+        if self.object_entity_id_list is not None:
+            result['object_entity_id_list'] = self.object_entity_id_list
+        if self.object_trustiotiot_id_list is not None:
+            result['object_trustiotiot_id_list'] = self.object_trustiotiot_id_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('subject_scene') is not None:
+            self.subject_scene = m.get('subject_scene')
+        if m.get('subject_entity_id') is not None:
+            self.subject_entity_id = m.get('subject_entity_id')
+        if m.get('subject_trustiot_id') is not None:
+            self.subject_trustiot_id = m.get('subject_trustiot_id')
+        if m.get('predicate') is not None:
+            self.predicate = m.get('predicate')
+        if m.get('object_entity_type') is not None:
+            self.object_entity_type = m.get('object_entity_type')
+        if m.get('object_scene') is not None:
+            self.object_scene = m.get('object_scene')
+        if m.get('object_entity_id_list') is not None:
+            self.object_entity_id_list = m.get('object_entity_id_list')
+        if m.get('object_trustiotiot_id_list') is not None:
+            self.object_trustiotiot_id_list = m.get('object_trustiotiot_id_list')
+        return self
+
+
+class UnbindEntityrelationResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class DetailThingmodelDeviceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        scene: str = None,
+        device_id: str = None,
+        device_imei: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 场景码
+        self.scene = scene
+        # 设备ID（当device_imei号为空时，会根据scene+device_id查询设备记录，获取device_imei）
+        self.device_id = device_id
+        # 设备imei号
+        self.device_imei = device_imei
+
+    def validate(self):
+        self.validate_required(self.scene, 'scene')
+        self.validate_required(self.device_id, 'device_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        if self.device_imei is not None:
+            result['device_imei'] = self.device_imei
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        if m.get('device_imei') is not None:
+            self.device_imei = m.get('device_imei')
+        return self
+
+
+class DetailThingmodelDeviceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        status: str = None,
+        status_available: bool = None,
+        sdk_version: str = None,
+        sdk_version_available: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 设备状态
+        self.status = status
+        # 设备状态是否可用
+        self.status_available = status_available
+        # SDK版本号
+        self.sdk_version = sdk_version
+        # SDK版本号是否可用
+        self.sdk_version_available = sdk_version_available
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.status is not None:
+            result['status'] = self.status
+        if self.status_available is not None:
+            result['status_available'] = self.status_available
+        if self.sdk_version is not None:
+            result['sdk_version'] = self.sdk_version
+        if self.sdk_version_available is not None:
+            result['sdk_version_available'] = self.sdk_version_available
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('status_available') is not None:
+            self.status_available = m.get('status_available')
+        if m.get('sdk_version') is not None:
+            self.sdk_version = m.get('sdk_version')
+        if m.get('sdk_version_available') is not None:
+            self.sdk_version_available = m.get('sdk_version_available')
+        return self
+
+
+class CreateCollectorUploadfileurlRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        scene: str = None,
+        data_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 场景码
+        self.scene = scene
+        # 待上传文件的业务类型，
+        # 设备心跳数据：COLLECT_MUL
+        # 设备业务数据： COLLECT_DEVICE_BIZ_DATA
+        self.data_type = data_type
+
+    def validate(self):
+        self.validate_required(self.scene, 'scene')
+        self.validate_required(self.data_type, 'data_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        return self
+
+
+class CreateCollectorUploadfileurlResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        upload_file_url: str = None,
+        upload_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 可以上传文件的预签名URL
+        self.upload_file_url = upload_file_url
+        # 上传任务唯一ID，后续流程中会用到
+        self.upload_id = upload_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.upload_file_url is not None:
+            result['upload_file_url'] = self.upload_file_url
+        if self.upload_id is not None:
+            result['upload_id'] = self.upload_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('upload_file_url') is not None:
+            self.upload_file_url = m.get('upload_file_url')
+        if m.get('upload_id') is not None:
+            self.upload_id = m.get('upload_id')
+        return self
+
+
+class ConfirmCollectorUploadfileRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        upload_id: str = None,
+        total: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 上报文件任务ID，blockchain.bot.collector.uploadfileurl.create接口中获取
+        self.upload_id = upload_id
+        # 上报数据的总数，用于和CSV文件中的数据进行核验
+        self.total = total
+
+    def validate(self):
+        self.validate_required(self.upload_id, 'upload_id')
+        self.validate_required(self.total, 'total')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.upload_id is not None:
+            result['upload_id'] = self.upload_id
+        if self.total is not None:
+            result['total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('upload_id') is not None:
+            self.upload_id = m.get('upload_id')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        return self
+
+
+class ConfirmCollectorUploadfileResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class ExecThingsdidOneapiRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         biz_content: str = None,
     ):
```

### Comparing `antchain_bot-1.8.7/setup.py` & `antchain_bot-1.8.70/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bot.
 
-Created on 28/02/2023
+Created on 17/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bot"
 NAME = "antchain_bot" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BOT SDK Library for Python"
```

