# Comparing `tmp/homeduino-0.0.7.3.tar.gz` & `tmp/homeduino-0.0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.7.3.tar", last modified: Tue May 16 22:22:34 2023, max compression
+gzip compressed data, was "homeduino-0.0.7.4.tar", last modified: Tue May 16 22:33:55 2023, max compression
```

## Comparing `homeduino-0.0.7.3.tar` & `homeduino-0.0.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:34.868888 homeduino-0.0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-16 22:22:20.000000 homeduino-0.0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 22:22:34.868888 homeduino-0.0.7.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:34.868888 homeduino-0.0.7.3/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 22:22:20.000000 homeduino-0.0.7.3/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 22:22:20.000000 homeduino-0.0.7.3/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-05-16 22:22:20.000000 homeduino-0.0.7.3/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:34.868888 homeduino-0.0.7.3/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 22:22:34.000000 homeduino-0.0.7.3/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 22:22:34.000000 homeduino-0.0.7.3/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:22:34.000000 homeduino-0.0.7.3/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 22:22:34.000000 homeduino-0.0.7.3/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 22:22:34.000000 homeduino-0.0.7.3/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 22:22:20.000000 homeduino-0.0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:22:34.868888 homeduino-0.0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:33:55.401606 homeduino-0.0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-16 22:33:44.000000 homeduino-0.0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 22:33:55.401606 homeduino-0.0.7.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:33:55.401606 homeduino-0.0.7.4/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 22:33:44.000000 homeduino-0.0.7.4/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 22:33:44.000000 homeduino-0.0.7.4/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-05-16 22:33:44.000000 homeduino-0.0.7.4/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:33:55.401606 homeduino-0.0.7.4/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 22:33:55.000000 homeduino-0.0.7.4/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 22:33:55.000000 homeduino-0.0.7.4/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:33:55.000000 homeduino-0.0.7.4/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 22:33:55.000000 homeduino-0.0.7.4/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 22:33:55.000000 homeduino-0.0.7.4/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 22:33:44.000000 homeduino-0.0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:33:55.401606 homeduino-0.0.7.4/setup.cfg
```

### Comparing `homeduino-0.0.7.3/LICENSE` & `homeduino-0.0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7.3/PKG-INFO` & `homeduino-0.0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.3
+Version: 0.0.7.4
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.3/homeduino/__main__.py` & `homeduino-0.0.7.4/homeduino/__main__.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7.3/homeduino/homeduino.py` & `homeduino-0.0.7.4/homeduino/homeduino.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         start_time = datetime.now()
         while self._tx_busy:
             if (datetime.now() - start_time).total_seconds() > _BUSY_TIMEOUT:
                 logger.error("Too busy to send %s", packet)
                 raise TooBusyError("Homeduino is too busy to send a command")
             logger.debug("Busy")
-            await asyncio.sleep(0)
+            await asyncio.sleep(0.1)
         self._tx_busy = True
 
         try:
             data = packet + "\n"
             logger.debug("Writing data: %s", repr(data))
             # type ignore: transport from create_connection is documented to be
             # implementation specific bidirectional, even though typed as
@@ -173,15 +173,15 @@
             # Wait for response
             start_time = datetime.now()
             while len(self.str_buffer) == 0:
                 if (datetime.now() - start_time).total_seconds() > _RESPONSE_TIMEOUT:
                     logger.error("Timeout while waiting for command response")
                     raise ResponseTimeoutError("Timeout while waiting for command response")
                 logger.debug("Waiting for command response")
-                await asyncio.sleep(0)
+                await asyncio.sleep(0.1)
 
             response = self.str_buffer.pop()
             logger.debug("Command response received: %s", response)
             return response.strip()
         finally:
             self._tx_busy = False
 
@@ -247,15 +247,15 @@
                 while not self.protocol.ready:
                     if (datetime.now() - start_time).total_seconds() > _READY_TIMEOUT:
                         logger.error("Timeout while waiting for Homeduino to become ready")
                         raise ResponseTimeoutError(
                             "Timeout while waiting for Homeduino to become ready"
                         )
                     logger.debug("Waiting for Homeduino to become ready")
-                    await asyncio.sleep(0)
+                    await asyncio.sleep(0.1)
 
                 await self.protocol.set_receive_interrupt(
                     self.receive_interrupt
                 )
 
                 for rf_receive_callback in self.rf_receive_callbacks:
                     self.protocol.add_rf_receive_callback(rf_receive_callback)
@@ -281,15 +281,15 @@
             while self.protocol.ready:
                 if (datetime.now() - start_time).total_seconds() > _READY_TIMEOUT:
                     logger.error("Timeout while waiting for Homeduino to disconnect")
                     raise ResponseTimeoutError(
                         "Timeout while waiting for Homeduino to disconnect"
                     )
                 logger.debug("Waiting for Homeduino to disconnect")
-                await asyncio.sleep(0)
+                await asyncio.sleep(0.1)
 
             self.protocol = None
             return True
             logger.debug("Homeduino disconnected")
 
         return False
```

### Comparing `homeduino-0.0.7.3/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.7.4/homeduino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.3
+Version: 0.0.7.4
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.3/pyproject.toml` & `homeduino-0.0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.7.3"
+version = "0.0.7.4"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
```

