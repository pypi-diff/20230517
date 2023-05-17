# Comparing `tmp/kedro-prefect-oliver-0.1.4.tar.gz` & `tmp/kedro-prefect-oliver-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-prefect-oliver-0.1.4.tar", last modified: Wed May 17 15:41:28 2023, max compression
+gzip compressed data, was "kedro-prefect-oliver-0.1.5.tar", last modified: Wed May 17 16:07:03 2023, max compression
```

## Comparing `kedro-prefect-oliver-0.1.4.tar` & `kedro-prefect-oliver-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.683102 kedro-prefect-oliver-0.1.4/
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     1140 2023-03-14 19:43:11.000000 kedro-prefect-oliver-0.1.4/LICENSE
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      577 2023-05-17 15:41:28.682985 kedro-prefect-oliver-0.1.4/PKG-INFO
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     4582 2023-03-14 19:43:11.000000 kedro-prefect-oliver-0.1.4/README
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     5684 2023-05-17 15:39:45.000000 kedro-prefect-oliver-0.1.4/pyproject.toml
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)       38 2023-05-17 15:41:28.683141 kedro-prefect-oliver-0.1.4/setup.cfg
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.680661 kedro-prefect-oliver-0.1.4/src/
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.682129 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      122 2023-03-24 12:46:02.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/__init__.py
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)     2068 2023-03-24 12:46:03.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/infrastructure.py
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)    13643 2023-05-17 15:32:07.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/register.py
-drwxr-xr-x   0 juandavidbarreto   (502) staff       (20)        0 2023-05-17 15:41:28.682834 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      577 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/PKG-INFO
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      385 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/SOURCES.txt
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)        1 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/dependency_links.txt
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)      366 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/requires.txt
--rw-r--r--   0 juandavidbarreto   (502) staff       (20)       21 2023-05-17 15:41:28.000000 kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4582 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/README
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/infrastructure.py
+-rw-rw-rw-   0 root         (0) root         (0)    13691 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/register.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-17 16:07:03.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/top_level.txt
```

### Comparing `kedro-prefect-oliver-0.1.4/LICENSE` & `kedro-prefect-oliver-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.4/PKG-INFO` & `kedro-prefect-oliver-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.4
+Version: 0.1.5
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kedro-prefect-oliver-0.1.4/README` & `kedro-prefect-oliver-0.1.5/README`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.4/pyproject.toml` & `kedro-prefect-oliver-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "kedro-prefect-oliver"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     {name = "Oliver OTL", email = "dev@olivetreeholdings.com"},
 ]
 description = "Kedro-Prefect integration library"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/infrastructure.py` & `kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/infrastructure.py`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver/register.py` & `kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/register.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,19 @@
         logger.info("Session created with ID %s", session.session_id)
         pipeline = pipelines.get(self.pipeline_name)
         context = session.load_context()
         catalog = context.catalog
         unregistered_ds = pipeline.data_sets() - set(catalog.list())  # NOQA
         for ds_name in unregistered_ds:
             catalog.add(ds_name, MemoryDataSet())
-        return {"catalog": catalog, "sess_id": session.session_id, "hook_manager": session._hook_manager} # NOQA
+        return {
+            "catalog": catalog,
+            "sess_id": session.session_id,
+            "hook_manager": session._hook_manager,
+        }  # NOQA
 
 
 class KedroTask(object):
     """Kedro node as a Prefect task."""
 
     def __init__(self, node: Node, name: str = None):
         self._node = node
```

### Comparing `kedro-prefect-oliver-0.1.4/src/kedro_prefect_oliver.egg-info/PKG-INFO` & `kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.4
+Version: 0.1.5
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

