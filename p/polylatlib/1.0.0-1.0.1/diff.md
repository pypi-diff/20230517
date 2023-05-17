# Comparing `tmp/polylatlib-1.0.0.tar.gz` & `tmp/polylatlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylatlib-1.0.0.tar", max compression
+gzip compressed data, was "polylatlib-1.0.1.tar", max compression
```

## Comparing `polylatlib-1.0.0.tar` & `polylatlib-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1140 2023-01-04 22:12:24.259520 polylatlib-1.0.0/README.md
--rw-r--r--   0        0        0      511 2023-05-17 19:52:11.959457 polylatlib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-17 19:01:49.251289 polylatlib-1.0.0/src/polylatlib/__init__.py
--rw-r--r--   0        0        0       81 2023-05-17 19:01:49.251473 polylatlib-1.0.0/src/polylatlib/classes/__init__.py
--rw-r--r--   0        0        0    41080 2023-05-17 19:01:49.251907 polylatlib-1.0.0/src/polylatlib/classes/base_shapes.py
--rw-r--r--   0        0        0     4329 2023-05-17 19:01:49.252123 polylatlib-1.0.0/src/polylatlib/classes/nonregular.py
--rw-r--r--   0        0        0    21954 2023-05-17 19:01:49.252392 polylatlib-1.0.0/src/polylatlib/classes/regular.py
--rw-r--r--   0        0        0     1525 2023-05-17 19:01:49.252587 polylatlib-1.0.0/src/polylatlib/exception.py
--rw-r--r--   0        0        0     1364 2023-05-17 19:01:49.252724 polylatlib-1.0.0/src/polylatlib/functions.py
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 polylatlib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      941 2023-05-17 19:56:52.262503 polylatlib-1.0.1/README.md
+-rw-r--r--   0        0        0      511 2023-05-17 19:58:29.230973 polylatlib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-05-17 19:01:49.251289 polylatlib-1.0.1/src/polylatlib/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-17 19:01:49.251473 polylatlib-1.0.1/src/polylatlib/classes/__init__.py
+-rw-r--r--   0        0        0    41080 2023-05-17 19:01:49.251907 polylatlib-1.0.1/src/polylatlib/classes/base_shapes.py
+-rw-r--r--   0        0        0     4329 2023-05-17 19:01:49.252123 polylatlib-1.0.1/src/polylatlib/classes/nonregular.py
+-rw-r--r--   0        0        0    21954 2023-05-17 19:01:49.252392 polylatlib-1.0.1/src/polylatlib/classes/regular.py
+-rw-r--r--   0        0        0     1525 2023-05-17 19:01:49.252587 polylatlib-1.0.1/src/polylatlib/exception.py
+-rw-r--r--   0        0        0     1364 2023-05-17 19:01:49.252724 polylatlib-1.0.1/src/polylatlib/functions.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 polylatlib-1.0.1/PKG-INFO
```

### Comparing `polylatlib-1.0.0/README.md` & `polylatlib-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,12 +11,11 @@
 ----------------
 - Basic class structure for Polygons.
 - Methods to generate and draw Regular Polygons, with preset regular polygons classes.
 - Lattice generation for Equilateral Triangles, Squares, and Hexagons.
 
 To Install:
 -----------
-1. Copy the repo's HTTPS address from the GitHub page: https://github.com/RexGreenway/polylatlib
-2. In the command line use that address and pip to install the library to your desired Python environment:
+You can install the library using `pip`:
 ```
-pip install git+https://github.com/RexGreenway/polylatlib
+pip install polylatlib
 ```
```

### Comparing `polylatlib-1.0.0/src/polylatlib/classes/base_shapes.py` & `polylatlib-1.0.1/src/polylatlib/classes/base_shapes.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.0/src/polylatlib/classes/nonregular.py` & `polylatlib-1.0.1/src/polylatlib/classes/nonregular.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.0/src/polylatlib/classes/regular.py` & `polylatlib-1.0.1/src/polylatlib/classes/regular.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.0/src/polylatlib/exception.py` & `polylatlib-1.0.1/src/polylatlib/exception.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.0/src/polylatlib/functions.py` & `polylatlib-1.0.1/src/polylatlib/functions.py`

 * *Files identical despite different names*

### Comparing `polylatlib-1.0.0/PKG-INFO` & `polylatlib-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylatlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library providing the functionality to generate, work with, view, and manipulate polygons and their lattices in the 2D space.
 Home-page: https://github.com/RexGreenway/PolyLatLib
 License: GPL-3.0-or-later
 Author: Rex Greenway
 Author-email: rexgreenway@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -30,13 +30,12 @@
 ----------------
 - Basic class structure for Polygons.
 - Methods to generate and draw Regular Polygons, with preset regular polygons classes.
 - Lattice generation for Equilateral Triangles, Squares, and Hexagons.
 
 To Install:
 -----------
-1. Copy the repo's HTTPS address from the GitHub page: https://github.com/RexGreenway/polylatlib
-2. In the command line use that address and pip to install the library to your desired Python environment:
+You can install the library using `pip`:
 ```
-pip install git+https://github.com/RexGreenway/polylatlib
+pip install polylatlib
 ```
```

