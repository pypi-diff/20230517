# Comparing `tmp/pix_framework-0.7.1.tar.gz` & `tmp/pix_framework-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.7.1.tar", max compression
+gzip compressed data, was "pix_framework-0.8.0.tar", max compression
```

## Comparing `pix_framework-0.7.1.tar` & `pix_framework-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-05-05 16:18:53.563943 pix_framework-0.7.1/LICENSE
--rw-r--r--   0        0        0      549 2023-05-05 16:18:53.563943 pix_framework-0.7.1/README.md
--rw-r--r--   0        0        0      744 2023-05-05 16:18:53.563943 pix_framework-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       57 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0    11236 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/calendar/resource_calendar.py
--rw-r--r--   0        0        0        0 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/enhancement/__init__.py
--rw-r--r--   0        0        0     5444 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/enhancement/multitasking.py
--rw-r--r--   0        0        0       27 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/input.py
--rw-r--r--   0        0        0     2058 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      970 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 pix_framework-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 13:40:44.215619 pix_framework-0.8.0/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-17 13:40:44.215619 pix_framework-0.8.0/README.md
+-rw-r--r--   0        0        0      744 2023-05-17 13:40:44.215619 pix_framework-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0    11236 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/calendar/resource_calendar.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/discovery/__init__.py
+-rw-r--r--   0        0        0     4903 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/discovery/gateway_probabilities.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5444 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2498 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/input.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/io/__init__.py
+-rw-r--r--   0        0        0    38314 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/io/bpm_graph.py
+-rw-r--r--   0        0        0     2058 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4414 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 pix_framework-0.8.0/PKG-INFO
```

### Comparing `pix_framework-0.7.1/LICENSE` & `pix_framework-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/README.md` & `pix_framework-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/pyproject.toml` & `pix_framework-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.7.1"
+version = "0.8.0"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>", "Ihar Suvorau <ihar.suvorau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "pix_framework", from = "src" },
 ]
```

### Comparing `pix_framework-0.7.1/src/pix_framework/calendar/resource_calendar.py` & `pix_framework-0.8.0/src/pix_framework/calendar/resource_calendar.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/src/pix_framework/enhancement/multitasking.py` & `pix_framework-0.8.0/src/pix_framework/enhancement/multitasking.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.8.0/src/pix_framework/filesystem/file_manager.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/src/pix_framework/input.py` & `pix_framework-0.8.0/src/pix_framework/input.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/src/pix_framework/log_ids.py` & `pix_framework-0.8.0/src/pix_framework/log_ids.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/src/pix_framework/log_split/log_split.py` & `pix_framework-0.8.0/src/pix_framework/log_split/log_split.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/src/pix_framework/statistics/distribution.py` & `pix_framework-0.8.0/src/pix_framework/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/src/pix_framework/statistics/utils.py` & `pix_framework-0.8.0/src/pix_framework/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.1/PKG-INFO` & `pix_framework-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.7.1
+Version: 0.8.0
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

