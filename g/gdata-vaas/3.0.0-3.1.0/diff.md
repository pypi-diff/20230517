# Comparing `tmp/gdata-vaas-3.0.0.tar.gz` & `tmp/gdata-vaas-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata-vaas-3.0.0.tar", last modified: Tue May  9 14:19:12 2023, max compression
+gzip compressed data, was "gdata-vaas-3.1.0.tar", last modified: Wed May 17 13:08:20 2023, max compression
```

## Comparing `gdata-vaas-3.0.0.tar` & `gdata-vaas-3.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.779696 gdata-vaas-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-09 14:19:12.000000 gdata-vaas-3.0.0/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10389 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:19:12.783696 gdata-vaas-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8305 2023-05-09 14:18:27.000000 gdata-vaas-3.0.0/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.760342 gdata-vaas-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11198 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8305 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/tests/test_vaas.py
```

### Comparing `gdata-vaas-3.0.0/LICENSE` & `gdata-vaas-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.0.0/PKG-INFO` & `gdata-vaas-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.0.0
+Version: 3.1.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.0.0/README.md` & `gdata-vaas-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.0.0/setup.cfg` & `gdata-vaas-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 3.0.0
+version = 3.1.0
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls =
```

### Comparing `gdata-vaas-3.0.0/src/gdata_vaas.egg-info/PKG-INFO` & `gdata-vaas-3.1.0/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.0.0
+Version: 3.1.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.0.0/src/vaas/__init__.py` & `gdata-vaas-3.1.0/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.0.0/src/vaas/client_credentials_grant_authenticator.py` & `gdata-vaas-3.1.0/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.0.0/src/vaas/vaas.py` & `gdata-vaas-3.1.0/src/vaas/vaas.py`

 * *Files 20% similar despite different names*

```diff
@@ -151,34 +151,40 @@
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, traceback):
         await self.close()
 
-    async def for_sha256(self, sha256):
+    async def for_sha256(self, sha256, verdict_request_attributes=None):
         """Returns the verdict for a SHA256 checksum"""
-        verdict_response = await self.__for_sha256(sha256)
+        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes)
         return {
             "Sha256": verdict_response.get("sha256"),
             "Guid": verdict_response.get("guid"),
             "Verdict": verdict_response.get("verdict"),
         }
 
-    async def __for_sha256(self, sha256):
+    async def __for_sha256(self, sha256, verdict_request_attributes=None):
+        if verdict_request_attributes is not None and not isinstance(
+            verdict_request_attributes, dict
+        ):
+            raise TypeError("verdict_request_attributes has to be dict(str, str)")
+
         websocket = self.get_authenticated_websocket()
         start = time.time()
         guid = str(uuid.uuid4())
         verdict_request = {
             "kind": "VerdictRequest",
             "sha256": sha256,
             "session_id": self.session_id,
             "guid": guid,
             "use_shed": self.options.use_shed,
             "use_cache": self.options.use_cache,
+            "verdict_request_attributes": verdict_request_attributes,
         }
         response_message = self.__response_message_for_guid(guid)
         await websocket.send(json.dumps(verdict_request))
 
         try:
             result = await asyncio.wait_for(response_message, timeout=TIMEOUT)
         except asyncio.TimeoutError as ex:
@@ -202,23 +208,23 @@
                     guid = vaas_message.get("guid")
                     future = self.results.get(guid)
                     if future is not None:
                         future.set_result(vaas_message)
         except Exception as error:
             raise VaasConnectionClosedError(error) from error
 
-    async def for_buffer(self, buffer):
+    async def for_buffer(self, buffer, verdict_request_attributes=None):
         """Returns the verdict for a buffer"""
 
         loop = asyncio.get_running_loop()
         sha256 = await loop.run_in_executor(
             None, lambda: hashlib.sha256(buffer).hexdigest()
         )
 
-        verdict_response = await self.__for_sha256(sha256)
+        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes)
         verdict = verdict_response.get("verdict")
 
         if verdict == "Unknown":
             verdict_response = await self._for_unknown_buffer(
                 verdict_response, buffer, len(buffer)
             )
 
@@ -239,21 +245,21 @@
             verdict_response = await asyncio.wait_for(response_message, timeout=TIMEOUT)
         except asyncio.TimeoutError as ex:
             self.tracing.trace_upload_result_timeout(buffer_len)
             raise VaasTimeoutError() from ex
         self.tracing.trace_upload_request(time.time() - start, buffer_len)
         return verdict_response
 
-    async def for_file(self, path):
+    async def for_file(self, path, verdict_request_attributes=None):
         """Returns the verdict for a file"""
 
         loop = asyncio.get_running_loop()
         sha256 = await loop.run_in_executor(None, lambda: hash_file(path))
 
-        verdict_response = await self.__for_sha256(sha256)
+        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes)
         verdict = verdict_response.get("verdict")
 
         if verdict == "Unknown":
             async with aiofiles.open(path, mode="rb") as file:
                 buffer = await file.read()
                 verdict_response = await self._for_unknown_buffer(
                     verdict_response, buffer, len(buffer)
@@ -280,26 +286,32 @@
                 },
                 timeout=UPLOAD_TIMEOUT,
             )
         except httpx.TimeoutException as ex:
             self.tracing.trace_upload_timeout(content_length)
             raise VaasTimeoutError() from ex
 
-    async def for_url(self, url):
+    async def for_url(self, url, verdict_request_attributes=None):
         """Returns the verdict for a file from an url"""
+        if verdict_request_attributes is not None and not isinstance(
+            verdict_request_attributes, dict
+        ):
+            raise TypeError("verdict_request_attributes has to be dict(str, str)")
+
         websocket = self.get_authenticated_websocket()
         start = time.time()
         guid = str(uuid.uuid4())
         verdict_request_for_url = {
             "kind": "VerdictRequestForUrl",
             "url": url,
             "session_id": self.session_id,
             "guid": guid,
             "use_shed": self.options.use_shed,
             "use_cache": self.options.use_cache,
+            "verdict_request_attributes": verdict_request_attributes,
         }
         response_message = self.__response_message_for_guid(guid)
         await websocket.send(json.dumps(verdict_request_for_url))
 
         try:
             result = await asyncio.wait_for(response_message, timeout=TIMEOUT)
         except asyncio.TimeoutError as ex:
```

### Comparing `gdata-vaas-3.0.0/tests/test_client_credentials_grant_authenticator.py` & `gdata-vaas-3.1.0/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.0.0/tests/test_vaas.py` & `gdata-vaas-3.1.0/tests/test_vaas.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     async def test_connects(self):
         async with await create_and_connect():
             pass
 
     async def test_for_sha256_returns_clean_for_clean_sha256(self):
         async with await create_and_connect() as vaas:
             verdict = await vaas.for_sha256(
-                "698CDA840A0B3D4639F0C5DBD5C629A847A27448A9A179CB6B7A648BC1186F23"
+                "3A78F382E8E2968EC201B33178102E06DB72E4F2D1505E058A4613C1E977825C"
             )
             self.assertEqual(verdict["Verdict"], "Clean")
             self.assertEqual(
                 verdict["Sha256"].casefold(),
-                "698CDA840A0B3D4639F0C5DBD5C629A847A27448A9A179CB6B7A648BC1186F23".casefold(),
+                "3A78F382E8E2968EC201B33178102E06DB72E4F2D1505E058A4613C1E977825C".casefold(),
             )
 
     async def test_use_for_sha256_when_connection_already_closed(self):
         authenticator = ClientCredentialsGrantAuthenticator(
             CLIENT_ID, CLIENT_SECRET, TOKEN_URL, SSL_VERIFICATION
         )
         vaas = Vaas(tracing=VaasTracing(), options=VaasOptions(), url=VAAS_URL)
```

