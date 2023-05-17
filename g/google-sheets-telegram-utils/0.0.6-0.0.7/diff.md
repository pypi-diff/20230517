# Comparing `tmp/google-sheets-telegram-utils-0.0.6.tar.gz` & `tmp/google-sheets-telegram-utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-sheets-telegram-utils-0.0.6.tar", last modified: Mon Dec 13 07:25:33 2021, max compression
+gzip compressed data, was "google-sheets-telegram-utils-0.0.7.tar", last modified: Wed May 17 15:37:42 2023, max compression
```

## Comparing `google-sheets-telegram-utils-0.0.6.tar` & `google-sheets-telegram-utils-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.607471 google-sheets-telegram-utils-0.0.6/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      640 2021-12-13 07:25:33.606141 google-sheets-telegram-utils-0.0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        4 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.550910 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/
--rwxrwxrwx   0 root         (0) root         (0)      164 2021-12-13 07:24:12.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.562834 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/examples/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-11-17 14:17:42.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/examples/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      249 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.565335 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/handlers/
--rwxrwxrwx   0 root         (0) root         (0)       79 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/handlers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      743 2021-11-17 14:21:36.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/handlers/testing_handlers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.572731 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1192 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/abstract_job.py
--rwxrwxrwx   0 root         (0) root         (0)     1196 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/inline_keyboard.py
--rwxrwxrwx   0 root         (0) root         (0)      820 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/main_example.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.574595 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.577498 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/
--rwxrwxrwx   0 root         (0) root         (0)       47 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1167 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/active_user_decorator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.581368 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/classes/
--rwxrwxrwx   0 root         (0) root         (0)       40 2021-11-17 06:44:18.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/classes/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      722 2021-11-17 15:17:33.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/classes/telegram_user.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.591497 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/configs/
--rwxrwxrwx   0 root         (0) root         (0)      132 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/configs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      150 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/configs/abstract_config.py
--rwxrwxrwx   0 root         (0) root         (0)      182 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/configs/csv_config.py
--rwxrwxrwx   0 root         (0) root         (0)      343 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/configs/google_sheet_config.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.599855 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/
--rwxrwxrwx   0 root         (0) root         (0)      150 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      619 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/abstract_connector.py
--rwxrwxrwx   0 root         (0) root         (0)     1577 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/csv_connector.py
--rwxrwxrwx   0 root         (0) root         (0)     1708 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/google_sheet_connector.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.603690 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/factories/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-11-17 07:00:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/factories/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1098 2021-12-13 07:22:57.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/factories/handlers_factory.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 07:25:33.560736 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      640 2021-12-13 07:25:33.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1631 2021-12-13 07:25:33.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-12-13 07:25:33.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      172 2021-12-13 07:25:33.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       29 2021-12-13 07:25:33.000000 google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2021-12-13 07:25:33.607471 google-sheets-telegram-utils-0.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1002 2021-12-13 07:24:12.000000 google-sheets-telegram-utils-0.0.6/setup.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.132162 google-sheets-telegram-utils-0.0.7/
+-rw-r--r--   0 varalex    (503) staff       (20)        0 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/LICENSE
+-rw-r--r--   0 varalex    (503) staff       (20)      624 2023-05-17 15:37:42.131705 google-sheets-telegram-utils-0.0.7/PKG-INFO
+-rw-r--r--   0 varalex    (503) staff       (20)        4 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/README.rst
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.109165 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/
+-rw-r--r--   0 varalex    (503) staff       (20)      164 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/__init__.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.113984 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/examples/
+-rw-r--r--   0 varalex    (503) staff       (20)        0 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/examples/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)      249 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/exceptions.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.115353 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/handlers/
+-rw-r--r--   0 varalex    (503) staff       (20)       79 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/handlers/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)      743 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/handlers/testing_handlers.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.118810 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/
+-rw-r--r--   0 varalex    (503) staff       (20)        0 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)     1192 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/abstract_job.py
+-rw-r--r--   0 varalex    (503) staff       (20)     1196 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/inline_keyboard.py
+-rw-r--r--   0 varalex    (503) staff       (20)      820 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/main_example.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.119730 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/tests/
+-rw-r--r--   0 varalex    (503) staff       (20)        0 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/tests/__init__.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.120981 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/
+-rw-r--r--   0 varalex    (503) staff       (20)       47 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)     1235 2023-05-17 14:19:14.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/active_user_decorator.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.122710 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/classes/
+-rw-r--r--   0 varalex    (503) staff       (20)       40 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/classes/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)     1173 2023-05-17 15:22:55.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/classes/telegram_user.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.125727 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/configs/
+-rw-r--r--   0 varalex    (503) staff       (20)      132 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/configs/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)      150 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/configs/abstract_config.py
+-rw-r--r--   0 varalex    (503) staff       (20)      182 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/configs/csv_config.py
+-rw-r--r--   0 varalex    (503) staff       (20)      343 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/configs/google_sheet_config.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.129104 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/
+-rw-r--r--   0 varalex    (503) staff       (20)      150 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)      629 2023-05-17 13:44:03.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/abstract_connector.py
+-rw-r--r--   0 varalex    (503) staff       (20)     1693 2023-05-17 15:26:03.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/csv_connector.py
+-rw-r--r--   0 varalex    (503) staff       (20)     1791 2023-05-17 15:22:55.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/google_sheet_connector.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.130619 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/factories/
+-rw-r--r--   0 varalex    (503) staff       (20)        0 2023-05-17 12:58:11.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/factories/__init__.py
+-rw-r--r--   0 varalex    (503) staff       (20)     1204 2023-05-17 14:08:35.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/factories/handlers_factory.py
+drwxr-xr-x   0 varalex    (503) staff       (20)        0 2023-05-17 15:37:42.113252 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/
+-rw-r--r--   0 varalex    (503) staff       (20)      624 2023-05-17 15:37:42.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/PKG-INFO
+-rw-r--r--   0 varalex    (503) staff       (20)     1631 2023-05-17 15:37:42.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 varalex    (503) staff       (20)        1 2023-05-17 15:37:42.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 varalex    (503) staff       (20)      151 2023-05-17 15:37:42.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/requires.txt
+-rw-r--r--   0 varalex    (503) staff       (20)       29 2023-05-17 15:37:42.000000 google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/top_level.txt
+-rw-r--r--   0 varalex    (503) staff       (20)       38 2023-05-17 15:37:42.132284 google-sheets-telegram-utils-0.0.7/setup.cfg
+-rw-r--r--   0 varalex    (503) staff       (20)      971 2023-05-17 13:28:02.000000 google-sheets-telegram-utils-0.0.7/setup.py
```

### Comparing `google-sheets-telegram-utils-0.0.6/PKG-INFO` & `google-sheets-telegram-utils-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: google-sheets-telegram-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package with utils to work with google spreadsheet and telegram bots
 Home-page: https://github.com/alexVarkalov/google_sheets_telegram_utils
 Author: Alexander Varkalov
 Author-email: alex.varkalov@gmail.com
 License: BSD 2-clause
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
```

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/handlers/testing_handlers.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/handlers/testing_handlers.py`

 * *Files identical despite different names*

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/abstract_job.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/abstract_job.py`

 * *Files identical despite different names*

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/inline_keyboard.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/presets/main_example.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/presets/main_example.py`

 * *Files identical despite different names*

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/active_user_decorator.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/active_user_decorator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from functools import wraps
+from typing import Callable
 
 from google_sheets_telegram_utils.exceptions import RowDoesNotExistException
 from google_sheets_telegram_utils.utils.classes import TelegramUser
 from google_sheets_telegram_utils.utils.connectors.abstract_connector import AbstractConnector
 
 
 def active_user(google_connector: AbstractConnector):
-    def decorator(func):
+    def decorator(func: Callable):
         @wraps(func)
-        def wrapper(update, context):
+        async def wrapper(update, context):
             pk = update.message.from_user.id
             try:
-                data = google_connector.get_row_by_id(pk=pk)
+                data = await google_connector.get_row_by_id(pk=pk)
             except RowDoesNotExistException:
-                context.bot.send_message(
+                await context.bot.send_message(
                     chat_id=update.effective_chat.id,
                     text="Sorry, you are not registered yet",
                 )
             else:
                 user = TelegramUser(data)
                 if not user.is_activated:
-                    context.bot.send_message(
+                    await context.bot.send_message(
                         chat_id=update.effective_chat.id,
                         text="Sorry, Admin has not activated you yet",
                     )
                 else:
-                    return func(update, context)
+                    return await func(update, context)
         return wrapper
     return decorator
```

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/abstract_connector.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/abstract_connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from abc import ABC, abstractmethod
 
 from google_sheets_telegram_utils.utils.configs.abstract_config import AbstractConfig
 
 
 class AbstractConnector(ABC):
     def __init__(self, config: AbstractConfig):
-        self.config = config
+        pass
 
     @abstractmethod
-    def get_data(self) -> dict:
+    async def get_data(self) -> dict:
         raise NotImplementedError
 
     @abstractmethod
-    def add_rows(self, rows: list) -> None:
+    async def add_rows(self, rows: list) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def add_row(self, row):
+    async def add_row(self, row):
         raise NotImplementedError
 
     @abstractmethod
-    def get_row_by_id(self, pk) -> dict:
-        raise NotImplementedError
+    async def get_row_by_id(self, pk) -> dict:
+        raise NotImplementedError
```

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/csv_connector.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/csv_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,47 +4,48 @@
 from google_sheets_telegram_utils.utils.connectors.abstract_connector import AbstractConnector
 
 
 class CsvConnector(AbstractConnector):
 
     def __init__(self, config: CsvConfig):
         super().__init__(config)
+        self.config = config
 
     def init_file(self):
         if not os.path.exists(self.config.file):
             with open(self.config.file, 'w'):
                 ...
 
-    def get_data(self) -> dict:
+    async def get_data(self) -> csv.DictReader:
         with open(self.config.file) as csv_file:
             data = csv.DictReader(csv_file)
         return data
 
-    def _read_fields_and_rows(self):
+    async def _read_fields_and_rows(self) -> list:
         rows = []
         with open(self.config.file) as csv_file:
             csvreader = csv.reader(csv_file)
             for row in csvreader:
                 rows.append(row)
         return rows
 
-    def _get_last_id(self):
-        data = self._read_fields_and_rows()
+    async def _get_last_id(self) -> int:
+        data = await self._read_fields_and_rows()
         if not data:
             return 0
         return int(data[-1][0])
 
-    def add_rows(self, rows: list) -> None:
-        new_id = self._get_last_id() + 1
+    async def add_rows(self, rows: list) -> None:
+        new_id = await self._get_last_id() + 1
         with open(self.config.file, 'a') as csv_file:
             csv_writer = csv.writer(csv_file)
             for row in rows:
                 row.insert(0, new_id)
                 csv_writer.writerow(row)
 
-    def add_row(self, row):
-        return self.add_rows([row])
+    async def add_row(self, row) -> None:
+        await self.add_rows([row])
 
-    def get_row_by_id(self, pk) -> dict:
-        data = self._read_fields_and_rows()
+    async def get_row_by_id(self, pk) -> dict:
+        data = await self._read_fields_and_rows()
         filtered_data = list(filter(lambda row: row[0] == pk, data))
         return filtered_data[0]
```

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/connectors/google_sheet_connector.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/connectors/google_sheet_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,40 +6,41 @@
 from google_sheets_telegram_utils.utils.connectors.abstract_connector import AbstractConnector
 
 
 class GoogleSheetConnector(AbstractConnector):
 
     def __init__(self, config: GoogleSheetConfig):
         super().__init__(config)
+        self.config = config
 
-    def get_data(self) -> dict:
-        workbook = self._get_workbook()
+    async def get_data(self) -> list:
+        workbook = await self._get_workbook()
         sheet = workbook.worksheet(self.config.sheet_name)
         data = sheet.get_all_records()
         return data
 
-    def _get_workbook(self) -> gspread.models.Spreadsheet:
+    async def _get_workbook(self) -> gspread.spreadsheet.Spreadsheet:
         credentials = ServiceAccountCredentials.from_json_keyfile_name(
             self.config.credentials_path,
             self.config.scope,
         )
         client = gspread.authorize(credentials)
         sheet = client.open(self.config.file)
         return sheet
 
-    def add_rows(self, rows: list) -> None:
-        workbook = self._get_workbook()
+    async def add_rows(self, rows: list) -> None:
+        workbook = await self._get_workbook()
         worksheet = workbook.worksheet(self.config.sheet_name)
         records = worksheet.get_all_records()
         insert_position = len(records) + 2
         worksheet.insert_rows(rows, insert_position, value_input_option='USER_ENTERED')
 
-    def add_row(self, row):
+    async def add_row(self, row):
         return self.add_rows([row])
 
-    def get_row_by_id(self, pk) -> dict:
-        rows = self.get_data()
+    async def get_row_by_id(self, pk) -> dict:
+        rows = await self.get_data()
         filtered_rows = list(filter(lambda row: row['id'] == pk, rows))
         if filtered_rows:
             data = filtered_rows[0]
             return data
         raise RowDoesNotExistException
```

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils/utils/factories/handlers_factory.py` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils/utils/factories/handlers_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from google_sheets_telegram_utils.utils.classes import TelegramUser
 from google_sheets_telegram_utils.utils.connectors.abstract_connector import AbstractConnector
 
 
 class HandlerFactory:
     @staticmethod
     def get_register_handler(connector: AbstractConnector):
-        def register_handler(update, context):
-            telegram_user = TelegramUser(update.message.from_user)
+        async def register_handler(update, context):
+            telegram_user = update.message.from_user
             try:
-                connector.get_row_by_id(telegram_user.id)
+                await connector.get_row_by_id(telegram_user.id)
             except RowDoesNotExistException:
                 try:
-                    connector.add_row(telegram_user.convert_to_list())
+                    telegram_user = TelegramUser.from_telegram_user(telegram_user)
+                    await connector.add_row(telegram_user.convert_to_list())
                 except Exception as err:  # TODO use more specific exception
-                    update.message.reply_text('Cannot register now :c')
+                    await update.message.reply_text('Cannot register now :c')
                 else:
-                    update.message.reply_text('You have been registered. Admin will activate you soon, maybe :3')
+                    await update.message.reply_text('You have been registered. Admin will activate you soon, maybe :3')
             else:
-                update.message.reply_text('You are already registered.')
+                await update.message.reply_text('You are already registered.')
         return register_handler
```

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/PKG-INFO` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: google-sheets-telegram-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package with utils to work with google spreadsheet and telegram bots
 Home-page: https://github.com/alexVarkalov/google_sheets_telegram_utils
 Author: Alexander Varkalov
 Author-email: alex.varkalov@gmail.com
 License: BSD 2-clause
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
```

### Comparing `google-sheets-telegram-utils-0.0.6/google_sheets_telegram_utils.egg-info/SOURCES.txt` & `google-sheets-telegram-utils-0.0.7/google_sheets_telegram_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-sheets-telegram-utils-0.0.6/setup.py` & `google-sheets-telegram-utils-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='google-sheets-telegram-utils',
-    version='0.0.6',
+    version='0.0.7',
     description='A package with utils to work with google spreadsheet and telegram bots',
     url='https://github.com/alexVarkalov/google_sheets_telegram_utils',
     author='Alexander Varkalov',
     author_email='alex.varkalov@gmail.com',
     license='BSD 2-clause',
     packages=find_packages(),
     install_requires=[
-        'python-telegram-bot==13.7',
-        'python-dotenv==0.19.0',
-        'google-api-python-client==2.22.0',
+        'python-telegram-bot==20.3',
+        'python-dotenv==1.0.0',
+        'google-api-python-client==2.86.0',
         'google-auth-httplib2==0.1.0',
-        'google-auth-oauthlib==0.4.6',
-        'gspread==4.0.1',
-        'oauth2client==4.1.3',
+        'google-auth-oauthlib==1.0.0',
+        'gspread==5.9.0',
     ],
 
     classifiers=[
         'Development Status :: 1 - Planning',
         'Environment :: Other Environment',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

