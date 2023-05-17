# Comparing `tmp/tinystream-0.1.0.tar.gz` & `tmp/tinystream-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinystream-0.1.0.tar", last modified: Tue May 16 14:08:38 2023, max compression
+gzip compressed data, was "tinystream-0.1.1.tar", last modified: Wed May 17 10:32:41 2023, max compression
```

## Comparing `tinystream-0.1.0.tar` & `tinystream-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-16 14:08:38.090384 tinystream-0.1.0/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.1.0/LICENSE
--rw-r--r--   0 mikereiche   (502) staff       (20)     4152 2023-05-16 14:08:38.090253 tinystream-0.1.0/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     3918 2023-05-16 11:33:29.000000 tinystream-0.1.0/README.md
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-16 14:08:38.090421 tinystream-0.1.0/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-16 14:08:26.000000 tinystream-0.1.0/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-16 14:08:38.090077 tinystream-0.1.0/tinystream.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     4152 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)     6598 2023-05-16 11:27:14.000000 tinystream-0.1.0/tinystream.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-17 10:32:41.782634 tinystream-0.1.1/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.1.1/LICENSE
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4303 2023-05-17 10:32:41.782483 tinystream-0.1.1/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4069 2023-05-17 10:25:29.000000 tinystream-0.1.1/README.md
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-17 10:32:41.782682 tinystream-0.1.1/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-17 10:32:07.000000 tinystream-0.1.1/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-17 10:32:41.782200 tinystream-0.1.1/tinystream.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4303 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-17 10:32:41.000000 tinystream-0.1.1/tinystream.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6713 2023-05-17 10:15:16.000000 tinystream-0.1.1/tinystream.py
```

### Comparing `tinystream-0.1.0/LICENSE` & `tinystream-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinystream-0.1.0/PKG-INFO` & `tinystream-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.1.0
+Version: 0.1.1
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
@@ -21,26 +21,57 @@
 ```python
 from tinystream import Stream
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
-    .filter(lambda x: x > 2) \    # filter_key()
+    .filter(lambda x: x > 2) \    # filter_key(), filter_type()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \
     .limit(2) \
     .concat([4]) \
     .sum()                        # reduce(), max(), min(), collect(), count()
 ```
 
 ## Aggregators
 
 Aggregator methods like `sum()`, `collect()`, `count()`... will end the stream.
 
+## Typehinting
+
+You can typehint datatypes like:
+
+```python
+from dataclasses import dataclass
+
+@dataclass
+class Node:
+    name: str
+    parent: "Node" = None
+
+parent = Node(name="B")
+child = Node(name="A", parent=parent)
+```
+
+for lambdas:
+
+```python
+stream = Stream.of([child])
+assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
+```
+
+This is not necessary when you pass a mapping function:
+```python
+def map_parent(n: Node):
+    return n.parent
+
+assert stream.map(map_parent).next().get().name == "B"
+```
+
 ## Built-in Optional support
 
 Some aggregator functions are *optional*:
 
 ```python
 assert Stream.of((1, 2, 3, 4, 5)).sum().empty is False
 ```
@@ -64,52 +95,24 @@
 assert Opt("String").map(len).get() == 6
 ```
 
 Get default value:
 ```python
 assert Opt(None).get(6) == 6
 assert Opt(None).get(lambda: 6) == 6
+assert Opt(None).if_empty(lambda: 3).empty is False
 ```
 
 Filter value:
 
 ```python
 assert Opt(0).filter(lambda x: x > 0).empty is True
 ```
 
-## Typehinting
-
-You can typehint datatypes like:
-
-```python
-from dataclasses import dataclass
-
-@dataclass
-class Node:
-    name: str
-    parent: "Node" = None
-
-parent = Node(name="B")
-child = Node(name="A", parent=parent)
-```
-
-for lambdas:
-
-```python
-stream = Stream.of([child])
-assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
-```
-
-This is not necessary when you pass a mapping function:
-```python
-def map_parent(n: Node):
-    return n.parent
-
-assert stream.map(map_parent).next().get().name == "B"
-```
+## More features
 
 ### Typed dictionaries
 
 Dictionaries are streamed as `tuple(key, value)`
 
 ```python
 children = {"a": Node(name="Child")} 
@@ -120,21 +123,24 @@
 ```
 
 This is the same like (but without known types):
 ```python
 stream = Stream.of(children)
 ```
 
-## More features
-
 ### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
+### Filter by type
+```python
+nodes_only = Stream.of([child]).filter_type(Node)
+```
+
 ### Map object name attribute
 ```python
 names = Stream.of([child]).map_key("name")
 ```
 
 ### Deep mapping of name attributes
 ```python
```

### Comparing `tinystream-0.1.0/README.md` & `tinystream-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,57 @@
 ```python
 from tinystream import Stream
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
-    .filter(lambda x: x > 2) \    # filter_key()
+    .filter(lambda x: x > 2) \    # filter_key(), filter_type()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \
     .limit(2) \
     .concat([4]) \
     .sum()                        # reduce(), max(), min(), collect(), count()
 ```
 
 ## Aggregators
 
 Aggregator methods like `sum()`, `collect()`, `count()`... will end the stream.
 
+## Typehinting
+
+You can typehint datatypes like:
+
+```python
+from dataclasses import dataclass
+
+@dataclass
+class Node:
+    name: str
+    parent: "Node" = None
+
+parent = Node(name="B")
+child = Node(name="A", parent=parent)
+```
+
+for lambdas:
+
+```python
+stream = Stream.of([child])
+assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
+```
+
+This is not necessary when you pass a mapping function:
+```python
+def map_parent(n: Node):
+    return n.parent
+
+assert stream.map(map_parent).next().get().name == "B"
+```
+
 ## Built-in Optional support
 
 Some aggregator functions are *optional*:
 
 ```python
 assert Stream.of((1, 2, 3, 4, 5)).sum().empty is False
 ```
@@ -55,52 +86,24 @@
 assert Opt("String").map(len).get() == 6
 ```
 
 Get default value:
 ```python
 assert Opt(None).get(6) == 6
 assert Opt(None).get(lambda: 6) == 6
+assert Opt(None).if_empty(lambda: 3).empty is False
 ```
 
 Filter value:
 
 ```python
 assert Opt(0).filter(lambda x: x > 0).empty is True
 ```
 
-## Typehinting
-
-You can typehint datatypes like:
-
-```python
-from dataclasses import dataclass
-
-@dataclass
-class Node:
-    name: str
-    parent: "Node" = None
-
-parent = Node(name="B")
-child = Node(name="A", parent=parent)
-```
-
-for lambdas:
-
-```python
-stream = Stream.of([child])
-assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
-```
-
-This is not necessary when you pass a mapping function:
-```python
-def map_parent(n: Node):
-    return n.parent
-
-assert stream.map(map_parent).next().get().name == "B"
-```
+## More features
 
 ### Typed dictionaries
 
 Dictionaries are streamed as `tuple(key, value)`
 
 ```python
 children = {"a": Node(name="Child")} 
@@ -111,21 +114,24 @@
 ```
 
 This is the same like (but without known types):
 ```python
 stream = Stream.of(children)
 ```
 
-## More features
-
 ### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
+### Filter by type
+```python
+nodes_only = Stream.of([child]).filter_type(Node)
+```
+
 ### Map object name attribute
 ```python
 names = Stream.of([child]).map_key("name")
 ```
 
 ### Deep mapping of name attributes
 ```python
```

### Comparing `tinystream-0.1.0/tinystream.egg-info/PKG-INFO` & `tinystream-0.1.1/tinystream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.1.0
+Version: 0.1.1
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
@@ -21,26 +21,57 @@
 ```python
 from tinystream import Stream
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
-    .filter(lambda x: x > 2) \    # filter_key()
+    .filter(lambda x: x > 2) \    # filter_key(), filter_type()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \
     .limit(2) \
     .concat([4]) \
     .sum()                        # reduce(), max(), min(), collect(), count()
 ```
 
 ## Aggregators
 
 Aggregator methods like `sum()`, `collect()`, `count()`... will end the stream.
 
+## Typehinting
+
+You can typehint datatypes like:
+
+```python
+from dataclasses import dataclass
+
+@dataclass
+class Node:
+    name: str
+    parent: "Node" = None
+
+parent = Node(name="B")
+child = Node(name="A", parent=parent)
+```
+
+for lambdas:
+
+```python
+stream = Stream.of([child])
+assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
+```
+
+This is not necessary when you pass a mapping function:
+```python
+def map_parent(n: Node):
+    return n.parent
+
+assert stream.map(map_parent).next().get().name == "B"
+```
+
 ## Built-in Optional support
 
 Some aggregator functions are *optional*:
 
 ```python
 assert Stream.of((1, 2, 3, 4, 5)).sum().empty is False
 ```
@@ -64,52 +95,24 @@
 assert Opt("String").map(len).get() == 6
 ```
 
 Get default value:
 ```python
 assert Opt(None).get(6) == 6
 assert Opt(None).get(lambda: 6) == 6
+assert Opt(None).if_empty(lambda: 3).empty is False
 ```
 
 Filter value:
 
 ```python
 assert Opt(0).filter(lambda x: x > 0).empty is True
 ```
 
-## Typehinting
-
-You can typehint datatypes like:
-
-```python
-from dataclasses import dataclass
-
-@dataclass
-class Node:
-    name: str
-    parent: "Node" = None
-
-parent = Node(name="B")
-child = Node(name="A", parent=parent)
-```
-
-for lambdas:
-
-```python
-stream = Stream.of([child])
-assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
-```
-
-This is not necessary when you pass a mapping function:
-```python
-def map_parent(n: Node):
-    return n.parent
-
-assert stream.map(map_parent).next().get().name == "B"
-```
+## More features
 
 ### Typed dictionaries
 
 Dictionaries are streamed as `tuple(key, value)`
 
 ```python
 children = {"a": Node(name="Child")} 
@@ -120,21 +123,24 @@
 ```
 
 This is the same like (but without known types):
 ```python
 stream = Stream.of(children)
 ```
 
-## More features
-
 ### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
+### Filter by type
+```python
+nodes_only = Stream.of([child]).filter_type(Node)
+```
+
 ### Map object name attribute
 ```python
 names = Stream.of([child]).map_key("name")
 ```
 
 ### Deep mapping of name attributes
 ```python
```

### Comparing `tinystream-0.1.0/tinystream.py` & `tinystream-0.1.1/tinystream.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 import functools
 import itertools
-import sys
-import warnings
 from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator, Generic, Type
 
 T = TypeVar("T")
 R = TypeVar("R")
 K = TypeVar("K")
 
 
 Mapper = Callable[[T], R]
 FlatMapper = Callable[[T], Iterable[R]]
 Consumer = Callable[[T], None]
 Comparator = Callable[[T, T], bool]
 Reducer = Callable[[T, T], R]
 Predicate = Callable[[T], bool]
+Supplier = Callable[[], T]
 
 
 class Opt(Generic[T]):
     def __init__(self, value: T):
         self.__val = value
 
     @property
     def empty(self):
         return self.__val is None
 
-    @property
-    def is_empty(self):
-        warnings.warn("Use empty property instead", DeprecationWarning)
-        return self.empty
-
     def get(self, *args) -> T:
         if not self.empty:
             return self.__val
         elif len(args) > 0:
             if isinstance(args[0], Callable):
                 return args[0]()
             else:
@@ -41,27 +35,35 @@
         else:
             raise Exception("Cannot get value of empty Opt without default value")
 
     def if_present(self, consumer: Consumer[T]):
         if not self.empty:
             consumer(self.get())
 
-    def or_else(self, consumer: Callable):
-        if self.empty:
-            return consumer()
-
     def filter(self, predicate: Predicate[T]):
         if predicate(self.__val):
             return self
         else:
             return Opt(None)
 
     def map(self, mapper: Mapper[T, R]):
         return Opt[R](mapper(self.__val))
 
+    def if_empty(self, supplier: Supplier[R]):
+        if self.empty:
+            return Opt[R](supplier())
+        else:
+            return self
+
+    def type(self, typehint: Type[R]) -> "Opt[R]":
+        return self
+
+    def filter_type(self, typehint: Type[R]) -> "Opt[R]":
+        return self.filter(lambda x: isinstance(x, typehint))
+
 
 class Stream:
 
     @staticmethod
     def of(iterable: Iterable[T]):
         return IterableStream[T](iterable)
 
@@ -95,35 +97,38 @@
         else:
             return iterable
 
     def __init__(self, iterable: Iterable[T]):
         self.__iterable = self.__normalize_iterator(iterable)
         self.__collected: List[T] = None
 
-    def map(self, mapper: Mapper[T, R], typehint: R = None):
+    def map(self, mapper: Mapper[T, R]):
         return IterableStream[R](map(mapper, self.__iterable))
 
-    def map_key(self, key: str | int, typehint: R = None) -> "IterableStream[R]":
+    def map_key(self, key: str | int):
         def __map_key(x):
             if isinstance(x, (list, dict, tuple)):
                 return x[key]
             else:
                 return getattr(x, key)
 
-        return self.filter_key(key).map(__map_key, R)
+        return self.filter_key(key).map(__map_key)
 
-    def map_keys(self, *iterables) -> "IterableStream":
+    def map_keys(self, *iterables):
         inst = self
         for key in iterables:
             inst = inst.map_key(key)
         return inst
 
-    def type(self, typehint: R) -> "IterableStream[R]":
+    def type(self, typehint: Type[R]) -> "IterableStream[R]":
         return self
 
+    def filter_type(self, typehint: Type[R]) -> "IterableStream[R]":
+        return self.filter(lambda x: isinstance(x, typehint))
+
     def filter(self, predicate: Predicate[T]):
         return IterableStream[T](filter(predicate, self.__iterable))
 
     def filter_key(self, key: str | int, invert: bool = False):
         def __filter_key(x):
             if isinstance(x, (list, tuple)):
                 size = len(x)
@@ -140,15 +145,15 @@
                 if invert:
                     return not hasattr(x, key)
                 else:
                     return hasattr(x, key)
 
         return self.filter(__filter_key)
 
-    def flatmap(self, mapper: FlatMapper[T, R] = None, typehint: R = None) -> "IterableStream[R]":
+    def flatmap(self, mapper: FlatMapper[T, R] = None):
 
         def __flatmap(f, xs):
             return (y for ys in xs for y in f(ys))
 
         def __flatten(xs):
             return (y for ys in xs for y in ys)
```

