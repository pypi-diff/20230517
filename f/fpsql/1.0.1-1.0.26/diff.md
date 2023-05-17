# Comparing `tmp/fpsql-1.0.1.tar.gz` & `tmp/fpsql-1.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpsql-1.0.1.tar", max compression
+gzip compressed data, was "fpsql-1.0.26.tar", max compression
```

## Comparing `fpsql-1.0.1.tar` & `fpsql-1.0.26.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.532794 fpsql-1.0.1/LICENSE
--rw-r--r--   0        0        0      162 2023-05-17 19:07:09.401248 fpsql-1.0.1/README.md
--rw-r--r--   0        0        0      864 2023-05-17 19:05:38.885295 fpsql-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5014 2023-05-17 19:07:39.225232 fpsql-1.0.1/src/fpsql/__init__.py
--rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 fpsql-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.532794 fpsql-1.0.26/LICENSE
+-rw-r--r--   0        0        0     2047 2023-05-15 19:26:02.011608 fpsql-1.0.26/README.md
+-rw-r--r--   0        0        0      865 2023-05-15 23:48:11.802544 fpsql-1.0.26/pyproject.toml
+-rw-r--r--   0        0        0     5064 2023-05-15 23:55:00.981663 fpsql-1.0.26/src/fpsql/__init__.py
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 fpsql-1.0.26/PKG-INFO
```

### Comparing `fpsql-1.0.1/LICENSE` & `fpsql-1.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `fpsql-1.0.1/pyproject.toml` & `fpsql-1.0.26/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fpsql"
-version = "1.0.1"
+version = "1.0.26"
 authors = ["Firepup650 <firepyp650@gmail.com>"]
 description = "An easy to use SQLite package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `fpsql-1.0.1/src/fpsql/__init__.py` & `fpsql-1.0.26/src/fpsql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 __VERSION__ = "1.0.26"
 __NEW__ = "Adds `remove_prefix` and `remove_suffix`, name mangles internal variables in `sql`, fixes a bug in `console.warn`, adds `__VERSION__`, `__NEW__`, and `__LICENSE__`, adds many aliases for interactive help."
 __LICENSE__ = "MIT"
 
 
 class sql:
+    """# Class: sql
+    Easy SQL manipulation"""
+
     def addTable(self, tableName: str) -> None:
         """# Function: sql.addTable
           Adds a table to the database
         # Inputs:
           tableName: str - The name of the table to create
 
         # Returns:
```

