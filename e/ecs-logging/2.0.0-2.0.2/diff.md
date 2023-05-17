# Comparing `tmp/ecs-logging-2.0.0.tar.gz` & `tmp/ecs_logging-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs-logging-2.0.0.tar", last modified: Wed May 18 18:51:47 2022, max compression
+gzip compressed data, was "ecs_logging-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ecs-logging-2.0.0.tar` & `ecs_logging-2.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1282 2022-05-18 18:33:33.495325 ecs-logging-2.0.0/README.md
--rw-r--r--   0        0        0     1057 2022-05-18 18:34:09.556529 ecs-logging-2.0.0/ecs_logging/__init__.py
--rw-r--r--   0        0        0      795 2022-05-18 18:32:38.841008 ecs-logging-2.0.0/ecs_logging/_meta.py
--rw-r--r--   0        0        0    11540 2022-05-18 18:45:06.452102 ecs-logging-2.0.0/ecs_logging/_stdlib.py
--rw-r--r--   0        0        0     1974 2022-05-18 18:32:38.841568 ecs-logging-2.0.0/ecs_logging/_structlog.py
--rw-r--r--   0        0        0     5998 2022-05-18 18:33:33.496125 ecs-logging-2.0.0/ecs_logging/_utils.py
--rw-r--r--   0        0        0        0 2022-05-18 18:32:38.841927 ecs-logging-2.0.0/ecs_logging/py.typed
--rw-r--r--   0        0        0     1416 2022-05-18 18:33:33.496663 ecs-logging-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      247 1970-01-01 00:00:00.000000 ecs-logging-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1239 2023-05-17 17:18:59.006825 ecs_logging-2.0.2/README.md
+-rw-r--r--   0        0        0     1057 2023-05-17 17:19:16.691964 ecs_logging-2.0.2/ecs_logging/__init__.py
+-rw-r--r--   0        0        0      795 2022-05-18 18:32:38.841008 ecs_logging-2.0.2/ecs_logging/_meta.py
+-rw-r--r--   0        0        0    11540 2023-05-17 17:18:59.009023 ecs_logging-2.0.2/ecs_logging/_stdlib.py
+-rw-r--r--   0        0        0     1974 2022-05-18 18:32:38.841568 ecs_logging-2.0.2/ecs_logging/_structlog.py
+-rw-r--r--   0        0        0     5998 2023-05-17 17:18:59.009748 ecs_logging-2.0.2/ecs_logging/_utils.py
+-rw-r--r--   0        0        0        0 2022-05-18 18:32:38.841927 ecs_logging-2.0.2/ecs_logging/py.typed
+-rw-r--r--   0        0        0     1375 2023-05-17 17:18:59.010998 ecs_logging-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 ecs_logging-2.0.2/PKG-INFO
```

### Comparing `ecs-logging-2.0.0/README.md` & `ecs_logging-2.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ecs-logging-python
 
-[![Build Status](https://apm-ci.elastic.co/job/apm-agent-python/job/ecs-logging-python-mbp/job/main/badge/icon)](https://apm-ci.elastic.co/blue/organizations/jenkins/apm-agent-python%2Fecs-logging-python-mbp/branches)
+[![Build Status](https://github.com/elastic/ecs-logging-python/actions/workflows/test.yml/badge.svg)](https://github.com/elastic/ecs-logging-pythonactions/workflows/test.yml)
 [![PyPI](https://img.shields.io/pypi/v/ecs-logging)](https://pypi.org/project/ecs-logging)
 [![Versions Supported](https://img.shields.io/pypi/pyversions/ecs-logging)](https://pypi.org/project/ecs-logging)
 
 Check out the [Elastic Common Schema (ECS) reference](https://www.elastic.co/guide/en/ecs/current/index.html)
 for more information.
 
 The library currently implements ECS 1.6.
```

### Comparing `ecs-logging-2.0.0/ecs_logging/__init__.py` & `ecs_logging-2.0.2/ecs_logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 # under the License.
 """Logging formatters for ECS (Elastic Common Schema) in Python"""
 
 from ._meta import ECS_VERSION
 from ._stdlib import StdlibFormatter
 from ._structlog import StructlogFormatter
 
-__version__ = "2.0.0"
+__version__ = "2.0.2"
 __all__ = [
     "ECS_VERSION",
     "StdlibFormatter",
     "StructlogFormatter",
 ]
```

### Comparing `ecs-logging-2.0.0/ecs_logging/_meta.py` & `ecs_logging-2.0.2/ecs_logging/_meta.py`

 * *Files identical despite different names*

### Comparing `ecs-logging-2.0.0/ecs_logging/_stdlib.py` & `ecs_logging-2.0.2/ecs_logging/_stdlib.py`

 * *Files identical despite different names*

### Comparing `ecs-logging-2.0.0/ecs_logging/_structlog.py` & `ecs_logging-2.0.2/ecs_logging/_structlog.py`

 * *Files identical despite different names*

### Comparing `ecs-logging-2.0.0/ecs_logging/_utils.py` & `ecs_logging-2.0.2/ecs_logging/_utils.py`

 * *Files identical despite different names*

### Comparing `ecs-logging-2.0.0/pyproject.toml` & `ecs_logging-2.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
-requires = ["flit_core >=2,<3"]
+requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 dist-name = "ecs-logging"
 module = "ecs_logging"
 description-file = "README.md"
 author = "Seth Michael Larson"
 author-email = "seth.larson@elastic.co"
 home-page = "https://github.com/elastic/ecs-logging-python"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
-  "Programming Language :: Python :: 2",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: System :: Logging",
```

