# Comparing `tmp/emilys-0.1.6.tar.gz` & `tmp/emilys-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emilys-0.1.6.tar", last modified: Fri Nov 18 14:10:10 2022, max compression
+gzip compressed data, was "emilys-0.1.7.tar", last modified: Wed May 17 13:44:41 2023, max compression
```

## Comparing `emilys-0.1.6.tar` & `emilys-0.1.7.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:10.000776 emilys-0.1.6/
--rw-rw-rw-   0        0        0      325 2022-11-18 14:10:09.999817 emilys-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2240 2022-11-18 14:05:18.000000 emilys-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.881093 emilys-0.1.6/emilys/
--rw-rw-rw-   0        0        0        0 2020-12-14 07:47:19.000000 emilys-0.1.6/emilys/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.889072 emilys-0.1.6/emilys/files/
--rw-rw-rw-   0        0        0        0 2022-11-18 12:44:43.000000 emilys-0.1.6/emilys/files/__init__.py
--rw-rw-rw-   0        0        0     5124 2022-11-18 12:44:43.000000 emilys-0.1.6/emilys/files/emd.py
--rw-rw-rw-   0        0        0     1810 2022-11-18 14:02:33.000000 emilys-0.1.6/emilys/files/txt.py
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.897085 emilys-0.1.6/emilys/functions/
--rw-rw-rw-   0        0        0        0 2020-12-14 07:47:19.000000 emilys-0.1.6/emilys/functions/__init__.py
--rw-rw-rw-   0        0        0     1015 2019-07-17 11:51:17.000000 emilys-0.1.6/emilys/functions/distributions.py
--rw-rw-rw-   0        0        0     3968 2019-07-13 10:44:24.000000 emilys-0.1.6/emilys/functions/peaks.py
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.932954 emilys-0.1.6/emilys/image/
--rw-rw-rw-   0        0        0        0 2020-12-14 07:47:19.000000 emilys-0.1.6/emilys/image/__init__.py
--rw-rw-rw-   0        0        0     4481 2022-11-18 12:44:43.000000 emilys-0.1.6/emilys/image/arrayplot.py
--rw-rw-rw-   0        0        0    17777 2022-11-18 14:02:33.000000 emilys-0.1.6/emilys/image/binning.py
--rw-rw-rw-   0        0        0     2626 2022-11-18 12:44:43.000000 emilys-0.1.6/emilys/image/dpc.py
--rw-rw-rw-   0        0        0     8522 2021-06-21 13:45:11.000000 emilys-0.1.6/emilys/image/geometry.py
--rw-rw-rw-   0        0        0    11233 2022-11-18 12:44:43.000000 emilys-0.1.6/emilys/image/imagedata.py
--rw-rw-rw-   0        0        0    18195 2021-06-01 08:43:35.000000 emilys-0.1.6/emilys/image/kernels.py
--rw-rw-rw-   0        0        0     2804 2020-09-19 09:19:14.000000 emilys-0.1.6/emilys/image/manipulations.py
--rw-rw-rw-   0        0        0     6392 2021-04-28 10:11:03.000000 emilys-0.1.6/emilys/image/peakfit.py
--rw-rw-rw-   0        0        0    22431 2022-11-18 14:02:33.000000 emilys-0.1.6/emilys/image/polar.py
--rw-rw-rw-   0        0        0     2515 2022-11-18 12:44:43.000000 emilys-0.1.6/emilys/image/powderdif.py
--rw-rw-rw-   0        0        0     3004 2021-01-04 15:36:03.000000 emilys-0.1.6/emilys/image/shift.py
--rw-rw-rw-   0        0        0     3658 2021-04-14 17:10:36.000000 emilys-0.1.6/emilys/image/thonrings.py
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.954921 emilys-0.1.6/emilys/numerics/
--rw-rw-rw-   0        0        0        0 2020-12-14 07:47:19.000000 emilys-0.1.6/emilys/numerics/__init__.py
--rw-rw-rw-   0        0        0     7729 2019-07-08 06:57:13.000000 emilys-0.1.6/emilys/numerics/cluster.py
--rw-rw-rw-   0        0        0     1029 2021-01-11 09:47:59.000000 emilys-0.1.6/emilys/numerics/correlation.py
--rw-rw-rw-   0        0        0     4370 2021-04-14 15:25:51.000000 emilys-0.1.6/emilys/numerics/linsearch.py
--rw-rw-rw-   0        0        0     6338 2019-07-08 10:05:44.000000 emilys-0.1.6/emilys/numerics/lstsq.py
--rw-rw-rw-   0        0        0     2123 2019-07-04 07:41:48.000000 emilys-0.1.6/emilys/numerics/mc.py
--rw-rw-rw-   0        0        0     2669 2020-12-18 16:22:57.000000 emilys-0.1.6/emilys/numerics/roots.py
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.982845 emilys-0.1.6/emilys/optics/
--rw-rw-rw-   0        0        0        0 2020-12-14 07:47:19.000000 emilys-0.1.6/emilys/optics/__init__.py
--rw-rw-rw-   0        0        0    14709 2021-03-23 12:53:15.000000 emilys-0.1.6/emilys/optics/aberration.py
--rw-rw-rw-   0        0        0    10888 2020-10-01 13:15:10.000000 emilys-0.1.6/emilys/optics/aperture.py
--rw-rw-rw-   0        0        0     3454 2020-12-15 12:57:46.000000 emilys-0.1.6/emilys/optics/crystal.py
--rw-rw-rw-   0        0        0     6237 2022-11-18 12:44:43.000000 emilys-0.1.6/emilys/optics/econst.py
--rw-rw-rw-   0        0        0     9050 2021-04-14 14:16:13.000000 emilys-0.1.6/emilys/optics/focusspread.py
--rw-rw-rw-   0        0        0     6904 2021-03-17 13:33:03.000000 emilys-0.1.6/emilys/optics/mtf.py
--rw-rw-rw-   0        0        0    35060 2021-06-24 06:30:25.000000 emilys-0.1.6/emilys/optics/projection.py
--rw-rw-rw-   0        0        0    19415 2022-01-03 14:19:12.000000 emilys-0.1.6/emilys/optics/waki.py
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.998779 emilys-0.1.6/emilys/structure/
--rw-rw-rw-   0        0        0        0 2021-04-30 07:40:07.000000 emilys-0.1.6/emilys/structure/__init__.py
--rw-rw-rw-   0        0        0     3230 2022-08-05 13:05:27.000000 emilys-0.1.6/emilys/structure/atom.py
--rw-rw-rw-   0        0        0     1520 2022-11-18 14:02:33.000000 emilys-0.1.6/emilys/structure/atomtype.py
--rw-rw-rw-   0        0        0     6576 2022-06-08 13:28:50.000000 emilys-0.1.6/emilys/structure/celio.py
--rw-rw-rw-   0        0        0    24458 2022-11-18 14:02:33.000000 emilys-0.1.6/emilys/structure/cifio.py
--rw-rw-rw-   0        0        0    41170 2022-08-05 13:05:27.000000 emilys-0.1.6/emilys/structure/supercell.py
--rw-rw-rw-   0        0        0    12541 2022-08-05 13:05:27.000000 emilys-0.1.6/emilys/structure/xtlio.py
-drwxrwxrwx   0        0        0        0 2022-11-18 14:10:09.886081 emilys-0.1.6/emilys.egg-info/
--rw-rw-rw-   0        0        0      325 2022-11-18 14:10:09.000000 emilys-0.1.6/emilys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1267 2022-11-18 14:10:09.000000 emilys-0.1.6/emilys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-18 14:10:09.000000 emilys-0.1.6/emilys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2022-11-18 14:10:09.000000 emilys-0.1.6/emilys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-18 14:10:09.000000 emilys-0.1.6/emilys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-18 14:10:10.000776 emilys-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      502 2022-11-18 14:08:31.000000 emilys-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.324929 emilys-0.1.7/
+-rw-rw-rw-   0        0        0    35823 2019-06-29 07:30:05.000000 emilys-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      339 2023-05-17 13:44:41.320739 emilys-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2023-05-17 13:29:52.000000 emilys-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.038257 emilys-0.1.7/emilys/
+-rw-rw-rw-   0        0        0        0 2020-12-14 07:47:19.000000 emilys-0.1.7/emilys/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.077796 emilys-0.1.7/emilys/files/
+-rw-rw-rw-   0        0        0        0 2022-09-14 10:18:08.000000 emilys-0.1.7/emilys/files/__init__.py
+-rw-rw-rw-   0        0        0     5124 2022-09-28 11:40:42.000000 emilys-0.1.7/emilys/files/emd.py
+-rw-rw-rw-   0        0        0     1705 2022-12-20 13:39:52.000000 emilys-0.1.7/emilys/files/mtf.py
+-rw-rw-rw-   0        0        0     1810 2022-11-18 14:00:09.000000 emilys-0.1.7/emilys/files/txt.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.091890 emilys-0.1.7/emilys/functions/
+-rw-rw-rw-   0        0        0        0 2020-12-17 14:44:57.000000 emilys-0.1.7/emilys/functions/__init__.py
+-rw-rw-rw-   0        0        0     1015 2019-07-17 11:51:17.000000 emilys-0.1.7/emilys/functions/distributions.py
+-rw-rw-rw-   0        0        0     3968 2019-07-13 10:44:24.000000 emilys-0.1.7/emilys/functions/peaks.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.170471 emilys-0.1.7/emilys/image/
+-rw-rw-rw-   0        0        0        0 2020-12-17 14:44:57.000000 emilys-0.1.7/emilys/image/__init__.py
+-rw-rw-rw-   0        0        0     4481 2022-10-28 14:08:45.000000 emilys-0.1.7/emilys/image/arrayplot.py
+-rw-rw-rw-   0        0        0    17777 2022-08-24 14:05:08.000000 emilys-0.1.7/emilys/image/binning.py
+-rw-rw-rw-   0        0        0     2626 2022-11-08 14:49:01.000000 emilys-0.1.7/emilys/image/dpc.py
+-rw-rw-rw-   0        0        0     8522 2021-07-26 13:11:28.000000 emilys-0.1.7/emilys/image/geometry.py
+-rw-rw-rw-   0        0        0    11233 2022-09-23 08:57:55.000000 emilys-0.1.7/emilys/image/imagedata.py
+-rw-rw-rw-   0        0        0    18195 2021-06-14 09:51:22.000000 emilys-0.1.7/emilys/image/kernels.py
+-rw-rw-rw-   0        0        0     2804 2020-09-19 09:19:14.000000 emilys-0.1.7/emilys/image/manipulations.py
+-rw-rw-rw-   0        0        0     6392 2022-08-19 14:15:30.000000 emilys-0.1.7/emilys/image/peakfit.py
+-rw-rw-rw-   0        0        0    22431 2022-11-18 13:08:21.000000 emilys-0.1.7/emilys/image/polar.py
+-rw-rw-rw-   0        0        0     2515 2022-09-28 11:07:48.000000 emilys-0.1.7/emilys/image/powderdif.py
+-rw-rw-rw-   0        0        0     3004 2021-02-04 09:28:09.000000 emilys-0.1.7/emilys/image/shift.py
+-rw-rw-rw-   0        0        0     3658 2021-05-17 06:52:48.000000 emilys-0.1.7/emilys/image/thonrings.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.210147 emilys-0.1.7/emilys/numerics/
+-rw-rw-rw-   0        0        0        0 2020-12-17 14:44:57.000000 emilys-0.1.7/emilys/numerics/__init__.py
+-rw-rw-rw-   0        0        0     7729 2019-07-08 06:57:13.000000 emilys-0.1.7/emilys/numerics/cluster.py
+-rw-rw-rw-   0        0        0     1029 2021-02-04 09:28:09.000000 emilys-0.1.7/emilys/numerics/correlation.py
+-rw-rw-rw-   0        0        0     4370 2021-05-17 06:52:48.000000 emilys-0.1.7/emilys/numerics/linsearch.py
+-rw-rw-rw-   0        0        0     6338 2019-07-08 10:05:44.000000 emilys-0.1.7/emilys/numerics/lstsq.py
+-rw-rw-rw-   0        0        0     2123 2019-07-04 07:41:48.000000 emilys-0.1.7/emilys/numerics/mc.py
+-rw-rw-rw-   0        0        0     2669 2020-12-22 13:59:42.000000 emilys-0.1.7/emilys/numerics/roots.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.271347 emilys-0.1.7/emilys/optics/
+-rw-rw-rw-   0        0        0        0 2020-12-17 14:44:57.000000 emilys-0.1.7/emilys/optics/__init__.py
+-rw-rw-rw-   0        0        0    14709 2021-04-12 15:47:54.000000 emilys-0.1.7/emilys/optics/aberration.py
+-rw-rw-rw-   0        0        0    10888 2020-09-28 14:58:03.000000 emilys-0.1.7/emilys/optics/aperture.py
+-rw-rw-rw-   0        0        0     3454 2021-04-22 08:38:01.000000 emilys-0.1.7/emilys/optics/crystal.py
+-rw-rw-rw-   0        0        0     6293 2023-02-01 15:37:27.000000 emilys-0.1.7/emilys/optics/econst.py
+-rw-rw-rw-   0        0        0     9050 2021-05-17 06:52:48.000000 emilys-0.1.7/emilys/optics/focusspread.py
+-rw-rw-rw-   0        0        0     6904 2021-03-12 15:09:30.000000 emilys-0.1.7/emilys/optics/mtf.py
+-rw-rw-rw-   0        0        0    35060 2021-07-26 13:11:28.000000 emilys-0.1.7/emilys/optics/projection.py
+-rw-rw-rw-   0        0        0     3415 2023-05-17 12:57:29.000000 emilys-0.1.7/emilys/optics/tp1dho.py
+-rw-rw-rw-   0        0        0    19415 2022-01-04 10:30:10.000000 emilys-0.1.7/emilys/optics/waki.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.314564 emilys-0.1.7/emilys/structure/
+-rw-rw-rw-   0        0        0        0 2021-05-17 06:52:48.000000 emilys-0.1.7/emilys/structure/__init__.py
+-rw-rw-rw-   0        0        0     3229 2023-01-30 14:22:24.000000 emilys-0.1.7/emilys/structure/atom.py
+-rw-rw-rw-   0        0        0     1520 2022-06-28 15:03:39.000000 emilys-0.1.7/emilys/structure/atomtype.py
+-rw-rw-rw-   0        0        0     6576 2022-06-20 09:32:25.000000 emilys-0.1.7/emilys/structure/celio.py
+-rw-rw-rw-   0        0        0    43632 2023-02-01 14:28:25.000000 emilys-0.1.7/emilys/structure/cifio.py
+-rw-rw-rw-   0        0        0    50777 2023-02-01 14:21:53.000000 emilys-0.1.7/emilys/structure/supercell.py
+-rw-rw-rw-   0        0        0    12541 2022-06-20 10:44:06.000000 emilys-0.1.7/emilys/structure/xtlio.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:44:41.060131 emilys-0.1.7/emilys.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-17 13:44:40.000000 emilys-0.1.7/emilys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1319 2023-05-17 13:44:40.000000 emilys-0.1.7/emilys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:44:40.000000 emilys-0.1.7/emilys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-17 13:44:40.000000 emilys-0.1.7/emilys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 13:44:40.000000 emilys-0.1.7/emilys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 13:44:41.324929 emilys-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      588 2023-05-17 13:43:52.000000 emilys-0.1.7/setup.py
```

### Comparing `emilys-0.1.6/README.md` & `emilys-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # emilys
 
 Electron Microscopy Image anaLYSis tools
 
-Version: 0.1.6
+Version: 0.1.7
 
 ## Authors and Copyright
 
 Juri Barthel, 
 Forschungszentrum Jülich GmbH, 52425 Jülich, Germany
 
-Copyright (c) 2019 - 2022 - Forschungszentrum Jülich GmbH
+Copyright (c) 2019 - 2023 - Forschungszentrum Jülich GmbH
    
 Published under the GNU General Public License, version 3,
 see <http://www.gnu.org/licenses/> and LICENSE!
 
 ## Installation
 
 If you want to play in the code, copy this source tree to some place, where your Python environment is able to find it.
 
 If you just want to use it, install via 
 
     pip install emilys
 
 ## Changes
 
+* Version 0.1.7:
+Added 1-dimensional harmonic oscillator functions and transitions.
 * Version 0.1.6:
 Modified a lot of functions. There are some functions in the structure section
 which are incomplete and under development. Use them with care.
 * Version 0.1.5:
 Added debug to emilys.image.peakfit.fit_local_gauss_2d. 
 Added sub-package structure for handling atomic structure models used in TEM simulations.
 Changed some kernel functions to regain compatibility with numba.
```

### Comparing `emilys-0.1.6/emilys/files/emd.py` & `emilys-0.1.7/emilys/files/emd.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/files/txt.py` & `emilys-0.1.7/emilys/files/txt.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/functions/distributions.py` & `emilys-0.1.7/emilys/functions/distributions.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/functions/peaks.py` & `emilys-0.1.7/emilys/functions/peaks.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/arrayplot.py` & `emilys-0.1.7/emilys/image/arrayplot.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/binning.py` & `emilys-0.1.7/emilys/image/binning.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/dpc.py` & `emilys-0.1.7/emilys/image/dpc.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/geometry.py` & `emilys-0.1.7/emilys/image/geometry.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/imagedata.py` & `emilys-0.1.7/emilys/image/imagedata.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/kernels.py` & `emilys-0.1.7/emilys/image/kernels.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/manipulations.py` & `emilys-0.1.7/emilys/image/manipulations.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/peakfit.py` & `emilys-0.1.7/emilys/image/peakfit.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/polar.py` & `emilys-0.1.7/emilys/image/polar.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/powderdif.py` & `emilys-0.1.7/emilys/image/powderdif.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/shift.py` & `emilys-0.1.7/emilys/image/shift.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/image/thonrings.py` & `emilys-0.1.7/emilys/image/thonrings.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/numerics/cluster.py` & `emilys-0.1.7/emilys/numerics/cluster.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/numerics/correlation.py` & `emilys-0.1.7/emilys/numerics/correlation.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/numerics/linsearch.py` & `emilys-0.1.7/emilys/numerics/linsearch.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/numerics/lstsq.py` & `emilys-0.1.7/emilys/numerics/lstsq.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/numerics/mc.py` & `emilys-0.1.7/emilys/numerics/mc.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/numerics/roots.py` & `emilys-0.1.7/emilys/numerics/roots.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/optics/aberration.py` & `emilys-0.1.7/emilys/optics/aberration.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/optics/aperture.py` & `emilys-0.1.7/emilys/optics/aperture.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/optics/crystal.py` & `emilys-0.1.7/emilys/optics/crystal.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/optics/econst.py` & `emilys-0.1.7/emilys/optics/econst.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 PHYS_HPL = 6.62607015E-34 # Planck's constant [ J s ]
 PHYS_QEL = 1.602176634E-19 # elementary charge [ C ]
 
 PHYS_HPLEV = 4.135667697E-15 # Planck's constant [ eV s ]
 PHYS_HBAR = 1.054571818E-34 # reduced Planck's constant [ J s ]
 PHYS_HBAREV = 6.582119570E-16 # reduced Planck's constant [ eV s ]
 PHYS_MASSU = 1.66053906660E-27 # atomic mass constant [kg]
+PHYS_KB = 1.380649E-23 # Boltzmann constant [J K^(-1)]
 
 # Derived constants
 
 EL_M0 = 9.1093837015E-31 # electron rest mass, error (28) in last digits [ kg ]
 EL_E0 = EL_M0 * PHYS_C**2 # electron rest energy [ J ]
 EL_E0EV = EL_E0 / PHYS_QEL # electron rest energy [ eV ]
 EL_E0KEV = EL_E0 / PHYS_QEL / 1000. # electron rest energy [ keV ]
```

### Comparing `emilys-0.1.6/emilys/optics/focusspread.py` & `emilys-0.1.7/emilys/optics/focusspread.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/optics/mtf.py` & `emilys-0.1.7/emilys/optics/mtf.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/optics/projection.py` & `emilys-0.1.7/emilys/optics/projection.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/optics/waki.py` & `emilys-0.1.7/emilys/optics/waki.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/structure/atom.py` & `emilys-0.1.7/emilys/structure/atom.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         pos : numpy.ndarray([x, y, z], dtype=float)
             fractional coordinates in a supercell
 
     Methods
     -------
 
         get_type_name(l_type_name_adds)
-            Returns a string for an atom type name with possible addistions
+            Returns a string for an atom type name with possible additions
             depending on other atom parameters.
 
     """
 
     def __init__(self, Z=1, pos=np.array([0.,0.,0.]), uiso=0.006332574, occ=1., charge=0.):
         self.Z = Z
         self.pos = pos
```

### Comparing `emilys-0.1.6/emilys/structure/atomtype.py` & `emilys-0.1.7/emilys/structure/atomtype.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/structure/celio.py` & `emilys-0.1.7/emilys/structure/celio.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys/structure/supercell.py` & `emilys-0.1.7/emilys/structure/supercell.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 This code is part of the 'emilys' repository
 https://github.com/ju-bar/emilys
 published under the GNU General Publishing License, version 3
 
 """
 
-import os, sys
 import numpy as np
 import emilys.structure.atomtype as aty
 from emilys.structure.atom import atom, get_str_from_charge
 from copy import deepcopy
 
 class supercell:
     """
@@ -109,27 +108,38 @@
             to be parallel to planes or lines.
 
         list_positions(l_atoms_idx):
             Returns a list of positions of atoms identified by index.
 
         list_close_atoms(l_atoms_idx, proximity, periodic):
             Returns a list of lists of atoms, which are closer than the
-            proximity parameter in nanometers. The periodic option switches
+            proximity parameter in Angstroms. The periodic option switches
             the check of proximity under periodic boundary conditions.
 
+        list_close_atoms_ref(pos, l_atoms_idx, proximity, periodic):
+            Returns a list indices in l_atoms, for atoms which are closer
+            to pos_ref than the proximity parameter in Angstroms.
+            The periodic option switches the check of proximity under
+            periodic boundary conditions.
+
         remove_close_atoms(l_atoms_idx, proximity):
             Returns a list of atom indices to be removed from l_atoms_idx.
-            The removel is not performed, so that l_atoms_idx remains 
+            The remove is not performed, so that l_atoms_idx remains 
             unchanged by this routine.
 
         list_atoms_in_range(dic_range):
             Returns a list of atoms which parameters fall into all range
             specifications listed in the dictionary dic_range. See the
             function definition on how to setup the dictionary.
 
+        dice_occupancy(l_atoms_idx, proximity, periodic):
+            Randomly selects, which site realizes full occupancy from sites
+            in list l_atoms_idx and replaces partial site occupation by
+            full atom occupations.
+
     """
 
     def __init__(self):
         self.a0 = np.array([1., 1., 1.]) # lattice constants [x, y, z]
         self.angles = np.array([90., 90., 90.]) # cell angles [alpha, beta, gamma] between [yz, zx, xy]
         self.basis = np.array([[1.,0.,0.],[0.,1.,0.],[0.,0.,1.]]) # list of basis vectors x, y, z
         self.l_atoms = [] # list of atoms
@@ -814,20 +824,20 @@
 
             l_atoms_idx : list
                 List of indices identifying atoms in member l_atoms
                 to be checked for mutual proximity. Atoms not included
                 in the list will be ignored in the proximity checks.
 
             proximity : float
-                Sets a threshold to which distance in nanometers is
+                Sets a threshold to which distance in Angstroms is
                 identified as close.
 
             periodic : boolean, default: True
                 Switches proximity checks under periodic boundary
-                condistions.
+                conditions.
 
             debug : boolean, default: False
                 Switches extra debug text output.
 
         Returns
         -------
 
@@ -863,32 +873,117 @@
                         l_close_cur.append(jdx) # add to current list
                 # handle the current list of atoms close to atim idx
                 if len(l_close_cur) > 1: # at least a pair?
                     l_close.append(l_close_cur) # append to output list
                     if debug: print('added list', l_close_cur)
         return l_close
 
+    def check_duplicate_atom(self, ato, proximity=1.E-3, periodic=True):
+        n = len(self.l_atoms)
+        mb0 = self.get_basis().T # get the transformation matrix to transform from fractional to physical coordinates
+        sdthr = proximity * proximity
+        if n > 0:
+            for idx in range(0, n):
+                ichk = 0 # reset checker
+                # distance check
+                vlp = self.l_atoms[idx].pos
+                if periodic: # fractional distance vector across periodic boundary conditions
+                    vdlp = ((vlp - ato.pos + 0.5) % 1.0 ) - 0.5
+                else: # fractional distance vector, no periodic boundary
+                    vdlp = vlp - ato.pos
+                vdp = np.dot(mb0, vdlp) # distance vector in physical coordinates [A]
+                sd = np.dot(vdp, vdp)
+                if sd <= sdthr: # squared distance check [A**2]
+                    ichk += 1
+                # type check
+                if ato.Z == self.l_atoms[idx].Z:
+                    ichk += 2
+                # are there other checks to do?
+                # final result
+                if ichk == 3: # duplicate found
+                    return True
+        return False
+
+    def list_close_atoms_ref(self, pos, l_atoms_idx, proximity, periodic=True, debug=False):
+        """
+
+        Returns a list of lists of atoms, which are closer than the
+        proximity parameter in nanometers. The periodic option switches
+        the check of proximity under periodic boundary conditions.
+
+        Parameters
+        ----------
+
+            pos : numpy ndarray((3),float)
+                Reference position in fractional cell coordinates. 
+
+            l_atoms_idx : list
+                List of indices identifying atoms in member l_atoms
+                to be checked for mutual proximity. Atoms not included
+                in the list will be ignored in the proximity checks.
+
+            proximity : float
+                Sets a threshold to which distance in Angstroms is
+                identified as close.
+
+            periodic : boolean, default: True
+                Switches proximity checks under periodic boundary
+                conditions.
+
+            debug : boolean, default: False
+                Switches extra debug text output.
+
+        Returns
+        -------
+
+            list
+                List of atom indices for atoms closer to pos than
+                proximity
+        
+        """
+        l_close = []
+        assert isinstance(l_atoms_idx, list), 'Input <l_atoms_idx> should be a list of numbers.'
+        n = len(l_atoms_idx) # list of atom indices to check for proximity
+        mb0 = self.get_basis().T # get the transformation matrix to transform from fractional to physical coordinates
+        sdthr = proximity * proximity
+        if n > 0: # need at least one atom to check
+            for i in range(0, n): # loop over atoms in list
+                idx = l_atoms_idx[i]
+                vlp = self.l_atoms[idx].pos
+                if periodic: # fractional distance vector across periodic boundary conditions
+                    vdlp = ((vlp - pos + 0.5) % 1.0 ) - 0.5
+                else: # fractional distance vector, no periodic boundary
+                    vdlp = vlp - pos
+                vdp = np.dot(mb0, vdlp) # distance vector in physical coordinates [A]
+                sd = np.dot(vdp, vdp)
+                if sd <= sdthr: # squared distance check [nm**2]
+                    if debug:
+                        print('- #{:d} {:s}: d = {:.4f} nm'.format(
+                            idx, aty.atom_type_symbol[self.l_atoms[idx].Z],np.sqrt(sd)))
+                    l_close.append(idx) # add to list
+        return l_close
+
     def remove_close_atoms(self, l_atoms_idx, proximity, debug=False):
         """
 
-        Returns a list of atom indices to be removed from l_atoms_idx. The removel is
+        Returns a list of atom indices to be removed from l_atoms_idx. The remove is
         not performed, so that l_atoms_idx remains unchanged by this routine.
         The list is parsed in sequence, checking proximity between atom i and atom i + x.
         Double checking should not occur in this implementation.
 
         Parameters
         ----------
 
             l_atoms_idx : list
                 List of indices identifying atoms in member l_atoms
                 to be checked for mutual proximity. Atoms not included
                 in the list will be ignored in the proximity checks.
 
             proximity : float
-                Sets a threshold to which distance in nanometers is
+                Sets a threshold to which distance in Angstroms is
                 identified as close.
 
             debug : boolean, default: False
                 Switches extra debug text output.
 
         Returns
         -------
@@ -944,23 +1039,27 @@
         Parameters
         ----------
 
             dic_range : dict, default {}
                 dictionary of range definitions
                 supported range keys are
                 'rng_Z' : [int, int]
-                    atomic numbers
+                    range of atomic numbers
+                'lst_Z' : list of int
+                    list of atomic numbers
                 'rng_charge' : [float, float]
                     ionic charges
                 'rng_pos_a' : [float, float]
                     fractional atom position along cell a axis
                 'rng_pos_b' : [float, float]
                     fractional atom position along cell b axis
                 'rng_pos_c' : [float, float]
                     fractional atom position along cell c axis
+                'rng_pos_r' : [[float, float, float], float]
+                    fractional atom 3d position, radius in Angs
                 'rng_uiso' : [float, float]
                     thermal vibration amplitudes
                 'rng_occ' : [float, float]
                     occupancy factors
 
         Returns
         -------
@@ -973,31 +1072,131 @@
             Ranges defined will be checked inclusive of the lower
             bound and exclusive for the upper bound,
             i.e. (x0 <= x) and (x < x1).
 
         """
         l_atoms_idx = [] # initialize empty list of selected atom indices
         n_atoms = len(self.l_atoms) # get number of atoms in the structure
+        mb0 = self.get_basis().T # get the transformation matrix to transform from fractional to physical coordinates
+        sdthr = 0.
+        pos_ref = np.array([0., 0., 0.])
+        if 'rng_pos_r' in dic_range:
+            pos_ref = np.dot(mb0, dic_range['rng_pos_r'][0]) # reference position [A]
+            proximity = dic_range['rng_pos_r'][1] # distance in [A]
+            sdthr = proximity * proximity
         if n_atoms > 0:
             for i in range(0, n_atoms): # loop over all atoms
                 ati = self.l_atoms[i]
                 b_add = True # assume adding and perform logical AND operations to turn it off in case of failing conditions
                 for sel_key in dic_range: # go through all conditions
                     min_val = min(dic_range[sel_key])
                     max_val = max(dic_range[sel_key])  
                     if sel_key == 'rng_Z': # atomic number range condition
                         b_add &= ((ati.Z >= min_val) and (ati.Z < max_val))
+                    if sel_key == 'lst_Z': # atomic number list condition
+                        b_add &= (ati.Z in dic_range[sel_key])
                     if sel_key == 'rng_charge': # charge range
                         b_add &= ((ati.charge >= min_val) and (ati.charge < max_val))
                     if sel_key == 'rng_uiso': # uiso range
                         b_add &= ((ati.uiso >= min_val) and (ati.uiso < max_val))
                     if sel_key == 'rng_occ': # occupancy range
                         b_add &= ((ati.occ >= min_val) and (ati.occ < max_val))
                     if sel_key == 'rng_pos_a': # position x range
                         b_add &= ((ati.pos[0] >= min_val) and (ati.pos[0] < max_val))
                     if sel_key == 'rng_pos_b': # position y range
                         b_add &= ((ati.pos[1] >= min_val) and (ati.pos[1] < max_val))
                     if sel_key == 'rng_pos_c': # position z range
                         b_add &= ((ati.pos[2] >= min_val) and (ati.pos[2] < max_val))
-                if b_add: # all conditions fullfilled ...
+                    if sel_key == 'rng_pos_r': # distance in A
+                        dpos = np.dot(mb0, ati.pos) - pos_ref
+                        sd = np.dot(dpos, dpos) # square distance [A^2]
+                        b_add &= (sd <= sdthr)
+                if b_add: # all conditions fulfilled ...
                     l_atoms_idx.append(i) # add atom index to list
-        return l_atoms_idx
+        return l_atoms_idx
+
+    def dice_occupancy(self, l_atoms_idx, proximity=0.01, periodic=True, debug=False):
+        """
+
+        Randomly selects, which site realizes full occupancy from sites
+        in list l_atoms_idx and replaces partial site occupation by
+        full atom occupations. This function modifies the list of atoms.
+        This means, the input list of indices becomes invalid afterwards.
+
+        Parameters
+        ----------
+
+            l_atoms_idx : list
+                List of indices identifying atoms in member l_atoms
+                to be checked for mutual proximity and occupancy selection.
+                Atoms not included in the list will be ignored in the proximity
+                checks.
+
+            proximity : float, default: 0.01
+                Sets a threshold to which distance in Angstroms is
+                identified as close.
+
+            periodic : boolean, default: True
+                Switches proximity checks under periodic boundary
+                conditions.
+
+            debug : boolean, default: False
+                Switches extra debug text output.
+
+        Returns
+        -------
+
+            None
+        
+        """
+        l_del = [] # list of atom indices to delete from the cell
+        l_atoms_occ = [] # list of atom data to insert to l_atoms
+        assert isinstance(l_atoms_idx, list), 'Input <l_atoms_idx> should be a list of numbers.'
+        l_work = deepcopy(l_atoms_idx) # working list, this will get smaller as we go
+        while len(l_work) > 0:
+            idx = l_work[0] # get the index of the atom in l_atoms
+            if self.l_atoms[idx].occ >= 1.0: # no dicing for atoms at full occupancy
+                del l_work[0]
+                continue
+            pos_ref = self.l_atoms[idx].pos
+            l_close = self.list_close_atoms_ref(pos_ref, l_work, proximity, periodic, debug)
+            if len(l_close)==0: # remove this bad case, not handled
+                del l_work[0]
+                continue
+            if debug:
+                print('- working on group of {:d} sites at position'.format(len(l_close)), pos_ref)
+            # setup occupancy thresholds
+            l_occ_thr = []
+            l_occ_total = 0.0
+            for jdx in l_close:
+                l_occ_total += self.l_atoms[jdx].occ
+                if debug:
+                    print('- #{:d}: occ={:.3f} -> total={:.3f}'.format(jdx, self.l_atoms[jdx].occ,l_occ_total))
+                l_occ_thr.append(l_occ_total)
+            if l_occ_total > 1.0:
+                print('Warning (dice_occupancy): total occupancy >1 ({:.3f}) in proximity {:.3f} A of atom #{:d}.'.format(l_occ_total, proximity, idx))
+            vrnd = np.random.rand() # random number [0,1)
+            kdx = -1 # default occupation selector is None
+            for j in range(0, len(l_occ_thr)): # find the occupation threshold which is bigger than vrnd
+                if vrnd < l_occ_thr[j]:
+                    kdx = l_close[j] # found site to fully occupy
+                    break # stop looking further
+            if kdx >= 0: # found something to occupy
+                at_keep = deepcopy(self.l_atoms[kdx]) # this is the atom to keep
+                at_keep.occ = 1.0 # fully occupy
+                l_atoms_occ.append(at_keep) # store in list
+                if debug:
+                    print('- group of {:d} sites at position'.format(len(l_close)), 
+                        pos_ref, 'occupied by ' + aty.atom_type_symbol[at_keep.Z] + 
+                        ' at position', at_keep.pos)
+            else:
+                if debug:
+                    print('- group of {:d} sites at position'.format(len(l_close)), 
+                        pos_ref, 'not occupied.')
+            l_del = l_del + l_close # add the current close group of sites to those to be deleted
+            for jdx in l_close: # remove close group of sites from work list
+                l_work.remove(jdx)
+        if len(l_del) > 0: # atoms to delete from the cell
+            self.delete_atoms(l_del) # deletion
+        if len(l_atoms_occ) > 0: # append fully occupied atoms
+            self.l_atoms = self.l_atoms + l_atoms_occ
+        return
```

### Comparing `emilys-0.1.6/emilys/structure/xtlio.py` & `emilys-0.1.7/emilys/structure/xtlio.py`

 * *Files identical despite different names*

### Comparing `emilys-0.1.6/emilys.egg-info/SOURCES.txt` & `emilys-0.1.7/emilys.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+LICENSE
 README.md
 setup.py
 emilys/__init__.py
 emilys.egg-info/PKG-INFO
 emilys.egg-info/SOURCES.txt
 emilys.egg-info/dependency_links.txt
 emilys.egg-info/requires.txt
 emilys.egg-info/top_level.txt
 emilys/files/__init__.py
 emilys/files/emd.py
+emilys/files/mtf.py
 emilys/files/txt.py
 emilys/functions/__init__.py
 emilys/functions/distributions.py
 emilys/functions/peaks.py
 emilys/image/__init__.py
 emilys/image/arrayplot.py
 emilys/image/binning.py
@@ -36,14 +38,15 @@
 emilys/optics/aberration.py
 emilys/optics/aperture.py
 emilys/optics/crystal.py
 emilys/optics/econst.py
 emilys/optics/focusspread.py
 emilys/optics/mtf.py
 emilys/optics/projection.py
+emilys/optics/tp1dho.py
 emilys/optics/waki.py
 emilys/structure/__init__.py
 emilys/structure/atom.py
 emilys/structure/atomtype.py
 emilys/structure/celio.py
 emilys/structure/cifio.py
 emilys/structure/supercell.py
```

