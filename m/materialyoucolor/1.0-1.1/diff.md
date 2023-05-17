# Comparing `tmp/materialyoucolor-1.0.tar.gz` & `tmp/materialyoucolor-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "materialyoucolor-1.0.tar", last modified: Sat Apr 22 12:50:44 2023, max compression
+gzip compressed data, was "materialyoucolor-1.1.tar", last modified: Thu Apr 27 16:45:47 2023, max compression
```

## Comparing `materialyoucolor-1.0.tar` & `materialyoucolor-1.1.tar`

### file list

```diff
@@ -1,12 +1,38 @@
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 12:50:44.629552 materialyoucolor-1.0/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     1068 2023-04-22 12:23:08.000000 materialyoucolor-1.0/LICENSE
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     2489 2023-04-22 12:50:44.629552 materialyoucolor-1.0/PKG-INFO
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     2244 2023-04-22 12:50:13.000000 materialyoucolor-1.0/README.md
-drwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)        0 2023-04-22 12:50:44.629552 materialyoucolor-1.0/materialyoucolor.egg-info/
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)     2489 2023-04-22 12:50:43.000000 materialyoucolor-1.0/materialyoucolor.egg-info/PKG-INFO
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)      225 2023-04-22 12:50:43.000000 materialyoucolor-1.0/materialyoucolor.egg-info/SOURCES.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        1 2023-04-22 12:50:43.000000 materialyoucolor-1.0/materialyoucolor.egg-info/dependency_links.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        7 2023-04-22 12:50:43.000000 materialyoucolor-1.0/materialyoucolor.egg-info/requires.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)        1 2023-04-22 12:50:43.000000 materialyoucolor-1.0/materialyoucolor.egg-info/top_level.txt
--rw-r--r--   0 tdynamos  (1000) tdynamos  (1000)       38 2023-04-22 12:50:44.629552 materialyoucolor-1.0/setup.cfg
--rwxr-xr-x   0 tdynamos  (1000) tdynamos  (1000)      623 2023-04-22 12:46:42.000000 materialyoucolor-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.593905 materialyoucolor-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 16:45:26.000000 materialyoucolor-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-27 16:45:47.593905 materialyoucolor-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-27 16:45:26.000000 materialyoucolor-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.585905 materialyoucolor-1.1/materialyoucolor/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/blend/blend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/hct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/cam16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/hct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/viewing_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/palettes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/core_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/tonal_palette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/scheme/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/score/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/score/score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.593905 materialyoucolor-1.1/materialyoucolor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/theme_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:45:47.593905 materialyoucolor-1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      750 2023-04-27 16:45:26.000000 materialyoucolor-1.1/setup.py
```

### Comparing `materialyoucolor-1.0/LICENSE` & `materialyoucolor-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.0/PKG-INFO` & `materialyoucolor-1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: materialyoucolor
-Version: 1.0
-Summary: Material You color generation algorithms in pure python!
-Author: Ansh Dadwal
-Author-email: anshdadwal298@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # materialyoucolor-pyhton
 Material You color algorithms for python (crossplatform)!
 
 SEE : https://m3.material.io/styles/color/dynamic-color/overview
 
 ## How does it works?
 Android performs the following steps to generate color schemes from a user's wallpaper.
@@ -31,19 +22,24 @@
 
 ## Where to use this colors?
 
 SEE : https://m3.material.io/styles/color/the-color-system/color-roles
 
 ## Install 
 
-Always use master branch
+Always prefer master branch
+
+```console
+pip3 install https://github.com/T-Dynamos/materialyoucolor-pyhton/archive/main.zip
 
 ```
- pip install https://github.com/T-Dynamos/materialyoucolor-pyhton/archive/main.zip
+or 
 
+```console
+pip3 install materialyoucolor
 ```
 
 ## Documentation
 
 Please see `example.py`, its well documented by AI.
 
 ## Example
```

### Comparing `materialyoucolor-1.0/README.md` & `materialyoucolor-1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: materialyoucolor
+Version: 1.1
+Summary: Material You color generation algorithms in pure python!
+Author: Ansh Dadwal
+Author-email: anshdadwal298@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # materialyoucolor-pyhton
 Material You color algorithms for python (crossplatform)!
 
 SEE : https://m3.material.io/styles/color/dynamic-color/overview
 
 ## How does it works?
 Android performs the following steps to generate color schemes from a user's wallpaper.
@@ -22,19 +31,24 @@
 
 ## Where to use this colors?
 
 SEE : https://m3.material.io/styles/color/the-color-system/color-roles
 
 ## Install 
 
-Always use master branch
+Always prefer master branch
+
+```console
+pip3 install https://github.com/T-Dynamos/materialyoucolor-pyhton/archive/main.zip
 
 ```
- pip install https://github.com/T-Dynamos/materialyoucolor-pyhton/archive/main.zip
+or 
 
+```console
+pip3 install materialyoucolor
 ```
 
 ## Documentation
 
 Please see `example.py`, its well documented by AI.
 
 ## Example
```

### Comparing `materialyoucolor-1.0/materialyoucolor.egg-info/PKG-INFO` & `materialyoucolor-1.1/materialyoucolor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: materialyoucolor
-Version: 1.0
+Version: 1.1
 Summary: Material You color generation algorithms in pure python!
 Author: Ansh Dadwal
 Author-email: anshdadwal298@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # materialyoucolor-pyhton
@@ -31,19 +31,24 @@
 
 ## Where to use this colors?
 
 SEE : https://m3.material.io/styles/color/the-color-system/color-roles
 
 ## Install 
 
-Always use master branch
+Always prefer master branch
+
+```console
+pip3 install https://github.com/T-Dynamos/materialyoucolor-pyhton/archive/main.zip
 
 ```
- pip install https://github.com/T-Dynamos/materialyoucolor-pyhton/archive/main.zip
+or 
 
+```console
+pip3 install materialyoucolor
 ```
 
 ## Documentation
 
 Please see `example.py`, its well documented by AI.
 
 ## Example
```

