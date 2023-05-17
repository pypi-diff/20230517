# Comparing `tmp/XS-treatment-0.0.5.4.tar.gz` & `tmp/XS-treatment-0.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XS-treatment-0.0.5.4.tar", last modified: Tue Nov 29 13:32:28 2022, max compression
+gzip compressed data, was "XS-treatment-0.0.5.5.tar", last modified: Wed May 17 01:50:45 2023, max compression
```

## Comparing `XS-treatment-0.0.5.4.tar` & `XS-treatment-0.0.5.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 standard  (1000) standard  (1000)        0 2022-11-29 13:32:28.441438 XS-treatment-0.0.5.4/
--rw-rw-r--   0 standard  (1000) standard  (1000)     2382 2022-11-29 13:32:28.441438 XS-treatment-0.0.5.4/PKG-INFO
--rw-rw-r--   0 standard  (1000) standard  (1000)     1803 2022-11-24 17:48:08.000000 XS-treatment-0.0.5.4/README.md
--rw-rw-r--   0 standard  (1000) standard  (1000)     1072 2022-11-29 13:18:01.000000 XS-treatment-0.0.5.4/pyproject.toml
--rw-rw-r--   0 standard  (1000) standard  (1000)       38 2022-11-29 13:32:28.441438 XS-treatment-0.0.5.4/setup.cfg
-drwxrwxr-x   0 standard  (1000) standard  (1000)        0 2022-11-29 13:32:28.433438 XS-treatment-0.0.5.4/src/
-drwxrwxr-x   0 standard  (1000) standard  (1000)        0 2022-11-29 13:32:28.437438 XS-treatment-0.0.5.4/src/XS-treatment/
--rwxrwxr-x   0 standard  (1000) standard  (1000)     1908 2022-11-29 13:19:04.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_A_checklib.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    12731 2022-11-29 13:24:58.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_azimuthalaverage.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    11362 2022-11-29 13:22:21.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_curveadd.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     8809 2022-11-29 13:22:45.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_curveplot.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    36967 2022-11-29 13:23:16.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_extractlog.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    10637 2022-11-29 13:23:36.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_getbeamcenter.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    10325 2022-11-29 13:20:03.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_help.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    12255 2022-11-29 13:26:05.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_imageadd.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    10677 2022-11-29 13:26:25.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_imagemerge.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     3917 2022-11-29 13:26:41.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_imageplot.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    14940 2022-11-29 13:27:00.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_libazimuthalaverage.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    12561 2022-11-29 13:27:13.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_libfileutils.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     4030 2022-11-24 17:48:08.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_libgetbeamcenter.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     5979 2022-11-29 13:27:36.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_libimageplot.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    11953 2022-11-29 13:27:51.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_libnormalizations.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    34810 2022-11-29 13:28:11.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_libreadparameters.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     3701 2022-11-24 17:48:08.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_maskconv.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     4588 2022-11-29 13:28:54.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_menu.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     9339 2022-11-29 13:29:05.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_ponifile.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)    22498 2022-11-29 13:29:23.000000 XS-treatment-0.0.5.4/src/XS-treatment/XS_radialaverage.py
--rw-rw-r--   0 standard  (1000) standard  (1000)      627 2022-11-28 14:44:52.000000 XS-treatment-0.0.5.4/src/XS-treatment/__init__.py
--rwxrwxr-x   0 standard  (1000) standard  (1000)     2561 2022-11-29 13:19:41.000000 XS-treatment-0.0.5.4/src/XS-treatment/clponize.py
-drwxrwxr-x   0 standard  (1000) standard  (1000)        0 2022-11-29 13:32:28.441438 XS-treatment-0.0.5.4/src/XS_treatment.egg-info/
--rw-rw-r--   0 standard  (1000) standard  (1000)     2382 2022-11-29 13:32:28.000000 XS-treatment-0.0.5.4/src/XS_treatment.egg-info/PKG-INFO
--rw-rw-r--   0 standard  (1000) standard  (1000)      984 2022-11-29 13:32:28.000000 XS-treatment-0.0.5.4/src/XS_treatment.egg-info/SOURCES.txt
--rw-rw-r--   0 standard  (1000) standard  (1000)        1 2022-11-29 13:32:28.000000 XS-treatment-0.0.5.4/src/XS_treatment.egg-info/dependency_links.txt
--rw-rw-r--   0 standard  (1000) standard  (1000)      153 2022-11-29 13:32:28.000000 XS-treatment-0.0.5.4/src/XS_treatment.egg-info/requires.txt
--rw-rw-r--   0 standard  (1000) standard  (1000)       13 2022-11-29 13:32:28.000000 XS-treatment-0.0.5.4/src/XS_treatment.egg-info/top_level.txt
+drwxrwxr-x   0 standard02  (1000) standard02  (1000)        0 2023-05-17 01:50:45.889861 XS-treatment-0.0.5.5/
+-rw-rw-r--   0 standard02  (1000) standard02  (1000)     2382 2023-05-17 01:50:45.889861 XS-treatment-0.0.5.5/PKG-INFO
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     1803 2022-11-24 17:48:08.000000 XS-treatment-0.0.5.5/README.md
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     1065 2023-05-17 01:49:10.000000 XS-treatment-0.0.5.5/pyproject.toml
+-rw-rw-r--   0 standard02  (1000) standard02  (1000)       38 2023-05-17 01:50:45.889861 XS-treatment-0.0.5.5/setup.cfg
+drwxrwxr-x   0 standard02  (1000) standard02  (1000)        0 2023-05-17 01:50:45.889861 XS-treatment-0.0.5.5/src/
+drwxrwxr-x   0 standard02  (1000) standard02  (1000)        0 2023-05-17 01:50:45.889861 XS-treatment-0.0.5.5/src/XS-treatment/
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     1908 2022-11-29 13:19:04.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_A_checklib.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    12731 2022-11-29 13:24:58.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_azimuthalaverage.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    11362 2022-11-29 13:22:21.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_curveadd.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     8809 2022-11-29 13:22:45.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_curveplot.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    36967 2022-11-29 13:23:16.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_extractlog.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    10637 2022-11-29 13:23:36.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_getbeamcenter.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    10325 2022-11-29 13:20:03.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_help.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    12255 2022-11-29 13:26:05.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_imageadd.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    10677 2022-11-29 13:26:25.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_imagemerge.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     3917 2022-11-29 13:26:41.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_imageplot.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    14940 2022-11-29 13:27:00.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_libazimuthalaverage.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    12561 2022-11-29 13:27:13.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_libfileutils.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     4030 2022-11-24 17:48:08.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_libgetbeamcenter.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     5979 2022-11-29 13:27:36.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_libimageplot.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    11953 2022-11-29 13:27:51.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_libnormalizations.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    34810 2022-11-29 13:28:11.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_libreadparameters.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     3701 2022-11-24 17:48:08.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_maskconv.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     4588 2022-11-29 13:28:54.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_menu.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     9339 2022-11-29 13:29:05.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_ponifile.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)    22498 2022-11-29 13:29:23.000000 XS-treatment-0.0.5.5/src/XS-treatment/XS_radialaverage.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)      627 2022-11-28 14:44:52.000000 XS-treatment-0.0.5.5/src/XS-treatment/__init__.py
+-rwxrwxrwx   0 standard02  (1000) standard02  (1000)     2561 2022-11-29 13:19:41.000000 XS-treatment-0.0.5.5/src/XS-treatment/clponize.py
+drwxrwxr-x   0 standard02  (1000) standard02  (1000)        0 2023-05-17 01:50:45.889861 XS-treatment-0.0.5.5/src/XS_treatment.egg-info/
+-rw-rw-r--   0 standard02  (1000) standard02  (1000)     2382 2023-05-17 01:50:45.000000 XS-treatment-0.0.5.5/src/XS_treatment.egg-info/PKG-INFO
+-rw-rw-r--   0 standard02  (1000) standard02  (1000)      984 2023-05-17 01:50:45.000000 XS-treatment-0.0.5.5/src/XS_treatment.egg-info/SOURCES.txt
+-rw-rw-r--   0 standard02  (1000) standard02  (1000)        1 2023-05-17 01:50:45.000000 XS-treatment-0.0.5.5/src/XS_treatment.egg-info/dependency_links.txt
+-rw-rw-r--   0 standard02  (1000) standard02  (1000)      153 2023-05-17 01:50:45.000000 XS-treatment-0.0.5.5/src/XS_treatment.egg-info/requires.txt
+-rw-rw-r--   0 standard02  (1000) standard02  (1000)       13 2023-05-17 01:50:45.000000 XS-treatment-0.0.5.5/src/XS_treatment.egg-info/top_level.txt
```

### Comparing `XS-treatment-0.0.5.4/PKG-INFO` & `XS-treatment-0.0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XS-treatment
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: XS-treatment suite for SAXS/WAXS data treatment.
 Author-email: "Arnaldo G. Oliveira-Filho" <agolivei@if.usp.br>, Dennys Reis <dreis@if.usp.br>
 Project-URL: Homepage, https://gitlab.uspdigital.usp.br/gfcx/XS-treatment.git
 Project-URL: Bug Tracker, https://gitlab.uspdigital.usp.br/gfcx/XS-treatment.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XS-treatment-0.0.5.4/README.md` & `XS-treatment-0.0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/pyproject.toml` & `XS-treatment-0.0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools","cython", "numpy","matplotlib","numba  @ git+https://github.com/numba/numba@0.56.4", "fabio @ git+https://github.com/silx-kit/fabio@master" ]
+requires = ["setuptools","cython", "numpy","matplotlib","numba  @ git+https://github.com/numba/numba@0.56.4", "fabio @ git+https://github.com/silx-kit/fabio" ]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "XS-treatment"
-version = "0.0.5.4"
+version = "0.0.5.5"
 authors = [
   { name="Arnaldo G. Oliveira-Filho", email="agolivei@if.usp.br" },
   { name="Dennys Reis", email="dreis@if.usp.br" },
 ]
 
 dependencies = ["math", "calendar", "copy", "datetime", "errno", "getopt",
 "glob", "gzip",
```

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_A_checklib.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_A_checklib.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_azimuthalaverage.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_azimuthalaverage.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_curveadd.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_curveadd.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_curveplot.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_curveplot.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_extractlog.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_extractlog.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_getbeamcenter.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_getbeamcenter.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_help.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_help.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_imageadd.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_imageadd.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_imagemerge.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_imagemerge.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_imageplot.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_imageplot.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_libazimuthalaverage.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_libazimuthalaverage.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_libfileutils.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_libfileutils.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_libgetbeamcenter.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_libgetbeamcenter.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_libimageplot.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_libimageplot.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_libnormalizations.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_libnormalizations.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_libreadparameters.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_libreadparameters.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_maskconv.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_maskconv.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_menu.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_menu.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_ponifile.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_ponifile.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/XS_radialaverage.py` & `XS-treatment-0.0.5.5/src/XS-treatment/XS_radialaverage.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/__init__.py` & `XS-treatment-0.0.5.5/src/XS-treatment/__init__.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS-treatment/clponize.py` & `XS-treatment-0.0.5.5/src/XS-treatment/clponize.py`

 * *Files identical despite different names*

### Comparing `XS-treatment-0.0.5.4/src/XS_treatment.egg-info/PKG-INFO` & `XS-treatment-0.0.5.5/src/XS_treatment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XS-treatment
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: XS-treatment suite for SAXS/WAXS data treatment.
 Author-email: "Arnaldo G. Oliveira-Filho" <agolivei@if.usp.br>, Dennys Reis <dreis@if.usp.br>
 Project-URL: Homepage, https://gitlab.uspdigital.usp.br/gfcx/XS-treatment.git
 Project-URL: Bug Tracker, https://gitlab.uspdigital.usp.br/gfcx/XS-treatment.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XS-treatment-0.0.5.4/src/XS_treatment.egg-info/SOURCES.txt` & `XS-treatment-0.0.5.5/src/XS_treatment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

