# Comparing `tmp/theonerig-0.0.1.tar.gz` & `tmp/theonerig-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theonerig-0.0.1.tar", last modified: Wed Dec  1 13:37:44 2021, max compression
+gzip compressed data, was "dist/theonerig-0.0.2.tar", last modified: Mon Dec 20 11:02:46 2021, max compression
```

## Comparing `theonerig-0.0.1.tar` & `theonerig-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-01 13:37:44.880546 theonerig-0.0.1/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    11357 2021-03-26 10:03:13.000000 theonerig-0.0.1/LICENSE
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     4883 2021-12-01 13:37:44.880546 theonerig-0.0.1/PKG-INFO
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     4102 2021-09-08 08:13:17.000000 theonerig-0.0.1/README.md
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       38 2021-12-01 13:37:44.880546 theonerig-0.0.1/setup.cfg
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     1893 2021-03-26 10:03:13.000000 theonerig-0.0.1/setup.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-01 13:37:44.880546 theonerig-0.0.1/theonerig/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       22 2021-12-01 13:15:32.000000 theonerig-0.0.1/theonerig/__init__.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    10440 2021-12-01 13:16:31.000000 theonerig-0.0.1/theonerig/_nbdev.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    26335 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/core.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     5228 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/database.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     6699 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/eyetrack.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    15148 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/leddome.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    20353 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/modelling.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    96209 2021-12-01 13:16:31.000000 theonerig-0.0.1/theonerig/plotting.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    35828 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/processing.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-01 13:37:44.880546 theonerig-0.0.1/theonerig/synchro/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)        0 2021-03-26 10:03:13.000000 theonerig-0.0.1/theonerig/synchro/__init__.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    11249 2021-12-01 13:16:31.000000 theonerig-0.0.1/theonerig/synchro/extracting.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    60534 2021-12-01 13:16:31.000000 theonerig-0.0.1/theonerig/synchro/io.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    21569 2021-12-01 13:16:31.000000 theonerig-0.0.1/theonerig/synchro/nested_stims.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    23268 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/synchro/processing.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     1903 2021-12-01 13:15:33.000000 theonerig-0.0.1/theonerig/testdata.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    34995 2021-12-01 13:16:31.000000 theonerig-0.0.1/theonerig/utils.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-01 13:37:44.880546 theonerig-0.0.1/theonerig.egg-info/
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)     4883 2021-12-01 13:37:44.000000 theonerig-0.0.1/theonerig.egg-info/PKG-INFO
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)      645 2021-12-01 13:37:44.000000 theonerig-0.0.1/theonerig.egg-info/SOURCES.txt
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)        1 2021-12-01 13:37:44.000000 theonerig-0.0.1/theonerig.egg-info/dependency_links.txt
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)       20 2021-12-01 13:37:44.000000 theonerig-0.0.1/theonerig.egg-info/entry_points.txt
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)        1 2021-01-18 08:40:32.000000 theonerig-0.0.1/theonerig.egg-info/not-zip-safe
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)       71 2021-12-01 13:37:44.000000 theonerig-0.0.1/theonerig.egg-info/requires.txt
--rwxr-xr-x   0 tristan   (1000) tristan   (1000)       10 2021-12-01 13:37:44.000000 theonerig-0.0.1/theonerig.egg-info/top_level.txt
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-20 11:02:46.417280 theonerig-0.0.2/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    11357 2021-03-26 10:03:13.000000 theonerig-0.0.2/LICENSE
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     4883 2021-12-20 11:02:46.417280 theonerig-0.0.2/PKG-INFO
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     4102 2021-09-08 08:13:17.000000 theonerig-0.0.2/README.md
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       38 2021-12-20 11:02:46.417280 theonerig-0.0.2/setup.cfg
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     1893 2021-03-26 10:03:13.000000 theonerig-0.0.2/setup.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-20 11:02:46.413280 theonerig-0.0.2/theonerig/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       22 2021-12-01 13:15:32.000000 theonerig-0.0.2/theonerig/__init__.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    10440 2021-12-01 13:16:31.000000 theonerig-0.0.2/theonerig/_nbdev.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    26335 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/core.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     5228 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/database.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     6699 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/eyetrack.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    15148 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/leddome.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    20353 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/modelling.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    96209 2021-12-01 13:16:31.000000 theonerig-0.0.2/theonerig/plotting.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    35828 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/processing.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-20 11:02:46.417280 theonerig-0.0.2/theonerig/synchro/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)        0 2021-03-26 10:03:13.000000 theonerig-0.0.2/theonerig/synchro/__init__.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    11249 2021-12-01 13:16:31.000000 theonerig-0.0.2/theonerig/synchro/extracting.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    60534 2021-12-01 13:16:31.000000 theonerig-0.0.2/theonerig/synchro/io.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    21569 2021-12-01 13:16:31.000000 theonerig-0.0.2/theonerig/synchro/nested_stims.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    23268 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/synchro/processing.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     1903 2021-12-01 13:15:33.000000 theonerig-0.0.2/theonerig/testdata.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    34995 2021-12-01 13:16:31.000000 theonerig-0.0.2/theonerig/utils.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2021-12-20 11:02:46.417280 theonerig-0.0.2/theonerig.egg-info/
+-rwxr-xr-x   0 tristan   (1000) tristan   (1000)     4883 2021-12-20 11:02:46.000000 theonerig-0.0.2/theonerig.egg-info/PKG-INFO
+-rwxr-xr-x   0 tristan   (1000) tristan   (1000)      645 2021-12-20 11:02:46.000000 theonerig-0.0.2/theonerig.egg-info/SOURCES.txt
+-rwxr-xr-x   0 tristan   (1000) tristan   (1000)        1 2021-12-20 11:02:46.000000 theonerig-0.0.2/theonerig.egg-info/dependency_links.txt
+-rwxr-xr-x   0 tristan   (1000) tristan   (1000)       20 2021-12-20 11:02:46.000000 theonerig-0.0.2/theonerig.egg-info/entry_points.txt
+-rwxr-xr-x   0 tristan   (1000) tristan   (1000)        1 2021-01-18 08:40:32.000000 theonerig-0.0.2/theonerig.egg-info/not-zip-safe
+-rwxr-xr-x   0 tristan   (1000) tristan   (1000)       88 2021-12-20 11:02:46.000000 theonerig-0.0.2/theonerig.egg-info/requires.txt
+-rwxr-xr-x   0 tristan   (1000) tristan   (1000)       10 2021-12-20 11:02:46.000000 theonerig-0.0.2/theonerig.egg-info/top_level.txt
```

### Comparing `theonerig-0.0.1/LICENSE` & `theonerig-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/PKG-INFO` & `theonerig-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theonerig
-Version: 0.0.1
+Version: 0.0.2
 Summary: Timeseries synchronisation toolkit for computational neuroscience
 Home-page: https://github.com/Tom-TBT/theonerig
 Author: Tom Boissonnet
 Author-email: tom.boissonnet@hotmail.fr
 License: Apache Software License 2.0
 Keywords: neuroscience synchronisation timeserie pipeline
 Platform: UNKNOWN
```

### Comparing `theonerig-0.0.1/README.md` & `theonerig-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/setup.py` & `theonerig-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/_nbdev.py` & `theonerig-0.0.2/theonerig/_nbdev.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/core.py` & `theonerig-0.0.2/theonerig/core.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/database.py` & `theonerig-0.0.2/theonerig/database.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/eyetrack.py` & `theonerig-0.0.2/theonerig/eyetrack.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/leddome.py` & `theonerig-0.0.2/theonerig/leddome.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/modelling.py` & `theonerig-0.0.2/theonerig/modelling.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/plotting.py` & `theonerig-0.0.2/theonerig/plotting.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/processing.py` & `theonerig-0.0.2/theonerig/processing.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/synchro/extracting.py` & `theonerig-0.0.2/theonerig/synchro/extracting.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/synchro/io.py` & `theonerig-0.0.2/theonerig/synchro/io.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/synchro/nested_stims.py` & `theonerig-0.0.2/theonerig/synchro/nested_stims.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/synchro/processing.py` & `theonerig-0.0.2/theonerig/synchro/processing.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/testdata.py` & `theonerig-0.0.2/theonerig/testdata.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig/utils.py` & `theonerig-0.0.2/theonerig/utils.py`

 * *Files identical despite different names*

### Comparing `theonerig-0.0.1/theonerig.egg-info/PKG-INFO` & `theonerig-0.0.2/theonerig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theonerig
-Version: 0.0.1
+Version: 0.0.2
 Summary: Timeseries synchronisation toolkit for computational neuroscience
 Home-page: https://github.com/Tom-TBT/theonerig
 Author: Tom Boissonnet
 Author-email: tom.boissonnet@hotmail.fr
 License: Apache Software License 2.0
 Keywords: neuroscience synchronisation timeserie pipeline
 Platform: UNKNOWN
```

### Comparing `theonerig-0.0.1/theonerig.egg-info/SOURCES.txt` & `theonerig-0.0.2/theonerig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

