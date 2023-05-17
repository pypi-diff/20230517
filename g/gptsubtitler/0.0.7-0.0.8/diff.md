# Comparing `tmp/gptsubtitler-0.0.7.tar.gz` & `tmp/gptsubtitler-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptsubtitler-0.0.7.tar", last modified: Wed May 17 15:17:57 2023, max compression
+gzip compressed data, was "gptsubtitler-0.0.8.tar", last modified: Wed May 17 16:20:11 2023, max compression
```

## Comparing `gptsubtitler-0.0.7.tar` & `gptsubtitler-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:17:57.314675 gptsubtitler-0.0.7/
--rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2887 2023-05-17 15:17:57.313675 gptsubtitler-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2460 2023-05-17 14:41:56.000000 gptsubtitler-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 15:17:57.295512 gptsubtitler-0.0.7/gptsubtitler/
--rw-rw-rw-   0        0        0      126 2023-05-17 08:29:20.000000 gptsubtitler-0.0.7/gptsubtitler/__init__.py
--rw-rw-rw-   0        0        0     5550 2023-05-17 15:17:42.000000 gptsubtitler-0.0.7/gptsubtitler/transcriber.py
--rw-rw-rw-   0        0        0     3914 2023-05-17 14:49:59.000000 gptsubtitler-0.0.7/gptsubtitler/translator.py
--rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.7/gptsubtitler/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:17:57.312674 gptsubtitler-0.0.7/gptsubtitler.egg-info/
--rw-rw-rw-   0        0        0     2887 2023-05-17 15:17:57.000000 gptsubtitler-0.0.7/gptsubtitler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-17 15:17:57.000000 gptsubtitler-0.0.7/gptsubtitler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 15:17:57.000000 gptsubtitler-0.0.7/gptsubtitler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-17 15:17:57.000000 gptsubtitler-0.0.7/gptsubtitler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 15:17:57.000000 gptsubtitler-0.0.7/gptsubtitler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 15:17:57.314675 gptsubtitler-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-05-17 15:17:55.000000 gptsubtitler-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:20:11.169638 gptsubtitler-0.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2887 2023-05-17 16:20:11.168638 gptsubtitler-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2460 2023-05-17 14:41:56.000000 gptsubtitler-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 16:20:11.147633 gptsubtitler-0.0.8/gptsubtitler/
+-rw-rw-rw-   0        0        0      126 2023-05-17 08:29:20.000000 gptsubtitler-0.0.8/gptsubtitler/__init__.py
+-rw-rw-rw-   0        0        0     5550 2023-05-17 15:17:42.000000 gptsubtitler-0.0.8/gptsubtitler/transcriber.py
+-rw-rw-rw-   0        0        0     3914 2023-05-17 14:49:59.000000 gptsubtitler-0.0.8/gptsubtitler/translator.py
+-rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.8/gptsubtitler/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:20:11.167637 gptsubtitler-0.0.8/gptsubtitler.egg-info/
+-rw-rw-rw-   0        0        0     2887 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 16:20:11.000000 gptsubtitler-0.0.8/gptsubtitler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:20:11.169638 gptsubtitler-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-05-17 16:19:53.000000 gptsubtitler-0.0.8/setup.py
```

### Comparing `gptsubtitler-0.0.7/LICENSE` & `gptsubtitler-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.7/PKG-INFO` & `gptsubtitler-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptsubtitler
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automatically subtitle any video spoken in any language to a language of your choice.
 Author: extremq
 Author-email: extremqcontact@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `gptsubtitler-0.0.7/README.md` & `gptsubtitler-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.7/gptsubtitler/transcriber.py` & `gptsubtitler-0.0.8/gptsubtitler/transcriber.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.7/gptsubtitler/translator.py` & `gptsubtitler-0.0.8/gptsubtitler/translator.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.7/gptsubtitler/video_utils.py` & `gptsubtitler-0.0.8/gptsubtitler/video_utils.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.7/gptsubtitler.egg-info/PKG-INFO` & `gptsubtitler-0.0.8/gptsubtitler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptsubtitler
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automatically subtitle any video spoken in any language to a language of your choice.
 Author: extremq
 Author-email: extremqcontact@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `gptsubtitler-0.0.7/setup.py` & `gptsubtitler-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name="gptsubtitler",
-    version="0.0.7",
+    version="0.0.8",
     author="extremq",
     author_email="extremqcontact@gmail.com",
     description="Automatically subtitle any video spoken in any language to a language of your choice.",
     install_requires=[
         "transformers",
         "openai-whisper",
+        "sentencepiece"
     ],
     packages=["gptsubtitler"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

