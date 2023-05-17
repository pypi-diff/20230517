# Comparing `tmp/anything2image-1.0.1.tar.gz` & `tmp/anything2image-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/extssd2/Anything2Image/dist/.tmp-20khvx0t/anything2image-1.0.1.tar", last modified: Wed May 17 02:55:19 2023, max compression
+gzip compressed data, was "/media/extssd2/Anything2Image/dist/.tmp-t42xlpd6/anything2image-1.0.2.tar", last modified: Wed May 17 03:09:55 2023, max compression
```

## Comparing `anything2image-1.0.1.tar` & `anything2image-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 02:55:19.000000 anything2image-1.0.1/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 02:55:19.000000 anything2image-1.0.1/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7797 2023-05-17 02:54:25.000000 anything2image-1.0.1/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:55:36.000000 anything2image-1.0.1/anything2image/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2305 2023-05-17 02:51:40.000000 anything2image-1.0.1/anything2image/api.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      450 2023-05-17 02:16:38.000000 anything2image-1.0.1/anything2image/app.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-17 02:52:25.000000 anything2image-1.0.1/anything2image/cli.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image/imagebind/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      200 2023-05-17 00:42:51.000000 anything2image-1.0.1/anything2image/imagebind/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image/imagebind/bpe/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)  1356917 2023-05-17 00:42:51.000000 anything2image-1.0.1/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11890 2023-05-17 00:42:51.000000 anything2image-1.0.1/anything2image/imagebind/data.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image/imagebind/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:42:51.000000 anything2image-1.0.1/anything2image/imagebind/models/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3983 2023-05-17 00:42:51.000000 anything2image-1.0.1/anything2image/imagebind/models/helpers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16640 2023-05-17 02:20:59.000000 anything2image-1.0.1/anything2image/imagebind/models/imagebind_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    23088 2023-05-17 00:42:51.000000 anything2image-1.0.1/anything2image/imagebind/models/multimodal_preprocessors.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9748 2023-05-17 00:42:51.000000 anything2image-1.0.1/anything2image/imagebind/models/transformer.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      673 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      109 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       15 2023-05-17 02:55:19.000000 anything2image-1.0.1/anything2image.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-17 02:55:19.000000 anything2image-1.0.1/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      534 2023-05-17 02:53:07.000000 anything2image-1.0.1/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 03:09:55.000000 anything2image-1.0.2/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7860 2023-05-17 03:01:04.000000 anything2image-1.0.2/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:55:36.000000 anything2image-1.0.2/anything2image/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2305 2023-05-17 02:51:40.000000 anything2image-1.0.2/anything2image/api.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      476 2023-05-17 02:58:53.000000 anything2image-1.0.2/anything2image/app.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-17 02:52:25.000000 anything2image-1.0.2/anything2image/cli.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/imagebind/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      200 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/imagebind/bpe/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)  1356917 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11890 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/data.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/imagebind/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3983 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/helpers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16640 2023-05-17 02:20:59.000000 anything2image-1.0.2/anything2image/imagebind/models/imagebind_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    23088 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/multimodal_preprocessors.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9748 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/transformer.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      673 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       96 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       15 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-17 03:09:55.000000 anything2image-1.0.2/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      510 2023-05-17 03:09:31.000000 anything2image-1.0.2/setup.py
```

### Comparing `anything2image-1.0.1/README.md` & `anything2image-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![PyPI](https://img.shields.io/pypi/v/anything2image)](https://pypi.org/project/anything2image/) 
 
 Generate image from anything with [ImageBind](https://github.com/facebookresearch/ImageBind)'s unified latent space and [stable-diffusion-2-1-unclip](https://huggingface.co/stabilityai/stable-diffusion-2-1-unclip). 
 
 - No training is need.
 - Integration with 🤗  [Diffusers](https://github.com/huggingface/diffusers).
 - Online gradio demo with [Huggingface Space](https://huggingface.co/spaces/aaronb/Anything2Image).
+- GPU Demo at [Here](https://50942325ab9a89e397.gradio.live/).
 
 **Support Tasks**
 
 - [Audio to Image](#audio-to-image)
 - [Audio+Text to Image](#audiotext-to-image)
 - [Audio+Image to Image](#audioimage-to-image)
 - [Image to Image](#image-to-image)
```

#### html2text {}

```diff
@@ -2,16 +2,17 @@
 %F0%9F%A4%97%20Hugging%20Face-Spaces-blue] [![PyPI](https://img.shields.io/
 pypi/v/anything2image)](https://pypi.org/project/anything2image/) Generate
 image from anything with [ImageBind](https://github.com/facebookresearch/
 ImageBind)'s unified latent space and [stable-diffusion-2-1-unclip](https://
 huggingface.co/stabilityai/stable-diffusion-2-1-unclip). - No training is need.
 - Integration with ð¤ [Diffusers](https://github.com/huggingface/diffusers).
 - Online gradio demo with [Huggingface Space](https://huggingface.co/spaces/
-aaronb/Anything2Image). **Support Tasks** - [Audio to Image](#audio-to-image) -
-[Audio+Text to Image](#audiotext-to-image) - [Audio+Image to Image]
+aaronb/Anything2Image). - GPU Demo at [Here](https://
+50942325ab9a89e397.gradio.live/). **Support Tasks** - [Audio to Image](#audio-
+to-image) - [Audio+Text to Image](#audiotext-to-image) - [Audio+Image to Image]
 (#audioimage-to-image) - [Image to Image](#image-to-image) - [Text to Image]
 (#text-to-image) **Usage** ```bash pip install anything2image # lanuch gradio
 demo python -m anything2image.app ``` ## Audio to Image | [bird_audio.wav]
 (assets/wav/bird_audio.wav) | [dog_audio.wav](assets/wav/dog_audio.wav) |
 [cattle.wav](assets/wav/cattle.wav) | [cat.wav](assets/wav/cat.wav) | | --- | -
 -- | --- | --- | | ![](assets/generated/audio_to_image/bird_audio.png) | ![]
 (assets/generated/audio_to_image/dog_audio.png) |![](assets/generated/
```

### Comparing `anything2image-1.0.1/anything2image/api.py` & `anything2image-1.0.2/anything2image/api.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image/cli.py` & `anything2image-1.0.2/anything2image/cli.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz` & `anything2image-1.0.2/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image/imagebind/data.py` & `anything2image-1.0.2/anything2image/imagebind/data.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image/imagebind/models/helpers.py` & `anything2image-1.0.2/anything2image/imagebind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image/imagebind/models/imagebind_model.py` & `anything2image-1.0.2/anything2image/imagebind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image/imagebind/models/multimodal_preprocessors.py` & `anything2image-1.0.2/anything2image/imagebind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image/imagebind/models/transformer.py` & `anything2image-1.0.2/anything2image/imagebind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.1/anything2image.egg-info/SOURCES.txt` & `anything2image-1.0.2/anything2image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

