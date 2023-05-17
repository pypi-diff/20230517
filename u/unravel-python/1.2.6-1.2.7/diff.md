# Comparing `tmp/unravel-python-1.2.6.tar.gz` & `tmp/unravel-python-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.2.6.tar", last modified: Wed May  3 18:29:28 2023, max compression
+gzip compressed data, was "unravel-python-1.2.7.tar", last modified: Wed May 17 15:23:14 2023, max compression
```

## Comparing `unravel-python-1.2.6.tar` & `unravel-python-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:29:27.990000 unravel-python-1.2.6/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     3950 2023-05-03 18:29:30.000000 unravel-python-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3442 2023-04-28 07:26:38.000000 unravel-python-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 18:29:30.000000 unravel-python-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1146 2023-04-28 13:02:26.000000 unravel-python-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel/
--rw-rw-rw-   0        0        0      358 2023-05-03 18:28:52.000000 unravel-python-1.2.6/unravel/__init__.py
--rw-rw-rw-   0        0        0    49987 2023-05-03 18:25:56.000000 unravel-python-1.2.6/unravel/core.py
--rw-rw-rw-   0        0        0     4558 2023-05-03 18:24:34.000000 unravel-python-1.2.6/unravel/example.py
--rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.6/unravel/utils.py
--rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.6/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3950 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:23:14.660000 unravel-python-1.2.7/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     3950 2023-05-17 15:23:16.000000 unravel-python-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3442 2023-04-28 07:26:38.000000 unravel-python-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 15:23:16.000000 unravel-python-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2023-04-28 13:02:26.000000 unravel-python-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:23:14.670000 unravel-python-1.2.7/unravel/
+-rw-rw-rw-   0        0        0      358 2023-05-17 15:23:04.000000 unravel-python-1.2.7/unravel/__init__.py
+-rw-rw-rw-   0        0        0    49991 2023-05-17 14:41:12.000000 unravel-python-1.2.7/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-05-03 18:24:34.000000 unravel-python-1.2.7/unravel/example.py
+-rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.7/unravel/utils.py
+-rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.7/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:23:14.680000 unravel-python-1.2.7/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3950 2023-05-17 15:23:16.000000 unravel-python-1.2.7/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-17 15:23:16.000000 unravel-python-1.2.7/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:23:16.000000 unravel-python-1.2.7/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-17 15:23:16.000000 unravel-python-1.2.7/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 15:23:16.000000 unravel-python-1.2.7/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.2.6/LICENSE` & `unravel-python-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.6/PKG-INFO` & `unravel-python-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.6
+Version: 1.2.7
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `unravel-python-1.2.6/README.md` & `unravel-python-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.6/setup.py` & `unravel-python-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.6/unravel/core.py` & `unravel-python-1.2.7/unravel/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,17 +276,17 @@
     v2n = v2/np.linalg.norm(v2)
 
     if (v1n == v2n).all():
         return 0
 
     dot = np.dot(v1n, v2n)
 
-    if dot > 1:
+    if dot >= 1:
         ang = 0
-    if dot < -1:
+    elif dot <= -1:
         ang = 180
     else:
         ang = math.acos(dot)*180/math.pi
 
     if ang > 90 and not direction:
         ang = 180-ang
```

### Comparing `unravel-python-1.2.6/unravel/example.py` & `unravel-python-1.2.7/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.6/unravel/utils.py` & `unravel-python-1.2.7/unravel/utils.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.6/unravel/viz.py` & `unravel-python-1.2.7/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.6/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.7/unravel_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.6
+Version: 1.2.7
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

