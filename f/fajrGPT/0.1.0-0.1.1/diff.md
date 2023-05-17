# Comparing `tmp/fajrGPT-0.1.0.tar.gz` & `tmp/fajrGPT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-0.1.0.tar", last modified: Wed May 17 14:09:39 2023, max compression
+gzip compressed data, was "fajrGPT-0.1.1.tar", last modified: Wed May 17 14:59:04 2023, max compression
```

## Comparing `fajrGPT-0.1.0.tar` & `fajrGPT-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 14:09:39.583846 fajrGPT-0.1.0/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-0.1.0/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2754 2023-05-17 14:09:39.583716 fajrGPT-0.1.0/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2091 2023-05-17 14:06:10.000000 fajrGPT-0.1.0/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 14:09:39.582489 fajrGPT-0.1.0/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-0.1.0/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-0.1.0/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     7306 2023-05-17 13:22:03.000000 fajrGPT-0.1.0/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 14:09:39.583523 fajrGPT-0.1.0/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2754 2023-05-17 14:09:39.000000 fajrGPT-0.1.0/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 14:09:39.000000 fajrGPT-0.1.0/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 14:09:39.000000 fajrGPT-0.1.0/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 14:09:39.000000 fajrGPT-0.1.0/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 14:09:39.000000 fajrGPT-0.1.0/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 14:09:39.000000 fajrGPT-0.1.0/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 14:09:39.583883 fajrGPT-0.1.0/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 14:07:14.000000 fajrGPT-0.1.0/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 14:59:04.371051 fajrGPT-0.1.1/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-0.1.1/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2927 2023-05-17 14:59:04.370927 fajrGPT-0.1.1/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2264 2023-05-17 14:58:42.000000 fajrGPT-0.1.1/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 14:59:04.369514 fajrGPT-0.1.1/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-05-17 12:47:41.000000 fajrGPT-0.1.1/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-0.1.1/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     7497 2023-05-17 14:57:53.000000 fajrGPT-0.1.1/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-05-17 14:59:04.370750 fajrGPT-0.1.1/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2927 2023-05-17 14:59:04.000000 fajrGPT-0.1.1/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-05-17 14:59:04.000000 fajrGPT-0.1.1/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-05-17 14:59:04.000000 fajrGPT-0.1.1/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-05-17 14:59:04.000000 fajrGPT-0.1.1/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       39 2023-05-17 14:59:04.000000 fajrGPT-0.1.1/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-05-17 14:59:04.000000 fajrGPT-0.1.1/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-05-17 14:59:04.371086 fajrGPT-0.1.1/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1104 2023-05-17 14:57:59.000000 fajrGPT-0.1.1/setup.py
```

### Comparing `fajrGPT-0.1.0/LICENSE` & `fajrGPT-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.0/PKG-INFO` & `fajrGPT-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python application to assist in waking up for Fajr prayerby providing 3 interactive verses + explanations from the Quran + ChatGPT explanationsaccompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,17 @@
 ## Usage
 
 1. Clone repo and install packages:
     ```bash
     pip install -r requirements.txt
     pip install .
     ```
-2. Install `fajrGPT`
+2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
     ```python
+    pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
     pip install fajrGPT
     ```
 3. Run the main.py script, passing the required parameters:
     ```bash
     fajrGPT --url <YouTube URL> --hours <Hours for Countdown> --output <Output filename>
     ```
     Replace `<YouTube URL>`, `<Hours for Countdown>`, and `<Output filename>` with appropriate values.
```

### Comparing `fajrGPT-0.1.0/README.md` & `fajrGPT-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 ## Usage
 
 1. Clone repo and install packages:
     ```bash
     pip install -r requirements.txt
     pip install .
     ```
-2. Install `fajrGPT`
+2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
     ```python
+    pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
     pip install fajrGPT
     ```
 3. Run the main.py script, passing the required parameters:
     ```bash
     fajrGPT --url <YouTube URL> --hours <Hours for Countdown> --output <Output filename>
     ```
     Replace `<YouTube URL>`, `<Hours for Countdown>`, and `<Output filename>` with appropriate values.
```

### Comparing `fajrGPT-0.1.0/fajrGPT/quran_metadata.py` & `fajrGPT-0.1.1/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-0.1.0/fajrGPT/wake.py` & `fajrGPT-0.1.1/fajrGPT/wake.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 @click.command()
 @click.option('--url', required=True, help='YouTube video URL.')
 @click.option('--hours', required=True, help='Countdown hours.')
 @click.option('--output', required=True, help='Name of the output file.')
 
 def main(url, hours, output):
     # Download video
-    download_video(url,output)
+    flag = download_video(url,output)
 
     # test audio
-    test_audio(f'{output}.mp3',output)
+    test_audio(f'{output}.mp3',output,flag)
 
     # Start countdown
     countdown(hours)
 
     # Play audio with fade-in effect
     play_audio(f'{output}.mp3')
 
@@ -42,29 +42,35 @@
             'preferredquality': '192',
         }],
         'outtmpl': f'{output}.mp3',  # name of the audio file
         'quiet': False,
         'verbose': True,
     }
     if not os.path.exists(f'{output}.mp3'):
+        converted_flag = False
         with youtube_dl.YoutubeDL(ydl_opts) as ydl:
             ydl.download([url])
+    else:
+        converted_flag = True
+    return converted_flag
 
-def test_audio(file_path,output):
+def test_audio(file_path,output,converted_flag):
     # rename the {output}.mp3 file to temp.mp3
-    if not os.path.exists(f'{output}.mp3'):
+    if not converted_flag:
         os.rename(f'{output}.mp3', 'temp.mp3')
         command = f'ffmpeg -i temp.mp3 {output}.mp3'
         # remove the temp.mp3 file
         subprocess.run(command, shell=True)
         os.remove('temp.mp3')
         try:
             audio = AudioSegment.from_file(file_path, format="mp3")
         except:
             print("Error: Audio file could not be loaded.")
+    else:
+        print(f'{output}.mp3 has already been downloaded and converted.')
 
 def countdown(hours):
     countdown_seconds = float(hours) * 60 * 60
     # use tqdm to display the countdown progress
     for i in tqdm(range(int(countdown_seconds))):
         time.sleep(1)
```

### Comparing `fajrGPT-0.1.0/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-0.1.1/fajrGPT.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python application to assist in waking up for Fajr prayerby providing 3 interactive verses + explanations from the Quran + ChatGPT explanationsaccompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,17 @@
 ## Usage
 
 1. Clone repo and install packages:
     ```bash
     pip install -r requirements.txt
     pip install .
     ```
-2. Install `fajrGPT`
+2. Alternatively, install some dependencies manually and `fajrGPT` through PyPI:
     ```python
+    pip install git+https://github.com/ytdl-org/youtube-dl.git git+https://github.com/UBISOFT-1/Quran_Module.git
     pip install fajrGPT
     ```
 3. Run the main.py script, passing the required parameters:
     ```bash
     fajrGPT --url <YouTube URL> --hours <Hours for Countdown> --output <Output filename>
     ```
     Replace `<YouTube URL>`, `<Hours for Countdown>`, and `<Output filename>` with appropriate values.
```

### Comparing `fajrGPT-0.1.0/setup.py` & `fajrGPT-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="0.1.0",
+    version="0.1.1",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer"
                  "by providing 3 interactive verses + explanations from the Quran + ChatGPT explanations"
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

