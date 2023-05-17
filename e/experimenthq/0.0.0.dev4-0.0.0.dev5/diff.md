# Comparing `tmp/experimenthq-0.0.0.dev4.tar.gz` & `tmp/experimenthq-0.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimenthq-0.0.0.dev4.tar", last modified: Wed May 17 00:15:12 2023, max compression
+gzip compressed data, was "experimenthq-0.0.0.dev5.tar", last modified: Wed May 17 01:07:09 2023, max compression
```

## Comparing `experimenthq-0.0.0.dev4.tar` & `experimenthq-0.0.0.dev5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.937007 experimenthq-0.0.0.dev4/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.0.0.dev4/LICENSE
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 00:15:12.937173 experimenthq-0.0.0.dev4/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2383 2023-05-14 20:21:42.000000 experimenthq-0.0.0.dev4/README.md
--rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-17 00:15:12.937657 experimenthq-0.0.0.dev4/setup.cfg
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3265 2023-05-17 00:15:07.000000 experimenthq-0.0.0.dev4/setup.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.933200 experimenthq-0.0.0.dev4/src/
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.934887 experimenthq-0.0.0.dev4/src/experimenthq/
--rw-r--r--   0 ramonabendias   (501) staff       (20)      148 2023-05-14 19:40:55.000000 experimenthq-0.0.0.dev4/src/experimenthq/__init__.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)      129 2023-05-17 00:14:26.000000 experimenthq-0.0.0.dev4/src/experimenthq/_about.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2832 2023-05-17 00:13:36.000000 experimenthq-0.0.0.dev4/src/experimenthq/experiment.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.936358 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)      386 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/SOURCES.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/dependency_links.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/not-zip-safe
--rw-r--r--   0 ramonabendias   (501) staff       (20)      126 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/requires.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/top_level.txt
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.936660 experimenthq-0.0.0.dev4/tests/
--rw-r--r--   0 ramonabendias   (501) staff       (20)       36 2023-05-15 17:54:05.000000 experimenthq-0.0.0.dev4/tests/test_experiment.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.298314 experimenthq-0.0.0.dev5/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.0.0.dev5/LICENSE
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 01:07:09.298408 experimenthq-0.0.0.dev5/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2383 2023-05-14 20:21:42.000000 experimenthq-0.0.0.dev5/README.md
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-17 01:07:09.298770 experimenthq-0.0.0.dev5/setup.cfg
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3265 2023-05-17 00:15:07.000000 experimenthq-0.0.0.dev5/setup.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.294641 experimenthq-0.0.0.dev5/src/
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.296589 experimenthq-0.0.0.dev5/src/experimenthq/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      148 2023-05-14 19:40:55.000000 experimenthq-0.0.0.dev5/src/experimenthq/__init__.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      129 2023-05-17 01:06:58.000000 experimenthq-0.0.0.dev5/src/experimenthq/_about.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2857 2023-05-17 01:06:47.000000 experimenthq-0.0.0.dev5/src/experimenthq/experiment.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.297857 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      386 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/SOURCES.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/dependency_links.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/not-zip-safe
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      126 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/requires.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/top_level.txt
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.298014 experimenthq-0.0.0.dev5/tests/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)       36 2023-05-15 17:54:05.000000 experimenthq-0.0.0.dev5/tests/test_experiment.py
```

### Comparing `experimenthq-0.0.0.dev4/LICENSE` & `experimenthq-0.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev4/PKG-INFO` & `experimenthq-0.0.0.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev4
+Version: 0.0.0.dev5
 Summary: A Python package for tracking experiments in Notion
 Author: 
 Author-email: 
 License: MIT
 Project-URL: Website, https://www.experiment-hq.com/
 Keywords: notion,tracking,ml,machine learning,experiment,experimentation,experiment tracking,python,sync
 Classifier: Programming Language :: Python :: 3
```

### Comparing `experimenthq-0.0.0.dev4/README.md` & `experimenthq-0.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev4/setup.cfg` & `experimenthq-0.0.0.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev4/setup.py` & `experimenthq-0.0.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev4/src/experimenthq/experiment.py` & `experimenthq-0.0.0.dev5/src/experimenthq/experiment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import json
-from typing import List, Optional
-
 import requests
+from typing import List, Optional
 
 API_URL = "https://www.api.experiment-hq.com/"
 
 
 class Experiment:
     """
     Experiment class for logging parameters to Notion.
@@ -27,62 +25,57 @@
         tags: Optional[List[str]] = None,
     ):
         self.project = project
         self.api_key = api_key
         self.name = name
         self.description = description
         self.tags = tags
+        self.session = requests.Session()
         self.experiment_id = self._start_experiment()
 
     def _start_experiment(self) -> str:
         post_data = {
             "project": self.project,
             "name": self.name,
             "description": self.description,
             "tags": self.tags,
         }
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}",
         }
-        response = requests.post(
-            url=f"{API_URL}experiment", data=json.dumps(post_data), headers=headers
+        response = self.session.post(
+            f"{API_URL}experiment",
+            json=post_data,
+            headers=headers,
         )
-
-        # Raise exception if maximum number of experiments reached
         if response.status_code == 401:
             raise Exception("Invalid API key")
-
-        # Raise exception if maximum number of experiments reached
         elif response.status_code == 403:
             raise Exception("Maximum number of experiments reached")
-
         elif response.status_code == 404:
             raise Exception("ExperimentHQ database not found")
-
         elif response.status_code != 200:
             raise Exception("Failed to start experiment with message: " + response.text)
-
-        response_json = response.json()
-        return response_json.get("experiment_id")
+        return response.json().get("experiment_id")
 
     def log_parameter(self, name: str, value: str) -> None:
         data = {"parameter_name": name, "parameter_value": value}
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}",
         }
-
-        response = requests.post(
-            url=f"{API_URL}experiments/{self.experiment_id}/parameters",
-            data=json.dumps(data),
+        response = self.session.post(
+            f"{API_URL}experiments/{self.experiment_id}/parameters",
+            json=data,
             headers=headers,
         )
-
         if response.status_code == 401:
             raise Exception("Invalid API key")
-
         elif response.status_code == 404:
             raise Exception("ExperimentHQ database not found")
-
+        elif response.status_code == 400:
+            raise Exception(
+                "Invalid parameter value or name. We currently only support text columns."
+            )
         elif response.status_code != 200:
             raise Exception("Failed to log parameter with message: " + response.text)
```

### Comparing `experimenthq-0.0.0.dev4/src/experimenthq.egg-info/PKG-INFO` & `experimenthq-0.0.0.dev5/src/experimenthq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev4
+Version: 0.0.0.dev5
 Summary: A Python package for tracking experiments in Notion
 Author: 
 Author-email: 
 License: MIT
 Project-URL: Website, https://www.experiment-hq.com/
 Keywords: notion,tracking,ml,machine learning,experiment,experimentation,experiment tracking,python,sync
 Classifier: Programming Language :: Python :: 3
```

