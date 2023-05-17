# Comparing `tmp/config_patterns-0.4.1.tar.gz` & `tmp/config_patterns-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_patterns-0.4.1.tar", last modified: Fri May 12 18:21:35 2023, max compression
+gzip compressed data, was "config_patterns-1.0.1.tar", last modified: Wed May 17 15:54:57 2023, max compression
```

## Comparing `config_patterns-0.4.1.tar` & `config_patterns-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.070524 config_patterns-0.4.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 01:08:10.000000 config_patterns-0.4.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-12 01:08:10.000000 config_patterns-0.4.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-12 01:08:10.000000 config_patterns-0.4.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-12 18:21:35.070383 config_patterns-0.4.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2892 2023-05-12 01:08:10.000000 config_patterns-0.4.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.067404 config_patterns-0.4.1/config_patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)      303 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 18:21:00.000000 config_patterns-0.4.1/config_patterns/_version.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068493 config_patterns-0.4.1/config_patterns/aws/
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/aws/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5169 2023-05-12 16:38:32.000000 config_patterns-0.4.1/config_patterns/aws/s3.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2792 2023-05-12 16:35:47.000000 config_patterns-0.4.1/config_patterns/aws/ssm.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068601 config_patterns-0.4.1/config_patterns/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/jsonutils.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      182 2023-05-12 03:09:13.000000 config_patterns-0.4.1/config_patterns/logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      724 2023-05-12 03:09:31.000000 config_patterns-0.4.1/config_patterns/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068829 config_patterns-0.4.1/config_patterns/patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/patterns/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    22411 2023-05-12 18:09:09.000000 config_patterns-0.4.1/config_patterns/patterns/multi_env_json.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.069308 config_patterns-0.4.1/config_patterns/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      149 2023-05-12 03:10:02.000000 config_patterns-0.4.1/config_patterns/tests/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1216 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.069769 config_patterns-0.4.1/config_patterns/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 15:37:26.000000 config_patterns-0.4.1/config_patterns/vendor/nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    44420 2023-05-12 01:08:10.000000 config_patterns-0.4.1/config_patterns/vendor/strutils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.068043 config_patterns-0.4.1/config_patterns.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      960 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      438 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-12 18:21:35.000000 config_patterns-0.4.1/config_patterns.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2126 2023-05-12 18:20:49.000000 config_patterns-0.4.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)       73 2023-05-12 18:03:12.000000 config_patterns-0.4.1/requirements-aws.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-12 01:08:10.000000 config_patterns-0.4.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-12 01:08:10.000000 config_patterns-0.4.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-12 16:53:20.000000 config_patterns-0.4.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       65 2023-05-12 01:08:10.000000 config_patterns-0.4.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 18:21:35.070567 config_patterns-0.4.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7961 2023-05-12 01:08:10.000000 config_patterns-0.4.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:21:35.070101 config_patterns-0.4.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      258 2023-05-12 01:08:10.000000 config_patterns-0.4.1/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.189868 config_patterns-1.0.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 01:08:10.000000 config_patterns-1.0.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-12 01:08:10.000000 config_patterns-1.0.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-12 01:08:10.000000 config_patterns-1.0.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-17 15:54:57.189713 config_patterns-1.0.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2892 2023-05-12 01:08:10.000000 config_patterns-1.0.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.184085 config_patterns-1.0.1/config_patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      303 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-17 15:54:41.000000 config_patterns-1.0.1/config_patterns/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.185615 config_patterns-1.0.1/config_patterns/aws/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/aws/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5169 2023-05-12 16:38:32.000000 config_patterns-1.0.1/config_patterns/aws/s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2792 2023-05-12 16:35:47.000000 config_patterns-1.0.1/config_patterns/aws/ssm.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.185883 config_patterns-1.0.1/config_patterns/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-05-17 07:06:41.000000 config_patterns-1.0.1/config_patterns/jsonutils.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      182 2023-05-12 03:09:13.000000 config_patterns-1.0.1/config_patterns/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      724 2023-05-12 03:09:31.000000 config_patterns-1.0.1/config_patterns/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.186513 config_patterns-1.0.1/config_patterns/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4585 2023-05-17 07:06:29.000000 config_patterns-1.0.1/config_patterns/patterns/hierarchy.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3213 2023-05-17 07:29:04.000000 config_patterns-1.0.1/config_patterns/patterns/merge_key_value.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.187104 config_patterns-1.0.1/config_patterns/patterns/multi_env_json/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-05-17 14:16:39.000000 config_patterns-1.0.1/config_patterns/patterns/multi_env_json/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    23831 2023-05-17 15:47:41.000000 config_patterns-1.0.1/config_patterns/patterns/multi_env_json/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.187943 config_patterns-1.0.1/config_patterns/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      149 2023-05-12 03:10:02.000000 config_patterns-1.0.1/config_patterns/tests/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1216 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.189082 config_patterns-1.0.1/config_patterns/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-17 15:41:42.000000 config_patterns-1.0.1/config_patterns/vendor/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 15:37:26.000000 config_patterns-1.0.1/config_patterns/vendor/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    44420 2023-05-12 01:08:10.000000 config_patterns-1.0.1/config_patterns/vendor/strutils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.184805 config_patterns-1.0.1/config_patterns.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4016 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1137 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      438 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-17 15:54:57.000000 config_patterns-1.0.1/config_patterns.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2912 2023-05-17 15:41:07.000000 config_patterns-1.0.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)       73 2023-05-12 18:03:12.000000 config_patterns-1.0.1/requirements-aws.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-12 01:08:10.000000 config_patterns-1.0.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-12 01:08:10.000000 config_patterns-1.0.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-12 16:53:20.000000 config_patterns-1.0.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       65 2023-05-12 01:08:10.000000 config_patterns-1.0.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-17 15:54:57.189912 config_patterns-1.0.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7961 2023-05-12 01:08:10.000000 config_patterns-1.0.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-17 15:54:57.189411 config_patterns-1.0.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      258 2023-05-12 01:08:10.000000 config_patterns-1.0.1/tests/test_import.py
```

### Comparing `config_patterns-0.4.1/LICENSE.txt` & `config_patterns-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/PKG-INFO` & `config_patterns-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: config_patterns
-Version: 0.4.1
+Version: 1.0.1
 Summary: Implement common config management patterns.
 Home-page: https://github.com/MacHu-GWU/config_patterns-project
-Download-URL: https://pypi.python.org/pypi/config_patterns/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/config_patterns/1.0.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `config_patterns-0.4.1/README.rst` & `config_patterns-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns/aws/s3.py` & `config_patterns-1.0.1/config_patterns/aws/s3.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns/aws/ssm.py` & `config_patterns-1.0.1/config_patterns/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns/jsonutils.py` & `config_patterns-1.0.1/config_patterns/jsonutils.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns/paths.py` & `config_patterns-1.0.1/config_patterns/paths.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns/patterns/multi_env_json.py` & `config_patterns-1.0.1/config_patterns/patterns/multi_env_json/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,37 @@
 import typing as T
 import copy
 import enum
 import string
 import dataclasses
 from pathlib import Path
 
-#
+# import optional dependencies
 try:
     import boto3
     import boto_session_manager
 except ImportError:  # pragma: no cover
     pass
 
-#
 try:
     import pysecret
     import aws_console_url
 
-    from ..aws.ssm import deploy_parameter, delete_parameter
-    from ..aws.s3 import deploy_config, delete_config, S3Object
+    from ...aws.ssm import deploy_parameter, delete_parameter
+    from ...aws.s3 import deploy_config, delete_config, S3Object
 except ImportError:  # pragma: no cover
     pass
 
-from ..logger import logger
-from ..jsonutils import json_loads
-from ..compat import cached_property
-from ..vendor.strutils import camel2under, slugify
+from ...logger import logger
+from ...jsonutils import json_loads
+from ...compat import cached_property
+from ...vendor.strutils import slugify
+from ...vendor.better_enum import BetterStrEnum
+from ..hierarchy import apply_shared_value
+from ..merge_key_value import merge_key_value
 
 
 def validate_project_name(project_name: str):
     if project_name[0] not in string.ascii_lowercase:
         raise ValueError("first letter of project_name has to be a-z!")
     if project_name[-1] not in (string.ascii_lowercase + string.digits):
         raise ValueError("last letter of project_name has to be a-z, 0-9!")
@@ -42,31 +44,24 @@
 def validate_env_name(env_name: str):
     if env_name[0] not in string.ascii_lowercase:
         raise ValueError("first letter of env_name has to be a-z!")
     if len(set(env_name).difference(string.ascii_lowercase + string.digits)):
         raise ValueError("env_name can only has a-z, 0-9")
 
 
-class BaseEnvEnum(str, enum.Enum):
+class BaseEnvEnum(BetterStrEnum):
     """
     Base per environment enumeration base class.
 
     an environment name is a string that is full lowercase, can include
     letters and digits, start with letter, no delimiter.
     Valid examples are: dev, test, prod, stage1, stage2,
     Invalid examples are: my_dev, 1dev
     """
 
-    @classmethod
-    def ensure_str(cls, value: T.Union[str, "BaseEnvEnum"]) -> str:
-        if isinstance(value, cls):
-            return value.value
-        else:
-            return value
-
 
 def normalize_parameter_name(param_name: str) -> str:
     """
     AWS has limitation that the name cannot be prefixed with "aws" or "ssm",
     so this method will automatically add prepend character to the name.
 
     Ref:
@@ -117,14 +112,27 @@
         """
         User should not overwrite this method. You can use __user_post_init__
         for any post init logics.
         """
         self._validate()
         self.__user_post_init__()
 
+    @classmethod
+    def from_dict(cls, data: dict):  # pragma: no cover
+        """
+        Create an instance from a dict.
+        """
+        raise NotImplementedError(
+            "Implement this method create an instance of "
+            "env config. For example:\n"
+            "@classmethod\n"
+            "def from_dict(cls, data: dict):\n"
+            "    return cls(**data)\n"
+        )
+
     @cached_property
     def project_name_slug(self) -> str:
         """
         Example: "my-project"
         """
         return slugify(self.project_name, delim="-")
 
@@ -297,68 +305,78 @@
 
     :param data: Nonsensitive config data.
     :param secret_data: Sensitive config data.
 
     Example data and secret_data::
 
         >>> {
-        ...     "shared": {
+        ...     "_shared": {
         ...         "project_name": "my_project", # has to have a key called ``project_name``
         ...         "key": "value",
         ...         ...
         ...     },
-        ...     "envs": {
-        ...         "dev": {
-        ...             "key": "value",
-        ...             ...
-        ...         },
-        ...         "int": {
-        ...             "key": "value",
-        ...             ...
-        ...         },
-        ...         "prod": {
-        ...             "key": "value",
-        ...             ...
-        ...         },
+        ...     "dev": {
+        ...         "key": "value",
         ...         ...
-        ...     }
+        ...     },
+        ...     "int": {
+        ...         "key": "value",
+        ...         ...
+        ...     },
+        ...     "prod": {
+        ...         "key": "value",
+        ...         ...
+        ...     },
+        ...     ...
         ... }
     """
 
     data: dict = dataclasses.field()
     secret_data: dict = dataclasses.field()
 
     Env: T.Type[BaseEnv] = dataclasses.field()
     EnvEnum: T.Type[BaseEnvEnum] = dataclasses.field()
 
+    _applied_data: dict = dataclasses.field(init=False)
+    _applied_secret_data: dict = dataclasses.field(init=False)
+    _merged: dict = dataclasses.field(init=False)
+
     def _validate(self):
         """
         Validate input arguments.
         """
         validate_project_name(self.project_name)
-        for env_name in self.data["envs"]:
-            validate_env_name(env_name)
+        for env_name in self.data:
+            if env_name != "_shared":
+                validate_env_name(env_name)
+
+    def _apply_shared(self):
+        self._applied_data = copy.deepcopy(self.data)
+        self._applied_secret_data = copy.deepcopy(self.secret_data)
+        apply_shared_value(self._applied_data)
+        apply_shared_value(self._applied_secret_data)
+        self._merged = merge_key_value(self._applied_data, self._applied_secret_data)
 
     def __user_post_init__(self):
         """
         A placeholder post init function for user.
         """
-        pass
 
     def __post_init__(self):
         """
         User should not overwrite this method. You can use __user_post_init__
         for any post init logics.
         """
         self._validate()
+        self._apply_shared()
         self.__user_post_init__()
 
     @cached_property
     def project_name(self) -> str:
-        return self.data["shared"]["project_name"]
+        return self.data["_shared"]["*.project_name"]
 
     @cached_property
     def project_name_slug(self) -> str:
         return slugify(self.project_name, delim="-")
 
     @cached_property
     def project_name_snake(self) -> str:
@@ -373,23 +391,19 @@
         Example: "my_project-dev"
         """
         return normalize_parameter_name(self.project_name_snake)
 
     # don't put type hint for return value, it should return a
     # user defined subclass, which is impossible to predict.
     def get_env(self, env_name: T.Union[str, BaseEnvEnum]):
-        env_name = BaseEnvEnum.ensure_str(env_name)
-        data = dict()
-        data.update(copy.deepcopy(self.data["shared"]))
-        data.update(copy.deepcopy(self.secret_data["shared"]))
-        data.update(copy.deepcopy(self.data["envs"][env_name]))
-        data.update(copy.deepcopy(self.secret_data["envs"][env_name]))
+        env_name = self.EnvEnum.ensure_str(env_name)
+        data = copy.deepcopy(self._merged[env_name])
         data["env_name"] = env_name
         try:
-            return self.Env(**data)
+            return self.Env.from_dict(data)
         except TypeError as e:
             if "got an unexpected keyword argument" in str(e):
                 raise TypeError(
                     f"{e}, please compare your config json file "
                     f"to your config object definition!"
                 )
             else:  # pragma: no cover
@@ -398,27 +412,41 @@
     @classmethod
     def get_current_env(cls) -> str:  # pragma: no cover
         """
         An abstract method that can figure out what is the environment this config
         should deal with. For example, you can define the git feature branch
         will become the dev env; the master branch will become the int env;
         the release branch will become prod env;
+
+        Example::
+
+            class Config(BaseConfig):
+                ...
+
+                @classmethod
+                def get_current_env(cls) -> str:
+                    if "CI" in os.environ:
+                        return EnvEnum.test.value
+                    elif "AWS_LAMBDA_FUNCTION_NAME" in os.environ:
+                        return EnvEnum.prod.value
+                    else:
+                        return EnvEnum.dev.value
         """
         raise NotImplementedError(
             "You have to implement this method to detect what environment "
             "you should use. It should be a class method that take no argument "
             "and returns a string. Usually you could use environment variable to detect "
             "whether you are on your local laptop, CI runtime, remote machine. "
             "Also you can use subprocess to call git CLI to check your current branch."
         )
 
     # don't put type hint for return value, it should return a
     # user defined subclass, which is impossible to predict.
     @cached_property
-    def env(self):
+    def env(self):  # pragma: no cover
         """
         Access the current :class:`Env` object.
         """
         return self.get_env(env_name=self.get_current_env())
 
     @classmethod
     def read(
@@ -521,22 +549,31 @@
         )
 
         # add per env parameter
         for env_name in self.EnvEnum:
             env_name = self.EnvEnum.ensure_str(env_name)
             env = self.get_env(env_name)
             parameter_name = env.parameter_name
+
             parameter_data = {
                 "data": {
-                    "shared": self.data["shared"],
-                    "envs": {env.env_name: self.data["envs"][env.env_name]},
+                    "_shared": {
+                        k: v
+                        for k, v in self.data.get("_shared", {}).items()
+                        if k.startswith("*") or k.startswith(f"{env.env_name}.")
+                    },
+                    env.env_name: self.data[env.env_name],
                 },
                 "secret_data": {
-                    "shared": self.secret_data["shared"],
-                    "envs": {env.env_name: self.secret_data["envs"][env.env_name]},
+                    "_shared": {
+                        k: v
+                        for k, v in self.secret_data.get("_shared", {}).items()
+                        if k.startswith("*") or k.startswith(f"{env.env_name}.")
+                    },
+                    env.env_name: self.secret_data[env.env_name],
                 },
             }
             deployment_list.append(
                 ConfigDeployment(
                     parameter_name=parameter_name,
                     parameter_data=parameter_data,
                     project_name=env.project_name,
```

### Comparing `config_patterns-0.4.1/config_patterns/tests/helper.py` & `config_patterns-1.0.1/config_patterns/tests/helper.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns/vendor/nest_logger.py` & `config_patterns-1.0.1/config_patterns/vendor/nest_logger.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns/vendor/strutils.py` & `config_patterns-1.0.1/config_patterns/vendor/strutils.py`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/config_patterns.egg-info/PKG-INFO` & `config_patterns-1.0.1/config_patterns.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: config-patterns
-Version: 0.4.1
+Version: 1.0.1
 Summary: Implement common config management patterns.
 Home-page: https://github.com/MacHu-GWU/config_patterns-project
-Download-URL: https://pypi.python.org/pypi/config_patterns/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/config_patterns/1.0.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `config_patterns-0.4.1/config_patterns.egg-info/SOURCES.txt` & `config_patterns-1.0.1/config_patterns.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 config_patterns.egg-info/requires.txt
 config_patterns.egg-info/top_level.txt
 config_patterns/aws/__init__.py
 config_patterns/aws/s3.py
 config_patterns/aws/ssm.py
 config_patterns/docs/__init__.py
 config_patterns/patterns/__init__.py
-config_patterns/patterns/multi_env_json.py
+config_patterns/patterns/hierarchy.py
+config_patterns/patterns/merge_key_value.py
+config_patterns/patterns/multi_env_json/__init__.py
+config_patterns/patterns/multi_env_json/impl.py
 config_patterns/tests/__init__.py
 config_patterns/tests/boto_ses.py
 config_patterns/tests/helper.py
 config_patterns/vendor/__init__.py
+config_patterns/vendor/better_enum.py
 config_patterns/vendor/nest_logger.py
 config_patterns/vendor/strutils.py
 tests/test_import.py
```

### Comparing `config_patterns-0.4.1/requirements-doc.txt` & `config_patterns-1.0.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `config_patterns-0.4.1/setup.py` & `config_patterns-1.0.1/setup.py`

 * *Files identical despite different names*

