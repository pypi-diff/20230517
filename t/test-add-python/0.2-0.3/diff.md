# Comparing `tmp/test_add_python-0.2.tar.gz` & `tmp/test_add_python-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_add_python-0.2.tar", last modified: Wed May 17 15:02:54 2023, max compression
+gzip compressed data, was "test_add_python-0.3.tar", last modified: Wed May 17 15:06:13 2023, max compression
```

## Comparing `test_add_python-0.2.tar` & `test_add_python-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:02:54.750240 test_add_python-0.2/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.2/MANIFEST.in
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      140 2023-05-17 15:02:54.750240 test_add_python-0.2/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.2/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.2/pyproject.toml
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:02:54.750240 test_add_python-0.2/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     4996 2023-05-17 15:02:49.000000 test_add_python-0.2/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:02:54.750240 test_add_python-0.2/src/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.2/src/test_add.cu
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.2/src/test_add.hh
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.2/src/test_add_cpu.cpp
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.2/src/test_add_cpu.hpp
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:02:54.750240 test_add_python-0.2/test_add_python.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      140 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.2/test_add_python.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.2/test_add_wrapper.pyx
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:06:13.920522 test_add_python-0.3/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.3/MANIFEST.in
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1918 2023-05-17 15:06:13.920522 test_add_python-0.3/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.3/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.3/pyproject.toml
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:06:13.920522 test_add_python-0.3/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     6832 2023-05-17 15:06:03.000000 test_add_python-0.3/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:06:13.916522 test_add_python-0.3/src/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.3/src/test_add.cu
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.3/src/test_add.hh
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.3/src/test_add_cpu.cpp
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.3/src/test_add_cpu.hpp
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:06:13.920522 test_add_python-0.3/test_add_python.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1918 2023-05-17 15:06:13.000000 test_add_python-0.3/test_add_python.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:06:13.000000 test_add_python-0.3/test_add_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:06:13.000000 test_add_python-0.3/test_add_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.3/test_add_python.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:06:13.000000 test_add_python-0.3/test_add_python.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.3/test_add_wrapper.pyx
```

### Comparing `test_add_python-0.2/README.md` & `test_add_python-0.3/README.md`

 * *Files identical despite different names*

### Comparing `test_add_python-0.2/src/test_add.cu` & `test_add_python-0.3/src/test_add.cu`

 * *Files identical despite different names*

### Comparing `test_add_python-0.2/src/test_add_cpu.cpp` & `test_add_python-0.3/src/test_add_cpu.cpp`

 * *Files identical despite different names*

### Comparing `test_add_python-0.2/test_add_wrapper.pyx` & `test_add_python-0.3/test_add_wrapper.pyx`

 * *Files identical despite different names*

