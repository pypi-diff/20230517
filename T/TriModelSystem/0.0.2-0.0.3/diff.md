# Comparing `tmp/TriModelSystem-0.0.2.tar.gz` & `tmp/TriModelSystem-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TriModelSystem-0.0.2.tar", last modified: Wed May 17 00:47:52 2023, max compression
+gzip compressed data, was "TriModelSystem-0.0.3.tar", last modified: Wed May 17 01:17:26 2023, max compression
```

## Comparing `TriModelSystem-0.0.2.tar` & `TriModelSystem-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:47:52.729228 TriModelSystem-0.0.2/
--rw-r--r--   0 echo       (501) staff       (20)     1324 2023-05-17 00:47:52.728978 TriModelSystem-0.0.2/PKG-INFO
--rw-r--r--   0 echo       (501) staff       (20)      736 2023-05-17 00:26:47.000000 TriModelSystem-0.0.2/README.md
-drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:47:52.727361 TriModelSystem-0.0.2/TriModelSystem/
--rw-r--r--   0 echo       (501) staff       (20)      144 2023-05-16 23:56:16.000000 TriModelSystem-0.0.2/TriModelSystem/__init__.py
--rw-r--r--   0 echo       (501) staff       (20)     3505 2023-05-16 11:31:20.000000 TriModelSystem-0.0.2/TriModelSystem/binclassification.py
--rw-r--r--   0 echo       (501) staff       (20)     1885 2023-05-16 11:35:17.000000 TriModelSystem-0.0.2/TriModelSystem/utils.py
-drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 00:47:52.728652 TriModelSystem-0.0.2/TriModelSystem.egg-info/
--rw-r--r--   0 echo       (501) staff       (20)     1324 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/PKG-INFO
--rw-r--r--   0 echo       (501) staff       (20)      294 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/SOURCES.txt
--rw-r--r--   0 echo       (501) staff       (20)        1 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/dependency_links.txt
--rw-r--r--   0 echo       (501) staff       (20)       11 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/requires.txt
--rw-r--r--   0 echo       (501) staff       (20)       15 2023-05-17 00:47:52.000000 TriModelSystem-0.0.2/TriModelSystem.egg-info/top_level.txt
--rw-r--r--   0 echo       (501) staff       (20)       38 2023-05-17 00:47:52.729301 TriModelSystem-0.0.2/setup.cfg
--rw-r--r--   0 echo       (501) staff       (20)     1055 2023-05-17 00:47:50.000000 TriModelSystem-0.0.2/setup.py
+drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 01:17:26.711332 TriModelSystem-0.0.3/
+-rw-r--r--   0 echo       (501) staff       (20)     1324 2023-05-17 01:17:26.711148 TriModelSystem-0.0.3/PKG-INFO
+-rw-r--r--   0 echo       (501) staff       (20)      736 2023-05-17 00:26:47.000000 TriModelSystem-0.0.3/README.md
+drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 01:17:26.709604 TriModelSystem-0.0.3/TriModelSystem/
+-rw-r--r--   0 echo       (501) staff       (20)      156 2023-05-17 01:16:42.000000 TriModelSystem-0.0.3/TriModelSystem/__init__.py
+-rw-r--r--   0 echo       (501) staff       (20)     3509 2023-05-17 01:15:49.000000 TriModelSystem-0.0.3/TriModelSystem/binclassification.py
+-rw-r--r--   0 echo       (501) staff       (20)     1885 2023-05-16 11:35:17.000000 TriModelSystem-0.0.3/TriModelSystem/tms_utils.py
+drwxr-xr-x   0 echo       (501) staff       (20)        0 2023-05-17 01:17:26.710865 TriModelSystem-0.0.3/TriModelSystem.egg-info/
+-rw-r--r--   0 echo       (501) staff       (20)     1324 2023-05-17 01:17:26.000000 TriModelSystem-0.0.3/TriModelSystem.egg-info/PKG-INFO
+-rw-r--r--   0 echo       (501) staff       (20)      298 2023-05-17 01:17:26.000000 TriModelSystem-0.0.3/TriModelSystem.egg-info/SOURCES.txt
+-rw-r--r--   0 echo       (501) staff       (20)        1 2023-05-17 01:17:26.000000 TriModelSystem-0.0.3/TriModelSystem.egg-info/dependency_links.txt
+-rw-r--r--   0 echo       (501) staff       (20)       11 2023-05-17 01:17:26.000000 TriModelSystem-0.0.3/TriModelSystem.egg-info/requires.txt
+-rw-r--r--   0 echo       (501) staff       (20)       15 2023-05-17 01:17:26.000000 TriModelSystem-0.0.3/TriModelSystem.egg-info/top_level.txt
+-rw-r--r--   0 echo       (501) staff       (20)       38 2023-05-17 01:17:26.711391 TriModelSystem-0.0.3/setup.cfg
+-rw-r--r--   0 echo       (501) staff       (20)     1055 2023-05-17 01:17:20.000000 TriModelSystem-0.0.3/setup.py
```

### Comparing `TriModelSystem-0.0.2/PKG-INFO` & `TriModelSystem-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TriModelSystem
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tri-Model Ensemble System for Classification
 Author: Arkitech (Joshua Tan)
 Author-email: <joshuatan.helios@gmail.com>
 Keywords: python,machine learning,tensorflow,classification,neural network
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TriModelSystem-0.0.2/README.md` & `TriModelSystem-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `TriModelSystem-0.0.2/TriModelSystem/binclassification.py` & `TriModelSystem-0.0.3/TriModelSystem/binclassification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from keras.layers import Input, Dense, Dropout, concatenate
 from keras.models import Model
 from keras.optimizers import RMSprop, Adadelta, Adam
 from keras import regularizers
-from utils import get_model_data
+from tms_utils import get_model_data
 
 
 def rms_adadelta_model(input_shape):
     model_A_data = get_model_data(mode='A')
     model_B_data = get_model_data(mode='B')
     model_C_data = get_model_data(mode='C')
```

### Comparing `TriModelSystem-0.0.2/TriModelSystem/utils.py` & `TriModelSystem-0.0.3/TriModelSystem/tms_utils.py`

 * *Files identical despite different names*

### Comparing `TriModelSystem-0.0.2/TriModelSystem.egg-info/PKG-INFO` & `TriModelSystem-0.0.3/TriModelSystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TriModelSystem
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tri-Model Ensemble System for Classification
 Author: Arkitech (Joshua Tan)
 Author-email: <joshuatan.helios@gmail.com>
 Keywords: python,machine learning,tensorflow,classification,neural network
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TriModelSystem-0.0.2/setup.py` & `TriModelSystem-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Tri-Model Ensemble System for Classification'
 
 # Setting up
 setup(
     name="TriModelSystem",
     version=VERSION,
     author="Arkitech (Joshua Tan)",
```

