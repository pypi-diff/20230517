# Comparing `tmp/airflow-provider-vdk-0.0.758850982.tar.gz` & `tmp/airflow-provider-vdk-0.0.870487610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow-provider-vdk-0.0.758850982.tar", last modified: Thu Jan 26 22:52:23 2023, max compression
+gzip compressed data, was "dist/airflow-provider-vdk-0.0.870487610.tar", last modified: Wed May 17 14:55:33 2023, max compression
```

## Comparing `airflow-provider-vdk-0.0.758850982.tar` & `airflow-provider-vdk-0.0.870487610.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/
--rw-rw-rw-   0 root         (0) root         (0)     9283 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1939 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1939 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-01-26 22:52:13.000000 airflow-provider-vdk-0.0.758850982/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/hooks/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9691 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/hooks/vdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/operators/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2492 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/operators/vdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 22:52:23.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/sensors/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3292 2023-01-26 22:52:04.000000 airflow-provider-vdk-0.0.758850982/vdk_provider/sensors/vdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/
+-rw-rw-rw-   0 root         (0) root         (0)     9283 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-05-17 14:55:21.000000 airflow-provider-vdk-0.0.870487610/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9696 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/hooks/vdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/operators/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/operators/vdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:55:33.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3297 2023-05-17 14:55:17.000000 airflow-provider-vdk-0.0.870487610/vdk_provider/sensors/vdk.py
```

### Comparing `airflow-provider-vdk-0.0.758850982/LICENSE` & `airflow-provider-vdk-0.0.870487610/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-vdk-0.0.758850982/PKG-INFO` & `airflow-provider-vdk-0.0.870487610/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-vdk
-Version: 0.0.758850982
+Version: 0.0.870487610
 Summary: Airflow provider for Versatile Data Kit.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: Versatile Data Kit Development Team
 Author-email: versatile-data-kit@vmware.com
 License: Apache License 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `airflow-provider-vdk-0.0.758850982/README.md` & `airflow-provider-vdk-0.0.870487610/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-vdk-0.0.758850982/airflow_provider_vdk.egg-info/PKG-INFO` & `airflow-provider-vdk-0.0.870487610/airflow_provider_vdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-vdk
-Version: 0.0.758850982
+Version: 0.0.870487610
 Summary: Airflow provider for Versatile Data Kit.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: Versatile Data Kit Development Team
 Author-email: versatile-data-kit@vmware.com
 License: Apache License 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `airflow-provider-vdk-0.0.758850982/setup.py` & `airflow-provider-vdk-0.0.870487610/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from setuptools import setup
 
-__version__ = "0.0.758850982"
+__version__ = "0.0.870487610"
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-provider-vdk",
     version=__version__,
```

### Comparing `airflow-provider-vdk-0.0.758850982/vdk_provider/hooks/vdk.py` & `airflow-provider-vdk-0.0.870487610/vdk_provider/hooks/vdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import os
 import sys
 import time
 import uuid
 from enum import Enum
```

### Comparing `airflow-provider-vdk-0.0.758850982/vdk_provider/operators/vdk.py` & `airflow-provider-vdk-0.0.870487610/vdk_provider/operators/vdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 from airflow.models import BaseOperator
```

### Comparing `airflow-provider-vdk-0.0.758850982/vdk_provider/sensors/vdk.py` & `airflow-provider-vdk-0.0.870487610/vdk_provider/sensors/vdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 from typing import Dict
 
 from airflow.sensors.base import BaseSensorOperator
 from vdk_provider.hooks.vdk import JobStatus
```

