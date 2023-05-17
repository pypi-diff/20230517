# Comparing `tmp/spicy-snow-0.0.1.tar.gz` & `tmp/spicy-snow-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicy-snow-0.0.1.tar", last modified: Wed May 17 18:35:58 2023, max compression
+gzip compressed data, was "spicy-snow-0.1.0.tar", last modified: Wed May 17 18:49:46 2023, max compression
```

## Comparing `spicy-snow-0.0.1.tar` & `spicy-snow-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-17 18:35:58.584044 spicy-snow-0.0.1/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     1063 2023-01-25 22:15:07.000000 spicy-snow-0.0.1/LICENSE
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     5732 2023-05-17 18:35:58.583510 spicy-snow-0.0.1/PKG-INFO
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     5076 2023-05-15 18:24:24.000000 spicy-snow-0.0.1/README.md
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       84 2023-05-17 18:35:10.000000 spicy-snow-0.0.1/pyproject.toml
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       38 2023-05-17 18:35:58.584188 spicy-snow-0.0.1/setup.cfg
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4231 2023-05-17 18:35:50.000000 spicy-snow-0.0.1/setup.py
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-17 18:35:58.578524 spicy-snow-0.0.1/spicy_snow/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       42 2023-02-23 18:11:03.000000 spicy-snow-0.0.1/spicy_snow/__init__.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     6095 2023-04-07 18:16:25.000000 spicy-snow-0.0.1/spicy_snow/retrieval.py
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-17 18:35:58.580402 spicy-snow-0.0.1/spicy_snow.egg-info/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     5732 2023-05-17 18:35:58.000000 spicy-snow-0.0.1/spicy_snow.egg-info/PKG-INFO
--rw-r--r--   0 zachkeskinen   (501) staff       (20)      373 2023-05-17 18:35:58.000000 spicy-snow-0.0.1/spicy_snow.egg-info/SOURCES.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)        1 2023-05-17 18:35:58.000000 spicy-snow-0.0.1/spicy_snow.egg-info/dependency_links.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       69 2023-05-17 18:35:58.000000 spicy-snow-0.0.1/spicy_snow.egg-info/requires.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       11 2023-05-17 18:35:58.000000 spicy-snow-0.0.1/spicy_snow.egg-info/top_level.txt
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-17 18:35:58.582759 spicy-snow-0.0.1/tests/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     3085 2023-02-23 18:11:03.000000 spicy-snow-0.0.1/tests/test_IO.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4592 2023-05-17 18:29:25.000000 spicy-snow-0.0.1/tests/test_downloads.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)    11456 2023-04-16 18:47:59.000000 spicy-snow-0.0.1/tests/test_preprocessing.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)    22511 2023-04-16 00:02:26.000000 spicy-snow-0.0.1/tests/test_snow_index.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)    23142 2023-02-21 16:19:44.000000 spicy-snow-0.0.1/tests/test_wetsnow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-17 18:49:33.000000 spicy-snow-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/spicy_snow/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/spicy_snow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/spicy_snow/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/spicy_snow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 18:49:46.000000 spicy-snow-0.1.0/spicy_snow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:49:46.611893 spicy-snow-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_snow_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23142 2023-05-17 18:49:32.000000 spicy-snow-0.1.0/tests/test_wetsnow.py
```

### Comparing `spicy-snow-0.0.1/LICENSE` & `spicy-snow-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.0.1/PKG-INFO` & `spicy-snow-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicy-snow
-Version: 0.0.1
+Version: 0.1.0
 Summary: Snow Depth Retrievals from Sentinel-1 Backscatter.
 Home-page: https://github.com/SnowEx/spicy-snow
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `spicy-snow-0.0.1/README.md` & `spicy-snow-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.0.1/setup.py` & `spicy-snow-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=VERSION, # '{{VERSION_PLACEHOLDER}}'
+    version='0.1.0', # change to value if not using github auto upload
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `spicy-snow-0.0.1/spicy_snow/retrieval.py` & `spicy-snow-0.1.0/spicy_snow/retrieval.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.0.1/spicy_snow.egg-info/PKG-INFO` & `spicy-snow-0.1.0/spicy_snow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicy-snow
-Version: 0.0.1
+Version: 0.1.0
 Summary: Snow Depth Retrievals from Sentinel-1 Backscatter.
 Home-page: https://github.com/SnowEx/spicy-snow
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `spicy-snow-0.0.1/tests/test_IO.py` & `spicy-snow-0.1.0/tests/test_IO.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.0.1/tests/test_downloads.py` & `spicy-snow-0.1.0/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.0.1/tests/test_preprocessing.py` & `spicy-snow-0.1.0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.0.1/tests/test_snow_index.py` & `spicy-snow-0.1.0/tests/test_snow_index.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.0.1/tests/test_wetsnow.py` & `spicy-snow-0.1.0/tests/test_wetsnow.py`

 * *Files identical despite different names*

