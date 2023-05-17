# Comparing `tmp/aws-cdk-secure-api-0.1.2.tar.gz` & `tmp/aws-cdk-secure-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-secure-api-0.1.2.tar", last modified: Fri Jun 24 19:08:47 2022, max compression
+gzip compressed data, was "aws-cdk-secure-api-0.2.0.tar", last modified: Wed May 17 16:40:30 2023, max compression
```

## Comparing `aws-cdk-secure-api-0.1.2.tar` & `aws-cdk-secure-api-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7831 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5060 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:46.997109 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7151 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/api_construct.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2681 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/client_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/ssm_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7831 2022-06-24 19:08:46.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-06-24 19:08:46.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 19:08:46.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 19:08:46.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-24 19:08:46.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-24 19:08:46.000000 aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/aws_cdk_secure_api.aws.rst
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/aws_cdk_secure_api.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4918 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 19:08:47.001109 aws-cdk-secure-api-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-06-24 19:08:41.000000 aws-cdk-secure-api-0.1.2/tests/unit/test_aws_cdk_secure_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/api_construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/client_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/ssm_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-17 16:40:29.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-17 16:40:30.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:40:29.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:40:29.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 16:40:29.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 16:40:29.000000 aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/aws_cdk_secure_api.aws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/aws_cdk_secure_api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4918 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:40:30.075630 aws-cdk-secure-api-0.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-17 16:40:22.000000 aws-cdk-secure-api-0.2.0/tests/unit/test_aws_cdk_secure_api.py
```

### Comparing `aws-cdk-secure-api-0.1.2/CONTRIBUTING.rst` & `aws-cdk-secure-api-0.2.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.7, 3.8, 3.9 and 3.10, and for PyPy. Check
+3. The pull request should work for Python 3.7, 3.8, 3.9, 3.10 and 3.11, and for PyPy. Check
    https://github.com/rnag/aws-cdk-secure-api/actions/workflows/dev.yml
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `aws-cdk-secure-api-0.1.2/LICENSE` & `aws-cdk-secure-api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/PKG-INFO` & `aws-cdk-secure-api-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-secure-api
-Version: 0.1.2
+Version: 0.2.0
 Summary: A CDK (v2) Construct Library for Secure REST APIs
 Home-page: https://github.com/rnag/aws-cdk-secure-api
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Project-URL: Documentation, https://aws-cdk-secure-api.readthedocs.io
 Project-URL: Source, https://github.com/rnag/aws-cdk-secure-api
@@ -147,14 +147,25 @@
         .. _`rnag/cookiecutter-pypackage`: https://github.com/rnag/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.2.0 (2023-05-17)
+        ------------------
+        
+        **Bugfixes**
+        
+        * Make code compatible with *Python 3.11*.
+        
+        **Features and Improvements**
+        
+        * Add *3.11* to the list of supported Python versions.
+        
         0.1.1 (2022-06-24)
         ------------------
         
         **Bugfixes**
         
         * Remove ``typing.Literal`` usage, so code is compatible with Python 3.7
         * Add an import ``from __future__ import annotations`` to modules where it was missing.
@@ -177,9 +188,10 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
```

### Comparing `aws-cdk-secure-api-0.1.2/README.rst` & `aws-cdk-secure-api-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/__init__.py` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/api_construct.py` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/api_construct.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/client_cache.py` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/client_cache.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/secrets_manager.py` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/aws/ssm_parameter_store.py` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/aws/ssm_parameter_store.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/cache.py` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/cache.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api/models.py` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum, auto
 
 from aws_cdk import aws_apigateway as apigateway
 
 
 @dataclass
 class Config:
@@ -24,23 +24,27 @@
     key_id: str | None = None
 
     # Whether to override the CDK stack output name for the API endpoint.
     # Defaults to `True` if not specified.
     override_endpoint_name = True
 
     # Throttle settings to associate with the Usage Plan for the REST API
-    throttle: apigateway.ThrottleSettings = apigateway.ThrottleSettings(
-        burst_limit=500,
-        rate_limit=1000
+    throttle: apigateway.ThrottleSettings = field(
+        default_factory=lambda: apigateway.ThrottleSettings(
+            burst_limit=500,
+            rate_limit=1000,
+        ),
     )
 
     # Quota settings to associate with the Usage Plan for the REST API
-    quota: apigateway.QuotaSettings = apigateway.QuotaSettings(
-        limit=10000000,
-        period=apigateway.Period.MONTH
+    quota: apigateway.QuotaSettings = field(
+        default_factory=lambda: apigateway.QuotaSettings(
+            limit=10000000,
+            period=apigateway.Period.MONTH,
+        ),
     )
 
 
 # noinspection PyArgumentList
 class Http(Enum):
     """Enum class to represent an HTTP method."""
     OPTIONS = auto()
```

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/PKG-INFO` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-secure-api
-Version: 0.1.2
+Version: 0.2.0
 Summary: A CDK (v2) Construct Library for Secure REST APIs
 Home-page: https://github.com/rnag/aws-cdk-secure-api
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Project-URL: Documentation, https://aws-cdk-secure-api.readthedocs.io
 Project-URL: Source, https://github.com/rnag/aws-cdk-secure-api
@@ -147,14 +147,25 @@
         .. _`rnag/cookiecutter-pypackage`: https://github.com/rnag/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.2.0 (2023-05-17)
+        ------------------
+        
+        **Bugfixes**
+        
+        * Make code compatible with *Python 3.11*.
+        
+        **Features and Improvements**
+        
+        * Add *3.11* to the list of supported Python versions.
+        
         0.1.1 (2022-06-24)
         ------------------
         
         **Bugfixes**
         
         * Remove ``typing.Literal`` usage, so code is compatible with Python 3.7
         * Add an import ``from __future__ import annotations`` to modules where it was missing.
@@ -177,9 +188,10 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
```

### Comparing `aws-cdk-secure-api-0.1.2/aws_cdk_secure_api.egg-info/SOURCES.txt` & `aws-cdk-secure-api-0.2.0/aws_cdk_secure_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/docs/Makefile` & `aws-cdk-secure-api-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/docs/aws_cdk_secure_api.aws.rst` & `aws-cdk-secure-api-0.2.0/docs/aws_cdk_secure_api.aws.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/docs/aws_cdk_secure_api.rst` & `aws-cdk-secure-api-0.2.0/docs/aws_cdk_secure_api.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/docs/conf.py` & `aws-cdk-secure-api-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/docs/installation.rst` & `aws-cdk-secure-api-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/docs/make.bat` & `aws-cdk-secure-api-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.1.2/setup.py` & `aws-cdk-secure-api-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,13 +55,14 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python'
     ],
     test_suite='tests',
     tests_require=test_requirements,
     zip_safe=False
 )
```

