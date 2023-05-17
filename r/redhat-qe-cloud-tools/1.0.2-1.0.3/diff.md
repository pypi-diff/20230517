# Comparing `tmp/redhat_qe_cloud_tools-1.0.2.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.2.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.3.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.2.tar` & `redhat_qe_cloud_tools-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-03-27 07:49:47.610163 redhat_qe_cloud_tools-1.0.2/LICENSE
--rw-r--r--   0        0        0      845 2023-03-27 07:49:47.610163 redhat_qe_cloud_tools-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-03-27 07:49:47.610163 redhat_qe_cloud_tools-1.0.2/clouds/__init__.py
--rw-r--r--   0        0        0      787 2023-03-27 07:49:47.610163 redhat_qe_cloud_tools-1.0.2/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2023-03-27 07:49:47.610163 redhat_qe_cloud_tools-1.0.2/clouds/aws/__init__.py
--rw-r--r--   0        0        0     1886 2023-03-27 07:49:47.611163 redhat_qe_cloud_tools-1.0.2/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     6191 2023-03-27 07:49:47.611163 redhat_qe_cloud_tools-1.0.2/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0     1807 2023-03-27 07:49:47.611163 redhat_qe_cloud_tools-1.0.2/clouds/logger.py
--rw-r--r--   0        0        0      757 2023-03-27 07:49:47.611163 redhat_qe_cloud_tools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/LICENSE
+-rw-r--r--   0        0        0      845 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/__init__.py
+-rw-r--r--   0        0        0      455 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_roles/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_roles/__init__.py
+-rw-r--r--   0        0        0     1591 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_roles/aws_roles.py
+-rw-r--r--   0        0        0     1893 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     6218 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      782 2023-05-17 11:51:42.829928 redhat_qe_cloud_tools-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.3/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.2/LICENSE` & `redhat_qe_cloud_tools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.2/README.md` & `redhat_qe_cloud_tools-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.2/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.3/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.2/clouds/aws/aws_utils.py` & `redhat_qe_cloud_tools-1.0.3/clouds/aws/aws_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from configparser import ConfigParser, NoOptionError, NoSectionError
 
-from clouds.logger import get_logger
+from simple_logger.logger import get_logger
 
 LOGGER = get_logger(name=__name__)
 
 
 class AWSConfigurationError(Exception):
     pass
```

### Comparing `redhat_qe_cloud_tools-1.0.2/clouds/aws/delete_s3_velero_bucket.py` & `redhat_qe_cloud_tools-1.0.3/clouds/aws/delete_s3_velero_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
-import logging
 import os
 import re
 import sys
 from http import HTTPStatus
 from typing import Union
 
 import boto3
 import click
+from simple_logger.logger import get_logger
 
-LOGGER = logging.getLogger(__name__)
+LOGGER = get_logger(name=__name__)
 
 
 def delete_velero_cluster_buckets(cluster, boto_client) -> None:
     """
     Delete the velero bucket associated with a cluster
 
     Args:
```

### Comparing `redhat_qe_cloud_tools-1.0.2/pyproject.toml` & `redhat_qe_cloud_tools-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "redhat-qe-cloud-tools"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python utilities to manage cloud services, such as AWS."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/cloud-tools"
 packages = [{include = "clouds"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 colorlog = "*"
 boto3 = "*"
 click = "*"
 configparser = "*"
+python-simple-logger="*"
 
 [tool.poetry.dev-dependencies]
 ipython = "*"
 ipdb = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `redhat_qe_cloud_tools-1.0.2/PKG-INFO` & `redhat_qe_cloud_tools-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
 Author: Meni Yakove
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3
 Requires-Dist: click
 Requires-Dist: colorlog
 Requires-Dist: configparser
+Requires-Dist: python-simple-logger
 Project-URL: Repository, https://github.com/RedHatQE/cloud-tools
 Description-Content-Type: text/markdown
 
 # cloud-tools
 Python utilities to manage cloud services, such as AWS.
 
 ## Local run
```

