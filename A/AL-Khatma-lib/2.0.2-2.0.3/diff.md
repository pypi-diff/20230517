# Comparing `tmp/AL_Khatma_lib-2.0.2.tar.gz` & `tmp/AL_Khatma_lib-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AL_Khatma_lib-2.0.2.tar", last modified: Wed May 17 13:57:21 2023, max compression
+gzip compressed data, was "AL_Khatma_lib-2.0.3.tar", last modified: Wed May 17 14:22:02 2023, max compression
```

## Comparing `AL_Khatma_lib-2.0.2.tar` & `AL_Khatma_lib-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 13:57:21.404327 AL_Khatma_lib-2.0.2/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.2/LICENSE
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    62364 2023-05-17 13:57:21.404327 AL_Khatma_lib-2.0.2/PKG-INFO
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61853 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.2/README.md
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      656 2023-05-17 13:52:25.000000 AL_Khatma_lib-2.0.2/pyproject.toml
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-05-17 13:57:21.404327 AL_Khatma_lib-2.0.2/setup.cfg
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 13:57:21.400327 AL_Khatma_lib-2.0.2/src/
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 13:57:21.404327 AL_Khatma_lib-2.0.2/src/AL_Khatma/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     2385 2023-05-17 13:23:28.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/__init__.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1974 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/adkar.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     3223 2023-05-17 13:22:24.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/cheak.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     9584 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/khatma.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1034 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/log.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     3084 2023-05-17 13:20:01.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/message.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     8764 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/pdf_page.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    16035 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/quran.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     5226 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma/tafser.py
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 13:57:21.404327 AL_Khatma_lib-2.0.2/src/AL_Khatma_lib.egg-info/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    62364 2023-05-17 13:57:21.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma_lib.egg-info/PKG-INFO
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      411 2023-05-17 13:57:21.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-05-17 13:57:21.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-05-17 13:57:21.000000 AL_Khatma_lib-2.0.2/src/AL_Khatma_lib.egg-info/top_level.txt
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 14:22:02.920161 AL_Khatma_lib-2.0.3/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.3/LICENSE
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    62364 2023-05-17 14:22:02.920161 AL_Khatma_lib-2.0.3/PKG-INFO
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61853 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.3/README.md
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      656 2023-05-17 14:18:38.000000 AL_Khatma_lib-2.0.3/pyproject.toml
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-05-17 14:22:02.920161 AL_Khatma_lib-2.0.3/setup.cfg
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 14:22:02.912161 AL_Khatma_lib-2.0.3/src/
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 14:22:02.916161 AL_Khatma_lib-2.0.3/src/AL_Khatma/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     2385 2023-05-17 14:18:53.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/__init__.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1974 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/adkar.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     3252 2023-05-17 14:20:46.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/cheak.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     9584 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/khatma.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1034 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/log.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     3084 2023-05-17 13:20:01.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/message.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     8764 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/pdf_page.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    16035 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/quran.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     5226 2023-05-17 11:52:36.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma/tafser.py
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-17 14:22:02.920161 AL_Khatma_lib-2.0.3/src/AL_Khatma_lib.egg-info/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    62364 2023-05-17 14:22:02.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      411 2023-05-17 14:22:02.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-05-17 14:22:02.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-05-17 14:22:02.000000 AL_Khatma_lib-2.0.3/src/AL_Khatma_lib.egg-info/top_level.txt
```

### Comparing `AL_Khatma_lib-2.0.2/LICENSE` & `AL_Khatma_lib-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/PKG-INFO` & `AL_Khatma_lib-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AL_Khatma_lib
-Version: 2.0.2
+Version: 2.0.3
 Summary: A library Specialized About Islamic
 Author-email: Osamah Awadh <osamahawadh01@gmail.com>
 Project-URL: Homepage, https://github.com/oaokm/AL-Khatma
 Project-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AL_Khatma_lib Version: 2.0.2 Summary: A library
+Metadata-Version: 2.1 Name: AL_Khatma_lib Version: 2.0.3 Summary: A library
 Specialized About Islamic Author-email: Osamah Awadh
 gmail.com> Project-URL: Homepage, https://github.com/oaokm/AL-Khatma Project-
 URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
                     [AL-Khatma Logo For Arabic and English]
```

### Comparing `AL_Khatma_lib-2.0.2/README.md` & `AL_Khatma_lib-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/pyproject.toml` & `AL_Khatma_lib-2.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AL_Khatma_lib"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Osamah Awadh", email="osamahawadh01@gmail.com" },
 ]
 description = "A library Specialized About Islamic"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/__init__.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .log import log
 from .cheak import cheak
 import json
 import platform
 
 #! لا تقم بتغير رقم الإصدار
 #! Do not change the version
-__version__   = '2.0.2'
+__version__   = '2.0.3'
 __main_path__ = os.path.dirname(__file__)
 
 class json_edit:
     def __init__(self, name_file:str, refresh=False):
         self.name_file = name_file
         self.refresh   = refresh
```

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/adkar.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/adkar.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/cheak.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/cheak.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import requests
 import os
 import json
 from .log import log
 from tqdm import tqdm
 import platform
 
-main_path = os.path.dirname(__file__)
-
+main_path   = os.path.dirname(__file__)
+system_path = {
+    "Linux": "/",
+    "Windows": "\\",
+    "Darwin": "/"
+}
 class cheak:
 
     def __init__(self):
         self.download_file = list()
         self.path_url      = list()
-        self.system_path   = json.load(open(f'{main_path}/DATA/path_system.json', 'r'))
+        self.system_path   = system_path
         try:
             self.system_path[platform.system()]
         except KeyError:
             log(
             f"{__file__} > cheak >  | Error: Key Error",
             f"Switch path system to '/' , system: {platform.system()}, uname:{platform.uname()}"
             ).write_message()
```

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/khatma.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/khatma.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/log.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/log.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/message.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/message.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/pdf_page.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/pdf_page.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/quran.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/quran.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma/tafser.py` & `AL_Khatma_lib-2.0.3/src/AL_Khatma/tafser.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.2/src/AL_Khatma_lib.egg-info/PKG-INFO` & `AL_Khatma_lib-2.0.3/src/AL_Khatma_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AL-Khatma-lib
-Version: 2.0.2
+Version: 2.0.3
 Summary: A library Specialized About Islamic
 Author-email: Osamah Awadh <osamahawadh01@gmail.com>
 Project-URL: Homepage, https://github.com/oaokm/AL-Khatma
 Project-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AL-Khatma-lib Version: 2.0.2 Summary: A library
+Metadata-Version: 2.1 Name: AL-Khatma-lib Version: 2.0.3 Summary: A library
 Specialized About Islamic Author-email: Osamah Awadh
 gmail.com> Project-URL: Homepage, https://github.com/oaokm/AL-Khatma Project-
 URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
                     [AL-Khatma Logo For Arabic and English]
```

