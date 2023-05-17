# Comparing `tmp/foxglove-websocket-0.1.0.tar.gz` & `tmp/foxglove-websocket-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-websocket-0.1.0.tar", last modified: Fri May 12 16:01:53 2023, max compression
+gzip compressed data, was "foxglove-websocket-0.1.1.tar", last modified: Wed May 17 18:12:55 2023, max compression
```

## Comparing `foxglove-websocket-0.1.0.tar` & `foxglove-websocket-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-12 16:01:53.305074 foxglove-websocket-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.289074 foxglove-websocket-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.293074 foxglove-websocket-0.1.0/src/foxglove_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/json_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/param_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/protobuf_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/src/foxglove_websocket/server/
--rw-r--r--   0 runner    (1001) docker     (123)    24188 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/server/client_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.297074 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:01:32.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/tests/test_client_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-17 18:12:55.922429 foxglove-websocket-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.902428 foxglove-websocket-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.906428 foxglove-websocket-0.1.1/src/foxglove_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/json_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/param_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/protobuf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/src/foxglove_websocket/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/server/client_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.914428 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:39.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/tests/test_client_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/tests/test_server.py
```

### Comparing `foxglove-websocket-0.1.0/PKG-INFO` & `foxglove-websocket-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-websocket
-Version: 0.1.0
+Version: 0.1.1
 Summary: Foxglove WebSocket server
 Home-page: https://github.com/foxglove/ws-protocol
 License: MIT
 Project-URL: GitHub Issues, https://github.com/foxglove/ws-protocol/issues
 Project-URL: Foxglove Studio Documentation, https://foxglove.dev/docs
 Keywords: foxglove,websocket,robotics,ros,ros2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `foxglove-websocket-0.1.0/README.md` & `foxglove-websocket-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/setup.cfg` & `foxglove-websocket-0.1.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-websocket
-version = 0.1.0
+version = 0.1.1
 description = Foxglove WebSocket server
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = foxglove, websocket, robotics, ros, ros2
 license = MIT
 url = https://github.com/foxglove/ws-protocol
 project_urls =
```

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket/__init__.py` & `foxglove-websocket-0.1.1/src/foxglove_websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket/examples/json_server.py` & `foxglove-websocket-0.1.1/src/foxglove_websocket/examples/json_server.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket/examples/param_server.py` & `foxglove-websocket-0.1.1/src/foxglove_websocket/examples/param_server.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket/examples/protobuf_server.py` & `foxglove-websocket-0.1.1/src/foxglove_websocket/examples/protobuf_server.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket/server/__init__.py` & `foxglove-websocket-0.1.1/src/foxglove_websocket/server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         name: str,
         *,
         capabilities: List[str] = [],
         supported_encodings: Optional[List[str]] = None,
         metadata: Optional[Mapping[str, str]] = None,
         session_id: Optional[str] = None,
         logger: logging.Logger = _get_default_logger(),
+        server_kwargs: Dict[str, Any] = {"compression": None},
     ):
         self.host = host
         self.port = port
         self.name = name
         self.capabilities = capabilities
         self.supported_encodings = supported_encodings
         self.metadata = metadata
@@ -174,14 +175,15 @@
         self._clients = ()
         self._channels = {}
         self._next_channel_id = ChannelId(0)
         self._services = {}
         self._next_service_id = ServiceId(0)
         self._subscribed_params = set([])
         self._logger = logger
+        self._server_kwargs = server_kwargs
         self._listener = None
         self._opened = asyncio.get_running_loop().create_future()
 
     def set_listener(self, listener: FoxgloveServerListener):
         self._listener = listener
 
     def _any_subscribed(self, chan_id: ChannelId):
@@ -218,14 +220,15 @@
         self._logger.info("Starting server...")
         try:
             server = await serve(
                 self._handle_connection,
                 self.host,
                 self.port,
                 subprotocols=[Subprotocol("foxglove.websocket.v1")],
+                **self._server_kwargs,
             )
             self._opened.set_result(server)
         except asyncio.CancelledError:
             self._logger.info("Canceled during server startup")
             return
 
         for sock in server.sockets or []:
```

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket/server/client_state.py` & `foxglove-websocket-0.1.1/src/foxglove_websocket/server/client_state.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket/types.py` & `foxglove-websocket-0.1.1/src/foxglove_websocket/types.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/PKG-INFO` & `foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-websocket
-Version: 0.1.0
+Version: 0.1.1
 Summary: Foxglove WebSocket server
 Home-page: https://github.com/foxglove/ws-protocol
 License: MIT
 Project-URL: GitHub Issues, https://github.com/foxglove/ws-protocol/issues
 Project-URL: Foxglove Studio Documentation, https://foxglove.dev/docs
 Keywords: foxglove,websocket,robotics,ros,ros2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/SOURCES.txt` & `foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/tests/test_client_state.py` & `foxglove-websocket-0.1.1/tests/test_client_state.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.0/tests/test_server.py` & `foxglove-websocket-0.1.1/tests/test_server.py`

 * *Files identical despite different names*

