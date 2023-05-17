# Comparing `tmp/scrapy_processors-1.1.0.tar.gz` & `tmp/scrapy_processors-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_processors-1.1.0.tar", max compression
+gzip compressed data, was "scrapy_processors-1.1.1.tar", max compression
```

## Comparing `scrapy_processors-1.1.0.tar` & `scrapy_processors-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_processors-1.1.0/LICENSE
--rw-r--r--   0        0        0     6604 2023-05-17 14:50:33.362775 scrapy_processors-1.1.0/README.md
--rw-r--r--   0        0        0      793 2023-05-17 14:25:20.631596 scrapy_processors-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-16 13:15:28.932402 scrapy_processors-1.1.0/scrapy_processors/__init__.py
--rw-r--r--   0        0        0     7178 2023-05-17 14:06:02.392719 scrapy_processors-1.1.0/scrapy_processors/processors.py
--rw-r--r--   0        0        0     7537 1970-01-01 00:00:00.000000 scrapy_processors-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_processors-1.1.1/LICENSE
+-rw-r--r--   0        0        0     6604 2023-05-17 14:50:33.362775 scrapy_processors-1.1.1/README.md
+-rw-r--r--   0        0        0      793 2023-05-17 18:10:40.314372 scrapy_processors-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-16 13:15:28.932402 scrapy_processors-1.1.1/scrapy_processors/__init__.py
+-rw-r--r--   0        0        0     8149 2023-05-17 18:12:28.874496 scrapy_processors-1.1.1/scrapy_processors/processors.py
+-rw-r--r--   0        0        0     7537 1970-01-01 00:00:00.000000 scrapy_processors-1.1.1/PKG-INFO
```

### Comparing `scrapy_processors-1.1.0/LICENSE` & `scrapy_processors-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_processors-1.1.0/README.md` & `scrapy_processors-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scrapy_processors-1.1.0/pyproject.toml` & `scrapy_processors-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "scrapy-processors"
-version = "1.1.0"
+version = "1.1.1"
 description = "Provides processors for the itemloaders package, commonly used with scrapy."
 authors = ["Nicholas Mischke <nmischkework@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "scrapy_processors"}]
 repository = "https://github.com/nicholas-mischke/scrapy-processors"
```

### Comparing `scrapy_processors-1.1.0/scrapy_processors/processors.py` & `scrapy_processors-1.1.1/scrapy_processors/processors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 
 # Standard library imports
 import re
 from datetime import datetime
-from inspect import isclass, isfunction, ismethod
+from builtins import callable as is_callable
+from inspect import isclass, isfunction, ismethod, ismethoddescriptor
 
 # itemloaders imports
 from itemloaders.processors import Identity
 from itemloaders.processors import MapCompose as BuiltInMapCompose
 from itemloaders.utils import arg_to_iter
 
 # 3rd 🎉 imports
 import emoji
 from bs4 import BeautifulSoup
 from price_parser import Price
 
 
 class MapCompose(BuiltInMapCompose):
     """
-    This class overwrites the built-in MapCompose class constructor 
-    to allow for passing of classes, class instances, and callables 
-    to the constructor.
-    """
+    This class overwrites the built-in MapCompose class constructor,
+    allowing it to accept any callable, or any class that once instantiated
+    is callable. 
+    
+    Additionally, it defines the __add__ method, allowing MapCompose objects
+    to be added together. The result is a new MapCompose object with the
+    functions and default_loader_contexts of both objects.
+    """
+
+    @classmethod
+    def get_callable(cls, arg):
+
+        if (
+            is_callable(arg)
+            and not isclass(arg)  # classes need to be instantiated
+        ):
+            return arg
+
+        if isclass(arg):
+            arg = arg()
+
+        if hasattr(arg, '__call__'):
+            return arg.__call__
+        else:
+            raise TypeError(
+                f"Unsupported callable type: '{type(arg).__name__}'"
+            )
 
     def __init__(self, *callables, **default_loader_context):
+        self.functions = tuple(
+            MapCompose.get_callable(callable) for callable in callables
+        )
         self.default_loader_context = default_loader_context
 
-        functions = []
-        for callable in callables:
-            if (
-                isfunction(callable)
-                or ismethod(callable)
-            ):
-                functions.append(callable)
-            elif isclass(callable):
-                functions.append(callable().__call__)
-            elif hasattr(callable, '__call__'):
-                functions.append(callable.__call__)
-        self.functions = tuple(functions)
-
-    def __add__(self, other):
+    def __add_MapCompose(self, other):
         # Must be of of type MapCompose or subclass
         if not isinstance(other, MapCompose):
             raise TypeError(
                 f"Unsupported operand type for +: 'MapCompose' and '{type(other).__name__}'"
             )
 
         # default_loader_context must have same key:value pairs
@@ -66,14 +80,32 @@
         default_loader_context.update(other.default_loader_context)
 
         # Combine functions
         functions = self.functions + other.functions
 
         return MapCompose(*functions, **default_loader_context)
 
+    def __add_callable(self, other):
+        try:
+            other = MapCompose.get_callable(other)
+        except TypeError:
+            raise TypeError(
+                f"Unsupported operand type for +: 'MapCompose' and '{type(other).__name__}'"
+            )
+
+        # Combine functions
+        functions = self.functions + (other,)
+
+        return MapCompose(*functions, **self.default_loader_context)
+
+    def __add__(self, other):
+        if isinstance(other, MapCompose):
+            return self.__add_MapCompose(other)
+        return self.__add_callable(other)
+
 
 class Processor:
 
     def process_value(self, value):
         raise NotImplementedError()
 
     def __call__(self, values):
@@ -180,15 +212,15 @@
     Assumes utf8, utf16, ascii or latin-1 encoding.
     """
 
     pattern = r'^[`ˋ‘’“”\'"\u0060\u02CB\x91\x92\x93\x94]+|[`ˋ‘’“”\'"\u0060\u02CB\x91\x92\x93\x94]+$'
 
     def process_value(self, value):
         return re.sub(self.pattern, '', value)
-    
+
 
 class StringToDateTime(Processor):
     """
     Given a string representing a date and time, return a datetime object.
     """
 
     def __init__(self, format='%Y-%m-%d, %H:%M:%S'):
```

### Comparing `scrapy_processors-1.1.0/PKG-INFO` & `scrapy_processors-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-processors
-Version: 1.1.0
+Version: 1.1.1
 Summary: Provides processors for the itemloaders package, commonly used with scrapy.
 Home-page: https://github.com/nicholas-mischke/scrapy-processors
 License: MIT
 Author: Nicholas Mischke
 Author-email: nmischkework@proton.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

