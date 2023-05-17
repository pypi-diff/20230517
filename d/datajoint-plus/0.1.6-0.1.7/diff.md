# Comparing `tmp/datajoint-plus-0.1.6.tar.gz` & `tmp/datajoint-plus-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/stelios/Documents/PyPI/datajoint-plus/dist/tmpm8ha6x18/datajoint-plus-0.1.6.tar", last modified: Mon Oct  3 19:58:24 2022, max compression
+gzip compressed data, was "/home/stelios/Documents/PyPI/datajoint-plus/dist/tmpqnb8yl9r/datajoint-plus-0.1.7.tar", last modified: Wed May 17 18:48:19 2023, max compression
```

## Comparing `datajoint-plus-0.1.6.tar` & `datajoint-plus-0.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus/
--rw-rw-r--   0 root         (0) root         (0)     8339 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/table.py
--rw-rw-r--   0 root         (0) root         (0)     1815 2022-05-16 06:15:26.000000 datajoint-plus-0.1.6/datajoint_plus/motif_base.py
--rw-rw-r--   0 root         (0) root         (0)     1895 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/compatibility.py
--rw-rw-r--   0 root         (0) root         (0)      553 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/errors.py
--rw-rw-r--   0 root         (0) root         (0)     2046 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/user_tables.py
--rw-rw-r--   0 root         (0) root         (0)    46270 2022-10-03 19:58:12.000000 datajoint-plus-0.1.6/datajoint_plus/base.py
--rw-rw-r--   0 root         (0) root         (0)     3580 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/definition.py
--rw-rw-r--   0 root         (0) root         (0)     2485 2022-10-03 19:58:12.000000 datajoint-plus-0.1.6/datajoint_plus/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6591 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/logging.py
--rw-rw-r--   0 root         (0) root         (0)     2782 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/validation.py
--rw-rw-r--   0 root         (0) root         (0)     9210 2022-10-03 19:58:12.000000 datajoint-plus-0.1.6/datajoint_plus/schema.py
--rw-rw-r--   0 root         (0) root         (0)       22 2022-10-03 19:58:12.000000 datajoint-plus-0.1.6/datajoint_plus/version.py
--rw-rw-r--   0 root         (0) root         (0)    12161 2022-10-03 19:58:12.000000 datajoint-plus-0.1.6/datajoint_plus/utils.py
--rw-rw-r--   0 root         (0) root         (0)     2463 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/hash.py
--rw-rw-r--   0 root         (0) root         (0)     3687 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/heading.py
--rw-rw-r--   0 root         (0) root         (0)    12644 2022-05-16 06:15:26.000000 datajoint-plus-0.1.6/datajoint_plus/motif.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/
--rw-rw-r--   0 root         (0) root         (0)     2787 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/load_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/
--rw-rw-r--   0 root         (0) root         (0)      655 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/filehandler_rotating.yml
--rw-rw-r--   0 root         (0) root         (0)      666 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/filehandler_timed_rotating.yml
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      574 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/filehandler_basic.yml
--rw-rw-r--   0 root         (0) root         (0)      445 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/console.yml
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-11 06:04:22.000000 datajoint-plus-0.1.6/datajoint_plus/config/logging/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      450 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      197 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/datajoint_plus/enum.py
--rw-rw-r--   0 root         (0) root         (0)      104 2022-05-11 06:42:09.000000 datajoint-plus-0.1.6/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)      302 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       37 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1112 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/datajoint_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      302 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    26526 2022-05-10 16:16:25.000000 datajoint-plus-0.1.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       37 2022-05-12 18:03:03.000000 datajoint-plus-0.1.6/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      772 2022-05-11 08:05:49.000000 datajoint-plus-0.1.6/setup.py
--rw-rw-r--   0 root         (0) root         (0)    16097 2022-05-11 06:47:55.000000 datajoint-plus-0.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-03 19:58:24.000000 datajoint-plus-0.1.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus/
+-rw-rw-r--   0 root         (0) root         (0)     8339 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/table.py
+-rw-rw-r--   0 root         (0) root         (0)     1815 2022-05-16 06:15:26.000000 datajoint-plus-0.1.7/datajoint_plus/motif_base.py
+-rw-rw-r--   0 root         (0) root         (0)     1895 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/compatibility.py
+-rw-rw-r--   0 root         (0) root         (0)      553 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     2046 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/user_tables.py
+-rw-rw-r--   0 root         (0) root         (0)    46345 2023-05-17 18:47:21.000000 datajoint-plus-0.1.7/datajoint_plus/base.py
+-rw-rw-r--   0 root         (0) root         (0)     3580 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/definition.py
+-rw-rw-r--   0 root         (0) root         (0)     2485 2022-10-03 19:58:12.000000 datajoint-plus-0.1.7/datajoint_plus/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6591 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/logging.py
+-rw-rw-r--   0 root         (0) root         (0)     2782 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/validation.py
+-rw-rw-r--   0 root         (0) root         (0)     9122 2023-05-17 18:47:21.000000 datajoint-plus-0.1.7/datajoint_plus/schema.py
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-05-17 18:47:21.000000 datajoint-plus-0.1.7/datajoint_plus/version.py
+-rw-rw-r--   0 root         (0) root         (0)    11861 2023-05-17 18:47:21.000000 datajoint-plus-0.1.7/datajoint_plus/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2463 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/hash.py
+-rw-rw-r--   0 root         (0) root         (0)     3687 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/heading.py
+-rw-rw-r--   0 root         (0) root         (0)    12644 2022-05-16 06:15:26.000000 datajoint-plus-0.1.7/datajoint_plus/motif.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus/config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/
+-rw-rw-r--   0 root         (0) root         (0)     2787 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/load_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/
+-rw-rw-r--   0 root         (0) root         (0)      655 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/filehandler_rotating.yml
+-rw-rw-r--   0 root         (0) root         (0)      666 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/filehandler_timed_rotating.yml
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      574 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/filehandler_basic.yml
+-rw-rw-r--   0 root         (0) root         (0)      445 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/console.yml
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-05-11 06:04:22.000000 datajoint-plus-0.1.7/datajoint_plus/config/logging/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      450 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      197 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/datajoint_plus/enum.py
+-rw-rw-r--   0 root         (0) root         (0)      104 2022-05-11 06:42:09.000000 datajoint-plus-0.1.7/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/datajoint_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      302 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    26526 2022-05-10 16:16:25.000000 datajoint-plus-0.1.7/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       37 2022-05-12 18:03:03.000000 datajoint-plus-0.1.7/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      772 2022-05-11 08:05:49.000000 datajoint-plus-0.1.7/setup.py
+-rw-rw-r--   0 root         (0) root         (0)    16097 2022-05-11 06:47:55.000000 datajoint-plus-0.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 18:48:19.000000 datajoint-plus-0.1.7/setup.cfg
```

### Comparing `datajoint-plus-0.1.6/datajoint_plus/table.py` & `datajoint-plus-0.1.7/datajoint_plus/table.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/motif_base.py` & `datajoint-plus-0.1.7/datajoint_plus/motif_base.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/compatibility.py` & `datajoint-plus-0.1.7/datajoint_plus/compatibility.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/errors.py` & `datajoint-plus-0.1.7/datajoint_plus/errors.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/user_tables.py` & `datajoint-plus-0.1.7/datajoint_plus/user_tables.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/base.py` & `datajoint-plus-0.1.7/datajoint_plus/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,19 +130,19 @@
         # ensure "index" not in attributes
         if "index" in cls.heading.names:
             raise AttributeError(f'Attributes cannot be named "index". There is a bug in this DJ version that does not handle this keyword correctly with respect to MySQL.')
 
         cls._is_insert_validated = True
 
     @classmethod
-    def load_dependencies(cls, force=True, verbose=True):
+    def load_dependencies(cls, force=True):
         """
         Loads dependencies into DataJoint networkx graph. 
         """
-        load_dependencies(cls.connection, force=force, verbose=verbose)
+        load_dependencies(cls.connection, force=force)
 
 
     @classmethod
     def add_constant_attrs_to_rows(cls, rows, constant_attrs:dict={}, overwrite_rows=False):
         """
         Adds attributes to all rows.
         Warning: rows must be able to be safely converted into a pandas dataframe.
@@ -576,14 +576,15 @@
         :param as_cls:
             If True, returns part table classes (will override as_objects)
         :param reload_dependencies: 
             If True, will force reload Datajoint networkx graph dependencies. 
 
         :returns: list
         """
+        # TODO: possibly not needed to reload dependencies if just looking through codebase (as_cls=True)
         if not cls.connection.dependencies._loaded or reload_dependencies:
             cls.load_dependencies()
 
         cls_parts = [getattr(cls, d) for d in dir(cls) if inspect.isclass(getattr(cls, d)) and issubclass(getattr(cls, d), dj.Part)]
         for cls_part in [p.full_table_name for p in cls_parts]:
             if cls_part not in super().parts(cls):
                 logger.warning('Part table defined in class definition not found in DataJoint graph. Reload dependencies.')
```

### Comparing `datajoint-plus-0.1.6/datajoint_plus/definition.py` & `datajoint-plus-0.1.7/datajoint_plus/definition.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/__init__.py` & `datajoint-plus-0.1.7/datajoint_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/logging.py` & `datajoint-plus-0.1.7/datajoint_plus/logging.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/validation.py` & `datajoint-plus-0.1.7/datajoint_plus/validation.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/schema.py` & `datajoint-plus-0.1.7/datajoint_plus/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     _, name = split_full_table_name(key['full_table_name'])
                     if name not in self.list_tables():
                         self.tables(full_table_name=key['full_table_name'], action='delete')
             except:
                 logger.warning('Could not update schema.tables')
         
         if load_dependencies:
-            self.load_dependencies(verbose=False)
+            self.load_dependencies()
 
 
     @classproperty
     def is_schema(cls):
         True
 
     @property
@@ -72,19 +72,19 @@
             except ValueError:
                 raise ValueError('Split full_table_name failed. Did you pass a table_name in full_table_name arg?')
             assert database == self.database, table_not_in_schema
         else:
             raise AttributeError('Provide table_name or full_table_name.')
         return FreeTable(self.connection, full_table_name)
     
-    def load_dependencies(self, force=True, verbose=True):
+    def load_dependencies(self, force=True):
         """
         Loads dependencies into DataJoint networkx graph. 
         """
-        load_dependencies(self.connection, force=force, verbose=verbose)
+        load_dependencies(self.connection, force=force)
 
 
 class VirtualModule(types.ModuleType):
     """
     A virtual module which will contain context for schema.
     """
     def __init__(self, module_name, schema_name, *, create_schema=False,
@@ -170,16 +170,16 @@
         if add_externals:
             register_externals(add_externals)
         
         if enable_dj_flags:
             enable_datajoint_flags()
         
         if load_dependencies:
-            self.load_dependencies(verbose=False)
+            self.load_dependencies()
 
         add_datajoint_plus(self)
 
-    def load_dependencies(self, verbose=True):
+    def load_dependencies(self):
         """
         Loads dependencies into DataJoint networkx graph. 
         """
-        load_dependencies(connection=self.schema.connection, force=True, verbose=verbose)
+        load_dependencies(connection=self.schema.connection, force=True)
```

### Comparing `datajoint-plus-0.1.6/datajoint_plus/utils.py` & `datajoint-plus-0.1.7/datajoint_plus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """General-purpose utilities"""
 
 import inspect
 import logging
 import re
 import sys
 from unittest import mock
+import os
 
 import numpy as np
 import pandas as pd
 import requests
 from datajoint.errors import _support_adapted_types, _switch_adapted_types, _support_filepath_types, _switch_filepath_types
 from datajoint.table import QueryExpression
 from datajoint.user_tables import UserTable
@@ -105,34 +106,26 @@
         rows = pd.DataFrame(rows)
     else:
         raise ValidationError('Format of rows not recognized. Try a list of dictionaries, a DataJoint expression, a DataJoint fetch object, or a pandas dataframe.')
 
     return rows
 
 
-def load_dependencies(connection, force=False, verbose=True):
+def load_dependencies(connection, force=False):
     """
     Loads dependencies in a DataJoint connection object.
 
     :param connection: (datajoint.connection) DataJoint connection object 
     :param force: (bool) default False. Whether to force reload.
     """
-    if verbose:
-        if force:
-            output = Output()
-            display(output)
-            with output:
-                pending_text = Label('Loading schema dependencies...')
-                confirmation = Label('Success.')
-                confirmation.layout.display = 'none'
-                display(HBox([pending_text, confirmation]))
-                connection.dependencies.load()
-                confirmation.layout.display = None
-    else:
-        connection.dependencies.load(force=force)
+    if connection.dependencies._loaded and not force:
+        return
+    logger.info('Loading schema dependencies...')
+    connection.dependencies.load(force=force)
+    logger.info('Schema dependencies loaded.')
 
 
 def enable_datajoint_flags(enable_python_native_blobs=True, support_adapted_types=True, support_filepath_types=True):
     """
     Enable experimental datajoint features
     
     These flags are required by 0.12.0+ (for now).
```

### Comparing `datajoint-plus-0.1.6/datajoint_plus/hash.py` & `datajoint-plus-0.1.7/datajoint_plus/hash.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/heading.py` & `datajoint-plus-0.1.7/datajoint_plus/heading.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/motif.py` & `datajoint-plus-0.1.7/datajoint_plus/motif.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/config/logging/load_config.py` & `datajoint-plus-0.1.7/datajoint_plus/config/logging/load_config.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/filehandler_rotating.yml` & `datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/filehandler_rotating.yml`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/filehandler_timed_rotating.yml` & `datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/filehandler_timed_rotating.yml`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus/config/logging/templates/filehandler_basic.yml` & `datajoint-plus-0.1.7/datajoint_plus/config/logging/templates/filehandler_basic.yml`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/datajoint_plus.egg-info/SOURCES.txt` & `datajoint-plus-0.1.7/datajoint_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/LICENSE` & `datajoint-plus-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/setup.py` & `datajoint-plus-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `datajoint-plus-0.1.6/README.md` & `datajoint-plus-0.1.7/README.md`

 * *Files identical despite different names*

