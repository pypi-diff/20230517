# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.892.tar", last modified: Tue May 16 00:33:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.893.tar", last modified: Wed May 17 03:28:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.892.tar` & `tencentcloud-sdk-python-cwp-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)     3900 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   250541 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   905982 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:33:44.000000 tencentcloud-sdk-python-cwp-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   253271 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   910717 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:28:23.000000 tencentcloud-sdk-python-cwp-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/README.rst` & `tencentcloud-sdk-python-cwp-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3107,14 +3107,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeLogStorageConfig(self, request):
+        """获取日志存储配置
+
+        :param request: Request instance for DescribeLogStorageConfig.
+        :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeLogStorageConfigRequest`
+        :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeLogStorageConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLogStorageConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLogStorageConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeLogStorageRecord(self, request):
+        """获取日志存储量记录
+
+        :param request: Request instance for DescribeLogStorageRecord.
+        :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeLogStorageRecordRequest`
+        :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeLogStorageRecordResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLogStorageRecord", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLogStorageRecordResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeLogStorageStatistic(self, request):
         """获取日志检索容量使用统计
 
         :param request: Request instance for DescribeLogStorageStatistic.
         :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeLogStorageStatisticRequest`
         :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeLogStorageStatisticResponse`
 
@@ -5729,14 +5775,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyLogStorageConfig(self, request):
+        """修改日志存储配置
+
+        :param request: Request instance for ModifyLogStorageConfig.
+        :type request: :class:`tencentcloud.cwp.v20180228.models.ModifyLogStorageConfigRequest`
+        :rtype: :class:`tencentcloud.cwp.v20180228.models.ModifyLogStorageConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyLogStorageConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyLogStorageConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyMachineRemark(self, request):
         """修改主机备注信息
 
         :param request: Request instance for ModifyMachineRemark.
         :type request: :class:`tencentcloud.cwp.v20180228.models.ModifyMachineRemarkRequest`
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/cwp/v20180228/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13605,14 +13605,85 @@
             for item in params.get("List"):
                 obj = LicenseDetail()
                 obj._deserialize(item)
                 self.List.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLogStorageConfigRequest(AbstractModel):
+    """DescribeLogStorageConfig请求参数结构体
+
+    """
+
+
+class DescribeLogStorageConfigResponse(AbstractModel):
+    """DescribeLogStorageConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Type: 存储类型，string数组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: list of str
+        :param Period: 日志存储天数，3640表示不限
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Period: int
+        :param PeriodModifyCount: 本月Period的修改次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PeriodModifyCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Type = None
+        self.Period = None
+        self.PeriodModifyCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Type = params.get("Type")
+        self.Period = params.get("Period")
+        self.PeriodModifyCount = params.get("PeriodModifyCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeLogStorageRecordRequest(AbstractModel):
+    """DescribeLogStorageRecord请求参数结构体
+
+    """
+
+
+class DescribeLogStorageRecordResponse(AbstractModel):
+    """DescribeLogStorageRecord返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Records: 存储量记录
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Records: list of LogStorageRecord
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Records = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Records") is not None:
+            self.Records = []
+            for item in params.get("Records"):
+                obj = LogStorageRecord()
+                obj._deserialize(item)
+                self.Records.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeLogStorageStatisticRequest(AbstractModel):
     """DescribeLogStorageStatistic请求参数结构体
 
     """
 
 
 class DescribeLogStorageStatisticResponse(AbstractModel):
@@ -21477,14 +21548,49 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class LogStorageRecord(AbstractModel):
+    """日志存储量记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Month: 年月份
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Month: str
+        :param UsedSize: 存储量，字节
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UsedSize: int
+        :param InquireSize: 总量，字节
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InquireSize: int
+        """
+        self.Month = None
+        self.UsedSize = None
+        self.InquireSize = None
+
+
+    def _deserialize(self, params):
+        self.Month = params.get("Month")
+        self.UsedSize = params.get("UsedSize")
+        self.InquireSize = params.get("InquireSize")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class LoginWhiteCombinedInfo(AbstractModel):
     """异地登录合并后白名单
 
     """
 
     def __init__(self):
         r"""
@@ -22809,14 +22915,63 @@
             for item in params.get("ErrMsg"):
                 obj = LicenseUnBindRsp()
                 obj._deserialize(item)
                 self.ErrMsg.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class ModifyLogStorageConfigRequest(AbstractModel):
+    """ModifyLogStorageConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param IsModifyPeriod: 是否修改有效期
+        :type IsModifyPeriod: bool
+        :param Type: 存储类型，string数组
+        :type Type: list of str
+        :param Period: 日志存储天数，3640表示不限
+        :type Period: int
+        """
+        self.IsModifyPeriod = None
+        self.Type = None
+        self.Period = None
+
+
+    def _deserialize(self, params):
+        self.IsModifyPeriod = params.get("IsModifyPeriod")
+        self.Type = params.get("Type")
+        self.Period = params.get("Period")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyLogStorageConfigResponse(AbstractModel):
+    """ModifyLogStorageConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyMachineRemarkRequest(AbstractModel):
     """ModifyMachineRemark请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.893/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.893/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.892/setup.py` & `tencentcloud-sdk-python-cwp-3.0.893/setup.py`

 * *Files identical despite different names*

