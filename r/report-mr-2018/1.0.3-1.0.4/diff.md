# Comparing `tmp/report_mr_2018-1.0.3.tar.gz` & `tmp/report_mr_2018-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report_mr_2018-1.0.3.tar", max compression
+gzip compressed data, was "report_mr_2018-1.0.4.tar", max compression
```

## Comparing `report_mr_2018-1.0.3.tar` & `report_mr_2018-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 report_mr_2018-1.0.3/LICENSE
--rwxr-xr-x   0        0        0     5709 2023-05-17 10:24:18.530543 report_mr_2018-1.0.3/README.md
--rwxr-xr-x   0        0        0      991 2023-05-17 12:12:34.115148 report_mr_2018-1.0.3/pyproject.toml
--rwxr-xr-x   0        0        0       37 2023-05-16 13:22:20.811322 report_mr_2018-1.0.3/report_mr_2018/.pytest_cache/.gitignore
--rwxr-xr-x   0        0        0      191 2023-05-16 13:22:20.819322 report_mr_2018-1.0.3/report_mr_2018/.pytest_cache/CACHEDIR.TAG
--rwxr-xr-x   0        0        0      302 2023-05-16 13:22:20.804314 report_mr_2018-1.0.3/report_mr_2018/.pytest_cache/README.md
--rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.829316 report_mr_2018-1.0.3/report_mr_2018/.pytest_cache/v/cache/nodeids
--rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.844313 report_mr_2018-1.0.3/report_mr_2018/.pytest_cache/v/cache/stepwise
--rwxr-xr-x   0        0        0      139 2023-05-16 13:30:25.547805 report_mr_2018-1.0.3/report_mr_2018/__init__.py
--rwxr-xr-x   0        0        0     7051 2023-05-17 10:24:40.093966 report_mr_2018-1.0.3/report_mr_2018/report.py
--rwxr-xr-x   0        0        0     2061 2023-05-17 10:24:43.379555 report_mr_2018-1.0.3/report_mr_2018/report_cli.py
--rw-r--r--   0        0        0     6346 1970-01-01 00:00:00.000000 report_mr_2018-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 report_mr_2018-1.0.4/LICENSE
+-rwxr-xr-x   0        0        0     5709 2023-05-17 10:24:18.530543 report_mr_2018-1.0.4/README.md
+-rwxr-xr-x   0        0        0      991 2023-05-17 12:24:35.335690 report_mr_2018-1.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0       37 2023-05-16 13:22:20.811322 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/.gitignore
+-rwxr-xr-x   0        0        0      191 2023-05-16 13:22:20.819322 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/CACHEDIR.TAG
+-rwxr-xr-x   0        0        0      302 2023-05-16 13:22:20.804314 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/README.md
+-rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.829316 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/v/cache/nodeids
+-rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.844313 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0        0        0      139 2023-05-16 13:30:25.547805 report_mr_2018-1.0.4/report_mr_2018/__init__.py
+-rwxr-xr-x   0        0        0     7051 2023-05-17 10:24:40.093966 report_mr_2018-1.0.4/report_mr_2018/report.py
+-rwxr-xr-x   0        0        0     2061 2023-05-17 10:24:43.379555 report_mr_2018-1.0.4/report_mr_2018/report_cli.py
+-rw-r--r--   0        0        0     6346 1970-01-01 00:00:00.000000 report_mr_2018-1.0.4/PKG-INFO
```

### Comparing `report_mr_2018-1.0.3/LICENSE` & `report_mr_2018-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.3/README.md` & `report_mr_2018-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.3/pyproject.toml` & `report_mr_2018-1.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "report_MR_2018"
-version = "1.0.3"
+version = "1.0.4"
 authors = [{ name = "Nazar Hots", email = "gotsjob@gmail.com" }]
 description = "Application that read data from 3 files, order racers by time and print report that shows 2 tables: the top 15 racers and other racers."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry]
 name = "report_MR_2018"
-version = "1.0.3"
+version = "1.0.4"
 readme = "/mnt/e/Foxminded/task-6-report-of-monaco-2018-racing/README.md"
 description = "Application that read data from 3 files, order racers by time and print report that shows 2 tables: the top 15 racers and other racers."
 authors = ["Nazar Hots <gotsjob@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = "^7.3.1"
```

### Comparing `report_mr_2018-1.0.3/report_mr_2018/report.py` & `report_mr_2018-1.0.4/report_mr_2018/report.py`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.3/report_mr_2018/report_cli.py` & `report_mr_2018-1.0.4/report_mr_2018/report_cli.py`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.3/PKG-INFO` & `report_mr_2018-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-mr-2018
-Version: 1.0.3
+Version: 1.0.4
 Summary: Application that read data from 3 files, order racers by time and print report that shows 2 tables: the top 15 racers and other racers.
 Author: Nazar Hots
 Author-email: gotsjob@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

