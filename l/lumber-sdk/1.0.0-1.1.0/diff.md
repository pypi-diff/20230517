# Comparing `tmp/lumber-sdk-1.0.0.tar.gz` & `tmp/lumber-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumber-sdk-1.0.0.tar", last modified: Fri Mar  3 14:28:44 2023, max compression
+gzip compressed data, was "lumber-sdk-1.1.0.tar", last modified: Wed May 17 06:56:27 2023, max compression
```

## Comparing `lumber-sdk-1.0.0.tar` & `lumber-sdk-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.251622 lumber-sdk-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.251622 lumber-sdk-1.0.0/src/lumber/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/src/lumber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/src/lumber/base/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/src/lumber/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/src/lumber/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/src/lumber/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/src/lumber/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/src/lumber/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/src/lumber/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/src/lumber/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/src/lumber/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-03 14:28:34.000000 lumber-sdk-1.0.0/src/lumber/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 14:28:44.255622 lumber-sdk-1.0.0/src/lumber_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-03 14:28:44.000000 lumber-sdk-1.0.0/src/lumber_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-03 14:28:44.000000 lumber-sdk-1.0.0/src/lumber_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 14:28:44.000000 lumber-sdk-1.0.0/src/lumber_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-03 14:28:44.000000 lumber-sdk-1.0.0/src/lumber_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 14:28:44.000000 lumber-sdk-1.0.0/src/lumber_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.062659 lumber-sdk-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/src/lumber/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/src/lumber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/src/lumber/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/src/lumber/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/src/lumber/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/src/lumber/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/src/lumber/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/src/lumber/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/src/lumber/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/src/lumber/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/src/lumber/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 06:56:18.000000 lumber-sdk-1.1.0/src/lumber/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:56:27.066659 lumber-sdk-1.1.0/src/lumber_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-17 06:56:27.000000 lumber-sdk-1.1.0/src/lumber_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-17 06:56:27.000000 lumber-sdk-1.1.0/src/lumber_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:56:27.000000 lumber-sdk-1.1.0/src/lumber_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 06:56:27.000000 lumber-sdk-1.1.0/src/lumber_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 06:56:27.000000 lumber-sdk-1.1.0/src/lumber_sdk.egg-info/top_level.txt
```

### Comparing `lumber-sdk-1.0.0/LICENSE` & `lumber-sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lumber-sdk-1.0.0/PKG-INFO` & `lumber-sdk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumber-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: An open-source Python SDK for connecting to the LumberHub platform
 Home-page: https://github.com/hivecv/lumber-sdk
 Author: HiveCV
 Author-email: lukasz@hivecv.com
 Keywords: data aggregation device configuration open source development kit
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lumber-sdk-1.0.0/setup.py` & `lumber-sdk-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `lumber-sdk-1.0.0/src/lumber/config/__init__.py` & `lumber-sdk-1.1.0/src/lumber/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-import json
-
 from lumber.base import HubEntity
 from jsonschema import validate, ValidationError
 
 
 class DeviceConfig(HubEntity):
     _schema = ""
     _config = None
 
     def __init__(self, schema):
         self._schema = schema
 
     def __iter__(self):
         yield 'config_schema', self._schema
 
+    def is_matching(self, other):
+        if isinstance(other, dict):
+            return 'config_schema' in other and self._schema == other['config_schema']
+        return False
+
     def should_update(self, api_data):
-        if 'config' not in api_data:
+        if not super().should_update(api_data) or 'config' not in api_data:
             return False
         return self._config != api_data['config']
 
     def on_update(self, api_data):
-        self._config = json.loads(api_data['config']) if api_data['config'] else {}
+        super().on_update(api_data)
+        self._config = api_data['config']
 
     def get_validation_schema(self):
         return {
             "type": "object",
             "properties": {
                 field_name: {"type": field_type}
-                for field_name, field_type in json.loads(self._schema).items()
+                for field_name, field_type in self._schema.items()
             },
         }
 
     def is_valid(self, strict=True):
         if not self._schema or not self._config:
             return False
         try:
```

### Comparing `lumber-sdk-1.0.0/src/lumber/hub/__init__.py` & `lumber-sdk-1.1.0/src/lumber/hub/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if api_data is None:
             api_data = self.fetch_api()
         if self._item.should_update(api_data):
             self._item.on_update(api_data)
 
     @staticmethod
     def _watcher_thread(instance):
-        while instance._watcherRunning:
+        while getattr(instance, "_watcherRunning", False):
             try:
                 instance.update()
             except:
                 pass
             time.sleep(5)
 
     def watch(self):
@@ -49,22 +49,23 @@
     def unwatch(self):
         self._watcherRunning = False
         self._watcher.join()
 
 
 class Routes:
     def __init__(self, api_url, device_uuid):
-        self.token = urljoin(api_url, "token/")
+        self.login = urljoin(api_url, "login/")
         self.users = urljoin(api_url, "users/")
-        self.devices = urljoin(api_url, "devices/")
         self.me = urljoin(api_url, "users/me/")
-        self.me_devices = urljoin(api_url, "users/me/devices/")
-        self.me_device = lambda device_id: urljoin(api_url, f"users/me/devices/{device_id}/")
-        self.device_heartbeat = urljoin(api_url, f"users/me/devices/{device_uuid}/heartbeat/")
-        self.device_logs = urljoin(api_url, f"users/me/devices/{device_uuid}/logs/")
+        self.devices = urljoin(api_url, "devices/")
+        self.device = urljoin(api_url, f"devices/{device_uuid}/")
+        self.device_heartbeat = urljoin(api_url, f"devices/{device_uuid}/heartbeat/")
+        self.device_logs = urljoin(api_url, f"devices/{device_uuid}/logs/")
+        self.device_configs = urljoin(api_url, f"devices/{device_uuid}/configs/")
+        self.device_config = lambda config_id: urljoin(api_url, f"devices/{device_uuid}/configs/{config_id}/")
 
 
 class LumberHubClient:
     api_url = None
     auth = None
 
     _heartbeat = None
@@ -73,50 +74,48 @@
     _watched = []
 
     def __init__(self, credentials, api_url=settings.get('api_url'), device_uuid=settings.get('device_uuid')):
         self.api_url = api_url
         self.device_uuid = device_uuid
 
         try:
-            self._init_response = requests.options(self.api_url)
-        except ConnectionError:
-            raise ValueError("Provided API url - {} - is incorrect (not served by uvicorn). Possible network error!".format(self.api_url))
+            self.routes = Routes(self.api_url, self.device_uuid)
 
-        self.routes = Routes(self.api_url, self.device_uuid)
+            self._login_response = requests.post(self.routes.login, json=credentials)
+            self._login_response.raise_for_status()
+            self.auth = self._login_response.json()
 
-        self._token_response = requests.post(self.routes.token, json=credentials)
-        self._token_response.raise_for_status()
-        self.auth = self._token_response.json()
+            self._me_response = requests.get(self.routes.me, headers=self.auth_headers)
+            self._me_response.raise_for_status()
 
-        self._me_response = requests.get(self.routes.me, headers=self.auth_headers)
-        self._me_response.raise_for_status()
+            response = requests.post(self.routes.devices, json={"device_uuid": self.device_uuid}, headers=self.auth_headers)
+            response.raise_for_status()
+        except ConnectionError:
+            raise ValueError("Provided API url - {} - is incorrect (not served by uvicorn). Possible network error!".format(self.api_url))
 
     @property
     def auth_headers(self):
         if self.auth is None:
             return {}
         return {"Authorization": f"{self.auth['token_type'].capitalize()} {self.auth['access_token']}"}
 
     def register(self, item: HubEntity):
         item.register_client(self)
 
         if isinstance(item, DeviceConfig):
-            devices_response = requests.get(self.routes.me_devices, headers=self.auth_headers)
-            devices_response.raise_for_status()
-            for device in devices_response.json():
-                if device["device_uuid"] == self.device_uuid:
-                    item._config = device.get("config", item._config)
-                    response = requests.put(self.routes.me_device(device["id"]), json={**device, **dict(item)}, headers=self.auth_headers)
-                    response.raise_for_status()
-                    item.on_update(response.json())
-                    return WatchedItem(self.routes.me_device(device["id"]), item)
-            response = requests.post(self.routes.me_devices, json={**dict(item), "device_uuid": self.device_uuid}, headers=self.auth_headers)
+            configs_response = requests.get(self.routes.device_configs, headers=self.auth_headers)
+            configs_response.raise_for_status()
+            for config in configs_response.json():
+                if item.is_matching(config):
+                    return WatchedItem(self.routes.device_config(config["id"]), item)
+
+            response = requests.post(self.routes.device_configs, json=dict(item), headers=self.auth_headers)
             response.raise_for_status()
-            item.on_update(response.json())
-            return WatchedItem(self.routes.me_device(item.raw["id"]), item)
+            data = response.json()
+            return WatchedItem(self.routes.device_config(data["id"]), item)
 
     def _heartbeat_thread(self):
         while self._heartbeat_running:
             try:
                 requests.patch(self.routes.device_heartbeat, headers=self.auth_headers)
             except:
                 pass
```

### Comparing `lumber-sdk-1.0.0/src/lumber/tools/__init__.py` & `lumber-sdk-1.1.0/src/lumber/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumber-sdk-1.0.0/src/lumber_sdk.egg-info/PKG-INFO` & `lumber-sdk-1.1.0/src/lumber_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumber-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: An open-source Python SDK for connecting to the LumberHub platform
 Home-page: https://github.com/hivecv/lumber-sdk
 Author: HiveCV
 Author-email: lukasz@hivecv.com
 Keywords: data aggregation device configuration open source development kit
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

