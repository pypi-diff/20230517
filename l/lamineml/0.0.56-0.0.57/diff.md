# Comparing `tmp/lamineml-0.0.56.tar.gz` & `tmp/lamineml-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.56.tar", last modified: Tue May 16 19:31:19 2023, max compression
+gzip compressed data, was "lamineml-0.0.57.tar", last modified: Wed May 17 12:25:33 2023, max compression
```

## Comparing `lamineml-0.0.56.tar` & `lamineml-0.0.57.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:31:19.085523 lamineml-0.0.56/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.56/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-16 19:31:19.085523 lamineml-0.0.56/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.56/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.56/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-16 19:31:19.085523 lamineml-0.0.56/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:31:19.081523 lamineml-0.0.56/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:31:19.085523 lamineml-0.0.56/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.56/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     3259 2023-05-16 19:30:15.000000 lamineml-0.0.56/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:31:19.085523 lamineml-0.0.56/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-16 19:31:19.000000 lamineml-0.0.56/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-16 19:31:19.000000 lamineml-0.0.56/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-16 19:31:19.000000 lamineml-0.0.56/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-16 19:31:19.000000 lamineml-0.0.56/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:25:33.615764 lamineml-0.0.57/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.57/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-17 12:25:33.619764 lamineml-0.0.57/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.57/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.57/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-17 12:25:33.619764 lamineml-0.0.57/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:25:33.595764 lamineml-0.0.57/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:25:33.595764 lamineml-0.0.57/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.57/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     3473 2023-05-17 12:24:14.000000 lamineml-0.0.57/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-17 12:25:33.615764 lamineml-0.0.57/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-17 12:25:33.000000 lamineml-0.0.57/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-17 12:25:33.000000 lamineml-0.0.57/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-17 12:25:33.000000 lamineml-0.0.57/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-17 12:25:33.000000 lamineml-0.0.57/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.56/PKG-INFO` & `lamineml-0.0.57/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.56
+Version: 0.0.57
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.56/README.md` & `lamineml-0.0.57/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.56/setup.cfg` & `lamineml-0.0.57/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.56
+version = 0.0.57
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.56/src/lamine/tools.py` & `lamineml-0.0.57/src/lamine/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 ##################################################"
 g =autoclass("android.view.Gravity")
 t= autoclass("android.widget.Toast")
 window=autoclass ("android.view.WindowManager$LayoutParams")
 
 
 from android.runnable import run_on_ui_thread
-
+def  get_all_packageName():
+    PackageManager = activity.getPackageManager()
+    installedPackages =PackageManager.getInstalledPackages(0);
+    for i in installedPackages:
+        a= i.packageName
+        return a
 def KEEP_SCREEN_ON():
     activity.getWindow(). addFlags (window.FLAG_KEEP_SCREEN_ON)
 def open_browser(url):
     intent = Intent()
     intent.setAction(Intent.ACTION_VIEW)
     intent.setData(uri.parse(url))
     activity.startActivity(intent)
```

### Comparing `lamineml-0.0.56/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.57/src/lamineml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.56
+Version: 0.0.57
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

