# Comparing `tmp/map_apply-0.1.0.tar.gz` & `tmp/map_apply-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_apply-0.1.0.tar", max compression
+gzip compressed data, was "map_apply-0.1.1.tar", max compression
```

## Comparing `map_apply-0.1.0.tar` & `map_apply-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       74 2023-05-16 12:45:26.000000 map_apply-0.1.0/map_apply/__init__.py
--rw-r--r--   0        0        0      981 2023-05-16 11:14:46.000000 map_apply-0.1.0/map_apply/cli.py
--rw-r--r--   0        0        0      344 2023-05-17 10:39:02.000000 map_apply-0.1.0/map_apply/file_handler.py
--rw-r--r--   0        0        0     2405 2023-05-17 12:08:36.000000 map_apply-0.1.0/map_apply/main.py
--rw-r--r--   0        0        0        0 2023-05-16 11:04:18.000000 map_apply-0.1.0/map_apply/scripts/__init__.py
--rw-r--r--   0        0        0      338 2023-05-16 12:04:50.000000 map_apply-0.1.0/map_apply/scripts/map_apply.py
--rw-r--r--   0        0        0      548 2023-05-17 07:08:40.000000 map_apply-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      815 2023-05-17 15:15:01.690407 map_apply-0.1.0/setup.py
--rw-r--r--   0        0        0      432 2023-05-17 15:15:01.690407 map_apply-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-05-16 12:45:26.000000 map_apply-0.1.1/map_apply/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-16 11:14:46.000000 map_apply-0.1.1/map_apply/cli.py
+-rw-r--r--   0        0        0      344 2023-05-17 10:39:02.000000 map_apply-0.1.1/map_apply/file_handler.py
+-rw-r--r--   0        0        0     2405 2023-05-17 12:08:36.000000 map_apply-0.1.1/map_apply/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:04:18.000000 map_apply-0.1.1/map_apply/scripts/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-16 12:04:50.000000 map_apply-0.1.1/map_apply/scripts/map_apply.py
+-rw-r--r--   0        0        0      524 2023-05-17 16:29:02.000000 map_apply-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      796 2023-05-17 16:29:03.802989 map_apply-0.1.1/setup.py
+-rw-r--r--   0        0        0      446 2023-05-17 16:29:03.802989 map_apply-0.1.1/PKG-INFO
```

### Comparing `map_apply-0.1.0/map_apply/cli.py` & `map_apply-0.1.1/map_apply/cli.py`

 * *Files identical despite different names*

### Comparing `map_apply-0.1.0/map_apply/main.py` & `map_apply-0.1.1/map_apply/main.py`

 * *Files identical despite different names*

### Comparing `map_apply-0.1.0/pyproject.toml` & `map_apply-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "map_apply"
-version = "0.1.0"
-description = "Scan through the given file and substitute one keyfield with another using 'map' file"
-authors = ["SergSm <smirnovserg.s@gmail.com>"]
+version = "0.1.1"
+description = "Copies the input file and substitute one keyfield with another using 'map' file"
+authors = ["Smirnov Sergey"]
 license = "MIT"
 packages = [{include="map_apply"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 argparse = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `map_apply-0.1.0/setup.py` & `map_apply-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['argparse>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['map_apply = map_apply.scripts.map_apply:main']}
 
 setup_kwargs = {
     'name': 'map-apply',
-    'version': '0.1.0',
-    'description': "Scan through the given file and substitute one keyfield with another using 'map' file",
+    'version': '0.1.1',
+    'description': "Copies the input file and substitute one keyfield with another using 'map' file",
     'long_description': None,
-    'author': 'SergSm',
-    'author_email': 'smirnovserg.s@gmail.com',
+    'author': 'Smirnov Sergey',
+    'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

