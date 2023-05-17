# Comparing `tmp/mid_to_gcode-0.0.0a0.tar.gz` & `tmp/mid_to_gcode-0.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mid_to_gcode-0.0.0a0.tar", last modified: Wed May 17 18:28:24 2023, max compression
+gzip compressed data, was "mid_to_gcode-0.0.0a1.tar", last modified: Wed May 17 18:36:51 2023, max compression
```

## Comparing `mid_to_gcode-0.0.0a0.tar` & `mid_to_gcode-0.0.0a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:28:24.698662 mid_to_gcode-0.0.0a0/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      677 2023-05-17 18:18:12.000000 mid_to_gcode-0.0.0a0/LICENSE
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      838 2023-05-17 18:28:24.698662 mid_to_gcode-0.0.0a0/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 15:30:19.000000 mid_to_gcode-0.0.0a0/README.rst
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:28:24.698662 mid_to_gcode-0.0.0a0/mid_to_gcode/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       35 2023-05-17 15:37:10.000000 mid_to_gcode-0.0.0a0/mid_to_gcode/__init__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1726 2023-05-17 18:17:01.000000 mid_to_gcode-0.0.0a0/mid_to_gcode/functions.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      466 2023-05-17 18:05:51.000000 mid_to_gcode-0.0.0a0/mid_to_gcode/mid_to_gcod.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      942 2023-05-17 18:15:55.000000 mid_to_gcode-0.0.0a0/mid_to_gcode/support_functions.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:28:24.698662 mid_to_gcode-0.0.0a0/mid_to_gcode.egg-info/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      838 2023-05-17 18:28:24.000000 mid_to_gcode-0.0.0a0/mid_to_gcode.egg-info/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      299 2023-05-17 18:28:24.000000 mid_to_gcode-0.0.0a0/mid_to_gcode.egg-info/SOURCES.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)        1 2023-05-17 18:28:24.000000 mid_to_gcode-0.0.0a0/mid_to_gcode.egg-info/dependency_links.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       13 2023-05-17 18:28:24.000000 mid_to_gcode-0.0.0a0/mid_to_gcode.egg-info/top_level.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      668 2023-05-17 18:27:05.000000 mid_to_gcode-0.0.0a0/pyproject.toml
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       38 2023-05-17 18:28:24.698662 mid_to_gcode-0.0.0a0/setup.cfg
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1332 2023-05-17 18:22:46.000000 mid_to_gcode-0.0.0a0/setup.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      677 2023-05-17 18:18:12.000000 mid_to_gcode-0.0.0a1/LICENSE
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      838 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 15:30:19.000000 mid_to_gcode-0.0.0a1/README.rst
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:36:51.003419 mid_to_gcode-0.0.0a1/mid_to_gcode/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       35 2023-05-17 15:37:10.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/__init__.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1726 2023-05-17 18:17:01.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/functions.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      466 2023-05-17 18:05:51.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/mid_to_gcod.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      942 2023-05-17 18:35:37.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/support_functions.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      838 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      299 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/SOURCES.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)        1 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/dependency_links.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       13 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/top_level.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      669 2023-05-17 18:36:23.000000 mid_to_gcode-0.0.0a1/pyproject.toml
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       38 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/setup.cfg
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1332 2023-05-17 18:22:46.000000 mid_to_gcode-0.0.0a1/setup.py
```

### Comparing `mid_to_gcode-0.0.0a0/LICENSE` & `mid_to_gcode-0.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mid_to_gcode-0.0.0a0/PKG-INFO` & `mid_to_gcode-0.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mid_to_gcode
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: The project for translate .mid format to 3d printers gcode 
 Home-page: https://github.com/GigantPro/mid_to_gcode
 Author: GigantPro
 Author-email: gigantpro2000@gmail.ru
 License: The GPLv3 License (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `mid_to_gcode-0.0.0a0/mid_to_gcode/functions.py` & `mid_to_gcode-0.0.0a1/mid_to_gcode/functions.py`

 * *Files identical despite different names*

### Comparing `mid_to_gcode-0.0.0a0/mid_to_gcode/support_functions.py` & `mid_to_gcode-0.0.0a1/mid_to_gcode/support_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             last = item
 
 def number_to_ghz(number: int) -> str:
     octo_size = 12
     A = 27.0  # ghz
     
     num_at_octo = number % octo_size
-    new_A = A * (2 ** (number // (octo_size - 1)))
+    new_A = A * (2 ** ((number // octo_size) - 1))
     
     config = {
         9: new_A,
         10: new_A * (16 / 15),
     }
     
     config[11] = config[10] * 1.0546875
```

### Comparing `mid_to_gcode-0.0.0a0/mid_to_gcode.egg-info/PKG-INFO` & `mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mid-to-gcode
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: The project for translate .mid format to 3d printers gcode 
 Home-page: https://github.com/GigantPro/mid_to_gcode
 Author: GigantPro
 Author-email: gigantpro2000@gmail.ru
 License: The GPLv3 License (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `mid_to_gcode-0.0.0a0/setup.py` & `mid_to_gcode-0.0.0a1/setup.py`

 * *Files identical despite different names*

