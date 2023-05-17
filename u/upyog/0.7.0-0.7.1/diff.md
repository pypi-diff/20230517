# Comparing `tmp/upyog-0.7.0.tar.gz` & `tmp/upyog-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyog-0.7.0.tar", last modified: Wed May 17 12:31:59 2023, max compression
+gzip compressed data, was "upyog-0.7.1.tar", last modified: Wed May 17 16:23:48 2023, max compression
```

## Comparing `upyog-0.7.0.tar` & `upyog-0.7.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.094256 upyog-0.7.0/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3233 2023-05-17 11:29:51.000000 upyog-0.7.0/CHANGELOG.md
--rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.0/MANIFEST.in
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 12:31:59.094352 upyog-0.7.0/PKG-INFO
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.0/README.md
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.085903 upyog-0.7.0/assets/
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.087566 upyog-0.7.0/assets/fonts/
--rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.0/assets/fonts/EuroStyleNormal.ttf
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1384 2023-05-17 12:31:59.094823 upyog-0.7.0/setup.cfg
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.0/setup.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.088538 upyog-0.7.0/upyog/
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.0/upyog/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.0/upyog/all.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.089989 upyog-0.7.0/upyog/ann/
--rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.0/upyog/ann/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.0/upyog/ann/annoy.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.0/upyog/cli.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.091242 upyog-0.7.0/upyog/image/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.0/upyog/image/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.0/upyog/image/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.0/upyog/image/composition.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    17228 2023-03-06 08:32:51.000000 upyog-0.7.0/upyog/image/draw.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.0/upyog/image/io.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.0/upyog/image/pil_operators.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.0/upyog/image/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.0/upyog/image/visualiser.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1159 2023-05-17 11:27:01.000000 upyog-0.7.0/upyog/imports.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.092389 upyog-0.7.0/upyog/ml/
--rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2023-05-17 10:38:37.000000 upyog-0.7.0/upyog/ml/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1419 2023-05-17 11:40:18.000000 upyog-0.7.0/upyog/ml/coreml_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1616 2023-05-17 11:20:19.000000 upyog-0.7.0/upyog/ml/eval_dataset.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      325 2023-05-17 11:22:12.000000 upyog-0.7.0/upyog/ml/imports.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1363 2023-05-17 11:08:40.000000 upyog-0.7.0/upyog/ml/model_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.0/upyog/ml/preprocessing.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1230 2023-05-17 11:25:25.000000 upyog-0.7.0/upyog/ml/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1138 2023-05-17 11:07:07.000000 upyog-0.7.0/upyog/ml/visualise.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.0/upyog/nb2script.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.093219 upyog-0.7.0/upyog/os/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.0/upyog/os/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.0/upyog/os/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.0/upyog/os/patch_pathlib.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3356 2022-10-26 00:24:37.000000 upyog-0.7.0/upyog/os/read_files.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.0/upyog/os/utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.094140 upyog-0.7.0/upyog/utils/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.7.0/upyog/utils/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.0/upyog/utils/boxes.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.0/upyog/utils/download.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.0/upyog/utils/prettify_df.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-04-16 03:45:58.000000 upyog-0.7.0/upyog/utils/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.0/upyog/utils/zip_utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.089729 upyog-0.7.0/upyog.egg-info/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/PKG-INFO
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1022 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/SOURCES.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/dependency_links.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/entry_points.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.0/upyog.egg-info/not-zip-safe
--rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/requires.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/top_level.txt
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.477124 upyog-0.7.1/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3412 2023-05-17 16:23:22.000000 upyog-0.7.1/CHANGELOG.md
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.1/MANIFEST.in
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 16:23:48.477207 upyog-0.7.1/PKG-INFO
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.1/README.md
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.468932 upyog-0.7.1/assets/
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.470354 upyog-0.7.1/assets/fonts/
+-rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.1/assets/fonts/EuroStyleNormal.ttf
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1384 2023-05-17 16:23:48.477600 upyog-0.7.1/setup.cfg
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.1/setup.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.471089 upyog-0.7.1/upyog/
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.1/upyog/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.1/upyog/all.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.472406 upyog-0.7.1/upyog/ann/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.1/upyog/ann/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.1/upyog/ann/annoy.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.1/upyog/cli.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.473948 upyog-0.7.1/upyog/image/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.1/upyog/image/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.1/upyog/image/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.1/upyog/image/composition.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    17228 2023-03-06 08:32:51.000000 upyog-0.7.1/upyog/image/draw.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.1/upyog/image/io.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.1/upyog/image/pil_operators.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.1/upyog/image/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.1/upyog/image/visualiser.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1306 2023-05-17 15:42:19.000000 upyog-0.7.1/upyog/imports.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.475291 upyog-0.7.1/upyog/ml/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      211 2023-05-17 15:36:44.000000 upyog-0.7.1/upyog/ml/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1419 2023-05-17 11:40:18.000000 upyog-0.7.1/upyog/ml/coreml_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1626 2023-05-17 15:35:49.000000 upyog-0.7.1/upyog/ml/eval_dataset.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      438 2023-05-17 15:42:14.000000 upyog-0.7.1/upyog/ml/imports.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3662 2023-05-17 16:21:13.000000 upyog-0.7.1/upyog/ml/model_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.1/upyog/ml/preprocessing.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1230 2023-05-17 11:25:25.000000 upyog-0.7.1/upyog/ml/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1138 2023-05-17 11:07:07.000000 upyog-0.7.1/upyog/ml/visualise.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.1/upyog/nb2script.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.476066 upyog-0.7.1/upyog/os/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.1/upyog/os/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.1/upyog/os/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.1/upyog/os/patch_pathlib.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3356 2022-10-26 00:24:37.000000 upyog-0.7.1/upyog/os/read_files.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.1/upyog/os/utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.476968 upyog-0.7.1/upyog/utils/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.7.1/upyog/utils/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.1/upyog/utils/boxes.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.1/upyog/utils/download.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.1/upyog/utils/prettify_df.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-04-16 03:45:58.000000 upyog-0.7.1/upyog/utils/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.1/upyog/utils/zip_utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 16:23:48.472107 upyog-0.7.1/upyog.egg-info/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/PKG-INFO
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1022 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/entry_points.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.1/upyog.egg-info/not-zip-safe
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/requires.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-05-17 16:23:48.000000 upyog-0.7.1/upyog.egg-info/top_level.txt
```

### Comparing `upyog-0.7.0/CHANGELOG.md` & `upyog-0.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 ## Unreleased
+
+## 0.7.1 -- 17 May 2023
+* Rename `InferenceDataset` to `ImageInferenceDataset`
+* Clean up imports
+* Add some more ML functionality from private packages
+
+## 0.7.0 -- 17 May 2023
 * Improve `move-files` and `generate-image-grid` CLI programs
 * Add new `ml` sub-package, copying over a bunch of common utilities across multiple private libraries
 
 ## 0.6.2 -- 11 Apr 2023
 * Myriad bugfixes
 
 ## 0.6.1 -- 6 Mar 2023
```

### Comparing `upyog-0.7.0/PKG-INFO` & `upyog-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.0
+Version: 0.7.1
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.0/README.md` & `upyog-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/assets/fonts/EuroStyleNormal.ttf` & `upyog-0.7.1/assets/fonts/EuroStyleNormal.ttf`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/setup.cfg` & `upyog-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = upyog
-version = 0.7.0
+version = 0.7.1
 author = Rahul Somani
 author_email = rsomani95@gmail.com
 description = Myriad Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = utilities
 license = MIT
```

### Comparing `upyog-0.7.0/upyog/all.py` & `upyog-0.7.1/upyog/all.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/ann/annoy.py` & `upyog-0.7.1/upyog/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/cli.py` & `upyog-0.7.1/upyog/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/image/cli.py` & `upyog-0.7.1/upyog/image/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/image/composition.py` & `upyog-0.7.1/upyog/image/composition.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/image/draw.py` & `upyog-0.7.1/upyog/image/draw.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/image/io.py` & `upyog-0.7.1/upyog/image/io.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/image/pil_operators.py` & `upyog-0.7.1/upyog/image/pil_operators.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/image/utils.py` & `upyog-0.7.1/upyog/image/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/image/visualiser.py` & `upyog-0.7.1/upyog/image/visualiser.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/imports.py` & `upyog-0.7.1/upyog/imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import enum
 import functools
+import importlib
 import io
 import inspect
 import json
 import math
 import mimetypes
 import operator
 import os
@@ -49,7 +50,12 @@
 from tqdm.auto import tqdm
 from typing_extensions import Literal
 
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 PathLike = Union[str, Path]
 
 logger = logger.opt(colors=True)
+
+def is_package_available(name: str) -> bool:
+    if importlib.util.find_spec(name):
+          return True
+    else: return False
```

### Comparing `upyog-0.7.0/upyog/ml/coreml_utils.py` & `upyog-0.7.1/upyog/ml/coreml_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/ml/eval_dataset.py` & `upyog-0.7.1/upyog/ml/eval_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from upyog.ml.imports import *
 from upyog.os import get_image_files
 from upyog.image import load_image
 
 
-__all__ = ["InferenceDataset"]
+__all__ = ["ImageInferenceDataset"]
 
 
-class InferenceDataset(Dataset, ABC):
+class ImageInferenceDataset(Dataset, ABC):
     """
     Base class that gathers files from a myriad number of folders / lists of
     filenames and stores them as `self.fnames`.
 
     Subclasses must implement the `__getitem__` method with the appropriate
     preprocessing for the model
     """
```

### Comparing `upyog-0.7.0/upyog/ml/preprocessing.py` & `upyog-0.7.1/upyog/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/ml/utils.py` & `upyog-0.7.1/upyog/ml/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/ml/visualise.py` & `upyog-0.7.1/upyog/ml/visualise.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/nb2script.py` & `upyog-0.7.1/upyog/nb2script.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/os/cli.py` & `upyog-0.7.1/upyog/os/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/os/read_files.py` & `upyog-0.7.1/upyog/os/read_files.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/os/utils.py` & `upyog-0.7.1/upyog/os/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/utils/download.py` & `upyog-0.7.1/upyog/utils/download.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/utils/prettify_df.py` & `upyog-0.7.1/upyog/utils/prettify_df.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/utils/utils.py` & `upyog-0.7.1/upyog/utils/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog/utils/zip_utils.py` & `upyog-0.7.1/upyog/utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.0/upyog.egg-info/PKG-INFO` & `upyog-0.7.1/upyog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.0
+Version: 0.7.1
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.0/upyog.egg-info/SOURCES.txt` & `upyog-0.7.1/upyog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

