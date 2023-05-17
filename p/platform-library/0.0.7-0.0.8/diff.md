# Comparing `tmp/platform-library-0.0.7.tar.gz` & `tmp/platform-library-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-library-0.0.7.tar", last modified: Mon May 15 12:18:35 2023, max compression
+gzip compressed data, was "platform-library-0.0.8.tar", last modified: Wed May 17 10:19:24 2023, max compression
```

## Comparing `platform-library-0.0.7.tar` & `platform-library-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.677415 platform-library-0.0.7/
--rw-r--r--   0 Artyom     (501) staff       (20)     1078 2022-11-08 13:08:16.000000 platform-library-0.0.7/LICENSE
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-15 12:18:35.677298 platform-library-0.0.7/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.0.7/README-public.md
--rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.0.7/README.md
--rw-r--r--   0 Artyom     (501) staff       (20)      593 2023-05-15 12:18:09.000000 platform-library-0.0.7/pyproject.toml
--rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-05-15 12:18:35.677452 platform-library-0.0.7/setup.cfg
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.674019 platform-library-0.0.7/src/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.675549 platform-library-0.0.7/src/platform_library.egg-info/
--rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/PKG-INFO
--rw-r--r--   0 Artyom     (501) staff       (20)      509 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/SOURCES.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/dependency_links.txt
--rw-r--r--   0 Artyom     (501) staff       (20)       51 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/requires.txt
--rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-05-15 12:18:35.000000 platform-library-0.0.7/src/platform_library.egg-info/top_level.txt
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.674213 platform-library-0.0.7/src/plib/
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.676369 platform-library-0.0.7/src/plib/auth/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/encrypt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/jwt.py
--rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.0.7/src/plib/auth/o2auth.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.676767 platform-library-0.0.7/src/plib/licensing/
--rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.0.7/src/plib/licensing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     4037 2023-05-11 06:38:08.000000 platform-library-0.0.7/src/plib/licensing/api.py
--rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.0.7/src/plib/licensing/exceptions.py
-drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-15 12:18:35.677137 platform-library-0.0.7/src/plib/tracing/
--rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.0.7/src/plib/tracing/__init__.py
--rw-r--r--   0 Artyom     (501) staff       (20)     3019 2023-05-15 12:18:09.000000 platform-library-0.0.7/src/plib/tracing/utils.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.637162 platform-library-0.0.8/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1078 2023-05-17 10:19:03.000000 platform-library-0.0.8/LICENSE
+-rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-17 10:19:24.637008 platform-library-0.0.8/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)       50 2023-03-06 08:11:34.000000 platform-library-0.0.8/README-public.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      524 2023-03-06 07:49:45.000000 platform-library-0.0.8/README.md
+-rw-r--r--   0 Artyom     (501) staff       (20)      593 2023-05-17 10:18:00.000000 platform-library-0.0.8/pyproject.toml
+-rw-r--r--   0 Artyom     (501) staff       (20)       38 2023-05-17 10:19:24.637231 platform-library-0.0.8/setup.cfg
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.633459 platform-library-0.0.8/src/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.635109 platform-library-0.0.8/src/platform_library.egg-info/
+-rw-r--r--   0 Artyom     (501) staff       (20)     1696 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/PKG-INFO
+-rw-r--r--   0 Artyom     (501) staff       (20)      509 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/SOURCES.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        1 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/dependency_links.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)       51 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/requires.txt
+-rw-r--r--   0 Artyom     (501) staff       (20)        5 2023-05-17 10:19:24.000000 platform-library-0.0.8/src/platform_library.egg-info/top_level.txt
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.633645 platform-library-0.0.8/src/plib/
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.635895 platform-library-0.0.8/src/plib/auth/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      559 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/encrypt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      309 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/jwt.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      682 2023-03-06 07:47:25.000000 platform-library-0.0.8/src/plib/auth/o2auth.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.636402 platform-library-0.0.8/src/plib/licensing/
+-rw-r--r--   0 Artyom     (501) staff       (20)        0 2023-03-06 07:29:21.000000 platform-library-0.0.8/src/plib/licensing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     4037 2023-05-11 06:38:08.000000 platform-library-0.0.8/src/plib/licensing/api.py
+-rw-r--r--   0 Artyom     (501) staff       (20)      553 2023-03-06 07:29:21.000000 platform-library-0.0.8/src/plib/licensing/exceptions.py
+drwxr-xr-x   0 Artyom     (501) staff       (20)        0 2023-05-17 10:19:24.636817 platform-library-0.0.8/src/plib/tracing/
+-rw-r--r--   0 Artyom     (501) staff       (20)     2287 2023-05-15 12:18:09.000000 platform-library-0.0.8/src/plib/tracing/__init__.py
+-rw-r--r--   0 Artyom     (501) staff       (20)     3007 2023-05-17 10:17:35.000000 platform-library-0.0.8/src/plib/tracing/utils.py
```

### Comparing `platform-library-0.0.7/LICENSE` & `platform-library-0.0.8/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 3DiVi Platform Library
+Copyright (c) 2023 3DiVi Platform Library
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `platform-library-0.0.7/PKG-INFO` & `platform-library-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
-        Copyright (c) 2022 3DiVi Platform Library
+        Copyright (c) 2023 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `platform-library-0.0.7/README.md` & `platform-library-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.7/pyproject.toml` & `platform-library-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "platform-library"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Artyom Vakilov", email="a.vakilov@3divi.com" },
 ]
 
 description = "A library for easy developing 3DiVi Platform"
 readme = "README-public.md"
 license = { file="LICENSE" }
```

### Comparing `platform-library-0.0.7/src/platform_library.egg-info/PKG-INFO` & `platform-library-0.0.8/src/platform_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: platform-library
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for easy developing 3DiVi Platform
 Author-email: Artyom Vakilov <a.vakilov@3divi.com>
 License: MIT License
         
-        Copyright (c) 2022 3DiVi Platform Library
+        Copyright (c) 2023 3DiVi Platform Library
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `platform-library-0.0.7/src/plib/auth/encrypt.py` & `platform-library-0.0.8/src/plib/auth/encrypt.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.7/src/plib/auth/o2auth.py` & `platform-library-0.0.8/src/plib/auth/o2auth.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.7/src/plib/licensing/api.py` & `platform-library-0.0.8/src/plib/licensing/api.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.7/src/plib/licensing/exceptions.py` & `platform-library-0.0.8/src/plib/licensing/exceptions.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.7/src/plib/tracing/__init__.py` & `platform-library-0.0.8/src/plib/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `platform-library-0.0.7/src/plib/tracing/utils.py` & `platform-library-0.0.8/src/plib/tracing/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from opentelemetry import trace
 from opentelemetry.context import Context
 from opentelemetry.trace import Tracer
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
-from plib.tracing import TRACING_ENABLED
+import plib.tracing as pt
 
 
 def get_tracer(tracer_name: Optional[str] = __name__) -> Optional[Tracer]:
     """
     Return Tracer object if tracing flag is True else return None
 
     Parameters
@@ -18,15 +18,15 @@
         module or class name.
 
     Returns
     -------
     Tracer:
         Tracer objects which is the interface for sending traces
     """
-    if TRACING_ENABLED:
+    if pt.TRACING_ENABLED:
         return trace.get_tracer(tracer_name)
     else:
         return None
 
 
 def get_current_tracing_context() -> dict:
     """
```

