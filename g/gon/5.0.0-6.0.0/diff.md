# Comparing `tmp/gon-5.0.0.tar.gz` & `tmp/gon-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gon-5.0.0.tar", last modified: Thu Apr 21 11:07:00 2022, max compression
+gzip compressed data, was "gon-6.0.0.tar", last modified: Wed May 17 10:20:04 2023, max compression
```

## Comparing `gon-5.0.0.tar` & `gon-6.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 11:07:00.795073 gon-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-04-21 11:06:46.000000 gon-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-04-21 11:06:46.000000 gon-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-04-21 11:07:00.795073 gon-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5129 2022-04-21 11:06:46.000000 gon-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 11:07:00.791073 gon-5.0.0/gon/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-21 11:06:46.000000 gon-5.0.0/gon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-04-21 11:06:46.000000 gon-5.0.0/gon/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 11:07:00.795073 gon-5.0.0/gon/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7079 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/angle.py
--rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/compound.py
--rw-r--r--   0 runner    (1001) docker     (121)    28379 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/contour.py
--rw-r--r--   0 runner    (1001) docker     (121)     8273 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/empty.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/iterable.py
--rw-r--r--   0 runner    (1001) docker     (121)    97392 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/mix.py
--rw-r--r--   0 runner    (1001) docker     (121)    18756 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/multipoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    48968 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (121)    27029 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/multisegment.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/packing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6665 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/point.py
--rw-r--r--   0 runner    (1001) docker     (121)    40268 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)    17260 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/segment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9625 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/vector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-04-21 11:06:46.000000 gon-5.0.0/gon/core/vertices.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-04-21 11:06:46.000000 gon-5.0.0/gon/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 11:07:00.791073 gon-5.0.0/gon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-04-21 11:07:00.000000 gon-5.0.0/gon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-04-21 11:07:00.000000 gon-5.0.0/gon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 11:07:00.000000 gon-5.0.0/gon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-04-21 11:07:00.000000 gon-5.0.0/gon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-04-21 11:07:00.000000 gon-5.0.0/gon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-04-21 11:06:46.000000 gon-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-21 11:07:00.795073 gon-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-04-21 11:06:46.000000 gon-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:20:04.568293 gon-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 10:19:52.000000 gon-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 10:19:52.000000 gon-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-17 10:20:04.568293 gon-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-17 10:19:52.000000 gon-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:20:04.564293 gon-6.0.0/gon/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 10:19:52.000000 gon-6.0.0/gon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-17 10:19:52.000000 gon-6.0.0/gon/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:20:04.564293 gon-6.0.0/gon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97392 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48968 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/multisegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40268 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 10:19:52.000000 gon-6.0.0/gon/core/vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 10:19:52.000000 gon-6.0.0/gon/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:20:04.564293 gon-6.0.0/gon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-17 10:20:04.000000 gon-6.0.0/gon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-17 10:20:04.000000 gon-6.0.0/gon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:20:04.000000 gon-6.0.0/gon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-17 10:20:04.000000 gon-6.0.0/gon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 10:20:04.000000 gon-6.0.0/gon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-17 10:19:52.000000 gon-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:20:04.568293 gon-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-17 10:19:52.000000 gon-6.0.0/setup.py
```

### Comparing `gon-5.0.0/LICENSE` & `gon-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/PKG-INFO` & `gon-6.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 Metadata-Version: 2.1
 Name: gon
-Version: 5.0.0
+Version: 6.0.0
 Summary: Processing of planar geometries.
 Home-page: https://github.com/lycantropos/gon/
 Download-URL: https://github.com/lycantropos/gon/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
-Platform: UNKNOWN
+        
+        Copyright (c) 2019 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.2
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 gon
 ===
 
 [![](https://github.com/lycantropos/gon/workflows/CI/badge.svg)](https://github.com/lycantropos/gon/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/gon/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/gon "Codecov")
@@ -51,16 +73,16 @@
 - efficiency: all operations are efficient
 in terms of both time & memory complexity,
 upper bound for expected time complexity is `O(n * log n)`,
 for memory complexity is `O(n)`.
 
 ---
 
-In what follows `python` is an alias for `python3.6` or `pypy3.6`
-or any later version (`python3.7`, `pypy3.7` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.7`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
@@ -245,9 +267,7 @@
   ```powershell
   .\run-tests.ps1 cpython
   ```
 - with `PyPy`
   ```powershell
   .\run-tests.ps1 pypy
   ```
-
-
```

### Comparing `gon-5.0.0/README.md` & `gon-6.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 - efficiency: all operations are efficient
 in terms of both time & memory complexity,
 upper bound for expected time complexity is `O(n * log n)`,
 for memory complexity is `O(n)`.
 
 ---
 
-In what follows `python` is an alias for `python3.6` or `pypy3.6`
-or any later version (`python3.7`, `pypy3.7` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.7`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
```

### Comparing `gon-5.0.0/gon/base.py` & `gon-6.0.0/gon/base.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/angle.py` & `gon-6.0.0/gon/core/angle.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/compound.py` & `gon-6.0.0/gon/core/compound.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/contour.py` & `gon-6.0.0/gon/core/contour.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/empty.py` & `gon-6.0.0/gon/core/empty.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/geometry.py` & `gon-6.0.0/gon/core/geometry.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/iterable.py` & `gon-6.0.0/gon/core/iterable.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/mix.py` & `gon-6.0.0/gon/core/mix.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/multipoint.py` & `gon-6.0.0/gon/core/multipoint.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/multipolygon.py` & `gon-6.0.0/gon/core/multipolygon.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/multisegment.py` & `gon-6.0.0/gon/core/multisegment.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/packing.py` & `gon-6.0.0/gon/core/packing.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/point.py` & `gon-6.0.0/gon/core/point.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/polygon.py` & `gon-6.0.0/gon/core/polygon.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/segment.py` & `gon-6.0.0/gon/core/segment.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/utils.py` & `gon-6.0.0/gon/core/utils.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/vector.py` & `gon-6.0.0/gon/core/vector.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon/core/vertices.py` & `gon-6.0.0/gon/core/vertices.py`

 * *Files identical despite different names*

### Comparing `gon-5.0.0/gon.egg-info/PKG-INFO` & `gon-6.0.0/gon.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 Metadata-Version: 2.1
 Name: gon
-Version: 5.0.0
+Version: 6.0.0
 Summary: Processing of planar geometries.
 Home-page: https://github.com/lycantropos/gon/
 Download-URL: https://github.com/lycantropos/gon/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
-Platform: UNKNOWN
+        
+        Copyright (c) 2019 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.2
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 gon
 ===
 
 [![](https://github.com/lycantropos/gon/workflows/CI/badge.svg)](https://github.com/lycantropos/gon/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/gon/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/gon "Codecov")
@@ -51,16 +73,16 @@
 - efficiency: all operations are efficient
 in terms of both time & memory complexity,
 upper bound for expected time complexity is `O(n * log n)`,
 for memory complexity is `O(n)`.
 
 ---
 
-In what follows `python` is an alias for `python3.6` or `pypy3.6`
-or any later version (`python3.7`, `pypy3.7` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.7`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
@@ -245,9 +267,7 @@
   ```powershell
   .\run-tests.ps1 cpython
   ```
 - with `PyPy`
   ```powershell
   .\run-tests.ps1 pypy
   ```
-
-
```

### Comparing `gon-5.0.0/gon.egg-info/SOURCES.txt` & `gon-6.0.0/gon.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.py
 gon/__init__.py
 gon/base.py
 gon/hints.py
 gon.egg-info/PKG-INFO
 gon.egg-info/SOURCES.txt
 gon.egg-info/dependency_links.txt
```

