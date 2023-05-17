# Comparing `tmp/driveup-0.5.0.tar.gz` & `tmp/driveup-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.5.0.tar", last modified: Fri May 12 11:45:54 2023, max compression
+gzip compressed data, was "driveup-0.6.0.tar", last modified: Wed May 17 13:49:32 2023, max compression
```

## Comparing `driveup-0.5.0.tar` & `driveup-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.997913 driveup-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.993914 driveup-0.5.0/Driveup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/drive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.997913 driveup-0.5.0/Driveup/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-12 11:45:39.000000 driveup-0.5.0/Driveup/features/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 11:45:39.000000 driveup-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 11:45:53.997913 driveup-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 11:45:39.000000 driveup-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:45:53.997913 driveup-0.5.0/driveup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 11:45:53.000000 driveup-0.5.0/driveup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:45:53.997913 driveup-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-12 11:45:39.000000 driveup-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:49:32.528219 driveup-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:49:32.528219 driveup-0.6.0/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:49:19.000000 driveup-0.6.0/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-17 13:49:19.000000 driveup-0.6.0/Driveup/drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:49:32.528219 driveup-0.6.0/Driveup/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:49:19.000000 driveup-0.6.0/Driveup/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-17 13:49:19.000000 driveup-0.6.0/Driveup/features/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 13:49:19.000000 driveup-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-17 13:49:32.528219 driveup-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 13:49:19.000000 driveup-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:49:32.528219 driveup-0.6.0/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-17 13:49:32.000000 driveup-0.6.0/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 13:49:32.000000 driveup-0.6.0/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:49:32.000000 driveup-0.6.0/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 13:49:32.000000 driveup-0.6.0/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 13:49:32.000000 driveup-0.6.0/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:49:32.528219 driveup-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-17 13:49:19.000000 driveup-0.6.0/setup.py
```

### Comparing `driveup-0.5.0/Driveup/features/auth.py` & `driveup-0.6.0/Driveup/features/auth.py`

 * *Files identical despite different names*

### Comparing `driveup-0.5.0/LICENSE` & `driveup-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `driveup-0.5.0/setup.py` & `driveup-0.6.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # ...
 
 setup(
     long_description=README_DESCRIPTION,
     long_description_content_type="text/markdown",
     name='driveup',
-    version='0.5.0',
+    version='0.6.0',
     author='Raúl M.R.',
     author_email="raul.martin4bc@gmail.com",
     url="https://github.com/raul-martin-dev/Driveup",
     license="MIT",
     description='Python package for uploading files and folders to Google Drive.',
     packages=find_packages(include=["Driveup","Driveup.features"]),
     install_requires=[
```

