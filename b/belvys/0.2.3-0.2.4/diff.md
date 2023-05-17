# Comparing `tmp/belvys-0.2.3.tar.gz` & `tmp/belvys-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "belvys-0.2.3.tar", last modified: Fri Apr 28 17:13:04 2023, max compression
+gzip compressed data, was "belvys-0.2.4.tar", last modified: Wed May 17 15:37:33 2023, max compression
```

## Comparing `belvys-0.2.3.tar` & `belvys-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-28 17:12:53.000000 belvys-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 17:12:53.000000 belvys-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 17:13:04.043545 belvys-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-28 17:12:53.000000 belvys-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/belvys/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:13:04.043545 belvys-0.2.3/belvys/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_api_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_api_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_structure_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/example_structure_complex.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-28 17:12:53.000000 belvys-0.2.3/belvys/tenant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/belvys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:13:03.000000 belvys-0.2.3/belvys.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:13:04.000000 belvys-0.2.3/belvys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 17:12:53.000000 belvys-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 17:13:04.043545 belvys-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 17:12:53.000000 belvys-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:13:04.043545 belvys-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 17:12:53.000000 belvys-0.2.3/tests/test_liveconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-28 17:12:53.000000 belvys-0.2.3/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-04-28 17:12:53.000000 belvys-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:37:33.666408 belvys-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 15:37:19.000000 belvys-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-17 15:37:19.000000 belvys-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-17 15:37:33.666408 belvys-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-17 15:37:19.000000 belvys-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:37:33.666408 belvys-0.2.4/belvys/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 15:37:33.666408 belvys-0.2.4/belvys/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/example_api_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/example_api_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/example_structure_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/example_structure_complex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-17 15:37:19.000000 belvys-0.2.4/belvys/tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:37:33.666408 belvys-0.2.4/belvys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-17 15:37:33.000000 belvys-0.2.4/belvys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 15:37:33.000000 belvys-0.2.4/belvys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:37:33.000000 belvys-0.2.4/belvys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:37:33.000000 belvys-0.2.4/belvys.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 15:37:33.000000 belvys-0.2.4/belvys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 15:37:33.000000 belvys-0.2.4/belvys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-17 15:37:19.000000 belvys-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-17 15:37:33.666408 belvys-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-17 15:37:19.000000 belvys-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:37:33.666408 belvys-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-17 15:37:19.000000 belvys-0.2.4/tests/test_liveconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-17 15:37:19.000000 belvys-0.2.4/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-05-17 15:37:19.000000 belvys-0.2.4/versioneer.py
```

### Comparing `belvys-0.2.3/LICENSE` & `belvys-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/PKG-INFO` & `belvys-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.2.3
+Version: 0.2.4
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.2.3/README.rst` & `belvys-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/adjustment.py` & `belvys-0.2.4/belvys/adjustment.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/api.py` & `belvys-0.2.4/belvys/api.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/example.py` & `belvys-0.2.4/belvys/example.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/example_api_complex.yaml` & `belvys-0.2.4/belvys/example_api_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/example_structure_basic.yaml` & `belvys-0.2.4/belvys/example_structure_basic.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/example_structure_complex.yaml` & `belvys-0.2.4/belvys/example_structure_complex.yaml`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/structure.py` & `belvys-0.2.4/belvys/structure.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/belvys/tenant.py` & `belvys-0.2.4/belvys/tenant.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         for pfid in self.structure.to_original_pfids(pfid):
             ts_tree = self.structure.tstree_pfline(pfid, pflineid)
             self._fetch_series(ts_tree, ts_left, ts_right, missing2zero=missing2zero)
             ts_trees.append(ts_tree)
         if debug:
             return ts_trees
         # Turn into portfolio line.
-        return sum([self._pfline(ts_tree) for ts_tree in ts_trees])
+        return sum([self._pfline(ts_tree) for ts_tree in ts_trees], None)
 
     def price_pfl(
         self,
         priceid: str,
         ts_left: pd.Timestamp,
         ts_right: pd.Timestamp,
         missing2zero: bool = True,
```

### Comparing `belvys-0.2.3/belvys.egg-info/PKG-INFO` & `belvys-0.2.4/belvys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvys
-Version: 0.2.3
+Version: 0.2.4
 Summary: Getting timeseries data from Belvis Rest API.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Belvys
```

### Comparing `belvys-0.2.3/belvys.egg-info/SOURCES.txt` & `belvys-0.2.4/belvys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/setup.py` & `belvys-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/tests/test_liveconnection.py` & `belvys-0.2.4/tests/test_liveconnection.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/tests/test_structure.py` & `belvys-0.2.4/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `belvys-0.2.3/versioneer.py` & `belvys-0.2.4/versioneer.py`

 * *Files identical despite different names*

