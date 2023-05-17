# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.892.tar", last modified: Tue May 16 00:30:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.893.tar", last modified: Wed May 17 03:25:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.892.tar` & `tencentcloud-sdk-python-ccc-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)    36406 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140571 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:30:34.000000 tencentcloud-sdk-python-ccc-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)    36406 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142135 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:25:15.000000 tencentcloud-sdk-python-ccc-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/README.rst` & `tencentcloud-sdk-python-ccc-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/ccc/v20200210/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,51 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CalleeAttribute(AbstractModel):
+    """被叫属性
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Callee: 被叫号码
+        :type Callee: str
+        :param UUI: 随路数据
+        :type UUI: str
+        :param Variables: 参数
+        :type Variables: list of Variable
+        """
+        self.Callee = None
+        self.UUI = None
+        self.Variables = None
+
+
+    def _deserialize(self, params):
+        self.Callee = params.get("Callee")
+        self.UUI = params.get("UUI")
+        if params.get("Variables") is not None:
+            self.Variables = []
+            for item in params.get("Variables"):
+                obj = Variable()
+                obj._deserialize(item)
+                self.Variables.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CarrierPrivilegeNumberApplicant(AbstractModel):
     """运营商白名单号码申请单
 
     """
 
     def __init__(self):
         r"""
@@ -450,25 +487,31 @@
         :type Description: str
         :param NotAfter: 任务停止时间戳，Unix 秒级时间戳
         :type NotAfter: int
         :param Tries: 最大尝试次数
         :type Tries: int
         :param Variables: 自定义变量（仅高级版支持）
         :type Variables: list of Variable
+        :param UUI: UUI
+        :type UUI: str
+        :param CalleeAttributes: 被叫属性
+        :type CalleeAttributes: list of CalleeAttribute
         """
         self.SdkAppId = None
         self.NotBefore = None
         self.Callees = None
         self.Callers = None
         self.IvrId = None
         self.Name = None
         self.Description = None
         self.NotAfter = None
         self.Tries = None
         self.Variables = None
+        self.UUI = None
+        self.CalleeAttributes = None
 
 
     def _deserialize(self, params):
         self.SdkAppId = params.get("SdkAppId")
         self.NotBefore = params.get("NotBefore")
         self.Callees = params.get("Callees")
         self.Callers = params.get("Callers")
@@ -479,14 +522,21 @@
         self.Tries = params.get("Tries")
         if params.get("Variables") is not None:
             self.Variables = []
             for item in params.get("Variables"):
                 obj = Variable()
                 obj._deserialize(item)
                 self.Variables.append(obj)
+        self.UUI = params.get("UUI")
+        if params.get("CalleeAttributes") is not None:
+            self.CalleeAttributes = []
+            for item in params.get("CalleeAttributes"):
+                obj = CalleeAttribute()
+                obj._deserialize(item)
+                self.CalleeAttributes.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.893/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.893/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.892/setup.py` & `tencentcloud-sdk-python-ccc-3.0.893/setup.py`

 * *Files identical despite different names*

