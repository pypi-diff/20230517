# Comparing `tmp/linushka_serializer-0.0.1.tar.gz` & `tmp/linushka_serializer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linushka_serializer-0.0.1.tar", last modified: Tue May 16 23:42:56 2023, max compression
+gzip compressed data, was "linushka_serializer-0.0.2.tar", last modified: Wed May 17 15:39:14 2023, max compression
```

## Comparing `linushka_serializer-0.0.1.tar` & `linushka_serializer-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 23:42:56.697199 linushka_serializer-0.0.1/
--rw-rw-rw-   0        0        0      110 2023-05-16 23:42:56.697199 linushka_serializer-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 23:42:56.657200 linushka_serializer-0.0.1/linushka_serializer.egg-info/
--rw-rw-rw-   0        0        0      110 2023-05-16 23:42:56.000000 linushka_serializer-0.0.1/linushka_serializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-05-16 23:42:56.000000 linushka_serializer-0.0.1/linushka_serializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 23:42:56.000000 linushka_serializer-0.0.1/linushka_serializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-16 23:42:56.000000 linushka_serializer-0.0.1/linushka_serializer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 23:42:56.662198 linushka_serializer-0.0.1/object_serializer/
--rw-rw-rw-   0        0        0       50 2023-05-16 22:00:28.000000 linushka_serializer-0.0.1/object_serializer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:42:56.674203 linushka_serializer-0.0.1/object_serializer/built_in_serializers/
--rw-rw-rw-   0        0        0      119 2023-05-16 22:00:28.000000 linushka_serializer-0.0.1/object_serializer/built_in_serializers/__init__.py
--rw-rw-rw-   0        0        0      275 2023-05-16 22:00:28.000000 linushka_serializer-0.0.1/object_serializer/built_in_serializers/base.py
--rw-rw-rw-   0        0        0     5234 2023-05-16 21:54:17.000000 linushka_serializer-0.0.1/object_serializer/built_in_serializers/json_serializer.py
--rw-rw-rw-   0        0        0     4670 2023-05-16 21:54:17.000000 linushka_serializer-0.0.1/object_serializer/built_in_serializers/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:42:56.696225 linushka_serializer-0.0.1/object_serializer/pre_serializer/
--rw-rw-rw-   0        0        0       32 2023-05-16 22:09:09.000000 linushka_serializer-0.0.1/object_serializer/pre_serializer/__init__.py
--rw-rw-rw-   0        0        0    10668 2023-05-16 22:09:09.000000 linushka_serializer-0.0.1/object_serializer/pre_serializer/tool.py
--rw-rw-rw-   0        0        0     1387 2023-05-16 21:25:27.000000 linushka_serializer-0.0.1/object_serializer/pre_serializer/utils.py
--rw-rw-rw-   0        0        0     1473 2023-05-16 22:22:13.000000 linushka_serializer-0.0.1/object_serializer/serializer_factory.py
--rw-rw-rw-   0        0        0     1078 2023-05-16 22:09:09.000000 linushka_serializer-0.0.1/object_serializer/serializer_proxy.py
--rw-rw-rw-   0        0        0       42 2023-05-16 23:42:56.698199 linushka_serializer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      321 2023-05-16 23:42:12.000000 linushka_serializer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:39:14.922120 linushka_serializer-0.0.2/
+-rw-rw-rw-   0        0        0      110 2023-05-17 15:39:14.921120 linushka_serializer-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 15:39:14.907338 linushka_serializer-0.0.2/linushka_serializer.egg-info/
+-rw-rw-rw-   0        0        0      110 2023-05-17 15:39:14.000000 linushka_serializer-0.0.2/linushka_serializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-05-17 15:39:14.000000 linushka_serializer-0.0.2/linushka_serializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:39:14.000000 linushka_serializer-0.0.2/linushka_serializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-17 15:39:14.000000 linushka_serializer-0.0.2/linushka_serializer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:39:14.910122 linushka_serializer-0.0.2/object_serializer/
+-rw-rw-rw-   0        0        0       50 2023-05-17 00:05:36.000000 linushka_serializer-0.0.2/object_serializer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:39:14.917121 linushka_serializer-0.0.2/object_serializer/built_in_serializers/
+-rw-rw-rw-   0        0        0      119 2023-05-17 00:05:36.000000 linushka_serializer-0.0.2/object_serializer/built_in_serializers/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-05-17 00:05:36.000000 linushka_serializer-0.0.2/object_serializer/built_in_serializers/base.py
+-rw-rw-rw-   0        0        0     5234 2023-05-17 00:05:36.000000 linushka_serializer-0.0.2/object_serializer/built_in_serializers/json_serializer.py
+-rw-rw-rw-   0        0        0     4670 2023-05-17 00:05:36.000000 linushka_serializer-0.0.2/object_serializer/built_in_serializers/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:39:14.920121 linushka_serializer-0.0.2/object_serializer/pre_serializer/
+-rw-rw-rw-   0        0        0       32 2023-05-17 00:06:26.000000 linushka_serializer-0.0.2/object_serializer/pre_serializer/__init__.py
+-rw-rw-rw-   0        0        0    12286 2023-05-17 15:23:01.000000 linushka_serializer-0.0.2/object_serializer/pre_serializer/tool.py
+-rw-rw-rw-   0        0        0     1446 2023-05-17 15:16:08.000000 linushka_serializer-0.0.2/object_serializer/pre_serializer/utils.py
+-rw-rw-rw-   0        0        0     1473 2023-05-17 00:07:22.000000 linushka_serializer-0.0.2/object_serializer/serializer_factory.py
+-rw-rw-rw-   0        0        0     1078 2023-05-17 00:06:26.000000 linushka_serializer-0.0.2/object_serializer/serializer_proxy.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 15:39:14.922652 linushka_serializer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      321 2023-05-17 15:38:58.000000 linushka_serializer-0.0.2/setup.py
```

### Comparing `linushka_serializer-0.0.1/linushka_serializer.egg-info/SOURCES.txt` & `linushka_serializer-0.0.2/linushka_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linushka_serializer-0.0.1/object_serializer/built_in_serializers/json_serializer.py` & `linushka_serializer-0.0.2/object_serializer/built_in_serializers/json_serializer.py`

 * *Files identical despite different names*

### Comparing `linushka_serializer-0.0.1/object_serializer/built_in_serializers/xml_serializer.py` & `linushka_serializer-0.0.2/object_serializer/built_in_serializers/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `linushka_serializer-0.0.1/object_serializer/pre_serializer/tool.py` & `linushka_serializer-0.0.2/object_serializer/pre_serializer/tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,14 +64,23 @@
 
         if isinstance(obj, type):  # class
             return self._encode_class(obj)
 
         if isinstance(obj, types.CodeType):  # code object
             return self._encode_code(obj)
 
+        if isinstance(obj, types.GeneratorType):
+            return self._encode_generator(obj)
+
+        if isinstance(obj, map):
+            return self._encode_map(obj)
+
+        if isinstance(obj, filter):
+            return self._encode_filter(obj)
+
         if is_iterable(obj):  # no analog in inspect
             return self._encode_iterator(obj)
 
         if isinstance(obj, types.ModuleType):
             return self._encode_module(obj)
 
         if isinstance(obj, object):  # instances
@@ -101,14 +110,26 @@
 
             if type_to_decode == TYPE.CELL:
                 return self._decode_cell(obj)
 
             if type_to_decode == TYPE.CLASS:
                 return self._decode_class(obj)
 
+            if type_to_decode == TYPE.GENERATOR:
+                return self._decode_generator(obj)
+
+            if type_to_decode == TYPE.FILTER:
+                return self._decode_filter(obj)
+
+            if type_to_decode == TYPE.MAP:
+                return self._decode_map(obj)
+
+            if type_to_decode == TYPE.FILTER:
+                return self._decode_filter(obj)
+
             if type_to_decode == TYPE.ITERATOR:
                 return self._decode_iterator(obj)
 
             if type_to_decode == TYPE.CODE:
                 return self._decode_code(obj)
 
             if type_to_decode == TYPE.OBJECT:
@@ -118,14 +139,26 @@
                 return self._decode_module(obj)
 
             if type_to_decode in (TYPE.TUPLE, TYPE.SET):
                 return self._decode_collection(obj)
 
         return obj
 
+    def _encode_generator(self, obj):
+        data = list(map(self.encode, obj))
+        return self._wrap_in_dict(
+            data=data,
+            _type=TYPE.GENERATOR,
+        )
+
+    def _decode_generator(self, obj):
+        data = self._get_data(obj)
+        print(data)
+        return iter(self.decode(value) for value in data)
+
     def _encode_bytes(self, bytes_obj: bytes):
         data = bytes_obj.hex()
         return self._wrap_in_dict(data, TYPE.BYTES)
 
     def _decode_bytes(self, encoded: str):
         return bytes.fromhex(self._get_data(encoded))
 
@@ -302,15 +335,15 @@
         return self._wrap_in_dict(
             data=data,
             _type=TYPE.ITERATOR,
         )
 
     def _decode_iterator(self, obj):
         data = self._get_data(obj)
-        return iter(self.decode(value) for value in data)
+        return iter(list(self.decode(value) for value in data))
 
     def _encode_object(self, obj):
         data = {
             "__class__": self.encode(obj.__class__),
             "attrs": {
                 attr: self.encode(value)
                 for (attr, value) in inspect.getmembers(obj)
@@ -331,7 +364,29 @@
         data = self._get_data(obj)
         obj_class = self.decode(data["__class__"])
 
         result = object.__new__(obj_class)
         result.__dict__ = {key: self.decode(value) for key, value in data["attrs"].items()}
 
         return result
+
+    def _encode_map(self, obj):
+        data = list(map(self.encode, obj))
+        return self._wrap_in_dict(
+            data=data,
+            _type=TYPE.MAP,
+        )
+
+    def _decode_map(self, obj):
+        data = self._get_data(obj)
+        return map(lambda x: x, list(self.decode(value) for value in data))
+
+    def _encode_filter(self, obj):
+        data = list(map(self.encode, obj))
+        return self._wrap_in_dict(
+            data=data,
+            _type=TYPE.FILTER,
+        )
+
+    def _decode_filter(self, obj):
+        data = self._get_data(obj)
+        return filter(lambda x: x, list(self.decode(value) for value in data))
```

### Comparing `linushka_serializer-0.0.1/object_serializer/pre_serializer/utils.py` & `linushka_serializer-0.0.2/object_serializer/pre_serializer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     ITERATOR = auto()
     CODE = auto()
     OBJECT = auto()
     MODULE = auto()
     TUPLE = auto()
     SET = auto()
     PROPERTY = auto()
-
+    GENERATOR = auto()
+    MAP = auto()
+    FILTER = auto()
 
 UNSERIALIZABLE_DUNDER = (
     "__mro__",
     "__base__",
     "__basicsize__",
     "__class__",
     "__dictoffset__",
```

### Comparing `linushka_serializer-0.0.1/object_serializer/serializer_factory.py` & `linushka_serializer-0.0.2/object_serializer/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `linushka_serializer-0.0.1/object_serializer/serializer_proxy.py` & `linushka_serializer-0.0.2/object_serializer/serializer_proxy.py`

 * *Files identical despite different names*

