# Comparing `tmp/Mattermost-API-0.14.tar.gz` & `tmp/Mattermost-API-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mattermost-API-0.14.tar", last modified: Wed May 17 17:08:41 2023, max compression
+gzip compressed data, was "Mattermost-API-0.15.tar", last modified: Wed May 17 17:22:05 2023, max compression
```

## Comparing `Mattermost-API-0.14.tar` & `Mattermost-API-0.15.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:08:41.201964 Mattermost-API-0.14/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 17:08:27.000000 Mattermost-API-0.14/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:08:41.201964 Mattermost-API-0.14/Mattermost-API/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/Mattermost_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mattermost.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_bleve_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_compliance_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_elasticsearch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_imports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_int_actions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_opengraph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_terms_of_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-17 17:08:27.000000 Mattermost-API-0.14/Mattermost-API/mm_usage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:08:41.201964 Mattermost-API-0.14/Mattermost_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 17:08:41.000000 Mattermost-API-0.14/Mattermost_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-17 17:08:41.000000 Mattermost-API-0.14/Mattermost_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:08:41.000000 Mattermost-API-0.14/Mattermost_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 17:08:41.000000 Mattermost-API-0.14/Mattermost_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 17:08:41.000000 Mattermost-API-0.14/Mattermost_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 17:08:41.201964 Mattermost-API-0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 17:08:27.000000 Mattermost-API-0.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-17 17:08:27.000000 Mattermost-API-0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:08:41.201964 Mattermost-API-0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 17:08:27.000000 Mattermost-API-0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:22:05.762494 Mattermost-API-0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 17:21:52.000000 Mattermost-API-0.15/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:22:05.762494 Mattermost-API-0.15/Mattermost-API/
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/Mattermost_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mattermost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_bleve_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_compliance_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_elasticsearch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_imports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_int_actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_opengraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_terms_of_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-17 17:21:52.000000 Mattermost-API-0.15/Mattermost-API/mm_usage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:22:05.762494 Mattermost-API-0.15/Mattermost_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 17:22:05.000000 Mattermost-API-0.15/Mattermost_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-17 17:22:05.000000 Mattermost-API-0.15/Mattermost_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:22:05.000000 Mattermost-API-0.15/Mattermost_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 17:22:05.000000 Mattermost-API-0.15/Mattermost_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 17:22:05.000000 Mattermost-API-0.15/Mattermost_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 17:22:05.762494 Mattermost-API-0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 17:21:52.000000 Mattermost-API-0.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-17 17:21:52.000000 Mattermost-API-0.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:22:05.762494 Mattermost-API-0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-17 17:21:52.000000 Mattermost-API-0.15/setup.py
```

### Comparing `Mattermost-API-0.14/LICENSE` & `Mattermost-API-0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/Mattermost_Base.py` & `Mattermost-API-0.15/Mattermost-API/Mattermost_Base.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/__init__.py` & `Mattermost-API-0.15/Mattermost-API/__init__.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mattermost.py` & `Mattermost-API-0.15/Mattermost-API/mattermost.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_bleve_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_bleve_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_compliance_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_compliance_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_elasticsearch_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_elasticsearch_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_exports_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_exports_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_imports_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_imports_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_int_actions_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_int_actions_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_opengraph_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_opengraph_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_permissions_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_permissions_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_terms_of_service_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_terms_of_service_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_uploads_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_uploads_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost-API/mm_usage_api.py` & `Mattermost-API-0.15/Mattermost-API/mm_usage_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/Mattermost_API.egg-info/PKG-INFO` & `Mattermost-API-0.15/Mattermost_API.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Mattermost-API
-Version: 0.14
+Version: 0.15
 Summary: Simple Mattermost API library
 Home-page: https://github.com/izhatomic/mattermost-api
 Download-URL: https://pypi.org/project/mattermost-api/
-Author: Aleksandr Kuznetsov, Aleksandr Zarin
+Author: Aleksandr Kuznetsov <izhatomic@yandex.ru>, Aleksandr Zarin <vector-777@yandex.ru>
 Author-email: Aleksandr Kuznetsov <izhatomic@yandex.ru>, Aleksandr Zarin <vector-777@yandex.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/izhatomic/mattermost-api
 Keywords: mattermost,mattermostapi,mattermost-api,mattermost api,mm api,mm-api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Mattermost-API-0.14/Mattermost_API.egg-info/SOURCES.txt` & `Mattermost-API-0.15/Mattermost_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.14/PKG-INFO` & `Mattermost-API-0.15/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Mattermost-API
-Version: 0.14
+Version: 0.15
 Summary: Simple Mattermost API library
 Home-page: https://github.com/izhatomic/mattermost-api
 Download-URL: https://pypi.org/project/mattermost-api/
-Author: Aleksandr Kuznetsov, Aleksandr Zarin
+Author: Aleksandr Kuznetsov <izhatomic@yandex.ru>, Aleksandr Zarin <vector-777@yandex.ru>
 Author-email: Aleksandr Kuznetsov <izhatomic@yandex.ru>, Aleksandr Zarin <vector-777@yandex.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/izhatomic/mattermost-api
 Keywords: mattermost,mattermostapi,mattermost-api,mattermost api,mm api,mm-api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Mattermost-API-0.14/pyproject.toml` & `Mattermost-API-0.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Mattermost-API"
-version = "0.14"
+version = "0.15"
 authors = [
     { name="Aleksandr Kuznetsov", email="izhatomic@yandex.ru" },
     { name="Aleksandr Zarin", email="vector-777@yandex.ru" },
 ]
 description = "Simple Mattermost API library"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `Mattermost-API-0.14/setup.py` & `Mattermost-API-0.15/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
-# HISTORY = ""
 
 setup_args = dict(
     name='Mattermost-API',
-    version='0.14',
+    version='0.15',
     description='Simple Mattermost API library',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
-    author='Aleksandr Kuznetsov, Aleksandr Zarin',
+    author='Aleksandr Kuznetsov <izhatomic@yandex.ru>, Aleksandr Zarin <vector-777@yandex.ru>',
     author_email='izhatomic@yandex.ru, vector-777@yandex.ru',
     keywords=['mattermost', 'mattermostapi', 'mattermost-api', "mattermost api", "mm api", "mm-api"],
     url='https://github.com/izhatomic/mattermost-api',
     download_url='https://pypi.org/project/mattermost-api/'
 )
 
 install_requires = [
```

