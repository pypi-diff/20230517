# Comparing `tmp/selenium_assist-0.2.1.tar.gz` & `tmp/selenium_assist-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_assist-0.2.1.tar", last modified: Mon May 15 21:17:53 2023, max compression
+gzip compressed data, was "selenium_assist-0.2.2.tar", last modified: Wed May 17 21:18:52 2023, max compression
```

## Comparing `selenium_assist-0.2.1.tar` & `selenium_assist-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-15 21:17:53.445025 selenium_assist-0.2.1/
--rw-rw-r--   0 mich      (1000) mich      (1000)     1071 2023-04-05 22:02:25.000000 selenium_assist-0.2.1/LICENSE
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-15 21:17:53.445025 selenium_assist-0.2.1/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)       71 2023-05-12 23:13:38.000000 selenium_assist-0.2.1/README.md
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-15 21:17:53.441027 selenium_assist-0.2.1/selenium_assist/
--rw-rw-r--   0 mich      (1000) mich      (1000)      458 2023-05-12 23:13:37.000000 selenium_assist-0.2.1/selenium_assist/__init__.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     1048 2023-04-05 22:44:18.000000 selenium_assist-0.2.1/selenium_assist/helpers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)      913 2023-05-12 21:20:58.000000 selenium_assist-0.2.1/selenium_assist/managers.py
--rw-rw-r--   0 mich      (1000) mich      (1000)     3847 2023-05-12 23:13:37.000000 selenium_assist-0.2.1/selenium_assist/wrappers.py
-drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-15 21:17:53.445025 selenium_assist-0.2.1/selenium_assist.egg-info/
--rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/PKG-INFO
--rw-rw-r--   0 mich      (1000) mich      (1000)      341 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/SOURCES.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)        1 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/dependency_links.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       39 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/requires.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       16 2023-05-15 21:17:53.000000 selenium_assist-0.2.1/selenium_assist.egg-info/top_level.txt
--rw-rw-r--   0 mich      (1000) mich      (1000)       79 2023-05-15 21:17:53.449022 selenium_assist-0.2.1/setup.cfg
--rw-rw-r--   0 mich      (1000) mich      (1000)     1097 2023-05-15 21:14:58.000000 selenium_assist-0.2.1/setup.py
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1071 2023-04-05 22:02:25.000000 selenium_assist-0.2.2/LICENSE
+-rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/PKG-INFO
+-rw-rw-r--   0 mich      (1000) mich      (1000)       71 2023-05-12 23:13:38.000000 selenium_assist-0.2.2/README.md
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-17 21:18:52.576188 selenium_assist-0.2.2/selenium_assist/
+-rw-rw-r--   0 mich      (1000) mich      (1000)      458 2023-05-12 23:13:37.000000 selenium_assist-0.2.2/selenium_assist/__init__.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1048 2023-04-05 22:44:18.000000 selenium_assist-0.2.2/selenium_assist/helpers.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1125 2023-05-17 20:55:52.000000 selenium_assist-0.2.2/selenium_assist/managers.py
+-rw-rw-r--   0 mich      (1000) mich      (1000)     3847 2023-05-12 23:13:37.000000 selenium_assist-0.2.2/selenium_assist/wrappers.py
+drwxrwxr-x   0 mich      (1000) mich      (1000)        0 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/selenium_assist.egg-info/
+-rw-rw-r--   0 mich      (1000) mich      (1000)      831 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/PKG-INFO
+-rw-rw-r--   0 mich      (1000) mich      (1000)      341 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/SOURCES.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)        1 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/dependency_links.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       39 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/requires.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       16 2023-05-17 21:18:52.000000 selenium_assist-0.2.2/selenium_assist.egg-info/top_level.txt
+-rw-rw-r--   0 mich      (1000) mich      (1000)       79 2023-05-17 21:18:52.580188 selenium_assist-0.2.2/setup.cfg
+-rw-rw-r--   0 mich      (1000) mich      (1000)     1097 2023-05-17 20:55:52.000000 selenium_assist-0.2.2/setup.py
```

### Comparing `selenium_assist-0.2.1/LICENSE` & `selenium_assist-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.1/PKG-INFO` & `selenium_assist-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium_assist
-Version: 0.2.1
+Version: 0.2.2
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.2.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.1/selenium_assist/helpers.py` & `selenium_assist-0.2.2/selenium_assist/helpers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.1/selenium_assist/wrappers.py` & `selenium_assist-0.2.2/selenium_assist/wrappers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.2.1/selenium_assist.egg-info/PKG-INFO` & `selenium_assist-0.2.2/selenium_assist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: selenium-assist
-Version: 0.2.1
+Version: 0.2.2
 Summary: Helper functions for selenium
 Home-page: https://github.com/ivanmicetic/selenium-assist
-Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.2.tar.gz
 Author: Ivan Mičetić
 Author-email: ivan.micetic@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Keywords: pypi,selenium_assist
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `selenium_assist-0.2.1/setup.py` & `selenium_assist-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium_assist",
-    version="0.2.1",
+    version="0.2.2",
     author="Ivan Mičetić",
     author_email="ivan.micetic@gmail.com",
     description="Helper functions for selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ivanmicetic/selenium-assist",
     project_urls={
@@ -22,9 +22,9 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
-    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.1.tar.gz"
+    download_url="https://github.com/ivanmicetic/selenium-assist/archive/refs/tags/v0.2.2.tar.gz"
 )
```

