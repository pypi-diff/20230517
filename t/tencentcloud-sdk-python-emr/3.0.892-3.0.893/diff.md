# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.892.tar", last modified: Tue May 16 00:36:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.893.tar", last modified: Wed May 17 03:31:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.892.tar` & `tencentcloud-sdk-python-emr-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    27330 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    13881 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258513 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:36:24.000000 tencentcloud-sdk-python-emr-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    27330 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    13881 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258513 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:30:59.000000 tencentcloud-sdk-python-emr-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:31:00.000000 tencentcloud-sdk-python-emr-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-emr-3.0.892/README.rst` & `tencentcloud-sdk-python-emr-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.892/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.893/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.892/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.893/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.892/setup.py` & `tencentcloud-sdk-python-emr-3.0.893/setup.py`

 * *Files identical despite different names*
