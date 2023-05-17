# Comparing `tmp/manim_lamination_builder-0.2.5.tar.gz` & `tmp/manim_lamination_builder-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_lamination_builder-0.2.5.tar", last modified: Wed May 17 17:17:37 2023, max compression
+gzip compressed data, was "manim_lamination_builder-0.2.6.tar", last modified: Wed May 17 21:22:35 2023, max compression
```

## Comparing `manim_lamination_builder-0.2.5.tar` & `manim_lamination_builder-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 17:17:37.176496 manim_lamination_builder-0.2.5/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/LICENSE
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 17:17:37.176496 manim_lamination_builder-0.2.5/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3590 2023-05-17 01:50:11.000000 manim_lamination_builder-0.2.5/README.md
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 17:17:37.176496 manim_lamination_builder-0.2.5/manim_lamination_builder/
--rw-r--r--   0 forrest   (1000) forrest   (1000)      998 2023-05-17 16:04:10.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/__init__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)      423 2023-05-16 01:05:30.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/__main__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/animation.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/chord.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/custom_json.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4398 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/generate.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/lamination.py
--rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/main.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4464 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/morph.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     6826 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.5/manim_lamination_builder/points.py
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 17:17:37.176496 manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 17:17:37.000000 manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)      635 2023-05-17 17:17:37.000000 manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/SOURCES.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-05-17 17:17:37.000000 manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/dependency_links.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       12 2023-05-17 17:17:37.000000 manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/requires.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-05-17 17:17:37.000000 manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/top_level.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)      693 2023-05-17 17:17:12.000000 manim_lamination_builder-0.2.5/pyproject.toml
--rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-05-17 17:17:37.176496 manim_lamination_builder-0.2.5/setup.cfg
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/LICENSE
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3590 2023-05-17 01:50:11.000000 manim_lamination_builder-0.2.6/README.md
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/manim_lamination_builder/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     1054 2023-05-17 21:22:09.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/__init__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      423 2023-05-16 01:05:30.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/__main__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/animation.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/chord.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/custom_json.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4398 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/generate.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/lamination.py
+-rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/main.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4464 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/morph.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     6826 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/points.py
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      635 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       12 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/requires.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/top_level.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      693 2023-05-17 21:22:29.000000 manim_lamination_builder-0.2.6/pyproject.toml
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/setup.cfg
```

### Comparing `manim_lamination_builder-0.2.5/LICENSE` & `manim_lamination_builder-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/PKG-INFO` & `manim_lamination_builder-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim_lamination_builder
-Version: 0.2.5
+Version: 0.2.6
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `manim_lamination_builder-0.2.5/README.md` & `manim_lamination_builder-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/__init__.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 from manim_lamination_builder.generate import (
     curried_colorize_with_respect_to,
     generate_sibling_portraits,
     generate_unicritical_lamination,
     remove_non_original_pollygons,
 )
 from manim_lamination_builder.main import group, Main
-import morph, __main__
+import manim_lamination_builder.morph
+import manim_lamination_builder.__main__
```

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/animation.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/animation.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/chord.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/chord.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/custom_json.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/custom_json.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/generate.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/generate.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/lamination.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/lamination.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/main.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/main.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/morph.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/morph.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder/points.py` & `manim_lamination_builder-0.2.6/manim_lamination_builder/points.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/PKG-INFO` & `manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-lamination-builder
-Version: 0.2.5
+Version: 0.2.6
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `manim_lamination_builder-0.2.5/manim_lamination_builder.egg-info/SOURCES.txt` & `manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.5/pyproject.toml` & `manim_lamination_builder-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "manim_lamination_builder"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Forrest Hilton", email="forrestmhilton@gmail.com" },
 ]
 description = "a replacement to lamination builder that uses manim instead of the browser"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

