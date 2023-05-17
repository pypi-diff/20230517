# Comparing `tmp/oapi-1.59.0.tar.gz` & `tmp/oapi-1.59.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oapi-1.59.0.tar", last modified: Fri Nov  4 22:37:24 2022, max compression
+gzip compressed data, was "oapi-1.59.3.tar", last modified: Wed May 17 04:37:51 2023, max compression
```

## Comparing `oapi-1.59.0.tar` & `oapi-1.59.3.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 22:37:24.456628 oapi-1.59.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-11-04 22:35:34.000000 oapi-1.59.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-11-04 22:37:24.456628 oapi-1.59.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3539 2022-11-04 22:35:34.000000 oapi-1.59.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 22:37:24.456628 oapi-1.59.0/oapi/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14773 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/_multipart_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)   126675 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    61478 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 22:37:24.456628 oapi-1.59.0/oapi/oas/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/oas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   125708 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/oas/model.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/oas/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    15335 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/oas/references.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 22:35:34.000000 oapi-1.59.0/oapi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 22:37:24.456628 oapi-1.59.0/oapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-11-04 22:37:24.000000 oapi-1.59.0/oapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-04 22:37:24.000000 oapi-1.59.0/oapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 22:37:24.000000 oapi-1.59.0/oapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-04 22:37:24.000000 oapi-1.59.0/oapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-04 22:37:24.000000 oapi-1.59.0/oapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-04 22:35:34.000000 oapi-1.59.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-11-04 22:37:24.456628 oapi-1.59.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-04 22:35:34.000000 oapi-1.59.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:51.670410 oapi-1.59.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 04:37:02.000000 oapi-1.59.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-17 04:37:51.674409 oapi-1.59.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-17 04:37:02.000000 oapi-1.59.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:51.670410 oapi-1.59.3/oapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/_multipart_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126802 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61478 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:51.670410 oapi-1.59.3/oapi/oas/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/oas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125708 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/oas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/oas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/oas/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:02.000000 oapi-1.59.3/oapi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:51.670410 oapi-1.59.3/oapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-17 04:37:51.000000 oapi-1.59.3/oapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 04:37:51.000000 oapi-1.59.3/oapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 04:37:51.000000 oapi-1.59.3/oapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 04:37:51.000000 oapi-1.59.3/oapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 04:37:51.000000 oapi-1.59.3/oapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 04:37:02.000000 oapi-1.59.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 04:37:51.674409 oapi-1.59.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 04:37:02.000000 oapi-1.59.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:37:51.670410 oapi-1.59.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-17 04:37:02.000000 oapi-1.59.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-17 04:37:02.000000 oapi-1.59.3/tests/test_model.py
```

### Comparing `oapi-1.59.0/LICENSE` & `oapi-1.59.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oapi-1.59.0/PKG-INFO` & `oapi-1.59.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oapi
-Version: 1.59.0
+Version: 1.59.3
 Summary: An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 Home-page: https://github.com/enorganic/oapi
 Author-email: david@belais.me
 License: MIT
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oapi-1.59.0/README.md` & `oapi-1.59.3/README.md`

 * *Files identical despite different names*

### Comparing `oapi-1.59.0/oapi/_multipart_request.py` & `oapi-1.59.3/oapi/_multipart_request.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.0/oapi/_utilities.py` & `oapi-1.59.3/oapi/_utilities.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.0/oapi/client.py` & `oapi-1.59.3/oapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,18 @@
         safe=safe,
         encoding=encoding,
         errors=errors,
         quote_via=quote_via,
     )
 
 
+def _item_is_not_empty(item: Tuple[str, Any]) -> bool:
+    return bool(item[0] and (item[-1] is not None) and item[-1] != "")
+
+
 def _censor_long_json_strings(text: str, limit: int = 2000) -> str:
     """
     Replace JSON strings (such as base-64 encoded images) longer than `limit`
     with "...".
     """
     limit_expression: str = '[^"]' * limit
     return re.sub(f'"{limit_expression}[^"]*"', '"..."', text)
@@ -844,63 +848,63 @@
 class Client(ABC):
     """
     A base class for OpenAPI clients.
 
     Initialization Parameters:
 
     - url (str): The base URL for API requests.
-    - user (str) = "": A user name for use with HTTP basic authentication.
-    - password (str) = "":  A password for use with HTTP basic authentication.
-    - bearer_token (str) = "": A token for use with HTTP bearer authentication.
-    - api_key (str) = "": An API key with which to authenticate requests.
-    - api_key_in (str) = "header": Where the API key should be conveyed:
+    - user (str): A user name for use with HTTP basic authentication.
+    - password (str):  A password for use with HTTP basic authentication.
+    - bearer_token (str): A token for use with HTTP bearer authentication.
+    - api_key (str): An API key with which to authenticate requests.
+    - api_key_in (str): Where the API key should be conveyed:
       "header", "query" or "cookie".
-    - api_key_name (str) = "": The name of the header, query parameter, or
+    - api_key_name (str): The name of the header, query parameter, or
       cookie parameter in which to convey the API key.
-    - oauth2_client_id (str) = "": An OAuth2 client ID.
-    - oauth2_client_secret (str) = "": An OAuth2 client secret.
-    - oauth2_username (str) = "": A *username* for the "password" OAuth2 grant
+    - oauth2_client_id (str): An OAuth2 client ID.
+    - oauth2_client_secret (str): An OAuth2 client secret.
+    - oauth2_username (str): A *username* for the "password" OAuth2 grant
       type.
-    - oauth2_password (str) = "": A *password* for the "password" OAuth2 grant
+    - oauth2_password (str): A *password* for the "password" OAuth2 grant
       type.
-    - oauth2_authorization_url (str) = "": The authorization URL to use for an
+    - oauth2_authorization_url (str): The authorization URL to use for an
       OAuth2 flow. Can be relative to `url`.
-    - oauth2_token_url (str) = "": The token URL to use for OAuth2
+    - oauth2_token_url (str): The token URL to use for OAuth2
       authentication.
       Can be relative to `url`.
-    - oauth2_refresh_url (str) = "": The URL to be used for obtaining refresh
+    - oauth2_refresh_url (str): The URL to be used for obtaining refresh
       tokens for OAuth2 authentication.
-    - oauth2_flows ((str,)) = (): A tuple containing one or more of the
+    - oauth2_flows ((str,)): A tuple containing one or more of the
       following: "authorizationCode", "implicit", "password" and/or
       "clientCredentials".
-    - open_id_connect_url (str) = "": An OpenID connect URL where a JSON
+    - open_id_connect_url (str): An OpenID connect URL where a JSON
       web token containing OAuth2 information can be found.
     - headers ({str: str}): Default headers to include with all requests.
       Method-specific header arguments will override or modify these, where
       applicable, as will dynamically modified headers such as content-length,
       authorization, cookie, etc.
     - timeout (int): The number of seconds before a request will timeout
       and throw an error. If this is 0 (the default), the system default
       timeout will be used.
-    - retry_number_of_attempts (int) = 1: The number of times to retry
+    - retry_number_of_attempts (int): The number of times to retry
       a request which results in an error.
     - retry_for_errors: A tuple of one or more exception types
       on which to retry a request. To retry for *all* errors,
       pass `(Exception,)` for this argument.
     - retry_hook: A function, accepting one argument (an Exception),
       and returning a boolean value indicating whether to retry the
       request (if retries have not been exhausted). This hook applies
       *only* for exceptions which are a sub-class of an exception
       included in `retry_for_errors`.
-    - verify_ssl_certificate (bool) = True: If `True`, SSL certificates
+    - verify_ssl_certificate (bool): If `True`, SSL certificates
       are verified, per usual. If `False`, SSL certificates are *not*
       verified.
-    - logger (logging.Logger|None) = None:
+    - logger (logging.Logger|None):
       A `logging.Logger` to which requests should be logged.
-    - echo (bool) = False: If `True`, requests/responses are printed as
+    - echo (bool): If `True`, requests/responses are printed as
       they occur.
     """
 
     __slots__: Tuple[str, ...] = CLIENT_SLOTS
 
     @rename_parameters(retry_for_exceptions="retry_for_errors")
     def __init__(
@@ -1242,14 +1246,16 @@
         content_encoding: str
         for content_encoding in request.headers.get(
             "Content-encoding", ""
         ).split(","):
             content_encoding = content_encoding.strip().lower()
             if content_encoding and content_encoding == "gzip":
                 curl_options = f"{curl_options} --compressed"
+        if not self._verify_ssl_certificate:
+            curl_options = f"{curl_options} -k"
         self._get_request_response_callback()(
             get_request_curl(request, options=curl_options)
         )
 
     def _request_oauth2_password_authorization(
         self,
     ) -> sob.abc.Readable:
@@ -1334,15 +1340,15 @@
         return self.headers["Authorization"]
 
     def _get_oauth2_password_authorization(self) -> str:
         if self._oauth2_authorization_expires < int(time.time()) or (
             "Authorization" not in self.headers
         ):
             # If our authorization has expired, get a new token
-            with (self._request_oauth2_password_authorization()) as response:
+            with self._request_oauth2_password_authorization() as response:
                 response_data: Dict[str, str] = json.loads(
                     str(response.read(), encoding="utf-8")
                 )
                 self._oauth2_authorization_expires = (
                     int(time.time()) + int(response_data["expires_in"]) - 1
                 )
                 self.headers["Authorization"] = (
@@ -3298,15 +3304,15 @@
             map(
                 lambda item: (
                     item[0],
                     sob.utilities.inspect.represent(item[1]),
                 ),
                 # Both key and value must resolve to `True` when cast as `bool`
                 filter(
-                    all,
+                    _item_is_not_empty,
                     self._init_parameter_defaults.items(),
                 ),
             ),
             self._init_parameter_defaults_source.items(),
         ):
             pattern: Pattern
             if parameter_name == "url":
```

### Comparing `oapi-1.59.0/oapi/model.py` & `oapi-1.59.3/oapi/model.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.0/oapi/oas/model.py` & `oapi-1.59.3/oapi/oas/model.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.0/oapi/oas/references.py` & `oapi-1.59.3/oapi/oas/references.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
           `open` as the value for the `urlopen` parameter
           in this case).
     """
 
     def __init__(
         self,
         root: OpenAPI,
-        url: str = None,
+        url: Optional[str] = None,
         urlopen: Callable = _urlopen,
     ) -> None:
         # Ensure arguments are of the correct types
         assert callable(urlopen)
         assert isinstance(root, OpenAPI)
         assert isinstance(url, (str, sob.utilities.types.NoneType))
         # This is the function used to open external pointer references
```

### Comparing `oapi-1.59.0/oapi.egg-info/PKG-INFO` & `oapi-1.59.3/oapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oapi
-Version: 1.59.0
+Version: 1.59.3
 Summary: An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 Home-page: https://github.com/enorganic/oapi
 Author-email: david@belais.me
 License: MIT
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oapi-1.59.0/setup.cfg` & `oapi-1.59.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oapi
-version = 1.59.0
+version = 1.59.3
 author_email = david@belais.me
 description = An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/enorganic/oapi
```

