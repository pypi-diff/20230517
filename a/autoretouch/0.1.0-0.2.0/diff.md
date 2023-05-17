# Comparing `tmp/autoretouch-0.1.0.tar.gz` & `tmp/autoretouch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autoretouch-0.1.0.tar", last modified: Fri May  5 08:29:13 2023, max compression
+gzip compressed data, was "autoretouch-0.2.0.tar", last modified: Wed May 17 09:17:01 2023, max compression
```

## Comparing `autoretouch-0.1.0.tar` & `autoretouch-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/
--rw-r--r--   0 antoine    (501) staff       (20)      644 2022-01-19 09:45:07.000000 autoretouch-0.1.0/LICENSE
--rw-r--r--   0 antoine    (501) staff       (20)     5205 2023-05-05 08:29:13.000000 autoretouch-0.1.0/PKG-INFO
--rw-r--r--   0 antoine    (501) staff       (20)     4859 2023-05-05 08:12:06.000000 autoretouch-0.1.0/README.md
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch/
--rw-r--r--   0 antoine    (501) staff       (20)      695 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/.autoretouch-complete.fish
--rw-r--r--   0 antoine    (501) staff       (20)     1002 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/.autoretouch-complete.zsh
--rw-r--r--   0 antoine    (501) staff       (20)        0 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/__init__.py
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch/api_client/
--rw-r--r--   0 antoine    (501) staff       (20)        0 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/api_client/__init__.py
--rw-r--r--   0 antoine    (501) staff       (20)     4889 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/api_client/authenticator.py
--rw-r--r--   0 antoine    (501) staff       (20)    25678 2023-05-05 08:12:06.000000 autoretouch-0.1.0/autoretouch/api_client/client.py
--rw-r--r--   0 antoine    (501) staff       (20)     2615 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/api_client/model.py
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch/cli/
--rw-r--r--   0 antoine    (501) staff       (20)        0 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/cli/__init__.py
--rw-r--r--   0 antoine    (501) staff       (20)     8530 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/cli/commands.py
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/
--rw-r--r--   0 antoine    (501) staff       (20)     5205 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/PKG-INFO
--rw-r--r--   0 antoine    (501) staff       (20)      597 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/SOURCES.txt
--rw-r--r--   0 antoine    (501) staff       (20)        1 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/dependency_links.txt
--rw-r--r--   0 antoine    (501) staff       (20)       73 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/entry_points.txt
--rw-r--r--   0 antoine    (501) staff       (20)       39 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/requires.txt
--rw-r--r--   0 antoine    (501) staff       (20)       12 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/top_level.txt
--rw-r--r--   0 antoine    (501) staff       (20)       85 2022-05-23 07:09:43.000000 autoretouch-0.1.0/pyproject.toml
--rw-r--r--   0 antoine    (501) staff       (20)       38 2023-05-05 08:29:13.000000 autoretouch-0.1.0/setup.cfg
--rw-r--r--   0 antoine    (501) staff       (20)     3695 2023-05-05 08:12:06.000000 autoretouch-0.1.0/setup.py
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/test/
--rw-r--r--   0 antoine    (501) staff       (20)     3073 2023-05-05 08:12:06.000000 autoretouch-0.1.0/test/test_authenticator.py
--rw-r--r--   0 antoine    (501) staff       (20)    11658 2023-05-05 08:12:06.000000 autoretouch-0.1.0/test/test_client.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-17 09:17:01.744394 autoretouch-0.2.0/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)      644 2021-10-06 09:14:54.000000 autoretouch-0.2.0/LICENSE
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     5205 2023-05-17 09:17:01.744144 autoretouch-0.2.0/PKG-INFO
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     4859 2023-03-21 14:15:18.000000 autoretouch-0.2.0/README.md
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-17 09:17:01.738767 autoretouch-0.2.0/autoretouch/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)      695 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/.autoretouch-complete.fish
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     1002 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/.autoretouch-complete.zsh
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/__init__.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-17 09:17:01.742003 autoretouch-0.2.0/autoretouch/api_client/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/api_client/__init__.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     4889 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/api_client/authenticator.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)    25776 2023-05-17 08:43:20.000000 autoretouch-0.2.0/autoretouch/api_client/client.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     2615 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/api_client/model.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-17 09:17:01.742684 autoretouch-0.2.0/autoretouch/cli/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        0 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/cli/__init__.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     8530 2022-07-29 09:51:42.000000 autoretouch-0.2.0/autoretouch/cli/commands.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-17 09:17:01.740619 autoretouch-0.2.0/autoretouch.egg-info/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     5205 2023-05-17 09:17:01.000000 autoretouch-0.2.0/autoretouch.egg-info/PKG-INFO
+-rw-r--r--   0 tlorentzen   (501) staff       (20)      597 2023-05-17 09:17:01.000000 autoretouch-0.2.0/autoretouch.egg-info/SOURCES.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)        1 2023-05-17 09:17:01.000000 autoretouch-0.2.0/autoretouch.egg-info/dependency_links.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       73 2023-05-17 09:17:01.000000 autoretouch-0.2.0/autoretouch.egg-info/entry_points.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       39 2023-05-17 09:17:01.000000 autoretouch-0.2.0/autoretouch.egg-info/requires.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       12 2023-05-17 09:17:01.000000 autoretouch-0.2.0/autoretouch.egg-info/top_level.txt
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       85 2022-07-29 09:51:42.000000 autoretouch-0.2.0/pyproject.toml
+-rw-r--r--   0 tlorentzen   (501) staff       (20)       38 2023-05-17 09:17:01.744465 autoretouch-0.2.0/setup.cfg
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     3695 2023-05-17 08:43:20.000000 autoretouch-0.2.0/setup.py
+drwxr-xr-x   0 tlorentzen   (501) staff       (20)        0 2023-05-17 09:17:01.743767 autoretouch-0.2.0/test/
+-rw-r--r--   0 tlorentzen   (501) staff       (20)     3073 2023-05-16 15:12:01.000000 autoretouch-0.2.0/test/test_authenticator.py
+-rw-r--r--   0 tlorentzen   (501) staff       (20)    11415 2023-05-17 08:43:20.000000 autoretouch-0.2.0/test/test_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autoretouch-0.1.0/LICENSE` & `autoretouch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/PKG-INFO` & `autoretouch-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoretouch
-Version: 0.1.0
+Version: 0.2.0
 Summary: cli and python package to communicate with the autoRetouch API
 Author: ['Antoine Daurat <antoine@autoretouch.com>', 'Oliver Allweyer <oliver@autoretouch.com>', 'Till Lorentzen <till@autoretouch.com>']
 License: BSD Zero
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # autoRetouch client
```

### Comparing `autoretouch-0.1.0/README.md` & `autoretouch-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/autoretouch/.autoretouch-complete.fish` & `autoretouch-0.2.0/autoretouch/.autoretouch-complete.fish`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/autoretouch/.autoretouch-complete.zsh` & `autoretouch-0.2.0/autoretouch/.autoretouch-complete.zsh`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/autoretouch/api_client/authenticator.py` & `autoretouch-0.2.0/autoretouch/api_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/autoretouch/api_client/client.py` & `autoretouch-0.2.0/autoretouch/api_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,15 @@
             self,
             workflow_id: UUID,
             image_content_hash: str,
             image_name: str,
             labels: Optional[Dict[str, str]] = None,
             workflow_version_id: Optional[UUID] = None,
             organization_id: Optional[UUID] = None,
+            settings: Optional[dict] = None,
     ) -> UUID:
         logger.info("creating workflow execution for image reference...")
         self.authenticated()
         organization_id = self._get_organization_id(organization_id)
         version_str = f"&version={workflow_version_id}" if workflow_version_id else ""
         url = (
             f"{self.api_config.BASE_API_URL_CURRENT}/workflow/execution/create"
@@ -376,14 +377,15 @@
         payload = {
             "image": {
                 "name": image_name,
                 "contentHash": image_content_hash,
                 "contentType": mimetype,
             },
             **({"labels": labels} if labels else {}),
+            "settings": settings if settings else {}
         }
 
         response = requests.post(url=url, headers=headers, data=json.dumps(payload))
         logger.debug(f"{url} answered with status {response.status_code}")
         response.raise_for_status()
         return UUID(response.content.decode(response.encoding))
```

### Comparing `autoretouch-0.1.0/autoretouch/api_client/model.py` & `autoretouch-0.2.0/autoretouch/api_client/model.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/autoretouch/cli/commands.py` & `autoretouch-0.2.0/autoretouch/cli/commands.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/autoretouch.egg-info/PKG-INFO` & `autoretouch-0.2.0/autoretouch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoretouch
-Version: 0.1.0
+Version: 0.2.0
 Summary: cli and python package to communicate with the autoRetouch API
 Author: ['Antoine Daurat <antoine@autoretouch.com>', 'Oliver Allweyer <oliver@autoretouch.com>', 'Till Lorentzen <till@autoretouch.com>']
 License: BSD Zero
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # autoRetouch client
```

### Comparing `autoretouch-0.1.0/autoretouch.egg-info/SOURCES.txt` & `autoretouch-0.2.0/autoretouch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/setup.py` & `autoretouch-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 with open("README.md", "r") as f:
     README = f.read()
 
 setup(
     name="autoretouch",
-    version="0.1.0",
+    version="0.2.0",
     author=[
         "Antoine Daurat <antoine@autoretouch.com>",
         "Oliver Allweyer <oliver@autoretouch.com>",
         "Till Lorentzen <till@autoretouch.com>"
     ],
     description="cli and python package to communicate with the autoRetouch API",
     long_description=README,
```

### Comparing `autoretouch-0.1.0/test/test_authenticator.py` & `autoretouch-0.2.0/test/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.1.0/test/test_client.py` & `autoretouch-0.2.0/test/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import time
 from typing import Tuple, Dict
 from unittest import TestCase
 from uuid import UUID
 from assertpy import assert_that
 
-from autoretouch.api_client.client import (
-    AutoRetouchAPIClient,
-)
+from autoretouch.api_client.client import AutoRetouchAPIClient
 from autoretouch.api_client.model import Organization, Workflow, WorkflowExecution
 from test.api_config_dev import CONFIG_DEV
 
 CREDENTIALS_PATH = "../tmp/credentials.json"
 USER_AGENT = "Python-Unit-Test-0.1.0"
 
 
@@ -43,15 +41,16 @@
         workflow_execution_id = (
             self.client.create_workflow_execution_for_image_reference(
                 workflow_id=workflow.id,
                 image_content_hash=input_image_content_hash,
                 image_name="input_image.jpeg",
                 labels={"myLabel": "myValue"},
                 workflow_version_id=workflow.version,
-                organization_id=organization.id)
+                organization_id=organization.id,
+                settings={"input": {"some": "settings"}})
         )
         self.assertIsNotNone(workflow_execution_id)
 
         self.__assert_execution_has_started(
             organization,
             workflow,
             workflow_execution_id,
@@ -77,18 +76,19 @@
             organization, workflow_execution_completed
         )
 
     def test_upload_image_from_memory(self):
         organization, _ = self.__get_organization_and_workflow()
         with open("../assets/input_image.jpeg", "rb") as file:
             file_content = file.read()
-        input_image_content_hash = self.client.upload_image_from_bytes(image_content=file_content,
-                                                                       image_name="input_image.jpeg",
-                                                                       mimetype="image/jpeg",
-                                                                       organization_id=organization.id)
+        input_image_content_hash = self.client.upload_image_from_bytes(
+            image_content=file_content,
+            image_name="input_image.jpeg",
+            mimetype="image/jpeg",
+            organization_id=organization.id)
         self.assertIsNotNone(input_image_content_hash)
         self.assertEqual(
             input_image_content_hash,
             "8bcac2125bd98cd96ba75667b9a8832024970ac05bf4123f864bb63bcfefbcf7",
         )
 
     def test_upload_image_from_disk(self):
@@ -110,18 +110,20 @@
             result_image_content_hashes.get("input_image.jpeg"),
             "8bcac2125bd98cd96ba75667b9a8832024970ac05bf4123f864bb63bcfefbcf7",
         )
 
     def test_start_workflow_execution_immediately_and_wait(self):
         organization, workflow = self.__get_organization_and_workflow()
 
-        workflow_execution_id = self.client.create_workflow_execution_for_image_file(workflow.id,
-                                                                                     "../assets/input_image.jpeg",
-                                                                                     {"myLabel": "myValue"},
-                                                                                     workflow.version, organization.id)
+        workflow_execution_id = self.client.create_workflow_execution_for_image_file(
+            workflow_id=workflow.id,
+            image_path="../assets/input_image.jpeg",
+            labels={"myLabel": "myValue"},
+            workflow_version_id=workflow.version,
+            organization_id=organization.id)
         self.assertIsNotNone(workflow_execution_id)
 
         input_image_content_hash = (
             "8bcac2125bd98cd96ba75667b9a8832024970ac05bf4123f864bb63bcfefbcf7"
         )
         self.__assert_execution_has_started(
             organization,
```

