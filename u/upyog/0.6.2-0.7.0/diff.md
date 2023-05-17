# Comparing `tmp/upyog-0.6.2.tar.gz` & `tmp/upyog-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyog-0.6.2.tar", last modified: Tue Apr 11 17:05:12 2023, max compression
+gzip compressed data, was "upyog-0.7.0.tar", last modified: Wed May 17 12:31:59 2023, max compression
```

## Comparing `upyog-0.6.2.tar` & `upyog-0.7.0.tar`

### file list

```diff
@@ -1,49 +1,58 @@
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.692442 upyog-0.6.2/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3053 2023-04-11 17:04:59.000000 upyog-0.6.2/CHANGELOG.md
--rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.6.2/MANIFEST.in
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-04-11 17:05:12.692537 upyog-0.6.2/PKG-INFO
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.6.2/README.md
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.686092 upyog-0.6.2/assets/
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.687449 upyog-0.6.2/assets/fonts/
--rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.6.2/assets/fonts/EuroStyleNormal.ttf
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1300 2023-04-11 17:05:12.692967 upyog-0.6.2/setup.cfg
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.6.2/setup.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.688433 upyog-0.6.2/upyog/
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.6.2/upyog/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.6.2/upyog/all.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.689791 upyog-0.6.2/upyog/ann/
--rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.6.2/upyog/ann/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.6.2/upyog/ann/annoy.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3040 2023-01-31 06:04:25.000000 upyog-0.6.2/upyog/cli.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.690908 upyog-0.6.2/upyog/image/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.6.2/upyog/image/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3037 2022-01-19 13:36:07.000000 upyog-0.6.2/upyog/image/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.6.2/upyog/image/composition.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    17228 2023-03-06 08:32:51.000000 upyog-0.6.2/upyog/image/draw.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1305 2022-03-25 10:21:09.000000 upyog-0.6.2/upyog/image/io.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.6.2/upyog/image/pil_operators.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1159 2023-02-28 09:04:22.000000 upyog-0.6.2/upyog/image/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.6.2/upyog/image/visualiser.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1102 2023-03-06 08:33:02.000000 upyog-0.6.2/upyog/imports.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.6.2/upyog/nb2script.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.691554 upyog-0.6.2/upyog/os/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.6.2/upyog/os/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     6196 2023-04-11 16:53:41.000000 upyog-0.6.2/upyog/os/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.6.2/upyog/os/patch_pathlib.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3356 2022-10-26 00:24:37.000000 upyog-0.6.2/upyog/os/read_files.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3149 2023-04-11 16:54:06.000000 upyog-0.6.2/upyog/os/utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.692323 upyog-0.6.2/upyog/utils/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.6.2/upyog/utils/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.6.2/upyog/utils/boxes.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.6.2/upyog/utils/download.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.6.2/upyog/utils/prettify_df.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-01-09 14:47:17.000000 upyog-0.6.2/upyog/utils/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.6.2/upyog/utils/zip_utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.689540 upyog-0.6.2/upyog.egg-info/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/PKG-INFO
--rw-r--r--   0 rahulsomani   (501) staff       (20)      841 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/SOURCES.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/dependency_links.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/entry_points.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.6.2/upyog.egg-info/not-zip-safe
--rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/requires.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/top_level.txt
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.094256 upyog-0.7.0/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3233 2023-05-17 11:29:51.000000 upyog-0.7.0/CHANGELOG.md
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.0/MANIFEST.in
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 12:31:59.094352 upyog-0.7.0/PKG-INFO
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.0/README.md
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.085903 upyog-0.7.0/assets/
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.087566 upyog-0.7.0/assets/fonts/
+-rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.0/assets/fonts/EuroStyleNormal.ttf
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1384 2023-05-17 12:31:59.094823 upyog-0.7.0/setup.cfg
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.0/setup.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.088538 upyog-0.7.0/upyog/
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.0/upyog/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.0/upyog/all.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.089989 upyog-0.7.0/upyog/ann/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.0/upyog/ann/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.0/upyog/ann/annoy.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.0/upyog/cli.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.091242 upyog-0.7.0/upyog/image/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.0/upyog/image/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.0/upyog/image/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.0/upyog/image/composition.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    17228 2023-03-06 08:32:51.000000 upyog-0.7.0/upyog/image/draw.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.0/upyog/image/io.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.0/upyog/image/pil_operators.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.0/upyog/image/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.0/upyog/image/visualiser.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1159 2023-05-17 11:27:01.000000 upyog-0.7.0/upyog/imports.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.092389 upyog-0.7.0/upyog/ml/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2023-05-17 10:38:37.000000 upyog-0.7.0/upyog/ml/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1419 2023-05-17 11:40:18.000000 upyog-0.7.0/upyog/ml/coreml_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1616 2023-05-17 11:20:19.000000 upyog-0.7.0/upyog/ml/eval_dataset.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      325 2023-05-17 11:22:12.000000 upyog-0.7.0/upyog/ml/imports.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1363 2023-05-17 11:08:40.000000 upyog-0.7.0/upyog/ml/model_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.0/upyog/ml/preprocessing.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1230 2023-05-17 11:25:25.000000 upyog-0.7.0/upyog/ml/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1138 2023-05-17 11:07:07.000000 upyog-0.7.0/upyog/ml/visualise.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.0/upyog/nb2script.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.093219 upyog-0.7.0/upyog/os/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.0/upyog/os/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.0/upyog/os/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.0/upyog/os/patch_pathlib.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3356 2022-10-26 00:24:37.000000 upyog-0.7.0/upyog/os/read_files.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.0/upyog/os/utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.094140 upyog-0.7.0/upyog/utils/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.7.0/upyog/utils/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.0/upyog/utils/boxes.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.0/upyog/utils/download.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.0/upyog/utils/prettify_df.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-04-16 03:45:58.000000 upyog-0.7.0/upyog/utils/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.0/upyog/utils/zip_utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-05-17 12:31:59.089729 upyog-0.7.0/upyog.egg-info/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/PKG-INFO
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1022 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/entry_points.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.0/upyog.egg-info/not-zip-safe
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/requires.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-05-17 12:31:59.000000 upyog-0.7.0/upyog.egg-info/top_level.txt
```

### Comparing `upyog-0.6.2/CHANGELOG.md` & `upyog-0.7.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## Unreleased
+* Improve `move-files` and `generate-image-grid` CLI programs
+* Add new `ml` sub-package, copying over a bunch of common utilities across multiple private libraries
+
 ## 0.6.2 -- 11 Apr 2023
 * Myriad bugfixes
 
 ## 0.6.1 -- 6 Mar 2023
 * Fix default font path (hacky but works)
 * Bugfix `write_json`
 * Add `title` func to `Visualiser`
```

### Comparing `upyog-0.6.2/PKG-INFO` & `upyog-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.6.2
+Version: 0.7.0
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.6.2/README.md` & `upyog-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/assets/fonts/EuroStyleNormal.ttf` & `upyog-0.7.0/assets/fonts/EuroStyleNormal.ttf`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/setup.cfg` & `upyog-0.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = upyog
-version = 0.6.2
+version = 0.7.0
 author = Rahul Somani
 author_email = rsomani95@gmail.com
 description = Myriad Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = utilities
 license = MIT
@@ -39,19 +39,19 @@
 	black >=20.8b1,<21
 	pytest >=6,<7
 	jupyter >=1.0.0,<2
 	pre-commit >=2.8.2,<3
 
 [options.entry_points]
 console_scripts = 
-	move-files = upyog.os.cli:move_files
-	remove-duplicates-from-folder = upyog.os.cli:remove_duplicates_from_folder
-	print-folder-distribution = upyog.os.cli:print_folder_distribution
-	generate-image-grid = upyog.image.cli:create_image_grid_from_folders
-	add-parent-folder-name = upyog.os.cli:add_parent_folder_name
+	remove-duplicates-from-folder     = upyog.os.cli:remove_duplicates_from_folder
+	print-folder-distribution         = upyog.os.cli:print_folder_distribution
+	generate-image-grid               = upyog.image.cli:create_image_grid_from_folders
+	add-parent-folder-name            = upyog.os.cli:add_parent_folder_name
+	move-files                        = upyog.os.cli:move_files
 	find-common-files-between-folders = upyog.os.cli:find_common_files_between_folders
-	nb2script = upyog.nb2script:notebook2script
+	nb2script                         = upyog.nb2script:notebook2script
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `upyog-0.6.2/upyog/all.py` & `upyog-0.7.0/upyog/all.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/ann/annoy.py` & `upyog-0.7.0/upyog/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/cli.py` & `upyog-0.7.0/upyog/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 This module makes some adjustments to the default behavior of the excellent
 `fastcore.script` package to easily create functions that can be easily used
 in regular code _and_ for command line interfaces with minimal additional code
 """
 
 from upyog.imports import *
-from fastcore.all import bool_arg
+from fastcore.all import bool_arg, store_true
 
 
-__all__ = ["Param", "P", "call_parse", "bool_arg"]
+__all__ = ["Param", "P", "call_parse", "bool_arg", "store_true"]
 
 
 class Param(fastcore.Param):
     def __init__(
         self,
         help=None,
         type=None,
```

### Comparing `upyog-0.6.2/upyog/image/cli.py` & `upyog-0.7.0/upyog/image/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 @call_parse
 def create_image_grid_from_folders(
     # fmt: off
     i: P("An arbitrary number of inputs folders", str, nargs="+") = None,
     o: P("Output path - must be a folder (created if it doesn't exist)", str) = None,
     H: P("Height of _each_ image inside the grid", int) = 384,
     W: P("Width of each image inside the grid", int) = 640,
+    N: P("(Optional) Max no. of images to select. If not specified, all are selected", int) = None,
     num_columns: P("Number of columns in the grid", int) = 3,
     sample:      P("Random sample this no. of files from the folder", int) = None,
     shuffle:   P("(Bool) shuffle the order of files", action="store_true") = False,
     foreach:     P("(Bool) Create a dedicated grid for _each_ input folder given", action="store_true") = False,
     exp_quality: P("Export quality (0-100). ~85 is a good tradeoff", int) = 85,
     # fmt: on
 ):
@@ -58,23 +59,28 @@
         )
     output_path.mkdir(exist_ok=True)
 
     # Create grids
     if foreach:
         for path in input_paths:
             files = get_image_files(path)
-            grid = make_grid_from_files(files, num_columns, (W, H), sample, shuffle)
-            grid.save(output_path / f"{path.stem}.jpg", quality=exp_quality)
+            grid = make_grid_from_files(files, num_columns, (W, H), sample, shuffle, N)
+
+            export_path = output_path / f"{path.stem}.jpg"
+            grid.save(export_path, quality=exp_quality)
+            rich.print(f"Saved to {export_path}")
     else:
         files = flatten(get_image_files(path) for path in input_paths)
-        grid = make_grid_from_files(files, num_columns, (W, H), sample, shuffle)
-        grid.save(output_path / "Image-Grid.jpg", quality=exp_quality)
+        grid = make_grid_from_files(files, num_columns, (W, H), sample, shuffle, N)
+
+        export_path = output_path / "Image-Grid.jpg"
+        grid.save(export_path, quality=exp_quality)
+        rich.print(f"Saved to {export_path}")
 
 
-def make_grid_from_files(files, ncol, size_WH, sample=None, shuffle=False):
-    if sample:
-        files = random.sample(files, sample)
-    if shuffle:
-        random.shuffle(files)
+def make_grid_from_files(files, ncol, size_WH, sample=None, shuffle=False, N=None):
+    if sample:  files = random.sample(files, sample)
+    if shuffle: random.shuffle(files)
+    if N:       files = files[:N]
 
     imgs = [load_image(fn) for fn in files]
     return make_img_grid(imgs, ncol, size_WH, pad=True)
```

### Comparing `upyog-0.6.2/upyog/image/composition.py` & `upyog-0.7.0/upyog/image/composition.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/image/draw.py` & `upyog-0.7.0/upyog/image/draw.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/image/io.py` & `upyog-0.7.0/upyog/image/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     return min([to_H / H, to_W / W])
 
 
 def resize_with_padding(
     img: Image.Image,
     target_WH,
-    pad_fill=0,
+    pad_fill: Union[int, Tuple[int, int, int]] = 0,
     pad_location: Literal["center", "top"] = "center",
     # mode: str = "RGB",
 ):
     to_W, to_H = target_WH
     W, H = img.size
     orig_mode = img.mode
 
@@ -43,12 +43,18 @@
 
     if pad_location == "top":
         box = (0, 0)
     else:
         box = ((to_W - W) // 2, (to_H - H) // 2)
 
     # Create a new image and paste the resized on it
-    color = (pad_fill, pad_fill, pad_fill) if pad_fill else None
+    if pad_fill:
+        if   isinstance(pad_fill, int):          color = (pad_fill, pad_fill, pad_fill)
+        elif isinstance(pad_fill, (list,tuple)): color = tuple(pad_fill)
+        assert isinstance(color, tuple)
+    else:
+        color = None
+
     padded_img = Image.new(orig_mode, (to_W, to_H), color=color)
     padded_img.paste(img.resize((W, H), Image.ANTIALIAS), box)
 
     return padded_img
```

### Comparing `upyog-0.6.2/upyog/image/pil_operators.py` & `upyog-0.7.0/upyog/image/pil_operators.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/image/utils.py` & `upyog-0.7.0/upyog/image/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from curses import meta
 from upyog.imports import *
 
 # Inspired by https://github.com/gordicaleksa/stable_diffusion_playground/blob/a4508d0650c6940f64b858aa818291cfa0bdad9c/generate_images.py#L84-L97
 def save_image_with_metadata(
     img: Image.Image, metadata: dict, filepath: PathLike
 ):
     """
@@ -29,7 +28,22 @@
     exif_img = exif.Image(
         cv2.imencode(".jpg", np.asarray(img)[..., ::-1])[1].tobytes()
     )
     exif_img.user_comment = json.dumps(metadata)
 
     with open(filepath, "wb") as f:
         f.write(exif_img.get_file())
+
+
+def fig_to_pil(fig, pad_inches: float = 0.25):
+    """
+    Convert a Matplotlib figure to a PIL Image and return it
+    """
+    # Save figure to buf in png format
+    buf = io.BytesIO()
+    fig.savefig(buf, format='png', bbox_inches='tight', pad_inches=pad_inches)
+    buf.seek(0)
+
+    # Convert to PIL Image
+    img = Image.open(buf).convert("RGB")
+    buf.close()
+    return img
```

### Comparing `upyog-0.6.2/upyog/image/visualiser.py` & `upyog-0.7.0/upyog/image/visualiser.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/imports.py` & `upyog-0.7.0/upyog/imports.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import argparse
 import enum
 import functools
+import io
 import inspect
 import json
 import math
 import mimetypes
 import operator
 import os
+import platform
 import random
 import re
 import shutil
 import socket
 import sys
 import time
 import typing
@@ -25,23 +27,24 @@
 from enum import Enum
 from functools import partial, reduce
 from pathlib import Path
 from pprint import pprint
 from types import SimpleNamespace, MethodType
 from typing import *
 from collections import OrderedDict, defaultdict, namedtuple
+from abc import abstractmethod, ABC
 
 import fastcore.all as fastcore
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import PIL
 import pyperclip
 import rich
 
+from fastcore.all import L
 from loguru import logger
 from PIL import Image, ImageDraw, ImageFile, ImageFont
 from PIL import features as PILFeatures
 from rich.progress import track
 from rich.traceback import install
 from tqdm.auto import tqdm
 from typing_extensions import Literal
```

### Comparing `upyog-0.6.2/upyog/nb2script.py` & `upyog-0.7.0/upyog/nb2script.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/os/read_files.py` & `upyog-0.7.0/upyog/os/read_files.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/os/utils.py` & `upyog-0.7.0/upyog/os/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from upyog.imports import *
 from upyog.os.read_files import PathLike, get_files
 
 __all__ = [
     "load_json", "read_json", "check_pil_simd_usage", "sanitise_filename", "get_file_size",
     "get_file_creation_date", "write_json", "write_text",
+    "is_platform_macos", "is_platform_windows", "is_platform_linux",
 ]
 
 
 def load_json(path: PathLike):
     "Load a JSON file"
     return json.loads(Path(path).read_bytes())
 
@@ -94,7 +95,11 @@
     # Get the timestamp of the file's creation date
     timestamp = os.path.getctime(path_to_file)
     
     # Convert the timestamp to a datetime object
     date = datetime.fromtimestamp(timestamp)
     return date.strftime('%Y-%m-%d')
 
+
+def is_platform_macos() -> bool:   return platform.system().lower() == "darwin"
+def is_platform_windows() -> bool: return platform.system().lower() == "windows"
+def is_platform_linux() -> bool:   return platform.system().lower() == "linux"
```

### Comparing `upyog-0.6.2/upyog/utils/download.py` & `upyog-0.7.0/upyog/utils/download.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/utils/prettify_df.py` & `upyog-0.7.0/upyog/utils/prettify_df.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/utils/utils.py` & `upyog-0.7.0/upyog/utils/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog/utils/zip_utils.py` & `upyog-0.7.0/upyog/utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.2/upyog.egg-info/PKG-INFO` & `upyog-0.7.0/upyog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.6.2
+Version: 0.7.0
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.6.2/upyog.egg-info/SOURCES.txt` & `upyog-0.7.0/upyog.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 upyog/image/cli.py
 upyog/image/composition.py
 upyog/image/draw.py
 upyog/image/io.py
 upyog/image/pil_operators.py
 upyog/image/utils.py
 upyog/image/visualiser.py
+upyog/ml/__init__.py
+upyog/ml/coreml_utils.py
+upyog/ml/eval_dataset.py
+upyog/ml/imports.py
+upyog/ml/model_utils.py
+upyog/ml/preprocessing.py
+upyog/ml/utils.py
+upyog/ml/visualise.py
 upyog/os/__init__.py
 upyog/os/cli.py
 upyog/os/patch_pathlib.py
 upyog/os/read_files.py
 upyog/os/utils.py
 upyog/utils/__init__.py
 upyog/utils/boxes.py
```

