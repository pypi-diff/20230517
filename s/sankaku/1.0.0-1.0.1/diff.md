# Comparing `tmp/sankaku-1.0.0.tar.gz` & `tmp/sankaku-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sankaku-1.0.0.tar", last modified: Mon May 15 18:37:55 2023, max compression
+gzip compressed data, was "sankaku-1.0.1.tar", last modified: Wed May 17 15:20:07 2023, max compression
```

## Comparing `sankaku-1.0.0.tar` & `sankaku-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,37 @@
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-15 18:37:55.245074 sankaku-1.0.0/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.0/LICENSE
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2120 2023-05-15 18:37:55.245074 sankaku-1.0.0/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1560 2023-05-15 18:17:08.000000 sankaku-1.0.0/README.md
--rw-r--r--   0 moldus    (1000) moldus    (1000)       81 2023-05-15 15:32:11.000000 sankaku-1.0.0/pyproject.toml
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-15 18:37:55.238074 sankaku-1.0.0/sankaku/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-10 14:37:51.000000 sankaku-1.0.0/sankaku/__init__.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-15 18:37:55.241074 sankaku-1.0.0/sankaku/clients/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      254 2023-05-15 09:09:08.000000 sankaku-1.0.0/sankaku/clients/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1222 2023-05-15 09:54:46.000000 sankaku-1.0.0/sankaku/clients/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    15189 2023-05-15 09:22:46.000000 sankaku-1.0.0/sankaku/clients/clients.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1998 2023-05-15 10:39:52.000000 sankaku-1.0.0/sankaku/clients/http_client.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1285 2023-05-15 10:30:11.000000 sankaku-1.0.0/sankaku/constants.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-15 09:54:46.000000 sankaku-1.0.0/sankaku/errors.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-15 18:37:55.243074 sankaku-1.0.0/sankaku/models/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.0/sankaku/models/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1900 2023-05-15 09:27:13.000000 sankaku-1.0.0/sankaku/models/books.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-15 09:37:39.000000 sankaku-1.0.0/sankaku/models/http.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      263 2023-05-15 09:37:39.000000 sankaku-1.0.0/sankaku/models/pages.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3466 2023-05-15 09:54:46.000000 sankaku-1.0.0/sankaku/models/posts.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3975 2023-05-15 09:54:46.000000 sankaku-1.0.0/sankaku/models/tags.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2131 2023-05-15 09:54:46.000000 sankaku-1.0.0/sankaku/models/users.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-15 18:37:55.244074 sankaku-1.0.0/sankaku/paginators/
--rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.0/sankaku/paginators/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      857 2023-05-15 09:54:46.000000 sankaku-1.0.0/sankaku/paginators/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    10342 2023-05-15 10:29:22.000000 sankaku-1.0.0/sankaku/paginators/paginators.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      265 2023-05-15 10:29:01.000000 sankaku-1.0.0/sankaku/typedefs.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1986 2023-05-15 09:54:46.000000 sankaku-1.0.0/sankaku/types.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1894 2023-05-15 10:32:52.000000 sankaku-1.0.0/sankaku/utils.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-15 18:37:55.240074 sankaku-1.0.0/sankaku.egg-info/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2120 2023-05-15 18:37:55.000000 sankaku-1.0.0/sankaku.egg-info/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)      718 2023-05-15 18:37:55.000000 sankaku-1.0.0/sankaku.egg-info/SOURCES.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-05-15 18:37:55.000000 sankaku-1.0.0/sankaku.egg-info/dependency_links.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       24 2023-05-15 18:37:55.000000 sankaku-1.0.0/sankaku.egg-info/requires.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-05-15 18:37:55.000000 sankaku-1.0.0/sankaku.egg-info/top_level.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-05-15 18:37:55.245074 sankaku-1.0.0/setup.cfg
--rw-r--r--   0 moldus    (1000) moldus    (1000)      847 2023-05-15 18:26:01.000000 sankaku-1.0.0/setup.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-15 18:37:55.245074 sankaku-1.0.0/tests/
--rw-r--r--   0 moldus    (1000) moldus    (1000)    13837 2023-05-15 08:40:39.000000 sankaku-1.0.0/tests/test_clients.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1200 2023-05-09 12:25:56.000000 sankaku-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.866396 sankaku-1.0.1/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.1/LICENSE
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2948 2023-05-17 15:20:07.866396 sankaku-1.0.1/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2388 2023-05-17 15:02:34.000000 sankaku-1.0.1/README.md
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       81 2023-05-15 15:32:11.000000 sankaku-1.0.1/pyproject.toml
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.863396 sankaku-1.0.1/sankaku/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-10 14:37:51.000000 sankaku-1.0.1/sankaku/__init__.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.864396 sankaku-1.0.1/sankaku/clients/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      351 2023-05-16 19:34:35.000000 sankaku-1.0.1/sankaku/clients/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1222 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/clients/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    15150 2023-05-17 14:47:16.000000 sankaku-1.0.1/sankaku/clients/clients.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1998 2023-05-15 10:39:52.000000 sankaku-1.0.1/sankaku/clients/http_client.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1285 2023-05-15 10:30:11.000000 sankaku-1.0.1/sankaku/constants.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/errors.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.865396 sankaku-1.0.1/sankaku/models/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.1/sankaku/models/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1900 2023-05-15 09:27:13.000000 sankaku-1.0.1/sankaku/models/books.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-15 09:37:39.000000 sankaku-1.0.1/sankaku/models/http.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      263 2023-05-15 09:37:39.000000 sankaku-1.0.1/sankaku/models/pages.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3466 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/models/posts.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3975 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/models/tags.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2131 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/models/users.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.866396 sankaku-1.0.1/sankaku/paginators/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.1/sankaku/paginators/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      857 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/paginators/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    10342 2023-05-15 10:29:22.000000 sankaku-1.0.1/sankaku/paginators/paginators.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      265 2023-05-15 10:29:01.000000 sankaku-1.0.1/sankaku/typedefs.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1986 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/types.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1905 2023-05-17 14:50:40.000000 sankaku-1.0.1/sankaku/utils.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.863396 sankaku-1.0.1/sankaku.egg-info/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2948 2023-05-17 15:20:06.000000 sankaku-1.0.1/sankaku.egg-info/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      676 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/SOURCES.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/dependency_links.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       24 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/requires.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/top_level.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-05-17 15:20:07.866396 sankaku-1.0.1/setup.cfg
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      847 2023-05-17 15:14:00.000000 sankaku-1.0.1/setup.py
```

### Comparing `sankaku-1.0.0/LICENSE` & `sankaku-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/PKG-INFO` & `sankaku-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7361 6e6b  : 2.1.Name: sank
 00000020: 616b 750a 5665 7273 696f 6e3a 2031 2e30  aku.Version: 1.0
-00000030: 2e30 0a53 756d 6d61 7279 3a20 4173 796e  .0.Summary: Asyn
+00000030: 2e31 0a53 756d 6d61 7279 3a20 4173 796e  .1.Summary: Asyn
 00000040: 6368 726f 6e6f 7573 2041 5049 2077 7261  chronous API wra
 00000050: 7070 6572 2066 6f72 2053 616e 6b61 6b75  pper for Sankaku
 00000060: 2043 6f6d 706c 6578 2e0a 486f 6d65 2d70   Complex..Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 7a65 7265 7832 3930  hub.com/zerex290
 00000090: 2f73 616e 6b61 6b75 0a41 7574 686f 723a  /sankaku.Author:
 000000a0: 207a 6572 6578 3239 300a 4175 7468 6f72   zerex290.Author
@@ -30,104 +30,156 @@
 000001d0: 6570 656e 6465 6e74 0a52 6571 7569 7265  ependent.Require
 000001e0: 732d 5079 7468 6f6e 3a20 3e3d 332e 3131  s-Python: >=3.11
 000001f0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 00000200: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 00000210: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
 00000220: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
 00000230: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000240: 7222 3e0a 2020 3c61 3e0a 2020 2020 3c69  r">.  <a>.    <i
-00000250: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000260: 6265 7461 2e73 616e 6b61 6b75 636f 6d70  beta.sankakucomp
-00000270: 6c65 782e 636f 6d2f 696d 6167 6573 2f61  lex.com/images/a
-00000280: 7070 6c65 2d74 6f75 6368 2d69 636f 6e2e  pple-touch-icon.
-00000290: 706e 6722 200a 2020 2020 7769 6474 683d  png" .    width=
-000002a0: 2231 3530 2220 6865 6967 6874 3d22 3135  "150" height="15
-000002b0: 3022 3e0a 2020 3c2f 613e 0a20 203c 6469  0">.  </a>.  <di
-000002c0: 763e 7361 6e6b 616b 753c 2f64 6976 3e0a  v>sankaku</div>.
-000002d0: 3c2f 6831 3e0a 3c70 2061 6c69 676e 3d22  </h1>.<p align="
-000002e0: 6365 6e74 6572 223e 3c65 6d3e 3c62 3e46  center"><em><b>F
-000002f0: 6f72 2072 6561 6c20 6d65 6e20 6f66 2063  or real men of c
-00000300: 756c 7475 7265 203c 2f62 3e3c 2f65 6d3e  ulture </b></em>
-00000310: 2623 3132 3835 3237 3c2f 703e 0a0a 2323  &#128527</p>..##
-00000320: 2041 626f 7574 0a0a 4173 796e 6368 726f   About..Asynchro
-00000330: 6e6f 7573 2041 5049 2077 7261 7070 6572  nous API wrapper
-00000340: 2066 6f72 205b 5361 6e6b 616b 7520 436f   for [Sankaku Co
-00000350: 6d70 6c65 785d 2868 7474 7073 3a2f 2f62  mplex](https://b
-00000360: 6574 612e 7361 6e6b 616b 7563 6f6d 706c  eta.sankakucompl
-00000370: 6578 2e63 6f6d 290a 7769 7468 202a 7479  ex.com).with *ty
-00000380: 7065 2d68 696e 7469 6e67 2a2c 2070 7964  pe-hinting*, pyd
-00000390: 616e 7469 6320 2a64 6174 6120 7661 6c69  antic *data vali
-000003a0: 6461 7469 6f6e 2a20 616e 6420 616e 206f  dation* and an o
-000003b0: 7074 696f 6e61 6c20 2a6c 6f67 6769 6e67  ptional *logging
-000003c0: 2073 7570 706f 7274 2a0a 7769 7468 206c   support*.with l
-000003d0: 6f67 7572 752e 0a0a 2323 2320 4665 6174  oguru...### Feat
-000003e0: 7572 6573 3a0a 0a2d 2054 7970 652d 6869  ures:..- Type-hi
-000003f0: 6e74 730a 2d20 4465 7365 7269 616c 697a  nts.- Deserializ
-00000400: 6174 696f 6e20 6f66 2072 6177 206a 736f  ation of raw jso
-00000410: 6e20 6461 7461 2074 6861 6e6b 7320 746f  n data thanks to
-00000420: 2070 7964 616e 7469 6320 6d6f 6465 6c73   pydantic models
-00000430: 0a2d 2045 6e75 6d65 7261 7469 6f6e 7320  .- Enumerations 
-00000440: 666f 7220 4150 4920 7265 7175 6573 7420  for API request 
-00000450: 7061 7261 6d65 7465 7273 2074 6f20 7072  parameters to pr
-00000460: 6f76 6964 6520 6265 7474 6572 2075 7365  ovide better use
-00000470: 7220 6578 7065 7269 656e 6365 0a20 203e  r experience.  >
-00000480: 2046 6f72 2069 6e73 7461 6e63 652c 2079   For instance, y
-00000490: 6f75 2063 616e 2074 7970 6520 6074 7970  ou can type `typ
-000004a0: 6573 2e54 6167 5479 7065 2e41 5254 4953  es.TagType.ARTIS
-000004b0: 5460 2069 6e73 7465 6164 206f 6620 6074  T` instead of `t
-000004c0: 7970 6573 5b5d 3d31 600a 0a2d 2d2d 0a0a  ypes[]=1`..---..
-000004d0: 446f 6375 6d65 6e74 6174 696f 6e3a 2054  Documentation: T
-000004e0: 4241 0a0a 536f 7572 6365 2063 6f64 653a  BA..Source code:
-000004f0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000500: 636f 6d2f 7a65 7265 7832 3930 2f73 616e  com/zerex290/san
-00000510: 6b61 6b75 0a0a 2d2d 2d0a 0a23 2320 5265  kaku..---..## Re
-00000520: 7175 6972 656d 656e 7473 0a0a 2d20 5079  quirements..- Py
-00000530: 7468 6f6e 2033 2e31 312b 0a2d 2061 696f  thon 3.11+.- aio
-00000540: 6874 7470 0a2d 2070 7964 616e 7469 630a  http.- pydantic.
-00000550: 2d20 6c6f 6775 7275 0a0a 2323 2049 6e73  - loguru..## Ins
-00000560: 7461 6c6c 6174 696f 6e0a 0a60 6060 636f  tallation..```co
-00000570: 6d6d 616e 646c 696e 650a 7069 7020 696e  mmandline.pip in
-00000580: 7374 616c 6c20 7361 6e6b 616b 750a 6060  stall sankaku.``
-00000590: 600a 0a23 2320 4578 616d 706c 650a 0a49  `..## Example..I
-000005a0: 7427 7320 7665 7279 2073 696d 706c 6520  t's very simple 
-000005b0: 746f 2075 7365 2061 6e64 2064 6f65 736e  to use and doesn
-000005c0: 2774 2072 6571 7569 7265 2074 6f20 616c  't require to al
-000005d0: 7761 7973 206b 6565 7020 6f70 656e 6564  ways keep opened
-000005e0: 2062 726f 7773 6572 2070 6167 650a 7769   browser page.wi
-000005f0: 7468 2064 6f63 756d 656e 7461 7469 6f6e  th documentation
-00000600: 2062 6563 6175 7365 2061 6c6c 206d 6574   because all met
-00000610: 686f 6473 2061 7265 2073 656c 662d 6578  hods are self-ex
-00000620: 706c 616e 6174 6f72 792e 0a0a 6060 6070  planatory...```p
-00000630: 790a 696d 706f 7274 2061 7379 6e63 696f  y.import asyncio
-00000640: 0a66 726f 6d20 7361 6e6b 616b 7520 696d  .from sankaku im
-00000650: 706f 7274 2053 616e 6b61 6b75 436c 6965  port SankakuClie
-00000660: 6e74 0a0a 6173 796e 6320 6465 6620 6d61  nt..async def ma
-00000670: 696e 2829 3a0a 2020 2020 636c 6965 6e74  in():.    client
-00000680: 203d 2053 616e 6b61 6b75 436c 6965 6e74   = SankakuClient
-00000690: 2829 0a0a 2020 2020 706f 7374 203d 2061  ()..    post = a
-000006a0: 7761 6974 2063 6c69 656e 742e 6765 745f  wait client.get_
-000006b0: 706f 7374 2832 3537 3432 3036 3429 0a20  post(25742064). 
-000006c0: 2020 2070 7269 6e74 2866 2252 6174 696e     print(f"Ratin
-000006d0: 673a 207b 706f 7374 2e72 6174 696e 677d  g: {post.rating}
-000006e0: 207c 2043 7265 6174 6564 3a20 7b70 6f73   | Created: {pos
-000006f0: 742e 6372 6561 7465 645f 6174 7d22 290a  t.created_at}").
-00000700: 2020 2020 2320 2252 6174 696e 673a 2052      # "Rating: R
-00000710: 6174 696e 672e 5155 4553 5449 4f4e 4142  ating.QUESTIONAB
-00000720: 4c45 207c 2043 7265 6174 6564 3a20 3230  LE | Created: 20
-00000730: 3231 2d30 382d 3031 2032 333a 3138 3a35  21-08-01 23:18:5
-00000740: 322b 3033 3a30 3022 0a0a 2020 2020 6177  2+03:00"..    aw
-00000750: 6169 7420 636c 6965 6e74 2e6c 6f67 696e  ait client.login
-00000760: 2861 6363 6573 735f 746f 6b65 6e3d 2274  (access_token="t
-00000770: 6f6b 656e 2229 0a20 2020 2023 204f 7220  oken").    # Or 
-00000780: 796f 7520 6361 6e20 6175 7468 6f72 697a  you can authoriz
-00000790: 6520 6279 2063 7265 6465 6e74 6961 6c73  e by credentials
-000007a0: 3a0a 2020 2020 2320 6177 6169 7420 636c  :.    # await cl
-000007b0: 6965 6e74 2e6c 6f67 696e 286c 6f67 696e  ient.login(login
-000007c0: 3d22 6e69 636b 6e61 6d65 206f 7220 656d  ="nickname or em
-000007d0: 6169 6c22 2c20 7061 7373 776f 7264 3d22  ail", password="
-000007e0: 7061 7373 776f 7264 2229 0a20 2020 2061  password").    a
-000007f0: 7379 6e63 2066 6f72 2062 6f6f 6b20 696e  sync for book in
-00000800: 2063 6c69 656e 742e 6765 745f 7265 6365   client.get_rece
-00000810: 6e74 6c79 5f72 6561 645f 626f 6f6b 7328  ntly_read_books(
-00000820: 293a 0a20 2020 2020 2020 202e 2e2e 0a0a  ):.        .....
-00000830: 6173 796e 6369 6f2e 7275 6e28 6d61 696e  asyncio.run(main
-00000840: 2829 290a 6060 600a                      ()).```.
+00000240: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
+00000250: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000260: 6d2f 7a65 7265 7832 3930 2f73 616e 6b61  m/zerex290/sanka
+00000270: 6b75 223e 0a20 2020 203c 696d 6720 7372  ku">.    <img sr
+00000280: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000290: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000002a0: 2e63 6f6d 2f7a 6572 6578 3239 302f 7361  .com/zerex290/sa
+000002b0: 6e6b 616b 752f 6d61 696e 2f64 6f63 732f  nkaku/main/docs/
+000002c0: 6963 6f6e 2e70 6e67 2220 616c 743d 2253  icon.png" alt="S
+000002d0: 616e 6b61 6b75 2043 6f6d 706c 6578 220a  ankaku Complex".
+000002e0: 2020 2020 7769 6474 683d 2231 3530 2220      width="150" 
+000002f0: 6865 6967 6874 3d22 3135 3022 2f3e 0a20  height="150"/>. 
+00000300: 203c 2f61 3e0a 2020 3c64 6976 3e73 616e   </a>.  <div>san
+00000310: 6b61 6b75 3c2f 6469 763e 0a3c 2f68 313e  kaku</div>.</h1>
+00000320: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000330: 7222 3e3c 656d 3e3c 623e 466f 7220 7265  r"><em><b>For re
+00000340: 616c 206d 656e 206f 6620 6375 6c74 7572  al men of cultur
+00000350: 6520 3c2f 623e 3c2f 656d 3e3c 2f70 3e0a  e </b></em></p>.
+00000360: 0a23 2320 4162 6f75 740a 0a41 7379 6e63  .## About..Async
+00000370: 6872 6f6e 6f75 7320 4150 4920 7772 6170  hronous API wrap
+00000380: 7065 7220 666f 7220 5b53 616e 6b61 6b75  per for [Sankaku
+00000390: 2043 6f6d 706c 6578 5d28 6874 7470 733a   Complex](https:
+000003a0: 2f2f 6265 7461 2e73 616e 6b61 6b75 636f  //beta.sankakuco
+000003b0: 6d70 6c65 782e 636f 6d29 0a77 6974 6820  mplex.com).with 
+000003c0: 2a74 7970 652d 6869 6e74 696e 672a 2c20  *type-hinting*, 
+000003d0: 7079 6461 6e74 6963 202a 6461 7461 2076  pydantic *data v
+000003e0: 616c 6964 6174 696f 6e2a 2061 6e64 2061  alidation* and a
+000003f0: 6e20 6f70 7469 6f6e 616c 202a 6c6f 6767  n optional *logg
+00000400: 696e 6720 7375 7070 6f72 742a 0a77 6974  ing support*.wit
+00000410: 6820 6c6f 6775 7275 2e0a 0a23 2323 2046  h loguru...### F
+00000420: 6561 7475 7265 733a 0a0a 2d20 5479 7065  eatures:..- Type
+00000430: 2d68 696e 7473 0a2d 2044 6573 6572 6961  -hints.- Deseria
+00000440: 6c69 7a61 7469 6f6e 206f 6620 7261 7720  lization of raw 
+00000450: 6a73 6f6e 2064 6174 6120 7468 616e 6b73  json data thanks
+00000460: 2074 6f20 7079 6461 6e74 6963 206d 6f64   to pydantic mod
+00000470: 656c 730a 2d20 456e 756d 6572 6174 696f  els.- Enumeratio
+00000480: 6e73 2066 6f72 2041 5049 2072 6571 7565  ns for API reque
+00000490: 7374 2070 6172 616d 6574 6572 7320 746f  st parameters to
+000004a0: 2070 726f 7669 6465 2062 6574 7465 7220   provide better 
+000004b0: 7573 6572 2065 7870 6572 6965 6e63 650a  user experience.
+000004c0: 2020 3e20 466f 7220 696e 7374 616e 6365    > For instance
+000004d0: 2c20 796f 7520 6361 6e20 7479 7065 2060  , you can type `
+000004e0: 7479 7065 732e 5461 6754 7970 652e 4152  types.TagType.AR
+000004f0: 5449 5354 6020 696e 7374 6561 6420 6f66  TIST` instead of
+00000500: 2060 7479 7065 735b 5d3d 3160 0a0a 2d2d   `types[]=1`..--
+00000510: 2d0a 0a44 6f63 756d 656e 7461 7469 6f6e  -..Documentation
+00000520: 3a20 6874 7470 733a 2f2f 7a65 7265 7832  : https://zerex2
+00000530: 3930 2e67 6974 6875 622e 696f 2f73 616e  90.github.io/san
+00000540: 6b61 6b75 0a0a 4150 4920 5265 6665 7265  kaku..API Refere
+00000550: 6e63 653a 2068 7474 7073 3a2f 2f7a 6572  nce: https://zer
+00000560: 6578 3239 302e 6769 7468 7562 2e69 6f2f  ex290.github.io/
+00000570: 7361 6e6b 616b 752f 6170 690a 0a53 6f75  sankaku/api..Sou
+00000580: 7263 6520 636f 6465 3a20 6874 7470 733a  rce code: https:
+00000590: 2f2f 6769 7468 7562 2e63 6f6d 2f7a 6572  //github.com/zer
+000005a0: 6578 3239 302f 7361 6e6b 616b 750a 0a2d  ex290/sankaku..-
+000005b0: 2d2d 0a0a 2323 2052 6571 7569 7265 6d65  --..## Requireme
+000005c0: 6e74 730a 0a2d 2050 7974 686f 6e20 332e  nts..- Python 3.
+000005d0: 3131 2b0a 2d20 6169 6f68 7474 700a 2d20  11+.- aiohttp.- 
+000005e0: 7079 6461 6e74 6963 0a2d 206c 6f67 7572  pydantic.- logur
+000005f0: 750a 0a23 2320 496e 7374 616c 6c61 7469  u..## Installati
+00000600: 6f6e 0a0a 546f 2069 6e73 7461 6c6c 2073  on..To install s
+00000610: 616e 6b61 6b75 2076 6961 2070 6970 2077  ankaku via pip w
+00000620: 7269 7465 2066 6f6c 6c6f 7769 6e67 206c  rite following l
+00000630: 696e 6520 6f66 2063 6f64 6520 696e 2079  ine of code in y
+00000640: 6f75 7220 7465 726d 696e 616c 3a0a 0a60  our terminal:..`
+00000650: 6060 636f 6d6d 616e 646c 696e 650a 7069  ``commandline.pi
+00000660: 7020 696e 7374 616c 6c20 7361 6e6b 616b  p install sankak
+00000670: 750a 6060 600a 0a54 6f20 696e 7374 616c  u.```..To instal
+00000680: 6c20 7468 6520 7361 6e6b 616b 7520 7669  l the sankaku vi
+00000690: 6120 446f 636b 6572 2c20 796f 7520 6361  a Docker, you ca
+000006a0: 6e20 666f 6c6c 6f77 2074 6865 7365 2073  n follow these s
+000006b0: 7465 7073 3a0a 0a23 2323 2323 2320 5374  teps:..###### St
+000006c0: 6570 2031 3a20 496e 7374 616c 6c20 446f  ep 1: Install Do
+000006d0: 636b 6572 0a0a 456e 7375 7265 2074 6861  cker..Ensure tha
+000006e0: 7420 446f 636b 6572 2069 7320 696e 7374  t Docker is inst
+000006f0: 616c 6c65 6420 6f6e 2079 6f75 7220 6d61  alled on your ma
+00000700: 6368 696e 652e 2049 6620 446f 636b 6572  chine. If Docker
+00000710: 2069 7320 6e6f 7420 616c 7265 6164 790a   is not already.
+00000720: 696e 7374 616c 6c65 642c 2079 6f75 2063  installed, you c
+00000730: 616e 2064 6f77 6e6c 6f61 6420 616e 6420  an download and 
+00000740: 696e 7374 616c 6c20 6974 2066 726f 6d20  install it from 
+00000750: 7468 6520 6f66 6669 6369 616c 0a5b 446f  the official.[Do
+00000760: 636b 6572 2077 6562 7369 7465 5d28 6874  cker website](ht
+00000770: 7470 733a 2f2f 7777 772e 646f 636b 6572  tps://www.docker
+00000780: 2e63 6f6d 2f67 6574 2d73 7461 7274 6564  .com/get-started
+00000790: 292e 0a0a 2323 2323 2323 2053 7465 7020  )...###### Step 
+000007a0: 323a 2055 7365 2064 6f63 6b65 7220 746f  2: Use docker to
+000007b0: 2069 6e73 7461 6c6c 2073 616e 6b61 6b75   install sankaku
+000007c0: 0a0a 4f70 656e 2061 2063 6f6d 6d61 6e64  ..Open a command
+000007d0: 2070 726f 6d70 742e 204e 6176 6967 6174   prompt. Navigat
+000007e0: 6520 746f 2074 6865 2064 6972 6563 746f  e to the directo
+000007f0: 7279 2077 6865 7265 2079 6f75 2077 616e  ry where you wan
+00000800: 740a 746f 2069 6e73 7461 6c6c 2053 616e  t.to install San
+00000810: 6b61 6b75 2e20 5479 7065 2074 6865 2066  kaku. Type the f
+00000820: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000830: 3a0a 0a60 6060 636f 6d6d 616e 646c 696e  :..```commandlin
+00000840: 650a 6769 7420 636c 6f6e 6520 6874 7470  e.git clone http
+00000850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f7a  s://github.com/z
+00000860: 6572 6578 3239 302f 7361 6e6b 616b 752e  erex290/sankaku.
+00000870: 6769 740a 6364 2073 616e 6b61 6b75 0a64  git.cd sankaku.d
+00000880: 6f63 6b65 7220 7275 6e20 2d69 7420 2d2d  ocker run -it --
+00000890: 6e61 6d65 2073 616e 6b61 6b75 202d 7720  name sankaku -w 
+000008a0: 2f6f 7074 202d 7624 2870 7764 293a 2f6f  /opt -v$(pwd):/o
+000008b0: 7074 2070 7974 686f 6e3a 332e 3131 2062  pt python:3.11 b
+000008c0: 6173 680a 6060 600a 0a23 2320 5573 6167  ash.```..## Usag
+000008d0: 6520 6578 616d 706c 650a 0a49 7427 7320  e example..It's 
+000008e0: 7665 7279 2073 696d 706c 6520 746f 2075  very simple to u
+000008f0: 7365 2061 6e64 2064 6f65 736e 2774 2072  se and doesn't r
+00000900: 6571 7569 7265 2074 6f20 616c 7761 7973  equire to always
+00000910: 206b 6565 7020 6f70 656e 6564 2062 726f   keep opened bro
+00000920: 7773 6572 2070 6167 650a 7769 7468 2064  wser page.with d
+00000930: 6f63 756d 656e 7461 7469 6f6e 2062 6563  ocumentation bec
+00000940: 6175 7365 2061 6c6c 206d 6574 686f 6473  ause all methods
+00000950: 2061 7265 2073 656c 662d 6578 706c 616e   are self-explan
+00000960: 6174 6f72 793a 0a0a 6060 6070 790a 696d  atory:..```py.im
+00000970: 706f 7274 2061 7379 6e63 696f 0a66 726f  port asyncio.fro
+00000980: 6d20 7361 6e6b 616b 7520 696d 706f 7274  m sankaku import
+00000990: 2053 616e 6b61 6b75 436c 6965 6e74 0a0a   SankakuClient..
+000009a0: 6173 796e 6320 6465 6620 6d61 696e 2829  async def main()
+000009b0: 3a0a 2020 2020 636c 6965 6e74 203d 2053  :.    client = S
+000009c0: 616e 6b61 6b75 436c 6965 6e74 2829 0a0a  ankakuClient()..
+000009d0: 2020 2020 706f 7374 203d 2061 7761 6974      post = await
+000009e0: 2063 6c69 656e 742e 6765 745f 706f 7374   client.get_post
+000009f0: 2832 3537 3432 3036 3429 0a20 2020 2070  (25742064).    p
+00000a00: 7269 6e74 2866 2252 6174 696e 673a 207b  rint(f"Rating: {
+00000a10: 706f 7374 2e72 6174 696e 677d 207c 2043  post.rating} | C
+00000a20: 7265 6174 6564 3a20 7b70 6f73 742e 6372  reated: {post.cr
+00000a30: 6561 7465 645f 6174 7d22 290a 2020 2020  eated_at}").    
+00000a40: 2320 2252 6174 696e 673a 2052 6174 696e  # "Rating: Ratin
+00000a50: 672e 5155 4553 5449 4f4e 4142 4c45 207c  g.QUESTIONABLE |
+00000a60: 2043 7265 6174 6564 3a20 3230 3231 2d30   Created: 2021-0
+00000a70: 382d 3031 2032 333a 3138 3a35 322b 3033  8-01 23:18:52+03
+00000a80: 3a30 3022 0a0a 2020 2020 6177 6169 7420  :00"..    await 
+00000a90: 636c 6965 6e74 2e6c 6f67 696e 2861 6363  client.login(acc
+00000aa0: 6573 735f 746f 6b65 6e3d 2274 6f6b 656e  ess_token="token
+00000ab0: 2229 0a20 2020 2023 204f 7220 796f 7520  ").    # Or you 
+00000ac0: 6361 6e20 6175 7468 6f72 697a 6520 6279  can authorize by
+00000ad0: 2063 7265 6465 6e74 6961 6c73 3a0a 2020   credentials:.  
+00000ae0: 2020 2320 6177 6169 7420 636c 6965 6e74    # await client
+00000af0: 2e6c 6f67 696e 286c 6f67 696e 3d22 6e69  .login(login="ni
+00000b00: 636b 6e61 6d65 206f 7220 656d 6169 6c22  ckname or email"
+00000b10: 2c20 7061 7373 776f 7264 3d22 7061 7373  , password="pass
+00000b20: 776f 7264 2229 0a20 2020 2061 7379 6e63  word").    async
+00000b30: 2066 6f72 2062 6f6f 6b20 696e 2063 6c69   for book in cli
+00000b40: 656e 742e 6765 745f 7265 6365 6e74 6c79  ent.get_recently
+00000b50: 5f72 6561 645f 626f 6f6b 7328 293a 0a20  _read_books():. 
+00000b60: 2020 2020 2020 202e 2e2e 0a0a 6173 796e         .....asyn
+00000b70: 6369 6f2e 7275 6e28 6d61 696e 2829 290a  cio.run(main()).
+00000b80: 6060 600a                                ```.
```

### Comparing `sankaku-1.0.0/README.md` & `sankaku-1.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,150 @@
 00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000010: 7222 3e0a 2020 3c61 3e0a 2020 2020 3c69  r">.  <a>.    <i
-00000020: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000030: 6265 7461 2e73 616e 6b61 6b75 636f 6d70  beta.sankakucomp
-00000040: 6c65 782e 636f 6d2f 696d 6167 6573 2f61  lex.com/images/a
-00000050: 7070 6c65 2d74 6f75 6368 2d69 636f 6e2e  pple-touch-icon.
-00000060: 706e 6722 200a 2020 2020 7769 6474 683d  png" .    width=
-00000070: 2231 3530 2220 6865 6967 6874 3d22 3135  "150" height="15
-00000080: 3022 3e0a 2020 3c2f 613e 0a20 203c 6469  0">.  </a>.  <di
-00000090: 763e 7361 6e6b 616b 753c 2f64 6976 3e0a  v>sankaku</div>.
-000000a0: 3c2f 6831 3e0a 3c70 2061 6c69 676e 3d22  </h1>.<p align="
-000000b0: 6365 6e74 6572 223e 3c65 6d3e 3c62 3e46  center"><em><b>F
-000000c0: 6f72 2072 6561 6c20 6d65 6e20 6f66 2063  or real men of c
-000000d0: 756c 7475 7265 203c 2f62 3e3c 2f65 6d3e  ulture </b></em>
-000000e0: 2623 3132 3835 3237 3c2f 703e 0a0a 2323  &#128527</p>..##
-000000f0: 2041 626f 7574 0a0a 4173 796e 6368 726f   About..Asynchro
-00000100: 6e6f 7573 2041 5049 2077 7261 7070 6572  nous API wrapper
-00000110: 2066 6f72 205b 5361 6e6b 616b 7520 436f   for [Sankaku Co
-00000120: 6d70 6c65 785d 2868 7474 7073 3a2f 2f62  mplex](https://b
-00000130: 6574 612e 7361 6e6b 616b 7563 6f6d 706c  eta.sankakucompl
-00000140: 6578 2e63 6f6d 290a 7769 7468 202a 7479  ex.com).with *ty
-00000150: 7065 2d68 696e 7469 6e67 2a2c 2070 7964  pe-hinting*, pyd
-00000160: 616e 7469 6320 2a64 6174 6120 7661 6c69  antic *data vali
-00000170: 6461 7469 6f6e 2a20 616e 6420 616e 206f  dation* and an o
-00000180: 7074 696f 6e61 6c20 2a6c 6f67 6769 6e67  ptional *logging
-00000190: 2073 7570 706f 7274 2a0a 7769 7468 206c   support*.with l
-000001a0: 6f67 7572 752e 0a0a 2323 2320 4665 6174  oguru...### Feat
-000001b0: 7572 6573 3a0a 0a2d 2054 7970 652d 6869  ures:..- Type-hi
-000001c0: 6e74 730a 2d20 4465 7365 7269 616c 697a  nts.- Deserializ
-000001d0: 6174 696f 6e20 6f66 2072 6177 206a 736f  ation of raw jso
-000001e0: 6e20 6461 7461 2074 6861 6e6b 7320 746f  n data thanks to
-000001f0: 2070 7964 616e 7469 6320 6d6f 6465 6c73   pydantic models
-00000200: 0a2d 2045 6e75 6d65 7261 7469 6f6e 7320  .- Enumerations 
-00000210: 666f 7220 4150 4920 7265 7175 6573 7420  for API request 
-00000220: 7061 7261 6d65 7465 7273 2074 6f20 7072  parameters to pr
-00000230: 6f76 6964 6520 6265 7474 6572 2075 7365  ovide better use
-00000240: 7220 6578 7065 7269 656e 6365 0a20 203e  r experience.  >
-00000250: 2046 6f72 2069 6e73 7461 6e63 652c 2079   For instance, y
-00000260: 6f75 2063 616e 2074 7970 6520 6074 7970  ou can type `typ
-00000270: 6573 2e54 6167 5479 7065 2e41 5254 4953  es.TagType.ARTIS
-00000280: 5460 2069 6e73 7465 6164 206f 6620 6074  T` instead of `t
-00000290: 7970 6573 5b5d 3d31 600a 0a2d 2d2d 0a0a  ypes[]=1`..---..
-000002a0: 446f 6375 6d65 6e74 6174 696f 6e3a 2054  Documentation: T
-000002b0: 4241 0a0a 536f 7572 6365 2063 6f64 653a  BA..Source code:
-000002c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000002d0: 636f 6d2f 7a65 7265 7832 3930 2f73 616e  com/zerex290/san
-000002e0: 6b61 6b75 0a0a 2d2d 2d0a 0a23 2320 5265  kaku..---..## Re
-000002f0: 7175 6972 656d 656e 7473 0a0a 2d20 5079  quirements..- Py
-00000300: 7468 6f6e 2033 2e31 312b 0a2d 2061 696f  thon 3.11+.- aio
-00000310: 6874 7470 0a2d 2070 7964 616e 7469 630a  http.- pydantic.
-00000320: 2d20 6c6f 6775 7275 0a0a 2323 2049 6e73  - loguru..## Ins
-00000330: 7461 6c6c 6174 696f 6e0a 0a60 6060 636f  tallation..```co
-00000340: 6d6d 616e 646c 696e 650a 7069 7020 696e  mmandline.pip in
-00000350: 7374 616c 6c20 7361 6e6b 616b 750a 6060  stall sankaku.``
-00000360: 600a 0a23 2320 4578 616d 706c 650a 0a49  `..## Example..I
-00000370: 7427 7320 7665 7279 2073 696d 706c 6520  t's very simple 
-00000380: 746f 2075 7365 2061 6e64 2064 6f65 736e  to use and doesn
-00000390: 2774 2072 6571 7569 7265 2074 6f20 616c  't require to al
-000003a0: 7761 7973 206b 6565 7020 6f70 656e 6564  ways keep opened
-000003b0: 2062 726f 7773 6572 2070 6167 650a 7769   browser page.wi
-000003c0: 7468 2064 6f63 756d 656e 7461 7469 6f6e  th documentation
-000003d0: 2062 6563 6175 7365 2061 6c6c 206d 6574   because all met
-000003e0: 686f 6473 2061 7265 2073 656c 662d 6578  hods are self-ex
-000003f0: 706c 616e 6174 6f72 792e 0a0a 6060 6070  planatory...```p
-00000400: 790a 696d 706f 7274 2061 7379 6e63 696f  y.import asyncio
-00000410: 0a66 726f 6d20 7361 6e6b 616b 7520 696d  .from sankaku im
-00000420: 706f 7274 2053 616e 6b61 6b75 436c 6965  port SankakuClie
-00000430: 6e74 0a0a 6173 796e 6320 6465 6620 6d61  nt..async def ma
-00000440: 696e 2829 3a0a 2020 2020 636c 6965 6e74  in():.    client
-00000450: 203d 2053 616e 6b61 6b75 436c 6965 6e74   = SankakuClient
-00000460: 2829 0a0a 2020 2020 706f 7374 203d 2061  ()..    post = a
-00000470: 7761 6974 2063 6c69 656e 742e 6765 745f  wait client.get_
-00000480: 706f 7374 2832 3537 3432 3036 3429 0a20  post(25742064). 
-00000490: 2020 2070 7269 6e74 2866 2252 6174 696e     print(f"Ratin
-000004a0: 673a 207b 706f 7374 2e72 6174 696e 677d  g: {post.rating}
-000004b0: 207c 2043 7265 6174 6564 3a20 7b70 6f73   | Created: {pos
-000004c0: 742e 6372 6561 7465 645f 6174 7d22 290a  t.created_at}").
-000004d0: 2020 2020 2320 2252 6174 696e 673a 2052      # "Rating: R
-000004e0: 6174 696e 672e 5155 4553 5449 4f4e 4142  ating.QUESTIONAB
-000004f0: 4c45 207c 2043 7265 6174 6564 3a20 3230  LE | Created: 20
-00000500: 3231 2d30 382d 3031 2032 333a 3138 3a35  21-08-01 23:18:5
-00000510: 322b 3033 3a30 3022 0a0a 2020 2020 6177  2+03:00"..    aw
-00000520: 6169 7420 636c 6965 6e74 2e6c 6f67 696e  ait client.login
-00000530: 2861 6363 6573 735f 746f 6b65 6e3d 2274  (access_token="t
-00000540: 6f6b 656e 2229 0a20 2020 2023 204f 7220  oken").    # Or 
-00000550: 796f 7520 6361 6e20 6175 7468 6f72 697a  you can authoriz
-00000560: 6520 6279 2063 7265 6465 6e74 6961 6c73  e by credentials
-00000570: 3a0a 2020 2020 2320 6177 6169 7420 636c  :.    # await cl
-00000580: 6965 6e74 2e6c 6f67 696e 286c 6f67 696e  ient.login(login
-00000590: 3d22 6e69 636b 6e61 6d65 206f 7220 656d  ="nickname or em
-000005a0: 6169 6c22 2c20 7061 7373 776f 7264 3d22  ail", password="
-000005b0: 7061 7373 776f 7264 2229 0a20 2020 2061  password").    a
-000005c0: 7379 6e63 2066 6f72 2062 6f6f 6b20 696e  sync for book in
-000005d0: 2063 6c69 656e 742e 6765 745f 7265 6365   client.get_rece
-000005e0: 6e74 6c79 5f72 6561 645f 626f 6f6b 7328  ntly_read_books(
-000005f0: 293a 0a20 2020 2020 2020 202e 2e2e 0a0a  ):.        .....
-00000600: 6173 796e 6369 6f2e 7275 6e28 6d61 696e  asyncio.run(main
-00000610: 2829 290a 6060 600a                      ()).```.
+00000010: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
+00000020: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000030: 6d2f 7a65 7265 7832 3930 2f73 616e 6b61  m/zerex290/sanka
+00000040: 6b75 223e 0a20 2020 203c 696d 6720 7372  ku">.    <img sr
+00000050: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000060: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000070: 2e63 6f6d 2f7a 6572 6578 3239 302f 7361  .com/zerex290/sa
+00000080: 6e6b 616b 752f 6d61 696e 2f64 6f63 732f  nkaku/main/docs/
+00000090: 6963 6f6e 2e70 6e67 2220 616c 743d 2253  icon.png" alt="S
+000000a0: 616e 6b61 6b75 2043 6f6d 706c 6578 220a  ankaku Complex".
+000000b0: 2020 2020 7769 6474 683d 2231 3530 2220      width="150" 
+000000c0: 6865 6967 6874 3d22 3135 3022 2f3e 0a20  height="150"/>. 
+000000d0: 203c 2f61 3e0a 2020 3c64 6976 3e73 616e   </a>.  <div>san
+000000e0: 6b61 6b75 3c2f 6469 763e 0a3c 2f68 313e  kaku</div>.</h1>
+000000f0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000100: 7222 3e3c 656d 3e3c 623e 466f 7220 7265  r"><em><b>For re
+00000110: 616c 206d 656e 206f 6620 6375 6c74 7572  al men of cultur
+00000120: 6520 3c2f 623e 3c2f 656d 3e3c 2f70 3e0a  e </b></em></p>.
+00000130: 0a23 2320 4162 6f75 740a 0a41 7379 6e63  .## About..Async
+00000140: 6872 6f6e 6f75 7320 4150 4920 7772 6170  hronous API wrap
+00000150: 7065 7220 666f 7220 5b53 616e 6b61 6b75  per for [Sankaku
+00000160: 2043 6f6d 706c 6578 5d28 6874 7470 733a   Complex](https:
+00000170: 2f2f 6265 7461 2e73 616e 6b61 6b75 636f  //beta.sankakuco
+00000180: 6d70 6c65 782e 636f 6d29 0a77 6974 6820  mplex.com).with 
+00000190: 2a74 7970 652d 6869 6e74 696e 672a 2c20  *type-hinting*, 
+000001a0: 7079 6461 6e74 6963 202a 6461 7461 2076  pydantic *data v
+000001b0: 616c 6964 6174 696f 6e2a 2061 6e64 2061  alidation* and a
+000001c0: 6e20 6f70 7469 6f6e 616c 202a 6c6f 6767  n optional *logg
+000001d0: 696e 6720 7375 7070 6f72 742a 0a77 6974  ing support*.wit
+000001e0: 6820 6c6f 6775 7275 2e0a 0a23 2323 2046  h loguru...### F
+000001f0: 6561 7475 7265 733a 0a0a 2d20 5479 7065  eatures:..- Type
+00000200: 2d68 696e 7473 0a2d 2044 6573 6572 6961  -hints.- Deseria
+00000210: 6c69 7a61 7469 6f6e 206f 6620 7261 7720  lization of raw 
+00000220: 6a73 6f6e 2064 6174 6120 7468 616e 6b73  json data thanks
+00000230: 2074 6f20 7079 6461 6e74 6963 206d 6f64   to pydantic mod
+00000240: 656c 730a 2d20 456e 756d 6572 6174 696f  els.- Enumeratio
+00000250: 6e73 2066 6f72 2041 5049 2072 6571 7565  ns for API reque
+00000260: 7374 2070 6172 616d 6574 6572 7320 746f  st parameters to
+00000270: 2070 726f 7669 6465 2062 6574 7465 7220   provide better 
+00000280: 7573 6572 2065 7870 6572 6965 6e63 650a  user experience.
+00000290: 2020 3e20 466f 7220 696e 7374 616e 6365    > For instance
+000002a0: 2c20 796f 7520 6361 6e20 7479 7065 2060  , you can type `
+000002b0: 7479 7065 732e 5461 6754 7970 652e 4152  types.TagType.AR
+000002c0: 5449 5354 6020 696e 7374 6561 6420 6f66  TIST` instead of
+000002d0: 2060 7479 7065 735b 5d3d 3160 0a0a 2d2d   `types[]=1`..--
+000002e0: 2d0a 0a44 6f63 756d 656e 7461 7469 6f6e  -..Documentation
+000002f0: 3a20 6874 7470 733a 2f2f 7a65 7265 7832  : https://zerex2
+00000300: 3930 2e67 6974 6875 622e 696f 2f73 616e  90.github.io/san
+00000310: 6b61 6b75 0a0a 4150 4920 5265 6665 7265  kaku..API Refere
+00000320: 6e63 653a 2068 7474 7073 3a2f 2f7a 6572  nce: https://zer
+00000330: 6578 3239 302e 6769 7468 7562 2e69 6f2f  ex290.github.io/
+00000340: 7361 6e6b 616b 752f 6170 690a 0a53 6f75  sankaku/api..Sou
+00000350: 7263 6520 636f 6465 3a20 6874 7470 733a  rce code: https:
+00000360: 2f2f 6769 7468 7562 2e63 6f6d 2f7a 6572  //github.com/zer
+00000370: 6578 3239 302f 7361 6e6b 616b 750a 0a2d  ex290/sankaku..-
+00000380: 2d2d 0a0a 2323 2052 6571 7569 7265 6d65  --..## Requireme
+00000390: 6e74 730a 0a2d 2050 7974 686f 6e20 332e  nts..- Python 3.
+000003a0: 3131 2b0a 2d20 6169 6f68 7474 700a 2d20  11+.- aiohttp.- 
+000003b0: 7079 6461 6e74 6963 0a2d 206c 6f67 7572  pydantic.- logur
+000003c0: 750a 0a23 2320 496e 7374 616c 6c61 7469  u..## Installati
+000003d0: 6f6e 0a0a 546f 2069 6e73 7461 6c6c 2073  on..To install s
+000003e0: 616e 6b61 6b75 2076 6961 2070 6970 2077  ankaku via pip w
+000003f0: 7269 7465 2066 6f6c 6c6f 7769 6e67 206c  rite following l
+00000400: 696e 6520 6f66 2063 6f64 6520 696e 2079  ine of code in y
+00000410: 6f75 7220 7465 726d 696e 616c 3a0a 0a60  our terminal:..`
+00000420: 6060 636f 6d6d 616e 646c 696e 650a 7069  ``commandline.pi
+00000430: 7020 696e 7374 616c 6c20 7361 6e6b 616b  p install sankak
+00000440: 750a 6060 600a 0a54 6f20 696e 7374 616c  u.```..To instal
+00000450: 6c20 7468 6520 7361 6e6b 616b 7520 7669  l the sankaku vi
+00000460: 6120 446f 636b 6572 2c20 796f 7520 6361  a Docker, you ca
+00000470: 6e20 666f 6c6c 6f77 2074 6865 7365 2073  n follow these s
+00000480: 7465 7073 3a0a 0a23 2323 2323 2320 5374  teps:..###### St
+00000490: 6570 2031 3a20 496e 7374 616c 6c20 446f  ep 1: Install Do
+000004a0: 636b 6572 0a0a 456e 7375 7265 2074 6861  cker..Ensure tha
+000004b0: 7420 446f 636b 6572 2069 7320 696e 7374  t Docker is inst
+000004c0: 616c 6c65 6420 6f6e 2079 6f75 7220 6d61  alled on your ma
+000004d0: 6368 696e 652e 2049 6620 446f 636b 6572  chine. If Docker
+000004e0: 2069 7320 6e6f 7420 616c 7265 6164 790a   is not already.
+000004f0: 696e 7374 616c 6c65 642c 2079 6f75 2063  installed, you c
+00000500: 616e 2064 6f77 6e6c 6f61 6420 616e 6420  an download and 
+00000510: 696e 7374 616c 6c20 6974 2066 726f 6d20  install it from 
+00000520: 7468 6520 6f66 6669 6369 616c 0a5b 446f  the official.[Do
+00000530: 636b 6572 2077 6562 7369 7465 5d28 6874  cker website](ht
+00000540: 7470 733a 2f2f 7777 772e 646f 636b 6572  tps://www.docker
+00000550: 2e63 6f6d 2f67 6574 2d73 7461 7274 6564  .com/get-started
+00000560: 292e 0a0a 2323 2323 2323 2053 7465 7020  )...###### Step 
+00000570: 323a 2055 7365 2064 6f63 6b65 7220 746f  2: Use docker to
+00000580: 2069 6e73 7461 6c6c 2073 616e 6b61 6b75   install sankaku
+00000590: 0a0a 4f70 656e 2061 2063 6f6d 6d61 6e64  ..Open a command
+000005a0: 2070 726f 6d70 742e 204e 6176 6967 6174   prompt. Navigat
+000005b0: 6520 746f 2074 6865 2064 6972 6563 746f  e to the directo
+000005c0: 7279 2077 6865 7265 2079 6f75 2077 616e  ry where you wan
+000005d0: 740a 746f 2069 6e73 7461 6c6c 2053 616e  t.to install San
+000005e0: 6b61 6b75 2e20 5479 7065 2074 6865 2066  kaku. Type the f
+000005f0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000600: 3a0a 0a60 6060 636f 6d6d 616e 646c 696e  :..```commandlin
+00000610: 650a 6769 7420 636c 6f6e 6520 6874 7470  e.git clone http
+00000620: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f7a  s://github.com/z
+00000630: 6572 6578 3239 302f 7361 6e6b 616b 752e  erex290/sankaku.
+00000640: 6769 740a 6364 2073 616e 6b61 6b75 0a64  git.cd sankaku.d
+00000650: 6f63 6b65 7220 7275 6e20 2d69 7420 2d2d  ocker run -it --
+00000660: 6e61 6d65 2073 616e 6b61 6b75 202d 7720  name sankaku -w 
+00000670: 2f6f 7074 202d 7624 2870 7764 293a 2f6f  /opt -v$(pwd):/o
+00000680: 7074 2070 7974 686f 6e3a 332e 3131 2062  pt python:3.11 b
+00000690: 6173 680a 6060 600a 0a23 2320 5573 6167  ash.```..## Usag
+000006a0: 6520 6578 616d 706c 650a 0a49 7427 7320  e example..It's 
+000006b0: 7665 7279 2073 696d 706c 6520 746f 2075  very simple to u
+000006c0: 7365 2061 6e64 2064 6f65 736e 2774 2072  se and doesn't r
+000006d0: 6571 7569 7265 2074 6f20 616c 7761 7973  equire to always
+000006e0: 206b 6565 7020 6f70 656e 6564 2062 726f   keep opened bro
+000006f0: 7773 6572 2070 6167 650a 7769 7468 2064  wser page.with d
+00000700: 6f63 756d 656e 7461 7469 6f6e 2062 6563  ocumentation bec
+00000710: 6175 7365 2061 6c6c 206d 6574 686f 6473  ause all methods
+00000720: 2061 7265 2073 656c 662d 6578 706c 616e   are self-explan
+00000730: 6174 6f72 793a 0a0a 6060 6070 790a 696d  atory:..```py.im
+00000740: 706f 7274 2061 7379 6e63 696f 0a66 726f  port asyncio.fro
+00000750: 6d20 7361 6e6b 616b 7520 696d 706f 7274  m sankaku import
+00000760: 2053 616e 6b61 6b75 436c 6965 6e74 0a0a   SankakuClient..
+00000770: 6173 796e 6320 6465 6620 6d61 696e 2829  async def main()
+00000780: 3a0a 2020 2020 636c 6965 6e74 203d 2053  :.    client = S
+00000790: 616e 6b61 6b75 436c 6965 6e74 2829 0a0a  ankakuClient()..
+000007a0: 2020 2020 706f 7374 203d 2061 7761 6974      post = await
+000007b0: 2063 6c69 656e 742e 6765 745f 706f 7374   client.get_post
+000007c0: 2832 3537 3432 3036 3429 0a20 2020 2070  (25742064).    p
+000007d0: 7269 6e74 2866 2252 6174 696e 673a 207b  rint(f"Rating: {
+000007e0: 706f 7374 2e72 6174 696e 677d 207c 2043  post.rating} | C
+000007f0: 7265 6174 6564 3a20 7b70 6f73 742e 6372  reated: {post.cr
+00000800: 6561 7465 645f 6174 7d22 290a 2020 2020  eated_at}").    
+00000810: 2320 2252 6174 696e 673a 2052 6174 696e  # "Rating: Ratin
+00000820: 672e 5155 4553 5449 4f4e 4142 4c45 207c  g.QUESTIONABLE |
+00000830: 2043 7265 6174 6564 3a20 3230 3231 2d30   Created: 2021-0
+00000840: 382d 3031 2032 333a 3138 3a35 322b 3033  8-01 23:18:52+03
+00000850: 3a30 3022 0a0a 2020 2020 6177 6169 7420  :00"..    await 
+00000860: 636c 6965 6e74 2e6c 6f67 696e 2861 6363  client.login(acc
+00000870: 6573 735f 746f 6b65 6e3d 2274 6f6b 656e  ess_token="token
+00000880: 2229 0a20 2020 2023 204f 7220 796f 7520  ").    # Or you 
+00000890: 6361 6e20 6175 7468 6f72 697a 6520 6279  can authorize by
+000008a0: 2063 7265 6465 6e74 6961 6c73 3a0a 2020   credentials:.  
+000008b0: 2020 2320 6177 6169 7420 636c 6965 6e74    # await client
+000008c0: 2e6c 6f67 696e 286c 6f67 696e 3d22 6e69  .login(login="ni
+000008d0: 636b 6e61 6d65 206f 7220 656d 6169 6c22  ckname or email"
+000008e0: 2c20 7061 7373 776f 7264 3d22 7061 7373  , password="pass
+000008f0: 776f 7264 2229 0a20 2020 2061 7379 6e63  word").    async
+00000900: 2066 6f72 2062 6f6f 6b20 696e 2063 6c69   for book in cli
+00000910: 656e 742e 6765 745f 7265 6365 6e74 6c79  ent.get_recently
+00000920: 5f72 6561 645f 626f 6f6b 7328 293a 0a20  _read_books():. 
+00000930: 2020 2020 2020 202e 2e2e 0a0a 6173 796e         .....asyn
+00000940: 6369 6f2e 7275 6e28 6d61 696e 2829 290a  cio.run(main()).
+00000950: 6060 600a                                ```.
```

### Comparing `sankaku-1.0.0/sankaku/clients/abc.py` & `sankaku-1.0.1/sankaku/clients/abc.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/clients/clients.py` & `sankaku-1.0.1/sankaku/clients/clients.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,17 +75,18 @@
         login: Optional[str] = None,
         password: Optional[str] = None
     ) -> None:
         """Login into sankakucomplex.com via access token or credentials.
         In case when all arguments are specified, preference will be given
         to authorization by credentials.
 
-        :param access_token: User access token
-        :param login: User email or nickname
-        :param password: User password
+        Args:
+            access_token: User access token
+            login: User email or nickname
+            password: User password
         """
         match (access_token, login, password):
             case [str(), str(), str()] | [_, str(), str()]:
                 await self._login_via_credentials(login, password)  # type: ignore[arg-type]
             case [str(), _, _]:
                 await self._login_via_access_token(access_token)  # type: ignore[arg-type]
             case _:
@@ -124,29 +125,30 @@
         *,
         page_number: Optional[int] = None,
         limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
 
     ) -> AsyncIterator[mdl.Post]:
         """Get posts from post pages.
 
-        :param order: Post order rule
-        :param date: Date or range of dates
-        :param rating: Post rating
-        :param threshold: Vote (quality) filter of posts
-        :param hide_posts_in_books: Whether show post from books or not
-        :param file_size: Size (aspect ratio) of mediafile
-        :param file_type: Type of mediafile in post
-        :param video_duration: Video duration in seconds or in range of seconds
-        :param recommended_for: Posts recommended for specified user
-        :param favorited_by: Posts favorited by specified user
-        :param tags: Tags available for search
-        :param added_by: Posts uploaded by specified users
-        :param voted: Posts voted by specified user
-        :param page_number: Page number from which to start iteration
-        :param limit: Maximum amount of posts per page
+        Args:
+            order: Post order rule
+            date: Date or range of dates
+            rating: Post rating
+            threshold: Vote (quality) filter of posts
+            hide_posts_in_books: Whether show post from books or not
+            file_size: Size (aspect ratio) of mediafile
+            file_type: Type of mediafile in post
+            video_duration: Video duration in seconds or in range of seconds
+            recommended_for: Posts recommended for specified user
+            favorited_by: Posts favorited by specified user
+            tags: Tags available for search
+            added_by: Posts uploaded by specified users
+            voted: Posts voted by specified user
+            page_number: Page number from which to start iteration
+            limit: Maximum amount of posts per page
         """
         async for page in PostPaginator(
             self._http_client, const.POST_URL, **from_locals(locals())
         ):
             for post in page.items:
                 yield post
 
@@ -211,16 +213,17 @@
         self,
         *,
         page_number: Optional[int] = None,
         limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
     ) -> AsyncIterator[mdl.AIPost]:
         """Get AI created posts from AI dedicated post pages.
 
-        :param page_number: Page number from which to start iteration
-        :param limit: Maximum amount of posts per page
+        Args:
+            page_number: Page number from which to start iteration
+            limit: Maximum amount of posts per page
         """
         async for page in Paginator(
             self._http_client, const.AI_POST_URL,
             mdl.AIPost, **from_locals(locals())
         ):
             for post in page.items:
                 yield post
@@ -251,22 +254,23 @@
         *,
         page_number: Optional[int] = None,
         limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
 
     ) -> AsyncIterator[mdl.PageTag]:
         """Get tags from tag pages.
 
-        :param tag_type: Tag type filter
-        :param order: Tag order rule
-        :param rating: Tag rating
-        :param max_post_count: Upper threshold for number of posts with tags found
-        :param sort_parameter: Tag sorting parameter
-        :param sort_direction: Tag sorting direction
-        :param page_number: Page number from which to start iteration
-        :param limit: Maximum amount of tags per page
+        Args:
+            tag_type: Tag type filter
+            order: Tag order rule
+            rating: Tag rating
+            max_post_count: Upper threshold for number of posts with tags found
+            sort_parameter: Tag sorting parameter
+            sort_direction: Tag sorting direction
+            page_number: Page number from which to start iteration
+            limit: Maximum amount of tags per page
         """
         async for page in TagPaginator(
             self._http_client, const.TAG_URL, **from_locals(locals())
         ):
             for tag in page.items:
                 yield tag
 
@@ -296,23 +300,24 @@
         voted: Optional[str] = None,
         *,
         page_number: Optional[int] = None,
         limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
     ) -> AsyncIterator[mdl.PageBook]:
         """Get books from book (pool) pages.
 
-        :param order: Book order rule
-        :param rating: Books rating
-        :param recommended_for: Books recommended for specified user
-        :param favorited_by: Books favorited by specified user
-        :param tags: Tags available for search
-        :param added_by: Books uploaded by specified users
-        :param voted: Books voted by specified user
-        :param page_number: Page number from which to start iteration
-        :param limit: Maximum amount of books per page
+        Args:
+            order: Book order rule
+            rating: Books rating
+            recommended_for: Books recommended for specified user
+            favorited_by: Books favorited by specified user
+            tags: Tags available for search
+            added_by: Books uploaded by specified users
+            voted: Books voted by specified user
+            page_number: Page number from which to start iteration
+            limit: Maximum amount of books per page
         """
         async for page in BookPaginator(
             self._http_client, const.BOOK_URL, **from_locals(locals())
         ):
             for book in page.items:
                 yield book
 
@@ -366,18 +371,19 @@
         level: Optional[types.UserLevel] = None,
         *,
         page_number: Optional[int] = None,
         limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
     ) -> AsyncIterator[mdl.User]:
         """Get user profiles from user pages.
 
-        :param order: User order rule
-        :param level: User level type
-        :param page_number: Page number from which to start iteration
-        :param limit: Maximum amount of users per page
+        Args:
+            order: User order rule
+            level: User level type
+            page_number: Page number from which to start iteration
+            limit: Maximum amount of users per page
         """
         async for page in UserPaginator(
             self._http_client, const.USER_URL, **from_locals(locals())
         ):
             for user in page.items:
                 yield user
```

### Comparing `sankaku-1.0.0/sankaku/clients/http_client.py` & `sankaku-1.0.1/sankaku/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/constants.py` & `sankaku-1.0.1/sankaku/constants.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/errors.py` & `sankaku-1.0.1/sankaku/errors.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/models/books.py` & `sankaku-1.0.1/sankaku/models/books.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/models/posts.py` & `sankaku-1.0.1/sankaku/models/posts.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/models/tags.py` & `sankaku-1.0.1/sankaku/models/tags.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/models/users.py` & `sankaku-1.0.1/sankaku/models/users.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/paginators/abc.py` & `sankaku-1.0.1/sankaku/paginators/abc.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/paginators/paginators.py` & `sankaku-1.0.1/sankaku/paginators/paginators.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/types.py` & `sankaku-1.0.1/sankaku/types.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.0/sankaku/utils.py` & `sankaku-1.0.1/sankaku/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,32 +19,32 @@
 
 
 def ratelimit(
     *,
     rps: Optional[int] = None,
     rpm: Optional[int] = None
 ) -> Callable[[Callable[_P, Awaitable[_T]]], Callable[_P, Awaitable[_T]]]:
-    """
-    Limit the number of requests.
+    """Limit the number of requests.
 
-    :param rps: Request per second
-    :param rpm: Requests per minute
+    Args:
+        rps: Request per second
+        rpm: Requests per minute
     """
     if all(locals().values()):
         raise RateLimitError
     elif not any(locals().values()):
         raise TypeError("At least one argument must be specified.")
 
     sleep_time: float = (1 / rps) if rps else (60 / rpm)  # type: ignore[operator]
 
     def wrapper(func: Callable[_P, Awaitable[_T]]) -> Callable[_P, Awaitable[_T]]:
         @wraps(func)
         async def inner(*args: _P.args, **kwargs: _P.kwargs) -> _T:
             await asyncio.sleep(sleep_time)
-            return await func(*args, **kwargs)
+            return await func(*args, **kwargs)  # noqa
         return inner
 
     return wrapper
 
 
 def convert_ts_to_datetime(ts: Timestamp) -> Optional[datetime]:
     """Convert timestamp in datetime dict into datetime class."""
@@ -54,11 +54,12 @@
 
 
 def from_locals(
     loc: dict[str, Any], exclude: tuple[str, ...] = ("self",)
 ) -> dict[str, Any]:
     """Get arguments of calling function from its locals to pass them to paginator.
 
-    :param loc: locals of calling function
-    :param exclude: arguments to be excluded
+    Args:
+        loc: locals of calling function
+        exclude: arguments to be excluded
     """
     return {k: v for k, v in loc.copy().items() if k not in exclude}
```

### Comparing `sankaku-1.0.0/sankaku.egg-info/PKG-INFO` & `sankaku-1.0.1/sankaku.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7361 6e6b  : 2.1.Name: sank
 00000020: 616b 750a 5665 7273 696f 6e3a 2031 2e30  aku.Version: 1.0
-00000030: 2e30 0a53 756d 6d61 7279 3a20 4173 796e  .0.Summary: Asyn
+00000030: 2e31 0a53 756d 6d61 7279 3a20 4173 796e  .1.Summary: Asyn
 00000040: 6368 726f 6e6f 7573 2041 5049 2077 7261  chronous API wra
 00000050: 7070 6572 2066 6f72 2053 616e 6b61 6b75  pper for Sankaku
 00000060: 2043 6f6d 706c 6578 2e0a 486f 6d65 2d70   Complex..Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 7a65 7265 7832 3930  hub.com/zerex290
 00000090: 2f73 616e 6b61 6b75 0a41 7574 686f 723a  /sankaku.Author:
 000000a0: 207a 6572 6578 3239 300a 4175 7468 6f72   zerex290.Author
@@ -30,104 +30,156 @@
 000001d0: 6570 656e 6465 6e74 0a52 6571 7569 7265  ependent.Require
 000001e0: 732d 5079 7468 6f6e 3a20 3e3d 332e 3131  s-Python: >=3.11
 000001f0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 00000200: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 00000210: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
 00000220: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
 00000230: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000240: 7222 3e0a 2020 3c61 3e0a 2020 2020 3c69  r">.  <a>.    <i
-00000250: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000260: 6265 7461 2e73 616e 6b61 6b75 636f 6d70  beta.sankakucomp
-00000270: 6c65 782e 636f 6d2f 696d 6167 6573 2f61  lex.com/images/a
-00000280: 7070 6c65 2d74 6f75 6368 2d69 636f 6e2e  pple-touch-icon.
-00000290: 706e 6722 200a 2020 2020 7769 6474 683d  png" .    width=
-000002a0: 2231 3530 2220 6865 6967 6874 3d22 3135  "150" height="15
-000002b0: 3022 3e0a 2020 3c2f 613e 0a20 203c 6469  0">.  </a>.  <di
-000002c0: 763e 7361 6e6b 616b 753c 2f64 6976 3e0a  v>sankaku</div>.
-000002d0: 3c2f 6831 3e0a 3c70 2061 6c69 676e 3d22  </h1>.<p align="
-000002e0: 6365 6e74 6572 223e 3c65 6d3e 3c62 3e46  center"><em><b>F
-000002f0: 6f72 2072 6561 6c20 6d65 6e20 6f66 2063  or real men of c
-00000300: 756c 7475 7265 203c 2f62 3e3c 2f65 6d3e  ulture </b></em>
-00000310: 2623 3132 3835 3237 3c2f 703e 0a0a 2323  &#128527</p>..##
-00000320: 2041 626f 7574 0a0a 4173 796e 6368 726f   About..Asynchro
-00000330: 6e6f 7573 2041 5049 2077 7261 7070 6572  nous API wrapper
-00000340: 2066 6f72 205b 5361 6e6b 616b 7520 436f   for [Sankaku Co
-00000350: 6d70 6c65 785d 2868 7474 7073 3a2f 2f62  mplex](https://b
-00000360: 6574 612e 7361 6e6b 616b 7563 6f6d 706c  eta.sankakucompl
-00000370: 6578 2e63 6f6d 290a 7769 7468 202a 7479  ex.com).with *ty
-00000380: 7065 2d68 696e 7469 6e67 2a2c 2070 7964  pe-hinting*, pyd
-00000390: 616e 7469 6320 2a64 6174 6120 7661 6c69  antic *data vali
-000003a0: 6461 7469 6f6e 2a20 616e 6420 616e 206f  dation* and an o
-000003b0: 7074 696f 6e61 6c20 2a6c 6f67 6769 6e67  ptional *logging
-000003c0: 2073 7570 706f 7274 2a0a 7769 7468 206c   support*.with l
-000003d0: 6f67 7572 752e 0a0a 2323 2320 4665 6174  oguru...### Feat
-000003e0: 7572 6573 3a0a 0a2d 2054 7970 652d 6869  ures:..- Type-hi
-000003f0: 6e74 730a 2d20 4465 7365 7269 616c 697a  nts.- Deserializ
-00000400: 6174 696f 6e20 6f66 2072 6177 206a 736f  ation of raw jso
-00000410: 6e20 6461 7461 2074 6861 6e6b 7320 746f  n data thanks to
-00000420: 2070 7964 616e 7469 6320 6d6f 6465 6c73   pydantic models
-00000430: 0a2d 2045 6e75 6d65 7261 7469 6f6e 7320  .- Enumerations 
-00000440: 666f 7220 4150 4920 7265 7175 6573 7420  for API request 
-00000450: 7061 7261 6d65 7465 7273 2074 6f20 7072  parameters to pr
-00000460: 6f76 6964 6520 6265 7474 6572 2075 7365  ovide better use
-00000470: 7220 6578 7065 7269 656e 6365 0a20 203e  r experience.  >
-00000480: 2046 6f72 2069 6e73 7461 6e63 652c 2079   For instance, y
-00000490: 6f75 2063 616e 2074 7970 6520 6074 7970  ou can type `typ
-000004a0: 6573 2e54 6167 5479 7065 2e41 5254 4953  es.TagType.ARTIS
-000004b0: 5460 2069 6e73 7465 6164 206f 6620 6074  T` instead of `t
-000004c0: 7970 6573 5b5d 3d31 600a 0a2d 2d2d 0a0a  ypes[]=1`..---..
-000004d0: 446f 6375 6d65 6e74 6174 696f 6e3a 2054  Documentation: T
-000004e0: 4241 0a0a 536f 7572 6365 2063 6f64 653a  BA..Source code:
-000004f0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000500: 636f 6d2f 7a65 7265 7832 3930 2f73 616e  com/zerex290/san
-00000510: 6b61 6b75 0a0a 2d2d 2d0a 0a23 2320 5265  kaku..---..## Re
-00000520: 7175 6972 656d 656e 7473 0a0a 2d20 5079  quirements..- Py
-00000530: 7468 6f6e 2033 2e31 312b 0a2d 2061 696f  thon 3.11+.- aio
-00000540: 6874 7470 0a2d 2070 7964 616e 7469 630a  http.- pydantic.
-00000550: 2d20 6c6f 6775 7275 0a0a 2323 2049 6e73  - loguru..## Ins
-00000560: 7461 6c6c 6174 696f 6e0a 0a60 6060 636f  tallation..```co
-00000570: 6d6d 616e 646c 696e 650a 7069 7020 696e  mmandline.pip in
-00000580: 7374 616c 6c20 7361 6e6b 616b 750a 6060  stall sankaku.``
-00000590: 600a 0a23 2320 4578 616d 706c 650a 0a49  `..## Example..I
-000005a0: 7427 7320 7665 7279 2073 696d 706c 6520  t's very simple 
-000005b0: 746f 2075 7365 2061 6e64 2064 6f65 736e  to use and doesn
-000005c0: 2774 2072 6571 7569 7265 2074 6f20 616c  't require to al
-000005d0: 7761 7973 206b 6565 7020 6f70 656e 6564  ways keep opened
-000005e0: 2062 726f 7773 6572 2070 6167 650a 7769   browser page.wi
-000005f0: 7468 2064 6f63 756d 656e 7461 7469 6f6e  th documentation
-00000600: 2062 6563 6175 7365 2061 6c6c 206d 6574   because all met
-00000610: 686f 6473 2061 7265 2073 656c 662d 6578  hods are self-ex
-00000620: 706c 616e 6174 6f72 792e 0a0a 6060 6070  planatory...```p
-00000630: 790a 696d 706f 7274 2061 7379 6e63 696f  y.import asyncio
-00000640: 0a66 726f 6d20 7361 6e6b 616b 7520 696d  .from sankaku im
-00000650: 706f 7274 2053 616e 6b61 6b75 436c 6965  port SankakuClie
-00000660: 6e74 0a0a 6173 796e 6320 6465 6620 6d61  nt..async def ma
-00000670: 696e 2829 3a0a 2020 2020 636c 6965 6e74  in():.    client
-00000680: 203d 2053 616e 6b61 6b75 436c 6965 6e74   = SankakuClient
-00000690: 2829 0a0a 2020 2020 706f 7374 203d 2061  ()..    post = a
-000006a0: 7761 6974 2063 6c69 656e 742e 6765 745f  wait client.get_
-000006b0: 706f 7374 2832 3537 3432 3036 3429 0a20  post(25742064). 
-000006c0: 2020 2070 7269 6e74 2866 2252 6174 696e     print(f"Ratin
-000006d0: 673a 207b 706f 7374 2e72 6174 696e 677d  g: {post.rating}
-000006e0: 207c 2043 7265 6174 6564 3a20 7b70 6f73   | Created: {pos
-000006f0: 742e 6372 6561 7465 645f 6174 7d22 290a  t.created_at}").
-00000700: 2020 2020 2320 2252 6174 696e 673a 2052      # "Rating: R
-00000710: 6174 696e 672e 5155 4553 5449 4f4e 4142  ating.QUESTIONAB
-00000720: 4c45 207c 2043 7265 6174 6564 3a20 3230  LE | Created: 20
-00000730: 3231 2d30 382d 3031 2032 333a 3138 3a35  21-08-01 23:18:5
-00000740: 322b 3033 3a30 3022 0a0a 2020 2020 6177  2+03:00"..    aw
-00000750: 6169 7420 636c 6965 6e74 2e6c 6f67 696e  ait client.login
-00000760: 2861 6363 6573 735f 746f 6b65 6e3d 2274  (access_token="t
-00000770: 6f6b 656e 2229 0a20 2020 2023 204f 7220  oken").    # Or 
-00000780: 796f 7520 6361 6e20 6175 7468 6f72 697a  you can authoriz
-00000790: 6520 6279 2063 7265 6465 6e74 6961 6c73  e by credentials
-000007a0: 3a0a 2020 2020 2320 6177 6169 7420 636c  :.    # await cl
-000007b0: 6965 6e74 2e6c 6f67 696e 286c 6f67 696e  ient.login(login
-000007c0: 3d22 6e69 636b 6e61 6d65 206f 7220 656d  ="nickname or em
-000007d0: 6169 6c22 2c20 7061 7373 776f 7264 3d22  ail", password="
-000007e0: 7061 7373 776f 7264 2229 0a20 2020 2061  password").    a
-000007f0: 7379 6e63 2066 6f72 2062 6f6f 6b20 696e  sync for book in
-00000800: 2063 6c69 656e 742e 6765 745f 7265 6365   client.get_rece
-00000810: 6e74 6c79 5f72 6561 645f 626f 6f6b 7328  ntly_read_books(
-00000820: 293a 0a20 2020 2020 2020 202e 2e2e 0a0a  ):.        .....
-00000830: 6173 796e 6369 6f2e 7275 6e28 6d61 696e  asyncio.run(main
-00000840: 2829 290a 6060 600a                      ()).```.
+00000240: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
+00000250: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000260: 6d2f 7a65 7265 7832 3930 2f73 616e 6b61  m/zerex290/sanka
+00000270: 6b75 223e 0a20 2020 203c 696d 6720 7372  ku">.    <img sr
+00000280: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000290: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000002a0: 2e63 6f6d 2f7a 6572 6578 3239 302f 7361  .com/zerex290/sa
+000002b0: 6e6b 616b 752f 6d61 696e 2f64 6f63 732f  nkaku/main/docs/
+000002c0: 6963 6f6e 2e70 6e67 2220 616c 743d 2253  icon.png" alt="S
+000002d0: 616e 6b61 6b75 2043 6f6d 706c 6578 220a  ankaku Complex".
+000002e0: 2020 2020 7769 6474 683d 2231 3530 2220      width="150" 
+000002f0: 6865 6967 6874 3d22 3135 3022 2f3e 0a20  height="150"/>. 
+00000300: 203c 2f61 3e0a 2020 3c64 6976 3e73 616e   </a>.  <div>san
+00000310: 6b61 6b75 3c2f 6469 763e 0a3c 2f68 313e  kaku</div>.</h1>
+00000320: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000330: 7222 3e3c 656d 3e3c 623e 466f 7220 7265  r"><em><b>For re
+00000340: 616c 206d 656e 206f 6620 6375 6c74 7572  al men of cultur
+00000350: 6520 3c2f 623e 3c2f 656d 3e3c 2f70 3e0a  e </b></em></p>.
+00000360: 0a23 2320 4162 6f75 740a 0a41 7379 6e63  .## About..Async
+00000370: 6872 6f6e 6f75 7320 4150 4920 7772 6170  hronous API wrap
+00000380: 7065 7220 666f 7220 5b53 616e 6b61 6b75  per for [Sankaku
+00000390: 2043 6f6d 706c 6578 5d28 6874 7470 733a   Complex](https:
+000003a0: 2f2f 6265 7461 2e73 616e 6b61 6b75 636f  //beta.sankakuco
+000003b0: 6d70 6c65 782e 636f 6d29 0a77 6974 6820  mplex.com).with 
+000003c0: 2a74 7970 652d 6869 6e74 696e 672a 2c20  *type-hinting*, 
+000003d0: 7079 6461 6e74 6963 202a 6461 7461 2076  pydantic *data v
+000003e0: 616c 6964 6174 696f 6e2a 2061 6e64 2061  alidation* and a
+000003f0: 6e20 6f70 7469 6f6e 616c 202a 6c6f 6767  n optional *logg
+00000400: 696e 6720 7375 7070 6f72 742a 0a77 6974  ing support*.wit
+00000410: 6820 6c6f 6775 7275 2e0a 0a23 2323 2046  h loguru...### F
+00000420: 6561 7475 7265 733a 0a0a 2d20 5479 7065  eatures:..- Type
+00000430: 2d68 696e 7473 0a2d 2044 6573 6572 6961  -hints.- Deseria
+00000440: 6c69 7a61 7469 6f6e 206f 6620 7261 7720  lization of raw 
+00000450: 6a73 6f6e 2064 6174 6120 7468 616e 6b73  json data thanks
+00000460: 2074 6f20 7079 6461 6e74 6963 206d 6f64   to pydantic mod
+00000470: 656c 730a 2d20 456e 756d 6572 6174 696f  els.- Enumeratio
+00000480: 6e73 2066 6f72 2041 5049 2072 6571 7565  ns for API reque
+00000490: 7374 2070 6172 616d 6574 6572 7320 746f  st parameters to
+000004a0: 2070 726f 7669 6465 2062 6574 7465 7220   provide better 
+000004b0: 7573 6572 2065 7870 6572 6965 6e63 650a  user experience.
+000004c0: 2020 3e20 466f 7220 696e 7374 616e 6365    > For instance
+000004d0: 2c20 796f 7520 6361 6e20 7479 7065 2060  , you can type `
+000004e0: 7479 7065 732e 5461 6754 7970 652e 4152  types.TagType.AR
+000004f0: 5449 5354 6020 696e 7374 6561 6420 6f66  TIST` instead of
+00000500: 2060 7479 7065 735b 5d3d 3160 0a0a 2d2d   `types[]=1`..--
+00000510: 2d0a 0a44 6f63 756d 656e 7461 7469 6f6e  -..Documentation
+00000520: 3a20 6874 7470 733a 2f2f 7a65 7265 7832  : https://zerex2
+00000530: 3930 2e67 6974 6875 622e 696f 2f73 616e  90.github.io/san
+00000540: 6b61 6b75 0a0a 4150 4920 5265 6665 7265  kaku..API Refere
+00000550: 6e63 653a 2068 7474 7073 3a2f 2f7a 6572  nce: https://zer
+00000560: 6578 3239 302e 6769 7468 7562 2e69 6f2f  ex290.github.io/
+00000570: 7361 6e6b 616b 752f 6170 690a 0a53 6f75  sankaku/api..Sou
+00000580: 7263 6520 636f 6465 3a20 6874 7470 733a  rce code: https:
+00000590: 2f2f 6769 7468 7562 2e63 6f6d 2f7a 6572  //github.com/zer
+000005a0: 6578 3239 302f 7361 6e6b 616b 750a 0a2d  ex290/sankaku..-
+000005b0: 2d2d 0a0a 2323 2052 6571 7569 7265 6d65  --..## Requireme
+000005c0: 6e74 730a 0a2d 2050 7974 686f 6e20 332e  nts..- Python 3.
+000005d0: 3131 2b0a 2d20 6169 6f68 7474 700a 2d20  11+.- aiohttp.- 
+000005e0: 7079 6461 6e74 6963 0a2d 206c 6f67 7572  pydantic.- logur
+000005f0: 750a 0a23 2320 496e 7374 616c 6c61 7469  u..## Installati
+00000600: 6f6e 0a0a 546f 2069 6e73 7461 6c6c 2073  on..To install s
+00000610: 616e 6b61 6b75 2076 6961 2070 6970 2077  ankaku via pip w
+00000620: 7269 7465 2066 6f6c 6c6f 7769 6e67 206c  rite following l
+00000630: 696e 6520 6f66 2063 6f64 6520 696e 2079  ine of code in y
+00000640: 6f75 7220 7465 726d 696e 616c 3a0a 0a60  our terminal:..`
+00000650: 6060 636f 6d6d 616e 646c 696e 650a 7069  ``commandline.pi
+00000660: 7020 696e 7374 616c 6c20 7361 6e6b 616b  p install sankak
+00000670: 750a 6060 600a 0a54 6f20 696e 7374 616c  u.```..To instal
+00000680: 6c20 7468 6520 7361 6e6b 616b 7520 7669  l the sankaku vi
+00000690: 6120 446f 636b 6572 2c20 796f 7520 6361  a Docker, you ca
+000006a0: 6e20 666f 6c6c 6f77 2074 6865 7365 2073  n follow these s
+000006b0: 7465 7073 3a0a 0a23 2323 2323 2320 5374  teps:..###### St
+000006c0: 6570 2031 3a20 496e 7374 616c 6c20 446f  ep 1: Install Do
+000006d0: 636b 6572 0a0a 456e 7375 7265 2074 6861  cker..Ensure tha
+000006e0: 7420 446f 636b 6572 2069 7320 696e 7374  t Docker is inst
+000006f0: 616c 6c65 6420 6f6e 2079 6f75 7220 6d61  alled on your ma
+00000700: 6368 696e 652e 2049 6620 446f 636b 6572  chine. If Docker
+00000710: 2069 7320 6e6f 7420 616c 7265 6164 790a   is not already.
+00000720: 696e 7374 616c 6c65 642c 2079 6f75 2063  installed, you c
+00000730: 616e 2064 6f77 6e6c 6f61 6420 616e 6420  an download and 
+00000740: 696e 7374 616c 6c20 6974 2066 726f 6d20  install it from 
+00000750: 7468 6520 6f66 6669 6369 616c 0a5b 446f  the official.[Do
+00000760: 636b 6572 2077 6562 7369 7465 5d28 6874  cker website](ht
+00000770: 7470 733a 2f2f 7777 772e 646f 636b 6572  tps://www.docker
+00000780: 2e63 6f6d 2f67 6574 2d73 7461 7274 6564  .com/get-started
+00000790: 292e 0a0a 2323 2323 2323 2053 7465 7020  )...###### Step 
+000007a0: 323a 2055 7365 2064 6f63 6b65 7220 746f  2: Use docker to
+000007b0: 2069 6e73 7461 6c6c 2073 616e 6b61 6b75   install sankaku
+000007c0: 0a0a 4f70 656e 2061 2063 6f6d 6d61 6e64  ..Open a command
+000007d0: 2070 726f 6d70 742e 204e 6176 6967 6174   prompt. Navigat
+000007e0: 6520 746f 2074 6865 2064 6972 6563 746f  e to the directo
+000007f0: 7279 2077 6865 7265 2079 6f75 2077 616e  ry where you wan
+00000800: 740a 746f 2069 6e73 7461 6c6c 2053 616e  t.to install San
+00000810: 6b61 6b75 2e20 5479 7065 2074 6865 2066  kaku. Type the f
+00000820: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000830: 3a0a 0a60 6060 636f 6d6d 616e 646c 696e  :..```commandlin
+00000840: 650a 6769 7420 636c 6f6e 6520 6874 7470  e.git clone http
+00000850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f7a  s://github.com/z
+00000860: 6572 6578 3239 302f 7361 6e6b 616b 752e  erex290/sankaku.
+00000870: 6769 740a 6364 2073 616e 6b61 6b75 0a64  git.cd sankaku.d
+00000880: 6f63 6b65 7220 7275 6e20 2d69 7420 2d2d  ocker run -it --
+00000890: 6e61 6d65 2073 616e 6b61 6b75 202d 7720  name sankaku -w 
+000008a0: 2f6f 7074 202d 7624 2870 7764 293a 2f6f  /opt -v$(pwd):/o
+000008b0: 7074 2070 7974 686f 6e3a 332e 3131 2062  pt python:3.11 b
+000008c0: 6173 680a 6060 600a 0a23 2320 5573 6167  ash.```..## Usag
+000008d0: 6520 6578 616d 706c 650a 0a49 7427 7320  e example..It's 
+000008e0: 7665 7279 2073 696d 706c 6520 746f 2075  very simple to u
+000008f0: 7365 2061 6e64 2064 6f65 736e 2774 2072  se and doesn't r
+00000900: 6571 7569 7265 2074 6f20 616c 7761 7973  equire to always
+00000910: 206b 6565 7020 6f70 656e 6564 2062 726f   keep opened bro
+00000920: 7773 6572 2070 6167 650a 7769 7468 2064  wser page.with d
+00000930: 6f63 756d 656e 7461 7469 6f6e 2062 6563  ocumentation bec
+00000940: 6175 7365 2061 6c6c 206d 6574 686f 6473  ause all methods
+00000950: 2061 7265 2073 656c 662d 6578 706c 616e   are self-explan
+00000960: 6174 6f72 793a 0a0a 6060 6070 790a 696d  atory:..```py.im
+00000970: 706f 7274 2061 7379 6e63 696f 0a66 726f  port asyncio.fro
+00000980: 6d20 7361 6e6b 616b 7520 696d 706f 7274  m sankaku import
+00000990: 2053 616e 6b61 6b75 436c 6965 6e74 0a0a   SankakuClient..
+000009a0: 6173 796e 6320 6465 6620 6d61 696e 2829  async def main()
+000009b0: 3a0a 2020 2020 636c 6965 6e74 203d 2053  :.    client = S
+000009c0: 616e 6b61 6b75 436c 6965 6e74 2829 0a0a  ankakuClient()..
+000009d0: 2020 2020 706f 7374 203d 2061 7761 6974      post = await
+000009e0: 2063 6c69 656e 742e 6765 745f 706f 7374   client.get_post
+000009f0: 2832 3537 3432 3036 3429 0a20 2020 2070  (25742064).    p
+00000a00: 7269 6e74 2866 2252 6174 696e 673a 207b  rint(f"Rating: {
+00000a10: 706f 7374 2e72 6174 696e 677d 207c 2043  post.rating} | C
+00000a20: 7265 6174 6564 3a20 7b70 6f73 742e 6372  reated: {post.cr
+00000a30: 6561 7465 645f 6174 7d22 290a 2020 2020  eated_at}").    
+00000a40: 2320 2252 6174 696e 673a 2052 6174 696e  # "Rating: Ratin
+00000a50: 672e 5155 4553 5449 4f4e 4142 4c45 207c  g.QUESTIONABLE |
+00000a60: 2043 7265 6174 6564 3a20 3230 3231 2d30   Created: 2021-0
+00000a70: 382d 3031 2032 333a 3138 3a35 322b 3033  8-01 23:18:52+03
+00000a80: 3a30 3022 0a0a 2020 2020 6177 6169 7420  :00"..    await 
+00000a90: 636c 6965 6e74 2e6c 6f67 696e 2861 6363  client.login(acc
+00000aa0: 6573 735f 746f 6b65 6e3d 2274 6f6b 656e  ess_token="token
+00000ab0: 2229 0a20 2020 2023 204f 7220 796f 7520  ").    # Or you 
+00000ac0: 6361 6e20 6175 7468 6f72 697a 6520 6279  can authorize by
+00000ad0: 2063 7265 6465 6e74 6961 6c73 3a0a 2020   credentials:.  
+00000ae0: 2020 2320 6177 6169 7420 636c 6965 6e74    # await client
+00000af0: 2e6c 6f67 696e 286c 6f67 696e 3d22 6e69  .login(login="ni
+00000b00: 636b 6e61 6d65 206f 7220 656d 6169 6c22  ckname or email"
+00000b10: 2c20 7061 7373 776f 7264 3d22 7061 7373  , password="pass
+00000b20: 776f 7264 2229 0a20 2020 2061 7379 6e63  word").    async
+00000b30: 2066 6f72 2062 6f6f 6b20 696e 2063 6c69   for book in cli
+00000b40: 656e 742e 6765 745f 7265 6365 6e74 6c79  ent.get_recently
+00000b50: 5f72 6561 645f 626f 6f6b 7328 293a 0a20  _read_books():. 
+00000b60: 2020 2020 2020 202e 2e2e 0a0a 6173 796e         .....asyn
+00000b70: 6369 6f2e 7275 6e28 6d61 696e 2829 290a  cio.run(main()).
+00000b80: 6060 600a                                ```.
```

### Comparing `sankaku-1.0.0/sankaku.egg-info/SOURCES.txt` & `sankaku-1.0.1/sankaku.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,10 +22,8 @@
 sankaku/models/http.py
 sankaku/models/pages.py
 sankaku/models/posts.py
 sankaku/models/tags.py
 sankaku/models/users.py
 sankaku/paginators/__init__.py
 sankaku/paginators/abc.py
-sankaku/paginators/paginators.py
-tests/test_clients.py
-tests/test_utils.py
+sankaku/paginators/paginators.py
```

### Comparing `sankaku-1.0.0/setup.py` & `sankaku-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sankaku",
-    version="1.0.0",
+    version="1.0.1",
     author="zerex290",
     author_email="zerex290@gmail.com",
     description="Asynchronous API wrapper for Sankaku Complex.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="sankaku sankakucomplex api".split(),
     url="https://github.com/zerex290/sankaku",
```

