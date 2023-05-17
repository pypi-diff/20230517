# Comparing `tmp/pace_python_logger-0.0.2.tar.gz` & `tmp/pace_python_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pace_python_logger-0.0.2.tar", last modified: Thu May 11 01:02:43 2023, max compression
+gzip compressed data, was "pace_python_logger-0.0.3.tar", last modified: Wed May 17 15:58:20 2023, max compression
```

## Comparing `pace_python_logger-0.0.2.tar` & `pace_python_logger-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 01:02:43.798985 pace_python_logger-0.0.2/
--rw-rw-rw-   0        0        0     1085 2023-05-08 14:54:47.000000 pace_python_logger-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1040 2023-05-11 01:02:43.797984 pace_python_logger-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-05-08 18:02:17.000000 pace_python_logger-0.0.2/README.md
--rw-rw-rw-   0        0        0      728 2023-05-11 01:02:20.000000 pace_python_logger-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 01:02:43.798985 pace_python_logger-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 01:02:43.769019 pace_python_logger-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 01:02:43.780992 pace_python_logger-0.0.2/src/pace_py_log_lib/
--rw-rw-rw-   0        0        0        0 2023-05-08 14:20:23.000000 pace_python_logger-0.0.2/src/pace_py_log_lib/__init__.py
--rw-rw-rw-   0        0        0     1739 2023-05-10 22:58:19.000000 pace_python_logger-0.0.2/src/pace_py_log_lib/logger.py
-drwxrwxrwx   0        0        0        0 2023-05-11 01:02:43.795986 pace_python_logger-0.0.2/src/pace_python_logger.egg-info/
--rw-rw-rw-   0        0        0     1040 2023-05-11 01:02:43.000000 pace_python_logger-0.0.2/src/pace_python_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-11 01:02:43.000000 pace_python_logger-0.0.2/src/pace_python_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 01:02:43.000000 pace_python_logger-0.0.2/src/pace_python_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-11 01:02:43.000000 pace_python_logger-0.0.2/src/pace_python_logger.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 01:02:43.796984 pace_python_logger-0.0.2/tests/
--rw-rw-rw-   0        0        0     1910 2023-05-10 22:59:33.000000 pace_python_logger-0.0.2/tests/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:58:20.084996 pace_python_logger-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 14:54:47.000000 pace_python_logger-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1040 2023-05-17 15:58:20.084996 pace_python_logger-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-05-08 18:02:17.000000 pace_python_logger-0.0.3/README.md
+-rw-rw-rw-   0        0        0      739 2023-05-11 03:21:11.000000 pace_python_logger-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 15:58:20.086504 pace_python_logger-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 15:58:20.026897 pace_python_logger-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:58:20.055364 pace_python_logger-0.0.3/src/pace_py_log_lib/
+-rw-rw-rw-   0        0        0        0 2023-05-08 14:20:23.000000 pace_python_logger-0.0.3/src/pace_py_log_lib/__init__.py
+-rw-rw-rw-   0        0        0     1739 2023-05-10 22:58:19.000000 pace_python_logger-0.0.3/src/pace_py_log_lib/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:58:20.074502 pace_python_logger-0.0.3/src/pace_python_logger.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-05-17 15:58:19.000000 pace_python_logger-0.0.3/src/pace_python_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-17 15:58:20.000000 pace_python_logger-0.0.3/src/pace_python_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:58:19.000000 pace_python_logger-0.0.3/src/pace_python_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-17 15:58:19.000000 pace_python_logger-0.0.3/src/pace_python_logger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:58:20.082988 pace_python_logger-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1910 2023-05-10 22:59:33.000000 pace_python_logger-0.0.3/tests/test_logger.py
```

### Comparing `pace_python_logger-0.0.2/LICENSE` & `pace_python_logger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pace_python_logger-0.0.2/PKG-INFO` & `pace_python_logger-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pace_python_logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python logging library for Productivity Assessment of Copilots with Econometrics (PACE)
 Author-email: Aadharsh Kannan <akannan@microsoft.com>
 Project-URL: Homepage, https://github.com/microsoft/PACE/logging_library/python
 Project-URL: Bug Tracker, https://github.com/microsoft/PACE/logging_library/python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pace_python_logger-0.0.2/pyproject.toml` & `pace_python_logger-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0","websocket-client"]
+requires = ["setuptools>=61.0","websocket-client","requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pace_python_logger"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Aadharsh Kannan", email="akannan@microsoft.com" },
 ]
 description = "Python logging library for Productivity Assessment of Copilots with Econometrics (PACE)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pace_python_logger-0.0.2/src/pace_py_log_lib/logger.py` & `pace_python_logger-0.0.3/src/pace_py_log_lib/logger.py`

 * *Files identical despite different names*

### Comparing `pace_python_logger-0.0.2/src/pace_python_logger.egg-info/PKG-INFO` & `pace_python_logger-0.0.3/src/pace_python_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pace-python-logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python logging library for Productivity Assessment of Copilots with Econometrics (PACE)
 Author-email: Aadharsh Kannan <akannan@microsoft.com>
 Project-URL: Homepage, https://github.com/microsoft/PACE/logging_library/python
 Project-URL: Bug Tracker, https://github.com/microsoft/PACE/logging_library/python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pace_python_logger-0.0.2/tests/test_logger.py` & `pace_python_logger-0.0.3/tests/test_logger.py`

 * *Files identical despite different names*

