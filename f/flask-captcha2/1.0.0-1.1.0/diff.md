# Comparing `tmp/flask_captcha2-1.0.0.tar.gz` & `tmp/flask_captcha2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flask_captcha2-1.0.0.tar", last modified: Wed May 17 16:59:00 2023, max compression
+gzip compressed data, was "dist\flask_captcha2-1.1.0.tar", last modified: Wed May 17 17:03:47 2023, max compression
```

## Comparing `flask_captcha2-1.0.0.tar` & `flask_captcha2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:59:00.123263 flask_captcha2-1.0.0/
--rw-rw-rw-   0        0        0      571 2023-05-17 16:59:00.122263 flask_captcha2-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      102 2023-05-17 15:52:17.000000 flask_captcha2-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 16:59:00.120262 flask_captcha2-1.0.0/flask_captcha2.egg-info/
--rw-rw-rw-   0        0        0      571 2023-05-17 16:59:00.000000 flask_captcha2-1.0.0/flask_captcha2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-17 16:59:00.000000 flask_captcha2-1.0.0/flask_captcha2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:59:00.000000 flask_captcha2-1.0.0/flask_captcha2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-17 16:59:00.000000 flask_captcha2-1.0.0/flask_captcha2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:59:00.000000 flask_captcha2-1.0.0/flask_captcha2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 16:59:00.123263 flask_captcha2-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-05-17 16:58:53.000000 flask_captcha2-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:47.234081 flask_captcha2-1.1.0/
+-rw-rw-rw-   0        0        0      571 2023-05-17 17:03:47.233081 flask_captcha2-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2023-05-17 15:52:17.000000 flask_captcha2-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:47.232082 flask_captcha2-1.1.0/flask_captcha2.egg-info/
+-rw-rw-rw-   0        0        0      571 2023-05-17 17:03:47.000000 flask_captcha2-1.1.0/flask_captcha2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-17 17:03:47.000000 flask_captcha2-1.1.0/flask_captcha2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:03:47.000000 flask_captcha2-1.1.0/flask_captcha2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-17 17:03:47.000000 flask_captcha2-1.1.0/flask_captcha2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:03:47.000000 flask_captcha2-1.1.0/flask_captcha2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:03:47.234081 flask_captcha2-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-17 17:02:55.000000 flask_captcha2-1.1.0/setup.py
```

### Comparing `flask_captcha2-1.0.0/PKG-INFO` & `flask_captcha2-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask_captcha2
-Version: 1.0.0
+Version: 1.1.0
 Summary: an light and simple flask extension for integrate google recaptcha with Flask Apps
 Home-page: https://github.com/alisharify7/flask_captcha2
 Author: Ali Sharify
 Author-email: alisharifyofficial@gmail.com
 License: MIT
 Description: # flask_captcha
         an light  and simple flask extension for integrate google recaptcha with Flask Apps
```

### Comparing `flask_captcha2-1.0.0/flask_captcha2.egg-info/PKG-INFO` & `flask_captcha2-1.1.0/flask_captcha2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: flask-captcha2
-Version: 1.0.0
+Version: 1.1.0
 Summary: an light and simple flask extension for integrate google recaptcha with Flask Apps
 Home-page: https://github.com/alisharify7/flask_captcha2
 Author: Ali Sharify
 Author-email: alisharifyofficial@gmail.com
 License: MIT
 Description: # flask_captcha
         an light  and simple flask extension for integrate google recaptcha with Flask Apps
```

### Comparing `flask_captcha2-1.0.0/setup.py` & `flask_captcha2-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("./readme.md") as f:
     long_description = f.read()
 
 setup(
     name="flask_captcha2",
-    version="1.0.0",
+    version="1.1.0",
     description="an light and simple flask extension for integrate google recaptcha with Flask Apps",
-    packages=find_packages(),
+    packages=find_packages(where="src/flask_captcha2"),
     author_email="alisharifyofficial@gmail.com",
     author="Ali Sharify",
     url="https://github.com/alisharify7/flask_captcha2",
     long_description=long_description,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10"
```

