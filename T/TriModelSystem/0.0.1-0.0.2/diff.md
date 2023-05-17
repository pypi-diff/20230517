# Comparing `tmp/TriModelSystem-0.0.1.tar.gz` & `tmp/TriModelSystem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TriModelSystem-0.0.1.tar", last modified: Wed May 17 00:39:19 2023, max compression
+gzip compressed data, was "TriModelSystem-0.0.2.tar", last modified: Wed May 17 00:47:52 2023, max compression
```

## Comparing `TriModelSystem-0.0.1.tar` & `TriModelSystem-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:39:19.805334 TriModelSystem-0.0.1/
--rw-r--r--   0 echo       (501) staff       (20)      545 2023-05-17 00:39:19.805099 TriModelSystem-0.0.1/PKG-INFO
--rw-r--r--   0 echo       (501) staff       (20)      736 2023-05-17 00:26:47.000000 TriModelSystem-0.0.1/README.md
-drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:39:19.803442 TriModelSystem-0.0.1/TriModelSystem/
--rw-r--r--   0 echo       (501) staff       (20)      144 2023-05-16 23:56:16.000000 TriModelSystem-0.0.1/TriModelSystem/__init__.py
--rw-r--r--   0 echo       (501) staff       (20)     3505 2023-05-16 11:31:20.000000 TriModelSystem-0.0.1/TriModelSystem/binclassification.py
--rw-r--r--   0 echo       (501) staff       (20)     1885 2023-05-16 11:35:17.000000 TriModelSystem-0.0.1/TriModelSystem/utils.py
-drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:39:19.804779 TriModelSystem-0.0.1/TriModelSystem.egg-info/
--rw-r--r--   0 echo       (501) staff       (20)      545 2023-05-17 00:39:19.000000 TriModelSystem-0.0.1/TriModelSystem.egg-info/PKG-INFO
--rw-r--r--   0 echo       (501) staff       (20)      294 2023-05-17 00:39:19.000000 TriModelSystem-0.0.1/TriModelSystem.egg-info/SOURCES.txt
--rw-r--r--   0 echo       (501) staff       (20)        1 2023-05-17 00:39:19.000000 TriModelSystem-0.0.1/TriModelSystem.egg-info/dependency_links.txt
--rw-r--r--   0 echo       (501) staff       (20)       11 2023-05-17 00:39:19.000000 TriModelSystem-0.0.1/TriModelSystem.egg-info/requires.txt
--rw-r--r--   0 echo       (501) staff       (20)       15 2023-05-17 00:39:19.000000 TriModelSystem-0.0.1/TriModelSystem.egg-info/top_level.txt
--rw-r--r--   0 echo       (501) staff       (20)       38 2023-05-17 00:39:19.805401 TriModelSystem-0.0.1/setup.cfg
--rw-r--r--   0 echo       (501) staff       (20)      965 2023-05-17 00:39:16.000000 TriModelSystem-0.0.1/setup.py
+drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:47:52.729228 TriModelSystem-0.0.2/
+-rw-r--r--   0 echo       (501) staff       (20)     1324 2023-05-17 00:47:52.728978 TriModelSystem-0.0.2/PKG-INFO
+-rw-r--r--   0 echo       (501) staff       (20)      736 2023-05-17 00:26:47.000000 TriModelSystem-0.0.2/README.md
+drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:47:52.727361 TriModelSystem-0.0.2/TriModelSystem/
+-rw-r--r--   0 echo       (501) staff       (20)      144 2023-05-16 23:56:16.000000 TriModelSystem-0.0.2/TriModelSystem/__init__.py
+-rw-r--r--   0 echo       (501) staff       (20)     3505 2023-05-16 11:31:20.000000 TriModelSystem-0.0.2/TriModelSystem/binclassification.py
+-rw-r--r--   0 echo       (501) staff       (20)     1885 2023-05-16 11:35:17.000000 TriModelSystem-0.0.2/TriModelSystem/utils.py
+drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:47:52.728652 TriModelSystem-0.0.2/TriModelSystem.egg-info/
+-rw-r--r--   0 echo       (501) staff       (20)     1324 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/PKG-INFO
+-rw-r--r--   0 echo       (501) staff       (20)      294 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/SOURCES.txt
+-rw-r--r--   0 echo       (501) staff       (20)        1 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/dependency_links.txt
+-rw-r--r--   0 echo       (501) staff       (20)       11 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/requires.txt
+-rw-r--r--   0 echo       (501) staff       (20)       15 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/top_level.txt
+-rw-r--r--   0 echo       (501) staff       (20)       38 2023-05-17 00:47:52.729301 TriModelSystem-0.0.2/setup.cfg
+-rw-r--r--   0 echo       (501) staff       (20)     1055 2023-05-17 00:47:50.000000 TriModelSystem-0.0.2/setup.py
```

### Comparing `TriModelSystem-0.0.1/README.md` & `TriModelSystem-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `TriModelSystem-0.0.1/TriModelSystem/binclassification.py` & `TriModelSystem-0.0.2/TriModelSystem/binclassification.py`

 * *Files identical despite different names*

### Comparing `TriModelSystem-0.0.1/TriModelSystem/utils.py` & `TriModelSystem-0.0.2/TriModelSystem/utils.py`

 * *Files identical despite different names*

### Comparing `TriModelSystem-0.0.1/setup.py` & `TriModelSystem-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Tri-Model Ensemble System for Classification'
 
 # Setting up
 setup(
     name="TriModelSystem",
     version=VERSION,
     author="Arkitech (Joshua Tan)",
     author_email="<joshuatan.helios@gmail.com>",
     description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
     packages=find_packages(),
     install_requires=['tensorflow'],
     keywords=['python', 'machine learning', 'tensorflow', 'classification', 'neural network'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
```

