# Comparing `tmp/alibabacloud_green20220302_py2-1.0.4.tar.gz` & `tmp/alibabacloud_green20220302_py2-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302_py2-1.0.4.tar", last modified: Wed Mar 15 06:48:35 2023, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302_py2-1.0.5.tar", last modified: Wed May 17 06:05:06 2023, max compression
```

## Comparing `alibabacloud_green20220302_py2-1.0.4.tar` & `alibabacloud_green20220302_py2-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/
--rw-r--r--   0 root         (0) root         (0)       88 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8075 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)    27347 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-03-15 06:48:35.000000 alibabacloud_green20220302_py2-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      139 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9185 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)    35779 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-05-17 06:05:06.000000 alibabacloud_green20220302_py2-1.0.5/setup.py
```

### Comparing `alibabacloud_green20220302_py2-1.0.4/LICENSE` & `alibabacloud_green20220302_py2-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.4/PKG-INFO` & `alibabacloud_green20220302_py2-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302_py2
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-1.0.4/README-CN.md` & `alibabacloud_green20220302_py2-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.4/README.md` & `alibabacloud_green20220302_py2-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,44 @@
     def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def describe_image_result_ext_with_options(self, request, runtime):
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
+    def describe_image_result_ext(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_image_result_ext_with_options(request, runtime)
+
     def image_moderation_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service):
             body['Service'] = request.service
         if not UtilClient.is_unset(request.service_parameters):
             body['ServiceParameters'] = request.service_parameters
```

### Comparing `alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,261 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
+class DescribeImageResultExtRequest(TeaModel):
+    def __init__(self, info_type=None, req_id=None):
+        self.info_type = info_type  # type: str
+        self.req_id = req_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeImageResultExtRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InfoType') is not None:
+            self.info_type = m.get('InfoType')
+        if m.get('ReqId') is not None:
+            self.req_id = m.get('ReqId')
+        return self
+
+
+class DescribeImageResultExtResponseBodyDataCustomImage(TeaModel):
+    def __init__(self, image_id=None, lib_id=None, lib_name=None):
+        # 图片ID。
+        self.image_id = image_id  # type: str
+        # 图库ID。
+        self.lib_id = lib_id  # type: str
+        # 图库名。
+        self.lib_name = lib_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeImageResultExtResponseBodyDataCustomImage, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, figure_id=None):
+        # 人物ID。
+        self.figure_id = figure_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeImageResultExtResponseBodyDataPublicFigure, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.figure_id is not None:
+            result['FigureId'] = self.figure_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('FigureId') is not None:
+            self.figure_id = m.get('FigureId')
+        return self
+
+
+class DescribeImageResultExtResponseBodyDataTextInImage(TeaModel):
+    def __init__(self, ocr_datas=None):
+        self.ocr_datas = ocr_datas  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeImageResultExtResponseBodyDataTextInImage, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ocr_datas is not None:
+            result['OcrDatas'] = self.ocr_datas
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OcrDatas') is not None:
+            self.ocr_datas = m.get('OcrDatas')
+        return self
+
+
+class DescribeImageResultExtResponseBodyData(TeaModel):
+    def __init__(self, custom_image=None, public_figure=None, text_in_image=None):
+        self.custom_image = custom_image  # type: list[DescribeImageResultExtResponseBodyDataCustomImage]
+        self.public_figure = public_figure  # type: list[DescribeImageResultExtResponseBodyDataPublicFigure]
+        self.text_in_image = text_in_image  # type: DescribeImageResultExtResponseBodyDataTextInImage
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
+        _map = super(DescribeImageResultExtResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, data=None, msg=None, request_id=None):
+        self.code = code  # type: int
+        self.data = data  # type: DescribeImageResultExtResponseBodyData
+        self.msg = msg  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(DescribeImageResultExtResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeImageResultExtResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeImageResultExtResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, service=None, service_parameters=None):
         self.service = service  # type: str
         self.service_parameters = service_parameters  # type: str
 
     def validate(self):
         pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_green20220302_py2-1.0.4/alibabacloud_green20220302_py2.egg-info/PKG-INFO` & `alibabacloud_green20220302_py2-1.0.5/alibabacloud_green20220302_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302-py2
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-1.0.4/setup.py` & `alibabacloud_green20220302_py2-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302_py2.
 
-Created on 15/03/2023
+Created on 17/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python2"
```

