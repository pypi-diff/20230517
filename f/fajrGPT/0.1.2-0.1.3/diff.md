# Comparing `tmp/fajrGPT-0.1.2.tar.gz` & `tmp/fajrGPT-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-0.1.2.tar", last modified: Wed May 17 15:01:50 2023, max compression
+gzip compressed data, was "fajrGPT-0.1.3.tar", last modified: Wed May 17 15:04:29 2023, max compression
```

## Comparing `fajrGPT-0.1.2.tar` & `fajrGPT-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:01:50.557989 fajrGPT-0.1.2/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-0.1.2/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2927 2023-05-17 15:01:50.557855 fajrGPT-0.1.2/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2264 2023-05-17 14:58:42.000000 fajrGPT-0.1.2/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:01:50.556613 fajrGPT-0.1.2/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-0.1.2/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-0.1.2/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     7497 2023-05-17 14:57:53.000000 fajrGPT-0.1.2/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:01:50.557650 fajrGPT-0.1.2/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2927 2023-05-17 15:01:50.000000 fajrGPT-0.1.2/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 15:01:50.000000 fajrGPT-0.1.2/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 15:01:50.000000 fajrGPT-0.1.2/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 15:01:50.000000 fajrGPT-0.1.2/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 15:01:50.000000 fajrGPT-0.1.2/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 15:01:50.000000 fajrGPT-0.1.2/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 15:01:50.558063 fajrGPT-0.1.2/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 15:01:46.000000 fajrGPT-0.1.2/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:04:29.347007 fajrGPT-0.1.3/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-0.1.3/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 15:04:29.346863 fajrGPT-0.1.3/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2326 2023-05-17 15:03:13.000000 fajrGPT-0.1.3/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:04:29.345550 fajrGPT-0.1.3/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-0.1.3/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-0.1.3/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     7497 2023-05-17 14:57:53.000000 fajrGPT-0.1.3/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:04:29.346607 fajrGPT-0.1.3/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 15:04:29.347046 fajrGPT-0.1.3/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 15:03:38.000000 fajrGPT-0.1.3/setup.py
```

### Comparing `fajrGPT-0.1.2/LICENSE` & `fajrGPT-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.2/PKG-INFO` & `fajrGPT-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -27,14 +27,15 @@
 - After each explanation, the program waits for the user to press Enter before proceeding.
 - Once all explanations are provided, the audio volume gradually decreases over a 5-second period.
 
 ## Usage
 
 1. Clone repo and install packages:
     ```bash
+    git clone https://github.com/malekinho8/quran-wake-up.git
     pip install -r requirements.txt
     pip install .
     ```
 2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
     ```python
     pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
     pip install fajrGPT
```

### Comparing `fajrGPT-0.1.2/README.md` & `fajrGPT-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 - After each explanation, the program waits for the user to press Enter before proceeding.
 - Once all explanations are provided, the audio volume gradually decreases over a 5-second period.
 
 ## Usage
 
 1. Clone repo and install packages:
     ```bash
+    git clone https://github.com/malekinho8/quran-wake-up.git
     pip install -r requirements.txt
     pip install .
     ```
 2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
     ```python
     pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
     pip install fajrGPT
```

### Comparing `fajrGPT-0.1.2/fajrGPT/quran_metadata.py` & `fajrGPT-0.1.3/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.2/fajrGPT/wake.py` & `fajrGPT-0.1.3/fajrGPT/wake.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.2/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-0.1.3/fajrGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -27,14 +27,15 @@
 - After each explanation, the program waits for the user to press Enter before proceeding.
 - Once all explanations are provided, the audio volume gradually decreases over a 5-second period.
 
 ## Usage
 
 1. Clone repo and install packages:
     ```bash
+    git clone https://github.com/malekinho8/quran-wake-up.git
     pip install -r requirements.txt
     pip install .
     ```
 2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
     ```python
     pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
     pip install fajrGPT
```

### Comparing `fajrGPT-0.1.2/setup.py` & `fajrGPT-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="0.1.2",
+    version="0.1.3",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

