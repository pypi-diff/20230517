# Comparing `tmp/manim_lamination_builder-0.2.1.tar.gz` & `tmp/manim_lamination_builder-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_lamination_builder-0.2.1.tar", last modified: Sun May 14 20:27:42 2023, max compression
+gzip compressed data, was "manim_lamination_builder-0.2.3.tar", last modified: Wed May 17 15:04:00 2023, max compression
```

## Comparing `manim_lamination_builder-0.2.1.tar` & `manim_lamination_builder-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/LICENSE
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43796 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3429 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/README.md
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/manim_lamination_builder/
--rw-r--r--   0 forrest   (1000) forrest   (1000)      975 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/__init__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)      429 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/__main__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/animation.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/chord.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/custom_json.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4398 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/generate.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/lamination.py
--rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/main.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4464 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/morph.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     6826 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/points.py
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43796 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)      635 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/SOURCES.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/dependency_links.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       17 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/requires.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/top_level.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)      701 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/pyproject.toml
--rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/setup.cfg
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 15:04:00.254668 manim_lamination_builder-0.2.3/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/LICENSE
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 15:04:00.251335 manim_lamination_builder-0.2.3/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3590 2023-05-17 01:50:11.000000 manim_lamination_builder-0.2.3/README.md
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 15:04:00.251335 manim_lamination_builder-0.2.3/manim_lamination_builder/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      975 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/__init__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      423 2023-05-16 01:05:30.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/__main__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/animation.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/chord.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/custom_json.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4398 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/generate.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/lamination.py
+-rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/main.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4464 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/morph.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     6826 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.3/manim_lamination_builder/points.py
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 15:04:00.251335 manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 15:04:00.000000 manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      635 2023-05-17 15:04:00.000000 manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-05-17 15:04:00.000000 manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       17 2023-05-17 15:04:00.000000 manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/requires.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-05-17 15:04:00.000000 manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/top_level.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      701 2023-05-17 01:50:32.000000 manim_lamination_builder-0.2.3/pyproject.toml
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-05-17 15:04:00.254668 manim_lamination_builder-0.2.3/setup.cfg
```

### Comparing `manim_lamination_builder-0.2.1/LICENSE` & `manim_lamination_builder-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/PKG-INFO` & `manim_lamination_builder-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim_lamination_builder
-Version: 0.2.1
+Version: 0.2.3
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -669,30 +669,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WORK IN PROGRESS
 This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
 
 # Installation:
 Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex. Afterward, you can simply run
 ```
 pip install manim_lamination_builder
 ```
 
-# Usage: 
+# Example Uses:
 ## render multiple laminations in one image
 ```
-python -m manim_lamination_builder file.json
+python -m manim_lamination_builder file.json5
 ```
-The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen). The blank lamination is permitted.
+The input format is as follows: A json or json5 list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom placemen). The blank lamination is permitted.
 ```
 [
   {
     polygons:[["_001","_010","_100"]],
     chords:[["_1","2"]],
     points: ["3"],
     radix: 4
@@ -719,15 +718,15 @@
 
 with tempconfig({"quality": "high_quality", "preview": True}):
     Main(generate_unicritical_lamination(4, 3)).render()
 ```
 ![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
 
 ## animate the leaves and points moving to their images
-Please not that sigma_d is understood as a dilation of angular position with wrapping, so the forgotten digit is recorded and used to determine how many times to wrap around. 
+Please note that the animation does over its duration what sigma_3 does in one step. Moreover, this relies on the understanding that sigma_d is a dilation of angular position with wrapping (by a factor of d). So the forgotten digit is recorded and used to determine how many times to wrap around, which might not always be desirable. 
 ```
 from manim import Scene, WHITE, tempconfig
 from manim_lamination_builder import (
     parse_lamination,
     curried_colorize_with_respect_to,
     sigma,
     AnimateLamination,
```

### Comparing `manim_lamination_builder-0.2.1/README.md` & `manim_lamination_builder-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# WORK IN PROGRESS
 This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
 
 # Installation:
 Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex. Afterward, you can simply run
 ```
 pip install manim_lamination_builder
 ```
 
-# Usage: 
+# Example Uses:
 ## render multiple laminations in one image
 ```
-python -m manim_lamination_builder file.json
+python -m manim_lamination_builder file.json5
 ```
-The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen). The blank lamination is permitted.
+The input format is as follows: A json or json5 list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom placemen). The blank lamination is permitted.
 ```
 [
   {
     polygons:[["_001","_010","_100"]],
     chords:[["_1","2"]],
     points: ["3"],
     radix: 4
@@ -44,15 +43,15 @@
 
 with tempconfig({"quality": "high_quality", "preview": True}):
     Main(generate_unicritical_lamination(4, 3)).render()
 ```
 ![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
 
 ## animate the leaves and points moving to their images
-Please not that sigma_d is understood as a dilation of angular position with wrapping, so the forgotten digit is recorded and used to determine how many times to wrap around. 
+Please note that the animation does over its duration what sigma_3 does in one step. Moreover, this relies on the understanding that sigma_d is a dilation of angular position with wrapping (by a factor of d). So the forgotten digit is recorded and used to determine how many times to wrap around, which might not always be desirable. 
 ```
 from manim import Scene, WHITE, tempconfig
 from manim_lamination_builder import (
     parse_lamination,
     curried_colorize_with_respect_to,
     sigma,
     AnimateLamination,
```

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/__init__.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/animation.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/animation.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/chord.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/chord.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/custom_json.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/custom_json.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/generate.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/generate.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/lamination.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/lamination.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/main.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/main.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/morph.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/morph.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder/points.py` & `manim_lamination_builder-0.2.3/manim_lamination_builder/points.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/PKG-INFO` & `manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-lamination-builder
-Version: 0.2.1
+Version: 0.2.3
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -669,30 +669,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WORK IN PROGRESS
 This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
 
 # Installation:
 Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex. Afterward, you can simply run
 ```
 pip install manim_lamination_builder
 ```
 
-# Usage: 
+# Example Uses:
 ## render multiple laminations in one image
 ```
-python -m manim_lamination_builder file.json
+python -m manim_lamination_builder file.json5
 ```
-The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen). The blank lamination is permitted.
+The input format is as follows: A json or json5 list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom placemen). The blank lamination is permitted.
 ```
 [
   {
     polygons:[["_001","_010","_100"]],
     chords:[["_1","2"]],
     points: ["3"],
     radix: 4
@@ -719,15 +718,15 @@
 
 with tempconfig({"quality": "high_quality", "preview": True}):
     Main(generate_unicritical_lamination(4, 3)).render()
 ```
 ![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
 
 ## animate the leaves and points moving to their images
-Please not that sigma_d is understood as a dilation of angular position with wrapping, so the forgotten digit is recorded and used to determine how many times to wrap around. 
+Please note that the animation does over its duration what sigma_3 does in one step. Moreover, this relies on the understanding that sigma_d is a dilation of angular position with wrapping (by a factor of d). So the forgotten digit is recorded and used to determine how many times to wrap around, which might not always be desirable. 
 ```
 from manim import Scene, WHITE, tempconfig
 from manim_lamination_builder import (
     parse_lamination,
     curried_colorize_with_respect_to,
     sigma,
     AnimateLamination,
```

### Comparing `manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/SOURCES.txt` & `manim_lamination_builder-0.2.3/manim_lamination_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.1/pyproject.toml` & `manim_lamination_builder-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "manim_lamination_builder"
-version = "0.2.1"
+version = "0.2.3"
 authors = [
   { name="Forrest Hilton", email="forrestmhilton@gmail.com" },
 ]
 description = "a replacement to lamination builder that uses manim instead of the browser"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

