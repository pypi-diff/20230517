# Comparing `tmp/hprint-2.0.4.tar.gz` & `tmp/hprint-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hprint-2.0.4.tar", last modified: Sun Jan 22 09:12:30 2023, max compression
+gzip compressed data, was "hprint-2.0.5.tar", last modified: Wed May 17 10:00:12 2023, max compression
```

## Comparing `hprint-2.0.4.tar` & `hprint-2.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-01-22 09:12:30.285650 hprint-2.0.4/
--rw-r--r--   0 haoru      (501) staff       (20)     1065 2022-12-17 06:41:01.000000 hprint-2.0.4/LICENSE
--rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-01-22 09:12:30.285879 hprint-2.0.4/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)     4211 2022-12-24 13:51:04.000000 hprint-2.0.4/README.md
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-01-22 09:12:30.282027 hprint-2.0.4/hprint/
--rw-r--r--   0 haoru      (501) staff       (20)     4501 2023-01-22 09:09:06.000000 hprint-2.0.4/hprint/__init__.py
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-01-22 09:12:30.285165 hprint-2.0.4/hprint.egg-info/
--rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-01-22 09:12:30.000000 hprint-2.0.4/hprint.egg-info/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)      204 2023-01-22 09:12:30.000000 hprint-2.0.4/hprint.egg-info/SOURCES.txt
--rw-r--r--   0 haoru      (501) staff       (20)        1 2023-01-22 09:12:30.000000 hprint-2.0.4/hprint.egg-info/dependency_links.txt
--rw-r--r--   0 haoru      (501) staff       (20)        9 2023-01-22 09:12:30.000000 hprint-2.0.4/hprint.egg-info/requires.txt
--rw-r--r--   0 haoru      (501) staff       (20)        7 2023-01-22 09:12:30.000000 hprint-2.0.4/hprint.egg-info/top_level.txt
--rw-r--r--   0 haoru      (501) staff       (20)      235 2023-01-22 09:12:30.286778 hprint-2.0.4/setup.cfg
--rw-r--r--   0 haoru      (501) staff       (20)     1506 2023-01-22 09:11:32.000000 hprint-2.0.4/setup.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-05-17 10:00:12.783317 hprint-2.0.5/
+-rw-r--r--   0 haoru      (501) staff       (20)     1065 2022-12-17 06:41:01.000000 hprint-2.0.5/LICENSE
+-rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-05-17 10:00:12.783472 hprint-2.0.5/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)     4211 2022-12-24 13:51:04.000000 hprint-2.0.5/README.md
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-05-17 10:00:12.780314 hprint-2.0.5/hprint/
+-rw-r--r--   0 haoru      (501) staff       (20)     5204 2023-04-15 04:09:13.000000 hprint-2.0.5/hprint/__init__.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-05-17 10:00:12.782779 hprint-2.0.5/hprint.egg-info/
+-rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)      204 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/SOURCES.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        1 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/dependency_links.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        9 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/requires.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        7 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/top_level.txt
+-rw-r--r--   0 haoru      (501) staff       (20)      235 2023-05-17 10:00:12.784134 hprint-2.0.5/setup.cfg
+-rw-r--r--   0 haoru      (501) staff       (20)     1506 2023-05-17 09:59:30.000000 hprint-2.0.5/setup.py
```

### Comparing `hprint-2.0.4/LICENSE` & `hprint-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hprint-2.0.4/PKG-INFO` & `hprint-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hprint
-Version: 2.0.4
+Version: 2.0.5
 Summary: Print python object in table/json format
 Home-page: https://github.com/ruanhao/hprint
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: utils,print,json
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hprint-2.0.4/README.md` & `hprint-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hprint-2.0.4/hprint/__init__.py` & `hprint-2.0.5/hprint/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from functools import partial
 from tabulate import tabulate
 import json
 from pprint import pformat
 import os
 import traceback
 import logging
+import textwrap
 
 _print = partial(print, flush=True)
 
-HPRINT_WRAP = os.getenv("HPRINT_WRAP", 50)
+HPRINT_WRAP = int(os.getenv("HPRINT_WRAP", 50))
 
 logger = logging.getLogger(__name__)
 
 HPRINT_DEBUG = os.getenv("HPRINT_DEBUG")
 
 __all__ = ['pretty_print', 'hprint']
 
@@ -24,33 +25,40 @@
 def json_print(data):
     if isinstance(data, dict):
         _print(json.dumps(data, indent=4, sort_keys=True))
     elif isinstance(data, list):
         try:
             _print(json.dumps([dict(d) for d in data], indent=4, sort_keys=True))
         except Exception:
-            _pprint([dict(d) for d in data])
+            try:
+                _pprint([dict(d) for d in data])
+            except Exception:
+                _pprint(data)
     else:
         _pprint(data)
 
 
 def _chain_get(data, chain, default=None):
     attrs = chain.split('.')
     if len(attrs) == 1:
         return data.get(attrs[0], default)
     result = data
     for attr in attrs[:-1]:
         result = result.get(attr, {})
     return result.get(attrs[-1], default)
 
 
-def _get(obj, key, default='n/a'):
+def _get(obj, key, default='[none]'):
     if not key:
         return obj
-    return _chain_get(obj, key, default)
+    # return _chain_get(obj, key, default)
+    result = _chain_get(obj, key, default)
+    if result is None:
+        return default
+    return result
 
 
 def tabulate_numbered_print(data, mappings, offset=0):
     if not data:
         return
     if not mappings:
         mappings = {k: k for k in data[0]}
@@ -74,38 +82,47 @@
 def _len(x):
     return min(len(str(x)), HPRINT_WRAP)
 
 
 def _indent(s: str, indent_cols, max_cols):
     lines = s.splitlines()
     if len(lines) <= 1:
-        return s.ljust(max_cols)
+        lines = textwrap.wrap(s, max_cols)
+        if len(lines) <= 1:
+            return s.ljust(max_cols)
     return lines[0] + '\n' + '\n'.join([(' ' * indent_cols + "| " + line) for line in lines[1:]])
 
 
 def x_print(records, headers, offset=0, header=True):
     headers = list(headers)
     left_max_len = max(len(max(headers, key=len)), len(f"-[ RECORD {len(records)} ]-")) + 1
     right_max_len = max(_len(max(record, key=_len)) for record in records) + 1
+    output = []
     for i, record in enumerate(records, 1 + offset):
         if header:
-            _print(f'-[ RECORD {i} ]'.ljust(left_max_len, '-') + '+' + '-' * right_max_len)
+            output.append(f'-[ RECORD {i} ]'.ljust(left_max_len, '-') + '+' + '-' * right_max_len)
+            # _print(f'-[ RECORD {i} ]'.ljust(left_max_len, '-') + '+' + '-' * right_max_len)
         for j, v in enumerate(record):
             # _print(f'{headers[j]}'.ljust(left_max_len) + '| ' + str(v).ljust(right_max_len))
-            _print(f'{headers[j]}'.ljust(left_max_len) + '| ' + _indent(str(v), left_max_len, right_max_len))
+            output.append(f'{headers[j]}'.ljust(left_max_len) + '| ' + _indent(str(v), left_max_len, right_max_len))
+            # _print(f'{headers[j]}'.ljust(left_max_len) + '| ' + _indent(str(v), left_max_len, right_max_len))
+    return os.linesep.join(output)
 
 
 def tabulate_print(data, mappings, x=False, offset=0, header=True, raw=False, tf='simple'):
     if not data:
         return
     if not mappings:
-        keys = set()
+        mappings = {}
+        # keys = set()
         for entry in data:
-            keys = keys.union(entry.keys())
-        mappings = {k: k for k in keys}
+            # keys = keys.union(entry.keys())
+            for k in entry.keys():
+                mappings[k] = k
+        # mappings = {k: k for k in keys}
         # entry_with_most_keys = max(data, key=len)
         # mappings = {k: k for k in entry_with_most_keys.keys()}
     headers = mappings.keys()
     tabdata = []
     for item in data:
         attrs = []
         for h in headers:
@@ -113,31 +130,33 @@
             if isinstance(k, tuple):
                 (k0, func) = k
                 attrs.append(func(_get(item, k0)))
             else:
                 attrs.append(_get(item, k))
         tabdata.append(attrs)
     if x:
-        x_print(tabdata, headers, offset=offset, header=header)
+        output = x_print(tabdata, headers, offset=offset, header=header)
     else:
         output = tabulate(tabdata, headers=headers if header else (), tablefmt=tf)
-        if raw:
-            return output
-        _print(output)
+    if raw:
+        return output
+    _print(output)
 
 
-def hprint(data, *, mappings=None, json_format=False, as_json=False, x=False, offset=0, numbered=False, missing_value='n/a', tf='simple', header=True, raw=False):
+def hprint(data, *, mappings=None, json_format=False, as_json=False, x=False, offset=0, numbered=False, missing_value='[none]', tf='simple', header=True, raw=False):
     as_json = as_json or json_format
     if not data:
         return
     global _get
     _get0 = _get
     _get = partial(_get, default=missing_value)
     try:
         if as_json:
+            if raw:
+                return data
             json_print(data)
         elif not x and numbered:
             tabulate_numbered_print(data, mappings, offset=offset)
         else:
             return tabulate_print(data, mappings=mappings, x=x, offset=offset, header=header, raw=raw, tf=tf)
     except Exception:
         json_print(data)
```

### Comparing `hprint-2.0.4/hprint.egg-info/PKG-INFO` & `hprint-2.0.5/hprint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hprint
-Version: 2.0.4
+Version: 2.0.5
 Summary: Print python object in table/json format
 Home-page: https://github.com/ruanhao/hprint
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: utils,print,json
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hprint-2.0.4/setup.py` & `hprint-2.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'license': 'MIT',
     "long_description": long_description,
     "long_description_content_type": 'text/markdown',
     'description': 'Print python object in table/json format',
     'author' : 'Hao Ruan',
     'author_email': 'ruanhao1116@gmail.com',
     'keywords': ['utils', 'print', 'json'],
-    'version': '2.0.4',
+    'version': '2.0.5',
     'packages': ['hprint'],
     'install_requires': [
         'tabulate',
     ],
     'python_requires': ">=3.7, <4",
     'setup_requires': ['wheel'],
     'classifiers': [
```

