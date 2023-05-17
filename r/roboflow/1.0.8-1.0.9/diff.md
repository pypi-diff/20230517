# Comparing `tmp/roboflow-1.0.8.tar.gz` & `tmp/roboflow-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.0.8.tar", last modified: Wed May  3 20:11:24 2023, max compression
+gzip compressed data, was "roboflow-1.0.9.tar", last modified: Wed May 17 15:30:07 2023, max compression
```

## Comparing `roboflow-1.0.8.tar` & `roboflow-1.0.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-03 20:10:55.000000 roboflow-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-03 20:11:24.586639 roboflow-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-03 20:10:55.000000 roboflow-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 20:10:55.000000 roboflow-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/archive/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:11:24.586639 roboflow-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-03 20:10:55.000000 roboflow-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-17 15:29:32.000000 roboflow-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-17 15:30:07.218940 roboflow-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-17 15:29:32.000000 roboflow-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 15:29:32.000000 roboflow-1.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/archive/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/models/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-17 15:29:32.000000 roboflow-1.0.9/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.214940 roboflow-1.0.9/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-17 15:30:07.000000 roboflow-1.0.9/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 15:30:06.000000 roboflow-1.0.9/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:30:07.218940 roboflow-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-17 15:29:32.000000 roboflow-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:07.218940 roboflow-1.0.9/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 15:29:32.000000 roboflow-1.0.9/tests/util/test_versions.py
```

### Comparing `roboflow-1.0.8/LICENSE` & `roboflow-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/PKG-INFO` & `roboflow-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.8
+Version: 1.0.9
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.8 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.9 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.8/README.md` & `roboflow-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/__init__.py` & `roboflow-1.0.9/roboflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.util.general import write_line
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
```

### Comparing `roboflow-1.0.8/roboflow/archive/plot.py` & `roboflow-1.0.9/roboflow/archive/plot.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/config.py` & `roboflow-1.0.9/roboflow/config.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/core/project.py` & `roboflow-1.0.9/roboflow/core/project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/core/version.py` & `roboflow-1.0.9/roboflow/core/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
                 )
             elif self.type == TYPE_INSTANCE_SEGMENTATION:
                 self.model = InstanceSegmentationModel(
                     self.__api_key,
                     self.id,
                     colors=self.colors,
                     preprocessing=self.preprocessing,
+                    local=local,
                 )
             elif self.type == TYPE_SEMANTIC_SEGMENTATION:
                 self.model = SemanticSegmentationModel(self.__api_key, self.id)
             else:
                 self.model = None
 
     def __check_if_generating(self):
```

### Comparing `roboflow-1.0.8/roboflow/core/workspace.py` & `roboflow-1.0.9/roboflow/core/workspace.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/models/classification.py` & `roboflow-1.0.9/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/models/inference.py` & `roboflow-1.0.9/roboflow/models/inference.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/models/instance_segmentation.py` & `roboflow-1.0.9/roboflow/models/instance_segmentation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from roboflow.config import INSTANCE_SEGMENTATION_MODEL, INSTANCE_SEGMENTATION_URL
 from roboflow.models.inference import InferenceModel
 
 
 class InstanceSegmentationModel(InferenceModel):
-    def __init__(self, api_key, version_id, colors=None, preprocessing=None):
+    def __init__(
+        self, api_key, version_id, colors=None, preprocessing=None, local=None
+    ):
         """
         :param api_key: Your API key (obtained via your workspace API settings page)
         :param version_id: The ID of the dataset version to use for predicting
         """
         super(InstanceSegmentationModel, self).__init__(api_key, version_id)
-        self.api_url = f"{INSTANCE_SEGMENTATION_URL}/{self.dataset_id}/{self.version}"
+        if local is None:
+            self.api_url = (
+                f"{INSTANCE_SEGMENTATION_URL}/{self.dataset_id}/{self.version}"
+            )
+        else:
+            self.api_url = f"{local}/{self.dataset_id}/{self.version}"
         self.colors = {} if colors is None else colors
         self.preprocessing = {} if preprocessing is None else preprocessing
 
     def predict(self, image_path, confidence=40):
         """
         Infers detections based on image from a specified model and image path
```

### Comparing `roboflow-1.0.8/roboflow/models/object_detection.py` & `roboflow-1.0.9/roboflow/models/object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/models/semantic_segmentation.py` & `roboflow-1.0.9/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/util/active_learning_utils.py` & `roboflow-1.0.9/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/util/clip_compare_utils.py` & `roboflow-1.0.9/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/util/image_utils.py` & `roboflow-1.0.9/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/util/prediction.py` & `roboflow-1.0.9/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/util/two_stage_utils.py` & `roboflow-1.0.9/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow/util/versions.py` & `roboflow-1.0.9/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/roboflow.egg-info/PKG-INFO` & `roboflow-1.0.9/roboflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.8
+Version: 1.0.9
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.8 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.9 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.8/roboflow.egg-info/SOURCES.txt` & `roboflow-1.0.9/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/setup.py` & `roboflow-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/models/test_instance_segmentation.py` & `roboflow-1.0.9/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/models/test_object_detection.py` & `roboflow-1.0.9/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/models/test_semantic_segmentation.py` & `roboflow-1.0.9/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/test_project.py` & `roboflow-1.0.9/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/test_queries.py` & `roboflow-1.0.9/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/test_version.py` & `roboflow-1.0.9/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/util/test_image_utils.py` & `roboflow-1.0.9/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.8/tests/util/test_versions.py` & `roboflow-1.0.9/tests/util/test_versions.py`

 * *Files identical despite different names*

