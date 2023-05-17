# Comparing `tmp/filesystem-dict-0.1.3.tar.gz` & `tmp/filesystem-dict-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesystem-dict-0.1.3.tar", last modified: Tue May 16 08:48:58 2023, max compression
+gzip compressed data, was "filesystem-dict-0.1.4.tar", last modified: Wed May 17 09:45:25 2023, max compression
```

## Comparing `filesystem-dict-0.1.3.tar` & `filesystem-dict-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:48:58.350837 filesystem-dict-0.1.3/
--rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.3/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)      855 2023-05-16 08:48:58.350837 filesystem-dict-0.1.3/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      540 2023-05-15 20:56:08.000000 filesystem-dict-0.1.3/README.md
--rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-16 08:48:58.350837 filesystem-dict-0.1.3/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.3/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:48:58.347504 filesystem-dict-0.1.3/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:48:58.347504 filesystem-dict-0.1.3/src/filesystem_dict.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      855 2023-05-16 08:48:58.000000 filesystem-dict-0.1.3/src/filesystem_dict.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-16 08:48:58.000000 filesystem-dict-0.1.3/src/filesystem_dict.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-16 08:48:58.000000 filesystem-dict-0.1.3/src/filesystem_dict.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-16 08:48:58.000000 filesystem-dict-0.1.3/src/filesystem_dict.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:48:58.350837 filesystem-dict-0.1.3/src/fsdict/
--rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-16 07:52:47.000000 filesystem-dict-0.1.3/src/fsdict/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3282 2023-05-16 08:47:18.000000 filesystem-dict-0.1.3/src/fsdict/fsdict.py
--rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-16 08:07:12.000000 filesystem-dict-0.1.3/src/fsdict/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/
+-rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.4/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      834 2023-05-17 08:45:31.000000 filesystem-dict-0.1.4/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.521004 filesystem-dict-0.1.4/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/src/fsdict/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-16 07:52:47.000000 filesystem-dict-0.1.4/src/fsdict/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5021 2023-05-17 09:43:21.000000 filesystem-dict-0.1.4/src/fsdict/fsdict.py
+-rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-16 08:07:12.000000 filesystem-dict-0.1.4/src/fsdict/utils.py
```

### Comparing `filesystem-dict-0.1.3/LICENSE.txt` & `filesystem-dict-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.3/PKG-INFO` & `filesystem-dict-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # FSDict
 
 ## Design principles
-1) Every key of a fsdict must be of type 'str'.
+1) Every key of a fsdict must be of type 'str' or 'FunctionType'.
 2) A fsdict may not be part of a list.
 3) A fsdict may contain other fsdicts.
 4) Dictionaries in python are passed by reference; so are fsdicts. By default
 an fsdict is always passed by refernece. That is, its values are not copied but
 the fsdict is symlinked to the new position.
 
 ## Internals
+Keys of type 'str' work just as normal dictionary keys. Keys of type
+'FunctionType' are used as filters for the keys of an fsdict. So
+```python
+dictionary[lambda key: "foo" in key]
+```
+would return a generator which yields the values for keys which contain the
+string 'foo'.
+
 Possible value types and how they are handled:
 - fsdict - a directory
 - 'bytes' type - written to file as is
 - any other python object (except for 'bytes') - pickled
```

### Comparing `filesystem-dict-0.1.3/src/filesystem_dict.egg-info/PKG-INFO` & `filesystem-dict-0.1.4/src/filesystem_dict.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # FSDict
 
 ## Design principles
-1) Every key of a fsdict must be of type 'str'.
+1) Every key of a fsdict must be of type 'str' or 'FunctionType'.
 2) A fsdict may not be part of a list.
 3) A fsdict may contain other fsdicts.
 4) Dictionaries in python are passed by reference; so are fsdicts. By default
 an fsdict is always passed by refernece. That is, its values are not copied but
 the fsdict is symlinked to the new position.
 
 ## Internals
+Keys of type 'str' work just as normal dictionary keys. Keys of type
+'FunctionType' are used as filters for the keys of an fsdict. So
+```python
+dictionary[lambda key: "foo" in key]
+```
+would return a generator which yields the values for keys which contain the
+string 'foo'.
+
 Possible value types and how they are handled:
 - fsdict - a directory
 - 'bytes' type - written to file as is
 - any other python object (except for 'bytes') - pickled
```

### Comparing `filesystem-dict-0.1.3/src/fsdict/utils.py` & `filesystem-dict-0.1.4/src/fsdict/utils.py`

 * *Files identical despite different names*

