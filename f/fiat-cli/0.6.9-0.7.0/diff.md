# Comparing `tmp/fiat_cli-0.6.9.tar.gz` & `tmp/fiat_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiat_cli-0.6.9.tar", max compression
+gzip compressed data, was "fiat_cli-0.7.0.tar", max compression
```

## Comparing `fiat_cli-0.6.9.tar` & `fiat_cli-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-04-20 03:17:26.809646 fiat_cli-0.6.9/LICENSE
--rw-r--r--   0        0        0       68 2023-04-20 03:18:44.649085 fiat_cli-0.6.9/README.md
--rw-r--r--   0        0        0        0 2023-04-23 03:34:08.157681 fiat_cli-0.6.9/fiat/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 02:49:11.357285 fiat_cli-0.6.9/fiat/apps/__init__.py
--rw-r--r--   0        0        0     1424 2023-05-12 07:36:01.033867 fiat_cli-0.6.9/fiat/apps/computing.py
--rw-r--r--   0        0        0     2318 2023-04-26 11:36:01.175418 fiat_cli-0.6.9/fiat/apps/dashboard.py
--rw-r--r--   0        0        0     1539 2023-05-16 13:40:04.322373 fiat_cli-0.6.9/fiat/apps/devs.py
--rw-r--r--   0        0        0     8844 2023-05-14 16:35:57.522232 fiat_cli-0.6.9/fiat/apps/envd.py
--rw-r--r--   0        0        0     5498 2023-04-26 15:24:52.709454 fiat_cli-0.6.9/fiat/apps/job.py
--rw-r--r--   0        0        0     6874 2023-05-16 16:41:30.292389 fiat_cli-0.6.9/fiat/apps/juicefs.py
--rw-r--r--   0        0        0     1458 2023-04-26 11:36:01.179870 fiat_cli-0.6.9/fiat/apps/metastore.py
--rw-r--r--   0        0        0     3261 2023-05-16 16:00:27.653216 fiat_cli-0.6.9/fiat/apps/server.py
--rw-r--r--   0        0        0     2012 2023-05-13 07:54:30.206971 fiat_cli-0.6.9/fiat/apps/templates.py
--rw-r--r--   0        0        0     4267 2023-05-16 15:53:27.211098 fiat_cli-0.6.9/fiat/apps/utils.py
--rw-r--r--   0        0        0      734 2023-05-16 12:23:10.412806 fiat_cli-0.6.9/fiat/main.py
--rw-r--r--   0        0        0      625 2023-05-16 16:41:49.695152 fiat_cli-0.6.9/pyproject.toml
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 fiat_cli-0.6.9/setup.py
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 fiat_cli-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-20 03:17:26.809646 fiat_cli-0.7.0/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-20 03:18:44.649085 fiat_cli-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 03:34:08.157681 fiat_cli-0.7.0/fiat/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 02:49:11.357285 fiat_cli-0.7.0/fiat/apps/__init__.py
+-rw-r--r--   0        0        0     1424 2023-05-12 07:36:01.033867 fiat_cli-0.7.0/fiat/apps/computing.py
+-rw-r--r--   0        0        0     2318 2023-04-26 11:36:01.175418 fiat_cli-0.7.0/fiat/apps/dashboard.py
+-rw-r--r--   0        0        0     1539 2023-05-16 13:40:04.322373 fiat_cli-0.7.0/fiat/apps/devs.py
+-rw-r--r--   0        0        0     8844 2023-05-14 16:35:57.522232 fiat_cli-0.7.0/fiat/apps/envd.py
+-rw-r--r--   0        0        0     5511 2023-05-16 17:15:05.298699 fiat_cli-0.7.0/fiat/apps/job.py
+-rw-r--r--   0        0        0     6874 2023-05-16 16:41:30.292389 fiat_cli-0.7.0/fiat/apps/juicefs.py
+-rw-r--r--   0        0        0     1458 2023-04-26 11:36:01.179870 fiat_cli-0.7.0/fiat/apps/metastore.py
+-rw-r--r--   0        0        0     3261 2023-05-16 16:00:27.653216 fiat_cli-0.7.0/fiat/apps/server.py
+-rw-r--r--   0        0        0     2012 2023-05-13 07:54:30.206971 fiat_cli-0.7.0/fiat/apps/templates.py
+-rw-r--r--   0        0        0     4580 2023-05-16 17:15:05.306893 fiat_cli-0.7.0/fiat/apps/utils.py
+-rw-r--r--   0        0        0      734 2023-05-16 12:23:10.412806 fiat_cli-0.7.0/fiat/main.py
+-rw-r--r--   0        0        0      625 2023-05-17 12:33:49.456103 fiat_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 fiat_cli-0.7.0/setup.py
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 fiat_cli-0.7.0/PKG-INFO
```

### Comparing `fiat_cli-0.6.9/LICENSE` & `fiat_cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/computing.py` & `fiat_cli-0.7.0/fiat/apps/computing.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/dashboard.py` & `fiat_cli-0.7.0/fiat/apps/dashboard.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/devs.py` & `fiat_cli-0.7.0/fiat/apps/devs.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/envd.py` & `fiat_cli-0.7.0/fiat/apps/envd.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/job.py` & `fiat_cli-0.7.0/fiat/apps/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 def submit_ray_job(
         cluster: str = Option(
             ...,
             "--cluster", "-c",
             help="Target Fiat Computing cluster URL", prompt="Please enter cluster URL"
         ),
         description_file: str = Option(
-            ..., "--file", "-f",
+            ...,
+            "--file", "-f",
             help="Descrption file of your project, please make sure it is available", prompt=True,
         ),
         timeout: int = Option(
             10, "--timeout", "-t", help="Timeout to submit the job before forcely abortion."
         )
 ):
     """
@@ -130,15 +131,15 @@
             ...,
             "--id",
             help="Target job id. Leave None to list all job details of the target cluster",
             prompt="Please enter the job id"
         ),
 ):
     """
-    🖨️ Job Logging
+    🖨️  Job Logging
     """
     print(":tangerine: Fetching job logs.")
     try:
         client: JobSubmissionClient = JobSubmissionClient(f"http://{cluster}")
         ret = client.get_job_logs(job_id)
         print(ret)
     except RuntimeError:
```

### Comparing `fiat_cli-0.6.9/fiat/apps/juicefs.py` & `fiat_cli-0.7.0/fiat/apps/juicefs.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/metastore.py` & `fiat_cli-0.7.0/fiat/apps/metastore.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/server.py` & `fiat_cli-0.7.0/fiat/apps/server.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/templates.py` & `fiat_cli-0.7.0/fiat/apps/templates.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/fiat/apps/utils.py` & `fiat_cli-0.7.0/fiat/apps/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 import json
 import logging
 import os
 import subprocess
 from pathlib import Path
 
 import click
-from click import Abort
+from typer import Abort
 from rich import print
 from rich.logging import RichHandler
 
 import docker
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 home_path = Path(os.environ['HOME'])
 app_conf_dir = home_path / ".fiat"
 docker_scripts_path = app_conf_dir / "docker"
 current_path = os.getcwd()
 
 
+def get_user_config() -> dict:
+    try:
+        with open(f"{current_path}/fiat.json", "r+") as file_obj:
+            conf = json.load(file_obj)
+
+        logging.debug(f"User configuration loaded: {conf}")
+    except FileNotFoundError:
+        logging.error("Please make sure you have the config file 'fiat.json' on your current folder.")
+        raise Abort()
+
+    return conf
+
+
 def get_logger():
-    with open(f"{current_path}/fiat.json", "r+") as file_obj:
-        conf = json.load(file_obj)
+    conf = get_user_config()
+
     if "log_level" in conf.keys():
         log_level = conf['log_level']
     else:
         log_level = "INFO"
 
     logging.basicConfig(
         level=log_level,
```

### Comparing `fiat_cli-0.6.9/fiat/main.py` & `fiat_cli-0.7.0/fiat/main.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.9/pyproject.toml` & `fiat_cli-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fiat-cli"
-version = "0.6.9"
+version = "0.7.0"
 license = "MIT"
 description = "🤩 - Fiat CLI Component"
 authors = ["Jiacheng Li <cheng2029@foxmail.com>"]
 readme = "README.md"
 packages = [{include = "fiat"}]
 
 [tool.poetry.scripts]
```

### Comparing `fiat_cli-0.6.9/setup.py` & `fiat_cli-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['fiat = fiat.main:app']}
 
 setup_kwargs = {
     'name': 'fiat-cli',
-    'version': '0.6.9',
+    'version': '0.7.0',
     'description': '🤩 - Fiat CLI Component',
     'long_description': '# Fiat CLI\n\n#### Description\n\n🛸 - The awesome Fiat CLI component!',
     'author': 'Jiacheng Li',
     'author_email': 'cheng2029@foxmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fiat_cli-0.6.9/PKG-INFO` & `fiat_cli-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiat-cli
-Version: 0.6.9
+Version: 0.7.0
 Summary: 🤩 - Fiat CLI Component
 License: MIT
 Author: Jiacheng Li
 Author-email: cheng2029@foxmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

