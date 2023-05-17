# Comparing `tmp/report_mr_2018-1.0.1.tar.gz` & `tmp/report_mr_2018-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "report_mr_2018-1.0.2.tar", max compression
```

## Comparing `report_mr_2018-1.0.1.tar` & `report_mr_2018-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,11 @@
--rwxr-xr-x   0        0        0     1211 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/conftest.py
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/requirements.txt
--rwxr-xr-x   0        0        0      663 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/data/abbreviations.txt
--rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/data/end.log
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/data/start.log
--rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/report_MR_2018/__init__.py
--rwxr-xr-x   0        0        0     7051 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/report_MR_2018/report.py
--rwxr-xr-x   0        0        0     2061 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/report_MR_2018/report_cli.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/tests/__init__.py
--rwxr-xr-x   0        0        0     6054 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/tests/test_report.py
--rwxr-xr-x   0        0        0     2377 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/tests/test_report_cli.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/LICENSE
--rwxr-xr-x   0        0        0     5709 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/README.md
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 report_mr_2018-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 report_mr_2018-1.0.2/LICENSE
+-rwxr-xr-x   0        0        0      916 2023-05-17 11:20:01.856232 report_mr_2018-1.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0       37 2023-05-16 13:22:20.811322 report_mr_2018-1.0.2/report_mr_2018/.pytest_cache/.gitignore
+-rwxr-xr-x   0        0        0      191 2023-05-16 13:22:20.819322 report_mr_2018-1.0.2/report_mr_2018/.pytest_cache/CACHEDIR.TAG
+-rwxr-xr-x   0        0        0      302 2023-05-16 13:22:20.804314 report_mr_2018-1.0.2/report_mr_2018/.pytest_cache/README.md
+-rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.829316 report_mr_2018-1.0.2/report_mr_2018/.pytest_cache/v/cache/nodeids
+-rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.844313 report_mr_2018-1.0.2/report_mr_2018/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0        0        0      139 2023-05-16 13:30:25.547805 report_mr_2018-1.0.2/report_mr_2018/__init__.py
+-rwxr-xr-x   0        0        0     7051 2023-05-17 10:24:40.093966 report_mr_2018-1.0.2/report_mr_2018/report.py
+-rwxr-xr-x   0        0        0     2061 2023-05-17 10:24:43.379555 report_mr_2018-1.0.2/report_mr_2018/report_cli.py
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 report_mr_2018-1.0.2/PKG-INFO
```

### Comparing `report_mr_2018-1.0.1/report_MR_2018/report.py` & `report_mr_2018-1.0.2/report_mr_2018/report.py`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.1/report_MR_2018/report_cli.py` & `report_mr_2018-1.0.2/report_mr_2018/report_cli.py`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.1/LICENSE` & `report_mr_2018-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.1/pyproject.toml` & `report_mr_2018-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "report_MR_2018"
-version = "1.0.1"
+version = "1.0.2"
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
-version = "1.0.1"
+version = "1.0.2"
 description = "Application that read data from 3 files, order racers by time and print report that shows 2 tables: the top 15 racers and other racers."
 authors = ["Nazar Hots <gotsjob@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = "^7.3.1"
 coverage = "^7.2.5"
```

