# Comparing `tmp/dustpylib-0.4.0.tar.gz` & `tmp/dustpylib-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustpylib-0.4.0.tar", last modified: Wed May 17 12:17:30 2023, max compression
+gzip compressed data, was "dustpylib-0.4.0rc0.tar", last modified: Tue May 16 15:39:38 2023, max compression
```

## Comparing `dustpylib-0.4.0.tar` & `dustpylib-0.4.0rc0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:30.117055 dustpylib-0.4.0/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1505 2023-04-19 09:53:48.000000 dustpylib-0.4.0/LICENSE
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      241 2023-04-27 17:40:52.000000 dustpylib-0.4.0/MANIFEST.in
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3054 2023-05-17 12:17:30.114053 dustpylib-0.4.0/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1927 2023-05-05 08:25:55.000000 dustpylib-0.4.0/README.md
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:28.719135 dustpylib-0.4.0/docs/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      637 2023-04-27 14:03:17.000000 dustpylib-0.4.0/docs/Makefile
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      763 2023-04-27 14:02:49.000000 dustpylib-0.4.0/docs/make.bat
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      166 2023-04-27 17:33:15.000000 dustpylib-0.4.0/docs/requirements.txt
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.333660 dustpylib-0.4.0/docs/source/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2803 2023-04-27 14:49:18.000000 dustpylib-0.4.0/docs/source/A_contrib_bug_feature.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      655 2023-04-29 20:42:06.000000 dustpylib-0.4.0/docs/source/api.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1962 2023-05-03 15:14:00.000000 dustpylib-0.4.0/docs/source/conf.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      150 2023-04-29 20:41:23.000000 dustpylib-0.4.0/docs/source/grid.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   185592 2023-05-05 09:08:42.000000 dustpylib-0.4.0/docs/source/grid_refinement.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      876 2023-04-29 20:40:27.000000 dustpylib-0.4.0/docs/source/index.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   254410 2023-05-17 12:10:15.000000 dustpylib-0.4.0/docs/source/planetary_gaps.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    25639 2023-05-05 09:08:47.000000 dustpylib-0.4.0/docs/source/planetesimal_formation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      224 2023-04-29 17:08:50.000000 dustpylib-0.4.0/docs/source/planetesimals.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1953166 2023-05-16 15:38:41.000000 dustpylib-0.4.0/docs/source/radmc3d.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      369 2023-04-29 17:09:25.000000 dustpylib-0.4.0/docs/source/radtrans.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      204 2023-04-29 20:40:49.000000 dustpylib-0.4.0/docs/source/substructures.rst
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.369660 dustpylib-0.4.0/dustpylib/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      353 2023-05-17 12:10:38.000000 dustpylib-0.4.0/dustpylib/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.618053 dustpylib-0.4.0/dustpylib/grid/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      133 2023-04-29 19:39:21.000000 dustpylib-0.4.0/dustpylib/grid/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.707053 dustpylib-0.4.0/dustpylib/grid/refinement/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      127 2023-04-29 19:39:03.000000 dustpylib-0.4.0/dustpylib/grid/refinement/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1200 2023-04-29 20:25:00.000000 dustpylib-0.4.0/dustpylib/grid/refinement/refinement.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.743055 dustpylib-0.4.0/dustpylib/planetesimals/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      137 2023-04-29 13:09:13.000000 dustpylib-0.4.0/dustpylib/planetesimals/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.825053 dustpylib-0.4.0/dustpylib/planetesimals/formation/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      361 2023-04-29 16:40:19.000000 dustpylib-0.4.0/dustpylib/planetesimals/formation/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3768 2023-04-30 08:03:28.000000 dustpylib-0.4.0/dustpylib/planetesimals/formation/formation.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.863055 dustpylib-0.4.0/dustpylib/radtrans/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      162 2023-04-28 16:08:04.000000 dustpylib-0.4.0/dustpylib/radtrans/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.944054 dustpylib-0.4.0/dustpylib/radtrans/radmc3d/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      417 2023-04-28 16:07:22.000000 dustpylib-0.4.0/dustpylib/radtrans/radmc3d/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    28365 2023-05-16 15:33:43.000000 dustpylib-0.4.0/dustpylib/radtrans/radmc3d/radmc3d.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.984054 dustpylib-0.4.0/dustpylib/substructures/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      157 2023-04-29 17:32:32.000000 dustpylib-0.4.0/dustpylib/substructures/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:30.077060 dustpylib-0.4.0/dustpylib/substructures/gaps/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      248 2023-05-17 08:39:14.000000 dustpylib-0.4.0/dustpylib/substructures/gaps/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2220 2023-05-16 15:00:13.000000 dustpylib-0.4.0/dustpylib/substructures/gaps/gaps.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-17 12:17:29.582054 dustpylib-0.4.0/dustpylib.egg-info/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3054 2023-05-17 12:17:27.000000 dustpylib-0.4.0/dustpylib.egg-info/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1104 2023-05-17 12:17:28.000000 dustpylib-0.4.0/dustpylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-05-17 12:17:27.000000 dustpylib-0.4.0/dustpylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-04-27 15:54:48.000000 dustpylib-0.4.0/dustpylib.egg-info/not-zip-safe
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       59 2023-05-17 12:17:27.000000 dustpylib-0.4.0/dustpylib.egg-info/requires.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       10 2023-05-17 12:17:27.000000 dustpylib-0.4.0/dustpylib.egg-info/top_level.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-05-17 12:17:30.118058 dustpylib-0.4.0/setup.cfg
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2133 2023-04-27 17:33:26.000000 dustpylib-0.4.0/setup.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:40.312659 dustpylib-0.4.0rc0/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1505 2023-04-19 09:53:48.000000 dustpylib-0.4.0rc0/LICENSE
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      241 2023-04-27 17:40:52.000000 dustpylib-0.4.0rc0/MANIFEST.in
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3057 2023-05-16 15:39:40.307669 dustpylib-0.4.0rc0/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1927 2023-05-05 08:25:55.000000 dustpylib-0.4.0rc0/README.md
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:38.875665 dustpylib-0.4.0rc0/docs/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      637 2023-04-27 14:03:17.000000 dustpylib-0.4.0rc0/docs/Makefile
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      763 2023-04-27 14:02:49.000000 dustpylib-0.4.0rc0/docs/make.bat
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      166 2023-04-27 17:33:15.000000 dustpylib-0.4.0rc0/docs/requirements.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:39.502660 dustpylib-0.4.0rc0/docs/source/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2803 2023-04-27 14:49:18.000000 dustpylib-0.4.0rc0/docs/source/A_contrib_bug_feature.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      655 2023-04-29 20:42:06.000000 dustpylib-0.4.0rc0/docs/source/api.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1962 2023-05-03 15:14:00.000000 dustpylib-0.4.0rc0/docs/source/conf.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      150 2023-04-29 20:41:23.000000 dustpylib-0.4.0rc0/docs/source/grid.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   185592 2023-05-05 09:08:42.000000 dustpylib-0.4.0rc0/docs/source/grid_refinement.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      876 2023-04-29 20:40:27.000000 dustpylib-0.4.0rc0/docs/source/index.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   254410 2023-05-16 15:00:55.000000 dustpylib-0.4.0rc0/docs/source/planetary_gaps.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    25639 2023-05-05 09:08:47.000000 dustpylib-0.4.0rc0/docs/source/planetesimal_formation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      224 2023-04-29 17:08:50.000000 dustpylib-0.4.0rc0/docs/source/planetesimals.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1953166 2023-05-16 15:38:41.000000 dustpylib-0.4.0rc0/docs/source/radmc3d.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      369 2023-04-29 17:09:25.000000 dustpylib-0.4.0rc0/docs/source/radtrans.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      204 2023-04-29 20:40:49.000000 dustpylib-0.4.0rc0/docs/source/substructures.rst
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:39.538667 dustpylib-0.4.0rc0/dustpylib/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      357 2023-05-16 15:39:21.000000 dustpylib-0.4.0rc0/dustpylib/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:39.786664 dustpylib-0.4.0rc0/dustpylib/grid/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      133 2023-04-29 19:39:21.000000 dustpylib-0.4.0rc0/dustpylib/grid/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:39.884658 dustpylib-0.4.0rc0/dustpylib/grid/refinement/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      127 2023-04-29 19:39:03.000000 dustpylib-0.4.0rc0/dustpylib/grid/refinement/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1200 2023-04-29 20:25:00.000000 dustpylib-0.4.0rc0/dustpylib/grid/refinement/refinement.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:39.930657 dustpylib-0.4.0rc0/dustpylib/planetesimals/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      137 2023-04-29 13:09:13.000000 dustpylib-0.4.0rc0/dustpylib/planetesimals/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:40.018660 dustpylib-0.4.0rc0/dustpylib/planetesimals/formation/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      361 2023-04-29 16:40:19.000000 dustpylib-0.4.0rc0/dustpylib/planetesimals/formation/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3768 2023-04-30 08:03:28.000000 dustpylib-0.4.0rc0/dustpylib/planetesimals/formation/formation.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:40.055664 dustpylib-0.4.0rc0/dustpylib/radtrans/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      162 2023-04-28 16:08:04.000000 dustpylib-0.4.0rc0/dustpylib/radtrans/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:40.143660 dustpylib-0.4.0rc0/dustpylib/radtrans/radmc3d/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      417 2023-04-28 16:07:22.000000 dustpylib-0.4.0rc0/dustpylib/radtrans/radmc3d/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    28365 2023-05-16 15:33:43.000000 dustpylib-0.4.0rc0/dustpylib/radtrans/radmc3d/radmc3d.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:40.182659 dustpylib-0.4.0rc0/dustpylib/substructures/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      157 2023-04-29 17:32:32.000000 dustpylib-0.4.0rc0/dustpylib/substructures/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:40.269660 dustpylib-0.4.0rc0/dustpylib/substructures/gaps/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      247 2023-05-16 13:45:50.000000 dustpylib-0.4.0rc0/dustpylib/substructures/gaps/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2220 2023-05-16 15:00:13.000000 dustpylib-0.4.0rc0/dustpylib/substructures/gaps/gaps.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-16 15:39:39.748658 dustpylib-0.4.0rc0/dustpylib.egg-info/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3057 2023-05-16 15:39:37.000000 dustpylib-0.4.0rc0/dustpylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1104 2023-05-16 15:39:38.000000 dustpylib-0.4.0rc0/dustpylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-05-16 15:39:37.000000 dustpylib-0.4.0rc0/dustpylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-04-27 15:54:48.000000 dustpylib-0.4.0rc0/dustpylib.egg-info/not-zip-safe
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       59 2023-05-16 15:39:37.000000 dustpylib-0.4.0rc0/dustpylib.egg-info/requires.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       10 2023-05-16 15:39:37.000000 dustpylib-0.4.0rc0/dustpylib.egg-info/top_level.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-05-16 15:39:40.313658 dustpylib-0.4.0rc0/setup.cfg
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2133 2023-04-27 17:33:26.000000 dustpylib-0.4.0rc0/setup.py
```

### Comparing `dustpylib-0.4.0/LICENSE` & `dustpylib-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/PKG-INFO` & `dustpylib-0.4.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustpylib
-Version: 0.4.0
+Version: 0.4.0rc0
 Home-page: https://github.com/stammler/dustpylib/
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/dustpylib/
 Project-URL: Documentation, https://dustpylib.rtfd.io/
```

### Comparing `dustpylib-0.4.0/README.md` & `dustpylib-0.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/Makefile` & `dustpylib-0.4.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/make.bat` & `dustpylib-0.4.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/A_contrib_bug_feature.ipynb` & `dustpylib-0.4.0rc0/docs/source/A_contrib_bug_feature.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/api.rst` & `dustpylib-0.4.0rc0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/conf.py` & `dustpylib-0.4.0rc0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/grid_refinement.ipynb` & `dustpylib-0.4.0rc0/docs/source/grid_refinement.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/index.rst` & `dustpylib-0.4.0rc0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/planetary_gaps.ipynb` & `dustpylib-0.4.0rc0/docs/source/planetary_gaps.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/planetesimal_formation.ipynb` & `dustpylib-0.4.0rc0/docs/source/planetesimal_formation.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/docs/source/radmc3d.ipynb` & `dustpylib-0.4.0rc0/docs/source/radmc3d.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/dustpylib/grid/refinement/refinement.py` & `dustpylib-0.4.0rc0/dustpylib/grid/refinement/refinement.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/dustpylib/planetesimals/formation/formation.py` & `dustpylib-0.4.0rc0/dustpylib/planetesimals/formation/formation.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/dustpylib/radtrans/radmc3d/radmc3d.py` & `dustpylib-0.4.0rc0/dustpylib/radtrans/radmc3d/radmc3d.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/dustpylib/substructures/gaps/gaps.py` & `dustpylib-0.4.0rc0/dustpylib/substructures/gaps/gaps.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/dustpylib.egg-info/PKG-INFO` & `dustpylib-0.4.0rc0/dustpylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustpylib
-Version: 0.4.0
+Version: 0.4.0rc0
 Home-page: https://github.com/stammler/dustpylib/
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/dustpylib/
 Project-URL: Documentation, https://dustpylib.rtfd.io/
```

### Comparing `dustpylib-0.4.0/dustpylib.egg-info/SOURCES.txt` & `dustpylib-0.4.0rc0/dustpylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dustpylib-0.4.0/setup.py` & `dustpylib-0.4.0rc0/setup.py`

 * *Files identical despite different names*

