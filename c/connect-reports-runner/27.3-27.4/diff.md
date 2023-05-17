# Comparing `tmp/connect_reports_runner-27.3.tar.gz` & `tmp/connect_reports_runner-27.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_reports_runner-27.3.tar", max compression
+gzip compressed data, was "connect_reports_runner-27.4.tar", max compression
```

## Comparing `connect_reports_runner-27.3.tar` & `connect_reports_runner-27.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/LICENSE
--rw-r--r--   0        0        0      140 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/README.md
--rw-r--r--   0        0        0        0 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/__init__.py
--rw-r--r--   0        0        0     3443 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/exception_handler.py
--rw-r--r--   0        0        0       43 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/exceptions.py
--rw-r--r--   0        0        0     6131 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/executor.py
--rw-r--r--   0        0        0     1738 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/runner.py
--rw-r--r--   0        0        0     3730 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/utils.py
--rw-r--r--   0        0        0     2783 2023-04-25 13:15:06.965207 connect_reports_runner-27.3/pyproject.toml
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 connect_reports_runner-27.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/LICENSE
+-rw-r--r--   0        0        0      140 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/executor/__init__.py
+-rw-r--r--   0        0        0     3443 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/executor/exception_handler.py
+-rw-r--r--   0        0        0       43 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/executor/exceptions.py
+-rw-r--r--   0        0        0     6131 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/executor/executor.py
+-rw-r--r--   0        0        0     1786 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/executor/runner.py
+-rw-r--r--   0        0        0     3730 2023-05-17 14:46:51.366654 connect_reports_runner-27.4/executor/utils.py
+-rw-r--r--   0        0        0     2798 2023-05-17 14:47:37.849021 connect_reports_runner-27.4/pyproject.toml
+-rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 connect_reports_runner-27.4/PKG-INFO
```

### Comparing `connect_reports_runner-27.3/LICENSE` & `connect_reports_runner-27.4/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.3/executor/exception_handler.py` & `connect_reports_runner-27.4/executor/exception_handler.py`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.3/executor/executor.py` & `connect_reports_runner-27.4/executor/executor.py`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.3/executor/runner.py` & `connect_reports_runner-27.4/executor/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     try:
         fail_report(
             client,
             report_id,
             'Report execution has failed due contains too much data, please try to exclude '
             'using report parameters some of it and try again.',
             False,
-            stdout,
+            f'stdout: {stdout.decode()} stderr: {stderr.decode()}',
         )
         logger.info(f'Report {report_id} has been failed successfully.')
     except ClientError as ce:
         logger.warning(f'Cannot switch report {report_id} to fail status: {ce}')
     return
```

### Comparing `connect_reports_runner-27.3/executor/utils.py` & `connect_reports_runner-27.4/executor/utils.py`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.3/pyproject.toml` & `connect_reports_runner-27.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-reports-runner"
-version = "27.3"
+version = "27.4"
 description = "Connect Reports Runner"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "executor" }
 ]
 readme = "./README.md"
@@ -36,14 +36,15 @@
 python = ">=3.8,<4"
 chardet = "3.*"
 connect-openapi-client = ">=25.4"
 connect-reports-core = "26.*"
 lxml = "4.*"
 openpyxl = "3.*"
 requests = "2.*"
+urllib3 = "<2"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=6.1.2,<8"
 pytest-cov = ">=2.10.1,<5"
 pytest-mock = "^3.3.1"
 coverage = {extras = ["toml"], version = ">=5.3,<7"}
 flake8 = ">=3.8,<6"
```

### Comparing `connect_reports_runner-27.3/PKG-INFO` & `connect_reports_runner-27.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-reports-runner
-Version: 27.3
+Version: 27.4
 Summary: Connect Reports Runner
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Keywords: utility,connect,cloudblue,reports
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,14 +24,15 @@
 Classifier: Topic :: Utilities
 Requires-Dist: chardet (>=3.0.0,<4.0.0)
 Requires-Dist: connect-openapi-client (>=25.4)
 Requires-Dist: connect-reports-core (>=26.0.0,<27.0.0)
 Requires-Dist: lxml (>=4.0.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.0,<4.0.0)
 Requires-Dist: requests (>=2.0.0,<3.0.0)
+Requires-Dist: urllib3 (<2)
 Project-URL: Documentation, https://github.com/cloudblue/connect-reports-runner
 Project-URL: Repository, https://github.com/cloudblue/connect-reports-runner
 Description-Content-Type: text/markdown
 
 Connect Reports Executor
 ========================
```

