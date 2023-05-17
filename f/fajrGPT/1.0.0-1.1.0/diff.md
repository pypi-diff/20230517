# Comparing `tmp/fajrGPT-1.0.0.tar.gz` & `tmp/fajrGPT-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.0.0.tar", last modified: Wed May 17 16:39:54 2023, max compression
+gzip compressed data, was "fajrGPT-1.1.0.tar", last modified: Wed May 17 17:17:52 2023, max compression
```

## Comparing `fajrGPT-1.0.0.tar` & `fajrGPT-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 16:39:54.185732 fajrGPT-1.0.0/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.0.0/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 16:39:54.185610 fajrGPT-1.0.0/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2326 2023-05-17 15:03:13.000000 fajrGPT-1.0.0/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 16:39:54.184315 fajrGPT-1.0.0/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-1.0.0/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.0.0/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     7753 2023-05-17 16:38:54.000000 fajrGPT-1.0.0/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 16:39:54.185390 fajrGPT-1.0.0/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 16:39:54.185803 fajrGPT-1.0.0/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 16:39:18.000000 fajrGPT-1.0.0/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 17:17:52.028252 fajrGPT-1.1.0/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.0/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 17:17:52.028118 fajrGPT-1.1.0/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2326 2023-05-17 15:03:13.000000 fajrGPT-1.1.0/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 17:17:52.026820 fajrGPT-1.1.0/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-1.1.0/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.0/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     8002 2023-05-17 17:16:11.000000 fajrGPT-1.1.0/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 17:17:52.027928 fajrGPT-1.1.0/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 17:17:51.000000 fajrGPT-1.1.0/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 17:17:52.000000 fajrGPT-1.1.0/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 17:17:51.000000 fajrGPT-1.1.0/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 17:17:51.000000 fajrGPT-1.1.0/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 17:17:51.000000 fajrGPT-1.1.0/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 17:17:51.000000 fajrGPT-1.1.0/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 17:17:52.028293 fajrGPT-1.1.0/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 17:16:21.000000 fajrGPT-1.1.0/setup.py
```

### Comparing `fajrGPT-1.0.0/LICENSE` & `fajrGPT-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.0.0/PKG-INFO` & `fajrGPT-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.0.0/README.md` & `fajrGPT-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.0.0/fajrGPT/quran_metadata.py` & `fajrGPT-1.1.0/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.0.0/fajrGPT/wake.py` & `fajrGPT-1.1.0/fajrGPT/wake.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 import random
 from tqdm import tqdm
 from Quran_Module import Project_Quran
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 COMPLETIONS_MODEL = "gpt-3.5-turbo"
 
-@click.command()
-@click.option('--url', required=True, help='YouTube video URL.')
-@click.option('--hours', required=True, help='Countdown hours.')
-@click.option('--output', required=True, help='Name of the output file.')
+# @click.command()
+# @click.option('--url', required=True, help='YouTube video URL.')
+# @click.option('--hours', required=True, help='Countdown hours.')
+# @click.option('--output', required=True, help='Name of the output file.')
 
 def main(url, hours, output):
     # Download video
     flag = download_video(url,output)
 
     # test audio
     test_audio(f'{output}.mp3',output,flag)
@@ -37,17 +37,18 @@
 
     # display the quran verses
     get_verses_and_explanations()
 
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
-    # Wait for the audio to stop
+    # return back to the main thread
     play_audio_thread.join()
 
+
 def download_video(url,output):
     ydl_opts = {
         'format': 'bestaudio/best',
         'postprocessors': [{
             'key': 'FFmpegExtractAudio',
             'preferredcodec': 'mp3',
             'preferredquality': '192',
@@ -202,17 +203,21 @@
     # Loop the audio until the stop_audio function is called
     while not stop_audio_called:
         if not pygame.mixer.music.get_busy():
             # The music has finished, restart it
             pygame.mixer.music.play()
         time.sleep(1)    
 
-    # Stop the audio
-    pygame.mixer.music.stop()
-
 def stop_audio():
     global stop_audio_called
+    stop_audio_called = True # stop the audio in the other thread
+    time.sleep(1)
+    stop_audio_called = False # reset back to False to allow volume to decrease
     gradually_change_volume(pygame.mixer.music.get_volume(), 0.0, 10)
+
+    # Stop the audio completely
     stop_audio_called = True
+    pygame.mixer.music.stop()
 
 if __name__ == "__main__":
-    main()
+    main("https://www.youtube.com/watch?v=zlOKoHk9W0I", "0", "islam1")
+
```

### Comparing `fajrGPT-1.0.0/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.1.0/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.0.0/setup.py` & `fajrGPT-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.0.0",
+    version="1.1.0",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

