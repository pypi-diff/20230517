# Comparing `tmp/georelate-0.0.0.tar.gz` & `tmp/georelate-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georelate-0.0.0.tar", max compression
+gzip compressed data, was "georelate-0.0.1.tar", max compression
```

## Comparing `georelate-0.0.0.tar` & `georelate-0.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-05-17 15:20:35.379129 georelate-0.0.0/LICENSE
--rw-r--r--   0        0        0        0 2023-05-17 15:20:35.379892 georelate-0.0.0/georelate/__init__.py
--rw-r--r--   0        0        0      189 2023-05-17 15:20:35.380043 georelate-0.0.0/georelate/demo.py
--rw-r--r--   0        0        0      415 2023-05-17 15:59:34.557796 georelate-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 georelate-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-17 15:20:35.379129 georelate-0.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-17 15:20:35.379892 georelate-0.0.1/georelate/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-17 15:20:35.380043 georelate-0.0.1/georelate/demo.py
+-rw-r--r--   0        0        0      415 2023-05-17 16:14:57.913346 georelate-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 georelate-0.0.1/PKG-INFO
```

### Comparing `georelate-0.0.0/LICENSE` & `georelate-0.0.1/LICENSE`

 * *Files identical despite different names*

