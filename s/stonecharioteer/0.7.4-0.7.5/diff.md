# Comparing `tmp/stonecharioteer-0.7.4.tar.gz` & `tmp/stonecharioteer-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stonecharioteer-0.7.4.tar", max compression
+gzip compressed data, was "stonecharioteer-0.7.5.tar", max compression
```

## Comparing `stonecharioteer-0.7.4.tar` & `stonecharioteer-0.7.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      708 2022-12-14 06:05:23.125568 stonecharioteer-0.7.4/pyproject.toml
--rw-r--r--   0        0        0       64 2022-12-14 05:30:47.351757 stonecharioteer-0.7.4/stonecharioteer/__init__.py
--rw-r--r--   0        0        0      586 2022-11-23 08:04:48.932952 stonecharioteer-0.7.4/stonecharioteer/constants.py
--rw-r--r--   0        0        0     1118 2022-12-14 05:30:47.351757 stonecharioteer-0.7.4/stonecharioteer/logger.py
--rw-r--r--   0        0        0     1922 2022-12-14 05:30:47.351757 stonecharioteer-0.7.4/stonecharioteer/qtile/__init__.py
--rw-r--r--   0        0        0      422 2022-12-07 05:07:31.994438 stonecharioteer-0.7.4/stonecharioteer/qtile/groups.py
--rw-r--r--   0        0        0      573 2022-12-14 05:30:47.351757 stonecharioteer-0.7.4/stonecharioteer/qtile/inputs.py
--rwxr-xr-x   0        0        0     4934 2022-12-14 05:30:47.351757 stonecharioteer-0.7.4/stonecharioteer/qtile/keymaps.py
--rw-r--r--   0        0        0      960 2022-11-23 08:04:48.932952 stonecharioteer-0.7.4/stonecharioteer/qtile/layouts.py
--rwxr-xr-x   0        0        0     6013 2022-12-14 06:05:23.125568 stonecharioteer-0.7.4/stonecharioteer/qtile/panels.py
--rw-r--r--   0        0        0     2499 2022-12-14 05:30:47.351757 stonecharioteer-0.7.4/stonecharioteer/qtile/screens.py
--rw-r--r--   0        0        0     1324 2022-11-23 08:04:48.932952 stonecharioteer-0.7.4/stonecharioteer/utils/displays.py
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 stonecharioteer-0.7.4/setup.py
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 stonecharioteer-0.7.4/PKG-INFO
+-rwxr-xr-x   0        0        0      708 2022-12-14 14:57:18.503951 stonecharioteer-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0       64 2022-12-14 05:30:47.351757 stonecharioteer-0.7.5/stonecharioteer/__init__.py
+-rw-r--r--   0        0        0      586 2022-11-23 08:04:48.932952 stonecharioteer-0.7.5/stonecharioteer/constants.py
+-rw-r--r--   0        0        0     1118 2022-12-14 05:30:47.351757 stonecharioteer-0.7.5/stonecharioteer/logger.py
+-rw-r--r--   0        0        0     1922 2022-12-14 05:30:47.351757 stonecharioteer-0.7.5/stonecharioteer/qtile/__init__.py
+-rw-r--r--   0        0        0      422 2022-12-07 05:07:31.994438 stonecharioteer-0.7.5/stonecharioteer/qtile/groups.py
+-rw-r--r--   0        0        0      573 2022-12-14 05:30:47.351757 stonecharioteer-0.7.5/stonecharioteer/qtile/inputs.py
+-rwxr-xr-x   0        0        0     4934 2022-12-14 05:30:47.351757 stonecharioteer-0.7.5/stonecharioteer/qtile/keymaps.py
+-rw-r--r--   0        0        0      189 2022-12-14 14:57:49.203958 stonecharioteer-0.7.5/stonecharioteer/qtile/layouts.py
+-rwxr-xr-x   0        0        0     6013 2022-12-14 06:05:23.125568 stonecharioteer-0.7.5/stonecharioteer/qtile/panels.py
+-rw-r--r--   0        0        0     2499 2022-12-14 05:30:47.351757 stonecharioteer-0.7.5/stonecharioteer/qtile/screens.py
+-rw-r--r--   0        0        0     1324 2022-11-23 08:04:48.932952 stonecharioteer-0.7.5/stonecharioteer/utils/displays.py
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 stonecharioteer-0.7.5/setup.py
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 stonecharioteer-0.7.5/PKG-INFO
```

### Comparing `stonecharioteer-0.7.4/pyproject.toml` & `stonecharioteer-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stonecharioteer"
-version = "0.7.4"
+version = "0.7.5"
 description = "My personal utils and configs, managed via python library"
 authors = ["Vinay Keerthi <11478411+stonecharioteer@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
 qtile = ">=0.18.1"
```

### Comparing `stonecharioteer-0.7.4/stonecharioteer/constants.py` & `stonecharioteer-0.7.5/stonecharioteer/constants.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/stonecharioteer/logger.py` & `stonecharioteer-0.7.5/stonecharioteer/logger.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/stonecharioteer/qtile/__init__.py` & `stonecharioteer-0.7.5/stonecharioteer/qtile/__init__.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/stonecharioteer/qtile/inputs.py` & `stonecharioteer-0.7.5/stonecharioteer/qtile/inputs.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/stonecharioteer/qtile/keymaps.py` & `stonecharioteer-0.7.5/stonecharioteer/qtile/keymaps.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/stonecharioteer/qtile/panels.py` & `stonecharioteer-0.7.5/stonecharioteer/qtile/panels.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/stonecharioteer/qtile/screens.py` & `stonecharioteer-0.7.5/stonecharioteer/qtile/screens.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/stonecharioteer/utils/displays.py` & `stonecharioteer-0.7.5/stonecharioteer/utils/displays.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.4/setup.py` & `stonecharioteer-0.7.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'rich>=10.12.0,<11.0.0',
  'toml>=0.10.2,<0.11.0',
  'typeguard>=2.13.3,<3.0.0',
  'types-toml>=0.10.1,<0.11.0']
 
 setup_kwargs = {
     'name': 'stonecharioteer',
-    'version': '0.7.4',
+    'version': '0.7.5',
     'description': 'My personal utils and configs, managed via python library',
     'long_description': 'None',
     'author': 'Vinay Keerthi',
     'author_email': '11478411+stonecharioteer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stonecharioteer-0.7.4/PKG-INFO` & `stonecharioteer-0.7.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stonecharioteer
-Version: 0.7.4
+Version: 0.7.5
 Summary: My personal utils and configs, managed via python library
 Author: Vinay Keerthi
 Author-email: 11478411+stonecharioteer@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

