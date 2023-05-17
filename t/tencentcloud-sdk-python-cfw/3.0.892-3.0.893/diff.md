# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.892.tar", last modified: Tue May 16 00:31:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.893.tar", last modified: Wed May 17 03:26:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.892.tar` & `tencentcloud-sdk-python-cfw-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65621 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   216862 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:31:28.000000 tencentcloud-sdk-python-cfw-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65635 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219501 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:26:06.000000 tencentcloud-sdk-python-cfw-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/README.rst` & `tencentcloud-sdk-python-cfw-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def AddNatAcRule(self, request):
-        """添加nat访问控制规则
+        """添加nat访问控制规则(地域必填)
 
         :param request: Request instance for AddNatAcRule.
         :type request: :class:`tencentcloud.cfw.v20190904.models.AddNatAcRuleRequest`
         :rtype: :class:`tencentcloud.cfw.v20190904.models.AddNatAcRuleResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/cfw/v20190904/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,23 +278,33 @@
 
     """
 
     def __init__(self):
         r"""
         :param Status: 状态值，0：添加成功，非0：添加失败
         :type Status: int
+        :param Rules: 规则uuid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Rules: list of SecurityGroupSimplifyRule
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Status = None
+        self.Rules = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
+        if params.get("Rules") is not None:
+            self.Rules = []
+            for item in params.get("Rules"):
+                obj = SecurityGroupSimplifyRule()
+                obj._deserialize(item)
+                self.Rules.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class AddNatAcRuleRequest(AbstractModel):
     """AddNatAcRule请求参数结构体
 
     """
@@ -620,44 +630,34 @@
 
     """
 
     def __init__(self):
         r"""
         :param Name: 检索的键值
         :type Name: str
-        :param Values: 检索的值
+        :param Values: 检索的值，各检索值间为OR关系
         :type Values: list of str
-        :param OperatorType: 枚举类型，代表name与values之间的匹配关系
+        :param OperatorType: 枚举类型，代表Name与Values之间的匹配关系
 enum FilterOperatorType {
-    //INVALID
-    FILTER_OPERATOR_TYPE_INVALID = 0;
     //等于
     FILTER_OPERATOR_TYPE_EQUAL = 1;
     //大于
     FILTER_OPERATOR_TYPE_GREATER = 2;
     //小于
     FILTER_OPERATOR_TYPE_LESS = 3;
     //大于等于
     FILTER_OPERATOR_TYPE_GREATER_EQ = 4;
     //小于等于
     FILTER_OPERATOR_TYPE_LESS_EQ = 5;
     //不等于
     FILTER_OPERATOR_TYPE_NO_EQ = 6;
-    //in，数组中包含
-    FILTER_OPERATOR_TYPE_IN = 7;
     //not in
     FILTER_OPERATOR_TYPE_NOT_IN = 8;
     //模糊匹配
     FILTER_OPERATOR_TYPE_FUZZINESS = 9;
-    //存在
-    FILTER_OPERATOR_TYPE_EXIST = 10;
-    //不存在
-    FILTER_OPERATOR_TYPE_NOT_EXIST = 11;
-    //正则
-    FILTER_OPERATOR_TYPE_REGULAR = 12;
 }
         :type OperatorType: int
         """
         self.Name = None
         self.Values = None
         self.OperatorType = None
 
@@ -2234,38 +2234,42 @@
 -1/-1：全部端口
 80：80端口
         :type Port: str
         :param Protocol: 协议；TCP/UDP/ICMP/ANY
         :type Protocol: str
         :param ServiceTemplateId: 端口协议类型参数模板id；协议端口模板id；与Protocol,Port互斥
         :type ServiceTemplateId: str
+        :param RuleUuid: 规则的uuid
+        :type RuleUuid: int
         """
         self.PageNo = None
         self.PageSize = None
         self.SourceContent = None
         self.DestContent = None
         self.Description = None
         self.RuleAction = None
         self.Enable = None
         self.Port = None
         self.Protocol = None
         self.ServiceTemplateId = None
+        self.RuleUuid = None
 
 
     def _deserialize(self, params):
         self.PageNo = params.get("PageNo")
         self.PageSize = params.get("PageSize")
         self.SourceContent = params.get("SourceContent")
         self.DestContent = params.get("DestContent")
         self.Description = params.get("Description")
         self.RuleAction = params.get("RuleAction")
         self.Enable = params.get("Enable")
         self.Port = params.get("Port")
         self.Protocol = params.get("Protocol")
         self.ServiceTemplateId = params.get("ServiceTemplateId")
+        self.RuleUuid = params.get("RuleUuid")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6013,14 +6017,76 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SecurityGroupSimplifyRule(AbstractModel):
+    """安全组规则
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SourceContent: 访问源示例：
+net：IP/CIDR(192.168.0.2)
+template：参数模板(ipm-dyodhpby)
+instance：资产实例(ins-123456)
+resourcegroup：资产分组(/全部分组/分组1/子分组1)
+tag：资源标签({"Key":"标签key值","Value":"标签Value值"})
+region：地域(ap-gaungzhou)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SourceContent: str
+        :param DestContent: 访问目的示例：
+net：IP/CIDR(192.168.0.2)
+template：参数模板(ipm-dyodhpby)
+instance：资产实例(ins-123456)
+resourcegroup：资产分组(/全部分组/分组1/子分组1)
+tag：资源标签({"Key":"标签key值","Value":"标签Value值"})
+region：地域(ap-gaungzhou)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DestContent: str
+        :param Protocol: 协议；TCP/UDP/ICMP/ANY
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Protocol: str
+        :param Description: 描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param RuleUuid: 规则对应的唯一id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RuleUuid: int
+        :param Sequence: 规则序号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Sequence: int
+        """
+        self.SourceContent = None
+        self.DestContent = None
+        self.Protocol = None
+        self.Description = None
+        self.RuleUuid = None
+        self.Sequence = None
+
+
+    def _deserialize(self, params):
+        self.SourceContent = params.get("SourceContent")
+        self.DestContent = params.get("DestContent")
+        self.Protocol = params.get("Protocol")
+        self.Description = params.get("Description")
+        self.RuleUuid = params.get("RuleUuid")
+        self.Sequence = params.get("Sequence")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class SequenceData(AbstractModel):
     """执行顺序对象
 
     """
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.893/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.892/setup.py` & `tencentcloud-sdk-python-cfw-3.0.893/setup.py`

 * *Files identical despite different names*

