# Comparing `tmp/nonebot_plugin_bilichat-2.0.1.tar.gz` & `tmp/nonebot_plugin_bilichat-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.0.1.tar", last modified: Sat May 13 07:16:46 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.0.2.tar", last modified: Wed May 17 03:49:46 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.0.1.tar` & `nonebot_plugin_bilichat-2.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-05-13 07:16:37.147339 nonebot_plugin_bilichat-2.0.1/LICENSE
--rw-r--r--   0        0        0    11827 2023-05-13 07:16:37.147339 nonebot_plugin_bilichat-2.0.1/README.md
--rw-r--r--   0        0        0     7854 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-05-13 07:16:37.155339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-05-13 07:16:37.159339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-05-13 07:16:37.159339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-05-13 07:16:37.159339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-05-13 07:16:37.159339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-05-13 07:16:37.159339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-05-13 07:16:37.159339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-05-13 07:16:37.159339 nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1447 2023-05-13 07:16:46.843274 nonebot_plugin_bilichat-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    13164 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-17 03:49:36.881691 nonebot_plugin_bilichat-2.0.2/LICENSE
+-rw-r--r--   0        0        0    11827 2023-05-17 03:49:36.881691 nonebot_plugin_bilichat-2.0.2/README.md
+-rw-r--r--   0        0        0     7999 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4805 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-05-17 03:49:36.885691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-05-17 03:49:36.889691 nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1447 2023-05-17 03:49:46.589766 nonebot_plugin_bilichat-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13164 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.0.1/LICENSE` & `nonebot_plugin_bilichat-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/README.md` & `nonebot_plugin_bilichat-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,28 +64,33 @@
         "version": __version__,
         "priority": 1,
     },
 )
 
 
 async def _bili_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
-    if str(event.get_user_id()) == str(bot.self_id):
-        return plugin_config.bilichat_enable_self
-    elif isinstance(event, (V11_PME, V12_PME, Mirai_PME)):
+    # check if self msg
+    if str(event.get_user_id()) == str(bot.self_id) and not plugin_config.bilichat_enable_self:
+        return False
+    # private msg use user id
+    if isinstance(event, (V11_PME, V12_PME, Mirai_PME)):
         state["_uid_"] = event.get_user_id()
         return plugin_config.bilichat_enable_private
+    # group msg use group id
     elif isinstance(event, (V11_GME, V12_GME)):
         state["_uid_"] = event.group_id
         return plugin_config.verify_permission(event.group_id)
     elif isinstance(event, Mirai_GME):
         state["_uid_"] = event.sender.group.id
         return plugin_config.verify_permission(event.sender.group.id)
+    # channel like msg use channel id
     elif isinstance(event, (V12_CME, QG_ME)):
         state["_uid_"] = event.channel_id
         return plugin_config.bilichat_enable_channel
+    # other
     else:
         state["_uid_"] = "unkown"
         return plugin_config.bilichat_enable_unkown_src
 
 
 bili = on_regex(
     r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})",
```

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.0.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.0.1/pyproject.toml` & `nonebot_plugin_bilichat-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.0.1"
+version = "2.0.2"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-2.0.1/PKG-INFO` & `nonebot_plugin_bilichat-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.0.1
+Version: 2.0.2
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.0.2 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot-plugin-
```

