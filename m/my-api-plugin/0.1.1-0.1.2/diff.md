# Comparing `tmp/my-api-plugin-0.1.1.tar.gz` & `tmp/my-api-plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-api-plugin-0.1.1.tar", last modified: Wed May 17 00:55:51 2023, max compression
+gzip compressed data, was "my-api-plugin-0.1.2.tar", last modified: Wed May 17 01:57:59 2023, max compression
```

## Comparing `my-api-plugin-0.1.1.tar` & `my-api-plugin-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 00:55:51.600656 my-api-plugin-0.1.1/
--rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-17 00:55:51.600462 my-api-plugin-0.1.1/PKG-INFO
--rw-r--r--   0 wangchan   (501) staff       (20)        0 2023-05-16 08:39:47.000000 my-api-plugin-0.1.1/README.md
-drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 00:55:51.598766 my-api-plugin-0.1.1/my_api_plugin/
--rw-r--r--   0 wangchan   (501) staff       (20)       33 2023-05-16 09:27:54.000000 my-api-plugin-0.1.1/my_api_plugin/__init__.py
--rw-r--r--   0 wangchan   (501) staff       (20)     1613 2023-05-16 09:27:56.000000 my-api-plugin-0.1.1/my_api_plugin/api_client.py
-drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 00:55:51.600185 my-api-plugin-0.1.1/my_api_plugin.egg-info/
--rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/PKG-INFO
--rw-r--r--   0 wangchan   (501) staff       (20)      256 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 wangchan   (501) staff       (20)        1 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 wangchan   (501) staff       (20)        9 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/requires.txt
--rw-r--r--   0 wangchan   (501) staff       (20)       14 2023-05-17 00:55:51.000000 my-api-plugin-0.1.1/my_api_plugin.egg-info/top_level.txt
--rw-r--r--   0 wangchan   (501) staff       (20)       38 2023-05-17 00:55:51.600736 my-api-plugin-0.1.1/setup.cfg
--rw-r--r--   0 wangchan   (501) staff       (20)      347 2023-05-17 00:55:42.000000 my-api-plugin-0.1.1/setup.py
+drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 01:57:59.593958 my-api-plugin-0.1.2/
+-rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-17 01:57:59.593775 my-api-plugin-0.1.2/PKG-INFO
+-rw-r--r--   0 wangchan   (501) staff       (20)        0 2023-05-16 08:39:47.000000 my-api-plugin-0.1.2/README.md
+drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 01:57:59.591972 my-api-plugin-0.1.2/my_api_plugin/
+-rw-r--r--   0 wangchan   (501) staff       (20)       25 2023-05-17 01:57:05.000000 my-api-plugin-0.1.2/my_api_plugin/__init__.py
+-rw-r--r--   0 wangchan   (501) staff       (20)     1567 2023-05-17 01:57:24.000000 my-api-plugin-0.1.2/my_api_plugin/api_client.py
+drwxr-xr-x   0 wangchan   (501) staff       (20)        0 2023-05-17 01:57:59.593480 my-api-plugin-0.1.2/my_api_plugin.egg-info/
+-rw-r--r--   0 wangchan   (501) staff       (20)      262 2023-05-17 01:57:59.000000 my-api-plugin-0.1.2/my_api_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 wangchan   (501) staff       (20)      256 2023-05-17 01:57:59.000000 my-api-plugin-0.1.2/my_api_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)        1 2023-05-17 01:57:59.000000 my-api-plugin-0.1.2/my_api_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)        9 2023-05-17 01:57:59.000000 my-api-plugin-0.1.2/my_api_plugin.egg-info/requires.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)       14 2023-05-17 01:57:59.000000 my-api-plugin-0.1.2/my_api_plugin.egg-info/top_level.txt
+-rw-r--r--   0 wangchan   (501) staff       (20)       38 2023-05-17 01:57:59.594012 my-api-plugin-0.1.2/setup.cfg
+-rw-r--r--   0 wangchan   (501) staff       (20)      347 2023-05-17 01:57:34.000000 my-api-plugin-0.1.2/setup.py
```

### Comparing `my-api-plugin-0.1.1/my_api_plugin/api_client.py` & `my-api-plugin-0.1.2/my_api_plugin/api_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 import time
 import json
 import hashlib
 import random
 import requests
 
-class APIClient:
-    def __init__(self, base_url):
-        self.base_url = base_url
-
-    def post(self, endpoint, data):
-        url = f"{self.base_url}/{endpoint}"
-        response = requests.post(url, json=data)
-        return response.json()
+# class APIClient:
+#     def __init__(self, base_url):
+#         self.base_url = base_url
+
+#     def post(self, endpoint, data):
+#         url = f"{self.base_url}/{endpoint}"
+#         response = requests.post(url, json=data)
+#         return response.json()
 
     # 签名对象
-# getSha256 = lambda content: hashlib.sha256(content.encode("utf-8")).hexdigest()
+getSha256 = lambda content: hashlib.sha256(content.encode("utf-8")).hexdigest()
 
-# # 密钥信息获取与帮助文档：https://www.aigcaas.cn/article/16.html
+# 密钥信息获取与帮助文档：https://www.aigcaas.cn/article/16.html
 
-# secret_id = 'MzVScjKLAQohekq'  # 密钥信息
-# secret_key = 'uoYhZTJfnNAawbw'  # 密钥信息
-# application_name = 'modi'  # 应用名称
-# api_name = 'modi'  # 接口名称
-
-# # 请求地址
-# url = "https://api.aigcaas.cn/product/%s/api/%s" % (application_name, api_name)
-# # 构建请求头
-# nonce = str(random.randint(1, 10000))
-# timestamp = str(int(time.time()))
-# token = getSha256(("%s%s%s" % (timestamp, secret_key, nonce)))
-# headers = {
-#     'SecretID': secret_id,
-#     'Nonce': nonce,
-#     'Token': token,
-#     'Timestamp': timestamp,
-#     'Content-Type': 'application/json'
-# }
-# # 构建请求 body
-# data = {
-#     "text": "a cute baby",
-#     "width": 512,
-#     "height": 512,
-#     "negative_prompt":"human",
-#     "num_inference_steps":40
-# }
-
-# # 获取响应
-# response = requests.request("POST", url, headers=headers, data=json.dumps(data))
-# print(response.text)
+secret_id = 'MzVScjKLAQohekq'  # 密钥信息
+secret_key = 'uoYhZTJfnNAawbw'  # 密钥信息
+application_name = 'modi'  # 应用名称
+api_name = 'modi'  # 接口名称
+
+# 请求地址
+url = "https://api.aigcaas.cn/product/%s/api/%s" % (application_name, api_name)
+# 构建请求头
+nonce = str(random.randint(1, 10000))
+timestamp = str(int(time.time()))
+token = getSha256(("%s%s%s" % (timestamp, secret_key, nonce)))
+headers = {
+    'SecretID': secret_id,
+    'Nonce': nonce,
+    'Token': token,
+    'Timestamp': timestamp,
+    'Content-Type': 'application/json'
+}
+# 构建请求 body
+data = {
+    "text": "a cute baby",
+    "width": 512,
+    "height": 512,
+    "negative_prompt":"human",
+    "num_inference_steps":40
+}
+
+# 获取响应
+response = requests.request("POST", url, headers=headers, data=json.dumps(data))
+print(response.text)
 
 # 如果是流式响应，可以参考下面的代码
 # response = requests.post(url, headers=headers, data=json.dumps(data), stream=True)
 # for chunk in response.iter_content():
 #      if chunk:
 #          print(chunk)
```

