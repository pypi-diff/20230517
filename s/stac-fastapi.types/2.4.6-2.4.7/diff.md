# Comparing `tmp/stac-fastapi.types-2.4.6.tar.gz` & `tmp/stac-fastapi.types-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.types-2.4.6.tar", last modified: Wed May 10 15:53:01 2023, max compression
+gzip compressed data, was "stac-fastapi.types-2.4.7.tar", last modified: Wed May 17 15:30:40 2023, max compression
```

## Comparing `stac-fastapi.types-2.4.6.tar` & `stac-fastapi.types-2.4.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.438334 stac-fastapi.types-2.4.6/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 15:30:40.272149 stac-fastapi.types-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/top_level.txt
```

### Comparing `stac-fastapi.types-2.4.6/PKG-INFO` & `stac-fastapi.types-2.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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

### Comparing `stac-fastapi.types-2.4.6/setup.py` & `stac-fastapi.types-2.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/config.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,32 @@
     Defines api configuration, potentially through environment variables.
     See https://pydantic-docs.helpmanual.io/usage/settings/.
     Attributes:
         environment: name of the environment (ex. dev/prod).
         debug: toggles debug mode.
         forbidden_fields: set of fields defined by STAC but not included in the database.
         indexed_fields:
-            set of fields which are usually in `item.properties` but are indexed as distinct columns in
-            the database.
+            set of fields which are usually in `item.properties` but are indexed
+            as distinct columns in the database.
     """
 
-    # TODO: Remove `default_includes` attribute so we can use `pydantic.BaseSettings` instead
+    # TODO: Remove `default_includes` attribute so we can use
+    # `pydantic.BaseSettings` instead
     default_includes: Optional[Set[str]] = None
 
     app_host: str = "0.0.0.0"
     app_port: int = 8000
     reload: bool = True
     enable_response_models: bool = False
 
     openapi_url: str = "/api"
     docs_url: str = "/api.html"
 
     class Config:
-        """model config (https://pydantic-docs.helpmanual.io/usage/model_config/)."""
+        """Model config (https://pydantic-docs.helpmanual.io/usage/model_config/)."""
 
         extra = "allow"
         env_file = ".env"
 
 
 class Settings:
     """Holds the global instance of settings."""
@@ -44,11 +45,14 @@
     @classmethod
     def set(cls, base_settings: ApiSettings):
         """Set the global settings."""
         cls._instance = base_settings
 
     @classmethod
     def get(cls) -> ApiSettings:
-        """Get the settings. If they have not yet been set, throws an exception."""
+        """Get the settings.
+
+        If they have not yet been set, throws an exception.
+        """
         if cls._instance is None:
             raise ValueError("Settings have not yet been set.")
         return cls._instance
```

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/conformance.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/core.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,39 +24,42 @@
 
 @attr.s  # type:ignore
 class BaseTransactionsClient(abc.ABC):
     """Defines a pattern for implementing the STAC API Transaction Extension."""
 
     @abc.abstractmethod
     def create_item(
-        self, collection_id: str, item: stac_types.Item, **kwargs
-    ) -> Optional[Union[stac_types.Item, Response]]:
+        self,
+        collection_id: str,
+        item: Union[stac_types.Item, stac_types.ItemCollection],
+        **kwargs,
+    ) -> Optional[Union[stac_types.Item, Response, None]]:
         """Create a new item.
 
         Called with `POST /collections/{collection_id}/items`.
 
         Args:
-            item: the item
+            item: the item or item collection
             collection_id: the id of the collection from the resource path
 
         Returns:
-            The item that was created.
-
+            The item that was created or None if item collection.
         """
         ...
 
     @abc.abstractmethod
     def update_item(
         self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Perform a complete update on an existing item.
 
-        Called with `PUT /collections/{collection_id}/items`. It is expected that this item already exists.  The update
-        should do a diff against the saved item and perform any necessary updates.  Partial updates are not supported
-        by the transactions extension.
+        Called with `PUT /collections/{collection_id}/items`. It is expected
+        that this item already exists.  The update should do a diff against the
+        saved item and perform any necessary updates.  Partial updates are not
+        supported by the transactions extension.
 
         Args:
             item: the item (must be complete)
             collection_id: the id of the collection from the resource path
 
         Returns:
             The updated item.
@@ -98,16 +101,17 @@
 
     @abc.abstractmethod
     def update_collection(
         self, collection: stac_types.Collection, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
-        Called with `PUT /collections`. It is expected that this item already exists.  The update should do a diff
-        against the saved collection and perform any necessary updates.  Partial updates are not supported by the
+        Called with `PUT /collections`. It is expected that this item already
+        exists.  The update should do a diff against the saved collection and
+        perform any necessary updates.  Partial updates are not supported by the
         transactions extension.
 
         Args:
             collection: the collection (must be complete)
             collection_id: the id of the collection from the resource path
 
         Returns:
@@ -134,38 +138,42 @@
 
 @attr.s  # type:ignore
 class AsyncBaseTransactionsClient(abc.ABC):
     """Defines a pattern for implementing the STAC transaction extension."""
 
     @abc.abstractmethod
     async def create_item(
-        self, collection_id: str, item: stac_types.Item, **kwargs
-    ) -> Optional[Union[stac_types.Item, Response]]:
+        self,
+        collection_id: str,
+        item: Union[stac_types.Item, stac_types.ItemCollection],
+        **kwargs,
+    ) -> Optional[Union[stac_types.Item, Response, None]]:
         """Create a new item.
 
         Called with `POST /collections/{collection_id}/items`.
 
         Args:
-            item: the item
+            item: the item or item collection
+            collection_id: the id of the collection from the resource path
 
         Returns:
-            The item that was created.
-
+            The item that was created or None if item collection.
         """
         ...
 
     @abc.abstractmethod
     async def update_item(
         self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Perform a complete update on an existing item.
 
-        Called with `PUT /collections/{collection_id}/items`. It is expected that this item already exists.  The update
-        should do a diff against the saved item and perform any necessary updates.  Partial updates are not supported
-        by the transactions extension.
+        Called with `PUT /collections/{collection_id}/items`. It is expected
+        that this item already exists.  The update should do a diff against the
+        saved item and perform any necessary updates.  Partial updates are not
+        supported by the transactions extension.
 
         Args:
             item: the item (must be complete)
 
         Returns:
             The updated item.
         """
@@ -206,16 +214,17 @@
 
     @abc.abstractmethod
     async def update_collection(
         self, collection: stac_types.Collection, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
-        Called with `PUT /collections`. It is expected that this item already exists.  The update should do a diff
-        against the saved collection and perform any necessary updates.  Partial updates are not supported by the
+        Called with `PUT /collections`. It is expected that this item already
+        exists.  The update should do a diff against the saved collection and
+        perform any necessary updates.  Partial updates are not supported by the
         transactions extension.
 
         Args:
             collection: the collection (must be complete)
 
         Returns:
             The updated collection.
@@ -314,15 +323,16 @@
     base_conformance_classes: List[str] = attr.ib(
         factory=lambda: BASE_CONFORMANCE_CLASSES
     )
     extensions: List[ApiExtension] = attr.ib(default=attr.Factory(list))
     post_request_model = attr.ib(default=BaseSearchPostRequest)
 
     def conformance_classes(self) -> List[str]:
-        """Generate conformance classes by adding extension conformance to base conformance classes."""
+        """Generate conformance classes by adding extension conformance to base
+        conformance classes."""
         base_conformance_classes = self.base_conformance_classes.copy()
 
         for extension in self.extensions:
             extension_classes = getattr(extension, "conformance_classes", [])
             base_conformance_classes.extend(extension_classes)
 
         return list(set(base_conformance_classes))
@@ -521,15 +531,16 @@
     base_conformance_classes: List[str] = attr.ib(
         factory=lambda: BASE_CONFORMANCE_CLASSES
     )
     extensions: List[ApiExtension] = attr.ib(default=attr.Factory(list))
     post_request_model = attr.ib(default=BaseSearchPostRequest)
 
     def conformance_classes(self) -> List[str]:
-        """Generate conformance classes by adding extension conformance to base conformance classes."""
+        """Generate conformance classes by adding extension conformance to base
+        conformance classes."""
         conformance_classes = self.base_conformance_classes.copy()
 
         for extension in self.extensions:
             extension_classes = getattr(extension, "conformance_classes", [])
             conformance_classes.extend(extension_classes)
 
         return list(set(conformance_classes))
@@ -714,20 +725,19 @@
     """Defines a pattern for implementing the STAC filter extension."""
 
     async def get_queryables(
         self, collection_id: Optional[str] = None, **kwargs
     ) -> Dict[str, Any]:
         """Get the queryables available for the given collection_id.
 
-        If collection_id is None, returns the intersection of all
-        queryables over all collections.
+        If collection_id is None, returns the intersection of all queryables over all
+        collections.
 
         This base implementation returns a blank queryable schema. This is not allowed
         under OGC CQL but it is allowed by the STAC API Filter Extension
-
         https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
         """
         return {
             "$schema": "https://json-schema.org/draft/2019-09/schema",
             "$id": "https://example.org/queryables",
             "type": "object",
             "title": "Queryables for Example STAC API",
@@ -741,20 +751,19 @@
     """Defines a pattern for implementing the STAC filter extension."""
 
     def get_queryables(
         self, collection_id: Optional[str] = None, **kwargs
     ) -> Dict[str, Any]:
         """Get the queryables available for the given collection_id.
 
-        If collection_id is None, returns the intersection of all
-        queryables over all collections.
+        If collection_id is None, returns the intersection of all queryables over all
+        collections.
 
         This base implementation returns a blank queryable schema. This is not allowed
         under OGC CQL but it is allowed by the STAC API Filter Extension
-
         https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
         """
         return {
             "$schema": "https://json-schema.org/draft/2019-09/schema",
             "$id": "https://example.org/queryables",
             "type": "object",
             "title": "Queryables for Example STAC API",
```

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/errors.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/extension.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""base api extension."""
+"""Base api extension."""
 import abc
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 from pydantic import BaseModel
```

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/links.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-"""link helpers."""
+"""Link helpers."""
 
 from typing import Any, Dict, List
 from urllib.parse import urljoin
 
 import attr
 from stac_pydantic.links import Relations
 from stac_pydantic.shared import MimeTypes
 
 # These can be inferred from the item/collection so they aren't included in the database
-# Instead they are dynamically generated when querying the database using the classes defined below
+# Instead they are dynamically generated when querying the database using the
+# classes defined below
 INFERRED_LINK_RELS = ["self", "item", "parent", "collection", "root"]
 
 
 def filter_links(links: List[Dict]) -> List[Dict]:
     """Remove inferred links."""
     return [link for link in links if link["rel"] not in INFERRED_LINK_RELS]
```

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/rfc3339.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/rfc3339.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import re
 from datetime import datetime, timezone
 from typing import Optional, Tuple
 
 import iso8601
 from pystac.utils import datetime_to_str
 
-RFC33339_PATTERN = r"^(\d\d\d\d)\-(\d\d)\-(\d\d)(T|t)(\d\d):(\d\d):(\d\d)([.]\d+)?(Z|([-+])(\d\d):(\d\d))$"
+RFC33339_PATTERN = (
+    r"^(\d\d\d\d)\-(\d\d)\-(\d\d)(T|t)(\d\d):(\d\d):(\d\d)([.]\d+)?"
+    r"(Z|([-+])(\d\d):(\d\d))$"
+)
 
 
 def rfc3339_str_to_datetime(s: str) -> datetime:
     """Convert a string conforming to RFC 3339 to a :class:`datetime.datetime`.
 
     Uses :meth:`iso8601.parse_date` under the hood.
 
@@ -59,17 +62,17 @@
     if len(values) != 2:
         raise ValueError(
             f"Interval string '{interval}' contains more than one forward slash."
         )
 
     start = None
     end = None
-    if not values[0] in ["..", ""]:
+    if values[0] not in ["..", ""]:
         start = rfc3339_str_to_datetime(values[0])
-    if not values[1] in ["..", ""]:
+    if values[1] not in ["..", ""]:
         end = rfc3339_str_to_datetime(values[1])
 
     if start is None and end is None:
         raise ValueError("Double open-ended intervals are not allowed.")
     if start is not None and end is not None and start > end:
         raise ValueError("Start datetime cannot be before end datetime.")
     else:
```

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/search.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 
 
 @attr.s  # type:ignore
 class APIRequest(abc.ABC):
     """Generic API Request base class."""
 
     def kwargs(self) -> Dict:
-        """Transform api request params into format which matches the signature of the endpoint."""
+        """Transform api request params into format which matches the signature of the
+        endpoint."""
         return self.__dict__
 
 
 @attr.s
 class BaseSearchGetRequest(APIRequest):
     """Base arguments for GET Request."""
 
@@ -102,16 +103,16 @@
     datetime: Optional[str] = attr.ib(default=None)
     limit: Optional[int] = attr.ib(default=10)
 
 
 class BaseSearchPostRequest(BaseModel):
     """Search model.
 
-    Replace base model in STAC-pydantic as it includes additional fields,
-    not in the core model.
+    Replace base model in STAC-pydantic as it includes additional fields, not in the core
+    model.
     https://github.com/radiantearth/stac-api-spec/tree/master/item-search#query-parameter-table
 
     PR to fix this:
     https://github.com/stac-utils/stac-pydantic/pull/100
     """
 
     collections: Optional[List[str]]
@@ -200,17 +201,19 @@
                 "Invalid datetime range, must match format (begin_date, end_date)"
             )
 
         return v
 
     @property
     def spatial_filter(self) -> Optional[_GeometryBase]:
-        """Return a geojson-pydantic object representing the spatial filter for the search request.
+        """Return a geojson-pydantic object representing the spatial filter for the search
+        request.
 
-        Check for both because the ``bbox`` and ``intersects`` parameters are mutually exclusive.
+        Check for both because the ``bbox`` and ``intersects`` parameters are
+        mutually exclusive.
         """
         if self.bbox:
             return Polygon(
                 coordinates=[
                     [
                         [self.bbox[0], self.bbox[3]],
                         [self.bbox[2], self.bbox[3]],
```

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi/types/stac.py` & `stac-fastapi.types-2.4.7/stac_fastapi/types/stac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """STAC types."""
 import sys
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 
 # Avoids a Pydantic error:
-# TypeError: You should use `typing_extensions.TypedDict` instead of `typing.TypedDict` with Python < 3.9.2.
-# Without it, there is no way to differentiate required and optional fields when subclassed.
+# TypeError: You should use `typing_extensions.TypedDict` instead of
+# `typing.TypedDict` with Python < 3.9.2.  Without it, there is no way to
+# differentiate required and optional fields when subclassed.
 if sys.version_info < (3, 9, 2):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 NumType = Union[float, int]
 
@@ -54,30 +55,30 @@
     summaries: Dict[str, Any]
     assets: Dict[str, Any]
 
 
 class Item(TypedDict, total=False):
     """STAC Item."""
 
-    type: str
+    type: Literal["Feature"]
     stac_version: str
     stac_extensions: Optional[List[str]]
     id: str
     geometry: Dict[str, Any]
     bbox: List[NumType]
     properties: Dict[str, Any]
     links: List[Dict[str, Any]]
     assets: Dict[str, Any]
     collection: str
 
 
 class ItemCollection(TypedDict, total=False):
     """STAC Item Collection."""
 
-    type: str
+    type: Literal["FeatureCollection"]
     features: List[Item]
     links: List[Dict[str, Any]]
     context: Optional[Dict[str, int]]
 
 
 class Collections(TypedDict, total=False):
     """All collections endpoint.
```

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/PKG-INFO` & `stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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

### Comparing `stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/SOURCES.txt` & `stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

