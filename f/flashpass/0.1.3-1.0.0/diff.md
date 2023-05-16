# Comparing `tmp/flashpass-0.1.3.tar.gz` & `tmp/flashpass-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashpass-0.1.3.tar", max compression
+gzip compressed data, was "flashpass-1.0.0.tar", max compression
```

## Comparing `flashpass-0.1.3.tar` & `flashpass-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    18091 2021-10-10 13:12:57.763815 flashpass-0.1.3/LICENSE
--rw-r--r--   0        0        0     1270 2021-10-27 01:49:31.265743 flashpass-0.1.3/README.rst
--rw-r--r--   0        0        0       45 2022-04-22 03:29:36.334614 flashpass-0.1.3/flashpass/__init__.py
--rw-r--r--   0        0        0       72 2021-11-11 20:38:11.890426 flashpass-0.1.3/flashpass/__main__.py
--rw-r--r--   0        0        0     4926 2022-04-22 03:38:21.071240 flashpass-0.1.3/flashpass/cli.py
--rw-r--r--   0        0        0     7064 2022-04-22 03:33:19.774341 flashpass-0.1.3/flashpass/crypto.py
--rw-r--r--   0        0        0     2823 2021-09-01 07:35:06.000000 flashpass-0.1.3/flashpass/exceptions.py
--rw-r--r--   0        0        0     4157 2022-04-22 03:33:58.384411 flashpass-0.1.3/flashpass/io.py
--rw-r--r--   0        0        0     1112 2022-04-22 03:45:59.080678 flashpass-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2140 2022-04-22 03:47:53.172494 flashpass-0.1.3/setup.py
--rw-r--r--   0        0        0     2203 2022-04-22 03:47:53.172696 flashpass-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    18091 2023-05-16 22:18:05.635681 flashpass-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1270 2023-05-16 22:18:05.635681 flashpass-1.0.0/README.rst
+-rw-r--r--   0        0        0       45 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/__init__.py
+-rw-r--r--   0        0        0       72 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/__main__.py
+-rw-r--r--   0        0        0     4926 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/cli.py
+-rw-r--r--   0        0        0     7064 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/crypto.py
+-rw-r--r--   0        0        0     2823 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/exceptions.py
+-rw-r--r--   0        0        0     4157 2023-05-16 22:18:05.635681 flashpass-1.0.0/flashpass/io.py
+-rw-r--r--   0        0        0     1500 2023-05-16 22:18:05.635681 flashpass-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 flashpass-1.0.0/PKG-INFO
```

### Comparing `flashpass-0.1.3/LICENSE` & `flashpass-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flashpass-0.1.3/README.rst` & `flashpass-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `flashpass-0.1.3/flashpass/cli.py` & `flashpass-1.0.0/flashpass/cli.py`

 * *Files identical despite different names*

### Comparing `flashpass-0.1.3/flashpass/crypto.py` & `flashpass-1.0.0/flashpass/crypto.py`

 * *Files identical despite different names*

### Comparing `flashpass-0.1.3/flashpass/exceptions.py` & `flashpass-1.0.0/flashpass/exceptions.py`

 * *Files identical despite different names*

### Comparing `flashpass-0.1.3/flashpass/io.py` & `flashpass-1.0.0/flashpass/io.py`

 * *Files identical despite different names*

### Comparing `flashpass-0.1.3/pyproject.toml` & `flashpass-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flashpass"
-version = "0.1.3"
+version = "1.0.0"
 description = "Encrypt & Decrypt FlashPass .fp files"
 authors = ["Carson Mullins <carsonmullins@yahoo.com>"]
 license = "GPL-2.0-only"
 readme = "README.rst"
 repository = "https://github.com/Septem151/flashpass"
 keywords = ["security", "passwords"]
 classifiers = [
@@ -15,34 +15,55 @@
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Security",
   "Topic :: Utilities",
   "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-cryptography = "^36.0.2"
+python = "^3.11"
+cryptography = "^40.0.2"
 pyperclip = "^1.8.2"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.1"
-black = "^22.3.0"
-pylint = "^2.13.7"
-mypy = "^0.942"
-isort = "^5.10.1"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+isort = "^5.12.0"
+lxml = "^4.9.2"
+mypy = "^1.3.0"
+pylint = "^2.17.4"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
+[tool.mypy]
+warn_return_any = true
+warn_unused_configs = true
+warn_unreachable = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+show_column_numbers = true
+check_untyped_defs = true
+follow_imports = "silent"
+
+[[tool.mypy.overrides]]
+module = [
+  "pyperclip",
+  "pytest"
+]
+ignore_missing_imports = true
+
+[tool.poetry.scripts]
+flashpass = "flashpass.cli:main"
+
 [tool.pylint.messages_control]
 disable = "C0330, C0326, W0511"
 
+[tool.pylint.design]
+max-args = "6"
+
 [tool.pylint.format]
 max-line-length = "88"
-
-
-[tool.poetry.scripts]
-flashpass = "flashpass.cli:main"
```

### Comparing `flashpass-0.1.3/PKG-INFO` & `flashpass-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: flashpass
-Version: 0.1.3
+Version: 1.0.0
 Summary: Encrypt & Decrypt FlashPass .fp files
 Home-page: https://github.com/Septem151/flashpass
 License: GPL-2.0-only
 Keywords: security,passwords
 Author: Carson Mullins
 Author-email: carsonmullins@yahoo.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: cryptography (>=36.0.2,<37.0.0)
+Requires-Dist: cryptography (>=40.0.2,<41.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Project-URL: Repository, https://github.com/Septem151/flashpass
 Description-Content-Type: text/x-rst
 
 =========
 FlashPass
 =========
```

