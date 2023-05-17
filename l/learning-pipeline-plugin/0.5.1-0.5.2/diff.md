# Comparing `tmp/learning_pipeline_plugin-0.5.1.tar.gz` & `tmp/learning_pipeline_plugin-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning_pipeline_plugin-0.5.1.tar", max compression
+gzip compressed data, was "learning_pipeline_plugin-0.5.2.tar", max compression
```

## Comparing `learning_pipeline_plugin-0.5.1.tar` & `learning_pipeline_plugin-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2538 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/README.md
--rw-r--r--   0        0        0      164 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/__init__.py
--rw-r--r--   0        0        0     2242 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/actfw_utils.py
--rw-r--r--   0        0        0       90 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/__init__.py
--rw-r--r--   0        0        0     5857 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/stream_al.py
--rw-r--r--   0        0        0    10929 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_diversity.py
--rw-r--r--   0        0        0     2405 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_utils.py
--rw-r--r--   0        0        0      802 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/type_helper.py
--rw-r--r--   0        0        0     2250 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/uncertainty.py
--rw-r--r--   0        0        0     3118 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/collect_pipe.py
--rw-r--r--   0        0        0      881 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/notifier.py
--rw-r--r--   0        0        0     3986 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/select_task.py
--rw-r--r--   0        0        0     9589 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/sender_task.py
--rw-r--r--   0        0        0      707 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/README.md
+-rw-r--r--   0        0        0      164 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/__init__.py
+-rw-r--r--   0        0        0     2242 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/actfw_utils.py
+-rw-r--r--   0        0        0       90 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/__init__.py
+-rw-r--r--   0        0        0     5857 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/stream_al.py
+-rw-r--r--   0        0        0    10929 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_diversity.py
+-rw-r--r--   0        0        0     2405 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_utils.py
+-rw-r--r--   0        0        0      802 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/type_helper.py
+-rw-r--r--   0        0        0     2250 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/uncertainty.py
+-rw-r--r--   0        0        0     3118 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/collect_pipe.py
+-rw-r--r--   0        0        0      881 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/notifier.py
+-rw-r--r--   0        0        0     3986 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/select_task.py
+-rw-r--r--   0        0        0    12048 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/sender_task.py
+-rw-r--r--   0        0        0      707 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.5.2/PKG-INFO
```

### Comparing `learning_pipeline_plugin-0.5.1/README.md` & `learning_pipeline_plugin-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/actfw_utils.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/actfw_utils.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/stream_al.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/stream_al.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_diversity.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_diversity.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_utils.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_utils.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/type_helper.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/type_helper.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/uncertainty.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/uncertainty.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/collect_pipe.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/collect_pipe.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/notifier.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/notifier.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/select_task.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/select_task.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/sender_task.py` & `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/sender_task.py`

 * *Files 25% similar despite different names*

```diff
@@ -40,25 +40,30 @@
 class AbstractSenderTaskGenericDated(Generic[T], AbstractSenderTask[T]):
     ServiceClient: Type[ServiceClientProtocol] = ServiceClient
 
     def __init__(self,
                  pipeline_id: str,
                  metadata: Optional[UserMetadata] = None,
                  endpoint_root: str = "https://api.autolearner.actcast.io",
+                 connection_timeout: float = 3.0,
+                 read_timeout: float = 29.0,
                  max_retries: int = 3,
                  backoff_time_base: float = 60.0,
                  inqueuesize: int = 0):
         """Abstract isolated task used to send data to the Learning pipeline servers.
         A concrete subclass should implement the two static methods: `timestamp_from_data` and
         `bytes_from_data`.
 
         - pipeline_id (str): ID of the pipeline to send data to (obtained after created a pipeline)
         - metadata (UserMetadata): JSON-like data that will be stored with the image
                                     (e.g. user may include here some act settings)
         - endpoint_root (str): endpoint root of the lp API server (https://....)
+        - connection_timeout (float): number of connection timeout seconds. (default: 3.0)
+        - read_timeout (float): number of timeout seconds. (default: 29.0)
+          this parameter is set for connect timeout and read timeout (default: 29.0)
         - max_retries (int): Max number of retry attempts.
         - backoff_time_base (float): The delay time between retry attempts
           is defined by random(backoff_time_base * (2 ** i)) seconds.
         - inqueuesize (int): size of the sending queue (default: 0 (no limit))
 
         Use example:
         ```
@@ -69,14 +74,16 @@
         ...
         st.enqueue(my_data)
         ```
         """
         super().__init__(inqueuesize)
         self.service_client = self.ServiceClient()
         self.endpoint_root = endpoint_root
+        self.connection_timeout = connection_timeout
+        self.read_timeout = read_timeout
         self.pipeline_id = pipeline_id
         self.notifier: AbstractNotifier = NullNotifier()
         self.user_metadata = {} if metadata is None else metadata
         self.device_token = None
         self.device_token_endpoint = os.path.join(endpoint_root, "device", "token")
         self.collect_requests_endpoint = os.path.join(endpoint_root, "collect", "requests")
         assert max_retries > 0
@@ -136,19 +143,31 @@
 
         sending_context = {
             "device_id": os.environ["ACTCAST_DEVICE_ID"],
             "group_id": os.environ["ACTCAST_GROUP_ID"],
             "pipeline_id": self.pipeline_id
         }
 
-        response = requests.get(
-            self.device_token_endpoint,
-            headers=generate_headers(sending_context),
-            proxies=self.proxies_common()
-        )
+        self.device_token = None
+        try:
+            response = requests.get(
+                self.device_token_endpoint,
+                headers=generate_headers(sending_context),
+                proxies=self.proxies_common(),
+                timeout=(self.connection_timeout, self.read_timeout)
+            )
+        except requests.exceptions.ConnectTimeout:
+            self.notifier.notify(f"Connection timeout (endpoint: {self.device_token_endpoint})")
+            return
+        except requests.exceptions.ReadTimeout:
+            self.notifier.notify(f"Read timeout (endpoint: {self.device_token_endpoint})")
+            return
+        except requests.exceptions.RequestException:
+            self.notifier.notify(f"Request failure (endpoint: {self.collect_requests_endpoint})")
+            return
 
         if response.status_code == 200:
             try:
                 payload = response.json()
                 device_token = payload["data_collect_token"]
                 expires_in = payload["expires_in"]
             except (requests.exceptions.JSONDecodeError, KeyError, TypeError):
@@ -162,27 +181,39 @@
             self.device_token = None
             failure_status = {"status_code": response.status_code, "text": response.text}
             self.notifier.notify(f"Failed to update Device Token. {failure_status}")
 
     def send_image(self, data: T) -> bool:
         def get_upload_url(data: T) -> Optional[str]:
             timestamp = self.timestamp_from_data(data)
-            response = requests.post(
-                self.collect_requests_endpoint,
-                json={
-                    "timestamp": timestamp,
-                    "act_id": os.environ.get("ACTCAST_ACT_ID"),
-                    "user_data": json.dumps(self.user_metadata)
-                },
-                headers={
-                    "Content-Type": "application/json",
-                    "Authorization": "Bearer {}".format(self.device_token),
-                },
-                proxies=self.proxies_common()
-            )
+            try:
+                response = requests.post(
+                    self.collect_requests_endpoint,
+                    json={
+                        "timestamp": timestamp,
+                        "act_id": os.environ.get("ACTCAST_ACT_ID"),
+                        "user_data": json.dumps(self.user_metadata)
+                    },
+                    headers={
+                        "Content-Type": "application/json",
+                        "Authorization": "Bearer {}".format(self.device_token),
+                    },
+                    proxies=self.proxies_common(),
+                    timeout=(self.connection_timeout, self.read_timeout)
+                )
+            except requests.exceptions.ConnectTimeout:
+                self.notifier.notify(f"Connection timeout (endpoint: {self.collect_requests_endpoint})")
+                return None
+            except requests.exceptions.ReadTimeout:
+                self.notifier.notify(f"Read timeout (endpoint: {self.collect_requests_endpoint})")
+                return None
+            except requests.exceptions.RequestException:
+                self.notifier.notify(f"Request failure (endpoint: {self.collect_requests_endpoint})")
+                return None
+
             if response.status_code == 200:
                 try:
                     payload = response.json()
                     upload_url = payload["url"]
                     return upload_url
                 except (requests.exceptions.JSONDecodeError, KeyError, TypeError):
                     self.notifier.notify(f"Invalid API response. (endpoint: {self.collect_requests_endpoint})")
@@ -191,15 +222,30 @@
                 failure_status = {"status_code": response.status_code, "text": response.text}
                 self.notifier.notify(f"Failed to get an upload url. {failure_status}")
                 return None
 
         def upload_image(upload_url: str, data: T) -> bool:
             image_bytes = self.bytes_from_data(data)
 
-            response = requests.put(upload_url, data=image_bytes, proxies=self.proxies_common())
+            try:
+                response = requests.put(
+                    upload_url,
+                    data=image_bytes,
+                    proxies=self.proxies_common(),
+                    timeout=(self.connection_timeout, self.read_timeout)
+                )
+            except requests.exceptions.ConnectTimeout:
+                self.notifier.notify(f"Connection timeout (endpoint: {upload_url})")
+                return False
+            except requests.exceptions.ReadTimeout:
+                self.notifier.notify(f"Read timeout (endpoint: {upload_url})")
+                return False
+            except requests.exceptions.RequestException:
+                self.notifier.notify(f"Request failure (endpoint: {self.collect_requests_endpoint})")
+                return False
 
             if response.status_code == 200:
                 return True
             else:
                 failure_status = {"status_code": response.status_code, "text": response.text}
                 self.notifier.notify(f"Failed to upload an image to {upload_url} . {failure_status}")
                 return False
```

### Comparing `learning_pipeline_plugin-0.5.1/pyproject.toml` & `learning_pipeline_plugin-0.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "learning-pipeline-plugin"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Idein Inc."]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "learning_pipeline_plugin"}]
 repository = "https://github.com/Idein/learning-pipeline-plugin"
```

### Comparing `learning_pipeline_plugin-0.5.1/PKG-INFO` & `learning_pipeline_plugin-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning-pipeline-plugin
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Home-page: https://github.com/Idein/learning-pipeline-plugin
 License: MIT
 Author: Idein Inc.
 Requires-Python: >=3.7.0,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

