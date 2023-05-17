# Comparing `tmp/PyLexia-1.14.tar.gz` & `tmp/PyLexia-1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLexia-1.14.tar", last modified: Wed May 17 07:59:27 2023, max compression
+gzip compressed data, was "PyLexia-1.15.tar", last modified: Wed May 17 08:08:06 2023, max compression
```

## Comparing `PyLexia-1.14.tar` & `PyLexia-1.15.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:59:27.272296 PyLexia-1.14/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:59:27.272296 PyLexia-1.14/PKG-INFO
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:59:27.272296 PyLexia-1.14/PyLexia/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.14/PyLexia/__init__.py
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.14/PyLexia/pylexia.py
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:59:27.272296 PyLexia-1.14/PyLexia.egg-info/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:59:27.000000 PyLexia-1.14/PyLexia.egg-info/PKG-INFO
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      181 2023-05-17 07:59:27.000000 PyLexia-1.14/PyLexia.egg-info/SOURCES.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 07:59:27.000000 PyLexia-1.14/PyLexia.egg-info/dependency_links.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        8 2023-05-17 07:59:27.000000 PyLexia-1.14/PyLexia.egg-info/top_level.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.14/README.md
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 07:59:27.272296 PyLexia-1.14/setup.cfg
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      211 2023-05-17 07:59:08.000000 PyLexia-1.14/setup.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 08:08:06.663362 PyLexia-1.15/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 08:08:06.663362 PyLexia-1.15/PKG-INFO
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 08:08:06.663362 PyLexia-1.15/PyLexia/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.15/PyLexia/__init__.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.15/PyLexia/pylexia.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 08:08:06.663362 PyLexia-1.15/PyLexia.egg-info/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 08:08:06.000000 PyLexia-1.15/PyLexia.egg-info/PKG-INFO
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      181 2023-05-17 08:08:06.000000 PyLexia-1.15/PyLexia.egg-info/SOURCES.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 08:08:06.000000 PyLexia-1.15/PyLexia.egg-info/dependency_links.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        8 2023-05-17 08:08:06.000000 PyLexia-1.15/PyLexia.egg-info/top_level.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.15/README.md
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 08:08:06.663362 PyLexia-1.15/setup.cfg
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      211 2023-05-17 08:07:29.000000 PyLexia-1.15/setup.py
```

