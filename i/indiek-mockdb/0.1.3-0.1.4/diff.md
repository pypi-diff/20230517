# Comparing `tmp/indiek-mockdb-0.1.3.tar.gz` & `tmp/indiek-mockdb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-ltlhbuh_/indiek-mockdb-0.1.3.tar", last modified: Tue May  9 22:07:37 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-xdocv56k/indiek-mockdb-0.1.4.tar", last modified: Wed May 17 01:33:56 2023, max compression
```

## Comparing `indiek-mockdb-0.1.3.tar` & `indiek-mockdb-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.3/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/PKG-INFO
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.829270 indiek-mockdb-0.1.3/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/indiek/mockdb/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.3/indiek/mockdb/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     5878 2023-05-08 22:01:42.000000 indiek-mockdb-0.1.3/indiek/mockdb/items.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      279 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      618 2023-05-07 14:33:45.000000 indiek-mockdb-0.1.3/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1338 2023-05-07 18:04:47.000000 indiek-mockdb-0.1.3/tests/test_items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-17 01:33:56.891425 indiek-mockdb-0.1.4/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.4/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-17 01:33:56.891425 indiek-mockdb-0.1.4/PKG-INFO
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-17 01:33:56.867424 indiek-mockdb-0.1.4/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-17 01:33:56.891425 indiek-mockdb-0.1.4/indiek/mockdb/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.4/indiek/mockdb/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     5620 2023-05-11 10:29:28.000000 indiek-mockdb-0.1.4/indiek/mockdb/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      246 2023-05-17 01:29:31.000000 indiek-mockdb-0.1.4/indiek/mockdb/persistence.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-17 01:33:56.891425 indiek-mockdb-0.1.4/indiek_mockdb.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-17 01:33:56.000000 indiek-mockdb-0.1.4/indiek_mockdb.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      308 2023-05-17 01:33:56.000000 indiek-mockdb-0.1.4/indiek_mockdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-17 01:33:56.000000 indiek-mockdb-0.1.4/indiek_mockdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-05-17 01:33:56.000000 indiek-mockdb-0.1.4/indiek_mockdb.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-17 01:33:56.000000 indiek-mockdb-0.1.4/indiek_mockdb.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-17 01:33:56.891425 indiek-mockdb-0.1.4/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      656 2023-05-09 23:27:45.000000 indiek-mockdb-0.1.4/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-17 01:33:56.891425 indiek-mockdb-0.1.4/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3766 2023-05-10 09:58:53.000000 indiek-mockdb-0.1.4/tests/test_items.py
```

### Comparing `indiek-mockdb-0.1.3/LICENSE` & `indiek-mockdb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-mockdb-0.1.3/indiek/mockdb/items.py` & `indiek-mockdb-0.1.4/indiek/mockdb/items.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from __future__ import annotations
 import re
-from typing import Sequence, Dict, Optional, List, Any
+from typing import Sequence, Optional, List, Any
+from frozendict import frozendict
+
+
+class MixedTypeOverrideError(Exception):
+    """
+    An item is trying to be saved with an ID 
+    pertaining to an existing item of a different type.
+    """
+    pass
 
 
 def generate_id(existing: Sequence[int]) -> int:
     """Generate ID."""
     return max(existing) + 1 if len(existing) else 0
 
 
@@ -18,31 +27,39 @@
 
     Attributes:
         name (str): item name.
         content (str): item content.
         _ikid (int): ID of item in mockdb. This is not part of indiek-core API.
     """
 
-    _item_dict = {}
-    """All items are stored in this class variable that maps item unique ID to their content."""
+    _item_dict = frozendict(
+        Definition = {},  # keys MUST match class names from module
+        Theorem = {},
+        Proof = {},
+    )
+    """
+    All items are stored in this class variable. It is a nested dict. First level of 
+    keys are classes, and values are dicts. Second level of keys are item unique IDs 
+    (_ikid) and values are dicts containing item data."""
+
+    _attr_defs = ['name', 'content', '_ikid']
+    """List of attr that fully define an Item."""
 
     def __repr__(self):
         _ikid = self._ikid
         name = self.name
         content_hash = hash(self.content)
         return f"MockDB Item:{_ikid=};{name=};{content_hash=}"
 
     def __str__(self):
         return f"MockDB Item with ID {self._ikid} and name {self.name}"
 
     def __eq__(self, other) -> bool:
-        cond = self._ikid == other._ikid
-        cond = cond and self.name == other.name
-        cond = cond and self.content == other.content
-        return cond and isinstance(other, self.__class__)
+        attr_eq = all(getattr(self, a) == getattr(other, a) for a in Item._attr_defs)
+        return attr_eq and type(other) == type(self)
 
     def __init__(
             self, *,
             name: str = '',
             content: str = '',
             _ikid: Optional[int] = None
     ):
@@ -55,43 +72,66 @@
                 item in the DB and a save operation occurs later on, the existing data will be overriden.
         """
         self._ikid = _ikid
         self.name = name
         self.content = content
 
     def save(self):
-        raise NotImplementedError(
-            f"Use specific Item type (subclass of {self.__class__.__name__}) to save.")
+        myclass = self.__class__.__name__
+
+        # check existing ids
+        existing_ids = set.union(*(set(d.keys()) for d in self._item_dict.values()))
+
+        if self._ikid is not None:  # item has an ID
+            if self._ikid in existing_ids:  # ID already present in DB
+                if self._ikid not in self._item_dict[myclass].keys():  # ID belongs to another type
+                    raise MixedTypeOverrideError()
+                # at this level we are dealing with an override; relegated to end of function
+                
+        else:  # we generate the ID
+            self._ikid = generate_id(existing_ids)
+
+        # we write or override safely
+        self._item_dict[myclass][self._ikid] = self.to_dict()
+        return self._ikid
 
     def to_dict(self):
         """Return mockdb Item instance content as dict.
 
         Returns:
             dict: mockdb Item instance
         """
-        return {
-            '_ikid': self._ikid,
-            'name': self.name,
-            'content': self.content
-        }
+        return {a: getattr(self, a) for a in self._attr_defs}
+    
+    def delete(self):
+        if self._ikid is not None:
+            self._item_dict[self.__class__.__name__].pop(self._ikid)
+            self._ikid = None
+
+    def reload(self):
+        """Reload written values if _ikid exists otherwise nothing happens."""
+        if self._ikid is not None:
+            written = self._item_dict[self.__class__.__name__][self._ikid]
+            for attribute in self._attr_defs:
+                setattr(self, attribute, written[attribute])
     
     @classmethod
     def str_filter(cls, regex: re.Pattern):
-        """Acts as list_all, but only returns items with regex match.
+        """Return list of items from specified class with a regex match.
 
         Regex is applied on name and content attr.
 
         Args:
             regex (re.Pattern): regex to match
 
         Returns:
             List[Item]: filtered list of stored items
         """
         filtered_dicts = []
-        for item_dict in cls._item_dict.values():
+        for item_dict in cls._item_dict[cls.__name__].values():
             if regex.search(item_dict['name']):
                 filtered_dicts.append(item_dict)
                 continue
             if regex.search(item_dict['content']):
                 filtered_dicts.append(item_dict)
 
         return [cls(**item_dict) for item_dict in filtered_dicts]
@@ -114,88 +154,29 @@
 
         Args:
             _ikid (int): item ID in mockdb.
 
         Returns:
             Item: mockdb Item instance
         """
-        dict_ = cls._item_dict[_ikid]
+        dict_ = cls._item_dict[cls.__name__][_ikid]
         return cls(**dict_)
 
     @classmethod
     def list_all(cls) -> List[Item]:
         """Fetch all stored mockdb items as a list.
 
         Returns:
             List[Item]: stored items.
         """
-        return [cls(**item_dict) for item_dict in cls._item_dict.values()]
+        class_items = cls._item_dict[cls.__name__]
+        return [cls(**item_dict) for item_dict in class_items.values()]
 
 
 class Definition(Item):
-    _item_dict = {}
-    """All definition items are stored in this class variable that maps item unique ID to their content."""
-
-    def save(self) -> int:
-        """Save instance data into mockdb.
-
-        If the instance doesn't have an id, (`ikid` attr), a new unique one (at global Item level)
-        is generated add added before saving.
-
-        Returns:
-            int: _ikid of item
-        """
-        if self._ikid is None:
-            self._ikid = generate_id(super()._item_dict.keys())
-
-        # update type-specific dict
-        self._item_dict[self._ikid] = self.to_dict()
-
-        # update generic Item dict
-        super()._item_dict[self._ikid] = self.to_dict()
-        return self._ikid
-
+    pass
 
 class Theorem(Item):
-    _item_dict = {}
-
-    def save(self) -> int:
-        """Save instance data into mockdb.
-
-        If the instance doesn't have an id, (`ikid` attr), a new unique one (at global Item level)
-        is generated add added before saving.
-
-        Returns:
-            int: _ikid of item
-        """
-        if self._ikid is None:
-            self._ikid = generate_id(super()._item_dict.keys())
-
-        # update type-specific dict
-        self._item_dict[self._ikid] = self.to_dict()
-
-        # update generic Item dict
-        super()._item_dict[self._ikid] = self.to_dict()
-        return self._ikid
-
+    pass
 
 class Proof(Item):
-    _item_dict = {}
-
-    def save(self) -> int:
-        """Save instance data into mockdb.
-
-        If the instance doesn't have an id, (`ikid` attr), a new unique one (at global Item level)
-        is generated add added before saving.
-
-        Returns:
-            int: _ikid of item
-        """
-        if self._ikid is None:
-            self._ikid = generate_id(super()._item_dict.keys())
-
-        # update type-specific dict
-        self._item_dict[self._ikid] = self.to_dict()
-
-        # update generic Item dict
-        super()._item_dict[self._ikid] = self.to_dict()
-        return self._ikid
+    pass
```

### Comparing `indiek-mockdb-0.1.3/setup.py` & `indiek-mockdb-0.1.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 
 setup(name='indiek-mockdb',
       python_requires='>=3.8',
-      version='0.1.3',
+      version='0.1.4',
       description='mock database for indiek',
       long_description='''This is an on-the-fly in-memory mock Database used by indiek-core
       for development and testing purposes. The versioning of this library is locked with that
       of indiek-core.''',
       author='Adrian Ernesto Radillo',
       author_email='adrian.radillo@gmail.com',
       license='GNU Affero General Public License v3.0',
       packages=['indiek.mockdb'],
+      install_require=['frozendict'],
       extras_require={'dev': ['pytest', 'pytest-pep8', 'pytest-cov']})
```

