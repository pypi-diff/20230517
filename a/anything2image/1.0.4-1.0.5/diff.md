# Comparing `tmp/anything2image-1.0.4.tar.gz` & `tmp/anything2image-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/extssd2/Anything2Image/dist/.tmp-d6_ghvoy/anything2image-1.0.4.tar", last modified: Wed May 17 04:59:12 2023, max compression
+gzip compressed data, was "/media/extssd2/Anything2Image/dist/.tmp-obrrsdoq/anything2image-1.0.5.tar", last modified: Wed May 17 06:55:06 2023, max compression
```

## Comparing `anything2image-1.0.4.tar` & `anything2image-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 04:59:12.000000 anything2image-1.0.4/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 04:59:12.000000 anything2image-1.0.4/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7850 2023-05-17 03:21:51.000000 anything2image-1.0.4/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:55:36.000000 anything2image-1.0.4/anything2image/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2305 2023-05-17 02:51:40.000000 anything2image-1.0.4/anything2image/api.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1593 2023-05-17 04:57:59.000000 anything2image-1.0.4/anything2image/app.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-17 02:52:25.000000 anything2image-1.0.4/anything2image/cli.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image/imagebind/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      200 2023-05-17 00:42:51.000000 anything2image-1.0.4/anything2image/imagebind/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image/imagebind/bpe/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)  1356917 2023-05-17 00:42:51.000000 anything2image-1.0.4/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11890 2023-05-17 00:42:51.000000 anything2image-1.0.4/anything2image/imagebind/data.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image/imagebind/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:42:51.000000 anything2image-1.0.4/anything2image/imagebind/models/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3983 2023-05-17 00:42:51.000000 anything2image-1.0.4/anything2image/imagebind/models/helpers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16640 2023-05-17 02:20:59.000000 anything2image-1.0.4/anything2image/imagebind/models/imagebind_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    23088 2023-05-17 00:42:51.000000 anything2image-1.0.4/anything2image/imagebind/models/multimodal_preprocessors.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9748 2023-05-17 00:42:51.000000 anything2image-1.0.4/anything2image/imagebind/models/transformer.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      673 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      120 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       15 2023-05-17 04:59:12.000000 anything2image-1.0.4/anything2image.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-17 04:59:12.000000 anything2image-1.0.4/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      555 2023-05-17 04:58:57.000000 anything2image-1.0.4/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 06:55:06.000000 anything2image-1.0.5/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 06:55:06.000000 anything2image-1.0.5/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7850 2023-05-17 03:21:51.000000 anything2image-1.0.5/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:55:36.000000 anything2image-1.0.5/anything2image/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2305 2023-05-17 02:51:40.000000 anything2image-1.0.5/anything2image/api.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1594 2023-05-17 06:52:41.000000 anything2image-1.0.5/anything2image/app.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-17 02:52:25.000000 anything2image-1.0.5/anything2image/cli.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image/imagebind/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      200 2023-05-17 00:42:51.000000 anything2image-1.0.5/anything2image/imagebind/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image/imagebind/bpe/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)  1356917 2023-05-17 00:42:51.000000 anything2image-1.0.5/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11890 2023-05-17 00:42:51.000000 anything2image-1.0.5/anything2image/imagebind/data.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image/imagebind/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 00:42:51.000000 anything2image-1.0.5/anything2image/imagebind/models/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3983 2023-05-17 00:42:51.000000 anything2image-1.0.5/anything2image/imagebind/models/helpers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    16640 2023-05-17 02:20:59.000000 anything2image-1.0.5/anything2image/imagebind/models/imagebind_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    23088 2023-05-17 00:42:51.000000 anything2image-1.0.5/anything2image/imagebind/models/multimodal_preprocessors.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9748 2023-05-17 00:42:51.000000 anything2image-1.0.5/anything2image/imagebind/models/transformer.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       58 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      673 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      120 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       15 2023-05-17 06:55:06.000000 anything2image-1.0.5/anything2image.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-17 06:55:06.000000 anything2image-1.0.5/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      555 2023-05-17 06:53:16.000000 anything2image-1.0.5/setup.py
```

### Comparing `anything2image-1.0.4/README.md` & `anything2image-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/api.py` & `anything2image-1.0.5/anything2image/api.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/app.py` & `anything2image-1.0.5/anything2image/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                 """)
         gr.Interface(fn=anything2img, 
                      inputs=["text",
                              "audio", 
                              "image", 
                              "text",
                              ], 
-                     outputs="text",
+                     outputs="image",
                      examples=[['', 'assets/wav/dog_audio.wav', None, None],
                                ['A painting', 'assets/wav/cat.wav', None, None],
                                ['', 'assets/wav/wave.wav', 'assets/image/bird.png', None],
                                ['', None, 'assets/image/bird_image.jpg', None],
                                ['', None, None, 'A sunset over the ocean.'],
                                ],
                      cache_examples=True,
```

#### html2text {}

```diff
@@ -4,13 +4,13 @@
 anything2img = Anything2Image(imagebind_download_dir=ckpt_dir) with gr.Blocks()
 as demo: gr.HTML( """
                         ****** Anything To Image ******
 Generate image from anything with ImageBind's unified latent space and stable-
                              diffusion-2-1-unclip.
                  https://github.com/Zeqiang-Lai/Anything2Image
 """) gr.Interface(fn=anything2img, inputs=["text", "audio", "image", "text", ],
-outputs="text", examples=[['', 'assets/wav/dog_audio.wav', None, None], ['A
+outputs="image", examples=[['', 'assets/wav/dog_audio.wav', None, None], ['A
 painting', 'assets/wav/cat.wav', None, None], ['', 'assets/wav/wave.wav',
 'assets/image/bird.png', None], ['', None, 'assets/image/bird_image.jpg',
 None], ['', None, None, 'A sunset over the ocean.'], ], cache_examples=True, )
 demo.queue(1).launch(server_name=ip, server_port=port, share=share) fire.Fire
 (main)
```

### Comparing `anything2image-1.0.4/anything2image/cli.py` & `anything2image-1.0.5/anything2image/cli.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz` & `anything2image-1.0.5/anything2image/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/imagebind/data.py` & `anything2image-1.0.5/anything2image/imagebind/data.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/imagebind/models/helpers.py` & `anything2image-1.0.5/anything2image/imagebind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/imagebind/models/imagebind_model.py` & `anything2image-1.0.5/anything2image/imagebind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/imagebind/models/multimodal_preprocessors.py` & `anything2image-1.0.5/anything2image/imagebind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image/imagebind/models/transformer.py` & `anything2image-1.0.5/anything2image/imagebind/models/transformer.py`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/anything2image.egg-info/SOURCES.txt` & `anything2image-1.0.5/anything2image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anything2image-1.0.4/setup.py` & `anything2image-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='anything2image',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     package_data={
         'anything2image': ['imagebind/bpe/bpe_simple_vocab_16e6.txt.gz']
     },
     include_package_data=True,
     install_requires=[
         'diffusers',
```

