# Comparing `tmp/anastasia_logging-1.3.0.tar.gz` & `tmp/anastasia_logging-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anastasia_logging-1.3.0.tar", max compression
+gzip compressed data, was "anastasia_logging-1.3.1.tar", max compression
```

## Comparing `anastasia_logging-1.3.0.tar` & `anastasia_logging-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6171 2023-05-16 18:44:03.254943 anastasia_logging-1.3.0/README.md
--rw-r--r--   0        0        0    12541 2023-05-16 19:03:05.770304 anastasia_logging-1.3.0/anastasia_logging/__init__.py
--rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.3.0/anastasia_logging/codes/__init__.py
--rw-r--r--   0        0        0     1200 2023-05-16 19:06:41.059173 anastasia_logging-1.3.0/anastasia_logging/codes/standard.py
--rw-r--r--   0        0        0       59 2023-05-16 19:04:35.614812 anastasia_logging-1.3.0/anastasia_logging/codes/standard_critical.py
--rw-r--r--   0        0        0       56 2023-05-16 19:03:57.198623 anastasia_logging-1.3.0/anastasia_logging/codes/standard_debug.py
--rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.3.0/anastasia_logging/codes/standard_errors.py
--rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.3.0/anastasia_logging/codes/standard_info.py
--rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.3.0/anastasia_logging/codes/standard_warning.py
--rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.3.0/anastasia_logging/env/__init__.py
--rw-r--r--   0        0        0      553 2023-05-16 19:09:23.183169 anastasia_logging-1.3.0/anastasia_logging/env/env_variables.py
--rw-r--r--   0        0        0    17527 2023-05-16 19:00:15.432605 anastasia_logging-1.3.0/anastasia_logging/logger.py
--rw-r--r--   0        0        0      285 2023-05-16 18:44:41.226247 anastasia_logging-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6614 1970-01-01 00:00:00.000000 anastasia_logging-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6291 2023-05-17 15:40:56.723080 anastasia_logging-1.3.1/README.md
+-rw-r--r--   0        0        0    12541 2023-05-17 15:16:00.243593 anastasia_logging-1.3.1/anastasia_logging/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.3.1/anastasia_logging/codes/__init__.py
+-rw-r--r--   0        0        0     1200 2023-05-17 15:16:00.243593 anastasia_logging-1.3.1/anastasia_logging/codes/standard.py
+-rw-r--r--   0        0        0       62 2023-05-17 15:40:56.723080 anastasia_logging-1.3.1/anastasia_logging/codes/standard_critical.py
+-rw-r--r--   0        0        0       57 2023-05-17 15:40:56.723080 anastasia_logging-1.3.1/anastasia_logging/codes/standard_debug.py
+-rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.3.1/anastasia_logging/codes/standard_errors.py
+-rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.3.1/anastasia_logging/codes/standard_info.py
+-rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.3.1/anastasia_logging/codes/standard_warning.py
+-rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.3.1/anastasia_logging/env/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-16 19:09:23.183169 anastasia_logging-1.3.1/anastasia_logging/env/env_variables.py
+-rw-r--r--   0        0        0    17527 2023-05-17 15:16:00.247593 anastasia_logging-1.3.1/anastasia_logging/logger.py
+-rw-r--r--   0        0        0      285 2023-05-17 15:40:56.723080 anastasia_logging-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6734 1970-01-01 00:00:00.000000 anastasia_logging-1.3.1/PKG-INFO
```

### Comparing `anastasia_logging-1.3.0/README.md` & `anastasia_logging-1.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -123,14 +123,20 @@
 logging.print("Some prints to show")
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
 ```
 
 ## **3. Versioning** ##
 
+### v1.3.1 ###
+
+* Fixes:
+
+    * Default unindentified ```debug```, ```critical``` and ```fatal``` standard codes fixed
+
 ### v1.3.0 ###
 
 * Features:
 
     * Functions ```critical```, ```fatal``` and ```debug``` incorporated
 
 ### v1.2.0 ###
```

### Comparing `anastasia_logging-1.3.0/anastasia_logging/__init__.py` & `anastasia_logging-1.3.1/anastasia_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.3.0/anastasia_logging/codes/standard.py` & `anastasia_logging-1.3.1/anastasia_logging/codes/standard.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.3.0/anastasia_logging/env/env_variables.py` & `anastasia_logging-1.3.1/anastasia_logging/env/env_variables.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.3.0/anastasia_logging/logger.py` & `anastasia_logging-1.3.1/anastasia_logging/logger.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.3.0/PKG-INFO` & `anastasia_logging-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anastasia-logging
-Version: 1.3.0
+Version: 1.3.1
 Summary: Anastasia Logging Standarization
 Author: anastasiaai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -136,14 +136,20 @@
 logging.print("Some prints to show")
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
 ```
 
 ## **3. Versioning** ##
 
+### v1.3.1 ###
+
+* Fixes:
+
+    * Default unindentified ```debug```, ```critical``` and ```fatal``` standard codes fixed
+
 ### v1.3.0 ###
 
 * Features:
 
     * Functions ```critical```, ```fatal``` and ```debug``` incorporated
 
 ### v1.2.0 ###
```

