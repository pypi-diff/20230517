# Comparing `tmp/flattrs-23.1.0b8.tar.gz` & `tmp/flattrs-23.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flattrs-23.1.0b8.tar", last modified: Wed May  3 10:59:42 2023, max compression
+gzip compressed data, was "flattrs-23.1.0b9.tar", last modified: Wed May 17 16:40:42 2023, max compression
```

## Comparing `flattrs-23.1.0b8.tar` & `flattrs-23.1.0b9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.893114 flattrs-23.1.0b8/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1074 2020-11-10 12:31:21.000000 flattrs-23.1.0b8/LICENSE
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-05-03 10:59:42.893250 flattrs-23.1.0b8/PKG-INFO
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2382 2023-05-03 10:51:46.000000 flattrs-23.1.0b8/README.rst
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      308 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/pyproject.toml
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      136 2023-05-03 10:59:42.893741 flattrs-23.1.0b8/setup.cfg
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1118 2023-05-03 10:57:32.000000 flattrs-23.1.0b8/setup.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.878152 flattrs-23.1.0b8/src/
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.882460 flattrs-23.1.0b8/src/flattrs/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      930 2023-02-28 15:21:53.000000 flattrs-23.1.0b8/src/flattrs/__init__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    11817 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/_analysis.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1686 2023-02-25 17:46:21.000000 flattrs-23.1.0b8/src/flattrs/_consts.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      489 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/_types.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.890634 flattrs-23.1.0b8/src/flattrs/cflattrs/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/__init__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)   701668 2023-05-02 23:55:06.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/builder.c
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    28957 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/builder.pyx
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)   170967 2023-02-23 10:23:16.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/encode.c
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1443 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/encode.pyx
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)   336629 2023-05-02 23:55:06.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.c
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      351 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.pxd
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2081 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.pyx
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    20943 2023-03-08 16:56:01.000000 flattrs-23.1.0b8/src/flattrs/converters.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.891959 flattrs-23.1.0b8/src/flattrs/modgen/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/modgen/__init__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      451 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/modgen/__main__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1664 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/modgen/parser.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    27816 2023-05-03 10:51:46.000000 flattrs-23.1.0b8/src/flattrs/modgen/renderer.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/py.typed
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1413 2023-02-25 17:46:21.000000 flattrs-23.1.0b8/src/flattrs/types.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2765 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/typing.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.884601 flattrs-23.1.0b8/src/flattrs.egg-info/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/PKG-INFO
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      915 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/SOURCES.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/dependency_links.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)       57 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/entry_points.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2020-11-10 12:31:30.000000 flattrs-23.1.0b8/src/flattrs.egg-info/not-zip-safe
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      142 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/requires.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        8 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/top_level.txt
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.892795 flattrs-23.1.0b8/tests/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1070 2023-03-08 16:53:46.000000 flattrs-23.1.0b8/tests/test_misc.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1511 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/tests/test_modgen.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-17 16:40:42.844193 flattrs-23.1.0b9/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1074 2020-11-10 12:31:21.000000 flattrs-23.1.0b9/LICENSE
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-05-17 16:40:42.844446 flattrs-23.1.0b9/PKG-INFO
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2511 2023-05-17 16:40:09.000000 flattrs-23.1.0b9/README.rst
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      308 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/pyproject.toml
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      136 2023-05-17 16:40:42.845496 flattrs-23.1.0b9/setup.cfg
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1128 2023-05-17 16:39:03.000000 flattrs-23.1.0b9/setup.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-17 16:40:42.818131 flattrs-23.1.0b9/src/
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-17 16:40:42.828030 flattrs-23.1.0b9/src/flattrs/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      930 2023-02-28 15:21:53.000000 flattrs-23.1.0b9/src/flattrs/__init__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    11802 2023-05-17 16:39:03.000000 flattrs-23.1.0b9/src/flattrs/_analysis.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1686 2023-02-25 17:46:21.000000 flattrs-23.1.0b9/src/flattrs/_consts.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      489 2023-03-15 13:05:01.000000 flattrs-23.1.0b9/src/flattrs/_types.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-17 16:40:42.839576 flattrs-23.1.0b9/src/flattrs/cflattrs/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/__init__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)   701668 2023-05-17 16:32:04.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/builder.c
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    28957 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/builder.pyx
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)   170967 2023-02-23 10:23:16.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/encode.c
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1443 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/encode.pyx
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)   336629 2023-05-17 16:32:04.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/number_types.c
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      351 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/number_types.pxd
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2081 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/src/flattrs/cflattrs/number_types.pyx
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    20962 2023-05-17 16:39:03.000000 flattrs-23.1.0b9/src/flattrs/converters.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-17 16:40:42.842391 flattrs-23.1.0b9/src/flattrs/modgen/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/src/flattrs/modgen/__init__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      451 2023-03-15 13:05:01.000000 flattrs-23.1.0b9/src/flattrs/modgen/__main__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1664 2023-03-15 13:05:01.000000 flattrs-23.1.0b9/src/flattrs/modgen/parser.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    27816 2023-05-03 10:51:46.000000 flattrs-23.1.0b9/src/flattrs/modgen/renderer.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b9/src/flattrs/py.typed
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1413 2023-02-25 17:46:21.000000 flattrs-23.1.0b9/src/flattrs/types.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1779 2023-05-17 16:39:03.000000 flattrs-23.1.0b9/src/flattrs/typing.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-17 16:40:42.832978 flattrs-23.1.0b9/src/flattrs.egg-info/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-05-17 16:40:42.000000 flattrs-23.1.0b9/src/flattrs.egg-info/PKG-INFO
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      915 2023-05-17 16:40:42.000000 flattrs-23.1.0b9/src/flattrs.egg-info/SOURCES.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2023-05-17 16:40:42.000000 flattrs-23.1.0b9/src/flattrs.egg-info/dependency_links.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)       57 2023-05-17 16:40:42.000000 flattrs-23.1.0b9/src/flattrs.egg-info/entry_points.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2020-11-10 12:31:30.000000 flattrs-23.1.0b9/src/flattrs.egg-info/not-zip-safe
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      150 2023-05-17 16:40:42.000000 flattrs-23.1.0b9/src/flattrs.egg-info/requires.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        8 2023-05-17 16:40:42.000000 flattrs-23.1.0b9/src/flattrs.egg-info/top_level.txt
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-17 16:40:42.843740 flattrs-23.1.0b9/tests/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1070 2023-03-08 16:53:46.000000 flattrs-23.1.0b9/tests/test_misc.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1511 2023-03-15 13:05:01.000000 flattrs-23.1.0b9/tests/test_modgen.py
```

### Comparing `flattrs-23.1.0b8/LICENSE` & `flattrs-23.1.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/README.rst` & `flattrs-23.1.0b9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .. image:: https://img.shields.io/github/license/pocketzworld/flattrs?style=flat-square
    :alt: MIT
 
 Changelog:
 ----------
 
+23.1.0b9 (2023-05-17)
+~~~~~~~~~~~~~~~~~~~~~
+* Set the minimum _attrs_ version to ensure we get the right `attrs.resolve_types`.
+
 23.1.0b8 (2023-05-03)
 ~~~~~~~~~~~~~~~~~~~~~
 * Greatly improve namespace handling.
 
 23.1.0b7 (2023-03-28)
 ~~~~~~~~~~~~~~~~~~~~~
 * Implement reordering of unions in the generated code where required.
```

### Comparing `flattrs-23.1.0b8/setup.py` & `flattrs-23.1.0b9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 else:
     ext_modules = []
 
 setup(
     name="flattrs",
     long_description="Flatbuffers support for Python",
     long_description_content_type="text/x-rst",
-    version="23.1.0.b8",
+    version="23.1.0.b9",
     install_requires=[
-        "attrs",
+        "attrs >= 23.1.0",
         "flatbuffers==23.1.4",
         "click",
         "lark >= 1.1.5",
         "immutables",
     ],
     packages=find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `flattrs-23.1.0b8/src/flattrs/__init__.py` & `flattrs-23.1.0b9/src/flattrs/__init__.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/_analysis.py` & `flattrs-23.1.0b9/src/flattrs/_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Types used internally."""
 from enum import IntEnum
 
-from attrs import NOTHING, AttrsInstance, fields, frozen, has
+from attrs import NOTHING, AttrsInstance, fields, frozen, has, resolve_types
 
 from ._consts import ENUM_TYPE_TO_SCALAR_TYPE, HELPER_TYPE_TO_SCALAR_TYPE, NoneType
 from ._types import (
     FieldName,
     MaybeDefault,
     Optionality,
     PythonScalarType,
@@ -18,15 +18,14 @@
     Float64,
     Int8,
     Int8Enum,
     Int16,
     Int16Enum,
     Int32,
     Int32Enum,
-    Int64,
     Int64Enum,
     ScalarMarker,
     Uint8,
     Uint8Enum,
     Uint16,
     Uint16Enum,
     Uint32,
@@ -37,15 +36,14 @@
 )
 from .typing import (
     get_annotation_and_base,
     get_optional_arg,
     get_union_args,
     is_generic_subclass,
     is_subclass,
-    resolve_types,
 )
 
 
 @frozen
 class FlatbufferTable:
     cl: type[AttrsInstance]
     num_slots: int
```

### Comparing `flattrs-23.1.0b8/src/flattrs/_consts.py` & `flattrs-23.1.0b9/src/flattrs/_consts.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/cflattrs/builder.c` & `flattrs-23.1.0b9/src/flattrs/cflattrs/builder.c`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/cflattrs/builder.pyx` & `flattrs-23.1.0b9/src/flattrs/cflattrs/builder.pyx`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/cflattrs/encode.c` & `flattrs-23.1.0b9/src/flattrs/cflattrs/encode.c`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/cflattrs/encode.pyx` & `flattrs-23.1.0b9/src/flattrs/cflattrs/encode.pyx`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.c` & `flattrs-23.1.0b9/src/flattrs/cflattrs/number_types.c`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.pyx` & `flattrs-23.1.0b9/src/flattrs/cflattrs/number_types.pyx`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/converters.py` & `flattrs-23.1.0b9/src/flattrs/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 try:
     from .cflattrs.builder import Builder
 except ImportError:  # NOQA
     from flatbuffers.builder import Builder
 
 T = TypeVar("T", bound=AttrsInstance)
 AddToBuilder: TypeAlias = Callable[[T, Builder, dict[int, int], dict[int, int]], int]
+start_struct: Final = struct.Struct("<I")
 
 
 @define
 class Converter:
     """A converter for loading and dumping Flatbuffers."""
 
     _dumps_cache: Callable = Factory(
@@ -69,18 +70,19 @@
     def _make_from_fb(self, cl: type[AttrsInstance]) -> Callable:
         """Generate all necessary functions for a class to work with Flatbuffers."""
         return make_from_fb_fn(analyze(cl), self._from_fb_cache)
 
     def make_loads(self, cl: type[T]) -> Callable[[bytes], T]:
         """Prepare a loading function for a model in advance."""
         from_fb = self._from_fb_cache(cl)
-        start_struct = struct.Struct("<I")
 
-        def loads(data: bytes, _from_fb=from_fb, _start_struct=start_struct) -> T:
-            start_offset = _start_struct.unpack_from(data, 0)[0]
+        def loads(
+            data: bytes, _from_fb=from_fb, _unpack_from=start_struct.unpack_from
+        ) -> T:
+            start_offset = _unpack_from(data, 0)[0]
             return _from_fb(Table(data, start_offset))
 
         return loads
 
     def make_dumps(self, cl: type[T]) -> Callable[[T, Builder | None], bytes]:
         """Prepare a dumping function for a model in advance."""
```

### Comparing `flattrs-23.1.0b8/src/flattrs/modgen/parser.py` & `flattrs-23.1.0b9/src/flattrs/modgen/parser.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/modgen/renderer.py` & `flattrs-23.1.0b9/src/flattrs/modgen/renderer.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs/types.py` & `flattrs-23.1.0b9/src/flattrs/types.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/src/flattrs.egg-info/SOURCES.txt` & `flattrs-23.1.0b9/src/flattrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/tests/test_misc.py` & `flattrs-23.1.0b9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b8/tests/test_modgen.py` & `flattrs-23.1.0b9/tests/test_modgen.py`

 * *Files identical despite different names*

