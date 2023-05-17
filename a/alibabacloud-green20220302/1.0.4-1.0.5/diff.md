# Comparing `tmp/alibabacloud_green20220302-1.0.4.tar.gz` & `tmp/alibabacloud_green20220302-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-1.0.4.tar", last modified: Wed Mar 15 06:48:57 2023, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-1.0.5.tar", last modified: Wed May 17 06:05:39 2023, max compression
```

## Comparing `alibabacloud_green20220302-1.0.4.tar` & `alibabacloud_green20220302-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16827 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)    27248 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-15 06:48:57.000000 alibabacloud_green20220302-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2023-03-15 06:48:56.000000 alibabacloud_green20220302-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19695 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)    35554 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:05:39.000000 alibabacloud_green20220302-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-05-17 06:05:38.000000 alibabacloud_green20220302-1.0.5/setup.py
```

### Comparing `alibabacloud_green20220302-1.0.4/LICENSE` & `alibabacloud_green20220302-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.4/PKG-INFO` & `alibabacloud_green20220302-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-1.0.4/README-CN.md` & `alibabacloud_green20220302-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.4/README.md` & `alibabacloud_green20220302-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-1.0.4/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,14 +57,88 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def describe_image_result_ext_with_options(
+        self,
+        request: green_20220302_models.DescribeImageResultExtRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> green_20220302_models.DescribeImageResultExtResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.info_type):
+            body['InfoType'] = request.info_type
+        if not UtilClient.is_unset(request.req_id):
+            body['ReqId'] = request.req_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeImageResultExt',
+            version='2022-03-02',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            green_20220302_models.DescribeImageResultExtResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_image_result_ext_with_options_async(
+        self,
+        request: green_20220302_models.DescribeImageResultExtRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> green_20220302_models.DescribeImageResultExtResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.info_type):
+            body['InfoType'] = request.info_type
+        if not UtilClient.is_unset(request.req_id):
+            body['ReqId'] = request.req_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeImageResultExt',
+            version='2022-03-02',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            green_20220302_models.DescribeImageResultExtResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_image_result_ext(
+        self,
+        request: green_20220302_models.DescribeImageResultExtRequest,
+    ) -> green_20220302_models.DescribeImageResultExtResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_image_result_ext_with_options(request, runtime)
+
+    async def describe_image_result_ext_async(
+        self,
+        request: green_20220302_models.DescribeImageResultExtRequest,
+    ) -> green_20220302_models.DescribeImageResultExtResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_image_result_ext_with_options_async(request, runtime)
+
     def image_moderation_with_options(
         self,
         request: green_20220302_models.ImageModerationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> green_20220302_models.ImageModerationResponse:
         UtilClient.validate_model(request)
         body = {}
```

### Comparing `alibabacloud_green20220302-1.0.4/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-1.0.5/alibabacloud_green20220302/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,293 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import List, Dict, Any
 
 
+class DescribeImageResultExtRequest(TeaModel):
+    def __init__(
+        self,
+        info_type: str = None,
+        req_id: str = None,
+    ):
+        self.info_type = info_type
+        self.req_id = req_id
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
+        if self.info_type is not None:
+            result['InfoType'] = self.info_type
+        if self.req_id is not None:
+            result['ReqId'] = self.req_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InfoType') is not None:
+            self.info_type = m.get('InfoType')
+        if m.get('ReqId') is not None:
+            self.req_id = m.get('ReqId')
+        return self
+
+
+class DescribeImageResultExtResponseBodyDataCustomImage(TeaModel):
+    def __init__(
+        self,
+        image_id: str = None,
+        lib_id: str = None,
+        lib_name: str = None,
+    ):
+        # 图片ID。
+        self.image_id = image_id
+        # 图库ID。
+        self.lib_id = lib_id
+        # 图库名。
+        self.lib_name = lib_name
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
+        if self.image_id is not None:
+            result['ImageId'] = self.image_id
+        if self.lib_id is not None:
+            result['LibId'] = self.lib_id
+        if self.lib_name is not None:
+            result['LibName'] = self.lib_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageId') is not None:
+            self.image_id = m.get('ImageId')
+        if m.get('LibId') is not None:
+            self.lib_id = m.get('LibId')
+        if m.get('LibName') is not None:
+            self.lib_name = m.get('LibName')
+        return self
+
+
+class DescribeImageResultExtResponseBodyDataPublicFigure(TeaModel):
+    def __init__(
+        self,
+        figure_id: str = None,
+    ):
+        # 人物ID。
+        self.figure_id = figure_id
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
+        if self.figure_id is not None:
+            result['FigureId'] = self.figure_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FigureId') is not None:
+            self.figure_id = m.get('FigureId')
+        return self
+
+
+class DescribeImageResultExtResponseBodyDataTextInImage(TeaModel):
+    def __init__(
+        self,
+        ocr_datas: List[str] = None,
+    ):
+        self.ocr_datas = ocr_datas
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
+        if self.ocr_datas is not None:
+            result['OcrDatas'] = self.ocr_datas
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OcrDatas') is not None:
+            self.ocr_datas = m.get('OcrDatas')
+        return self
+
+
+class DescribeImageResultExtResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        custom_image: List[DescribeImageResultExtResponseBodyDataCustomImage] = None,
+        public_figure: List[DescribeImageResultExtResponseBodyDataPublicFigure] = None,
+        text_in_image: DescribeImageResultExtResponseBodyDataTextInImage = None,
+    ):
+        self.custom_image = custom_image
+        self.public_figure = public_figure
+        self.text_in_image = text_in_image
+
+    def validate(self):
+        if self.custom_image:
+            for k in self.custom_image:
+                if k:
+                    k.validate()
+        if self.public_figure:
+            for k in self.public_figure:
+                if k:
+                    k.validate()
+        if self.text_in_image:
+            self.text_in_image.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['CustomImage'] = []
+        if self.custom_image is not None:
+            for k in self.custom_image:
+                result['CustomImage'].append(k.to_map() if k else None)
+        result['PublicFigure'] = []
+        if self.public_figure is not None:
+            for k in self.public_figure:
+                result['PublicFigure'].append(k.to_map() if k else None)
+        if self.text_in_image is not None:
+            result['TextInImage'] = self.text_in_image.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.custom_image = []
+        if m.get('CustomImage') is not None:
+            for k in m.get('CustomImage'):
+                temp_model = DescribeImageResultExtResponseBodyDataCustomImage()
+                self.custom_image.append(temp_model.from_map(k))
+        self.public_figure = []
+        if m.get('PublicFigure') is not None:
+            for k in m.get('PublicFigure'):
+                temp_model = DescribeImageResultExtResponseBodyDataPublicFigure()
+                self.public_figure.append(temp_model.from_map(k))
+        if m.get('TextInImage') is not None:
+            temp_model = DescribeImageResultExtResponseBodyDataTextInImage()
+            self.text_in_image = temp_model.from_map(m['TextInImage'])
+        return self
+
+
+class DescribeImageResultExtResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: DescribeImageResultExtResponseBodyData = None,
+        msg: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.msg = msg
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.msg is not None:
+            result['Msg'] = self.msg
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeImageResultExtResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Msg') is not None:
+            self.msg = m.get('Msg')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeImageResultExtResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeImageResultExtResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeImageResultExtResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ImageModerationRequest(TeaModel):
     def __init__(
         self,
         service: str = None,
         service_parameters: str = None,
     ):
         self.service = service
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_green20220302-1.0.4/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-1.0.5/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-1.0.4/setup.py` & `alibabacloud_green20220302-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 15/03/2023
+Created on 17/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
```

