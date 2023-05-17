# Comparing `tmp/seaplayer-0.3.4.tar.gz` & `tmp/seaplayer-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.3.4.tar", max compression
+gzip compressed data, was "seaplayer-0.3.5.tar", max compression
```

## Comparing `seaplayer-0.3.4.tar` & `seaplayer-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1085 2023-04-25 14:05:19.406661 seaplayer-0.3.4/LICENSE
--rw-r--r--   0        0        0      995 2023-05-17 19:21:47.243599 seaplayer-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      957 2023-05-10 21:29:14.599641 seaplayer-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-05-02 23:42:08.763410 seaplayer-0.3.4/seaplayer/__init__.py
--rw-r--r--   0        0        0      295 2023-05-17 19:11:05.795693 seaplayer-0.3.4/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-10 21:24:30.252393 seaplayer-0.3.4/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0     5596 2023-05-16 23:08:28.381945 seaplayer-0.3.4/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-03 15:09:20.919585 seaplayer-0.3.4/seaplayer/css/configurate.css
--rw-r--r--   0        0        0      979 2023-05-05 21:48:10.082210 seaplayer-0.3.4/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-03 14:02:48.505884 seaplayer-0.3.4/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-02 23:29:23.509840 seaplayer-0.3.4/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      374 2023-05-10 16:57:45.981727 seaplayer-0.3.4/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1496 2023-05-16 23:20:22.149932 seaplayer-0.3.4/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-02 22:35:56.414811 seaplayer-0.3.4/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-12 20:40:27.939248 seaplayer-0.3.4/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0    11693 2023-05-10 21:20:05.638838 seaplayer-0.3.4/seaplayer/objects.py
--rw-r--r--   0        0        0     5980 2023-05-10 19:09:06.370823 seaplayer-0.3.4/seaplayer/screens.py
--rw-r--r--   0        0        0    15442 2023-05-17 19:16:29.372687 seaplayer-0.3.4/seaplayer/seaplayer.py
--rw-r--r--   0        0        0     4863 2023-05-16 23:18:30.476622 seaplayer-0.3.4/seaplayer/types.py
--rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 seaplayer-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-25 14:05:19.406661 seaplayer-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1020 2023-05-17 20:13:36.652207 seaplayer-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1117 2023-05-17 19:33:47.703429 seaplayer-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:42:08.763410 seaplayer-0.3.5/seaplayer/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-17 19:11:05.795693 seaplayer-0.3.5/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-10 21:24:30.252393 seaplayer-0.3.5/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0     5596 2023-05-16 23:08:28.381945 seaplayer-0.3.5/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:09:20.919585 seaplayer-0.3.5/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0      979 2023-05-05 21:48:10.082210 seaplayer-0.3.5/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-03 14:02:48.505884 seaplayer-0.3.5/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-02 23:29:23.509840 seaplayer-0.3.5/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      374 2023-05-10 16:57:45.981727 seaplayer-0.3.5/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1496 2023-05-16 23:20:22.149932 seaplayer-0.3.5/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-02 22:35:56.414811 seaplayer-0.3.5/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-12 20:40:27.939248 seaplayer-0.3.5/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0    12292 2023-05-17 20:11:39.578820 seaplayer-0.3.5/seaplayer/objects.py
+-rw-r--r--   0        0        0     5980 2023-05-10 19:09:06.370823 seaplayer-0.3.5/seaplayer/screens.py
+-rw-r--r--   0        0        0    15442 2023-05-17 20:13:24.781253 seaplayer-0.3.5/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0     4863 2023-05-16 23:18:30.476622 seaplayer-0.3.5/seaplayer/types.py
+-rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 seaplayer-0.3.5/PKG-INFO
```

### Comparing `seaplayer-0.3.4/LICENSE` & `seaplayer-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/pyproject.toml` & `seaplayer-0.3.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.3.4"
+version = "0.3.5"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "seaplayer" }]
@@ -26,12 +26,13 @@
 rich = ">=13.3.5"
 mutagen = "1.45.1"
 textual = ">=0.24.1"
 playsoundsimple-py = "0.6.3"
 properties-py = "1.1.0"
 typing-inspect = "^0.8.0"
 ripix = ">=2.2.3"
+platformdirs = "^3.5.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seaplayer-0.3.4/seaplayer/assets/image-not-found.png` & `seaplayer-0.3.5/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/seaplayer/config.py` & `seaplayer-0.3.5/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/seaplayer/css/objects.css` & `seaplayer-0.3.5/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/seaplayer/css/seaplayer.css` & `seaplayer-0.3.5/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/seaplayer/functions.py` & `seaplayer-0.3.5/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/seaplayer/modules/colorizer.py` & `seaplayer-0.3.5/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/seaplayer/objects.py` & `seaplayer-0.3.5/seaplayer/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 from PIL import Image
-from playsoundsimple import Sound
+# > Sound Works
+try:
+    from playsoundsimple import Sound
+    SOUND_IMPORTED = True
+except:
+    SOUND_IMPORTED = False
 # > Graphics
 from PIL.Image import Resampling
 from ripix import AsyncPixels, Pixels
 from rich.progress import Progress, BarColumn, TextColumn
 from textual.widgets import Static, Label, ListItem, ListView, Input
 # > Typing
 from typing import Optional, Tuple, TypeVar, Union
@@ -11,137 +16,138 @@
 from .types import *
 from .functions import *
 
 # ! Types
 T = TypeVar('T')
 
 # ! Music List
-class MusicListViewItem(ListItem):
-    def __init__(
-        self,
-        title: str="",
-        first_subtitle: str="",
-        second_subtitle: str="",
-        sound_uuid: Optional[str]=None
-    ) -> None:
-        super().__init__(classes="music-list-view-item")
-        self.title_label = Label(title, classes="music-list-view-item-title-label")
-        self.first_subtitle_label = Label(f" {first_subtitle}", classes="music-list-view-item-subtitle-label")
-        self.second_subtitle_label = Label(f" {second_subtitle}", classes="music-list-view-item-subtitle-label")
-        self.sound_uuid = sound_uuid
-        
-        self.compose_add_child(self.title_label)
-        self.compose_add_child(self.first_subtitle_label)
-        self.compose_add_child(self.second_subtitle_label)
-    
-    async def update_labels(
-        self,
-        title: Optional[str]=None,
-        first_subtitle: Optional[str]=None,
-        second_subtitle: Optional[str]=None,
-    ) -> None:
-        if title is not None: self.title_label.update(title)
-        if first_subtitle is not None: self.first_subtitle_label.update(title)
-        if second_subtitle is not None: self.second_subtitle_label.update(title)
+if SOUND_IMPORTED:
+    class MusicListViewItem(ListItem):
+        def __init__(
+            self,
+            title: str="",
+            first_subtitle: str="",
+            second_subtitle: str="",
+            sound_uuid: Optional[str]=None
+        ) -> None:
+            super().__init__(classes="music-list-view-item")
+            self.title_label = Label(title, classes="music-list-view-item-title-label")
+            self.first_subtitle_label = Label(f" {first_subtitle}", classes="music-list-view-item-subtitle-label")
+            self.second_subtitle_label = Label(f" {second_subtitle}", classes="music-list-view-item-subtitle-label")
+            self.sound_uuid = sound_uuid
+            
+            self.compose_add_child(self.title_label)
+            self.compose_add_child(self.first_subtitle_label)
+            self.compose_add_child(self.second_subtitle_label)
+        
+        async def update_labels(
+            self,
+            title: Optional[str]=None,
+            first_subtitle: Optional[str]=None,
+            second_subtitle: Optional[str]=None,
+        ) -> None:
+            if title is not None: self.title_label.update(title)
+            if first_subtitle is not None: self.first_subtitle_label.update(title)
+            if second_subtitle is not None: self.second_subtitle_label.update(title)
 
-class MusicListView(ListView):
-    def __init__(self, **kwargs) -> None:
-        kwargs["classes"] = "music-list-view"
-        super().__init__(**kwargs)
-        self.music_list: MusicList = MusicList()
-    
-    def add_sound(self, sound: Sound) -> str:
-        sound_uuid = self.music_list.add(sound)
-        self.append(
-            MusicListViewItem(
-                f"{get_sound_basename(sound)}",
-                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps".format(
-                    duration=round(sound.duration),
-                    channel_mode="Mono" if sound.channels <= 1 else "Stereo",
-                    samplerate=round(sound.samplerate),
-                    bitrate=round(sound.bitrate / 1000)
-                ),
-                os.path.abspath(sound.name),
-                sound_uuid
-            )
-        )
-        return sound_uuid
-    
-    def get_sound(self, sound_uuid: str) -> Optional[Sound]: return self.music_list.get(sound_uuid)
-    
-    async def aio_add_sound(self, sound: Sound):
-        sound_uuid = await self.music_list.aio_add(sound)
-        await self.append(
-            MusicListViewItem(
-                f"{get_sound_basename(sound)}",
-                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps".format(
-                    duration=round(sound.duration),
-                    channel_mode="Mono" if sound.channels <= 1 else "Stereo",
-                    samplerate=round(sound.samplerate),
-                    bitrate=round(sound.bitrate / 1000)
-                ),
-                os.path.abspath(sound.name),
-                sound_uuid
+    class MusicListView(ListView):
+        def __init__(self, **kwargs) -> None:
+            kwargs["classes"] = "music-list-view"
+            super().__init__(**kwargs)
+            self.music_list: MusicList = MusicList()
+        
+        def add_sound(self, sound: Sound) -> str:
+            sound_uuid = self.music_list.add(sound)
+            self.append(
+                MusicListViewItem(
+                    f"{get_sound_basename(sound)}",
+                    "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps".format(
+                        duration=round(sound.duration),
+                        channel_mode="Mono" if sound.channels <= 1 else "Stereo",
+                        samplerate=round(sound.samplerate),
+                        bitrate=round(sound.bitrate / 1000)
+                    ),
+                    os.path.abspath(sound.name),
+                    sound_uuid
+                )
             )
-        )
-        return sound_uuid
-    
-    def get_items_count(self) -> int: return len(self.children)
-    def exists_item_index(self, index: int) -> bool: return 0 >= index < self.get_items_count()
-    def get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
-        item: MusicListViewItem
-        for idx, item in enumerate(self.children):
-            if item.sound_uuid == sound_uuid:
-                return idx
-    
-    def get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
-        try: return self.children[index]
-        except:
-            try: return self.children[0]
-            except: pass
-    
-    def get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
-        if (index:=self.get_item_index_from_sound_uuid(sound_uuid)) is not None:
-            if (mli:=self.get_item_from_index(index+1)) is not None:
-                return mli.sound_uuid
-    
-    def select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
-        try:
-            super()._on_list_item__child_clicked(
-                ListItem._ChildClicked(
-                    self.children[self.get_item_index_from_sound_uuid(sound_uuid)]
+            return sound_uuid
+        
+        def get_sound(self, sound_uuid: str) -> Optional[Sound]: return self.music_list.get(sound_uuid)
+        
+        async def aio_add_sound(self, sound: Sound):
+            sound_uuid = await self.music_list.aio_add(sound)
+            await self.append(
+                MusicListViewItem(
+                    f"{get_sound_basename(sound)}",
+                    "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps".format(
+                        duration=round(sound.duration),
+                        channel_mode="Mono" if sound.channels <= 1 else "Stereo",
+                        samplerate=round(sound.samplerate),
+                        bitrate=round(sound.bitrate / 1000)
+                    ),
+                    os.path.abspath(sound.name),
+                    sound_uuid
                 )
             )
-        except: pass
-    
-    async def aio_get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
-        try: return self.children[index]
-        except:
-            try: return self.children[0]
+            return sound_uuid
+        
+        def get_items_count(self) -> int: return len(self.children)
+        def exists_item_index(self, index: int) -> bool: return 0 >= index < self.get_items_count()
+        def get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
+            item: MusicListViewItem
+            for idx, item in enumerate(self.children):
+                if item.sound_uuid == sound_uuid:
+                    return idx
+        
+        def get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
+            try: return self.children[index]
+            except:
+                try: return self.children[0]
+                except: pass
+        
+        def get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
+            if (index:=self.get_item_index_from_sound_uuid(sound_uuid)) is not None:
+                if (mli:=self.get_item_from_index(index+1)) is not None:
+                    return mli.sound_uuid
+        
+        def select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
+            try:
+                super()._on_list_item__child_clicked(
+                    ListItem._ChildClicked(
+                        self.children[self.get_item_index_from_sound_uuid(sound_uuid)]
+                    )
+                )
             except: pass
-    
-    async def aio_get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
-        item: MusicListViewItem
-        async for idx, item in aiter(enumerate(self.children)):
-            if item.sound_uuid == sound_uuid:
-                return idx
-    
-    async def aio_get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
-        if (index:=await self.aio_get_item_index_from_sound_uuid(sound_uuid)) is not None:
-            if (mli:=await self.aio_get_item_from_index(index+1)) is not None:
-                return mli.sound_uuid
-    
-    async def aio_select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
-        try:
-            super()._on_list_item__child_clicked(
-                ListItem._ChildClicked(
-                    self.children[await self.aio_get_item_index_from_sound_uuid(sound_uuid)]
+        
+        async def aio_get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
+            try: return self.children[index]
+            except:
+                try: return self.children[0]
+                except: pass
+        
+        async def aio_get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
+            item: MusicListViewItem
+            async for idx, item in aiter(enumerate(self.children)):
+                if item.sound_uuid == sound_uuid:
+                    return idx
+        
+        async def aio_get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
+            if (index:=await self.aio_get_item_index_from_sound_uuid(sound_uuid)) is not None:
+                if (mli:=await self.aio_get_item_from_index(index+1)) is not None:
+                    return mli.sound_uuid
+        
+        async def aio_select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
+            try:
+                super()._on_list_item__child_clicked(
+                    ListItem._ChildClicked(
+                        self.children[await self.aio_get_item_index_from_sound_uuid(sound_uuid)]
+                    )
                 )
-            )
-        except: pass
+            except: pass
 
 # ! ProgressBar
 class IndeterminateProgress(Static):
     def __init__(self, getfunc=get_bar_status, fps: int=15):
         super().__init__("", classes="indeterminate-progress-bar")
         self._bar = Progress(BarColumn(), TextColumn("{task.description}"))
         self._task_id = self._bar.add_task("", total=None)
```

### Comparing `seaplayer-0.3.4/seaplayer/screens.py` & `seaplayer-0.3.5/seaplayer/screens.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/seaplayer/seaplayer.py` & `seaplayer-0.3.5/seaplayer/seaplayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # > Local Imports
 from .objects import *
 from .config import *
 from .screens import Unknown, UNKNOWN_OPEN_KEY, Configurate
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.3.4/seaplayer/types.py` & `seaplayer-0.3.5/seaplayer/types.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.3.4/PKG-INFO` & `seaplayer-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.3.4
+Version: 0.3.5
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -12,35 +12,46 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: mutagen (==1.45.1)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
 Requires-Dist: playsoundsimple-py (==0.6.3)
 Requires-Dist: properties-py (==1.1.0)
 Requires-Dist: rich (>=13.3.5)
 Requires-Dist: ripix (>=2.2.3)
 Requires-Dist: textual (>=0.24.1)
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/romanin-rf/SeaPlayer
 Description-Content-Type: text/markdown
 
 # SeaPlayer
 ## Descriptions
 SeaPlayer is a player that works in the terminal. Works with `MP3`, `OGG`, `WAV`, `MIDI` files.
 
-## Install 
-You can use [Release](https://github.com/romanin-rf/sea-player/releases) or ***download clone repository*** install the dependencies from `requirements.txt` and run via [Python](https://www.python.org).
+## Install
+
+
+1. You can use [Release](https://github.com/romanin-rf/sea-player/releases)
+2. ***Download clone repository*** install the dependencies from `requirements.txt` and run via [Python](https://www.python.org).
+3.  ```
+    pip install --upgrade seaplayer
+    ```
 
 ### For MIDI playback
 ***If you have Windows*** you can skip this part as ***Windows*** has a default decoder for `MIDI` and ***does not need to be installed***.
 
 
 ***For Linux or MacOS users:***
 
 You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
 
 ## Using
+```shell
+python -m seaplayer # Method for `downloaded repository` or `installed via pip`
+```
+
 ![MainScreen-v0.3.4-unrelease.1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/80b1cf95-7801-4fdd-9336-4d566804735a)
 ![ConfigurateScreen-v0.3.4-unrelease.1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/79ca17ad-d4af-4cc6-84d7-9329855746e9)
```

