# Comparing `tmp/graphql-api-1.3.7.tar.gz` & `tmp/graphql-api-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.7.tar", last modified: Wed May 17 16:15:44 2023, max compression
+gzip compressed data, was "graphql-api-1.3.8.tar", last modified: Wed May 17 19:27:46 2023, max compression
```

## Comparing `graphql-api-1.3.7.tar` & `graphql-api-1.3.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.513540 graphql-api-1.3.7/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-17 16:15:34.000000 graphql-api-1.3.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-17 16:15:34.000000 graphql-api-1.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 16:15:44.513540 graphql-api-1.3.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-17 16:15:34.000000 graphql-api-1.3.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-17 16:15:43.000000 graphql-api-1.3.7/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.507540 graphql-api-1.3.7/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    24330 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3069 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     4155 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-17 16:15:34.000000 graphql-api-1.3.7/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.509540 graphql-api-1.3.7/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-17 16:15:44.000000 graphql-api-1.3.7/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-17 16:15:44.513540 graphql-api-1.3.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-17 16:15:34.000000 graphql-api-1.3.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:15:44.512540 graphql-api-1.3.7/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5704 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_dataclass.py
--rwxrwxrwx   0 root         (0) root         (0)     6125 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4024 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-17 16:15:34.000000 graphql-api-1.3.7/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.313406 graphql-api-1.3.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-17 19:27:38.000000 graphql-api-1.3.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-17 19:27:38.000000 graphql-api-1.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 19:27:46.313406 graphql-api-1.3.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-17 19:27:38.000000 graphql-api-1.3.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-17 19:27:45.000000 graphql-api-1.3.8/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.310406 graphql-api-1.3.8/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    24330 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     4155 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-17 19:27:38.000000 graphql-api-1.3.8/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.311406 graphql-api-1.3.8/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      830 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-17 19:27:46.000000 graphql-api-1.3.8/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-17 19:27:46.314406 graphql-api-1.3.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-17 19:27:38.000000 graphql-api-1.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 19:27:46.313406 graphql-api-1.3.8/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5704 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_dataclass.py
+-rwxrwxrwx   0 root         (0) root         (0)     6125 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-17 19:27:38.000000 graphql-api-1.3.8/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.7/LICENSE` & `graphql-api-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/PKG-INFO` & `graphql-api-1.3.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.7
+Version: 1.3.8
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.7/graphql-api-v1.3.7.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.8/graphql-api-v1.3.8.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.7/README.md` & `graphql-api-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/api.py` & `graphql-api-1.3.8/graphql_api/api.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/context.py` & `graphql-api-1.3.8/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.8/graphql_api/dataclass_mapping.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/error.py` & `graphql-api-1.3.8/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/executor.py` & `graphql-api-1.3.8/graphql_api/executor.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/mapper.py` & `graphql-api-1.3.8/graphql_api/mapper.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/middleware.py` & `graphql-api-1.3.8/graphql_api/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     if return_type and isinstance(return_type, GraphQLNonNull):
         return_type = return_type.of_type
 
     kwargs = {}
     if return_type and isinstance(return_type, GraphQLObjectType):
         sub_loc = info.field_nodes[0].selection_set.loc
-        kwargs["query"] = sub_loc.source.body[sub_loc.start: sub_loc.end]
+        kwargs["query"] = sub_loc.source.body[sub_loc.start : sub_loc.end]
 
     info.context.field = GraphQLFieldContext(meta=field_meta, **kwargs)
 
     try:
         value = next()
     finally:
         info.context.field = None
```

### Comparing `graphql-api-1.3.7/graphql_api/reduce.py` & `graphql-api-1.3.8/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/relay.py` & `graphql-api-1.3.8/graphql_api/relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/remote.py` & `graphql-api-1.3.8/graphql_api/remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/types.py` & `graphql-api-1.3.8/graphql_api/types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/graphql_api/utils.py` & `graphql-api-1.3.8/graphql_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,11 +199,10 @@
 
         else:
             raise AttributeError(f"Invalid HTTP method {http_method}")
 
         try:
             json = await r.json(content_type=None)
         except JSONDecodeError as e:
-            raise ValueError(
-                f"{e}, unable to decode JSON from response: `{str(r.text())}`"
-            )
+            text = await r.text()
+            raise ValueError(f"{e}, unable to decode JSON from response: `{str(text)}`")
     return json
```

### Comparing `graphql-api-1.3.7/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.8/graphql_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.7
+Version: 1.3.8
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.7/graphql-api-v1.3.7.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.8/graphql-api-v1.3.8.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.7/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.8/graphql_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/setup.py` & `graphql-api-1.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_custom_types.py` & `graphql-api-1.3.8/tests/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_dataclass.py` & `graphql-api-1.3.8/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_docstrings.py` & `graphql-api-1.3.8/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_error.py` & `graphql-api-1.3.8/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_filtering.py` & `graphql-api-1.3.8/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_graphql.py` & `graphql-api-1.3.8/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_relay.py` & `graphql-api-1.3.8/tests/test_relay.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,23 @@
                         self.has_previous_page = True
 
                 if self._before is not None:
                     end_index = cursors.index(self._before)
                     if end_index < len(cursors) - 1:
                         self.has_next_page = True
 
-                self.filtered_cursors = cursors[start_index: end_index + 1]
+                self.filtered_cursors = cursors[start_index : end_index + 1]
 
                 self.people = people
 
                 if self._first is not None:
                     self.filtered_cursors = self.filtered_cursors[: self._first]
 
                 elif self._last is not None:
-                    self.filtered_cursors = self.filtered_cursors[-self._last:]
+                    self.filtered_cursors = self.filtered_cursors[-self._last :]
 
             @api.field
             def edges(self) -> List[Edge]:
                 return [
                     Edge(cursor=cursor, node=self.people[cursor])
                     for cursor in self.filtered_cursors
                 ]
```

### Comparing `graphql-api-1.3.7/tests/test_remote.py` & `graphql-api-1.3.8/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_schema.py` & `graphql-api-1.3.8/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.7/tests/test_subscriptions.py` & `graphql-api-1.3.8/tests/test_subscriptions.py`

 * *Files identical despite different names*

