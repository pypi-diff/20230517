# Comparing `tmp/pbsrollout-0.3.4.tar.gz` & `tmp/pbsrollout-0.3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.4.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.4.1.tar", max compression
```

## Comparing `pbsrollout-0.3.4.tar` & `pbsrollout-0.3.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.4/LICENSE
--rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.4/pbsrollout/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 00:14:13.401261 pbsrollout-0.3.4/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1226 2023-04-27 00:14:13.401590 pbsrollout-0.3.4/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2023-04-27 00:14:13.401821 pbsrollout-0.3.4/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3733 2023-04-27 00:14:13.402052 pbsrollout-0.3.4/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0     9181 2023-04-27 00:14:13.402305 pbsrollout-0.3.4/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2023-04-27 00:14:13.402559 pbsrollout-0.3.4/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1217 2023-04-27 00:14:13.402806 pbsrollout-0.3.4/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      444 2023-04-27 00:14:13.403016 pbsrollout-0.3.4/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      151 2023-04-27 00:14:13.403246 pbsrollout-0.3.4/pbsrollout/internal/test_utils.py
--rw-r--r--   0        0        0     1076 2023-04-27 21:20:15.861757 pbsrollout-0.3.4/pbsrollout/internal/test_utils_gh.py
--rw-r--r--   0        0        0     1155 2023-04-27 00:14:13.403703 pbsrollout-0.3.4/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     2966 2023-04-27 21:28:28.932187 pbsrollout-0.3.4/pbsrollout/internal/utils_gh.py
--rw-r--r--   0        0        0     5123 2023-04-27 21:38:27.099717 pbsrollout-0.3.4/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2023-04-27 00:14:13.404614 pbsrollout-0.3.4/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0     9374 2023-04-27 00:14:13.404945 pbsrollout-0.3.4/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2023-04-27 00:14:13.405041 pbsrollout-0.3.4/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     7259 2023-04-27 21:29:29.119174 pbsrollout-0.3.4/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      522 2023-04-27 21:38:05.695021 pbsrollout-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.4.1/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.4.1/pbsrollout/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:14:13.401261 pbsrollout-0.3.4.1/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1226 2023-04-27 00:14:13.401590 pbsrollout-0.3.4.1/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2023-04-27 00:14:13.401821 pbsrollout-0.3.4.1/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3733 2023-04-27 00:14:13.402052 pbsrollout-0.3.4.1/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0     9181 2023-05-17 14:19:10.455948 pbsrollout-0.3.4.1/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2023-04-27 00:14:13.402559 pbsrollout-0.3.4.1/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1217 2023-04-27 00:14:13.402806 pbsrollout-0.3.4.1/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      444 2023-04-27 00:14:13.403016 pbsrollout-0.3.4.1/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      151 2023-04-27 00:14:13.403246 pbsrollout-0.3.4.1/pbsrollout/internal/test_utils.py
+-rw-r--r--   0        0        0     1076 2023-04-27 21:20:15.861757 pbsrollout-0.3.4.1/pbsrollout/internal/test_utils_gh.py
+-rw-r--r--   0        0        0     1155 2023-04-27 00:14:13.403703 pbsrollout-0.3.4.1/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     2966 2023-04-27 21:28:28.932187 pbsrollout-0.3.4.1/pbsrollout/internal/utils_gh.py
+-rw-r--r--   0        0        0     5226 2023-05-17 14:27:04.413651 pbsrollout-0.3.4.1/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:14:13.404614 pbsrollout-0.3.4.1/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0     9374 2023-04-27 00:14:13.404945 pbsrollout-0.3.4.1/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:14:13.405041 pbsrollout-0.3.4.1/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     7285 2023-05-17 14:19:26.836340 pbsrollout-0.3.4.1/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      585 2023-05-17 14:19:52.346789 pbsrollout-0.3.4.1/pyproject.toml
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 pbsrollout-0.3.4.1/PKG-INFO
```

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/aws_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/test_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/test_utils_gh.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/test_utils_gh.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/utils.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/internal/utils_gh.py` & `pbsrollout-0.3.4.1/pbsrollout/internal/utils_gh.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/main.py` & `pbsrollout-0.3.4.1/pbsrollout/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,27 +50,28 @@
                 exit(0)
 
 
 def print_changelog(console: Console):
     txt = """[bold gold1]What's new?[/bold gold1]
 [bold misty_rose1]Big features (v/0.3)[/bold misty_rose1]:
 - Support for [italic]staging[/italic]! You can now release/sync/migrate staging envs!
+- staging tags now include github PR description + author
 
-[bold thistle1]Other[/bold thistle1]:
-- staging tags now includ github PR description + author
+[bold thistle1]Changelog (v[VERSION])[/bold thistle1]:
+- fix: add staging 20 to the list of available stagings 
 """
-    console.print(txt)
+    console.print(txt.replace("[VERSION]", VERSION))
 
 
 def print_welcome(console: Console):
     """
     Print the welcome message.
     Message format:
 
-                                          Better Rollout (v0.2.8)
+                                          Better Rollout (vXXX)
     """
     if VERSION != "":
         console.print(
             f"\n[blink underline italic dark_orange3]Better[/blink underline italic dark_orange3] [bold medium_purple3]Rollout[/bold medium_purple3] (v{VERSION})\n",
             justify="center")
     else:
         console.print(
```

### Comparing `pbsrollout-0.3.4/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.4.1/pbsrollout/pbs_release/main_view.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.4.1/pbsrollout/stg_release/main_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,21 @@
         console.print('GOPATH should be set in your environ! Contact a publica engineer for help')
         raise RuntimeError('GOPATH should be set in your environ! Contact a publica engineer for help')
     return os.environ['GOPATH']
 
 
 def choose_staging_idx(console: Console) -> List[str]:
     idx = str(input('What is your staging idx? 1, 2, 18. Input "all" for all staging! '))
-    possible_stagings = [str(i) for i in range(1, 20)]
+    possible_stagings = [str(i) for i in range(1, NB_STAGINGS + 1)]
     possible_stagings.append('all')
     if idx not in possible_stagings:
         console.print(f'[red]your choice must be in [/red]: {possible_stagings}')
         return choose_staging_idx(console)
     if idx == 'all':
-        return [str(i).zfill(3) for i in range(1, 20)]
+        return [str(i).zfill(3) for i in range(1, NB_STAGINGS + 1)]
     return [idx.zfill(3)]
 
 
 def launch_staging_pod(stg_idx: str, dir_path: str) -> bool:
     with Dir(dir_path):
         print(f'\tLaunching staging pods for stg: {stg_idx}')
         # run make clean deploy-new-pbs-prod
```

### Comparing `pbsrollout-0.3.4/PKG-INFO` & `pbsrollout-0.3.4.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.4
-Summary: 
+Version: 0.3.4.1
+Summary: A tool to help Publica engineer test and release the platform
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

