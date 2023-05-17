# Comparing `tmp/nonebot_plugin_session-0.0.1.tar.gz` & `tmp/nonebot_plugin_session-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_session-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_session-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_session-0.0.1.tar` & `nonebot_plugin_session-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/LICENSE
--rw-r--r--   0        0        0     4183 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/README.md
--rw-r--r--   0        0        0      161 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/__init__.py
--rw-r--r--   0        0        0       65 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/__init__.py
--rw-r--r--   0        0        0      585 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/console.py
--rw-r--r--   0        0        0     1190 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/kaiheila.py
--rw-r--r--   0        0        0     2719 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3537 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/onebot_v12.py
--rw-r--r--   0        0        0     1421 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/qqguild.py
--rw-r--r--   0        0        0      346 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/const.py
--rw-r--r--   0        0        0     2700 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/extractor.py
--rw-r--r--   0        0        0     1525 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
--rw-r--r--   0        0        0     2793 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/model.py
--rw-r--r--   0        0        0     2155 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/saa.py
--rw-r--r--   0        0        0     2053 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/nonebot_plugin_session/session.py
--rw-r--r--   0        0        0     1618 2023-05-16 12:49:47.680011 nonebot_plugin_session-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5199 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4183 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/README.md
+-rw-r--r--   0        0        0      161 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/__init__.py
+-rw-r--r--   0        0        0      585 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/console.py
+-rw-r--r--   0        0        0     1190 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/kaiheila.py
+-rw-r--r--   0        0        0     2719 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3537 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     1421 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/qqguild.py
+-rw-r--r--   0        0        0      346 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/const.py
+-rw-r--r--   0        0        0     2700 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/extractor.py
+-rw-r--r--   0        0        0     1525 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
+-rw-r--r--   0        0        0     2793 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/model.py
+-rw-r--r--   0        0        0     2155 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/saa.py
+-rw-r--r--   0        0        0     2053 2023-05-16 13:15:35.271589 nonebot_plugin_session-0.0.2/nonebot_plugin_session/session.py
+-rw-r--r--   0        0        0     1772 2023-05-16 13:15:35.275589 nonebot_plugin_session-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_session-0.0.1/LICENSE` & `nonebot_plugin_session-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/README.md` & `nonebot_plugin_session-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
   <a href="https://v2.nonebot.dev/">
     <img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot">
   </a>
 
 # nonebot-plugin-session
 
-_✨ [Nonebot2](https://github.com/nonebot/nonebot2) 会话目标提取与会话 id 定义插件 ✨_
+_✨ [Nonebot2](https://github.com/nonebot/nonebot2) 会话信息提取与会话 id 定义插件 ✨_
 
 <p align="center">
   <img src="https://img.shields.io/github/license/noneplugin/nonebot-plugin-session" alt="license">
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">
   <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
   <a href="https://pypi.org/project/nonebot-plugin-session">
     <img src="https://badgen.net/pypi/v/nonebot-plugin-session" alt="pypi">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [nonebot] # nonebot-plugin-session _â¨ [Nonebot2](https://github.com/nonebot/
-          nonebot2) ä¼è¯ç®æ æåä¸ä¼è¯ id å®ä¹æä»¶ â¨_
+          nonebot2) ä¼è¯ä¿¡æ¯æåä¸ä¼è¯ id å®ä¹æä»¶ â¨_
                       [license] [Python] [NoneBot] [pypi]
 - è¿ä¸ªæä»¶å¯ä»¥åä»ä¹ï¼ æ¬æä»¶æä¾äºä¸ä¸ªç»ä¸çä¼è¯æ¨¡å
 `Session`ï¼ å¯ä»¥ä»ä¸åééå¨ç `Bot` å `Event`
 ä¸­æåä¸ä¼è¯ç¸å³ç
 âå¹³å°âãâä¼è¯ç­çº§âï¼åç¨æ·ãåçº§ç¾¤ç»ãä¸¤çº§ç¾¤ç»ï¼ãâç®æ 
 idâ ç­å±æ§ï¼ åæ¶æä¾äºè·åä¼è¯ id
 çå½æ°ï¼å¯ä»¥æç§ä¸åçç±»åè·åä¼è¯idï¼æ¹ä¾¿ä¸ååºæ¯ä¸çä½¿ç¨
```

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/console.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/kaiheila.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/onebot_v11.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/onebot_v12.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/adapters/qqguild.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/extractor.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/extractor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/migrations/36de70108aeb_init_db.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/migrations/36de70108aeb_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/model.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/saa.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/saa.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/nonebot_plugin_session/session.py` & `nonebot_plugin_session-0.0.2/nonebot_plugin_session/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.1/pyproject.toml` & `nonebot_plugin_session-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "nonebot_plugin_session"
-version = "0.0.1"
-description = "Nonebot2 会话目标提取与会话id定义"
+version = "0.0.2"
+description = "Nonebot2 会话信息提取与会话id定义"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-session"
 repository = "https://github.com/noneplugin/nonebot-plugin-session"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = { version = "^2.0.0-rc.1", extras = ["fastapi"] }
+strenum = "^0.4.8"
 nonebot-plugin-datastore = { version = "^0.6.3", optional = true }
 nonebot-plugin-send-anything-anywhere = { version = "^0.2.4", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 
 [tool.poetry.group.test.dependencies]
@@ -33,14 +34,16 @@
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_session"]
 adapters = [
   { name = "Console", module_name = "nonebot.adapters.console" },
   { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
   { name = "OneBot V12", module_name = "nonebot.adapters.onebot.v12" },
+  { name = "Kaiheila", module_name = "nonebot.adapters.kaiheila" },
+  { name = "QQ Guild", module_name = "nonebot.adapters.qqguild" },
 ]
 
 [tool.poetry.extras]
 datastore = ["nonebot-plugin-datastore"]
 saa = ["nonebot-plugin-send-anything-anywhere"]
 all = ["nonebot-plugin-datastore", "nonebot-plugin-send-anything-anywhere"]
```

### Comparing `nonebot_plugin_session-0.0.1/PKG-INFO` & `nonebot_plugin_session-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-session
-Version: 0.0.1
-Summary: Nonebot2 会话目标提取与会话id定义
+Version: 0.0.2
+Summary: Nonebot2 会话信息提取与会话id定义
 Home-page: https://github.com/noneplugin/nonebot-plugin-session
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,26 +15,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: datastore
 Provides-Extra: saa
 Requires-Dist: nonebot-plugin-datastore (>=0.6.3,<0.7.0) ; extra == "datastore" or extra == "all"
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4,<0.3.0) ; extra == "saa" or extra == "all"
 Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
+Requires-Dist: strenum (>=0.4.8,<0.5.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-session
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   <a href="https://v2.nonebot.dev/">
     <img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot">
   </a>
 
 # nonebot-plugin-session
 
-_✨ [Nonebot2](https://github.com/nonebot/nonebot2) 会话目标提取与会话 id 定义插件 ✨_
+_✨ [Nonebot2](https://github.com/nonebot/nonebot2) 会话信息提取与会话 id 定义插件 ✨_
 
 <p align="center">
   <img src="https://img.shields.io/github/license/noneplugin/nonebot-plugin-session" alt="license">
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">
   <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
   <a href="https://pypi.org/project/nonebot-plugin-session">
     <img src="https://badgen.net/pypi/v/nonebot-plugin-session" alt="pypi">
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.1 Summary:
-Nonebot2 ä¼è¯ç®æ æåä¸ä¼è¯idå®ä¹ Home-page: https://github.com/
+Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.2 Summary:
+Nonebot2 ä¼è¯ä¿¡æ¯æåä¸ä¼è¯idå®ä¹ Home-page: https://github.com/
 noneplugin/nonebot-plugin-session License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
 Provides-Extra: datastore Provides-Extra: saa Requires-Dist: nonebot-plugin-
 datastore (>=0.6.3,<0.7.0) ; extra == "datastore" or extra == "all" Requires-
 Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4,<0.3.0) ; extra == "saa"
 or extra == "all" Requires-Dist: nonebot2[fastapi] (>=2.0.0-rc.1,<3.0.0)
-Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-session
-Description-Content-Type: text/markdown
+Requires-Dist: strenum (>=0.4.8,<0.5.0) Project-URL: Repository, https://
+github.com/noneplugin/nonebot-plugin-session Description-Content-Type: text/
+markdown
 [nonebot] # nonebot-plugin-session _â¨ [Nonebot2](https://github.com/nonebot/
-          nonebot2) ä¼è¯ç®æ æåä¸ä¼è¯ id å®ä¹æä»¶ â¨_
+          nonebot2) ä¼è¯ä¿¡æ¯æåä¸ä¼è¯ id å®ä¹æä»¶ â¨_
                       [license] [Python] [NoneBot] [pypi]
 - è¿ä¸ªæä»¶å¯ä»¥åä»ä¹ï¼ æ¬æä»¶æä¾äºä¸ä¸ªç»ä¸çä¼è¯æ¨¡å
 `Session`ï¼ å¯ä»¥ä»ä¸åééå¨ç `Bot` å `Event`
 ä¸­æåä¸ä¼è¯ç¸å³ç
 âå¹³å°âãâä¼è¯ç­çº§âï¼åç¨æ·ãåçº§ç¾¤ç»ãä¸¤çº§ç¾¤ç»ï¼ãâç®æ 
 idâ ç­å±æ§ï¼ åæ¶æä¾äºè·åä¼è¯ id
 çå½æ°ï¼å¯ä»¥æç§ä¸åçç±»åè·åä¼è¯idï¼æ¹ä¾¿ä¸ååºæ¯ä¸çä½¿ç¨
```

