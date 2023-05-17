# Comparing `tmp/nonebot_plugin_rename-1.2.2.tar.gz` & `tmp/nonebot_plugin_rename-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.2.3.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.2.2.tar` & `nonebot_plugin_rename-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-05-17 04:29:53.316762 nonebot_plugin_rename-1.2.2/LICENSE
--rw-r--r--   0        0        0     5230 2023-05-17 04:29:53.316762 nonebot_plugin_rename-1.2.2/README.md
--rw-r--r--   0        0        0      363 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      293 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      789 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0     1020 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      408 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      607 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      604 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      338 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0     9234 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      187 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      838 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0      643 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/download.py
--rw-r--r--   0        0        0     1534 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      423 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      663 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6135 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-17 04:38:07.406701 nonebot_plugin_rename-1.2.3/LICENSE
+-rw-r--r--   0        0        0     5230 2023-05-17 04:38:07.406701 nonebot_plugin_rename-1.2.3/README.md
+-rw-r--r--   0        0        0      363 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      293 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      789 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0     1020 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      408 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      607 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      893 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/starrail_time.py
+-rw-r--r--   0        0        0      604 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      338 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0     9234 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      187 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      838 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0      643 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/download.py
+-rw-r--r--   0        0        0     1534 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      423 2023-05-17 04:38:07.438701 nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      663 2023-05-17 04:38:07.442701 nonebot_plugin_rename-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6135 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.2.2/LICENSE` & `nonebot_plugin_rename-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/README.md` & `nonebot_plugin_rename-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/genshin_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/one_word.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/one_word.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/download.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.2.3/nonebot_plugin_rename/utils/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.2/pyproject.toml` & `nonebot_plugin_rename-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.2.2"
+version = "1.2.3"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
 
 [[tool.poetry.source]]
```

### Comparing `nonebot_plugin_rename-1.2.2/PKG-INFO` & `nonebot_plugin_rename-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.2.2
+Version: 1.2.3
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.2.3 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
```

