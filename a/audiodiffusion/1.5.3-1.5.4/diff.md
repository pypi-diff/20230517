# Comparing `tmp/audiodiffusion-1.5.3.tar.gz` & `tmp/audiodiffusion-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiodiffusion-1.5.3.tar", last modified: Sat Apr 22 08:37:15 2023, max compression
+gzip compressed data, was "audiodiffusion-1.5.4.tar", last modified: Wed May 17 15:16:42 2023, max compression
```

## Comparing `audiodiffusion-1.5.3.tar` & `audiodiffusion-1.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.3/LICENSE
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.3/README.md
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-04-22 08:37:15.789655 audiodiffusion-1.5.3/audiodiffusion/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-04-22 08:32:34.000000 audiodiffusion-1.5.3/audiodiffusion/__init__.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     3490 2022-12-24 15:06:00.000000 audiodiffusion-1.5.3/audiodiffusion/audio_encoder.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5671 2023-02-01 22:49:09.000000 audiodiffusion-1.5.3/audiodiffusion/mel.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    10809 2023-04-22 08:29:21.000000 audiodiffusion-1.5.3/audiodiffusion/pipeline_audio_diffusion.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.3/audiodiffusion/utils.py
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/audiodiffusion.egg-info/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/SOURCES.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/dependency_links.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/not-zip-safe
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/requires.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/top_level.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.3/pyproject.toml
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/setup.cfg
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.3/setup.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.4/LICENSE
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.4/README.md
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-17 15:16:42.695539 audiodiffusion-1.5.4/audiodiffusion/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-05-17 15:13:51.000000 audiodiffusion-1.5.4/audiodiffusion/__init__.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     3490 2022-12-24 15:06:00.000000 audiodiffusion-1.5.4/audiodiffusion/audio_encoder.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5680 2023-05-17 15:12:31.000000 audiodiffusion-1.5.4/audiodiffusion/mel.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    10809 2023-04-22 08:29:21.000000 audiodiffusion-1.5.4/audiodiffusion/pipeline_audio_diffusion.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.4/audiodiffusion/utils.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/audiodiffusion.egg-info/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/not-zip-safe
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/requires.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-05-17 15:16:42.000000 audiodiffusion-1.5.4/audiodiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.4/pyproject.toml
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-05-17 15:16:42.699539 audiodiffusion-1.5.4/setup.cfg
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.4/setup.py
```

### Comparing `audiodiffusion-1.5.3/LICENSE` & `audiodiffusion-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.3/PKG-INFO` & `audiodiffusion-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.3
+Version: 1.5.4
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

### Comparing `audiodiffusion-1.5.3/README.md` & `audiodiffusion-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.3/audiodiffusion/__init__.py` & `audiodiffusion-1.5.4/audiodiffusion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from librosa.beat import beat_track
 from PIL import Image
 from tqdm.auto import tqdm
 
 # from diffusers import AudioDiffusionPipeline
 from .pipeline_audio_diffusion import AudioDiffusionPipeline
 
-VERSION = "1.5.3"
+VERSION = "1.5.4"
 
 
 class AudioDiffusion:
     def __init__(
         self,
         model_id: str = "teticio/audio-diffusion-256",
         cuda: bool = torch.cuda.is_available(),
```

### Comparing `audiodiffusion-1.5.3/audiodiffusion/audio_encoder.py` & `audiodiffusion-1.5.4/audiodiffusion/audio_encoder.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.3/audiodiffusion/mel.py` & `audiodiffusion-1.5.4/audiodiffusion/mel.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,27 +128,27 @@
         """Get sample rate:
 
         Returns:
             `int`: sample rate of audio
         """
         return self.sr
 
-    def audio_slice_to_image(self, slice: int) -> Image.Image:
+    def audio_slice_to_image(self, slice: int, ref=np.max) -> Image.Image:
         """Convert slice of audio to spectrogram.
 
         Args:
             slice (`int`): slice number of audio to convert (out of get_number_of_slices())
 
         Returns:
             `PIL Image`: grayscale image of x_res x y_res
         """
         S = librosa.feature.melspectrogram(
             y=self.get_audio_slice(slice), sr=self.sr, n_fft=self.n_fft, hop_length=self.hop_length, n_mels=self.n_mels
         )
-        log_S = librosa.power_to_db(S, ref=np.max, top_db=self.top_db)
+        log_S = librosa.power_to_db(S, ref=ref, top_db=self.top_db)
         bytedata = (((log_S + self.top_db) * 255 / self.top_db).clip(0, 255) + 0.5).astype(np.uint8)
         image = Image.fromarray(bytedata)
         return image
 
     def image_to_audio(self, image: Image.Image) -> np.ndarray:
         """Converts spectrogram to audio.
```

### Comparing `audiodiffusion-1.5.3/audiodiffusion/pipeline_audio_diffusion.py` & `audiodiffusion-1.5.4/audiodiffusion/pipeline_audio_diffusion.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.3/audiodiffusion/utils.py` & `audiodiffusion-1.5.4/audiodiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.3/audiodiffusion.egg-info/PKG-INFO` & `audiodiffusion-1.5.4/audiodiffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.3
+Version: 1.5.4
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

