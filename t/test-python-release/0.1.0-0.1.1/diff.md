# Comparing `tmp/test_python_release-0.1.0.tar.gz` & `tmp/test_python_release-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_python_release-0.1.0.tar", max compression
+gzip compressed data, was "test_python_release-0.1.1.tar", max compression
```

## Comparing `test_python_release-0.1.0.tar` & `test_python_release-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-17 10:25:25.238612 test_python_release-0.1.0/LICENSE
--rw-r--r--   0        0        0       22 2023-05-17 10:25:25.238612 test_python_release-0.1.0/README.md
--rw-r--r--   0        0        0      762 2023-05-17 10:25:58.362577 test_python_release-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/__init__.py
--rw-r--r--   0        0        0    34905 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/check_firewall.py
--rw-r--r--   0        0        0    34296 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/firewall_proxy.py
--rw-r--r--   0        0        0    29922 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/snapshot_compare.py
--rw-r--r--   0        0        0    11729 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/utils.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 test_python_release-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-17 10:28:10.756326 test_python_release-0.1.1/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-17 10:28:10.756326 test_python_release-0.1.1/README.md
+-rw-r--r--   0        0        0      763 2023-05-17 10:28:46.315214 test_python_release-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 10:28:10.756326 test_python_release-0.1.1/test_python_release/__init__.py
+-rw-r--r--   0        0        0    34905 2023-05-17 10:28:10.756326 test_python_release-0.1.1/test_python_release/check_firewall.py
+-rw-r--r--   0        0        0    34296 2023-05-17 10:28:10.756326 test_python_release-0.1.1/test_python_release/firewall_proxy.py
+-rw-r--r--   0        0        0    29922 2023-05-17 10:28:10.756326 test_python_release-0.1.1/test_python_release/snapshot_compare.py
+-rw-r--r--   0        0        0    11729 2023-05-17 10:28:10.756326 test_python_release-0.1.1/test_python_release/utils.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 test_python_release-0.1.1/PKG-INFO
```

### Comparing `test_python_release-0.1.0/LICENSE` & `test_python_release-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `test_python_release-0.1.0/pyproject.toml` & `test_python_release-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-python-release"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["FoSIX"]
 readme = "README.md"
 packages = [
     { include = "test_python_release" }
 ]
 classifiers = [
@@ -25,8 +25,8 @@
 
 [tool.poetry.group.dev.dependencies]
 pydoc-markdown = "^4.6"
 python-semantic-release = "^7.33"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `test_python_release-0.1.0/test_python_release/check_firewall.py` & `test_python_release-0.1.1/test_python_release/check_firewall.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.1.0/test_python_release/firewall_proxy.py` & `test_python_release-0.1.1/test_python_release/firewall_proxy.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.1.0/test_python_release/snapshot_compare.py` & `test_python_release-0.1.1/test_python_release/snapshot_compare.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.1.0/test_python_release/utils.py` & `test_python_release-0.1.1/test_python_release/utils.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.1.0/PKG-INFO` & `test_python_release-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-python-release
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: FoSIX
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

