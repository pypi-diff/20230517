# Comparing `tmp/persian_num2words-1.0.2.tar.gz` & `tmp/persian_num2words-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian_num2words-1.0.2.tar", last modified: Sun May 14 13:33:53 2023, max compression
+gzip compressed data, was "persian_num2words-1.1.tar", last modified: Wed May 17 18:21:24 2023, max compression
```

## Comparing `persian_num2words-1.0.2.tar` & `persian_num2words-1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:33:53.978482 persian_num2words-1.0.2/
--rw-r--r--   0 mostafa    (501) staff       (20)     1068 2023-05-14 12:03:58.000000 persian_num2words-1.0.2/LICENSE.txt
--rw-r--r--   0 mostafa    (501) staff       (20)     1846 2023-05-14 13:33:53.978524 persian_num2words-1.0.2/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)      163 2023-05-14 12:03:02.000000 persian_num2words-1.0.2/README.md
--rw-r--r--   0 mostafa    (501) staff       (20)       84 2023-05-14 12:00:11.000000 persian_num2words-1.0.2/pyproject.toml
--rw-r--r--   0 mostafa    (501) staff       (20)      736 2023-05-14 13:33:53.978729 persian_num2words-1.0.2/setup.cfg
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:33:53.976815 persian_num2words-1.0.2/src/
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:33:53.977548 persian_num2words-1.0.2/src/main_module/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.0.2/src/main_module/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    12495 2023-05-14 13:32:45.000000 persian_num2words-1.0.2/src/main_module/num2words.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:33:53.978012 persian_num2words-1.0.2/src/persian_num2words.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)     1846 2023-05-14 13:33:53.000000 persian_num2words-1.0.2/src/persian_num2words.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)      370 2023-05-14 13:33:53.000000 persian_num2words-1.0.2/src/persian_num2words.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2023-05-14 13:33:53.000000 persian_num2words-1.0.2/src/persian_num2words.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       25 2023-05-14 13:33:53.000000 persian_num2words-1.0.2/src/persian_num2words.egg-info/top_level.txt
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:33:53.978260 persian_num2words-1.0.2/src/small_module/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.0.2/src/small_module/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)      156 2023-05-13 19:21:29.000000 persian_num2words-1.0.2/src/small_module/small_function.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:33:53.978374 persian_num2words-1.0.2/tests/
--rw-r--r--   0 mostafa    (501) staff       (20)      228 2023-05-14 11:52:26.000000 persian_num2words-1.0.2/tests/test_num2word.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522441 persian_num2words-1.1/
+-rw-r--r--   0 mostafa    (501) staff       (20)     1068 2023-05-14 12:03:58.000000 persian_num2words-1.1/LICENSE.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)     1844 2023-05-17 18:21:24.522486 persian_num2words-1.1/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)      163 2023-05-14 12:03:02.000000 persian_num2words-1.1/README.md
+-rw-r--r--   0 mostafa    (501) staff       (20)       84 2023-05-14 12:00:11.000000 persian_num2words-1.1/pyproject.toml
+-rw-r--r--   0 mostafa    (501) staff       (20)      734 2023-05-17 18:21:24.522716 persian_num2words-1.1/setup.cfg
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.520718 persian_num2words-1.1/src/
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.521485 persian_num2words-1.1/src/num2words/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.1/src/num2words/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    12495 2023-05-14 13:32:45.000000 persian_num2words-1.1/src/num2words/num2words.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522027 persian_num2words-1.1/src/persian_num2words.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)     1844 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)      352 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       16 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522216 persian_num2words-1.1/src/utils/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.1/src/utils/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      156 2023-05-13 19:21:29.000000 persian_num2words-1.1/src/utils/small_function.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522334 persian_num2words-1.1/tests/
+-rw-r--r--   0 mostafa    (501) staff       (20)      228 2023-05-14 11:52:26.000000 persian_num2words-1.1/tests/test_num2word.py
```

### Comparing `persian_num2words-1.0.2/LICENSE.txt` & `persian_num2words-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `persian_num2words-1.0.2/PKG-INFO` & `persian_num2words-1.1/src/persian_num2words.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: persian_num2words
-Version: 1.0.2
+Name: persian-num2words
+Version: 1.1
 Summary: A Package to Convert Numbers to Words in Persian.
 Home-page: https://github.com/mosihere/persian_num2words
 Author: Mosihere
 Author-email: mosihere@gmail.com
 Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/issues
 Project-URL: repository, https://github.com/mosihere/persian_num2words
 Classifier: Programming Language :: Python :: 3
```

### Comparing `persian_num2words-1.0.2/setup.cfg` & `persian_num2words-1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = persian_num2words
-version = 1.0.2
+version = 1.1
 author = Mosihere
 author_email = mosihere@gmail.com
 description = A Package to Convert Numbers to Words in Persian.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mosihere/persian_num2words
 project_urls =
```

### Comparing `persian_num2words-1.0.2/src/main_module/num2words.py` & `persian_num2words-1.1/src/num2words/num2words.py`

 * *Files identical despite different names*

### Comparing `persian_num2words-1.0.2/src/persian_num2words.egg-info/PKG-INFO` & `persian_num2words-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: persian-num2words
-Version: 1.0.2
+Name: persian_num2words
+Version: 1.1
 Summary: A Package to Convert Numbers to Words in Persian.
 Home-page: https://github.com/mosihere/persian_num2words
 Author: Mosihere
 Author-email: mosihere@gmail.com
 Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/issues
 Project-URL: repository, https://github.com/mosihere/persian_num2words
 Classifier: Programming Language :: Python :: 3
```

