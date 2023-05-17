# Comparing `tmp/highyield-1.0.8.tar.gz` & `tmp/highyield-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highyield-1.0.8.tar", last modified: Wed Jan 18 22:32:06 2023, max compression
+gzip compressed data, was "highyield-1.0.9.tar", last modified: Wed May 17 01:26:49 2023, max compression
```

## Comparing `highyield-1.0.8.tar` & `highyield-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-01-18 22:32:06.084376 highyield-1.0.8/
--rw-r--r--   0 v1         (502) wheel        (0)    35129 2023-01-06 21:21:15.000000 highyield-1.0.8/LICENSE
--rw-r--r--   0 v1         (502) wheel        (0)       29 2023-01-06 21:17:34.000000 highyield-1.0.8/MANIFEST.in
--rw-r--r--   0 v1         (502) wheel        (0)     1597 2023-01-18 22:32:06.084206 highyield-1.0.8/PKG-INFO
--rw-r--r--   0 v1         (502) wheel        (0)     1085 2023-01-15 13:23:03.000000 highyield-1.0.8/README.md
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-01-18 22:32:06.082605 highyield-1.0.8/highyield/
--rw-r--r--   0 v1         (502) wheel        (0)      198 2023-01-06 23:04:04.000000 highyield-1.0.8/highyield/__init__.py
--rw-r--r--   0 v1         (502) wheel        (0)     3075 2023-01-02 19:44:42.000000 highyield-1.0.8/highyield/converter.py
--rw-r--r--   0 v1         (502) wheel        (0)     4265 2023-01-04 22:06:46.000000 highyield-1.0.8/highyield/copy.py
--rw-r--r--   0 v1         (502) wheel        (0)     1691 2023-01-18 22:18:24.000000 highyield-1.0.8/highyield/create.py
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-01-18 22:32:06.083789 highyield-1.0.8/highyield/data/
--rw-r--r--   0 v1         (502) wheel        (0)     1906 2023-01-03 23:05:21.000000 highyield-1.0.8/highyield/data/RR.csv
--rw-r--r--   0 v1         (502) wheel        (0)      346 2023-01-07 14:41:36.000000 highyield-1.0.8/highyield/imports.py
--rw-r--r--   0 v1         (502) wheel        (0)     1534 2023-01-06 18:44:52.000000 highyield-1.0.8/highyield/pdf.py
--rw-r--r--   0 v1         (502) wheel        (0)     1330 2023-01-15 13:10:42.000000 highyield-1.0.8/highyield/rename.py
--rw-r--r--   0 v1         (502) wheel        (0)     4878 2023-01-07 14:45:09.000000 highyield-1.0.8/highyield/tts.py
-drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-01-18 22:32:06.083676 highyield-1.0.8/highyield.egg-info/
--rw-r--r--   0 v1         (502) wheel        (0)     1597 2023-01-18 22:32:06.000000 highyield-1.0.8/highyield.egg-info/PKG-INFO
--rw-r--r--   0 v1         (502) wheel        (0)      429 2023-01-18 22:32:06.000000 highyield-1.0.8/highyield.egg-info/SOURCES.txt
--rw-r--r--   0 v1         (502) wheel        (0)        1 2023-01-18 22:32:06.000000 highyield-1.0.8/highyield.egg-info/dependency_links.txt
--rw-r--r--   0 v1         (502) wheel        (0)        1 2023-01-06 23:47:02.000000 highyield-1.0.8/highyield.egg-info/not-zip-safe
--rw-r--r--   0 v1         (502) wheel        (0)       30 2023-01-18 22:32:06.000000 highyield-1.0.8/highyield.egg-info/requires.txt
--rw-r--r--   0 v1         (502) wheel        (0)       10 2023-01-18 22:32:06.000000 highyield-1.0.8/highyield.egg-info/top_level.txt
--rw-r--r--   0 v1         (502) wheel        (0)      103 2023-01-06 22:57:09.000000 highyield-1.0.8/pyproject.toml
--rw-r--r--   0 v1         (502) wheel        (0)       38 2023-01-18 22:32:06.084413 highyield-1.0.8/setup.cfg
--rw-r--r--   0 v1         (502) wheel        (0)      993 2023-01-18 22:31:58.000000 highyield-1.0.8/setup.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.197835 highyield-1.0.9/
+-rw-r--r--   0 v1         (502) wheel        (0)    35129 2023-01-06 21:21:15.000000 highyield-1.0.9/LICENSE
+-rw-r--r--   0 v1         (502) wheel        (0)       29 2023-01-06 21:17:34.000000 highyield-1.0.9/MANIFEST.in
+-rw-r--r--   0 v1         (502) wheel        (0)     1980 2023-05-17 01:26:49.197602 highyield-1.0.9/PKG-INFO
+-rw-r--r--   0 v1         (502) wheel        (0)     1469 2023-05-17 01:03:18.000000 highyield-1.0.9/README.md
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.196186 highyield-1.0.9/highyield/
+-rw-r--r--   0 v1         (502) wheel        (0)      198 2023-01-06 23:04:04.000000 highyield-1.0.9/highyield/__init__.py
+-rw-r--r--   0 v1         (502) wheel        (0)      491 2023-05-17 01:12:26.000000 highyield-1.0.9/highyield/basics.py
+-rw-r--r--   0 v1         (502) wheel        (0)     3075 2023-01-02 19:44:42.000000 highyield-1.0.9/highyield/converter.py
+-rw-r--r--   0 v1         (502) wheel        (0)     4265 2023-01-04 22:06:46.000000 highyield-1.0.9/highyield/copy.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1691 2023-01-18 22:18:24.000000 highyield-1.0.9/highyield/create.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.197045 highyield-1.0.9/highyield/data/
+-rw-r--r--   0 v1         (502) wheel        (0)     1906 2023-01-03 23:05:21.000000 highyield-1.0.9/highyield/data/RR.csv
+-rw-r--r--   0 v1         (502) wheel        (0)      346 2023-01-07 14:41:36.000000 highyield-1.0.9/highyield/imports.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1534 2023-01-06 18:44:52.000000 highyield-1.0.9/highyield/pdf.py
+-rw-r--r--   0 v1         (502) wheel        (0)     1330 2023-01-15 13:10:42.000000 highyield-1.0.9/highyield/rename.py
+-rw-r--r--   0 v1         (502) wheel        (0)     4878 2023-01-07 14:45:09.000000 highyield-1.0.9/highyield/tts.py
+drwxr-xr-x   0 v1         (502) wheel        (0)        0 2023-05-17 01:26:49.196931 highyield-1.0.9/highyield.egg-info/
+-rw-r--r--   0 v1         (502) wheel        (0)     1980 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/PKG-INFO
+-rw-r--r--   0 v1         (502) wheel        (0)      449 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/SOURCES.txt
+-rw-r--r--   0 v1         (502) wheel        (0)        1 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/dependency_links.txt
+-rw-r--r--   0 v1         (502) wheel        (0)        1 2023-01-06 23:47:02.000000 highyield-1.0.9/highyield.egg-info/not-zip-safe
+-rw-r--r--   0 v1         (502) wheel        (0)       30 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/requires.txt
+-rw-r--r--   0 v1         (502) wheel        (0)       10 2023-05-17 01:26:49.000000 highyield-1.0.9/highyield.egg-info/top_level.txt
+-rw-r--r--   0 v1         (502) wheel        (0)      103 2023-01-06 22:57:09.000000 highyield-1.0.9/pyproject.toml
+-rw-r--r--   0 v1         (502) wheel        (0)       38 2023-05-17 01:26:49.197891 highyield-1.0.9/setup.cfg
+-rw-r--r--   0 v1         (502) wheel        (0)      993 2023-05-17 01:03:39.000000 highyield-1.0.9/setup.py
```

### Comparing `highyield-1.0.8/LICENSE` & `highyield-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/PKG-INFO` & `highyield-1.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6869 6768  : 2.1.Name: high
 00000020: 7969 656c 640a 5665 7273 696f 6e3a 2031  yield.Version: 1
-00000030: 2e30 2e38 0a53 756d 6d61 7279 3a20 436f  .0.8.Summary: Co
+00000030: 2e30 2e39 0a53 756d 6d61 7279 3a20 436f  .0.9.Summary: Co
 00000040: 6c6c 6563 7469 6f6e 206f 6620 6869 6768  llection of high
 00000050: 2d79 6965 6c64 2066 756e 6374 696f 6e73  -yield functions
 00000060: 2069 6e74 656e 6465 6420 746f 2073 696d   intended to sim
 00000070: 706c 6966 7920 616e 6420 6175 746f 6d61  plify and automa
 00000080: 7465 2073 7065 6369 6669 6320 7461 736b  te specific task
 00000090: 732e 0a48 6f6d 652d 7061 6765 3a20 6874  s..Home-page: ht
 000000a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
@@ -26,75 +26,99 @@
 00000190: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 000001a0: 6570 656e 6465 6e74 0a52 6571 7569 7265  ependent.Require
 000001b0: 732d 5079 7468 6f6e 3a20 3e3d 332e 380a  s-Python: >=3.8.
 000001c0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 000001d0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 000001e0: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
 000001f0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
-00000200: 2320 6869 6768 7969 656c 640a 0a5b 215b  # highyield..[![
-00000210: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
-00000220: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000230: 692f 762f 6869 6768 7969 656c 642e 7376  i/v/highyield.sv
-00000240: 6729 5d28 6874 7470 733a 2f2f 7079 7069  g)](https://pypi
-00000250: 2e6f 7267 2f70 726f 6a65 6374 2f68 6967  .org/project/hig
-00000260: 6879 6965 6c64 2920 5b21 5b4c 6963 656e  hyield) [![Licen
-00000270: 7365 3a20 4750 4c20 7633 5d28 6874 7470  se: GPL v3](http
-00000280: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000290: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
-000002a0: 2d47 504c 7633 2d62 7269 6768 7467 7265  -GPLv3-brightgre
-000002b0: 656e 2e73 7667 295d 2868 7474 7073 3a2f  en.svg)](https:/
-000002c0: 2f77 7777 2e67 6e75 2e6f 7267 2f6c 6963  /www.gnu.org/lic
-000002d0: 656e 7365 732f 6770 6c2d 332e 3029 205b  enses/gpl-3.0) [
-000002e0: 215b 5d28 6874 7470 733a 2f2f 696d 672e  ![](https://img.
-000002f0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000300: 2f2d 446f 6375 6d65 6e74 6174 696f 6e2d  /-Documentation-
-00000310: 7965 6c6c 6f77 295d 2868 7474 7073 3a2f  yellow)](https:/
-00000320: 2f6b 656e 6631 2e67 6974 6875 622e 696f  /kenf1.github.io
-00000330: 2f52 656e 6465 7265 642f 6869 6768 7969  /Rendered/highyi
-00000340: 656c 6425 3230 446f 6375 6d65 6e74 6174  eld%20Documentat
-00000350: 696f 6e2f 290a 0a60 6869 6768 7969 656c  ion/)..`highyiel
-00000360: 6460 2069 7320 6120 5079 7468 6f6e 2070  d` is a Python p
-00000370: 6163 6b61 6765 2063 6f6e 7461 696e 696e  ackage containin
-00000380: 6720 6120 636f 6c6c 6563 7469 6f6e 206f  g a collection o
-00000390: 6620 6869 6768 2d79 6965 6c64 2066 756e  f high-yield fun
-000003a0: 6374 696f 6e73 2028 6772 6f75 7065 6420  ctions (grouped 
-000003b0: 6279 206d 6f64 756c 6573 2920 696e 7465  by modules) inte
-000003c0: 6e64 6564 2074 6f20 7369 6d70 6c69 6679  nded to simplify
-000003d0: 2061 6e64 2061 7574 6f6d 6174 6520 7370   and automate sp
-000003e0: 6563 6966 6963 2074 6173 6b73 2e0a 0a54  ecific tasks...T
-000003f0: 6869 7320 7061 636b 6167 6520 7265 7175  his package requ
-00000400: 6972 6573 2050 7974 686f 6e20 3e3d 2033  ires Python >= 3
-00000410: 2e38 2064 7565 2074 6f20 7265 6c69 616e  .8 due to relian
-00000420: 6365 206f 6e20 5b60 7061 6e64 6173 6020  ce on [`pandas` 
-00000430: 7061 636b 6167 655d 2868 7474 7073 3a2f  package](https:/
-00000440: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000450: 742f 7061 6e64 6173 2f29 2e0a 0a23 2323  t/pandas/)...###
-00000460: 2049 6e73 7461 6c6c 0a0a 546f 2069 6e73   Install..To ins
-00000470: 7461 6c6c 2c20 6f70 656e 2074 6865 2074  tall, open the t
-00000480: 6572 6d69 6e61 6c20 616e 6420 7479 7065  erminal and type
-00000490: 2069 6e20 7468 6520 666f 6c6c 6f77 696e   in the followin
-000004a0: 672e 0a0a 466f 7220 5769 6e64 6f77 7320  g...For Windows 
-000004b0: 616e 6420 4c69 6e75 783a 0a0a 6060 607b  and Linux:..```{
-000004c0: 7079 7468 6f6e 7d0a 7069 7020 696e 7374  python}.pip inst
-000004d0: 616c 6c20 6869 6768 7969 656c 640a 6060  all highyield.``
-000004e0: 600a 0a46 6f72 206d 6163 4f53 3a0a 0a60  `..For macOS:..`
-000004f0: 6060 7b70 7974 686f 6e7d 0a70 7974 686f  ``{python}.pytho
-00000500: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
-00000510: 6c20 6869 6768 7969 656c 640a 6060 600a  l highyield.```.
-00000520: 0a23 2323 2044 6570 656e 6465 6e63 6965  .### Dependencie
-00000530: 730a 0a54 6865 2074 6162 6c65 2062 656c  s..The table bel
-00000540: 6f77 206c 6973 7473 2074 6865 2064 6570  ow lists the dep
-00000550: 656e 6465 6e63 6965 7320 666f 7220 6561  endencies for ea
-00000560: 6368 206d 6f64 756c 6520 7769 7468 696e  ch module within
-00000570: 2074 6869 7320 7061 636b 6167 653a 0a0a   this package:..
-00000580: 7c4d 6f64 756c 657c 5061 636b 6167 6573  |Module|Packages
-00000590: 7c0a 7c2d 2d2d 7c2d 2d2d 7c0a 7c63 6f6e  |.|---|---|.|con
-000005a0: 7665 7274 6572 7c6f 732c 2070 616e 6461  verter|os, panda
-000005b0: 732c 2064 6f63 7832 7064 667c 0a7c 636f  s, docx2pdf|.|co
-000005c0: 7079 7c6f 732c 2073 6875 7469 6c2c 2070  py|os, shutil, p
-000005d0: 616e 6461 737c 0a7c 6372 6561 7465 7c6f  andas|.|create|o
-000005e0: 732c 2073 6875 7469 6c7c 0a7c 696d 706f  s, shutil|.|impo
-000005f0: 7274 737c 696d 706f 7274 6c69 622c 2070  rts|importlib, p
-00000600: 616e 6461 737c 0a7c 7064 667c 6f73 2c20  andas|.|pdf|os, 
-00000610: 7079 7064 667c 0a7c 7265 6e61 6d65 7c6f  pypdf|.|rename|o
-00000620: 732c 2072 657c 0a7c 7474 737c 7079 7474  s, re|.|tts|pytt
-00000630: 7378 332c 2070 616e 6461 737c 0a         sx3, pandas|.
+00000200: 2320 6869 6768 7969 656c 6420 603c 6120  # highyield `<a 
+00000210: 6872 6566 3d22 6874 7470 733a 2f2f 6b65  href="https://ke
+00000220: 6e66 312e 6769 7468 7562 2e69 6f2f 5265  nf1.github.io/Re
+00000230: 6e64 6572 6564 2f68 6967 6879 6965 6c64  ndered/highyield
+00000240: 2532 3044 6f63 756d 656e 7461 7469 6f6e  %20Documentation
+00000250: 2f22 3e3c 696d 6720 7372 633d 2268 7474  /"><img src="htt
+00000260: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000270: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f6b  sercontent.com/k
+00000280: 656e 6631 2f52 656e 6465 7265 642f 6d61  enf1/Rendered/ma
+00000290: 696e 2f48 6578 5f53 7469 636b 6572 2f48  in/Hex_Sticker/H
+000002a0: 6967 682d 5969 656c 642e 706e 6722 2061  igh-Yield.png" a
+000002b0: 6c69 676e 3d22 7269 6768 7422 2068 6569  lign="right" hei
+000002c0: 6768 743d 2231 3338 2e35 2220 2f3e 6060  ght="138.5" />``
+000002d0: 3c2f 613e 600a 0a5b 215b 5079 5049 5d28  </a>`..[![PyPI](
+000002e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000002f0: 6c64 732e 696f 2f70 7970 692f 762f 6869  lds.io/pypi/v/hi
+00000300: 6768 7969 656c 642e 7376 6729 5d28 6874  ghyield.svg)](ht
+00000310: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000320: 726f 6a65 6374 2f68 6967 6879 6965 6c64  roject/highyield
+00000330: 2920 5b21 5b4c 6963 656e 7365 3a20 4750  ) [![License: GP
+00000340: 4c20 7633 5d28 6874 7470 733a 2f2f 696d  L v3](https://im
+00000350: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000360: 6765 2f4c 6963 656e 7365 2d47 504c 7633  ge/License-GPLv3
+00000370: 2d62 7269 6768 7467 7265 656e 2e73 7667  -brightgreen.svg
+00000380: 295d 2868 7474 7073 3a2f 2f77 7777 2e67  )](https://www.g
+00000390: 6e75 2e6f 7267 2f6c 6963 656e 7365 732f  nu.org/licenses/
+000003a0: 6770 6c2d 332e 3029 205b 215b 5d28 6874  gpl-3.0) [![](ht
+000003b0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000003c0: 732e 696f 2f62 6164 6765 2f2d 446f 6375  s.io/badge/-Docu
+000003d0: 6d65 6e74 6174 696f 6e2d 7965 6c6c 6f77  mentation-yellow
+000003e0: 295d 2868 7474 7073 3a2f 2f6b 656e 6631  )](https://kenf1
+000003f0: 2e67 6974 6875 622e 696f 2f52 656e 6465  .github.io/Rende
+00000400: 7265 642f 6869 6768 7969 656c 6425 3230  red/highyield%20
+00000410: 446f 6375 6d65 6e74 6174 696f 6e2f 290a  Documentation/).
+00000420: 0a60 6869 6768 7969 656c 6460 2069 7320  .`highyield` is 
+00000430: 6120 5079 7468 6f6e 2070 6163 6b61 6765  a Python package
+00000440: 2063 6f6e 7461 696e 696e 6720 6120 636f   containing a co
+00000450: 6c6c 6563 7469 6f6e 206f 6620 6869 6768  llection of high
+00000460: 2d79 6965 6c64 2066 756e 6374 696f 6e73  -yield functions
+00000470: 2028 6772 6f75 7065 6420 6279 206d 6f64   (grouped by mod
+00000480: 756c 6573 2920 696e 7465 6e64 6564 2074  ules) intended t
+00000490: 6f20 7369 6d70 6c69 6679 2061 6e64 2061  o simplify and a
+000004a0: 7574 6f6d 6174 6520 7370 6563 6966 6963  utomate specific
+000004b0: 2074 6173 6b73 2e0a 0a54 6869 7320 7061   tasks...This pa
+000004c0: 636b 6167 6520 7265 7175 6972 6573 2050  ckage requires P
+000004d0: 7974 686f 6e20 3e3d 2033 2e38 2064 7565  ython >= 3.8 due
+000004e0: 2074 6f20 7265 6c69 616e 6365 206f 6e20   to reliance on 
+000004f0: 5b60 7061 6e64 6173 6020 7061 636b 6167  [`pandas` packag
+00000500: 655d 2868 7474 7073 3a2f 2f70 7970 692e  e](https://pypi.
+00000510: 6f72 672f 7072 6f6a 6563 742f 7061 6e64  org/project/pand
+00000520: 6173 2f29 2e0a 0a23 2323 2049 6e73 7461  as/)...### Insta
+00000530: 6c6c 0a0a 546f 2069 6e73 7461 6c6c 2c20  ll..To install, 
+00000540: 6f70 656e 2074 6865 2074 6572 6d69 6e61  open the termina
+00000550: 6c20 616e 6420 7479 7065 2069 6e20 7468  l and type in th
+00000560: 6520 666f 6c6c 6f77 696e 672e 0a0a 466f  e following...Fo
+00000570: 7220 5769 6e64 6f77 7320 616e 6420 4c69  r Windows and Li
+00000580: 6e75 783a 0a0a 6060 607b 7079 7468 6f6e  nux:..```{python
+00000590: 7d0a 7069 7020 696e 7374 616c 6c20 6869  }.pip install hi
+000005a0: 6768 7969 656c 640a 6060 600a 0a46 6f72  ghyield.```..For
+000005b0: 206d 6163 4f53 3a0a 0a60 6060 7b70 7974   macOS:..```{pyt
+000005c0: 686f 6e7d 0a70 7974 686f 6e33 202d 6d20  hon}.python3 -m 
+000005d0: 7069 7020 696e 7374 616c 6c20 6869 6768  pip install high
+000005e0: 7969 656c 640a 6060 600a 0a23 2323 2044  yield.```..### D
+000005f0: 6570 656e 6465 6e63 6965 730a 0a54 6865  ependencies..The
+00000600: 2074 6162 6c65 2062 656c 6f77 206c 6973   table below lis
+00000610: 7473 2074 6865 2064 6570 656e 6465 6e63  ts the dependenc
+00000620: 6965 7320 666f 7220 6561 6368 206d 6f64  ies for each mod
+00000630: 756c 6520 7769 7468 696e 2074 6869 7320  ule within this 
+00000640: 7061 636b 6167 653a 0a0a 7c20 4d6f 6475  package:..| Modu
+00000650: 6c65 2020 2020 7c20 5061 636b 6167 6573  le    | Packages
+00000660: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00000670: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+00000680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000690: 2d20 7c0a 7c20 6261 7369 6373 2020 2020  - |.| basics    
+000006a0: 7c20 6f73 2020 2020 2020 2020 2020 2020  | os            
+000006b0: 2020 2020 2020 207c 0a7c 2063 6f6e 7665         |.| conve
+000006c0: 7274 6572 207c 206f 732c 2070 616e 6461  rter | os, panda
+000006d0: 732c 2064 6f63 7832 7064 6620 7c0a 7c20  s, docx2pdf |.| 
+000006e0: 636f 7079 2020 2020 2020 7c20 6f73 2c20  copy      | os, 
+000006f0: 7368 7574 696c 2c20 7061 6e64 6173 2020  shutil, pandas  
+00000700: 207c 0a7c 2063 7265 6174 6520 2020 207c   |.| create    |
+00000710: 206f 732c 2073 6875 7469 6c20 2020 2020   os, shutil     
+00000720: 2020 2020 2020 7c0a 7c20 696d 706f 7274        |.| import
+00000730: 7320 2020 7c20 696d 706f 7274 6c69 622c  s   | importlib,
+00000740: 2070 616e 6461 7320 2020 207c 0a7c 2070   pandas    |.| p
+00000750: 6466 2020 2020 2020 207c 206f 732c 2070  df       | os, p
+00000760: 7970 6466 2020 2020 2020 2020 2020 2020  ypdf            
+00000770: 7c0a 7c20 7265 6e61 6d65 2020 2020 7c20  |.| rename    | 
+00000780: 6f73 2c20 7265 2020 2020 2020 2020 2020  os, re          
+00000790: 2020 2020 207c 0a7c 2074 7473 2020 2020       |.| tts    
+000007a0: 2020 207c 2070 7974 7473 7833 2c20 7061     | pyttsx3, pa
+000007b0: 6e64 6173 2020 2020 2020 7c0a            ndas      |.
```

### Comparing `highyield-1.0.8/README.md` & `highyield-1.0.9/highyield.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,124 @@
-00000000: 2323 2068 6967 6879 6965 6c64 0a0a 5b21  ## highyield..[!
-00000010: 5b50 7950 495d 2868 7474 7073 3a2f 2f69  [PyPI](https://i
-00000020: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000030: 7069 2f76 2f68 6967 6879 6965 6c64 2e73  pi/v/highyield.s
-00000040: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
-00000050: 692e 6f72 672f 7072 6f6a 6563 742f 6869  i.org/project/hi
-00000060: 6768 7969 656c 6429 205b 215b 4c69 6365  ghyield) [![Lice
-00000070: 6e73 653a 2047 504c 2076 335d 2868 7474  nse: GPL v3](htt
-00000080: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000090: 2e69 6f2f 6261 6467 652f 4c69 6365 6e73  .io/badge/Licens
-000000a0: 652d 4750 4c76 332d 6272 6967 6874 6772  e-GPLv3-brightgr
-000000b0: 6565 6e2e 7376 6729 5d28 6874 7470 733a  een.svg)](https:
-000000c0: 2f2f 7777 772e 676e 752e 6f72 672f 6c69  //www.gnu.org/li
-000000d0: 6365 6e73 6573 2f67 706c 2d33 2e30 2920  censes/gpl-3.0) 
-000000e0: 5b21 5b5d 2868 7474 7073 3a2f 2f69 6d67  [![](https://img
-000000f0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000100: 652f 2d44 6f63 756d 656e 7461 7469 6f6e  e/-Documentation
-00000110: 2d79 656c 6c6f 7729 5d28 6874 7470 733a  -yellow)](https:
-00000120: 2f2f 6b65 6e66 312e 6769 7468 7562 2e69  //kenf1.github.i
-00000130: 6f2f 5265 6e64 6572 6564 2f68 6967 6879  o/Rendered/highy
-00000140: 6965 6c64 2532 3044 6f63 756d 656e 7461  ield%20Documenta
-00000150: 7469 6f6e 2f29 0a0a 6068 6967 6879 6965  tion/)..`highyie
-00000160: 6c64 6020 6973 2061 2050 7974 686f 6e20  ld` is a Python 
-00000170: 7061 636b 6167 6520 636f 6e74 6169 6e69  package containi
-00000180: 6e67 2061 2063 6f6c 6c65 6374 696f 6e20  ng a collection 
-00000190: 6f66 2068 6967 682d 7969 656c 6420 6675  of high-yield fu
-000001a0: 6e63 7469 6f6e 7320 2867 726f 7570 6564  nctions (grouped
-000001b0: 2062 7920 6d6f 6475 6c65 7329 2069 6e74   by modules) int
-000001c0: 656e 6465 6420 746f 2073 696d 706c 6966  ended to simplif
-000001d0: 7920 616e 6420 6175 746f 6d61 7465 2073  y and automate s
-000001e0: 7065 6369 6669 6320 7461 736b 732e 0a0a  pecific tasks...
-000001f0: 5468 6973 2070 6163 6b61 6765 2072 6571  This package req
-00000200: 7569 7265 7320 5079 7468 6f6e 203e 3d20  uires Python >= 
-00000210: 332e 3820 6475 6520 746f 2072 656c 6961  3.8 due to relia
-00000220: 6e63 6520 6f6e 205b 6070 616e 6461 7360  nce on [`pandas`
-00000230: 2070 6163 6b61 6765 5d28 6874 7470 733a   package](https:
-00000240: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000250: 6374 2f70 616e 6461 732f 292e 0a0a 2323  ct/pandas/)...##
-00000260: 2320 496e 7374 616c 6c0a 0a54 6f20 696e  # Install..To in
-00000270: 7374 616c 6c2c 206f 7065 6e20 7468 6520  stall, open the 
-00000280: 7465 726d 696e 616c 2061 6e64 2074 7970  terminal and typ
-00000290: 6520 696e 2074 6865 2066 6f6c 6c6f 7769  e in the followi
-000002a0: 6e67 2e0a 0a46 6f72 2057 696e 646f 7773  ng...For Windows
-000002b0: 2061 6e64 204c 696e 7578 3a0a 0a60 6060   and Linux:..```
-000002c0: 7b70 7974 686f 6e7d 0a70 6970 2069 6e73  {python}.pip ins
-000002d0: 7461 6c6c 2068 6967 6879 6965 6c64 0a60  tall highyield.`
-000002e0: 6060 0a0a 466f 7220 6d61 634f 533a 0a0a  ``..For macOS:..
-000002f0: 6060 607b 7079 7468 6f6e 7d0a 7079 7468  ```{python}.pyth
-00000300: 6f6e 3320 2d6d 2070 6970 2069 6e73 7461  on3 -m pip insta
-00000310: 6c6c 2068 6967 6879 6965 6c64 0a60 6060  ll highyield.```
-00000320: 0a0a 2323 2320 4465 7065 6e64 656e 6369  ..### Dependenci
-00000330: 6573 0a0a 5468 6520 7461 626c 6520 6265  es..The table be
-00000340: 6c6f 7720 6c69 7374 7320 7468 6520 6465  low lists the de
-00000350: 7065 6e64 656e 6369 6573 2066 6f72 2065  pendencies for e
-00000360: 6163 6820 6d6f 6475 6c65 2077 6974 6869  ach module withi
-00000370: 6e20 7468 6973 2070 6163 6b61 6765 3a0a  n this package:.
-00000380: 0a7c 4d6f 6475 6c65 7c50 6163 6b61 6765  .|Module|Package
-00000390: 737c 0a7c 2d2d 2d7c 2d2d 2d7c 0a7c 636f  s|.|---|---|.|co
-000003a0: 6e76 6572 7465 727c 6f73 2c20 7061 6e64  nverter|os, pand
-000003b0: 6173 2c20 646f 6378 3270 6466 7c0a 7c63  as, docx2pdf|.|c
-000003c0: 6f70 797c 6f73 2c20 7368 7574 696c 2c20  opy|os, shutil, 
-000003d0: 7061 6e64 6173 7c0a 7c63 7265 6174 657c  pandas|.|create|
-000003e0: 6f73 2c20 7368 7574 696c 7c0a 7c69 6d70  os, shutil|.|imp
-000003f0: 6f72 7473 7c69 6d70 6f72 746c 6962 2c20  orts|importlib, 
-00000400: 7061 6e64 6173 7c0a 7c70 6466 7c6f 732c  pandas|.|pdf|os,
-00000410: 2070 7970 6466 7c0a 7c72 656e 616d 657c   pypdf|.|rename|
-00000420: 6f73 2c20 7265 7c0a 7c74 7473 7c70 7974  os, re|.|tts|pyt
-00000430: 7473 7833 2c20 7061 6e64 6173 7c         tsx3, pandas|
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6869 6768  : 2.1.Name: high
+00000020: 7969 656c 640a 5665 7273 696f 6e3a 2031  yield.Version: 1
+00000030: 2e30 2e39 0a53 756d 6d61 7279 3a20 436f  .0.9.Summary: Co
+00000040: 6c6c 6563 7469 6f6e 206f 6620 6869 6768  llection of high
+00000050: 2d79 6965 6c64 2066 756e 6374 696f 6e73  -yield functions
+00000060: 2069 6e74 656e 6465 6420 746f 2073 696d   intended to sim
+00000070: 706c 6966 7920 616e 6420 6175 746f 6d61  plify and automa
+00000080: 7465 2073 7065 6369 6669 6320 7461 736b  te specific task
+00000090: 732e 0a48 6f6d 652d 7061 6765 3a20 6874  s..Home-page: ht
+000000a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000000b0: 2f6b 656e 6631 2f48 6967 682d 5969 656c  /kenf1/High-Yiel
+000000c0: 640a 4175 7468 6f72 3a20 4b46 0a41 7574  d.Author: KF.Aut
+000000d0: 686f 722d 656d 6169 6c3a 206b 656e 6676  hor-email: kenfv
+000000e0: 3140 6f75 746c 6f6f 6b2e 636f 6d0a 4c69  1@outlook.com.Li
+000000f0: 6365 6e73 653a 2047 504c 7633 0a43 6c61  cense: GPLv3.Cla
+00000100: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000110: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000120: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
+00000130: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00000140: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000150: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+00000160: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+00000170: 3320 2847 504c 7633 290a 436c 6173 7369  3 (GPLv3).Classi
+00000180: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000190: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001a0: 6570 656e 6465 6e74 0a52 6571 7569 7265  ependent.Require
+000001b0: 732d 5079 7468 6f6e 3a20 3e3d 332e 380a  s-Python: >=3.8.
+000001c0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+000001d0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+000001e0: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
+000001f0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
+00000200: 2320 6869 6768 7969 656c 6420 603c 6120  # highyield `<a 
+00000210: 6872 6566 3d22 6874 7470 733a 2f2f 6b65  href="https://ke
+00000220: 6e66 312e 6769 7468 7562 2e69 6f2f 5265  nf1.github.io/Re
+00000230: 6e64 6572 6564 2f68 6967 6879 6965 6c64  ndered/highyield
+00000240: 2532 3044 6f63 756d 656e 7461 7469 6f6e  %20Documentation
+00000250: 2f22 3e3c 696d 6720 7372 633d 2268 7474  /"><img src="htt
+00000260: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000270: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f6b  sercontent.com/k
+00000280: 656e 6631 2f52 656e 6465 7265 642f 6d61  enf1/Rendered/ma
+00000290: 696e 2f48 6578 5f53 7469 636b 6572 2f48  in/Hex_Sticker/H
+000002a0: 6967 682d 5969 656c 642e 706e 6722 2061  igh-Yield.png" a
+000002b0: 6c69 676e 3d22 7269 6768 7422 2068 6569  lign="right" hei
+000002c0: 6768 743d 2231 3338 2e35 2220 2f3e 6060  ght="138.5" />``
+000002d0: 3c2f 613e 600a 0a5b 215b 5079 5049 5d28  </a>`..[![PyPI](
+000002e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000002f0: 6c64 732e 696f 2f70 7970 692f 762f 6869  lds.io/pypi/v/hi
+00000300: 6768 7969 656c 642e 7376 6729 5d28 6874  ghyield.svg)](ht
+00000310: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000320: 726f 6a65 6374 2f68 6967 6879 6965 6c64  roject/highyield
+00000330: 2920 5b21 5b4c 6963 656e 7365 3a20 4750  ) [![License: GP
+00000340: 4c20 7633 5d28 6874 7470 733a 2f2f 696d  L v3](https://im
+00000350: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000360: 6765 2f4c 6963 656e 7365 2d47 504c 7633  ge/License-GPLv3
+00000370: 2d62 7269 6768 7467 7265 656e 2e73 7667  -brightgreen.svg
+00000380: 295d 2868 7474 7073 3a2f 2f77 7777 2e67  )](https://www.g
+00000390: 6e75 2e6f 7267 2f6c 6963 656e 7365 732f  nu.org/licenses/
+000003a0: 6770 6c2d 332e 3029 205b 215b 5d28 6874  gpl-3.0) [![](ht
+000003b0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000003c0: 732e 696f 2f62 6164 6765 2f2d 446f 6375  s.io/badge/-Docu
+000003d0: 6d65 6e74 6174 696f 6e2d 7965 6c6c 6f77  mentation-yellow
+000003e0: 295d 2868 7474 7073 3a2f 2f6b 656e 6631  )](https://kenf1
+000003f0: 2e67 6974 6875 622e 696f 2f52 656e 6465  .github.io/Rende
+00000400: 7265 642f 6869 6768 7969 656c 6425 3230  red/highyield%20
+00000410: 446f 6375 6d65 6e74 6174 696f 6e2f 290a  Documentation/).
+00000420: 0a60 6869 6768 7969 656c 6460 2069 7320  .`highyield` is 
+00000430: 6120 5079 7468 6f6e 2070 6163 6b61 6765  a Python package
+00000440: 2063 6f6e 7461 696e 696e 6720 6120 636f   containing a co
+00000450: 6c6c 6563 7469 6f6e 206f 6620 6869 6768  llection of high
+00000460: 2d79 6965 6c64 2066 756e 6374 696f 6e73  -yield functions
+00000470: 2028 6772 6f75 7065 6420 6279 206d 6f64   (grouped by mod
+00000480: 756c 6573 2920 696e 7465 6e64 6564 2074  ules) intended t
+00000490: 6f20 7369 6d70 6c69 6679 2061 6e64 2061  o simplify and a
+000004a0: 7574 6f6d 6174 6520 7370 6563 6966 6963  utomate specific
+000004b0: 2074 6173 6b73 2e0a 0a54 6869 7320 7061   tasks...This pa
+000004c0: 636b 6167 6520 7265 7175 6972 6573 2050  ckage requires P
+000004d0: 7974 686f 6e20 3e3d 2033 2e38 2064 7565  ython >= 3.8 due
+000004e0: 2074 6f20 7265 6c69 616e 6365 206f 6e20   to reliance on 
+000004f0: 5b60 7061 6e64 6173 6020 7061 636b 6167  [`pandas` packag
+00000500: 655d 2868 7474 7073 3a2f 2f70 7970 692e  e](https://pypi.
+00000510: 6f72 672f 7072 6f6a 6563 742f 7061 6e64  org/project/pand
+00000520: 6173 2f29 2e0a 0a23 2323 2049 6e73 7461  as/)...### Insta
+00000530: 6c6c 0a0a 546f 2069 6e73 7461 6c6c 2c20  ll..To install, 
+00000540: 6f70 656e 2074 6865 2074 6572 6d69 6e61  open the termina
+00000550: 6c20 616e 6420 7479 7065 2069 6e20 7468  l and type in th
+00000560: 6520 666f 6c6c 6f77 696e 672e 0a0a 466f  e following...Fo
+00000570: 7220 5769 6e64 6f77 7320 616e 6420 4c69  r Windows and Li
+00000580: 6e75 783a 0a0a 6060 607b 7079 7468 6f6e  nux:..```{python
+00000590: 7d0a 7069 7020 696e 7374 616c 6c20 6869  }.pip install hi
+000005a0: 6768 7969 656c 640a 6060 600a 0a46 6f72  ghyield.```..For
+000005b0: 206d 6163 4f53 3a0a 0a60 6060 7b70 7974   macOS:..```{pyt
+000005c0: 686f 6e7d 0a70 7974 686f 6e33 202d 6d20  hon}.python3 -m 
+000005d0: 7069 7020 696e 7374 616c 6c20 6869 6768  pip install high
+000005e0: 7969 656c 640a 6060 600a 0a23 2323 2044  yield.```..### D
+000005f0: 6570 656e 6465 6e63 6965 730a 0a54 6865  ependencies..The
+00000600: 2074 6162 6c65 2062 656c 6f77 206c 6973   table below lis
+00000610: 7473 2074 6865 2064 6570 656e 6465 6e63  ts the dependenc
+00000620: 6965 7320 666f 7220 6561 6368 206d 6f64  ies for each mod
+00000630: 756c 6520 7769 7468 696e 2074 6869 7320  ule within this 
+00000640: 7061 636b 6167 653a 0a0a 7c20 4d6f 6475  package:..| Modu
+00000650: 6c65 2020 2020 7c20 5061 636b 6167 6573  le    | Packages
+00000660: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00000670: 202d 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d   --------- | ---
+00000680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000690: 2d20 7c0a 7c20 6261 7369 6373 2020 2020  - |.| basics    
+000006a0: 7c20 6f73 2020 2020 2020 2020 2020 2020  | os            
+000006b0: 2020 2020 2020 207c 0a7c 2063 6f6e 7665         |.| conve
+000006c0: 7274 6572 207c 206f 732c 2070 616e 6461  rter | os, panda
+000006d0: 732c 2064 6f63 7832 7064 6620 7c0a 7c20  s, docx2pdf |.| 
+000006e0: 636f 7079 2020 2020 2020 7c20 6f73 2c20  copy      | os, 
+000006f0: 7368 7574 696c 2c20 7061 6e64 6173 2020  shutil, pandas  
+00000700: 207c 0a7c 2063 7265 6174 6520 2020 207c   |.| create    |
+00000710: 206f 732c 2073 6875 7469 6c20 2020 2020   os, shutil     
+00000720: 2020 2020 2020 7c0a 7c20 696d 706f 7274        |.| import
+00000730: 7320 2020 7c20 696d 706f 7274 6c69 622c  s   | importlib,
+00000740: 2070 616e 6461 7320 2020 207c 0a7c 2070   pandas    |.| p
+00000750: 6466 2020 2020 2020 207c 206f 732c 2070  df       | os, p
+00000760: 7970 6466 2020 2020 2020 2020 2020 2020  ypdf            
+00000770: 7c0a 7c20 7265 6e61 6d65 2020 2020 7c20  |.| rename    | 
+00000780: 6f73 2c20 7265 2020 2020 2020 2020 2020  os, re          
+00000790: 2020 2020 207c 0a7c 2074 7473 2020 2020       |.| tts    
+000007a0: 2020 207c 2070 7974 7473 7833 2c20 7061     | pyttsx3, pa
+000007b0: 6e64 6173 2020 2020 2020 7c0a            ndas      |.
```

### Comparing `highyield-1.0.8/highyield/converter.py` & `highyield-1.0.9/highyield/converter.py`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/highyield/copy.py` & `highyield-1.0.9/highyield/copy.py`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/highyield/create.py` & `highyield-1.0.9/highyield/create.py`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/highyield/data/RR.csv` & `highyield-1.0.9/highyield/data/RR.csv`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/highyield/pdf.py` & `highyield-1.0.9/highyield/pdf.py`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/highyield/rename.py` & `highyield-1.0.9/highyield/rename.py`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/highyield/tts.py` & `highyield-1.0.9/highyield/tts.py`

 * *Files identical despite different names*

### Comparing `highyield-1.0.8/setup.py` & `highyield-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text()
 
 setup(name="highyield",
-      version="1.0.8",
+      version="1.0.9",
       description="Collection of high-yield functions intended to simplify and automate specific tasks.",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/kenf1/High-Yield",
       author="KF",
       author_email="kenfv1@outlook.com",
       license="GPLv3",
```

