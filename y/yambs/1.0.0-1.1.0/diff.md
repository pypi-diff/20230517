# Comparing `tmp/yambs-1.0.0.tar.gz` & `tmp/yambs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.0.0.tar", last modified: Tue May 16 08:31:13 2023, max compression
+gzip compressed data, was "yambs-1.1.0.tar", last modified: Wed May 17 02:44:16 2023, max compression
```

## Comparing `yambs-1.0.0.tar` & `yambs-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 08:30:07.000000 yambs-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-16 08:31:13.057013 yambs-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-16 08:30:07.000000 yambs-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 08:30:07.000000 yambs-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:31:13.057013 yambs-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-16 08:30:07.000000 yambs-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.053013 yambs-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 08:30:07.000000 yambs-1.0.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 08:30:07.000000 yambs-1.0.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.053013 yambs-1.0.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.053013 yambs-1.0.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 02:43:13.000000 yambs-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-17 02:44:16.654503 yambs-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-17 02:43:13.000000 yambs-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 02:43:13.000000 yambs-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 02:44:16.654503 yambs-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-17 02:43:13.000000 yambs-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.650503 yambs-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-17 02:43:13.000000 yambs-1.1.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-17 02:43:13.000000 yambs-1.1.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.650503 yambs-1.1.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.650503 yambs-1.1.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 02:43:13.000000 yambs-1.1.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:44:16.654503 yambs-1.1.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 02:44:16.000000 yambs-1.1.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.0.0/LICENSE` & `yambs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/PKG-INFO` & `yambs-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=10d8dec6920a0145a083815ad6bc3e00
+    hash=6f0dde62ff0b6f57cc4c8520ac87412c
     =====================================
 -->
 
-# yambs ([1.0.0](https://pypi.org/project/yambs/))
+# yambs ([1.1.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.0.0/README.md` & `yambs-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=10d8dec6920a0145a083815ad6bc3e00
+    hash=6f0dde62ff0b6f57cc4c8520ac87412c
     =====================================
 -->
 
-# yambs ([1.0.0](https://pypi.org/project/yambs/))
+# yambs ([1.1.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.0.0/pyproject.toml` & `yambs-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.0.0"
+version = "1.1.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.0.0/setup.py` & `yambs-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/tests/test_entry.py` & `yambs-1.1.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/app.py` & `yambs-1.1.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/commands/all.py` & `yambs-1.1.0/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/commands/gen.py` & `yambs-1.1.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/config/__init__.py` & `yambs-1.1.0/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/data/schemas/Chip.yaml` & `yambs-1.1.0/yambs/data/schemas/Chip.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 ---
 type: object
 additionalProperties: false
-required: [arch, cpu]
+required: [architecture, cpu]
 
 properties:
-  toolchain:
-    type: string
-    default: arm-picolibc-eabi
-  arch:
+  architecture:
     type: string
   cpu:
     type: string
 
   extra_cflags:
     type: array
     default: []
```

### Comparing `yambs-1.0.0/yambs/data/schemas/Config.yaml` & `yambs-1.1.0/yambs/data/schemas/Config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 type: object
 additionalProperties: false
-required: [boards, chips, toolchains]
+required: [boards, chips, toolchains, architectures]
 
 properties:
   boards:
     type: array
     items:
       $ref: package://yambs/schemas/Board.yaml
 
@@ -19,14 +19,21 @@
   toolchains:
     type: object
     additionalProperties: false
     patternProperties:
       "^[a-zA-Z0-9-_.]+$":
         $ref: package://yambs/schemas/Toolchain.yaml
 
+  architectures:
+    type: object
+    additionalProperties: false
+    patternProperties:
+      "^[a-zA-Z0-9-_.+]+$":
+        $ref: package://yambs/schemas/Architecture.yaml
+
   src_root:
     type: string
     default: src
 
   default_target:
     type: string
     default: all_boards
@@ -39,16 +46,21 @@
     type: string
     default: build
 
   toolchains_root:
     type: string
     default: "./toolchains/$toolchain/out/bin"
 
+  # If set, overrides any other toolchain pathing or prefix construction.
+  toolchain_prefix:
+    type: string
+    default: ""
+
   cc:
     type: string
     default: gcc
 
   common_cflags:
     type: array
-    default: [-Wall, -Werror]
+    default: [-Wall, -Werror, -g]
     items:
       type: string
```

### Comparing `yambs-1.0.0/yambs/entry.py` & `yambs-1.1.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/generate/boards.py` & `yambs-1.1.0/yambs/generate/boards.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,28 +27,40 @@
 
 
 def write_continuation(stream: TextIO, offset: str) -> None:
     """Write a line continuation."""
     stream.write(" $" + linesep + offset)
 
 
-def write_link_line(stream: TextIO, source: Path, all_srcs: Set[Path]) -> None:
+def write_link_line(
+    stream: TextIO, source: Path, all_srcs: Set[Path], base: Path
+) -> None:
     """
     Write a ninja configuration line for an application requiring linking.
     """
 
-    line = f"build $build_dir/{source.with_suffix('.elf')}: link "
+    source = source.relative_to(base)
+
+    elf = f"$build_dir/{source.with_suffix('.elf')}"
+    line = f"build {elf}: link "
     offset = " " * len(line)
     stream.write(line + f"$build_dir/{source.with_suffix('.o')}")
 
     for src in all_srcs:
         write_continuation(stream, offset)
-        stream.write(f"$build_dir/{src.with_suffix('.o')}")
+        stream.write(f"$build_dir/{src.relative_to(base).with_suffix('.o')}")
+    stream.write(linesep)
 
-    stream.write(linesep + linesep)
+    # Add lines for creating binaries.
+    bin_path = f"$build_dir/{source.with_suffix('.bin')}"
+    stream.write(f"build {bin_path}: bin {elf}" + linesep)
+
+    # Add an objdump target.
+    dump_path = f"$build_dir/{source.with_suffix('.dump')}"
+    stream.write(f"build {dump_path}: dump {elf}" + linesep + linesep)
 
 
 def is_source(path: Path) -> bool:
     """Determine if a file is a source file."""
 
     return path.name.endswith(".c") or path.name.endswith(".cc")
 
@@ -73,29 +85,25 @@
     """Create paths based on common pathing conventions."""
 
     chip = config.data["chips"][board["chip"]]  # type: ignore
 
     return {
         "Common": root.joinpath("common"),
         "Chip": root.joinpath("chips", board["chip"]),
-        "Architecture": root.joinpath(chip["arch"]),  # type: ignore
+        "Architecture": root.joinpath(chip["architecture"]),  # type: ignore
         "CPU": root.joinpath(chip["cpu"]),  # type: ignore
         "Board": root.joinpath("boards", board["name"]),
     }
 
 
 def write_sources(
-    stream: TextIO, board: Dict[str, Any], config: Config
+    stream: TextIO, board: Dict[str, Any], config: Config, src_root: Path
 ) -> Tuple[Set[Path], Set[Path]]:
     """Write the source-file manifest."""
 
-    stream.write(f"src_dir = {config.data['src_root']}" + linesep)
-
-    src_root = rel(config.directory("src_root"))
-
     # Add regular sources.
     all_srcs: Set[Path] = set()
     for kind, path in create_paths_dict(src_root, board, config).items():
         add_dir(
             stream,
             all_srcs,
             path,
@@ -111,57 +119,68 @@
         add_dir(
             stream, app_srcs, path, f"{kind} application sources", src_root
         )
 
     return all_srcs, app_srcs
 
 
-def write_phony(stream: TextIO, all_srcs: Set[Path]) -> None:
+def write_phony(stream: TextIO, app_srcs: Set[Path], base: Path) -> None:
     """Write the phony target."""
 
-    if all_srcs:
-        srcs = list(all_srcs)
-        first = srcs[0]
-        srcs = srcs[1:]
-
-        line = "build apps: phony "
-        offset = " " * len(line)
-        stream.write(line + f"$build_dir/{first.with_suffix('.elf')}")
-        for src in srcs:
-            write_continuation(stream, offset)
-            stream.write(f"$build_dir/{src.with_suffix('.elf')}")
+    phonies = [("apps", ".bin"), ("dumps", ".dump")]
+
+    if app_srcs:
+        for phony, suffix in phonies:
+            srcs = list(app_srcs)
+            first = srcs[0].relative_to(base)
+            srcs = srcs[1:]
+
+            line = f"build {phony}: phony "
+            offset = " " * len(line)
+            stream.write(line + f"$build_dir/{first.with_suffix(suffix)}")
+            for src in srcs:
+                write_continuation(stream, offset)
+                src = src.relative_to(base)
+                stream.write(f"$build_dir/{src.with_suffix(suffix)}")
+
+            stream.write(linesep)
 
 
 def generate(jinja: Environment, ninja_root: Path, config: Config) -> None:
     """Generate board-related ninja files."""
 
     # Render the board manifest and rules file.
     for template in ["all.ninja", "rules.ninja"]:
         render_template(jinja, ninja_root, template, config.data)
 
+    src_root = rel(config.directory("src_root"))
+
     # Render board top-level files.
     board: Dict[str, Any] = {}
     for board in config.data["boards"]:  # type: ignore
         board_root = ninja_root.joinpath("boards", board["name"])
         board_root.mkdir(parents=True, exist_ok=True)
         render_template(jinja, board_root, "board.ninja", board)
 
         # Perform source-file discovery.
         with board_root.joinpath("sources.ninja").open("w") as path_fd:
-            all_srcs, app_srcs = write_sources(path_fd, board, config)
+            path_fd.write(f"src_dir = {config.data['src_root']}" + linesep)
+
+            all_srcs, app_srcs = write_sources(
+                path_fd, board, config, src_root
+            )
 
         print(
             (
                 f"({board['name']}) Found {len(all_srcs)} "
                 f"sources and {len(app_srcs)} applications."
             )
         )
 
         # Write the application manifest.
         with board_root.joinpath("apps.ninja").open("w") as path_fd:
             for app_src in app_srcs:
-                write_link_line(path_fd, app_src, all_srcs)
+                write_link_line(path_fd, app_src, all_srcs, src_root)
 
             # Write the phony target.
             path_fd.write("# A target to build all applications." + linesep)
-            write_phony(path_fd, all_srcs)
-            path_fd.write(linesep)
+            write_phony(path_fd, app_srcs, src_root)
```

### Comparing `yambs-1.0.0/yambs/generate/chips.py` & `yambs-1.1.0/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/generate/common.py` & `yambs-1.1.0/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/generate/toolchains.py` & `yambs-1.1.0/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs/schemas.py` & `yambs-1.1.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.0.0/yambs.egg-info/PKG-INFO` & `yambs-1.1.0/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=10d8dec6920a0145a083815ad6bc3e00
+    hash=6f0dde62ff0b6f57cc4c8520ac87412c
     =====================================
 -->
 
-# yambs ([1.0.0](https://pypi.org/project/yambs/))
+# yambs ([1.1.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.0.0/yambs.egg-info/SOURCES.txt` & `yambs-1.1.0/yambs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,26 @@
 yambs.egg-info/entry_points.txt
 yambs.egg-info/requires.txt
 yambs.egg-info/top_level.txt
 yambs/commands/__init__.py
 yambs/commands/all.py
 yambs/commands/gen.py
 yambs/config/__init__.py
+yambs/data/schemas/Architecture.yaml
 yambs/data/schemas/Board.yaml
 yambs/data/schemas/Chip.yaml
 yambs/data/schemas/Config.yaml
 yambs/data/schemas/Toolchain.yaml
 yambs/data/templates/all.ninja.j2
+yambs/data/templates/architecture.ninja.j2
 yambs/data/templates/board.ninja.j2
 yambs/data/templates/build.ninja.j2
 yambs/data/templates/chip.ld.j2
 yambs/data/templates/chip.ninja.j2
 yambs/data/templates/rules.ninja.j2
 yambs/data/templates/toolchain.ninja.j2
 yambs/generate/__init__.py
+yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
 yambs/generate/common.py
 yambs/generate/toolchains.py
```

