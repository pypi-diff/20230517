# Comparing `tmp/restscript-0.7.tar.gz` & `tmp/restscript-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\restscript-0.7.tar", last modified: Tue May 16 11:09:13 2023, max compression
+gzip compressed data, was "dist\restscript-1.0.tar", last modified: Wed May 17 11:02:46 2023, max compression
```

## Comparing `restscript-0.7.tar` & `restscript-1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:09:13.408778 restscript-0.7/
--rw-rw-rw-   0        0        0      534 2023-05-16 11:09:13.407804 restscript-0.7/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-05-16 10:43:26.000000 restscript-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 11:09:13.400780 restscript-0.7/restscript/
--rw-rw-rw-   0        0        0        0 2023-05-16 11:03:06.000000 restscript-0.7/restscript/__init__.py
--rw-rw-rw-   0        0        0       66 2023-05-16 11:07:48.000000 restscript-0.7/restscript/__main__.py
--rw-rw-rw-   0        0        0       27 2023-05-16 10:53:04.000000 restscript-0.7/restscript/run_script.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:09:13.405805 restscript-0.7/restscript.egg-info/
--rw-rw-rw-   0        0        0      534 2023-05-16 11:09:13.000000 restscript-0.7/restscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-05-16 11:09:13.000000 restscript-0.7/restscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:09:13.000000 restscript-0.7/restscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 11:09:13.000000 restscript-0.7/restscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 11:09:13.408778 restscript-0.7/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-05-16 11:08:16.000000 restscript-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:46.577773 restscript-1.0/
+-rw-rw-rw-   0        0        0      534 2023-05-17 11:02:46.577773 restscript-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-05-16 10:43:26.000000 restscript-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:46.569743 restscript-1.0/restscript/
+-rw-rw-rw-   0        0        0        0 2023-05-16 11:03:06.000000 restscript-1.0/restscript/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-05-17 10:59:06.000000 restscript-1.0/restscript/__main__.py
+-rw-rw-rw-   0        0        0     8032 2023-05-17 10:55:06.000000 restscript-1.0/restscript/grammar.py
+-rw-rw-rw-   0        0        0     5584 2023-05-17 10:55:05.000000 restscript-1.0/restscript/rest_client.py
+-rw-rw-rw-   0        0        0    18625 2023-05-17 10:57:23.000000 restscript-1.0/restscript/run_script.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:46.575742 restscript-1.0/restscript.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-05-17 11:02:46.000000 restscript-1.0/restscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-05-17 11:02:46.000000 restscript-1.0/restscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:02:46.000000 restscript-1.0/restscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 11:02:46.000000 restscript-1.0/restscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 11:02:46.578746 restscript-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-05-17 11:02:27.000000 restscript-1.0/setup.py
```

### Comparing `restscript-0.7/PKG-INFO` & `restscript-1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restscript
-Version: 0.7
+Version: 1.0
 Summary: Script runner for REST API
 Home-page: https://github.com/topherCantrell/restscript
 Author: Chris Cantrell
 Author-email: topherCantrell@gmail.com
 License: UNKNOWN
 Description: # restscript
         Scripting for REST APIs
```

### Comparing `restscript-0.7/restscript.egg-info/PKG-INFO` & `restscript-1.0/restscript.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restscript
-Version: 0.7
+Version: 1.0
 Summary: Script runner for REST API
 Home-page: https://github.com/topherCantrell/restscript
 Author: Chris Cantrell
 Author-email: topherCantrell@gmail.com
 License: UNKNOWN
 Description: # restscript
         Scripting for REST APIs
```

### Comparing `restscript-0.7/setup.py` & `restscript-1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #   py -m twine upload dist/*
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="restscript",  # Replace with your own username
-    version="0.7",
+    version="1.0",
     author="Chris Cantrell",
     author_email="topherCantrell@gmail.com",
     description="Script runner for REST API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/topherCantrell/restscript",
     packages=setuptools.find_packages(),
```

