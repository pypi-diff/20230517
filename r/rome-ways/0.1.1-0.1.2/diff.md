# Comparing `tmp/rome_ways-0.1.1.tar.gz` & `tmp/rome_ways-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rome_ways-0.1.1.tar", max compression
+gzip compressed data, was "rome_ways-0.1.2.tar", max compression
```

## Comparing `rome_ways-0.1.1.tar` & `rome_ways-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11357 2023-05-11 12:11:01.507301 rome_ways-0.1.1/LICENSE
--rw-r--r--   0        0        0     3733 2023-05-16 18:58:53.675406 rome_ways-0.1.1/README.md
--rw-r--r--   0        0        0      865 2023-05-16 19:03:19.003957 rome_ways-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      765 2023-05-15 12:02:13.821901 rome_ways-0.1.1/romeways/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:44:54.800383 rome_ways-0.1.1/romeways/src/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 13:07:43.213165 rome_ways-0.1.1/romeways/src/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 13:08:20.829356 rome_ways-0.1.1/romeways/src/core/abstract/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 14:15:44.190692 rome_ways-0.1.1/romeways/src/core/abstract/infrastructure/__init__.py
--rw-r--r--   0        0        0       38 2023-05-12 13:56:58.866680 rome_ways-0.1.1/romeways/src/core/abstract/infrastructure/queue_connector/__init__.py
--rw-r--r--   0        0        0      800 2023-05-15 13:38:14.930120 rome_ways-0.1.1/romeways/src/core/abstract/infrastructure/queue_connector/abstract.py
--rw-r--r--   0        0        0        0 2023-05-11 13:08:04.397273 rome_ways-0.1.1/romeways/src/core/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 14:16:08.206973 rome_ways-0.1.1/romeways/src/core/interfaces/infrastructure/__init__.py
--rw-r--r--   0        0        0       39 2023-05-12 17:20:32.364902 rome_ways-0.1.1/romeways/src/core/interfaces/infrastructure/queue_connector/__init__.py
--rw-r--r--   0        0        0      590 2023-05-14 12:00:59.588538 rome_ways-0.1.1/romeways/src/core/interfaces/infrastructure/queue_connector/interface.py
--rw-r--r--   0        0        0        0 2023-05-12 17:11:45.049844 rome_ways-0.1.1/romeways/src/core/interfaces/infrastructure/spawner/__init__.py
--rw-r--r--   0        0        0      231 2023-05-15 13:02:15.923737 rome_ways-0.1.1/romeways/src/core/interfaces/infrastructure/spawner/interface.py
--rw-r--r--   0        0        0        0 2023-05-11 13:36:16.783498 rome_ways-0.1.1/romeways/src/core/interfaces/service/__init__.py
--rw-r--r--   0        0        0       34 2023-05-13 15:22:50.871685 rome_ways-0.1.1/romeways/src/core/interfaces/service/chauffeur/__init__.py
--rw-r--r--   0        0        0      488 2023-05-16 12:42:33.729584 rome_ways-0.1.1/romeways/src/core/interfaces/service/chauffeur/interface.py
--rw-r--r--   0        0        0       30 2023-05-12 13:48:10.874337 rome_ways-0.1.1/romeways/src/core/interfaces/service/guide/__init__.py
--rw-r--r--   0        0        0      778 2023-05-13 16:46:51.626178 rome_ways-0.1.1/romeways/src/core/interfaces/service/guide/interface.py
--rw-r--r--   0        0        0        0 2023-05-11 13:09:56.301820 rome_ways-0.1.1/romeways/src/domain/__init__.py
--rw-r--r--   0        0        0       39 2023-05-15 12:02:13.805903 rome_ways-0.1.1/romeways/src/domain/exceptions/__init__.py
--rw-r--r--   0        0        0       43 2023-05-15 12:02:13.809903 rome_ways-0.1.1/romeways/src/domain/exceptions/exception.py
--rw-r--r--   0        0        0        0 2023-05-11 13:27:28.222781 rome_ways-0.1.1/romeways/src/domain/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 13:33:56.811479 rome_ways-0.1.1/romeways/src/domain/models/config/__init__.py
--rw-r--r--   0        0        0       42 2023-05-13 17:06:21.483290 rome_ways-0.1.1/romeways/src/domain/models/config/connector/__init__.py
--rw-r--r--   0        0        0      182 2023-05-16 18:58:53.675406 rome_ways-0.1.1/romeways/src/domain/models/config/connector/model.py
--rw-r--r--   0        0        0       29 2023-05-12 13:48:10.878338 rome_ways-0.1.1/romeways/src/domain/models/config/itinerary/__init__.py
--rw-r--r--   0        0        0      263 2023-05-16 18:08:29.151930 rome_ways-0.1.1/romeways/src/domain/models/config/itinerary/model.py
--rw-r--r--   0        0        0       29 2023-05-12 18:07:38.312466 rome_ways-0.1.1/romeways/src/domain/models/config/map/__init__.py
--rw-r--r--   0        0        0      375 2023-05-16 18:08:21.279965 rome_ways-0.1.1/romeways/src/domain/models/config/map/model.py
--rw-r--r--   0        0        0       38 2023-05-13 17:06:26.458455 rome_ways-0.1.1/romeways/src/domain/models/config/queue/__init__.py
--rw-r--r--   0        0        0      505 2023-05-16 18:58:53.675406 rome_ways-0.1.1/romeways/src/domain/models/config/queue/model.py
--rw-r--r--   0        0        0       27 2023-05-15 12:02:13.809903 rome_ways-0.1.1/romeways/src/domain/models/message/__init__.py
--rw-r--r--   0        0        0      761 2023-05-16 18:58:53.675406 rome_ways-0.1.1/romeways/src/domain/models/message/model.py
--rw-r--r--   0        0        0        0 2023-05-12 13:29:15.631498 rome_ways-0.1.1/romeways/src/infrastructure/__init__.py
--rw-r--r--   0        0        0       36 2023-05-12 18:07:38.316467 rome_ways-0.1.1/romeways/src/infrastructure/spawner/__init__.py
--rw-r--r--   0        0        0     1988 2023-05-16 12:33:53.069444 rome_ways-0.1.1/romeways/src/infrastructure/spawner/infrastructure.py
--rw-r--r--   0        0        0     1528 2023-05-16 14:00:00.056285 rome_ways-0.1.1/romeways/src/romeways.py
--rw-r--r--   0        0        0        0 2023-05-16 12:40:59.434398 rome_ways-0.1.1/romeways/src/service/__init__.py
--rw-r--r--   0        0        0       38 2023-05-13 15:22:50.799687 rome_ways-0.1.1/romeways/src/service/chauffeur/__init__.py
--rw-r--r--   0        0        0     4365 2023-05-16 18:58:53.675406 rome_ways-0.1.1/romeways/src/service/chauffeur/service.py
--rw-r--r--   0        0        0       34 2023-05-12 13:48:10.886341 rome_ways-0.1.1/romeways/src/service/guide/__init__.py
--rw-r--r--   0        0        0     2246 2023-05-16 12:36:22.442702 rome_ways-0.1.1/romeways/src/service/guide/service.py
--rw-r--r--   0        0        0     5637 1970-01-01 00:00:00.000000 rome_ways-0.1.1/setup.py
--rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 rome_ways-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 12:11:01.507301 rome_ways-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3748 2023-05-17 12:58:18.110563 rome_ways-0.1.2/README.md
+-rw-r--r--   0        0        0      865 2023-05-17 12:58:18.110563 rome_ways-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      766 2023-05-17 12:53:53.029044 rome_ways-0.1.2/romeways/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:44:54.800383 rome_ways-0.1.2/romeways/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:07:43.213165 rome_ways-0.1.2/romeways/src/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:08:20.829356 rome_ways-0.1.2/romeways/src/core/abstract/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:15:44.190692 rome_ways-0.1.2/romeways/src/core/abstract/infrastructure/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-12 13:56:58.866680 rome_ways-0.1.2/romeways/src/core/abstract/infrastructure/queue_connector/__init__.py
+-rw-r--r--   0        0        0      800 2023-05-15 13:38:14.930120 rome_ways-0.1.2/romeways/src/core/abstract/infrastructure/queue_connector/abstract.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:08:04.397273 rome_ways-0.1.2/romeways/src/core/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:16:08.206973 rome_ways-0.1.2/romeways/src/core/interfaces/infrastructure/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-12 17:20:32.364902 rome_ways-0.1.2/romeways/src/core/interfaces/infrastructure/queue_connector/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-14 12:00:59.588538 rome_ways-0.1.2/romeways/src/core/interfaces/infrastructure/queue_connector/interface.py
+-rw-r--r--   0        0        0        0 2023-05-12 17:11:45.049844 rome_ways-0.1.2/romeways/src/core/interfaces/infrastructure/spawner/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-15 13:02:15.923737 rome_ways-0.1.2/romeways/src/core/interfaces/infrastructure/spawner/interface.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:36:16.783498 rome_ways-0.1.2/romeways/src/core/interfaces/service/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-13 15:22:50.871685 rome_ways-0.1.2/romeways/src/core/interfaces/service/chauffeur/__init__.py
+-rw-r--r--   0        0        0      488 2023-05-16 12:42:33.729584 rome_ways-0.1.2/romeways/src/core/interfaces/service/chauffeur/interface.py
+-rw-r--r--   0        0        0       30 2023-05-12 13:48:10.874337 rome_ways-0.1.2/romeways/src/core/interfaces/service/guide/__init__.py
+-rw-r--r--   0        0        0      778 2023-05-13 16:46:51.626178 rome_ways-0.1.2/romeways/src/core/interfaces/service/guide/interface.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:09:56.301820 rome_ways-0.1.2/romeways/src/domain/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-15 12:02:13.805903 rome_ways-0.1.2/romeways/src/domain/exceptions/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-15 12:02:13.809903 rome_ways-0.1.2/romeways/src/domain/exceptions/exception.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:27:28.222781 rome_ways-0.1.2/romeways/src/domain/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:33:56.811479 rome_ways-0.1.2/romeways/src/domain/models/config/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-13 17:06:21.483290 rome_ways-0.1.2/romeways/src/domain/models/config/connector/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-16 19:05:26.928431 rome_ways-0.1.2/romeways/src/domain/models/config/connector/model.py
+-rw-r--r--   0        0        0       29 2023-05-12 13:48:10.878338 rome_ways-0.1.2/romeways/src/domain/models/config/itinerary/__init__.py
+-rw-r--r--   0        0        0      263 2023-05-16 18:08:29.151930 rome_ways-0.1.2/romeways/src/domain/models/config/itinerary/model.py
+-rw-r--r--   0        0        0       29 2023-05-12 18:07:38.312466 rome_ways-0.1.2/romeways/src/domain/models/config/map/__init__.py
+-rw-r--r--   0        0        0      375 2023-05-16 18:08:21.279965 rome_ways-0.1.2/romeways/src/domain/models/config/map/model.py
+-rw-r--r--   0        0        0       38 2023-05-13 17:06:26.458455 rome_ways-0.1.2/romeways/src/domain/models/config/queue/__init__.py
+-rw-r--r--   0        0        0      505 2023-05-16 19:05:26.928431 rome_ways-0.1.2/romeways/src/domain/models/config/queue/model.py
+-rw-r--r--   0        0        0       27 2023-05-15 12:02:13.809903 rome_ways-0.1.2/romeways/src/domain/models/message/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-16 19:05:26.928431 rome_ways-0.1.2/romeways/src/domain/models/message/model.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:29:15.631498 rome_ways-0.1.2/romeways/src/infrastructure/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-12 18:07:38.316467 rome_ways-0.1.2/romeways/src/infrastructure/spawner/__init__.py
+-rw-r--r--   0        0        0     1988 2023-05-16 12:33:53.069444 rome_ways-0.1.2/romeways/src/infrastructure/spawner/infrastructure.py
+-rw-r--r--   0        0        0     1528 2023-05-16 14:00:00.056285 rome_ways-0.1.2/romeways/src/romeways.py
+-rw-r--r--   0        0        0        0 2023-05-16 12:40:59.434398 rome_ways-0.1.2/romeways/src/service/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-13 15:22:50.799687 rome_ways-0.1.2/romeways/src/service/chauffeur/__init__.py
+-rw-r--r--   0        0        0     4365 2023-05-16 19:05:26.928431 rome_ways-0.1.2/romeways/src/service/chauffeur/service.py
+-rw-r--r--   0        0        0       34 2023-05-12 13:48:10.886341 rome_ways-0.1.2/romeways/src/service/guide/__init__.py
+-rw-r--r--   0        0        0     2246 2023-05-16 12:36:22.442702 rome_ways-0.1.2/romeways/src/service/guide/service.py
+-rw-r--r--   0        0        0     5653 1970-01-01 00:00:00.000000 rome_ways-0.1.2/setup.py
+-rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 rome_ways-0.1.2/PKG-INFO
```

### Comparing `rome_ways-0.1.1/LICENSE` & `rome_ways-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/README.md` & `rome_ways-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -87,35 +87,36 @@
 
 ## Spawn a process
 
 Romeways can run each connector in a separate process or in async workers for that use the parameter `spawn_process` to configure that.
 
 # Example
 
-For this example we are using the extra memory
+For this example we are using the extra package `memory`
 
 ```python
 from multiprocessing import Queue
 
 import romeways
 
+# Config the connector
+queue = Queue()
+
 # Create a queue config
 config_q = romeways.MemoryQueueConfig(
-    connector_name="memory-dev1"
+    connector_name="memory-dev1", 
+    queue=queue
 )
 
 # Register a controller/consumer for the queue name
 @romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)
 async def controller(message: romeways.Message):
     print(message)
 
-# Config the connector
-queue = Queue()
-
-config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1", queue=queue)
+config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1")
 
 # Register a connector
 romeways.connector_register(
     connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True
 )
 
 ```
```

### Comparing `rome_ways-0.1.1/pyproject.toml` & `rome_ways-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "rome-ways"
-version = "0.1.1"
+version = "0.1.2"
 description = "A queue framework"
 authors = ["Marco Sievers de Almeida Ximit Gaia <im.ximit@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     {include = "romeways"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 meeseeks-singleton = "^0.4.2"
-romeways_memory_queue = { version = "^0.1.0", optional = true}
+romeways_memory_queue = { version = "^0.2.0", optional = true}
 
 [tool.poetry.extras]
 memory = ["romeways_memory_queue"]
 
 [tool.poetry.urls]
 homepage = "https://github.com/CenturyBoys/romeways"
 repository = "https://github.com/CenturyBoys/romeways"
```

### Comparing `rome_ways-0.1.1/romeways/__init__.py` & `rome_ways-0.1.2/romeways/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "AQueueConnector",
     "ResendException",
     "Message",
 ]
 
 # Memory queue extra
 try:
+
     from romeways_memory_queue import (
         MemoryConnectorConfig,
         MemoryQueueConnector,
         MemoryQueueConfig,
     )
 
     __all__ += ("MemoryConnectorConfig", "MemoryQueueConnector", "MemoryQueueConfig")
```

### Comparing `rome_ways-0.1.1/romeways/src/core/abstract/infrastructure/queue_connector/abstract.py` & `rome_ways-0.1.2/romeways/src/core/abstract/infrastructure/queue_connector/abstract.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/romeways/src/core/interfaces/infrastructure/queue_connector/interface.py` & `rome_ways-0.1.2/romeways/src/core/interfaces/infrastructure/queue_connector/interface.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/romeways/src/core/interfaces/service/guide/interface.py` & `rome_ways-0.1.2/romeways/src/core/interfaces/service/guide/interface.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/romeways/src/domain/models/message/model.py` & `rome_ways-0.1.2/romeways/src/domain/models/message/model.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/romeways/src/infrastructure/spawner/infrastructure.py` & `rome_ways-0.1.2/romeways/src/infrastructure/spawner/infrastructure.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/romeways/src/romeways.py` & `rome_ways-0.1.2/romeways/src/romeways.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/romeways/src/service/chauffeur/service.py` & `rome_ways-0.1.2/romeways/src/service/chauffeur/service.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/romeways/src/service/guide/service.py` & `rome_ways-0.1.2/romeways/src/service/guide/service.py`

 * *Files identical despite different names*

### Comparing `rome_ways-0.1.1/setup.py` & `rome_ways-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['meeseeks-singleton>=0.4.2,<0.5.0']
 
 extras_require = \
-{'memory': ['romeways_memory_queue>=0.1.0,<0.2.0']}
+{'memory': ['romeways_memory_queue>=0.2.0,<0.3.0']}
 
 setup_kwargs = {
     'name': 'rome-ways',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A queue framework',
-    'long_description': '# Romeways\n\n<img src="./docs/images/banner.png" width="200"/>\nby: CenturyBoys\n\nThis project has as goal help developers to not reimplemented default queue consumer behaviour.\n\n# Basics\n\nRomeways works with two basic concepts queue handler and queue connector. The queue connector is a queue consumer and can be spawned in a separate process or in async worker. The queue handler is the callback function that will be called for each retrieved message.\n\nHere you can see all implemented consumer:\n\n| Queue Type            | Install using extra | description                                    |\n|-----------------------|---------------------|------------------------------------------------|\n| multiprocessing.Queue | memory              | [here](romeways_extras/memory_queue/README.md) |\n\nHow to install extra packages?\n\n```shell\npoetry add romeways -E memory\nOR\npip install \'romeways[memory]\'\n```\n\n# Configuration\n\n## Queue connector config\n\nThe queue connector config is all configurations that you need to be able to retrieve messages from the queue.\n\nBellow are the `romeways.GenericConnectorConfig` implementation. This class can be inheritance to allow extra configurations.\n\n#### Params:\n\n- `connector_name: str` For what connector this queue must be delivered\n\n```python\nfrom dataclasses import dataclass\n\n\n@dataclass(slots=True, frozen=True)\nclass GenericConnectorConfig:\n    """\n    connector_name: str Connector name\n    """\n    connector_name: str\n\n```\n\n## Queue handler config\n\nWhen you register a queue consumer you are setting configs and a callback handler for each message that this queue receives.\n\nBellow are the `romeways.GenericQueueConfig` implementation. This class can be inheritance to allow extra configurations.\n\n#### Params:\n\n- `connector_name: str` For what connector this queue must be delivered\n- `frequency: float` Time in seconds for retrieve messages from queue\n- `max_chunk_size: int` Max quantity for messages that one retrieve will get\n- `sequential: bool` If the handler call must be sequential or in asyncio.gather\n\n```python\nfrom dataclasses import dataclass\n\n\n@dataclass(slots=True, frozen=True)\nclass GenericQueueConfig:\n    """\n    connector_name: str For what connector this queue must be delivered\n    frequency: float Time in seconds for retrieve messages from queue\n    max_chunk_size: int Max quantity for messages that one retrieve will get\n    sequential: bool If the handler call must be sequential or in asyncio.gather\n    """\n    connector_name: str\n    frequency: float\n    max_chunk_size: int\n    sequential: bool\n\n```\n\n## Resend on error\n\nRomeways allow you to resend the message to the queue if something in your handler do not perform correctly. For that your code need tho raise the `romeways.ResendException` exception, the message will be resent to the same queue and the `romeways.Message.rw_resend_times` parameter will be raized\n\n\n## Spawn a process\n\nRomeways can run each connector in a separate process or in async workers for that use the parameter `spawn_process` to configure that.\n\n# Example\n\nFor this example we are using the extra memory\n\n```python\nfrom multiprocessing import Queue\n\nimport romeways\n\n# Create a queue config\nconfig_q = romeways.MemoryQueueConfig(\n    connector_name="memory-dev1"\n)\n\n# Register a controller/consumer for the queue name\n@romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)\nasync def controller(message: romeways.Message):\n    print(message)\n\n# Config the connector\nqueue = Queue()\n\nconfig_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1", queue=queue)\n\n# Register a connector\nromeways.connector_register(\n    connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True\n)\n\n```',
+    'long_description': '# Romeways\n\n<img src="./docs/images/banner.png" width="200"/>\nby: CenturyBoys\n\nThis project has as goal help developers to not reimplemented default queue consumer behaviour.\n\n# Basics\n\nRomeways works with two basic concepts queue handler and queue connector. The queue connector is a queue consumer and can be spawned in a separate process or in async worker. The queue handler is the callback function that will be called for each retrieved message.\n\nHere you can see all implemented consumer:\n\n| Queue Type            | Install using extra | description                                    |\n|-----------------------|---------------------|------------------------------------------------|\n| multiprocessing.Queue | memory              | [here](romeways_extras/memory_queue/README.md) |\n\nHow to install extra packages?\n\n```shell\npoetry add romeways -E memory\nOR\npip install \'romeways[memory]\'\n```\n\n# Configuration\n\n## Queue connector config\n\nThe queue connector config is all configurations that you need to be able to retrieve messages from the queue.\n\nBellow are the `romeways.GenericConnectorConfig` implementation. This class can be inheritance to allow extra configurations.\n\n#### Params:\n\n- `connector_name: str` For what connector this queue must be delivered\n\n```python\nfrom dataclasses import dataclass\n\n\n@dataclass(slots=True, frozen=True)\nclass GenericConnectorConfig:\n    """\n    connector_name: str Connector name\n    """\n    connector_name: str\n\n```\n\n## Queue handler config\n\nWhen you register a queue consumer you are setting configs and a callback handler for each message that this queue receives.\n\nBellow are the `romeways.GenericQueueConfig` implementation. This class can be inheritance to allow extra configurations.\n\n#### Params:\n\n- `connector_name: str` For what connector this queue must be delivered\n- `frequency: float` Time in seconds for retrieve messages from queue\n- `max_chunk_size: int` Max quantity for messages that one retrieve will get\n- `sequential: bool` If the handler call must be sequential or in asyncio.gather\n\n```python\nfrom dataclasses import dataclass\n\n\n@dataclass(slots=True, frozen=True)\nclass GenericQueueConfig:\n    """\n    connector_name: str For what connector this queue must be delivered\n    frequency: float Time in seconds for retrieve messages from queue\n    max_chunk_size: int Max quantity for messages that one retrieve will get\n    sequential: bool If the handler call must be sequential or in asyncio.gather\n    """\n    connector_name: str\n    frequency: float\n    max_chunk_size: int\n    sequential: bool\n\n```\n\n## Resend on error\n\nRomeways allow you to resend the message to the queue if something in your handler do not perform correctly. For that your code need tho raise the `romeways.ResendException` exception, the message will be resent to the same queue and the `romeways.Message.rw_resend_times` parameter will be raized\n\n\n## Spawn a process\n\nRomeways can run each connector in a separate process or in async workers for that use the parameter `spawn_process` to configure that.\n\n# Example\n\nFor this example we are using the extra package `memory`\n\n```python\nfrom multiprocessing import Queue\n\nimport romeways\n\n# Config the connector\nqueue = Queue()\n\n# Create a queue config\nconfig_q = romeways.MemoryQueueConfig(\n    connector_name="memory-dev1", \n    queue=queue\n)\n\n# Register a controller/consumer for the queue name\n@romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)\nasync def controller(message: romeways.Message):\n    print(message)\n\nconfig_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1")\n\n# Register a connector\nromeways.connector_register(\n    connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True\n)\n\n```',
     'author': 'Marco Sievers de Almeida Ximit Gaia',
     'author_email': 'im.ximit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rome_ways-0.1.1/PKG-INFO` & `rome_ways-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rome-ways
-Version: 0.1.1
+Version: 0.1.2
 Summary: A queue framework
 License: Apache-2.0
 Author: Marco Sievers de Almeida Ximit Gaia
 Author-email: im.ximit@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: memory
 Requires-Dist: meeseeks-singleton (>=0.4.2,<0.5.0)
-Requires-Dist: romeways_memory_queue (>=0.1.0,<0.2.0) ; extra == "memory"
+Requires-Dist: romeways_memory_queue (>=0.2.0,<0.3.0) ; extra == "memory"
 Project-URL: documentation, https://github.com/CenturyBoys/romeways
 Project-URL: homepage, https://github.com/CenturyBoys/romeways
 Project-URL: repository, https://github.com/CenturyBoys/romeways
 Description-Content-Type: text/markdown
 
 # Romeways
 
@@ -106,35 +106,36 @@
 
 ## Spawn a process
 
 Romeways can run each connector in a separate process or in async workers for that use the parameter `spawn_process` to configure that.
 
 # Example
 
-For this example we are using the extra memory
+For this example we are using the extra package `memory`
 
 ```python
 from multiprocessing import Queue
 
 import romeways
 
+# Config the connector
+queue = Queue()
+
 # Create a queue config
 config_q = romeways.MemoryQueueConfig(
-    connector_name="memory-dev1"
+    connector_name="memory-dev1", 
+    queue=queue
 )
 
 # Register a controller/consumer for the queue name
 @romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)
 async def controller(message: romeways.Message):
     print(message)
 
-# Config the connector
-queue = Queue()
-
-config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1", queue=queue)
+config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1")
 
 # Register a connector
 romeways.connector_register(
     connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True
 )
 
 ```
```

