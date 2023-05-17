# Comparing `tmp/gptsubtitler-0.0.3.tar.gz` & `tmp/gptsubtitler-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptsubtitler-0.0.3.tar", last modified: Wed May 17 08:31:32 2023, max compression
+gzip compressed data, was "gptsubtitler-0.0.4.tar", last modified: Wed May 17 08:32:31 2023, max compression
```

## Comparing `gptsubtitler-0.0.3.tar` & `gptsubtitler-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 08:31:32.487065 gptsubtitler-0.0.3/
--rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2737 2023-05-17 08:31:32.486065 gptsubtitler-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2310 2023-05-17 08:27:03.000000 gptsubtitler-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 08:31:32.478061 gptsubtitler-0.0.3/gptsubtitler/
--rw-rw-rw-   0        0        0      126 2023-05-17 08:29:20.000000 gptsubtitler-0.0.3/gptsubtitler/__init__.py
--rw-rw-rw-   0        0        0     5496 2023-05-17 07:50:23.000000 gptsubtitler-0.0.3/gptsubtitler/transcriber.py
--rw-rw-rw-   0        0        0     4030 2023-05-17 07:39:13.000000 gptsubtitler-0.0.3/gptsubtitler/translator.py
--rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.3/gptsubtitler/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:31:32.485063 gptsubtitler-0.0.3/gptsubtitler.egg-info/
--rw-rw-rw-   0        0        0     2737 2023-05-17 08:31:32.000000 gptsubtitler-0.0.3/gptsubtitler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-17 08:31:32.000000 gptsubtitler-0.0.3/gptsubtitler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 08:31:32.000000 gptsubtitler-0.0.3/gptsubtitler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-17 08:31:32.000000 gptsubtitler-0.0.3/gptsubtitler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 08:31:32.000000 gptsubtitler-0.0.3/gptsubtitler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 08:31:32.487065 gptsubtitler-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      682 2023-05-17 08:31:30.000000 gptsubtitler-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:32:31.425799 gptsubtitler-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2729 2023-05-17 08:32:31.424797 gptsubtitler-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2302 2023-05-17 08:32:17.000000 gptsubtitler-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 08:32:31.409794 gptsubtitler-0.0.4/gptsubtitler/
+-rw-rw-rw-   0        0        0      126 2023-05-17 08:29:20.000000 gptsubtitler-0.0.4/gptsubtitler/__init__.py
+-rw-rw-rw-   0        0        0     5496 2023-05-17 07:50:23.000000 gptsubtitler-0.0.4/gptsubtitler/transcriber.py
+-rw-rw-rw-   0        0        0     4030 2023-05-17 07:39:13.000000 gptsubtitler-0.0.4/gptsubtitler/translator.py
+-rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.4/gptsubtitler/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:32:31.423797 gptsubtitler-0.0.4/gptsubtitler.egg-info/
+-rw-rw-rw-   0        0        0     2729 2023-05-17 08:32:31.000000 gptsubtitler-0.0.4/gptsubtitler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-17 08:32:31.000000 gptsubtitler-0.0.4/gptsubtitler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 08:32:31.000000 gptsubtitler-0.0.4/gptsubtitler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-17 08:32:31.000000 gptsubtitler-0.0.4/gptsubtitler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 08:32:31.000000 gptsubtitler-0.0.4/gptsubtitler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 08:32:31.425799 gptsubtitler-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      682 2023-05-17 08:32:29.000000 gptsubtitler-0.0.4/setup.py
```

### Comparing `gptsubtitler-0.0.3/LICENSE` & `gptsubtitler-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.3/PKG-INFO` & `gptsubtitler-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptsubtitler
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automatically subtitle any video spoken in any language to a language of your choice.
 Author: extremq
 Author-email: extremqcontact@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -50,32 +50,32 @@
 ```
 
 # Quick guide
 Example usage for adding subtitles and translating them in Romanian:
 
 You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
 ```py
-from src.transcriber import Transcriber
+from gptsubtitler import Transcriber
 
 # I strongly recommend using the "medium" model_type.
 Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda")
 ```
 
 You can also use the `Translator` class from `translator.py` if you just want to translate some text.
 
 Example usage for translating from English to Romanian:
 ```py
-from src.translator import Translator
+from gptsubtitler import Translator
 
 print(Translator.translate("Hi!", target_language="ro", source_language="en", device="cuda"))
 ```
 
 If you have generated a `.srt` file and just want to add subtitles:
 ```py
-from src.video_utils import create_video_with_subtitles
+from gptsubtitler import create_video_with_subtitles
 create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
 ```
 
 # Options
 Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
 - cpu - default
 - cuda
```

### Comparing `gptsubtitler-0.0.3/README.md` & `gptsubtitler-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -38,32 +38,32 @@
 ```
 
 # Quick guide
 Example usage for adding subtitles and translating them in Romanian:
 
 You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
 ```py
-from src.transcriber import Transcriber
+from gptsubtitler import Transcriber
 
 # I strongly recommend using the "medium" model_type.
 Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda")
 ```
 
 You can also use the `Translator` class from `translator.py` if you just want to translate some text.
 
 Example usage for translating from English to Romanian:
 ```py
-from src.translator import Translator
+from gptsubtitler import Translator
 
 print(Translator.translate("Hi!", target_language="ro", source_language="en", device="cuda"))
 ```
 
 If you have generated a `.srt` file and just want to add subtitles:
 ```py
-from src.video_utils import create_video_with_subtitles
+from gptsubtitler import create_video_with_subtitles
 create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
 ```
 
 # Options
 Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
 - cpu - default
 - cuda
```

### Comparing `gptsubtitler-0.0.3/gptsubtitler/transcriber.py` & `gptsubtitler-0.0.4/gptsubtitler/transcriber.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.3/gptsubtitler/translator.py` & `gptsubtitler-0.0.4/gptsubtitler/translator.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.3/gptsubtitler/video_utils.py` & `gptsubtitler-0.0.4/gptsubtitler/video_utils.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.3/gptsubtitler.egg-info/PKG-INFO` & `gptsubtitler-0.0.4/gptsubtitler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptsubtitler
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automatically subtitle any video spoken in any language to a language of your choice.
 Author: extremq
 Author-email: extremqcontact@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -50,32 +50,32 @@
 ```
 
 # Quick guide
 Example usage for adding subtitles and translating them in Romanian:
 
 You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
 ```py
-from src.transcriber import Transcriber
+from gptsubtitler import Transcriber
 
 # I strongly recommend using the "medium" model_type.
 Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda")
 ```
 
 You can also use the `Translator` class from `translator.py` if you just want to translate some text.
 
 Example usage for translating from English to Romanian:
 ```py
-from src.translator import Translator
+from gptsubtitler import Translator
 
 print(Translator.translate("Hi!", target_language="ro", source_language="en", device="cuda"))
 ```
 
 If you have generated a `.srt` file and just want to add subtitles:
 ```py
-from src.video_utils import create_video_with_subtitles
+from gptsubtitler import create_video_with_subtitles
 create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
 ```
 
 # Options
 Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
 - cpu - default
 - cuda
```

### Comparing `gptsubtitler-0.0.3/setup.py` & `gptsubtitler-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name="gptsubtitler",
-    version="0.0.3",
+    version="0.0.4",
     author="extremq",
     author_email="extremqcontact@gmail.com",
     description="Automatically subtitle any video spoken in any language to a language of your choice.",
     install_requires=[
         "transformers",
         "openai-whisper",
     ],
```

