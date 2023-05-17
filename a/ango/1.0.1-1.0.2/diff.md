# Comparing `tmp/ango-1.0.1.tar.gz` & `tmp/ango-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.1.tar", last modified: Fri May 12 14:51:53 2023, max compression
+gzip compressed data, was "ango-1.0.2.tar", last modified: Wed May 17 07:04:13 2023, max compression
```

## Comparing `ango-1.0.1.tar` & `ango-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-12 14:51:53.025334 ango-1.0.1/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.1/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.1/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.1/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.1/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.1/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.1/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5319 2023-04-05 12:21:08.000000 ango-1.0.1/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    13957 2023-05-12 14:51:41.000000 ango-1.0.1/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-12 14:51:52.000000 ango-1.0.1/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-12 14:51:53.000000 ango-1.0.1/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-12 14:51:52.000000 ango-1.0.1/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-12 14:51:52.000000 ango-1.0.1/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-12 14:51:53.000000 ango-1.0.1/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-12 14:51:53.025334 ango-1.0.1/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-12 14:51:50.000000 ango-1.0.1/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.870472 ango-1.0.2/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 07:04:13.866472 ango-1.0.2/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.2/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.866472 ango-1.0.2/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.2/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.866472 ango-1.0.2/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.2/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.2/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.2/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.2/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5319 2023-04-05 12:21:08.000000 ango-1.0.2/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14441 2023-05-17 06:55:02.000000 ango-1.0.2/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 07:04:13.866472 ango-1.0.2/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-17 07:04:13.000000 ango-1.0.2/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-17 07:04:13.870472 ango-1.0.2/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-17 07:03:52.000000 ango-1.0.2/setup.py
```

### Comparing `ango-1.0.1/PKG-INFO` & `ango-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.1/README.md` & `ango-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.1/ango/models/label_category.py` & `ango-1.0.2/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.1/ango/plugin_logger.py` & `ango-1.0.2/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.1/ango/plugins.py` & `ango-1.0.2/ango/plugins.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.1/ango/sdk.py` & `ango-1.0.2/ango/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -372,15 +372,14 @@
         payload = {
             "name": name,
             "description": description,
         }
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
 
-
     def _annotate(self, task_id: str, answer: dict):
         url = "%s/v2/annotate/%s?nextStage=true" % (self.host, task_id)
         headers = {
             'apikey': self.api_key
         }
         payload = {
             "answer": answer,
@@ -397,7 +396,23 @@
         }
         payload = {
             "stages": stages
         }
 
         response = self.session.post(url, headers=headers, json=payload)
         return response.json()
+
+    def get_task_history(self, id: str = None, task_id: str = None):
+
+        url = None
+        if id:
+            url = "%s/v2/taskHistory/%s" % (self.host, id)
+        elif task_id:
+            url = "%s/v2/task/%s/history" % (self.host, task_id)
+        else:
+            raise Exception("id or task_id should be specified!")
+
+        headers = {
+            'apikey': self.api_key
+        }
+        response = self.session.get(url, headers=headers)
+        return response.json()
```

### Comparing `ango-1.0.1/ango.egg-info/PKG-INFO` & `ango-1.0.2/ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.1/setup.py` & `ango-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.1",
+    version="1.0.2",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

