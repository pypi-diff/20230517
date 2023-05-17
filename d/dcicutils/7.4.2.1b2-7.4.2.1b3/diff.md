# Comparing `tmp/dcicutils-7.4.2.1b2.tar.gz` & `tmp/dcicutils-7.4.2.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.2.1b2.tar", max compression
+gzip compressed data, was "dcicutils-7.4.2.1b3.tar", max compression
```

## Comparing `dcicutils-7.4.2.1b2.tar` & `dcicutils-7.4.2.1b3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1098 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/README.rst
--rw-r--r--   0        0        0        0 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-17 17:35:17.751791 dcicutils-7.4.2.1b2/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    11602 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154684 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4010 2023-05-17 17:35:17.755791 dcicutils-7.4.2.1b2/pyproject.toml
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b2/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/README.rst
+-rw-r--r--   0        0        0        0 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-17 18:32:26.740041 dcicutils-7.4.2.1b3/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    12859 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154684 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     4010 2023-05-17 18:32:26.744041 dcicutils-7.4.2.1b3/pyproject.toml
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b3/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.4.2.1b3/PKG-INFO
```

### Comparing `dcicutils-7.4.2.1b2/LICENSE.txt` & `dcicutils-7.4.2.1b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/README.rst` & `dcicutils-7.4.2.1b3/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/base.py` & `dcicutils-7.4.2.1b3/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/codebuild_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/command_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/common.py` & `dcicutils-7.4.2.1b3/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/creds_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/data_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/deployment_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/diff_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/docker_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/ecr_scripts.py` & `dcicutils-7.4.2.1b3/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/ecr_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/ecs_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/env_base.py` & `dcicutils-7.4.2.1b3/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/env_manager.py` & `dcicutils-7.4.2.1b3/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/env_scripts.py` & `dcicutils-7.4.2.1b3/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/env_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.2.1b3/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/es_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/exceptions.py` & `dcicutils-7.4.2.1b3/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/ff_mocks.py` & `dcicutils-7.4.2.1b3/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/ff_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.2.1b3/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/glacier_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/jh_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.2.1b3/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/kibana/readme.md` & `dcicutils-7.4.2.1b3/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/lang_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/log_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/misc_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/opensearch_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/project_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/project_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,15 @@
+import contextlib
 import os
 import toml
 
 from pkg_resources import resource_filename
 from typing import Optional
 from .env_utils import EnvUtils
-from .misc_utils import classproperty
-
-
-def project_filename(filename):
-    # TODO: In fact we should do this based on the working dir so that when this is imported to another repo,
-    #       it gets the inserts out of that repo's tests, not our own.
-    return resource_filename(Project.PACKAGE_NAME, filename)
+from .misc_utils import classproperty, local_attrs
 
 
 class ProjectRegistry:
 
     SHOW_HERALD_WHEN_INITIALIZED = True
 
     REGISTERED_PROJECTS = {}
@@ -64,42 +59,53 @@
                     and declared_pyproject_name != inferred_pyproject_name):
                 raise RuntimeError(f"APPLICATION_PYPROJECT_NAME={declared_pyproject_name!r},"
                                    f" but {pyproject_toml_file} says it should be {inferred_pyproject_name!r}")
 
             cls._PYPROJECT_NAME = declared_pyproject_name or inferred_pyproject_name
 
     @classmethod
-    def register(cls, name):
+    def register(cls, pyproject_name):
         """
-        Registers a class to be used based on the name in the top of pyproject.toml.
+        Registers a class to be used based on pyproject_name (the name in the top of pyproject.toml).
         Note that this means that cgap-portal and fourfront will both register as 'encoded',
         as in:
 
             @Project.register('encoded')
             class FourfrontProject(EncodedCoreProject):
                 PRETTY_NAME = "Fourfront"
 
         Since fourfront and cgap-portal don't occupy the same space, no confusion should result.
         """
         def _wrap_class(the_class):
             the_class_name = the_class.__name__
             if not issubclass(the_class, Project):
                 raise ValueError(f"The class {the_class_name} must inherit from Project.")
-            lower_registry_name = name.lower()
+            explicit_pyproject_name = the_class.__dict__.get('PYPROJECT_NAME')
+            if explicit_pyproject_name:
+                message = f"Explicit {the_class_name}.PYPROJECT_NAME={explicit_pyproject_name!r} is not permitted."
+                if explicit_pyproject_name != pyproject_name:
+                    message += f" An assignment to {pyproject_name!r} is intended to be managed implicitly."
+                else:
+                    message += " This assignment is intended to be managed implicitly."
+                raise ValueError(message)
+            else:
+                the_class._PYPROJECT_NAME = pyproject_name  # no need for the caller to say this redundantly
+
+            lower_registry_name = pyproject_name.lower()
             for x in ['cgap-portal', 'fourfront', 'smaht']:
                 if x in lower_registry_name:
                     # It's an easy error to make, but the name of the project from which we're gaining foothold
                     # in pyproject.toml is 'encoded', not 'cgap-portal', etc., so the name 'encoded' will be
                     # needed for bootstrapping. So it should look like
                     # -kmp 15-May-2023
                     raise ValueError(f"Please use ProjectRegistry.register('encoded'),"
-                                     f" not ProjectRegistry.register({name!r})."
+                                     f" not ProjectRegistry.register({pyproject_name!r})."
                                      f" This registration is just for bootstrapping."
                                      f" The class can still be {the_class_name}.")
-            cls.REGISTERED_PROJECTS[name] = the_class
+            cls.REGISTERED_PROJECTS[pyproject_name] = the_class
             return the_class
         return _wrap_class
 
     @classmethod
     def _lookup(cls, name):
         """
         Returns the project object with the given name.
@@ -176,14 +182,21 @@
         """
         if cls._app_project is None:
             # You need to put a call to
             raise RuntimeError(f"Attempt to access {cls.__name__}.project before .initialize() called.")
         app_project: Project = cls._app_project
         return app_project
 
+    @classmethod
+    @contextlib.contextmanager
+    def project_registry_test_context(cls):
+        with local_attrs(cls, REGISTERED_PROJECTS={}):
+            assert cls.REGISTERED_PROJECTS == {}
+            yield
+
 
 class Project:
     """
     A class that should be a superclass of all classes registered using ProjectRegistry.register
 
     All such classes have these names:
       .NAME - The name of the project in pyproject.toml
@@ -204,23 +217,32 @@
      encoded      | smaht-portal |  smaht-portal  | SMaHT Portal | smaht     | SMaHT
 
      The registered name is the one used with the ProjectRegistry.register() decorator.
     """
 
     NAME = 'project'
 
+    _PYPROJECT_NAME = None
+
     @classmethod
     def _prettify(cls, name):
         return name.title().replace("Cgap", "CGAP").replace("Smaht", "SMaHT").replace("-", " ")
 
     @classproperty
     def PACKAGE_NAME(cls):  # noQA - PyCharm wants the variable name to be self
         return cls.NAME.replace('dcic', '')
 
     @classproperty
+    def PYPROJECT_NAME(cls) -> str:  # noQA - PyCharm wants the variable name to be self
+        pyproject_name = cls._PYPROJECT_NAME
+        if not pyproject_name:
+            raise RuntimeError(f"Class {cls} was not defined with ProjectRegistry.register")
+        return pyproject_name
+
+    @classproperty
     def PRETTY_NAME(cls):  # noQA - PyCharm wants the variable name to be self
         return cls._prettify(cls.PACKAGE_NAME)
 
     @classproperty
     def APP_NAME(cls):  # noQA - PyCharm wants the variable name to be self
         return cls.PACKAGE_NAME.replace('-portal', '').replace('encoded-', '')
 
@@ -250,7 +272,12 @@
 
         def app_project(initialize=False, initialization_options: Optional[dict] = None):
             if initialize:
                 Project.initialize_app_project(**(initialization_options or {}))
             return Project.app_project
 
         return app_project
+
+    @classmethod
+    def app_project_filename(cls, filename):
+        """Returns a filename relative to the current app_project."""
+        return resource_filename(cls.app_project.PYPROJECT_NAME, filename)
```

### Comparing `dcicutils-7.4.2.1b2/dcicutils/qa_checkers.py` & `dcicutils-7.4.2.1b3/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/qa_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/redis_tools.py` & `dcicutils-7.4.2.1b3/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/redis_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/s3_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.2.1b3/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/secrets_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/snapshot_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/task_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/dcicutils/trace_utils.py` & `dcicutils-7.4.2.1b3/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.2.1b2/pyproject.toml` & `dcicutils-7.4.2.1b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.2.1b2"  # to become 7.5.0
+version = "7.4.2.1b3"  # to become 7.5.0
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.2.1b2/setup.py` & `dcicutils-7.4.2.1b3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.2.1b2',
+    'version': '7.4.2.1b3',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.2.1b2/PKG-INFO` & `dcicutils-7.4.2.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.2.1b2
+Version: 7.4.2.1b3
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

