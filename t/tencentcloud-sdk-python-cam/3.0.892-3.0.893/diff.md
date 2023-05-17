# Comparing `tmp/tencentcloud-sdk-python-cam-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-cam-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.892.tar", last modified: Tue May 16 00:29:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.893.tar", last modified: Wed May 17 03:24:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cam-3.0.892.tar` & `tencentcloud-sdk-python-cam-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/
--rw-r--r--   0 root         (0) root         (0)    78006 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/cam_client.py
--rw-r--r--   0 root         (0) root         (0)    10965 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/__init__.py
--rw-r--r--   0 root         (0) root         (0)   188385 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud_sdk_python_cam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:29:54.000000 tencentcloud-sdk-python-cam-3.0.892/tencentcloud_sdk_python_cam.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/
+-rw-r--r--   0 root         (0) root         (0)    78006 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/cam_client.py
+-rw-r--r--   0 root         (0) root         (0)    10965 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   188916 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud_sdk_python_cam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:24:36.000000 tencentcloud-sdk-python-cam-3.0.893/tencentcloud_sdk_python_cam.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cam-3.0.892/README.rst` & `tencentcloud-sdk-python-cam-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cam-3.0.893/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.892'
+__version__ = '3.0.893'
```

### Comparing `tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/cam_client.py` & `tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/cam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/errorcodes.py` & `tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.892/tencentcloud/cam/v20190116/models.py` & `tencentcloud-sdk-python-cam-3.0.893/tencentcloud/cam/v20190116/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1204,20 +1204,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param SAMLMetadataDocument: SAML元数据文档，需要base64 encode
         :type SAMLMetadataDocument: str
+        :param AuxiliaryDomain: 辅助域名
+        :type AuxiliaryDomain: str
         """
         self.SAMLMetadataDocument = None
+        self.AuxiliaryDomain = None
 
 
     def _deserialize(self, params):
         self.SAMLMetadataDocument = params.get("SAMLMetadataDocument")
+        self.AuxiliaryDomain = params.get("AuxiliaryDomain")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2132,25 +2136,29 @@
 
     def __init__(self):
         r"""
         :param SAMLMetadata: SAML元数据文档
         :type SAMLMetadata: str
         :param Status: 状态：0:未设置，1:已开启，2:已禁用
         :type Status: int
+        :param AuxiliaryDomain: 辅助域名
+        :type AuxiliaryDomain: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.SAMLMetadata = None
         self.Status = None
+        self.AuxiliaryDomain = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.SAMLMetadata = params.get("SAMLMetadata")
         self.Status = params.get("Status")
+        self.AuxiliaryDomain = params.get("AuxiliaryDomain")
         self.RequestId = params.get("RequestId")
 
 
 class DetachGroupPolicyRequest(AbstractModel):
     """DetachGroupPolicy请求参数结构体
 
     """
@@ -5825,22 +5833,26 @@
 
     def __init__(self):
         r"""
         :param Operate: 修改的操作类型:enable:启用,disable:禁用,updateSAML:修改元数据文档
         :type Operate: str
         :param SAMLMetadataDocument: 元数据文档，需要base64 encode，仅当Operate为updateSAML时需要此参数
         :type SAMLMetadataDocument: str
+        :param AuxiliaryDomain: 辅助域名
+        :type AuxiliaryDomain: str
         """
         self.Operate = None
         self.SAMLMetadataDocument = None
+        self.AuxiliaryDomain = None
 
 
     def _deserialize(self, params):
         self.Operate = params.get("Operate")
         self.SAMLMetadataDocument = params.get("SAMLMetadataDocument")
+        self.AuxiliaryDomain = params.get("AuxiliaryDomain")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cam-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.893/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cam-3.0.892/setup.py` & `tencentcloud-sdk-python-cam-3.0.893/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.892/tencentcloud_sdk_python_cam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.893/tencentcloud_sdk_python_cam.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

