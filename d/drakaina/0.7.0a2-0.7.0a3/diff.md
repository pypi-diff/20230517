# Comparing `tmp/drakaina-0.7.0a2.tar.gz` & `tmp/drakaina-0.7.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.0a2.tar", max compression
+gzip compressed data, was "drakaina-0.7.0a3.tar", max compression
```

## Comparing `drakaina-0.7.0a2.tar` & `drakaina-0.7.0a3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     9580 2023-05-16 20:10:51.138750 drakaina-0.7.0a2/drakaina/__init__.py
--rw-r--r--   0        0        0    11634 2023-05-16 20:10:51.139749 drakaina-0.7.0a2/drakaina/_types.py
--rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0a2/drakaina/asgi.py
--rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0a2/drakaina/client/__init__.py
--rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0a2/drakaina/client/base.py
--rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0a2/drakaina/client/http.py
--rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0a2/drakaina/client/tcp.py
--rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0a2/drakaina/client/websocket.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0a2/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0a2/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0a2/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0a2/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0a2/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0a2/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     9102 2023-05-16 20:10:51.140763 drakaina-0.7.0a2/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      913 2023-04-03 15:58:34.495338 drakaina-0.7.0a2/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18791 2023-05-16 20:10:51.140763 drakaina-0.7.0a2/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     1651 2023-05-05 11:41:17.675178 drakaina-0.7.0a2/drakaina/drakaina_openapi.py
--rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0a2/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0a2/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1378 2023-03-29 21:57:07.601330 drakaina-0.7.0a2/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7586 2023-05-16 20:10:51.141750 drakaina-0.7.0a2/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     2040 2023-05-16 20:10:51.142823 drakaina-0.7.0a2/drakaina/middleware/exception.py
--rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0a2/drakaina/middleware/gzip.py
--rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0a2/drakaina/middleware/logging.py
--rw-r--r--   0        0        0     1138 2023-01-18 00:52:37.644550 drakaina-0.7.0a2/drakaina/middleware/openapi/__init__.py
--rw-r--r--   0        0        0     1079 2023-04-04 11:19:41.580823 drakaina-0.7.0a2/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12345 2023-05-16 20:10:51.143818 drakaina-0.7.0a2/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0a2/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0    12453 2023-05-16 20:10:51.143818 drakaina-0.7.0a2/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    10527 2023-05-16 19:17:53.349082 drakaina-0.7.0a2/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0a2/drakaina/rsgi.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0a2/drakaina/serializers.py
--rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0a2/drakaina/tcp.py
--rw-r--r--   0        0        0     3740 2023-05-16 20:10:51.144819 drakaina-0.7.0a2/drakaina/utils.py
--rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0a2/drakaina/ws.py
--rw-r--r--   0        0        0     8181 2023-05-16 20:10:51.145819 drakaina-0.7.0a2/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0a2/LICENSE
--rw-r--r--   0        0        0     2715 2023-05-16 20:10:51.145819 drakaina-0.7.0a2/pyproject.toml
--rw-r--r--   0        0        0     5416 2023-05-16 20:10:51.138750 drakaina-0.7.0a2/README.md
--rw-r--r--   0        0        0     6701 1970-01-01 00:00:00.000000 drakaina-0.7.0a2/setup.py
--rw-r--r--   0        0        0     6933 1970-01-01 00:00:00.000000 drakaina-0.7.0a2/PKG-INFO
+-rw-r--r--   0        0        0     9580 2023-05-17 12:11:16.145233 drakaina-0.7.0a3/drakaina/__init__.py
+-rw-r--r--   0        0        0    11634 2023-05-17 12:11:16.146249 drakaina-0.7.0a3/drakaina/_types.py
+-rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0a3/drakaina/asgi.py
+-rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0a3/drakaina/client/__init__.py
+-rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0a3/drakaina/client/base.py
+-rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0a3/drakaina/client/http.py
+-rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0a3/drakaina/client/tcp.py
+-rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0a3/drakaina/client/websocket.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0a3/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0a3/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0a3/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0a3/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0a3/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0a3/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     9102 2023-05-17 12:11:16.147248 drakaina-0.7.0a3/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      913 2023-04-03 15:58:34.495338 drakaina-0.7.0a3/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18791 2023-05-17 12:11:16.148232 drakaina-0.7.0a3/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     1651 2023-05-05 11:41:17.675178 drakaina-0.7.0a3/drakaina/drakaina_openapi.py
+-rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0a3/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0a3/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1378 2023-03-29 21:57:07.601330 drakaina-0.7.0a3/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7586 2023-05-17 12:11:16.148232 drakaina-0.7.0a3/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     2040 2023-05-17 12:11:16.149237 drakaina-0.7.0a3/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0a3/drakaina/middleware/gzip.py
+-rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0a3/drakaina/middleware/logging.py
+-rw-r--r--   0        0        0     1138 2023-01-18 00:52:37.644550 drakaina-0.7.0a3/drakaina/middleware/openapi/__init__.py
+-rw-r--r--   0        0        0     1079 2023-04-04 11:19:41.580823 drakaina-0.7.0a3/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12639 2023-05-17 12:11:16.150232 drakaina-0.7.0a3/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0a3/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0    12453 2023-05-17 12:11:16.150232 drakaina-0.7.0a3/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    10527 2023-05-16 19:17:53.349082 drakaina-0.7.0a3/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0a3/drakaina/rsgi.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0a3/drakaina/serializers.py
+-rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0a3/drakaina/tcp.py
+-rw-r--r--   0        0        0     3740 2023-05-17 12:11:16.151231 drakaina-0.7.0a3/drakaina/utils.py
+-rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0a3/drakaina/ws.py
+-rw-r--r--   0        0        0     8181 2023-05-17 12:11:16.152248 drakaina-0.7.0a3/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0a3/LICENSE
+-rw-r--r--   0        0        0     2715 2023-05-17 12:11:16.152248 drakaina-0.7.0a3/pyproject.toml
+-rw-r--r--   0        0        0     5416 2023-05-17 12:11:16.144062 drakaina-0.7.0a3/README.md
+-rw-r--r--   0        0        0     6701 1970-01-01 00:00:00.000000 drakaina-0.7.0a3/setup.py
+-rw-r--r--   0        0        0     6933 1970-01-01 00:00:00.000000 drakaina-0.7.0a3/PKG-INFO
```

### Comparing `drakaina-0.7.0a2/drakaina/__init__.py` & `drakaina-0.7.0a3/drakaina/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/_types.py` & `drakaina-0.7.0a3/drakaina/_types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/asgi.py` & `drakaina-0.7.0a3/drakaina/asgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/client/__init__.py` & `drakaina-0.7.0a3/drakaina/client/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/client/base.py` & `drakaina-0.7.0a3/drakaina/client/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/client/http.py` & `drakaina-0.7.0a3/drakaina/client/http.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/client/tcp.py` & `drakaina-0.7.0a3/drakaina/client/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/client/websocket.py` & `drakaina-0.7.0a3/drakaina/client/websocket.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/contrib/django/__init__.py` & `drakaina-0.7.0a3/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/contrib/django/middleware.py` & `drakaina-0.7.0a3/drakaina/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/contrib/django/views.py` & `drakaina-0.7.0a3/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.0a3/drakaina/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/contrib/jwt/types.py` & `drakaina-0.7.0a3/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.0a3/drakaina/contrib/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/drakaina_openapi.py` & `drakaina-0.7.0a3/drakaina/drakaina_openapi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/exceptions.py` & `drakaina-0.7.0a3/drakaina/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/middleware/base.py` & `drakaina-0.7.0a3/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/middleware/cors.py` & `drakaina-0.7.0a3/drakaina/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/middleware/exception.py` & `drakaina-0.7.0a3/drakaina/middleware/exception.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/middleware/logging.py` & `drakaina-0.7.0a3/drakaina/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/middleware/openapi/__init__.py` & `drakaina-0.7.0a3/drakaina/middleware/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.0a3/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/registries.py` & `drakaina-0.7.0a3/drakaina/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,19 @@
                 param_schema = ParameterSchema(
                     name=parameter.name,
                     kind=parameter.kind,  # noqa
                 )
 
             # Set type
             if parameter.annotation is not Parameter.empty:
-                param_schema.setdefault("type", parameter.annotation.__name__)
+                if isinstance(parameter.annotation, type):
+                    _type = parameter.annotation.__name__
+                else:
+                    _type = parameter.annotation
+                param_schema.setdefault("type", _type)
 
             # Set default value
             if parameter.default is not Parameter.empty:
                 param_schema.setdefault("default", parameter.default)
                 param_schema.setdefault("required", False)
             else:
                 param_schema.setdefault("required", True)
@@ -203,18 +207,19 @@
 
             # Add in method schema
             schema["parameters"].setdefault(parameter.name, param_schema)
 
         # Get return info from signature
         if proc_signature.return_annotation is not Signature.empty:
             # Set return type
-            schema["result"].setdefault(
-                "type",
-                proc_signature.return_annotation.__name__,
-            )
+            if isinstance(proc_signature.return_annotation, type):
+                _type = proc_signature.return_annotation.__name__
+            else:
+                _type = proc_signature.return_annotation
+            schema["result"].setdefault("type", _type)
 
         # Get values from docstring
         if docstring:
             # Return info
             returns = docstring.returns
             if returns and returns.return_name:
                 schema["result"].setdefault("name", returns.return_name)
```

### Comparing `drakaina-0.7.0a2/drakaina/rpc_protocols/base.py` & `drakaina-0.7.0a3/drakaina/rpc_protocols/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/rpc_protocols/jsonrpc20.py` & `drakaina-0.7.0a3/drakaina/rpc_protocols/jsonrpc20.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/serializers.py` & `drakaina-0.7.0a3/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/tcp.py` & `drakaina-0.7.0a3/drakaina/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/utils.py` & `drakaina-0.7.0a3/drakaina/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/drakaina/wsgi.py` & `drakaina-0.7.0a3/drakaina/wsgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/LICENSE` & `drakaina-0.7.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/pyproject.toml` & `drakaina-0.7.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drakaina"
-version = "0.7.0-alpha.2"
+version = "0.7.0-alpha.3"
 description = "Module for simple RPC service implementation"
 authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
 license = "Apache License 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
```

### Comparing `drakaina-0.7.0a2/README.md` & `drakaina-0.7.0a3/README.md`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0a2/setup.py` & `drakaina-0.7.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
            'ujson>=5.7.0,<6.0.0',
            'pyjwt>=2.6.0,<3.0.0',
            'docstring-parser>=0.15,<0.16'],
  'ujson': ['ujson>=5.7.0,<6.0.0']}
 
 setup_kwargs = {
     'name': 'drakaina',
-    'version': '0.7.0a2',
+    'version': '0.7.0a3',
     'description': 'Module for simple RPC service implementation',
     'long_description': '# drakaina\n\n![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}\n\n[![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)\n\n❗ WIP ❗\n\nFramework for simple RPC service implementation.\n\n\n## Quickstart\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina\n```\n\nA minimal Drakaina example is:\n\n```python\nfrom drakaina import remote_procedure\nfrom drakaina.wsgi import WSGIHandler\n\n@remote_procedure("hello")\ndef hello_method(name):\n    return f"Hello, {name}!"\n\n"""\n>>> from drakaina.rpc_protocols import JsonRPCv2\n>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})\n{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}\n"""\n\n# Or define WSGI application\napp = WSGIHandler(route="/jrpc")\n\n```\n\n\n## Features\n\n- Serializers layer.\n  - `json`, `orjson`, `ujson` and `msgpack` serializers.\n- Generates schemas for documentation in OpenRPC format.\n- WSGI protocol implementation\n  - CORS middleware\n  - JWT Authorization middleware.\n  - Compatible with middlewares for others wsgi-frameworks,\n    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),\n    [Flask](https://palletsprojects.com/p/flask/)\n- `login_required` and `check_permissions` decorators.\n\n\n# Documentation\n\n\n## Installation\n\n```shell\npip install drakaina\n```\n\n\n## Middlewares\n\n\n### CORS\n\n\n### JWT\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina[jwt]\n```\n\nExample of using Drakaina:\n\n```python\nfrom functools import partial\nfrom drakaina import check_permissions\nfrom drakaina import ENV_IS_AUTHENTICATED\nfrom drakaina import ENV_USER_ID\nfrom drakaina import login_required\nfrom drakaina import match_any\nfrom drakaina import remote_procedure\nfrom drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware\nfrom drakaina.wsgi import WSGIHandler\n\nimport user_store\n\n\n@login_required\n@remote_procedure(provide_request=True)\ndef my_method(request):\n    assert request[ENV_IS_AUTHENTICATED]\n    return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"\n\n\n@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)\n@remote_procedure\ndef my_method():\n    return "Hello Bro! ✋️"\n\n\ndef get_user(request, payload):\n    user_id = request[ENV_USER_ID] or payload["user_id"]\n    return user_store.get(id=user_id)\n\n\ndef get_jwt_scopes(request, payload):\n    # here `scp` is the key for the scopes value in the token payload\n    return payload.get("scp")\n\n\napp = WSGIHandler(\n    middlewares=[\n        partial(\n            JWTAuthenticationMiddleware,\n            secret_phrase="_secret_",\n            credentials_required=True,\n            auth_scheme="Bearer",\n            # token_getter=custom_implementation_get_token,\n            user_getter=get_user,\n            scopes_getter=get_jwt_scopes,\n            # revoke_checker=is_revoked,\n        )\n    ]\n)\n```\n\nDrakaina may be ran with any WSGI-compliant server,\nsuch as [Gunicorn](http://gunicorn.org).\n\n```shell\ngunicorn main:app\n```\n\nor ran with any ASGI-compliant server\n\n```shell\nuvicorn main:app2\n```\n\n\n### Using with Django\n\nCreate file `rpc_views.py` in your django application.\nDefine function and wrap it `remote_procedure` decorator:\n\n```python\nfrom drakaina import remote_procedure\n\n@remote_procedure\ndef my_method():\n    return "Hello, Django Bro! ✋"\n```\n\nAdd `RPCView` class to urlpatterns. The `as_view` method\nmust accept the `autodiscover` argument as the name of\nthe remote procedure files.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django.views import RPCView\n\nurlpatterns = [\n    ...,\n    path("api/", RPCView.as_view(autodiscover="rpc_views")),\n]\n```\n\n\n### JWT Authentication in your Django project\n\nWrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware\n\nurlpatterns = [\n    ...,\n    path("api/", JWTAuthenticationMiddleware(\n        RPCView.as_view(autodiscover="rpc_views")\n    )),\n]\n```\n\nDefine the parameters in the `settings.py` file.\n\n```python\n...\n\nDRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"\n\n...\n```\n\n\n## License\n\nApache License 2.0\n\n## Artwork\n\n"[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under\n<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).\n',
     'author': 'Aleksey Terentyev',
     'author_email': 'terentyev.a@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tau_lex/drakaina',
```

### Comparing `drakaina-0.7.0a2/PKG-INFO` & `drakaina-0.7.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.0a2
+Version: 0.7.0a3
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
 Requires-Python: >=3.7,<4.0
```

