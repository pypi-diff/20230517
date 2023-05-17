# Comparing `tmp/osnap_client-0.1.1a1.tar.gz` & `tmp/osnap_client-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osnap_client-0.1.1a1.tar", max compression
+gzip compressed data, was "osnap_client-0.1.1a2.tar", max compression
```

## Comparing `osnap_client-0.1.1a1.tar` & `osnap_client-0.1.1a2.tar`

### file list

```diff
@@ -1,31 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-05-12 13:26:06.322716 osnap_client-0.1.1a1/LICENSE
--rw-r--r--   0        0        0     2100 2023-05-12 13:26:06.322997 osnap_client-0.1.1a1/README.md
--rw-r--r--   0        0        0      104 2023-05-15 15:30:42.332818 osnap_client-0.1.1a1/osnap_client/README.md
--rw-r--r--   0        0        0      214 2023-05-16 10:31:58.826057 osnap_client-0.1.1a1/osnap_client/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-16 10:31:58.826379 osnap_client-0.1.1a1/osnap_client/adapters/AdapterBase.py
--rw-r--r--   0        0        0     4521 2023-05-16 10:31:58.826577 osnap_client-0.1.1a1/osnap_client/adapters/DiscordAdapter.py
--rw-r--r--   0        0        0      190 2023-05-16 10:31:58.826785 osnap_client-0.1.1a1/osnap_client/adapters/QueueTaskStruct.py
--rw-r--r--   0        0        0        0 2023-05-16 10:31:58.826811 osnap_client-0.1.1a1/osnap_client/adapters/__init__.py
--rw-r--r--   0        0        0       53 2023-05-16 10:31:58.827074 osnap_client-0.1.1a1/osnap_client/agents/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 10:31:58.827101 osnap_client-0.1.1a1/osnap_client/agents/base.py
--rw-r--r--   0        0        0     3744 2023-05-16 10:31:58.827745 osnap_client-0.1.1a1/osnap_client/agents/swarm_agents/swarm_agent.py
--rw-r--r--   0        0        0      199 2023-05-16 10:31:58.828093 osnap_client-0.1.1a1/osnap_client/core/__init__.py
--rw-r--r--   0        0        0     5934 2023-05-16 10:31:58.828320 osnap_client-0.1.1a1/osnap_client/core/agent.py
--rw-r--r--   0        0        0     1419 2023-05-15 15:30:42.335469 osnap_client-0.1.1a1/osnap_client/core/api.py
--rw-r--r--   0        0        0     1314 2023-05-15 15:30:42.335759 osnap_client-0.1.1a1/osnap_client/core/crypt.py
--rw-r--r--   0        0        0     6296 2023-05-16 10:31:58.828625 osnap_client-0.1.1a1/osnap_client/core/osnap.py
--rw-r--r--   0        0        0     5177 2023-05-15 15:30:42.336130 osnap_client-0.1.1a1/osnap_client/main.py
--rw-r--r--   0        0        0       46 2023-05-15 15:30:42.336488 osnap_client-0.1.1a1/osnap_client/pubsub/__init__.py
--rw-r--r--   0        0        0     2666 2023-05-15 15:30:42.336780 osnap_client-0.1.1a1/osnap_client/pubsub/pubsub.py
--rw-r--r--   0        0        0       98 2023-05-15 15:30:42.337005 osnap_client-0.1.1a1/osnap_client/registry/__init__.py
--rw-r--r--   0        0        0     3149 2023-05-15 15:30:42.337231 osnap_client-0.1.1a1/osnap_client/registry/agent_registry.py
--rw-r--r--   0        0        0        0 2023-05-15 15:30:42.337257 osnap_client-0.1.1a1/osnap_client/registry/registry.py
--rw-r--r--   0        0        0     1813 2023-05-15 15:30:42.337386 osnap_client-0.1.1a1/osnap_client/registry/tool_registry.py
--rw-r--r--   0        0        0        0 2023-05-15 15:30:42.337442 osnap_client-0.1.1a1/osnap_client/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:30:42.337481 osnap_client-0.1.1a1/osnap_client/tools/main.py
--rw-r--r--   0        0        0     2449 2023-05-15 15:30:42.337767 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/EngineBase.py
--rw-r--r--   0        0        0     2846 2023-05-15 15:30:42.337959 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/GPTConversEngine.py
--rw-r--r--   0        0        0     2972 2023-05-15 15:30:42.338318 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
--rw-r--r--   0        0        0      136 2023-05-15 15:30:42.338425 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/__init__.py
--rw-r--r--   0        0        0     1181 2023-05-16 10:36:06.881324 osnap_client-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     3193 1970-01-01 00:00:00.000000 osnap_client-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 08:21:07.375494 osnap_client-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0     2487 2023-05-17 08:21:07.375494 osnap_client-0.1.1a2/README.md
+-rw-r--r--   0        0        0      214 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/__init__.py
+-rw-r--r--   0        0        0     1759 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/AdapterBase.py
+-rw-r--r--   0        0        0     4525 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/DiscordAdapter.py
+-rw-r--r--   0        0        0      190 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/QueueTaskStruct.py
+-rw-r--r--   0        0        0       79 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/__init__.py
+-rw-r--r--   0        0        0     3681 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/agents/SwarmAgentBase.py
+-rw-r--r--   0        0        0       42 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/agents/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/__init__.py
+-rw-r--r--   0        0        0     5934 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/agent.py
+-rw-r--r--   0        0        0     1419 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/api.py
+-rw-r--r--   0        0        0     1314 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/crypt.py
+-rw-r--r--   0        0        0     6296 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/osnap.py
+-rw-r--r--   0        0        0       46 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/pubsub/__init__.py
+-rw-r--r--   0        0        0     2666 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/pubsub/pubsub.py
+-rw-r--r--   0        0        0       98 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/__init__.py
+-rw-r--r--   0        0        0     3149 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/agent_registry.py
+-rw-r--r--   0        0        0        0 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/registry.py
+-rw-r--r--   0        0        0     1813 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/tool_registry.py
+-rw-r--r--   0        0        0        0 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/tools/main.py
+-rw-r--r--   0        0        0     2449 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/EngineBase.py
+-rw-r--r--   0        0        0     2846 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/GPTConversEngine.py
+-rw-r--r--   0        0        0     2972 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
+-rw-r--r--   0        0        0      136 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 osnap_client-0.1.1a2/PKG-INFO
```

### Comparing `osnap_client-0.1.1a1/LICENSE` & `osnap_client-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/README.md` & `osnap_client-0.1.1a2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 # OSNAP
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/seKVhCtcAJ?style=flat)](https://discord.gg/seKVhCtcAJ)
 
-The Open Swarm Network Agent Protocol (OSNAP) is a standardized protocol for building autonomous AI agents and swarms or organizations of agents. The primary goal of OSNAP is to facilitate interoperability, collaboration, and ease of development across various autonomous AI systems, similar to how HTTP serves as a standard protocol for the World Wide Web.
+The Open Swarm Network Agent Protocol (OSNAP) is a standardized toolkit for building AI agents that interact with each other. Currently, the development and implementation of interacting autonomous AI agents and swarms are highly fragmented, with different projects utilizing various custom-built protocols and communication methods. This lack of standardization can lead to difficulties. OSNAP aims to address these issues by providing a well-defined, standardized toolkit for building and interacting with autonomous AI agents and swarms.
+
 <p align="center">
   <img src="content/logo_midjourney.png" alt="Project logo" width="1080">
 </p>
 
 ## Table of Contents
-- [Why](#why)
 - [How to use in your project](#how-to-use-in-your-project)
 - [Examples](#examples)
 - [Architecture Overview](#architecture-overview)
 - [Next-Ups](#next-ups)
 - [How to Contribute](#how-to-contribute)
 
-# Why
-Currently, the development and implementation of autonomous AI agents and swarms are highly fragmented, with different projects utilizing various custom-built protocols and communication methods. This lack of standardization can lead to difficulties in:
-
-Interoperability between different AI systems and swarm implementations.
-Reusability of code, components, and algorithms.
-Collaboration between researchers and practitioners in the field of autonomous AI and swarm intelligence.
-OSNAP aims to address these issues by providing a well-defined, standardized protocol for building and interacting with autonomous AI agents and swarms.
-
-
 # How to use in your project
-1. aaaa
+Coming soon...
 
 # Examples
 
+First, setup the environment:
+1. Installing dependencies:
+    - If you use poetry, use `pyproject.toml`
+    - Otherwise, create a new [venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/) and use `requirements.txt`. 
+2. Adding environment variables:
+    - use `.env.template` to create a `.env` file
+    - every example has a separate `.env` file
+
+## Discord Swarm
+[To Example](examples\discord_swarm\README.md)\
+Discord swarm allows you to deploy multiple independent agents (can be in different networks) and let them communicate with each other over a discord server. For example, agents can ask other bots for help and solve the task colaboratively.
+
+The communication is handleded via the DiscordAdapter and the only think you need to do is to implement the logic of the `SwarmAgentBase`.
 
 # Architecture overview
 <p align="center">
-  <img src="content/diagram.png" alt="Project diagram" width="720">
+  <img src="content/architecture_diagram.png" alt="Project diagram" width="720">
 </p>
 
 
 # Next-ups
 - make adding new models as easy as possible, including custom deployed ones like llama
 - multi-key support for higher scalability
```

### Comparing `osnap_client-0.1.1a1/osnap_client/adapters/DiscordAdapter.py` & `osnap_client-0.1.1a2/osnap_client/adapters/DiscordAdapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # discord_adapter.py
 import discord
-from osnap.SwarmAdapters.AdapterBase import AdapterBase
-from osnap.SwarmAdapters.QueueTaskStruct import QueueTaskStruct
+from osnap_client.adapters.AdapterBase import AdapterBase
+from osnap_client.adapters.QueueTaskStruct import QueueTaskStruct
 import asyncio
 
 class DiscordAdapter(AdapterBase):
     """This is an adapter that allows the agent to communicate with Discord and receive/send messages.
 
     Args:
     - intents_list (list[str]): A list of intents that the bot will listen to.
```

### Comparing `osnap_client-0.1.1a1/osnap_client/agents/swarm_agents/swarm_agent.py` & `osnap_client-0.1.1a2/osnap_client/agents/SwarmAgentBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,89 @@
 from abc import ABC, abstractmethod
 import asyncio
 import time
 import threading
 
-from osnap_client.adapters.DiscordAdapter import DiscordAdapter
-from osnap_client.agents import SwarmAgentBase
-
+from osnap_client.adapters.AdapterBase import AdapterBase
+from osnap_client.adapters.QueueTaskStruct import QueueTaskStruct
 
 class SwarmAgentBase(ABC):
     """
     This is a base class that the user needs to implement to define the logic of the bot
     for request handling and sending.
     """
-
     def __init__(self, name: str, description: str, swarm_adapter: AdapterBase) -> None:
         super().__init__()
         self.name = name
         self.description = description
         self.swarm_adapter = swarm_adapter
         self.event_queue = swarm_adapter.event_queue
         self.command_map = {}
 
         # Register "ready" command
         self.command_map["on_ready"] = self.on_ready
-
+    
     def command(self, name: str):
         def decorator(func):
             self.command_map[name] = func
             return func
-
         return decorator
-
+    
     async def on_callback_event_listener(self):
         while True:
             task = None
             try:
                 task = self.event_queue.get_nowait()
             except asyncio.QueueEmpty:
                 time.sleep(0.5)
                 continue
             if not isinstance(task, QueueTaskStruct):
                 raise TypeError(f"Expected a QueueTaskStruct, got {type(task)}")
-
+            
             command = task.command_type
             data = task.data
 
             if command in self.command_map:
                 # check if the adapter loop is running
                 if not self.swarm_adapter.adapter_loop.is_running():
                     print("Adapter loop is not running, starting it now")
                     try:
                         self.start_adapter()
                     except Exception as e:
                         print(f"Error starting adapter: {e}")
                     if not self.swarm_adapter.adapter_loop.is_running():
-                        raise Exception(
-                            "Adapter loop is still not running after starting it"
-                        )
-
+                        raise Exception("Adapter loop is still not running after starting it")
+                
                 try:
-                    asyncio.run_coroutine_threadsafe(
-                        self.command_map[command](data), self.swarm_adapter.adapter_loop
-                    )
+                    asyncio.run_coroutine_threadsafe(self.command_map[command](data), self.swarm_adapter.adapter_loop)
                 except Exception as e:
                     print(f"Error in {command} command: {e}")
             else:
                 print(f"Unknown command: {command}")
 
     def start_adapter(self):
         adapter_thread = threading.Thread(target=self.swarm_adapter.start)
         adapter_thread.start()
 
     async def on_ready(self, data: str):
         """This method is called when the apter is loaded."""
-        self_description = (
-            f"Hi everyone!\nName: {self.name}\nDescription: {self.description}"
-        )
+        self_description = f"Hi everyone!\nName: {self.name}\nDescription: {self.description}"
         await self.swarm_adapter.send_message(self_description, "intros")
 
     def run(self):
         """This method is called to start the bot
-
+        
         Clarification on the event loops. Bear with me here =)
         Ideally we'd like the adapter and the agent to run in the same event loop,
         but both the discord process and the adent process are blocking the event loop.
 
         So we need to split the process into two event loops, one for the agent and one for the adapter.
 
         However, now we cannot await the adapter methods from the agent, because they are running in different event loops.
         Therefore in the agent we need to use the run_coroutine_threadsafe method to run the adapter methods in the adapter event loop.
-        """
+        """       
         # run the adapter in a separate thread
         self.start_adapter()
 
         # run the event listener in the main thread
         agent_loop = asyncio.get_event_loop()
         agent_loop.run_until_complete(self.on_callback_event_listener())
```

### Comparing `osnap_client-0.1.1a1/osnap_client/core/agent.py` & `osnap_client-0.1.1a2/osnap_client/core/agent.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/core/api.py` & `osnap_client-0.1.1a2/osnap_client/core/api.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/core/crypt.py` & `osnap_client-0.1.1a2/osnap_client/core/crypt.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/core/osnap.py` & `osnap_client-0.1.1a2/osnap_client/core/osnap.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/pubsub/pubsub.py` & `osnap_client-0.1.1a2/osnap_client/pubsub/pubsub.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/registry/agent_registry.py` & `osnap_client-0.1.1a2/osnap_client/registry/agent_registry.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/registry/tool_registry.py` & `osnap_client-0.1.1a2/osnap_client/registry/tool_registry.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/utils/ai_engines/EngineBase.py` & `osnap_client-0.1.1a2/osnap_client/utils/ai_engines/EngineBase.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/utils/ai_engines/GPTConversEngine.py` & `osnap_client-0.1.1a2/osnap_client/utils/ai_engines/GPTConversEngine.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/osnap_client/utils/ai_engines/LanchainGoogleEngine.py` & `osnap_client-0.1.1a2/osnap_client/utils/ai_engines/LanchainGoogleEngine.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a1/pyproject.toml` & `osnap_client-0.1.1a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "osnap-client"
-version = "0.1.1a1"
+version = "0.1.1a2"
 description = ""
-authors = ["Forrest Murray <FMurray@gmail.com>"]
+authors = ["Forrest Murray <FMurray@gmail.com>", "Vlad Samoilov <nicelir1996@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 langchain = ">=0.0.153,<0.1.0"
 fastapi = ">=0.95.1,<0.96.0"
 uvicorn = ">=0.22.0,<0.23.0"
@@ -22,16 +22,14 @@
 python-dotenv = "^1.0.0"
 discord = "^2.2.3"
 jsonschema = "^4.17.3"
 pytest = "^7.3.1"
 ipykernel = "^6.23.0"
 tiktoken = "^0.4.0"
 
-
-
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
```

