# Comparing `tmp/dcicutils-7.4.1.tar.gz` & `tmp/dcicutils-7.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.1.tar", max compression
+gzip compressed data, was "dcicutils-7.4.2.tar", max compression
```

## Comparing `dcicutils-7.4.1.tar` & `dcicutils-7.4.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1098 2023-05-12 17:56:15.118342 dcicutils-7.4.1/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-12 17:56:15.122341 dcicutils-7.4.1/README.rst
--rw-r--r--   0        0        0        0 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3587 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    32242 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-12 17:56:15.122341 dcicutils-7.4.1/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20234 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154684 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-12 17:56:15.126341 dcicutils-7.4.1/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3987 2023-05-12 17:56:15.126341 dcicutils-7.4.1/pyproject.toml
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 dcicutils-7.4.1/setup.py
--rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-17 16:33:39.421344 dcicutils-7.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-17 16:33:39.421344 dcicutils-7.4.2/README.rst
+-rw-r--r--   0        0        0        0 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-17 16:33:39.421344 dcicutils-7.4.2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154684 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-17 16:33:39.425344 dcicutils-7.4.2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-05-17 16:33:39.429344 dcicutils-7.4.2/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-17 16:33:39.429344 dcicutils-7.4.2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-17 16:33:39.429344 dcicutils-7.4.2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-17 16:33:39.429344 dcicutils-7.4.2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-17 16:33:39.429344 dcicutils-7.4.2/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-17 16:33:39.429344 dcicutils-7.4.2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3987 2023-05-17 16:33:39.429344 dcicutils-7.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 dcicutils-7.4.2/setup.py
+-rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.4.2/PKG-INFO
```

### Comparing `dcicutils-7.4.1/LICENSE.txt` & `dcicutils-7.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/README.rst` & `dcicutils-7.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/base.py` & `dcicutils-7.4.2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/codebuild_utils.py` & `dcicutils-7.4.2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/command_utils.py` & `dcicutils-7.4.2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/common.py` & `dcicutils-7.4.2/dcicutils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,14 @@
     'STANDARD', 'STANDARD_IA', 'INTELLIGENT_TIERING'
 ]
 # Refs:
 #  * https://docs.aws.amazon.com/AmazonS3/latest/userguide/storage-class-intro.html
 #
 # See boto3 docs for info on possible values, but these 3 are the current ones used for
 # glacier (that require restore calls) - Will 7 Apr 2023
-
 S3_GLACIER_CLASSES = [
     'GLACIER_IR',  # Glacier Instant Retrieval
     'GLACIER',  # Glacier Flexible Retrieval
     'DEEP_ARCHIVE'  # Glacier Deep Archive
 ]
 S3GlacierClass = Union[
     Literal['GLACIER_IR'],
@@ -114,11 +113,15 @@
     Literal['GLACIER'],
     Literal['DEEP_ARCHIVE'],
     Literal['OUTPOSTS'],
     Literal['GLACIER_IR'],
 ]
 
 
+# This constant is used in our Lifecycle management system to automatically transition objects
+ENCODED_LIFECYCLE_TAG_KEY = 'Lifecycle'
+
+
 # These numbers come from AWS and is the max size that can be copied with a single request
 # Any larger than this requires a multipart upload - Will 24 April 2023
 MAX_STANDARD_COPY_SIZE = 5368709120
 MAX_MULTIPART_CHUNKS = 10000
```

### Comparing `dcicutils-7.4.1/dcicutils/creds_utils.py` & `dcicutils-7.4.2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/data_utils.py` & `dcicutils-7.4.2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/deployment_utils.py` & `dcicutils-7.4.2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/diff_utils.py` & `dcicutils-7.4.2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/docker_utils.py` & `dcicutils-7.4.2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/ecr_scripts.py` & `dcicutils-7.4.2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/ecr_utils.py` & `dcicutils-7.4.2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/ecs_utils.py` & `dcicutils-7.4.2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/env_base.py` & `dcicutils-7.4.2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/env_manager.py` & `dcicutils-7.4.2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/env_scripts.py` & `dcicutils-7.4.2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/env_utils.py` & `dcicutils-7.4.2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/es_utils.py` & `dcicutils-7.4.2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/exceptions.py` & `dcicutils-7.4.2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/ff_mocks.py` & `dcicutils-7.4.2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/ff_utils.py` & `dcicutils-7.4.2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.2/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/glacier_utils.py` & `dcicutils-7.4.2/dcicutils/glacier_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import boto3
 from typing import Union, List, Tuple
 from concurrent.futures import ThreadPoolExecutor
 from tqdm import tqdm
-from .common import S3_GLACIER_CLASSES, S3StorageClass, MAX_MULTIPART_CHUNKS, MAX_STANDARD_COPY_SIZE
+from .common import (
+    S3_GLACIER_CLASSES, S3StorageClass, MAX_MULTIPART_CHUNKS, MAX_STANDARD_COPY_SIZE,
+    ENCODED_LIFECYCLE_TAG_KEY
+)
 from .command_utils import require_confirmation
 from .misc_utils import PRINT
 from .ff_utils import get_metadata, search_metadata, get_health_page, patch_metadata
 from .creds_utils import CGAPKeyManager
 
 
 class GlacierRestoreException(Exception):
@@ -251,35 +254,52 @@
                 PRINT(f'No Glacier version found for object {bucket}/{key}')
                 return False
             return True
         except Exception as e:
             PRINT(f'Error deleting Glacier versions of object {bucket}/{key}: {str(e)}')
             return False
 
+    @staticmethod
+    def _format_tags(tags: List[dict]) -> str:
+        """ Helper method that formats tags so that they match the format expected by the boto3 API
+
+        :param tags: array of dictionaries containing Key, Value mappings to be reformatted
+        :return: String formatted tag list ie:
+            [{Key: key1, Value: value1}, Key: key2, Value: value2}] --> 'key1=value1&key2=value2'
+        """
+        return '&'.join([f'{tag["Key"]}={tag["Value"]}' for tag in tags])
+
     def _do_multipart_upload(self, bucket: str, key: str, total_size: int, part_size: int = 200,
-                             storage_class: str = 'STANDARD', version_id: Union[str, None] = None) -> Union[dict, None]:
+                             storage_class: str = 'STANDARD', tags: str = '',
+                             version_id: Union[str, None] = None) -> Union[dict, None]:
         """ Helper function for copy_object_back_to_original_location, not intended to
             be called directly, will arrange for a multipart copy of large updates
             to change storage class
 
         :param bucket: bucket to copy from
         :param key: key to copy within bucket
         :param total_size: total size of object
         :param part_size: what size to divide the object into when uploading the chunks
         :param storage_class: new storage class to use
+        :param tags: string of tags to apply
         :param version_id: object version ID, if applicable
         :return: response, if successful, or else None
         """
         try:
             part_size = part_size * 1024 * 1024  # convert MB to B
             num_parts = int(total_size / part_size) + 1
             if num_parts > MAX_MULTIPART_CHUNKS:
                 raise GlacierRestoreException(f'Must user a part_size larger than {part_size}'
                                               f' that will result in fewer than {MAX_MULTIPART_CHUNKS} chunks')
-            mpu = self.s3.create_multipart_upload(Bucket=bucket, Key=key, StorageClass=storage_class)
+            cmu = {
+                'Bucket': bucket, 'Key': key, 'StorageClass': storage_class
+            }
+            if tags:
+                cmu['Tagging'] = tags
+            mpu = self.s3.create_multipart_upload(**cmu)
             mpu_upload_id = mpu['UploadId']
         except Exception as e:
             PRINT(f'Error creating multipart upload for {bucket}/{key} : {str(e)}')
             return None
         parts = []
         for i in range(num_parts):
             start = i * part_size
@@ -323,45 +343,57 @@
                 'Parts': parts
             },
             UploadId=mpu_upload_id
         )
 
     def copy_object_back_to_original_location(self, bucket: str, key: str, storage_class: str = 'STANDARD',
                                               part_size: int = 200,  # MB
+                                              preserve_lifecycle_tag: bool = False,
                                               version_id: Union[str, None] = None) -> Union[dict, None]:
         """ Reads the temporary location from the restored object and copies it back to the original location
 
         :param bucket: bucket where object is stored
         :param key: key within bucket where object is stored
         :param storage_class: new storage class for this object
         :param part_size: if doing a large copy, size of chunks to upload (in MB)
+        :param preserve_lifecycle_tag: whether to keep existing lifecycle tag on the object
         :param version_id: version of object, if applicable
         :return: boolean whether the copy was successful
         """
         # Determine file size
         try:
             response = self.s3.head_object(Bucket=bucket, Key=key)
             size = response['ContentLength']
             multipart = (size >= MAX_STANDARD_COPY_SIZE)
+            if not preserve_lifecycle_tag:  # default: preserve tags except 'Lifecycle'
+                tags = self.s3.get_object_tagging(Bucket=bucket, Key=key).get('TagSet', [])
+                tags = [tag for tag in tags if tag['Key'] != ENCODED_LIFECYCLE_TAG_KEY]
+                tags = self._format_tags(tags)
+                if not tags:
+                    self.s3.delete_object_tagging(Bucket=bucket, Key=key)
+            else:
+                tags = ''
         except Exception as e:
             PRINT(f'Could not retrieve metadata on file {bucket}/{key} : {str(e)}')
             return None
         try:
             if multipart:
-                return self._do_multipart_upload(bucket, key, size, part_size, storage_class, version_id)
+                return self._do_multipart_upload(bucket, key, size, part_size, storage_class, tags, version_id)
             else:
                 # Force copy the object into standard in a single operation
                 copy_source = {'Bucket': bucket, 'Key': key}
                 copy_target = {
                     'Bucket': bucket, 'Key': key,
                     'StorageClass': storage_class,
                 }
                 if version_id:
                     copy_source['VersionId'] = version_id
                     copy_target['CopySourceVersionId'] = version_id
+                if tags:
+                    copy_target['Tagging'] = tags
                 response = self.s3.copy_object(CopySource=copy_source, **copy_target)
                 PRINT(f'Response from boto3 copy:\n{response}')
                 PRINT(f'Object {bucket}/{key} copied back to its original location in S3')
                 return response
         except Exception as e:
             PRINT(f'Error copying object {bucket}/{key} back to its original location in S3: {str(e)}')
             return None
```

### Comparing `dcicutils-7.4.1/dcicutils/jh_utils.py` & `dcicutils-7.4.2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/kibana/readme.md` & `dcicutils-7.4.2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/lang_utils.py` & `dcicutils-7.4.2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/log_utils.py` & `dcicutils-7.4.2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/misc_utils.py` & `dcicutils-7.4.2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/opensearch_utils.py` & `dcicutils-7.4.2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/qa_checkers.py` & `dcicutils-7.4.2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/qa_utils.py` & `dcicutils-7.4.2/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/redis_tools.py` & `dcicutils-7.4.2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/redis_utils.py` & `dcicutils-7.4.2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/s3_utils.py` & `dcicutils-7.4.2/dcicutils/s3_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,14 +458,16 @@
     def s3_put(self, obj, upload_key, acl=None):
         """
         try to guess content type
         """
         content_type = mimetypes.guess_type(upload_key)[0]
         if content_type is None:
             content_type = 'binary/octet-stream'
+        if isinstance(obj, dict):
+            obj = json.dumps(obj)
         if acl:
             # we use this to set some of the object as public
             return self.s3.put_object(Bucket=self.outfile_bucket,
                                       Key=upload_key,
                                       Body=obj,
                                       ContentType=content_type,
                                       ACL=acl)
@@ -476,14 +478,16 @@
                                       ContentType=content_type)
 
     def s3_put_secret(self, data, keyname, bucket=None, secret=None):
         if not bucket:
             bucket = self.sys_bucket
         if not secret:
             secret = os.environ["S3_ENCRYPT_KEY"]
+        if isinstance(data, dict):
+            data = json.dumps(data)
         return self.s3.put_object(Bucket=bucket,
                                   Key=keyname,
                                   Body=data,
                                   SSECustomerKey=secret,
                                   SSECustomerAlgorithm='AES256')
 
     def s3_read_dir(self, prefix):
```

### Comparing `dcicutils-7.4.1/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.2/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/secrets_utils.py` & `dcicutils-7.4.2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/snapshot_utils.py` & `dcicutils-7.4.2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.2/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/task_utils.py` & `dcicutils-7.4.2/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/dcicutils/trace_utils.py` & `dcicutils-7.4.2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.1/pyproject.toml` & `dcicutils-7.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.1"
+version = "7.4.2"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.1/setup.py` & `dcicutils-7.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.1',
+    'version': '7.4.2',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.1/PKG-INFO` & `dcicutils-7.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.1
+Version: 7.4.2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

