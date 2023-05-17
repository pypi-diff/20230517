# Comparing `tmp/flask_ninja-1.2.1.tar.gz` & `tmp/flask_ninja-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_ninja-1.2.1.tar", max compression
+gzip compressed data, was "flask_ninja-1.2.2.tar", max compression
```

## Comparing `flask_ninja-1.2.1.tar` & `flask_ninja-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2238 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/README.md
--rw-r--r--   0        0        0      315 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/__init__.py
--rw-r--r--   0        0        0     4574 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/api.py
--rw-r--r--   0        0        0      587 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/constants.py
--rw-r--r--   0        0        0    10505 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/models.py
--rw-r--r--   0        0        0    15253 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/operation.py
--rw-r--r--   0        0        0     7612 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/param.py
--rw-r--r--   0        0        0     3156 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/param_functions.py
--rw-r--r--   0        0        0     1728 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/parse_rule.py
--rw-r--r--   0        0        0        0 2023-04-03 09:12:51.213979 flask_ninja-1.2.1/flask_ninja/py.typed
--rw-r--r--   0        0        0     2480 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/router.py
--rw-r--r--   0        0        0     1103 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/security.py
--rw-r--r--   0        0        0      173 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/README.md
--rw-r--r--   0        0        0      665 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/favicon-16x16.png
--rw-r--r--   0        0        0      628 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/favicon-32x32.png
--rw-r--r--   0        0        0     1825 2023-04-03 09:12:32.877568 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/index.j2
--rw-r--r--   0        0        0        0 2023-04-03 09:12:51.213979 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/py.typed
--rw-r--r--   0        0        0  1096189 2023-04-03 09:12:32.885568 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/swagger-ui-bundle.js
--rw-r--r--   0        0        0   339541 2023-04-03 09:12:32.885568 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/swagger-ui-standalone-preset.js
--rw-r--r--   0        0        0   143981 2023-04-03 09:12:32.885568 flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/swagger-ui.css
--rw-r--r--   0        0        0      247 2023-04-03 09:12:32.885568 flask_ninja-1.2.1/flask_ninja/swagger_ui.py
--rw-r--r--   0        0        0     4768 2023-04-03 09:12:32.885568 flask_ninja-1.2.1/flask_ninja/utils.py
--rw-r--r--   0        0        0     2283 2023-04-03 09:12:32.885568 flask_ninja-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 flask_ninja-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2238 2023-05-17 13:01:37.025002 flask_ninja-1.2.2/README.md
+-rw-r--r--   0        0        0      315 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/__init__.py
+-rw-r--r--   0        0        0     4574 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/api.py
+-rw-r--r--   0        0        0      587 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/constants.py
+-rw-r--r--   0        0        0    10505 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/models.py
+-rw-r--r--   0        0        0    15539 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/operation.py
+-rw-r--r--   0        0        0     7612 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/param.py
+-rw-r--r--   0        0        0     3156 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/param_functions.py
+-rw-r--r--   0        0        0     1728 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/parse_rule.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:01:57.260825 flask_ninja-1.2.2/flask_ninja/py.typed
+-rw-r--r--   0        0        0     2480 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/router.py
+-rw-r--r--   0        0        0     1103 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/security.py
+-rw-r--r--   0        0        0      173 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/README.md
+-rw-r--r--   0        0        0      665 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/favicon-16x16.png
+-rw-r--r--   0        0        0      628 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/favicon-32x32.png
+-rw-r--r--   0        0        0     1825 2023-05-17 13:01:37.029002 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/index.j2
+-rw-r--r--   0        0        0        0 2023-05-17 13:01:57.260825 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/py.typed
+-rw-r--r--   0        0        0  1096189 2023-05-17 13:01:37.033002 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   339541 2023-05-17 13:01:37.037001 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/swagger-ui-standalone-preset.js
+-rw-r--r--   0        0        0   143981 2023-05-17 13:01:37.037001 flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/swagger-ui.css
+-rw-r--r--   0        0        0      247 2023-05-17 13:01:37.037001 flask_ninja-1.2.2/flask_ninja/swagger_ui.py
+-rw-r--r--   0        0        0     5593 2023-05-17 13:01:37.037001 flask_ninja-1.2.2/flask_ninja/utils.py
+-rw-r--r--   0        0        0     2283 2023-05-17 13:01:37.037001 flask_ninja-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 flask_ninja-1.2.2/PKG-INFO
```

### Comparing `flask_ninja-1.2.1/README.md` & `flask_ninja-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/api.py` & `flask_ninja-1.2.2/flask_ninja/api.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/constants.py` & `flask_ninja-1.2.2/flask_ninja/constants.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/models.py` & `flask_ninja-1.2.2/flask_ninja/models.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/operation.py` & `flask_ninja-1.2.2/flask_ninja/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     RequestBody,
     Response,
     Schema,
 )
 from .param import FuncParam
 from .parse_rule import parse_rule
 from .security import HttpAuthBase
-from .utils import create_model_field, get_param_model_field
+from .utils import create_model_field, get_param_model_field, is_scalar_sequence_field
 
 ModelNameMapType = dict[Union[Type[BaseModel], Type[Enum]], str]
 
 
 class SerializationModel(BaseModel):
     data: Any
 
@@ -83,17 +83,22 @@
             return jsonify("Unauthorized"), 401
 
         try:
             for param in self.params:
                 # Parse query params
                 field_info = cast(FuncParam, param.field_info)
                 if field_info.in_ == ParamType.QUERY and param.name in request.args:
-                    kwargs[param.name] = parse_obj_as(
-                        param.type_, request.args[param.alias]
-                    )
+                    if is_scalar_sequence_field(param):
+                        kwargs[param.name] = parse_obj_as(
+                            param.outer_type_, request.args.getlist(param.alias)
+                        )
+                    else:
+                        kwargs[param.name] = parse_obj_as(
+                            param.type_, request.args[param.alias]
+                        )
                 elif field_info.in_ == ParamType.HEADER:
                     kwargs[param.name] = parse_obj_as(
                         param.type_, request.headers.get(param.alias)
                     )
                 # Parse request body
                 elif field_info.in_ == ParamType.BODY:
                     kwargs[param.name] = parse_obj_as(param.outer_type_, request.json)
```

### Comparing `flask_ninja-1.2.1/flask_ninja/param.py` & `flask_ninja-1.2.2/flask_ninja/param.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/param_functions.py` & `flask_ninja-1.2.2/flask_ninja/param_functions.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/parse_rule.py` & `flask_ninja-1.2.2/flask_ninja/parse_rule.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/router.py` & `flask_ninja-1.2.2/flask_ninja/router.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/security.py` & `flask_ninja-1.2.2/flask_ninja/security.py`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/favicon-16x16.png` & `flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/favicon-32x32.png` & `flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/index.j2` & `flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/index.j2`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/swagger-ui-bundle.js` & `flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/swagger-ui-standalone-preset.js` & `flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/swagger-ui-4.12.0/swagger-ui.css` & `flask_ninja-1.2.2/flask_ninja/swagger-ui-4.12.0/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask_ninja-1.2.1/flask_ninja/utils.py` & `flask_ninja-1.2.2/flask_ninja/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,41 @@
 import inspect
 from enum import Enum
 from typing import Any, Dict, Optional, Set, Type, Union
 
 from pydantic import BaseConfig, BaseModel
 from pydantic.class_validators import Validator
 from pydantic.fields import (
+    SHAPE_FROZENSET,
+    SHAPE_LIST,
+    SHAPE_SEQUENCE,
+    SHAPE_SET,
     SHAPE_SINGLETON,
+    SHAPE_TUPLE,
+    SHAPE_TUPLE_ELLIPSIS,
     FieldInfo,
     ModelField,
     Required,
     Undefined,
     UndefinedType,
 )
 from pydantic.schema import model_process_schema
 from pydantic.utils import lenient_issubclass
 
 from flask_ninja.constants import REF_PREFIX, ApiConfigError
-from flask_ninja.param import FuncParam, ParamType
+from flask_ninja.param import FuncParam, Header, ParamType, Query
 
+sequence_shapes = {
+    SHAPE_LIST,
+    SHAPE_SET,
+    SHAPE_FROZENSET,
+    SHAPE_TUPLE,
+    SHAPE_SEQUENCE,
+    SHAPE_TUPLE_ELLIPSIS,
+}
 sequence_types = (list, set, tuple)
 
 
 def create_model_field(
     name: str,
     type_: Type[Any],
     class_validators: Optional[Dict[str, Validator]] = None,
@@ -59,14 +73,28 @@
     if field.sub_fields:
         if not all(is_scalar_field(f) for f in field.sub_fields):
             return False
 
     return True
 
 
+def is_scalar_sequence_field(field: ModelField) -> bool:
+    if (field.shape in sequence_shapes) and not lenient_issubclass(
+        field.type_, BaseModel
+    ):
+        if field.sub_fields is not None:
+            for sub_field in field.sub_fields:
+                if not is_scalar_field(sub_field):
+                    return False
+        return True
+    if lenient_issubclass(field.type_, sequence_types):
+        return True
+    return False
+
+
 def get_model_definitions(
     flat_models: Set[Union[Type[BaseModel], Type[Enum]]],
     model_name_map: Dict[Union[Type[BaseModel], Type[Enum]], str],
 ) -> Dict[str, Any]:
     definitions: Dict[str, Dict[str, Any]] = {}
     for model in flat_models:
         m_schema, m_definitions, _ = model_process_schema(
@@ -144,13 +172,15 @@
 
     if getattr(field.field_info, "in_", None) is None:
         if is_scalar_field(field):
             field.field_info.in_ = ParamType.QUERY  # type:ignore
         else:
             field.field_info.in_ = ParamType.BODY  # type:ignore
 
+    if isinstance(param.default, (Query, Header)) and is_scalar_sequence_field(field):
+        return field
     if field.field_info.in_ != ParamType.BODY and not is_scalar_field(  # type:ignore
         field
     ):
         raise ApiConfigError("Path param must be of a simple type.")
 
     return field
```

### Comparing `flask_ninja-1.2.1/pyproject.toml` & `flask_ninja-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-ninja"
-version = "1.2.1"
+version = "1.2.2"
 description = "Flask Ninja is a web framework for building APIs with Flask and Python 3.9+ type hints."
 readme = "README.md"
 authors = ["Michal Korbela <michal.korbela@kiwi.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Flask = ">=1.1.2"
```

### Comparing `flask_ninja-1.2.1/PKG-INFO` & `flask_ninja-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ninja
-Version: 1.2.1
+Version: 1.2.2
 Summary: Flask Ninja is a web framework for building APIs with Flask and Python 3.9+ type hints.
 Author: Michal Korbela
 Author-email: michal.korbela@kiwi.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

