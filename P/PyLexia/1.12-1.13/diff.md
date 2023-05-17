# Comparing `tmp/PyLexia-1.12.tar.gz` & `tmp/PyLexia-1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLexia-1.12.tar", last modified: Wed May 17 07:53:47 2023, max compression
+gzip compressed data, was "PyLexia-1.13.tar", last modified: Wed May 17 07:56:50 2023, max compression
```

## Comparing `PyLexia-1.12.tar` & `PyLexia-1.13.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:53:47.970380 PyLexia-1.12/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:53:47.970380 PyLexia-1.12/PKG-INFO
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:53:47.970380 PyLexia-1.12/PyLexia/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.12/PyLexia/__init__.py
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:53:47.970380 PyLexia-1.12/PyLexia.egg-info/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:53:47.000000 PyLexia-1.12/PyLexia.egg-info/PKG-INFO
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      162 2023-05-17 07:53:47.000000 PyLexia-1.12/PyLexia.egg-info/SOURCES.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 07:53:47.000000 PyLexia-1.12/PyLexia.egg-info/dependency_links.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 07:53:47.000000 PyLexia-1.12/PyLexia.egg-info/top_level.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.12/README.md
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 07:53:47.970380 PyLexia-1.12/setup.cfg
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      233 2023-05-17 07:52:54.000000 PyLexia-1.12/setup.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:56:50.603728 PyLexia-1.13/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:56:50.603728 PyLexia-1.13/PKG-INFO
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:56:50.603728 PyLexia-1.13/PyLexia/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.13/PyLexia/__init__.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.13/PyLexia/pylexia.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:56:50.603728 PyLexia-1.13/PyLexia.egg-info/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:56:50.000000 PyLexia-1.13/PyLexia.egg-info/PKG-INFO
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      181 2023-05-17 07:56:50.000000 PyLexia-1.13/PyLexia.egg-info/SOURCES.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 07:56:50.000000 PyLexia-1.13/PyLexia.egg-info/dependency_links.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        8 2023-05-17 07:56:50.000000 PyLexia-1.13/PyLexia.egg-info/top_level.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.13/README.md
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 07:56:50.603728 PyLexia-1.13/setup.cfg
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      211 2023-05-17 07:56:24.000000 PyLexia-1.13/setup.py
```

