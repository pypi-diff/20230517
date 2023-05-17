# Comparing `tmp/test_python_release-0.0.4.tar.gz` & `tmp/test_python_release-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_python_release-0.0.4.tar", max compression
+gzip compressed data, was "test_python_release-0.1.0.tar", max compression
```

## Comparing `test_python_release-0.0.4.tar` & `test_python_release-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-05-09 06:13:35.366704 test_python_release-0.0.4/LICENSE
--rw-r--r--   0        0        0       22 2023-05-17 06:37:48.252868 test_python_release-0.0.4/README.md
--rw-r--r--   0        0        0     1438 2023-05-17 08:10:26.686960 test_python_release-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 06:37:48.255428 test_python_release-0.0.4/test_python_release/__init__.py
--rw-r--r--   0        0        0    34905 2023-05-17 06:37:48.256472 test_python_release-0.0.4/test_python_release/check_firewall.py
--rw-r--r--   0        0        0    34296 2023-05-17 06:37:48.257364 test_python_release-0.0.4/test_python_release/firewall_proxy.py
--rw-r--r--   0        0        0    29922 2023-05-17 06:37:48.258130 test_python_release-0.0.4/test_python_release/snapshot_compare.py
--rw-r--r--   0        0        0    11729 2023-05-17 06:37:48.258756 test_python_release-0.0.4/test_python_release/utils.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 test_python_release-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-17 10:25:25.238612 test_python_release-0.1.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-17 10:25:25.238612 test_python_release-0.1.0/README.md
+-rw-r--r--   0        0        0      762 2023-05-17 10:25:58.362577 test_python_release-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/__init__.py
+-rw-r--r--   0        0        0    34905 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/check_firewall.py
+-rw-r--r--   0        0        0    34296 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/firewall_proxy.py
+-rw-r--r--   0        0        0    29922 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/snapshot_compare.py
+-rw-r--r--   0        0        0    11729 2023-05-17 10:25:25.242612 test_python_release-0.1.0/test_python_release/utils.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 test_python_release-0.1.0/PKG-INFO
```

### Comparing `test_python_release-0.0.4/LICENSE` & `test_python_release-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `test_python_release-0.0.4/test_python_release/check_firewall.py` & `test_python_release-0.1.0/test_python_release/check_firewall.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.0.4/test_python_release/firewall_proxy.py` & `test_python_release-0.1.0/test_python_release/firewall_proxy.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.0.4/test_python_release/snapshot_compare.py` & `test_python_release-0.1.0/test_python_release/snapshot_compare.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.0.4/test_python_release/utils.py` & `test_python_release-0.1.0/test_python_release/utils.py`

 * *Files identical despite different names*

### Comparing `test_python_release-0.0.4/PKG-INFO` & `test_python_release-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-python-release
-Version: 0.0.4
+Version: 0.1.0
 Summary: 
 Author: FoSIX
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

