# Comparing `tmp/gama_client-1.1.2.tar.gz` & `tmp/gama_client-1.1.3.tar.gz`

## Comparing `gama_client-1.1.2.tar` & `gama_client-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/__init__.py
--rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/base_client.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/command_types.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 gama_client-1.1.2/gama_client/message_types.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 gama_client-1.1.2/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 gama_client-1.1.2/LICENSE
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 gama_client-1.1.2/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 gama_client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 gama_client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/__init__.py
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/base_client.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/command_types.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/message_types.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 gama_client-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 gama_client-1.1.3/LICENSE
+-rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 gama_client-1.1.3/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 gama_client-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 gama_client-1.1.3/PKG-INFO
```

### Comparing `gama_client-1.1.2/gama_client/base_client.py` & `gama_client-1.1.3/gama_client/base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,45 +29,48 @@
         self.port = port
         self.message_handler = message_handler
         self.socket_id = ""
         self.socket = None
         self.event_loop = asyncio.get_running_loop()
         self.connection_future = None
 
-    async def connect(self, set_socket_id: bool = True):
+    async def connect(self, set_socket_id: bool = True, ping_interval: float = 20, ping_timeout: float = 20):
         """
         Tries to connect the client to gama-server using the url and port given at the initialization.
         Once the connection is done it runs **start_listening_loop** and sets **socket_id** if **set_socket_id**
         is True
 
         :param set_socket_id: If true, the listening loop will filter out the messages of type ConnectionSuccessful and
             the GamaClient will set its socket_id itself. If set to false, the users will have to set the client's
             socket_id field themselves in the message_handler function
+        :param ping_interval: The interval between each ping send to keepalive the connection, use None to deactivate this behaviour
+        :param ping_timeout: The time the client is waiting for an answer to the ping sent before declaring that the connection is lost (part of the keepalive loop)
         :returns: Returns either once the listening loop starts if set_socket_id is False or when a socket_id is
             sent by gama-server
         :raise Exception: Can throw exceptions in case of connection problems.
         """
         self.connection_future = self.event_loop.create_future()
-        self.socket = await websockets.connect(f"ws://{self.url}:{self.port}")
+        self.socket = await websockets.connect(f"ws://{self.url}:{self.port}", ping_interval=ping_interval, ping_timeout=ping_timeout)
         self.event_loop.create_task(self.start_listening_loop(set_socket_id))
         if set_socket_id:
             self.socket_id = await self.connection_future
 
-    async def start_listening_loop(self, handle_connection_message: bool):
+    async def start_listening_loop(self, handle_connection_message: bool, timeout: float = 20.0):
         """
         Internal method. It starts an infinite listening loop that will transmit gama-server's messages to the
         message_handler function
 
         :param handle_connection_message: If set to true, the function checks for messages of type ConnectionSuccessful
             and will set its content field as the result of connection_future that is used in connect to wait for the socket_id
+        :param timeout: timeout for reading the next message
         :return: Never returns
         """
         while True:
             try:
-                mess = await self.socket.recv()
+                mess = await asyncio.wait_for(self.socket.recv(), timeout=timeout)
                 try:
                     js = json.loads(mess)
                     if handle_connection_message \
                         and "type" in js \
                         and "content" in js \
                         and js["type"] == MessageTypes.ConnectionSuccessful.value:
```

### Comparing `gama_client-1.1.2/gama_client/message_types.py` & `gama_client-1.1.3/gama_client/message_types.py`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.2/.gitignore` & `gama_client-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.2/LICENSE` & `gama_client-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.2/README.md` & `gama_client-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Gama client
- Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the multi-agent modeling platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
+ Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the modeling and simulation platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
 This wrapper will take care of the connection with gama-server and of sending properly formatted requests to gama-server. It is made to fit the asynchronous nature of gama-server and thus makes it possible to handle multiple simulations at the same time, but the counterpart is that the users will still have to manage what to do with the received messages (command confirmation, simulation output, errors etc.) by themselves. We provide a working example that shows the architecture you can deploy if you still want to have a sequential execution.
 
 # Installation
 In your python environment, install the gama-client package with the command:
 
 ```
 pip install gama-client
```

### Comparing `gama_client-1.1.2/pyproject.toml` & `gama_client-1.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "gama_client"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Baptiste Lesquoy", email="baptistelesquoy@protonmail.com" },
 ]
 description = "A python library to interact with Gama server"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `gama_client-1.1.2/PKG-INFO` & `gama_client-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_client
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python library to interact with Gama server
 Project-URL: Homepage, https://github.com/gama-platform/Gama-client-python
 Project-URL: Bug Tracker, https://github.com/gama-platform/Gama-client-python/issues
 Author-email: Baptiste Lesquoy <baptistelesquoy@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Baptiste Lesquoy
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: websockets~=10.3
 Description-Content-Type: text/markdown
 
 # Gama client
- Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the multi-agent modeling platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
+ Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the modeling and simulation platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
 This wrapper will take care of the connection with gama-server and of sending properly formatted requests to gama-server. It is made to fit the asynchronous nature of gama-server and thus makes it possible to handle multiple simulations at the same time, but the counterpart is that the users will still have to manage what to do with the received messages (command confirmation, simulation output, errors etc.) by themselves. We provide a working example that shows the architecture you can deploy if you still want to have a sequential execution.
 
 # Installation
 In your python environment, install the gama-client package with the command:
 
 ```
 pip install gama-client
```

