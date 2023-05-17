# Comparing `tmp/imaginepy-1.0.1.tar.gz` & `tmp/imaginepy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaginepy-1.0.1.tar", last modified: Sun May 14 18:28:04 2023, max compression
+gzip compressed data, was "imaginepy-1.0.5.tar", last modified: Wed May 17 16:48:07 2023, max compression
```

## Comparing `imaginepy-1.0.1.tar` & `imaginepy-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 18:28:04.720192 imaginepy-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3974 2023-05-14 18:28:04.719692 imaginepy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3275 2023-05-14 18:22:45.000000 imaginepy-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 18:28:04.710191 imaginepy-1.0.1/imaginepy/
--rw-rw-rw-   0        0        0    23083 2023-05-14 17:34:40.000000 imaginepy-1.0.1/imaginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:28:04.719192 imaginepy-1.0.1/imaginepy.egg-info/
--rw-rw-rw-   0        0        0     3974 2023-05-14 18:28:04.000000 imaginepy-1.0.1/imaginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-14 18:28:04.000000 imaginepy-1.0.1/imaginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 18:28:04.000000 imaginepy-1.0.1/imaginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 18:28:04.000000 imaginepy-1.0.1/imaginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 18:28:04.000000 imaginepy-1.0.1/imaginepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 18:28:04.720692 imaginepy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1045 2023-05-14 18:27:42.000000 imaginepy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:48:07.370766 imaginepy-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4054 2023-05-17 16:48:07.370267 imaginepy-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3355 2023-05-14 18:30:19.000000 imaginepy-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 16:48:07.351766 imaginepy-1.0.5/imaginepy/
+-rw-rw-rw-   0        0        0    25557 2023-05-17 16:43:19.000000 imaginepy-1.0.5/imaginepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:48:07.369266 imaginepy-1.0.5/imaginepy.egg-info/
+-rw-rw-rw-   0        0        0     4054 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:48:07.370766 imaginepy-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2023-05-17 16:44:25.000000 imaginepy-1.0.5/setup.py
```

### Comparing `imaginepy-1.0.1/LICENSE` & `imaginepy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imaginepy-1.0.1/PKG-INFO` & `imaginepy-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaginepy
-Version: 1.0.1
+Version: 1.0.5
 Summary: Python library to create Art with AI.
 Home-page: https://github.com/ItsCEED/ImaginePY-Midjourney-Free-Alternative
 Author: CEED
 Author-email: 
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 
 - 🎨 Turn words into art
 - 👓 Choose from an array of art styles
 - 🔧 Adjust your masterpiece with creative controls!
 - 📦 Stay ahead of the game with the ever-growing art library!
 - 🌇 Generate wallpapers
 - 🔎 Discover and explore similar artistic designs
+- This is refactored and improved version of the original from [hyugogirubato]
 
 ## Installation
 
 _Note: Requires [Python] 3.7.0 or newer with PIP installed._
 
 ```shell
 $ python setup.py install
```

### Comparing `imaginepy-1.0.1/README.md` & `imaginepy-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 - 🎨 Turn words into art
 - 👓 Choose from an array of art styles
 - 🔧 Adjust your masterpiece with creative controls!
 - 📦 Stay ahead of the game with the ever-growing art library!
 - 🌇 Generate wallpapers
 - 🔎 Discover and explore similar artistic designs
+- This is refactored and improved version of the original from [hyugogirubato]
 
 ## Installation
 
 _Note: Requires [Python] 3.7.0 or newer with PIP installed._
 
 ```shell
 $ python setup.py install
```

### Comparing `imaginepy-1.0.1/imaginepy.egg-info/PKG-INFO` & `imaginepy-1.0.5/imaginepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaginepy
-Version: 1.0.1
+Version: 1.0.5
 Summary: Python library to create Art with AI.
 Home-page: https://github.com/ItsCEED/ImaginePY-Midjourney-Free-Alternative
 Author: CEED
 Author-email: 
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 
 - 🎨 Turn words into art
 - 👓 Choose from an array of art styles
 - 🔧 Adjust your masterpiece with creative controls!
 - 📦 Stay ahead of the game with the ever-growing art library!
 - 🌇 Generate wallpapers
 - 🔎 Discover and explore similar artistic designs
+- This is refactored and improved version of the original from [hyugogirubato]
 
 ## Installation
 
 _Note: Requires [Python] 3.7.0 or newer with PIP installed._
 
 ```shell
 $ python setup.py install
```

### Comparing `imaginepy-1.0.1/setup.py` & `imaginepy-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='imaginepy',
-    version='1.0.1',
+    version='1.0.5',
     author='CEED',
     author_email='',
     description='Python library to create Art with AI.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ItsCEED/ImaginePY-Midjourney-Free-Alternative',
     packages=find_packages(),
```

