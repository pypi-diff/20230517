# Comparing `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8.tar.gz` & `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8.tar", last modified: Wed May 17 06:41:33 2023, max compression
+gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9.tar", last modified: Wed May 17 07:13:13 2023, max compression
```

## Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8.tar` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32882 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
--rw-r--r--   0 root         (0) root         (0)    28210 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-17 06:41:33.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35252 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
+-rw-r--r--   0 root         (0) root         (0)    31032 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-17 07:13:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/setup.py
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/LICENSE` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/README-CN.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/README.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py`

 * *Files 1% similar despite different names*

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
-                    'sdk_version': '1.0.8',
+                    'sdk_version': '1.0.9',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -495,14 +495,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindDemoAsdAsdAsdResponse(),
             await self.do_request_async('1.0', 'demo.asd.asd.asd.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def reset_demo_com_cn_cc(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcResponse:
+        """
+        Description: 测试api描述
+        Summary: api简介
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.reset_demo_com_cn_cc_ex(request, headers, runtime)
+
+    async def reset_demo_com_cn_cc_async(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcResponse:
+        """
+        Description: 测试api描述
+        Summary: api简介
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.reset_demo_com_cn_cc_ex_async(request, headers, runtime)
+
+    def reset_demo_com_cn_cc_ex(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcResponse:
+        """
+        Description: 测试api描述
+        Summary: api简介
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcResponse(),
+            self.do_request('1.0', 'demo.com.cn.cc.reset', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def reset_demo_com_cn_cc_ex_async(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcResponse:
+        """
+        Description: 测试api描述
+        Summary: api简介
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.ResetDemoComCnCcResponse(),
+            await self.do_request_async('1.0', 'demo.com.cn.cc.reset', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def upload_demo_cjtest_source_file(
         self,
         request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.UploadDemoCjtestSourceFileRequest,
     ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.UploadDemoCjtestSourceFileResponse:
         """
         Description: 文件测试1
         Summary: 文件测试
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,14 +497,104 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class ResetDemoComCnCcRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        order_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # orderid
+        self.order_id = order_id
+
+    def validate(self):
+        self.validate_required(self.order_id, 'order_id')
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
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class ResetDemoComCnCcResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 订单id
+        self.order_id = order_id
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
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
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
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
 class UploadDemoCjtestSourceFileRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         file_object: BinaryIO = None,
         file_object_name: str = None,
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.8/setup.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.9/setup.py`

 * *Files identical despite different names*

