# Comparing `tmp/amuse-mesa-2023.5.1.tar.gz` & `tmp/amuse-mesa-2023.5.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-mesa-2023.5.1.tar", last modified: Wed May 17 13:03:39 2023, max compression
+gzip compressed data, was "amuse-mesa-2023.5.1.post1.tar", last modified: Wed May 17 13:13:45 2023, max compression
```

## Comparing `amuse-mesa-2023.5.1.tar` & `amuse-mesa-2023.5.1.post1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:03:39.442331 amuse-mesa-2023.5.1/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-mesa-2023.5.1/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1180 2023-05-17 13:03:39.442145 amuse-mesa-2023.5.1/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       57 2022-11-22 11:55:14.000000 amuse-mesa-2023.5.1/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:03:39.440220 amuse-mesa-2023.5.1/amuse_mesa.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1180 2023-05-17 13:03:37.000000 amuse-mesa-2023.5.1/amuse_mesa.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      508 2023-05-17 13:03:39.000000 amuse-mesa-2023.5.1/amuse_mesa.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 13:03:37.000000 amuse-mesa-2023.5.1/amuse_mesa.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 13:03:37.000000 amuse-mesa-2023.5.1/amuse_mesa.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 13:03:37.000000 amuse-mesa-2023.5.1/amuse_mesa.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)      124 2023-05-17 12:59:10.000000 amuse-mesa-2023.5.1/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 13:03:39.442383 amuse-mesa-2023.5.1/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1763 2023-05-17 12:54:40.000000 amuse-mesa-2023.5.1/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:03:39.438891 amuse-mesa-2023.5.1/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:03:39.438948 amuse-mesa-2023.5.1/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:03:39.439002 amuse-mesa-2023.5.1/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:03:39.440629 amuse-mesa-2023.5.1/src/amuse/community/mesa/
--rw-r--r--   0 rieder     (501) staff       (20)       83 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/src/amuse/community/mesa/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      924 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/src/amuse/community/mesa/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 13:03:37.000000 amuse-mesa-2023.5.1/src/amuse/community/mesa/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:03:39.441890 amuse-mesa-2023.5.1/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-mesa-2023.5.1/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-mesa-2023.5.1/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:13:45.532413 amuse-mesa-2023.5.1.post1/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-mesa-2023.5.1.post1/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1276 2023-05-17 13:13:45.532228 amuse-mesa-2023.5.1.post1/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      147 2023-05-17 13:12:13.000000 amuse-mesa-2023.5.1.post1/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:13:45.530095 amuse-mesa-2023.5.1.post1/amuse_mesa.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1276 2023-05-17 13:13:43.000000 amuse-mesa-2023.5.1.post1/amuse_mesa.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      508 2023-05-17 13:13:45.000000 amuse-mesa-2023.5.1.post1/amuse_mesa.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 13:13:43.000000 amuse-mesa-2023.5.1.post1/amuse_mesa.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 13:13:43.000000 amuse-mesa-2023.5.1.post1/amuse_mesa.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 13:13:43.000000 amuse-mesa-2023.5.1.post1/amuse_mesa.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      124 2023-05-17 12:59:10.000000 amuse-mesa-2023.5.1.post1/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 13:13:45.532473 amuse-mesa-2023.5.1.post1/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1763 2023-05-17 12:54:40.000000 amuse-mesa-2023.5.1.post1/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:13:45.528744 amuse-mesa-2023.5.1.post1/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:13:45.528794 amuse-mesa-2023.5.1.post1/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:13:45.528844 amuse-mesa-2023.5.1.post1/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:13:45.530511 amuse-mesa-2023.5.1.post1/src/amuse/community/mesa/
+-rw-r--r--   0 rieder     (501) staff       (20)       83 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/src/amuse/community/mesa/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      924 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/src/amuse/community/mesa/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)      154 2023-05-17 13:13:43.000000 amuse-mesa-2023.5.1.post1/src/amuse/community/mesa/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 13:13:45.531954 amuse-mesa-2023.5.1.post1/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-mesa-2023.5.1.post1/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-mesa-2023.5.1.post1/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-mesa-2023.5.1.post1/support/version.py
```

### Comparing `amuse-mesa-2023.5.1/PKG-INFO` & `amuse-mesa-2023.5.1.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-mesa
-Version: 2023.5.1
+Version: 2023.5.1.post1
 Summary: The Astrophysical Multipurpose Software Environment - MESA
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -23,7 +23,8 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 This package installs the MESA community code for AMUSE.
+It will not build MESA itself, rather it requires the amuse-mesa-r15140 package for this.
```

### Comparing `amuse-mesa-2023.5.1/amuse_mesa.egg-info/PKG-INFO` & `amuse-mesa-2023.5.1.post1/amuse_mesa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-mesa
-Version: 2023.5.1
+Version: 2023.5.1.post1
 Summary: The Astrophysical Multipurpose Software Environment - MESA
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -23,7 +23,8 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 This package installs the MESA community code for AMUSE.
+It will not build MESA itself, rather it requires the amuse-mesa-r15140 package for this.
```

### Comparing `amuse-mesa-2023.5.1/setup.py` & `amuse-mesa-2023.5.1.post1/setup.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/src/amuse/community/mesa/interface.py` & `amuse-mesa-2023.5.1.post1/src/amuse/community/mesa/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/__init__.py` & `amuse-mesa-2023.5.1.post1/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/classifiers.py` & `amuse-mesa-2023.5.1.post1/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/config.py` & `amuse-mesa-2023.5.1.post1/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/generate_main.py` & `amuse-mesa-2023.5.1.post1/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/getsp.class` & `amuse-mesa-2023.5.1.post1/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/getsp.java` & `amuse-mesa-2023.5.1.post1/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/misc.py` & `amuse-mesa-2023.5.1.post1/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-2023.5.1/support/setup_codes.py` & `amuse-mesa-2023.5.1.post1/support/setup_codes.py`

 * *Files identical despite different names*

