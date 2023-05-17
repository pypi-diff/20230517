# Comparing `tmp/nkust-ucl-k12-bot-2.9.1.tar.gz` & `tmp/nkust-ucl-k12-bot-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.9.1.tar", last modified: Mon May  8 04:28:38 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.9.2.tar", last modified: Wed May 17 11:42:18 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.9.1.tar` & `nkust-ucl-k12-bot-2.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.404140 nkust-ucl-k12-bot-2.9.1/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.9.1/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     6029 2023-05-08 04:28:38.403880 nkust-ucl-k12-bot-2.9.1/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5616 2023-05-08 04:28:10.000000 nkust-ucl-k12-bot-2.9.1/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.400763 nkust-ucl-k12-bot-2.9.1/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)    10758 2023-05-08 04:23:27.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.402503 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/config.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.403618 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     6029 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      407 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      744 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/requires.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-08 04:28:38.404207 nkust-ucl-k12-bot-2.9.1/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1880 2023-05-08 04:28:29.000000 nkust-ucl-k12-bot-2.9.1/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-17 11:42:18.635198 nkust-ucl-k12-bot-2.9.2/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.9.2/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     6029 2023-05-17 11:42:18.634994 nkust-ucl-k12-bot-2.9.2/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     5616 2023-05-08 04:28:10.000000 nkust-ucl-k12-bot-2.9.2/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-17 11:42:18.631791 nkust-ucl-k12-bot-2.9.2/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)    11066 2023-05-17 11:33:40.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-17 11:42:18.633468 nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/config.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-17 11:42:18.634638 nkust-ucl-k12-bot-2.9.2/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     6029 2023-05-17 11:42:18.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      407 2023-05-17 11:42:18.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-17 11:42:18.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       46 2023-05-17 11:42:18.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl_k12_bot.egg-info/requires.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-17 11:42:18.000000 nkust-ucl-k12-bot-2.9.2/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-17 11:42:18.635256 nkust-ucl-k12-bot-2.9.2/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      740 2023-05-17 11:41:52.000000 nkust-ucl-k12-bot-2.9.2/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.9.1/LICENSE` & `nkust-ucl-k12-bot-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.1/PKG-INFO` & `nkust-ucl-k12-bot-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.9.1
+Version: 2.9.2
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.9.1/README.md` & `nkust-ucl-k12-bot-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.1/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.9.2/nkust_ucl/k12.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class MsgType(Enum):
     TEXT = "Text"
     IMAGE = "Image"
     AUDIO = "audio"
     DOCUMENT = "Document"
     STICKER = "Sticker"
+    
 
 class BOT:
     # K12 class 的實現
     def __init__(self, config_file='config/k12.yaml') -> None:
         self.logger = setup_logger('chatbot')
 
         self.header = {
@@ -272,20 +273,26 @@
         """
         if msg_type not in MsgType.__members__.values():
             raise ValueError(f"Invalid message type '{msg_type}'")
         self.commands[(command, msg_type.value)] = func
 
     def handle_command(self, message: ChatMessage, *args, **kwargs):
         """
-        該函數會根據訊息類型與指令來呼叫對應的函數
+        TODO:
+        預計要實現的函數，如果非文字訊息，則透過其他方式來處理  
+
+        該函數會根據訊息類型與指令來呼叫對應的函數，目前只接受文字訊息，因為其他訊息類型的指令還沒有實現
         Message: ChatMessage
         *args: 額外的參數
         **kwargs: 額外的參數
         """
-        command = message.msg_body.split()[0]
-        msg_type = str(message.msg_type)
-        if msg_type not in MsgType._value2member_map_:
-            raise ValueError(f"Invalid message type '{msg_type}'")
-        if (command, msg_type) in self.commands:
-            return self.commands[(command, msg_type)](message, *args, **kwargs)
+        if message.msg_type == MsgType.TEXT:
+            command = message.msg_body.split()[0]
+            if message.msg_type not in MsgType._value2member_map_:
+                raise ValueError(f"Invalid message type '{message.msg_type}'")
+            if (command, message.msg_type) in self.commands:
+                return self.commands[(command, message.msg_type)](message, *args, **kwargs)
+            else:
+                return None
         else:
+            
             return None
```

### Comparing `nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.9.2/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.9.2/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.9.1
+Version: 2.9.2
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

