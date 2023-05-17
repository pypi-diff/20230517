# Comparing `tmp/zep_python-0.24.tar.gz` & `tmp/zep_python-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.24.tar", max compression
+gzip compressed data, was "zep_python-0.25.tar", max compression
```

## Comparing `zep_python-0.24.tar` & `zep_python-0.25.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-15 20:33:14.641595 zep_python-0.24/LICENSE
--rw-r--r--   0        0        0    11572 2023-05-15 20:33:14.641595 zep_python-0.24/README.md
--rw-r--r--   0        0        0      775 2023-05-15 20:33:14.641595 zep_python-0.24/pyproject.toml
--rw-r--r--   0        0        0      340 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/exceptions.py
--rw-r--r--   0        0        0     4861 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/py.typed
--rw-r--r--   0        0        0      670 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/utils.py
--rw-r--r--   0        0        0    12664 2023-05-15 20:33:14.641595 zep_python-0.24/zep_python/zep_client.py
--rw-r--r--   0        0        0    12251 1970-01-01 00:00:00.000000 zep_python-0.24/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 05:23:06.606851 zep_python-0.25/LICENSE
+-rw-r--r--   0        0        0     2434 2023-05-17 05:23:06.606851 zep_python-0.25/README.md
+-rw-r--r--   0        0        0      775 2023-05-17 05:23:06.610851 zep_python-0.25/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/exceptions.py
+-rw-r--r--   0        0        0     4861 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/py.typed
+-rw-r--r--   0        0        0      670 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/utils.py
+-rw-r--r--   0        0        0    12621 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/zep_client.py
+-rw-r--r--   0        0        0     3113 1970-01-01 00:00:00.000000 zep_python-0.25/PKG-INFO
```

### Comparing `zep_python-0.24/LICENSE` & `zep_python-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.24/pyproject.toml` & `zep_python-0.25/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.24"
+version = "0.25"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
```

### Comparing `zep_python-0.24/zep_python/exceptions.py` & `zep_python-0.25/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.24/zep_python/models.py` & `zep_python-0.25/zep_python/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.24/zep_python/utils.py` & `zep_python-0.25/zep_python/utils.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.24/zep_python/zep_client.py` & `zep_python-0.25/zep_python/zep_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         exc_type: Type[Exception],
         exc_val: Exception,
         exc_tb: TracebackType,
     ) -> None:
         self.close()
 
     @sync
-    def get_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]:
+    def get_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
         Retrieve memory for the specified session. This method is a synchronous wrapper
         for the asynchronous method `aget_memory`.
 
         Parameters
         ----------
         session_id : str
@@ -104,32 +104,30 @@
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         return self.aget_memory(session_id, lastn)  # type: ignore
 
-    async def aget_memory(
-        self, session_id: str, lastn: Optional[int] = None
-    ) -> List[Memory]:
+    async def aget_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
         Asynchronously retrieve memory for the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which to retrieve memory.
         lastn : Optional[int], optional
             The number of most recent memory entries to retrieve. Defaults to None (all
             entries).
 
         Returns
         -------
-        List[Memory]
-            A list of Memory objects representing the retrieved memory entries.
+        Memory
+            A Memory object representing the retrieved memory entries.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id == "":
@@ -165,15 +163,15 @@
         memory = Memory(
             messages=messages,
             # Add the 'summary' field if it is present in the response.
             summary=summary,
             # Add any other fields from the response that are relevant to the
             # Memory class.
         )
-        return [memory]
+        return memory
 
     @sync
     def add_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Add memory to the specified session. This method is a synchronous wrapper for
         the asynchronous method `aadd_memory`.
```

