# Comparing `tmp/carefree-client-0.1.8.tar.gz` & `tmp/carefree-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-client-0.1.8.tar", last modified: Thu Mar  9 01:05:08 2023, max compression
+gzip compressed data, was "carefree-client-0.1.9.tar", last modified: Thu Mar  9 12:52:52 2023, max compression
```

## Comparing `carefree-client-0.1.8.tar` & `carefree-client-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 01:05:08.069931 carefree-client-0.1.8/
--rw-rw-rw-   0        0        0     1290 2023-03-09 01:05:08.067963 carefree-client-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1037 2023-03-08 14:51:16.000000 carefree-client-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 01:05:08.047616 carefree-client-0.1.8/carefree_client.egg-info/
--rw-rw-rw-   0        0        0     1290 2023-03-09 01:05:07.000000 carefree-client-0.1.8/carefree_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-03-09 01:05:07.000000 carefree-client-0.1.8/carefree_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 01:05:07.000000 carefree-client-0.1.8/carefree_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2023-03-09 01:05:07.000000 carefree-client-0.1.8/carefree_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-09 01:05:07.000000 carefree-client-0.1.8/carefree_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 01:05:08.055111 carefree-client-0.1.8/cfclient/
--rw-rw-rw-   0        0        0        0 2023-03-08 14:51:16.000000 carefree-client-0.1.8/cfclient/__init__.py
--rw-rw-rw-   0        0        0    17202 2023-03-08 14:51:16.000000 carefree-client-0.1.8/cfclient/core.py
-drwxrwxrwx   0        0        0        0 2023-03-09 01:05:08.065944 carefree-client-0.1.8/cfclient/models/
--rw-rw-rw-   0        0        0       42 2023-03-08 14:51:16.000000 carefree-client-0.1.8/cfclient/models/__init__.py
--rw-rw-rw-   0        0        0       25 2023-03-08 14:51:16.000000 carefree-client-0.1.8/cfclient/models/constants.py
--rw-rw-rw-   0        0        0     7956 2023-03-08 14:51:16.000000 carefree-client-0.1.8/cfclient/models/core.py
--rw-rw-rw-   0        0        0      738 2023-03-08 14:51:16.000000 carefree-client-0.1.8/cfclient/models/demo.py
--rw-rw-rw-   0        0        0     5772 2023-03-08 14:59:59.000000 carefree-client-0.1.8/cfclient/utils.py
--rw-rw-rw-   0        0        0       42 2023-03-09 01:05:08.069931 carefree-client-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-03-09 00:59:09.000000 carefree-client-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-09 12:52:52.622279 carefree-client-0.1.9/
+-rw-rw-rw-   0        0        0     1290 2023-03-09 12:52:52.621282 carefree-client-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1037 2022-11-03 11:43:08.000000 carefree-client-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-09 12:52:52.618296 carefree-client-0.1.9/carefree_client.egg-info/
+-rw-rw-rw-   0        0        0     1290 2023-03-09 12:52:52.000000 carefree-client-0.1.9/carefree_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-03-09 12:52:52.000000 carefree-client-0.1.9/carefree_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-09 12:52:52.000000 carefree-client-0.1.9/carefree_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2023-03-09 12:52:52.000000 carefree-client-0.1.9/carefree_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-09 12:52:52.000000 carefree-client-0.1.9/carefree_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-09 12:52:52.619289 carefree-client-0.1.9/cfclient/
+-rw-rw-rw-   0        0        0        0 2022-11-03 11:43:08.000000 carefree-client-0.1.9/cfclient/__init__.py
+-rw-rw-rw-   0        0        0    17202 2022-11-03 11:43:08.000000 carefree-client-0.1.9/cfclient/core.py
+drwxrwxrwx   0        0        0        0 2023-03-09 12:52:52.621282 carefree-client-0.1.9/cfclient/models/
+-rw-rw-rw-   0        0        0       42 2022-11-03 11:43:08.000000 carefree-client-0.1.9/cfclient/models/__init__.py
+-rw-rw-rw-   0        0        0       25 2022-11-03 11:43:08.000000 carefree-client-0.1.9/cfclient/models/constants.py
+-rw-rw-rw-   0        0        0     7956 2022-11-03 11:43:08.000000 carefree-client-0.1.9/cfclient/models/core.py
+-rw-rw-rw-   0        0        0      738 2022-11-03 11:43:08.000000 carefree-client-0.1.9/cfclient/models/demo.py
+-rw-rw-rw-   0        0        0     5784 2023-03-09 12:48:17.000000 carefree-client-0.1.9/cfclient/utils.py
+-rw-rw-rw-   0        0        0       42 2023-03-09 12:52:52.622279 carefree-client-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-03-09 12:52:26.000000 carefree-client-0.1.9/setup.py
```

### Comparing `carefree-client-0.1.8/PKG-INFO` & `carefree-client-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Client framework based on FastAPI
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 
 `carefree-client` is a client framework based on `FastAPI`. It also supports interacting with Triton Inference Server.
```

### Comparing `carefree-client-0.1.8/README.md` & `carefree-client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `carefree-client-0.1.8/carefree_client.egg-info/PKG-INFO` & `carefree-client-0.1.9/carefree_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Client framework based on FastAPI
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 
 `carefree-client` is a client framework based on `FastAPI`. It also supports interacting with Triton Inference Server.
```

### Comparing `carefree-client-0.1.8/cfclient/core.py` & `carefree-client-0.1.9/cfclient/core.py`

 * *Files identical despite different names*

### Comparing `carefree-client-0.1.8/cfclient/models/core.py` & `carefree-client-0.1.9/cfclient/models/core.py`

 * *Files identical despite different names*

### Comparing `carefree-client-0.1.8/cfclient/models/demo.py` & `carefree-client-0.1.9/cfclient/models/demo.py`

 * *Files identical despite different names*

### Comparing `carefree-client-0.1.8/cfclient/utils.py` & `carefree-client-0.1.9/cfclient/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     except Exception:
         return requests.get(url).content
 
 
 async def _download_image(session: ClientSession, url: str) -> Image.Image:
     raw_data = None
     try:
-        raw_data = await _download(url, session)
+        raw_data = await _download(session, url)
         return Image.open(BytesIO(raw_data))
     except Exception as err:
         if raw_data is None:
             msg = f"raw | None | err | {err}"
         else:
             try:
                 msg = raw_data.decode("utf-8")
@@ -165,25 +165,25 @@
 async def download_with_retry(
     session: ClientSession,
     url: str,
     *,
     retry: int = 3,
     interval: int = 1,
 ) -> bytes:
-    return _download_with_retry(_download, session, url, retry, interval)
+    return await _download_with_retry(_download, session, url, retry, interval)
 
 
 async def download_image_with_retry(
     session: ClientSession,
     url: str,
     *,
     retry: int = 3,
     interval: int = 1,
 ) -> Image.Image:
-    return _download_with_retry(_download_image, session, url, retry, interval)
+    return await _download_with_retry(_download_image, session, url, retry, interval)
 
 
 def distances2scores(distances: List[float]) -> List[float]:
     distances_arr = np.array(distances, np.float32)
     if len(distances_arr) == 1:
         scores_arr = np.array([1.0], np.float32)
     else:
```

### Comparing `carefree-client-0.1.8/setup.py` & `carefree-client-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 DESCRIPTION = "Client framework based on FastAPI"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="carefree-client",
     version=VERSION,
```

