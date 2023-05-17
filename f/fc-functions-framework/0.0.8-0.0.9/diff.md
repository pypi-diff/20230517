# Comparing `tmp/fc-functions-framework-0.0.8.tar.gz` & `tmp/fc-functions-framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc-functions-framework-0.0.8.tar", last modified: Fri May  6 02:50:04 2022, max compression
+gzip compressed data, was "fc-functions-framework-0.0.9.tar", last modified: Fri May  6 03:04:06 2022, max compression
```

## Comparing `fc-functions-framework-0.0.8.tar` & `fc-functions-framework-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.682184 fc-functions-framework-0.0.8/
--rw-rw-rw-   0        0        0     1097 2022-05-06 02:50:04.682184 fc-functions-framework-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      160 2022-05-03 08:29:13.000000 fc-functions-framework-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-05-06 02:50:04.682184 fc-functions-framework-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2670 2022-05-06 02:49:59.000000 fc-functions-framework-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.600045 fc-functions-framework-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.646923 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/
--rw-rw-rw-   0        0        0     1097 2022-05-06 02:50:04.000000 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1244 2022-05-06 02:50:04.000000 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-06 02:50:04.000000 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      161 2022-05-06 02:50:04.000000 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2022-05-06 02:50:04.000000 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0      176 2022-05-06 02:50:04.000000 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-05-06 02:50:04.000000 fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.646923 fc-functions-framework-0.0.8/src/functions_framework/
--rw-rw-rw-   0        0        0    14964 2022-05-01 07:55:29.000000 fc-functions-framework-0.0.8/src/functions_framework/__init__.py
--rw-rw-rw-   0        0        0      684 2022-05-03 14:53:22.000000 fc-functions-framework-0.0.8/src/functions_framework/__main__.py
--rw-rw-rw-   0        0        0     2378 2022-05-06 02:49:59.000000 fc-functions-framework-0.0.8/src/functions_framework/_cli.py
--rw-rw-rw-   0        0        0     4446 2022-04-30 09:11:48.000000 fc-functions-framework-0.0.8/src/functions_framework/_function_registry.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.662545 fc-functions-framework-0.0.8/src/functions_framework/_http/
--rw-rw-rw-   0        0        0     1434 2022-05-01 02:54:57.000000 fc-functions-framework-0.0.8/src/functions_framework/_http/__init__.py
--rw-rw-rw-   0        0        0      913 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/functions_framework/_http/flask.py
--rw-rw-rw-   0        0        0     1233 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/functions_framework/_http/gunicorn.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.662545 fc-functions-framework-0.0.8/src/functions_framework/_of/
--rw-rw-rw-   0        0        0      371 2022-05-01 06:43:44.000000 fc-functions-framework-0.0.8/src/functions_framework/_of/__init__.py
--rw-rw-rw-   0        0        0      232 2022-05-01 02:54:57.000000 fc-functions-framework-0.0.8/src/functions_framework/_of/dapr.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.662545 fc-functions-framework-0.0.8/src/functions_framework/_of/v2/
--rw-rw-rw-   0        0        0        0 2022-05-01 03:29:26.000000 fc-functions-framework-0.0.8/src/functions_framework/_of/v2/__init__.py
--rw-rw-rw-   0        0        0     1495 2022-05-01 04:30:25.000000 fc-functions-framework-0.0.8/src/functions_framework/_of/v2/context.py
--rw-rw-rw-   0        0        0     1503 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/functions_framework/background_event.py
--rw-rw-rw-   0        0        0    14926 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/functions_framework/event_conversion.py
--rw-rw-rw-   0        0        0     1345 2022-05-01 04:43:22.000000 fc-functions-framework-0.0.8/src/functions_framework/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.662545 fc-functions-framework-0.0.8/src/google/
--rw-rw-rw-   0        0        0      770 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.662545 fc-functions-framework-0.0.8/src/google/cloud/
--rw-rw-rw-   0        0        0      770 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/cloud/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.678172 fc-functions-framework-0.0.8/src/google/cloud/functions/
--rw-rw-rw-   0        0        0      588 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/cloud/functions/__init__.py
--rw-rw-rw-   0        0        0      735 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/cloud/functions/context.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.682184 fc-functions-framework-0.0.8/src/google/cloud/functions_v1/
--rw-rw-rw-   0        0        0      588 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/cloud/functions_v1/__init__.py
--rw-rw-rw-   0        0        0     1196 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/cloud/functions_v1/context.py
-drwxrwxrwx   0        0        0        0 2022-05-06 02:50:04.682184 fc-functions-framework-0.0.8/src/google/cloud/functions_v1beta2/
--rw-rw-rw-   0        0        0      588 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/cloud/functions_v1beta2/__init__.py
--rw-rw-rw-   0        0        0     1196 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.8/src/google/cloud/functions_v1beta2/context.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.888404 fc-functions-framework-0.0.9/
+-rw-rw-rw-   0        0        0     1097 2022-05-06 03:04:06.888404 fc-functions-framework-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2022-05-03 08:29:13.000000 fc-functions-framework-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-05-06 03:04:06.888404 fc-functions-framework-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2670 2022-05-06 03:04:03.000000 fc-functions-framework-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.668713 fc-functions-framework-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.699968 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/
+-rw-rw-rw-   0        0        0     1097 2022-05-06 03:04:06.000000 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1244 2022-05-06 03:04:06.000000 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-06 03:04:06.000000 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      161 2022-05-06 03:04:06.000000 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2022-05-06 03:04:06.000000 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0      176 2022-05-06 03:04:06.000000 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2022-05-06 03:04:06.000000 fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.778550 fc-functions-framework-0.0.9/src/functions_framework/
+-rw-rw-rw-   0        0        0    14964 2022-05-01 07:55:29.000000 fc-functions-framework-0.0.9/src/functions_framework/__init__.py
+-rw-rw-rw-   0        0        0      684 2022-05-03 14:53:22.000000 fc-functions-framework-0.0.9/src/functions_framework/__main__.py
+-rw-rw-rw-   0        0        0     2368 2022-05-06 03:03:35.000000 fc-functions-framework-0.0.9/src/functions_framework/_cli.py
+-rw-rw-rw-   0        0        0     4446 2022-04-30 09:11:48.000000 fc-functions-framework-0.0.9/src/functions_framework/_function_registry.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.825422 fc-functions-framework-0.0.9/src/functions_framework/_http/
+-rw-rw-rw-   0        0        0     1434 2022-05-01 02:54:57.000000 fc-functions-framework-0.0.9/src/functions_framework/_http/__init__.py
+-rw-rw-rw-   0        0        0      913 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/functions_framework/_http/flask.py
+-rw-rw-rw-   0        0        0     1233 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/functions_framework/_http/gunicorn.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.825422 fc-functions-framework-0.0.9/src/functions_framework/_of/
+-rw-rw-rw-   0        0        0      371 2022-05-01 06:43:44.000000 fc-functions-framework-0.0.9/src/functions_framework/_of/__init__.py
+-rw-rw-rw-   0        0        0      232 2022-05-01 02:54:57.000000 fc-functions-framework-0.0.9/src/functions_framework/_of/dapr.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.841047 fc-functions-framework-0.0.9/src/functions_framework/_of/v2/
+-rw-rw-rw-   0        0        0        0 2022-05-01 03:29:26.000000 fc-functions-framework-0.0.9/src/functions_framework/_of/v2/__init__.py
+-rw-rw-rw-   0        0        0     1495 2022-05-01 04:30:25.000000 fc-functions-framework-0.0.9/src/functions_framework/_of/v2/context.py
+-rw-rw-rw-   0        0        0     1503 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/functions_framework/background_event.py
+-rw-rw-rw-   0        0        0    14926 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/functions_framework/event_conversion.py
+-rw-rw-rw-   0        0        0     1345 2022-05-01 04:43:22.000000 fc-functions-framework-0.0.9/src/functions_framework/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.841047 fc-functions-framework-0.0.9/src/google/
+-rw-rw-rw-   0        0        0      770 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.841047 fc-functions-framework-0.0.9/src/google/cloud/
+-rw-rw-rw-   0        0        0      770 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/cloud/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.856675 fc-functions-framework-0.0.9/src/google/cloud/functions/
+-rw-rw-rw-   0        0        0      588 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/cloud/functions/__init__.py
+-rw-rw-rw-   0        0        0      735 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/cloud/functions/context.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.872720 fc-functions-framework-0.0.9/src/google/cloud/functions_v1/
+-rw-rw-rw-   0        0        0      588 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/cloud/functions_v1/__init__.py
+-rw-rw-rw-   0        0        0     1196 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/cloud/functions_v1/context.py
+drwxrwxrwx   0        0        0        0 2022-05-06 03:04:06.872720 fc-functions-framework-0.0.9/src/google/cloud/functions_v1beta2/
+-rw-rw-rw-   0        0        0      588 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/cloud/functions_v1beta2/__init__.py
+-rw-rw-rw-   0        0        0     1196 2022-04-22 09:03:11.000000 fc-functions-framework-0.0.9/src/google/cloud/functions_v1beta2/context.py
```

### Comparing `fc-functions-framework-0.0.8/PKG-INFO` & `fc-functions-framework-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-functions-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open source FaaS (Function as a service) framework for writing portable Python functions
 Home-page: https://www.cucloud.cn/
 Author: Chinaunicom Cloud
 Author-email: lxfaaaa@qq.com
 License: UNKNOWN
 Description: this program fork from  google python functions-framework  .
         if you like this. find  ![here]{https://github.com/googlecloudplatform/functions-framework-python}
```

### Comparing `fc-functions-framework-0.0.8/setup.py` & `fc-functions-framework-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="fc-functions-framework",
-    version="0.0.8",
+    version="0.0.9",
     description="An open source FaaS (Function as a service) framework for writing portable Python functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.cucloud.cn/",
     author="Chinaunicom Cloud",
     author_email="lxfaaaa@qq.com",
     classifiers=[
```

### Comparing `fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/PKG-INFO` & `fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-functions-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open source FaaS (Function as a service) framework for writing portable Python functions
 Home-page: https://www.cucloud.cn/
 Author: Chinaunicom Cloud
 Author-email: lxfaaaa@qq.com
 License: UNKNOWN
 Description: this program fork from  google python functions-framework  .
         if you like this. find  ![here]{https://github.com/googlecloudplatform/functions-framework-python}
```

### Comparing `fc-functions-framework-0.0.8/src/fc_functions_framework.egg-info/SOURCES.txt` & `fc-functions-framework-0.0.9/src/fc_functions_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/__init__.py` & `fc-functions-framework-0.0.9/src/functions_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/__main__.py` & `fc-functions-framework-0.0.9/src/functions_framework/__main__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/_cli.py` & `fc-functions-framework-0.0.9/src/functions_framework/_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,23 +39,22 @@
 @click.option("--debug", envvar="DEBUG", is_flag=True)
 @click.option("--dry-run", envvar="DRY_RUN", is_flag=True)
 def _cli(target, source, signature_type, host, port, debug, dry_run):
     ff = os.getenv("FUNC_CONTEXT", "")
     if signature_type == "http" and ff == "":
         app = create_app(target, source, signature_type)
     else:
-        ctx = parse_function_context()
-        port = ctx.port
-        if ctx.runtime == KNATIVE_FUNC:
+        _ctx = parse_function_context()
+        port = _ctx.port
+        if _ctx.runtime == KNATIVE_FUNC:
             app = create_app(target, source, signature_type)
-        elif ctx.runtime == ASYNC:
-
+        elif _ctx.runtime == ASYNC:
             signature_type = "of"
             app = create_dapr_app(target, source, signature_type, ctx)
     if dry_run:
         click.echo("Function: {}".format(target))
         click.echo("URL: http://{}:{}/".format(host, port))
         click.echo("Dry run successful, shutting down.")
-    elif ctx.runtime == ASYNC:
+    elif ff != "":
         create_dapr_server(app, port).run()
     else:
         create_server(app, debug).run(host, port)
```

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/_function_registry.py` & `fc-functions-framework-0.0.9/src/functions_framework/_function_registry.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/_http/__init__.py` & `fc-functions-framework-0.0.9/src/functions_framework/_http/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/_http/flask.py` & `fc-functions-framework-0.0.9/src/functions_framework/_http/flask.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/_http/gunicorn.py` & `fc-functions-framework-0.0.9/src/functions_framework/_http/gunicorn.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/_of/v2/context.py` & `fc-functions-framework-0.0.9/src/functions_framework/_of/v2/context.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/background_event.py` & `fc-functions-framework-0.0.9/src/functions_framework/background_event.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/event_conversion.py` & `fc-functions-framework-0.0.9/src/functions_framework/event_conversion.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/functions_framework/exceptions.py` & `fc-functions-framework-0.0.9/src/functions_framework/exceptions.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/__init__.py` & `fc-functions-framework-0.0.9/src/google/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/cloud/__init__.py` & `fc-functions-framework-0.0.9/src/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/cloud/functions/__init__.py` & `fc-functions-framework-0.0.9/src/google/cloud/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/cloud/functions/context.py` & `fc-functions-framework-0.0.9/src/google/cloud/functions/context.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/cloud/functions_v1/__init__.py` & `fc-functions-framework-0.0.9/src/google/cloud/functions_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/cloud/functions_v1/context.py` & `fc-functions-framework-0.0.9/src/google/cloud/functions_v1/context.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/cloud/functions_v1beta2/__init__.py` & `fc-functions-framework-0.0.9/src/google/cloud/functions_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-functions-framework-0.0.8/src/google/cloud/functions_v1beta2/context.py` & `fc-functions-framework-0.0.9/src/google/cloud/functions_v1beta2/context.py`

 * *Files identical despite different names*

