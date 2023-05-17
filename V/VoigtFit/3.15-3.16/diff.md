# Comparing `tmp/VoigtFit-3.15.tar.gz` & `tmp/VoigtFit-3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VoigtFit-3.15.tar", last modified: Wed Feb 15 13:31:14 2023, max compression
+gzip compressed data, was "VoigtFit-3.16.tar", last modified: Wed May 17 08:46:58 2023, max compression
```

## Comparing `VoigtFit-3.15.tar` & `VoigtFit-3.16.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.976636 VoigtFit-3.15/
--rw-r--r--   0 krogager   (501) staff       (20)      248 2022-03-27 13:11:46.000000 VoigtFit-3.15/AUTHORS.rst
--rw-r--r--   0 krogager   (501) staff       (20)     1095 2022-03-27 13:11:46.000000 VoigtFit-3.15/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)       90 2022-03-27 13:11:46.000000 VoigtFit-3.15/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)     2974 2023-02-15 13:31:14.976498 VoigtFit-3.15/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2393 2022-05-03 11:48:30.000000 VoigtFit-3.15/README.rst
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.968911 VoigtFit-3.15/VoigtFit/
--rw-r--r--   0 krogager   (501) staff       (20)        5 2023-02-15 13:18:53.000000 VoigtFit-3.15/VoigtFit/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1313 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)       71 2022-05-03 13:06:10.000000 VoigtFit-3.15/VoigtFit/__main__.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.970759 VoigtFit-3.15/VoigtFit/container/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/container/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     5401 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/container/components.py
--rw-r--r--   0 krogager   (501) staff       (20)   102336 2022-06-17 12:53:58.000000 VoigtFit-3.15/VoigtFit/container/dataset.py
--rw-r--r--   0 krogager   (501) staff       (20)     4466 2022-07-21 13:29:16.000000 VoigtFit-3.15/VoigtFit/container/lines.py
--rw-r--r--   0 krogager   (501) staff       (20)    23426 2022-07-21 13:29:16.000000 VoigtFit-3.15/VoigtFit/container/regions.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.971087 VoigtFit-3.15/VoigtFit/funcs/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/funcs/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     4009 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/funcs/limits.py
--rw-r--r--   0 krogager   (501) staff       (20)    13357 2023-02-15 13:28:01.000000 VoigtFit-3.15/VoigtFit/funcs/voigt.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.971816 VoigtFit-3.15/VoigtFit/io/
--rw-r--r--   0 krogager   (501) staff       (20)       43 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/io/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)    16618 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/io/fits_input.py
--rw-r--r--   0 krogager   (501) staff       (20)    16812 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/io/hdf5_save.py
--rw-r--r--   0 krogager   (501) staff       (20)    81016 2023-02-15 13:28:38.000000 VoigtFit-3.15/VoigtFit/io/output.py
--rw-r--r--   0 krogager   (501) staff       (20)    28670 2022-06-17 12:53:58.000000 VoigtFit-3.15/VoigtFit/io/parse_input.py
--rw-r--r--   0 krogager   (501) staff       (20)    25072 2022-07-21 13:18:40.000000 VoigtFit-3.15/VoigtFit/main.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.973563 VoigtFit-3.15/VoigtFit/static/
--rw-r--r--   0 krogager   (501) staff       (20)     2116 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/static/Asplund2009.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2747 2022-07-21 13:05:22.000000 VoigtFit-3.15/VoigtFit/static/Asplund2021.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2435 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/static/C_complexes.dat
--rw-r--r--   0 krogager   (501) staff       (20)     5437 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/static/C_full_labels.txt
--rw-r--r--   0 krogager   (501) staff       (20)     2750 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/static/Lodders2009.dat
--rw-r--r--   0 krogager   (501) staff       (20)     5328 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/static/input_template.txt
--rw-r--r--   0 krogager   (501) staff       (20)   168716 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/static/linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)  2536616 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/static/telluric_em_abs.npz
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.976174 VoigtFit-3.15/VoigtFit/utils/
--rw-r--r--   0 krogager   (501) staff       (20)     1285 2022-07-21 13:29:16.000000 VoigtFit-3.15/VoigtFit/utils/Asplund.py
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/utils/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     2625 2022-07-21 13:29:16.000000 VoigtFit-3.15/VoigtFit/utils/line_complexes.py
--rw-r--r--   0 krogager   (501) staff       (20)    23052 2022-05-03 11:57:56.000000 VoigtFit-3.15/VoigtFit/utils/molecules.py
--rw-r--r--   0 krogager   (501) staff       (20)      603 2022-03-27 13:11:46.000000 VoigtFit-3.15/VoigtFit/utils/terminal_attributes.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-02-15 13:31:14.969611 VoigtFit-3.15/VoigtFit.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)     2974 2023-02-15 13:31:14.000000 VoigtFit-3.15/VoigtFit.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     1087 2023-02-15 13:31:14.000000 VoigtFit-3.15/VoigtFit.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2023-02-15 13:31:14.000000 VoigtFit-3.15/VoigtFit.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)       48 2023-02-15 13:31:14.000000 VoigtFit-3.15/VoigtFit.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)       54 2023-02-15 13:31:14.000000 VoigtFit-3.15/VoigtFit.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        9 2023-02-15 13:31:14.000000 VoigtFit-3.15/VoigtFit.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)       38 2023-02-15 13:31:14.976670 VoigtFit-3.15/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5137 2022-05-03 13:02:06.000000 VoigtFit-3.15/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.821203 VoigtFit-3.16/
+-rw-r--r--   0 krogager   (501) staff       (20)      248 2022-03-27 13:11:46.000000 VoigtFit-3.16/AUTHORS.rst
+-rw-r--r--   0 krogager   (501) staff       (20)     1095 2022-03-27 13:11:46.000000 VoigtFit-3.16/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)       90 2022-03-27 13:11:46.000000 VoigtFit-3.16/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)     2974 2023-05-17 08:46:58.821081 VoigtFit-3.16/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2393 2022-05-03 11:48:30.000000 VoigtFit-3.16/README.rst
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.811543 VoigtFit-3.16/VoigtFit/
+-rw-r--r--   0 krogager   (501) staff       (20)        5 2023-05-17 08:44:47.000000 VoigtFit-3.16/VoigtFit/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1313 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)       71 2022-05-03 13:06:10.000000 VoigtFit-3.16/VoigtFit/__main__.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.813751 VoigtFit-3.16/VoigtFit/container/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/container/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5401 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/container/components.py
+-rw-r--r--   0 krogager   (501) staff       (20)   102336 2022-06-17 12:53:58.000000 VoigtFit-3.16/VoigtFit/container/dataset.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4466 2022-07-21 13:29:16.000000 VoigtFit-3.16/VoigtFit/container/lines.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23426 2022-07-21 13:29:16.000000 VoigtFit-3.16/VoigtFit/container/regions.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.814366 VoigtFit-3.16/VoigtFit/funcs/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/funcs/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4009 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/funcs/limits.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13357 2023-02-15 13:28:01.000000 VoigtFit-3.16/VoigtFit/funcs/voigt.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.815749 VoigtFit-3.16/VoigtFit/io/
+-rw-r--r--   0 krogager   (501) staff       (20)       43 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/io/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)    16618 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/io/fits_input.py
+-rw-r--r--   0 krogager   (501) staff       (20)    16812 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/io/hdf5_save.py
+-rw-r--r--   0 krogager   (501) staff       (20)    81016 2023-02-15 13:28:38.000000 VoigtFit-3.16/VoigtFit/io/output.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28670 2022-06-17 12:53:58.000000 VoigtFit-3.16/VoigtFit/io/parse_input.py
+-rw-r--r--   0 krogager   (501) staff       (20)    25086 2023-05-17 08:44:21.000000 VoigtFit-3.16/VoigtFit/main.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.817237 VoigtFit-3.16/VoigtFit/static/
+-rw-r--r--   0 krogager   (501) staff       (20)     2116 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/static/Asplund2009.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2747 2022-07-21 13:05:22.000000 VoigtFit-3.16/VoigtFit/static/Asplund2021.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2435 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/static/C_complexes.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     5437 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/static/C_full_labels.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      561 2023-05-17 08:46:43.000000 VoigtFit-3.16/VoigtFit/static/Konstantopoulou2022.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2750 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/static/Lodders2009.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     5328 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/static/input_template.txt
+-rw-r--r--   0 krogager   (501) staff       (20)   168728 2023-05-17 08:46:43.000000 VoigtFit-3.16/VoigtFit/static/linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)  2536616 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/static/telluric_em_abs.npz
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.820798 VoigtFit-3.16/VoigtFit/utils/
+-rw-r--r--   0 krogager   (501) staff       (20)     1285 2022-07-21 13:29:16.000000 VoigtFit-3.16/VoigtFit/utils/Asplund.py
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/utils/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)      638 2023-05-17 08:46:43.000000 VoigtFit-3.16/VoigtFit/utils/depletion.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2625 2022-07-21 13:29:16.000000 VoigtFit-3.16/VoigtFit/utils/line_complexes.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23052 2022-05-03 11:57:56.000000 VoigtFit-3.16/VoigtFit/utils/molecules.py
+-rw-r--r--   0 krogager   (501) staff       (20)      603 2022-03-27 13:11:46.000000 VoigtFit-3.16/VoigtFit/utils/terminal_attributes.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-17 08:46:58.812561 VoigtFit-3.16/VoigtFit.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)     2974 2023-05-17 08:46:58.000000 VoigtFit-3.16/VoigtFit.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     1155 2023-05-17 08:46:58.000000 VoigtFit-3.16/VoigtFit.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2023-05-17 08:46:58.000000 VoigtFit-3.16/VoigtFit.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       48 2023-05-17 08:46:58.000000 VoigtFit-3.16/VoigtFit.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       54 2023-05-17 08:46:58.000000 VoigtFit-3.16/VoigtFit.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        9 2023-05-17 08:46:58.000000 VoigtFit-3.16/VoigtFit.egg-info/top_level.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2023-05-17 08:46:58.821232 VoigtFit-3.16/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5137 2022-05-03 13:02:06.000000 VoigtFit-3.16/setup.py
```

### Comparing `VoigtFit-3.15/LICENSE` & `VoigtFit-3.16/LICENSE`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/PKG-INFO` & `VoigtFit-3.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoigtFit
-Version: 3.15
+Version: 3.16
 Summary: Voigt Profile Fitting in Python
 Home-page: https://github.com/jkrogager/VoigtFit
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: voigtfit absorption analysis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VoigtFit-3.15/README.rst` & `VoigtFit-3.16/README.rst`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/__init__.py` & `VoigtFit-3.16/VoigtFit/__init__.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/container/components.py` & `VoigtFit-3.16/VoigtFit/container/components.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/container/dataset.py` & `VoigtFit-3.16/VoigtFit/container/dataset.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/container/lines.py` & `VoigtFit-3.16/VoigtFit/container/lines.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/container/regions.py` & `VoigtFit-3.16/VoigtFit/container/regions.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/funcs/limits.py` & `VoigtFit-3.16/VoigtFit/funcs/limits.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/funcs/voigt.py` & `VoigtFit-3.16/VoigtFit/funcs/voigt.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/io/fits_input.py` & `VoigtFit-3.16/VoigtFit/io/fits_input.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/io/hdf5_save.py` & `VoigtFit-3.16/VoigtFit/io/hdf5_save.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/io/output.py` & `VoigtFit-3.16/VoigtFit/io/output.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/io/parse_input.py` & `VoigtFit-3.16/VoigtFit/io/parse_input.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/main.py` & `VoigtFit-3.16/VoigtFit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from argparse import ArgumentParser
 
 from VoigtFit import container
 from VoigtFit import io
 
 
-warnings.filterwarnings("ignore", category=matplotlib.mplDeprecation)
+warnings.filterwarnings("ignore", category=matplotlib.MatplotlibDeprecationWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
 
 plt.interactive(True)
 
 code_dir = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(code_dir, 'VERSION')) as version_file:
     version = version_file.read().strip()
```

### Comparing `VoigtFit-3.15/VoigtFit/static/Asplund2009.dat` & `VoigtFit-3.16/VoigtFit/static/Asplund2009.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/static/Asplund2021.dat` & `VoigtFit-3.16/VoigtFit/static/Asplund2021.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/static/C_complexes.dat` & `VoigtFit-3.16/VoigtFit/static/C_complexes.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/static/C_full_labels.txt` & `VoigtFit-3.16/VoigtFit/static/C_full_labels.txt`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/static/Lodders2009.dat` & `VoigtFit-3.16/VoigtFit/static/Lodders2009.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/static/input_template.txt` & `VoigtFit-3.16/VoigtFit/static/input_template.txt`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/static/linelist.dat` & `VoigtFit-3.16/VoigtFit/static/linelist.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1704,20 +1704,20 @@
 C13Ib_1561.44    C13Ib      1561.4240  6.01e-02  3.020e+08  13.003
 C13Ia_1656       C13Ia      1656.2710  5.98e-02  3.981e+08  13.003
 C13I_1656        C13I       1656.9320  1.43e-01  3.981e+08  13.003
 C13Ib_1657       C13Ib      1657.0120  1.07e-01  3.981e+08  13.003
 C13Ia_1657       C13Ia      1657.3831  3.56e-02  3.981e+08  13.003
 C13Ia_1657.9     C13Ia      1657.9160  4.76e-02  3.981e+08  13.003
 C13Ib_1658       C13Ib      1658.1250  3.57e-02  3.981e+08  13.003
-Mg25II_2796      MgII       2796.3480  6.29e-01  2.692e+08  24.305
-Mg26II_2796      MgII       2796.3442  6.29e-01  2.692e+08  24.305
-Mg25II_2803      MgII       2803.5268  3.08e-01  2.692e+08  24.305
-Mg26II_2803      MgII       2803.5230  3.08e-01  2.692e+08  24.305
-Mg25I_2852       MgI        2852.9622  1.80e+00  5.129e+08  24.305
-Mg26I_2852       MgI        2852.9604  1.80e+00  5.129e+08  24.305
+Mg25II_2796      Mg25II       2796.3480  6.29e-01  2.692e+08  24.305
+Mg26II_2796      Mg26II       2796.3442  6.29e-01  2.692e+08  24.305
+Mg25II_2803      Mg25II       2803.5268  3.08e-01  2.692e+08  24.305
+Mg26II_2803      Mg26II       2803.5230  3.08e-01  2.692e+08  24.305
+Mg25I_2852       Mg25I        2852.9622  1.80e+00  5.129e+08  24.305
+Mg26I_2852       Mg26I        2852.9604  1.80e+00  5.129e+08  24.305
 OIa_1304         OIa        1304.8576  4.78e-02  5.650e+08  15.999
 OIb_1306         OIb        1306.0286  4.78e-02  5.650e+08  15.999
 NiII_1317        NiII       1317.2170  5.96e-02  8.128e+08  57.935
 NiII_1370        NiII       1370.1320  6.16e-02  1.202e+09  57.935
 NiII_1393        NiII       1393.3240  1.25e-02  4.571e+08  57.935
 NiII_1454        NiII       1454.8420  2.20e-02  5.888e+08  57.935
 NiII_1467        NiII       1467.2590  4.00e-03  5.888e+08  57.935
```

### Comparing `VoigtFit-3.15/VoigtFit/static/telluric_em_abs.npz` & `VoigtFit-3.16/VoigtFit/static/telluric_em_abs.npz`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/utils/Asplund.py` & `VoigtFit-3.16/VoigtFit/utils/Asplund.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/utils/line_complexes.py` & `VoigtFit-3.16/VoigtFit/utils/line_complexes.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/utils/molecules.py` & `VoigtFit-3.16/VoigtFit/utils/molecules.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit/utils/terminal_attributes.py` & `VoigtFit-3.16/VoigtFit/utils/terminal_attributes.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.15/VoigtFit.egg-info/PKG-INFO` & `VoigtFit-3.16/VoigtFit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoigtFit
-Version: 3.15
+Version: 3.16
 Summary: Voigt Profile Fitting in Python
 Home-page: https://github.com/jkrogager/VoigtFit
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: voigtfit absorption analysis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VoigtFit-3.15/VoigtFit.egg-info/SOURCES.txt` & `VoigtFit-3.16/VoigtFit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 VoigtFit/io/hdf5_save.py
 VoigtFit/io/output.py
 VoigtFit/io/parse_input.py
 VoigtFit/static/Asplund2009.dat
 VoigtFit/static/Asplund2021.dat
 VoigtFit/static/C_complexes.dat
 VoigtFit/static/C_full_labels.txt
+VoigtFit/static/Konstantopoulou2022.dat
 VoigtFit/static/Lodders2009.dat
 VoigtFit/static/input_template.txt
 VoigtFit/static/linelist.dat
 VoigtFit/static/telluric_em_abs.npz
 VoigtFit/utils/Asplund.py
 VoigtFit/utils/__init__.py
+VoigtFit/utils/depletion.py
 VoigtFit/utils/line_complexes.py
 VoigtFit/utils/molecules.py
 VoigtFit/utils/terminal_attributes.py
```

### Comparing `VoigtFit-3.15/setup.py` & `VoigtFit-3.16/setup.py`

 * *Files identical despite different names*

