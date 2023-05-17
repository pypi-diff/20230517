# Comparing `tmp/shieldapi-1.0.0.tar.gz` & `tmp/shieldapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shieldapi-1.0.0.tar", last modified: Thu Apr 20 10:43:32 2023, max compression
+gzip compressed data, was "shieldapi-1.1.0.tar", last modified: Wed May 17 09:45:22 2023, max compression
```

## Comparing `shieldapi-1.0.0.tar` & `shieldapi-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:32.272446 shieldapi-1.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-04-20 10:43:16.000000 shieldapi-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-04-20 10:43:32.272446 shieldapi-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    18374 2023-04-20 10:43:16.000000 shieldapi-1.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-04-20 10:43:16.000000 shieldapi-1.0.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-04-20 10:43:32.272446 shieldapi-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-20 10:43:16.000000 shieldapi-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:32.268445 shieldapi-1.0.0/shieldapi/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:16.000000 shieldapi-1.0.0/shieldapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:32.272446 shieldapi-1.0.0/shieldapi/frameworks/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:16.000000 shieldapi-1.0.0/shieldapi/frameworks/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5484 2023-04-20 10:43:16.000000 shieldapi-1.0.0/shieldapi/frameworks/fastapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-04-20 10:43:16.000000 shieldapi-1.0.0/shieldapi/frameworks/flask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15151 2023-04-20 10:43:16.000000 shieldapi-1.0.0/shieldapi/keycloak_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:32.272446 shieldapi-1.0.0/shieldapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-04-20 10:43:32.000000 shieldapi-1.0.0/shieldapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-20 10:43:32.000000 shieldapi-1.0.0/shieldapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:43:32.000000 shieldapi-1.0.0/shieldapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 10:43:32.000000 shieldapi-1.0.0/shieldapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 10:43:32.000000 shieldapi-1.0.0/shieldapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:32.272446 shieldapi-1.0.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:43:16.000000 shieldapi-1.0.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2373 2023-04-20 10:43:16.000000 shieldapi-1.0.0/tests/mock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3177 2023-04-20 10:43:16.000000 shieldapi-1.0.0/tests/test_fastapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      771 2023-04-20 10:43:16.000000 shieldapi-1.0.0/tests/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-20 10:43:16.000000 shieldapi-1.0.0/tests/test_keycloak_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:22.940350 shieldapi-1.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-05-17 09:45:05.000000 shieldapi-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-05-17 09:45:22.940350 shieldapi-1.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18374 2023-05-17 09:45:05.000000 shieldapi-1.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-05-17 09:45:05.000000 shieldapi-1.1.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-05-17 09:45:22.940350 shieldapi-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-17 09:45:05.000000 shieldapi-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:22.940350 shieldapi-1.1.0/shieldapi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:05.000000 shieldapi-1.1.0/shieldapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:22.940350 shieldapi-1.1.0/shieldapi/frameworks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:05.000000 shieldapi-1.1.0/shieldapi/frameworks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5484 2023-05-17 09:45:05.000000 shieldapi-1.1.0/shieldapi/frameworks/fastapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3853 2023-05-17 09:45:05.000000 shieldapi-1.1.0/shieldapi/frameworks/flask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14530 2023-05-17 09:45:05.000000 shieldapi-1.1.0/shieldapi/keycloak_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:22.940350 shieldapi-1.1.0/shieldapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-05-17 09:45:22.000000 shieldapi-1.1.0/shieldapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-17 09:45:22.000000 shieldapi-1.1.0/shieldapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:45:22.000000 shieldapi-1.1.0/shieldapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-17 09:45:22.000000 shieldapi-1.1.0/shieldapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 09:45:22.000000 shieldapi-1.1.0/shieldapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:22.940350 shieldapi-1.1.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:45:05.000000 shieldapi-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-17 09:45:05.000000 shieldapi-1.1.0/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2369 2023-05-17 09:45:05.000000 shieldapi-1.1.0/tests/mock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3177 2023-05-17 09:45:05.000000 shieldapi-1.1.0/tests/test_fastapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-05-17 09:45:05.000000 shieldapi-1.1.0/tests/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-17 09:45:05.000000 shieldapi-1.1.0/tests/test_keycloak_utils.py
```

### Comparing `shieldapi-1.0.0/LICENSE` & `shieldapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shieldapi-1.0.0/PKG-INFO` & `shieldapi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shieldapi
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package for endpoint protection of APIs using Keycloak
 Author: sintef, Fraunhofer IWM
 Author-email: yoav.nahshon@iwm.fraunhofer.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -59,15 +59,15 @@
 In order to successfully enable the callback for the token-generation and token-verification, make sure that the following environmental variables are set correctly.
 
 | Variable name                   | Description                                                                                                | Example value                          |
 | ------------------------------- | ---------------------------------------------------------------------------------------------------------- | -------------------------------------- |
 | `KEYCLOAK_HOST`                 | Hostname of the the Keycloak instance                                                                      | "http://localhost:8080"                |
 | `KEYCLOAK_REALM_NAME`           | Realm name you set under step 2 in the previous chapter                                                    | "my_realm"                             |
 | `KEYCLOAK_CLIENT_ID`            | Client ID you created under step 3.                                                                        | "shieldapi"                            |
-| `KEYCLOAK_CLIENT_SECRET_KEY`    | Client secret you created under step 3 (`access_type` should be set to "confidential").                    | "1169a83e-a237-40ad-90db-8b8d4848de09" |
+| `KEYCLOAK_CLIENT_SECRET`        | Client secret you created under step 3 (`access_type` should be set to "confidential").                    | "1169a83e-a237-40ad-90db-8b8d4848de09" |
 | `KEYCLOAK_VERIFY_HOST`          | Controls whether SSL certificates are verified for HTTPS requests. Default is set to `False`.              | "True"                                 |
 | `KEYCLOAK_REALM_ADMIN_USER`     | User name of the realm admin, if any action shall be performed as admin in your Flask/FastAPI application. | "admin"                                |
 | `KEYCLOAK_REALM_ADMIN_PASSWORD` | Password of the realm admin, if any action shall be performed as admin in your Flask/FastAPI application.  | "admin_password"                       |
 
 ## Usage with Flask
 
 There are several decorators which can be included into the Flask app for authentication of endpoints.
```

### Comparing `shieldapi-1.0.0/README.md` & `shieldapi-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 In order to successfully enable the callback for the token-generation and token-verification, make sure that the following environmental variables are set correctly.
 
 | Variable name                   | Description                                                                                                | Example value                          |
 | ------------------------------- | ---------------------------------------------------------------------------------------------------------- | -------------------------------------- |
 | `KEYCLOAK_HOST`                 | Hostname of the the Keycloak instance                                                                      | "http://localhost:8080"                |
 | `KEYCLOAK_REALM_NAME`           | Realm name you set under step 2 in the previous chapter                                                    | "my_realm"                             |
 | `KEYCLOAK_CLIENT_ID`            | Client ID you created under step 3.                                                                        | "shieldapi"                            |
-| `KEYCLOAK_CLIENT_SECRET_KEY`    | Client secret you created under step 3 (`access_type` should be set to "confidential").                    | "1169a83e-a237-40ad-90db-8b8d4848de09" |
+| `KEYCLOAK_CLIENT_SECRET`        | Client secret you created under step 3 (`access_type` should be set to "confidential").                    | "1169a83e-a237-40ad-90db-8b8d4848de09" |
 | `KEYCLOAK_VERIFY_HOST`          | Controls whether SSL certificates are verified for HTTPS requests. Default is set to `False`.              | "True"                                 |
 | `KEYCLOAK_REALM_ADMIN_USER`     | User name of the realm admin, if any action shall be performed as admin in your Flask/FastAPI application. | "admin"                                |
 | `KEYCLOAK_REALM_ADMIN_PASSWORD` | Password of the realm admin, if any action shall be performed as admin in your Flask/FastAPI application.  | "admin_password"                       |
 
 ## Usage with Flask
 
 There are several decorators which can be included into the Flask app for authentication of endpoints.
```

### Comparing `shieldapi-1.0.0/setup.cfg` & `shieldapi-1.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shieldapi
-version = v1.0.0
+version = v1.1.0
 author = sintef, Fraunhofer IWM
 author_email = yoav.nahshon@iwm.fraunhofer.de
 description = A package for endpoint protection of APIs using Keycloak
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
@@ -25,14 +25,15 @@
 	dunamai==1.7.0
 	pre-commit~=2.20.0
 tests = 
 	pytest>=7.1.3,<8.0
 	requests-mock>=1.10.0,<2.0
 	httpx>=0.23.3,<1.0
 	semver>=2.13.0,<3.0
+	pytest-mock>=3.10.0
 
 [bumpver]
 current_version = "v0.0.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
```

### Comparing `shieldapi-1.0.0/shieldapi/frameworks/fastapi.py` & `shieldapi-1.1.0/shieldapi/frameworks/fastapi.py`

 * *Files identical despite different names*

### Comparing `shieldapi-1.0.0/shieldapi/frameworks/flask.py` & `shieldapi-1.1.0/shieldapi/frameworks/flask.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """functions and decorators for shieldapi in Flask."""
 from functools import wraps
 from typing import Callable, List
 
 from flask import abort, request
 
-from shieldapi.keycloak_utils import get_keycloak_openid
+from shieldapi.keycloak_utils import (
+    check_role,
+    check_token_validity,
+    get_keycloak_openid,
+)
 
 
 def get_access_token():
     """
     Returns the access token from the Authorization header of the request.
 
     Returns:
@@ -61,17 +65,17 @@
 
     @wraps(fn)
     def decorated_view(*args, **kwargs):
         access_token = get_access_token()
         if not access_token:
             abort(401)
 
-        token_info = get_keycloak_openid().introspect(access_token)
+        valid = check_token_validity(access_token)
 
-        if not token_info["active"]:
+        if not valid:
             abort(401)
 
         return fn(*args, **kwargs)
 
     return decorated_view
 
 
@@ -90,30 +94,57 @@
 
     @wraps(fn)
     def decorated_view(*args, **kwargs):
         access_token = get_access_token()
         if not access_token:
             abort(401)
 
-        token_info = get_keycloak_openid().introspect(access_token)
-
-        if not token_info["active"]:
-            abort(401)
-
-        if not ("roles" in token_info and "admin" in token_info["roles"]):
+        if not check_role(access_token, "admin"):
             abort(403)
 
         return fn(*args, **kwargs)
 
     return decorated_view
 
 
+def role_required(role: str) -> Callable:
+    """
+    Decorator that limits access to users with a certain role.
+
+    Args:
+        role (str):
+            The required role.
+
+    Returns:
+        Callable:
+            The decorator function.
+    """
+
+    def decorator(f: Callable) -> Callable:
+        @wraps(f)
+        def restricted_function(*args, **kwargs):
+            access_token = get_access_token()
+            if not access_token:
+                abort(401)
+
+            if not check_role(access_token, role):
+                abort(403)
+
+            res = f(*args, **kwargs)
+
+            return res
+
+        return restricted_function
+
+    return decorator
+
+
 def has_scope(scope_list: List[str]) -> Callable:
     """
-    Create a decorator that limits access to the applications which have been
+    Decorator that limits access to the applications which have been
     granted the required scopes.
 
     Args:
         scope_list (List[str]):
             The list of required scopes.
 
     Returns:
```

### Comparing `shieldapi-1.0.0/shieldapi/keycloak_utils.py` & `shieldapi-1.1.0/shieldapi/keycloak_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,180 +8,175 @@
 from keycloak import KeycloakAdmin, KeycloakOpenID
 
 
 def get_keycloak_openid(
     server_url: Optional[str] = None,
     realm_name: Optional[str] = None,
     client_id: Optional[str] = None,
-    client_secret_key: Optional[str] = None,
+    client_secret: Optional[str] = None,
     verify: Optional[bool] = None,
 ) -> KeycloakOpenID:
     """
     Creates a KeycloakOpenID instance using the provided parameters or environment variables.
 
     Kwargs:
         server_url (Optional[str]):
-            The URL of the Keycloak server. If not provided, the value from the environment variable
-            KEYCLOAK_HOST will be used.
+            The URL of the Keycloak server. If missing, $KEYCLOAK_HOST  or 'http://keycloak:8080/auth/' will be used.
         realm_name (Optional[str]):
-            The name of the realm in Keycloak. If not provided, the value from the environment variable
-            KEYCLOAK_REALM_NAME will be used.
+            The name of the realm in Keycloak. If missing, $KEYCLOAK_REALM_NAME will be used.
         client_id (Optional[str]):
-            The id of the client in Keycloak. If not provided, the value from the environment
-            variable KEYCLOAK_CLIENT_ID will be used.
-        client_secret_key (Optional[str]):
-            The client secret key for the client in Keycloak. If not provided, the value from the environment
-            variable KEYCLOAK_CLIENT_SECRET_KEY will be used.
+            The id of the client in Keycloak. If missing, $KEYCLOAK_CLIENT_ID or 'shieldapi' will be used.
+        client_secret (Optional[str]):
+            The client secret key for the client in Keycloak. If missing, $KEYCLOAK_CLIENT_SECRET will be used.
         verify (Optional[bool]):
             Controls whether SSL certificates are verified for HTTPS requests. If set to False, SSL
             verification is disabled. If set to a string, it should be the path to a CA_BUNDLE file or
             a directory containing certificates of trusted CA.
 
     Returns:
         KeycloakOpenID: An object for communicating with Keycloak via OpenID Connect.
 
     Raises:
-        KeyError: If any required environment variables are missing.
+        KeyError: If any required values are missing.
     """
 
     return KeycloakOpenID(
-        server_url=_get_value(server_url, "KEYCLOAK_HOST"),
+        server_url=_get_value(
+            server_url, "KEYCLOAK_HOST", "http://keycloak:8080/auth/"
+        ),
         realm_name=_get_value(realm_name, "KEYCLOAK_REALM_NAME"),
-        client_id=_get_value(client_id, "KEYCLOAK_CLIENT_ID"),
-        client_secret_key=_get_value(client_secret_key, "KEYCLOAK_CLIENT_SECRET_KEY"),
-        verify=_eval_bool(verify, "KEYCLOAK_VERIFY_HOST"),
+        client_id=_get_value(client_id, "KEYCLOAK_CLIENT_ID", "shieldapi"),
+        client_secret_key=_get_value(client_secret, "KEYCLOAK_CLIENT_SECRET"),
+        verify=_get_value(verify, "KEYCLOAK_VERIFY_HOST", True, True),
     )
 
 
 def get_keycloak_admin(
     server_url: Optional[str] = None,
     username: Optional[str] = None,
     password: Optional[str] = None,
     realm_name: Optional[str] = None,
     verify: Optional[bool] = None,
 ) -> KeycloakAdmin:
     """Create and return a KeycloakAdmin object with the provided credentials.
 
     Kwargs:
         server_url (Optional[str]):
-            The URL of the Keycloak server. If not provided, the value from the environment variable
-            KEYCLOAK_HOST will be used.
+            The URL of the Keycloak server. If missing, $KEYCLOAK_HOST or 'http://keycloak:8080/auth/' will be used.
         username (Optional[str]):
-            The username to log in with. If not provided, the value from the environment variable
-            KEYCLOAK_REALM_ADMIN_USER will be used.
+            The username to log in with. If missing, $KEYCLOAK_REALM_ADMIN_USER will be used.
         password (Optional[str]):
-            The password to log in with. If not provided, the value from the environment variable
-            KEYCLOAK_REALM_ADMIN_PASSWORD will be used.
+            The password to log in with. If missing, $KEYCLOAK_REALM_ADMIN_PASSWORD will be used.
         realm_name (Optional[str]):
-            The name of the realm in Keycloak. If not provided, the value from the environment variable
-            KEYCLOAK_REALM_NAME will be used.
+            The name of the realm in Keycloak. If missing, $KEYCLOAK_REALM_NAME will be used.
         verify (Optional[bool]):
             Controls whether SSL certificates are verified for HTTPS requests. If set to False, SSL
             verification is disabled. If set to a string, it should be the path to a CA_BUNDLE file or
             a directory containing certificates of trusted CA.
 
     Returns:
         KeycloakAdmin:
             An object with the provided credentials.
 
     Raises:
         KeyError:
-            If any required environment variables are missing.
+            If any required values are missing.
     """
     return KeycloakAdmin(
-        server_url=_get_value(server_url, "KEYCLOAK_HOST"),
+        server_url=_get_value(
+            server_url, "KEYCLOAK_HOST", "http://keycloak:8080/auth/"
+        ),
         username=_get_value(username, "KEYCLOAK_REALM_ADMIN_USER"),
         password=_get_value(password, "KEYCLOAK_REALM_ADMIN_PASSWORD"),
         realm_name=_get_value(realm_name, "KEYCLOAK_REALM_NAME"),
-        verify=_eval_bool(verify, "KEYCLOAK_VERIFY_HOST"),
+        verify=_get_value(verify, "KEYCLOAK_VERIFY_HOST", True, True),
     )
 
 
-def _get_value(var: Any, env_var: str) -> Any:
-    """Check if both, a Python-object and the corresponding
-    env-variable are `None` or not. If both not `None`, a warning
-    is raised. If the Python-object is `None`, it returns the
-    value of the env-variable, even if it is `None`. If the Python-object
-    is an instance of type <bool>, the env-variable will be neglected,
-    even if not `None`.
+def _get_value(
+    param: Any,
+    env_var: str,
+    default: Optional[Any] = None,
+    boolean: Optional[bool] = False,
+) -> Any:
+    """Get a value by following the assignment priority.
+
+    Parameters take priority over environment variables and defaults.
+    An error is raised if no values are defined.
 
     Args:
         var (Any):
-            Python-object passed to the respective upstream function.
+            parameter passed to the respective upstream function.
         env_var (str):
             Name of the corresponding environmental variable.
+        default (Optional[Any]):
+            Default value when no others are provided
+        boolean (Optional[bool]):
+            Whether the expected values is a boolean
     Returns:
         Any: The value of the Python-object (preferred) or its respective env-variable.
         The latter can also resolve into a `None`, if not set.
 
     Raises:
-       UserWarning: If both variables are not `None`.
-
-       ValueError: If both variables are `None` or if the Python-object is `False`
-       and env-variable not `None`.
+       UserWarning: If both the parameter and env-variable are set.
+       ValueError: If both the parameter and env-variable are None, or a boolean
     """
     env = os.environ.get(env_var)
-    if var and env:
-        message = f"""Both the kwarg and the env-variable for `{env_var}` are assigned.
+
+    if (param or isinstance(param, bool)) and env:
+        message = f"""Both the kwarg ({param}) and the env-variable for '{env_var}' ({env}) are assigned.
         Note that the argument takes precedence over the env-variable."""
         warnings.warn(UserWarning(message))
-    elif isinstance(var, bool) and env:
-        message = f"""Both the kwarg and the env-variable for `{env_var}` are assigned.
-        The kwarg is of type `bool` and valued `{var}` whereas the env-variable is set
-        to `{env}`. Note that the argument takes precedence over the env-variable."""
-        warnings.warn(UserWarning(message))
-    elif var is None and env is None:
-        message = f"""Both the kwarg and the env-variable for `{env_var}` are `None`.
+    elif param is None and env is None and default is None:
+        message = f"""Both the kwarg and the env-variable for '{env_var}' are None.
         Please assign one of them to a value."""
         raise ValueError(message)
-    if isinstance(var, bool):
-        return var
+
+    if isinstance(param, bool):
+        return param
     else:
-        return var or env
+        if boolean and env:
+            try:
+                env = literal_eval(env)
+                if not isinstance(env, bool):
+                    raise ValueError
+            except (ValueError, SyntaxError):
+                message = (
+                    f"The '{env_var}' env-var valued '{env}' must be 'True' or 'False'."
+                )
+                print(message, flush=True)
+                raise TypeError(message)
+        return param or env or default
 
 
-def _eval_bool(var: Any, env_var: str) -> Optional[bool]:
-    """Execute the `_get_value`-helper function and evaluate if
-    the value of the environment variable is a string matching to a bool.
+def check_role(token: str, role: str) -> bool:
+    """Check if a token contains a certain role
 
     Args:
-        var (Any):
-            Python-object passed to the respective upstream function.
-        env_var (str):
-            Name of the corresponding environmental variable.
+        token (str): token from a user
+        role (str): role to be checked
+
     Returns:
-        Optional[bool]:
-            The evaluated value of the environment variable as a boolean, or None
-            if the environment variable does not exist.
-    Raises:
-        TypeError: If the value of the environmental variable cannot be evaluated or it
-        can be evaluated but is not an instance of <bool>.
+        bool: whether the token contains the role
     """
-    boolean = _get_value(var, env_var)
-    if isinstance(boolean, str):
-        try:
-            value = literal_eval(boolean)
-            assert isinstance(value, bool)
-            return value
-        except (ValueError, AssertionError, SyntaxError):
-            message = f"""Env-variable `{env_var}` valued `{boolean}` is not a boolean.
-            Must be valued `True` or `False`."""
-            raise TypeError(message)
-    elif isinstance(boolean, bool):
-        return boolean
+    token_info = get_keycloak_openid().introspect(token)
+    valid_token = _check_active_token(token_info)
+    if valid_token:
+        return "roles" in token_info and role in token_info["roles"]
+    return False
 
 
 def check_token_validity(
     access_token: str,
     server_url: Optional[str] = None,
     realm_name: Optional[str] = None,
     client_id: Optional[str] = None,
-    client_secret_key: Optional[str] = None,
+    client_secret: Optional[str] = None,
     verify: Optional[bool] = None,
-) -> str:
+) -> bool:
     """Check if the given access token is valid.
 
     Args:
         access_token: str
             The access token to check.
     Kwargs:
         server_url (Optional[str]):
@@ -189,40 +184,50 @@
             KEYCLOAK_HOST will be used.
         realm_name (Optional[str]):
             The name of the realm in Keycloak. If not provided, the value from the environment variable
             KEYCLOAK_REALM_NAME will be used.
         client_id (Optional[str]):
             The id of the client in Keycloak. If not provided, the value from the environment
             variable KEYCLOAK_CLIENT_ID will be used.
-        client_secret_key (Optional[str]):
+        client_secret (Optional[str]):
             The client secret key for the client in Keycloak. If not provided, the value from the environment
-            variable KEYCLOAK_CLIENT_SECRET_KEY will be used.
+            variable KEYCLOAK_CLIENT_SECRET will be used.
         verify (Optional[bool]):
             Controls whether SSL certificates are verified for HTTPS requests. If set to False, SSL
             verification is disabled. If set to a string, it should be the path to a CA_BUNDLE file or
             a directory containing certificates of trusted CA.
 
     Returns:
-        str: If the token is valid, returns the string "valid". Otherwise, returns the string "Invalid Token".
+        bool: Whether the token is valid.
     """
     token_info = get_keycloak_openid(
-        server_url, realm_name, client_id, client_secret_key, verify
+        server_url, realm_name, client_id, client_secret, verify
     ).introspect(access_token)
 
-    if not token_info.json()["active"]:
-        return "Invalid Token"
-    return "valid"
+    return _check_active_token(token_info)
+
+
+def _check_active_token(token_info) -> bool:
+    """Checks if a given token introspect information is marked as valid
+
+    Args:
+        token_info (Any): output from the introspect request
+
+    Returns:
+        bool: Whether the token is valid
+    """
+    return bool(token_info.json()["active"])
 
 
 def check_useraccount_access(
     access_token: str,
     server_url: Optional[str] = None,
     realm_name: Optional[str] = None,
     client_id: Optional[str] = None,
-    client_secret_key: Optional[str] = None,
+    client_secret: Optional[str] = None,
     verify: Optional[bool] = None,
 ) -> str:
     """
     Check if an access token has the 'openid' scope.
 
     Args:
         access_token: str
@@ -233,41 +238,41 @@
             KEYCLOAK_HOST will be used.
         realm_name (Optional[str]):
             The name of the realm in Keycloak. If not provided, the value from the environment variable
             KEYCLOAK_REALM_NAME will be used.
         client_id (Optional[str]):
             The id of the client in Keycloak. If not provided, the value from the environment
             variable KEYCLOAK_CLIENT_ID will be used.
-        client_secret_key (Optional[str]):
+        client_secret (Optional[str]):
             The client secret key for the client in Keycloak. If not provided, the value from the environment
-            variable KEYCLOAK_CLIENT_SECRET_KEY will be used.
+            variable KEYCLOAK_CLIENT_SECRET will be used.
         verify (Optional[bool]):
             Controls whether SSL certificates are verified for HTTPS requests. If set to False, SSL
             verification is disabled. If set to a string, it should be the path to a CA_BUNDLE file or
             a directory containing certificates of trusted CA.
 
     Returns:
         str: A string indicating whether or not the access token has the 'openid' scope.
     """
     token_info = get_keycloak_openid(
-        server_url, realm_name, client_id, client_secret_key, verify
+        server_url, realm_name, client_id, client_secret, verify
     ).introspect(access_token)
     granted_scope = token_info.json()["scope"].split()
     if "openid" not in granted_scope:
         return "openid scope not granted!", 401
     return "Has access!", 200
 
 
 def login(
     username: str,
     password: str,
     server_url: Optional[str] = None,
     realm_name: Optional[str] = None,
     client_id: Optional[str] = None,
-    client_secret_key: Optional[str] = None,
+    client_secret: Optional[str] = None,
     verify: Optional[bool] = None,
 ) -> str:
     """
     Logs in the user with the given username and password and generates an access token.
 
     Args:
         username (Optional[str]):
@@ -280,43 +285,43 @@
             KEYCLOAK_HOST will be used.
         realm_name (Optional[str]):
             The name of the realm in Keycloak. If not provided, the value from the environment variable
             KEYCLOAK_REALM_NAME will be used.
         client_id (Optional[str]):
             The id of the client in Keycloak. If not provided, the value from the environment
             variable KEYCLOAK_CLIENT_ID will be used.
-        client_secret_key (Optional[str]):
+        client_secret (Optional[str]):
             The client secret key for the client in Keycloak. If not provided, the value from the environment
-            variable KEYCLOAK_CLIENT_SECRET_KEY will be used.
+            variable KEYCLOAK_CLIENT_SECRET will be used.
         verify (Optional[Union[bool, str]]):
             Controls whether SSL certificates are verified for HTTPS requests. If set to False, SSL
             verification is disabled. If set to a string, it should be the path to a CA_BUNDLE file or
             a directory containing certificates of trusted CA.
 
     Returns:
         str:
             If successful, returns a string representing the access token. Otherwise, returns
             a tuple containing the status code and an error message.
     """
     token = get_keycloak_openid(
-        server_url, realm_name, client_id, client_secret_key, verify
+        server_url, realm_name, client_id, client_secret, verify
     ).token(username=username, password=password)
     if not token.get("access_token") and token.get("token_type"):
         return 401, "Token could not be generated. Please contact the admin."
     else:
         return f"{token.get('token_type')} {token.get('access_token')}"
 
 
 def make_auth_header(
     username: str,
     password: str,
     server_url: Optional[str] = None,
     realm_name: Optional[str] = None,
     client_id: Optional[str] = None,
-    client_secret_key: Optional[str] = None,
+    client_secret: Optional[str] = None,
     verify: Optional[bool] = None,
 ) -> Union[int, Tuple[int, str]]:
     """
     Logs into the Keycloak server and generates an access token using the given credentials.
 
     Args:
         username (Optional[str]):
@@ -329,28 +334,34 @@
             KEYCLOAK_HOST will be used.
         realm_name (Optional[str]):
             The name of the realm in Keycloak. If not provided, the value from the environment variable
             KEYCLOAK_REALM_NAME will be used.
         client_id (Optional[str]):
             The id of the client in Keycloak. If not provided, the value from the environment
             variable KEYCLOAK_CLIENT_ID will be used.
-        client_secret_key (Optional[str]):
+        client_secret (Optional[str]):
             The client secret key for the client in Keycloak. If not provided, the value from the environment
-            variable KEYCLOAK_CLIENT_SECRET_KEY will be used.
+            variable KEYCLOAK_CLIENT_SECRET will be used.
         verify (Optional[bool]):
             Controls whether SSL certificates are verified for HTTPS requests. If set to False, SSL
             verification is disabled. If set to a string, it should be the path to a CA_BUNDLE file or
             a directory containing certificates of trusted CA.
 
     Returns:
         Union[int, Tuple[int, str]]:
             If successful, a string containing the access token in the form of "{token_type} {access_token}".
             Otherwise, a tuple containing a status code and an error message.
 
     """
     credentials = login(
-        username, password, server_url, realm_name, client_id, client_secret_key, verify
+        username,
+        password,
+        server_url,
+        realm_name,
+        client_id,
+        client_secret,
+        verify,
     )
     if type(credentials) == str:
         return {"Authorization": credentials}
     else:
         return credentials
```

### Comparing `shieldapi-1.0.0/shieldapi.egg-info/PKG-INFO` & `shieldapi-1.1.0/shieldapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shieldapi
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package for endpoint protection of APIs using Keycloak
 Author: sintef, Fraunhofer IWM
 Author-email: yoav.nahshon@iwm.fraunhofer.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -59,15 +59,15 @@
 In order to successfully enable the callback for the token-generation and token-verification, make sure that the following environmental variables are set correctly.
 
 | Variable name                   | Description                                                                                                | Example value                          |
 | ------------------------------- | ---------------------------------------------------------------------------------------------------------- | -------------------------------------- |
 | `KEYCLOAK_HOST`                 | Hostname of the the Keycloak instance                                                                      | "http://localhost:8080"                |
 | `KEYCLOAK_REALM_NAME`           | Realm name you set under step 2 in the previous chapter                                                    | "my_realm"                             |
 | `KEYCLOAK_CLIENT_ID`            | Client ID you created under step 3.                                                                        | "shieldapi"                            |
-| `KEYCLOAK_CLIENT_SECRET_KEY`    | Client secret you created under step 3 (`access_type` should be set to "confidential").                    | "1169a83e-a237-40ad-90db-8b8d4848de09" |
+| `KEYCLOAK_CLIENT_SECRET`        | Client secret you created under step 3 (`access_type` should be set to "confidential").                    | "1169a83e-a237-40ad-90db-8b8d4848de09" |
 | `KEYCLOAK_VERIFY_HOST`          | Controls whether SSL certificates are verified for HTTPS requests. Default is set to `False`.              | "True"                                 |
 | `KEYCLOAK_REALM_ADMIN_USER`     | User name of the realm admin, if any action shall be performed as admin in your Flask/FastAPI application. | "admin"                                |
 | `KEYCLOAK_REALM_ADMIN_PASSWORD` | Password of the realm admin, if any action shall be performed as admin in your Flask/FastAPI application.  | "admin_password"                       |
 
 ## Usage with Flask
 
 There are several decorators which can be included into the Flask app for authentication of endpoints.
```

### Comparing `shieldapi-1.0.0/tests/mock.py` & `shieldapi-1.1.0/tests/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from requests_mock import Mocker
 
 MESSAGE = {"message": "Hello World"}
 VARIABLES = dict(
     KEYCLOAK_HOST="http://example_keycloak.org/auth/",
     KEYCLOAK_REALM_NAME="my_realm",
     KEYCLOAK_CLIENT_ID="testshield",
-    KEYCLOAK_CLIENT_SECRET_KEY="123a",
+    KEYCLOAK_CLIENT_SECRET="123a",
     KEYCLOAK_REALM_ADMIN_USER="admin",
     KEYCLOAK_REALM_ADMIN_PASSWORD="passwd",
     KEYCLOAK_VERIFY_HOST="True",
 )
 
 
 def register_mock(requests_mock: Mocker, var: dict = VARIABLES) -> None:
```

### Comparing `shieldapi-1.0.0/tests/test_fastapi.py` & `shieldapi-1.1.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `shieldapi-1.0.0/tests/test_flask.py` & `shieldapi-1.1.0/tests/test_flask.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @app.get("/login")
 @login_required
 def login():
     """Arbitrary login route"""
     return MESSAGE
 
 
-def test_flask(requests_mock):
+def test_flask(mock_introspect, requests_mock):
     """Pytest for token verification through Keycloak-mock."""
     register_mock(requests_mock)
     client = app.test_client()
     headers = {"Authorization": "Bearer 123"}
     response = client.get("login", headers=headers)  # calls keycloak-mock
     host_list = [resp.hostname for resp in requests_mock.request_history]
     assert host_list.count("example_keycloak.org") == 1  # called 1x keycloak-mock
```

### Comparing `shieldapi-1.0.0/tests/test_keycloak_utils.py` & `shieldapi-1.1.0/tests/test_keycloak_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,39 +50,39 @@
     register_mock(requests_mock)
     key = "KEYCLOAK_REALM_NAME"
     if env_var:
         os.environ[key] = env_var
     else:
         os.environ.pop(key)
     if var is None and env_var is None:
-        match = f"Both the kwarg and the env-variable for `{key}` are `None`."
+        match = f"Both the kwarg and the env-variable for '{key}' are None."
         with pytest.raises(ValueError, match=match):
             no_warning_raised(_get_value, args=(var, key), expected=var)
     elif isinstance(var, bool) and env_var or (var and env_var):
-        match = f"Both the kwarg and the env-variable for `{key}` are assigned."
+        match = f"Both the kwarg ({var}) and the env-variable for '{key}' ({env_var}) are assigned."
         warning_raised(_get_value, match, args=(var, key), expected=var)
 
 
 @pytest.mark.parametrize("func", [get_keycloak_openid, get_keycloak_admin])
 def test_keycloak_warning(func, requests_mock):
     """Pytest for `get_keycloak_openid` and `get_keycloak_admin` with
     both not None-typed values."""
-    match = "Both the kwarg and the env-variable for `KEYCLOAK_HOST`"
+    match = f"Both the kwarg (http://example_keycloak.org/auth/) and the env-variable for 'KEYCLOAK_HOST'"
     register_mock(requests_mock)
     warning_raised(
         func, match, kwargs={"server_url": "http://example_keycloak.org/auth/"}
     )
 
 
 @pytest.mark.parametrize("func", [get_keycloak_openid, get_keycloak_admin])
 def test_keycloak_valueerror(func, requests_mock):
     """Pytest for `get_keycloak_openid` and `get_keycloak_admin` with
     both None-typed values."""
     register_mock(requests_mock)
-    match = "Both the kwarg and the env-variable for `KEYCLOAK_REALM_NAME`"
+    match = "Both the kwarg and the env-variable for 'KEYCLOAK_REALM_NAME'"
     os.environ.pop("KEYCLOAK_REALM_NAME")
     with pytest.raises(ValueError, match=match):
         no_warning_raised(func)
 
 
 @pytest.mark.parametrize("var", [True, False, None])
 @pytest.mark.parametrize(
@@ -90,20 +90,21 @@
 )
 @pytest.mark.parametrize("func", [get_keycloak_openid, get_keycloak_admin])
 def test_keycloak_typeerror_bool(var, test_input, func, requests_mock):
     """Pytest for `get_keycloak_openid` and `get_keycloak_admin` with
     `KEYCLOAK_VERIFY_HOST`."""
     register_mock(requests_mock)
     os.environ["KEYCLOAK_VERIFY_HOST"] = test_input
-    match = "Env-variable `KEYCLOAK_VERIFY_HOST` valued"
+    match = f"The 'KEYCLOAK_VERIFY_HOST' env-var valued"
     if not isinstance(var, bool):
         with pytest.raises(TypeError, match=match):
+            print(match, flush=True)
             no_warning_raised(func)
     else:
-        match = "Both the kwarg and the env-variable for `KEYCLOAK_VERIFY_HOST` are assigned."
+        match = f"Both the kwarg ({var}) and the env-variable for 'KEYCLOAK_VERIFY_HOST' ({test_input}) are assigned."
         warning_raised(func, match, kwargs={"verify": var})
 
 
 @pytest.mark.parametrize("var", [True, False, None])
 @pytest.mark.parametrize("env_var", ["True", "False", None])
 @pytest.mark.parametrize("func", [get_keycloak_openid, get_keycloak_admin])
 def test_keycloak_warning_bool(var, env_var, func, requests_mock):
@@ -112,17 +113,11 @@
     register_mock(requests_mock)
     if env_var:
         os.environ["KEYCLOAK_VERIFY_HOST"] = env_var
     else:
         os.environ.pop("KEYCLOAK_VERIFY_HOST")
 
     if isinstance(var, bool) and env_var:
-        match = "Both the kwarg and the env-variable for `KEYCLOAK_VERIFY_HOST` are assigned."
+        match = f"Both the kwarg ({var}) and the env-variable for 'KEYCLOAK_VERIFY_HOST' ({env_var}) are assigned."
         warning_raised(func, match, kwargs={"verify": var})
-    elif var is None and env_var is None:
-        match = (
-            "Both the kwarg and the env-variable for `KEYCLOAK_VERIFY_HOST` are `None`."
-        )
-        with pytest.raises(ValueError, match=match):
-            no_warning_raised(func, kwargs={"verify": var})
     else:
         no_warning_raised(func, kwargs={"verify": var})
```

