# Comparing `tmp/fiat_copilot-0.1.0.tar.gz` & `tmp/fiat_copilot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiat_copilot-0.1.0.tar", max compression
+gzip compressed data, was "fiat_copilot-0.2.0.tar", max compression
```

## Comparing `fiat_copilot-0.1.0.tar` & `fiat_copilot-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1067 2023-05-15 09:19:33.630484 fiat_copilot-0.1.0/LICENSE
--rw-r--r--   0        0        0      126 2023-05-15 09:20:58.931340 fiat_copilot-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-15 09:25:30.519704 fiat_copilot-0.1.0/fiat_copilot/__init__.py
--rw-r--r--   0        0        0      938 2023-05-12 17:47:29.851966 fiat_copilot-0.1.0/fiat_copilot/examples/assets/asset_reload.py
--rw-r--r--   0        0        0     3629 2023-05-15 09:00:19.381887 fiat_copilot-0.1.0/fiat_copilot/examples/assets/lightning_tuning_with_job_submission.py
--rw-r--r--   0        0        0     2071 2023-05-11 13:34:07.488799 fiat_copilot-0.1.0/fiat_copilot/examples/assets/my_assets.py
--rw-r--r--   0        0        0     4782 2023-05-15 11:53:52.451814 fiat_copilot-0.1.0/fiat_copilot/examples/assets/xgboost_test.py
--rw-r--r--   0        0        0     1688 2023-05-15 04:56:55.649644 fiat_copilot-0.1.0/fiat_copilot/examples/serving/batch.py
--rw-r--r--   0        0        0      811 2023-05-14 09:24:43.688900 fiat_copilot-0.1.0/fiat_copilot/examples/serving/local_dev.py
--rw-r--r--   0        0        0     2202 2023-05-12 17:10:08.831843 fiat_copilot-0.1.0/fiat_copilot/examples/storage/obs_test.py
--rw-r--r--   0        0        0     1576 2023-05-10 04:18:02.732534 fiat_copilot-0.1.0/fiat_copilot/examples/storage/oss_test.py
--rw-r--r--   0        0        0        0 2023-05-09 10:04:13.657137 fiat_copilot-0.1.0/fiat_copilot/serving/__init__.py
--rw-r--r--   0        0        0     2399 2023-05-11 12:49:02.722534 fiat_copilot-0.1.0/fiat_copilot/serving/attendant.py
--rw-r--r--   0        0        0     2618 2023-05-15 09:35:11.492225 fiat_copilot-0.1.0/fiat_copilot/serving/context.py
--rw-r--r--   0        0        0      314 2023-05-11 13:00:55.141462 fiat_copilot-0.1.0/fiat_copilot/serving/domain.py
--rw-r--r--   0        0        0        0 2023-05-11 14:42:37.236819 fiat_copilot-0.1.0/fiat_copilot/trainer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 03:07:25.672572 fiat_copilot-0.1.0/fiat_copilot/trainer/hf_util.py
--rw-r--r--   0        0        0     2604 2023-05-15 07:31:26.572249 fiat_copilot-0.1.0/fiat_copilot/trainer/torch_util.py
--rw-r--r--   0        0        0     2126 2023-05-15 09:35:11.496849 fiat_copilot-0.1.0/fiat_copilot/trainer/xgboost_util.py
--rw-r--r--   0        0        0        0 2023-05-11 06:04:14.053753 fiat_copilot-0.1.0/fiat_copilot/utils/__init__.py
--rw-r--r--   0        0        0     2105 2023-05-15 09:35:34.528045 fiat_copilot-0.1.0/fiat_copilot/utils/alioss.py
--rw-r--r--   0        0        0      570 2023-05-11 06:05:22.164619 fiat_copilot-0.1.0/fiat_copilot/utils/config.py
--rw-r--r--   0        0        0     2171 2023-05-11 17:14:52.474698 fiat_copilot-0.1.0/fiat_copilot/utils/huaweiobs.py
--rw-r--r--   0        0        0     2763 2023-05-12 06:48:40.249657 fiat_copilot-0.1.0/fiat_copilot/utils/tencentcos.py
--rw-r--r--   0        0        0        0 2023-05-05 13:26:09.485594 fiat_copilot-0.1.0/fiat_copilot/workflow/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-11 05:12:26.593453 fiat_copilot-0.1.0/fiat_copilot/workflow/annotations.py
--rw-r--r--   0        0        0     2572 2023-05-15 09:35:11.495022 fiat_copilot-0.1.0/fiat_copilot/workflow/ray_utils.py
--rw-r--r--   0        0        0     2556 2023-05-15 09:35:11.490015 fiat_copilot-0.1.0/fiat_copilot/workflow/storage.py
--rw-r--r--   0        0        0      729 2023-05-15 09:40:11.891392 fiat_copilot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 fiat_copilot-0.1.0/setup.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 fiat_copilot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-15 09:19:33.630484 fiat_copilot-0.2.0/LICENSE
+-rw-r--r--   0        0        0      126 2023-05-15 09:20:58.931340 fiat_copilot-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 09:25:30.519704 fiat_copilot-0.2.0/fiat_copilot/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-12 17:47:29.851966 fiat_copilot-0.2.0/fiat_copilot/examples/assets/asset_reload.py
+-rw-r--r--   0        0        0     3629 2023-05-15 09:00:19.381887 fiat_copilot-0.2.0/fiat_copilot/examples/assets/lightning_tuning_with_job_submission.py
+-rw-r--r--   0        0        0     2120 2023-05-17 06:48:23.538946 fiat_copilot-0.2.0/fiat_copilot/examples/assets/my_assets.py
+-rw-r--r--   0        0        0     4782 2023-05-15 11:53:52.451814 fiat_copilot-0.2.0/fiat_copilot/examples/assets/xgboost_test.py
+-rw-r--r--   0        0        0     1688 2023-05-15 04:56:55.649644 fiat_copilot-0.2.0/fiat_copilot/examples/serving/batch.py
+-rw-r--r--   0        0        0      811 2023-05-14 09:24:43.688900 fiat_copilot-0.2.0/fiat_copilot/examples/serving/local_dev.py
+-rw-r--r--   0        0        0     2202 2023-05-12 17:10:08.831843 fiat_copilot-0.2.0/fiat_copilot/examples/storage/obs_test.py
+-rw-r--r--   0        0        0     1576 2023-05-10 04:18:02.732534 fiat_copilot-0.2.0/fiat_copilot/examples/storage/oss_test.py
+-rw-r--r--   0        0        0     1640 2023-05-17 12:59:25.100714 fiat_copilot-0.2.0/fiat_copilot/examples/training/lightning_mnist.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:04:13.657137 fiat_copilot-0.2.0/fiat_copilot/serving/__init__.py
+-rw-r--r--   0        0        0     2399 2023-05-11 12:49:02.722534 fiat_copilot-0.2.0/fiat_copilot/serving/attendant.py
+-rw-r--r--   0        0        0     2618 2023-05-15 09:35:11.492225 fiat_copilot-0.2.0/fiat_copilot/serving/context.py
+-rw-r--r--   0        0        0      314 2023-05-11 13:00:55.141462 fiat_copilot-0.2.0/fiat_copilot/serving/domain.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:42:37.236819 fiat_copilot-0.2.0/fiat_copilot/trainer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 03:07:25.672572 fiat_copilot-0.2.0/fiat_copilot/trainer/hf_util.py
+-rw-r--r--   0        0        0     2982 2023-05-17 12:59:25.098339 fiat_copilot-0.2.0/fiat_copilot/trainer/torch_util.py
+-rw-r--r--   0        0        0     2126 2023-05-15 09:35:11.496849 fiat_copilot-0.2.0/fiat_copilot/trainer/xgboost_util.py
+-rw-r--r--   0        0        0        0 2023-05-11 06:04:14.053753 fiat_copilot-0.2.0/fiat_copilot/utils/__init__.py
+-rw-r--r--   0        0        0     2105 2023-05-15 09:35:34.528045 fiat_copilot-0.2.0/fiat_copilot/utils/alioss.py
+-rw-r--r--   0        0        0      570 2023-05-11 06:05:22.164619 fiat_copilot-0.2.0/fiat_copilot/utils/config.py
+-rw-r--r--   0        0        0     2171 2023-05-11 17:14:52.474698 fiat_copilot-0.2.0/fiat_copilot/utils/huaweiobs.py
+-rw-r--r--   0        0        0     2763 2023-05-12 06:48:40.249657 fiat_copilot-0.2.0/fiat_copilot/utils/tencentcos.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:26:09.485594 fiat_copilot-0.2.0/fiat_copilot/workflow/__init__.py
+-rw-r--r--   0        0        0     1140 2023-05-11 05:12:26.593453 fiat_copilot-0.2.0/fiat_copilot/workflow/annotations.py
+-rw-r--r--   0        0        0     2572 2023-05-15 09:35:11.495022 fiat_copilot-0.2.0/fiat_copilot/workflow/ray_utils.py
+-rw-r--r--   0        0        0     2556 2023-05-15 09:35:11.490015 fiat_copilot-0.2.0/fiat_copilot/workflow/storage.py
+-rw-r--r--   0        0        0      729 2023-05-17 13:23:43.839411 fiat_copilot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 fiat_copilot-0.2.0/setup.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 fiat_copilot-0.2.0/PKG-INFO
```

### Comparing `fiat_copilot-0.1.0/LICENSE` & `fiat_copilot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/assets/asset_reload.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/assets/asset_reload.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/assets/lightning_tuning_with_job_submission.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/assets/lightning_tuning_with_job_submission.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/assets/my_assets.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/assets/my_assets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 
 import requests
 from rich import print
 
-from workflow.annotations import as_asset, form_definitions
-from workflow.ray_utils import adhoc_task_on_ray, ResourceQuota
-from workflow.storage import PersistStorage, DataFormat, get_io_manager
-from utils.config import get_application_conf
+from fiat_copilot.workflow.annotations import as_asset, form_definitions
+from fiat_copilot.workflow.ray_utils import adhoc_task_on_ray, ResourceQuota
+from fiat_copilot.workflow.storage import PersistStorage, DataFormat, get_io_manager
+from fiat_copilot.utils.config import get_application_conf
 
 
 @as_asset(
     name="get_baidu_html",
     description="get baidu",
     io_manager_key="text_io_manager"
 )
@@ -21,15 +21,15 @@
 
 @as_asset(
     name="get_user_info",
     description="get user information",
     io_manager_key="json_io_manager"
 )
 def get_user_info():
-    with open("../application.json", "r+", encoding='utf-8') as file_obj:
+    with open("application.json", "r+", encoding='utf-8') as file_obj:
         conf: dict = json.load(file_obj)
         info: dict = conf['info']
 
     return info
 
 
 @as_asset(
```

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/assets/xgboost_test.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/assets/xgboost_test.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/serving/batch.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/serving/batch.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/serving/local_dev.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/serving/local_dev.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/storage/obs_test.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/storage/obs_test.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/examples/storage/oss_test.py` & `fiat_copilot-0.2.0/fiat_copilot/examples/storage/oss_test.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/serving/attendant.py` & `fiat_copilot-0.2.0/fiat_copilot/serving/attendant.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/serving/context.py` & `fiat_copilot-0.2.0/fiat_copilot/serving/context.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/trainer/xgboost_util.py` & `fiat_copilot-0.2.0/fiat_copilot/trainer/xgboost_util.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/utils/alioss.py` & `fiat_copilot-0.2.0/fiat_copilot/utils/alioss.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/utils/config.py` & `fiat_copilot-0.2.0/fiat_copilot/utils/config.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/utils/huaweiobs.py` & `fiat_copilot-0.2.0/fiat_copilot/utils/huaweiobs.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/utils/tencentcos.py` & `fiat_copilot-0.2.0/fiat_copilot/utils/tencentcos.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/workflow/annotations.py` & `fiat_copilot-0.2.0/fiat_copilot/workflow/annotations.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/workflow/ray_utils.py` & `fiat_copilot-0.2.0/fiat_copilot/workflow/ray_utils.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/fiat_copilot/workflow/storage.py` & `fiat_copilot-0.2.0/fiat_copilot/workflow/storage.py`

 * *Files identical despite different names*

### Comparing `fiat_copilot-0.1.0/pyproject.toml` & `fiat_copilot-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fiat-copilot"
-version = "0.1.0"
+version = "0.2.0"
 description = "🧑‍🚀 - Fiat Copilot is a variety of utilities to smooth your ML development workflow."
 authors = ["ValerioL29 <cheng2029@foxmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "fiat_copilot"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fiat_copilot-0.1.0/setup.py` & `fiat_copilot-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from setuptools import setup
 
 packages = \
 ['fiat_copilot',
  'fiat_copilot.examples.assets',
  'fiat_copilot.examples.serving',
  'fiat_copilot.examples.storage',
+ 'fiat_copilot.examples.training',
  'fiat_copilot.serving',
  'fiat_copilot.trainer',
  'fiat_copilot.utils',
  'fiat_copilot.workflow']
 
 package_data = \
 {'': ['*']}
@@ -22,15 +23,15 @@
  'oss2>=2.17.0,<3.0.0',
  'ray[default]>=2.4.0,<3.0.0',
  'xgboost-ray>=0.1.15,<0.2.0',
  'xgboost>=1.7.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'fiat-copilot',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '🧑\u200d🚀 - Fiat Copilot is a variety of utilities to smooth your ML development workflow.',
     'long_description': '# Fiat-Copilot\n\n#### Description\n🧑\u200d🚀 - Fiat Copilot is a variety of utilities to smooth your ML development workflow.\n',
     'author': 'ValerioL29',
     'author_email': 'cheng2029@foxmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fiat_copilot-0.1.0/PKG-INFO` & `fiat_copilot-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiat-copilot
-Version: 0.1.0
+Version: 0.2.0
 Summary: 🧑‍🚀 - Fiat Copilot is a variety of utilities to smooth your ML development workflow.
 License: MIT
 Author: ValerioL29
 Author-email: cheng2029@foxmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

