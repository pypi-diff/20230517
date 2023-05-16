# Comparing `tmp/jsoninja-1.0.2.tar.gz` & `tmp/jsoninja-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jsoninja/jsoninja/dist/.tmp-skm1qpbh/jsoninja-1.0.2.tar", last modified: Sat Apr 29 22:05:37 2023, max compression
+gzip compressed data, was "/home/runner/work/jsoninja/jsoninja/dist/.tmp-z7dwm9sf/jsoninja-1.0.3.tar", last modified: Tue May 16 23:36:38 2023, max compression
```

## Comparing `jsoninja-1.0.2.tar` & `jsoninja-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:05:37.000000 jsoninja-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-29 22:05:28.000000 jsoninja-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-29 22:05:37.000000 jsoninja-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-29 22:05:28.000000 jsoninja-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:05:37.000000 jsoninja-1.0.2/jsoninja/
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-29 22:05:28.000000 jsoninja-1.0.2/jsoninja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:05:37.000000 jsoninja-1.0.2/jsoninja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-29 22:05:37.000000 jsoninja-1.0.2/jsoninja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-29 22:05:37.000000 jsoninja-1.0.2/jsoninja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 22:05:37.000000 jsoninja-1.0.2/jsoninja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-29 22:05:37.000000 jsoninja-1.0.2/jsoninja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 22:05:37.000000 jsoninja-1.0.2/jsoninja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-29 22:05:28.000000 jsoninja-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 22:05:37.000000 jsoninja-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:36:38.000000 jsoninja-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 23:36:29.000000 jsoninja-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-16 23:36:38.000000 jsoninja-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-16 23:36:29.000000 jsoninja-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:36:38.000000 jsoninja-1.0.3/jsoninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-16 23:36:29.000000 jsoninja-1.0.3/jsoninja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:36:38.000000 jsoninja-1.0.3/jsoninja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-16 23:36:38.000000 jsoninja-1.0.3/jsoninja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 23:36:38.000000 jsoninja-1.0.3/jsoninja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:36:38.000000 jsoninja-1.0.3/jsoninja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 23:36:38.000000 jsoninja-1.0.3/jsoninja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 23:36:38.000000 jsoninja-1.0.3/jsoninja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-16 23:36:29.000000 jsoninja-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:36:38.000000 jsoninja-1.0.3/setup.cfg
```

### Comparing `jsoninja-1.0.2/LICENSE` & `jsoninja-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsoninja-1.0.2/PKG-INFO` & `jsoninja-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoninja
-Version: 1.0.2
+Version: 1.0.3
 Summary: Jsoninja is a library that allows you to generate JSON's from templates written with Python data types.
 Author-email: Víctor Lázaro <vlazaro@outlook.es>
 License: MIT License
         
         Copyright (c) 2023 Víctor Lázaro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsoninja-1.0.2/README.md` & `jsoninja-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jsoninja-1.0.2/jsoninja/__init__.py` & `jsoninja-1.0.3/jsoninja/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 """
 
 import copy
 import re
 from typing import Any, Dict, List, Union
 
 
+class NoReplacement:
+    """
+    Class for representing an empty type when there is no replacement.
+    """
+
+
 class Jsoninja:
     """
     Class that contains the necessary methods of Jsoninja.
     """
 
     def __init__(self) -> None:
         """
@@ -133,15 +139,15 @@
         Args:
             structure (list | dict): Declares the structure and variables.
             replacements (dict): The values to be used as replacements.
             key (Any): The key of the node.
             variable (Any): The template variable.
         """
         replacement = self.__get_replacement(variable, replacements)
-        if replacement is not None:
+        if not isinstance(replacement, NoReplacement):
             if callable(replacement):
                 structure[key] = replacement()
             else:
                 structure[key] = replacement
 
     def __get_replacement(self, variable: Any, replacements: Dict[str, Any]) -> Any:
         """
@@ -153,23 +159,23 @@
 
         Returns:
             The replacement associated for the template variable or None.
 
         Raises:
             KeyError: Unable to find a replacement for "...".
         """
-        replacement: Any = None
+        replacement: Any = NoReplacement()
         matches = self.__variable_regex.finditer(str(variable))
         for match in matches:
             var_name = self.__clean_variable(match.group(0))
             if var_name not in replacements:
                 raise KeyError(f'Unable to find a replacement for "{var_name}".')
             if match.group(0) == variable:
                 return replacements[var_name]
-            if replacement is None:
+            if isinstance(replacement, NoReplacement):
                 replacement = variable
             replacement = replacement.replace(match.group(0), replacements[var_name])
         return replacement
 
     def __clean_variable(self, variable: str) -> str:
         """
         Removes the brackets that declare the template variable.
```

### Comparing `jsoninja-1.0.2/jsoninja.egg-info/PKG-INFO` & `jsoninja-1.0.3/jsoninja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoninja
-Version: 1.0.2
+Version: 1.0.3
 Summary: Jsoninja is a library that allows you to generate JSON's from templates written with Python data types.
 Author-email: Víctor Lázaro <vlazaro@outlook.es>
 License: MIT License
         
         Copyright (c) 2023 Víctor Lázaro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsoninja-1.0.2/pyproject.toml` & `jsoninja-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsoninja"
-version = "1.0.2"
+version = "1.0.3"
 description = "Jsoninja is a library that allows you to generate JSON's from templates written with Python data types."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 authors = [
     { name = "Víctor Lázaro", email = "vlazaro@outlook.es" },
 ]
```

