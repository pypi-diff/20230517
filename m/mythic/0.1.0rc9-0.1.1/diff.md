# Comparing `tmp/mythic-0.1.0rc9.tar.gz` & `tmp/mythic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.0rc9.tar", last modified: Mon May  1 17:50:40 2023, max compression
+gzip compressed data, was "mythic-0.1.1.tar", last modified: Wed May 17 21:07:29 2023, max compression
```

## Comparing `mythic-0.1.0rc9.tar` & `mythic-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-01 17:50:40.115728 mythic-0.1.0rc9/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-05-01 17:50:40.115341 mythic-0.1.0rc9/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc9/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-01 17:50:40.112937 mythic-0.1.0rc9/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc9/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc9/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    97649 2023-05-01 17:49:45.000000 mythic-0.1.0rc9/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-25 16:38:38.000000 mythic-0.1.0rc9/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc9/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc9/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-01 17:50:40.114907 mythic-0.1.0rc9/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-01 17:50:40.115831 mythic-0.1.0rc9/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-05-01 17:50:32.000000 mythic-0.1.0rc9/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-17 21:07:29.893484 mythic-0.1.1/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-17 21:07:29.893108 mythic-0.1.1/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1707 2023-05-10 02:44:23.000000 mythic-0.1.1/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-17 21:07:29.891115 mythic-0.1.1/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.1/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.1/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    99712 2023-05-17 20:24:46.000000 mythic-0.1.1/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3373 2023-05-17 19:32:31.000000 mythic-0.1.1/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.1/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7607 2023-05-17 19:28:56.000000 mythic-0.1.1/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-17 21:07:29.892671 mythic-0.1.1/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-17 21:07:29.893586 mythic-0.1.1/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      818 2023-05-17 20:38:50.000000 mythic-0.1.1/setup.py
```

### Comparing `mythic-0.1.0rc9/PKG-INFO` & `mythic-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc9
+Version: 0.1.1
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
@@ -33,13 +33,13 @@
 Version 0.0.21-25 of the `mythic` package supports version 2.2.8+ of the Mythic project (reports as version "3").
 
 Version 0.0.26 of the `mythic` package supports version 2.3+ of the Mythic project (reports as version "3").
 
 Version 0.0.29-0.0.36 of the `mythic` package supports version 2.3+ of the Mythic project utilizing the new GraphQL endpoints and reports as version "3".
 This will be the last version that supports the old mythic_rest interface. Starting with version 0.1.0, the `mythic` PyPi package will only support the new GraphQL interface and will report as version "4".
 
-Version 0.1.0rc1+ of the `mythic` package supports version 3.0 of the Mythic project utilizing the new GraphQL endpoints.
+Version 0.1.0 of the `mythic` package supports version 3.0 of the Mythic project utilizing the new GraphQL endpoints.
 
 # Information
 
 The Jupyter Notebook container within Mythic provides many examples on how to use the package. 
 The `mythic` package leverages async HTTP requests and WebSocket connections, so it's important to make sure your codebase is running asynchronously.
```

### Comparing `mythic-0.1.0rc9/README.md` & `mythic-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 Version 0.0.21-25 of the `mythic` package supports version 2.2.8+ of the Mythic project (reports as version "3").
 
 Version 0.0.26 of the `mythic` package supports version 2.3+ of the Mythic project (reports as version "3").
 
 Version 0.0.29-0.0.36 of the `mythic` package supports version 2.3+ of the Mythic project utilizing the new GraphQL endpoints and reports as version "3".
 This will be the last version that supports the old mythic_rest interface. Starting with version 0.1.0, the `mythic` PyPi package will only support the new GraphQL interface and will report as version "4".
 
-Version 0.1.0rc1+ of the `mythic` package supports version 3.0 of the Mythic project utilizing the new GraphQL endpoints.
+Version 0.1.0 of the `mythic` package supports version 3.0 of the Mythic project utilizing the new GraphQL endpoints.
 
 # Information
 
 The Jupyter Notebook container within Mythic provides many examples on how to use the package. 
 The `mythic` package leverages async HTTP requests and WebSocket connections, so it's important to make sure your codebase is running asynchronously.
```

### Comparing `mythic-0.1.0rc9/mythic/graphql_queries.py` & `mythic-0.1.1/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc9/mythic/mythic.py` & `mythic-0.1.1/mythic/mythic.py`

 * *Files 4% similar despite different names*

```diff
@@ -2168,14 +2168,80 @@
     }
     """
 
     return await mythic_utilities.graphql_post(mythic=mythic, query=query, variables={"webhook_data": webhook_data,
                                                                                       "webhook_type": webhook_type})
 
 
+# ####### C2 Functions #############
+
+async def start_stop_c2_profile(
+        mythic: mythic_classes.Mythic,
+        c2_profile_name: str,
+        action: str = "start"
+):
+    query = """
+    query getC2IdFromName($c2_name: String!) {
+      c2profile(where: {name: {_eq: $c2_name}}){
+        id
+      }
+    }
+    """
+    resp = await mythic_utilities.graphql_post(mythic=mythic, query=query, variables={
+        "c2_name": c2_profile_name,
+    })
+    if len(resp["c2profile"]) == 0:
+        raise Exception(f"Failed to find c2 profile {c2_profile_name}")
+    start_stop = """
+    mutation startStopC2Profile($id: Int!, $action: String!){
+        startStopProfile(id: $id, action: $action){
+            status
+            error
+            output
+        }
+    }
+    """
+    resp = await mythic_utilities.graphql_post(mythic=mythic, query=start_stop, variables={
+        "id": resp["c2profile"][0]["id"], "action": action,
+    })
+    return resp["startStopProfile"]
+
+
+async def create_saved_c2_instance(
+        mythic: mythic_classes.Mythic,
+        instance_name: str,
+        c2_profile_name: str,
+        c2_parameters: dict
+):
+    query = """
+    query getC2IdFromName($c2_name: String!) {
+      c2profile(where: {name: {_eq: $c2_name}}){
+        id
+      }
+    }
+    """
+    resp = await mythic_utilities.graphql_post(mythic=mythic, query=query, variables={
+        "c2_name": c2_profile_name,
+    })
+    if len(resp["c2profile"]) == 0:
+        raise Exception(f"Failed to find c2 profile {c2_profile_name}")
+    mutation = """
+    mutation createNewC2Instance($instance_name: String!, $c2_instance: String!, $c2profile_id: Int!){
+      create_c2_instance(c2_instance: $c2_instance, instance_name: $instance_name, c2profile_id: $c2profile_id){
+        status
+        error
+      }
+    }
+    """
+    resp = await mythic_utilities.graphql_post(mythic=mythic, query=mutation, variables={
+        "instance_name": instance_name, "c2profile_id": resp["c2profile"][0]["id"], "c2_instance": json.dumps(c2_parameters)
+    })
+    return resp["create_c2_instance"]
+
+
 # ####### Tag Functions ############
 
 
 async def create_tag_type(
         mythic: mythic_classes.Mythic,
         color: str = "#71a0d0",
         description: str = "",
```

### Comparing `mythic-0.1.0rc9/mythic/mythic_classes.py` & `mythic-0.1.1/mythic/mythic_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.refresh_token = refresh_token
         self.server_ip = server_ip
         self.server_port = server_port
         self.ssl = ssl
         self.http = "http://" if not ssl else "https://"
         self.ws = "ws://" if not ssl else "wss://"
         self.global_timeout = global_timeout if global_timeout is not None else -1
-        self.scripting_version = "0.1.0rc8"
+        self.scripting_version = "0.1.1"
         self.current_operation_id = 0
         self.schema = schema
 
     def __str__(self):
         return json.dumps(
             {
                 "username": self.username,
```

### Comparing `mythic-0.1.0rc9/mythic/mythic_utilities.py` & `mythic-0.1.1/mythic/mythic_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 async def get_ws_transport(mythic: mythic_classes.Mythic) -> WebsocketsTransport:
     ssl_context = ssl.create_default_context()
     ssl_context.check_hostname = False
     ssl_context.verify_mode = ssl.CERT_NONE
     websocket_transport = WebsocketsTransport(
         url=f"{mythic.ws}{mythic.server_ip}:{mythic.server_port}/graphql/",
         headers=get_headers(mythic),
-        ssl=ssl_context,
+        ssl=ssl_context if mythic.ssl else False,
     )
     return websocket_transport
 
 
 async def http_post(mythic: mythic_classes.Mythic, data: dict, url: str) -> dict:
     try:
         async with aiohttp.ClientSession() as session:
```

### Comparing `mythic-0.1.0rc9/mythic.egg-info/PKG-INFO` & `mythic-0.1.1/mythic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc9
+Version: 0.1.1
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
@@ -33,13 +33,13 @@
 Version 0.0.21-25 of the `mythic` package supports version 2.2.8+ of the Mythic project (reports as version "3").
 
 Version 0.0.26 of the `mythic` package supports version 2.3+ of the Mythic project (reports as version "3").
 
 Version 0.0.29-0.0.36 of the `mythic` package supports version 2.3+ of the Mythic project utilizing the new GraphQL endpoints and reports as version "3".
 This will be the last version that supports the old mythic_rest interface. Starting with version 0.1.0, the `mythic` PyPi package will only support the new GraphQL interface and will report as version "4".
 
-Version 0.1.0rc1+ of the `mythic` package supports version 3.0 of the Mythic project utilizing the new GraphQL endpoints.
+Version 0.1.0 of the `mythic` package supports version 3.0 of the Mythic project utilizing the new GraphQL endpoints.
 
 # Information
 
 The Jupyter Notebook container within Mythic provides many examples on how to use the package. 
 The `mythic` package leverages async HTTP requests and WebSocket connections, so it's important to make sure your codebase is running asynchronously.
```

### Comparing `mythic-0.1.0rc9/setup.py` & `mythic-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.0rc9",
+    version="0.1.1",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

