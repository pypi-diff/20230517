# Comparing `tmp/panml-0.0.4.tar.gz` & `tmp/panml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.4.tar", last modified: Tue May 16 08:17:49 2023, max compression
+gzip compressed data, was "panml-0.0.5.tar", last modified: Wed May 17 07:22:52 2023, max compression
```

## Comparing `panml-0.0.4.tar` & `panml-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-16 08:17:49.440327 panml-0.0.4/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1501 2023-05-16 08:17:49.440426 panml-0.0.4/PKG-INFO
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-16 08:17:49.440281 panml-0.0.4/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.4/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    22590 2023-05-16 08:12:47.827759 panml-0.0.4/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     7024 2023-05-16 08:12:47.828416 panml-0.0.4/panml/search.py
--rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.4/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     3304 2023-05-16 08:15:50.944002 panml-0.0.4/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 07:22:52.848962 panml-0.0.5/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1501 2023-05-17 07:22:52.849086 panml-0.0.5/PKG-INFO
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 07:22:52.848912 panml-0.0.5/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.5/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    22590 2023-05-16 08:12:47.827759 panml-0.0.5/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     7024 2023-05-16 08:12:47.828416 panml-0.0.5/panml/search.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.5/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3304 2023-05-17 07:22:12.706012 panml-0.0.5/setup.py
```

### Comparing `panml-0.0.4/PKG-INFO` & `panml-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: panml
-Version: 0.0.4
+Version: 0.0.5
 Summary: PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: williamxn.z@gmail.com
 License: MIT
 Download-URL: https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.3.tar.gz
 Description: PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers.                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others.
```

### Comparing `panml-0.0.4/panml/models.py` & `panml-0.0.5/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.4/panml/search.py` & `panml-0.0.5/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.4/setup.py` & `panml-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'panml', # package name     
   packages = ['panml'], # package name
-  version = '0.0.4', # version
+  version = '0.0.5', # version
   license = 'MIT', # license
   description = 'PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.', # short description about the package
   long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
                       \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide \
                       \n\nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki', # long description
   author = 'PanML team', # team name
```

