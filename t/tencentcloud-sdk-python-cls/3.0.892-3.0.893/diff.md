# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.892.tar", last modified: Tue May 16 00:32:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.893.tar", last modified: Wed May 17 03:27:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.892.tar` & `tencentcloud-sdk-python-cls-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   253720 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67925 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:32:47.000000 tencentcloud-sdk-python-cls-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   254085 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67925 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:27:15.000000 tencentcloud-sdk-python-cls-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.892/README.rst` & `tencentcloud-sdk-python-cls-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,30 +268,36 @@
         :type Number: int
         :param StartTimeOffset: 查询范围起始时间相对于告警执行时间的偏移，单位为分钟，取值为非正，最大值为0，最小值为-1440。
         :type StartTimeOffset: int
         :param EndTimeOffset: 查询范围终止时间相对于告警执行时间的偏移，单位为分钟，取值为非正，须大于StartTimeOffset，最大值为0，最小值为-1440。
         :type EndTimeOffset: int
         :param LogsetId: 日志集ID。
         :type LogsetId: str
+        :param SyntaxRule: 检索语法规则，默认值为0。
+0：Lucene语法，1：CQL语法。
+详细说明参见<a href="https://cloud.tencent.com/document/product/614/47044#RetrievesConditionalRules" target="_blank">检索条件语法规则</a>
+        :type SyntaxRule: int
         """
         self.TopicId = None
         self.Query = None
         self.Number = None
         self.StartTimeOffset = None
         self.EndTimeOffset = None
         self.LogsetId = None
+        self.SyntaxRule = None
 
 
     def _deserialize(self, params):
         self.TopicId = params.get("TopicId")
         self.Query = params.get("Query")
         self.Number = params.get("Number")
         self.StartTimeOffset = params.get("StartTimeOffset")
         self.EndTimeOffset = params.get("EndTimeOffset")
         self.LogsetId = params.get("LogsetId")
+        self.SyntaxRule = params.get("SyntaxRule")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.892/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.893/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.892/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.893/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.892/setup.py` & `tencentcloud-sdk-python-cls-3.0.893/setup.py`

 * *Files identical despite different names*

