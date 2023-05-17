# Comparing `tmp/cohere-4.4.2.tar.gz` & `tmp/cohere-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-4.4.2.tar", max compression
+gzip compressed data, was "cohere-4.5.0.tar", max compression
```

## Comparing `cohere-4.4.2.tar` & `cohere-4.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1063 2023-05-17 10:42:54.821429 cohere-4.4.2/LICENSE
--rw-r--r--   0        0        0     4480 2023-05-17 10:42:54.821429 cohere-4.4.2/README.md
--rw-r--r--   0        0        0      771 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/__init__.py
--rw-r--r--   0        0        0    38039 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/client.py
--rw-r--r--   0        0        0    28351 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/client_async.py
--rw-r--r--   0        0        0     1187 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/error.py
--rw-r--r--   0        0        0      529 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/logging.py
--rw-r--r--   0        0        0      839 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/__init__.py
--rw-r--r--   0        0        0     2678 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/base.py
--rw-r--r--   0        0        0     3438 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/bulk_embed.py
--rw-r--r--   0        0        0     3501 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/chat.py
--rw-r--r--   0        0        0     1461 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/classify.py
--rw-r--r--   0        0        0     4826 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/cluster.py
--rw-r--r--   0        0        0      436 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/codebook.py
--rw-r--r--   0        0        0      552 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/detectlang.py
--rw-r--r--   0        0        0      587 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/embeddings.py
--rw-r--r--   0        0        0      342 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/feedback.py
--rw-r--r--   0        0        0     5990 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/generation.py
--rw-r--r--   0        0        0     2057 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/rerank.py
--rw-r--r--   0        0        0      667 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/summarize.py
--rw-r--r--   0        0        0     1221 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/responses/tokenize.py
--rw-r--r--   0        0        0     2614 2023-05-17 10:42:54.821429 cohere-4.4.2/cohere/utils.py
--rw-r--r--   0        0        0      653 2023-05-17 10:42:54.821429 cohere-4.4.2/pyproject.toml
--rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.4.2/setup.py
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-17 11:31:24.168947 cohere-4.5.0/LICENSE
+-rw-r--r--   0        0        0     4480 2023-05-17 11:31:24.168947 cohere-4.5.0/README.md
+-rw-r--r--   0        0        0      771 2023-05-17 11:31:24.168947 cohere-4.5.0/cohere/__init__.py
+-rw-r--r--   0        0        0    39032 2023-05-17 11:31:24.168947 cohere-4.5.0/cohere/client.py
+-rw-r--r--   0        0        0    28190 2023-05-17 11:31:24.168947 cohere-4.5.0/cohere/client_async.py
+-rw-r--r--   0        0        0     1187 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/error.py
+-rw-r--r--   0        0        0      529 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/logging.py
+-rw-r--r--   0        0        0      839 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/__init__.py
+-rw-r--r--   0        0        0     2678 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/base.py
+-rw-r--r--   0        0        0     3438 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/bulk_embed.py
+-rw-r--r--   0        0        0     3501 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/chat.py
+-rw-r--r--   0        0        0     1461 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/classify.py
+-rw-r--r--   0        0        0     4826 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/cluster.py
+-rw-r--r--   0        0        0      436 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/codebook.py
+-rw-r--r--   0        0        0      552 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/detectlang.py
+-rw-r--r--   0        0        0      587 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/embeddings.py
+-rw-r--r--   0        0        0      342 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/feedback.py
+-rw-r--r--   0        0        0     5990 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/generation.py
+-rw-r--r--   0        0        0     2057 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/rerank.py
+-rw-r--r--   0        0        0      667 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/summarize.py
+-rw-r--r--   0        0        0     1221 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/responses/tokenize.py
+-rw-r--r--   0        0        0     3283 2023-05-17 11:31:24.172947 cohere-4.5.0/cohere/utils.py
+-rw-r--r--   0        0        0      653 2023-05-17 11:31:24.172947 cohere-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.5.0/setup.py
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.5.0/PKG-INFO
```

### Comparing `cohere-4.4.2/LICENSE` & `cohere-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/README.md` & `cohere-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/__init__.py` & `cohere-4.5.0/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/client.py` & `cohere-4.5.0/cohere/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json as jsonlib
 import os
-from concurrent import futures
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import asdict
 from functools import partial
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 from requests.adapters import HTTPAdapter
@@ -32,15 +31,15 @@
 from cohere.responses.feedback import (
     GenerateFeedbackResponse,
     GeneratePreferenceFeedbackResponse,
     PreferenceRating,
 )
 from cohere.responses.rerank import Reranking
 from cohere.responses.summarize import SummarizeResponse
-from cohere.utils import is_api_key_valid, wait_for_job
+from cohere.utils import is_api_key_valid, threadpool_map, wait_for_job
 
 
 class Client:
     """Cohere Client
 
     Args:
         api_key (str): Your API key.
@@ -82,19 +81,30 @@
         """
         Checks the api key, which happens automatically during Client initialization, but not in AsyncClient.
         check_api_key raises an exception when the key is invalid, but the return value for valid keys is kept for
         backwards compatibility.
         """
         return {"valid": is_api_key_valid(self.api_key)}
 
-    def batch_generate(self, prompts: List[str], **kwargs) -> List[Generations]:
-        """A batched version of generate with multiple prompts."""
-        with futures.ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-            res = executor.map(lambda prompt: self.generate(prompt=prompt, **kwargs), prompts)
-        return list(res)
+    def batch_generate(
+        self, prompts: List[str], return_exceptions=False, **kwargs
+    ) -> List[Union[Generations, Exception]]:
+        """A batched version of generate with multiple prompts.
+
+        Args:
+            prompts: list of prompts
+            return_exceptions (bool): Return exceptions as list items rather than raise them. Ensures your entire batch is not lost on one of the items failing.
+            kwargs: other arguments to `generate`
+        """
+        return threadpool_map(
+            self.generate,
+            [dict(prompt=prompt, **kwargs) for prompt in prompts],
+            num_workers=self.num_workers,
+            return_exceptions=return_exceptions,
+        )
 
     def generate(
         self,
         prompt: Optional[str] = None,
         prompt_vars: object = {},
         model: Optional[str] = None,
         preset: Optional[str] = None,
@@ -448,35 +458,53 @@
         }
         # remove None values from the dict
         json_body = {k: v for k, v in json_body.items() if v is not None}
         response = self._request(cohere.SUMMARIZE_URL, json=json_body)
 
         return SummarizeResponse(id=response["id"], summary=response["summary"], meta=response["meta"])
 
-    def batch_tokenize(self, texts: List[str]) -> List[Tokens]:
-        """A batched version of tokenize"""
-        with futures.ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-            res = executor.map(self.tokenize, texts)
-        return list(res)
+    def batch_tokenize(self, texts: List[str], return_exceptions=False) -> List[Union[Tokens, Exception]]:
+        """A batched version of tokenize.
+
+        Args:
+            texts: list of texts
+            return_exceptions (bool): Return exceptions as list items rather than raise them. Ensures your entire batch is not lost on one of the items failing.
+        """
+        return threadpool_map(
+            self.tokenize,
+            [dict(text=text) for text in texts],
+            num_workers=self.num_workers,
+            return_exceptions=return_exceptions,
+        )
 
     def tokenize(self, text: str) -> Tokens:
         """Returns a Tokens object of the provided text, see https://docs.cohere.ai/reference/tokenize for advanced usage.
 
         Args:
             text (str): Text to summarize.
         """
         json_body = {"text": text}
         res = self._request(cohere.TOKENIZE_URL, json=json_body)
         return Tokens(tokens=res["tokens"], token_strings=res["token_strings"], meta=res.get("meta"))
 
-    def batch_detokenize(self, list_of_tokens: List[List[int]]) -> List[Detokenization]:
-        """A batched version of detokenize"""
-        with futures.ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-            res = executor.map(self.detokenize, list_of_tokens)
-        return list(res)
+    def batch_detokenize(
+        self, list_of_tokens: List[List[int]], return_exceptions=False
+    ) -> List[Union[Detokenization, Exception]]:
+        """A batched version of detokenize.
+
+        Args:
+            list_of_tokens: list of list of tokens
+            return_exceptions (bool): Return exceptions as list items rather than raise them. Ensures your entire batch is not lost on one of the items failing.
+        """
+        return threadpool_map(
+            self.detokenize,
+            [dict(tokens=tokens) for tokens in list_of_tokens],
+            num_workers=self.num_workers,
+            return_exceptions=return_exceptions,
+        )
 
     def detokenize(self, tokens: List[int]) -> Detokenization:
         """Returns a Detokenization object of the provided tokens, see https://docs.cohere.ai/reference/detokenize for advanced usage.
 
         Args:
             tokens (List[int]): A list of tokens to convert to strings
         """
```

### Comparing `cohere-4.4.2/cohere/client_async.py` & `cohere-4.5.0/cohere/client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,15 @@
 
 
 class AsyncClient(Client):
     """AsyncClient
 
     This client provides an asyncio/aiohttp interface.
     Using this client is recommended when you are making highly parallel request,
-    or when calling the Cohere API from a server such as FastAPI.
-
-    The methods here are typically identical to those in the main `Client`, with an extra argument
-    `return_exceptions` for the batch* methods, which is passed to asyncio.gather."""
+    or when calling the Cohere API from a server such as FastAPI."""
 
     def __init__(
         self,
         api_key: str = None,
         num_workers: int = 16,
         request_dict: dict = {},
         check_api_key: bool = True,
@@ -114,16 +111,17 @@
     async def check_api_key(self) -> Dict[str, bool]:
         """
         check_api_key raises an exception when the key is invalid, but the return value for valid keys is kept for
         backwards compatibility.
         """
         return {"valid": is_api_key_valid(self.api_key)}
 
-    async def batch_generate(self, prompts: List[str], return_exceptions=False, **kwargs) -> List[Generations]:
-        """return_exceptions is passed to asyncio.gather"""
+    async def batch_generate(
+        self, prompts: List[str], return_exceptions=False, **kwargs
+    ) -> List[Union[Exception, Generations]]:
         return await asyncio.gather(
             *[self.generate(prompt, **kwargs) for prompt in prompts], return_exceptions=return_exceptions
         )
 
     async def generate(
         self,
         prompt: Optional[str] = None,
@@ -323,23 +321,25 @@
             "extractiveness": extractiveness,
         }
         # remove None values from the dict
         json_body = {k: v for k, v in json_body.items() if v is not None}
         response = await self._request(cohere.SUMMARIZE_URL, json=json_body)
         return SummarizeResponse(id=response["id"], summary=response["summary"], meta=response["meta"])
 
-    async def batch_tokenize(self, texts: List[str], return_exceptions=False) -> List[Tokens]:
+    async def batch_tokenize(self, texts: List[str], return_exceptions=False) -> List[Union[Tokens, Exception]]:
         return await asyncio.gather(*[self.tokenize(t) for t in texts], return_exceptions=return_exceptions)
 
     async def tokenize(self, text: str) -> Tokens:
         json_body = {"text": text}
         res = await self._request(cohere.TOKENIZE_URL, json_body)
         return Tokens(tokens=res["tokens"], token_strings=res["token_strings"], meta=res["meta"])
 
-    async def batch_detokenize(self, list_of_tokens: List[List[int]], return_exceptions=False) -> List[Detokenization]:
+    async def batch_detokenize(
+        self, list_of_tokens: List[List[int]], return_exceptions=False
+    ) -> List[Union[Detokenization, Exception]]:
         return await asyncio.gather(*[self.detokenize(t) for t in list_of_tokens], return_exceptions=return_exceptions)
 
     async def detokenize(self, tokens: List[int]) -> Detokenization:
         json_body = {"tokens": tokens}
         res = await self._request(cohere.DETOKENIZE_URL, json_body)
         return Detokenization(text=res["text"], meta=res["meta"])
```

### Comparing `cohere-4.4.2/cohere/error.py` & `cohere-4.5.0/cohere/error.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/logging.py` & `cohere-4.5.0/cohere/logging.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/__init__.py` & `cohere-4.5.0/cohere/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/base.py` & `cohere-4.5.0/cohere/responses/base.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/bulk_embed.py` & `cohere-4.5.0/cohere/responses/bulk_embed.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/chat.py` & `cohere-4.5.0/cohere/responses/chat.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/classify.py` & `cohere-4.5.0/cohere/responses/classify.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/cluster.py` & `cohere-4.5.0/cohere/responses/cluster.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/detectlang.py` & `cohere-4.5.0/cohere/responses/detectlang.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/embeddings.py` & `cohere-4.5.0/cohere/responses/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/generation.py` & `cohere-4.5.0/cohere/responses/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/rerank.py` & `cohere-4.5.0/cohere/responses/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/summarize.py` & `cohere-4.5.0/cohere/responses/summarize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/responses/tokenize.py` & `cohere-4.5.0/cohere/responses/tokenize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.4.2/cohere/utils.py` & `cohere-4.5.0/cohere/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import asyncio
 import json
 import time
-import typing
-from typing import Awaitable, Callable, Optional, TypeVar
+from concurrent import futures
+from typing import Awaitable, Callable, Dict, List, Optional, TypeVar
 
 from cohere.error import CohereError
 
 try:  # numpy is optional, but support json encoding if the user has it
     import numpy as np
 
     class CohereJsonEncoder(json.JSONEncoder):
@@ -37,15 +37,15 @@
                 return super().default(obj)
 
 
 def np_json_dumps(data, **kwargs):
     return json.dumps(data, cls=CohereJsonEncoder, **kwargs)
 
 
-def is_api_key_valid(key: typing.Optional[str]) -> bool:
+def is_api_key_valid(key: Optional[str]) -> bool:
     """is_api_key_valid returns True when the key is valid and raises a CohereError when it is invalid."""
     if not key:
         raise CohereError(
             "No API key provided. Provide the API key in the client initialization or the CO_API_KEY environment variable."  # noqa: E501
         )
 
     return True
@@ -90,7 +90,23 @@
         if timeout is not None and time.time() - start_time > timeout:
             raise TimeoutError(f"wait_for_job timed out after {timeout} seconds")
 
         await asyncio.sleep(interval)
         job = await get_job()
 
     return job
+
+
+def threadpool_map(f, call_args: List[Dict], num_workers, return_exceptions: bool = False) -> List:
+    """Helper function similar to futures.ThreadPoolExecutor.map, but allows returning exceptions"""
+    results = []
+    with futures.ThreadPoolExecutor(max_workers=num_workers) as executor:
+        futures_list = [executor.submit(f, **args) for args in call_args]
+        for future in futures_list:
+            try:
+                results.append(future.result())
+            except Exception as e:
+                if return_exceptions:
+                    results.append(e)
+                else:
+                    raise
+    return results
```

### Comparing `cohere-4.4.2/pyproject.toml` & `cohere-4.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "4.4.2"
+version = "4.5.0"
 description = ""
 authors = ["Cohere"]
 readme = "README.md"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
```

### Comparing `cohere-4.4.2/setup.py` & `cohere-4.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0,<4.0', 'backoff>=2.0,<3.0', 'requests>=2.0,<3.0']
 
 setup_kwargs = {
     'name': 'cohere',
-    'version': '4.4.2',
+    'version': '4.5.0',
     'description': '',
     'long_description': '![ci badge](https://github.com/cohere-ai/cohere-python/actions/workflows/test.yaml/badge.svg)\n![version badge](https://img.shields.io/pypi/v/cohere)\n![license badge](https://img.shields.io/github/license/cohere-ai/cohere-python)\n\n# Cohere Python SDK\n\nThis package provides functionality developed to simplify interfacing with the [Cohere API](https://docs.cohere.ai/) in Python 3.\n\n## Documentation\n\n* SDK Documentation is hosted on [Read the docs](https://cohere-sdk.readthedocs.io/en/latest/).\n  * You can build SDK documentation locally using `cd docs; make clean html`.\n* For more details on advanced parameters, you can also consult the [API documentation](https://docs.cohere.ai/reference/about).\n* See the [examples](examples/) directory for examples, including  some additional functionality for visualizations in Jupyter notebooks.\n\n## Installation\n\nThe package can be installed with `pip`:\n\n```bash\npip install --upgrade cohere\n```\n\nInstall from source:\n\n```bash\npip install .\n```\n\n### Requirements\n\n- Python 3.7+\n\n## Quick Start\n\nTo use this library, you must have an API key and specify it as a string when creating the `cohere.Client` object. API keys can be created through the [platform](https://os.cohere.ai). This is a basic example of the creating the client and using the `generate` endpoint.\n\n```python\nimport cohere\n\n# initialize the Cohere Client with an API Key\nco = cohere.Client(\'YOUR_API_KEY\')\n\n# generate a prediction for a prompt\nprediction = co.generate(\n            model=\'large\',\n            prompt=\'co:here\',\n            max_tokens=10)\n\n# print the predicted text\nprint(\'prediction: {}\'.format(prediction.generations[0].text))\n```\n\nThere is also an asyncio compatible client called `cohere.AsyncClient` with an equivalent interface. Consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) for more details.\n\n## Versioning\n\nEach SDK release is only compatible with the latest version of the Cohere API at the time of release. To use the SDK with an older API version, you need to download a version of the SDK tied to the API version you want. Look at the [Changelog](https://github.com/cohere-ai/cohere-python/blob/main/CHANGELOG.md) to see which SDK version to download.\n\n\n## Endpoints\n\nFor a full breakdown of endpoints and arguments, please consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere API Docs](https://docs.cohere.ai/).\n\n| Cohere Endpoint  | Function             |\n| ---------------- | -------------------- |\n| /generate        | co.generate()        |\n| /embed           | co.embed()           |\n| /classify        | co.classify()        |\n| /tokenize        | co.tokenize()        |\n| /detokenize      | co.detokenize()      |\n| /detect-language | co.detect_language() |\n\n## Models\n\nWhen you call Cohere\'s APIs we decide on a good default model for your use-case behind the scenes. The default model is great to get you started, but in production environments we recommend that you specify the model size yourself via the `model` parameter. Learn more about the available models here(https://os.cohere.ai)\n\n## Responses\n\nAll of the endpoint functions will return a Cohere object corresponding to the endpoint (e.g. for generation, it would be `Generation`). The responses can be found as instance variables of the object (e.g. generation would be `Generation.text`). The names of these instance variables and a detailed breakdown of the response body can be found in the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere Docs](https://docs.cohere.ai/). Printing the Cohere response object itself will display an organized view of the instance variables.\n\n## Exceptions\n\nUnsuccessful API calls from the SDK will raise an exception. Please see the documentation\'s page on [errors](https://docs.cohere.ai/errors-reference) for more information about what the errors mean.\n\n## Contributing\n\nTo set up a development environment, run:\n\n```\npoetry shell    # any time you want to run code or tests\npoetry install  # install and update dependencies in your environment, the first time\n```\n\nIn addition, to ensure your code is formatted correctly, install pre-commit hooks using:\n\n```bash\npre-commit install\n```\n\nYou can run tests locally using:\n```\npython -m pytest\n```\n\nYou can configure a different base url with:\n```bash\nCO_API_URL="https://localhost:8050" python3 foo.py\n```\nor\n```python\ncohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization\n```\n',
     'author': 'Cohere',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cohere-4.4.2/PKG-INFO` & `cohere-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 4.4.2
+Version: 4.5.0
 Summary: 
 Author: Cohere
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

