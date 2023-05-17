# Comparing `tmp/lamineml-0.0.58.tar.gz` & `tmp/lamineml-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.58.tar", last modified: Wed May 17 12:35:35 2023, max compression
+gzip compressed data, was "lamineml-0.0.59.tar", last modified: Wed May 17 12:40:14 2023, max compression
```

## Comparing `lamineml-0.0.58.tar` & `lamineml-0.0.59.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:35:35.259063 lamineml-0.0.58/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.58/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-17 12:35:35.259063 lamineml-0.0.58/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.58/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.58/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-17 12:35:35.259063 lamineml-0.0.58/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:35:35.255063 lamineml-0.0.58/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:35:35.259063 lamineml-0.0.58/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.58/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     3504 2023-05-17 12:34:47.000000 lamineml-0.0.58/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:35:35.259063 lamineml-0.0.58/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-17 12:35:35.000000 lamineml-0.0.58/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-17 12:35:35.000000 lamineml-0.0.58/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-17 12:35:35.000000 lamineml-0.0.58/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-17 12:35:35.000000 lamineml-0.0.58/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:40:14.838750 lamineml-0.0.59/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.59/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-17 12:40:14.838750 lamineml-0.0.59/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.59/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.59/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-17 12:40:14.842751 lamineml-0.0.59/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:40:14.802749 lamineml-0.0.59/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:40:14.806749 lamineml-0.0.59/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.59/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     3509 2023-05-17 12:37:47.000000 lamineml-0.0.59/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:40:14.838750 lamineml-0.0.59/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-17 12:40:14.000000 lamineml-0.0.59/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-17 12:40:14.000000 lamineml-0.0.59/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-17 12:40:14.000000 lamineml-0.0.59/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-17 12:40:14.000000 lamineml-0.0.59/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.58/PKG-INFO` & `lamineml-0.0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.58
+Version: 0.0.59
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.58/README.md` & `lamineml-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.58/setup.cfg` & `lamineml-0.0.59/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.58
+version = 0.0.59
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.58/src/lamine/tools.py` & `lamineml-0.0.59/src/lamine/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def  get_all_packageName():
     al = []
 
     PackageManager = activity.getPackageManager()
     installedPackages =PackageManager.getInstalledPackages(0);
     for i in installedPackages:
         a= i.packageName
-        al.append(a)
+        al.append(a+"\n")
     return al
 def KEEP_SCREEN_ON():
     activity.getWindow(). addFlags (window.FLAG_KEEP_SCREEN_ON)
 def open_browser(url):
     intent = Intent()
     intent.setAction(Intent.ACTION_VIEW)
     intent.setData(uri.parse(url))
```

### Comparing `lamineml-0.0.58/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.59/src/lamineml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.58
+Version: 0.0.59
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

