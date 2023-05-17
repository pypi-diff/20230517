# Comparing `tmp/kedro-prefect-oliver-0.1.3.tar.gz` & `tmp/kedro-prefect-oliver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-prefect-oliver-0.1.3.tar", last modified: Wed Apr 12 14:29:02 2023, max compression
+gzip compressed data, was "kedro-prefect-oliver-0.1.4.tar", last modified: Wed May 17 15:41:28 2023, max compression
```

## Comparing `kedro-prefect-oliver-0.1.3.tar` & `kedro-prefect-oliver-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4582 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/README
--rw-rw-rw-   0 root         (0) root         (0)     5684 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/infrastructure.py
--rw-rw-rw-   0 root         (0) root         (0)    13601 2023-04-12 14:28:45.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/register.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 14:29:02.364066 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-12 14:29:02.000000 kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/top_level.txt
+drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.683102 kedro-prefect-oliver-0.1.4/
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)     1140 2023-03-14 19:43:11.000000 kedro-prefect-oliver-0.1.4/LICENSE
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)      577 2023-05-17 15:41:28.682985 kedro-prefect-oliver-0.1.4/PKG-INFO
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)     4582 2023-03-14 19:43:11.000000 kedro-prefect-oliver-0.1.4/README
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)     5684 2023-05-17 15:39:45.000000 kedro-prefect-oliver-0.1.4/pyproject.toml
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)       38 2023-05-17 15:41:28.683141 kedro-prefect-oliver-0.1.4/setup.cfg
+drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.680661 kedro-prefect-oliver-0.1.4/src/
+drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.682129 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)      122 2023-03-24 12:46:02.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/__init__.py
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)     2068 2023-03-24 12:46:03.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/infrastructure.py
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)    13643 2023-05-17 15:32:07.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/register.py
+drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.682834 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)      577 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/PKG-INFO
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)      385 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/SOURCES.txt
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)        1 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/dependency_links.txt
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)      366 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/requires.txt
+-rw-r--r--   0 juandavidbarreto   (502) staff       (20)       21 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/top_level.txt
```

### Comparing `kedro-prefect-oliver-0.1.3/LICENSE` & `kedro-prefect-oliver-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.3/PKG-INFO` & `kedro-prefect-oliver-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.3
+Version: 0.1.4
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kedro-prefect-oliver-0.1.3/README` & `kedro-prefect-oliver-0.1.4/README`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.3/pyproject.toml` & `kedro-prefect-oliver-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "kedro-prefect-oliver"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     {name = "Oliver OTL", email = "dev@olivetreeholdings.com"},
 ]
 description = "Kedro-Prefect integration library"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/infrastructure.py` & `kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/infrastructure.py`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver/register.py` & `kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from typing import Any, Dict, List, Tuple, Union
 
-from kedro.framework.hooks.manager import _create_hook_manager
 from kedro.framework.project import pipelines, find_pipelines
 from kedro.framework.session import KedroSession
 from kedro.framework.startup import bootstrap_project
 from kedro.io import DataCatalog, MemoryDataSet
 from kedro.runner import run_node
 from kedro.pipeline.node import Node
+from pluggy import PluginManager
 
 from prefect.infrastructure.kubernetes import KubernetesJob
 from prefect.task_runners import SequentialTaskRunner
 from prefect import flow, get_run_logger, task
 from prefect.deployments import Deployment
 from prefect.filesystems import GCS
 import prefect
@@ -65,29 +65,29 @@
         logger.info("Session created with ID %s", session.session_id)
         pipeline = pipelines.get(self.pipeline_name)
         context = session.load_context()
         catalog = context.catalog
         unregistered_ds = pipeline.data_sets() - set(catalog.list())  # NOQA
         for ds_name in unregistered_ds:
             catalog.add(ds_name, MemoryDataSet())
-        return {"catalog": catalog, "sess_id": session.session_id}
+        return {"catalog": catalog, "sess_id": session.session_id, "hook_manager": session._hook_manager} # NOQA
 
 
 class KedroTask(object):
     """Kedro node as a Prefect task."""
 
     def __init__(self, node: Node, name: str = None):
         self._node = node
         self.name = name or node.name
 
-    def run(self, task_dict: Dict[str, Union[DataCatalog, str]]):
+    def run(self, task_dict: Dict[str, Union[DataCatalog, str, PluginManager]]) -> None:
         run_node(
             self._node,
             task_dict["catalog"],
-            _create_hook_manager(),
+            task_dict["hook_manager"],
             False,
             task_dict["sess_id"],
         )
 
 
 def instantiate_task(
     node: Node,
```

### Comparing `kedro-prefect-oliver-0.1.3/src/kedro_prefect_oliver.egg-info/PKG-INFO` & `kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.3
+Version: 0.1.4
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

