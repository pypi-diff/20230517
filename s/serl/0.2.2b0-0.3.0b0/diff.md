# Comparing `tmp/serl-0.2.2b0.tar.gz` & `tmp/serl-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serl-0.2.2b0.tar", last modified: Sat Apr 29 17:36:04 2023, max compression
+gzip compressed data, was "serl-0.3.0b0.tar", last modified: Wed May 17 09:12:51 2023, max compression
```

## Comparing `serl-0.2.2b0.tar` & `serl-0.3.0b0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.767347 serl-0.2.2b0/
--rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.2.2b0/LICENSE
--rw-rw-rw-   0        0        0     2294 2023-04-29 17:36:04.767347 serl-0.2.2b0/PKG-INFO
--rw-rw-rw-   0        0        0      652 2023-04-27 13:33:45.000000 serl-0.2.2b0/README.md
--rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.2.2b0/pyproject.toml
--rw-rw-rw-   0        0        0      897 2023-04-29 17:36:04.774681 serl-0.2.2b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.651546 serl-0.2.2b0/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.715644 serl-0.2.2b0/src/serl/
--rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.2.2b0/src/serl/__init__.py
--rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.2.2b0/src/serl/__main__.py
--rw-rw-rw-   0        0        0     2726 2023-04-17 21:26:43.000000 serl-0.2.2b0/src/serl/config.py
--rw-rw-rw-   0        0        0     3691 2023-04-29 17:34:44.000000 serl-0.2.2b0/src/serl/constants.py
--rw-rw-rw-   0        0        0     3768 2023-04-28 08:16:32.000000 serl-0.2.2b0/src/serl/highlight.py
--rw-rw-rw-   0        0        0     3731 2023-04-26 14:18:07.000000 serl-0.2.2b0/src/serl/lexer.py
--rw-rw-rw-   0        0        0     3359 2023-04-17 20:35:29.000000 serl-0.2.2b0/src/serl/logger.py
--rw-rw-rw-   0        0        0    18751 2023-04-27 13:50:07.000000 serl-0.2.2b0/src/serl/main.py
--rw-rw-rw-   0        0        0     4893 2023-04-27 13:16:35.000000 serl-0.2.2b0/src/serl/parser.py
--rw-rw-rw-   0        0        0     2933 2023-04-21 14:34:29.000000 serl-0.2.2b0/src/serl/schema.py
--rw-rw-rw-   0        0        0     4819 2023-04-27 13:25:04.000000 serl-0.2.2b0/src/serl/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.748816 serl-0.2.2b0/src/serl.egg-info/
--rw-rw-rw-   0        0        0     2294 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-29 17:36:04.000000 serl-0.2.2b0/src/serl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 17:36:04.765060 serl-0.2.2b0/tests/
--rw-rw-rw-   0        0        0      572 2023-04-17 18:50:19.000000 serl-0.2.2b0/tests/test_config.py
--rw-rw-rw-   0        0        0      807 2023-04-04 06:33:54.000000 serl-0.2.2b0/tests/test_highlight.py
--rw-rw-rw-   0        0        0     2156 2023-04-26 14:06:44.000000 serl-0.2.2b0/tests/test_lexer.py
--rw-rw-rw-   0        0        0     4461 2023-04-20 22:48:18.000000 serl-0.2.2b0/tests/test_main.py
--rw-rw-rw-   0        0        0     2390 2023-04-17 18:00:20.000000 serl-0.2.2b0/tests/test_parser.py
--rw-rw-rw-   0        0        0     1896 2023-04-17 08:06:23.000000 serl-0.2.2b0/tests/test_schema.py
--rw-rw-rw-   0        0        0     5486 2023-04-25 06:59:43.000000 serl-0.2.2b0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:12:51.756569 serl-0.3.0b0/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.3.0b0/LICENSE
+-rw-rw-rw-   0        0        0     2938 2023-05-17 09:12:51.756569 serl-0.3.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2023-05-17 09:08:04.000000 serl-0.3.0b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.3.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0      917 2023-05-17 09:12:51.756569 serl-0.3.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 09:12:51.658517 serl-0.3.0b0/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 09:12:51.723087 serl-0.3.0b0/src/serl/
+-rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.3.0b0/src/serl/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.3.0b0/src/serl/__main__.py
+-rw-rw-rw-   0        0        0     2726 2023-04-17 21:26:43.000000 serl-0.3.0b0/src/serl/config.py
+-rw-rw-rw-   0        0        0     3911 2023-05-16 14:06:29.000000 serl-0.3.0b0/src/serl/constants.py
+-rw-rw-rw-   0        0        0     3768 2023-04-28 08:16:32.000000 serl-0.3.0b0/src/serl/highlight.py
+-rw-rw-rw-   0        0        0     3731 2023-04-26 14:18:07.000000 serl-0.3.0b0/src/serl/lexer.py
+-rw-rw-rw-   0        0        0     3359 2023-04-17 20:35:29.000000 serl-0.3.0b0/src/serl/logger.py
+-rw-rw-rw-   0        0        0    18992 2023-05-15 20:59:30.000000 serl-0.3.0b0/src/serl/main.py
+-rw-rw-rw-   0        0        0     4893 2023-04-27 13:16:35.000000 serl-0.3.0b0/src/serl/parser.py
+-rw-rw-rw-   0        0        0     2933 2023-04-21 14:34:29.000000 serl-0.3.0b0/src/serl/schema.py
+-rw-rw-rw-   0        0        0     4819 2023-04-27 13:25:04.000000 serl-0.3.0b0/src/serl/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:12:51.756569 serl-0.3.0b0/src/serl.egg-info/
+-rw-rw-rw-   0        0        0     2938 2023-05-17 09:12:51.000000 serl-0.3.0b0/src/serl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-17 09:12:51.000000 serl-0.3.0b0/src/serl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 09:12:51.000000 serl-0.3.0b0/src/serl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-17 09:12:51.000000 serl-0.3.0b0/src/serl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-05-17 09:12:51.000000 serl-0.3.0b0/src/serl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-17 09:12:51.000000 serl-0.3.0b0/src/serl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 09:12:51.756569 serl-0.3.0b0/tests/
+-rw-rw-rw-   0        0        0      572 2023-04-17 18:50:19.000000 serl-0.3.0b0/tests/test_config.py
+-rw-rw-rw-   0        0        0      807 2023-04-04 06:33:54.000000 serl-0.3.0b0/tests/test_highlight.py
+-rw-rw-rw-   0        0        0     2156 2023-04-26 14:06:44.000000 serl-0.3.0b0/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     4461 2023-04-20 22:48:18.000000 serl-0.3.0b0/tests/test_main.py
+-rw-rw-rw-   0        0        0     2390 2023-04-17 18:00:20.000000 serl-0.3.0b0/tests/test_parser.py
+-rw-rw-rw-   0        0        0     1896 2023-04-17 08:06:23.000000 serl-0.3.0b0/tests/test_schema.py
+-rw-rw-rw-   0        0        0     5486 2023-04-25 06:59:43.000000 serl-0.3.0b0/tests/test_utils.py
```

### Comparing `serl-0.2.2b0/LICENSE` & `serl-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/PKG-INFO` & `serl-0.3.0b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,144 +1,184 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2073 6572  : 2.1..Name: ser
-00000020: 6c0d 0a56 6572 7369 6f6e 3a20 302e 322e  l..Version: 0.2.
-00000030: 3262 300d 0a53 756d 6d61 7279 3a20 5365  2b0..Summary: Se
-00000040: 7269 616c 697a 6564 204c 616e 6775 6167  rialized Languag
-00000050: 6520 2873 6572 6c29 0d0a 4175 7468 6f72  e (serl)..Author
-00000060: 3a20 4861 7272 7920 446f 776e 696e 670d  : Harry Downing.
-00000070: 0a41 7574 686f 722d 656d 6169 6c3a 2068  .Author-email: h
-00000080: 6172 7279 2e64 6f77 6e69 6e67 3137 4067  arry.downing17@g
-00000090: 6d61 696c 2e63 6f6d 0d0a 4c69 6365 6e73  mail.com..Licens
-000000a0: 653a 204d 4954 0d0a 5072 6f6a 6563 742d  e: MIT..Project-
-000000b0: 5552 4c3a 2052 6570 6f73 6974 6f72 792c  URL: Repository,
-000000c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000d0: 636f 6d2f 6861 7272 7964 6f77 6e69 6e67  com/harrydowning
-000000e0: 2f73 6572 6c0d 0a50 726f 6a65 6374 2d55  /serl..Project-U
-000000f0: 524c 3a20 446f 6375 6d65 6e74 6174 696f  RL: Documentatio
-00000100: 6e2c 2068 7474 7073 3a2f 2f73 6572 6c2e  n, https://serl.
-00000110: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000120: 6e2f 6c61 7465 7374 2f69 6e64 6578 2e68  n/latest/index.h
-00000130: 746d 6c0d 0a43 6c61 7373 6966 6965 723a  tml..Classifier:
-00000140: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000150: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000160: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
-00000170: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000180: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000190: 204c 6963 656e 7365 0d0a 436c 6173 7369   License..Classi
-000001a0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-000001b0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001c0: 6570 656e 6465 6e74 0d0a 5265 7175 6972  ependent..Requir
-000001d0: 6573 2d50 7974 686f 6e3a 203e 3d33 2e31  es-Python: >=3.1
-000001e0: 310d 0a44 6573 6372 6970 7469 6f6e 2d43  1..Description-C
-000001f0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000200: 742f 6d61 726b 646f 776e 0d0a 4c69 6365  t/markdown..Lice
-00000210: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-00000220: 450d 0a0d 0a23 2053 6572 6961 6c69 7a65  E....# Serialize
-00000230: 6420 4c61 6e67 7561 6765 2028 7365 726c  d Language (serl
-00000240: 290d 0a53 6572 6c20 6973 2061 2063 6f6d  )..Serl is a com
-00000250: 6d61 6e64 206c 696e 6520 746f 6f6c 2075  mand line tool u
-00000260: 7365 6420 746f 206d 616e 6167 6520 616e  sed to manage an
-00000270: 6420 6578 6563 7574 6520 7072 6f67 7261  d execute progra
-00000280: 6d6d 696e 6720 6c61 6e67 7561 6765 7320  mming languages 
-00000290: 7365 7269 616c 697a 6564 2077 6974 6820  serialized with 
-000002a0: 5941 4d4c 2e0d 0a0d 0a44 6f63 756d 656e  YAML.....Documen
-000002b0: 7461 7469 6f6e 2063 616e 2062 6520 666f  tation can be fo
-000002c0: 756e 6420 6f6e 205b 5265 6164 2054 6865  und on [Read The
-000002d0: 2044 6f63 735d 2868 7474 7073 3a2f 2f73   Docs](https://s
-000002e0: 6572 6c2e 7265 6164 7468 6564 6f63 732e  erl.readthedocs.
-000002f0: 696f 2f65 6e2f 6c61 7465 7374 2f69 6e64  io/en/latest/ind
-00000300: 6578 2e68 746d 6c29 2e0d 0a0d 0a23 2323  ex.html).....###
-00000310: 2044 6576 656c 6f70 6d65 6e74 2057 6f72   Development Wor
-00000320: 6b66 6c6f 770d 0a7c 2043 6f6d 6d61 6e64  kflow..| Command
-00000330: 207c 2044 6573 6372 6970 7469 6f6e 207c   | Description |
-00000340: 0d0a 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ..| ------- | --
-00000350: 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 2060  --------- |..| `
-00000360: 7069 7020 696e 7374 616c 6c20 2e60 207c  pip install .` |
-00000370: 2042 7569 6c64 2f69 6e73 7461 6c6c 206c   Build/install l
-00000380: 6f63 616c 6c79 207c 0d0a 7c20 6073 6572  ocally |..| `ser
-00000390: 6c20 6865 6c70 6020 7c20 5368 6f77 2074  l help` | Show t
-000003a0: 6865 2074 6f6f 6c20 636f 6d6d 616e 6420  he tool command 
-000003b0: 6c69 6e65 2068 656c 7020 7363 7265 656e  line help screen
-000003c0: 207c 0d0a 7c20 6070 7974 6573 7420 7465   |..| `pytest te
-000003d0: 7374 7360 206f 7220 6074 6573 742e 6261  sts` or `test.ba
-000003e0: 7460 207c 2052 756e 2061 7574 6f6d 6174  t` | Run automat
-000003f0: 6564 2074 6573 7420 7375 6974 6520 7c0d  ed test suite |.
-00000400: 0a7c 2060 7079 202d 6d20 6275 696c 6460  .| `py -m build`
-00000410: 207c 2042 7569 6c64 2064 6973 7472 6962   | Build distrib
-00000420: 7574 696f 6e20 7c0d 0a7c 2060 7079 202d  ution |..| `py -
-00000430: 6d20 7477 696e 6520 7570 6c6f 6164 2064  m twine upload d
-00000440: 6973 742f 2a60 207c 2055 706c 6f61 6420  ist/*` | Upload 
-00000450: 6469 7374 7269 6275 7469 6f6e 207c 0d0a  distribution |..
-00000460: 7c20 6073 7068 696e 782d 6275 696c 6420  | `sphinx-build 
-00000470: 2d62 2068 746d 6c20 646f 6373 2f73 6f75  -b html docs/sou
-00000480: 7263 652f 2064 6f63 732f 6275 696c 642f  rce/ docs/build/
-00000490: 6874 6d6c 6020 7c20 4275 696c 6420 646f  html` | Build do
-000004a0: 6375 6d65 6e74 6174 696f 6e20 7c0d 0a0d  cumentation |...
-000004b0: 0a0d 0a4d 4954 204c 6963 656e 7365 0d0a  ...MIT License..
-000004c0: 0d0a 436f 7079 7269 6768 7420 2863 2920  ..Copyright (c) 
-000004d0: 3230 3233 2048 6172 7279 2044 6f77 6e69  2023 Harry Downi
-000004e0: 6e67 0d0a 0d0a 5065 726d 6973 7369 6f6e  ng....Permission
-000004f0: 2069 7320 6865 7265 6279 2067 7261 6e74   is hereby grant
-00000500: 6564 2c20 6672 6565 206f 6620 6368 6172  ed, free of char
-00000510: 6765 2c20 746f 2061 6e79 2070 6572 736f  ge, to any perso
-00000520: 6e20 6f62 7461 696e 696e 6720 6120 636f  n obtaining a co
-00000530: 7079 0d0a 6f66 2074 6869 7320 736f 6674  py..of this soft
-00000540: 7761 7265 2061 6e64 2061 7373 6f63 6961  ware and associa
-00000550: 7465 6420 646f 6375 6d65 6e74 6174 696f  ted documentatio
-00000560: 6e20 6669 6c65 7320 2874 6865 2022 536f  n files (the "So
-00000570: 6674 7761 7265 2229 2c20 746f 2064 6561  ftware"), to dea
-00000580: 6c0d 0a69 6e20 7468 6520 536f 6674 7761  l..in the Softwa
-00000590: 7265 2077 6974 686f 7574 2072 6573 7472  re without restr
-000005a0: 6963 7469 6f6e 2c20 696e 636c 7564 696e  iction, includin
-000005b0: 6720 7769 7468 6f75 7420 6c69 6d69 7461  g without limita
-000005c0: 7469 6f6e 2074 6865 2072 6967 6874 730d  tion the rights.
-000005d0: 0a74 6f20 7573 652c 2063 6f70 792c 206d  .to use, copy, m
-000005e0: 6f64 6966 792c 206d 6572 6765 2c20 7075  odify, merge, pu
-000005f0: 626c 6973 682c 2064 6973 7472 6962 7574  blish, distribut
-00000600: 652c 2073 7562 6c69 6365 6e73 652c 2061  e, sublicense, a
-00000610: 6e64 2f6f 7220 7365 6c6c 0d0a 636f 7069  nd/or sell..copi
-00000620: 6573 206f 6620 7468 6520 536f 6674 7761  es of the Softwa
-00000630: 7265 2c20 616e 6420 746f 2070 6572 6d69  re, and to permi
-00000640: 7420 7065 7273 6f6e 7320 746f 2077 686f  t persons to who
-00000650: 6d20 7468 6520 536f 6674 7761 7265 2069  m the Software i
-00000660: 730d 0a66 7572 6e69 7368 6564 2074 6f20  s..furnished to 
-00000670: 646f 2073 6f2c 2073 7562 6a65 6374 2074  do so, subject t
-00000680: 6f20 7468 6520 666f 6c6c 6f77 696e 6720  o the following 
-00000690: 636f 6e64 6974 696f 6e73 3a0d 0a0d 0a54  conditions:....T
-000006a0: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
-000006b0: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
-000006c0: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
-000006d0: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
-000006e0: 636c 7564 6564 2069 6e20 616c 6c0d 0a63  cluded in all..c
-000006f0: 6f70 6965 7320 6f72 2073 7562 7374 616e  opies or substan
-00000700: 7469 616c 2070 6f72 7469 6f6e 7320 6f66  tial portions of
-00000710: 2074 6865 2053 6f66 7477 6172 652e 0d0a   the Software...
-00000720: 0d0a 5448 4520 534f 4654 5741 5245 2049  ..THE SOFTWARE I
-00000730: 5320 5052 4f56 4944 4544 2022 4153 2049  S PROVIDED "AS I
-00000740: 5322 2c20 5749 5448 4f55 5420 5741 5252  S", WITHOUT WARR
-00000750: 414e 5459 204f 4620 414e 5920 4b49 4e44  ANTY OF ANY KIND
-00000760: 2c20 4558 5052 4553 5320 4f52 0d0a 494d  , EXPRESS OR..IM
-00000770: 504c 4945 442c 2049 4e43 4c55 4449 4e47  PLIED, INCLUDING
-00000780: 2042 5554 204e 4f54 204c 494d 4954 4544   BUT NOT LIMITED
-00000790: 2054 4f20 5448 4520 5741 5252 414e 5449   TO THE WARRANTI
-000007a0: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
-000007b0: 494c 4954 592c 0d0a 4649 544e 4553 5320  ILITY,..FITNESS 
-000007c0: 464f 5220 4120 5041 5254 4943 554c 4152  FOR A PARTICULAR
-000007d0: 2050 5552 504f 5345 2041 4e44 204e 4f4e   PURPOSE AND NON
-000007e0: 494e 4652 494e 4745 4d45 4e54 2e20 494e  INFRINGEMENT. IN
-000007f0: 204e 4f20 4556 454e 5420 5348 414c 4c20   NO EVENT SHALL 
-00000800: 5448 450d 0a41 5554 484f 5253 204f 5220  THE..AUTHORS OR 
-00000810: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
-00000820: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
-00000830: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
-00000840: 4553 204f 5220 4f54 4845 520d 0a4c 4941  ES OR OTHER..LIA
-00000850: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
-00000860: 494e 2041 4e20 4143 5449 4f4e 204f 4620  IN AN ACTION OF 
-00000870: 434f 4e54 5241 4354 2c20 544f 5254 204f  CONTRACT, TORT O
-00000880: 5220 4f54 4845 5257 4953 452c 2041 5249  R OTHERWISE, ARI
-00000890: 5349 4e47 2046 524f 4d2c 0d0a 4f55 5420  SING FROM,..OUT 
-000008a0: 4f46 204f 5220 494e 2043 4f4e 4e45 4354  OF OR IN CONNECT
-000008b0: 494f 4e20 5749 5448 2054 4845 2053 4f46  ION WITH THE SOF
-000008c0: 5457 4152 4520 4f52 2054 4845 2055 5345  TWARE OR THE USE
-000008d0: 204f 5220 4f54 4845 5220 4445 414c 494e   OR OTHER DEALIN
-000008e0: 4753 2049 4e20 5448 450d 0a53 4f46 5457  GS IN THE..SOFTW
-000008f0: 4152 452e 0d0a                           ARE...
+00000020: 6c0d 0a56 6572 7369 6f6e 3a20 302e 332e  l..Version: 0.3.
+00000030: 3062 300d 0a53 756d 6d61 7279 3a20 5365  0b0..Summary: Se
+00000040: 726c 202d 2041 2074 6f6f 6c20 666f 7220  rl - A tool for 
+00000050: 6372 6561 7469 6e67 2061 6e64 2075 7369  creating and usi
+00000060: 6e67 206c 616e 6775 6167 6573 0d0a 4175  ng languages..Au
+00000070: 7468 6f72 3a20 4861 7272 7920 446f 776e  thor: Harry Down
+00000080: 696e 670d 0a41 7574 686f 722d 656d 6169  ing..Author-emai
+00000090: 6c3a 2068 6172 7279 2e64 6f77 6e69 6e67  l: harry.downing
+000000a0: 3137 4067 6d61 696c 2e63 6f6d 0d0a 4c69  17@gmail.com..Li
+000000b0: 6365 6e73 653a 204d 4954 0d0a 5072 6f6a  cense: MIT..Proj
+000000c0: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
+000000d0: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
+000000e0: 6875 622e 636f 6d2f 6861 7272 7964 6f77  hub.com/harrydow
+000000f0: 6e69 6e67 2f73 6572 6c0d 0a50 726f 6a65  ning/serl..Proje
+00000100: 6374 2d55 524c 3a20 446f 6375 6d65 6e74  ct-URL: Document
+00000110: 6174 696f 6e2c 2068 7474 7073 3a2f 2f73  ation, https://s
+00000120: 6572 6c2e 7265 6164 7468 6564 6f63 732e  erl.readthedocs.
+00000130: 696f 2f65 6e2f 6c61 7465 7374 2f69 6e64  io/en/latest/ind
+00000140: 6578 2e68 746d 6c0d 0a43 6c61 7373 6966  ex.html..Classif
+00000150: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000160: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000170: 686f 6e20 3a3a 2033 0d0a 436c 6173 7369  hon :: 3..Classi
+00000180: 6669 6572 3a20 4c69 6365 6e73 6520 3a3a  fier: License ::
+00000190: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001a0: 204d 4954 204c 6963 656e 7365 0d0a 436c   MIT License..Cl
+000001b0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000001c0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000001d0: 2049 6e64 6570 656e 6465 6e74 0d0a 5265   Independent..Re
+000001e0: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+000001f0: 3d33 2e31 310d 0a44 6573 6372 6970 7469  =3.11..Descripti
+00000200: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000210: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+00000220: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000230: 4345 4e53 450d 0a0d 0a23 2053 6572 6c20  CENSE....# Serl 
+00000240: 2d20 4120 746f 6f6c 2066 6f72 2063 7265  - A tool for cre
+00000250: 6174 696e 6720 616e 6420 7573 696e 6720  ating and using 
+00000260: 6c61 6e67 7561 6765 730d 0a3c 6120 6872  languages..<a hr
+00000270: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000280: 2e6f 7267 2f70 726f 6a65 6374 2f73 6572  .org/project/ser
+00000290: 6c2f 223e 0d0a 2020 3c69 6d67 2073 7263  l/">..  <img src
+000002a0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000002b0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+000002c0: 7365 726c 222f 3e0d 0a3c 2f61 3e0d 0a3c  serl"/>..</a>..<
+000002d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000002e0: 6769 7468 7562 2e63 6f6d 2f68 6172 7279  github.com/harry
+000002f0: 646f 776e 696e 672f 7365 726c 2f62 6c6f  downing/serl/blo
+00000300: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
+00000310: 223e 0d0a 2020 3c69 6d67 2073 7263 3d22  ">..  <img src="
+00000320: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000330: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
+00000340: 6365 6e73 652f 6861 7272 7964 6f77 6e69  cense/harrydowni
+00000350: 6e67 2f73 6572 6c22 2f3e 0d0a 3c2f 613e  ng/serl"/>..</a>
+00000360: 0d0a 0d0a 5365 726c 2028 7365 7269 616c  ....Serl (serial
+00000370: 697a 6564 206c 616e 6775 6167 6573 2920  ized languages) 
+00000380: 6973 2061 2066 6f72 6d61 7420 616e 6420  is a format and 
+00000390: 636f 7272 6573 706f 6e64 696e 6720 636f  corresponding co
+000003a0: 6d6d 616e 6420 6c69 6e65 2074 6f6f 6c20  mmand line tool 
+000003b0: 666f 7220 6372 6561 7469 6e67 2061 6e64  for creating and
+000003c0: 2075 7369 6e67 2074 6578 7475 616c 2064   using textual d
+000003d0: 6f6d 6169 6e20 7370 6563 6966 6963 206f  omain specific o
+000003e0: 7220 6d61 726b 7570 206c 616e 6775 6167  r markup languag
+000003f0: 6573 2077 6974 6820 6172 6269 7472 6172  es with arbitrar
+00000400: 7920 7379 6e74 6178 2e20 5468 6973 2069  y syntax. This i
+00000410: 7320 6163 6869 6576 6564 2074 6872 6f75  s achieved throu
+00000420: 6768 2074 6865 2063 6f6e 6365 7074 206f  gh the concept o
+00000430: 6620 6c61 6e67 7561 6765 2063 6f6e 6669  f language confi
+00000440: 6775 7261 7469 6f6e 732c 2077 6869 6368  gurations, which
+00000450: 2061 7265 2059 414d 4c20 6669 6c65 7320   are YAML files 
+00000460: 666f 7220 7370 6563 6966 7969 6e67 206c  for specifying l
+00000470: 616e 6775 6167 6520 7379 6e74 6178 2061  anguage syntax a
+00000480: 6e64 2066 756e 6374 696f 6e61 6c69 7479  nd functionality
+00000490: 2c20 7573 6564 2062 7920 7468 6520 746f  , used by the to
+000004a0: 6f6c 2074 6f20 6578 6563 7574 6520 6c61  ol to execute la
+000004b0: 6e67 7561 6765 2070 726f 6772 616d 732e  nguage programs.
+000004c0: 2054 6865 7365 2063 6f6e 6669 6775 7261   These configura
+000004d0: 7469 6f6e 7320 6361 6e20 7468 656e 2062  tions can then b
+000004e0: 6520 6c69 6e6b 6564 2c20 616c 6c6f 7769  e linked, allowi
+000004f0: 6e67 206c 616e 6775 6167 6573 2074 6f20  ng languages to 
+00000500: 6265 2075 7365 6420 6c69 6b65 2061 6e79  be used like any
+00000510: 206f 7468 6572 2063 6f6d 6d61 6e64 206c   other command l
+00000520: 696e 6520 746f 6f6c 2e0d 0a0d 0a44 6f63  ine tool.....Doc
+00000530: 756d 656e 7461 7469 6f6e 2063 616e 2062  umentation can b
+00000540: 6520 666f 756e 6420 6f6e 205b 5265 6164  e found on [Read
+00000550: 2054 6865 2044 6f63 735d 2868 7474 7073   The Docs](https
+00000560: 3a2f 2f73 6572 6c2e 7265 6164 7468 6564  ://serl.readthed
+00000570: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000580: 2f69 6e64 6578 2e68 746d 6c29 2e0d 0a0d  /index.html)....
+00000590: 0a23 2323 2044 6576 656c 6f70 6d65 6e74  .### Development
+000005a0: 2057 6f72 6b66 6c6f 770d 0a7c 2043 6f6d   Workflow..| Com
+000005b0: 6d61 6e64 207c 2044 6573 6372 6970 7469  mand | Descripti
+000005c0: 6f6e 207c 0d0a 7c20 2d2d 2d2d 2d2d 2d20  on |..| ------- 
+000005d0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d  | ----------- |.
+000005e0: 0a7c 2060 7069 7020 696e 7374 616c 6c20  .| `pip install 
+000005f0: 2e60 207c 2042 7569 6c64 2f69 6e73 7461  .` | Build/insta
+00000600: 6c6c 206c 6f63 616c 6c79 207c 0d0a 7c20  ll locally |..| 
+00000610: 6073 6572 6c20 6865 6c70 6020 7c20 5368  `serl help` | Sh
+00000620: 6f77 2074 6865 2074 6f6f 6c20 636f 6d6d  ow the tool comm
+00000630: 616e 6420 6c69 6e65 2068 656c 7020 7363  and line help sc
+00000640: 7265 656e 207c 0d0a 7c20 6070 7974 6573  reen |..| `pytes
+00000650: 7420 7465 7374 7360 206f 7220 6074 6573  t tests` or `tes
+00000660: 742e 6261 7460 207c 2052 756e 2061 7574  t.bat` | Run aut
+00000670: 6f6d 6174 6564 2074 6573 7420 7375 6974  omated test suit
+00000680: 6520 7c0d 0a7c 2060 7079 202d 6d20 6275  e |..| `py -m bu
+00000690: 696c 6460 207c 2042 7569 6c64 2064 6973  ild` | Build dis
+000006a0: 7472 6962 7574 696f 6e20 7c0d 0a7c 2060  tribution |..| `
+000006b0: 7079 202d 6d20 7477 696e 6520 7570 6c6f  py -m twine uplo
+000006c0: 6164 2064 6973 742f 2a60 207c 2055 706c  ad dist/*` | Upl
+000006d0: 6f61 6420 6469 7374 7269 6275 7469 6f6e  oad distribution
+000006e0: 207c 0d0a 7c20 6073 7068 696e 782d 6275   |..| `sphinx-bu
+000006f0: 696c 6420 2d62 2068 746d 6c20 646f 6373  ild -b html docs
+00000700: 2f73 6f75 7263 652f 2064 6f63 732f 6275  /source/ docs/bu
+00000710: 696c 642f 6874 6d6c 6020 7c20 4275 696c  ild/html` | Buil
+00000720: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
+00000730: 7c0d 0a0d 0a0d 0a4d 4954 204c 6963 656e  |......MIT Licen
+00000740: 7365 0d0a 0d0a 436f 7079 7269 6768 7420  se....Copyright 
+00000750: 2863 2920 3230 3233 2048 6172 7279 2044  (c) 2023 Harry D
+00000760: 6f77 6e69 6e67 0d0a 0d0a 5065 726d 6973  owning....Permis
+00000770: 7369 6f6e 2069 7320 6865 7265 6279 2067  sion is hereby g
+00000780: 7261 6e74 6564 2c20 6672 6565 206f 6620  ranted, free of 
+00000790: 6368 6172 6765 2c20 746f 2061 6e79 2070  charge, to any p
+000007a0: 6572 736f 6e20 6f62 7461 696e 696e 6720  erson obtaining 
+000007b0: 6120 636f 7079 0d0a 6f66 2074 6869 7320  a copy..of this 
+000007c0: 736f 6674 7761 7265 2061 6e64 2061 7373  software and ass
+000007d0: 6f63 6961 7465 6420 646f 6375 6d65 6e74  ociated document
+000007e0: 6174 696f 6e20 6669 6c65 7320 2874 6865  ation files (the
+000007f0: 2022 536f 6674 7761 7265 2229 2c20 746f   "Software"), to
+00000800: 2064 6561 6c0d 0a69 6e20 7468 6520 536f   deal..in the So
+00000810: 6674 7761 7265 2077 6974 686f 7574 2072  ftware without r
+00000820: 6573 7472 6963 7469 6f6e 2c20 696e 636c  estriction, incl
+00000830: 7564 696e 6720 7769 7468 6f75 7420 6c69  uding without li
+00000840: 6d69 7461 7469 6f6e 2074 6865 2072 6967  mitation the rig
+00000850: 6874 730d 0a74 6f20 7573 652c 2063 6f70  hts..to use, cop
+00000860: 792c 206d 6f64 6966 792c 206d 6572 6765  y, modify, merge
+00000870: 2c20 7075 626c 6973 682c 2064 6973 7472  , publish, distr
+00000880: 6962 7574 652c 2073 7562 6c69 6365 6e73  ibute, sublicens
+00000890: 652c 2061 6e64 2f6f 7220 7365 6c6c 0d0a  e, and/or sell..
+000008a0: 636f 7069 6573 206f 6620 7468 6520 536f  copies of the So
+000008b0: 6674 7761 7265 2c20 616e 6420 746f 2070  ftware, and to p
+000008c0: 6572 6d69 7420 7065 7273 6f6e 7320 746f  ermit persons to
+000008d0: 2077 686f 6d20 7468 6520 536f 6674 7761   whom the Softwa
+000008e0: 7265 2069 730d 0a66 7572 6e69 7368 6564  re is..furnished
+000008f0: 2074 6f20 646f 2073 6f2c 2073 7562 6a65   to do so, subje
+00000900: 6374 2074 6f20 7468 6520 666f 6c6c 6f77  ct to the follow
+00000910: 696e 6720 636f 6e64 6974 696f 6e73 3a0d  ing conditions:.
+00000920: 0a0d 0a54 6865 2061 626f 7665 2063 6f70  ...The above cop
+00000930: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
+00000940: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
+00000950: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
+00000960: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
+00000970: 6c0d 0a63 6f70 6965 7320 6f72 2073 7562  l..copies or sub
+00000980: 7374 616e 7469 616c 2070 6f72 7469 6f6e  stantial portion
+00000990: 7320 6f66 2074 6865 2053 6f66 7477 6172  s of the Softwar
+000009a0: 652e 0d0a 0d0a 5448 4520 534f 4654 5741  e.....THE SOFTWA
+000009b0: 5245 2049 5320 5052 4f56 4944 4544 2022  RE IS PROVIDED "
+000009c0: 4153 2049 5322 2c20 5749 5448 4f55 5420  AS IS", WITHOUT 
+000009d0: 5741 5252 414e 5459 204f 4620 414e 5920  WARRANTY OF ANY 
+000009e0: 4b49 4e44 2c20 4558 5052 4553 5320 4f52  KIND, EXPRESS OR
+000009f0: 0d0a 494d 504c 4945 442c 2049 4e43 4c55  ..IMPLIED, INCLU
+00000a00: 4449 4e47 2042 5554 204e 4f54 204c 494d  DING BUT NOT LIM
+00000a10: 4954 4544 2054 4f20 5448 4520 5741 5252  ITED TO THE WARR
+00000a20: 414e 5449 4553 204f 4620 4d45 5243 4841  ANTIES OF MERCHA
+00000a30: 4e54 4142 494c 4954 592c 0d0a 4649 544e  NTABILITY,..FITN
+00000a40: 4553 5320 464f 5220 4120 5041 5254 4943  ESS FOR A PARTIC
+00000a50: 554c 4152 2050 5552 504f 5345 2041 4e44  ULAR PURPOSE AND
+00000a60: 204e 4f4e 494e 4652 494e 4745 4d45 4e54   NONINFRINGEMENT
+00000a70: 2e20 494e 204e 4f20 4556 454e 5420 5348  . IN NO EVENT SH
+00000a80: 414c 4c20 5448 450d 0a41 5554 484f 5253  ALL THE..AUTHORS
+00000a90: 204f 5220 434f 5059 5249 4748 5420 484f   OR COPYRIGHT HO
+00000aa0: 4c44 4552 5320 4245 204c 4941 424c 4520  LDERS BE LIABLE 
+00000ab0: 464f 5220 414e 5920 434c 4149 4d2c 2044  FOR ANY CLAIM, D
+00000ac0: 414d 4147 4553 204f 5220 4f54 4845 520d  AMAGES OR OTHER.
+00000ad0: 0a4c 4941 4249 4c49 5459 2c20 5748 4554  .LIABILITY, WHET
+00000ae0: 4845 5220 494e 2041 4e20 4143 5449 4f4e  HER IN AN ACTION
+00000af0: 204f 4620 434f 4e54 5241 4354 2c20 544f   OF CONTRACT, TO
+00000b00: 5254 204f 5220 4f54 4845 5257 4953 452c  RT OR OTHERWISE,
+00000b10: 2041 5249 5349 4e47 2046 524f 4d2c 0d0a   ARISING FROM,..
+00000b20: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
+00000b30: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
+00000b40: 2053 4f46 5457 4152 4520 4f52 2054 4845   SOFTWARE OR THE
+00000b50: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
+00000b60: 414c 494e 4753 2049 4e20 5448 450d 0a53  ALINGS IN THE..S
+00000b70: 4f46 5457 4152 452e 0d0a                 OFTWARE...
```

### Comparing `serl-0.2.2b0/setup.cfg` & `serl-0.3.0b0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -3,55 +3,56 @@
 00000020: 203d 2061 7474 723a 2073 6572 6c2e 636f   = attr: serl.co
 00000030: 6e73 7461 6e74 732e 5645 5253 494f 4e0d  nstants.VERSION.
 00000040: 0a61 7574 686f 7220 3d20 4861 7272 7920  .author = Harry 
 00000050: 446f 776e 696e 670d 0a61 7574 686f 725f  Downing..author_
 00000060: 656d 6169 6c20 3d20 6861 7272 792e 646f  email = harry.do
 00000070: 776e 696e 6731 3740 676d 6169 6c2e 636f  wning17@gmail.co
 00000080: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
-00000090: 2053 6572 6961 6c69 7a65 6420 4c61 6e67   Serialized Lang
-000000a0: 7561 6765 2028 7365 726c 290d 0a6c 6f6e  uage (serl)..lon
-000000b0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-000000c0: 6669 6c65 3a20 5245 4144 4d45 2e6d 642c  file: README.md,
-000000d0: 204c 4943 454e 5345 0d0a 6c6f 6e67 5f64   LICENSE..long_d
-000000e0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-000000f0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-00000100: 6172 6b64 6f77 6e0d 0a6c 6963 656e 7365  arkdown..license
-00000110: 203d 204d 4954 0d0a 7072 6f6a 6563 745f   = MIT..project_
-00000120: 7572 6c73 203d 200d 0a09 5265 706f 7369  urls = ...Reposi
-00000130: 746f 7279 203d 2068 7474 7073 3a2f 2f67  tory = https://g
-00000140: 6974 6875 622e 636f 6d2f 6861 7272 7964  ithub.com/harryd
-00000150: 6f77 6e69 6e67 2f73 6572 6c0d 0a09 446f  owning/serl...Do
-00000160: 6375 6d65 6e74 6174 696f 6e20 3d20 6874  cumentation = ht
-00000170: 7470 733a 2f2f 7365 726c 2e72 6561 6474  tps://serl.readt
-00000180: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000190: 6573 742f 696e 6465 782e 6874 6d6c 0d0a  est/index.html..
-000001a0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001b0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001d0: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
-000001e0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000001f0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-00000200: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000210: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000220: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000230: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000240: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
-00000250: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000260: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000270: 2e31 310d 0a69 6e73 7461 6c6c 5f72 6571  .11..install_req
-00000280: 7569 7265 7320 3d20 0d0a 0950 7959 414d  uires = ...PyYAM
-00000290: 4c0d 0a09 646f 636f 7074 0d0a 0970 6c79  L...docopt...ply
-000002a0: 3d3d 332e 3131 0d0a 0972 6567 6578 0d0a  ==3.11...regex..
-000002b0: 096e 6574 776f 726b 780d 0a09 6a73 6f6e  .networkx...json
-000002c0: 7363 6865 6d61 0d0a 0950 7967 6d65 6e74  schema...Pygment
-000002d0: 730d 0a09 5069 6c6c 6f77 0d0a 0972 6571  s...Pillow...req
-000002e0: 7565 7374 730d 0a0d 0a5b 6f70 7469 6f6e  uests....[option
-000002f0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000300: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000310: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-00000320: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
-00000330: 5f73 6372 6970 7473 203d 200d 0a09 7365  _scripts = ...se
-00000340: 726c 203d 2073 6572 6c2e 6d61 696e 3a6d  rl = serl.main:m
-00000350: 6169 6e0d 0a0d 0a5b 6567 675f 696e 666f  ain....[egg_info
-00000360: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000370: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000380: 0a                                       .
+00000090: 2053 6572 6c20 2d20 4120 746f 6f6c 2066   Serl - A tool f
+000000a0: 6f72 2063 7265 6174 696e 6720 616e 6420  or creating and 
+000000b0: 7573 696e 6720 6c61 6e67 7561 6765 730d  using languages.
+000000c0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000d0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000e0: 2e6d 642c 204c 4943 454e 5345 0d0a 6c6f  .md, LICENSE..lo
+000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+00000100: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000110: 7874 2f6d 6172 6b64 6f77 6e0d 0a6c 6963  xt/markdown..lic
+00000120: 656e 7365 203d 204d 4954 0d0a 7072 6f6a  ense = MIT..proj
+00000130: 6563 745f 7572 6c73 203d 200d 0a09 5265  ect_urls = ...Re
+00000140: 706f 7369 746f 7279 203d 2068 7474 7073  pository = https
+00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 6861  ://github.com/ha
+00000160: 7272 7964 6f77 6e69 6e67 2f73 6572 6c0d  rrydowning/serl.
+00000170: 0a09 446f 6375 6d65 6e74 6174 696f 6e20  ..Documentation 
+00000180: 3d20 6874 7470 733a 2f2f 7365 726c 2e72  = https://serl.r
+00000190: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+000001a0: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
+000001b0: 6d6c 0d0a 636c 6173 7369 6669 6572 7320  ml..classifiers 
+000001c0: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
+000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001e0: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
+000001f0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000200: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000210: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+00000220: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000230: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
+00000240: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+00000250: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
+00000260: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+00000270: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000280: 203e 3d33 2e31 310d 0a69 6e73 7461 6c6c   >=3.11..install
+00000290: 5f72 6571 7569 7265 7320 3d20 0d0a 0950  _requires = ...P
+000002a0: 7959 414d 4c0d 0a09 646f 636f 7074 0d0a  yYAML...docopt..
+000002b0: 0970 6c79 3d3d 332e 3131 0d0a 0972 6567  .ply==3.11...reg
+000002c0: 6578 0d0a 096e 6574 776f 726b 780d 0a09  ex...networkx...
+000002d0: 6a73 6f6e 7363 6865 6d61 0d0a 0950 7967  jsonschema...Pyg
+000002e0: 6d65 6e74 730d 0a09 5069 6c6c 6f77 0d0a  ments...Pillow..
+000002f0: 0972 6571 7565 7374 730d 0a0d 0a5b 6f70  .requests....[op
+00000300: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000310: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000320: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  c....[options.en
+00000330: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+00000340: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+00000350: 0a09 7365 726c 203d 2073 6572 6c2e 6d61  ..serl = serl.ma
+00000360: 696e 3a6d 6169 6e0d 0a0d 0a5b 6567 675f  in:main....[egg_
+00000370: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000380: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000390: 300d 0a0d 0a                             0....
```

### Comparing `serl-0.2.2b0/src/serl/config.py` & `serl-0.3.0b0/src/serl/config.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/src/serl/constants.py` & `serl-0.3.0b0/src/serl/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 NAME = __package__
-VERSION = '0.2.2-beta'
+VERSION = '0.3.0-beta'
 
 SYSTEM_CONFIG_DIR = f'.{NAME}'
 SYSTEM_CONFIG_ENV_DIR = 'environments'
 SHELL_CHAR = '$'
 VENV_CONFIG = 'pyvenv.cfg'
 EXCEPTION_ATTR = 'serl_loc'
 
@@ -18,14 +18,15 @@
     {NAME} [options] <command> [<args>...]
 
 Commands:
     link       Create a language symbolic link.
     install    install language to {SYSTEM_CONFIG_DIR} in home directory.
     uninstall  Uninstall language from {SYSTEM_CONFIG_DIR} in home directory.
     list       list installed languages.
+    show       Display language.
     run        Execute language.
     help       Show help for commands.
 
 {OPTIONS}"""
 
 CLI_LINK = f"""{NAME} link
 
@@ -58,14 +59,24 @@
     list [options]
 
 List Options:
     --venv  List installed virtual environments.
 
 {OPTIONS}"""
 
+CLI_SHOW = f"""{NAME} show
+
+Usage:
+    show [options] <language>
+
+Show Options:
+    -o, --output=FILE  Write language config to file.
+    
+{OPTIONS}"""
+
 RUN_OPTIONS = f"""Run Options:
     -r, --requirements            Install pip requirements.
     --debug-lexer                 Output tokens found line-by-line.
     --debug-parser=FILE           Create parser state file.
     -H, --highlight=FILE          Create highlighted version of <src> in the 
                                   format of the extension of FILE.
     -f, --format=FORMAT           Override file extension format.
@@ -100,14 +111,15 @@
     help [<command>]"""
 
 CLI_COMMANDS = {
     'link': CLI_LINK,
     'install': CLI_INSTALL,
     'uninstall': CLI_UNINSTALL,
     'list': CLI_LIST,
+    'show': CLI_SHOW,
     'run': CLI_RUN,
     'help': CLI_HELP
 }
 
 DEFAULT_REF = r'^token(?= )|(?<= )token(?= )|(?<= )token$'
 
 PLY_ERR_MSG = {
```

### Comparing `serl-0.2.2b0/src/serl/highlight.py` & `serl-0.3.0b0/src/serl/highlight.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/src/serl/lexer.py` & `serl-0.3.0b0/src/serl/lexer.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/src/serl/logger.py` & `serl-0.3.0b0/src/serl/logger.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/src/serl/main.py` & `serl-0.3.0b0/src/serl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,21 @@
         files, name = envs, 'environments'
     
     if files == []:
         print(f'No {name} installed.')
     else:
         print(*files, sep='\n')
 
+def command_line_show(args):
+    language = args['<language>']
+    config_text = get_config_text(language, get_link_filename())
+    filename = args['--output'] or 1
+    with open(filename, 'w') as file:
+      file.write(config_text)
+
 def get_symlink_args(filename, version) -> dict:
     # Stop initial args acting on the tool and not the language
     if not '--' in sys.argv:
         sys.argv.insert(1, '--')
     
     args = docopt(SYMLINK_CLI, version=version, options_first=True)
```

### Comparing `serl-0.2.2b0/src/serl/parser.py` & `serl-0.3.0b0/src/serl/parser.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/src/serl/schema.py` & `serl-0.3.0b0/src/serl/schema.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/src/serl/utils.py` & `serl-0.3.0b0/src/serl/utils.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/src/serl.egg-info/PKG-INFO` & `serl-0.3.0b0/src/serl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,144 +1,184 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2073 6572  : 2.1..Name: ser
-00000020: 6c0d 0a56 6572 7369 6f6e 3a20 302e 322e  l..Version: 0.2.
-00000030: 3262 300d 0a53 756d 6d61 7279 3a20 5365  2b0..Summary: Se
-00000040: 7269 616c 697a 6564 204c 616e 6775 6167  rialized Languag
-00000050: 6520 2873 6572 6c29 0d0a 4175 7468 6f72  e (serl)..Author
-00000060: 3a20 4861 7272 7920 446f 776e 696e 670d  : Harry Downing.
-00000070: 0a41 7574 686f 722d 656d 6169 6c3a 2068  .Author-email: h
-00000080: 6172 7279 2e64 6f77 6e69 6e67 3137 4067  arry.downing17@g
-00000090: 6d61 696c 2e63 6f6d 0d0a 4c69 6365 6e73  mail.com..Licens
-000000a0: 653a 204d 4954 0d0a 5072 6f6a 6563 742d  e: MIT..Project-
-000000b0: 5552 4c3a 2052 6570 6f73 6974 6f72 792c  URL: Repository,
-000000c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000d0: 636f 6d2f 6861 7272 7964 6f77 6e69 6e67  com/harrydowning
-000000e0: 2f73 6572 6c0d 0a50 726f 6a65 6374 2d55  /serl..Project-U
-000000f0: 524c 3a20 446f 6375 6d65 6e74 6174 696f  RL: Documentatio
-00000100: 6e2c 2068 7474 7073 3a2f 2f73 6572 6c2e  n, https://serl.
-00000110: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000120: 6e2f 6c61 7465 7374 2f69 6e64 6578 2e68  n/latest/index.h
-00000130: 746d 6c0d 0a43 6c61 7373 6966 6965 723a  tml..Classifier:
-00000140: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000150: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000160: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
-00000170: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000180: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000190: 204c 6963 656e 7365 0d0a 436c 6173 7369   License..Classi
-000001a0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-000001b0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001c0: 6570 656e 6465 6e74 0d0a 5265 7175 6972  ependent..Requir
-000001d0: 6573 2d50 7974 686f 6e3a 203e 3d33 2e31  es-Python: >=3.1
-000001e0: 310d 0a44 6573 6372 6970 7469 6f6e 2d43  1..Description-C
-000001f0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000200: 742f 6d61 726b 646f 776e 0d0a 4c69 6365  t/markdown..Lice
-00000210: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-00000220: 450d 0a0d 0a23 2053 6572 6961 6c69 7a65  E....# Serialize
-00000230: 6420 4c61 6e67 7561 6765 2028 7365 726c  d Language (serl
-00000240: 290d 0a53 6572 6c20 6973 2061 2063 6f6d  )..Serl is a com
-00000250: 6d61 6e64 206c 696e 6520 746f 6f6c 2075  mand line tool u
-00000260: 7365 6420 746f 206d 616e 6167 6520 616e  sed to manage an
-00000270: 6420 6578 6563 7574 6520 7072 6f67 7261  d execute progra
-00000280: 6d6d 696e 6720 6c61 6e67 7561 6765 7320  mming languages 
-00000290: 7365 7269 616c 697a 6564 2077 6974 6820  serialized with 
-000002a0: 5941 4d4c 2e0d 0a0d 0a44 6f63 756d 656e  YAML.....Documen
-000002b0: 7461 7469 6f6e 2063 616e 2062 6520 666f  tation can be fo
-000002c0: 756e 6420 6f6e 205b 5265 6164 2054 6865  und on [Read The
-000002d0: 2044 6f63 735d 2868 7474 7073 3a2f 2f73   Docs](https://s
-000002e0: 6572 6c2e 7265 6164 7468 6564 6f63 732e  erl.readthedocs.
-000002f0: 696f 2f65 6e2f 6c61 7465 7374 2f69 6e64  io/en/latest/ind
-00000300: 6578 2e68 746d 6c29 2e0d 0a0d 0a23 2323  ex.html).....###
-00000310: 2044 6576 656c 6f70 6d65 6e74 2057 6f72   Development Wor
-00000320: 6b66 6c6f 770d 0a7c 2043 6f6d 6d61 6e64  kflow..| Command
-00000330: 207c 2044 6573 6372 6970 7469 6f6e 207c   | Description |
-00000340: 0d0a 7c20 2d2d 2d2d 2d2d 2d20 7c20 2d2d  ..| ------- | --
-00000350: 2d2d 2d2d 2d2d 2d2d 2d20 7c0d 0a7c 2060  --------- |..| `
-00000360: 7069 7020 696e 7374 616c 6c20 2e60 207c  pip install .` |
-00000370: 2042 7569 6c64 2f69 6e73 7461 6c6c 206c   Build/install l
-00000380: 6f63 616c 6c79 207c 0d0a 7c20 6073 6572  ocally |..| `ser
-00000390: 6c20 6865 6c70 6020 7c20 5368 6f77 2074  l help` | Show t
-000003a0: 6865 2074 6f6f 6c20 636f 6d6d 616e 6420  he tool command 
-000003b0: 6c69 6e65 2068 656c 7020 7363 7265 656e  line help screen
-000003c0: 207c 0d0a 7c20 6070 7974 6573 7420 7465   |..| `pytest te
-000003d0: 7374 7360 206f 7220 6074 6573 742e 6261  sts` or `test.ba
-000003e0: 7460 207c 2052 756e 2061 7574 6f6d 6174  t` | Run automat
-000003f0: 6564 2074 6573 7420 7375 6974 6520 7c0d  ed test suite |.
-00000400: 0a7c 2060 7079 202d 6d20 6275 696c 6460  .| `py -m build`
-00000410: 207c 2042 7569 6c64 2064 6973 7472 6962   | Build distrib
-00000420: 7574 696f 6e20 7c0d 0a7c 2060 7079 202d  ution |..| `py -
-00000430: 6d20 7477 696e 6520 7570 6c6f 6164 2064  m twine upload d
-00000440: 6973 742f 2a60 207c 2055 706c 6f61 6420  ist/*` | Upload 
-00000450: 6469 7374 7269 6275 7469 6f6e 207c 0d0a  distribution |..
-00000460: 7c20 6073 7068 696e 782d 6275 696c 6420  | `sphinx-build 
-00000470: 2d62 2068 746d 6c20 646f 6373 2f73 6f75  -b html docs/sou
-00000480: 7263 652f 2064 6f63 732f 6275 696c 642f  rce/ docs/build/
-00000490: 6874 6d6c 6020 7c20 4275 696c 6420 646f  html` | Build do
-000004a0: 6375 6d65 6e74 6174 696f 6e20 7c0d 0a0d  cumentation |...
-000004b0: 0a0d 0a4d 4954 204c 6963 656e 7365 0d0a  ...MIT License..
-000004c0: 0d0a 436f 7079 7269 6768 7420 2863 2920  ..Copyright (c) 
-000004d0: 3230 3233 2048 6172 7279 2044 6f77 6e69  2023 Harry Downi
-000004e0: 6e67 0d0a 0d0a 5065 726d 6973 7369 6f6e  ng....Permission
-000004f0: 2069 7320 6865 7265 6279 2067 7261 6e74   is hereby grant
-00000500: 6564 2c20 6672 6565 206f 6620 6368 6172  ed, free of char
-00000510: 6765 2c20 746f 2061 6e79 2070 6572 736f  ge, to any perso
-00000520: 6e20 6f62 7461 696e 696e 6720 6120 636f  n obtaining a co
-00000530: 7079 0d0a 6f66 2074 6869 7320 736f 6674  py..of this soft
-00000540: 7761 7265 2061 6e64 2061 7373 6f63 6961  ware and associa
-00000550: 7465 6420 646f 6375 6d65 6e74 6174 696f  ted documentatio
-00000560: 6e20 6669 6c65 7320 2874 6865 2022 536f  n files (the "So
-00000570: 6674 7761 7265 2229 2c20 746f 2064 6561  ftware"), to dea
-00000580: 6c0d 0a69 6e20 7468 6520 536f 6674 7761  l..in the Softwa
-00000590: 7265 2077 6974 686f 7574 2072 6573 7472  re without restr
-000005a0: 6963 7469 6f6e 2c20 696e 636c 7564 696e  iction, includin
-000005b0: 6720 7769 7468 6f75 7420 6c69 6d69 7461  g without limita
-000005c0: 7469 6f6e 2074 6865 2072 6967 6874 730d  tion the rights.
-000005d0: 0a74 6f20 7573 652c 2063 6f70 792c 206d  .to use, copy, m
-000005e0: 6f64 6966 792c 206d 6572 6765 2c20 7075  odify, merge, pu
-000005f0: 626c 6973 682c 2064 6973 7472 6962 7574  blish, distribut
-00000600: 652c 2073 7562 6c69 6365 6e73 652c 2061  e, sublicense, a
-00000610: 6e64 2f6f 7220 7365 6c6c 0d0a 636f 7069  nd/or sell..copi
-00000620: 6573 206f 6620 7468 6520 536f 6674 7761  es of the Softwa
-00000630: 7265 2c20 616e 6420 746f 2070 6572 6d69  re, and to permi
-00000640: 7420 7065 7273 6f6e 7320 746f 2077 686f  t persons to who
-00000650: 6d20 7468 6520 536f 6674 7761 7265 2069  m the Software i
-00000660: 730d 0a66 7572 6e69 7368 6564 2074 6f20  s..furnished to 
-00000670: 646f 2073 6f2c 2073 7562 6a65 6374 2074  do so, subject t
-00000680: 6f20 7468 6520 666f 6c6c 6f77 696e 6720  o the following 
-00000690: 636f 6e64 6974 696f 6e73 3a0d 0a0d 0a54  conditions:....T
-000006a0: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
-000006b0: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
-000006c0: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
-000006d0: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
-000006e0: 636c 7564 6564 2069 6e20 616c 6c0d 0a63  cluded in all..c
-000006f0: 6f70 6965 7320 6f72 2073 7562 7374 616e  opies or substan
-00000700: 7469 616c 2070 6f72 7469 6f6e 7320 6f66  tial portions of
-00000710: 2074 6865 2053 6f66 7477 6172 652e 0d0a   the Software...
-00000720: 0d0a 5448 4520 534f 4654 5741 5245 2049  ..THE SOFTWARE I
-00000730: 5320 5052 4f56 4944 4544 2022 4153 2049  S PROVIDED "AS I
-00000740: 5322 2c20 5749 5448 4f55 5420 5741 5252  S", WITHOUT WARR
-00000750: 414e 5459 204f 4620 414e 5920 4b49 4e44  ANTY OF ANY KIND
-00000760: 2c20 4558 5052 4553 5320 4f52 0d0a 494d  , EXPRESS OR..IM
-00000770: 504c 4945 442c 2049 4e43 4c55 4449 4e47  PLIED, INCLUDING
-00000780: 2042 5554 204e 4f54 204c 494d 4954 4544   BUT NOT LIMITED
-00000790: 2054 4f20 5448 4520 5741 5252 414e 5449   TO THE WARRANTI
-000007a0: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
-000007b0: 494c 4954 592c 0d0a 4649 544e 4553 5320  ILITY,..FITNESS 
-000007c0: 464f 5220 4120 5041 5254 4943 554c 4152  FOR A PARTICULAR
-000007d0: 2050 5552 504f 5345 2041 4e44 204e 4f4e   PURPOSE AND NON
-000007e0: 494e 4652 494e 4745 4d45 4e54 2e20 494e  INFRINGEMENT. IN
-000007f0: 204e 4f20 4556 454e 5420 5348 414c 4c20   NO EVENT SHALL 
-00000800: 5448 450d 0a41 5554 484f 5253 204f 5220  THE..AUTHORS OR 
-00000810: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
-00000820: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
-00000830: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
-00000840: 4553 204f 5220 4f54 4845 520d 0a4c 4941  ES OR OTHER..LIA
-00000850: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
-00000860: 494e 2041 4e20 4143 5449 4f4e 204f 4620  IN AN ACTION OF 
-00000870: 434f 4e54 5241 4354 2c20 544f 5254 204f  CONTRACT, TORT O
-00000880: 5220 4f54 4845 5257 4953 452c 2041 5249  R OTHERWISE, ARI
-00000890: 5349 4e47 2046 524f 4d2c 0d0a 4f55 5420  SING FROM,..OUT 
-000008a0: 4f46 204f 5220 494e 2043 4f4e 4e45 4354  OF OR IN CONNECT
-000008b0: 494f 4e20 5749 5448 2054 4845 2053 4f46  ION WITH THE SOF
-000008c0: 5457 4152 4520 4f52 2054 4845 2055 5345  TWARE OR THE USE
-000008d0: 204f 5220 4f54 4845 5220 4445 414c 494e   OR OTHER DEALIN
-000008e0: 4753 2049 4e20 5448 450d 0a53 4f46 5457  GS IN THE..SOFTW
-000008f0: 4152 452e 0d0a                           ARE...
+00000020: 6c0d 0a56 6572 7369 6f6e 3a20 302e 332e  l..Version: 0.3.
+00000030: 3062 300d 0a53 756d 6d61 7279 3a20 5365  0b0..Summary: Se
+00000040: 726c 202d 2041 2074 6f6f 6c20 666f 7220  rl - A tool for 
+00000050: 6372 6561 7469 6e67 2061 6e64 2075 7369  creating and usi
+00000060: 6e67 206c 616e 6775 6167 6573 0d0a 4175  ng languages..Au
+00000070: 7468 6f72 3a20 4861 7272 7920 446f 776e  thor: Harry Down
+00000080: 696e 670d 0a41 7574 686f 722d 656d 6169  ing..Author-emai
+00000090: 6c3a 2068 6172 7279 2e64 6f77 6e69 6e67  l: harry.downing
+000000a0: 3137 4067 6d61 696c 2e63 6f6d 0d0a 4c69  17@gmail.com..Li
+000000b0: 6365 6e73 653a 204d 4954 0d0a 5072 6f6a  cense: MIT..Proj
+000000c0: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
+000000d0: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
+000000e0: 6875 622e 636f 6d2f 6861 7272 7964 6f77  hub.com/harrydow
+000000f0: 6e69 6e67 2f73 6572 6c0d 0a50 726f 6a65  ning/serl..Proje
+00000100: 6374 2d55 524c 3a20 446f 6375 6d65 6e74  ct-URL: Document
+00000110: 6174 696f 6e2c 2068 7474 7073 3a2f 2f73  ation, https://s
+00000120: 6572 6c2e 7265 6164 7468 6564 6f63 732e  erl.readthedocs.
+00000130: 696f 2f65 6e2f 6c61 7465 7374 2f69 6e64  io/en/latest/ind
+00000140: 6578 2e68 746d 6c0d 0a43 6c61 7373 6966  ex.html..Classif
+00000150: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000160: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000170: 686f 6e20 3a3a 2033 0d0a 436c 6173 7369  hon :: 3..Classi
+00000180: 6669 6572 3a20 4c69 6365 6e73 6520 3a3a  fier: License ::
+00000190: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001a0: 204d 4954 204c 6963 656e 7365 0d0a 436c   MIT License..Cl
+000001b0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000001c0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000001d0: 2049 6e64 6570 656e 6465 6e74 0d0a 5265   Independent..Re
+000001e0: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+000001f0: 3d33 2e31 310d 0a44 6573 6372 6970 7469  =3.11..Descripti
+00000200: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000210: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+00000220: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000230: 4345 4e53 450d 0a0d 0a23 2053 6572 6c20  CENSE....# Serl 
+00000240: 2d20 4120 746f 6f6c 2066 6f72 2063 7265  - A tool for cre
+00000250: 6174 696e 6720 616e 6420 7573 696e 6720  ating and using 
+00000260: 6c61 6e67 7561 6765 730d 0a3c 6120 6872  languages..<a hr
+00000270: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000280: 2e6f 7267 2f70 726f 6a65 6374 2f73 6572  .org/project/ser
+00000290: 6c2f 223e 0d0a 2020 3c69 6d67 2073 7263  l/">..  <img src
+000002a0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000002b0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+000002c0: 7365 726c 222f 3e0d 0a3c 2f61 3e0d 0a3c  serl"/>..</a>..<
+000002d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000002e0: 6769 7468 7562 2e63 6f6d 2f68 6172 7279  github.com/harry
+000002f0: 646f 776e 696e 672f 7365 726c 2f62 6c6f  downing/serl/blo
+00000300: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
+00000310: 223e 0d0a 2020 3c69 6d67 2073 7263 3d22  ">..  <img src="
+00000320: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000330: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
+00000340: 6365 6e73 652f 6861 7272 7964 6f77 6e69  cense/harrydowni
+00000350: 6e67 2f73 6572 6c22 2f3e 0d0a 3c2f 613e  ng/serl"/>..</a>
+00000360: 0d0a 0d0a 5365 726c 2028 7365 7269 616c  ....Serl (serial
+00000370: 697a 6564 206c 616e 6775 6167 6573 2920  ized languages) 
+00000380: 6973 2061 2066 6f72 6d61 7420 616e 6420  is a format and 
+00000390: 636f 7272 6573 706f 6e64 696e 6720 636f  corresponding co
+000003a0: 6d6d 616e 6420 6c69 6e65 2074 6f6f 6c20  mmand line tool 
+000003b0: 666f 7220 6372 6561 7469 6e67 2061 6e64  for creating and
+000003c0: 2075 7369 6e67 2074 6578 7475 616c 2064   using textual d
+000003d0: 6f6d 6169 6e20 7370 6563 6966 6963 206f  omain specific o
+000003e0: 7220 6d61 726b 7570 206c 616e 6775 6167  r markup languag
+000003f0: 6573 2077 6974 6820 6172 6269 7472 6172  es with arbitrar
+00000400: 7920 7379 6e74 6178 2e20 5468 6973 2069  y syntax. This i
+00000410: 7320 6163 6869 6576 6564 2074 6872 6f75  s achieved throu
+00000420: 6768 2074 6865 2063 6f6e 6365 7074 206f  gh the concept o
+00000430: 6620 6c61 6e67 7561 6765 2063 6f6e 6669  f language confi
+00000440: 6775 7261 7469 6f6e 732c 2077 6869 6368  gurations, which
+00000450: 2061 7265 2059 414d 4c20 6669 6c65 7320   are YAML files 
+00000460: 666f 7220 7370 6563 6966 7969 6e67 206c  for specifying l
+00000470: 616e 6775 6167 6520 7379 6e74 6178 2061  anguage syntax a
+00000480: 6e64 2066 756e 6374 696f 6e61 6c69 7479  nd functionality
+00000490: 2c20 7573 6564 2062 7920 7468 6520 746f  , used by the to
+000004a0: 6f6c 2074 6f20 6578 6563 7574 6520 6c61  ol to execute la
+000004b0: 6e67 7561 6765 2070 726f 6772 616d 732e  nguage programs.
+000004c0: 2054 6865 7365 2063 6f6e 6669 6775 7261   These configura
+000004d0: 7469 6f6e 7320 6361 6e20 7468 656e 2062  tions can then b
+000004e0: 6520 6c69 6e6b 6564 2c20 616c 6c6f 7769  e linked, allowi
+000004f0: 6e67 206c 616e 6775 6167 6573 2074 6f20  ng languages to 
+00000500: 6265 2075 7365 6420 6c69 6b65 2061 6e79  be used like any
+00000510: 206f 7468 6572 2063 6f6d 6d61 6e64 206c   other command l
+00000520: 696e 6520 746f 6f6c 2e0d 0a0d 0a44 6f63  ine tool.....Doc
+00000530: 756d 656e 7461 7469 6f6e 2063 616e 2062  umentation can b
+00000540: 6520 666f 756e 6420 6f6e 205b 5265 6164  e found on [Read
+00000550: 2054 6865 2044 6f63 735d 2868 7474 7073   The Docs](https
+00000560: 3a2f 2f73 6572 6c2e 7265 6164 7468 6564  ://serl.readthed
+00000570: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000580: 2f69 6e64 6578 2e68 746d 6c29 2e0d 0a0d  /index.html)....
+00000590: 0a23 2323 2044 6576 656c 6f70 6d65 6e74  .### Development
+000005a0: 2057 6f72 6b66 6c6f 770d 0a7c 2043 6f6d   Workflow..| Com
+000005b0: 6d61 6e64 207c 2044 6573 6372 6970 7469  mand | Descripti
+000005c0: 6f6e 207c 0d0a 7c20 2d2d 2d2d 2d2d 2d20  on |..| ------- 
+000005d0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0d  | ----------- |.
+000005e0: 0a7c 2060 7069 7020 696e 7374 616c 6c20  .| `pip install 
+000005f0: 2e60 207c 2042 7569 6c64 2f69 6e73 7461  .` | Build/insta
+00000600: 6c6c 206c 6f63 616c 6c79 207c 0d0a 7c20  ll locally |..| 
+00000610: 6073 6572 6c20 6865 6c70 6020 7c20 5368  `serl help` | Sh
+00000620: 6f77 2074 6865 2074 6f6f 6c20 636f 6d6d  ow the tool comm
+00000630: 616e 6420 6c69 6e65 2068 656c 7020 7363  and line help sc
+00000640: 7265 656e 207c 0d0a 7c20 6070 7974 6573  reen |..| `pytes
+00000650: 7420 7465 7374 7360 206f 7220 6074 6573  t tests` or `tes
+00000660: 742e 6261 7460 207c 2052 756e 2061 7574  t.bat` | Run aut
+00000670: 6f6d 6174 6564 2074 6573 7420 7375 6974  omated test suit
+00000680: 6520 7c0d 0a7c 2060 7079 202d 6d20 6275  e |..| `py -m bu
+00000690: 696c 6460 207c 2042 7569 6c64 2064 6973  ild` | Build dis
+000006a0: 7472 6962 7574 696f 6e20 7c0d 0a7c 2060  tribution |..| `
+000006b0: 7079 202d 6d20 7477 696e 6520 7570 6c6f  py -m twine uplo
+000006c0: 6164 2064 6973 742f 2a60 207c 2055 706c  ad dist/*` | Upl
+000006d0: 6f61 6420 6469 7374 7269 6275 7469 6f6e  oad distribution
+000006e0: 207c 0d0a 7c20 6073 7068 696e 782d 6275   |..| `sphinx-bu
+000006f0: 696c 6420 2d62 2068 746d 6c20 646f 6373  ild -b html docs
+00000700: 2f73 6f75 7263 652f 2064 6f63 732f 6275  /source/ docs/bu
+00000710: 696c 642f 6874 6d6c 6020 7c20 4275 696c  ild/html` | Buil
+00000720: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
+00000730: 7c0d 0a0d 0a0d 0a4d 4954 204c 6963 656e  |......MIT Licen
+00000740: 7365 0d0a 0d0a 436f 7079 7269 6768 7420  se....Copyright 
+00000750: 2863 2920 3230 3233 2048 6172 7279 2044  (c) 2023 Harry D
+00000760: 6f77 6e69 6e67 0d0a 0d0a 5065 726d 6973  owning....Permis
+00000770: 7369 6f6e 2069 7320 6865 7265 6279 2067  sion is hereby g
+00000780: 7261 6e74 6564 2c20 6672 6565 206f 6620  ranted, free of 
+00000790: 6368 6172 6765 2c20 746f 2061 6e79 2070  charge, to any p
+000007a0: 6572 736f 6e20 6f62 7461 696e 696e 6720  erson obtaining 
+000007b0: 6120 636f 7079 0d0a 6f66 2074 6869 7320  a copy..of this 
+000007c0: 736f 6674 7761 7265 2061 6e64 2061 7373  software and ass
+000007d0: 6f63 6961 7465 6420 646f 6375 6d65 6e74  ociated document
+000007e0: 6174 696f 6e20 6669 6c65 7320 2874 6865  ation files (the
+000007f0: 2022 536f 6674 7761 7265 2229 2c20 746f   "Software"), to
+00000800: 2064 6561 6c0d 0a69 6e20 7468 6520 536f   deal..in the So
+00000810: 6674 7761 7265 2077 6974 686f 7574 2072  ftware without r
+00000820: 6573 7472 6963 7469 6f6e 2c20 696e 636c  estriction, incl
+00000830: 7564 696e 6720 7769 7468 6f75 7420 6c69  uding without li
+00000840: 6d69 7461 7469 6f6e 2074 6865 2072 6967  mitation the rig
+00000850: 6874 730d 0a74 6f20 7573 652c 2063 6f70  hts..to use, cop
+00000860: 792c 206d 6f64 6966 792c 206d 6572 6765  y, modify, merge
+00000870: 2c20 7075 626c 6973 682c 2064 6973 7472  , publish, distr
+00000880: 6962 7574 652c 2073 7562 6c69 6365 6e73  ibute, sublicens
+00000890: 652c 2061 6e64 2f6f 7220 7365 6c6c 0d0a  e, and/or sell..
+000008a0: 636f 7069 6573 206f 6620 7468 6520 536f  copies of the So
+000008b0: 6674 7761 7265 2c20 616e 6420 746f 2070  ftware, and to p
+000008c0: 6572 6d69 7420 7065 7273 6f6e 7320 746f  ermit persons to
+000008d0: 2077 686f 6d20 7468 6520 536f 6674 7761   whom the Softwa
+000008e0: 7265 2069 730d 0a66 7572 6e69 7368 6564  re is..furnished
+000008f0: 2074 6f20 646f 2073 6f2c 2073 7562 6a65   to do so, subje
+00000900: 6374 2074 6f20 7468 6520 666f 6c6c 6f77  ct to the follow
+00000910: 696e 6720 636f 6e64 6974 696f 6e73 3a0d  ing conditions:.
+00000920: 0a0d 0a54 6865 2061 626f 7665 2063 6f70  ...The above cop
+00000930: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
+00000940: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
+00000950: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
+00000960: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
+00000970: 6c0d 0a63 6f70 6965 7320 6f72 2073 7562  l..copies or sub
+00000980: 7374 616e 7469 616c 2070 6f72 7469 6f6e  stantial portion
+00000990: 7320 6f66 2074 6865 2053 6f66 7477 6172  s of the Softwar
+000009a0: 652e 0d0a 0d0a 5448 4520 534f 4654 5741  e.....THE SOFTWA
+000009b0: 5245 2049 5320 5052 4f56 4944 4544 2022  RE IS PROVIDED "
+000009c0: 4153 2049 5322 2c20 5749 5448 4f55 5420  AS IS", WITHOUT 
+000009d0: 5741 5252 414e 5459 204f 4620 414e 5920  WARRANTY OF ANY 
+000009e0: 4b49 4e44 2c20 4558 5052 4553 5320 4f52  KIND, EXPRESS OR
+000009f0: 0d0a 494d 504c 4945 442c 2049 4e43 4c55  ..IMPLIED, INCLU
+00000a00: 4449 4e47 2042 5554 204e 4f54 204c 494d  DING BUT NOT LIM
+00000a10: 4954 4544 2054 4f20 5448 4520 5741 5252  ITED TO THE WARR
+00000a20: 414e 5449 4553 204f 4620 4d45 5243 4841  ANTIES OF MERCHA
+00000a30: 4e54 4142 494c 4954 592c 0d0a 4649 544e  NTABILITY,..FITN
+00000a40: 4553 5320 464f 5220 4120 5041 5254 4943  ESS FOR A PARTIC
+00000a50: 554c 4152 2050 5552 504f 5345 2041 4e44  ULAR PURPOSE AND
+00000a60: 204e 4f4e 494e 4652 494e 4745 4d45 4e54   NONINFRINGEMENT
+00000a70: 2e20 494e 204e 4f20 4556 454e 5420 5348  . IN NO EVENT SH
+00000a80: 414c 4c20 5448 450d 0a41 5554 484f 5253  ALL THE..AUTHORS
+00000a90: 204f 5220 434f 5059 5249 4748 5420 484f   OR COPYRIGHT HO
+00000aa0: 4c44 4552 5320 4245 204c 4941 424c 4520  LDERS BE LIABLE 
+00000ab0: 464f 5220 414e 5920 434c 4149 4d2c 2044  FOR ANY CLAIM, D
+00000ac0: 414d 4147 4553 204f 5220 4f54 4845 520d  AMAGES OR OTHER.
+00000ad0: 0a4c 4941 4249 4c49 5459 2c20 5748 4554  .LIABILITY, WHET
+00000ae0: 4845 5220 494e 2041 4e20 4143 5449 4f4e  HER IN AN ACTION
+00000af0: 204f 4620 434f 4e54 5241 4354 2c20 544f   OF CONTRACT, TO
+00000b00: 5254 204f 5220 4f54 4845 5257 4953 452c  RT OR OTHERWISE,
+00000b10: 2041 5249 5349 4e47 2046 524f 4d2c 0d0a   ARISING FROM,..
+00000b20: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
+00000b30: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
+00000b40: 2053 4f46 5457 4152 4520 4f52 2054 4845   SOFTWARE OR THE
+00000b50: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
+00000b60: 414c 494e 4753 2049 4e20 5448 450d 0a53  ALINGS IN THE..S
+00000b70: 4f46 5457 4152 452e 0d0a                 OFTWARE...
```

### Comparing `serl-0.2.2b0/src/serl.egg-info/SOURCES.txt` & `serl-0.3.0b0/src/serl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/tests/test_config.py` & `serl-0.3.0b0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/tests/test_highlight.py` & `serl-0.3.0b0/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/tests/test_lexer.py` & `serl-0.3.0b0/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/tests/test_main.py` & `serl-0.3.0b0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/tests/test_parser.py` & `serl-0.3.0b0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/tests/test_schema.py` & `serl-0.3.0b0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `serl-0.2.2b0/tests/test_utils.py` & `serl-0.3.0b0/tests/test_utils.py`

 * *Files identical despite different names*

