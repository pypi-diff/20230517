# Comparing `tmp/anything2image-1.0.2.tar.gz` & `tmp/anything2image-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/extssd2/Anything2Image/dist/.tmp-t42xlpd6/anything2image-1.0.2.tar", last modified: Wed May 17 03:09:55 2023, max compression
+gzip compressed data, was "/media/extssd2/Anything2Image/dist/.tmp-sxe0quvy/anything2image-1.0.3.tar", last modified: Wed May 17 03:21:05 2023, max compression
```

## Comparing `anything2image-1.0.2.tar` & `anything2image-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 03:09:55.000000 anything2image-1.0.2/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7860 2023-05-17 03:01:04.000000 anything2image-1.0.2/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:55:36.000000 anything2image-1.0.2/anything2image/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2305 2023-05-17 02:51:40.000000 anything2image-1.0.2/anything2image/api.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      476 2023-05-17 02:58:53.000000 anything2image-1.0.2/anything2image/app.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-17 02:52:25.000000 anything2image-1.0.2/anything2image/cli.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/imagebind/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      200 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/imagebind/bpe/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)  1356917 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11890 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/data.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image/imagebind/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3983 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/helpers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16640 2023-05-17 02:20:59.000000 anything2image-1.0.2/anything2image/imagebind/models/imagebind_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    23088 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/multimodal_preprocessors.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9748 2023-05-17 00:42:51.000000 anything2image-1.0.2/anything2image/imagebind/models/transformer.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      673 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       96 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       15 2023-05-17 03:09:55.000000 anything2image-1.0.2/anything2image.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-17 03:09:55.000000 anything2image-1.0.2/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      510 2023-05-17 03:09:31.000000 anything2image-1.0.2/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:21:05.000000 anything2image-1.0.3/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 03:21:05.000000 anything2image-1.0.3/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7913 2023-05-17 03:14:02.000000 anything2image-1.0.3/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:55:36.000000 anything2image-1.0.3/anything2image/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2305 2023-05-17 02:51:40.000000 anything2image-1.0.3/anything2image/api.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      476 2023-05-17 02:58:53.000000 anything2image-1.0.3/anything2image/app.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-17 02:52:25.000000 anything2image-1.0.3/anything2image/cli.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image/imagebind/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      200 2023-05-17 00:42:51.000000 anything2image-1.0.3/anything2image/imagebind/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image/imagebind/bpe/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)  1356917 2023-05-17 00:42:51.000000 anything2image-1.0.3/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11890 2023-05-17 00:42:51.000000 anything2image-1.0.3/anything2image/imagebind/data.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image/imagebind/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:42:51.000000 anything2image-1.0.3/anything2image/imagebind/models/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3983 2023-05-17 00:42:51.000000 anything2image-1.0.3/anything2image/imagebind/models/helpers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16640 2023-05-17 02:20:59.000000 anything2image-1.0.3/anything2image/imagebind/models/imagebind_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    23088 2023-05-17 00:42:51.000000 anything2image-1.0.3/anything2image/imagebind/models/multimodal_preprocessors.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9748 2023-05-17 00:42:51.000000 anything2image-1.0.3/anything2image/imagebind/models/transformer.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      673 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      120 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       15 2023-05-17 03:21:05.000000 anything2image-1.0.3/anything2image.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-17 03:21:05.000000 anything2image-1.0.3/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      555 2023-05-17 03:20:22.000000 anything2image-1.0.3/setup.py
```

### Comparing `anything2image-1.0.2/README.md` & `anything2image-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 - [Audio to Image](#audio-to-image)
 - [Audio+Text to Image](#audiotext-to-image)
 - [Audio+Image to Image](#audioimage-to-image)
 - [Image to Image](#image-to-image)
 - [Text to Image](#text-to-image)
 
+**Requirements**
+
+- Python >= 3.8
+- PyTorch >= 1.13
+
 **Usage**
 
 ```bash
 pip install anything2image
 # lanuch gradio demo
 python -m anything2image.app
 ```
```

#### html2text {}

```diff
@@ -6,30 +6,31 @@
 huggingface.co/stabilityai/stable-diffusion-2-1-unclip). - No training is need.
 - Integration with ð¤ [Diffusers](https://github.com/huggingface/diffusers).
 - Online gradio demo with [Huggingface Space](https://huggingface.co/spaces/
 aaronb/Anything2Image). - GPU Demo at [Here](https://
 50942325ab9a89e397.gradio.live/). **Support Tasks** - [Audio to Image](#audio-
 to-image) - [Audio+Text to Image](#audiotext-to-image) - [Audio+Image to Image]
 (#audioimage-to-image) - [Image to Image](#image-to-image) - [Text to Image]
-(#text-to-image) **Usage** ```bash pip install anything2image # lanuch gradio
-demo python -m anything2image.app ``` ## Audio to Image | [bird_audio.wav]
-(assets/wav/bird_audio.wav) | [dog_audio.wav](assets/wav/dog_audio.wav) |
-[cattle.wav](assets/wav/cattle.wav) | [cat.wav](assets/wav/cat.wav) | | --- | -
--- | --- | --- | | ![](assets/generated/audio_to_image/bird_audio.png) | ![]
-(assets/generated/audio_to_image/dog_audio.png) |![](assets/generated/
-audio_to_image/cattle.png) |![](assets/generated/audio_to_image/cat.png) | |
-[fire_engine.wav](assets/wav/fire_engine.wav) | [train.wav](assets/wav/
-train.wav) | [motorcycle.wav](assets/wav/motorcycle.wav) | [plane.wav](assets/
-wav/plane.wav) | | --- | --- | --- | --- | | ![](assets/generated/
-audio_to_image/fire_engine.png) | ![](assets/generated/audio_to_image/
-train.png) |![](assets/generated/audio_to_image/motorcycle.png) |![](assets/
-generated/audio_to_image/plane.png) | ```bash python -m anything2image.cli --
-audio assets/wav/cat.wav ``` See also [audio2img.py](tasks/audio2img.py).
-```python import anything2image.imagebind as ib import torch from diffusers
-import StableUnCLIPImg2ImgPipeline # construct models device = "cuda:0" if
+(#text-to-image) **Requirements** - Python >= 3.8 - PyTorch >= 1.13 **Usage**
+```bash pip install anything2image # lanuch gradio demo python -
+m anything2image.app ``` ## Audio to Image | [bird_audio.wav](assets/wav/
+bird_audio.wav) | [dog_audio.wav](assets/wav/dog_audio.wav) | [cattle.wav]
+(assets/wav/cattle.wav) | [cat.wav](assets/wav/cat.wav) | | --- | --- | --- | -
+-- | | ![](assets/generated/audio_to_image/bird_audio.png) | ![](assets/
+generated/audio_to_image/dog_audio.png) |![](assets/generated/audio_to_image/
+cattle.png) |![](assets/generated/audio_to_image/cat.png) | | [fire_engine.wav]
+(assets/wav/fire_engine.wav) | [train.wav](assets/wav/train.wav) |
+[motorcycle.wav](assets/wav/motorcycle.wav) | [plane.wav](assets/wav/plane.wav)
+| | --- | --- | --- | --- | | ![](assets/generated/audio_to_image/
+fire_engine.png) | ![](assets/generated/audio_to_image/train.png) |![](assets/
+generated/audio_to_image/motorcycle.png) |![](assets/generated/audio_to_image/
+plane.png) | ```bash python -m anything2image.cli --audio assets/wav/cat.wav
+``` See also [audio2img.py](tasks/audio2img.py). ```python import
+anything2image.imagebind as ib import torch from diffusers import
+StableUnCLIPImg2ImgPipeline # construct models device = "cuda:0" if
 torch.cuda.is_available() else "cpu" pipe =
 StableUnCLIPImg2ImgPipeline.from_pretrained( "stabilityai/stable-diffusion-2-1-
 unclip", torch_dtype=torch.float16 ).to(device) model = ib.imagebind_huge
 (pretrained=True).eval().to(device) # generate image with torch.no_grad():
 audio_paths=["assets/wav/bird_audio.wav"] embeddings = model.forward(
 { ib.ModalityType.AUDIO: ib.load_and_transform_audio_data(audio_paths, device),
 }) embeddings = embeddings[ib.ModalityType.AUDIO] images = pipe
```

### Comparing `anything2image-1.0.2/anything2image/api.py` & `anything2image-1.0.3/anything2image/api.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image/cli.py` & `anything2image-1.0.3/anything2image/cli.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz` & `anything2image-1.0.3/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image/imagebind/data.py` & `anything2image-1.0.3/anything2image/imagebind/data.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image/imagebind/models/helpers.py` & `anything2image-1.0.3/anything2image/imagebind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image/imagebind/models/imagebind_model.py` & `anything2image-1.0.3/anything2image/imagebind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image/imagebind/models/multimodal_preprocessors.py` & `anything2image-1.0.3/anything2image/imagebind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image/imagebind/models/transformer.py` & `anything2image-1.0.3/anything2image/imagebind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.2/anything2image.egg-info/SOURCES.txt` & `anything2image-1.0.3/anything2image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

