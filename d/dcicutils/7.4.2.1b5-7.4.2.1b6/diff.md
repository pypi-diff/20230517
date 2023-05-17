# Comparing `tmp/dcicutils-7.4.2.1b5.tar.gz` & `tmp/dcicutils-7.4.2.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.2.1b5.tar", max compression
+gzip compressed data, was "dcicutils-7.4.2.1b6.tar", max compression
```

## Comparing `dcicutils-7.4.2.1b5.tar` & `dcicutils-7.4.2.1b6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1098 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/README.rst
--rw-r--r--   0        0        0        0 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-17 19:05:44.291545 dcicutils-7.4.2.1b5/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    12913 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154684 2023-05-17 19:05:44.295545 dcicutils-7.4.2.1b5/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4010 2023-05-17 19:05:44.299545 dcicutils-7.4.2.1b5/pyproject.toml
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b5/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/README.rst
+-rw-r--r--   0        0        0        0 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-17 20:25:21.652726 dcicutils-7.4.2.1b6/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    14466 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-17 20:25:21.656726 dcicutils-7.4.2.1b6/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154684 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     4010 2023-05-17 20:25:21.660726 dcicutils-7.4.2.1b6/pyproject.toml
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b6/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b6/PKG-INFO
```

### Comparing `dcicutils-7.4.2.1b5/LICENSE.txt` & `dcicutils-7.4.2.1b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/README.rst` & `dcicutils-7.4.2.1b6/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/base.py` & `dcicutils-7.4.2.1b6/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/codebuild_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/command_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/common.py` & `dcicutils-7.4.2.1b6/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/creds_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/data_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/deployment_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/diff_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/docker_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/ecr_scripts.py` & `dcicutils-7.4.2.1b6/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/ecr_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/ecs_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/env_base.py` & `dcicutils-7.4.2.1b6/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/env_manager.py` & `dcicutils-7.4.2.1b6/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/env_scripts.py` & `dcicutils-7.4.2.1b6/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/env_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.2.1b6/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/es_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/exceptions.py` & `dcicutils-7.4.2.1b6/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/ff_mocks.py` & `dcicutils-7.4.2.1b6/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/ff_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.2.1b6/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/glacier_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/jh_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.2.1b6/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/kibana/readme.md` & `dcicutils-7.4.2.1b6/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/lang_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/log_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/misc_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/opensearch_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/project_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/project_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,46 +192,64 @@
 
 
 class Project:
     """
     A class that should be a superclass of all classes registered using ProjectRegistry.register
 
     All such classes have these names:
-      .NAME - The name of the project in pyproject.toml
-      .PACKAGE_NAME - The pypi name of the project, useful for pkg_resources, for example.
+      .PYPROJECT_NAME - The name used in the .register decorator on the class, and in pyproject.toml
+      .NAME - The name of the project in pypi
+      .REPO_NAME - The name of the repo
+      .PACKAGE_NAME - The installed name of the project as a package in a venv, for use with pkg_resources
       .PRETTY_NAME - The pretty name of the package name
       .APP_NAME - The ame of the project application (see dcicutils.common and the orchestrated app in EnvUtils)
       .APP_PRETTY_NAME - The pretty name of the project application.
 
-    Some sample usess of pre-defined attributes of a Project that may help motivate the choice of attribute names:
+    Some sample usess of pre-defined attributes of a Project that may help motivate the choice of attribute names,
+    though how these get initialized is easier if you're basing your package on C4Project,
 
-     registered name |
-          and        |
-     PYPROJECT_NAME  |    name     |     NAME     |  PACKAGE_NAME  |  PRETTY NAME |  APP_NAME | APP_PRETTY_NAME
-     ----------------+--------------+----------------+--------------+-----------+----------------
-     snovault        | dcicsnovault |  snovault      | Snovault     | snovault  | Snovault
-     encoded-core    | encoded-core |  encoded-core  | Encoded Core | core      | Core
-     encoded         | cgap-portal  |  cgap-portal   | CGAP Portal  | cgap      | CGAP
-     encoded         | fourfront    |  fourfront     | Fourfront    | fourfront | Fourfront
-     encoded         | smaht-portal |  smaht-portal  | SMaHT Portal | smaht     | SMaHT
+     registered name |   pypi name   |   repo name    |  name in venv |              |  env utils | pretty env utils
+          and        |     and       |      and       |     a.k.a.    |              |  name and  |   name and
+     PYPROJECT_NAME  |     NAME      |   REPO_NAME    |  PACKAGE_NAME |  PRETTY NAME |  APP_NAME  | APP_PRETTY_NAME
+     ----------------+---------------+----------------+---------------+--------------+------------+------------------
+     dcicsnovault    | dcicsnovault  |  snovault      |  snovault     | Snovault     | snovault   | Snovault
+     encoded-core    | encoded-core  |  encoded-core  |  encoded-core | Encoded Core | core       | Core
+     encoded         | cgap-portal   |  cgap-portal   |  encoded      | CGAP Portal  | cgap       | CGAP
+     encoded         | fourfront     |  fourfront     |  encoded      | Fourfront    | fourfront  | Fourfront
+     encoded         | smaht-portal  |  smaht-portal  |  encoded      | SMaHT Portal | smaht      | SMaHT
 
      The registered name is the one used with the ProjectRegistry.register() decorator.
     """
 
     NAME = 'project'
 
     _PYPROJECT_NAME = None
+    _PACKAGE_NAME = None
 
     @classmethod
     def _prettify(cls, name):
-        return name.title().replace("Cgap", "CGAP").replace("Smaht", "SMaHT").replace("-", " ")
+        return name.replace("-", " ")
+
+    @classproperty
+    def REPO_NAME(cls):  # noQA - PyCharm wants the variable name to be self
+        return cls.NAME
 
     @classproperty
     def PACKAGE_NAME(cls):  # noQA - PyCharm wants the variable name to be self
-        return cls.NAME.replace('dcic', '')
+        if cls._PACKAGE_NAME:
+            return cls._PACKAGE_NAME
+        poetry_data = ProjectRegistry.POETRY_DATA
+        if poetry_data:
+            # We expect the first package in the declared packages to be the primary export
+            # Other exported dirs, such as scripts or tests should be in later entries.
+            package_name = poetry_data['packages'][0]['include']
+        else:
+            package_name = cls.PYPROJECT_NAME
+        cls._PACKAGE_NAME = package_name
+        return package_name
 
     @classproperty
     def PYPROJECT_NAME(cls) -> str:  # noQA - PyCharm wants the variable name to be self
         pyproject_name = cls._PYPROJECT_NAME
         if not pyproject_name:
             raise RuntimeError(f"Class {cls} was not defined with ProjectRegistry.register")
         return pyproject_name
@@ -277,7 +295,22 @@
 
     def project_filename(self, filename):
         """Returns a filename relative to given instance."""
         if self != self.app_project:
             raise RuntimeError(f"{self}.project_filename invoked,"
                                f" but {self} is not the app_project, {self.app_project}.")
         return resource_filename(self.PYPROJECT_NAME, filename)
+
+
+class C4Project(Project):
+    """
+    Collect C4-specific functionality so that outside organizations don't have to use these heuristics
+    if they don't want to.
+    """
+
+    @classproperty
+    def REPO_NAME(cls):  # noQA - PyCharm wants the variable name to be self
+        return cls.NAME.replace('dcic', '')
+
+    @classmethod
+    def _prettify(cls, name):
+        return super()._prettify(name.title().replace("Cgap", "CGAP").replace("Smaht", "SMaHT"))
```

### Comparing `dcicutils-7.4.2.1b5/dcicutils/qa_checkers.py` & `dcicutils-7.4.2.1b6/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/qa_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/redis_tools.py` & `dcicutils-7.4.2.1b6/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/redis_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/s3_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.2.1b6/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/secrets_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/snapshot_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/task_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/dcicutils/trace_utils.py` & `dcicutils-7.4.2.1b6/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b5/pyproject.toml` & `dcicutils-7.4.2.1b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.2.1b5"  # to become 7.5.0
+version = "7.4.2.1b6"  # to become 7.5.0
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.2.1b5/setup.py` & `dcicutils-7.4.2.1b6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.2.1b5',
+    'version': '7.4.2.1b6',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.2.1b5/PKG-INFO` & `dcicutils-7.4.2.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.2.1b5
+Version: 7.4.2.1b6
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

