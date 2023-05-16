# Comparing `tmp/flashpass-1.0.0.tar.gz` & `tmp/flashpass-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashpass-1.0.0.tar", max compression
+gzip compressed data, was "flashpass-1.0.1.tar", max compression
```

## Comparing `flashpass-1.0.0.tar` & `flashpass-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    18091 2023-05-16 22:18:05.635681 flashpass-1.0.0/LICENSE
--rw-r--r--   0        0        0     1270 2023-05-16 22:18:05.635681 flashpass-1.0.0/README.rst
--rw-r--r--   0        0        0       45 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/__init__.py
--rw-r--r--   0        0        0       72 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/__main__.py
--rw-r--r--   0        0        0     4926 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/cli.py
--rw-r--r--   0        0        0     7064 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/crypto.py
--rw-r--r--   0        0        0     2823 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/exceptions.py
--rw-r--r--   0        0        0     4157 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/io.py
--rw-r--r--   0        0        0     1500 2023-05-16 22:18:05.635681 flashpass-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 flashpass-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18091 2023-05-16 22:28:16.555334 flashpass-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1270 2023-05-16 22:28:16.555334 flashpass-1.0.1/README.rst
+-rw-r--r--   0        0        0       45 2023-05-16 22:28:16.555334 flashpass-1.0.1/flashpass/__init__.py
+-rw-r--r--   0        0        0       72 2023-05-16 22:28:16.555334 flashpass-1.0.1/flashpass/__main__.py
+-rw-r--r--   0        0        0     4926 2023-05-16 22:28:16.555334 flashpass-1.0.1/flashpass/cli.py
+-rw-r--r--   0        0        0     7064 2023-05-16 22:28:16.559334 flashpass-1.0.1/flashpass/crypto.py
+-rw-r--r--   0        0        0     2823 2023-05-16 22:28:16.559334 flashpass-1.0.1/flashpass/exceptions.py
+-rw-r--r--   0        0        0     4157 2023-05-16 22:28:16.559334 flashpass-1.0.1/flashpass/io.py
+-rw-r--r--   0        0        0     1500 2023-05-16 22:28:16.559334 flashpass-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 flashpass-1.0.1/PKG-INFO
```

### Comparing `flashpass-1.0.0/LICENSE` & `flashpass-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flashpass-1.0.0/README.rst` & `flashpass-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `flashpass-1.0.0/flashpass/cli.py` & `flashpass-1.0.1/flashpass/cli.py`

 * *Files identical despite different names*

### Comparing `flashpass-1.0.0/flashpass/crypto.py` & `flashpass-1.0.1/flashpass/crypto.py`

 * *Files identical despite different names*

### Comparing `flashpass-1.0.0/flashpass/exceptions.py` & `flashpass-1.0.1/flashpass/exceptions.py`

 * *Files identical despite different names*

### Comparing `flashpass-1.0.0/flashpass/io.py` & `flashpass-1.0.1/flashpass/io.py`

 * *Files identical despite different names*

### Comparing `flashpass-1.0.0/pyproject.toml` & `flashpass-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flashpass"
-version = "1.0.0"
+version = "1.0.1"
 description = "Encrypt & Decrypt FlashPass .fp files"
 authors = ["Carson Mullins <carsonmullins@yahoo.com>"]
 license = "GPL-2.0-only"
 readme = "README.rst"
 repository = "https://github.com/Septem151/flashpass"
 keywords = ["security", "passwords"]
 classifiers = [
```

### Comparing `flashpass-1.0.0/PKG-INFO` & `flashpass-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashpass
-Version: 1.0.0
+Version: 1.0.1
 Summary: Encrypt & Decrypt FlashPass .fp files
 Home-page: https://github.com/Septem151/flashpass
 License: GPL-2.0-only
 Keywords: security,passwords
 Author: Carson Mullins
 Author-email: carsonmullins@yahoo.com
 Requires-Python: >=3.11,<4.0
```

