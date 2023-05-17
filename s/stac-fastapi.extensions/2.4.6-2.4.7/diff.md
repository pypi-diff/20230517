# Comparing `tmp/stac-fastapi.extensions-2.4.6.tar.gz` & `tmp/stac-fastapi.extensions-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.extensions-2.4.6.tar", last modified: Wed May 10 15:53:08 2023, max compression
+gzip compressed data, was "stac-fastapi.extensions-2.4.7.tar", last modified: Wed May 17 15:30:44 2023, max compression
```

## Comparing `stac-fastapi.extensions-2.4.6.tar` & `stac-fastapi.extensions-2.4.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 15:53:08.086403 stac-fastapi.extensions-2.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 15:53:08.086403 stac-fastapi.extensions-2.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/token_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 15:30:44.968150 stac-fastapi.extensions-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/token_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/top_level.txt
```

### Comparing `stac-fastapi.extensions-2.4.6/PKG-INFO` & `stac-fastapi.extensions-2.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
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

### Comparing `stac-fastapi.extensions-2.4.6/setup.py` & `stac-fastapi.extensions-2.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/__init__.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/context.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""context extension."""
+"""Context extension."""
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
 
 
 @attr.s
 class ContextExtension(ApiExtension):
     """Context Extension.
 
-    The Context extension adds a JSON object to ItemCollection responses (`/search`, `/collections/{collection_id}/items`)
-    which includes the number of items matched, returned, and the limit requested.
-
+    The Context extension adds a JSON object to ItemCollection responses (`/search`,
+    `/collections/{collection_id}/items`) which includes the number of items matched,
+    returned, and the limit requested.
     https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#context
     """
 
     conformance_classes: List[str] = attr.ib(
         factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#context"]
     )
     schema_href: Optional[str] = attr.ib(
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/fields.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-"""fields extension."""
+"""Fields extension."""
 from typing import List, Optional, Set
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
 
 from .request import FieldsExtensionGetRequest, FieldsExtensionPostRequest
 
 
 @attr.s
 class FieldsExtension(ApiExtension):
     """Fields Extension.
 
-    The Fields extension adds functionality to the `/search` endpoint which allows the caller to include or exclude
-    specific from the API response.  Registering this extension with the application has the added effect of removing
-    the `ItemCollection` response model from the `/search` endpoint, as the Fields extension allows the API to return
-    potentially invalid responses by excluding fields which are required by the STAC spec, such as geometry.
+    The Fields extension adds functionality to the `/search` endpoint which
+    allows the caller to include or exclude specific from the API response.
+    Registering this extension with the application has the added effect of
+    removing the `ItemCollection` response model from the `/search` endpoint, as
+    the Fields extension allows the API to return potentially invalid responses
+    by excluding fields which are required by the STAC spec, such as geometry.
 
     https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#fields
 
     Attributes:
         default_includes (set): defines the default set of included fields.
-        conformance_classes (list): Defines the list of conformance classes for the extension
-
+        conformance_classes (list): Defines the list of conformance classes for
+            the extension
     """
 
     GET = FieldsExtensionGetRequest
     POST = FieldsExtensionPostRequest
 
     conformance_classes: List[str] = attr.ib(
         factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#fields"]
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/request.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     include: Optional[Set[str]] = set()
     exclude: Optional[Set[str]] = set()
 
     @staticmethod
     def _get_field_dict(fields: Optional[Set[str]]) -> Dict:
         """Pydantic include/excludes notation.
 
-        Internal method to create a dictionary for advanced include or exclude of pydantic fields on model export
+        Internal method to create a dictionary for advanced include or exclude
+        of pydantic fields on model export
         Ref: https://pydantic-docs.helpmanual.io/usage/exporting_models/#advanced-include-and-exclude
         """
         field_dict = {}
         for field in fields or []:
             if "." in field:
                 parent, key = field.split(".")
                 if parent not in field_dict:
@@ -40,16 +41,16 @@
                 field_dict[field] = ...  # type:ignore
         return field_dict
 
     @property
     def filter_fields(self) -> Dict:
         """Create pydantic include/exclude expression.
 
-        Create dictionary of fields to include/exclude on model export based on the included and excluded fields passed
-        to the API
+        Create dictionary of fields to include/exclude on model export based on
+        the included and excluded fields passed to the API
         Ref: https://pydantic-docs.helpmanual.io/usage/exporting_models/#advanced-include-and-exclude
         """
         # Always include default_includes, even if they
         # exist in the exclude list.
         include = (self.include or set()) - (self.exclude or set())
         include |= Settings.get().default_includes or set()
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/filter.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 from .request import FilterExtensionGetRequest, FilterExtensionPostRequest
 
 
 class FilterConformanceClasses(str, Enum):
     """Conformance classes for the Filter extension.
 
-    See https://github.com/radiantearth/stac-api-spec/tree/v1.0.0-rc.1/fragments/filter
+    See
+    https://github.com/radiantearth/stac-api-spec/tree/v1.0.0-rc.1/fragments/filter
     """
 
     FILTER = "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/filter"
     FEATURES_FILTER = (
         "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/features-filter"
     )
     ITEM_SEARCH_FILTER = "https://api.stacspec.org/v1.0.0-rc.1/item-search#filter"
@@ -46,25 +47,25 @@
     )
 
 
 @attr.s
 class FilterExtension(ApiExtension):
     """Filter Extension.
 
-    The filter extension adds several endpoints which allow the retrieval of queryables and
-    provides an expressive mechanism for searching based on Item Attributes:
+    The filter extension adds several endpoints which allow the retrieval of
+    queryables and provides an expressive mechanism for searching based on Item
+    Attributes:
         GET /queryables
         GET /collections/{collection_id}/queryables
 
     https://github.com/radiantearth/stac-api-spec/blob/master/fragments/filter/README.md
 
     Attributes:
         client: Queryables endpoint logic
         conformance_classes: Conformance classes provided by the extension
-
     """
 
     GET = FilterExtensionGetRequest
     POST = FilterExtensionPostRequest
 
     client: Union[AsyncBaseFiltersClient, BaseFiltersClient] = attr.ib(
         factory=BaseFiltersClient
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/request.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 from stac_fastapi.types.search import APIRequest
 
 
 class FilterLang(str, Enum):
     """Choices for filter-lang value in a POST request.
 
-    Based on https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
+    Based on
+    https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
 
     Note the addition of cql2-json, which is used by the pgstac backend,
     but is not included in the spec above.
     """
 
     cql_json = "cql-json"
     cql2_json = "cql2-json"
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/pagination.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/pagination.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from stac_fastapi.types.extension import ApiExtension
 
 
 @attr.s
 class PaginationExtension(ApiExtension):
     """Token Pagination.
 
-    Though not strictly an extension, the chosen pagination will modify the
-    form of the request object. By making pagination an extension class, we can
-    use create_request_model to dynamically add the correct pagination parameter
-    to the request model for OpenAPI generation.
+    Though not strictly an extension, the chosen pagination will modify the form of the
+    request object. By making pagination an extension class, we can use
+    create_request_model to dynamically add the correct pagination parameter to the
+    request model for OpenAPI generation.
     """
 
     GET = GETPagination
     POST = POSTPagination
 
     conformance_classes: List[str] = attr.ib(factory=list)
     schema_href: Optional[str] = attr.ib(default=None)
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/token_pagination.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/token_pagination.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from stac_fastapi.types.extension import ApiExtension
 
 
 @attr.s
 class TokenPaginationExtension(ApiExtension):
     """Token Pagination.
 
-    Though not strictly an extension, the chosen pagination will modify the
-    form of the request object. By making pagination an extension class, we can
-    use create_request_model to dynamically add the correct pagination parameter
-    to the request model for OpenAPI generation.
+    Though not strictly an extension, the chosen pagination will modify the form of the
+    request object. By making pagination an extension class, we can use
+    create_request_model to dynamically add the correct pagination parameter to the
+    request model for OpenAPI generation.
     """
 
     GET = GETTokenPagination
     POST = POSTTokenPagination
 
     conformance_classes: List[str] = attr.ib(factory=list)
     schema_href: Optional[str] = attr.ib(default=None)
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/query.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/sort.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""query extension."""
+"""Sort extension."""
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
 
-from .request import QueryExtensionGetRequest, QueryExtensionPostRequest
+from .request import SortExtensionGetRequest, SortExtensionPostRequest
 
 
 @attr.s
-class QueryExtension(ApiExtension):
-    """Query Extension.
+class SortExtension(ApiExtension):
+    """Sort Extension.
 
-    The Query extension adds an additional `query` parameter to `/search` requests which allows the caller to perform
-    queries against item metadata (ex. find all images with cloud cover less than 15%).
-
-    https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#query
+    The Sort extension adds the `sortby` parameter to the `/search` endpoint, allowing the
+    caller to specify the sort order of the returned items.
+    https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#sort
     """
 
-    GET = QueryExtensionGetRequest
-    POST = QueryExtensionPostRequest
+    GET = SortExtensionGetRequest
+    POST = SortExtensionPostRequest
 
     conformance_classes: List[str] = attr.ib(
-        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#query"]
+        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#sort"]
     )
     schema_href: Optional[str] = attr.ib(default=None)
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/request.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/sort.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""sort extension."""
+"""Query extension."""
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
 
-from .request import SortExtensionGetRequest, SortExtensionPostRequest
+from .request import QueryExtensionGetRequest, QueryExtensionPostRequest
 
 
 @attr.s
-class SortExtension(ApiExtension):
-    """Sort Extension.
+class QueryExtension(ApiExtension):
+    """Query Extension.
 
-    The Sort extension adds the `sortby` parameter to the `/search` endpoint, allowing the caller to specify the sort
-    order of the returned items.
-
-    https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#sort
+    The Query extension adds an additional `query` parameter to `/search` requests which
+    allows the caller to perform queries against item metadata (ex. find all images with
+    cloud cover less than 15%).
+    https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#query
     """
 
-    GET = SortExtensionGetRequest
-    POST = SortExtensionPostRequest
+    GET = QueryExtensionGetRequest
+    POST = QueryExtensionPostRequest
 
     conformance_classes: List[str] = attr.ib(
-        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#sort"]
+        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#query"]
     )
     schema_href: Optional[str] = attr.ib(default=None)
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/transaction.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""transaction extension."""
+"""Transaction extension."""
 from typing import List, Optional, Type, Union
 
 import attr
 from fastapi import APIRouter, Body, FastAPI
 from stac_pydantic import Collection, Item
 from starlette.responses import JSONResponse, Response
 
@@ -14,30 +14,32 @@
 from stac_fastapi.types.extension import ApiExtension
 
 
 @attr.s
 class PostItem(CollectionUri):
     """Create Item."""
 
-    item: stac_types.Item = attr.ib(default=Body(None))
+    item: Union[stac_types.Item, stac_types.ItemCollection] = attr.ib(
+        default=Body(None)
+    )
 
 
 @attr.s
 class PutItem(ItemUri):
     """Update Item."""
 
     item: stac_types.Item = attr.ib(default=Body(None))
 
 
 @attr.s
 class TransactionExtension(ApiExtension):
     """Transaction Extension.
 
-    The transaction extension adds several endpoints which allow the creation, deletion, and updating of items and
-    collections:
+    The transaction extension adds several endpoints which allow the creation,
+    deletion, and updating of items and collections:
         POST /collections
         PUT /collections/{collection_id}
         DELETE /collections/{collection_id}
         POST /collections/{collection_id}/items
         PUT /collections/{collection_id}/items
         DELETE /collections/{collection_id}/items
 
@@ -69,28 +71,30 @@
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=create_async_endpoint(self.client.create_item, PostItem),
         )
 
     def register_update_item(self):
-        """Register update item endpoint (PUT /collections/{collection_id}/items/{item_id})."""
+        """Register update item endpoint (PUT
+        /collections/{collection_id}/items/{item_id})."""
         self.router.add_api_route(
             name="Update Item",
             path="/collections/{collection_id}/items/{item_id}",
             response_model=Item if self.settings.enable_response_models else None,
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["PUT"],
             endpoint=create_async_endpoint(self.client.update_item, PutItem),
         )
 
     def register_delete_item(self):
-        """Register delete item endpoint (DELETE /collections/{collection_id}/items/{item_id})."""
+        """Register delete item endpoint (DELETE
+        /collections/{collection_id}/items/{item_id})."""
         self.router.add_api_route(
             name="Delete Item",
             path="/collections/{collection_id}/items/{item_id}",
             response_model=Item if self.settings.enable_response_models else None,
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/bulk_transactions.py` & `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/bulk_transactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""bulk transactions extension."""
+"""Bulk transactions extension."""
 import abc
 from typing import Any, Dict, List, Optional, Union
 
 import attr
 from fastapi import APIRouter, FastAPI
 from pydantic import BaseModel
 
@@ -42,15 +42,14 @@
 
         Args:
             items: list of items.
             chunk_size: number of items processed at a time.
 
         Returns:
             Message indicating the status of the insert.
-
         """
         raise NotImplementedError
 
 
 @attr.s  # type: ignore
 class AsyncBaseBulkTransactionsClient(abc.ABC):
     """BulkTransactionsClient."""
@@ -60,34 +59,34 @@
         """Bulk creation of items.
 
         Args:
             items: list of items.
 
         Returns:
             Message indicating the status of the insert.
-
         """
         raise NotImplementedError
 
 
 @attr.s
 class BulkTransactionExtension(ApiExtension):
     """Bulk Transaction Extension.
 
-    Bulk Transaction extension adds the `POST /collections/{collection_id}/bulk_items` endpoint to the application
-    for efficient bulk insertion of items. The input to this is an object with an attribute  "items", that has a value
-    that is an object with a group of attributes that are the ids of each Item, and the value is the Item entity.
+    Bulk Transaction extension adds the `POST
+    /collections/{collection_id}/bulk_items` endpoint to the application for
+    efficient bulk insertion of items. The input to this is an object with an
+    attribute  "items", that has a value that is an object with a group of
+    attributes that are the ids of each Item, and the value is the Item entity.
 
         {
         "items": {
             "id1": { "type": "Feature", ... },
             "id2": { "type": "Feature", ... },
             "id3": { "type": "Feature", ... }
         }
-
     """
 
     client: Union[
         AsyncBaseBulkTransactionsClient, BaseBulkTransactionsClient
     ] = attr.ib()
     conformance_classes: List[str] = attr.ib(default=list())
     schema_href: Optional[str] = attr.ib(default=None)
```

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/PKG-INFO` & `stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
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

### Comparing `stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/SOURCES.txt` & `stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

