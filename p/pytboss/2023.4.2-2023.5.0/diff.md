# Comparing `tmp/pytboss-2023.4.2.tar.gz` & `tmp/pytboss-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytboss-2023.4.2.tar", last modified: Tue Apr  4 21:21:15 2023, max compression
+gzip compressed data, was "pytboss-2023.5.0.tar", last modified: Wed May 17 12:57:37 2023, max compression
```

## Comparing `pytboss-2023.4.2.tar` & `pytboss-2023.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:21:15.425599 pytboss-2023.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 21:20:58.000000 pytboss-2023.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-04 21:20:58.000000 pytboss-2023.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-04-04 21:21:15.425599 pytboss-2023.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-04-04 21:20:58.000000 pytboss-2023.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:21:15.421599 pytboss-2023.4.2/pytboss/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-04 21:21:15.000000 pytboss-2023.4.2/pytboss/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/ble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)   537876 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/grills.json
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-04 21:20:58.000000 pytboss-2023.4.2/pytboss/grills.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:21:15.425599 pytboss-2023.4.2/pytboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-04-04 21:21:15.000000 pytboss-2023.4.2/pytboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-04 21:21:15.000000 pytboss-2023.4.2/pytboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 21:21:15.000000 pytboss-2023.4.2/pytboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 21:21:15.000000 pytboss-2023.4.2/pytboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-04 21:21:15.000000 pytboss-2023.4.2/pytboss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 21:21:15.000000 pytboss-2023.4.2/pytboss.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-04 21:20:58.000000 pytboss-2023.4.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 21:20:58.000000 pytboss-2023.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-04 21:20:58.000000 pytboss-2023.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 21:21:15.425599 pytboss-2023.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:37.813426 pytboss-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 12:57:11.000000 pytboss-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 12:57:11.000000 pytboss-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-17 12:57:37.813426 pytboss-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-17 12:57:11.000000 pytboss-2023.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:37.809426 pytboss-2023.5.0/pytboss/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   537876 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/grills.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/grills.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:37.813426 pytboss-2023.5.0/pytboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 12:57:11.000000 pytboss-2023.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 12:57:11.000000 pytboss-2023.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 12:57:11.000000 pytboss-2023.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:57:37.813426 pytboss-2023.5.0/setup.cfg
```

### Comparing `pytboss-2023.4.2/LICENSE` & `pytboss-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/PKG-INFO` & `pytboss-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytboss
-Version: 2023.4.2
+Version: 2023.5.0
 Summary: Python library for interacting with Pitboss grills and smokers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Keywords: pitboss,api,iot,ble
```

### Comparing `pytboss-2023.4.2/README.md` & `pytboss-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/pyproject.toml` & `pytboss-2023.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/pytboss/api.py` & `pytboss-2023.5.0/pytboss/api.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/pytboss/ble.py` & `pytboss-2023.5.0/pytboss/ble.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from __future__ import annotations
 
 import asyncio
 import json
 from typing import Awaitable, Callable
 from uuid import UUID
 
-import bleak_retry_connector
 from bleak import BleakClient, BleakGATTCharacteristic, BLEDevice
+import bleak_retry_connector
 from bleak_retry_connector import BleakClientWithServiceCache
 
 from .exceptions import RPCError
 
 
 def _uuid(s: str) -> str:
     return str(UUID(bytes=s.encode()))
@@ -80,15 +80,20 @@
 
     def _on_disconnected(self, unused_client):
         """Called when our Bluetooth client is disconnected."""
         self._is_connected = False
 
     async def disconnect(self) -> None:
         """Stops the connection to the device."""
-        await self._ble_client.disconnect()
+        if self._ble_client:
+            try:
+                await self._ble_client.disconnect()
+            except:
+                # Bluetooth is awful. Sometimes even disconnects fail.
+                pass
         self._is_connected = False
 
     async def reset_device(self, ble_device: BLEDevice):
         """Resets the BLE device used for transport.
 
         :param ble_device: BLE device to use for transport.
         :type ble_device: bleak.BLEDevice
```

### Comparing `pytboss-2023.4.2/pytboss/config.py` & `pytboss-2023.5.0/pytboss/config.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/pytboss/fs.py` & `pytboss-2023.5.0/pytboss/fs.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/pytboss/grills.json` & `pytboss-2023.5.0/pytboss/grills.json`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/pytboss/grills.py` & `pytboss-2023.5.0/pytboss/grills.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.4.2/pytboss.egg-info/PKG-INFO` & `pytboss-2023.5.0/pytboss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytboss
-Version: 2023.4.2
+Version: 2023.5.0
 Summary: Python library for interacting with Pitboss grills and smokers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Keywords: pitboss,api,iot,ble
```

