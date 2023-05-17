# Comparing `tmp/pymino-1.1.7.5.tar.gz` & `tmp/pymino-1.1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\submit v2\pymino-1.1.7.4\dist\.tmp-w_q_2xun\pymino-1.1.7.5.tar", last modified: Fri May  5 19:28:17 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.5\dist\.tmp-_m8_kqrb\pymino-1.1.7.6.tar", last modified: Wed May 17 03:25:30 2023, max compression
```

## Comparing `pymino-1.1.7.5.tar` & `pymino-1.1.7.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.030415 pymino-1.1.7.5/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.5/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-05-05 19:28:17.030415 pymino-1.1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 19:28:16.985278 pymino-1.1.7.5/pymino/
--rw-rw-rw-   0        0        0      676 2023-05-05 19:27:51.000000 pymino-1.1.7.5/pymino/__init__.py
--rw-rw-rw-   0        0        0    26133 2023-04-03 18:49:59.000000 pymino-1.1.7.5/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.5/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.011566 pymino-1.1.7.5/pymino/ext/
--rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.5/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.5/pymino/ext/account.py
--rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.5/pymino/ext/community.py
--rw-rw-rw-   0        0        0    39581 2023-05-05 19:27:29.000000 pymino-1.1.7.5/pymino/ext/context.py
--rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.5/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.024462 pymino-1.1.7.5/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.5/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.5/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14506 2023-03-10 06:04:42.000000 pymino-1.1.7.5/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    48713 2023-02-25 04:12:35.000000 pymino-1.1.7.5/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     2536 2023-03-03 22:30:34.000000 pymino-1.1.7.5/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    42816 2023-02-06 10:45:41.000000 pymino-1.1.7.5/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.5/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.5/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2230 2023-03-05 23:07:39.000000 pymino-1.1.7.5/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0     7414 2023-03-03 22:30:22.000000 pymino-1.1.7.5/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.029422 pymino-1.1.7.5/pymino/ext/utilities/
--rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.5/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.5/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.5/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.5/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.003630 pymino-1.1.7.5/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-05-05 19:28:17.033886 pymino-1.1.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:25:30.688195 pymino-1.1.7.6/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.6/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-05-17 03:25:30.688691 pymino-1.1.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 03:25:30.650499 pymino-1.1.7.6/pymino/
+-rw-rw-rw-   0        0        0      676 2023-05-17 03:04:23.000000 pymino-1.1.7.6/pymino/__init__.py
+-rw-rw-rw-   0        0        0    26133 2023-04-03 18:49:59.000000 pymino-1.1.7.6/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.6/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:25:30.670339 pymino-1.1.7.6/pymino/ext/
+-rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.6/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.6/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.6/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    44985 2023-05-17 03:16:26.000000 pymino-1.1.7.6/pymino/ext/context.py
+-rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.6/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:25:30.682739 pymino-1.1.7.6/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.6/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.6/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14506 2023-05-17 03:04:03.000000 pymino-1.1.7.6/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    49421 2023-05-17 03:04:26.000000 pymino-1.1.7.6/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     2536 2023-03-03 22:30:34.000000 pymino-1.1.7.6/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.7.6/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.6/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.6/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.7.6/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.7.6/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:25:30.687203 pymino-1.1.7.6/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.6/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.6/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.6/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.6/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:25:30.660916 pymino-1.1.7.6/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-17 03:25:30.000000 pymino-1.1.7.6/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-17 03:25:30.000000 pymino-1.1.7.6/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 03:25:30.000000 pymino-1.1.7.6/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-17 03:25:30.000000 pymino-1.1.7.6/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 03:25:30.000000 pymino-1.1.7.6/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-05-17 03:25:30.690179 pymino-1.1.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.6/setup.py
```

### Comparing `pymino-1.1.7.5/LICENSE` & `pymino-1.1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/PKG-INFO` & `pymino-1.1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.5
+Version: 1.1.7.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.5/README.md` & `pymino-1.1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/__init__.py` & `pymino-1.1.7.6/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.7.5'
+__version__ = '1.1.7.6'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .client import Client as Client
 
 from requests import get
 from colorama import Fore, Style
```

### Comparing `pymino-1.1.7.5/pymino/bot.py` & `pymino-1.1.7.6/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/client.py` & `pymino-1.1.7.6/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/account.py` & `pymino-1.1.7.6/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/community.py` & `pymino-1.1.7.6/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/context.py` & `pymino-1.1.7.6/pymino/ext/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from requests import get
+from diskcache import Cache
 from threading import Thread
 from base64 import b64encode
 from contextlib import suppress
 from colorama import Fore, Style
 from time import sleep as delay, time
 from inspect import signature as inspect_signature
 from typing import BinaryIO, Callable, List, Union
 
 from .entities.general import ApiResponse
 from .entities.userprofile import OnlineMembers
 from .utilities.commands import Command, Commands
 from .entities.exceptions import InvalidImage, MustRunInContext
 from .entities.messages import (
-    CMessage, Message, MessageAuthor, PrepareMessage
+    CMessage, Message, MessageAuthor, PrepareMessage, NNotification
     )
 
 class Context():
     """
     `Context` - This handles the event context.
 
     `**Parameters**``
     - `message` - The message which triggered the event.
     - `session` - The session we will use to send requests.
 
     """
     def __init__(self, message: Message, session):
-        self.message:  Message = message
-        self.userId:   str = session.userId
-        self.request   = session
+        self.message:   Message = message
+        self.userId:    str = session.userId
+        self.request    = session
 
     @property
     def author(self) -> MessageAuthor:
         """The author of the message."""
         with suppress(AttributeError): return self.message.author
 
     @property
@@ -110,15 +111,62 @@
         
         """
         delay(delete_after)
         return ApiResponse(self.request.handler(
             method = "DELETE",
             url = f"/{self.communityId}/s/chat/thread/{self.message.chatId}/message/{delete_message.messageId}"
             ))
+    
+    def wait_for_message(self, message: str, timeout: int = 10) -> Message:
+        """
+        `wait_for_message` - This waits for a message. 
+        
+        `**Parameters**`
+        - `message` - The message to wait for.
+        - `timeout` - The time to wait before timing out.
+        
+        `**Returns**`
+        - `Message` - The message that was sent.
+        
+        `**Example**`
+        ```py
+        @bot.on_member_join()
+        def on_member_join(ctx: Context):
+            if ctx.comId != bot.community.community_id:
+                return
+                
+            TIMEOUT = 15
+
+            ctx.send(content="Welcome to the chat! Please verify yourself by typing `$verify` in the chat.", delete_after=TIMEOUT)
 
+            response = ctx.wait_for_message(message="$verify", timeout=15)
+
+            if response is None:
+                ctx.send(content="You took too long to verify yourself. You have been kicked from the chat.", delete_after=TIMEOUT)
+                return bot.community.kick(userId=ctx.author.userId, chatId=ctx.chatId, allowRejoin=True, comId=ctx.comId)
+
+            else:
+                ctx.send(content="You have been verified!", delete_after=TIMEOUT)
+        ```
+        """
+        start = time()
+        cache = Cache("cache")
+        
+        while True:
+            cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
+            if time() - start >= timeout:
+                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                return None
+            if cached_message is not None and cached_message != message:
+                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                return None
+            if cached_message == message:
+                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                return self.message
+    
     @_run
     def send(self, content: str, delete_after: int= None, mentioned: Union[str, List[str]]= None) -> CMessage:
         """
         `send` - This sends a message.
 
         `**Parameters**``
         - `content` - The message you want to send.
@@ -138,16 +186,16 @@
             content=content,
             extensions = {
             "mentionedArray": [
             {"uid": self.message.author.userId}
             ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
             ] if isinstance(mentioned, list) else None
             })
-        
-        self._delete(message, delete_after) if delete_after else None
+
+        Thread(target=self._delete, args=(message, delete_after)) if delete_after else None
 
         return message
 
     @_run
     def reply(self, content: str, delete_after: int= None, mentioned: Union[str, List[str]]= None) -> CMessage:
         """
         `reply` - This replies to the message.
@@ -172,15 +220,15 @@
             extensions = {
             "mentionedArray": [
             {"uid": self.message.author.userId}
             ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
             ] if isinstance(mentioned, list) else None
             })
         
-        self._delete(message, delete_after) if delete_after else None
+        Thread(target=self._delete, args=(message, delete_after)) if delete_after else None
         
         return message
 
     def prepare_mentions(self, mentioned: dict) -> list:
         """
         `prepare_mentions` - This prepares the mentions for the message.
         
@@ -477,27 +525,30 @@
         ```
         """
         return ApiResponse(self.request.handler(
             method="DELETE",
             url=f"/{self.communityId}/s/chat/thread/{chatId or self.chatId}/member/{self.userId}"
             ))
     
-class EventHandler(Context):
+class EventHandler: #NEW.
+    #OLD: class EventHandler(Context):
     """
     `EventHandler` - AKA where all the events are handled.
 
     `**Parameters**``
     - `session` - The session we are using.
 
     """
     def __init__(self):
         self.command_prefix:    str = self.command_prefix
         self._events:           dict = {}
+        self._wait_for:         Cache = Cache("cache")
         self._commands:         Commands = Commands()
-        super().__init__(self, self.request)
+        self.context:           Context = Context
+
 
     def start_task(self, func):
         """`start_task` - This starts a task."""
         Thread(target=func).start()
 
     def _handle_task(self, func, interval):
         """
@@ -660,45 +711,45 @@
         `**Parameters**``
         - `command_name` - The name of the command.
         
         `**Returns**`` - Command
         """
         return self._commands.fetch_command(command_name)
 
-    def _handle_command(self, data: Message):
+    def _handle_command(self, data: Message, context: Context):
         """`_handle_command` is a function that handles commands."""
         command_name = data.content[len(self.command_prefix):].split(" ")[0]
 
         if any([self.command_exists(command_name) != True, self.command_prefix != data.content[:len(self.command_prefix)]]):
             if (
                 command_name == "help"
                 and data.content == f"{self.command_prefix}help"
             ):
-                return Context(data, self.request).reply(self._commands.__help__())
+                return context.reply(self._commands.__help__())
             elif "text_message" in self._events:
                 return self._handle_text_message(data)
             else:
                 return None
 
         if data.content[:len(self.command_prefix)] != self.command_prefix:
             return None
 
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
         parameters = [{
-            "ctx": Context(data, self.request),
+            "ctx": context,
             "message": None if len(message) == 0 else message,
             "username": data.author.username,
             "userId": data.author.userId
         }.get(i) for i in inspect_signature(self.fetch_command(command_name).func).parameters]
 
         command_name = dict(self._commands.__command_aliases__().copy()).get(command_name, command_name)  
 
         if self._commands.fetch_command(command_name).cooldown > 0:
             if self._commands.fetch_cooldown(command_name, data.author.userId) > time():
-                return Context(data, self.request).reply(f"You are on cooldown for {int(self._commands.fetch_cooldown(command_name, data.author.userId) - time())} seconds.")
+                return context.reply(f"You are on cooldown for {int(self._commands.fetch_cooldown(command_name, data.author.userId) - time())} seconds.")
             self._commands.set_cooldown(command_name, self._commands.fetch_command(command_name).cooldown, data.author.userId)
 
         return self._commands.fetch_command(command_name).func(*parameters)
         
     def on_error(self):
         """
         `on_error` - This is an event that handles errors to prevent the bot from crashing.
@@ -749,31 +800,41 @@
             print(userId)
         ```
         """
         def decorator(func):
             self._events["text_message"] = func
             return func
         return decorator
+    
+    def _add_cache(self, chatId: str, userId: str, content: str):
+        if self._wait_for.get(f"{chatId}_{userId}") is not None:
+            self._wait_for.clear(f"{chatId}_{userId}")
+
+        self._wait_for.add(
+            key=f"{chatId}_{userId}",
+            value=content,
+            expire=90
+            )
+        
+    def _remove_cache(self, chatId: str, userId: str):
+        self._wait_for.clear(f"{chatId}_{userId}")
 
-    def _handle_text_message(self, data: Message):
+    def _handle_text_message(self, data: Message, context: Context):
         """`_handle_text_message` is a function that handles text messages."""
-
-        ctx: Context = Context(data, self.request)
-        
         if data.content.startswith(self.command_prefix):
             command_name = data.content.split(" ")[0][len(self.command_prefix):]
         else:
             command_name = None
 
         parameters = [{
-            "ctx": ctx,
+            "ctx": context,
             "command": self.command_prefix + command_name if command_name != None else "Command not found",
-            "message": ctx.message.content[len(command_name) + len(self.command_prefix) + 1:] if command_name else ctx.message.content,
-            "username": ctx.author.username,
-            "userId": ctx.author.userId
+            "message": context.message.content[len(command_name) + len(self.command_prefix) + 1:] if command_name else context.message.content,
+            "username": context.author.username,
+            "userId": context.author.userId
         }.get(i) for i in inspect_signature(self._events["text_message"]).parameters]
 
         return self._events["text_message"](*parameters)
 
     def on_image_message(self):
         """
         `on_image_message` - This is an event that is called when an image message is received.
@@ -1143,17 +1204,101 @@
 
     def on_user_online(self):
         def decorator(func):
             self._events["user_online"] = func
             return func
         return decorator
 
-    def _handle_event(self, event: str, data: Message):
+
+    def on_member_set_you_host(self):
+        """
+        `on_member_set_you_host` - This is an event that is called when you are set as host.
+
+        `**Example**``
+        ```py
+        from pymino.ext import *
+        chatId = "0000-0000-0000-0000"
+
+        @bot.on_member_set_you_host()
+        def member_set_you_host(notification: NNotification):
+            if notification.chatId == chatId:
+                print("You are now host")
+                bot.community.send_message(chatId=chatId, content="I am now host", comId=notification.comId)
+        ```
+        """
+        def decorator(func):
+            self._events["member_set_you_host"] = func
+            return func
+        return decorator
+    
+    def on_member_set_you_cohost(self):
+        """
+        `on_member_set_you_cohost` - This is an event that is called when you are set as cohost.
+        
+        `**Example**``
+        ```py
+        from pymino.ext import *
+        chatId = "0000-0000-0000-0000"
+        
+        @bot.on_member_set_you_cohost()
+        def member_set_you_cohost(notification: NNotification):
+            if notification.chatId == chatId:
+                print("You are now cohost")
+                bot.community.send_message(chatId=chatId, content="I am now cohost", comId=notification.comId)
+        ```
+        """
+        def decorator(func):
+            self._events["member_set_you_cohost"] = func
+            return func
+        return decorator
+    
+    def on_member_remove_your_cohost(self):
+        """
+        `on_member_remove_your_cohost` - This is an event that is called when you are removed as cohost.
+        
+        `**Example**``
+        ```py
+        from pymino.ext import *
+        chatId = "0000-0000-0000-0000"
+        
+        @bot.on_member_remove_your_cohost()
+        def member_remove_your_cohost(notification: NNotification):
+            if notification.chatId == chatId:
+                print("You are no longer cohost")
+                bot.community.send_message(chatId=chatId, content="I am no longer cohost", comId=notification.comId)
+        ```
+        """
+        def decorator(func):
+            self._events["member_remove_your_cohost"] = func
+            return func
+        return decorator
+
+    def _handle_event(
+        self,
+        event: str,
+        data: Union[Message, OnlineMembers, NNotification, Context]
+        ) -> Union[Context, None]:
+        """
+        `_handle_event` is a function that handles events.
+        """
+        context = self.context(data, self.request)
+
         if event == "text_message":
-            return self._handle_command(data)
+            self._add_cache(data.chatId, data.author.userId, data.content)
+            if event in self._events:
+                return self._handle_command(data=data, context=context)
+        
+        if event in self._events:
+            self._remove_cache(data.chatId, data.author.userId)
+            if event == "user_online":
+                return self._events[event](data)
+
+            if event in {
+                "member_set_you_host",
+                "member_set_you_cohost",
+                "member_remove_your_cohost",
+            }:
+                return self._events[event](data)
 
-        elif event == "user_online":
-            return self._events["user_online"](OnlineMembers(data.json()))
+            return self._events[event](context)
 
-        elif any([event != "text_message", event != "user_online"]):
-            with suppress(KeyError):
-                return self._events[event](Context(data, self.request))
+        return None
```

### Comparing `pymino-1.1.7.5/pymino/ext/dispatcher.py` & `pymino-1.1.7.6/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/entities/enums.py` & `pymino-1.1.7.6/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/entities/exceptions.py` & `pymino-1.1.7.6/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/entities/general.py` & `pymino-1.1.7.6/pymino/ext/entities/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,18 @@
 
         if isinstance(data, dict):
             self.checkInHistory:          dict = self.data.get("checkInHistory", self.checkInHistory)
             self.consecutiveCheckInDays:  Union[int, None] = self.checkInHistory.get("consecutiveCheckInDays", self.consecutiveCheckInDays)
             self.hasCheckInToday:         Union[bool, None] = self.checkInHistory.get("hasCheckInToday", self.hasCheckInToday)
             self.hasAnyCheckIn:           Union[bool, None] = self.checkInHistory.get("hasAnyCheckIn", self.hasAnyCheckIn)
             self.history:                 dict = self.checkInHistory.get("history", self.history)
-            self.userProfile:             dict = self.data.get("userProfile", self.userProfile)
+            try:
+                self.userProfile:         Union[dict, None] = self.data.get("userProfile", self.userProfile)
+            except Exception:
+                self.userProfile:         Union[dict, None] = None
 
     def json(self) -> Union[dict, str]:
         return self.data
 
 class InvitationId:
     def __init__(self, data: Union[dict, str]) -> None:
         self.data = data
@@ -277,15 +280,20 @@
             self.globalCommentsCount:   int = self.data.get("globalCommentsCount", self.globalCommentsCount)
             self.modifiedTime:          str = self.data.get("modifiedTime", self.modifiedTime)
             self.widgetDisplayInterval: str = self.data.get("widgetDisplayInterval", self.widgetDisplayInterval)
             self.totalPollVoteCount:    int = self.data.get("totalPollVoteCount", self.totalPollVoteCount)
             self.blogId:                str = self.data.get("blogId", self.blogId)
             self.viewCount:             int = self.data.get("viewCount", self.viewCount)
             self.language:              str = self.data.get("language", self.language)
-            self.author:                UserProfile = UserProfile(data=self.data.get("author", self.author))
+
+            try:
+                self.author:            Union[UserProfile, None] = UserProfile(data=self.data.get("author", self.author))
+            except Exception:
+                self.author:            Union[UserProfile, None] = None
+
             self.extensions:            dict = self.data.get("extensions", self.extensions)
             self.votesCount:            int = self.data.get("votesCount", self.votesCount)
             self.ndcId:                 int = self.data.get("ndcId", self.ndcId)
             self.createdTime:           str = self.data.get("createdTime", self.createdTime)
             self.endTime:               str = self.data.get("endTime", self.endTime)
             self.commentsCount:         int = self.data.get("commentsCount", self.commentsCount)
 
@@ -423,15 +431,20 @@
 
         if isinstance(data, dict):
             self.parentText:        Union[str, None] = self.data.get("parentText", self.parentText)
             self.objectId:          Union[str, None] = self.data.get("objectId", self.objectId)
             self.contextText:       Union[str, None] = self.data.get("contextText", self.contextText)
             self.type:              Union[int, None] = self.data.get("type", self.type)
             self.parentId:          Union[str, None] = self.data.get("parentId", self.parentId)
-            self.operator:          UserProfile = UserProfile(self.data.get("operator", self.operator))
+
+            try:
+                self.operator:          Union[UserProfile, None] = UserProfile(self.data.get("operator", self.operator))
+            except Exception:
+                self.operator:          Union[UserProfile, None] = None
+
             self.createdTime:       Union[str, None] = self.data.get("createdTime", self.createdTime)
             self.parentType:        Union[int, None] = self.data.get("parentType", self.parentType)
             self.comId:             Union[int, None] = self.data.get("ndcId", self.comId)
             self.notificationId:    Union[str, None] = self.data.get("notificationId", self.notificationId)
             self.objectText:        Union[str, None] = self.data.get("objectText", self.objectText)
             self.contextValue:      Union[str, None] = self.data.get("contextValue", self.contextValue)
             self.contextComId:      Union[int, None] = self.data.get("contextNdcId", self.contextComId)
@@ -527,15 +540,20 @@
             self.ndcId:             Union[int, None] = self.data.get("ndcId", self.ndcId)
             self.votedValue:        Union[int, None] = self.data.get("votedValue", self.votedValue)
             self.parentType:        Union[int, None] = self.data.get("parentType", self.parentType)
             self.commentId:         Union[str, None] = self.data.get("commentId", self.commentId)
             self.parentNdcId:       Union[int, None] = self.data.get("parentNdcId", self.parentNdcId)
             self.mediaList:         Union[None, None] = self.data.get("mediaList", self.mediaList)
             self.votesSum:          Union[int, None] = self.data.get("votesSum", self.votesSum)
-            self.author:            UserProfile = UserProfile(self.data.get("author", self.author))
+
+            try:
+                self.author:            Union[UserProfile, None] = UserProfile(self.data.get("author", self.author))
+            except Exception:
+                self.author:            Union[UserProfile, None] = None
+
             self.extensions:        CCommentExtensions = CCommentExtensions(self.data.get("extensions", self.extensions))
             self.content:           Union[str, None] = self.data.get("content", self.content)
             self.parentId:          Union[str, None] = self.data.get("parentId", self.parentId)
             self.createdTime:       Union[str, None] = self.data.get("createdTime", self.createdTime)
             self.subcommentsCount:  Union[int, None] = self.data.get("subcommentsCount", self.subcommentsCount)
             self.type:              Union[int, None] = self.data.get("type", self.type)
         
@@ -750,16 +768,19 @@
     @property
     @return_none
     def ref_object_id(self) -> Union[str, None]:
         return self.ref_object.get('refObjectId')
     
     @property
     @return_none
-    def author(self) -> UserProfile:
-        return UserProfile(self.ref_object.get('author'))
+    def author(self) -> Union[UserProfile, None]:
+        try:
+            return UserProfile(self.ref_object.get('author'))
+        except Exception:
+            return None
 
     def json(self) -> Union[dict, None]:
         return self.data
 
 class FeaturedBlogs:
     def __init__(self, data: dict):
         self.data:                      dict = data.get("featuredList", data)
@@ -880,15 +901,18 @@
     
     @property
     @return_none
     def author(self) -> UserProfile:
         """
         `author` - Returns the author of the quiz.
         """
-        return UserProfile(self.data.get('author'))
+        try:
+            return UserProfile(self.data.get('author'))
+        except Exception:
+            return None
     
     @property
     @return_none
     def latest_mode(self) -> Union[int, None]:
         """
         `latest_mode` - Returns the latest mode of the quiz.
         """
```

### Comparing `pymino-1.1.7.5/pymino/ext/entities/handlers.py` & `pymino-1.1.7.6/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/entities/messages.py` & `pymino-1.1.7.6/pymino/ext/entities/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,24 +388,27 @@
             - `None` means that there was an error while trying to get the user id.
 
         """
         return self.uid
     
     @property
     @return_none
-    def author(self) -> UserProfile:
+    def author(self) -> Union[UserProfile, None]:
         """
         `Author` - is the user profile of the user who sent the message that was replied to.
 
          THIS IS NOT THE BOT'S USER PROFILE.
             - `UserProfile` means that the user profile was successfully retrieved.
             - `None` means that there was an error while trying to get the user profile.
 
         """
-        return UserProfile(self.data.get('author'))
+        try:
+            return UserProfile(self.data.get('author'))
+        except Exception:
+            return None
     
     @property
     @return_none
     def isHidden(self) -> Union[bool, None]:
         """
         `Is Hidden` - is a boolean value that determines whether the message that was replied to is hidden.
 
@@ -1275,8 +1278,66 @@
             - `None` means that there was an error while trying to get the chatId.
 
         """
         return self.threadId
     
     def json(self) -> Union[dict, str]:
         """`JSON` - returns the raw data."""
+        return self.data
+    
+class NNotification:
+    def __init__(self, data: dict):
+        """
+        `NNotification - This contains all attributes aor any notification event.
+        """
+        self.data: dict = data
+
+    @property
+    def __parser__(self) -> dict:
+        try:
+            return self.data.get("o")
+        except Exception:
+            print(self.data)
+            return self.data
+    
+    @property
+    def payload(self) -> dict:
+        return self.__parser__.get("payload")
+    
+    @property
+    def exp(self) -> int:
+        return self.payload.get("exp")
+    
+    @property
+    def ndcId(self) -> int:
+        return self.payload.get("ndcId")
+    
+    @property
+    def comId(self) -> int:
+        return self.ndcId
+    
+    @property
+    def chatId(self) -> str:
+        return self.payload.get("tid")
+    
+    @property
+    def aps(self) -> dict:
+        return self.payload.get("aps")
+    
+    @property
+    def sound(self) -> str:
+        return self.aps.get("sound")
+    
+    @property
+    def alert(self) -> str:
+        return self.aps.get("alert")
+    
+    @property
+    def notifType(self) -> int:
+        return self.payload.get("notifType")
+    
+    @property
+    def id(self) -> str:
+        return self.payload.get("id")
+    
+    def json(self) -> dict:
         return self.data
```

### Comparing `pymino-1.1.7.5/pymino/ext/entities/threads.py` & `pymino-1.1.7.6/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/entities/userprofile.py` & `pymino-1.1.7.6/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/entities/wsevents.py` & `pymino-1.1.7.6/pymino/ext/entities/wsevents.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 class EventTypes:
-    def __init__(self):
+    def __init__(self) -> None:
         self.events = {
             "0:0": "text_message",
             "0:100": "image_message",
             "0:103": "youtube_message",
             "1:0": "strike_message",
             "2:110": "voice_message",
             "3:113": "sticker_message",
@@ -46,8 +46,16 @@
             "126:0": "chat_view_only_disabled",
             "127:0": "chat_unpin_announcement",
             "128:0": "chat_tipping_enabled",
             "129:0": "chat_tipping_disabled",
             "65281:0": "timestamp_message",
             "65282:0": "welcome_message",
             "65283:0": "invite_message"
-            }
+            }
+        
+class NotifTypes:
+    def __init__(self) -> None:
+        self.notifs = {
+        53: "member_set_you_host",
+        67: "member_set_you_cohost",
+        68: "member_remove_your_cohost"
+        }
```

### Comparing `pymino-1.1.7.5/pymino/ext/socket.py` & `pymino-1.1.7.6/pymino/ext/socket.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from contextlib import suppress
 from urllib.parse import urlencode
 from time import sleep as delay, time
 from ujson import loads, dumps, JSONDecodeError
 
 from .context import EventHandler
 from .dispatcher import MessageDispatcher
-from .entities.wsevents import EventTypes
+from .entities.wsevents import EventTypes, NotifTypes
 from .entities.userprofile import OnlineMembers
-from .entities.messages import Channel, Message
+from .entities.messages import Channel, Message, NNotification
 from .entities.exceptions import WrongWebSocketPackage
 from .utilities.generate import device_id, generate_signature
 from .entities.handlers import is_android, is_repl, notify, orjson_exists
 
 if orjson_exists():
     from orjson import (
         loads as orjson_loads, dumps as orjson_dumps
@@ -33,18 +33,20 @@
     `WSClient` is a class that handles the websocket.
     """
     def __init__(self):
         self.ws:            WebSocketApp = None
         self.online_status: bool = True        
         self._communities:  set = set()
         self.event_types:   dict =  EventTypes().events
+        self.notif_types:   dict =  NotifTypes().notifs
         self.dispatcher:    MessageDispatcher = MessageDispatcher()
         self.channel:       Optional[Channel] = None
         self.orjson:        bool = orjson_exists()
         
+        self.dispatcher.register(10, self._handle_notification)
         self.dispatcher.register(201, self._handle_agora_channel)
         self.dispatcher.register(400, self._handle_user_online)
         self.dispatcher.register(1000, self._handle_message)
         EventHandler.__init__(self)
         
     def fetch_ws_url(self) -> str:
         return f"wss://ws{randint(1, 4)}.aminoapps.com"
@@ -87,26 +89,32 @@
         except JSONDecodeError:
             raw_message = loads(message)
 
         self.dispatcher.handle(raw_message)
 
     def _handle_message(self, message: dict) -> None:
         """Sends the message to the event handler."""
-        message: Message = Message(message)
-        if self.userId == message.userId: return None
-        
-        None if any(
-            [message.ndcId is None, message.ndcId == 0]
-        ) else self._communities.add(message.ndcId)
+        _message: Message = Message(message)
 
-        key = self.event_types.get(f"{message.type}:{message.mediaType}")
+        if self.userId == _message.userId: return None
+        None if any(
+            [_message.ndcId is None, _message.ndcId == 0]
+        ) else self._communities.add(_message.ndcId)
 
+        key = self.event_types.get(f"{_message.type}:{_message.mediaType}")
         if key != None:
-            return Thread(target=self._handle_event, args=(key, message)).start()
+            return Thread(target=self._handle_event, args=(key, _message)).start()
 
+    def _handle_notification(self, message: dict) -> None:
+        """Handles notifications."""
+        notification: NNotification = NNotification(message)
+        key = self.notif_types.get(notification.notifType)
+        if key != None:
+            return Thread(target=self._handle_event, args=(key, notification)).start()
+    
     def _handle_agora_channel(self, message: dict) -> None:
         """Sets the agora channel."""
         self.channel: Channel = Channel(message)
 
     def _handle_user_online(self, message: dict) -> None:
         """Handles user online events."""
         return self._handle_event("user_online", OnlineMembers(message))
```

### Comparing `pymino-1.1.7.5/pymino/ext/utilities/commands.py` & `pymino-1.1.7.6/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/utilities/generate.py` & `pymino-1.1.7.6/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino/ext/utilities/request_handler.py` & `pymino-1.1.7.6/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/pymino.egg-info/PKG-INFO` & `pymino-1.1.7.6/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.5
+Version: 1.1.7.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.5/pymino.egg-info/SOURCES.txt` & `pymino-1.1.7.6/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.5/setup.cfg` & `pymino-1.1.7.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e37 2e35 0d0a 6175  on = 1.1.7.5..au
+00000020: 6f6e 203d 2031 2e31 2e37 2e36 0d0a 6175  on = 1.1.7.6..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.7.5/setup.py` & `pymino-1.1.7.6/setup.py`

 * *Files identical despite different names*

