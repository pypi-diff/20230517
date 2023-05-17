# Comparing `tmp/graphql-api-1.3.6.tar.gz` & `tmp/graphql-api-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.6.tar", last modified: Tue May  9 14:49:41 2023, max compression
+gzip compressed data, was "graphql-api-1.3.7.tar", last modified: Wed May 17 16:15:44 2023, max compression
```

## Comparing `graphql-api-1.3.6.tar` & `graphql-api-1.3.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.141230 graphql-api-1.3.6/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 14:49:31.000000 graphql-api-1.3.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-09 14:49:31.000000 graphql-api-1.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-09 14:49:41.141230 graphql-api-1.3.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-09 14:49:31.000000 graphql-api-1.3.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-09 14:49:40.000000 graphql-api-1.3.6/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.135230 graphql-api-1.3.6/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    24096 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     4155 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.137230 graphql-api-1.3.6/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-09 14:49:41.141230 graphql-api-1.3.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-09 14:49:31.000000 graphql-api-1.3.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.141230 graphql-api-1.3.6/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5704 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_dataclass.py
--rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.513540 graphql-api-1.3.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-17 16:15:34.000000 graphql-api-1.3.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-17 16:15:34.000000 graphql-api-1.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 16:15:44.513540 graphql-api-1.3.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-17 16:15:34.000000 graphql-api-1.3.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-17 16:15:43.000000 graphql-api-1.3.7/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.507540 graphql-api-1.3.7/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    24330 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3069 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     4155 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.509540 graphql-api-1.3.7/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      830 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-17 16:15:44.513540 graphql-api-1.3.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-17 16:15:34.000000 graphql-api-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.512540 graphql-api-1.3.7/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5704 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_dataclass.py
+-rwxrwxrwx   0 root         (0) root         (0)     6125 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4024 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.6/LICENSE` & `graphql-api-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/PKG-INFO` & `graphql-api-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.6
+Version: 1.3.7
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.6/graphql-api-v1.3.6.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.7/graphql-api-v1.3.7.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.6/README.md` & `graphql-api-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/api.py` & `graphql-api-1.3.7/graphql_api/api.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/context.py` & `graphql-api-1.3.7/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.7/graphql_api/dataclass_mapping.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/error.py` & `graphql-api-1.3.7/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/executor.py` & `graphql-api-1.3.7/graphql_api/executor.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/mapper.py` & `graphql-api-1.3.7/graphql_api/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
     error_protection = "ERROR_PROTECTION"
 
 
 class GraphQLMutableField(GraphQLField):
     pass
 
 
+class GraphQLGenericEnum(enum.Enum):
+    pass
+
+
 class GraphQLTypeMapper:
     def __init__(
         self,
         as_mutable=False,
         as_input=False,
         registry=None,
         reverse_registry=None,
@@ -294,16 +298,19 @@
         return self.map(_type)
 
     # noinspection PyMethodMayBeStatic
     def map_to_enum(self, type_: Type[enum.Enum]) -> GraphQLEnumType:
         enum_type = type_
         name = f"{type_.__name__}Enum"
         # Enums don't include a suffix as they are immutable
+        description = to_camel_case_text(inspect.getdoc(type_))
+        default_description = to_camel_case_text(inspect.getdoc(GraphQLGenericEnum))
 
-        description = to_camel_case_text(inspect.getdoc(enum_type))
+        if not description or description == default_description:
+            description = f"A {name}."
 
         enum_type = GraphQLMappedEnumType(
             name=name, values=enum_type, description=description
         )
 
         enum_type.enum_type = type_
```

### Comparing `graphql-api-1.3.6/graphql_api/middleware.py` & `graphql-api-1.3.7/graphql_api/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     if return_type and isinstance(return_type, GraphQLNonNull):
         return_type = return_type.of_type
 
     kwargs = {}
     if return_type and isinstance(return_type, GraphQLObjectType):
         sub_loc = info.field_nodes[0].selection_set.loc
-        kwargs["query"] = sub_loc.source.body[sub_loc.start : sub_loc.end]
+        kwargs["query"] = sub_loc.source.body[sub_loc.start: sub_loc.end]
 
     info.context.field = GraphQLFieldContext(meta=field_meta, **kwargs)
 
     try:
         value = next()
     finally:
         info.context.field = None
```

### Comparing `graphql-api-1.3.6/graphql_api/reduce.py` & `graphql-api-1.3.7/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/relay.py` & `graphql-api-1.3.7/graphql_api/relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/remote.py` & `graphql-api-1.3.7/graphql_api/remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/types.py` & `graphql-api-1.3.7/graphql_api/types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api/utils.py` & `graphql-api-1.3.7/graphql_api/utils.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.7/graphql_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.6
+Version: 1.3.7
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.6/graphql-api-v1.3.6.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.7/graphql-api-v1.3.7.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.6/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.7/graphql_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/setup.py` & `graphql-api-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/tests/test_custom_types.py` & `graphql-api-1.3.7/tests/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/tests/test_dataclass.py` & `graphql-api-1.3.7/tests/test_dataclass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, List
 from graphql_api.api import GraphQLAPI
 
 
 class TestDataclass:
     def test_dataclass(self):
         api = GraphQLAPI()
 
@@ -29,28 +29,36 @@
         assert not result.errors
         assert result.data == expected
 
     def test_dataclas_inheritance(self):
         api = GraphQLAPI()
 
         @dataclass
-        class Person:
+        class Entity:
             name: str
+            embedding: List[float]
+
+        @dataclass
+        class Person(Entity):
+            name: str
+            embedding: List[float]
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         @dataclass
         class Root:
             person: Person
 
-        executor = api.executor(root_value=Root(person=Person(name="rob")))
+        executor = api.executor(
+            root_value=Root(person=Person(name="rob", embedding=[1, 2]))
+        )
 
         test_query = """
             query {
-                person { name }
+                person { name, embedding }
             }
         """
 
         result = executor.execute(test_query)
 
         assert not result.errors
-        assert result.data == {"person": {"name": "rob"}}
+        assert result.data == {"person": {"name": "rob", "embedding": [1, 2]}}
```

### Comparing `graphql-api-1.3.6/tests/test_docstrings.py` & `graphql-api-1.3.7/tests/test_docstrings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from enum import Enum
 from typing import Optional
 
 from graphql_api.api import GraphQLAPI
 
 
 class TestGraphQL:
     def test_basic_docstring(self):
@@ -45,14 +46,49 @@
 
         assert root_field_type.description == "NODE_DOCSTRING"
 
         node_field = root_field_type.fields["nodeField"]
 
         assert node_field.description == "NODE_FIELD_DOCSTRING"
 
+    def test_enum_docstring(self):
+        api = GraphQLAPI()
+
+        class TestEnumA(Enum):
+            VALUE_A = "value_a"
+            VALUE_B = "value_b"
+
+        class TestEnumB(Enum):
+            """
+            TEST_ENUM_B_DOCSTRING
+            """
+
+            VALUE_A = "value_a"
+            VALUE_B = "value_b"
+
+        @api.type(root=True)
+        class Root:
+            @api.field
+            def enum_field_a(self) -> TestEnumA:
+                return TestEnumA.VALUE_A
+
+            @api.field
+            def enum_field_b(self) -> TestEnumB:
+                return TestEnumB.VALUE_A
+
+        schema = api.graphql_schema()[0]
+
+        enum_field = schema.query_type.fields["enumFieldA"]
+
+        assert enum_field.type.of_type.description == "A TestEnumAEnum."
+
+        enum_field_b = schema.query_type.fields["enumFieldB"]
+
+        assert enum_field_b.type.of_type.description == "TEST_ENUM_B_DOCSTRING"
+
     def test_basic_dataclass_docstring(self):
         api = GraphQLAPI()
 
         @dataclass
         class Node:
             """
             NODE_DOCSTRING
```

### Comparing `graphql-api-1.3.6/tests/test_error.py` & `graphql-api-1.3.7/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/tests/test_filtering.py` & `graphql-api-1.3.7/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/tests/test_graphql.py` & `graphql-api-1.3.7/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/tests/test_relay.py` & `graphql-api-1.3.7/tests/test_relay.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,23 @@
                         self.has_previous_page = True
 
                 if self._before is not None:
                     end_index = cursors.index(self._before)
                     if end_index < len(cursors) - 1:
                         self.has_next_page = True
 
-                self.filtered_cursors = cursors[start_index : end_index + 1]
+                self.filtered_cursors = cursors[start_index: end_index + 1]
 
                 self.people = people
 
                 if self._first is not None:
                     self.filtered_cursors = self.filtered_cursors[: self._first]
 
                 elif self._last is not None:
-                    self.filtered_cursors = self.filtered_cursors[-self._last :]
+                    self.filtered_cursors = self.filtered_cursors[-self._last:]
 
             @api.field
             def edges(self) -> List[Edge]:
                 return [
                     Edge(cursor=cursor, node=self.people[cursor])
                     for cursor in self.filtered_cursors
                 ]
```

### Comparing `graphql-api-1.3.6/tests/test_remote.py` & `graphql-api-1.3.7/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/tests/test_schema.py` & `graphql-api-1.3.7/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.6/tests/test_subscriptions.py` & `graphql-api-1.3.7/tests/test_subscriptions.py`

 * *Files identical despite different names*

