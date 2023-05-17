# Comparing `tmp/lackadaisical-1.0.0a0-py3-none-any.whl.zip` & `tmp/lackadaisical-1.0.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,13 @@
-Zip file size: 1590 bytes, number of entries: 6
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-28 15:00 lackadaisical/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-28 15:00 revers3/__init__.py
--rw-rw-r--  2.0 unx      683 b- defN 23-May-17 15:56 lackadaisical-1.0.0a0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-17 15:56 lackadaisical-1.0.0a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-17 15:56 lackadaisical-1.0.0a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      481 b- defN 23-May-17 15:56 lackadaisical-1.0.0a0.dist-info/RECORD
-6 files, 1270 bytes uncompressed, 704 bytes compressed:  44.6%
+Zip file size: 4276 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        8 b- defN 23-May-17 16:46 lackadaisical/VERSION
+-rw-r--r--  2.0 unx     1167 b- defN 23-May-17 16:46 lackadaisical/__init__.py
+-rw-r--r--  2.0 unx      359 b- defN 23-May-17 16:46 lackadaisical/faster_than.py
+-rw-r--r--  2.0 unx       67 b- defN 23-May-17 16:46 lackadaisical/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-17 16:46 lackadaisical/py.typed
+-rw-r--r--  2.0 unx      368 b- defN 23-May-17 16:46 lackadaisical/too_slow.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      880 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      902 b- defN 23-May-17 16:46 lackadaisical-1.0.0a1.dist-info/RECORD
+11 files, 4930 bytes uncompressed, 2730 bytes compressed:  44.6%
```

## zipnote {}

```diff
@@ -1,19 +1,34 @@
+Filename: lackadaisical/VERSION
+Comment: 
+
 Filename: lackadaisical/__init__.py
 Comment: 
 
-Filename: revers3/__init__.py
+Filename: lackadaisical/faster_than.py
+Comment: 
+
+Filename: lackadaisical/logging.py
+Comment: 
+
+Filename: lackadaisical/py.typed
+Comment: 
+
+Filename: lackadaisical/too_slow.py
+Comment: 
+
+Filename: lackadaisical-1.0.0a1.dist-info/LICENSE
 Comment: 
 
-Filename: lackadaisical-1.0.0a0.dist-info/METADATA
+Filename: lackadaisical-1.0.0a1.dist-info/METADATA
 Comment: 
 
-Filename: lackadaisical-1.0.0a0.dist-info/WHEEL
+Filename: lackadaisical-1.0.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: lackadaisical-1.0.0a0.dist-info/top_level.txt
+Filename: lackadaisical-1.0.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: lackadaisical-1.0.0a0.dist-info/RECORD
+Filename: lackadaisical-1.0.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lackadaisical/__init__.py

```diff
@@ -0,0 +1,73 @@
+00000000: 2222 220a 2320 5375 7070 6f72 740a 0a50  """.# Support..P
+00000010: 6c65 6173 6520 7375 626d 6974 2061 6c6c  lease submit all
+00000020: 2079 6f75 7220 7175 6573 7469 6f6e 732c   your questions,
+00000030: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
+00000040: 7320 616e 6420 6275 6720 7265 706f 7274  s and bug report
+00000050: 7320 6174 0a5b 6769 7468 7562 2e63 6f6d  s at.[github.com
+00000060: 2f63 6172 6961 642f 6c61 636b 6164 6169  /cariad/lackadai
+00000070: 7369 6361 6c2f 6973 7375 6573 5d28 6874  sical/issues](ht
+00000080: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000090: 2f63 6172 6961 642f 6c61 636b 6164 6169  /cariad/lackadai
+000000a0: 7369 6361 6c2f 6973 7375 6573 292e 0a54  sical/issues)..T
+000000b0: 6861 6e6b 2079 6f75 210a 0a23 204c 6963  hank you!..# Lic
+000000c0: 656e 6365 0a0a 4c61 636b 6164 6169 7369  ence..Lackadaisi
+000000d0: 6361 6c20 6973 205b 6f70 656e 2d73 6f75  cal is [open-sou
+000000e0: 7263 655d 2868 7474 7073 3a2f 2f67 6974  rce](https://git
+000000f0: 6875 622e 636f 6d2f 6361 7269 6164 2f6c  hub.com/cariad/l
+00000100: 6163 6b61 6461 6973 6963 616c 2920 616e  ackadaisical) an
+00000110: 640a 7265 6c65 6173 6564 2075 6e64 6572  d.released under
+00000120: 2074 6865 0a5b 4d49 5420 4c69 6365 6e73   the.[MIT Licens
+00000130: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000140: 622e 636f 6d2f 6361 7269 6164 2f6c 6163  b.com/cariad/lac
+00000150: 6b61 6461 6973 6963 616c 2f62 6c6f 622f  kadaisical/blob/
+00000160: 6d61 696e 2f4c 4943 454e 5345 292e 0a0a  main/LICENSE)...
+00000170: 596f 7520 646f 6e27 7420 6861 7665 2074  You don't have t
+00000180: 6f20 6769 7665 2061 7474 7269 6275 7469  o give attributi
+00000190: 6f6e 2069 6e20 796f 7572 2070 726f 6a65  on in your proje
+000001a0: 6374 2c20 6275 7420 2d2d 2061 7320 6120  ct, but -- as a 
+000001b0: 6672 6565 6c61 6e63 650a 6465 7665 6c6f  freelance.develo
+000001c0: 7065 7220 7769 7468 2072 656e 7420 746f  per with rent to
+000001d0: 2070 6179 202d 2d20 4920 6170 7072 6563   pay -- I apprec
+000001e0: 6961 7465 2069 7421 0a0a 2320 4175 7468  iate it!..# Auth
+000001f0: 6f72 0a0a 4865 6c6c 6f21 20f0 9f91 8b20  or..Hello! .... 
+00000200: 4927 6d20 2a2a 4361 7269 6164 2045 6363  I'm **Cariad Ecc
+00000210: 6c65 7374 6f6e 2a2a 2c20 616e 6420 4927  leston**, and I'
+00000220: 6d20 6120 6672 6565 6c61 6e63 6520 416d  m a freelance Am
+00000230: 617a 6f6e 2057 6562 2053 6572 7669 6365  azon Web Service
+00000240: 730a 6172 6368 6974 6563 742c 2044 6576  s.architect, Dev
+00000250: 4f70 7320 6576 616e 6765 6c69 7374 2c20  Ops evangelist, 
+00000260: 4349 2f43 4420 7069 7065 6c69 6e65 2065  CI/CD pipeline e
+00000270: 6e67 696e 6565 7220 616e 6420 6261 636b  ngineer and back
+00000280: 656e 6420 6465 7665 6c6f 7065 722e 0a0a  end developer...
+00000290: 596f 7520 6361 6e20 6669 6e64 206d 6520  You can find me 
+000002a0: 6174 205b 6361 7269 6164 2e65 6172 7468  at [cariad.earth
+000002b0: 5d28 6874 7470 733a 2f2f 7777 772e 6361  ](https://www.ca
+000002c0: 7269 6164 2e65 6172 7468 292c 0a5b 6769  riad.earth),.[gi
+000002d0: 7468 7562 2f63 6172 6961 645d 2868 7474  thub/cariad](htt
+000002e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000002f0: 6361 7269 6164 292c 0a5b 6c69 6e6b 6564  cariad),.[linked
+00000300: 696e 2f63 6172 6961 645d 2868 7474 7073  in/cariad](https
+00000310: 3a2f 2f6c 696e 6b65 6469 6e2e 636f 6d2f  ://linkedin.com/
+00000320: 696e 2f63 6172 6961 6429 2061 6e64 206f  in/cariad) and o
+00000330: 6e20 4d61 7374 6f64 6f6e 2061 740a 5b40  n Mastodon at.[@
+00000340: 6361 7269 6164 4074 6563 682e 6c67 6274  cariad@tech.lgbt
+00000350: 5d28 6874 7470 733a 2f2f 7465 6368 2e6c  ](https://tech.l
+00000360: 6762 742f 4063 6172 6961 6429 2e0a 2222  gbt/@cariad)..""
+00000370: 220a 0a66 726f 6d20 696d 706f 7274 6c69  "..from importli
+00000380: 622e 7265 736f 7572 6365 7320 696d 706f  b.resources impo
+00000390: 7274 206f 7065 6e5f 7465 7874 0a0a 6672  rt open_text..fr
+000003a0: 6f6d 206c 6163 6b61 6461 6973 6963 616c  om lackadaisical
+000003b0: 2e66 6173 7465 725f 7468 616e 2069 6d70  .faster_than imp
+000003c0: 6f72 7420 6173 7365 7274 5f66 6173 7465  ort assert_faste
+000003d0: 725f 7468 616e 0a66 726f 6d20 6c61 636b  r_than.from lack
+000003e0: 6164 6169 7369 6361 6c2e 746f 6f5f 736c  adaisical.too_sl
+000003f0: 6f77 2069 6d70 6f72 7420 546f 6f53 6c6f  ow import TooSlo
+00000400: 770a 0a77 6974 6820 6f70 656e 5f74 6578  w..with open_tex
+00000410: 7428 5f5f 7061 636b 6167 655f 5f2c 2022  t(__package__, "
+00000420: 5645 5253 494f 4e22 2920 6173 2074 3a0a  VERSION") as t:.
+00000430: 2020 2020 5f5f 7665 7273 696f 6e5f 5f20      __version__ 
+00000440: 3d20 742e 7265 6164 6c69 6e65 2829 2e73  = t.readline().s
+00000450: 7472 6970 2829 0a0a 5f5f 616c 6c5f 5f20  trip()..__all__ 
+00000460: 3d20 5b0a 2020 2020 2254 6f6f 536c 6f77  = [.    "TooSlow
+00000470: 222c 0a20 2020 2022 6173 7365 7274 5f66  ",.    "assert_f
+00000480: 6173 7465 725f 7468 616e 222c 0a5d 0a    aster_than",.].
```

## Comparing `lackadaisical-1.0.0a0.dist-info/METADATA` & `lackadaisical-1.0.0a1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: lackadaisical
-Version: 1.0.0a0
-Summary: Keeps an eye on your slow tests
-Home-page: https://github.com/cariad/lackadaisical
+Version: 1.0.0a1
+Summary: Keeps an eye on slow tests
 Author: Cariad Eccleston
 Author-email: cariad@cariad.earth
 License: MIT
+Project-URL: Documentation, https://cariad.github.io/lackadaisical/lackadaisical.html
+Project-URL: Source, https://github.com/cariad/lackadaisical
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Typing :: Typed
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# Lackadaisical
-
-Keeps an eye on your slow tests.
+# lackadaisical
+A Python package to keep an eye on slow tests
```

