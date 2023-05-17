# Comparing `tmp/PyLexia-1.16.tar.gz` & `tmp/PyLexia-1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLexia-1.16.tar", last modified: Wed May 17 08:42:33 2023, max compression
+gzip compressed data, was "PyLexia-1.17.tar", last modified: Wed May 17 09:29:40 2023, max compression
```

## Comparing `PyLexia-1.16.tar` & `PyLexia-1.17.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 08:42:33.202897 PyLexia-1.16/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 08:42:33.202897 PyLexia-1.16/PKG-INFO
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 08:42:33.202897 PyLexia-1.16/PyLexia/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.16/PyLexia/__init__.py
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.16/PyLexia/pylexia.py
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 08:42:33.202897 PyLexia-1.16/PyLexia.egg-info/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 08:42:33.000000 PyLexia-1.16/PyLexia.egg-info/PKG-INFO
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      181 2023-05-17 08:42:33.000000 PyLexia-1.16/PyLexia.egg-info/SOURCES.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 08:42:33.000000 PyLexia-1.16/PyLexia.egg-info/dependency_links.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 08:42:33.000000 PyLexia-1.16/PyLexia.egg-info/top_level.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.16/README.md
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 08:42:33.202897 PyLexia-1.16/setup.cfg
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      227 2023-05-17 08:42:20.000000 PyLexia-1.16/setup.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:29:40.056344 PyLexia-1.17/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 09:29:40.056344 PyLexia-1.17/PKG-INFO
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:29:40.056344 PyLexia-1.17/PyLexia/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.17/PyLexia/__init__.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.17/PyLexia/pylexia.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 09:29:40.056344 PyLexia-1.17/PyLexia.egg-info/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 09:29:40.000000 PyLexia-1.17/PyLexia.egg-info/PKG-INFO
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      181 2023-05-17 09:29:40.000000 PyLexia-1.17/PyLexia.egg-info/SOURCES.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 09:29:40.000000 PyLexia-1.17/PyLexia.egg-info/dependency_links.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        8 2023-05-17 09:29:40.000000 PyLexia-1.17/PyLexia.egg-info/top_level.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.17/README.md
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 09:29:40.056344 PyLexia-1.17/setup.cfg
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      211 2023-05-17 08:46:47.000000 PyLexia-1.17/setup.py
```

