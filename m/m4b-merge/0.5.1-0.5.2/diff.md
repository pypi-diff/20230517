# Comparing `tmp/m4b-merge-0.5.1.tar.gz` & `tmp/m4b-merge-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m4b-merge-0.5.1.tar", last modified: Fri Feb 24 01:27:35 2023, max compression
+gzip compressed data, was "m4b-merge-0.5.2.tar", last modified: Wed May 17 06:16:39 2023, max compression
```

## Comparing `m4b-merge-0.5.1.tar` & `m4b-merge-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:27:35.600168 m4b-merge-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-02-24 01:27:35.600168 m4b-merge-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 01:27:35.600168 m4b-merge-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:27:35.592168 m4b-merge-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:27:35.596168 m4b-merge-0.5.1/src/m4b_merge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/src/m4b_merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/src/m4b_merge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/src/m4b_merge/audible_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/src/m4b_merge/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/src/m4b_merge/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/src/m4b_merge/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16873 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/src/m4b_merge/m4b_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:27:35.596168 m4b-merge-0.5.1/src/m4b_merge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-02-24 01:27:35.000000 m4b-merge-0.5.1/src/m4b_merge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-24 01:27:35.000000 m4b-merge-0.5.1/src/m4b_merge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 01:27:35.000000 m4b-merge-0.5.1/src/m4b_merge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-24 01:27:35.000000 m4b-merge-0.5.1/src/m4b_merge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 01:27:35.000000 m4b-merge-0.5.1/src/m4b_merge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-24 01:27:35.000000 m4b-merge-0.5.1/src/m4b_merge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:27:35.600168 m4b-merge-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/tests/test_audible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/tests/test_multiple_m4b_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/tests/test_multiple_mp3_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/tests/test_single_m4b_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-02-24 01:27:25.000000 m4b-merge-0.5.1/tests/test_single_mp3_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:16:39.197312 m4b-merge-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-17 06:16:39.197312 m4b-merge-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:16:39.197312 m4b-merge-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:16:39.193312 m4b-merge-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:16:39.193312 m4b-merge-0.5.2/src/m4b_merge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/src/m4b_merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/src/m4b_merge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/src/m4b_merge/audible_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/src/m4b_merge/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/src/m4b_merge/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/src/m4b_merge/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/src/m4b_merge/m4b_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:16:39.197312 m4b-merge-0.5.2/src/m4b_merge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-17 06:16:39.000000 m4b-merge-0.5.2/src/m4b_merge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-17 06:16:39.000000 m4b-merge-0.5.2/src/m4b_merge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:16:39.000000 m4b-merge-0.5.2/src/m4b_merge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 06:16:39.000000 m4b-merge-0.5.2/src/m4b_merge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 06:16:39.000000 m4b-merge-0.5.2/src/m4b_merge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 06:16:39.000000 m4b-merge-0.5.2/src/m4b_merge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:16:39.197312 m4b-merge-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/tests/test_audible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/tests/test_multiple_m4b_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/tests/test_multiple_mp3_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/tests/test_single_m4b_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-17 06:16:28.000000 m4b-merge-0.5.2/tests/test_single_mp3_merge.py
```

### Comparing `m4b-merge-0.5.1/LICENSE` & `m4b-merge-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/PKG-INFO` & `m4b-merge-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m4b-merge
-Version: 0.5.1
+Version: 0.5.2
 Summary: A tool to standardize audiobook files into single m4b files with clean metadata based on Audible and chapters.
 Home-page: https://github.com/djdembeck/m4b-merge
 Author: David Dembeck
 Author-email: dembeck.david@protonmail.com
 Project-URL: Bug Tracker, https://github.com/djdembeck/m4b-merge/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `m4b-merge-0.5.1/README.md` & `m4b-merge-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/setup.py` & `m4b-merge-0.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='m4b-merge',
-    version='0.5.1',
+    version='0.5.2',
     url='https://github.com/djdembeck/m4b-merge',
     description=(
                 "A tool to standardize audiobook files"
                 " into single m4b files with clean metadata"
                 " based on Audible and chapters."),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `m4b-merge-0.5.1/src/m4b_merge/__main__.py` & `m4b-merge-0.5.2/src/m4b_merge/__main__.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/src/m4b_merge/audible_helper.py` & `m4b-merge-0.5.2/src/m4b_merge/audible_helper.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/src/m4b_merge/config.py` & `m4b-merge-0.5.2/src/m4b_merge/config.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/src/m4b_merge/helpers.py` & `m4b-merge-0.5.2/src/m4b_merge/helpers.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/src/m4b_merge/m4b_helper.py` & `m4b-merge-0.5.2/src/m4b_merge/m4b_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         # Handle single mp3 input file
         elif self.input_path.is_file() and self.input_extension == "mp3":
             self.merge_single_mp3()
         # If none of the above are true, log error
         else:
             logging.error(
                 f"Couldn't determine input type/extension for"
-                f" {self.file_title}")
+                f" {self.title}")
 
     def merge_multiple_files(self):
         logging.info("Processing multiple files in a dir...")
 
         first_file = self.find_file_for_mediainfo()
 
         # Mediainfo data
```

### Comparing `m4b-merge-0.5.1/src/m4b_merge.egg-info/PKG-INFO` & `m4b-merge-0.5.2/src/m4b_merge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m4b-merge
-Version: 0.5.1
+Version: 0.5.2
 Summary: A tool to standardize audiobook files into single m4b files with clean metadata based on Audible and chapters.
 Home-page: https://github.com/djdembeck/m4b-merge
 Author: David Dembeck
 Author-email: dembeck.david@protonmail.com
 Project-URL: Bug Tracker, https://github.com/djdembeck/m4b-merge/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `m4b-merge-0.5.1/src/m4b_merge.egg-info/SOURCES.txt` & `m4b-merge-0.5.2/src/m4b_merge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/tests/test_audible.py` & `m4b-merge-0.5.2/tests/test_audible.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/tests/test_multiple_m4b_merge.py` & `m4b-merge-0.5.2/tests/test_multiple_m4b_merge.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/tests/test_multiple_mp3_merge.py` & `m4b-merge-0.5.2/tests/test_multiple_mp3_merge.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/tests/test_single_m4b_merge.py` & `m4b-merge-0.5.2/tests/test_single_m4b_merge.py`

 * *Files identical despite different names*

### Comparing `m4b-merge-0.5.1/tests/test_single_mp3_merge.py` & `m4b-merge-0.5.2/tests/test_single_mp3_merge.py`

 * *Files identical despite different names*

