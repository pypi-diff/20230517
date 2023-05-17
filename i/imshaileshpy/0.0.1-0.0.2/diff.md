# Comparing `tmp/imshaileshpy-0.0.1.tar.gz` & `tmp/imshaileshpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imshaileshpy-0.0.1.tar", last modified: Wed May 17 18:20:13 2023, max compression
+gzip compressed data, was "imshaileshpy-0.0.2.tar", last modified: Wed May 17 18:23:04 2023, max compression
```

## Comparing `imshaileshpy-0.0.1.tar` & `imshaileshpy-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-17 18:20:13.778990 imshaileshpy-0.0.1/
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     1073 2023-05-17 17:53:34.000000 imshaileshpy-0.0.1/LICENSE
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      957 2023-05-17 18:20:13.778602 imshaileshpy-0.0.1/PKG-INFO
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      170 2023-05-17 17:53:15.000000 imshaileshpy-0.0.1/README.md
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-17 18:20:13.775815 imshaileshpy-0.0.1/imshaileshpy.egg-info/
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      957 2023-05-17 18:20:13.000000 imshaileshpy-0.0.1/imshaileshpy.egg-info/PKG-INFO
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      363 2023-05-17 18:20:13.000000 imshaileshpy-0.0.1/imshaileshpy.egg-info/SOURCES.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)        1 2023-05-17 18:20:13.000000 imshaileshpy-0.0.1/imshaileshpy.egg-info/dependency_links.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)        1 2023-05-17 18:16:04.000000 imshaileshpy-0.0.1/imshaileshpy.egg-info/not-zip-safe
--rw-r--r--   0 shaileshmishra   (501) staff       (20)       38 2023-05-17 18:20:13.000000 imshaileshpy-0.0.1/imshaileshpy.egg-info/requires.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)       18 2023-05-17 18:20:13.000000 imshaileshpy-0.0.1/imshaileshpy.egg-info/top_level.txt
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      576 2023-05-17 17:55:44.000000 imshaileshpy-0.0.1/pyproject.toml
--rw-r--r--   0 shaileshmishra   (501) staff       (20)       38 2023-05-17 18:20:13.779108 imshaileshpy-0.0.1/setup.cfg
--rw-r--r--   0 shaileshmishra   (501) staff       (20)     1545 2023-05-17 18:20:09.000000 imshaileshpy-0.0.1/setup.py
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-17 18:20:13.770922 imshaileshpy-0.0.1/src/
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-17 18:20:13.777100 imshaileshpy-0.0.1/src/imshaileshpy/
--rw-r--r--   0 shaileshmishra   (501) staff       (20)        0 2023-05-17 17:46:25.000000 imshaileshpy-0.0.1/src/imshaileshpy/__init__.py'.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)        0 2023-05-17 17:46:40.000000 imshaileshpy-0.0.1/src/imshaileshpy/example.py
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      519 2023-05-17 17:42:20.000000 imshaileshpy-0.0.1/src/imshaileshpy/main.py
-drwxr-xr-x   0 shaileshmishra   (501) staff       (20)        0 2023-05-17 18:20:13.777815 imshaileshpy-0.0.1/tests/
--rw-r--r--   0 shaileshmishra   (501) staff       (20)      193 2023-05-17 18:15:12.000000 imshaileshpy-0.0.1/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:23:04.793543 imshaileshpy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-17 18:23:04.793543 imshaileshpy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:23:04.793543 imshaileshpy-0.0.2/imshaileshpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-17 18:23:04.000000 imshaileshpy-0.0.2/imshaileshpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-17 18:23:04.000000 imshaileshpy-0.0.2/imshaileshpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:23:04.000000 imshaileshpy-0.0.2/imshaileshpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/imshaileshpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:23:04.000000 imshaileshpy-0.0.2/imshaileshpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 18:23:04.000000 imshaileshpy-0.0.2/imshaileshpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:23:04.793543 imshaileshpy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:23:04.793543 imshaileshpy-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:23:04.793543 imshaileshpy-0.0.2/src/imshaileshpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/src/imshaileshpy/__init__.py'.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/src/imshaileshpy/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/src/imshaileshpy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:23:04.793543 imshaileshpy-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-17 18:22:52.000000 imshaileshpy-0.0.2/tests/test_package.py
```

### Comparing `imshaileshpy-0.0.1/LICENSE` & `imshaileshpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imshaileshpy-0.0.1/PKG-INFO` & `imshaileshpy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imshaileshpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: imshaileshpy is an example package.
 Home-page: https://github.com/ishaileshmishra/imshaileshpy
 Author: imshaileshpy
 Author-email: mshaileshr@gmail.com
 License: MIT
 Keywords: imshaileshpy-python-package
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imshaileshpy-0.0.1/imshaileshpy.egg-info/PKG-INFO` & `imshaileshpy-0.0.2/imshaileshpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imshaileshpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: imshaileshpy is an example package.
 Home-page: https://github.com/ishaileshmishra/imshaileshpy
 Author: imshaileshpy
 Author-email: mshaileshr@gmail.com
 License: MIT
 Keywords: imshaileshpy-python-package
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imshaileshpy-0.0.1/pyproject.toml` & `imshaileshpy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 name = "imshaileshpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Shailesh Misra", email = "shaileshmishra@google.com" },
 ]
 description = "A small example test package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `imshaileshpy-0.0.1/setup.py` & `imshaileshpy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'requests>=2.20.0,<3.0',
     'python-dateutil'
 ]
 
 setup(
     name="imshaileshpy",
     keywords="imshaileshpy-python-package",
-    version="0.0.1",
+    version="0.0.2",
     author="imshaileshpy",
     author_email="mshaileshr@gmail.com",
     description="imshaileshpy is an example package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ishaileshmishra/imshaileshpy",
     packages=['src/imshaileshpy/'],
```

### Comparing `imshaileshpy-0.0.1/src/imshaileshpy/main.py` & `imshaileshpy-0.0.2/src/imshaileshpy/main.py`

 * *Files identical despite different names*

