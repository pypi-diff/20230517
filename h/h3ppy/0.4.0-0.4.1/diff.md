# Comparing `tmp/h3ppy-0.4.0.tar.gz` & `tmp/h3ppy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h3ppy-0.4.0.tar", last modified: Wed Apr 26 11:22:08 2023, max compression
+gzip compressed data, was "h3ppy-0.4.1.tar", last modified: Wed May 17 13:42:37 2023, max compression
```

## Comparing `h3ppy-0.4.0.tar` & `h3ppy-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.951875 h3ppy-0.4.0/
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    35149 2023-04-26 11:15:41.000000 h3ppy-0.4.0/LICENSE
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       75 2023-04-26 11:15:41.000000 h3ppy-0.4.0/MANIFEST.in
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      812 2023-04-26 11:22:08.950665 h3ppy-0.4.0/PKG-INFO
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    17036 2023-04-26 11:15:41.000000 h3ppy-0.4.0/README.md
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.932927 h3ppy-0.4.0/h3ppy/
--rwx------   0 hpm5     (18177) _lpoperator   (100)    29332 2023-04-26 10:44:15.000000 h3ppy-0.4.0/h3ppy/__init__.py
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.948377 h3ppy-0.4.0/h3ppy/data/
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)     4367 2023-04-26 11:15:41.000000 h3ppy-0.4.0/h3ppy/data/h2_line_list_roueff_2019_subset.txt
--rwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)   107921 2023-04-26 11:15:41.000000 h3ppy-0.4.0/h3ppy/data/h3p_line_list_neale_1996_subset.txt
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.943767 h3ppy-0.4.0/h3ppy.egg-info/
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      812 2023-04-26 11:22:07.000000 h3ppy-0.4.0/h3ppy.egg-info/PKG-INFO
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      314 2023-04-26 11:22:08.000000 h3ppy-0.4.0/h3ppy.egg-info/SOURCES.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        1 2023-04-26 11:22:07.000000 h3ppy-0.4.0/h3ppy.egg-info/dependency_links.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-04-26 11:22:08.000000 h3ppy-0.4.0/h3ppy.egg-info/requires.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-04-26 11:22:08.000000 h3ppy-0.4.0/h3ppy.egg-info/top_level.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       38 2023-04-26 11:22:08.952210 h3ppy-0.4.0/setup.cfg
--rwx------   0 hpm5     (18177) _lpoperator   (100)     2319 2023-04-26 08:25:09.000000 h3ppy-0.4.0/setup.py
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-05-17 13:42:37.726180 h3ppy-0.4.1/
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    35149 2023-04-26 11:15:41.000000 h3ppy-0.4.1/LICENSE
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       75 2023-04-26 11:15:41.000000 h3ppy-0.4.1/MANIFEST.in
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      776 2023-05-17 13:42:37.725121 h3ppy-0.4.1/PKG-INFO
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    17036 2023-04-26 11:15:41.000000 h3ppy-0.4.1/README.md
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-05-17 13:42:37.706381 h3ppy-0.4.1/h3ppy/
+-rwx------   0 hpm5     (18177) _lpoperator   (100)    29332 2023-04-26 10:44:15.000000 h3ppy-0.4.1/h3ppy/__init__.py
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-05-17 13:42:37.721493 h3ppy-0.4.1/h3ppy/data/
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)     4367 2023-04-26 11:15:41.000000 h3ppy-0.4.1/h3ppy/data/h2_line_list_roueff_2019_subset.txt
+-rwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)   107921 2023-04-26 11:15:41.000000 h3ppy-0.4.1/h3ppy/data/h3p_line_list_neale_1996_subset.txt
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-05-17 13:42:37.717222 h3ppy-0.4.1/h3ppy.egg-info/
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      776 2023-05-17 13:42:37.000000 h3ppy-0.4.1/h3ppy.egg-info/PKG-INFO
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      314 2023-05-17 13:42:37.000000 h3ppy-0.4.1/h3ppy.egg-info/SOURCES.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        1 2023-05-17 13:42:37.000000 h3ppy-0.4.1/h3ppy.egg-info/dependency_links.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-05-17 13:42:37.000000 h3ppy-0.4.1/h3ppy.egg-info/requires.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-05-17 13:42:37.000000 h3ppy-0.4.1/h3ppy.egg-info/top_level.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       38 2023-05-17 13:42:37.726385 h3ppy-0.4.1/setup.cfg
+-rwx------   0 hpm5     (18177) _lpoperator   (100)     2330 2023-05-17 13:42:31.000000 h3ppy-0.4.1/setup.py
```

### Comparing `h3ppy-0.4.0/LICENSE` & `h3ppy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `h3ppy-0.4.0/PKG-INFO` & `h3ppy-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: h3ppy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Model and fit H3+ and H2 spectra
 Home-page: https://github.com/henrikmelin/h3ppy
 Author: Henrik Melin
 Author-email: h.melin@gmail.com
-License: UNKNOWN
 Keywords: infrared spectroscopy H3+ modelling
-Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,8 +21,7 @@
 ## Install via pip
 ```
 pip3 install h3ppy
 ```
 
 Full [documentation on Github](https://github.com/henrikmelin/h3ppy).
     
-
```

### Comparing `h3ppy-0.4.0/README.md` & `h3ppy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `h3ppy-0.4.0/h3ppy/__init__.py` & `h3ppy-0.4.1/h3ppy/__init__.py`

 * *Files identical despite different names*

### Comparing `h3ppy-0.4.0/h3ppy/data/h2_line_list_roueff_2019_subset.txt` & `h3ppy-0.4.1/h3ppy/data/h2_line_list_roueff_2019_subset.txt`

 * *Files identical despite different names*

### Comparing `h3ppy-0.4.0/h3ppy/data/h3p_line_list_neale_1996_subset.txt` & `h3ppy-0.4.1/h3ppy/data/h3p_line_list_neale_1996_subset.txt`

 * *Files identical despite different names*

### Comparing `h3ppy-0.4.0/h3ppy.egg-info/PKG-INFO` & `h3ppy-0.4.1/h3ppy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: h3ppy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Model and fit H3+ and H2 spectra
 Home-page: https://github.com/henrikmelin/h3ppy
 Author: Henrik Melin
 Author-email: h.melin@gmail.com
-License: UNKNOWN
 Keywords: infrared spectroscopy H3+ modelling
-Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,8 +21,7 @@
 ## Install via pip
 ```
 pip3 install h3ppy
 ```
 
 Full [documentation on Github](https://github.com/henrikmelin/h3ppy).
     
-
```

### Comparing `h3ppy-0.4.0/setup.py` & `h3ppy-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 SOFTWARE.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name             = 'h3ppy',
-    version          = '0.4.0',
+    version          = '0.4.1',
     author           = 'Henrik Melin',
     author_email     = 'h.melin@gmail.com',
     description      = 'Model and fit H3+ and H2 spectra',
     url              = 'https://github.com/henrikmelin/h3ppy',
     keywords         = 'infrared spectroscopy H3+ modelling',
     packages         = find_packages(),
     install_requires = ['numpy'], 
     package_dir      = {"": "."},
-    package_data     = {'h3ppy': ['h3ppy/data/h3p_line_list_neale_1996_subset.txt', 'h2_line_list_roueff_2019_subset.txt']},
+    package_data     = {'h3ppy': ['h3ppy/data/h3p_line_list_neale_1996_subset.txt', 'h3ppy/data/h2_line_list_roueff_2019_subset.txt']},
     include_package_data=True,    
     long_description = """
 # h3ppy
 A python package for modelling and fitting H<sub>3</sub><sup>+</sup> and H<sub>2</sub> spectra
 
 ## Install via pip
 ```
```

