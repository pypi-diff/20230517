# Comparing `tmp/miquido_spawn_gitlab_job-1.0.3.tar.gz` & `tmp/miquido_spawn_gitlab_job-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miquido_spawn_gitlab_job-1.0.3.tar", last modified: Tue May 16 11:55:47 2023, max compression
+gzip compressed data, was "miquido_spawn_gitlab_job-1.0.4.tar", last modified: Wed May 17 13:42:34 2023, max compression
```

## Comparing `miquido_spawn_gitlab_job-1.0.3.tar` & `miquido_spawn_gitlab_job-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 11:55:47.565332 miquido_spawn_gitlab_job-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-16 11:55:47.565332 miquido_spawn_gitlab_job-1.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 11:55:47.565332 miquido_spawn_gitlab_job-1.0.3/gitlab_env_spawner/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-16 11:55:01.981228 miquido_spawn_gitlab_job-1.0.3/gitlab_env_spawner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-16 11:55:01.981228 miquido_spawn_gitlab_job-1.0.3/gitlab_env_spawner/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-05-16 11:55:01.981228 miquido_spawn_gitlab_job-1.0.3/gitlab_env_spawner/spawner.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-16 11:55:47.253304 miquido_spawn_gitlab_job-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:42:34.362109 miquido_spawn_gitlab_job-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-17 13:42:34.362109 miquido_spawn_gitlab_job-1.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:42:34.362109 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-17 13:42:20.761028 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-17 13:42:20.761028 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2023-05-17 13:42:20.761028 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/spawner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-17 13:42:34.214097 miquido_spawn_gitlab_job-1.0.4/setup.py
```

### Comparing `miquido_spawn_gitlab_job-1.0.3/PKG-INFO` & `miquido_spawn_gitlab_job-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: miquido_spawn_gitlab_job
-Version: 1.0.3
+Version: 1.0.4
 Summary: Launches dynamic environment on AWS ECS
 Home-page: UNKNOWN
 Author: Marek
 Author-email: marek.moscichowski@miquido.com
 License: MIT
 Description: UNKNOWN
 Keywords: GITLAB
```

### Comparing `miquido_spawn_gitlab_job-1.0.3/gitlab_env_spawner/spawner.py` & `miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/spawner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import json
 import os
 from functools import reduce
 
 import boto3
 
 
+def __map_container_files(s):
+    with open(s[1], 'r') as f:
+        return f.read()
+
+
 def spawn():
     lb = boto3.client('lambda')
+    additional_containers = list(filter(lambda x: x[0][0:11] == 'DD_SERVICE_', os.environ.items()))
+    additional_containers = list(map(__map_container_files, additional_containers))
+
     environment_variables = list(filter(lambda x: x[0][0:3] == 'DD_', os.environ.items()))
     environment_variables = list(map(lambda x: (x[0][3:], x[1]), environment_variables))
     environment_variables = reduce(lambda res, x: {**res, **{x[0]: x[1]}}, environment_variables, {})
 
     function_name = os.getenv('SPAWNER_FUNCTION_NAME', 'prod-dynamic-containers-lambda-terraform')
     name = f"{os.getenv('CI_PROJECT_NAME')}-{os.getenv('CI_COMMIT_REF_SLUG')}"
     image = os.getenv('CI_REGISTRY_IMAGE')
@@ -19,14 +27,14 @@
     gitlab_password = os.getenv('CI_DEPLOY_PASSWORD')
     payload = {
         'name': name,
         'image': image,
         'tag': tag,
         'gitlab_user': gitlab_user,
         'gitlab_password': gitlab_password,
-        'service_envs': environment_variables
+        'service_envs': environment_variables,
+        'additional_containers': additional_containers
     }
 
     res = lb.invoke(FunctionName=function_name,
                     Payload=bytes(json.dumps(payload), 'utf-8'))
     print(res)
-
```

### Comparing `miquido_spawn_gitlab_job-1.0.3/setup.py` & `miquido_spawn_gitlab_job-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='miquido_spawn_gitlab_job',  # How you named your package folder (MyLib)
     packages=['gitlab_env_spawner'],  # Chose the same as "name"
-    version='1.0.3',
+    version='1.0.4',
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Launches dynamic environment on AWS ECS',
     # Give a short description about your library
     author='Marek',  # Type in your name
     author_email='marek.moscichowski@miquido.com',  # Type in your E-Mail
     keywords=['GITLAB'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
```

