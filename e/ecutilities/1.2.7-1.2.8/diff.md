# Comparing `tmp/ecutilities-1.2.7.tar.gz` & `tmp/ecutilities-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecutilities-1.2.7.tar", last modified: Tue May  2 09:46:38 2023, max compression
+gzip compressed data, was "ecutilities-1.2.8.tar", last modified: Wed May 17 07:06:25 2023, max compression
```

## Comparing `ecutilities-1.2.7.tar` & `ecutilities-1.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-02 09:46:38.755649 ecutilities-1.2.7/
--rwxr-xr-x   0 vtec      (1000) vtec      (1000)     1077 2022-10-25 09:14:41.000000 ecutilities-1.2.7/LICENSE.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       90 2022-10-28 16:19:44.000000 ecutilities-1.2.7/MANIFEST.in
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-05-02 09:46:38.755649 ecutilities-1.2.7/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)      830 2023-05-02 09:46:06.000000 ecutilities-1.2.7/README.md
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-02 09:46:38.745649 ecutilities-1.2.7/ecutilities/
--rw-r--r--   0 vtec      (1000) vtec      (1000)       22 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    10826 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/_modidx.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    11545 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/core.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     4841 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/dev_utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2830 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/eda_stats_utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     7902 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/image_utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     5292 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/ipython.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     7346 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/ml.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     5670 2023-05-02 09:45:59.000000 ecutilities-1.2.7/ecutilities/plotting.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-02 09:46:38.755649 ecutilities-1.2.7/ecutilities.egg-info/
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)      516 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/SOURCES.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/dependency_links.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       44 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/entry_points.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-01-27 05:44:01.000000 ecutilities-1.2.7/ecutilities.egg-info/not-zip-safe
--rw-r--r--   0 vtec      (1000) vtec      (1000)       80 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/requires.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       12 2023-05-02 09:46:38.000000 ecutilities-1.2.7/ecutilities.egg-info/top_level.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)      928 2023-03-30 05:59:24.000000 ecutilities-1.2.7/settings.ini
--rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-05-02 09:46:38.755649 ecutilities-1.2.7/setup.cfg
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2534 2022-10-28 06:03:02.000000 ecutilities-1.2.7/setup.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:06:25.034060 ecutilities-1.2.8/
+-rwxr-xr-x   0 vtec      (1000) vtec      (1000)     1077 2022-10-25 09:14:41.000000 ecutilities-1.2.8/LICENSE.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       90 2022-10-28 16:19:44.000000 ecutilities-1.2.8/MANIFEST.in
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-05-17 07:06:25.034060 ecutilities-1.2.8/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      830 2023-05-02 09:46:06.000000 ecutilities-1.2.8/README.md
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:06:25.024060 ecutilities-1.2.8/ecutilities/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       22 2023-05-17 06:43:24.000000 ecutilities-1.2.8/ecutilities/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    10826 2023-05-17 06:43:25.000000 ecutilities-1.2.8/ecutilities/_modidx.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    11944 2023-05-17 06:45:36.000000 ecutilities-1.2.8/ecutilities/core.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     4841 2023-05-17 06:43:24.000000 ecutilities-1.2.8/ecutilities/dev_utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2830 2023-05-17 06:43:24.000000 ecutilities-1.2.8/ecutilities/eda_stats_utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     7902 2023-05-17 06:43:24.000000 ecutilities-1.2.8/ecutilities/image_utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5505 2023-05-17 06:45:36.000000 ecutilities-1.2.8/ecutilities/ipython.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     7346 2023-05-17 06:43:24.000000 ecutilities-1.2.8/ecutilities/ml.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5670 2023-05-17 06:43:24.000000 ecutilities-1.2.8/ecutilities/plotting.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:06:25.034060 ecutilities-1.2.8/ecutilities.egg-info/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1549 2023-05-17 07:06:24.000000 ecutilities-1.2.8/ecutilities.egg-info/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      516 2023-05-17 07:06:24.000000 ecutilities-1.2.8/ecutilities.egg-info/SOURCES.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-05-17 07:06:24.000000 ecutilities-1.2.8/ecutilities.egg-info/dependency_links.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       44 2023-05-17 07:06:24.000000 ecutilities-1.2.8/ecutilities.egg-info/entry_points.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-01-27 05:44:01.000000 ecutilities-1.2.8/ecutilities.egg-info/not-zip-safe
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       80 2023-05-17 07:06:24.000000 ecutilities-1.2.8/ecutilities.egg-info/requires.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       12 2023-05-17 07:06:24.000000 ecutilities-1.2.8/ecutilities.egg-info/top_level.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      928 2023-05-02 09:50:51.000000 ecutilities-1.2.8/settings.ini
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-05-17 07:06:25.034060 ecutilities-1.2.8/setup.cfg
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2534 2022-10-28 06:03:02.000000 ecutilities-1.2.8/setup.py
```

### Comparing `ecutilities-1.2.7/LICENSE.txt` & `ecutilities-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/PKG-INFO` & `ecutilities-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecutilities
-Version: 1.2.7
+Version: 1.2.8
 Summary: Set of utility functions used on regular basis
 Home-page: https://github.com/vtecftwy/ecutils
 Author: Etienne Charlier
 Author-email: github@procurasia.com
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ecutilities-1.2.7/README.md` & `ecutilities-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/ecutilities/_modidx.py` & `ecutilities-1.2.8/ecutilities/_modidx.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/ecutilities/core.py` & `ecutilities-1.2.8/ecutilities/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -269,19 +269,26 @@
     return paths
 
 # %% ../nbs-dev/0_00_core.ipynb 50
 def path_to_parent_dir(
     pattern:str,               # pattern to identify the parent directory
     path:str|Path|None = None, # optional path from where to seek for parent directory
 )-> Path:                      # path of the parent directory
-    """Climb directory tree up to a directory starting with the string `pattern`, and return its path
+    """Climb directory tree up to a directory starting with `pattern`, and return its path.
     
-    Can pass a starting path to climb from. 
+    - When no directory is found in the tree starting with `pattern`, return the current directory path.
+    
+    - It is possible to pass a `path` as starting path to climb from. 
     """
     if path is None: path = Path()
     path = safe_path(path).absolute()
     tree = [path.name] + [p.name for p in path.parents]
     mask = [True if n.startswith(pattern) else False for n in tree]
-    tree = tree[mask.index(True):]
-    tree.reverse()
-    nbs = Path('/'.join(tree))
-    return nbs
+    # A parent directory with the pattern is found in the tree, return that directory
+    if any(mask):
+        tree = tree[mask.index(True):]
+        tree.reverse()
+        parent_dir = Path('/'.join(tree))
+    # No parent directory with the pattern is found in the tree, return the current directory
+    else:
+        parent_dir = Path().absolute()
+    return parent_dir
```

### Comparing `ecutilities-1.2.7/ecutilities/dev_utils.py` & `ecutilities-1.2.8/ecutilities/dev_utils.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/ecutilities/eda_stats_utils.py` & `ecutilities-1.2.8/ecutilities/eda_stats_utils.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/ecutilities/image_utils.py` & `ecutilities-1.2.8/ecutilities/image_utils.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/ecutilities/ipython.py` & `ecutilities-1.2.8/ecutilities/ipython.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,18 @@
 # %% ../nbs-dev/0_01_ipython.ipynb 8
 def nb_setup(
     autoreload:bool = True,       # True to set autoreload in this notebook
     paths:List[str|Path] = None   # Paths to add to the path environment variable
     ):
     """Use in first cell of notebook to set autoreload, and add system paths
     
-    Always add a path to 'src' in the project root, if the directory exists
+    Always add a path to the directoruy 'src' if `srs` directory exists at the same level as the `nbs` directory.
+
+    When the notebook is not located in a tree including the name `nbs`, `src` directory is searched at the same level
+    as the directory in which the notebook is located.
     """
     #  Handle paths
     #  Add src if it exists
     nbs_root = path_to_parent_dir('nbs')
     p2src = (nbs_root / '../src').resolve().absolute()
     if p2src.is_dir():
         p = str(p2src.absolute())
```

### Comparing `ecutilities-1.2.7/ecutilities/ml.py` & `ecutilities-1.2.8/ecutilities/ml.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/ecutilities/plotting.py` & `ecutilities-1.2.8/ecutilities/plotting.py`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/ecutilities.egg-info/PKG-INFO` & `ecutilities-1.2.8/ecutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecutilities
-Version: 1.2.7
+Version: 1.2.8
 Summary: Set of utility functions used on regular basis
 Home-page: https://github.com/vtecftwy/ecutils
 Author: Etienne Charlier
 Author-email: github@procurasia.com
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ecutilities-1.2.7/ecutilities.egg-info/SOURCES.txt` & `ecutilities-1.2.8/ecutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecutilities-1.2.7/settings.ini` & `ecutilities-1.2.8/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ecutils
 lib_name = ecutilities
-version = 1.2.7
+version = 1.2.8
 min_python = 3.8
 license = MIT
 doc_path = _docs
 lib_path = ecutilities
 nbs_path = nbs-dev
 recursive = True
 tst_flags = notest
```

### Comparing `ecutilities-1.2.7/setup.py` & `ecutilities-1.2.8/setup.py`

 * *Files identical despite different names*

