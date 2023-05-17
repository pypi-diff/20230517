# Comparing `tmp/romeways_memory_queue-0.1.0.tar.gz` & `tmp/romeways_memory_queue-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romeways_memory_queue-0.1.0.tar", max compression
+gzip compressed data, was "romeways_memory_queue-0.2.0.tar", max compression
```

## Comparing `romeways_memory_queue-0.1.0.tar` & `romeways_memory_queue-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-11 12:11:01.507301 romeways_memory_queue-0.1.0/LICENSE
--rw-r--r--   0        0        0     1666 2023-05-16 17:17:52.586089 romeways_memory_queue-0.1.0/README.md
--rw-r--r--   0        0        0      358 2023-05-14 11:37:09.927001 romeways_memory_queue-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      110 2023-05-13 19:25:10.042766 romeways_memory_queue-0.1.0/romeways_memory_queue/__init__.py
--rw-r--r--   0        0        0       82 2023-05-13 17:16:04.059979 romeways_memory_queue-0.1.0/romeways_memory_queue/config/__init__.py
--rw-r--r--   0        0        0       41 2023-05-13 17:03:10.532049 romeways_memory_queue-0.1.0/romeways_memory_queue/config/connector/__init__.py
--rw-r--r--   0        0        0      221 2023-05-14 12:10:14.378153 romeways_memory_queue-0.1.0/romeways_memory_queue/config/connector/model.py
--rw-r--r--   0        0        0       37 2023-05-13 17:03:10.516053 romeways_memory_queue-0.1.0/romeways_memory_queue/config/queue/__init__.py
--rw-r--r--   0        0        0      320 2023-05-16 15:16:04.771831 romeways_memory_queue-0.1.0/romeways_memory_queue/config/queue/model.py
--rw-r--r--   0        0        0       44 2023-05-13 17:16:04.059979 romeways_memory_queue-0.1.0/romeways_memory_queue/infrastructure/__init__.py
--rw-r--r--   0        0        0       49 2023-05-13 17:16:04.063978 romeways_memory_queue-0.1.0/romeways_memory_queue/infrastructure/connector/__init__.py
--rw-r--r--   0        0        0      661 2023-05-16 14:41:09.897030 romeways_memory_queue-0.1.0/romeways_memory_queue/infrastructure/connector/infrastructure.py
--rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 romeways_memory_queue-0.1.0/setup.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 romeways_memory_queue-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 12:11:01.507301 romeways_memory_queue-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-17 12:48:44.434467 romeways_memory_queue-0.2.0/README.md
+-rw-r--r--   0        0        0      358 2023-05-17 12:23:33.601970 romeways_memory_queue-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-05-13 19:25:10.042766 romeways_memory_queue-0.2.0/romeways_memory_queue/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-13 17:16:04.059979 romeways_memory_queue-0.2.0/romeways_memory_queue/config/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-13 17:03:10.532049 romeways_memory_queue-0.2.0/romeways_memory_queue/config/connector/__init__.py
+-rw-r--r--   0        0        0      212 2023-05-17 12:19:45.159259 romeways_memory_queue-0.2.0/romeways_memory_queue/config/connector/model.py
+-rw-r--r--   0        0        0       37 2023-05-13 17:03:10.516053 romeways_memory_queue-0.2.0/romeways_memory_queue/config/queue/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-17 12:41:59.532382 romeways_memory_queue-0.2.0/romeways_memory_queue/config/queue/model.py
+-rw-r--r--   0        0        0       44 2023-05-13 17:16:04.059979 romeways_memory_queue-0.2.0/romeways_memory_queue/infrastructure/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-13 17:16:04.063978 romeways_memory_queue-0.2.0/romeways_memory_queue/infrastructure/connector/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-17 12:38:42.815665 romeways_memory_queue-0.2.0/romeways_memory_queue/infrastructure/connector/infrastructure.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 romeways_memory_queue-0.2.0/setup.py
+-rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 romeways_memory_queue-0.2.0/PKG-INFO
```

### Comparing `romeways_memory_queue-0.1.0/LICENSE` & `romeways_memory_queue-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `romeways_memory_queue-0.1.0/README.md` & `romeways_memory_queue-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,66 +2,74 @@
 
 This is an extra package for romeways for more details access the [romeways](https://github.com/CenturyBoys/romeways) Github page.
 
 ## Configs
 
 ### Queue
 
-The only difference between the `romeways.GenericQueueConfig` and `romeways_memory_queue.MemoryQueueConfig` are some default parameters.
+The only difference between the `romeways.GenericQueueConfig` and `romeways_memory_queue.MemoryQueueConfig` is the `multiprocessing.Queue` instance.
 
 ```python
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from multiprocessing import Queue
 
 from romeways import GenericQueueConfig
 
 
 @dataclass(slots=True, frozen=True)
 class MemoryQueueConfig(GenericQueueConfig):
     connector_name: str
-    frequency: float = field(default=0.25)
-    max_chunk_size: int = field(default=10)
-    sequential: bool = field(default=False)
+    frequency: float
+    max_chunk_size: int
+    sequential: bool
+    queue: Queue
 ```
 ### Connector
 
-Obs: Because the package use the multiprocessing.Queue is allowed to register only one queue consumer.
 
 ```python
 from dataclasses import dataclass
-from multiprocessing import Queue
 
 from romeways import GenericConnectorConfig
 
 @dataclass(slots=True, frozen=True)
 class MemoryConnectorConfig(GenericConnectorConfig):
     connector_name: str
-    queue: Queue
 ```
 
 ## Use case
 
 ```python
 from multiprocessing import Queue
+import asyncio
 
 import romeways
 
+# Config the connector
+queue = Queue()
+
 # Create a queue config
 config_q = romeways.MemoryQueueConfig(
-    connector_name="memory-dev1"
+    connector_name="memory-dev1",
+    frequency=1,
+    max_chunk_size=10,
+    sequential=False,
+    queue=queue
 )
 
 # Register a controller/consumer for the queue name
 @romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)
 async def controller(message: romeways.Message):
     print(message)
 
-# Config the connector
-queue = Queue()
 
-config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1", queue=queue)
+
+config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1")
 
 # Register a connector
 romeways.connector_register(
     connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True
 )
 
+asyncio.run(romeways.start())
+
 ```
```

### Comparing `romeways_memory_queue-0.1.0/romeways_memory_queue/infrastructure/connector/infrastructure.py` & `romeways_memory_queue-0.2.0/romeways_memory_queue/infrastructure/connector/infrastructure.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from multiprocessing import Queue
 from typing import List
 
 from romeways import AQueueConnector
 
 
 class MemoryQueueConnector(AQueueConnector):
+
     async def on_start(self):
         pass
 
     async def get_messages(self, max_chunk_size: int) -> List[bytes]:
-        queue: Queue = self._connector_config.queue
+        queue: Queue = self._config.queue
         buffer = []
         for _ in range(abs(max_chunk_size)):
             if not queue.empty():
                 buffer.append(queue.get_nowait())
                 continue
             break
         return buffer
 
     async def send_messages(self, message: bytes):
-        queue: Queue = self._connector_config.queue
+        queue: Queue = self._config.queue
         queue.put_nowait(message)
```

### Comparing `romeways_memory_queue-0.1.0/setup.py` & `romeways_memory_queue-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,17 @@
  'romeways_memory_queue.infrastructure.connector']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'romeways-memory-queue',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
-    'long_description': '# Romeways memory queue\n\nThis is an extra package for romeways for more details access the [romeways](https://github.com/CenturyBoys/romeways) Github page.\n\n## Configs\n\n### Queue\n\nThe only difference between the `romeways.GenericQueueConfig` and `romeways_memory_queue.MemoryQueueConfig` are some default parameters.\n\n```python\nfrom dataclasses import dataclass, field\n\nfrom romeways import GenericQueueConfig\n\n\n@dataclass(slots=True, frozen=True)\nclass MemoryQueueConfig(GenericQueueConfig):\n    connector_name: str\n    frequency: float = field(default=0.25)\n    max_chunk_size: int = field(default=10)\n    sequential: bool = field(default=False)\n```\n### Connector\n\nObs: Because the package use the multiprocessing.Queue is allowed to register only one queue consumer.\n\n```python\nfrom dataclasses import dataclass\nfrom multiprocessing import Queue\n\nfrom romeways import GenericConnectorConfig\n\n@dataclass(slots=True, frozen=True)\nclass MemoryConnectorConfig(GenericConnectorConfig):\n    connector_name: str\n    queue: Queue\n```\n\n## Use case\n\n```python\nfrom multiprocessing import Queue\n\nimport romeways\n\n# Create a queue config\nconfig_q = romeways.MemoryQueueConfig(\n    connector_name="memory-dev1"\n)\n\n# Register a controller/consumer for the queue name\n@romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)\nasync def controller(message: romeways.Message):\n    print(message)\n\n# Config the connector\nqueue = Queue()\n\nconfig_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1", queue=queue)\n\n# Register a connector\nromeways.connector_register(\n    connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True\n)\n\n```\n',
+    'long_description': '# Romeways memory queue\n\nThis is an extra package for romeways for more details access the [romeways](https://github.com/CenturyBoys/romeways) Github page.\n\n## Configs\n\n### Queue\n\nThe only difference between the `romeways.GenericQueueConfig` and `romeways_memory_queue.MemoryQueueConfig` is the `multiprocessing.Queue` instance.\n\n```python\nfrom dataclasses import dataclass\nfrom multiprocessing import Queue\n\nfrom romeways import GenericQueueConfig\n\n\n@dataclass(slots=True, frozen=True)\nclass MemoryQueueConfig(GenericQueueConfig):\n    connector_name: str\n    frequency: float\n    max_chunk_size: int\n    sequential: bool\n    queue: Queue\n```\n### Connector\n\n\n```python\nfrom dataclasses import dataclass\n\nfrom romeways import GenericConnectorConfig\n\n@dataclass(slots=True, frozen=True)\nclass MemoryConnectorConfig(GenericConnectorConfig):\n    connector_name: str\n```\n\n## Use case\n\n```python\nfrom multiprocessing import Queue\nimport asyncio\n\nimport romeways\n\n# Config the connector\nqueue = Queue()\n\n# Create a queue config\nconfig_q = romeways.MemoryQueueConfig(\n    connector_name="memory-dev1",\n    frequency=1,\n    max_chunk_size=10,\n    sequential=False,\n    queue=queue\n)\n\n# Register a controller/consumer for the queue name\n@romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)\nasync def controller(message: romeways.Message):\n    print(message)\n\n\n\nconfig_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1")\n\n# Register a connector\nromeways.connector_register(\n    connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True\n)\n\nasyncio.run(romeways.start())\n\n```\n',
     'author': 'Marco Sievers de Almeida Ximit Gaia',
     'author_email': 'im.ximit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `romeways_memory_queue-0.1.0/PKG-INFO` & `romeways_memory_queue-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romeways-memory-queue
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Marco Sievers de Almeida Ximit Gaia
 Author-email: im.ximit@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -13,67 +13,75 @@
 
 This is an extra package for romeways for more details access the [romeways](https://github.com/CenturyBoys/romeways) Github page.
 
 ## Configs
 
 ### Queue
 
-The only difference between the `romeways.GenericQueueConfig` and `romeways_memory_queue.MemoryQueueConfig` are some default parameters.
+The only difference between the `romeways.GenericQueueConfig` and `romeways_memory_queue.MemoryQueueConfig` is the `multiprocessing.Queue` instance.
 
 ```python
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from multiprocessing import Queue
 
 from romeways import GenericQueueConfig
 
 
 @dataclass(slots=True, frozen=True)
 class MemoryQueueConfig(GenericQueueConfig):
     connector_name: str
-    frequency: float = field(default=0.25)
-    max_chunk_size: int = field(default=10)
-    sequential: bool = field(default=False)
+    frequency: float
+    max_chunk_size: int
+    sequential: bool
+    queue: Queue
 ```
 ### Connector
 
-Obs: Because the package use the multiprocessing.Queue is allowed to register only one queue consumer.
 
 ```python
 from dataclasses import dataclass
-from multiprocessing import Queue
 
 from romeways import GenericConnectorConfig
 
 @dataclass(slots=True, frozen=True)
 class MemoryConnectorConfig(GenericConnectorConfig):
     connector_name: str
-    queue: Queue
 ```
 
 ## Use case
 
 ```python
 from multiprocessing import Queue
+import asyncio
 
 import romeways
 
+# Config the connector
+queue = Queue()
+
 # Create a queue config
 config_q = romeways.MemoryQueueConfig(
-    connector_name="memory-dev1"
+    connector_name="memory-dev1",
+    frequency=1,
+    max_chunk_size=10,
+    sequential=False,
+    queue=queue
 )
 
 # Register a controller/consumer for the queue name
 @romeways.queue_consumer(queue_name="queue.payment.done", config=config_q)
 async def controller(message: romeways.Message):
     print(message)
 
-# Config the connector
-queue = Queue()
 
-config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1", queue=queue)
+
+config_p = romeways.MemoryConnectorConfig(connector_name="memory-dev1")
 
 # Register a connector
 romeways.connector_register(
     connector=romeways.MemoryQueueConnector, config=config_p, spawn_process=True
 )
 
+asyncio.run(romeways.start())
+
 ```
```

