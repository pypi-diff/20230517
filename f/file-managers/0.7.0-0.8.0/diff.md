# Comparing `tmp/file-managers-0.7.0.tar.gz` & `tmp/file-managers-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-managers-0.7.0.tar", last modified: Wed May 17 07:49:05 2023, max compression
+gzip compressed data, was "file-managers-0.8.0.tar", last modified: Wed May 17 08:11:44 2023, max compression
```

## Comparing `file-managers-0.7.0.tar` & `file-managers-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:49:05.228365 file-managers-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 07:49:05.228365 file-managers-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-17 07:48:57.000000 file-managers-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:49:05.224365 file-managers-0.7.0/file_managers/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 07:48:57.000000 file-managers-0.7.0/file_managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:49:05.228365 file-managers-0.7.0/file_managers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:49:05.228365 file-managers-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-17 07:48:57.000000 file-managers-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:44.616163 file-managers-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 08:11:44.616163 file-managers-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-17 08:11:34.000000 file-managers-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:44.612163 file-managers-0.8.0/file_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 08:11:34.000000 file-managers-0.8.0/file_managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:44.616163 file-managers-0.8.0/file_managers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 08:11:44.000000 file-managers-0.8.0/file_managers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-17 08:11:44.000000 file-managers-0.8.0/file_managers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:11:44.000000 file-managers-0.8.0/file_managers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 08:11:44.000000 file-managers-0.8.0/file_managers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 08:11:44.000000 file-managers-0.8.0/file_managers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 08:11:44.616163 file-managers-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-17 08:11:34.000000 file-managers-0.8.0/setup.py
```

### Comparing `file-managers-0.7.0/setup.py` & `file-managers-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='file-managers',
-    version='0.7.0',
+    version='0.8.0',
     author='Md. Musfiqur Rahaman',
     author_email='musfiqur.rahaman@northsouth.edu',
     description='A Python Package to manage your files and folders easily in different ways.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['file_managers'],
     install_requires=['twine', 'wheel'],
```

