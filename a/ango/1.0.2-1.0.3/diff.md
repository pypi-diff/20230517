# Comparing `tmp/ango-1.0.2.tar.gz` & `tmp/ango-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.2.tar", last modified: Wed May 17 07:04:13 2023, max compression
+gzip compressed data, was "ango-1.0.3.tar", last modified: Wed May 17 14:28:39 2023, max compression
```

## Comparing `ango-1.0.2.tar` & `ango-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.870472 ango-1.0.2/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 07:04:13.866472 ango-1.0.2/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.2/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.866472 ango-1.0.2/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.2/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.866472 ango-1.0.2/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.2/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.2/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.2/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.2/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5319 2023-04-05 12:21:08.000000 ango-1.0.2/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14441 2023-05-17 06:55:02.000000 ango-1.0.2/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.866472 ango-1.0.2/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-17 07:04:13.870472 ango-1.0.2/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-17 07:03:52.000000 ango-1.0.2/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 14:28:39.297436 ango-1.0.3/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.3/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.3/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.3/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.3/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.3/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.3/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5337 2023-05-17 13:09:55.000000 ango-1.0.3/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14425 2023-05-17 14:28:05.000000 ango-1.0.3/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-17 14:28:39.297436 ango-1.0.3/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-17 12:30:01.000000 ango-1.0.3/setup.py
```

### Comparing `ango-1.0.2/PKG-INFO` & `ango-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.2/README.md` & `ango-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.2/ango/models/label_category.py` & `ango-1.0.3/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.2/ango/plugin_logger.py` & `ango-1.0.3/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.2/ango/plugins.py` & `ango-1.0.3/ango/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         logger = PluginLogger("logger", self.id, org_id, run_by, session, self)
         return logger
 
 
 class ExportPlugin(Plugin):
 
     def __init__(self, id: str, secret: str, callback: Callable[[str, dict], Tuple[str, BytesIO]],
-                 host="https://api.ango.ai"):
+                 host="https://imeritapi.ango.ai"):
         super().__init__(id, secret, callback)
         self.host = host
 
     def on_plugin(self, data):
         """
         :param data: {project_id: str, assignees: List[str] = None, completed_at: List[datetime.datetime] = None,
                updated_at: List[datetime.datetime = None, tags: List[str] = None}
@@ -95,15 +95,15 @@
             "response": upload_url.split("?")[0],
             "session": data.get("session", "")
         }
         self.emit('response', response)
 
 
 class ModelPlugin(Plugin):
-    def __init__(self, id: str, secret: str, callback: Callable, host="https://api.ango.ai"):
+    def __init__(self, id: str, secret: str, callback: Callable, host="https://imeritapi.ango.ai"):
         super().__init__(id, secret, callback)
         self.host = host
 
     def on_plugin(self, data):
         workflow = data.get('workflow')
         if not workflow:
             return super().on_plugin(data)
@@ -134,15 +134,15 @@
 
 
 class MarkdownPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
-def run(plugin, host="https://api.ango.ai"):
+def run(plugin, host="https://imeritapi.ango.ai"):
     sio = socketio.Client()
     sio.register_namespace(plugin)
     sio.connect(host, namespaces=["/plugin"], wait_timeout=100)
     try:
         asyncio.get_event_loop().run_forever()
     except (KeyboardInterrupt, SystemExit):
         logging.getLogger().warning("Plugin Stopped")
```

### Comparing `ango-1.0.2/ango/sdk.py` & `ango-1.0.3/ango/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,17 +249,17 @@
 
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
     def export(self, project_id: str, assignees: List[str] = None, completed_at: List[datetime.datetime] = None,
                updated_at: List[datetime.datetime] = None, batches: List[str] = None):
 
-        url = "%s/v2/export?project=%s&sendEmail=false&format=json&stage=Complete&" \
-              "includeMetadata=true&includeHistory=true&includeMask=false&" \
-              "includeSegmentationPoints=true&doNotNotify=true" % (self.host, project_id)
+        url = "%s/v2/export?project=%s&sendEmail=false&format=json&stage=[\"Complete\"]&" \
+              "includeMetadata=true&includeHistory=true&includeSegmentationPoints=true&doNotNotify=true"\
+              % (self.host, project_id)
         if type(assignees) == list and len(assignees) > 0:
             url += "&assignee=" + json.dumps(assignees)
         if type(batches) == list and len(batches) > 0:
             url += "&batches=" + json.dumps(batches)
         if type(completed_at) == list and len(completed_at) == 2:
             if completed_at[0] is not None:
                 url += "&completedAt[gt]=" + completed_at[0].isoformat()
```

### Comparing `ango-1.0.2/ango.egg-info/PKG-INFO` & `ango-1.0.3/ango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.2/setup.py` & `ango-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.2",
+    version="1.0.3",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

