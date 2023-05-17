# Comparing `tmp/nonebot-plugin-msgbuf-0.1.0.tar.gz` & `tmp/nonebot-plugin-msgbuf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-msgbuf-0.1.0.tar", last modified: Fri May 12 17:24:02 2023, max compression
+gzip compressed data, was "nonebot-plugin-msgbuf-0.2.0.tar", last modified: Wed May 17 07:32:53 2023, max compression
```

## Comparing `nonebot-plugin-msgbuf-0.1.0.tar` & `nonebot-plugin-msgbuf-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:24:02.229600 nonebot-plugin-msgbuf-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 17:23:48.000000 nonebot-plugin-msgbuf-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-12 17:24:02.229600 nonebot-plugin-msgbuf-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-12 17:23:48.000000 nonebot-plugin-msgbuf-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:24:02.229600 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-12 17:23:48.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-12 17:23:48.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-12 17:23:48.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:24:02.229600 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-12 17:24:02.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-12 17:24:02.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:24:02.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 17:24:02.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 17:24:02.000000 nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-12 17:23:48.000000 nonebot-plugin-msgbuf-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:24:02.229600 nonebot-plugin-msgbuf-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:32:53.004829 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 07:32:53.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/setup.cfg
```

### Comparing `nonebot-plugin-msgbuf-0.1.0/LICENSE` & `nonebot-plugin-msgbuf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.1.0/PKG-INFO` & `nonebot-plugin-msgbuf-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-msgbuf
-Version: 0.1.0
-Summary: 适用于 NoneBot2 插件的被动消息构造集成
-Author-email: HivertMoZara <worldmozara@163.com>
-License: MIT
-Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
-Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 # nonebot-plugin-msgbuf
 
 _✨ 适用于 NoneBot2 插件的被动消息构造集成 ✨_
 
 ~~代码比 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 和 [SegBuilder](https://github.com/Well2333/nonebot-plugin-segbuilder) 好看（不是）~~
@@ -46,67 +34,79 @@
 |  🟨  | 部分支持，需要用户额外分平台处理 |
 |  ❌  | 不支持，发送时自动转化为后备文本 |
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
+|                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
 nb plugin install nonebot-plugin-msgbuf
 ```
 
 ## 使用
 
+> 关于 `require()` 的使用问题：
+>
+> NoneBot2 插件的**首次**导入**必须**通过 NoneBot2 自身的方式（包括但不限于 `require()`, `load_plugin()` 等）完成，否则之后使用 NoneBot2 方式导入该插件的插件将**无法**正常工作。
+>
+> NoneBot2 插件体系要求**必须**使用 `require()` 加载插件依赖。
+
+### 竞品对比
+
 这是常规的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
 
 ```python
 from nonebot import on_message
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pathlib import Path
 
 ma = on_message()
 
 @ma.handle()
 async def test():
-    await ma.send(MessageSegment.image(Path("image.png")) + "")
+    await ma.send(MessageSegment.image(Path("image.png")) + "Hello world!")
 ```
 
 </details>
 
-***
+---
 
 这是 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
 
 ```python
-from nonebot import on_message
+from nonebot import on_message, require
 from pathlib import Path
+
+require("nonebot_plugin_saa")
+
 from nonebot_plugin_saa import MessageFactory, Text, Image
 
 ma = on_message()
 
 @ma.handle()
 async def test():
     await MessageFactory([Image(Path("image.png")), Text("Hello world!")]).send()
 ```
 
 </details>
 
-***
+---
 
 这是 [SegBuilder](https://github.com/Well2333/nonebot-plugin-segbuilder) 的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
 
 ```python
@@ -122,22 +122,24 @@
 @ma.handle()
 async def test():
     await ma.send(SegmentBuilder.image(Path("image.png")) + "Hello world!")
 ```
 
 </details>
 
-***
+---
 
 这是 MsgBuf 的消息构造与发送方法：
 
 ```python
-from nonebot import on_message
+from nonebot import on_message, require
 from pathlib import Path
 
+require("nonebot_plugin_msgbuf")
+
 from nonebot_plugin_msgbuf import MsgBuf
 
 ma = on_message()
 
 @ma.handle()
 async def test():
     async with MsgBuf() as mb:
@@ -162,7 +164,19 @@
 ```
 
 ```python
 @ma.handle()
 async def test():
     await MsgBuf().image(Path("image.png")).text("Hello world!").send()
 ```
+
+### 使用 Go-CQHTTP 拓展
+
+```python
+from nonebot_plugin_msgbuf import Specs
+from pathlib import Path
+
+@ma.handle()
+async def test():
+    async with MsgBuf(specs=Specs.OB11_GOCQHTTP) as mb:
+        mb.image(Path("image.png")).text("Hello world!").file(Path("image.png"))
+```
```

### Comparing `nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf/__init__.py` & `nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,51 @@
 import asyncio
 from collections import deque
 from types import TracebackType
 from typing import (
     Any,        Deque,      Generic,    List,       Optional,   Type,
-    Union, cast
+    Union,      cast
 )
-from nonebot import logger
+from nonebot import logger, __version__ as nbver
 from nonebot.adapters import MessageSegment
 from nonebot.exception import ActionFailed
 from nonebot.matcher import current_bot, current_event
+from nonebot.plugin import PluginMetadata
 
 from .models import (
     Face,               File,               Image,              Location,
     Mention,            Model,              Raw,                Reply,
     Share,              SupportedFileData,  Text,               Video,
     Voice
 )
 from .platforms import _BotT, _EventT, Specs, find_proxy
 
+_extra_meta_source = {
+    "type": "library",
+    "homepage": "https://github.com/NCBM/nonebot-plugin-msgbuf"
+}
+
+if (
+    not nbver
+    or not nbver.startswith("2.0.0")
+    or not (_suf := nbver[5:])
+    or _suf[0] not in "abr"
+    or (_suf.startswith("rc") and int(_suf[2:]) > 4)
+):
+    _extra_meta = _extra_meta_source
+else:
+    _extra_meta = {"extra": _extra_meta_source}
+
+__plugin_meta__ = PluginMetadata(
+    name="信鸽巴夫",
+    description="适用于 NoneBot2 插件的被动消息构造集成",
+    usage="无",
+    **_extra_meta
+)
+
 
 class MessageBuffer(Generic[_BotT, _EventT]):
     """消息构造器"""
 
     def __init__(
         self,
         bot: Optional[_BotT] = None,
@@ -94,20 +118,20 @@
         return self
 
     def add(self, *m: Model):
         """批量插入消息结构"""
         self.msgbuf.extend(m)
         return self
     
-    def export(
+    async def export(
         self, convert: bool = False
     ) -> Union[List[MessageSegment], List[Model], List[str]]:
         if convert:
-            return list(
-                self.proxy.convert(s) for s in self.msgbuf
+            return await asyncio.gather(
+                *(self.proxy.convert(s) for s in self.msgbuf)
             )
         return list(self.msgbuf)
 
     def revert(self, n: int = 1):
         """
         从末尾删除消息结构
```

### Comparing `nonebot-plugin-msgbuf-0.1.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO` & `nonebot-plugin-msgbuf-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.1.0
+Version: 0.2.0
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -46,67 +46,79 @@
 |  🟨  | 部分支持，需要用户额外分平台处理 |
 |  ❌  | 不支持，发送时自动转化为后备文本 |
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
+|                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
 nb plugin install nonebot-plugin-msgbuf
 ```
 
 ## 使用
 
+> 关于 `require()` 的使用问题：
+>
+> NoneBot2 插件的**首次**导入**必须**通过 NoneBot2 自身的方式（包括但不限于 `require()`, `load_plugin()` 等）完成，否则之后使用 NoneBot2 方式导入该插件的插件将**无法**正常工作。
+>
+> NoneBot2 插件体系要求**必须**使用 `require()` 加载插件依赖。
+
+### 竞品对比
+
 这是常规的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
 
 ```python
 from nonebot import on_message
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pathlib import Path
 
 ma = on_message()
 
 @ma.handle()
 async def test():
-    await ma.send(MessageSegment.image(Path("image.png")) + "")
+    await ma.send(MessageSegment.image(Path("image.png")) + "Hello world!")
 ```
 
 </details>
 
-***
+---
 
 这是 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
 
 ```python
-from nonebot import on_message
+from nonebot import on_message, require
 from pathlib import Path
+
+require("nonebot_plugin_saa")
+
 from nonebot_plugin_saa import MessageFactory, Text, Image
 
 ma = on_message()
 
 @ma.handle()
 async def test():
     await MessageFactory([Image(Path("image.png")), Text("Hello world!")]).send()
 ```
 
 </details>
 
-***
+---
 
 这是 [SegBuilder](https://github.com/Well2333/nonebot-plugin-segbuilder) 的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
 
 ```python
@@ -122,22 +134,24 @@
 @ma.handle()
 async def test():
     await ma.send(SegmentBuilder.image(Path("image.png")) + "Hello world!")
 ```
 
 </details>
 
-***
+---
 
 这是 MsgBuf 的消息构造与发送方法：
 
 ```python
-from nonebot import on_message
+from nonebot import on_message, require
 from pathlib import Path
 
+require("nonebot_plugin_msgbuf")
+
 from nonebot_plugin_msgbuf import MsgBuf
 
 ma = on_message()
 
 @ma.handle()
 async def test():
     async with MsgBuf() as mb:
@@ -162,7 +176,19 @@
 ```
 
 ```python
 @ma.handle()
 async def test():
     await MsgBuf().image(Path("image.png")).text("Hello world!").send()
 ```
+
+### 使用 Go-CQHTTP 拓展
+
+```python
+from nonebot_plugin_msgbuf import Specs
+from pathlib import Path
+
+@ma.handle()
+async def test():
+    async with MsgBuf(specs=Specs.OB11_GOCQHTTP) as mb:
+        mb.image(Path("image.png")).text("Hello world!").file(Path("image.png"))
+```
```

