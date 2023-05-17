# Comparing `tmp/edx-rest-api-client-5.5.1.tar.gz` & `tmp/edx-rest-api-client-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-rest-api-client-5.5.1.tar", last modified: Tue May 16 12:28:12 2023, max compression
+gzip compressed data, was "edx-rest-api-client-5.5.2.tar", last modified: Wed May 17 15:27:29 2023, max compression
```

## Comparing `edx-rest-api-client-5.5.1.tar` & `edx-rest-api-client-5.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4890 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/edx_rest_api_client/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4890 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.791263 edx-rest-api-client-5.5.2/edx_rest_api_client/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13918 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/setup.py
```

### Comparing `edx-rest-api-client-5.5.1/LICENSE` & `edx-rest-api-client-5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.1/PKG-INFO` & `edx-rest-api-client-5.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-rest-api-client
-Version: 5.5.1
+Version: 5.5.2
 Summary: Client utilities to access various Open edX Platform REST APIs.
 Home-page: https://github.com/openedx/edx-rest-api-client
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx rest api client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edx-rest-api-client-5.5.1/README.rst` & `edx-rest-api-client-5.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.1/edx_rest_api_client/auth.py` & `edx-rest-api-client-5.5.2/edx_rest_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.1/edx_rest_api_client/client.py` & `edx-rest-api-client-5.5.2/edx_rest_api_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,18 @@
 
 
 def get_request_id():
     """
     Helper to get the request id - usually set via an X-Request-ID header
     """
     request = crum.get_current_request()
-    return getattr(request, 'id', None)
+    if request is not None and request.headers is not None:
+        return request.headers.get('X-Request-ID')
+    else:
+        return None
 
 
 def get_oauth_access_token(url, client_id, client_secret, token_type='jwt', grant_type='client_credentials',
                            refresh_token=None,
                            timeout=(REQUEST_CONNECT_TIMEOUT, REQUEST_READ_TIMEOUT)):
     """
     Retrieves OAuth 2.0 access token using the given grant type.
```

### Comparing `edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/PKG-INFO` & `edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-rest-api-client
-Version: 5.5.1
+Version: 5.5.2
 Summary: Client utilities to access various Open edX Platform REST APIs.
 Home-page: https://github.com/openedx/edx-rest-api-client
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx rest api client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edx-rest-api-client-5.5.1/requirements/constraints.txt` & `edx-rest-api-client-5.5.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.1/setup.py` & `edx-rest-api-client-5.5.2/setup.py`

 * *Files identical despite different names*

