# Comparing `tmp/fajrGPT-1.1.1.tar.gz` & `tmp/fajrGPT-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.1.1.tar", last modified: Wed May 17 17:20:44 2023, max compression
+gzip compressed data, was "fajrGPT-1.1.2.tar", last modified: Wed May 17 18:53:09 2023, max compression
```

## Comparing `fajrGPT-1.1.1.tar` & `fajrGPT-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 17:20:44.370031 fajrGPT-1.1.1/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.1/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 17:20:44.369882 fajrGPT-1.1.1/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2326 2023-05-17 15:03:13.000000 fajrGPT-1.1.1/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 17:20:44.368502 fajrGPT-1.1.1/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-1.1.1/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.1/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     7934 2023-05-17 17:20:11.000000 fajrGPT-1.1.1/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 17:20:44.369585 fajrGPT-1.1.1/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 17:20:44.000000 fajrGPT-1.1.1/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 17:20:44.000000 fajrGPT-1.1.1/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 17:20:44.000000 fajrGPT-1.1.1/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 17:20:44.000000 fajrGPT-1.1.1/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 17:20:44.000000 fajrGPT-1.1.1/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 17:20:44.000000 fajrGPT-1.1.1/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 17:20:44.370076 fajrGPT-1.1.1/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 17:20:42.000000 fajrGPT-1.1.1/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 18:53:09.931729 fajrGPT-1.1.2/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.2/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2920 2023-05-17 18:53:09.931578 fajrGPT-1.1.2/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2257 2023-05-17 18:52:37.000000 fajrGPT-1.1.2/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 18:53:09.930273 fajrGPT-1.1.2/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-1.1.2/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.2/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     7934 2023-05-17 17:20:11.000000 fajrGPT-1.1.2/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 18:53:09.931392 fajrGPT-1.1.2/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2920 2023-05-17 18:53:09.000000 fajrGPT-1.1.2/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 18:53:09.000000 fajrGPT-1.1.2/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 18:53:09.000000 fajrGPT-1.1.2/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 18:53:09.000000 fajrGPT-1.1.2/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-05-17 18:53:09.000000 fajrGPT-1.1.2/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 18:53:09.000000 fajrGPT-1.1.2/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 18:53:09.931765 fajrGPT-1.1.2/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-05-17 18:52:03.000000 fajrGPT-1.1.2/setup.py
```

### Comparing `fajrGPT-1.1.1/LICENSE` & `fajrGPT-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.1/PKG-INFO` & `fajrGPT-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -31,18 +31,17 @@
 
 1. Clone repo and install packages:
     ```bash
     git clone https://github.com/malekinho8/quran-wake-up.git
     pip install -r requirements.txt
     pip install .
     ```
-2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
+2. Alternatively, install one dependency manually and `fajrGPT` through PyPI:
     ```python
-    pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
-    pip install fajrGPT
+    pip install git+https://github.com/ytdl-org/youtube-dl.git fajrGPT
     ```
 3. Run the main.py script, passing the required parameters:
     ```bash
     fajrGPT --url <YouTube URL> --hours <Hours for Countdown> --output <Output filename>
     ```
     Replace `<YouTube URL>`, `<Hours for Countdown>`, and `<Output filename>` with appropriate values.
```

### Comparing `fajrGPT-1.1.1/README.md` & `fajrGPT-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 
 1. Clone repo and install packages:
     ```bash
     git clone https://github.com/malekinho8/quran-wake-up.git
     pip install -r requirements.txt
     pip install .
     ```
-2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
+2. Alternatively, install one dependency manually and `fajrGPT` through PyPI:
     ```python
-    pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
-    pip install fajrGPT
+    pip install git+https://github.com/ytdl-org/youtube-dl.git fajrGPT
     ```
 3. Run the main.py script, passing the required parameters:
     ```bash
     fajrGPT --url <YouTube URL> --hours <Hours for Countdown> --output <Output filename>
     ```
     Replace `<YouTube URL>`, `<Hours for Countdown>`, and `<Output filename>` with appropriate values.
```

### Comparing `fajrGPT-1.1.1/fajrGPT/quran_metadata.py` & `fajrGPT-1.1.2/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.1/fajrGPT/wake.py` & `fajrGPT-1.1.2/fajrGPT/wake.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.1/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.1.2/fajrGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -31,18 +31,17 @@
 
 1. Clone repo and install packages:
     ```bash
     git clone https://github.com/malekinho8/quran-wake-up.git
     pip install -r requirements.txt
     pip install .
     ```
-2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
+2. Alternatively, install one dependency manually and `fajrGPT` through PyPI:
     ```python
-    pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
-    pip install fajrGPT
+    pip install git+https://github.com/ytdl-org/youtube-dl.git fajrGPT
     ```
 3. Run the main.py script, passing the required parameters:
     ```bash
     fajrGPT --url <YouTube URL> --hours <Hours for Countdown> --output <Output filename>
     ```
     Replace `<YouTube URL>`, `<Hours for Countdown>`, and `<Output filename>` with appropriate values.
```

### Comparing `fajrGPT-1.1.1/setup.py` & `fajrGPT-1.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.1.1",
+    version="1.1.2",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
@@ -22,14 +22,15 @@
     install_requires=[
         "click",
         "pygame",
         "pydub",
         "moviepy",
         "openai",
         "tqdm",
+        "TheQuranModule"
     ],
     entry_points={
         'console_scripts': [
             'fajrGPT=fajrGPT.wake:main',
         ],
     },
 )
```

