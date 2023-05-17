# Comparing `tmp/smarthouse-0.1.1.tar.gz` & `tmp/smarthouse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarthouse-0.1.1.tar", last modified: Wed May 17 15:05:23 2023, max compression
+gzip compressed data, was "smarthouse-0.1.2.tar", last modified: Wed May 17 16:28:22 2023, max compression
```

## Comparing `smarthouse-0.1.1.tar` & `smarthouse-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 15:05:23.525052 smarthouse-0.1.1/
--rw-r--r--   0 ivan       (501) staff       (20)     4833 2023-05-17 15:05:23.524288 smarthouse-0.1.1/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     4294 2023-05-17 15:01:34.000000 smarthouse-0.1.1/README.md
--rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.1/pyproject.toml
--rw-r--r--   0 ivan       (501) staff       (20)       38 2023-05-17 15:05:23.525261 smarthouse-0.1.1/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1734 2023-05-17 15:03:45.000000 smarthouse-0.1.1/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 15:05:23.517093 smarthouse-0.1.1/smarthouse/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/action_decorators.py
--rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.1/smarthouse/app.py
--rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/device.py
--rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/device_generator.py
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/logger.py
--rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/storage.py
--rw-r--r--   0 ivan       (501) staff       (20)     8499 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/telegram_client.py
--rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.1/smarthouse/utils.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 15:05:23.523181 smarthouse-0.1.1/smarthouse.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)     4833 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      290 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)       11 2023-05-17 15:05:23.000000 smarthouse-0.1.1/smarthouse.egg-info/top_level.txt
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 16:28:22.365688 smarthouse-0.1.2/
+-rw-r--r--   0 ivan       (501) staff       (20)     4845 2023-05-17 16:28:22.362554 smarthouse-0.1.2/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     4306 2023-05-17 16:27:56.000000 smarthouse-0.1.2/README.md
+-rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.2/pyproject.toml
+-rw-r--r--   0 ivan       (501) staff       (20)       38 2023-05-17 16:28:22.366019 smarthouse-0.1.2/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1734 2023-05-17 16:27:56.000000 smarthouse-0.1.2/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 16:28:22.353646 smarthouse-0.1.2/smarthouse/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/action_decorators.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.2/smarthouse/app.py
+-rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/device.py
+-rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/device_generator.py
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/logger.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/storage.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8436 2023-05-17 16:27:56.000000 smarthouse-0.1.2/smarthouse/telegram_client.py
+-rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.2/smarthouse/utils.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-17 16:28:22.360947 smarthouse-0.1.2/smarthouse.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)     4845 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      290 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       11 2023-05-17 16:28:22.000000 smarthouse-0.1.2/smarthouse.egg-info/top_level.txt
```

### Comparing `smarthouse-0.1.1/PKG-INFO` & `smarthouse-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.1
+Version: 0.1.2
 Summary: Smart House Scenarios
 Home-page: UNKNOWN
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -50,15 +50,15 @@
 import datetime
 import time
 
 from aiohttp import web
 
 from smarthouse.action_decorators import looper, scheduler
 from smarthouse.app import App
-from smarthouse.device import HSVLamp, LuxSensor, run
+from smarthouse.device import HSVLamp, LuxSensor, run_async
 from smarthouse.storage import Storage
 from smarthouse.telegram_client import TGClient
 
 
 def calc_sunset():
     return datetime.timedelta(hours=18)
 
@@ -78,15 +78,15 @@
 
     state_lux = await lux_sensor.illumination()
     if lux_sensor.in_quarantine() and lux_sensor.quarantine().timestamp + 5 * 60 > time.time():
         state_lux = await lux_sensor.illumination(proceeded_last=True)
 
     needed_b = 1 - min(state_lux.result, 200) / 200
 
-    await run([lamp.on_temp(4500, needed_b) for lamp in (lamp_g_1, lamp_g_2)])
+    await run_async([lamp.on_temp(4500, needed_b) for lamp in (lamp_g_1, lamp_g_2)])
 
 
 async def tg_pause_handler(tg_client: TGClient, update):
     storage = Storage()
     storage.put("pause", True)
     await tg_client.write_tg("done")
```

### Comparing `smarthouse-0.1.1/README.md` & `smarthouse-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import datetime
 import time
 
 from aiohttp import web
 
 from smarthouse.action_decorators import looper, scheduler
 from smarthouse.app import App
-from smarthouse.device import HSVLamp, LuxSensor, run
+from smarthouse.device import HSVLamp, LuxSensor, run_async
 from smarthouse.storage import Storage
 from smarthouse.telegram_client import TGClient
 
 
 def calc_sunset():
     return datetime.timedelta(hours=18)
 
@@ -60,15 +60,15 @@
 
     state_lux = await lux_sensor.illumination()
     if lux_sensor.in_quarantine() and lux_sensor.quarantine().timestamp + 5 * 60 > time.time():
         state_lux = await lux_sensor.illumination(proceeded_last=True)
 
     needed_b = 1 - min(state_lux.result, 200) / 200
 
-    await run([lamp.on_temp(4500, needed_b) for lamp in (lamp_g_1, lamp_g_2)])
+    await run_async([lamp.on_temp(4500, needed_b) for lamp in (lamp_g_1, lamp_g_2)])
 
 
 async def tg_pause_handler(tg_client: TGClient, update):
     storage = Storage()
     storage.put("pause", True)
     await tg_client.write_tg("done")
```

### Comparing `smarthouse-0.1.1/pyproject.toml` & `smarthouse-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.1/setup.py` & `smarthouse-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "python-dotenv",
     ]
 }
 
 
 setup(
     name="smarthouse",
-    version="0.1.1",
+    version="0.1.2",
     description="Smart House Scenarios",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://smarthouse.readthedocs.io/",
     author="Ivan Kriuchkov",
     author_email="vivenchik@gmail.com",
     license="MIT",
```

### Comparing `smarthouse-0.1.1/smarthouse/action_decorators.py` & `smarthouse-0.1.2/smarthouse/action_decorators.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.1/smarthouse/app.py` & `smarthouse-0.1.2/smarthouse/app.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.1/smarthouse/device.py` & `smarthouse-0.1.2/smarthouse/device.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.1/smarthouse/storage.py` & `smarthouse-0.1.2/smarthouse/storage.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.1/smarthouse/telegram_client.py` & `smarthouse-0.1.2/smarthouse/telegram_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,15 @@
                             )
                             return
                         elif exc.message == "Message text is empty":
                             pass
                         else:
                             await asyncio.sleep(1)
 
-                    except telegram.error.TimedOut as exc:
-                        _exc = exc
-                    except telegram.error.NetworkError:
+                    except (telegram.error.NetworkError, telegram.error.TimedOut):
                         pass
                     except Exception as exc:
                         _exc = exc
 
         if _exc is not None:
             raise _exc
         if not done:
@@ -160,17 +158,17 @@
                         await self._bot.send_document(
                             chat_id=self._chat_id,
                             document=document,
                             disable_notification=True,
                             read_timeout=10,
                         )
                         return
-                    except (httpx.ReadError, telegram.error.BadRequest, telegram.error.TimedOut) as exc:
+                    except (httpx.ReadError, telegram.error.BadRequest) as exc:
                         _exc = exc
-                    except telegram.error.NetworkError:
+                    except (telegram.error.NetworkError, telegram.error.TimedOut):
                         pass
                     except Exception as exc:
                         _exc = exc
 
         if _exc is not None:
             raise _exc
         raise TGException("try again")
@@ -182,20 +180,20 @@
         _exc = None
         for _ in range(20):
             async with self._w_lock:
                 async with self._bot:
                     try:
                         await self._bot.delete_message(chat_id=self._chat_id, message_id=message_id, read_timeout=10)
                         return
-                    except (httpx.ReadError, telegram.error.TimedOut) as exc:
+                    except httpx.ReadError as exc:
                         _exc = exc
                     except telegram.error.BadRequest as exc:
                         if exc.message == "Message to delete not found":
                             pass
-                    except telegram.error.NetworkError:
+                    except (telegram.error.NetworkError, telegram.error.TimedOut):
                         pass
                     except Exception as exc:
                         _exc = exc
 
         if _exc is not None:
             raise _exc
         raise TGException("try again")
@@ -207,17 +205,17 @@
         updates = []
         async with self._r_lock:
             async with self._bot:
                 try:
                     updates = await self._bot.get_updates(
                         offset=storage.get(SKeys.offset_tg), timeout=10, read_timeout=10
                     )
-                except (httpx.ReadError, telegram.error.BadRequest, telegram.error.TimedOut) as exc:
+                except (httpx.ReadError, telegram.error.BadRequest) as exc:
                     raise exc
-                except telegram.error.NetworkError:
+                except (telegram.error.NetworkError, telegram.error.TimedOut):
                     pass
                 except Exception as exc:
                     raise exc
 
         for update in updates:
             storage.put(SKeys.offset_tg, update.update_id + 1)
             if str(update.message.chat_id) == self._chat_id:
```

### Comparing `smarthouse-0.1.1/smarthouse/utils.py` & `smarthouse-0.1.2/smarthouse/utils.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.1/smarthouse.egg-info/PKG-INFO` & `smarthouse-0.1.2/smarthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.1
+Version: 0.1.2
 Summary: Smart House Scenarios
 Home-page: UNKNOWN
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -50,15 +50,15 @@
 import datetime
 import time
 
 from aiohttp import web
 
 from smarthouse.action_decorators import looper, scheduler
 from smarthouse.app import App
-from smarthouse.device import HSVLamp, LuxSensor, run
+from smarthouse.device import HSVLamp, LuxSensor, run_async
 from smarthouse.storage import Storage
 from smarthouse.telegram_client import TGClient
 
 
 def calc_sunset():
     return datetime.timedelta(hours=18)
 
@@ -78,15 +78,15 @@
 
     state_lux = await lux_sensor.illumination()
     if lux_sensor.in_quarantine() and lux_sensor.quarantine().timestamp + 5 * 60 > time.time():
         state_lux = await lux_sensor.illumination(proceeded_last=True)
 
     needed_b = 1 - min(state_lux.result, 200) / 200
 
-    await run([lamp.on_temp(4500, needed_b) for lamp in (lamp_g_1, lamp_g_2)])
+    await run_async([lamp.on_temp(4500, needed_b) for lamp in (lamp_g_1, lamp_g_2)])
 
 
 async def tg_pause_handler(tg_client: TGClient, update):
     storage = Storage()
     storage.put("pause", True)
     await tg_client.write_tg("done")
```

