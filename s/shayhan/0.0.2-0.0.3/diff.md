# Comparing `tmp/shayhan-0.0.2.tar.gz` & `tmp/shayhan-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shayhan-0.0.2.tar", last modified: Tue May 16 11:15:55 2023, max compression
+gzip compressed data, was "shayhan-0.0.3.tar", last modified: Wed May 17 09:34:49 2023, max compression
```

## Comparing `shayhan-0.0.2.tar` & `shayhan-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:15:55.464717 shayhan-0.0.2/
--rw-rw-rw-   0        0        0      241 2023-05-16 11:08:24.000000 shayhan-0.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1083 2022-05-21 23:27:50.000000 shayhan-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2022-05-21 23:35:18.000000 shayhan-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      795 2023-05-16 11:15:55.464717 shayhan-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       34 2022-05-21 23:14:55.000000 shayhan-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 11:15:55.465715 shayhan-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-05-16 11:08:58.000000 shayhan-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:15:55.453715 shayhan-0.0.2/shayhan/
--rw-rw-rw-   0        0        0     4387 2023-05-16 11:04:18.000000 shayhan-0.0.2/shayhan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:15:55.462718 shayhan-0.0.2/shayhan.egg-info/
--rw-rw-rw-   0        0        0      795 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 09:34:49.500891 shayhan-0.0.3/
+-rw-rw-rw-   0        0        0      320 2023-05-17 09:23:49.000000 shayhan-0.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1083 2022-05-21 23:27:50.000000 shayhan-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2022-05-21 23:35:18.000000 shayhan-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      874 2023-05-17 09:34:49.499887 shayhan-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2022-05-21 23:14:55.000000 shayhan-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 09:34:49.500891 shayhan-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-05-17 09:23:07.000000 shayhan-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:34:49.492888 shayhan-0.0.3/shayhan/
+-rw-rw-rw-   0        0        0     4696 2023-05-17 09:24:51.000000 shayhan-0.0.3/shayhan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:34:49.498888 shayhan-0.0.3/shayhan.egg-info/
+-rw-rw-rw-   0        0        0      874 2023-05-17 09:34:49.000000 shayhan-0.0.3/shayhan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-17 09:34:49.000000 shayhan-0.0.3/shayhan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 09:34:49.000000 shayhan-0.0.3/shayhan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 09:34:49.000000 shayhan-0.0.3/shayhan.egg-info/top_level.txt
```

### Comparing `shayhan-0.0.2/LICENSE.txt` & `shayhan-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shayhan-0.0.2/PKG-INFO` & `shayhan-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shayhan
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a libriry of some fuctions
 Home-page: 
 Author: Shayhan Ameen Chowdhury
 Author-email: shayhan.ameen@gmail.com
 License: MIT
 Keywords: print
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,18 @@
 License-File: LICENSE.txt
 
 This is a libriry of some fuctions
 
 Change Log
 ============
 
+0.0.3 (May 17, 2023)
+----------------------
+- Now can show variable names
+
 0.0.2 (May 16, 2023)
 ----------------------
 - Can now display information of multiple variables in a table
 - Support torch, tensorflow ans sparse
 
 0.0.1 (May 22, 2022)
 ----------------------
```

### Comparing `shayhan-0.0.2/setup.py` & `shayhan-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='shayhan',
-  version='0.0.2',
+  version='0.0.3',
   description='This is a libriry of some fuctions',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.md').read(),
   url='',  
   author='Shayhan Ameen Chowdhury',
   author_email='shayhan.ameen@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `shayhan-0.0.2/shayhan/__init__.py` & `shayhan-0.0.3/shayhan/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 from prettytable import PrettyTable
 
-def peek(variable_objects, limit=5):
+
+def peek(variable_objects, limit=5, variable_names=None):
     """ This is function to print the type, shape, and value of a variable
 
     Args:
         variable_objects (any type): any type of variable
         limit (int, optional): The length of a variable. Defaults to 5.
     """
     variableTable = PrettyTable(["Variable","Type", "Shape", "Value"])
     if not isinstance(variable_objects, (list)):
         variable_objects = [variable_objects]
+    variable_names= variable_names.split(',')
     
     i=0
     for variable_object in variable_objects:
 #         variable_name = f"{variable_object=}".split("=")[0]
         short_data_type =f'{type(variable_object)}'.split("<class '")[1].split('.')[0]
         full_data_type = f'{type(variable_object)}'.split("<class '")[1].split("'")[0]
+        variable_name = i if variable_names==None else variable_names[i]
 
         if isinstance(variable_object, (float, int, str,)):
-            variableTable.add_row([i, full_data_type, "1", variable_object], divider=True)        
+            variableTable.add_row([variable_name, full_data_type, "1", variable_object], divider=True)        
         elif isinstance(variable_object, (list, dict, tuple, set)):
-            variableTable.add_row([i, full_data_type, len(variable_object), variable_object[:limit]], divider=True) 
+            variableTable.add_row([variable_name, full_data_type, len(variable_object), variable_object[:limit]], divider=True) 
         elif short_data_type == 'numpy': #type(value)==numpy.ndarray:
             import numpy
-            variableTable.add_row([i, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]], divider=True)
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]], divider=True)
         elif short_data_type == 'torch': 
             import torch
-            variableTable.add_row([i, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]], divider=True)
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]], divider=True)
         elif short_data_type == 'tensorflow': #type(value)==numpy.ndarray:
             import tensorflow
-            variableTable.add_row([i, full_data_type, variable_object.shape, variable_object[:limit,:limit].todense()])
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, variable_object[:limit,:limit].todense()], divider=True)
         elif short_data_type == 'scipy': #type(value)==numpy.ndarray:
             import scipy
-            variableTable.add_row([i, full_data_type, variable_object.shape, "-"])
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, "-"], divider=True)
         else:
-            variableTable.add_row([i, type(variable_object), "-", "-"], divider=True)
+            variableTable.add_row([variable_name, type(variable_object), "-", "-"], divider=True)
         i=i+1
     print(variableTable)
     
 def peek_no_division(variable_objects, limit=5):
     """ This is function to print the type, shape, and value of a variable
 
     Args:
         variable_objects (any type): any type of variable
         limit (int, optional): The length of a variable. Defaults to 5.
     """
-    variableTable = PrettyTable(["SL","Type", "Shape", "Value"])
+    variableTable = PrettyTable(["Variable","Type", "Shape", "Value"])
     if not isinstance(variable_objects, (list)):
         variable_objects = [variable_objects]
+    variable_names= variable_names.split(',')
     
     i=0
     for variable_object in variable_objects:
 #         variable_name = f"{variable_object=}".split("=")[0]
         short_data_type =f'{type(variable_object)}'.split("<class '")[1].split('.')[0]
         full_data_type = f'{type(variable_object)}'.split("<class '")[1].split("'")[0]
+        variable_name = i if variable_names==None else variable_names[i]
 
         if isinstance(variable_object, (float, int, str,)):
-            variableTable.add_row([i, full_data_type, "1", variable_object], divider=True)        
+            variableTable.add_row([variable_name, full_data_type, "1", variable_object])        
         elif isinstance(variable_object, (list, dict, tuple, set)):
-            variableTable.add_row([i, full_data_type, len(variable_object), variable_object[:limit]]) 
-        elif short_data_type == 'numpy': #type(value)==numpy.ndarray:
+            variableTable.add_row([variable_name, full_data_type, len(variable_object), variable_object[:limit]]) 
+        elif short_data_type == 'numpy': 
             import numpy
-            variableTable.add_row([i, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]])
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]])
         elif short_data_type == 'torch': 
             import torch
-            variableTable.add_row([i, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]])
-        elif short_data_type == 'tensorflow': #type(value)==numpy.ndarray:
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]])
+        elif short_data_type == 'tensorflow': 
             import tensorflow
-            variableTable.add_row([i, full_data_type, variable_object.shape, variable_object[:limit] if variable_object.ndim==1 else variable_object[:limit,:limit]])
-        elif short_data_type == 'scipy': #type(value)==numpy.ndarray:
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, variable_object[:limit,:limit].todense()])
+        elif short_data_type == 'scipy': 
             import scipy
-            variableTable.add_row([i, full_data_type, variable_object.shape, "-"])
+            variableTable.add_row([variable_name, full_data_type, variable_object.shape, "-"])
         else:
-            variableTable.add_row([i, type(variable_object), "-", "-"], divider=True)
+            variableTable.add_row([variable_name, type(variable_object), "-", "-"])
         i=i+1
     print(variableTable)
```

### Comparing `shayhan-0.0.2/shayhan.egg-info/PKG-INFO` & `shayhan-0.0.3/shayhan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shayhan
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a libriry of some fuctions
 Home-page: 
 Author: Shayhan Ameen Chowdhury
 Author-email: shayhan.ameen@gmail.com
 License: MIT
 Keywords: print
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,18 @@
 License-File: LICENSE.txt
 
 This is a libriry of some fuctions
 
 Change Log
 ============
 
+0.0.3 (May 17, 2023)
+----------------------
+- Now can show variable names
+
 0.0.2 (May 16, 2023)
 ----------------------
 - Can now display information of multiple variables in a table
 - Support torch, tensorflow ans sparse
 
 0.0.1 (May 22, 2022)
 ----------------------
```

