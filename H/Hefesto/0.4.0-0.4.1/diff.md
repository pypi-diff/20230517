# Comparing `tmp/Hefesto-0.4.0.tar.gz` & `tmp/Hefesto-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.4.0.tar", last modified: Fri Apr 21 09:51:58 2023, max compression
+gzip compressed data, was "Hefesto-0.4.1.tar", last modified: Wed May 17 07:46:09 2023, max compression
```

## Comparing `Hefesto-0.4.0.tar` & `Hefesto-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-21 09:51:58.443345 Hefesto-0.4.0/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-21 09:51:58.443345 Hefesto-0.4.0/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.0/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    11950 2023-04-21 09:50:03.000000 Hefesto-0.4.0/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     8594 2023-04-21 09:41:24.000000 Hefesto-0.4.0/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-21 09:51:58.443345 Hefesto-0.4.0/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-04-21 09:51:58.000000 Hefesto-0.4.0/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.0/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-21 09:51:58.443345 Hefesto-0.4.0/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.0/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.4.0/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-04-21 09:51:58.443345 Hefesto-0.4.0/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-04-21 09:51:44.000000 Hefesto-0.4.0/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-17 07:46:09.189123 Hefesto-0.4.1/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-17 07:46:09.189123 Hefesto-0.4.1/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.1/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    11950 2023-05-17 07:22:54.000000 Hefesto-0.4.1/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     8594 2023-04-21 09:41:24.000000 Hefesto-0.4.1/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-17 07:46:09.189123 Hefesto-0.4.1/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.1/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-17 07:46:09.189123 Hefesto-0.4.1/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.1/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.4.1/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-05-17 07:46:09.189123 Hefesto-0.4.1/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-05-17 07:44:20.000000 Hefesto-0.4.1/setup.py
```

### Comparing `Hefesto-0.4.0/Hefesto/main.py` & `Hefesto-0.4.1/Hefesto/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from perseo.main import milisec
-from template import Template
-# from Hefesto.template import Template
+# from template import Template
+from Hefesto.template import Template
 import sys
 import yaml
 import math
 import requests
 
 class Hefesto():
```

### Comparing `Hefesto-0.4.0/Hefesto/template.py` & `Hefesto-0.4.1/Hefesto/template.py`

 * *Files identical despite different names*

### Comparing `Hefesto-0.4.0/README.md` & `Hefesto-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Hefesto-0.4.0/setup.py` & `Hefesto-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.4.0",
+    version="0.4.1",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

