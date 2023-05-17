# Comparing `tmp/covidillness-0.0.6.tar.gz` & `tmp/covidillness-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covidillness-0.0.6.tar", last modified: Wed May 17 15:26:42 2023, max compression
+gzip compressed data, was "covidillness-0.0.8.tar", last modified: Wed May 17 16:10:12 2023, max compression
```

## Comparing `covidillness-0.0.6.tar` & `covidillness-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-05-17 15:26:42.223606 covidillness-0.0.6/
--rw-r--r--   0 inoseizuru   (501) staff       (20)     1316 2023-05-17 15:26:42.222603 covidillness-0.0.6/PKG-INFO
--rw-r--r--   0 inoseizuru   (501) staff       (20)      801 2022-11-08 17:14:08.000000 covidillness-0.0.6/README.md
--rw-r--r--   0 inoseizuru   (501) staff       (20)       38 2023-05-17 15:26:42.223728 covidillness-0.0.6/setup.cfg
--rw-r--r--   0 inoseizuru   (501) staff       (20)      966 2023-05-17 15:23:19.000000 covidillness-0.0.6/setup.py
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-05-17 15:26:42.214275 covidillness-0.0.6/src/
-drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-05-17 15:26:42.221696 covidillness-0.0.6/src/covidillness.egg-info/
--rw-r--r--   0 inoseizuru   (501) staff       (20)     1316 2023-05-17 15:26:41.000000 covidillness-0.0.6/src/covidillness.egg-info/PKG-INFO
--rw-r--r--   0 inoseizuru   (501) staff       (20)      241 2023-05-17 15:26:42.000000 covidillness-0.0.6/src/covidillness.egg-info/SOURCES.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)        1 2023-05-17 15:26:41.000000 covidillness-0.0.6/src/covidillness.egg-info/dependency_links.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)       51 2023-05-17 15:26:41.000000 covidillness-0.0.6/src/covidillness.egg-info/entry_points.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)       13 2023-05-17 15:26:41.000000 covidillness-0.0.6/src/covidillness.egg-info/top_level.txt
--rw-r--r--   0 inoseizuru   (501) staff       (20)     2089 2023-05-17 15:22:50.000000 covidillness-0.0.6/src/covidillness.py
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-05-17 16:10:12.767453 covidillness-0.0.8/
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     1315 2023-05-17 16:10:12.767266 covidillness-0.0.8/PKG-INFO
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      801 2022-11-08 17:14:08.000000 covidillness-0.0.8/README.md
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       38 2023-05-17 16:10:12.767499 covidillness-0.0.8/setup.cfg
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      965 2023-05-17 16:09:18.000000 covidillness-0.0.8/setup.py
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-05-17 16:10:12.765989 covidillness-0.0.8/src/
+drwxr-xr-x   0 inoseizuru   (501) staff       (20)        0 2023-05-17 16:10:12.767027 covidillness-0.0.8/src/covidillness.egg-info/
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     1315 2023-05-17 16:10:12.000000 covidillness-0.0.8/src/covidillness.egg-info/PKG-INFO
+-rw-r--r--   0 inoseizuru   (501) staff       (20)      241 2023-05-17 16:10:12.000000 covidillness-0.0.8/src/covidillness.egg-info/SOURCES.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)        1 2023-05-17 16:10:12.000000 covidillness-0.0.8/src/covidillness.egg-info/dependency_links.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       51 2023-05-17 16:10:12.000000 covidillness-0.0.8/src/covidillness.egg-info/entry_points.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)       13 2023-05-17 16:10:12.000000 covidillness-0.0.8/src/covidillness.egg-info/top_level.txt
+-rw-r--r--   0 inoseizuru   (501) staff       (20)     2089 2023-05-17 15:22:50.000000 covidillness-0.0.8/src/covidillness.py
```

### Comparing `covidillness-0.0.6/PKG-INFO` & `covidillness-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: covidillness
-Version: 0.0.6
-Summary: The graph of the number of ICU patients and deaths due to Covid-19
+Version: 0.0.8
+Summary: The graph of the number of ICU patients and cases due to Covid-19
 Home-page: https://github.com/i-inose/covidillness
 Author: Izuru Inose
 Author-email: i.inose0304@gmail.com
 Project-URL: Bug Tracker, https://github.com/i-inose/covidillness
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `covidillness-0.0.6/README.md` & `covidillness-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `covidillness-0.0.6/setup.py` & `covidillness-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covidillness",
-    version="0.0.6",
+    version="0.0.8",
     author="Izuru Inose",
     author_email="i.inose0304@gmail.com",
-    description="The graph of the number of ICU patients and deaths due to Covid-19",
+    description="The graph of the number of ICU patients and cases due to Covid-19",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/i-inose/covidillness",
     project_urls={
         "Bug Tracker": "https://github.com/i-inose/covidillness",
     },
     classifiers=[
```

### Comparing `covidillness-0.0.6/src/covidillness.egg-info/PKG-INFO` & `covidillness-0.0.8/src/covidillness.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: covidillness
-Version: 0.0.6
-Summary: The graph of the number of ICU patients and deaths due to Covid-19
+Version: 0.0.8
+Summary: The graph of the number of ICU patients and cases due to Covid-19
 Home-page: https://github.com/i-inose/covidillness
 Author: Izuru Inose
 Author-email: i.inose0304@gmail.com
 Project-URL: Bug Tracker, https://github.com/i-inose/covidillness
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `covidillness-0.0.6/src/covidillness.py` & `covidillness-0.0.8/src/covidillness.py`

 * *Files identical despite different names*

