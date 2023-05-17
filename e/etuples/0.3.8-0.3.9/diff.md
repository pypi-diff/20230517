# Comparing `tmp/etuples-0.3.8.tar.gz` & `tmp/etuples-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etuples-0.3.8.tar", last modified: Tue Sep  6 20:32:10 2022, max compression
+gzip compressed data, was "etuples-0.3.9.tar", last modified: Wed May 17 05:29:50 2023, max compression
```

## Comparing `etuples-0.3.8.tar` & `etuples-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:32:10.721389 etuples-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11527 2022-09-06 20:32:10.000000 etuples-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-06 20:32:10.000000 etuples-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5770 2022-09-06 20:32:10.721389 etuples-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-09-06 20:32:10.000000 etuples-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:32:10.721389 etuples-0.3.8/etuples/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-06 20:32:10.721389 etuples-0.3.8/etuples/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    10130 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     5523 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:32:10.721389 etuples-0.3.8/etuples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5770 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-06 20:32:10.000000 etuples-0.3.8/etuples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-09-06 20:32:10.721389 etuples-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-09-06 20:32:10.000000 etuples-0.3.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80044 2022-09-06 20:32:10.000000 etuples-0.3.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:29:50.815104 etuples-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-05-17 05:29:49.000000 etuples-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 05:29:49.000000 etuples-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-17 05:29:50.815104 etuples-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-17 05:29:49.000000 etuples-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:29:50.815104 etuples-0.3.9/etuples/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-17 05:29:49.000000 etuples-0.3.9/etuples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 05:29:50.815104 etuples-0.3.9/etuples/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-05-17 05:29:49.000000 etuples-0.3.9/etuples/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-17 05:29:49.000000 etuples-0.3.9/etuples/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:29:50.815104 etuples-0.3.9/etuples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-17 05:29:50.000000 etuples-0.3.9/etuples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-17 05:29:50.000000 etuples-0.3.9/etuples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:29:50.000000 etuples-0.3.9/etuples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 05:29:50.000000 etuples-0.3.9/etuples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 05:29:50.000000 etuples-0.3.9/etuples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-17 05:29:50.815104 etuples-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-17 05:29:49.000000 etuples-0.3.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-17 05:29:49.000000 etuples-0.3.9/versioneer.py
```

### Comparing `etuples-0.3.8/LICENSE` & `etuples-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `etuples-0.3.8/PKG-INFO` & `etuples-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: etuples
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python S-expression emulation using tuple-like objects.
 Home-page: http://github.com/pythological/etuples
 Maintainer: Brandon T. Willard
 Maintainer-email: brandonwillard+etuples@gmail.com
 License: UNKNOWN
 Description: # `etuples`
-        
-        [![Build Status](https://travis-ci.org/pythological/etuples.svg?branch=main)](https://travis-ci.org/pythological/etuples) [![Coverage Status](https://coveralls.io/repos/github/pythological/etuples/badge.svg?branch=main)](https://coveralls.io/github/pythological/etuples?branch=main) [![PyPI](https://img.shields.io/pypi/v/etuples)](https://pypi.org/project/etuples/)
+        [![Tests](https://github.com/pythological/etuples/actions/workflows/tests.yml/badge.svg)](https://github.com/pythological/etuples/actions/workflows/tests.yml) [![Coverage Status](https://coveralls.io/repos/github/pythological/etuples/badge.svg?branch=main)](https://coveralls.io/github/pythological/etuples?branch=main) [![PyPI](https://img.shields.io/pypi/v/etuples)](https://pypi.org/project/etuples/)
         
         Python [S-expression](https://en.wikipedia.org/wiki/S-expression) emulation using tuple-like objects.
         
         ## Examples
         
         `etuple`s are like tuples:
         
@@ -168,15 +167,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `etuples-0.3.8/README.md` & `etuples-0.3.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # `etuples`
-
-[![Build Status](https://travis-ci.org/pythological/etuples.svg?branch=main)](https://travis-ci.org/pythological/etuples) [![Coverage Status](https://coveralls.io/repos/github/pythological/etuples/badge.svg?branch=main)](https://coveralls.io/github/pythological/etuples?branch=main) [![PyPI](https://img.shields.io/pypi/v/etuples)](https://pypi.org/project/etuples/)
+[![Tests](https://github.com/pythological/etuples/actions/workflows/tests.yml/badge.svg)](https://github.com/pythological/etuples/actions/workflows/tests.yml) [![Coverage Status](https://coveralls.io/repos/github/pythological/etuples/badge.svg?branch=main)](https://coveralls.io/github/pythological/etuples?branch=main) [![PyPI](https://img.shields.io/pypi/v/etuples)](https://pypi.org/project/etuples/)
 
 Python [S-expression](https://en.wikipedia.org/wiki/S-expression) emulation using tuple-like objects.
 
 ## Examples
 
 `etuple`s are like tuples:
```

### Comparing `etuples-0.3.8/etuples/core.py` & `etuples-0.3.9/etuples/core.py`

 * *Files identical despite different names*

### Comparing `etuples-0.3.8/etuples/dispatch.py` & `etuples-0.3.9/etuples/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,20 @@
             # Everything is equal and there are no logic variables
             yield u
             return
 
         if getattr(u, "_parent", None) and all(res_same):
             # If we simply swapped-out logic variables, then we don't want to
             # lose the parent etuple information.
-            res = etuple(*res)
+            res = type(u)(res)
             res._parent = u._parent
             yield res
             return
 
-        yield etuple(*res)
+        yield type(u)(res)
 
     _reify.add((ExpressionTuple, Mapping), _reify_ExpressionTuple)
 
     def _reify_KwdPair(u, s):
         arg = yield _reify(u.arg, s)
         value = yield _reify(u.value, s)
```

### Comparing `etuples-0.3.8/etuples.egg-info/PKG-INFO` & `etuples-0.3.9/etuples.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: etuples
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python S-expression emulation using tuple-like objects.
 Home-page: http://github.com/pythological/etuples
 Maintainer: Brandon T. Willard
 Maintainer-email: brandonwillard+etuples@gmail.com
 License: UNKNOWN
 Description: # `etuples`
-        
-        [![Build Status](https://travis-ci.org/pythological/etuples.svg?branch=main)](https://travis-ci.org/pythological/etuples) [![Coverage Status](https://coveralls.io/repos/github/pythological/etuples/badge.svg?branch=main)](https://coveralls.io/github/pythological/etuples?branch=main) [![PyPI](https://img.shields.io/pypi/v/etuples)](https://pypi.org/project/etuples/)
+        [![Tests](https://github.com/pythological/etuples/actions/workflows/tests.yml/badge.svg)](https://github.com/pythological/etuples/actions/workflows/tests.yml) [![Coverage Status](https://coveralls.io/repos/github/pythological/etuples/badge.svg?branch=main)](https://coveralls.io/github/pythological/etuples?branch=main) [![PyPI](https://img.shields.io/pypi/v/etuples)](https://pypi.org/project/etuples/)
         
         Python [S-expression](https://en.wikipedia.org/wiki/S-expression) emulation using tuple-like objects.
         
         ## Examples
         
         `etuple`s are like tuples:
         
@@ -168,15 +167,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `etuples-0.3.8/setup.cfg` & `etuples-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `etuples-0.3.8/setup.py` & `etuples-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     packages=["etuples"],
     install_requires=[
         "cons",
         "multipledispatch",
     ],
     long_description=open("README.md").read() if exists("README.md") else "",
     long_description_content_type="text/markdown",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
```

### Comparing `etuples-0.3.8/versioneer.py` & `etuples-0.3.9/versioneer.py`

 * *Files identical despite different names*

