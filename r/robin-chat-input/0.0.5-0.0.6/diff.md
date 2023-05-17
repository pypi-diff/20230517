# Comparing `tmp/robin-chat-input-0.0.5.tar.gz` & `tmp/robin-chat-input-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin-chat-input-0.0.5.tar", last modified: Wed May 17 15:56:18 2023, max compression
+gzip compressed data, was "robin-chat-input-0.0.6.tar", last modified: Wed May 17 15:57:17 2023, max compression
```

## Comparing `robin-chat-input-0.0.5.tar` & `robin-chat-input-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:56:18.575814 robin-chat-input-0.0.5/
--rw-r--r--   0 chris      (501) staff       (20)     1063 2023-05-17 11:31:38.000000 robin-chat-input-0.0.5/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       52 2023-05-17 15:07:24.000000 robin-chat-input-0.0.5/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:56:18.575676 robin-chat-input-0.0.5/PKG-INFO
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:56:18.569120 robin-chat-input-0.0.5/robin_chat_input/
--rw-r--r--   0 chris      (501) staff       (20)     3490 2023-05-17 15:53:57.000000 robin-chat-input-0.0.5/robin_chat_input/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:56:18.568259 robin-chat-input-0.0.5/robin_chat_input/frontend/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:56:18.571057 robin-chat-input-0.0.5/robin_chat_input/frontend/build/
--rw-r--r--   0 chris      (501) staff       (20)      691 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/asset-manifest.json
--rw-r--r--   0 chris      (501) staff       (20)   197459 2023-05-17 15:07:39.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/bootstrap.min.css
--rw-r--r--   0 chris      (501) staff       (20)     2101 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/index.html
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:56:18.568389 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:56:18.575345 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/
--rw-r--r--   0 chris      (501) staff       (20)   464246 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js
--rw-r--r--   0 chris      (501) staff       (20)     2059 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt
--rw-r--r--   0 chris      (501) staff       (20)  1710225 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map
--rw-r--r--   0 chris      (501) staff       (20)     1620 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js
--rw-r--r--   0 chris      (501) staff       (20)     4657 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map
--rw-r--r--   0 chris      (501) staff       (20)     1598 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js
--rw-r--r--   0 chris      (501) staff       (20)     8383 2023-05-17 15:07:42.000000 robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:56:18.569950 robin-chat-input-0.0.5/robin_chat_input.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:56:18.000000 robin-chat-input-0.0.5/robin_chat_input.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      875 2023-05-17 15:56:18.000000 robin-chat-input-0.0.5/robin_chat_input.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-17 15:56:18.000000 robin-chat-input-0.0.5/robin_chat_input.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-05-17 15:56:18.000000 robin-chat-input-0.0.5/robin_chat_input.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       17 2023-05-17 15:56:18.000000 robin-chat-input-0.0.5/robin_chat_input.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-17 15:56:18.575853 robin-chat-input-0.0.5/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      440 2023-05-17 15:55:56.000000 robin-chat-input-0.0.5/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:17.000902 robin-chat-input-0.0.6/
+-rw-r--r--   0 chris      (501) staff       (20)     1063 2023-05-17 11:31:38.000000 robin-chat-input-0.0.6/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       52 2023-05-17 15:07:24.000000 robin-chat-input-0.0.6/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:57:17.000737 robin-chat-input-0.0.6/PKG-INFO
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.994705 robin-chat-input-0.0.6/robin_chat_input/
+-rw-r--r--   0 chris      (501) staff       (20)     3489 2023-05-17 15:57:06.000000 robin-chat-input-0.0.6/robin_chat_input/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.993838 robin-chat-input-0.0.6/robin_chat_input/frontend/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.996568 robin-chat-input-0.0.6/robin_chat_input/frontend/build/
+-rw-r--r--   0 chris      (501) staff       (20)      691 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/asset-manifest.json
+-rw-r--r--   0 chris      (501) staff       (20)   197459 2023-05-17 15:07:39.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/bootstrap.min.css
+-rw-r--r--   0 chris      (501) staff       (20)     2101 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/index.html
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.993974 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:17.000388 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/
+-rw-r--r--   0 chris      (501) staff       (20)   464246 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js
+-rw-r--r--   0 chris      (501) staff       (20)     2059 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt
+-rw-r--r--   0 chris      (501) staff       (20)  1710225 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map
+-rw-r--r--   0 chris      (501) staff       (20)     1620 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js
+-rw-r--r--   0 chris      (501) staff       (20)     4657 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map
+-rw-r--r--   0 chris      (501) staff       (20)     1598 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js
+-rw-r--r--   0 chris      (501) staff       (20)     8383 2023-05-17 15:07:42.000000 robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:57:16.995336 robin-chat-input-0.0.6/robin_chat_input.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      875 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       17 2023-05-17 15:57:16.000000 robin-chat-input-0.0.6/robin_chat_input.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-17 15:57:17.000947 robin-chat-input-0.0.6/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      440 2023-05-17 15:57:12.000000 robin-chat-input-0.0.6/setup.py
```

### Comparing `robin-chat-input-0.0.5/LICENSE` & `robin-chat-input-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/__init__.py` & `robin-chat-input-0.0.6/robin_chat_input/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False 
+_RELEASE = True 
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/asset-manifest.json` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/bootstrap.min.css` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/index.html` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map` & `robin-chat-input-0.0.6/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.5/robin_chat_input.egg-info/SOURCES.txt` & `robin-chat-input-0.0.6/robin_chat_input.egg-info/SOURCES.txt`

 * *Files identical despite different names*

