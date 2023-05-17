# Comparing `tmp/nonebot_plugin_multincm-0.2.4.tar.gz` & `tmp/nonebot_plugin_multincm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.2.4.tar", last modified: Tue May 16 20:52:06 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.2.5.tar", last modified: Wed May 17 19:27:49 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.2.4.tar` & `nonebot_plugin_multincm-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/LICENSE
--rw-r--r--   0        0        0     5832 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/README.md
--rw-r--r--   0        0        0     1172 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0     7323 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      512 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0     4562 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    10221 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2518 2023-05-16 20:51:46.545564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0   212591 2023-05-16 20:51:46.549564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     1688 2023-05-16 20:51:46.549564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-05-16 20:51:46.549564 nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      826 2023-05-16 20:52:06.377673 nonebot_plugin_multincm-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6733 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/LICENSE
+-rw-r--r--   0        0        0     6066 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/README.md
+-rw-r--r--   0        0        0     1248 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0     8572 2023-05-17 19:27:36.549958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      512 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     4457 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    10221 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2957 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2143 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     1688 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-05-17 19:27:36.553958 nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      867 2023-05-17 19:27:49.437802 nonebot_plugin_multincm-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7016 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.2.4/LICENSE` & `nonebot_plugin_multincm-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.4/README.md` & `nonebot_plugin_multincm-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,20 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.5
+
+- `解析`、`歌词`、`链接` 指令可以直接根据 Bot 发送的上个音乐卡片作出回应了
+- 歌词解析会合并多行空行和去掉首尾空行了
+- 现在插件会定时清理自身内存中的缓存了
+
 ### 0.2.4
 
 - 修复一个歌词解析 bug
 
 ### 0.2.3
 
 - 微调歌曲列表排版
```

#### html2text {}

```diff
@@ -51,12 +51,16 @@
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.4 - ä¿®å¤ä¸ä¸ªæ­è¯è§£æ
-bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç - å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 -
-ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 -
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
+åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
+ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
+ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
+å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from nonebot.plugin import PluginMetadata
+from nonebot.plugin import PluginMetadata, require
 
-from . import __main__ as __main__
-from .config import ConfigModel
+require("nonebot_plugin_apscheduler")
 
-__version__ = "0.2.4"
+from . import __main__ as __main__  # noqa: E402
+from .config import ConfigModel  # noqa: E402
+
+__version__ = "0.2.5"
 __plugin_meta__ = PluginMetadata(
     "MultiNCM",
     "网易云多选点歌",
     (
         "指令列表\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：顾名思义。当输入音乐 ID 时会直接发送对应音乐\n"
```

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-from pathlib import Path
 from typing import Any, Callable, Dict, List, cast
 
 import anyio
 from nonebot import get_available_plugin_names, logger, require
 from pyncm import (
     DumpSessionAsString,
     GetCurrentSession,
@@ -16,21 +15,18 @@
     LoginViaAnonymousAccount,
     LoginViaCellphone,
     LoginViaEmail,
 )
 from pyncm.apis.track import GetTrackAudio, GetTrackDetail, GetTrackLyrics
 
 from .config import config
+from .const import DATA_PATH
 from .types import LyricData, Privilege, Song, SongSearchResult, TrackAudio
 from .utils import awaitable
 
-DATA_PATH = Path().cwd() / "data" / "multincm"
-if not DATA_PATH.exists():
-    DATA_PATH.mkdir(parents=True)
-
 SESSION_FILE = DATA_PATH / "session.cache"
 
 
 async def ncm_request(api: Callable, *args, **kwargs) -> Dict[str, Any]:
     ret = await awaitable(api)(*args, **kwargs)
     if ret.get("code", 200) != 200:
         raise RuntimeError(f"请求 {api.__name__} 失败\n{ret}")
```

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/lrc_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 from dataclasses import dataclass
-from enum import Enum
 from typing import Callable, List, Optional, TypeVar
 
 T = TypeVar("T")
 
 
 @dataclass
 class LrcLine:
@@ -23,15 +22,19 @@
     for i in range(len(array) - 1, -1, -1):
         it = array[i]
         if predicate(it):
             return it
     return None
 
 
-def parse(lrc: str, ignore_empty: bool = False) -> List[LrcLine]:
+def parse(
+    lrc: str,
+    ignore_empty: bool = False,
+    merge_empty: bool = True,
+) -> List[LrcLine]:
     parsed = []
     for line in re.finditer(LRC_LINE_REGEX, lrc):
         lrc = line["lrc"].strip().replace("\u3000", " ")
         times = [x.groupdict() for x in re.finditer(LRC_TIME_REGEX, line[0])]
 
         parsed.extend(
             [
@@ -46,31 +49,48 @@
                 for i in times
             ],
         )
 
     if ignore_empty:
         parsed = [x for x in parsed if x.lrc]
 
+    elif merge_empty:
+        new_parsed = []
+
+        for line in parsed:
+            if line.lrc or (new_parsed and new_parsed[-1].lrc and (not line.lrc)):
+                new_parsed.append(line)
+
+        if new_parsed and (not new_parsed[-1].lrc):
+            new_parsed.pop()
+
+        parsed = new_parsed
+
     parsed.sort(key=lambda x: x.time)
     return parsed
 
 
-def merge(*lyrics: List[LrcLine], threshold: int = 20) -> List[List[LrcLine]]:
+def merge(
+    *lyrics: List[LrcLine],
+    threshold: int = 20,
+    replace_empty_line: Optional[str] = "--------",
+) -> List[List[LrcLine]]:
     lyrics = tuple(x.copy() for x in lyrics)
 
     for lrc in lyrics:
         while not lrc[-1].lrc:
             lrc.pop()
 
     main_lyric = lyrics[0]
     sub_lyrics = lyrics[1:]
 
-    for x in main_lyric:
-        if not x.lrc:
-            x.lrc = "--------"
+    if replace_empty_line:
+        for x in main_lyric:
+            if not x.lrc:
+                x.lrc = replace_empty_line
 
     merged: List[List[LrcLine]] = [[x] for x in main_lyric]
     for merged_line in merged:
         main_line = merged_line[0]
         main_time = main_line.time
 
         for sub_lrc in sub_lyrics:
```

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.4/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.2.5/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.4/pyproject.toml` & `nonebot_plugin_multincm-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.2.4"
+version = "0.2.5"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
     "pydantic>=1.10.4",
     "pil-utils>=0.1.7",
     "pyncm>=1.6.8.9.1",
     "typing-extensions>=4.5.0",
     "anyio>=3.6.2",
+    "nonebot-plugin-apscheduler>=0.2.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_multincm-0.2.4/PKG-INFO` & `nonebot_plugin_multincm-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.2.4
+Version: 0.2.5
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
 Requires-Dist: pydantic>=1.10.4
 Requires-Dist: pil-utils>=0.1.7
 Requires-Dist: pyncm>=1.6.8.9.1
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: anyio>=3.6.2
+Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
 Requires-Dist: pip>=23.0.1; extra == "dev"
 Requires-Dist: setuptools>=67.6.1; extra == "dev"
 Requires-Dist: nb-cli>=1.0.5; extra == "dev"
 Requires-Dist: black>=23.3.0; extra == "dev"
 Requires-Dist: ruff>=0.0.260; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
 Provides-Extra: dev
@@ -196,14 +197,20 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.5
+
+- `解析`、`歌词`、`链接` 指令可以直接根据 Bot 发送的上个音乐卡片作出回应了
+- 歌词解析会合并多行空行和去掉首尾空行了
+- 现在插件会定时清理自身内存中的缓存了
+
 ### 0.2.4
 
 - 修复一个歌词解析 bug
 
 ### 0.2.3
 
 - 微调歌曲列表排版
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.4 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.5 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
-anyio>=3.6.2 Requires-Dist: pip>=23.0.1; extra == "dev" Requires-Dist:
-setuptools>=67.6.1; extra == "dev" Requires-Dist: nb-cli>=1.0.5; extra == "dev"
-Requires-Dist: black>=23.3.0; extra == "dev" Requires-Dist: ruff>=0.0.260;
-extra == "dev" Requires-Dist: isort>=5.12.0; extra == "dev" Provides-Extra: dev
-Description-Content-Type: text/markdown
+anyio>=3.6.2 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0 Requires-Dist:
+pip>=23.0.1; extra == "dev" Requires-Dist: setuptools>=67.6.1; extra == "dev"
+Requires-Dist: nb-cli>=1.0.5; extra == "dev" Requires-Dist: black>=23.3.0;
+extra == "dev" Requires-Dist: ruff>=0.0.260; extra == "dev" Requires-Dist:
+isort>=5.12.0; extra == "dev" Provides-Extra: dev Description-Content-Type:
+text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-MultiNCM _â¨ NoneBot æä»¶ç®åæè¿° â¨_ [python] [pdm-
                              managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
@@ -64,12 +65,16 @@
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.4 - ä¿®å¤ä¸ä¸ªæ­è¯è§£æ
-bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç - å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 -
-ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.5 -
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot
+åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
+æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
+ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
+ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
+å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
 å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

