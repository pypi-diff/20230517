# Comparing `tmp/term-music-0.1.0.tar.gz` & `tmp/term-music-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-music-0.1.0.tar", last modified: Mon May 15 23:18:29 2023, max compression
+gzip compressed data, was "term-music-0.2.0.tar", last modified: Tue May 16 21:50:25 2023, max compression
```

## Comparing `term-music-0.1.0.tar` & `term-music-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-15 23:18:29.617248 term-music-0.1.0/
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1069 2023-05-14 21:24:42.000000 term-music-0.1.0/LICENCE.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)     3162 2023-05-15 23:18:29.617248 term-music-0.1.0/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2773 2023-05-14 21:21:49.000000 term-music-0.1.0/README.md
--rw-r--r--   0 ivan      (1000) ivan      (1000)      459 2023-05-15 23:10:54.000000 term-music-0.1.0/pyproject.toml
--rw-r--r--   0 ivan      (1000) ivan      (1000)      288 2023-05-15 23:18:29.617248 term-music-0.1.0/setup.cfg
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-15 23:18:29.613915 term-music-0.1.0/term_music/
--rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-05-15 00:04:01.000000 term-music-0.1.0/term_music/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     6668 2023-05-15 22:58:27.000000 term-music-0.1.0/term_music/app.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     2943 2023-05-15 00:07:53.000000 term-music-0.1.0/term_music/app_data.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1663 2023-05-15 23:06:01.000000 term-music-0.1.0/term_music/config.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-15 23:18:29.617248 term-music-0.1.0/term_music/domain/
--rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-02-17 22:36:57.000000 term-music-0.1.0/term_music/domain/__init__.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     6300 2023-05-15 00:07:53.000000 term-music-0.1.0/term_music/domain/music_library.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1733 2023-02-17 23:06:38.000000 term-music-0.1.0/term_music/domain/playlist.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      430 2023-04-03 21:42:19.000000 term-music-0.1.0/term_music/domain/song.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)      751 2023-05-14 23:50:48.000000 term-music-0.1.0/term_music/keyboard.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     5158 2023-05-15 22:58:58.000000 term-music-0.1.0/term_music/main.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     1603 2023-05-15 00:07:53.000000 term-music-0.1.0/term_music/player.py
--rw-r--r--   0 ivan      (1000) ivan      (1000)     3426 2023-05-14 21:41:14.000000 term-music-0.1.0/term_music/ui.py
-drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-15 23:18:29.617248 term-music-0.1.0/term_music.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)     3162 2023-05-15 23:18:29.000000 term-music-0.1.0/term_music.egg-info/PKG-INFO
--rw-r--r--   0 ivan      (1000) ivan      (1000)      538 2023-05-15 23:18:29.000000 term-music-0.1.0/term_music.egg-info/SOURCES.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2023-05-15 23:18:29.000000 term-music-0.1.0/term_music.egg-info/dependency_links.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       52 2023-05-15 23:18:29.000000 term-music-0.1.0/term_music.egg-info/entry_points.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       27 2023-05-15 23:18:29.000000 term-music-0.1.0/term_music.egg-info/requires.txt
--rw-r--r--   0 ivan      (1000) ivan      (1000)       11 2023-05-15 23:18:29.000000 term-music-0.1.0/term_music.egg-info/top_level.txt
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-16 21:50:25.776053 term-music-0.2.0/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1069 2023-05-14 21:24:42.000000 term-music-0.2.0/LICENCE.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     3162 2023-05-16 21:50:25.776053 term-music-0.2.0/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2773 2023-05-14 21:21:49.000000 term-music-0.2.0/README.md
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      459 2023-05-16 21:50:11.000000 term-music-0.2.0/pyproject.toml
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      288 2023-05-16 21:50:25.779386 term-music-0.2.0/setup.cfg
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-16 21:50:25.772719 term-music-0.2.0/term_music/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-05-15 00:04:01.000000 term-music-0.2.0/term_music/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     6618 2023-05-16 21:27:59.000000 term-music-0.2.0/term_music/app.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2943 2023-05-15 00:07:53.000000 term-music-0.2.0/term_music/app_data.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2151 2023-05-16 21:48:17.000000 term-music-0.2.0/term_music/commands.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1663 2023-05-15 23:06:01.000000 term-music-0.2.0/term_music/config.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-16 21:50:25.776053 term-music-0.2.0/term_music/domain/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        0 2023-02-17 22:36:57.000000 term-music-0.2.0/term_music/domain/__init__.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     6300 2023-05-15 00:07:53.000000 term-music-0.2.0/term_music/domain/music_library.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1733 2023-02-17 23:06:38.000000 term-music-0.2.0/term_music/domain/playlist.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      430 2023-04-03 21:42:19.000000 term-music-0.2.0/term_music/domain/song.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      751 2023-05-14 23:50:48.000000 term-music-0.2.0/term_music/keyboard.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     2995 2023-05-16 21:50:11.000000 term-music-0.2.0/term_music/main.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     1603 2023-05-15 00:07:53.000000 term-music-0.2.0/term_music/player.py
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     3426 2023-05-14 21:41:14.000000 term-music-0.2.0/term_music/ui.py
+drwxr-xr-x   0 ivan      (1000) ivan      (1000)        0 2023-05-16 21:50:25.776053 term-music-0.2.0/term_music.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)     3162 2023-05-16 21:50:25.000000 term-music-0.2.0/term_music.egg-info/PKG-INFO
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      561 2023-05-16 21:50:25.000000 term-music-0.2.0/term_music.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)        1 2023-05-16 21:50:25.000000 term-music-0.2.0/term_music.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       52 2023-05-16 21:50:25.000000 term-music-0.2.0/term_music.egg-info/entry_points.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       27 2023-05-16 21:50:25.000000 term-music-0.2.0/term_music.egg-info/requires.txt
+-rw-r--r--   0 ivan      (1000) ivan      (1000)       11 2023-05-16 21:50:25.000000 term-music-0.2.0/term_music.egg-info/top_level.txt
```

### Comparing `term-music-0.1.0/LICENCE.txt` & `term-music-0.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/PKG-INFO` & `term-music-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-music
-Version: 0.1.0
+Version: 0.2.0
 Summary: A music player for the terminal
 Author: tracksuitdev
 Project-URL: Homepage, https://github.com/tracksuitdev/term-music
 Project-URL: Source, https://github.com/tracksuitdev/term-music
 Keywords: terminal,music,player,library,youtube-dl
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `term-music-0.1.0/README.md` & `term-music-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music/app.py` & `term-music-0.2.0/term_music/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from threading import Thread
 from typing import Optional
 
 from blessed import Terminal
 from pygame import mixer
 
 from term_music.app_data import APP_DATA
-from term_music.config import KEYMAP, UI_SETTINGS
 from term_music.domain.music_library import MusicLibrary
 from term_music.domain.song import Song
 from term_music.keyboard import Keyboard
 from term_music.player import Player
 from term_music.ui import UserInterface
```

### Comparing `term-music-0.1.0/term_music/app_data.py` & `term-music-0.2.0/term_music/app_data.py`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music/config.py` & `term-music-0.2.0/term_music/config.py`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music/domain/music_library.py` & `term-music-0.2.0/term_music/domain/music_library.py`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music/domain/playlist.py` & `term-music-0.2.0/term_music/domain/playlist.py`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music/keyboard.py` & `term-music-0.2.0/term_music/keyboard.py`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music/player.py` & `term-music-0.2.0/term_music/player.py`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music/ui.py` & `term-music-0.2.0/term_music/ui.py`

 * *Files identical despite different names*

### Comparing `term-music-0.1.0/term_music.egg-info/PKG-INFO` & `term-music-0.2.0/term_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-music
-Version: 0.1.0
+Version: 0.2.0
 Summary: A music player for the terminal
 Author: tracksuitdev
 Project-URL: Homepage, https://github.com/tracksuitdev/term-music
 Project-URL: Source, https://github.com/tracksuitdev/term-music
 Keywords: terminal,music,player,library,youtube-dl
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `term-music-0.1.0/term_music.egg-info/SOURCES.txt` & `term-music-0.2.0/term_music.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENCE.txt
 README.md
 pyproject.toml
 setup.cfg
 term_music/__init__.py
 term_music/app.py
 term_music/app_data.py
+term_music/commands.py
 term_music/config.py
 term_music/keyboard.py
 term_music/main.py
 term_music/player.py
 term_music/ui.py
 term_music.egg-info/PKG-INFO
 term_music.egg-info/SOURCES.txt
```

