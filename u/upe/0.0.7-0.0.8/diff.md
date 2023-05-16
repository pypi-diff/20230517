# Comparing `tmp/upe-0.0.7.tar.gz` & `tmp/upe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upe-0.0.7.tar", last modified: Tue May 16 22:16:19 2023, max compression
+gzip compressed data, was "upe-0.0.8.tar", last modified: Tue May 16 22:20:28 2023, max compression
```

## Comparing `upe-0.0.7.tar` & `upe-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:16:19.990922 upe-0.0.7/
--rw-rw-rw-   0        0        0      191 2023-05-16 22:16:19.990922 upe-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 22:16:19.976740 upe-0.0.7/libname/
--rw-rw-rw-   0        0        0       53 2023-05-16 22:02:41.000000 upe-0.0.7/libname/__init__.py
--rw-rw-rw-   0        0        0    55734 2023-05-16 22:14:54.000000 upe-0.0.7/libname/cdlab.py
--rw-rw-rw-   0        0        0    30036 2023-05-16 20:15:16.000000 upe-0.0.7/libname/nqueen.py
--rw-rw-rw-   0        0        0       42 2023-05-16 22:16:19.990922 upe-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      428 2023-05-16 22:15:12.000000 upe-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:16:19.988921 upe-0.0.7/upe.egg-info/
--rw-rw-rw-   0        0        0      191 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 22:20:28.974044 upe-0.0.8/
+-rw-rw-rw-   0        0        0      191 2023-05-16 22:20:28.974044 upe-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 22:20:28.957083 upe-0.0.8/libname/
+-rw-rw-rw-   0        0        0       26 2023-05-16 22:20:20.000000 upe-0.0.8/libname/__init__.py
+-rw-rw-rw-   0        0        0    30036 2023-05-16 20:15:16.000000 upe-0.0.8/libname/nqueen.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:20:28.974044 upe-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      428 2023-05-16 22:19:54.000000 upe-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:20:28.972044 upe-0.0.8/upe.egg-info/
+-rw-rw-rw-   0        0        0      191 2023-05-16 22:20:28.000000 upe-0.0.8/upe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-05-16 22:20:28.000000 upe-0.0.8/upe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:20:28.000000 upe-0.0.8/upe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 22:20:28.000000 upe-0.0.8/upe.egg-info/top_level.txt
```

### Comparing `upe-0.0.7/libname/nqueen.py` & `upe-0.0.8/libname/nqueen.py`

 * *Files identical despite different names*

