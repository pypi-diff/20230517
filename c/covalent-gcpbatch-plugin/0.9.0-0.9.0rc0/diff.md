# Comparing `tmp/covalent-gcpbatch-plugin-0.9.0.tar.gz` & `tmp/covalent-gcpbatch-plugin-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-gcpbatch-plugin-0.9.0.tar", last modified: Wed May 17 01:05:22 2023, max compression
+gzip compressed data, was "covalent-gcpbatch-plugin-0.9.0rc0.tar", last modified: Wed May 17 00:39:22 2023, max compression
```

## Comparing `covalent-gcpbatch-plugin-0.9.0.tar` & `covalent-gcpbatch-plugin-0.9.0rc0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 01:05:22.446144 covalent-gcpbatch-plugin-0.9.0/
--rw-r--r--   0 will      (1000) will      (1000)    34523 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/LICENSE
--rw-r--r--   0 will      (1000) will      (1000)      211 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/MANIFEST.in
--rw-r--r--   0 will      (1000) will      (1000)     6325 2023-05-17 01:05:22.446144 covalent-gcpbatch-plugin-0.9.0/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)     4987 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/README.md
--rw-r--r--   0 will      (1000) will      (1000)        5 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/VERSION
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 01:05:22.445144 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/
--rw-r--r--   0 will      (1000) will      (1000)      875 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/__init__.py
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 01:05:22.445144 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 01:05:22.446144 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/infra/
--rw-r--r--   0 will      (1000) will      (1000)     3754 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/infra/main.tf
--rw-r--r--   0 will      (1000) will      (1000)     1443 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/infra/outputs.tf
--rw-r--r--   0 will      (1000) will      (1000)     1627 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/infra/variables.tf
--rw-r--r--   0 will      (1000) will      (1000)     3086 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/exec.py
--rw-r--r--   0 will      (1000) will      (1000)    22050 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/gcpbatch.py
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 01:05:22.446144 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)     6325 2023-05-17 01:05:22.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)      699 2023-05-17 01:05:22.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-17 01:05:22.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)       82 2023-05-17 01:05:22.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/entry_points.txt
--rw-r--r--   0 will      (1000) will      (1000)       75 2023-05-17 01:05:22.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/requires.txt
--rw-r--r--   0 will      (1000) will      (1000)       31 2023-05-17 01:05:22.000000 covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/top_level.txt
--rw-r--r--   0 will      (1000) will      (1000)     1238 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/pyproject.toml
--rw-r--r--   0 will      (1000) will      (1000)      968 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/requirements.txt
--rw-r--r--   0 will      (1000) will      (1000)       38 2023-05-17 01:05:22.446144 covalent-gcpbatch-plugin-0.9.0/setup.cfg
--rw-r--r--   0 will      (1000) will      (1000)     2953 2023-05-17 00:27:37.000000 covalent-gcpbatch-plugin-0.9.0/setup.py
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 01:05:22.446144 covalent-gcpbatch-plugin-0.9.0/tests/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/tests/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     3240 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/tests/gcpbatch_exec_test.py
--rw-r--r--   0 will      (1000) will      (1000)    24766 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0/tests/gcpbatch_executor_test.py
+drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 00:39:22.009761 covalent-gcpbatch-plugin-0.9.0rc0/
+-rw-r--r--   0 will      (1000) will      (1000)    34523 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/LICENSE
+-rw-r--r--   0 will      (1000) will      (1000)      211 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/MANIFEST.in
+-rw-r--r--   0 will      (1000) will      (1000)     6328 2023-05-17 00:39:22.009761 covalent-gcpbatch-plugin-0.9.0rc0/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)     4987 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/README.md
+-rw-r--r--   0 will      (1000) will      (1000)        5 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/VERSION
+drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 00:39:22.008761 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/
+-rw-r--r--   0 will      (1000) will      (1000)      875 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/__init__.py
+drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 00:39:22.008761 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/
+drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 00:39:22.009761 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/infra/
+-rw-r--r--   0 will      (1000) will      (1000)     3754 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/infra/main.tf
+-rw-r--r--   0 will      (1000) will      (1000)     1443 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/infra/outputs.tf
+-rw-r--r--   0 will      (1000) will      (1000)     1627 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/infra/variables.tf
+-rw-r--r--   0 will      (1000) will      (1000)     3086 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/exec.py
+-rw-r--r--   0 will      (1000) will      (1000)    22050 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/gcpbatch.py
+drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 00:39:22.009761 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/
+-rw-r--r--   0 will      (1000) will      (1000)     6328 2023-05-17 00:39:21.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)      699 2023-05-17 00:39:21.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-17 00:39:21.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 will      (1000) will      (1000)       82 2023-05-17 00:39:21.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 will      (1000) will      (1000)       75 2023-05-17 00:39:21.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/requires.txt
+-rw-r--r--   0 will      (1000) will      (1000)       31 2023-05-17 00:39:21.000000 covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/top_level.txt
+-rw-r--r--   0 will      (1000) will      (1000)     1238 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/pyproject.toml
+-rw-r--r--   0 will      (1000) will      (1000)      968 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/requirements.txt
+-rw-r--r--   0 will      (1000) will      (1000)       41 2023-05-17 00:39:22.009761 covalent-gcpbatch-plugin-0.9.0rc0/setup.cfg
+-rw-r--r--   0 will      (1000) will      (1000)     2953 2023-05-17 00:27:37.000000 covalent-gcpbatch-plugin-0.9.0rc0/setup.py
+drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-05-17 00:39:22.009761 covalent-gcpbatch-plugin-0.9.0rc0/tests/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/tests/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     3240 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/tests/gcpbatch_exec_test.py
+-rw-r--r--   0 will      (1000) will      (1000)    24766 2023-05-17 00:10:29.000000 covalent-gcpbatch-plugin-0.9.0rc0/tests/gcpbatch_executor_test.py
```

### Comparing `covalent-gcpbatch-plugin-0.9.0/LICENSE` & `covalent-gcpbatch-plugin-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/PKG-INFO` & `covalent-gcpbatch-plugin-0.9.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-gcpbatch-plugin
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: Covalent GCP Batch Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-gcpbatch-plugin
 Download-URL: https://github.com/AgnostiqHQ/covalent-gcpbatch-plugin/archive/v0.9.0.tar.gz
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
```

### Comparing `covalent-gcpbatch-plugin-0.9.0/README.md` & `covalent-gcpbatch-plugin-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/__init__.py` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/infra/main.tf` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/infra/main.tf`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/infra/outputs.tf` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/infra/outputs.tf`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/assets/infra/variables.tf` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/assets/infra/variables.tf`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/exec.py` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/exec.py`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin/gcpbatch.py` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin/gcpbatch.py`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/PKG-INFO` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-gcpbatch-plugin
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: Covalent GCP Batch Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-gcpbatch-plugin
 Download-URL: https://github.com/AgnostiqHQ/covalent-gcpbatch-plugin/archive/v0.9.0.tar.gz
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
```

### Comparing `covalent-gcpbatch-plugin-0.9.0/covalent_gcpbatch_plugin.egg-info/SOURCES.txt` & `covalent-gcpbatch-plugin-0.9.0rc0/covalent_gcpbatch_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/pyproject.toml` & `covalent-gcpbatch-plugin-0.9.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/requirements.txt` & `covalent-gcpbatch-plugin-0.9.0rc0/requirements.txt`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/setup.py` & `covalent-gcpbatch-plugin-0.9.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/tests/gcpbatch_exec_test.py` & `covalent-gcpbatch-plugin-0.9.0rc0/tests/gcpbatch_exec_test.py`

 * *Files identical despite different names*

### Comparing `covalent-gcpbatch-plugin-0.9.0/tests/gcpbatch_executor_test.py` & `covalent-gcpbatch-plugin-0.9.0rc0/tests/gcpbatch_executor_test.py`

 * *Files identical despite different names*

