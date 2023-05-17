# Comparing `tmp/aitest-cli-0.2.8.tar.gz` & `tmp/aitest-cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitest-cli-0.2.8.tar", last modified: Fri Mar 10 10:53:24 2023, max compression
+gzip compressed data, was "aitest-cli-0.2.9.tar", last modified: Tue Mar 14 13:16:48 2023, max compression
```

## Comparing `aitest-cli-0.2.8.tar` & `aitest-cli-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-10 10:53:24.016185 aitest-cli-0.2.8/
--rw-r--r--   0 root         (0) staff       (20)     1062 2023-02-09 07:34:24.000000 aitest-cli-0.2.8/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     7102 2023-03-10 10:53:24.016077 aitest-cli-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     5510 2023-03-06 11:20:21.000000 aitest-cli-0.2.8/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-10 10:53:24.015603 aitest-cli-0.2.8/aitest_cli.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     7102 2023-03-10 10:53:24.000000 aitest-cli-0.2.8/aitest_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      273 2023-03-10 10:53:24.000000 aitest-cli-0.2.8/aitest_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-03-10 10:53:24.000000 aitest-cli-0.2.8/aitest_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       71 2023-03-10 10:53:24.000000 aitest-cli-0.2.8/aitest_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       66 2023-03-10 10:53:24.000000 aitest-cli-0.2.8/aitest_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       35 2023-03-10 10:53:24.000000 aitest-cli-0.2.8/aitest_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      437 2023-02-09 07:34:24.000000 aitest-cli-0.2.8/aitest_tool.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-10 10:53:24.015709 aitest-cli-0.2.8/app/
--rw-r--r--   0 root         (0) staff       (20)    13421 2023-03-10 10:36:56.000000 aitest-cli-0.2.8/app/aitest_application.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-03-10 10:53:24.016221 aitest-cli-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      948 2023-03-10 10:38:20.000000 aitest-cli-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-14 13:16:48.049338 aitest-cli-0.2.9/
+-rw-r--r--   0 root         (0) staff       (20)     7102 2023-03-14 13:16:48.049231 aitest-cli-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     5510 2023-03-10 11:10:18.000000 aitest-cli-0.2.9/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-14 13:16:48.048829 aitest-cli-0.2.9/aitest_cli.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     7102 2023-03-14 13:16:48.000000 aitest-cli-0.2.9/aitest_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      265 2023-03-14 13:16:48.000000 aitest-cli-0.2.9/aitest_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-03-14 13:16:48.000000 aitest-cli-0.2.9/aitest_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       71 2023-03-14 13:16:48.000000 aitest-cli-0.2.9/aitest_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       66 2023-03-14 13:16:48.000000 aitest-cli-0.2.9/aitest_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-03-14 13:16:48.000000 aitest-cli-0.2.9/aitest_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      437 2023-03-10 11:10:18.000000 aitest-cli-0.2.9/aitest_tool.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-14 13:16:48.048940 aitest-cli-0.2.9/app/
+-rw-r--r--   0 root         (0) staff       (20)    13688 2023-03-14 13:14:47.000000 aitest-cli-0.2.9/app/aitest_application.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-03-14 13:16:48.049372 aitest-cli-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      948 2023-03-14 13:16:06.000000 aitest-cli-0.2.9/setup.py
```

### Comparing `aitest-cli-0.2.8/PKG-INFO` & `aitest-cli-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitest-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: aitest
 Home-page: https://github.com/applied-ai-consulting/aiTest--CLI
 Author: aitest
 Author-email: vishwas@appliedaiconsulting.com
 License: MIT License
 Description: # aitest
         The  aitest  Command  Line  Interface is a unified tool to manage your aitest services.
```

### Comparing `aitest-cli-0.2.8/README.md` & `aitest-cli-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aitest-cli-0.2.8/aitest_cli.egg-info/PKG-INFO` & `aitest-cli-0.2.9/aitest_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitest-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: aitest
 Home-page: https://github.com/applied-ai-consulting/aiTest--CLI
 Author: aitest
 Author-email: vishwas@appliedaiconsulting.com
 License: MIT License
 Description: # aitest
         The  aitest  Command  Line  Interface is a unified tool to manage your aitest services.
```

### Comparing `aitest-cli-0.2.8/app/aitest_application.py` & `aitest-cli-0.2.9/app/aitest_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import click
 import os
 import requests
 import json
 from sys import *
 import base64
 from prettytable import PrettyTable
+import time
 
 
 
 # Command Group
 @click.group(name='configure')
 def configure():
     pass
@@ -165,25 +166,26 @@
         try:
             test_data=json.loads(res_body['body'])
         except:
             click.echo(res_body)
             exit(-1)
         project_id=test_data['load_test_details']['project_id']
         test_type=test_data['load_test_details']['test_type']
+        testrun_id_new = test_data['load_test_details']['testrun_id']
         if test_type == 'functional_test':
             sub_link='multi-browser-test'
         elif test_type == 'load_test':
             sub_link='performance-test'
         else:
             sub_link='url-test'
         if profile == 'dev':
             aitest_ui="https://app.aitest.dev.appliedaiconsulting.com/"
         else:
             aitest_ui="https://app.aitest.appliedaiconsulting.com/"
-        testrun_link=aitest_ui+sub_link+"?testrun_id="+testrun_id+"&project_id="+project_id
+        testrun_link=aitest_ui+sub_link+"?testrun_id="+testrun_id_new+"&project_id="+project_id
         click.echo(f"\nTestrun created successfully\nTestrun Name : {test_data['load_test_details']['testrun_name']}\nTestrun ID : {test_data['load_test_details']['testrun_id']}\n")
         click.echo(f"\nTestrun Link: {testrun_link}\n")
         if wait_time:
             click.echo("Testrun is in progress, result will be displayed once it get completed.")
             new_time = datetime.now() +timedelta(minutes=int(wait_time))
             test_status=""
             while test_status!="completed":
@@ -192,15 +194,18 @@
                     exit()
                 if profile=='dev':
                     base_url = f"https://api.aitest.dev.appliedaiconsulting.com/public/v1/testrun_result/status/{test_data['load_test_details']['testrun_id']}"
                 else:
                     base_url = f"https://api.aitest.appliedaiconsulting.com/public/v1/testrun_result/status/{test_data['load_test_details']['testrun_id']}"
                 status_res =requests.get(base_url,headers=headers)
                 status_test_data=status_res.json()
-                if status_test_data['statusCode'] == 200:
+
+                #adding a wait time so that we don't make continuous CALLS to status API.
+                time.sleep(int((wait_time*60)/10))
+                if status_test_data.get("statusCode") and status_test_data['statusCode'] == 200:
                     body=json.loads(status_test_data['body'])
                     test_status = body['testrun_status'] 
                 else:
                     test_status = ""
                 if test_status=="completed":
                     testrun_status_details=body['testrun_status_details']
                     table = PrettyTable(["browser_name", "browser_version","test run result id", "status", "time taken"])
```

### Comparing `aitest-cli-0.2.8/setup.py` & `aitest-cli-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name = 'aitest-cli',
-    version = '0.2.8',
+    version = '0.2.9',
     author = 'aitest',
     author_email = 'vishwas@appliedaiconsulting.com',
     license = 'MIT License',
     description = 'aitest',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/applied-ai-consulting/aiTest--CLI',
```

