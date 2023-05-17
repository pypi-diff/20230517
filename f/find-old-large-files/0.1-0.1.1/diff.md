# Comparing `tmp/find_old_large_files-0.1.tar.gz` & `tmp/find_old_large_files-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.1.tar", last modified: Wed May 17 20:46:55 2023, max compression
+gzip compressed data, was "find_old_large_files-0.1.1.tar", last modified: Wed May 17 20:59:08 2023, max compression
```

## Comparing `find_old_large_files-0.1.tar` & `find_old_large_files-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:46:55.984611 find_old_large_files-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 20:46:39.000000 find_old_large_files-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-17 20:46:55.980611 find_old_large_files-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-17 20:46:39.000000 find_old_large_files-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:46:55.980611 find_old_large_files-0.1/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 20:46:39.000000 find_old_large_files-0.1/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-17 20:46:39.000000 find_old_large_files-0.1/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:46:55.980611 find_old_large_files-0.1/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-17 20:46:55.000000 find_old_large_files-0.1/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-17 20:46:55.000000 find_old_large_files-0.1/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:46:55.000000 find_old_large_files-0.1/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 20:46:55.000000 find_old_large_files-0.1/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 20:46:55.000000 find_old_large_files-0.1/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:46:55.984611 find_old_large_files-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 20:46:39.000000 find_old_large_files-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:59:08.439686 find_old_large_files-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 20:58:51.000000 find_old_large_files-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 20:59:08.439686 find_old_large_files-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-17 20:58:51.000000 find_old_large_files-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:59:08.439686 find_old_large_files-0.1.1/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 20:58:51.000000 find_old_large_files-0.1.1/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-17 20:58:51.000000 find_old_large_files-0.1.1/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:59:08.439686 find_old_large_files-0.1.1/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 20:59:08.000000 find_old_large_files-0.1.1/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-17 20:59:08.000000 find_old_large_files-0.1.1/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:59:08.000000 find_old_large_files-0.1.1/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 20:59:08.000000 find_old_large_files-0.1.1/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 20:59:08.000000 find_old_large_files-0.1.1/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:59:08.439686 find_old_large_files-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-17 20:58:51.000000 find_old_large_files-0.1.1/setup.py
```

### Comparing `find_old_large_files-0.1/LICENSE` & `find_old_large_files-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.1/PKG-INFO` & `find_old_large_files-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.1
+Version: 0.1.1
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.1/README.md` & `find_old_large_files-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.1/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.1.1/find_old_large_files/find_old_large_files.py`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.1/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.1.1/find_old_large_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.1
+Version: 0.1.1
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.1/setup.py` & `find_old_large_files-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.1",
+    version="0.1.1",  # Increment the version here
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
     author="Disant Upadhyay",
```

