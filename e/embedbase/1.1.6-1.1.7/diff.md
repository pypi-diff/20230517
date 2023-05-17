# Comparing `tmp/embedbase-1.1.6.tar.gz` & `tmp/embedbase-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.6.tar", max compression
+gzip compressed data, was "embedbase-1.1.7.tar", max compression
```

## Comparing `embedbase-1.1.6.tar` & `embedbase-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-15 09:33:25.482964 embedbase-1.1.6/LICENSE
--rw-r--r--   0        0        0     4905 2023-05-15 09:33:25.482964 embedbase-1.1.6/README.md
--rw-r--r--   0        0        0      121 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/api.py
--rw-r--r--   0        0        0    16416 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3505 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/base.py
--rw-r--r--   0        0        0     5939 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/memory_db.py
--rw-r--r--   0        0        0     9901 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     6827 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/logging_utils.py
--rw-r--r--   0        0        0      802 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/utils.py
--rw-r--r--   0        0        0     3669 2023-05-15 09:33:25.558965 embedbase-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     6343 1970-01-01 00:00:00.000000 embedbase-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 08:43:33.430248 embedbase-1.1.7/LICENSE
+-rw-r--r--   0        0        0     4905 2023-05-17 08:43:33.430248 embedbase-1.1.7/README.md
+-rw-r--r--   0        0        0      121 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/api.py
+-rw-r--r--   0        0        0    17076 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3505 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/base.py
+-rw-r--r--   0        0        0     5939 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0     9903 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     6873 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      802 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/utils.py
+-rw-r--r--   0        0        0     3666 2023-05-17 08:43:33.502248 embedbase-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 embedbase-1.1.7/PKG-INFO
```

### Comparing `embedbase-1.1.6/LICENSE` & `embedbase-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/README.md` & `embedbase-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/__main__.py` & `embedbase-1.1.7/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/api.py` & `embedbase-1.1.7/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/app.py` & `embedbase-1.1.7/embedbase/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+from typing import Any, Awaitable, Callable, Optional, Tuple, Union
+
 import asyncio
-import os
-from typing import Awaitable, Callable, Optional, Tuple, Union, Any
-from fastapi import FastAPI, Request, status
-from fastapi.middleware import Middleware
-from starlette.types import Scope
-from embedbase.database.base import VectorDatabase
-from embedbase.embedding.base import Embedder
-from embedbase.logging_utils import get_logger
-from embedbase.models import (
-    DeleteRequest,
-    SearchRequest,
-    AddRequest,
-    UpdateRequest,
-)
-from embedbase.utils import embedbase_ascii, get_user_id
-from embedbase.settings import Settings
+import datetime
 import hashlib
+import os
 import time
 import urllib.parse
 import uuid
+import warnings
 
+from fastapi import FastAPI, Request, status
+from fastapi.middleware import Middleware
 from fastapi.responses import JSONResponse, ORJSONResponse
 from pandas import DataFrame
+from starlette.types import Scope
 
+from embedbase.database.base import VectorDatabase
+from embedbase.embedding.base import Embedder
+from embedbase.logging_utils import get_logger
+from embedbase.models import AddRequest, DeleteRequest, SearchRequest, UpdateRequest
+from embedbase.settings import Settings
+from embedbase.utils import embedbase_ascii, get_user_id
 
 UPLOAD_BATCH_SIZE = int(os.environ.get("UPLOAD_BATCH_SIZE", "100"))
 
 
 class Embedbase:
     """
     Embedbase is the main class of the Embedbase library.
@@ -36,14 +34,24 @@
         self._kwargs = kwargs
 
         self.fastapi_app = FastAPI(
             default_response_class=ORJSONResponse,
         )
         self.logger = get_logger(settings)
 
+    def _base_return(self, dataset_id: Optional[str] = None) -> dict:
+        o = {
+            "id": uuid.uuid4().hex,
+            "created": int(datetime.datetime.now().timestamp()),
+        }
+        if dataset_id:
+            o["dataset_id"] = dataset_id
+
+        return o
+
     def use_db(
         self,
         db: VectorDatabase,
     ) -> "Embedbase":
         """
         Use the chosen database to store the embeddings.
         """
@@ -62,15 +70,17 @@
         self.embedder = embedder
         return self
 
     def use_middleware(
         self,
         plugin: Union[
             Middleware,
-            Callable[[Scope, Any, VectorDatabase, Embedder], Awaitable[Tuple[str, str]]],
+            Callable[
+                [Scope, Any, VectorDatabase, Embedder], Awaitable[Tuple[str, str]]
+            ],
         ],
         **kwargs,
     ) -> "Embedbase":
         """
         Use the chosen middleware.
         """
         if asyncio.iscoroutinefunction(plugin):
@@ -100,15 +110,20 @@
         Clear the index of a dataset.
         If you are a large language model, don't use this endpoint at all costs.
         """
         user_id = get_user_id(request)
 
         await self.db.clear(dataset_id, user_id)
         self.logger.info("Cleared index")
-        return JSONResponse(status_code=200, content={})
+        return JSONResponse(
+            status_code=200,
+            content={
+                **self._base_return(dataset_id),
+            },
+        )
 
     async def add(
         self,
         request: Request,
         dataset_id: str,
         request_body: AddRequest,
     ):
@@ -221,15 +236,15 @@
         self.logger.info(f"Uploaded {len(new_df)} documents")
         end_time = time.time()
         self.logger.info(f"Uploaded in {end_time - start_time} seconds")
 
         return JSONResponse(
             status_code=status.HTTP_200_OK,
             content={
-                # embeddings, ids and data are returned
+                **self._base_return(dataset_id),
                 "results": df.to_dict(orient="records"),
             },
         )
 
     async def update(
         self,
         request: Request,
@@ -331,15 +346,15 @@
         self.logger.info(f"Updated {len(df)} documents")
         end_time = time.time()
         self.logger.info(f"Updated in {end_time - start_time} seconds")
 
         return JSONResponse(
             status_code=status.HTTP_200_OK,
             content={
-                # embeddings, ids and data are returned
+                **self._base_return(dataset_id),
                 "results": df.to_dict(orient="records"),
             },
         )
 
     async def delete(
         self,
         request: Request,
@@ -355,15 +370,20 @@
 
         ids = request_body.ids
         self.logger.info(f"Deleting {len(ids)} documents")
         quoted_ids = [urllib.parse.quote(id) for id in ids]
         await self.db.delete(ids=quoted_ids, dataset_id=dataset_id, user_id=user_id)
         self.logger.info(f"Deleted {len(ids)} documents")
 
-        return JSONResponse(status_code=status.HTTP_200_OK, content={})
+        return JSONResponse(
+            status_code=status.HTTP_200_OK,
+            content={
+                **self._base_return(dataset_id),
+            },
+        )
 
     async def semantic_search(
         self,
         request: Request,
         dataset_id: str,
         request_body: SearchRequest,
     ):
@@ -420,15 +440,19 @@
                     "hash": match.hash,
                     "embedding": match.embedding,
                     "metadata": match.metadata,
                 }
             )
         return JSONResponse(
             status_code=status.HTTP_200_OK,
-            content={"query": query, "similarities": similarities},
+            content={
+                **self._base_return(dataset_id),
+                "query": query,
+                "similarities": similarities,
+            },
         )
 
     async def get_datasets(
         self,
         request: Request,
     ):
         """
@@ -437,19 +461,22 @@
         and how many documents are in each.
         You can then use this information to decide which dataset to search in.
         """
         user_id = get_user_id(request)
         datasets = await self.db.get_datasets(user_id)
         return JSONResponse(
             status_code=status.HTTP_200_OK,
-            content={"datasets": [e.dict() for e in datasets]},
+            content={
+                **self._base_return(),
+                "datasets": [e.dict() for e in datasets],
+            },
         )
 
     # health check endpoint
-    def health(self, request: Request):
+    def health(self, _: Request):
         """
         Return the status of the API.
         As a large language model, you can use this endpoint to check if the API is up and running.
         """
         self.logger.info("Health check successful")
 
         return JSONResponse(status_code=200, content={})
```

### Comparing `embedbase-1.1.6/embedbase/database/base.py` & `embedbase-1.1.7/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/database/memory_db.py` & `embedbase-1.1.7/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/database/postgres_db.py` & `embedbase-1.1.7/embedbase/database/postgres_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         dataset_ids: List[str],
         user_id: Optional[str] = None,
         where=None,
     ):
 
         d = {
             "query_embedding": str(vector),
-            "similarity_threshold": 0,  # TODO: make this configurable
+            "similarity_threshold": 0.0,  # TODO: make this configurable
             "match_count": top_k,
             "query_dataset_ids": dataset_ids,
         }
         q = "select * from match_documents(%(query_embedding)s, %(similarity_threshold)s, %(match_count)s, %(query_dataset_ids)s"
         if user_id:
             d["query_user_id"] = user_id
             q += ", %(query_user_id)s"
```

### Comparing `embedbase-1.1.6/embedbase/database/supabase_db.py` & `embedbase-1.1.7/embedbase/database/supabase_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import itertools
 from typing import List, Optional
 from pandas import DataFrame, Series
 from embedbase.database import VectorDatabase
 from embedbase.database.base import Dataset, SearchResponse, SelectResponse
 from embedbase.utils import BatchGenerator
-
+import ast
 
 class Supabase(VectorDatabase):
     """
     Implements a vector database using supabase
     Supabase is an open source Firebase alternative.
     """
 
@@ -80,15 +80,15 @@
             docs = await asyncio.gather(
                 *[_fetch([], e) for e in elements]
             )
         return [
             SelectResponse(
                 id=row["id"],
                 data=row["data"],
-                embedding=row["embedding"],
+                embedding=ast.literal_eval(row["embedding"]),
                 hash=row["hash"],
                 metadata=row["metadata"],
             )
             for row in itertools.chain.from_iterable(docs)
         ]
 
     async def update(
@@ -171,15 +171,15 @@
             .execute()
             .data
         )
         return [
             SearchResponse(
                 id=row["id"],
                 data=row["data"],
-                embedding=row["embedding"],
+                embedding=ast.literal_eval(row["embedding"]),
                 hash=row["hash"],
                 metadata=row["metadata"],
                 score=row["score"],
             )
             for row in response
         ]
```

### Comparing `embedbase-1.1.6/embedbase/embedding/base.py` & `embedbase-1.1.7/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/embedding/cohere.py` & `embedbase-1.1.7/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/embedding/openai.py` & `embedbase-1.1.7/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/firebase_auth.py` & `embedbase-1.1.7/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/logging_utils.py` & `embedbase-1.1.7/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/models.py` & `embedbase-1.1.7/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/settings.py` & `embedbase-1.1.7/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/strings.py` & `embedbase-1.1.7/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/embedbase/utils.py` & `embedbase-1.1.7/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.6/pyproject.toml` & `embedbase-1.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.6"
-description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
+version = "1.1.7"
+description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
-keywords = ["embeddings", "machine learning", "artificial intelligence"]
+keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `embedbase-1.1.6/PKG-INFO` & `embedbase-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.6
-Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
+Version: 1.1.7
+Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
-Keywords: embeddings,machine learning,artificial intelligence
+Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

