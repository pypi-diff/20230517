# Comparing `tmp/smarthouse-0.1.0.tar.gz` & `tmp/smarthouse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarthouse-0.1.0.tar", last modified: Tue May 16 12:38:07 2023, max compression
+gzip compressed data, was "smarthouse-0.1.1.tar", last modified: Wed May 17 15:05:23 2023, max compression
```

## Comparing `smarthouse-0.1.0.tar` & `smarthouse-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-16 12:38:07.198805 smarthouse-0.1.0/
--rw-r--r--   0 ivan       (501) staff       (20)      735 2023-05-16 12:38:07.198343 smarthouse-0.1.0/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      196 2023-05-16 12:33:30.000000 smarthouse-0.1.0/README.md
--rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.0/pyproject.toml
--rw-r--r--   0 ivan       (501) staff       (20)       38 2023-05-16 12:38:07.198962 smarthouse-0.1.0/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1734 2023-05-16 12:36:24.000000 smarthouse-0.1.0/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-16 12:38:07.194837 smarthouse-0.1.0/smarthouse/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-14 21:44:12.000000 smarthouse-0.1.0/smarthouse/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-16 12:29:15.000000 smarthouse-0.1.0/smarthouse/action_decorators.py
--rw-r--r--   0 ivan       (501) staff       (20)     2577 2023-05-16 12:29:15.000000 smarthouse-0.1.0/smarthouse/app.py
--rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-16 12:29:15.000000 smarthouse-0.1.0/smarthouse/device.py
--rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-16 12:29:15.000000 smarthouse-0.1.0/smarthouse/device_generator.py
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-14 21:44:12.000000 smarthouse-0.1.0/smarthouse/logger.py
--rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-16 12:29:15.000000 smarthouse-0.1.0/smarthouse/storage.py
--rw-r--r--   0 ivan       (501) staff       (20)     8499 2023-05-16 12:29:15.000000 smarthouse-0.1.0/smarthouse/telegram_client.py
--rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-14 21:44:12.000000 smarthouse-0.1.0/smarthouse/utils.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-16 12:38:07.197610 smarthouse-0.1.0/smarthouse.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)      735 2023-05-16 12:38:07.000000 smarthouse-0.1.0/smarthouse.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-16 12:38:07.000000 smarthouse-0.1.0/smarthouse.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-05-16 12:38:07.000000 smarthouse-0.1.0/smarthouse.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      290 2023-05-16 12:38:07.000000 smarthouse-0.1.0/smarthouse.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)       11 2023-05-16 12:38:07.000000 smarthouse-0.1.0/smarthouse.egg-info/top_level.txt
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 15:05:23.525052 smarthouse-0.1.1/
+-rw-r--r--   0 ivan       (501) staff       (20)     4833 2023-05-17 15:05:23.524288 smarthouse-0.1.1/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     4294 2023-05-17 15:01:34.000000 smarthouse-0.1.1/README.md
+-rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.1/pyproject.toml
+-rw-r--r--   0 ivan       (501) staff       (20)       38 2023-05-17 15:05:23.525261 smarthouse-0.1.1/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1734 2023-05-17 15:03:45.000000 smarthouse-0.1.1/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 15:05:23.517093 smarthouse-0.1.1/smarthouse/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/action_decorators.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.1/smarthouse/app.py
+-rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/device.py
+-rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/device_generator.py
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/logger.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/storage.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8499 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/telegram_client.py
+-rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/utils.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 15:05:23.523181 smarthouse-0.1.1/smarthouse.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)     4833 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      290 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       11 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/top_level.txt
```

### Comparing `smarthouse-0.1.0/pyproject.toml` & `smarthouse-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.0/setup.py` & `smarthouse-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "python-dotenv",
     ]
 }
 
 
 setup(
     name="smarthouse",
-    version="0.1.0",
+    version="0.1.1",
     description="Smart House Scenarios",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://smarthouse.readthedocs.io/",
     author="Ivan Kriuchkov",
     author_email="vivenchik@gmail.com",
     license="MIT",
```

### Comparing `smarthouse-0.1.0/smarthouse/action_decorators.py` & `smarthouse-0.1.1/smarthouse/action_decorators.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.0/smarthouse/app.py` & `smarthouse-0.1.1/smarthouse/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 from collections.abc import Coroutine
-from typing import Awaitable
+from typing import Awaitable, Iterable
 
 from aiohttp import web
+from aiohttp.web_routedef import AbstractRouteDef
 
 from smarthouse.device import RunQueuesSet
 from smarthouse.logger import logger
 from smarthouse.scenarios.light_scenarios import (
     clear_retries,
     clear_tg,
     notifications_storage,
@@ -14,14 +15,15 @@
     ping_devices,
     stats,
     tg_actions,
     worker_check_and_run,
     worker_run,
     write_storage,
 )
+from smarthouse.scenarios.system_scenarios import clear_quarantine, detect_human
 from smarthouse.storage import Storage
 from smarthouse.telegram_client import TGClient
 from smarthouse.yandex_client.client import YandexClient
 
 
 class App:
     def __init__(
@@ -29,15 +31,15 @@
         storage_name: str | None,
         yandex_token: str = "",
         telegram_token: str | None = None,
         telegram_chat_id: str = "",
         tg_commands: list[tuple[str, str]] | None = None,
         tg_handlers: list[tuple[str, Awaitable]] | None = None,
         prod: bool = False,
-        aiohttp_routes: list | None = None,
+        aiohttp_routes: Iterable[AbstractRouteDef] | None = None,
     ):
         self.storage_name = storage_name
         self.yandex_token = yandex_token
         self.telegram_token = telegram_token
         self.telegram_chat_id = telegram_chat_id
         self.tg_commands = tg_commands
         self.tg_handlers = tg_handlers
@@ -49,14 +51,16 @@
                 notifications_ya_client(),
                 tg_actions(),
                 stats(),
                 clear_retries(),
                 ping_devices(),
                 clear_tg(),
                 write_storage(),
+                clear_quarantine(),
+                detect_human(),
             ]
             + [worker_run()] * 10
             + [worker_check_and_run()] * 3
         )
 
         if aiohttp_routes is not None:
             app = web.Application()
```

### Comparing `smarthouse-0.1.0/smarthouse/device.py` & `smarthouse-0.1.1/smarthouse/device.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.0/smarthouse/storage.py` & `smarthouse-0.1.1/smarthouse/storage.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.0/smarthouse/telegram_client.py` & `smarthouse-0.1.1/smarthouse/telegram_client.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.0/smarthouse/utils.py` & `smarthouse-0.1.1/smarthouse/utils.py`

 * *Files identical despite different names*

