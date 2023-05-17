# Comparing `tmp/tencentcloud-sdk-python-batch-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-batch-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.892.tar", last modified: Tue May 16 00:28:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.893.tar", last modified: Wed May 17 03:23:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-batch-3.0.892.tar` & `tencentcloud-sdk-python-batch-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)     8555 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194547 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    31537 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud_sdk_python_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/tencentcloud_sdk_python_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:28:26.000000 tencentcloud-sdk-python-batch-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)     8555 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194613 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    31537 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud_sdk_python_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/tencentcloud_sdk_python_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:23:06.000000 tencentcloud-sdk-python-batch-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-batch-3.0.892/README.rst` & `tencentcloud-sdk-python-batch-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4274,14 +4274,15 @@
         :type DiskType: str
         :param DiskId: 系统盘ID。LOCAL_BASIC 和 LOCAL_SSD 类型没有ID。暂时不支持该参数。
 该参数目前仅用于`DescribeInstances`等查询类接口的返回参数，不可用于`RunInstances`等写接口的入参。
         :type DiskId: str
         :param DiskSize: 系统盘大小，单位：GB。默认值为 50
         :type DiskSize: int
         :param CdcId: 所属的独享集群ID。
+注意：此字段可能返回 null，表示取不到有效值。
         :type CdcId: str
         """
         self.DiskType = None
         self.DiskId = None
         self.DiskSize = None
         self.CdcId = None
```

### Comparing `tencentcloud-sdk-python-batch-3.0.892/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-batch-3.0.893/tencentcloud/batch/v20170312/batch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-batch-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-batch-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.893/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.892/tencentcloud_sdk_python_batch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.893/tencentcloud_sdk_python_batch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.892/setup.py` & `tencentcloud-sdk-python-batch-3.0.893/setup.py`

 * *Files identical despite different names*

