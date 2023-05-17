# Comparing `tmp/hugchat-0.0.6.tar.gz` & `tmp/hugchat-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.6.tar", last modified: Tue May 16 00:55:46 2023, max compression
+gzip compressed data, was "hugchat-0.0.6.1.tar", last modified: Wed May 17 00:32:20 2023, max compression
```

## Comparing `hugchat-0.0.6.tar` & `hugchat-0.0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.116840 hugchat-0.0.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.6/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3827 2023-05-16 00:55:46.116840 hugchat-0.0.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2809 2023-05-16 00:53:53.000000 hugchat-0.0.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-16 00:55:46.116840 hugchat-0.0.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1434 2023-05-16 00:55:39.000000 hugchat-0.0.6/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.108840 hugchat-0.0.6/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.116840 hugchat-0.0.6/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.6/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.6/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10664 2023-05-16 00:53:53.000000 hugchat-0.0.6/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.116840 hugchat-0.0.6/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3827 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.523693 hugchat-0.0.6.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.6.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3829 2023-05-17 00:32:20.519693 hugchat-0.0.6.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2809 2023-05-16 00:53:53.000000 hugchat-0.0.6.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-17 00:32:20.523693 hugchat-0.0.6.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1436 2023-05-17 00:32:09.000000 hugchat-0.0.6.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.507692 hugchat-0.0.6.1/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.515693 hugchat-0.0.6.1/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.6.1/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.6.1/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10716 2023-05-17 00:31:10.000000 hugchat-0.0.6.1/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.519693 hugchat-0.0.6.1/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3829 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.6/LICENSE` & `hugchat-0.0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.6/PKG-INFO` & `hugchat-0.0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hugchat-0.0.6/README.md` & `hugchat-0.0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.6/setup.py` & `hugchat-0.0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.6",
+    version="0.0.6.1",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.6/src/hugchat/hugchat.py` & `hugchat-0.0.6.1/src/hugchat/hugchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,20 @@
         session.get(self.hf_base_url + "/chat")
         return session
     
     def get_headers(self, ref=True) -> dict:
         _h = {
             "Accept": "*/*",
             "Connection": "keep-alive",
-
             "Host": "huggingface.co",
             "Origin": "https://huggingface.co",
             "sec-gpc": "1",
-
             "Sec-Fetch-Site": "same-origin",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Dest": "empty",
-
             "Accept-Encoding": "gzip, deflate, br",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
         }
         if ref:
             _h["Referer"] = f"https://huggingface.co/chat/conversation/{self.current_conversation}"
         return _h
     
@@ -93,16 +90,17 @@
         
         return True
     
     def new_conversation(self) -> str:
         err_count = 0
 
         # Accept the welcome modal when init.
-        if not self.accepted_welcome_modal:
-            self.accept_ethics_modal()
+        # 17/5/2023: This is not required anymore.
+        # if not self.accepted_welcome_modal:
+        #     self.accept_ethics_modal()
 
         # Create new conversation and get a conversation id.
         resp = ""
         while True:
             try:
                 resp = self.session.post(self.hf_base_url + "/chat/conversation", json={"model": self.active_model}, headers=self.json_header)
                 # print(resp.text)
```

### Comparing `hugchat-0.0.6/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.6.1/src/hugchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

