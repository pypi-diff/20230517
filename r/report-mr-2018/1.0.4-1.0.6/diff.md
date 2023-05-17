# Comparing `tmp/report_mr_2018-1.0.4.tar.gz` & `tmp/report_mr_2018-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report_mr_2018-1.0.4.tar", max compression
+gzip compressed data, was "report_mr_2018-1.0.6.tar", max compression
```

## Comparing `report_mr_2018-1.0.4.tar` & `report_mr_2018-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,7 @@
--rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 report_mr_2018-1.0.4/LICENSE
--rwxr-xr-x   0        0        0     5709 2023-05-17 10:24:18.530543 report_mr_2018-1.0.4/README.md
--rwxr-xr-x   0        0        0      991 2023-05-17 12:24:35.335690 report_mr_2018-1.0.4/pyproject.toml
--rwxr-xr-x   0        0        0       37 2023-05-16 13:22:20.811322 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/.gitignore
--rwxr-xr-x   0        0        0      191 2023-05-16 13:22:20.819322 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/CACHEDIR.TAG
--rwxr-xr-x   0        0        0      302 2023-05-16 13:22:20.804314 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/README.md
--rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.829316 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/v/cache/nodeids
--rwxr-xr-x   0        0        0        2 2023-05-16 13:22:20.844313 report_mr_2018-1.0.4/report_mr_2018/.pytest_cache/v/cache/stepwise
--rwxr-xr-x   0        0        0      139 2023-05-16 13:30:25.547805 report_mr_2018-1.0.4/report_mr_2018/__init__.py
--rwxr-xr-x   0        0        0     7051 2023-05-17 10:24:40.093966 report_mr_2018-1.0.4/report_mr_2018/report.py
--rwxr-xr-x   0        0        0     2061 2023-05-17 10:24:43.379555 report_mr_2018-1.0.4/report_mr_2018/report_cli.py
--rw-r--r--   0        0        0     6346 1970-01-01 00:00:00.000000 report_mr_2018-1.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 report_mr_2018-1.0.6/LICENSE
+-rwxr-xr-x   0        0        0     5709 2023-05-17 10:24:18.530543 report_mr_2018-1.0.6/README.md
+-rwxr-xr-x   0        0        0      502 2023-05-17 13:32:02.474043 report_mr_2018-1.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0      139 2023-05-16 13:30:25.547805 report_mr_2018-1.0.6/report_MR_2018/__init__.py
+-rwxr-xr-x   0        0        0     7051 2023-05-17 10:24:40.093966 report_mr_2018-1.0.6/report_MR_2018/report.py
+-rwxr-xr-x   0        0        0     2061 2023-05-17 10:24:43.379555 report_mr_2018-1.0.6/report_MR_2018/report_cli.py
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 report_mr_2018-1.0.6/PKG-INFO
```

### Comparing `report_mr_2018-1.0.4/LICENSE` & `report_mr_2018-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.4/README.md` & `report_mr_2018-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.4/report_mr_2018/report.py` & `report_mr_2018-1.0.6/report_MR_2018/report.py`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.4/report_mr_2018/report_cli.py` & `report_mr_2018-1.0.6/report_MR_2018/report_cli.py`

 * *Files identical despite different names*

### Comparing `report_mr_2018-1.0.4/PKG-INFO` & `report_mr_2018-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: report-mr-2018
-Version: 1.0.4
+Version: 1.0.6
 Summary: Application that read data from 3 files, order racers by time and print report that shows 2 tables: the top 15 racers and other racers.
+License: MIT
 Author: Nazar Hots
 Author-email: gotsjob@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PTable (>=0.9.0,<0.10.0)
-Requires-Dist: coverage (>=7.2.5,<8.0.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: PTable (>=0.9.2,<0.10.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Report of Monaco 2018 Racing
 
 ## Installation
 Clone this repository to your local machine:
```

