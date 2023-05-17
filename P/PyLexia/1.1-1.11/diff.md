# Comparing `tmp/PyLexia-1.1.tar.gz` & `tmp/PyLexia-1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLexia-1.1.tar", last modified: Wed May 17 07:28:03 2023, max compression
+gzip compressed data, was "PyLexia-1.11.tar", last modified: Wed May 17 07:44:52 2023, max compression
```

## Comparing `PyLexia-1.1.tar` & `PyLexia-1.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:28:03.405744 PyLexia-1.1/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       68 2023-05-17 07:28:03.405744 PyLexia-1.1/PKG-INFO
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:28:03.405744 PyLexia-1.1/PyLexia/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-16 11:31:18.000000 PyLexia-1.1/PyLexia/Experimental.py
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.1/PyLexia/__init__.py
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.1/PyLexia/app.py
-drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:28:03.405744 PyLexia-1.1/PyLexia.egg-info/
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       68 2023-05-17 07:28:03.000000 PyLexia-1.1/PyLexia.egg-info/PKG-INFO
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      201 2023-05-17 07:28:03.000000 PyLexia-1.1/PyLexia.egg-info/SOURCES.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 07:28:03.000000 PyLexia-1.1/PyLexia.egg-info/dependency_links.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)        8 2023-05-17 07:28:03.000000 PyLexia-1.1/PyLexia.egg-info/top_level.txt
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.1/README.md
--rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 07:28:03.405744 PyLexia-1.1/setup.cfg
--rw-rw-r--   0 lexia     (1000) lexia     (1000)      210 2023-05-17 07:23:57.000000 PyLexia-1.1/setup.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:44:52.658765 PyLexia-1.11/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:44:52.658765 PyLexia-1.11/PKG-INFO
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:44:52.658765 PyLexia-1.11/PyLexia/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-16 11:31:18.000000 PyLexia-1.11/PyLexia/Experimental.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        0 2023-05-03 19:37:53.000000 PyLexia-1.11/PyLexia/__init__.py
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       37 2023-05-03 19:56:14.000000 PyLexia-1.11/PyLexia/app.py
+drwxrwxr-x   0 lexia     (1000) lexia     (1000)        0 2023-05-17 07:44:52.658765 PyLexia-1.11/PyLexia.egg-info/
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       69 2023-05-17 07:44:52.000000 PyLexia-1.11/PyLexia.egg-info/PKG-INFO
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      201 2023-05-17 07:44:52.000000 PyLexia-1.11/PyLexia.egg-info/SOURCES.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 07:44:52.000000 PyLexia-1.11/PyLexia.egg-info/dependency_links.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)        1 2023-05-17 07:44:52.000000 PyLexia-1.11/PyLexia.egg-info/top_level.txt
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       18 2023-05-03 19:54:40.000000 PyLexia-1.11/README.md
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)       38 2023-05-17 07:44:52.658765 PyLexia-1.11/setup.cfg
+-rw-rw-r--   0 lexia     (1000) lexia     (1000)      233 2023-05-17 07:44:14.000000 PyLexia-1.11/setup.py
```

