# Comparing `tmp/jautomate-0.0.4.tar.gz` & `tmp/jautomate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jautomate-0.0.4.tar", last modified: Mon Mar 20 14:50:36 2023, max compression
+gzip compressed data, was "jautomate-0.0.5.tar", last modified: Wed Mar 22 12:14:49 2023, max compression
```

## Comparing `jautomate-0.0.4.tar` & `jautomate-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-20 14:50:36.762785 jautomate-0.0.4/
--rw-r--r--   0 yoxall     (503) staff       (20)     2474 2023-03-20 14:50:36.762841 jautomate-0.0.4/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)     2116 2023-03-17 14:27:58.000000 jautomate-0.0.4/README.md
--rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-03-16 19:32:05.000000 jautomate-0.0.4/pyproject.toml
--rw-r--r--   0 yoxall     (503) staff       (20)      782 2023-03-20 14:50:36.763168 jautomate-0.0.4/setup.cfg
--rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-03-15 18:48:35.000000 jautomate-0.0.4/setup.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-20 14:50:36.756831 jautomate-0.0.4/src/
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-20 14:50:36.760077 jautomate-0.0.4/src/jautomate/
--rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-03-20 14:49:09.000000 jautomate-0.0.4/src/jautomate/__init__.py
--rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-03-20 14:47:59.000000 jautomate-0.0.4/src/jautomate/__main__.py
--rw-r--r--   0 yoxall     (503) staff       (20)     7148 2023-03-13 15:40:58.000000 jautomate-0.0.4/src/jautomate/actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-03-13 19:41:21.000000 jautomate-0.0.4/src/jautomate/api.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1588 2023-03-15 18:11:11.000000 jautomate-0.0.4/src/jautomate/assets.py
--rw-r--r--   0 yoxall     (503) staff       (20)     4805 2023-03-16 19:29:53.000000 jautomate-0.0.4/src/jautomate/cli.py
--rw-r--r--   0 yoxall     (503) staff       (20)      961 2023-03-20 14:31:19.000000 jautomate-0.0.4/src/jautomate/logger.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-03-16 18:53:21.000000 jautomate-0.0.4/src/jautomate/utils.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-20 14:50:36.761705 jautomate-0.0.4/src/jautomate.egg-info/
--rw-r--r--   0 yoxall     (503) staff       (20)     2474 2023-03-20 14:50:36.000000 jautomate-0.0.4/src/jautomate.egg-info/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-03-20 14:50:36.000000 jautomate-0.0.4/src/jautomate.egg-info/SOURCES.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-20 14:50:36.000000 jautomate-0.0.4/src/jautomate.egg-info/dependency_links.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-03-20 14:50:36.000000 jautomate-0.0.4/src/jautomate.egg-info/entry_points.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.4/src/jautomate.egg-info/not-zip-safe
--rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-03-20 14:50:36.000000 jautomate-0.0.4/src/jautomate.egg-info/requires.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-03-20 14:50:36.000000 jautomate-0.0.4/src/jautomate.egg-info/top_level.txt
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-20 14:50:36.762414 jautomate-0.0.4/tests/
--rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-03-16 19:08:13.000000 jautomate-0.0.4/tests/test_actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-03-16 15:17:54.000000 jautomate-0.0.4/tests/test_jautomate.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-03-16 19:12:12.000000 jautomate-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 12:14:49.849115 jautomate-0.0.5/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2474 2023-03-22 12:14:49.849224 jautomate-0.0.5/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)     2116 2023-03-17 14:27:58.000000 jautomate-0.0.5/README.md
+-rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-03-16 19:32:05.000000 jautomate-0.0.5/pyproject.toml
+-rw-r--r--   0 yoxall     (503) staff       (20)      804 2023-03-22 12:14:49.849693 jautomate-0.0.5/setup.cfg
+-rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-03-15 18:48:35.000000 jautomate-0.0.5/setup.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 12:14:49.840439 jautomate-0.0.5/src/
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 12:14:49.846446 jautomate-0.0.5/src/jautomate/
+-rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-03-22 12:14:09.000000 jautomate-0.0.5/src/jautomate/__init__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-03-20 14:47:59.000000 jautomate-0.0.5/src/jautomate/__main__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     7148 2023-03-13 15:40:58.000000 jautomate-0.0.5/src/jautomate/actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-03-13 19:41:21.000000 jautomate-0.0.5/src/jautomate/api.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1588 2023-03-15 18:11:11.000000 jautomate-0.0.5/src/jautomate/assets.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     4805 2023-03-16 19:29:53.000000 jautomate-0.0.5/src/jautomate/cli.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      962 2023-03-22 12:07:02.000000 jautomate-0.0.5/src/jautomate/logger.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-03-16 18:53:21.000000 jautomate-0.0.5/src/jautomate/utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 12:14:49.847960 jautomate-0.0.5/src/jautomate.egg-info/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2474 2023-03-22 12:14:49.000000 jautomate-0.0.5/src/jautomate.egg-info/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-03-22 12:14:49.000000 jautomate-0.0.5/src/jautomate.egg-info/SOURCES.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-22 12:14:49.000000 jautomate-0.0.5/src/jautomate.egg-info/dependency_links.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-03-22 12:14:49.000000 jautomate-0.0.5/src/jautomate.egg-info/entry_points.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.5/src/jautomate.egg-info/not-zip-safe
+-rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-03-22 12:14:49.000000 jautomate-0.0.5/src/jautomate.egg-info/requires.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-03-22 12:14:49.000000 jautomate-0.0.5/src/jautomate.egg-info/top_level.txt
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-03-22 12:14:49.848821 jautomate-0.0.5/tests/
+-rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-03-16 19:08:13.000000 jautomate-0.0.5/tests/test_actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-03-16 15:17:54.000000 jautomate-0.0.5/tests/test_jautomate.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-03-16 19:12:12.000000 jautomate-0.0.5/tests/test_utils.py
```

### Comparing `jautomate-0.0.4/PKG-INFO` & `jautomate-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jautomate
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automates MDM tasks using the Jamf APIs
 Author: Dustin Yoxall
 Author-email: yoxall.dustin@ccpsstaff.org
 License: MIT
 Keywords: python,jamf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jautomate-0.0.4/README.md` & `jautomate-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.4/setup.cfg` & `jautomate-0.0.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jautomate
-version = 0.0.4
+version = attr: jautomate.__version__
 author = Dustin Yoxall
 author_email = yoxall.dustin@ccpsstaff.org
 description = Automates MDM tasks using the Jamf APIs
 long_description = file: README.md, CHANGELOG.md, LICENSE.txt
 long_description_content_type = text/markdown
 keywords = python, jamf
 license = MIT
```

### Comparing `jautomate-0.0.4/src/jautomate/actions.py` & `jautomate-0.0.5/src/jautomate/actions.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.4/src/jautomate/assets.py` & `jautomate-0.0.5/src/jautomate/assets.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.4/src/jautomate/cli.py` & `jautomate-0.0.5/src/jautomate/cli.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.4/src/jautomate/logger.py` & `jautomate-0.0.5/src/jautomate/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Errors are logged in error.log while debugging messages are sent
 to the console.
 """
 
 import logging
 
 J_ERROR_LOG = logging.ERROR
-J_DEBUG_LOG = logging.INFO
+J_DEBUG_LOG = logging.DEBUG
 
 
 def init_logger():
     # Set up logging, debug will output to stream, errors will log to file.
     logger = logging.getLogger("jautomate")
     logger.setLevel(J_DEBUG_LOG)
```

### Comparing `jautomate-0.0.4/src/jautomate/utils.py` & `jautomate-0.0.5/src/jautomate/utils.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.4/src/jautomate.egg-info/PKG-INFO` & `jautomate-0.0.5/src/jautomate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jautomate
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automates MDM tasks using the Jamf APIs
 Author: Dustin Yoxall
 Author-email: yoxall.dustin@ccpsstaff.org
 License: MIT
 Keywords: python,jamf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jautomate-0.0.4/src/jautomate.egg-info/SOURCES.txt` & `jautomate-0.0.5/src/jautomate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.4/tests/test_utils.py` & `jautomate-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

