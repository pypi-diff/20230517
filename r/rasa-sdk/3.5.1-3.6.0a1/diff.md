# Comparing `tmp/rasa_sdk-3.5.1.tar.gz` & `tmp/rasa_sdk-3.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa_sdk-3.5.1.tar", max compression
+gzip compressed data, was "rasa_sdk-3.6.0a1.tar", max compression
```

## Comparing `rasa_sdk-3.5.1.tar` & `rasa_sdk-3.6.0a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11553 2023-04-12 09:49:45.759693 rasa_sdk-3.5.1/LICENSE.txt
--rw-r--r--   0        0        0     5236 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/README.md
--rw-r--r--   0        0        0     2701 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/pyproject.toml
--rw-r--r--   0        0        0      370 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/__init__.py
--rw-r--r--   0        0        0      947 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/__main__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/cli/__init__.py
--rw-r--r--   0        0        0     1528 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/cli/arguments.py
--rw-r--r--   0        0        0      399 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/constants.py
--rw-r--r--   0        0        0     5510 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/endpoint.py
--rw-r--r--   0        0        0     6427 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/events.py
--rw-r--r--   0        0        0     1905 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/exceptions.py
--rw-r--r--   0        0        0    15168 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/executor.py
--rw-r--r--   0        0        0    11265 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/forms.py
--rw-r--r--   0        0        0    12929 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/__init__.py
--rw-r--r--   0        0        0     8842 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/actions.py
--rw-r--r--   0        0        0     7698 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/storage.py
--rw-r--r--   0        0        0     6226 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/utils.py
--rw-r--r--   0        0        0     7066 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/slots.py
--rw-r--r--   0        0        0     1683 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/types.py
--rw-r--r--   0        0        0    11303 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/utils.py
--rw-r--r--   0        0        0      116 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/version.py
--rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 rasa_sdk-3.5.1/setup.py
--rw-r--r--   0        0        0     6759 1970-01-01 00:00:00.000000 rasa_sdk-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11553 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     5282 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/README.md
+-rw-r--r--   0        0        0     3114 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/__init__.py
+-rw-r--r--   0        0        0      947 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/cli/__init__.py
+-rw-r--r--   0        0        0     1528 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/cli/arguments.py
+-rw-r--r--   0        0        0      399 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/constants.py
+-rw-r--r--   0        0        0     5727 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/endpoint.py
+-rw-r--r--   0        0        0     6459 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/events.py
+-rw-r--r--   0        0        0     1905 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/exceptions.py
+-rw-r--r--   0        0        0    15183 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/executor.py
+-rw-r--r--   0        0        0    11265 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/forms.py
+-rw-r--r--   0        0        0    12929 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/interfaces.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     8970 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/actions.py
+-rw-r--r--   0        0        0     7766 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/storage.py
+-rw-r--r--   0        0        0     6287 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/utils.py
+-rw-r--r--   0        0        0     1039 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/plugin.py
+-rw-r--r--   0        0        0     7066 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/slots.py
+-rw-r--r--   0        0        0     1683 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/types.py
+-rw-r--r--   0        0        0    11308 2023-05-17 17:52:30.728710 rasa_sdk-3.6.0a1/rasa_sdk/utils.py
+-rw-r--r--   0        0        0      118 2023-05-17 17:52:30.728710 rasa_sdk-3.6.0a1/rasa_sdk/version.py
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rasa_sdk-3.6.0a1/PKG-INFO
```

### Comparing `rasa_sdk-3.5.1/LICENSE.txt` & `rasa_sdk-3.6.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/README.md` & `rasa_sdk-3.6.0a1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 # To install packages from PyPI
 RUN pip install --no-cache-dir <A_REQUIRED_PACKAGE_ON_PYPI>
 
 # Switch back to non-root to run code
 USER 1001
 ```
 
-
 ## Building from source
 
 Rasa SDK uses Poetry for packaging and dependency management. If you want to build it from source,
 you have to install Poetry first. This is how it can be done:
 
 ```
 curl -sSL https://install.python-poetry.org | python3 -
@@ -126,16 +125,16 @@
 
 *Release steps*:
 1. Switch to the branch you want to cut the release from (`main` in case of a
   major / minor, the current release branch for patch releases).
 2. If this is a minor / major release: Make sure all fixes from currently supported minor versions have been merged from their respective release branches (e.g. 3.3.x) back into main.
 3. Run `make release`
 4. Create a PR against main or the release branch (e.g. `1.2.x`)
-5. Once your PR is merged, tag a new release (this SHOULD always happen on
-  `main` or release branches), e.g. using
+5. Once your PR is merged, pull the release branch locally.
+6. Create a tag for a new release (this SHOULD always happen on `main` or release branches), e.g. using
     ```bash
     git tag 1.2.0 -m "next release"
     git push origin 1.2.0
     ```
     GitHub Actions will build this tag and push a package to
     [pypi](https://pypi.python.org/pypi/rasa-sdk).
 6. **If this is a minor release**, a new release branch should be created
```

### Comparing `rasa_sdk-3.5.1/pyproject.toml` & `rasa_sdk-3.6.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .mypy_cache | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa-sdk"
-version = "3.5.1"
+version = "3.6.0a1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa-sdk"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -58,31 +58,52 @@
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "misc"
 name = "Miscellaneous internal changes"
 showcontent = false
 
+[tool.mypy]
+ignore_missing_imports = true
+show_error_codes = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+
+[tool.ruff]
+ignore = [ "D100", "D104", "D105", "RUF005",]
+line-length = 88
+select = [ "D", "E", "F", "W", "RUF",]
+
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
+python = ">=3.8,<3.11"
 coloredlogs = ">=10,<16"
 sanic = "^21.12.0"
 typing-extensions = ">=4.1.1,<5.0.0"
 Sanic-Cors = "^2.0.0"
 prompt-toolkit = "^3.0,<3.0.29"
 "ruamel.yaml" = ">=0.16.5,<0.18.0"
 websockets = ">=10.0,<11.0"
+pluggy = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^4.0.0"
 coveralls = "^3.0.1"
 pytest = "^7.2.1"
 black = "22.12.0"
-flake8 = "^5.0.4"
-flake8-docstrings = "^1.5.0"
 questionary = ">=1.5.1,<1.11.0"
 towncrier = "^22.8.0"
 toml = "^0.10.0"
 pep440-version-utils = "^0.3.0"
 semantic_version = "^2.8.5"
-mypy = "^0.991"
+mypy = "^1.1"
 sanic-testing = "^22.3.0, <22.9.0"
+
+[tool.pytest.ini_options]
+python_functions = "test_"
+asyncio_mode = "auto"
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.256"
+pytest-asyncio = "^0.21.0"
```

### Comparing `rasa_sdk-3.5.1/rasa_sdk/__main__.py` & `rasa_sdk-3.6.0a1/rasa_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/rasa_sdk/cli/arguments.py` & `rasa_sdk-3.6.0a1/rasa_sdk/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/rasa_sdk/endpoint.py` & `rasa_sdk-3.6.0a1/rasa_sdk/endpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import argparse
 import logging
 import os
 import types
 import zlib
 import json
-from typing import List, Text, Union, Optional, Any
+from typing import List, Text, Union, Optional
 from ssl import SSLContext
 
 from sanic import Sanic, response
 from sanic.response import HTTPResponse
 from sanic.request import Request
 from sanic_cors import CORS
 
 from rasa_sdk import utils
 from rasa_sdk.cli.arguments import add_endpoint_arguments
 from rasa_sdk.constants import DEFAULT_SERVER_PORT
 from rasa_sdk.executor import ActionExecutor
 from rasa_sdk.interfaces import ActionExecutionRejection, ActionNotFoundException
+from rasa_sdk.plugin import plugin_manager
 
 logger = logging.getLogger(__name__)
 
 
 def configure_cors(
     app: Sanic, cors_origins: Union[Text, List[Text], None] = ""
 ) -> None:
@@ -152,14 +153,17 @@
     auto_reload: bool = False,
 ) -> None:
     """Starts the action endpoint server with given config values."""
     logger.info("Starting action endpoint server...")
     app = create_app(
         action_package_name, cors_origins=cors_origins, auto_reload=auto_reload
     )
+    ## Attach additional sanic extensions: listeners, middleware and routing
+    logger.info("Starting plugins...")
+    plugin_manager().hook.attach_sanic_app_extensions(app=app)
     ssl_context = create_ssl_context(ssl_certificate, ssl_keyfile, ssl_password)
     protocol = "https" if ssl_context else "http"
     host = os.environ.get("SANIC_HOST", "0.0.0.0")
 
     logger.info(f"Action endpoint is up and running on {protocol}://{host}:{port}")
     app.run(host, port, ssl=ssl_context, workers=utils.number_of_sanic_workers())
```

### Comparing `rasa_sdk-3.5.1/rasa_sdk/events.py` & `rasa_sdk-3.6.0a1/rasa_sdk/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     name: Optional[Text] = None,
     kill_on_user_message: bool = True,
     timestamp: Optional[float] = None,
 ) -> EventType:
     if _is_probably_action_name(intent_name):
         warnings.warn(
             f"ReminderScheduled intent starts with 'utter_' or 'action_'. "
-            f"If '{intent_name}' is indeed an intent, then you can ignore this warning.",
+            f"If '{intent_name}' is indeed an intent, "
+            f"then you can ignore this warning.",
             FutureWarning,
         )
     return {
         "event": "reminder",
         "timestamp": timestamp,
         "intent": intent_name,
         "entities": entities,
@@ -105,15 +106,16 @@
     intent_name: Optional[Text] = None,
     entities: Optional[Union[List[Dict[Text, Any]], Dict[Text, Text]]] = None,
     timestamp: Optional[float] = None,
 ) -> EventType:
     if _is_probably_action_name(intent_name):
         warnings.warn(
             f"ReminderCancelled intent starts with 'utter_' or 'action_'. "
-            f"If '{intent_name}' is indeed an intent, then you can ignore this warning.",
+            f"If '{intent_name}' is indeed an intent, "
+            f"then you can ignore this warning.",
             FutureWarning,
         )
     return {
         "event": "cancel_reminder",
         "timestamp": timestamp,
         "intent": intent_name,
         "entities": entities,
```

### Comparing `rasa_sdk-3.5.1/rasa_sdk/exceptions.py` & `rasa_sdk-3.6.0a1/rasa_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/rasa_sdk/executor.py` & `rasa_sdk-3.6.0a1/rasa_sdk/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,16 @@
         tracker: Tracker,
         silent_fail: bool = False,
         **kwargs: Any,
     ) -> None:
         """Sends a message template with buttons to the output channel."""
         warnings.warn(
             "Use of `utter_button_template` is deprecated. "
-            "Use `utter_message(template=<template name>, buttons=<list of buttons>)` instead.",
+            "Use `utter_message(template=<template name>, buttons=<list of buttons>)`"
+            " instead.",
             FutureWarning,
         )
 
         self.utter_message(template=template, buttons=buttons, **kwargs)
 
     # noinspection PyUnusedLocal
     def utter_template(
```

### Comparing `rasa_sdk-3.5.1/rasa_sdk/forms.py` & `rasa_sdk-3.6.0a1/rasa_sdk/forms.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/rasa_sdk/interfaces.py` & `rasa_sdk-3.6.0a1/rasa_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/rasa_sdk/knowledge_base/actions.py` & `rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,25 @@
             dispatcher: the dispatcher
             object_name: the name of the object
             attribute_name: the name of the attribute
             attribute_value: the value of the attribute
         """
         if attribute_value:
             dispatcher.utter_message(
-                text=f"'{object_name}' has the value '{attribute_value}' for attribute '{attribute_name}'."
+                text=(
+                    f"'{object_name}' has the value '{attribute_value}' "
+                    f"for attribute '{attribute_name}'."
+                )
             )
         else:
             dispatcher.utter_message(
-                text=f"Did not find a valid value for attribute '{attribute_name}' for object '{object_name}'."
+                text=(
+                    f"Did not find a valid value for attribute '{attribute_name}' "
+                    f"for object '{object_name}'."
+                )
             )
 
     async def utter_objects(
         self,
         dispatcher: CollectingDispatcher,
         object_type: Text,
         objects: List[Dict[Text, Any]],
```

### Comparing `rasa_sdk-3.5.1/rasa_sdk/knowledge_base/storage.py` & `rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 logger = logging.getLogger(__name__)
 
 
 class KnowledgeBase:
     def __init__(self) -> None:
 
         self.ordinal_mention_mapping = {
-            "1": lambda l: l[0],
-            "2": lambda l: l[1],
-            "3": lambda l: l[2],
-            "4": lambda l: l[3],
-            "5": lambda l: l[4],
-            "6": lambda l: l[5],
-            "7": lambda l: l[6],
-            "8": lambda l: l[7],
-            "9": lambda l: l[8],
-            "10": lambda l: l[9],
-            "ANY": lambda l: random.choice(l),
-            "LAST": lambda l: l[-1],
+            "1": lambda lst: lst[0],
+            "2": lambda lst: lst[1],
+            "3": lambda lst: lst[2],
+            "4": lambda lst: lst[3],
+            "5": lambda lst: lst[4],
+            "6": lambda lst: lst[5],
+            "7": lambda lst: lst[6],
+            "8": lambda lst: lst[7],
+            "9": lambda lst: lst[8],
+            "10": lambda lst: lst[9],
+            "ANY": lambda lst: random.choice(lst),
+            "LAST": lambda lst: lst[-1],
         }
 
         self.key_attribute: DefaultDict[Text, Text] = defaultdict(lambda: "id")
         self.representation_function: DefaultDict[
             Text, Callable[[Dict[Text, Text]], Text]
         ] = defaultdict(lambda: lambda obj: obj["name"])
 
@@ -135,15 +135,16 @@
         except OSError:
             raise ValueError(f"File '{self.data_file}' does not exist.")
 
         try:
             self.data = json.loads(content)
         except ValueError as e:
             raise ValueError(
-                f"Failed to read json from '{os.path.abspath(self.data_file)}'. Error: {e}"
+                f"Failed to read json from "
+                f"'{os.path.abspath(self.data_file)}'. Error: {e}"
             )
 
     def set_representation_function_of_object(
         self, object_type: Text, representation_function: Callable
     ) -> None:
         """
         Set the representation function of the given object type.
```

### Comparing `rasa_sdk-3.5.1/rasa_sdk/knowledge_base/utils.py` & `rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from rasa_sdk.events import SlotSet
-from typing import Text, Callable, Dict, List, Any, Optional
+from typing import Text, Callable, Dict, List, Optional
 import typing
 
 SLOT_MENTION = "mention"
 SLOT_OBJECT_TYPE = "object_type"
 SLOT_ATTRIBUTE = "attribute"
 SLOT_LISTED_OBJECTS = "knowledge_base_listed_objects"
 SLOT_LAST_OBJECT = "knowledge_base_last_object"
@@ -22,15 +22,16 @@
     Get the name of the object the user referred to. Either the NER detected the
     object and stored its name in the corresponding slot (e.g. "PastaBar"
     is detected as "restaurant") or the user referred to the object by any kind of
     mention, such as "first one" or "it".
 
     Args:
         tracker: the tracker
-        ordinal_mention_mapping: mapping that maps an ordinal mention to an object in a list
+        ordinal_mention_mapping: mapping that maps
+                                 an ordinal mention to an object in a list
         use_last_object_mention: if true the last mentioned object is returned if
         no other mention could be detected
 
     Returns: the name of the actual object (value of key attribute in the
     knowledge base)
     """
     mention = tracker.get_slot(SLOT_MENTION)
@@ -67,15 +68,16 @@
     as a list. We resolve the mention, such as 'the first one', to the list index
     and retrieve the actual object (using the 'ordinal_mention_mapping').
     For any other mention, such as 'it' or 'that restaurant', we just assume the
     user is referring to the last mentioned object in the conversation.
 
     Args:
         tracker: the tracker
-        ordinal_mention_mapping: mapping that maps an ordinal mention to an object in a list
+        ordinal_mention_mapping: mapping that maps an ordinal mention
+                                 to an object in a list
 
     Returns: name of the actually object
     """
 
     mention = tracker.get_slot(SLOT_MENTION)
     listed_items = tracker.get_slot(SLOT_LISTED_OBJECTS)
     last_object = tracker.get_slot(SLOT_LAST_OBJECT)
```

### Comparing `rasa_sdk-3.5.1/rasa_sdk/slots.py` & `rasa_sdk-3.6.0a1/rasa_sdk/slots.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/rasa_sdk/types.py` & `rasa_sdk-3.6.0a1/rasa_sdk/types.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.1/rasa_sdk/utils.py` & `rasa_sdk-3.6.0a1/rasa_sdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,17 @@
 def arguments_of(func) -> AbstractSet[Text]:
     """Return the parameters of the function `func` as a list of their names."""
     return inspect.signature(func).parameters.keys()
 
 
 def number_of_sanic_workers() -> int:
     """Get the number of Sanic workers to use in `app.run()`.
-    If the environment variable `constants.ENV_SANIC_WORKERS` is set and is not equal to 1.
+
+    If the environment variable `constants.ENV_SANIC_WORKERS`
+    is set and is not equal to 1.
     """
 
     def _log_and_get_default_number_of_workers():
         logger.debug(
             f"Using the default number of Sanic workers ({DEFAULT_SANIC_WORKERS})."
         )
         return DEFAULT_SANIC_WORKERS
```

### Comparing `rasa_sdk-3.5.1/setup.py` & `rasa_sdk-3.6.0a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,187 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rasa-sdk
+Version: 3.6.0a1
+Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
+Home-page: https://rasa.com
+License: Apache-2.0
+Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
+Author: Rasa Technologies GmbH
+Author-email: hi@rasa.com
+Maintainer: Tom Bocklisch
+Maintainer-email: tom@rasa.com
+Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: Sanic-Cors (>=2.0.0,<3.0.0)
+Requires-Dist: coloredlogs (>=10,<16)
+Requires-Dist: pluggy (>=1.0.0,<2.0.0)
+Requires-Dist: prompt-toolkit (>=3.0,<3.0.29)
+Requires-Dist: ruamel.yaml (>=0.16.5,<0.18.0)
+Requires-Dist: sanic (>=21.12.0,<22.0.0)
+Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
+Requires-Dist: websockets (>=10.0,<11.0)
+Project-URL: Documentation, https://rasa.com/docs
+Project-URL: Repository, https://github.com/rasahq/rasa-sdk
+Description-Content-Type: text/markdown
+
+# Rasa Python-SDK
+[![Join the chat on Rasa Community Forum](https://img.shields.io/badge/forum-join%20discussions-brightgreen.svg)](https://forum.rasa.com/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Build Status](https://github.com/RasaHQ/rasa-sdk/workflows/Continous%20Integration/badge.svg?event=push)](https://github.com/RasaHQ/rasa-sdk/actions/runs/)
+[![Coverage Status](https://coveralls.io/repos/github/RasaHQ/rasa-sdk/badge.svg?branch=main)](https://coveralls.io/github/RasaHQ/rasa-sdk?branch=main)
+[![PyPI version](https://img.shields.io/pypi/v/rasa-sdk.svg)](https://pypi.python.org/pypi/rasa-sdk)
+
+Python SDK for the development of custom actions for Rasa.
+
+<hr />
+
+💡 **We're migrating issues to Jira** 💡
+
+Starting January 2023, issues for Rasa Open Source are located in
+[this Jira board](https://rasa-open-source.atlassian.net/browse/OSS). You can browse issues without being logged in;
+if you want to create issues, you'll need to create a Jira account.
+
+<hr />
+
+## Installation
+
+To install the SDK run
+
+```bash
+pip install rasa-sdk
+```
+
+## Compatibility
+
+`rasa-sdk` package:
+
+| SDK version    | compatible Rasa version           |
+|----------------|-----------------------------------|
+| `1.0.x`        | `>=1.0.x`                         |
+
+old `rasa_core_sdk` package:
+
+| SDK version    | compatible Rasa Core version           |
+|----------------|----------------------------------------|
+| `0.12.x`       | `>=0.12.x`                             |
+| `0.11.x`       | `0.11.x`                               |
+| not compatible | `<=0.10.x`                             |
+
+## Usage
+
+Detailed instructions can be found in the Rasa Documentation about
+[Custom Actions](https://rasa.com/docs/rasa/core/actions).
+
+## Docker
+
+### Usage
+
+In order to start an action server using implemented custom actions,
+you can use the available Docker image `rasa/rasa-sdk`.
+
+Before starting the action server ensure that the folder containing
+your actions is handled as Python module and therefore has to contain
+a file called `__init__.py`
+
+Then start the action server using:
+
+```bash
+docker run -p 5055:5055 --mount type=bind,source=<ABSOLUTE_PATH_TO_YOUR_ACTIONS>,target=/app/actions \
+	rasa/rasa-sdk:<version>
+```
+
+The action server is then available at `http://localhost:5055/webhook`.
+
+### Custom Dependencies
+
+To add custom dependencies you enhance the given Docker image, e.g.:
+
+```
+# Extend the official Rasa SDK image
+FROM rasa/rasa-sdk:<version>
+
+# Change back to root user to install dependencies
+USER root
+
+# To install system dependencies
+RUN apt-get update -qq && \
+    apt-get install -y <NAME_OF_REQUIRED_PACKAGE> && \
+    apt-get clean && \
+    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
+
+# To install packages from PyPI
+RUN pip install --no-cache-dir <A_REQUIRED_PACKAGE_ON_PYPI>
+
+# Switch back to non-root to run code
+USER 1001
+```
+
+## Building from source
+
+Rasa SDK uses Poetry for packaging and dependency management. If you want to build it from source,
+you have to install Poetry first. This is how it can be done:
+
+```
+curl -sSL https://install.python-poetry.org | python3 -
+```
+
+There are several other ways to install Poetry. Please, follow
+[the official guide](https://python-poetry.org/docs/#installation) to see all possible options.
+
+To install dependencies and `rasa-sdk` itself in editable mode execute
+```
+make install
+```
+
+## Code Style
+
+To ensure a standardized code style we use the formatter [black](https://github.com/ambv/black).
+If your code is not formatted properly, GitHub CI will fail to build.
+
+If you want to automatically format your code on every commit, you can use [pre-commit](https://pre-commit.com/).
+Just install it via `pip install pre-commit` and execute `pre-commit install`.
+
+To check and reformat files execute
+```
+make lint
+```
+
+## Steps to release a new version
+Releasing a new version is quite simple, as the packages are build and distributed
+by GitHub Actions.
+
+*Release steps*:
+1. Switch to the branch you want to cut the release from (`main` in case of a
+  major / minor, the current release branch for patch releases).
+2. If this is a minor / major release: Make sure all fixes from currently supported minor versions have been merged from their respective release branches (e.g. 3.3.x) back into main.
+3. Run `make release`
+4. Create a PR against main or the release branch (e.g. `1.2.x`)
+5. Once your PR is merged, pull the release branch locally.
+6. Create a tag for a new release (this SHOULD always happen on `main` or release branches), e.g. using
+    ```bash
+    git tag 1.2.0 -m "next release"
+    git push origin 1.2.0
+    ```
+    GitHub Actions will build this tag and push a package to
+    [pypi](https://pypi.python.org/pypi/rasa-sdk).
+6. **If this is a minor release**, a new release branch should be created
+  pointing to the same commit as the tag to allow for future patch releases,
+  e.g.
+    ```bash
+    git checkout -b 1.2.x
+    git push origin 1.2.x
+    ```
+
+## License
+Licensed under the Apache License, Version 2.0. Copyright 2021 Rasa
+Technologies GmbH. [Copy of the license](LICENSE.txt).
+
+A list of the Licenses of the dependencies of the project can be found at
+the bottom of the
+[Libraries Summary](https://libraries.io/github/RasaHQ/rasa-sdk).
 
-packages = \
-['rasa_sdk', 'rasa_sdk.cli', 'rasa_sdk.knowledge_base']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Sanic-Cors>=2.0.0,<3.0.0',
- 'coloredlogs>=10,<16',
- 'prompt-toolkit>=3.0,<3.0.29',
- 'ruamel.yaml>=0.16.5,<0.18.0',
- 'sanic>=21.12.0,<22.0.0',
- 'typing-extensions>=4.1.1,<5.0.0',
- 'websockets>=10.0,<11.0']
-
-setup_kwargs = {
-    'name': 'rasa-sdk',
-    'version': '3.5.1',
-    'description': 'Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants',
-    'long_description': '# Rasa Python-SDK\n[![Join the chat on Rasa Community Forum](https://img.shields.io/badge/forum-join%20discussions-brightgreen.svg)](https://forum.rasa.com/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)\n[![Build Status](https://github.com/RasaHQ/rasa-sdk/workflows/Continous%20Integration/badge.svg?event=push)](https://github.com/RasaHQ/rasa-sdk/actions/runs/)\n[![Coverage Status](https://coveralls.io/repos/github/RasaHQ/rasa-sdk/badge.svg?branch=main)](https://coveralls.io/github/RasaHQ/rasa-sdk?branch=main)\n[![PyPI version](https://img.shields.io/pypi/v/rasa-sdk.svg)](https://pypi.python.org/pypi/rasa-sdk)\n\nPython SDK for the development of custom actions for Rasa.\n\n<hr />\n\n💡 **We\'re migrating issues to Jira** 💡\n\nStarting January 2023, issues for Rasa Open Source are located in\n[this Jira board](https://rasa-open-source.atlassian.net/browse/OSS). You can browse issues without being logged in;\nif you want to create issues, you\'ll need to create a Jira account.\n\n<hr />\n\n## Installation\n\nTo install the SDK run\n\n```bash\npip install rasa-sdk\n```\n\n## Compatibility\n\n`rasa-sdk` package:\n\n| SDK version    | compatible Rasa version           |\n|----------------|-----------------------------------|\n| `1.0.x`        | `>=1.0.x`                         |\n\nold `rasa_core_sdk` package:\n\n| SDK version    | compatible Rasa Core version           |\n|----------------|----------------------------------------|\n| `0.12.x`       | `>=0.12.x`                             |\n| `0.11.x`       | `0.11.x`                               |\n| not compatible | `<=0.10.x`                             |\n\n## Usage\n\nDetailed instructions can be found in the Rasa Documentation about\n[Custom Actions](https://rasa.com/docs/rasa/core/actions).\n\n## Docker\n\n### Usage\n\nIn order to start an action server using implemented custom actions,\nyou can use the available Docker image `rasa/rasa-sdk`.\n\nBefore starting the action server ensure that the folder containing\nyour actions is handled as Python module and therefore has to contain\na file called `__init__.py`\n\nThen start the action server using:\n\n```bash\ndocker run -p 5055:5055 --mount type=bind,source=<ABSOLUTE_PATH_TO_YOUR_ACTIONS>,target=/app/actions \\\n\trasa/rasa-sdk:<version>\n```\n\nThe action server is then available at `http://localhost:5055/webhook`.\n\n### Custom Dependencies\n\nTo add custom dependencies you enhance the given Docker image, e.g.:\n\n```\n# Extend the official Rasa SDK image\nFROM rasa/rasa-sdk:<version>\n\n# Change back to root user to install dependencies\nUSER root\n\n# To install system dependencies\nRUN apt-get update -qq && \\\n    apt-get install -y <NAME_OF_REQUIRED_PACKAGE> && \\\n    apt-get clean && \\\n    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*\n\n# To install packages from PyPI\nRUN pip install --no-cache-dir <A_REQUIRED_PACKAGE_ON_PYPI>\n\n# Switch back to non-root to run code\nUSER 1001\n```\n\n\n## Building from source\n\nRasa SDK uses Poetry for packaging and dependency management. If you want to build it from source,\nyou have to install Poetry first. This is how it can be done:\n\n```\ncurl -sSL https://install.python-poetry.org | python3 -\n```\n\nThere are several other ways to install Poetry. Please, follow\n[the official guide](https://python-poetry.org/docs/#installation) to see all possible options.\n\nTo install dependencies and `rasa-sdk` itself in editable mode execute\n```\nmake install\n```\n\n## Code Style\n\nTo ensure a standardized code style we use the formatter [black](https://github.com/ambv/black).\nIf your code is not formatted properly, GitHub CI will fail to build.\n\nIf you want to automatically format your code on every commit, you can use [pre-commit](https://pre-commit.com/).\nJust install it via `pip install pre-commit` and execute `pre-commit install`.\n\nTo check and reformat files execute\n```\nmake lint\n```\n\n## Steps to release a new version\nReleasing a new version is quite simple, as the packages are build and distributed\nby GitHub Actions.\n\n*Release steps*:\n1. Switch to the branch you want to cut the release from (`main` in case of a\n  major / minor, the current release branch for patch releases).\n2. If this is a minor / major release: Make sure all fixes from currently supported minor versions have been merged from their respective release branches (e.g. 3.3.x) back into main.\n3. Run `make release`\n4. Create a PR against main or the release branch (e.g. `1.2.x`)\n5. Once your PR is merged, tag a new release (this SHOULD always happen on\n  `main` or release branches), e.g. using\n    ```bash\n    git tag 1.2.0 -m "next release"\n    git push origin 1.2.0\n    ```\n    GitHub Actions will build this tag and push a package to\n    [pypi](https://pypi.python.org/pypi/rasa-sdk).\n6. **If this is a minor release**, a new release branch should be created\n  pointing to the same commit as the tag to allow for future patch releases,\n  e.g.\n    ```bash\n    git checkout -b 1.2.x\n    git push origin 1.2.x\n    ```\n\n## License\nLicensed under the Apache License, Version 2.0. Copyright 2021 Rasa\nTechnologies GmbH. [Copy of the license](LICENSE.txt).\n\nA list of the Licenses of the dependencies of the project can be found at\nthe bottom of the\n[Libraries Summary](https://libraries.io/github/RasaHQ/rasa-sdk).\n',
-    'author': 'Rasa Technologies GmbH',
-    'author_email': 'hi@rasa.com',
-    'maintainer': 'Tom Bocklisch',
-    'maintainer_email': 'tom@rasa.com',
-    'url': 'https://rasa.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

