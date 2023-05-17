# Comparing `tmp/streamlit-option-menu-0.3.3.tar.gz` & `tmp/streamlit-option-menu-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-option-menu-0.3.3.tar", last modified: Wed May 17 15:54:41 2023, max compression
+gzip compressed data, was "streamlit-option-menu-0.3.4.tar", last modified: Wed May 17 16:19:49 2023, max compression
```

## Comparing `streamlit-option-menu-0.3.3.tar` & `streamlit-option-menu-0.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/
--rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.3/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       56 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2430 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     4694 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2769 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/streamlit_option_menu/
--rwxr-xr-x   0 root         (0) root         (0)     4284 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/css/
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/css/app.9b0f7d0b.css
--rw-r--r--   0 root         (0) root         (0)   273142 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/fonts/
--rw-r--r--   0 root         (0) root         (0)   164360 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff
--rw-r--r--   0 root         (0) root         (0)   121340 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/
--rw-r--r--   0 root         (0) root         (0)     7352 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/app.625674d3.js
--rw-r--r--   0 root         (0) root         (0)    28619 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/app.625674d3.js.map
--rw-r--r--   0 root         (0) root         (0)   328486 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js
--rw-r--r--   0 root         (0) root         (0)  1616052 2023-05-17 15:53:26.000000 streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:54:41.455740 streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2430 2023-05-17 15:54:41.000000 streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      860 2023-05-17 15:54:41.000000 streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 15:54:41.000000 streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 15:54:41.000000 streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 15:54:41.000000 streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/
+-rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       56 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     4694 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2769 2023-05-17 16:18:28.000000 streamlit-option-menu-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/
+-rwxr-xr-x   0 root         (0) root         (0)     4284 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/app.9b0f7d0b.css
+-rw-r--r--   0 root         (0) root         (0)   273142 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)   164360 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff
+-rw-r--r--   0 root         (0) root         (0)   121340 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/
+-rw-r--r--   0 root         (0) root         (0)     7352 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js
+-rw-r--r--   0 root         (0) root         (0)    28619 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js.map
+-rw-r--r--   0 root         (0) root         (0)   328486 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js
+-rw-r--r--   0 root         (0) root         (0)  1616052 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      860 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/top_level.txt
```

### Comparing `streamlit-option-menu-0.3.3/LICENSE` & `streamlit-option-menu-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/PKG-INFO` & `streamlit-option-menu-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-option-menu
-Version: 0.3.3
+Version: 0.3.4
 Summary: streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.
 Home-page: https://github.com/victoryhb/streamlit-option-menu
 Author: Victor Yan
 Author-email: victoryhb@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `streamlit-option-menu-0.3.3/README.md` & `streamlit-option-menu-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/setup.py` & `streamlit-option-menu-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-option-menu",
-    version="0.3.3",
+    version="0.3.4",
     author="Victor Yan",
     author_email="victoryhb@163.com",
     description="streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.",
     long_description="""streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.
 It is similar in function to st.selectbox(), except that:
 - It uses a simple static list to display the options instead of a dropdown
 - It has configurable icons for each option item and the menu title
```

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/__init__.py` & `streamlit-option-menu-0.3.4/streamlit_option_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/css/app.9b0f7d0b.css` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/app.9b0f7d0b.css`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/index.html` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/app.625674d3.js` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/app.625674d3.js.map` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map` & `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/PKG-INFO` & `streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-option-menu
-Version: 0.3.3
+Version: 0.3.4
 Summary: streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.
 Home-page: https://github.com/victoryhb/streamlit-option-menu
 Author: Victor Yan
 Author-email: victoryhb@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `streamlit-option-menu-0.3.3/streamlit_option_menu.egg-info/SOURCES.txt` & `streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

