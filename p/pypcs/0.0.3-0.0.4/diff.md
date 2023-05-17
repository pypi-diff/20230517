# Comparing `tmp/pypcs-0.0.3.tar.gz` & `tmp/pypcs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pypcs-0.0.3.tar", last modified: Wed May 17 19:09:23 2023, max compression
+gzip compressed data, was "dist\pypcs-0.0.4.tar", last modified: Wed May 17 19:21:49 2023, max compression
```

## Comparing `pypcs-0.0.3.tar` & `pypcs-0.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.591319 pypcs-0.0.3/
--rw-rw-rw-   0        0        0    17096 2023-05-08 05:43:04.000000 pypcs-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       51 2023-05-17 19:04:31.000000 pypcs-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    13272 2023-05-17 19:09:23.591319 pypcs-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12880 2023-05-17 18:12:55.000000 pypcs-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.551424 pypcs-0.0.3/pyPCS/
--rw-rw-rw-   0        0        0    83140 2023-05-17 06:28:12.000000 pypcs-0.0.3/pyPCS/ChordAttr.json
--rw-rw-rw-   0        0        0     1656 2023-05-15 09:00:39.000000 pypcs-0.0.3/pyPCS/MidiInputHandler.py
--rw-rw-rw-   0        0        0     3362 2023-05-14 17:34:03.000000 pypcs-0.0.3/pyPCS/__init__.py
--rw-rw-rw-   0        0        0    23593 2023-05-16 14:33:37.000000 pypcs-0.0.3/pyPCS/_basicData.py
--rw-rw-rw-   0        0        0     3020 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/_player.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.553419 pypcs-0.0.3/pyPCS/basicGenerator/
--rw-rw-rw-   0        0        0      364 2023-05-14 17:33:49.000000 pypcs-0.0.3/pyPCS/basicGenerator/__init__.py
--rw-rw-rw-   0        0        0    10426 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/basicGenerator/basicGenerator.py
--rw-rw-rw-   0        0        0     7163 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/chorder.py
--rw-rw-rw-   0        0        0    45352 2023-05-17 14:15:11.000000 pypcs-0.0.3/pyPCS/circle_of_fifth.png
--rw-rw-rw-   0        0        0      487 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/classmethod_dec.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.555414 pypcs-0.0.3/pyPCS/piecesGenerator/
--rw-rw-rw-   0        0        0      154 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/piecesGenerator/__init__.py
--rw-rw-rw-   0        0        0      299 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/piecesGenerator/pieces_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.561397 pypcs-0.0.3/pyPCS/series/
--rw-rw-rw-   0        0        0      653 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/series/__init__.py
--rw-rw-rw-   0        0        0    29983 2023-05-17 14:59:44.000000 pypcs-0.0.3/pyPCS/series/funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.564390 pypcs-0.0.3/pyPCS/series/images/
--rw-rw-rw-   0        0        0    69072 2023-05-17 17:44:21.000000 pypcs-0.0.3/pyPCS/series/images/cof_show.png
--rw-rw-rw-   0        0        0    83930 2023-05-17 17:54:00.000000 pypcs-0.0.3/pyPCS/series/images/cofs_show.png
--rw-rw-rw-   0        0        0    25430 2023-05-17 17:16:38.000000 pypcs-0.0.3/pyPCS/series/series1d.py
--rw-rw-rw-   0        0        0    25167 2023-05-15 08:35:30.000000 pypcs-0.0.3/pyPCS/series/series2d.py
--rw-rw-rw-   0        0        0     4833 2023-05-08 05:43:04.000000 pypcs-0.0.3/pyPCS/series/tree.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.571371 pypcs-0.0.3/pypcs.egg-info/
--rw-rw-rw-   0        0        0    13272 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1089 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-17 19:09:23.000000 pypcs-0.0.3/pypcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 19:09:23.591319 pypcs-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-05-17 19:08:19.000000 pypcs-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.577395 pypcs-0.0.3/test/
--rw-rw-rw-   0        0        0     2517 2023-05-16 13:00:44.000000 pypcs-0.0.3/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.580347 pypcs-0.0.3/test/basicGenerator/
--rw-rw-rw-   0        0        0       26 2023-05-15 08:57:40.000000 pypcs-0.0.3/test/basicGenerator/__init__.py
--rw-rw-rw-   0        0        0       12 2023-05-15 08:58:51.000000 pypcs-0.0.3/test/basicGenerator/test_basicGenerator.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.582342 pypcs-0.0.3/test/piecesGenerator/
--rw-rw-rw-   0        0        0       99 2023-05-15 08:58:51.000000 pypcs-0.0.3/test/piecesGenerator/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-15 08:58:51.000000 pypcs-0.0.3/test/piecesGenerator/test_pieces_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:09:23.589323 pypcs-0.0.3/test/series/
--rw-rw-rw-   0        0        0      352 2023-05-15 08:57:52.000000 pypcs-0.0.3/test/series/__init__.py
--rw-rw-rw-   0        0        0     3679 2023-05-14 21:28:30.000000 pypcs-0.0.3/test/series/test_funcs.py
--rw-rw-rw-   0        0        0    12028 2023-05-17 17:57:22.000000 pypcs-0.0.3/test/series/test_series1d.py
--rw-rw-rw-   0        0        0     1994 2023-05-15 08:49:15.000000 pypcs-0.0.3/test/series/test_series2d.py
--rw-rw-rw-   0        0        0     4833 2023-05-08 05:43:04.000000 pypcs-0.0.3/test/series/test_tree.py
--rw-rw-rw-   0        0        0      474 2023-05-15 08:55:20.000000 pypcs-0.0.3/test/test_MidiInputHandler.py
--rw-rw-rw-   0        0        0      430 2023-05-14 17:14:53.000000 pypcs-0.0.3/test/test_chorder.py
--rw-rw-rw-   0        0        0        2 2023-05-14 17:15:00.000000 pypcs-0.0.3/test/test_classmethod_dec.py
--rw-rw-rw-   0        0        0      271 2023-05-14 17:11:03.000000 pypcs-0.0.3/test/test_player.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.798043 pypcs-0.0.4/
+-rw-rw-rw-   0        0        0    17096 2023-05-08 05:43:04.000000 pypcs-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-05-17 19:19:28.000000 pypcs-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    13272 2023-05-17 19:21:49.797046 pypcs-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12880 2023-05-17 18:12:55.000000 pypcs-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.754160 pypcs-0.0.4/pyPCS/
+-rw-rw-rw-   0        0        0    83140 2023-05-17 06:28:12.000000 pypcs-0.0.4/pyPCS/ChordAttr.json
+-rw-rw-rw-   0        0        0     1656 2023-05-15 09:00:39.000000 pypcs-0.0.4/pyPCS/MidiInputHandler.py
+-rw-rw-rw-   0        0        0     3362 2023-05-14 17:34:03.000000 pypcs-0.0.4/pyPCS/__init__.py
+-rw-rw-rw-   0        0        0    23593 2023-05-16 14:33:37.000000 pypcs-0.0.4/pyPCS/_basicData.py
+-rw-rw-rw-   0        0        0     3020 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/_player.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.758151 pypcs-0.0.4/pyPCS/basicGenerator/
+-rw-rw-rw-   0        0        0      364 2023-05-14 17:33:49.000000 pypcs-0.0.4/pyPCS/basicGenerator/__init__.py
+-rw-rw-rw-   0        0        0    10426 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/basicGenerator/basicGenerator.py
+-rw-rw-rw-   0        0        0     7163 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/chorder.py
+-rw-rw-rw-   0        0        0    45352 2023-05-17 14:15:11.000000 pypcs-0.0.4/pyPCS/circle_of_fifth.png
+-rw-rw-rw-   0        0        0      487 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/classmethod_dec.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.762138 pypcs-0.0.4/pyPCS/piecesGenerator/
+-rw-rw-rw-   0        0        0      154 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/piecesGenerator/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/piecesGenerator/pieces_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.768123 pypcs-0.0.4/pyPCS/series/
+-rw-rw-rw-   0        0        0      653 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/series/__init__.py
+-rw-rw-rw-   0        0        0    29983 2023-05-17 14:59:44.000000 pypcs-0.0.4/pyPCS/series/funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.771117 pypcs-0.0.4/pyPCS/series/images/
+-rw-rw-rw-   0        0        0    69072 2023-05-17 17:44:21.000000 pypcs-0.0.4/pyPCS/series/images/cof_show.png
+-rw-rw-rw-   0        0        0    83930 2023-05-17 17:54:00.000000 pypcs-0.0.4/pyPCS/series/images/cofs_show.png
+-rw-rw-rw-   0        0        0    25430 2023-05-17 17:16:38.000000 pypcs-0.0.4/pyPCS/series/series1d.py
+-rw-rw-rw-   0        0        0    25167 2023-05-15 08:35:30.000000 pypcs-0.0.4/pyPCS/series/series2d.py
+-rw-rw-rw-   0        0        0     4833 2023-05-08 05:43:04.000000 pypcs-0.0.4/pyPCS/series/tree.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.778097 pypcs-0.0.4/pypcs.egg-info/
+-rw-rw-rw-   0        0        0    13272 2023-05-17 19:21:49.000000 pypcs-0.0.4/pypcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2023-05-17 19:21:49.000000 pypcs-0.0.4/pypcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 19:21:49.000000 pypcs-0.0.4/pypcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-17 19:21:49.000000 pypcs-0.0.4/pypcs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 19:21:49.000000 pypcs-0.0.4/pypcs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 19:21:49.798043 pypcs-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-05-17 19:21:32.000000 pypcs-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.784081 pypcs-0.0.4/test/
+-rw-rw-rw-   0        0        0     2517 2023-05-16 13:00:44.000000 pypcs-0.0.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.787074 pypcs-0.0.4/test/basicGenerator/
+-rw-rw-rw-   0        0        0       26 2023-05-15 08:57:40.000000 pypcs-0.0.4/test/basicGenerator/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-05-15 08:58:51.000000 pypcs-0.0.4/test/basicGenerator/test_basicGenerator.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.790065 pypcs-0.0.4/test/piecesGenerator/
+-rw-rw-rw-   0        0        0       99 2023-05-15 08:58:51.000000 pypcs-0.0.4/test/piecesGenerator/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 08:58:51.000000 pypcs-0.0.4/test/piecesGenerator/test_pieces_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:21:49.796049 pypcs-0.0.4/test/series/
+-rw-rw-rw-   0        0        0      352 2023-05-15 08:57:52.000000 pypcs-0.0.4/test/series/__init__.py
+-rw-rw-rw-   0        0        0     3679 2023-05-14 21:28:30.000000 pypcs-0.0.4/test/series/test_funcs.py
+-rw-rw-rw-   0        0        0    12028 2023-05-17 17:57:22.000000 pypcs-0.0.4/test/series/test_series1d.py
+-rw-rw-rw-   0        0        0     1994 2023-05-15 08:49:15.000000 pypcs-0.0.4/test/series/test_series2d.py
+-rw-rw-rw-   0        0        0     4833 2023-05-08 05:43:04.000000 pypcs-0.0.4/test/series/test_tree.py
+-rw-rw-rw-   0        0        0      474 2023-05-15 08:55:20.000000 pypcs-0.0.4/test/test_MidiInputHandler.py
+-rw-rw-rw-   0        0        0      430 2023-05-14 17:14:53.000000 pypcs-0.0.4/test/test_chorder.py
+-rw-rw-rw-   0        0        0        2 2023-05-14 17:15:00.000000 pypcs-0.0.4/test/test_classmethod_dec.py
+-rw-rw-rw-   0        0        0      271 2023-05-14 17:11:03.000000 pypcs-0.0.4/test/test_player.py
```

### Comparing `pypcs-0.0.3/LICENSE` & `pypcs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/PKG-INFO` & `pypcs-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypcs
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/JasonLee-p/pyPCS
 Author: Jason Lee
 Author-email: 2593292614@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pypcs-0.0.3/README.md` & `pypcs-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/ChordAttr.json` & `pypcs-0.0.4/pyPCS/ChordAttr.json`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/MidiInputHandler.py` & `pypcs-0.0.4/pyPCS/MidiInputHandler.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/__init__.py` & `pypcs-0.0.4/pyPCS/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/_basicData.py` & `pypcs-0.0.4/pyPCS/_basicData.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/_player.py` & `pypcs-0.0.4/pyPCS/_player.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/basicGenerator/basicGenerator.py` & `pypcs-0.0.4/pyPCS/basicGenerator/basicGenerator.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/chorder.py` & `pypcs-0.0.4/pyPCS/chorder.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/circle_of_fifth.png` & `pypcs-0.0.4/pyPCS/circle_of_fifth.png`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/series/__init__.py` & `pypcs-0.0.4/pyPCS/series/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/series/funcs.py` & `pypcs-0.0.4/pyPCS/series/funcs.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/series/images/cof_show.png` & `pypcs-0.0.4/pyPCS/series/images/cof_show.png`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/series/images/cofs_show.png` & `pypcs-0.0.4/pyPCS/series/images/cofs_show.png`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/series/series1d.py` & `pypcs-0.0.4/pyPCS/series/series1d.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/series/series2d.py` & `pypcs-0.0.4/pyPCS/series/series2d.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pyPCS/series/tree.py` & `pypcs-0.0.4/pyPCS/series/tree.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/pypcs.egg-info/PKG-INFO` & `pypcs-0.0.4/pypcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypcs
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/JasonLee-p/pyPCS
 Author: Jason Lee
 Author-email: 2593292614@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pypcs-0.0.3/pypcs.egg-info/SOURCES.txt` & `pypcs-0.0.4/pypcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/setup.py` & `pypcs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = 3
+VERSION = 4
 
 
 setuptools.setup(
     name="pypcs",
     version='0.0.' + str(VERSION),
     author="Jason Lee",
     author_email="2593292614@qq.com",
```

### Comparing `pypcs-0.0.3/test/__init__.py` & `pypcs-0.0.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/test/series/test_funcs.py` & `pypcs-0.0.4/test/series/test_funcs.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/test/series/test_series1d.py` & `pypcs-0.0.4/test/series/test_series1d.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/test/series/test_series2d.py` & `pypcs-0.0.4/test/series/test_series2d.py`

 * *Files identical despite different names*

### Comparing `pypcs-0.0.3/test/series/test_tree.py` & `pypcs-0.0.4/test/series/test_tree.py`

 * *Files identical despite different names*

