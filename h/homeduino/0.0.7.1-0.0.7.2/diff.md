# Comparing `tmp/homeduino-0.0.7.1.tar.gz` & `tmp/homeduino-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.7.1.tar", last modified: Tue May 16 20:32:37 2023, max compression
+gzip compressed data, was "homeduino-0.0.7.2.tar", last modified: Tue May 16 22:06:29 2023, max compression
```

## Comparing `homeduino-0.0.7.1.tar` & `homeduino-0.0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:06:29.168464 homeduino-0.0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-16 22:06:15.000000 homeduino-0.0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 22:06:29.168464 homeduino-0.0.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:06:29.164464 homeduino-0.0.7.2/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 22:06:15.000000 homeduino-0.0.7.2/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 22:06:15.000000 homeduino-0.0.7.2/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-16 22:06:15.000000 homeduino-0.0.7.2/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:06:29.168464 homeduino-0.0.7.2/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 22:06:29.000000 homeduino-0.0.7.2/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 22:06:29.000000 homeduino-0.0.7.2/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:06:29.000000 homeduino-0.0.7.2/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 22:06:29.000000 homeduino-0.0.7.2/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 22:06:29.000000 homeduino-0.0.7.2/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 22:06:15.000000 homeduino-0.0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:06:29.168464 homeduino-0.0.7.2/setup.cfg
```

### Comparing `homeduino-0.0.7.1/LICENSE` & `homeduino-0.0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7.1/PKG-INFO` & `homeduino-0.0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.1/homeduino/__main__.py` & `homeduino-0.0.7.2/homeduino/__main__.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7.1/homeduino/homeduino.py` & `homeduino-0.0.7.2/homeduino/homeduino.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,43 +150,42 @@
             raise DisconnectedError("Homeduino is not connected")
 
         if not self.ready:
             logger.error("Not ready")
             raise NotReadyError("Homeduino is not ready")
 
         start_time = datetime.now()
-        while self._tx_busy is True:
+        while self._tx_busy:
+            if (datetime.now() - start_time).total_seconds() > _BUSY_TIMEOUT:
+                logger.error("Too busy to send %s", packet)
+                raise TooBusyError("Homeduino is too busy to send a command")
             logger.debug("Busy")
-            if (datetime.now() - start_time).total_seconds() < _BUSY_TIMEOUT:
-                await asyncio.sleep(0.01)
-            else:
-                logger.error("Too busy to transmit %s", packet)
-                raise TooBusyError("Homeduino is too busy to transmit")
+            await asyncio.sleep(0)
         self._tx_busy = True
 
         try:
             data = packet + "\n"
             logger.debug("Writing data: %s", repr(data))
             # type ignore: transport from create_connection is documented to be
             # implementation specific bidirectional, even though typed as
             # BaseTransport
             self.transport.write(data.encode())  # type: ignore
 
             # Wait for response
-            logger.debug("Waiting for command response")
             start_time = datetime.now()
-            while (datetime.now() - start_time).total_seconds() < _RESPONSE_TIMEOUT:
-                if len(self.str_buffer) > 0:
-                    response = self.str_buffer.pop()
-                    logger.debug("Command response received: %s", response)
-                    return response.strip()
-                await asyncio.sleep(0.01)
-
-            logger.error("Timeout while waiting for command response")
-            raise ResponseTimeoutError("Timeout while waiting for command response")
+            while len(self.str_buffer) == 0:
+                if (datetime.now() - start_time).total_seconds() > _RESPONSE_TIMEOUT:
+                    logger.error("Timeout while waiting for command response")
+                    raise ResponseTimeoutError("Timeout while waiting for command response")
+                logger.debug("Waiting for command response")
+                await asyncio.sleep(0)
+
+            response = self.str_buffer.pop()
+            logger.debug("Command response received: %s", response)
+            return response.strip()
         finally:
             self._tx_busy = False
 
         return None
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
         logger.info("Port closed")
@@ -241,32 +240,31 @@
                     baudrate=self.baud_rate,
                     bytesize=serial_asyncio.serial.EIGHTBITS,
                     parity=serial_asyncio.serial.PARITY_NONE,
                     stopbits=serial_asyncio.serial.STOPBITS_ONE,
                 )
 
                 start_time = datetime.now()
-                while (datetime.now() - start_time).total_seconds() < _READY_TIMEOUT:
-                    if self.protocol.ready:
-                        await self.protocol.set_receive_interrupt(
-                            self.receive_interrupt
+                while not self.protocol.ready:
+                    if (datetime.now() - start_time).total_seconds() > _READY_TIMEOUT:
+                        logger.error("Timeout while waiting for Homeduino to become ready")
+                        raise ResponseTimeoutError(
+                            "Timeout while waiting for Homeduino to become ready"
                         )
-
-                        for rf_receive_callback in self.rf_receive_callbacks:
-                            self.protocol.add_rf_receive_callback(rf_receive_callback)
-
-                        return True
-
                     logger.debug("Waiting for Homeduino to become ready")
-                    await asyncio.sleep(0.01)
+                    await asyncio.sleep(0)
 
-                logger.error("Timeout while waiting for Homeduino to become ready")
-                raise ResponseTimeoutError(
-                    "Timeout while waiting for Homeduino to become ready"
+                await self.protocol.set_receive_interrupt(
+                    self.receive_interrupt
                 )
+
+                for rf_receive_callback in self.rf_receive_callbacks:
+                    self.protocol.add_rf_receive_callback(rf_receive_callback)
+
+                return True
             except SerialException as ex:
                 logger.error(ex)
 
         return False
 
     def connected(self) -> bool:
         if self.protocol is None or self.protocol.transport is None:
@@ -276,21 +274,23 @@
 
     async def disconnect(self) -> bool:
         if self.connected():
             logger.debug("Disconnecting Homeduino")
             self.protocol.transport.close()
 
             start_time = datetime.now()
-            while (datetime.now() - start_time).total_seconds() < _READY_TIMEOUT:
-                if not self.protocol.ready:
-                    self.protocol = None
-                    return True
-
+            while self.protocol.ready:
+                if (datetime.now() - start_time).total_seconds() > _READY_TIMEOUT:
+                    break
                 logger.debug("Waiting for Homeduino to disconnect")
-                await asyncio.sleep(0.01)
+                await asyncio.sleep(0)
+
+            self.protocol = None
+            return True
+            logger.debug("Homeduino disconnected")
 
         return False
 
     async def ping(self) -> bool:
         if not self.connected():
             raise DisconnectedError("Homeduino is not connected")
```

### Comparing `homeduino-0.0.7.1/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.7.2/homeduino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.1/pyproject.toml` & `homeduino-0.0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.7.1"
+version = "0.0.7.2"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
```

