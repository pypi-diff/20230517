# Comparing `tmp/stac-fastapi.api-2.4.6.tar.gz` & `tmp/stac-fastapi.api-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.api-2.4.6.tar", last modified: Wed May 10 15:53:13 2023, max compression
+gzip compressed data, was "stac-fastapi.api-2.4.7.tar", last modified: Wed May 17 15:30:48 2023, max compression
```

## Comparing `stac-fastapi.api-2.4.6.tar` & `stac-fastapi.api-2.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.570464 stac-fastapi.api-2.4.6/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.570464 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/top_level.txt
```

### Comparing `stac-fastapi.api-2.4.6/PKG-INFO` & `stac-fastapi.api-2.4.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 2.4.6
+Version: 2.4.7
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.api-2.4.6/setup.py` & `stac-fastapi.api-2.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi/api/app.py` & `stac-fastapi.api-2.4.7/stac_fastapi/api/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""fastapi app creation."""
+"""Fastapi app creation."""
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import attr
 from brotli_asgi import BrotliMiddleware
 from fastapi import APIRouter, FastAPI
 from fastapi.openapi.utils import get_openapi
 from fastapi.params import Depends
@@ -33,30 +33,40 @@
 from stac_fastapi.types.search import BaseSearchGetRequest, BaseSearchPostRequest
 
 
 @attr.s
 class StacApi:
     """StacApi factory.
 
-    Factory for creating a STAC-compliant FastAPI application.  After instantation, the application is accessible from
-    the `StacApi.app` attribute.
+    Factory for creating a STAC-compliant FastAPI application.  After
+    instantation, the application is accessible from the `StacApi.app` attribute.
 
     Attributes:
         settings:
-            API settings and configuration, potentially using environment variables. See https://pydantic-docs.helpmanual.io/usage/settings/.
+            API settings and configuration, potentially using environment
+            variables. See https://pydantic-docs.helpmanual.io/usage/settings/.
         client:
-            A subclass of `stac_api.clients.BaseCoreClient`.  Defines the application logic which is injected into the API.
+            A subclass of `stac_api.clients.BaseCoreClient`.  Defines the
+            application logic which is injected into the API.
         extensions:
-            API extensions to include with the application.  This may include official STAC extensions as well as third-party add ons.
+            API extensions to include with the application.  This may include
+            official STAC extensions as well as third-party add ons.
         exceptions:
-            Defines a global mapping between exceptions and status codes, allowing configuration of response behavior on certain exceptions (https://fastapi.tiangolo.com/tutorial/handling-errors/#install-custom-exception-handlers).
+            Defines a global mapping between exceptions and status codes,
+            allowing configuration of response behavior on certain exceptions
+            (https://fastapi.tiangolo.com/tutorial/handling-errors/#install-custom-exception-handlers).
         app:
             The FastAPI application, defaults to a fresh application.
-        route_dependencies (list of tuples of route scope dicts (eg `{'path': '/collections', 'method': 'POST'}`) and list of dependencies (e.g. `[Depends(oauth2_scheme)]`)):
-            Applies specified dependencies to specified routes. This is useful for applying custom auth requirements to routes defined elsewhere in the application.
+        route_dependencies:
+            List of tuples of route scope dicts (eg `{'path':
+            '/collections', 'method': 'POST'}`) and list of dependencies (e.g.
+            `[Depends(oauth2_scheme)]`)).  Applies specified dependencies to
+            specified routes. This is useful
+            for applying custom auth requirements to routes defined elsewhere in
+            the application.
     """
 
     settings: ApiSettings = attr.ib()
     client: Union[AsyncBaseCoreClient, BaseCoreClient] = attr.ib()
     extensions: List[ApiExtension] = attr.ib(default=attr.Factory(list))
     exceptions: Dict[Type[Exception], int] = attr.ib(
         default=attr.Factory(lambda: DEFAULT_STATUS_CODES)
@@ -337,16 +347,19 @@
 
     def add_route_dependencies(
         self, scopes: List[Scope], dependencies=List[Depends]
     ) -> None:
         """Add custom dependencies to routes.
 
         Args:
-            scopes: list of scopes. Each scope should be a dict with a `path` and `method` property.
-            dependencies: list of [FastAPI dependencies](https://fastapi.tiangolo.com/tutorial/dependencies/) to apply to each scope.
+            scopes: list of scopes. Each scope should be a dict with a `path`
+                and `method` property.
+            dependencies: list of [FastAPI
+                dependencies](https://fastapi.tiangolo.com/tutorial/dependencies/)
+                to apply to each scope.
 
         Returns:
             None
         """
         return add_route_dependencies(self.app.router.routes, scopes, dependencies)
 
     def __attrs_post_init__(self):
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi/api/config.py` & `stac-fastapi.api-2.4.7/stac_fastapi/api/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Application settings."""
 import enum
 
 
 # TODO: Move to stac-pydantic
-# Does that make sense now? The shift to json schema rather than a well-known enumeration makes that less obvious.
+# Does that make sense now? The shift to json schema rather than a well-known
+# enumeration makes that less obvious.
 class ApiExtensions(enum.Enum):
     """Enumeration of available stac api extensions.
 
     Ref: https://github.com/radiantearth/stac-api-spec/tree/master/extensions
     """
 
     context = "context"
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi/api/errors.py` & `stac-fastapi.api-2.4.7/stac_fastapi/api/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     InvalidQueryParameter: status.HTTP_400_BAD_REQUEST,
 }
 
 
 class ErrorResponse(TypedDict):
     """A JSON error response returned by the API.
 
-    The STAC API spec expects that `code` and `description` are both present in the payload.
+    The STAC API spec expects that `code` and `description` are both present in
+    the payload.
 
     Attributes:
         code: A code representing the error, semantics are up to implementor.
         description: A description of the error.
     """
 
     code: str
@@ -73,15 +74,15 @@
     Args:
         app: the FastAPI application.
         status_codes: mapping between exceptions and status codes.
 
     Returns:
         None
     """
-    for (exc, code) in status_codes.items():
+    for exc, code in status_codes.items():
         app.add_exception_handler(exc, exception_handler_factory(code))
 
     # By default FastAPI will return 422 status codes for invalid requests
     # But the STAC api spec suggests returning a 400 in this case
     def request_validation_exception_handler(
         request: Request, exc: RequestValidationError
     ) -> JSONResponse:
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi/api/middleware.py` & `stac-fastapi.api-2.4.7/stac_fastapi/api/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""api middleware."""
+"""Api middleware."""
 import re
 import typing
 from http.client import HTTP_PORT, HTTPS_PORT
 from typing import List, Tuple
 
 from starlette.middleware.cors import CORSMiddleware as _CORSMiddleware
 from starlette.types import ASGIApp, Receive, Scope, Send
 
 
 class CORSMiddleware(_CORSMiddleware):
-    """
-    Subclass of Starlette's standard CORS middleware with default values set to those reccomended by the STAC API spec.
+    """Subclass of Starlette's standard CORS middleware with default values set to those
+    reccomended by the STAC API spec.
 
     https://github.com/radiantearth/stac-api-spec/blob/914cf8108302e2ec734340080a45aaae4859bb63/implementation.md#cors
     """
 
     def __init__(
         self,
         app: ASGIApp,
@@ -40,20 +40,19 @@
             allow_origin_regex,
             expose_headers,
             max_age,
         )
 
 
 class ProxyHeaderMiddleware:
-    """
-    Account for forwarding headers when deriving base URL.
+    """Account for forwarding headers when deriving base URL.
 
     Prioritise standard Forwarded header, look for non-standard X-Forwarded-* if missing.
-    Default to what can be derived from the URL if no headers provided.
-    Middleware updates the host header that is interpreted by starlette when deriving Request.base_url.
+    Default to what can be derived from the URL if no headers provided. Middleware updates
+    the host header that is interpreted by starlette when deriving Request.base_url.
     """
 
     def __init__(self, app: ASGIApp):
         """Create proxy header middleware."""
         self.app = app
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi/api/models.py` & `stac-fastapi.api-2.4.7/stac_fastapi/api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""api request/response models."""
+"""Api request/response models."""
 
 import importlib.util
 from typing import Optional, Type, Union
 
 import attr
 from fastapi import Body, Path
 from pydantic import BaseModel, create_model
@@ -40,15 +40,15 @@
     # Handle GET requests
     if all([issubclass(m, APIRequest) for m in models]):
         return attr.make_class(model_name, attrs={}, bases=tuple(models))
 
     # Handle POST requests
     elif all([issubclass(m, BaseModel) for m in models]):
         for model in models:
-            for (k, v) in model.__fields__.items():
+            for k, v in model.__fields__.items():
                 field_info = v.field_info
                 body = Body(
                     None
                     if isinstance(field_info.default, UndefinedType)
                     else field_info.default,
                     default_factory=field_info.default_factory,
                     alias=field_info.alias,
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi/api/openapi.py` & `stac-fastapi.api-2.4.7/stac_fastapi/api/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         )
         super().__init__(*args, **kwargs)
 
 
 def update_openapi(app: FastAPI) -> FastAPI:
     """Update OpenAPI response content-type.
 
-    This function modifies the openapi route to comply with the STAC API spec's
-    required content-type response header.
+    This function modifies the openapi route to comply with the STAC API spec's required
+    content-type response header.
     """
     # Find the route for the openapi_url in the app
     openapi_route: Route = next(
         route for route in app.router.routes if route.path == app.openapi_url
     )
     # Store the old endpoint function so we can call it from the patched function
     old_endpoint = openapi_route.endpoint
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi/api/routes.py` & `stac-fastapi.api-2.4.7/stac_fastapi/api/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""route factories."""
+"""Route factories."""
 import functools
 import inspect
 from typing import Any, Callable, Dict, List, Optional, Type, TypedDict, Union
 
 from fastapi import Depends, params
 from fastapi.dependencies.utils import get_parameterless_sub_dependant
 from pydantic import BaseModel
@@ -100,15 +100,14 @@
     defined.
 
     Returns:
         None
     """
     for scope in scopes:
         for route in routes:
-
             match, _ = route.matches({"type": "http", **scope})
             if match != Match.FULL:
                 continue
 
             # Mimicking how APIRoute handles dependencies:
             # https://github.com/tiangolo/fastapi/blob/1760da0efa55585c19835d81afa8ca386036c325/fastapi/routing.py#L408-L412
             for depends in dependencies[::-1]:
@@ -116,11 +115,12 @@
                     0,
                     get_parameterless_sub_dependant(
                         depends=depends, path=route.path_format
                     ),
                 )
 
             # Register dependencies directly on route so that they aren't ignored if
-            # the routes are later associated with an app (e.g. app.include_router(router))
+            # the routes are later associated with an app (e.g.
+            # app.include_router(router))
             # https://github.com/tiangolo/fastapi/blob/58ab733f19846b4875c5b79bfb1f4d1cb7f4823f/fastapi/applications.py#L337-L360
             # https://github.com/tiangolo/fastapi/blob/58ab733f19846b4875c5b79bfb1f4d1cb7f4823f/fastapi/routing.py#L677-L678
             route.dependencies.extend(dependencies)
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/PKG-INFO` & `stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 2.4.6
+Version: 2.4.7
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/SOURCES.txt` & `stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

