# Comparing `tmp/test_add_python-0.1.tar.gz` & `tmp/test_add_python-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_add_python-0.1.tar", last modified: Sat May  6 09:28:21 2023, max compression
+gzip compressed data, was "test_add_python-0.2.tar", last modified: Wed May 17 15:02:54 2023, max compression
```

## Comparing `test_add_python-0.1.tar` & `test_add_python-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-06 09:28:21.281404 test_add_python-0.1/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.1/MANIFEST.in
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       82 2023-05-06 09:28:21.281404 test_add_python-0.1/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-05-06 09:24:07.000000 test_add_python-0.1/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.1/pyproject.toml
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-06 09:28:21.281404 test_add_python-0.1/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     4887 2023-05-06 03:22:42.000000 test_add_python-0.1/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-06 09:28:21.281404 test_add_python-0.1/src/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.1/src/test_add.cu
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.1/src/test_add.hh
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.1/src/test_add_cpu.cpp
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.1/src/test_add_cpu.hpp
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-06 09:28:21.281404 test_add_python-0.1/test_add_python.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       82 2023-05-06 09:28:21.000000 test_add_python-0.1/test_add_python.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-06 09:28:21.000000 test_add_python-0.1/test_add_python.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-06 09:28:21.000000 test_add_python-0.1/test_add_python.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-06 09:28:21.000000 test_add_python-0.1/test_add_python.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-06 09:28:21.000000 test_add_python-0.1/test_add_python.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.1/test_add_wrapper.pyx
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:02:54.750240 test_add_python-0.2/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      107 2023-05-06 09:26:23.000000 test_add_python-0.2/MANIFEST.in
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      140 2023-05-17 15:02:54.750240 test_add_python-0.2/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1086 2023-05-06 19:52:27.000000 test_add_python-0.2/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      125 2023-05-06 09:25:05.000000 test_add_python-0.2/pyproject.toml
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-05-17 15:02:54.750240 test_add_python-0.2/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     4996 2023-05-17 15:02:49.000000 test_add_python-0.2/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:02:54.750240 test_add_python-0.2/src/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1478 2023-05-06 05:59:44.000000 test_add_python-0.2/src/test_add.cu
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      151 2023-05-06 06:03:17.000000 test_add_python-0.2/src/test_add.hh
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      674 2023-05-06 09:20:34.000000 test_add_python-0.2/src/test_add_cpu.cpp
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      265 2023-05-06 09:08:49.000000 test_add_python-0.2/src/test_add_cpu.hpp
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-05-17 15:02:54.750240 test_add_python-0.2/test_add_python.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      140 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      334 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-05-17 15:01:01.000000 test_add_python-0.2/test_add_python.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       16 2023-05-17 15:02:54.000000 test_add_python-0.2/test_add_python.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1510 2023-05-06 09:09:07.000000 test_add_python-0.2/test_add_wrapper.pyx
```

### Comparing `test_add_python-0.1/setup.py` & `test_add_python-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,16 +127,19 @@
         )
 
 
 
 setup(name = 'test_add_python',
       # Random metadata. there's more you can supply
       author = 'Dmitry Michaylin',
-      version = '0.1',
-
+      version = '0.2',
+      
+      long_description='### Hello world!',
+      long_description_content_type='text/markdown',
+      
       ext_modules = [ext],
 
       # Inject our custom trigger
       cmdclass = {'build_ext': custom_build_ext},
 
       # Since the package has c code, the egg cannot be zipped
       zip_safe = False)
```

### Comparing `test_add_python-0.1/src/test_add.cu` & `test_add_python-0.2/src/test_add.cu`

 * *Files identical despite different names*

### Comparing `test_add_python-0.1/src/test_add_cpu.cpp` & `test_add_python-0.2/src/test_add_cpu.cpp`

 * *Files identical despite different names*

### Comparing `test_add_python-0.1/test_add_wrapper.pyx` & `test_add_python-0.2/test_add_wrapper.pyx`

 * *Files identical despite different names*

