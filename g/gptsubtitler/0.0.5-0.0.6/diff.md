# Comparing `tmp/gptsubtitler-0.0.5.tar.gz` & `tmp/gptsubtitler-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptsubtitler-0.0.5.tar", last modified: Wed May 17 09:21:36 2023, max compression
+gzip compressed data, was "gptsubtitler-0.0.6.tar", last modified: Wed May 17 14:51:50 2023, max compression
```

## Comparing `gptsubtitler-0.0.5.tar` & `gptsubtitler-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hustler   (1000) hustler   (1000)        0 2023-05-17 09:21:36.234932 gptsubtitler-0.0.5/
--rw-rw-r--   0 hustler   (1000) hustler   (1000)     1064 2023-05-17 09:15:29.000000 gptsubtitler-0.0.5/LICENSE
--rw-rw-r--   0 hustler   (1000) hustler   (1000)     2693 2023-05-17 09:21:36.234932 gptsubtitler-0.0.5/PKG-INFO
--rw-rw-r--   0 hustler   (1000) hustler   (1000)     2222 2023-05-17 09:15:29.000000 gptsubtitler-0.0.5/README.md
-drwxrwxr-x   0 hustler   (1000) hustler   (1000)        0 2023-05-17 09:21:36.234932 gptsubtitler-0.0.5/gptsubtitler/
--rw-rw-r--   0 hustler   (1000) hustler   (1000)      124 2023-05-17 09:15:29.000000 gptsubtitler-0.0.5/gptsubtitler/__init__.py
--rw-rw-r--   0 hustler   (1000) hustler   (1000)     5330 2023-05-17 09:15:29.000000 gptsubtitler-0.0.5/gptsubtitler/transcriber.py
--rw-rw-r--   0 hustler   (1000) hustler   (1000)     3910 2023-05-17 09:15:29.000000 gptsubtitler-0.0.5/gptsubtitler/translator.py
--rw-rw-r--   0 hustler   (1000) hustler   (1000)     1316 2023-05-17 09:15:29.000000 gptsubtitler-0.0.5/gptsubtitler/video_utils.py
-drwxrwxr-x   0 hustler   (1000) hustler   (1000)        0 2023-05-17 09:21:36.234932 gptsubtitler-0.0.5/gptsubtitler.egg-info/
--rw-rw-r--   0 hustler   (1000) hustler   (1000)     2693 2023-05-17 09:21:36.000000 gptsubtitler-0.0.5/gptsubtitler.egg-info/PKG-INFO
--rw-rw-r--   0 hustler   (1000) hustler   (1000)      313 2023-05-17 09:21:36.000000 gptsubtitler-0.0.5/gptsubtitler.egg-info/SOURCES.txt
--rw-rw-r--   0 hustler   (1000) hustler   (1000)        1 2023-05-17 09:21:36.000000 gptsubtitler-0.0.5/gptsubtitler.egg-info/dependency_links.txt
--rw-rw-r--   0 hustler   (1000) hustler   (1000)       28 2023-05-17 09:21:36.000000 gptsubtitler-0.0.5/gptsubtitler.egg-info/requires.txt
--rw-rw-r--   0 hustler   (1000) hustler   (1000)       13 2023-05-17 09:21:36.000000 gptsubtitler-0.0.5/gptsubtitler.egg-info/top_level.txt
--rw-rw-r--   0 hustler   (1000) hustler   (1000)       38 2023-05-17 09:21:36.234932 gptsubtitler-0.0.5/setup.cfg
--rw-rw-r--   0 hustler   (1000) hustler   (1000)      690 2023-05-17 09:20:10.000000 gptsubtitler-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:51:50.179642 gptsubtitler-0.0.6/
+-rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2887 2023-05-17 14:51:50.178641 gptsubtitler-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2460 2023-05-17 14:41:56.000000 gptsubtitler-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:51:50.164240 gptsubtitler-0.0.6/gptsubtitler/
+-rw-rw-rw-   0        0        0      126 2023-05-17 08:29:20.000000 gptsubtitler-0.0.6/gptsubtitler/__init__.py
+-rw-rw-rw-   0        0        0     5523 2023-05-17 14:51:03.000000 gptsubtitler-0.0.6/gptsubtitler/transcriber.py
+-rw-rw-rw-   0        0        0     3914 2023-05-17 14:49:59.000000 gptsubtitler-0.0.6/gptsubtitler/translator.py
+-rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.6/gptsubtitler/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:51:50.177641 gptsubtitler-0.0.6/gptsubtitler.egg-info/
+-rw-rw-rw-   0        0        0     2887 2023-05-17 14:51:50.000000 gptsubtitler-0.0.6/gptsubtitler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-17 14:51:50.000000 gptsubtitler-0.0.6/gptsubtitler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:51:50.000000 gptsubtitler-0.0.6/gptsubtitler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-17 14:51:50.000000 gptsubtitler-0.0.6/gptsubtitler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 14:51:50.000000 gptsubtitler-0.0.6/gptsubtitler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:51:50.179642 gptsubtitler-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-05-17 14:51:48.000000 gptsubtitler-0.0.6/setup.py
```

### Comparing `gptsubtitler-0.0.5/PKG-INFO` & `gptsubtitler-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,95 @@
-Metadata-Version: 2.1
-Name: gptsubtitler
-Version: 0.0.5
-Summary: Automatically subtitle any video spoken in any language to a language of your choice.
-Home-page: UNKNOWN
-Author: extremq
-Author-email: extremqcontact@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Subtitler
-Automatically subtitle any video spoken in any language to a language of your choice.
-
-Models used:
-- [OpenAI whisper](https://openai.com/research/whisper) - for text-to-audio
-- [Facebook M2M10](https://huggingface.co/facebook/m2m100_418M) - for translation
-
-Tools used:
-- `ffmpeg`
-
-**Please don't forget to star the repository if you find it useful or educational!**
-
-Before:
-
-https://github.com/extremq/subtitler/assets/45830561/49f6ecce-cfdc-4f1c-97eb-07a36ac841c9
-
-After (in Romanian - `model_type=medium, language_model_type=base`):
-
-https://github.com/extremq/subtitler/assets/45830561/20bc5169-0ce3-47cd-adb7-15d75daf27f4
-
-# Setup
-Install using `pip`.
-
-```
-pip install gptsubtitler
-```
-
-Install [`ffmpeg`](https://ffmpeg.org/):
-```bash
-# Ubuntu or Debian
-sudo apt update && sudo apt install ffmpeg
-
-# MacOS
-brew install ffmpeg
-
-# Windows using Chocolatey https://chocolatey.org/
-choco install ffmpeg
-```
-
-# Quick guide
-Example usage for adding subtitles and translating them in Romanian:
-
-You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
-```py
-from gptsubtitler import Transcriber
-
-# I strongly recommend using the "medium" model_type.
-Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda")
-```
-
-You can also use the `Translator` class from `translator.py` if you just want to translate some text.
-
-Example usage for translating from English to Romanian:
-```py
-from gptsubtitler import Translator
-
-print(Translator.translate("Hi!", target_language="ro", source_language="en", device="cuda"))
-```
-
-If you have generated a `.srt` file and just want to add subtitles:
-```py
-from gptsubtitler import create_video_with_subtitles
-create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
-```
-
-# Options
-Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
-- cpu - default
-- cuda
-
-Available options for `model_type` (the audio to text model):
-- tiny
-- base - default
-- small
-- medium
-- large
-
-Available options for `language_model_type` (the language translator model):
-- base - default
-- large
-
-
+Metadata-Version: 2.1
+Name: gptsubtitler
+Version: 0.0.6
+Summary: Automatically subtitle any video spoken in any language to a language of your choice.
+Author: extremq
+Author-email: extremqcontact@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Subtitler
+Automatically subtitle any video spoken in any language to a language of your choice using AI.
+
+Models used:
+- [OpenAI whisper](https://openai.com/research/whisper) - for audio-to-text
+- [Facebook M2M10](https://huggingface.co/facebook/m2m100_418M) - for translation
+
+Tools used:
+- `ffmpeg`
+
+**Please don't forget to star the repository if you find it useful or educational!**
+
+Before:
+
+https://github.com/extremq/subtitler/assets/45830561/49f6ecce-cfdc-4f1c-97eb-07a36ac841c9
+
+After (in Romanian - `model_type=medium, language_model_type=base`):
+
+https://github.com/extremq/subtitler/assets/45830561/20bc5169-0ce3-47cd-adb7-15d75daf27f4
+
+# Setup
+Install using `pip`.
+
+```
+pip install gptsubtitler
+```
+
+Install [`ffmpeg`](https://ffmpeg.org/):
+```bash
+# Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
+
+# MacOS
+brew install ffmpeg
+
+# Windows using Chocolatey https://chocolatey.org/
+choco install ffmpeg
+```
+
+# Quick guide
+Example usage for adding subtitles and translating them in Romanian:
+
+You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
+```py
+from gptsubtitler import Transcriber
+
+# I strongly recommend using the "medium" model_type.
+Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base")
+
+# If you want to use the gpu, add device="cuda"
+# Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda") 
+```
+
+You can also use the `Translator` class from `translator.py` if you just want to translate some text.
+
+Example usage for translating from English to Romanian:
+```py
+from gptsubtitler import Translator
+
+print(Translator.translate("Hi!", target_language="ro", source_language="en"))
+```
+
+If you have generated a `.srt` file and just want to add subtitles:
+```py
+from gptsubtitler import create_video_with_subtitles
+create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
+```
+
+# Options
+Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
+- cpu - default
+- cuda
+
+Available options for `model_type` (the audio to text model):
+- tiny
+- base - default
+- small
+- medium
+- large
+
+Available options for `language_model_type` (the language translator model):
+- base - default
+- large
```

### Comparing `gptsubtitler-0.0.5/README.md` & `gptsubtitler-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,83 @@
-# Subtitler
-Automatically subtitle any video spoken in any language to a language of your choice.
-
-Models used:
-- [OpenAI whisper](https://openai.com/research/whisper) - for text-to-audio
-- [Facebook M2M10](https://huggingface.co/facebook/m2m100_418M) - for translation
-
-Tools used:
-- `ffmpeg`
-
-**Please don't forget to star the repository if you find it useful or educational!**
-
-Before:
-
-https://github.com/extremq/subtitler/assets/45830561/49f6ecce-cfdc-4f1c-97eb-07a36ac841c9
-
-After (in Romanian - `model_type=medium, language_model_type=base`):
-
-https://github.com/extremq/subtitler/assets/45830561/20bc5169-0ce3-47cd-adb7-15d75daf27f4
-
-# Setup
-Install using `pip`.
-
-```
-pip install gptsubtitler
-```
-
-Install [`ffmpeg`](https://ffmpeg.org/):
-```bash
-# Ubuntu or Debian
-sudo apt update && sudo apt install ffmpeg
-
-# MacOS
-brew install ffmpeg
-
-# Windows using Chocolatey https://chocolatey.org/
-choco install ffmpeg
-```
-
-# Quick guide
-Example usage for adding subtitles and translating them in Romanian:
-
-You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
-```py
-from gptsubtitler import Transcriber
-
-# I strongly recommend using the "medium" model_type.
-Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda")
-```
-
-You can also use the `Translator` class from `translator.py` if you just want to translate some text.
-
-Example usage for translating from English to Romanian:
-```py
-from gptsubtitler import Translator
-
-print(Translator.translate("Hi!", target_language="ro", source_language="en", device="cuda"))
-```
-
-If you have generated a `.srt` file and just want to add subtitles:
-```py
-from gptsubtitler import create_video_with_subtitles
-create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
-```
-
-# Options
-Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
-- cpu - default
-- cuda
-
-Available options for `model_type` (the audio to text model):
-- tiny
-- base - default
-- small
-- medium
-- large
-
-Available options for `language_model_type` (the language translator model):
-- base - default
-- large
+# Subtitler
+Automatically subtitle any video spoken in any language to a language of your choice using AI.
+
+Models used:
+- [OpenAI whisper](https://openai.com/research/whisper) - for audio-to-text
+- [Facebook M2M10](https://huggingface.co/facebook/m2m100_418M) - for translation
+
+Tools used:
+- `ffmpeg`
+
+**Please don't forget to star the repository if you find it useful or educational!**
+
+Before:
+
+https://github.com/extremq/subtitler/assets/45830561/49f6ecce-cfdc-4f1c-97eb-07a36ac841c9
+
+After (in Romanian - `model_type=medium, language_model_type=base`):
+
+https://github.com/extremq/subtitler/assets/45830561/20bc5169-0ce3-47cd-adb7-15d75daf27f4
+
+# Setup
+Install using `pip`.
+
+```
+pip install gptsubtitler
+```
+
+Install [`ffmpeg`](https://ffmpeg.org/):
+```bash
+# Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
+
+# MacOS
+brew install ffmpeg
+
+# Windows using Chocolatey https://chocolatey.org/
+choco install ffmpeg
+```
+
+# Quick guide
+Example usage for adding subtitles and translating them in Romanian:
+
+You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
+```py
+from gptsubtitler import Transcriber
+
+# I strongly recommend using the "medium" model_type.
+Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base")
+
+# If you want to use the gpu, add device="cuda"
+# Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda") 
+```
+
+You can also use the `Translator` class from `translator.py` if you just want to translate some text.
+
+Example usage for translating from English to Romanian:
+```py
+from gptsubtitler import Translator
+
+print(Translator.translate("Hi!", target_language="ro", source_language="en"))
+```
+
+If you have generated a `.srt` file and just want to add subtitles:
+```py
+from gptsubtitler import create_video_with_subtitles
+create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
+```
+
+# Options
+Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
+- cpu - default
+- cuda
+
+Available options for `model_type` (the audio to text model):
+- tiny
+- base - default
+- small
+- medium
+- large
+
+Available options for `language_model_type` (the language translator model):
+- base - default
+- large
```

### Comparing `gptsubtitler-0.0.5/gptsubtitler/translator.py` & `gptsubtitler-0.0.6/gptsubtitler/translator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,118 @@
-from transformers import M2M100ForConditionalGeneration, M2M100Tokenizer
-import torch
-
-
-class Translator(object):
-    model = None
-    tokenizer = None
-    model_type = None
-    AVAILABLE_MODELS = ["base", "large"]
-
-    @staticmethod
-    def create_model_and_tokenizer():
-        if Translator.model is None:
-            try:
-                if Translator.model_type == "base":
-                    Translator.model = M2M100ForConditionalGeneration.from_pretrained(
-                        "facebook/m2m100_418M"
-                    )
-                elif Translator.model_type == "large":
-                    Translator.model = M2M100ForConditionalGeneration.from_pretrained(
-                        "facebook/m2m100_1.2B"
-                    )
-            except Exception as e:
-                print("Couldn't load model.")
-                print(e)
-
-        if Translator.tokenizer is None:
-            try:
-                if Translator.model_type == "base":
-                    Translator.tokenizer = M2M100Tokenizer.from_pretrained(
-                        "facebook/m2m100_418M"
-                    )
-                elif Translator.model_type == "large":
-                    Translator.tokenizer = M2M100Tokenizer.from_pretrained(
-                        "facebook/m2m100_1.2B"
-                    )
-            except Exception as e:
-                print("Couldn't load tokenizer.")
-                print(e)
-
-    @staticmethod
-    def translate(
-        text,
-        source_language="en",
-        target_language="ro",
-        model_type="base",
-        device="cpu",
-    ):
-        """Translate text.
-        
-        Args:
-            text (str): Text to translate.
-
-            source_language (str, optional): Source language. Defaults to "en".
-
-            target_language (str, optional): Target language. Defaults to "ro".
-
-            model_type (str, optional): Model type. Defaults to "base".
-
-            device (str, optional): Device to use. Defaults to "cpu".
-        Returns:
-            str: Translated text.
-        """
-        if model_type not in Translator.AVAILABLE_MODELS:
-            print(
-                f"Invalid 'model_type'. Using base model. Available models: {Translator.AVAILABLE_MODELS}"
-            )
-            model_type = "base"
-
-        if device == "cuda":
-            if not torch.cuda.is_available():
-                print("CUDA is not available. Using CPU.")
-                device = "cpu"
-            else:
-                print("CUDA is available. Using GPU.")
-                device = "cuda:0"
-
-        # Set model type
-        Translator.model_type = model_type
-
-        Translator.create_model_and_tokenizer()
-
-        # Set source language for tokenizer
-        Translator.tokenizer.src_lang = source_language
-
-        # Try to encode text
-        try:
-            encoded_text = Translator.tokenizer(text, return_tensors="pt").to(device)
-        except Exception as e:
-            print("Couldn't encode text.")
-            print(e)
-
-        # Try to generate tokens
-        try:
-            # Move to device first
-            Translator.model = Translator.model.to(device)
-            generated_tokens = Translator.model.generate(
-                **encoded_text,
-                forced_bos_token_id=Translator.tokenizer.get_lang_id(target_language),
-            )
-        except Exception as e:
-            print("Couldn't generate tokens. Maybe language is not supported.")
-            print(e)
-
-        target_text = None
-
-        # Try to decode tokens
-        try:
-            target_text = Translator.tokenizer.batch_decode(
-                generated_tokens, skip_special_tokens=True
-            )
-        except Exception as e:
-            print("Couldn't decode tokens.")
-            print(e)
-
-        # Return translated text
-        if target_text is not None:
-            return target_text[0]
-        else:
-            return target_text
+from transformers import M2M100ForConditionalGeneration, M2M100Tokenizer
+import torch
+
+
+class Translator(object):
+    model = None
+    tokenizer = None
+    model_type = None
+    AVAILABLE_MODELS = ["base", "large"]
+
+    @staticmethod
+    def create_model_and_tokenizer():
+        if Translator.model is None:
+            try:
+                if Translator.model_type == "base":
+                    Translator.model = M2M100ForConditionalGeneration.from_pretrained(
+                        "facebook/m2m100_418M"
+                    )
+                elif Translator.model_type == "large":
+                    Translator.model = M2M100ForConditionalGeneration.from_pretrained(
+                        "facebook/m2m100_1.2B"
+                    )
+            except Exception as e:
+                print("Couldn't load model.")
+                print(e)
+
+        if Translator.tokenizer is None:
+            try:
+                if Translator.model_type == "base":
+                    Translator.tokenizer = M2M100Tokenizer.from_pretrained(
+                        "facebook/m2m100_418M"
+                    )
+                elif Translator.model_type == "large":
+                    Translator.tokenizer = M2M100Tokenizer.from_pretrained(
+                        "facebook/m2m100_1.2B"
+                    )
+            except Exception as e:
+                print("Couldn't load tokenizer.")
+                print(e)
+
+    @staticmethod
+    def translate(
+        text,
+        source_language="en",
+        target_language="ro",
+        model_type="base",
+        device="cpu",
+    ):
+        """Translate text.
+        
+        Args:
+            text (str): Text to translate.
+
+            source_language (str, optional): Source language. Defaults to "en".
+
+            target_language (str, optional): Target language. Defaults to "ro".
+
+            model_type (str, optional): Model type. Defaults to "base".
+
+            device (str, optional): Device to use. Defaults to "cpu".
+        Returns:
+            str: Translated text.
+        """
+        if model_type not in Translator.AVAILABLE_MODELS:
+            print(
+                f"Invalid 'model_type'. Using base model. Available models: {Translator.AVAILABLE_MODELS}"
+            )
+            model_type = "base"
+
+        if device == "cuda":
+            if not torch.cuda.is_available():
+                device = "cpu"
+            else:
+                device = "cuda:0"
+
+        # Set model type
+        Translator.model_type = model_type
+
+        Translator.create_model_and_tokenizer()
+
+        # Set source language for tokenizer
+        Translator.tokenizer.src_lang = source_language
+
+        # Try to encode text
+        try:
+            encoded_text = Translator.tokenizer(text, return_tensors="pt").to(device)
+        except Exception as e:
+            print("Couldn't encode text.")
+            print(e)
+
+        # Try to generate tokens
+        try:
+            # Move to device first
+            Translator.model = Translator.model.to(device)
+            generated_tokens = Translator.model.generate(
+                **encoded_text,
+                forced_bos_token_id=Translator.tokenizer.get_lang_id(target_language),
+            )
+        except Exception as e:
+            print("Couldn't generate tokens. Maybe language is not supported.")
+            print(e)
+
+        target_text = None
+
+        # Try to decode tokens
+        try:
+            target_text = Translator.tokenizer.batch_decode(
+                generated_tokens, skip_special_tokens=True
+            )
+        except Exception as e:
+            print("Couldn't decode tokens.")
+            print(e)
+
+        # Return translated text
+        if target_text is not None:
+            return target_text[0]
+        else:
+            return target_text
```

### Comparing `gptsubtitler-0.0.5/gptsubtitler.egg-info/PKG-INFO` & `gptsubtitler-0.0.6/gptsubtitler.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,95 @@
-Metadata-Version: 2.1
-Name: gptsubtitler
-Version: 0.0.5
-Summary: Automatically subtitle any video spoken in any language to a language of your choice.
-Home-page: UNKNOWN
-Author: extremq
-Author-email: extremqcontact@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Subtitler
-Automatically subtitle any video spoken in any language to a language of your choice.
-
-Models used:
-- [OpenAI whisper](https://openai.com/research/whisper) - for text-to-audio
-- [Facebook M2M10](https://huggingface.co/facebook/m2m100_418M) - for translation
-
-Tools used:
-- `ffmpeg`
-
-**Please don't forget to star the repository if you find it useful or educational!**
-
-Before:
-
-https://github.com/extremq/subtitler/assets/45830561/49f6ecce-cfdc-4f1c-97eb-07a36ac841c9
-
-After (in Romanian - `model_type=medium, language_model_type=base`):
-
-https://github.com/extremq/subtitler/assets/45830561/20bc5169-0ce3-47cd-adb7-15d75daf27f4
-
-# Setup
-Install using `pip`.
-
-```
-pip install gptsubtitler
-```
-
-Install [`ffmpeg`](https://ffmpeg.org/):
-```bash
-# Ubuntu or Debian
-sudo apt update && sudo apt install ffmpeg
-
-# MacOS
-brew install ffmpeg
-
-# Windows using Chocolatey https://chocolatey.org/
-choco install ffmpeg
-```
-
-# Quick guide
-Example usage for adding subtitles and translating them in Romanian:
-
-You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
-```py
-from gptsubtitler import Transcriber
-
-# I strongly recommend using the "medium" model_type.
-Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda")
-```
-
-You can also use the `Translator` class from `translator.py` if you just want to translate some text.
-
-Example usage for translating from English to Romanian:
-```py
-from gptsubtitler import Translator
-
-print(Translator.translate("Hi!", target_language="ro", source_language="en", device="cuda"))
-```
-
-If you have generated a `.srt` file and just want to add subtitles:
-```py
-from gptsubtitler import create_video_with_subtitles
-create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
-```
-
-# Options
-Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
-- cpu - default
-- cuda
-
-Available options for `model_type` (the audio to text model):
-- tiny
-- base - default
-- small
-- medium
-- large
-
-Available options for `language_model_type` (the language translator model):
-- base - default
-- large
-
-
+Metadata-Version: 2.1
+Name: gptsubtitler
+Version: 0.0.6
+Summary: Automatically subtitle any video spoken in any language to a language of your choice.
+Author: extremq
+Author-email: extremqcontact@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Subtitler
+Automatically subtitle any video spoken in any language to a language of your choice using AI.
+
+Models used:
+- [OpenAI whisper](https://openai.com/research/whisper) - for audio-to-text
+- [Facebook M2M10](https://huggingface.co/facebook/m2m100_418M) - for translation
+
+Tools used:
+- `ffmpeg`
+
+**Please don't forget to star the repository if you find it useful or educational!**
+
+Before:
+
+https://github.com/extremq/subtitler/assets/45830561/49f6ecce-cfdc-4f1c-97eb-07a36ac841c9
+
+After (in Romanian - `model_type=medium, language_model_type=base`):
+
+https://github.com/extremq/subtitler/assets/45830561/20bc5169-0ce3-47cd-adb7-15d75daf27f4
+
+# Setup
+Install using `pip`.
+
+```
+pip install gptsubtitler
+```
+
+Install [`ffmpeg`](https://ffmpeg.org/):
+```bash
+# Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
+
+# MacOS
+brew install ffmpeg
+
+# Windows using Chocolatey https://chocolatey.org/
+choco install ffmpeg
+```
+
+# Quick guide
+Example usage for adding subtitles and translating them in Romanian:
+
+You only need to specify the language you want the subtitles to be in, the program will handle the rest of the work.
+```py
+from gptsubtitler import Transcriber
+
+# I strongly recommend using the "medium" model_type.
+Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base")
+
+# If you want to use the gpu, add device="cuda"
+# Transcriber.transcribe("soldier.mp4", target_language="ro", model_type="medium", language_model_type="base", device="cuda") 
+```
+
+You can also use the `Translator` class from `translator.py` if you just want to translate some text.
+
+Example usage for translating from English to Romanian:
+```py
+from gptsubtitler import Translator
+
+print(Translator.translate("Hi!", target_language="ro", source_language="en"))
+```
+
+If you have generated a `.srt` file and just want to add subtitles:
+```py
+from gptsubtitler import create_video_with_subtitles
+create_video_with_subtitles("video.mp4", "output.srt", "video_subtitled.mp4")
+```
+
+# Options
+Device (if you have a gpu and have installed [pytorch](https://pytorch.org/get-started/locally/), use "cuda"):
+- cpu - default
+- cuda
+
+Available options for `model_type` (the audio to text model):
+- tiny
+- base - default
+- small
+- medium
+- large
+
+Available options for `language_model_type` (the language translator model):
+- base - default
+- large
```

### Comparing `gptsubtitler-0.0.5/setup.py` & `gptsubtitler-0.0.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from setuptools import setup
-
-def readme():
-    with open('README.md') as f:
-        return f.read()
-
-setup(
-    name="gptsubtitler",
-    version="0.0.5",
-    author="extremq",
-    author_email="extremqcontact@gmail.com",
-    description="Automatically subtitle any video spoken in any language to a language of your choice.",
-    install_requires=[
-        "transformers",
-        "openai-whisper",
-    ],
-    packages=["gptsubtitler"],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    long_description=readme(),
-    long_description_content_type = "text/markdown"
+from setuptools import setup
+
+def readme():
+    with open('README.md') as f:
+        return f.read()
+
+setup(
+    name="gptsubtitler",
+    version="0.0.6",
+    author="extremq",
+    author_email="extremqcontact@gmail.com",
+    description="Automatically subtitle any video spoken in any language to a language of your choice.",
+    install_requires=[
+        "transformers",
+        "openai-whisper",
+    ],
+    packages=["gptsubtitler"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    long_description=readme(),
+    long_description_content_type = "text/markdown"
 )
```

