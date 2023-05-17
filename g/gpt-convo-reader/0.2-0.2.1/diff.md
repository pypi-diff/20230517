# Comparing `tmp/gpt-convo-reader-0.2.tar.gz` & `tmp/gpt-convo-reader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-convo-reader-0.2.tar", last modified: Wed May 17 10:24:01 2023, max compression
+gzip compressed data, was "gpt-convo-reader-0.2.1.tar", last modified: Wed May 17 10:43:08 2023, max compression
```

## Comparing `gpt-convo-reader-0.2.tar` & `gpt-convo-reader-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.2/LICENSE
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     3168 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2580 2023-05-17 10:15:47.000000 gpt-convo-reader-0.2/README.md
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/setup.cfg
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1065 2023-05-17 10:05:52.000000 gpt-convo-reader-0.2/setup.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.841961 gpt-convo-reader-0.2/src/
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/src/converter/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.2/src/converter/__init__.py
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1542 2023-05-17 10:04:19.000000 gpt-convo-reader-0.2/src/converter/config.py
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2391 2023-05-17 10:11:35.000000 gpt-convo-reader-0.2/src/converter/convert.py
--rwxrwxr-x   0 romilly   (1000) romilly   (1000)     4132 2023-05-17 10:11:35.000000 gpt-convo-reader-0.2/src/converter/gui.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     3168 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      398 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/entry_points.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       15 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/requires.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/top_level.txt
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:43:08.025932 gpt-convo-reader-0.2.1/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.2.1/LICENSE
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     3170 2023-05-17 10:43:08.025932 gpt-convo-reader-0.2.1/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2580 2023-05-17 10:15:47.000000 gpt-convo-reader-0.2.1/README.md
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-17 10:43:08.029932 gpt-convo-reader-0.2.1/setup.cfg
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1085 2023-05-17 10:42:48.000000 gpt-convo-reader-0.2.1/setup.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:43:08.025932 gpt-convo-reader-0.2.1/src/
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:43:08.025932 gpt-convo-reader-0.2.1/src/converter/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.2.1/src/converter/__init__.py
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1542 2023-05-17 10:04:19.000000 gpt-convo-reader-0.2.1/src/converter/config.py
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2391 2023-05-17 10:11:35.000000 gpt-convo-reader-0.2.1/src/converter/convert.py
+-rwxrwxr-x   0 romilly   (1000) romilly   (1000)     4132 2023-05-17 10:11:35.000000 gpt-convo-reader-0.2.1/src/converter/gui.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:43:08.025932 gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     3170 2023-05-17 10:43:08.000000 gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      398 2023-05-17 10:43:08.000000 gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-17 10:43:08.000000 gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-17 10:43:08.000000 gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/entry_points.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       23 2023-05-17 10:43:08.000000 gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/requires.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-17 10:43:08.000000 gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/top_level.txt
```

### Comparing `gpt-convo-reader-0.2/LICENSE` & `gpt-convo-reader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2/PKG-INFO` & `gpt-convo-reader-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-convo-reader
-Version: 0.2
+Version: 0.2.1
 Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
 Home-page: https://github.com/romilly/gpt-convo-reader
 Author: Romilly Cocking
 Author-email: romilly.cocking@gmail.com
 Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpt-convo-reader-0.2/README.md` & `gpt-convo-reader-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2/setup.cfg` & `gpt-convo-reader-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2/setup.py` & `gpt-convo-reader-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-convo-reader",
-    version="0.2",
+    version="0.2.1",
     author="Romilly Cocking",
     author_email="romilly.cocking@gmail.com",
     description="Lets you find, view and format the conversations you've had with ChatGPT in the playground.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/romilly/gpt-convo-reader",
     project_urls={
@@ -21,14 +21,15 @@
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.10",
     install_requires=[
         "guizero >= 1.4.0",
+        "appdirs"
     ],
     entry_points={
         "console_scripts": [
             "gpt_reader_gui = converter:start",
         ],
     },
```

### Comparing `gpt-convo-reader-0.2/src/converter/config.py` & `gpt-convo-reader-0.2.1/src/converter/config.py`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2/src/converter/convert.py` & `gpt-convo-reader-0.2.1/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2/src/converter/gui.py` & `gpt-convo-reader-0.2.1/src/converter/gui.py`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/PKG-INFO` & `gpt-convo-reader-0.2.1/src/gpt_convo_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-convo-reader
-Version: 0.2
+Version: 0.2.1
 Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
 Home-page: https://github.com/romilly/gpt-convo-reader
 Author: Romilly Cocking
 Author-email: romilly.cocking@gmail.com
 Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

