# Comparing `tmp/quorum_mininode_py-1.2.7.tar.gz` & `tmp/quorum_mininode_py-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_mininode_py-1.2.7.tar", last modified: Tue May 16 12:57:39 2023, max compression
+gzip compressed data, was "quorum_mininode_py-1.2.8.tar", last modified: Wed May 17 03:54:15 2023, max compression
```

## Comparing `quorum_mininode_py-1.2.7.tar` & `quorum_mininode_py-1.2.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.862223 quorum_mininode_py-1.2.7/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.7/LICENSE
--rw-rw-rw-   0        0        0     2440 2023-05-16 12:57:39.861226 quorum_mininode_py-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.819362 quorum_mininode_py-1.2.7/quorum_mininode_py/
--rw-rw-rw-   0        0        0      364 2023-05-16 12:47:34.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.835295 quorum_mininode_py-1.2.7/quorum_mininode_py/api/
--rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/api/__init__.py
--rw-rw-rw-   0        0        0     2281 2023-05-16 12:50:30.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/api/base.py
--rw-rw-rw-   0        0        0     3812 2023-05-03 11:14:28.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/api/lightnode.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.840283 quorum_mininode_py-1.2.7/quorum_mininode_py/client/
--rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/client/__init__.py
--rw-rw-rw-   0        0        0     2667 2023-05-16 12:50:32.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/client/_http.py
--rw-rw-rw-   0        0        0     2625 2023-05-16 12:50:30.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/client/mininode.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.850254 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/
--rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/__init__.py
--rw-rw-rw-   0        0        0     2361 2023-05-03 11:14:57.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/account.py
--rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/aes.py
--rw-rw-rw-   0        0        0     1824 2023-05-03 11:15:00.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/age.py
--rw-rw-rw-   0        0        0     3846 2023-05-03 11:36:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/trx.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.854246 quorum_mininode_py-1.2.7/quorum_mininode_py/proto/
--rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/proto/__init__.py
--rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/proto/quorum_pb2.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.858234 quorum_mininode_py-1.2.7/quorum_mininode_py/utils/
--rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/utils/__init__.py
--rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/utils/url.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.829311 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/
--rw-rw-rw-   0        0        0     2440 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 12:57:39.862223 quorum_mininode_py-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-05-16 12:47:34.000000 quorum_mininode_py-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.661516 quorum_mininode_py-1.2.8/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0     2440 2023-05-17 03:54:15.660517 quorum_mininode_py-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.575490 quorum_mininode_py-1.2.8/quorum_mininode_py/
+-rw-rw-rw-   0        0        0      364 2023-05-17 03:51:15.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.632392 quorum_mininode_py-1.2.8/quorum_mininode_py/api/
+-rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     2281 2023-05-16 12:50:30.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/api/base.py
+-rw-rw-rw-   0        0        0     3812 2023-05-03 11:14:28.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/api/lightnode.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.637909 quorum_mininode_py-1.2.8/quorum_mininode_py/client/
+-rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     2827 2023-05-17 03:50:47.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/client/_http.py
+-rw-rw-rw-   0        0        0     2636 2023-05-17 03:49:00.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/client/mininode.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.649690 quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/
+-rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2361 2023-05-03 11:14:57.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/account.py
+-rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/aes.py
+-rw-rw-rw-   0        0        0     1824 2023-05-03 11:15:00.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/age.py
+-rw-rw-rw-   0        0        0     3846 2023-05-03 11:36:39.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/trx.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.653683 quorum_mininode_py-1.2.8/quorum_mininode_py/proto/
+-rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/proto/__init__.py
+-rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/proto/quorum_pb2.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.657696 quorum_mininode_py-1.2.8/quorum_mininode_py/utils/
+-rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/utils/__init__.py
+-rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.8/quorum_mininode_py/utils/url.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:54:15.625243 quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/
+-rw-rw-rw-   0        0        0     2440 2023-05-17 03:54:15.000000 quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-05-17 03:54:15.000000 quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 03:54:15.000000 quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-17 03:54:15.000000 quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-17 03:54:15.000000 quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 03:54:15.661516 quorum_mininode_py-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1308 2023-05-17 03:51:15.000000 quorum_mininode_py-1.2.8/setup.py
```

### Comparing `quorum_mininode_py-1.2.7/LICENSE` & `quorum_mininode_py-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/PKG-INFO` & `quorum_mininode_py-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_mininode_py
-Version: 1.2.7
+Version: 1.2.8
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.7/README.md` & `quorum_mininode_py-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/api/base.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/api/base.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/api/lightnode.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/api/lightnode.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/client/_http.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/client/_http.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,27 @@
 
 
 class HttpRequest:
     """Class for making http requests"""
 
     def __init__(
         self,
-        chain_urls: list,
+        api_base: str = None,
+        jwt_token: str = None,
+        chain_urls: list = None,
         timeout: int = 5,
         retries: int = 3,
     ):
         """
         Initializes the HttpRequest class
         chain_urls: list of dict of api_base and jwt_token
         """
         requests.adapters.DEFAULT_RETRIES = 5
+        if api_base:
+            chain_urls = [{"baseurl": api_base, "jwt": jwt_token}]
         self.chain_urls = chain_urls
         self.current_chain_url = 0
         self.session = requests.Session()
         self.timeout = timeout
         self.retries = retries
         self.headers = {"Content-Type": "application/json"}
         self.session.headers.update(self.headers)
```

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/client/mininode.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/client/mininode.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 class MiniNode:
     """python for quorum lightnode, without datastore, one MiniNode client for one group"""
 
     def __init__(self, seed_url: str, pvtkey=None, age_pvtkey=None):
         self.group = RumGroup(seed_url)
-        self.http = HttpRequest(self.group.chain_urls or [])
+        self.http = HttpRequest(chain_urls=self.group.chain_urls or [])
         self.account = RumAccount(pvtkey, age_pvtkey, self.group.encryption_type)
         self.api = LightNodeAPI(self)
 
     def change_account(self, pvtkey, age_pvtkey=None):
         age_pvtkey = age_pvtkey or self.account.age_pvtkey
         if pvtkey != self.account.pvtkey or age_pvtkey != self.account.age_pvtkey:
             self.account = RumAccount(pvtkey, age_pvtkey, self.group.encryption_type)
```

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/account.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/account.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/aes.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/age.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/age.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/trx.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/crypto/trx.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/proto/quorum_pb2.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/proto/quorum_pb2.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py/utils/url.py` & `quorum_mininode_py-1.2.8/quorum_mininode_py/utils/url.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/PKG-INFO` & `quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-mininode-py
-Version: 1.2.7
+Version: 1.2.8
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/SOURCES.txt` & `quorum_mininode_py-1.2.8/quorum_mininode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.7/setup.py` & `quorum_mininode_py-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_mininode_py",
-    version="1.2.7",
+    version="1.2.8",
     author="liujuanjuan1984, zhangwm404",
     author_email="qiaoanlu@163.com",
     description="a mini python sdk for quorum lightnode with http/https requests to quorum fullnode",
     keywords=["rumsystem", "quorum", "lightnode", "sdk"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_mininode_py",
@@ -27,10 +27,10 @@
     packages=setuptools.find_packages(exclude=["example"]),
     python_requires=">=3.5",
     install_requires=[
         "requests",
         "eth_keys",
         "pyrage",
         "protobuf",
-        "eth_account",
+        "eth_account>=0.8.0",
     ],
 )
```

