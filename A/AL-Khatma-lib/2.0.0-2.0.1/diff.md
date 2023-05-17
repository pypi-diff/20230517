# Comparing `tmp/AL_Khatma_lib-2.0.0.tar.gz` & `tmp/AL_Khatma_lib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AL_Khatma_lib-2.0.0.tar", last modified: Tue May 16 10:57:38 2023, max compression
+gzip compressed data, was "AL_Khatma_lib-2.0.1.tar", last modified: Tue May 16 17:38:35 2023, max compression
```

## Comparing `AL_Khatma_lib-2.0.0.tar` & `AL_Khatma_lib-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:38.029604 AL_Khatma_lib-2.0.0/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.0/LICENSE
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61528 2023-05-16 10:57:38.029604 AL_Khatma_lib-2.0.0/PKG-INFO
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61017 2023-05-16 10:43:17.000000 AL_Khatma_lib-2.0.0/README.md
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      656 2023-05-16 10:56:33.000000 AL_Khatma_lib-2.0.0/pyproject.toml
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-05-16 10:57:38.029604 AL_Khatma_lib-2.0.0/setup.cfg
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:37.933599 AL_Khatma_lib-2.0.0/src/
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:38.025604 AL_Khatma_lib-2.0.0/src/AL_Khatma/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1080 2023-05-16 02:45:36.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/__init__.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1974 2023-05-16 10:17:59.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/adkar.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     2640 2023-05-16 02:22:31.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/cheak.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     9584 2023-05-16 09:51:17.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/khatma.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1034 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/log.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     4034 2023-05-16 02:44:08.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/message.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     8766 2023-05-16 10:31:28.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/pdf_page.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    16035 2023-05-16 03:26:12.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/quran.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     5226 2023-05-16 10:22:47.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/tafser.py
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:38.025604 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61528 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/PKG-INFO
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      411 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/top_level.txt
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 17:38:35.789275 AL_Khatma_lib-2.0.1/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.1/LICENSE
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61537 2023-05-16 17:38:35.785275 AL_Khatma_lib-2.0.1/PKG-INFO
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61025 2023-05-16 17:36:57.000000 AL_Khatma_lib-2.0.1/README.md
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      656 2023-05-16 17:37:32.000000 AL_Khatma_lib-2.0.1/pyproject.toml
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-05-16 17:38:35.789275 AL_Khatma_lib-2.0.1/setup.cfg
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 17:38:35.757274 AL_Khatma_lib-2.0.1/src/
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 17:38:35.785275 AL_Khatma_lib-2.0.1/src/AL_Khatma/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1080 2023-05-16 17:37:42.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/__init__.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1974 2023-05-16 10:17:59.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/adkar.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     2640 2023-05-16 02:22:31.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/cheak.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     9584 2023-05-16 09:51:17.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/khatma.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1034 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/log.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     4034 2023-05-16 02:44:08.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/message.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     8764 2023-05-16 17:34:55.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/pdf_page.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    16035 2023-05-16 03:26:12.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/quran.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     5226 2023-05-16 10:22:47.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma/tafser.py
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 17:38:35.785275 AL_Khatma_lib-2.0.1/src/AL_Khatma_lib.egg-info/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61537 2023-05-16 17:38:35.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      411 2023-05-16 17:38:35.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-05-16 17:38:35.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-05-16 17:38:35.000000 AL_Khatma_lib-2.0.1/src/AL_Khatma_lib.egg-info/top_level.txt
```

### Comparing `AL_Khatma_lib-2.0.0/LICENSE` & `AL_Khatma_lib-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/PKG-INFO` & `AL_Khatma_lib-2.0.1/src/AL_Khatma_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: AL_Khatma_lib
-Version: 2.0.0
+Name: AL-Khatma-lib
+Version: 2.0.1
 Summary: A library Specialized About Islamic
 Author-email: Osamah Awadh <osamahawadh01@gmail.com>
 Project-URL: Homepage, https://github.com/oaokm/AL-Khatma
 Project-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,15 @@
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#الترخيص">الترخيص</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/oaokm/AL-Khatma/blob/main/UPDATE.md">التحديثات</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/oaokm/AL-Khatma/issues">صفحة حل المشكلات</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
-  <a href="https://github.com/oaokm/AL-Khatma/issues/new/choose">إنشاء مشكلة</a>
+  <a href="https://github.com/oaokm/AL-Khatma/issues/new/choose">التبليغ عن مشكلة</a>
 </p>
 
 <!-- <details>
   <summary>الوصول السريع</summary>
     <p align="center">
       <a href="#فكرة_الختمة">فكرة الختمة</a>
       &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: AL_Khatma_lib Version: 2.0.0 Summary: A library
+Metadata-Version: 2.1 Name: AL-Khatma-lib Version: 2.0.1 Summary: A library
 Specialized About Islamic Author-email: Osamah Awadh
 gmail.com> Project-URL: Homepage, https://github.com/oaokm/AL-Khatma Project-
 URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
                     [AL-Khatma Logo For Arabic and English]
                             Arabic    |    English
 ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©    |    ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙØªØ¹Ø§ÙÙ
    ÙØ¹_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙÙØµØ§Ø¯Ø±    |    Ø§ÙØªØ±Ø®ÙØµ    |   
- Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª    |    ØµÙØ­Ø©_Ø­Ù_Ø§ÙÙØ´ÙÙØ§Øª    |    Ø¥ÙØ´Ø§Ø¡
-                                  ÙØ´ÙÙØ©
+       Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª    |    ØµÙØ­Ø©_Ø­Ù_Ø§ÙÙØ´ÙÙØ§Øª    |   
+                        Ø§ÙØªØ¨ÙÙØº_Ø¹Ù_ÙØ´ÙÙØ©
  ![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https:/
 /img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI]
 (https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://
 img.shields.io/github/repo-size/oaokm/AL-Khatma) --| --| -- | --| ##
 **Ø¨ÙØ§Ù** ÙÙ ÙÙÙ Ø§ÙØ«Ø§ÙØ« ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023
 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ Ø¹Ø´Ø± ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙÙ
 ÙØ°Ø§ Ø§ÙÙÙÙ Ø¨Ø¯Ø£Øª Ø§ÙÙÙØ±Ø© ÙØ¨Ø¹Ø¯ÙØ§ ÙÙØª Ø¨ØªØ·Ø¨ÙÙ
```

### Comparing `AL_Khatma_lib-2.0.0/README.md` & `AL_Khatma_lib-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: AL_Khatma_lib
+Version: 2.0.1
+Summary: A library Specialized About Islamic
+Author-email: Osamah Awadh <osamahawadh01@gmail.com>
+Project-URL: Homepage, https://github.com/oaokm/AL-Khatma
+Project-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/oaokm/AL-Khatma/main/Logo/AL_Khatma_logo_one.png" alt="AL-Khatma Logo For Arabic and English">
 </p>
 
 <p align="center">
   <a href="https://github.com/oaokm/AL-Khatma/blob/main/README.md">Arabic</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
@@ -19,15 +33,15 @@
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#الترخيص">الترخيص</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/oaokm/AL-Khatma/blob/main/UPDATE.md">التحديثات</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/oaokm/AL-Khatma/issues">صفحة حل المشكلات</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
-  <a href="https://github.com/oaokm/AL-Khatma/issues/new/choose">إنشاء مشكلة</a>
+  <a href="https://github.com/oaokm/AL-Khatma/issues/new/choose">التبليغ عن مشكلة</a>
 </p>
 
 <!-- <details>
   <summary>الوصول السريع</summary>
     <p align="center">
       <a href="#فكرة_الختمة">فكرة الختمة</a>
       &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
```

#### html2text {}

```diff
@@ -1,13 +1,20 @@
+Metadata-Version: 2.1 Name: AL_Khatma_lib Version: 2.0.1 Summary: A library
+Specialized About Islamic Author-email: Osamah Awadh
+gmail.com> Project-URL: Homepage, https://github.com/oaokm/AL-Khatma Project-
+URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE
                     [AL-Khatma Logo For Arabic and English]
                             Arabic    |    English
 ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©    |    ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙØªØ¹Ø§ÙÙ
    ÙØ¹_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙÙØµØ§Ø¯Ø±    |    Ø§ÙØªØ±Ø®ÙØµ    |   
- Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª    |    ØµÙØ­Ø©_Ø­Ù_Ø§ÙÙØ´ÙÙØ§Øª    |    Ø¥ÙØ´Ø§Ø¡
-                                  ÙØ´ÙÙØ©
+       Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª    |    ØµÙØ­Ø©_Ø­Ù_Ø§ÙÙØ´ÙÙØ§Øª    |   
+                        Ø§ÙØªØ¨ÙÙØº_Ø¹Ù_ÙØ´ÙÙØ©
  ![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https:/
 /img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI]
 (https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://
 img.shields.io/github/repo-size/oaokm/AL-Khatma) --| --| -- | --| ##
 **Ø¨ÙØ§Ù** ÙÙ ÙÙÙ Ø§ÙØ«Ø§ÙØ« ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023
 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ Ø¹Ø´Ø± ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙÙ
 ÙØ°Ø§ Ø§ÙÙÙÙ Ø¨Ø¯Ø£Øª Ø§ÙÙÙØ±Ø© ÙØ¨Ø¹Ø¯ÙØ§ ÙÙØª Ø¨ØªØ·Ø¨ÙÙ
```

### Comparing `AL_Khatma_lib-2.0.0/pyproject.toml` & `AL_Khatma_lib-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AL_Khatma_lib"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Osamah Awadh", email="osamahawadh01@gmail.com" },
 ]
 description = "A library Specialized About Islamic"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/__init__.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 from .log import log
 from .cheak import cheak
 
 #! لا تقم بتغير رقم الإصدار
 #! Do not change the version
-__version__   = '2.0.0'
+__version__   = '2.0.1'
 __main_path__ = os.path.dirname(__file__)
 
 
 def Download_DATA():
     log(
         f'{__file__} | Download DATA Request ', 
         f'The user to been request the cheak and download files form Github'
```

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/adkar.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/adkar.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/cheak.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/cheak.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/khatma.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/khatma.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/log.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/log.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/message.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/message.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/pdf_page.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/pdf_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             ).write_message()
 
         if not os.path.exists(path=f"{self.pic_path}/quran_pages"):
             log(
                 f'{file_name} > quran_pdf | Create a folder', 
                 f'Create a folder which will have high resolution images of the Quran'
                 ).write_message()
-            os.mkdir(path=f"{self.pic_path}/quran_pages")
+            os.makedirs(f"{self.pic_path}/quran_pages")
         else:
             pass
         
     def download_pages(self):
         #! التحقق من وجود تحديث جديد للمكتبة
         message().cheak_version()
         log(
```

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/quran.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/quran.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma/tafser.py` & `AL_Khatma_lib-2.0.1/src/AL_Khatma/tafser.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/PKG-INFO` & `AL_Khatma_lib-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: AL-Khatma-lib
-Version: 2.0.0
-Summary: A library Specialized About Islamic
-Author-email: Osamah Awadh <osamahawadh01@gmail.com>
-Project-URL: Homepage, https://github.com/oaokm/AL-Khatma
-Project-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img src="https://raw.githubusercontent.com/oaokm/AL-Khatma/main/Logo/AL_Khatma_logo_one.png" alt="AL-Khatma Logo For Arabic and English">
 </p>
 
 <p align="center">
   <a href="https://github.com/oaokm/AL-Khatma/blob/main/README.md">Arabic</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
@@ -33,15 +19,15 @@
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="#الترخيص">الترخيص</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/oaokm/AL-Khatma/blob/main/UPDATE.md">التحديثات</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/oaokm/AL-Khatma/issues">صفحة حل المشكلات</a>
   &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
-  <a href="https://github.com/oaokm/AL-Khatma/issues/new/choose">إنشاء مشكلة</a>
+  <a href="https://github.com/oaokm/AL-Khatma/issues/new/choose">التبليغ عن مشكلة</a>
 </p>
 
 <!-- <details>
   <summary>الوصول السريع</summary>
     <p align="center">
       <a href="#فكرة_الختمة">فكرة الختمة</a>
       &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
@@ -682,8 +668,8 @@
   * [azkar_list Muhammed-Ayad | github](https://github.com/Muhammed-Ayad/Balgho-Convey/blob/dev/lib/data/local/json/azkar_list.dart)
   * [azkar-db - osamayy | github](https://github.com/osamayy/azkar-db)
   * [hisn_almuslim - Alsarmad | github](https://github.com/Alsarmad/hisn_almuslim_json)
 
 
 
 ## **الترخيص**
-ترخيص هو: إم آي تي ([MIT © Osamah Awadh](https://github.com/oaokm/AL-Khatma/blob/main/LICENSE))
+ترخيص هو: إم آي تي ([MIT © Osamah Awadh](https://github.com/oaokm/AL-Khatma/blob/main/LICENSE))
```

#### html2text {}

```diff
@@ -1,20 +1,13 @@
-Metadata-Version: 2.1 Name: AL-Khatma-lib Version: 2.0.0 Summary: A library
-Specialized About Islamic Author-email: Osamah Awadh
-gmail.com> Project-URL: Homepage, https://github.com/oaokm/AL-Khatma Project-
-URL: Bug Tracker, https://github.com/oaokm/AL-Khatma/issues Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE
                     [AL-Khatma Logo For Arabic and English]
                             Arabic    |    English
 ÙÙØ±Ø©_Ø§ÙØ®ØªÙØ©    |    ØªØ­ÙÙÙ_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙØªØ¹Ø§ÙÙ
    ÙØ¹_Ø§ÙÙÙØªØ¨Ø©    |    Ø§ÙÙØµØ§Ø¯Ø±    |    Ø§ÙØªØ±Ø®ÙØµ    |   
- Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª    |    ØµÙØ­Ø©_Ø­Ù_Ø§ÙÙØ´ÙÙØ§Øª    |    Ø¥ÙØ´Ø§Ø¡
-                                  ÙØ´ÙÙØ©
+       Ø§ÙØªØ­Ø¯ÙØ«Ø§Øª    |    ØµÙØ­Ø©_Ø­Ù_Ø§ÙÙØ´ÙÙØ§Øª    |   
+                        Ø§ÙØªØ¨ÙÙØº_Ø¹Ù_ÙØ´ÙÙØ©
  ![GitHub](https://img.shields.io/github/license/oaokm/AL-Khatma) | ![](https:/
 /img.shields.io/badge/Programing%20Language-Python_3_and_top-orange) | ![PyPI]
 (https://img.shields.io/pypi/v/AL-Khatma-lib) | ![GitHub repo size](https://
 img.shields.io/github/repo-size/oaokm/AL-Khatma) --| --| -- | --| ##
 **Ø¨ÙØ§Ù** ÙÙ ÙÙÙ Ø§ÙØ«Ø§ÙØ« ÙÙ Ø£Ø¨Ø±ÙÙ ÙÙ Ø¹Ø§Ù 2023
 Ø§ÙÙÙØ§ÙÙ Ø§ÙØ«Ø§ÙÙ Ø¹Ø´Ø± ÙÙ Ø±ÙØ¶Ø§Ù ÙØ¹Ø§Ù 1444 ÙÙ ÙÙ
 ÙØ°Ø§ Ø§ÙÙÙÙ Ø¨Ø¯Ø£Øª Ø§ÙÙÙØ±Ø© ÙØ¨Ø¹Ø¯ÙØ§ ÙÙØª Ø¨ØªØ·Ø¨ÙÙ
```

