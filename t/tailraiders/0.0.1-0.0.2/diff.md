# Comparing `tmp/tailraiders-0.0.1.tar.gz` & `tmp/tailraiders-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailraiders-0.0.1.tar", last modified: Tue May 16 22:18:23 2023, max compression
+gzip compressed data, was "tailraiders-0.0.2.tar", last modified: Tue May 16 22:44:44 2023, max compression
```

## Comparing `tailraiders-0.0.1.tar` & `tailraiders-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.830303 tailraiders-0.0.1/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      678 2023-05-16 22:18:23.829030 tailraiders-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-16 22:14:49.000000 tailraiders-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 22:18:23.831311 tailraiders-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-05-16 22:18:06.000000 tailraiders-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.771829 tailraiders-0.0.1/tailraiders/
--rw-rw-rw-   0        0        0      159 2023-05-16 11:43:39.000000 tailraiders-0.0.1/tailraiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.809237 tailraiders-0.0.1/tailraiders/boaboa/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 tailraiders-0.0.1/tailraiders/boaboa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.810464 tailraiders-0.0.1/tailraiders/bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 tailraiders-0.0.1/tailraiders/bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.822115 tailraiders-0.0.1/tailraiders/gajalaka/
--rw-rw-rw-   0        0        0       46 2023-05-16 12:15:36.000000 tailraiders-0.0.1/tailraiders/gajalaka/__init__.py
--rw-rw-rw-   0        0        0     2337 2023-05-16 21:59:03.000000 tailraiders-0.0.1/tailraiders/gajalaka/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.823597 tailraiders-0.0.1/tailraiders/plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.1/tailraiders/plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.825672 tailraiders-0.0.1/tailraiders/protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 tailraiders-0.0.1/tailraiders/protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.826957 tailraiders-0.0.1/tailraiders/trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.1/tailraiders/trouper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:18:23.807233 tailraiders-0.0.1/tailraiders.egg-info/
--rw-rw-rw-   0        0        0      678 2023-05-16 22:18:22.000000 tailraiders-0.0.1/tailraiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-05-16 22:18:23.000000 tailraiders-0.0.1/tailraiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:18:22.000000 tailraiders-0.0.1/tailraiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 22:18:23.000000 tailraiders-0.0.1/tailraiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 22:18:23.000000 tailraiders-0.0.1/tailraiders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.413922 tailraiders-0.0.2/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      678 2023-05-16 22:44:44.412784 tailraiders-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-05-16 22:14:49.000000 tailraiders-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:44:44.414928 tailraiders-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-05-16 22:44:25.000000 tailraiders-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.377720 tailraiders-0.0.2/tailraiders/
+-rw-rw-rw-   0        0        0      159 2023-05-16 11:43:39.000000 tailraiders-0.0.2/tailraiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.400764 tailraiders-0.0.2/tailraiders/boaboa/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 tailraiders-0.0.2/tailraiders/boaboa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.401769 tailraiders-0.0.2/tailraiders/bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 tailraiders-0.0.2/tailraiders/bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.406130 tailraiders-0.0.2/tailraiders/gajalaka/
+-rw-rw-rw-   0        0        0       46 2023-05-16 12:15:36.000000 tailraiders-0.0.2/tailraiders/gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     2645 2023-05-16 22:35:53.000000 tailraiders-0.0.2/tailraiders/gajalaka/nan.py
+-rw-rw-rw-   0        0        0     2337 2023-05-16 21:59:03.000000 tailraiders-0.0.2/tailraiders/gajalaka/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.408588 tailraiders-0.0.2/tailraiders/plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.2/tailraiders/plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.409981 tailraiders-0.0.2/tailraiders/protector/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 tailraiders-0.0.2/tailraiders/protector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.410485 tailraiders-0.0.2/tailraiders/trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.2/tailraiders/trouper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:44:44.399413 tailraiders-0.0.2/tailraiders.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-05-16 22:44:44.000000 tailraiders-0.0.2/tailraiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 22:44:43.000000 tailraiders-0.0.2/tailraiders.egg-info/top_level.txt
```

### Comparing `tailraiders-0.0.1/LICENSE` & `tailraiders-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.1/PKG-INFO` & `tailraiders-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tailraiders-0.0.1/setup.py` & `tailraiders-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier, versions with 0.0.x are trials and tests',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     name = 'tailraiders',
-    version = '0.0.1',
+    version = '0.0.2',
     packages = find_packages(include = ['tailraiders', 'tailraiders.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

### Comparing `tailraiders-0.0.1/tailraiders/gajalaka/plots.py` & `tailraiders-0.0.2/tailraiders/gajalaka/plots.py`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.1/tailraiders.egg-info/PKG-INFO` & `tailraiders-0.0.2/tailraiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for making Data Science easier, versions with 0.0.x are trials and tests
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

