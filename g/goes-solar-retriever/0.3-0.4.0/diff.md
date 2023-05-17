# Comparing `tmp/goes_solar_retriever-0.3.tar.gz` & `tmp/goes_solar_retriever-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goes_solar_retriever-0.3.tar", last modified: Fri May 20 19:34:49 2022, max compression
+gzip compressed data, was "goes_solar_retriever-0.4.0.tar", last modified: Tue May 16 23:57:26 2023, max compression
```

## Comparing `goes_solar_retriever-0.3.tar` & `goes_solar_retriever-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2022-05-20 19:34:49.879241 goes_solar_retriever-0.3/
--rw-r--r--   0 jhughes  (1624782681) 1567826318      239 2022-05-20 19:34:49.878926 goes_solar_retriever-0.3/PKG-INFO
--rw-r--r--   0 jhughes  (1624782681) 1567826318     1749 2022-05-20 19:31:58.000000 goes_solar_retriever-0.3/README.md
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2022-05-20 19:34:49.876423 goes_solar_retriever-0.3/goes_solar_retriever.egg-info/
--rw-r--r--   0 jhughes  (1624782681) 1567826318      239 2022-05-20 19:34:49.000000 goes_solar_retriever-0.3/goes_solar_retriever.egg-info/PKG-INFO
--rw-r--r--   0 jhughes  (1624782681) 1567826318      324 2022-05-20 19:34:49.000000 goes_solar_retriever-0.3/goes_solar_retriever.egg-info/SOURCES.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318        1 2022-05-20 19:34:49.000000 goes_solar_retriever-0.3/goes_solar_retriever.egg-info/dependency_links.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       16 2022-05-20 19:34:49.000000 goes_solar_retriever-0.3/goes_solar_retriever.egg-info/requires.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       19 2022-05-20 19:34:49.000000 goes_solar_retriever-0.3/goes_solar_retriever.egg-info/top_level.txt
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2022-05-20 19:34:49.878260 goes_solar_retriever-0.3/goessolarretriever/
--rw-r--r--   0 jhughes  (1624782681) 1567826318      102 2022-05-20 19:28:06.000000 goes_solar_retriever-0.3/goessolarretriever/__init__.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318     5467 2022-05-20 19:28:06.000000 goes_solar_retriever-0.3/goessolarretriever/fetch.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318      739 2022-05-20 19:31:58.000000 goes_solar_retriever-0.3/goessolarretriever/kinds.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318       38 2022-05-20 19:34:49.879350 goes_solar_retriever-0.3/setup.cfg
--rw-r--r--   0 jhughes  (1624782681) 1567826318      327 2022-05-20 19:34:14.000000 goes_solar_retriever-0.3/setup.py
+drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-05-16 23:57:26.773253 goes_solar_retriever-0.4.0/
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      178 2023-05-16 23:57:26.772764 goes_solar_retriever-0.4.0/PKG-INFO
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     1749 2023-05-16 23:45:41.000000 goes_solar_retriever-0.4.0/README.md
+drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-05-16 23:57:26.766418 goes_solar_retriever-0.4.0/goes_solar_retriever.egg-info/
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      178 2023-05-16 23:57:26.000000 goes_solar_retriever-0.4.0/goes_solar_retriever.egg-info/PKG-INFO
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      324 2023-05-16 23:57:26.000000 goes_solar_retriever-0.4.0/goes_solar_retriever.egg-info/SOURCES.txt
+-rw-r--r--   0 jhughes  (1624782681) 1567826318        1 2023-05-16 23:57:26.000000 goes_solar_retriever-0.4.0/goes_solar_retriever.egg-info/dependency_links.txt
+-rw-r--r--   0 jhughes  (1624782681) 1567826318       16 2023-05-16 23:57:26.000000 goes_solar_retriever-0.4.0/goes_solar_retriever.egg-info/requires.txt
+-rw-r--r--   0 jhughes  (1624782681) 1567826318       19 2023-05-16 23:57:26.000000 goes_solar_retriever-0.4.0/goes_solar_retriever.egg-info/top_level.txt
+drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2023-05-16 23:57:26.771092 goes_solar_retriever-0.4.0/goessolarretriever/
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      102 2022-05-20 19:28:06.000000 goes_solar_retriever-0.4.0/goessolarretriever/__init__.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318     5505 2023-05-16 23:50:59.000000 goes_solar_retriever-0.4.0/goessolarretriever/fetch.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      759 2023-05-16 23:56:47.000000 goes_solar_retriever-0.4.0/goessolarretriever/kinds.py
+-rw-r--r--   0 jhughes  (1624782681) 1567826318       38 2023-05-16 23:57:26.773536 goes_solar_retriever-0.4.0/setup.cfg
+-rw-r--r--   0 jhughes  (1624782681) 1567826318      329 2023-05-16 23:56:47.000000 goes_solar_retriever-0.4.0/setup.py
```

### Comparing `goes_solar_retriever-0.3/README.md` & `goes_solar_retriever-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ## Satellites included:
 * GOES 16: `Satellite.GOES16`
 * GOES 17: `Satellite.GOES17`
 
 ## Products included:
 * 94 angstrom composite: `Product.suvi_l2_ci094`
-* 134 angstrom composite: `Product.suvi_l2_ci134`
+* 131 angstrom composite: `Product.suvi_l2_ci131`
 * 171 angstrom composite: `Product.suvi_l2_ci171`
 * 195 angstrom composite: `Product.suvi_l2_ci195`
 * 284 angstrom composite: `Product.suvi_l2_ci284`
 * 304 angstrom composite: `Product.suvi_l2_ci304`
 * 94 ansgstrom L1b: `Product.suvi_l1b_fe094`
 * 131 angstrom L1b: `Product.suvi_l1b_fe131`
 * 171 angstrom L1b: `Product.suvi_l1b_fe171`
```

### Comparing `goes_solar_retriever-0.3/goessolarretriever/fetch.py` & `goes_solar_retriever-0.4.0/goessolarretriever/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 class NameParser:
     suvi_ci = {Product.suvi_l2_ci094,
                Product.suvi_l2_ci131,
                Product.suvi_l2_ci171,
                Product.suvi_l2_ci195,
                Product.suvi_l2_ci284,
-               Product.suvi_l2_ci304}
+               Product.suvi_l2_ci304,
+               Product.suvi_l2_thmap}
 
     suvi_lib = {Product.suvi_l1b_fe094,
                 Product.suvi_l1b_fe131,
                 Product.suvi_l1b_fe171,
                 Product.suvi_l1b_fe195,
                 Product.suvi_l1b_fe284,
                 Product.suvi_l1b_he304}
```

### Comparing `goes_solar_retriever-0.3/goessolarretriever/kinds.py` & `goes_solar_retriever-0.4.0/goessolarretriever/kinds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum, unique, auto
 
 
 @unique
 class Satellite(Enum):
     GOES16 = auto()
     GOES17 = auto()
+    GOES18 = auto()
 
 
 @unique
 class Product(Enum):
     mag_l1b_geof = auto()
     seis_l1b_ehis = auto()
     seis_l1b_mpsh = auto()
```

