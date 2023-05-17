# Comparing `tmp/fajrGPT-0.1.3.tar.gz` & `tmp/fajrGPT-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-0.1.3.tar", last modified: Wed May 17 15:04:29 2023, max compression
+gzip compressed data, was "fajrGPT-1.0.0.tar", last modified: Wed May 17 16:39:54 2023, max compression
```

## Comparing `fajrGPT-0.1.3.tar` & `fajrGPT-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:04:29.347007 fajrGPT-0.1.3/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-0.1.3/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 15:04:29.346863 fajrGPT-0.1.3/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2326 2023-05-17 15:03:13.000000 fajrGPT-0.1.3/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:04:29.345550 fajrGPT-0.1.3/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-0.1.3/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-0.1.3/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     7497 2023-05-17 14:57:53.000000 fajrGPT-0.1.3/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 15:04:29.346607 fajrGPT-0.1.3/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 15:04:29.000000 fajrGPT-0.1.3/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 15:04:29.347046 fajrGPT-0.1.3/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 15:03:38.000000 fajrGPT-0.1.3/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 16:39:54.185732 fajrGPT-1.0.0/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.0.0/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 16:39:54.185610 fajrGPT-1.0.0/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2326 2023-05-17 15:03:13.000000 fajrGPT-1.0.0/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 16:39:54.184315 fajrGPT-1.0.0/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-1.0.0/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.0.0/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     7753 2023-05-17 16:38:54.000000 fajrGPT-1.0.0/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 16:39:54.185390 fajrGPT-1.0.0/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2989 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 16:39:54.000000 fajrGPT-1.0.0/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 16:39:54.185803 fajrGPT-1.0.0/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 16:39:18.000000 fajrGPT-1.0.0/setup.py
```

### Comparing `fajrGPT-0.1.3/LICENSE` & `fajrGPT-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.3/PKG-INFO` & `fajrGPT-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 0.1.3
+Version: 1.0.0
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-0.1.3/README.md` & `fajrGPT-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.3/fajrGPT/quran_metadata.py` & `fajrGPT-1.0.0/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.3/fajrGPT/wake.py` & `fajrGPT-1.0.0/fajrGPT/wake.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys; sys.path.append('./')
 import click
 import youtube_dl
 import pygame
 from pydub import AudioSegment
 from threading import Thread
 from fajrGPT.quran_metadata import quran_chapter_to_verse
 import time
@@ -26,16 +27,26 @@
 
     # test audio
     test_audio(f'{output}.mp3',output,flag)
 
     # Start countdown
     countdown(hours)
 
-    # Play audio with fade-in effect
-    play_audio(f'{output}.mp3')
+    # Play audio with fade-in effect on a separate thread
+    play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',))
+    play_audio_thread.start()
+
+    # display the quran verses
+    get_verses_and_explanations()
+
+    # stop the audio once the user has completed reading the verses
+    stop_audio()
+
+    # Wait for the audio to stop
+    play_audio_thread.join()
 
 def download_video(url,output):
     ydl_opts = {
         'format': 'bestaudio/best',
         'postprocessors': [{
             'key': 'FFmpegExtractAudio',
             'preferredcodec': 'mp3',
@@ -67,30 +78,32 @@
             print("Error: Audio file could not be loaded.")
     else:
         print(f'{output}.mp3 has already been downloaded and converted.')
 
 def countdown(hours):
     countdown_seconds = float(hours) * 60 * 60
     # use tqdm to display the countdown progress
+    print('\n\n\n\n ---------------- BEGINNING COUNTDOWN ---------------- \n\n\n\n')
     for i in tqdm(range(int(countdown_seconds))):
         time.sleep(1)
+    print('\n\n\n\n ---------------- COUNTDOWN COMPLETE ----------------')
 
 def get_verses_and_explanations():
     # Get the verses
     verses_Quran_Module, verses  = select_quran_verse()
     # print(f"Verse 1:\n{verses}")
 
     # initialize the verse_texts output and explanations output
     verse_texts = []
     explanations = []
 
     # Get the explanations
     for verse_QM, verse in zip(verses_Quran_Module, verses):
         verse_text = Project_Quran().Get_Ayah_English(verse_QM).split('"')[1][0:-1]
-        prompt2 = f"You are an Islamic Scholar with extensive knowledge on the Quran and the life of Prophet Muhammad (pbuh). Please provide the Tafsir (meaning) of {verse_text}, and if you know of any other alternative translations of the verse in question, please provide that too."
+        prompt2 = f"To the best of your knowledge, please provide the Tafsir (meaning) of {verse_text} which comes from verse {verse} of the Quran. If you know of any other alternative translations of the verse in question, please provide that too, but if you are not familiar with this verse, simply try to explain the language of the verse."
         explanation = query_gpt(prompt2)
         verse_texts.append(verse_text)
         explanations.append(explanation)
     
     # begin the interactive session
     for verse_text, explanation, verse in zip(verse_texts, explanations, verses):
         print(f'\n\n\n\n\n\n ------------------ FIRST VERSE ------------------') if verse == verses[0] else None
@@ -143,68 +156,63 @@
     response = openai.ChatCompletion.create(
                 messages = [{"role": "user", "content": prompt}],
                 **COMPLETIONS_API_PARAMS
             )
 
     return response['choices'][0]['message']['content']
 
-def gradually_decrease_volume():
-    # Gradually decrease the volume over 5 seconds
-    for i in range(1, 501):  # 500 steps over 5 seconds
-        pygame.mixer.music.set_volume(1 - i / 500.0)  # gradually decrease the volume
-        time.sleep(0.01)
-
-def stop_audio():
-    # Gradually decrease the volume over 5 seconds
-    get_verses_and_explanations()
-
-    # Start a new thread to gradually decrease the volume
-    Thread(target=gradually_decrease_volume).start()
+def gradually_change_volume(start_volume, end_volume, duration):
+    # Compute the number of steps and the change in volume per step
+    steps = duration
+    delta_volume = (end_volume - start_volume) / steps
+
+    # Set the initial volume
+    pygame.mixer.music.set_volume(start_volume)
+
+    # Gradually change the volume
+    for i in range(steps):
+        # Wait for 1 second
+        time.sleep(1)
 
-    # Stop the audio
-    pygame.mixer.music.stop()
+        # Change the volume
+        new_volume = start_volume + i * delta_volume
+        pygame.mixer.music.set_volume(new_volume)
+
+        # If the stop_audio function has been called, break the loop
+        if stop_audio_called:
+            print("Stopping volume change due to stop_audio being called")
+            break
 
 def play_audio(file_path):
+    global stop_audio_called
+    stop_audio_called = False
+
     # Initialize pygame mixer
     pygame.mixer.init()
 
     # Load the audio file
     pygame.mixer.music.load(file_path)
 
-    SONG_END = pygame.USEREVENT + 1
-    pygame.mixer.music.set_endevent(SONG_END)
-
-    # Start a new thread to gradually stop the audio
-    stop_audio_thread = Thread(target=stop_audio)
-    stop_audio_thread.start()
-
     # Start playing the audio with volume 0
     pygame.mixer.music.set_volume(0.0)
     pygame.mixer.music.play()
 
-    # Gradually increase the volume over 15 minutes
-    for i in range(1, 901):  # 900 seconds = 15 minutes
-        time.sleep(1)
-        pygame.mixer.music.set_volume(i / 900.0)  # gradually increase the volume
-        # break the loop if the stop_audio thread has finished
-        if not stop_audio_thread.is_alive():
-            break
-    
-    # if the audio reaches the end, restart from the beginning until the stop_audio thread has finished
-    while True:
-        for event in pygame.event.get():
-            if event.type == SONG_END:
-                pygame.mixer.music.stop()
-                pygame.mixer.music.play()
-        if not stop_audio_thread.is_alive():
-            break
-        time.sleep(0.5)  # Check more frequently to stop the music in a timely manner
+    # Gradually increase the volume over 15 minutes in a separate thread
+    gradually_change_volume(0.0, 1.0, 900)
 
-    # Wait for the stop_audio thread to finish
-    stop_audio_thread.join()
-    time.sleep(5)
+    # Loop the audio until the stop_audio function is called
+    while not stop_audio_called:
+        if not pygame.mixer.music.get_busy():
+            # The music has finished, restart it
+            pygame.mixer.music.play()
+        time.sleep(1)    
 
     # Stop the audio
     pygame.mixer.music.stop()
 
+def stop_audio():
+    global stop_audio_called
+    gradually_change_volume(pygame.mixer.music.get_volume(), 0.0, 10)
+    stop_audio_called = True
+
 if __name__ == "__main__":
     main()
```

### Comparing `fajrGPT-0.1.3/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.0.0/fajrGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 0.1.3
+Version: 1.0.0
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-0.1.3/setup.py` & `fajrGPT-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="0.1.3",
+    version="1.0.0",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

