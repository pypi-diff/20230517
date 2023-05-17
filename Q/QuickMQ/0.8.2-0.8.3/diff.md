# Comparing `tmp/QuickMQ-0.8.2.tar.gz` & `tmp/QuickMQ-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickMQ-0.8.2.tar", last modified: Mon May 15 17:20:31 2023, max compression
+gzip compressed data, was "QuickMQ-0.8.3.tar", last modified: Wed May 17 15:19:02 2023, max compression
```

## Comparing `QuickMQ-0.8.2.tar` & `QuickMQ-0.8.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1071 2023-02-17 21:40:50.000000 QuickMQ-0.8.2/LICENSE
--rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/PKG-INFO
--rw-r--r--   0 mdrexler (29089) domain users   (700)     4522 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/README.md
--rw-r--r--   0 mdrexler (29089) domain users   (700)      295 2023-03-22 22:41:02.000000 QuickMQ-0.8.2/pyproject.toml
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1506 2023-05-15 17:20:31.309718 QuickMQ-0.8.2/setup.cfg
--rw-r--r--   0 mdrexler (29089) domain users   (700)      154 2023-04-28 15:01:45.000000 QuickMQ-0.8.2/setup.py
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.306717 QuickMQ-0.8.2/src/
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.307717 QuickMQ-0.8.2/src/QuickMQ.egg-info/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     6038 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/PKG-INFO
--rw-r--r--   0 mdrexler (29089) domain users   (700)      686 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/SOURCES.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)        1 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/dependency_links.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)       50 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/entry_points.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)      113 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/requires.txt
--rw-r--r--   0 mdrexler (29089) domain users   (700)        8 2023-05-15 17:20:31.000000 QuickMQ-0.8.2/src/QuickMQ.egg-info/top_level.txt
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/src/quickmq/
--rw-r--r--   0 mdrexler (29089) domain users   (700)      511 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/src/quickmq/__init__.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     4791 2023-05-15 17:19:27.000000 QuickMQ-0.8.2/src/quickmq/__main__.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)       82 2023-05-15 17:20:27.000000 QuickMQ-0.8.2/src/quickmq/__version__.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1469 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/src/quickmq/api.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     5108 2023-05-15 13:58:38.000000 QuickMQ-0.8.2/src/quickmq/config.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)    10394 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/src/quickmq/connection.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)       39 2023-03-03 20:16:51.000000 QuickMQ-0.8.2/src/quickmq/consume.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1968 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/src/quickmq/editor.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)      462 2023-03-03 21:47:49.000000 QuickMQ-0.8.2/src/quickmq/exceptions.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1193 2023-04-28 14:28:11.000000 QuickMQ-0.8.2/src/quickmq/message.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2545 2023-04-28 14:28:41.000000 QuickMQ-0.8.2/src/quickmq/publish.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)        0 2023-01-13 22:27:07.000000 QuickMQ-0.8.2/src/quickmq/py.typed
--rw-r--r--   0 mdrexler (29089) domain users   (700)     3394 2023-04-28 14:27:52.000000 QuickMQ-0.8.2/src/quickmq/session.py
-drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-15 17:20:31.308718 QuickMQ-0.8.2/test/
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2446 2023-04-28 14:26:29.000000 QuickMQ-0.8.2/test/test_api.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1127 2023-04-28 14:57:16.000000 QuickMQ-0.8.2/test/test_cli.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1820 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/test/test_config.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     2675 2023-03-03 21:47:49.000000 QuickMQ-0.8.2/test/test_connection.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)      535 2023-03-29 21:03:07.000000 QuickMQ-0.8.2/test/test_message.py
--rw-r--r--   0 mdrexler (29089) domain users   (700)     1437 2023-03-03 20:12:14.000000 QuickMQ-0.8.2/test/test_session.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-17 15:19:02.922692 QuickMQ-0.8.3/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1071 2023-02-17 21:40:50.000000 QuickMQ-0.8.3/LICENSE
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     6036 2023-05-17 15:19:02.923692 QuickMQ-0.8.3/PKG-INFO
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     4520 2023-05-17 15:15:59.000000 QuickMQ-0.8.3/README.md
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      295 2023-03-22 22:41:02.000000 QuickMQ-0.8.3/pyproject.toml
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1529 2023-05-17 15:19:02.923692 QuickMQ-0.8.3/setup.cfg
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      154 2023-04-28 15:01:45.000000 QuickMQ-0.8.3/setup.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-17 15:19:02.919692 QuickMQ-0.8.3/src/
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-17 15:19:02.921692 QuickMQ-0.8.3/src/QuickMQ.egg-info/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     6036 2023-05-17 15:19:02.000000 QuickMQ-0.8.3/src/QuickMQ.egg-info/PKG-INFO
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      686 2023-05-17 15:19:02.000000 QuickMQ-0.8.3/src/QuickMQ.egg-info/SOURCES.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        1 2023-05-17 15:19:02.000000 QuickMQ-0.8.3/src/QuickMQ.egg-info/dependency_links.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       50 2023-05-17 15:19:02.000000 QuickMQ-0.8.3/src/QuickMQ.egg-info/entry_points.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      113 2023-05-17 15:19:02.000000 QuickMQ-0.8.3/src/QuickMQ.egg-info/requires.txt
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        8 2023-05-17 15:19:02.000000 QuickMQ-0.8.3/src/QuickMQ.egg-info/top_level.txt
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-17 15:19:02.922692 QuickMQ-0.8.3/src/quickmq/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      512 2023-05-15 18:43:36.000000 QuickMQ-0.8.3/src/quickmq/__init__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     4791 2023-05-16 19:26:13.000000 QuickMQ-0.8.3/src/quickmq/__main__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       82 2023-05-17 15:18:35.000000 QuickMQ-0.8.3/src/quickmq/__version__.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1469 2023-04-28 14:26:29.000000 QuickMQ-0.8.3/src/quickmq/api.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     5108 2023-05-15 13:58:38.000000 QuickMQ-0.8.3/src/quickmq/config.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)    12312 2023-05-17 15:11:15.000000 QuickMQ-0.8.3/src/quickmq/connection.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)       39 2023-03-03 20:16:51.000000 QuickMQ-0.8.3/src/quickmq/consume.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1988 2023-05-16 19:33:00.000000 QuickMQ-0.8.3/src/quickmq/editor.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      462 2023-03-03 21:47:49.000000 QuickMQ-0.8.3/src/quickmq/exceptions.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1192 2023-05-17 15:00:25.000000 QuickMQ-0.8.3/src/quickmq/message.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2578 2023-05-17 15:03:09.000000 QuickMQ-0.8.3/src/quickmq/publish.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)        0 2023-01-13 22:27:07.000000 QuickMQ-0.8.3/src/quickmq/py.typed
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     3354 2023-05-17 15:00:25.000000 QuickMQ-0.8.3/src/quickmq/session.py
+drwxr-xr-x   0 mdrexler (29089) domain users   (700)        0 2023-05-17 15:19:02.922692 QuickMQ-0.8.3/test/
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2446 2023-04-28 14:26:29.000000 QuickMQ-0.8.3/test/test_api.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1240 2023-05-17 15:00:25.000000 QuickMQ-0.8.3/test/test_cli.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1820 2023-03-29 21:03:07.000000 QuickMQ-0.8.3/test/test_config.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     2667 2023-05-17 15:00:25.000000 QuickMQ-0.8.3/test/test_connection.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)      535 2023-03-29 21:03:07.000000 QuickMQ-0.8.3/test/test_message.py
+-rw-r--r--   0 mdrexler (29089) domain users   (700)     1437 2023-03-03 20:12:14.000000 QuickMQ-0.8.3/test/test_session.py
```

### Comparing `QuickMQ-0.8.2/LICENSE` & `QuickMQ-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.2/PKG-INFO` & `QuickMQ-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickMQ
-Version: 0.8.2
+Version: 0.8.3
 Summary: A simple RabbitMQ client
 Home-page: https://gitlab.ssec.wisc.edu/mdrexler/easymq
 Author: Max Drexler
 Author-email: mndrexler@wisc.edu
 License: MIT
 Keywords: rabbitmq,message publisher,amqp message
 Classifier: Programming Language :: Python :: 3
@@ -14,17 +14,15 @@
 License-File: LICENSE
 
 # QuickMQ
 
 An easy-to-use RabbitMQ client.
 
 [![pipeline status](https://gitlab.ssec.wisc.edu/mdrexler/easymq/badges/main/pipeline.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/commits/main)
-
 [![coverage report](https://gitlab.ssec.wisc.edu/mdrexler/easymq/badges/main/coverage.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/commits/main)
-
 [![Latest Release](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/badges/release.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/releases)
 
 
 ## Table of Contents
 
 * [Description](#description)
 * [Installation](#installation)
```

### Comparing `QuickMQ-0.8.2/README.md` & `QuickMQ-0.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # QuickMQ
 
 An easy-to-use RabbitMQ client.
 
 [![pipeline status](https://gitlab.ssec.wisc.edu/mdrexler/easymq/badges/main/pipeline.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/commits/main)
-
 [![coverage report](https://gitlab.ssec.wisc.edu/mdrexler/easymq/badges/main/coverage.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/commits/main)
-
 [![Latest Release](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/badges/release.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/releases)
 
 
 ## Table of Contents
 
 * [Description](#description)
 * [Installation](#installation)
```

### Comparing `QuickMQ-0.8.2/setup.cfg` & `QuickMQ-0.8.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 version = attr: quickmq.__version__.__version__
 url = https://gitlab.ssec.wisc.edu/mdrexler/easymq
 description = A simple RabbitMQ client
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = Max Drexler
 author_email = mndrexler@wisc.edu
+python_version = 3.6.8
 keywords = rabbitmq, message publisher, amqp message
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `QuickMQ-0.8.2/src/QuickMQ.egg-info/PKG-INFO` & `QuickMQ-0.8.3/src/QuickMQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickMQ
-Version: 0.8.2
+Version: 0.8.3
 Summary: A simple RabbitMQ client
 Home-page: https://gitlab.ssec.wisc.edu/mdrexler/easymq
 Author: Max Drexler
 Author-email: mndrexler@wisc.edu
 License: MIT
 Keywords: rabbitmq,message publisher,amqp message
 Classifier: Programming Language :: Python :: 3
@@ -14,17 +14,15 @@
 License-File: LICENSE
 
 # QuickMQ
 
 An easy-to-use RabbitMQ client.
 
 [![pipeline status](https://gitlab.ssec.wisc.edu/mdrexler/easymq/badges/main/pipeline.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/commits/main)
-
 [![coverage report](https://gitlab.ssec.wisc.edu/mdrexler/easymq/badges/main/coverage.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/commits/main)
-
 [![Latest Release](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/badges/release.svg)](https://gitlab.ssec.wisc.edu/mdrexler/easymq/-/releases)
 
 
 ## Table of Contents
 
 * [Description](#description)
 * [Installation](#installation)
```

### Comparing `QuickMQ-0.8.2/src/QuickMQ.egg-info/SOURCES.txt` & `QuickMQ-0.8.3/src/QuickMQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.2/src/quickmq/__main__.py` & `QuickMQ-0.8.3/src/quickmq/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         except KeyboardInterrupt:
             return
 
 
 def print_quickmq_info() -> None:
     print(title_str)
     print()
-    print(f'version : {__version__}')
-    print(f'user config file : {CFG_FILE_PATH}')
+    print(f"version : {__version__}")
+    print(f"user config file : {CFG_FILE_PATH}")
 
 
 def parse_arguments(
     argv: Optional[List[str]] = None,
 ) -> Tuple[argparse.Namespace, argparse.ArgumentParser]:
     """Parses
 
@@ -164,15 +164,15 @@
             servers=args.servers,
             route=args.key,
         )
     elif sub_command == "consume":
         raise NotImplementedError(
             "command line consumption behavior is not yet implemented!"
         )
-    elif sub_command == 'info':
+    elif sub_command == "info":
         print_quickmq_info()
     else:
         if getattr(args, "version"):
             print(version_str)
         else:
             parser.print_usage()
     return 0
```

### Comparing `QuickMQ-0.8.2/src/quickmq/api.py` & `QuickMQ-0.8.3/src/quickmq/api.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.2/src/quickmq/config.py` & `QuickMQ-0.8.3/src/quickmq/config.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.2/src/quickmq/connection.py` & `QuickMQ-0.8.3/src/quickmq/connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,56 +11,132 @@
 from pika.exceptions import (
     AMQPConnectionError,
     AuthenticationError,
     ConnectionClosed,
     ProbableAccessDeniedError,
     ProbableAuthenticationError,
     StreamLostError,
+    ConnectionWrongStateError
 )
 
 from .config import CURRENT_CONFIG
 from .exceptions import NotAuthenticatedError
 
 LOGGER = logging.getLogger("quickmq")
 
 
+def create_default_channel(connection: pika.BlockingConnection) -> BlockingChannel:
+    """Creates a default channel on the given connection and returns a reference
+
+    Args:
+        connection (pika.BlockingConnection): connection to create a channel on
+
+    Raises:
+        ConnectionError: if the connection is currently closed
+
+    Returns:
+        BlockingChannel: a reference to the created channel
+    """
+    if connection.is_closed:
+        raise ConnectionError(
+            f"Cannot setup channels on {connection}, the connection is closed"
+        )
+    non_confirm_channel = connection.channel()
+    return non_confirm_channel
+
+
+def create_confirm_channel(connection: pika.BlockingConnection) -> BlockingChannel:
+    """Creates a confirmed channel on the given connection and returns a reference
+
+    Args:
+        connection (pika.BlockingConnection): connection to create a channel on
+
+    Raises:
+        ConnectionError: if the connection is currently closed
+
+    Returns:
+        BlockingChannel: a reference to the created channel
+    """
+    if connection.is_closed:
+        raise ConnectionError(
+            f"Cannot setup channels on {connection}, the connection is closed"
+        )
+    confirm_channel = connection.channel()
+    confirm_channel.confirm_delivery()
+    return confirm_channel
+
+
+def create_connection(
+    connection_parameters: pika.ConnectionParameters,
+) -> pika.BlockingConnection:
+    """Creates a connection and raises necessary errors
+
+    Args:
+        connection_parameters (pika.ConnectionParameters): parameters to create connection with
+
+    Raises:
+        ConnectionError: The server doesn't exist
+        NotAuthenticatedError: user isn't authenticated to connect to the server
+
+    Returns:
+        pika.BlockingConnection: The connection to the server
+    """
+    try:
+        connection = pika.BlockingConnection(parameters=connection_parameters)
+        LOGGER.info(f"Connection established to {connection_parameters.host}")
+        return connection
+    except (socket.gaierror, socket.herror) as e:
+        LOGGER.error(f"Socket error connecting to {connection_parameters.host}: {e}")
+        raise ConnectionError("Could not connect to server")
+    except (
+        AuthenticationError,
+        ProbableAccessDeniedError,
+        ProbableAuthenticationError,
+    ):
+        LOGGER.error(
+            f"Not authenticated to connect to {connection_parameters.host} "
+            f"with username {connection_parameters.credentials.username}"
+        )
+        raise NotAuthenticatedError(
+            f"Not authenticated to connect to server {connection_parameters.host}"
+        )
+
+
 class ServerConnection(threading.Thread):
     def __init__(
         self,
         host: str,
         port: Optional[int] = None,
         vhost: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
     ) -> None:
         super().__init__(
             None, None, f"Thread-MQConnection({host})", (), {}, daemon=True
         )
-
-        self._running = False
-        self._callback_queue: queue.Queue = queue.Queue()
-        self._connection: Optional[pika.BlockingConnection] = None
-        self._channel: Optional[BlockingChannel] = None
-        self._confirmed_channel: BlockingChannel = None
         self._con_params = pika.ConnectionParameters(
             host=host,
             port=port or CURRENT_CONFIG.get("RABBITMQ_PORT"),
             virtual_host=vhost or "/",
             credentials=pika.PlainCredentials(
                 username or CURRENT_CONFIG.get("DEFAULT_USER"),
                 password or CURRENT_CONFIG.get("DEFAULT_PASS"),
             ),
         )
         LOGGER.info(
-            f"Setting up connection to '{host}' with username \
-'{self._con_params.credentials.username}' on port \
-'{self._con_params.port}' and vhost '{self._con_params.virtual_host}'"
+            f"Setting up connection to '{host}' with username "
+            f"'{self._con_params.credentials.username}' on port "
+            f"'{self._con_params.port}' and vhost '{self._con_params.virtual_host}'"
         )
-        self.connect()
-        self.start()
+
+        self._running = False
+        self._callback_queue: queue.Queue = queue.Queue()
+        self._connection: pika.BlockingConnection = create_connection(self._con_params)
+        self._default_channel = create_default_channel(self._connection)
+        self._confirmed_channel = create_confirm_channel(self._connection)
 
     @property
     def user(self) -> str:
         return self._con_params.credentials.username
 
     @property
     def port(self) -> int:
@@ -72,27 +148,28 @@
 
     @property
     def server(self) -> str:
         return self._con_params.host
 
     @property
     def connected(self) -> bool:
-        return self._running and not self._connection.is_closed
+        return self._running and self._connection.is_open
 
     @contextmanager
     def wrapper(self):
         if not self._running:
             LOGGER.error(f"Connection to {self.server} closed")
             raise ConnectionAbortedError(f"Connection to {self.server} closed")
         try:
             yield
         finally:
-            if self._channel.is_closed or self._confirmed_channel.is_closed:
-                LOGGER.info(f"Re-establishing channels on connection to {self.server}")
-                self._channel_setup()
+            if self._default_channel.is_closed:
+                self._default_channel = create_default_channel(self._connection)
+            if self._confirmed_channel.is_closed:
+                self._confirmed_channel = create_confirm_channel(self._connection)
 
     def run(self) -> None:
         self._running = True
         while self._running:
             try:
                 self._connection.process_data_events(0.005)
             except (
@@ -112,69 +189,48 @@
 
     def _on_connection_error(self, exception: BaseException) -> None:
         LOGGER.error(
             f"Error in connection to {self.server}: {exception}, closing connection"
         )
         self.close()
 
-    def connect(self) -> None:
-        if self._connection is not None and self._connection.is_open:
-            self._channel_setup()
-        try:
-            self._connection = pika.BlockingConnection(parameters=self._con_params)
-            self._channel_setup()
-        except (socket.gaierror, socket.herror) as e:
-            LOGGER.error(f"Socket error connecting to {self.server}: {e}")
-            raise ConnectionError("Could not connect to server")
-        except (
-            AuthenticationError,
-            ProbableAccessDeniedError,
-            ProbableAuthenticationError,
-        ):
-            LOGGER.error(
-                f"Not authenticated to connect to {self.server} with username {self.user}"
-            )
-            raise NotAuthenticatedError(
-                f"Not authenticated to connect to server {self.server}"
-            )
-        LOGGER.info(f"Connection established to {self.server}")
-
     def _close(self) -> None:
+        if self._connection is None:
+            return
         self._connection.process_data_events()
-        if self._connection is not None and self._connection.is_open:
+        if self._connection.is_open:
             self._connection.close()
         LOGGER.info(f"Closed connection to {self.server}")
 
     def close(self) -> None:
         LOGGER.info(f"Closing connection to {self.server}")
         self._running = False
-        if self._connection is None or self._connection.is_closed:
+        if self._connection.is_closed:
             LOGGER.info(f"Closed connection to {self.server}")
             return
         self.add_callback(self._close)
 
-    def _channel_setup(self) -> None:
-        if self._channel is None or self._channel.is_closed:
-            self._channel = self._connection.channel()
-        if self._confirmed_channel is None or self._confirmed_channel.is_closed:
-            self._confirmed_channel = self._connection.channel()
-            self._confirmed_channel.confirm_delivery()
-
     def add_callback(self, callback: Callable, *args, **kwargs) -> None:
         LOGGER.debug(
             f"Adding callback on {self.server}: {callback}, args: {args}, kwargs: {kwargs}"
         )
         LOGGER.debug(
             f"Currently {self._callback_queue.qsize()} callbacks in queue for {self.server}"
         )
         self._callback_queue.put((callback, args, kwargs))
 
     def __del__(self) -> None:
-        self.close()
-        del self._connection
+        """Close connection at garbage collection
+        """
+        if not hasattr(self, '_connection'):  # class attributes not gauranteed
+            return
+        try:
+            self._connection.close(500, 'Garbage collection')
+        except ConnectionWrongStateError:
+            return
 
     def __eq__(self, _obj: Any) -> bool:
         if isinstance(_obj, str):
             return _obj == self.server
         return super().__eq__(_obj)
 
     def __hash__(self) -> int:
@@ -192,19 +248,18 @@
         self,
         host: str,
         port: Optional[int] = None,
         vhost: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
     ) -> None:
+        super().__init__(host, port, vhost, username, password)
         self._reconnecting = threading.Event()
         self._reconnecting.set()  # not currently reconnecting, threads shouldn't wait
 
-        super().__init__(host, port, vhost, username, password)
-
     @property
     def is_reconnecting(self) -> bool:
         return not self._reconnecting.is_set()
 
     def close(self) -> None:
         self._running = False
         self.wait_for_reconnect()
@@ -226,18 +281,20 @@
                     {CURRENT_CONFIG.get('RECONNECT_TRIES')} attempt(s), exiting..."
                 )
                 raise RuntimeWarning(
                     f"Could not reconnect to {self.server} after \
                     {CURRENT_CONFIG.get('RECONNECT_TRIES')} attempt(s), exiting..."
                 )
             try:
-                self.connect()
+                self._connection = create_connection(self._con_params)
+                if self._connection is None:
+                    raise AMQPConnectionError("Connection not established")
                 if self._connection.is_open:
                     break
-            except AMQPConnectionError:
+            except (AMQPConnectionError, ConnectionError):
                 pass
             if self._running:
                 LOGGER.debug(
                     f"Waiting {CURRENT_CONFIG.get('RECONNECT_DELAY')} seconds before next reconnect attempt"
                 )
                 time.sleep(CURRENT_CONFIG.get("RECONNECT_DELAY"))
             if tries < 0:
@@ -257,45 +314,43 @@
     def __init__(self) -> None:
         self._connections: List[ServerConnection] = []
 
     @property
     def connections(self) -> List[ServerConnection]:
         return self._connections
 
-    def _remove_connection(self, server: str) -> None:
-        try:
-            con_index = self._connections.index(server)
-        except ValueError:
-            LOGGER.debug(f"{server} not in current connection pool")
-            return
-        connection = self._connections.pop(con_index)
-        connection.close()
+    def remove_server(self, server: str) -> bool:
+        for serv in self._connections.copy():
+            if serv.server == server:
+                LOGGER.info(f'Found {serv.server} in pool, removing')
+                serv.close()
+                self._connections.remove(serv)
+                return True
+        return False
 
     def add_server(
         self, new_server: str, auth: Tuple[Optional[str], Optional[str]] = (None, None)
     ) -> None:
-        self._remove_connection(new_server)  # Remove connection if it already exists
-        self._connections.append(
-            ReconnectConnection(
+        self.remove_server(new_server)  # Remove connection if it already exists
+        new_con = ReconnectConnection(
                 host=new_server,
                 username=auth[0],
                 password=auth[1],
             )
-        )
+        self._connections.append(new_con)
+        new_con.start()
 
     def add_connection(self, new_conn: ServerConnection) -> None:
-        self._remove_connection(new_conn.server)
+        self.remove_server(new_conn.server)
         self._connections.append(new_conn)
 
-    def remove_server(self, server: str) -> None:
-        self._remove_connection(server)
-
     def remove_all(self) -> None:
-        for con in self._connections:
-            self._remove_connection(con.server)
+        for con in self._connections.copy():
+            LOGGER.debug(f"removing {con.server} from connection pool")
+            self.remove_server(con.server)
 
     def __len__(self) -> int:
         return len(self._connections)
 
     def __iter__(self):
         return iter(self._connections)
```

### Comparing `QuickMQ-0.8.2/src/quickmq/editor.py` & `QuickMQ-0.8.3/src/quickmq/editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,26 +41,26 @@
         pass
 
     def exchange_unbind(
         self, destination: str, source: str, route_key: Optional[str] = None
     ) -> None:
         pass
 
-    def __exchange_check():
+    def __exchange_check(self):
         pass
 
     def exchange_check(
         self,
         exchange: str,
         exchange_type=ExchangeType.DIRECT,
         durable=False,
         auto_delete=False,
         internal=False,
     ) -> bool:
-        pass
+        return False
 
     def exchange_delete(self, exchange: str, if_unused=False) -> None:
         pass
 
     def queue_declare(
         self, queue: str, durable=False, exclusive=False, auto_delete=False
     ) -> None:
@@ -68,15 +68,15 @@
 
     def queue_delete(self, queue: str, if_unused=False, if_empty=False) -> None:
         pass
 
     def queue_check(
         self, queue: str, durable=False, exclusive=False, auto_delete=False
     ) -> bool:
-        pass
+        return False
 
     def queue_purge(self, queue: str) -> None:
         pass
 
     def queue_bind(
         self, queue: str, exchange: str, route_key: Optional[str] = None
     ) -> None:
```

### Comparing `QuickMQ-0.8.2/src/quickmq/message.py` & `QuickMQ-0.8.3/src/quickmq/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,11 +40,11 @@
 
 
 @dataclass
 class Packet:
     message: Message
     routing_key: str
     exchange: str
-    confirm: bool = False
+    confirm: bool = True
     properties: pika.BasicProperties = pika.BasicProperties(
         delivery_mode=1, content_type="application/json"
     )
```

### Comparing `QuickMQ-0.8.2/src/quickmq/publish.py` & `QuickMQ-0.8.3/src/quickmq/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,19 @@
         LOGGER.warning(f"Error detected while publishing: {self._publishing_err}")
         err = to_raise or self._publishing_err
         self._publishing_err = None
         raise err
 
     def _publish(self, connection: ServerConnection, packet: Packet) -> None:
         pub_channel = (
-            connection._confirmed_channel if packet.confirm else connection._channel
+            connection._confirmed_channel
+            if packet.confirm
+            else connection._default_channel
         )
+
         try:
             with connection.wrapper():
                 LOGGER.debug(
                     f"Connection to {connection.server} ready, attempting to publish to {packet.exchange} exchange"
                 )
                 pub_channel.basic_publish(
                     packet.exchange,
```

### Comparing `QuickMQ-0.8.2/src/quickmq/session.py` & `QuickMQ-0.8.3/src/quickmq/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,45 +14,46 @@
 from .connection import ConnectionPool
 from .message import Packet, Message
 from .config import CURRENT_CONFIG
 
 LOGGER = logging.getLogger("quickmq")
 
 
+def connection_required(func: Callable) -> Callable:
+    @wraps(func)
+    def check_conn(self, *args: Any, **kwargs: Any) -> Any:
+        if len(self.servers) > 0:
+            return func(self, *args, **kwargs)
+
+        try:
+            self.connect(CURRENT_CONFIG.get("DEFAULT_SERVER"))
+            return func(self, *args, **kwargs)
+        except (NotAuthenticatedError, ConnectionError, AttributeError) as e:
+            LOGGER.critical(f"Error when connecting to default server: {e}")
+            raise NotConnectedError(
+                f"Need to be connected to a server, "
+                f"could not connect to default '{CURRENT_CONFIG.get('DEFAULT_SERVER')}"
+            )
+
+    return check_conn
+
+
 class AmqpSession:
     def __init__(self) -> None:
         self._connections = ConnectionPool()
         self._publisher = AmqpPublisher()
 
     @property
     def servers(self) -> List[str]:
         return [con.server for con in self._connections]
 
     @property
     def pool(self) -> ConnectionPool:
         return self._connections
 
-    def connection_required(func: Callable) -> Callable:
-        @wraps(func)
-        def check_conn(self, *args: Any, **kwargs: Any) -> Any:
-            if len(self.servers) > 0:
-                return func(self, *args, **kwargs)
-
-            try:
-                self.connect(CURRENT_CONFIG.get("DEFAULT_SERVER"))
-                return func(self, *args, **kwargs)
-            except (NotAuthenticatedError, ConnectionError, AttributeError) as e:
-                LOGGER.critical(f"Error when connecting to default server: {e}")
-                raise NotConnectedError(
-                    f"Need to be connected to a server,\
-    could not connect to default '{CURRENT_CONFIG.get('DEFAULT_SERVER')}"
-                )
-
-        return check_conn
-
     @connection_required
     def publish(
         self,
         message: Union[Message, Any],
         key: Optional[str] = None,
         exchange: Optional[str] = None,
         confirm_delivery=True,
```

### Comparing `QuickMQ-0.8.2/test/test_api.py` & `QuickMQ-0.8.3/test/test_api.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.2/test/test_cli.py` & `QuickMQ-0.8.3/test/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from json import loads
 import subprocess
+import sys
 
 import pytest
 
 from quickmq import __version__
 
 
+def run_command(input: str) -> str:
+    if sys.version_info[1] < 7:
+        compl = subprocess.run(input.split(' '), stdout=subprocess.PIPE)
+    else:
+        compl = subprocess.run(input.split(' '), capture_output=True)
+    return str(compl.stdout, encoding='utf-8')
+
+
 def test_version():
-    vInfo = subprocess.run(['quickmq', '-V'], capture_output=True)
-    assert __version__ in str(vInfo.stdout, encoding='utf-8')
+    assert __version__ in run_command('quickmq -V')
 
 
 def test_usage():
-    info = subprocess.run(['quickmq'], capture_output=True)
-    assert 'usage' in str(info.stdout, encoding='utf-8')
+    assert 'usage' in run_command('quickmq')
 
 
 @pytest.mark.parametrize('exchange', ['amq.fanout'])
 def test_publish(create_listener):
-    subprocess.run(['quickmq', 'publish', '-s=localhost', '-e=amq.fanout', '-m=Hello'])
+    run_command('quickmq publish -s=localhost -e=amq.fanout -m=Hello')
     rcvd_bytes = create_listener.get_message(block=True)
     assert loads(rcvd_bytes) == 'Hello'
 
 
 @pytest.mark.parametrize('exchange', ['amq.fanout'])
 def test_publish_from_stdin(create_listener):
     proc = subprocess.Popen(['quickmq', 'publish', '-s=localhost', '-e=amq.fanout'], stdin=subprocess.PIPE)
     try:
-        proc.communicate(input=b'Hello', timeout=.1)
+        proc.communicate(input=b'Hello', timeout=1)
     except subprocess.TimeoutExpired:
         proc.kill()
-    rcvd_bytes = create_listener.get_message(block=False)
+    rcvd_bytes = create_listener.get_message(block=True)
     if rcvd_bytes is None:
         assert False
     assert loads(rcvd_bytes) == 'Hello'
```

### Comparing `QuickMQ-0.8.2/test/test_config.py` & `QuickMQ-0.8.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.2/test/test_connection.py` & `QuickMQ-0.8.3/test/test_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 def test_callback():
     evnt = threading.Event()
 
     def callback():
         evnt.set()
     connection = ServerConnection('localhost')
+    connection.start()
     connection.add_callback(callback)
     evnt.wait()
 
 
 def test_reconnect(disconnect_rabbitmq, restart_rabbitmq):
     quickmq.connect("localhost")
     assert len(_CURRENT_SESSION.pool.connections) == 1
@@ -79,26 +80,28 @@
 def test_connection_pool():
     event = threading.Event()
 
     def callbck(_connection):
         event.set()
 
     pool = ConnectionPool()
-    pool.add_connection(ReconnectConnection("localhost"))
+    con = ReconnectConnection("localhost")
+    con.start()
+    pool.add_connection(con)
     assert len(pool) == 1
     pool.add_callback(callbck)
     event.wait(2.0)
     assert event.is_set()
     pool.remove_all()
 
 
 @pytest.mark.skip
 def test_close_on_error(disconnect_rabbitmq, restart_rabbitmq, capsys):
     con = ServerConnection("localhost")
-    con.connect()  # this is automatically called, just for testing purposes
+    con.start()
     assert con.connected
     try:
         disconnect_rabbitmq()
         assert not con.connected
     finally:
         restart_rabbitmq()
         assert not con.connected
```

### Comparing `QuickMQ-0.8.2/test/test_message.py` & `QuickMQ-0.8.3/test/test_message.py`

 * *Files identical despite different names*

### Comparing `QuickMQ-0.8.2/test/test_session.py` & `QuickMQ-0.8.3/test/test_session.py`

 * *Files identical despite different names*

