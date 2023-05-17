# Comparing `tmp/datadog-cdk-constructs-v2-1.6.1.tar.gz` & `tmp/datadog-cdk-constructs-v2-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-cdk-constructs-v2-1.6.1.tar", last modified: Tue Apr 25 15:46:03 2023, max compression
+gzip compressed data, was "datadog-cdk-constructs-v2-1.7.0.tar", last modified: Wed May 17 21:24:43 2023, max compression
```

## Comparing `datadog-cdk-constructs-v2-1.6.1.tar` & `datadog-cdk-constructs-v2-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.785806 datadog-cdk-constructs-v2-1.6.1/
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    11358 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/LICENSE
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       23 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/MANIFEST.in
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    22293 2023-04-25 15:46:03.785655 datadog-cdk-constructs-v2-1.6.1/PKG-INFO
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    21313 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/README.md
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      236 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/pyproject.toml
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       38 2023-04-25 15:46:03.785879 datadog-cdk-constructs-v2-1.6.1/setup.cfg
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)     1921 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/setup.py
-drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.782670 datadog-cdk-constructs-v2-1.6.1/src/
-drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.784058 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    83134 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/__init__.py
-drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.785341 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/_jsii/
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      475 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/_jsii/__init__.py
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)   106621 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.6.1.jsii.tgz
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)        1 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/py.typed
-drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.784968 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    22293 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      523 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)        1 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      161 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/requires.txt
--rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       26 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.121111 datadog-cdk-constructs-v2-1.7.0/
+-rw-r--r--   0 david.lee   (503) staff       (20)    11358 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/LICENSE
+-rw-r--r--   0 david.lee   (503) staff       (20)       23 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/MANIFEST.in
+-rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-17 21:24:43.120968 datadog-cdk-constructs-v2-1.7.0/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)    21527 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/README.md
+-rw-r--r--   0 david.lee   (503) staff       (20)      236 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/pyproject.toml
+-rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-05-17 21:24:43.121165 datadog-cdk-constructs-v2-1.7.0/setup.cfg
+-rw-r--r--   0 david.lee   (503) staff       (20)     1921 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/setup.py
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.118023 datadog-cdk-constructs-v2-1.7.0/src/
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.119396 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/
+-rw-r--r--   0 david.lee   (503) staff       (20)    62499 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/__init__.py
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.120641 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/_jsii/
+-rw-r--r--   0 david.lee   (503) staff       (20)      475 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/_jsii/__init__.py
+-rw-r--r--   0 david.lee   (503) staff       (20)   133242 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.0.jsii.tgz
+-rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-17 21:24:39.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2/py.typed
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-17 21:24:43.120276 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/
+-rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-17 21:24:42.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)      523 2023-05-17 21:24:43.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-17 21:24:42.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)      161 2023-05-17 21:24:43.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/requires.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)       26 2023-05-17 21:24:43.000000 datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
```

### Comparing `datadog-cdk-constructs-v2-1.6.1/LICENSE` & `datadog-cdk-constructs-v2-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.6.1/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.6.1
+Version: 1.7.0
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -223,14 +223,15 @@
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
 | `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `redirectHandler` | `redirect_handler` | When set to `false`, skip redirecting handler to the Datadog Lambda Library's handler. Useful when only instrumenting with Datadog Lambda Extension. Defaults to `true`. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
```

### Comparing `datadog-cdk-constructs-v2-1.6.1/README.md` & `datadog-cdk-constructs-v2-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,15 @@
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
 | `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `redirectHandler` | `redirect_handler` | When set to `false`, skip redirecting handler to the Datadog Lambda Library's handler. Useful when only instrumenting with Datadog Lambda Extension. Defaults to `true`. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
```

### Comparing `datadog-cdk-constructs-v2-1.6.1/setup.py` & `datadog-cdk-constructs-v2-1.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "datadog-cdk-constructs-v2",
-    "version": "1.6.1",
+    "version": "1.7.0",
     "description": "CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2",
     "license": "Apache-2.0",
     "url": "https://github.com/DataDog/datadog-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Datadog",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "datadog_cdk_constructs_v2",
         "datadog_cdk_constructs_v2._jsii"
     ],
     "package_data": {
         "datadog_cdk_constructs_v2._jsii": [
-            "datadog-cdk-constructs-v2@1.6.1.jsii.tgz"
+            "datadog-cdk-constructs-v2@1.7.0.jsii.tgz"
         ],
         "datadog_cdk_constructs_v2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.6.1
+Version: 1.7.0
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -223,14 +223,15 @@
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
 | `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `redirectHandler` | `redirect_handler` | When set to `false`, skip redirecting handler to the Datadog Lambda Library's handler. Useful when only instrumenting with Datadog Lambda Extension. Defaults to `true`. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
```

### Comparing `datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt` & `datadog-cdk-constructs-v2-1.7.0/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/datadog_cdk_constructs_v2/py.typed
 src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
 src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
 src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
 src/datadog_cdk_constructs_v2.egg-info/requires.txt
 src/datadog_cdk_constructs_v2.egg-info/top_level.txt
 src/datadog_cdk_constructs_v2/_jsii/__init__.py
-src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.6.1.jsii.tgz
+src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.0.jsii.tgz
```

