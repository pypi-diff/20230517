# Comparing `tmp/jautomate-0.0.7.tar.gz` & `tmp/jautomate-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jautomate-0.0.7.tar", last modified: Wed May 17 18:42:58 2023, max compression
+gzip compressed data, was "jautomate-0.0.8.tar", last modified: Wed May 17 19:26:33 2023, max compression
```

## Comparing `jautomate-0.0.7.tar` & `jautomate-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.147237 jautomate-0.0.7/
--rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 18:42:58.147337 jautomate-0.0.7/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)     2372 2023-05-16 18:24:54.000000 jautomate-0.0.7/README.md
--rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-05-05 12:20:37.000000 jautomate-0.0.7/pyproject.toml
--rw-r--r--   0 yoxall     (503) staff       (20)      805 2023-05-17 18:42:58.147684 jautomate-0.0.7/setup.cfg
--rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-05-05 12:20:37.000000 jautomate-0.0.7/setup.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.142417 jautomate-0.0.7/src/
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.145307 jautomate-0.0.7/src/jautomate/
--rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-05-16 15:22:01.000000 jautomate-0.0.7/src/jautomate/__init__.py
--rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/__main__.py
--rw-r--r--   0 yoxall     (503) staff       (20)     8320 2023-05-17 15:53:41.000000 jautomate-0.0.7/src/jautomate/actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/api.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1768 2023-05-16 12:57:26.000000 jautomate-0.0.7/src/jautomate/assets.py
--rw-r--r--   0 yoxall     (503) staff       (20)     6023 2023-05-17 15:49:16.000000 jautomate-0.0.7/src/jautomate/cli.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1138 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/logger.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-05-05 12:20:37.000000 jautomate-0.0.7/src/jautomate/utils.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.146519 jautomate-0.0.7/src/jautomate.egg-info/
--rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/SOURCES.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/dependency_links.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/entry_points.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.7/src/jautomate.egg-info/not-zip-safe
--rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/requires.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-05-17 18:42:58.000000 jautomate-0.0.7/src/jautomate.egg-info/top_level.txt
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 18:42:58.147053 jautomate-0.0.7/tests/
--rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-05-05 12:20:37.000000 jautomate-0.0.7/tests/test_actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-05-05 12:20:37.000000 jautomate-0.0.7/tests/test_jautomate.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-05-05 12:20:37.000000 jautomate-0.0.7/tests/test_utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.042077 jautomate-0.0.8/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 19:26:33.042173 jautomate-0.0.8/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)     2372 2023-05-16 18:24:54.000000 jautomate-0.0.8/README.md
+-rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-05-05 12:20:37.000000 jautomate-0.0.8/pyproject.toml
+-rw-r--r--   0 yoxall     (503) staff       (20)      805 2023-05-17 19:26:33.042527 jautomate-0.0.8/setup.cfg
+-rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-05-05 12:20:37.000000 jautomate-0.0.8/setup.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.037235 jautomate-0.0.8/src/
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.040117 jautomate-0.0.8/src/jautomate/
+-rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-05-17 19:26:23.000000 jautomate-0.0.8/src/jautomate/__init__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/__main__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     8320 2023-05-17 15:53:41.000000 jautomate-0.0.8/src/jautomate/actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/api.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1768 2023-05-16 12:57:26.000000 jautomate-0.0.8/src/jautomate/assets.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     6023 2023-05-17 15:49:16.000000 jautomate-0.0.8/src/jautomate/cli.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1138 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/logger.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.041452 jautomate-0.0.8/src/jautomate.egg-info/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/SOURCES.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/dependency_links.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/entry_points.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.8/src/jautomate.egg-info/not-zip-safe
+-rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/requires.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/top_level.txt
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.041906 jautomate-0.0.8/tests/
+-rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-05-05 12:20:37.000000 jautomate-0.0.8/tests/test_actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-05-05 12:20:37.000000 jautomate-0.0.8/tests/test_jautomate.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-05-05 12:20:37.000000 jautomate-0.0.8/tests/test_utils.py
```

### Comparing `jautomate-0.0.7/PKG-INFO` & `jautomate-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jautomate
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automates MDM tasks using the Jamf APIs
 Author: Dustin Yoxall
 Author-email: yoxall.dustin@ccpsstaff.org
 License: MIT
 Keywords: python,jamf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Jautomate
 This tool automates MDM tasks on Jamf using the Jamf Pro and Jamf Classic API. For now there are only tasks focused on mobile devices. Computer versions of those tasks are in the works.
 
 ## Installation
 ---
```

### Comparing `jautomate-0.0.7/README.md` & `jautomate-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.7/setup.cfg` & `jautomate-0.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
-python_requires = >=3.11
+python_requires = >=3.10
 install_requires = 
 	jps_api_wrapper
 	typer
 	python-dotenv
 
 [options.packages.find]
 where = src
```

### Comparing `jautomate-0.0.7/src/jautomate/actions.py` & `jautomate-0.0.8/src/jautomate/actions.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.7/src/jautomate/assets.py` & `jautomate-0.0.8/src/jautomate/assets.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.7/src/jautomate/cli.py` & `jautomate-0.0.8/src/jautomate/cli.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.7/src/jautomate/logger.py` & `jautomate-0.0.8/src/jautomate/logger.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.7/src/jautomate/utils.py` & `jautomate-0.0.8/src/jautomate/utils.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.7/src/jautomate.egg-info/PKG-INFO` & `jautomate-0.0.8/src/jautomate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jautomate
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automates MDM tasks using the Jamf APIs
 Author: Dustin Yoxall
 Author-email: yoxall.dustin@ccpsstaff.org
 License: MIT
 Keywords: python,jamf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Jautomate
 This tool automates MDM tasks on Jamf using the Jamf Pro and Jamf Classic API. For now there are only tasks focused on mobile devices. Computer versions of those tasks are in the works.
 
 ## Installation
 ---
```

### Comparing `jautomate-0.0.7/src/jautomate.egg-info/SOURCES.txt` & `jautomate-0.0.8/src/jautomate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.7/tests/test_utils.py` & `jautomate-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

