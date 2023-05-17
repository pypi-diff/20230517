# Comparing `tmp/syscolouringspackage-1.0.0.tar.gz` & `tmp/syscolouringspackage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscolouringspackage-1.0.0.tar", last modified: Wed May 17 21:54:07 2023, max compression
+gzip compressed data, was "syscolouringspackage-1.1.0.tar", last modified: Wed May 17 21:56:13 2023, max compression
```

## Comparing `syscolouringspackage-1.0.0.tar` & `syscolouringspackage-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 21:54:07.548588 syscolouringspackage-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-17 21:54:07.548588 syscolouringspackage-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 21:54:07.548588 syscolouringspackage-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-17 21:54:07.000000 syscolouringspackage-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 21:54:07.548588 syscolouringspackage-1.0.0/syscolouringspackage/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 21:54:07.000000 syscolouringspackage-1.0.0/syscolouringspackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 21:54:07.548588 syscolouringspackage-1.0.0/syscolouringspackage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-17 21:54:07.000000 syscolouringspackage-1.0.0/syscolouringspackage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-17 21:54:07.000000 syscolouringspackage-1.0.0/syscolouringspackage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 21:54:07.000000 syscolouringspackage-1.0.0/syscolouringspackage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 21:54:07.000000 syscolouringspackage-1.0.0/syscolouringspackage.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 21:56:13.339106 syscolouringspackage-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-17 21:56:13.339106 syscolouringspackage-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 21:56:13.339106 syscolouringspackage-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-17 21:56:13.000000 syscolouringspackage-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 21:56:13.339106 syscolouringspackage-1.1.0/syscolouringspackage/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-17 21:56:13.000000 syscolouringspackage-1.1.0/syscolouringspackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 21:56:13.339106 syscolouringspackage-1.1.0/syscolouringspackage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-17 21:56:13.000000 syscolouringspackage-1.1.0/syscolouringspackage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-17 21:56:13.000000 syscolouringspackage-1.1.0/syscolouringspackage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 21:56:13.000000 syscolouringspackage-1.1.0/syscolouringspackage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 21:56:13.000000 syscolouringspackage-1.1.0/syscolouringspackage.egg-info/top_level.txt
```

### Comparing `syscolouringspackage-1.0.0/setup.py` & `syscolouringspackage-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syscolouringspackage",
     version=VERSION,
```

