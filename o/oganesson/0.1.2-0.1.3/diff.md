# Comparing `tmp/oganesson-0.1.2.tar.gz` & `tmp/oganesson-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson-0.1.2.tar", last modified: Wed May 17 00:04:44 2023, max compression
+gzip compressed data, was "oganesson-0.1.3.tar", last modified: Wed May 17 00:47:12 2023, max compression
```

## Comparing `oganesson-0.1.2.tar` & `oganesson-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.171761 oganesson-0.1.2/
--rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.2/.gitattributes
--rw-rw-rw-   0        0        0      297 2023-05-17 00:04:16.000000 oganesson-0.1.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2692 2023-05-17 00:04:44.170752 oganesson-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2239 2023-05-16 07:00:01.000000 oganesson-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.104276 oganesson-0.1.2/oganesson/
--rw-rw-rw-   0        0        0        5 2023-05-17 00:04:16.000000 oganesson-0.1.2/oganesson/VERSION
--rw-rw-rw-   0        0        0       74 2023-05-09 00:52:11.000000 oganesson-0.1.2/oganesson/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.2/oganesson/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.2/oganesson/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.146719 oganesson-0.1.2/oganesson/descriptors/
--rw-rw-rw-   0        0        0     1226 2023-05-16 04:44:12.000000 oganesson-0.1.2/oganesson/descriptors/__init__.py
--rw-rw-rw-   0        0        0     7896 2023-05-11 01:10:06.000000 oganesson-0.1.2/oganesson/descriptors/bacd.py
--rw-rw-rw-   0        0        0       29 2023-05-17 00:02:20.000000 oganesson-0.1.2/oganesson/descriptors/gpaw.py
--rw-rw-rw-   0        0        0     3646 2023-05-16 23:54:40.000000 oganesson-0.1.2/oganesson/descriptors/rosa.py
--rw-rw-rw-   0        0        0     2801 2023-05-16 03:55:40.000000 oganesson-0.1.2/oganesson/descriptors/symmetry_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.148227 oganesson-0.1.2/oganesson/genetic_algorithms/
--rw-rw-rw-   0        0        0     7853 2023-05-17 00:02:20.000000 oganesson-0.1.2/oganesson/genetic_algorithms/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.2/oganesson/ogai.py
--rw-rw-rw-   0        0        0     6700 2023-05-16 04:38:44.000000 oganesson-0.1.2/oganesson/ogstructure.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.168748 oganesson-0.1.2/oganesson/utilities/
--rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.2/oganesson/utilities/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.2/oganesson/utilities/atomic_data.py
--rw-rw-rw-   0        0        0   405452 2023-05-16 02:56:53.000000 oganesson-0.1.2/oganesson/utilities/bonds_dictionary.py
--rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.2/oganesson/version.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:04:44.122273 oganesson-0.1.2/oganesson.egg-info/
--rw-rw-rw-   0        0        0     2692 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 00:04:44.000000 oganesson-0.1.2/oganesson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 00:04:44.171761 oganesson-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-05-17 00:02:20.000000 oganesson-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.143987 oganesson-0.1.3/
+-rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.3/.gitattributes
+-rw-rw-rw-   0        0        0      344 2023-05-17 00:45:53.000000 oganesson-0.1.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2678 2023-05-17 00:47:12.143987 oganesson-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2239 2023-05-17 00:22:04.000000 oganesson-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.116986 oganesson-0.1.3/oganesson/
+-rw-rw-rw-   0        0        0        5 2023-05-17 00:46:43.000000 oganesson-0.1.3/oganesson/VERSION
+-rw-rw-rw-   0        0        0      428 2023-05-17 00:46:24.000000 oganesson-0.1.3/oganesson/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.3/oganesson/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.3/oganesson/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.136986 oganesson-0.1.3/oganesson/descriptors/
+-rw-rw-rw-   0        0        0     1226 2023-05-17 00:39:53.000000 oganesson-0.1.3/oganesson/descriptors/__init__.py
+-rw-rw-rw-   0        0        0     7896 2023-05-11 01:10:06.000000 oganesson-0.1.3/oganesson/descriptors/bacd.py
+-rw-rw-rw-   0        0        0     3646 2023-05-16 23:54:40.000000 oganesson-0.1.3/oganesson/descriptors/rosa.py
+-rw-rw-rw-   0        0        0     2801 2023-05-16 03:55:40.000000 oganesson-0.1.3/oganesson/descriptors/symmetry_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.137987 oganesson-0.1.3/oganesson/genetic_algorithms/
+-rw-rw-rw-   0        0        0     7853 2023-05-17 00:02:20.000000 oganesson-0.1.3/oganesson/genetic_algorithms/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.3/oganesson/ogai.py
+-rw-rw-rw-   0        0        0     6700 2023-05-16 04:38:44.000000 oganesson-0.1.3/oganesson/ogstructure.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.141985 oganesson-0.1.3/oganesson/utilities/
+-rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.3/oganesson/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.3/oganesson/utilities/atomic_data.py
+-rw-rw-rw-   0        0        0   405452 2023-05-16 02:56:53.000000 oganesson-0.1.3/oganesson/utilities/bonds_dictionary.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.3/oganesson/version.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:47:12.132989 oganesson-0.1.3/oganesson.egg-info/
+-rw-rw-rw-   0        0        0     2678 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 00:47:12.000000 oganesson-0.1.3/oganesson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 00:47:12.143987 oganesson-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-17 00:46:24.000000 oganesson-0.1.3/setup.py
```

### Comparing `oganesson-0.1.2/CONTRIBUTING.rst` & `oganesson-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/LICENSE` & `oganesson-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/PKG-INFO` & `oganesson-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.2
+Version: 0.1.3
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
-Keywords: ai,machine learning,model testing
+Keywords: ai,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./assets/logo.svg" width="200px">
 
 # Oganesson
```

### Comparing `oganesson-0.1.2/README.md` & `oganesson-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/cli.py` & `oganesson-0.1.3/oganesson/cli.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/descriptors/__init__.py` & `oganesson-0.1.3/oganesson/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/descriptors/bacd.py` & `oganesson-0.1.3/oganesson/descriptors/bacd.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/descriptors/rosa.py` & `oganesson-0.1.3/oganesson/descriptors/rosa.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/descriptors/symmetry_functions.py` & `oganesson-0.1.3/oganesson/descriptors/symmetry_functions.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/genetic_algorithms/__init__.py` & `oganesson-0.1.3/oganesson/genetic_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/ogstructure.py` & `oganesson-0.1.3/oganesson/ogstructure.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/utilities/__init__.py` & `oganesson-0.1.3/oganesson/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/utilities/atomic_data.py` & `oganesson-0.1.3/oganesson/utilities/atomic_data.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson/utilities/bonds_dictionary.py` & `oganesson-0.1.3/oganesson/utilities/bonds_dictionary.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.2/oganesson.egg-info/PKG-INFO` & `oganesson-0.1.3/oganesson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.2
+Version: 0.1.3
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
-Keywords: ai,machine learning,model testing
+Keywords: ai,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./assets/logo.svg" width="200px">
 
 # Oganesson
```

### Comparing `oganesson-0.1.2/oganesson.egg-info/SOURCES.txt` & `oganesson-0.1.3/oganesson.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,13 @@
 oganesson.egg-info/SOURCES.txt
 oganesson.egg-info/dependency_links.txt
 oganesson.egg-info/entry_points.txt
 oganesson.egg-info/requires.txt
 oganesson.egg-info/top_level.txt
 oganesson/descriptors/__init__.py
 oganesson/descriptors/bacd.py
-oganesson/descriptors/gpaw.py
 oganesson/descriptors/rosa.py
 oganesson/descriptors/symmetry_functions.py
 oganesson/genetic_algorithms/__init__.py
 oganesson/utilities/__init__.py
 oganesson/utilities/atomic_data.py
 oganesson/utilities/bonds_dictionary.py
```

### Comparing `oganesson-0.1.2/setup.py` & `oganesson-0.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,18 +17,17 @@
     license='mit',
     description='oganesson enables rapid AI workflows for material science and chemistry',
     long_description=README,
     long_description_content_type='text/markdown',
     author='Sherif Abdulkader Tawfik Abbas',
     author_email='sherif.tawfic@gmail.com',
     url='https://github.com/oganesson-ai/oganesson',
-    keywords=['ai', 'machine learning',
-              'model testing'],
+    keywords=['ai', 'machine learning'],
     install_requires=['ase',
                       'pandas',
                       'numpy',
                       'm3gnet',
-                      'pymatgen'
+                      'pymatgen',
                       'm3gnet',
                       'gpaw'],
 
 )
```

