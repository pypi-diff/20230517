# Comparing `tmp/p67_awstools-0.1.1.tar.gz` & `tmp/p67_awstools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p67_awstools-0.1.1.tar", max compression
+gzip compressed data, was "p67_awstools-0.1.2.tar", max compression
```

## Comparing `p67_awstools-0.1.1.tar` & `p67_awstools-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2849 2023-05-17 12:16:10.507506 p67_awstools-0.1.1/README.md
--rwxr-xr-x   0        0        0     2587 2023-05-17 12:06:57.417439 p67_awstools-0.1.1/p67_awstools/cli_scale_ec2_asg.py
--rw-r--r--   0        0        0     1174 2023-05-16 17:19:19.830543 p67_awstools-0.1.1/p67_awstools/password_rotate.py
--rw-r--r--   0        0        0      442 2023-05-17 12:17:34.166931 p67_awstools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 p67_awstools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2849 2023-05-17 12:16:10.507506 p67_awstools-0.1.2/README.md
+-rwxr-xr-x   0        0        0     2587 2023-05-17 12:06:57.417439 p67_awstools-0.1.2/p67_awstools/cli_scale_ec2_asg.py
+-rw-r--r--   0        0        0     1174 2023-05-16 17:19:19.830543 p67_awstools-0.1.2/p67_awstools/password_rotate.py
+-rw-r--r--   0        0        0      442 2023-05-17 12:24:42.964144 p67_awstools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 p67_awstools-0.1.2/PKG-INFO
```

### Comparing `p67_awstools-0.1.1/README.md` & `p67_awstools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `p67_awstools-0.1.1/p67_awstools/cli_scale_ec2_asg.py` & `p67_awstools-0.1.2/p67_awstools/cli_scale_ec2_asg.py`

 * *Files identical despite different names*

### Comparing `p67_awstools-0.1.1/p67_awstools/password_rotate.py` & `p67_awstools-0.1.2/p67_awstools/password_rotate.py`

 * *Files identical despite different names*

### Comparing `p67_awstools-0.1.1/PKG-INFO` & `p67_awstools-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p67-awstools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Various AWS code
 Author: Rene Benner
 Author-email: rene@fortytwo.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

