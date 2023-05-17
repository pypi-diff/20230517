# Comparing `tmp/robin-chat-input-0.0.3.tar.gz` & `tmp/robin-chat-input-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin-chat-input-0.0.3.tar", last modified: Wed May 17 15:44:06 2023, max compression
+gzip compressed data, was "robin-chat-input-0.0.4.tar", last modified: Wed May 17 15:49:39 2023, max compression
```

## Comparing `robin-chat-input-0.0.3.tar` & `robin-chat-input-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:44:06.453754 robin-chat-input-0.0.3/
--rw-r--r--   0 chris      (501) staff       (20)     1063 2023-05-17 11:31:38.000000 robin-chat-input-0.0.3/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       52 2023-05-17 15:07:24.000000 robin-chat-input-0.0.3/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:44:06.453601 robin-chat-input-0.0.3/PKG-INFO
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:44:06.447377 robin-chat-input-0.0.3/robin_chat_input/
--rw-r--r--   0 chris      (501) staff       (20)     3489 2023-05-17 15:43:54.000000 robin-chat-input-0.0.3/robin_chat_input/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:44:06.446338 robin-chat-input-0.0.3/robin_chat_input/frontend/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:44:06.449486 robin-chat-input-0.0.3/robin_chat_input/frontend/build/
--rw-r--r--   0 chris      (501) staff       (20)      691 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/asset-manifest.json
--rw-r--r--   0 chris      (501) staff       (20)   197459 2023-05-17 15:07:39.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/bootstrap.min.css
--rw-r--r--   0 chris      (501) staff       (20)     2101 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/index.html
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:44:06.446473 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:44:06.453276 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/
--rw-r--r--   0 chris      (501) staff       (20)   464246 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js
--rw-r--r--   0 chris      (501) staff       (20)     2059 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt
--rw-r--r--   0 chris      (501) staff       (20)  1710225 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map
--rw-r--r--   0 chris      (501) staff       (20)     1620 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js
--rw-r--r--   0 chris      (501) staff       (20)     4657 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map
--rw-r--r--   0 chris      (501) staff       (20)     1598 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js
--rw-r--r--   0 chris      (501) staff       (20)     8383 2023-05-17 15:07:42.000000 robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:44:06.448170 robin-chat-input-0.0.3/robin_chat_input.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:44:06.000000 robin-chat-input-0.0.3/robin_chat_input.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      875 2023-05-17 15:44:06.000000 robin-chat-input-0.0.3/robin_chat_input.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-17 15:44:06.000000 robin-chat-input-0.0.3/robin_chat_input.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-05-17 15:44:06.000000 robin-chat-input-0.0.3/robin_chat_input.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       17 2023-05-17 15:44:06.000000 robin-chat-input-0.0.3/robin_chat_input.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-17 15:44:06.453793 robin-chat-input-0.0.3/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      440 2023-05-17 15:44:04.000000 robin-chat-input-0.0.3/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:49:39.479781 robin-chat-input-0.0.4/
+-rw-r--r--   0 chris      (501) staff       (20)     1063 2023-05-17 11:31:38.000000 robin-chat-input-0.0.4/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       52 2023-05-17 15:07:24.000000 robin-chat-input-0.0.4/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:49:39.479627 robin-chat-input-0.0.4/PKG-INFO
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:49:39.473110 robin-chat-input-0.0.4/robin_chat_input/
+-rw-r--r--   0 chris      (501) staff       (20)     3489 2023-05-17 15:43:54.000000 robin-chat-input-0.0.4/robin_chat_input/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:49:39.472309 robin-chat-input-0.0.4/robin_chat_input/frontend/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:49:39.475150 robin-chat-input-0.0.4/robin_chat_input/frontend/build/
+-rw-r--r--   0 chris      (501) staff       (20)      691 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/asset-manifest.json
+-rw-r--r--   0 chris      (501) staff       (20)   197459 2023-05-17 15:07:39.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/bootstrap.min.css
+-rw-r--r--   0 chris      (501) staff       (20)     2101 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/index.html
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:49:39.472438 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:49:39.479313 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/
+-rw-r--r--   0 chris      (501) staff       (20)   464246 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js
+-rw-r--r--   0 chris      (501) staff       (20)     2059 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt
+-rw-r--r--   0 chris      (501) staff       (20)  1710225 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map
+-rw-r--r--   0 chris      (501) staff       (20)     1620 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js
+-rw-r--r--   0 chris      (501) staff       (20)     4657 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map
+-rw-r--r--   0 chris      (501) staff       (20)     1598 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js
+-rw-r--r--   0 chris      (501) staff       (20)     8383 2023-05-17 15:07:42.000000 robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-17 15:49:39.474009 robin-chat-input-0.0.4/robin_chat_input.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      208 2023-05-17 15:49:39.000000 robin-chat-input-0.0.4/robin_chat_input.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      875 2023-05-17 15:49:39.000000 robin-chat-input-0.0.4/robin_chat_input.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-17 15:49:39.000000 robin-chat-input-0.0.4/robin_chat_input.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-05-17 15:49:39.000000 robin-chat-input-0.0.4/robin_chat_input.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       17 2023-05-17 15:49:39.000000 robin-chat-input-0.0.4/robin_chat_input.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-17 15:49:39.479822 robin-chat-input-0.0.4/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      440 2023-05-17 15:49:36.000000 robin-chat-input-0.0.4/setup.py
```

### Comparing `robin-chat-input-0.0.3/LICENSE` & `robin-chat-input-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/__init__.py` & `robin-chat-input-0.0.4/robin_chat_input/__init__.py`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/asset-manifest.json` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/bootstrap.min.css` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/index.html` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/2.08b0a941.chunk.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/main.63e3d358.chunk.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map` & `robin-chat-input-0.0.4/robin_chat_input/frontend/build/static/js/runtime-main.e6b0ae4c.js.map`

 * *Files identical despite different names*

### Comparing `robin-chat-input-0.0.3/robin_chat_input.egg-info/SOURCES.txt` & `robin-chat-input-0.0.4/robin_chat_input.egg-info/SOURCES.txt`

 * *Files identical despite different names*

