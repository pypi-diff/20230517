# Comparing `tmp/alacorder-80.6.0.tar.gz` & `tmp/alacorder-80.6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.0.tar", max compression
+gzip compressed data, was "alacorder-80.6.0.1.tar", max compression
```

## Comparing `alacorder-80.6.0.tar` & `alacorder-80.6.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.0/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.6.0/README.md
--rw-r--r--   0        0        0      746 2023-05-17 17:55:09.872937 alacorder-80.6.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-17 13:55:53.336379 alacorder-80.6.0/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   234285 2023-05-17 17:54:48.794246 alacorder-80.6.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   234285 2023-05-17 17:54:52.738672 alacorder-80.6.0/src/alacorder/alac.py
--rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.0.1/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.0.1/README.md
+-rw-r--r--   0        0        0      748 2023-05-17 18:01:35.060602 alacorder-80.6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-17 17:59:02.346002 alacorder-80.6.0.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.0.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   234285 2023-05-17 17:54:48.794246 alacorder-80.6.0.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   234285 2023-05-17 17:54:52.738672 alacorder-80.6.0.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 alacorder-80.6.0.1/PKG-INFO
```

### Comparing `alacorder-80.6.0/LICENSE` & `alacorder-80.6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.0/README.md` & `alacorder-80.6.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -250,163 +250,155 @@
 00000f90: 6420 5445 5854 2020 2020 2020 2020 2050  d TEXT         P
 00000fa0: 6173 7377 6f72 6420 6f6e 2041 6c61 636f  assword on Alaco
 00000fb0: 7572 742e 636f 6d20 205b 7265 7175 6972  urt.com  [requir
 00000fc0: 6564 5d0a 2020 2d63 7269 6d69 6e61 6c2c  ed].  -criminal,
 00000fd0: 202d 2d63 7269 6d69 6e61 6c2d 6f6e 6c79   --criminal-only
 00000fe0: 2020 4f6e 6c79 2073 6561 7263 6820 6372    Only search cr
 00000ff0: 696d 696e 616c 2063 6173 6573 0a20 202d  iminal cases.  -
-00001000: 6d61 782c 202d 2d6d 6178 2049 4e54 4547  max, --max INTEG
-00001010: 4552 2020 2020 2020 2020 204d 6178 696d  ER         Maxim
-00001020: 756d 2071 7565 7269 6573 2074 6f20 636f  um queries to co
-00001030: 6e64 7563 7420 6f6e 2041 6c61 636f 7572  nduct on Alacour
-00001040: 742e 636f 6d0a 2020 2d73 6b69 702c 202d  t.com.  -skip, -
-00001050: 2d73 6b69 7020 494e 5445 4745 5220 2020  -skip INTEGER   
-00001060: 2020 2020 536b 6970 2065 6e74 7269 6573      Skip entries
-00001070: 2061 7420 746f 7020 6f66 2071 7565 7279   at top of query
-00001080: 2066 696c 650a 2020 2d6e 2c20 2d2d 6e6f   file.  -n, --no
-00001090: 2d6d 6172 6b20 2020 2020 2020 2020 2020  -mark           
-000010a0: 2020 2020 446f 206e 6f74 2075 7064 6174      Do not updat
-000010b0: 6520 7175 6572 7920 7465 6d70 6c61 7465  e query template
-000010c0: 2061 6674 6572 2063 6f6d 706c 6574 696f   after completio
-000010d0: 6e0a 2020 2d2d 6465 6275 6720 2020 2020  n.  --debug     
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 5072 696e 7420 6465 7461 696c 6564 2072  Print detailed r
-00001100: 756e 7469 6d65 2069 6e66 6f72 6d61 7469  untime informati
-00001110: 6f6e 2074 6f20 636f 6e73 6f6c 650a 2020  on to console.  
-00001120: 2d68 2c20 2d2d 6865 6c70 2020 2020 2020  -h, --help      
-00001130: 2020 2020 2020 2020 2020 2020 5368 6f77              Show
-00001140: 2074 6869 7320 6d65 7373 6167 6520 616e   this message an
-00001150: 6420 6578 6974 2e0a 6060 600a 0a0a 2323  d exit..```...##
-00001160: 202a 2a57 6f72 6b20 7769 7468 2063 6173   **Work with cas
-00001170: 6520 6461 7461 2069 6e20 5079 7468 6f6e  e data in Python
-00001180: 2a2a 0a0a 0a4f 7574 206f 6620 7468 6520  **...Out of the 
-00001190: 626f 782c 2041 6c61 636f 7264 6572 2065  box, Alacorder e
-000011a0: 7870 6f72 7473 2074 6f20 602e 786c 7378  xports to `.xlsx
-000011b0: 602c 2060 2e78 6c73 602c 2060 2e63 7376  `, `.xls`, `.csv
-000011c0: 602c 2060 2e6a 736f 6e60 2c20 616e 6420  `, `.json`, and 
-000011d0: 602e 7061 7271 7565 7460 2e20 4275 7420  `.parquet`. But 
-000011e0: 796f 7520 6361 6e20 7573 6520 6070 6f6c  you can use `pol
-000011f0: 6172 7360 2061 6e64 206f 7468 6572 2070  ars` and other p
-00001200: 7974 686f 6e20 6c69 6272 6172 6965 7320  ython libraries 
-00001210: 746f 2063 7265 6174 6520 796f 7572 206f  to create your o
-00001220: 776e 2064 6174 6120 636f 6c6c 6563 7469  wn data collecti
-00001230: 6f6e 2077 6f72 6b66 6c6f 7773 2061 6e64  on workflows and
-00001240: 2063 7573 746f 6d69 7a65 2041 6c61 636f   customize Alaco
-00001250: 7264 6572 2065 7870 6f72 7473 2e20 0a0a  rder exports. ..
-00001260: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00001270: 616c 6163 6f72 6465 7220 696d 706f 7274  alacorder import
-00001280: 2061 6c61 630a 696d 706f 7274 2070 6f6c   alac.import pol
-00001290: 6172 7320 6173 2070 6c0a 0a71 7565 7565  ars as pl..queue
-000012a0: 203d 2061 6c61 632e 6765 745f 7061 7468   = alac.get_path
-000012b0: 7328 222f 5573 6572 732f 6372 696d 736f  s("/Users/crimso
-000012c0: 6e2f 4465 736b 746f 702f 5475 7477 696c  n/Desktop/Tutwil
-000012d0: 6572 2f22 2920 2320 2d3e 205b 7374 725d  er/") # -> [str]
-000012e0: 0a0a 726f 7773 203d 205b 5d0a 0a66 6f72  ..rows = []..for
-000012f0: 2069 2c20 7061 7468 2069 6e20 656e 756d   i, path in enum
-00001300: 6572 6174 6528 7175 6575 6529 3a0a 2020  erate(queue):.  
-00001310: 2020 7465 7874 203d 2061 6c61 632e 6578    text = alac.ex
-00001320: 7472 6163 745f 7465 7874 2870 6174 6829  tract_text(path)
-00001330: 0a20 2020 2063 6e75 6d20 3d20 616c 6163  .    cnum = alac
-00001340: 2e67 6574 4361 7365 4e75 6d62 6572 2874  .getCaseNumber(t
-00001350: 6578 7429 0a20 2020 2063 7479 203d 2061  ext).    cty = a
-00001360: 6c61 632e 6765 7443 6f75 6e74 7928 7465  lac.getCounty(te
-00001370: 7874 290a 2020 2020 7462 616c 203d 2061  xt).    tbal = a
-00001380: 6c61 632e 6765 7454 6f74 616c 4261 6c61  lac.getTotalBala
-00001390: 6e63 6528 7465 7874 290a 2020 2020 7074  nce(text).    pt
-000013a0: 7220 3d20 616c 6163 2e67 6574 5061 796d  r = alac.getPaym
-000013b0: 656e 7454 6f52 6573 746f 7265 2874 6578  entToRestore(tex
-000013c0: 7429 2023 2069 2e65 2e20 766f 7469 6e67  t) # i.e. voting
-000013d0: 2072 6967 6874 730a 2020 2020 726f 7773   rights.    rows
-000013e0: 202b 3d20 5b5b 636e 756d 2c20 6374 792c   += [[cnum, cty,
-000013f0: 2074 6261 6c2c 2070 7472 5d5d 0a0a 6361   tbal, ptr]]..ca
-00001400: 7365 7320 3d20 706c 2e44 6174 6146 7261  ses = pl.DataFra
-00001410: 6d65 2872 6f77 7329 0a0a 6361 7365 732e  me(rows)..cases.
-00001420: 7772 6974 655f 6578 6365 6c28 222f 5573  write_excel("/Us
-00001430: 6572 732f 6372 696d 736f 6e2f 4465 736b  ers/crimson/Desk
-00001440: 746f 702f 5475 7477 696c 6572 2f73 756d  top/Tutwiler/sum
-00001450: 6d61 7279 2e78 6c73 7822 290a 0a60 6060  mary.xlsx")..```
-00001460: 0a0a 2323 2045 7874 656e 6420 416c 6163  ..## Extend Alac
-00001470: 6f72 6465 7220 7769 7468 2060 706f 6c61  order with `pola
-00001480: 7273 6020 616e 6420 6f74 6865 7220 746f  rs` and other to
-00001490: 6f6c 730a 0a41 6c61 636f 7264 6572 2072  ols..Alacorder r
-000014a0: 756e 7320 6f6e 205b 6070 6f6c 6172 7360  uns on [`polars`
-000014b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000014c0: 2e63 6f6d 2f70 6f6c 612d 7273 2f70 6f6c  .com/pola-rs/pol
-000014d0: 6172 7329 2c20 6120 6461 7461 6672 616d  ars), a datafram
-000014e0: 6573 206c 6962 7261 7279 2079 6f75 2063  es library you c
-000014f0: 616e 2075 7365 2074 6f20 776f 726b 2077  an use to work w
-00001500: 6974 6820 616e 6420 616e 616c 797a 6520  ith and analyze 
-00001510: 7461 6275 6c61 7220 6461 7461 2e20 6070  tabular data. `p
-00001520: 6f6c 6172 7360 2063 616e 2072 6561 6420  olars` can read 
-00001530: 6672 6f6d 2061 6e64 2077 7269 7465 2074  from and write t
-00001540: 6f20 616c 6c20 6d61 6a6f 7220 6461 7461  o all major data
-00001550: 2073 746f 7261 6765 2066 6f72 6d61 7473   storage formats
-00001560: 2e20 4974 2063 616e 2063 6f6e 6e65 6374  . It can connect
-00001570: 2074 6f20 6120 7769 6465 2076 6172 6965   to a wide varie
-00001580: 7479 206f 6620 7365 7276 6963 6573 2074  ty of services t
-00001590: 6f20 7072 6f76 6964 6520 666f 7220 6561  o provide for ea
-000015a0: 7379 2069 6d70 6f72 7420 616e 6420 6578  sy import and ex
-000015b0: 706f 7274 2e0a 0a60 6060 7079 7468 6f6e  port...```python
-000015c0: 0a69 6d70 6f72 7420 706f 6c61 7273 2061  .import polars a
-000015d0: 7320 706c 0a63 6f6e 7465 6e74 7320 3d20  s pl.contents = 
-000015e0: 706c 2e72 6561 645f 6a73 6f6e 2822 2f70  pl.read_json("/p
-000015f0: 6174 682f 746f 2f61 7263 6869 7665 2e6a  ath/to/archive.j
-00001600: 736f 6e22 290a 6060 600a 0a49 6620 796f  son").```..If yo
-00001610: 7520 776f 756c 6420 6c69 6b65 2074 6f20  u would like to 
-00001620: 7669 7375 616c 697a 6520 6461 7461 2077  visualize data w
-00001630: 6974 686f 7574 2065 7870 6f72 7469 6e67  ithout exporting
-00001640: 2074 6f20 4578 6365 6c20 6f72 2061 6e6f   to Excel or ano
-00001650: 7468 6572 2066 6f72 6d61 742c 2063 7265  ther format, cre
-00001660: 6174 6520 6120 606a 7570 7974 6572 206e  ate a `jupyter n
-00001670: 6f74 6562 6f6f 6b60 2061 6e64 2069 6e73  otebook` and ins
-00001680: 7461 6c6c 2074 6f6f 6c73 206c 696b 6520  tall tools like 
-00001690: 606d 6174 706c 6f74 6c69 6260 2c20 6074  `matplotlib`, `t
-000016a0: 6162 756c 6174 6560 2c20 616e 6420 6069  abulate`, and `i
-000016b0: 7461 626c 6573 6020 746f 2067 6574 2073  tables` to get s
-000016c0: 7461 7274 6564 2e20 5b4a 7570 7974 6572  tarted. [Jupyter
-000016d0: 204e 6f74 6562 6f6f 6b5d 2868 7474 7073   Notebook](https
-000016e0: 3a2f 2f64 6f63 732e 6a75 7079 7465 722e  ://docs.jupyter.
-000016f0: 6f72 672f 656e 2f6c 6174 6573 742f 7374  org/en/latest/st
-00001700: 6172 742f 696e 6465 782e 6874 6d6c 2920  art/index.html) 
-00001710: 6973 2061 2050 7974 686f 6e20 7072 6f6a  is a Python proj
-00001720: 6563 7420 796f 7520 6361 6e20 7573 6520  ect you can use 
-00001730: 746f 2063 7265 6174 6520 696e 7465 7261  to create intera
-00001740: 6374 6976 6520 6e6f 7465 626f 6f6b 7320  ctive notebooks 
-00001750: 666f 7220 6461 7461 2061 6e61 6c79 7369  for data analysi
-00001760: 7320 616e 6420 6f74 6865 7220 7075 7270  s and other purp
-00001770: 6f73 6573 2e20 4974 2063 616e 2062 6520  oses. It can be 
-00001780: 696e 7374 616c 6c65 6420 7573 696e 6720  installed using 
-00001790: 6070 6970 2069 6e73 7461 6c6c 206a 7570  `pip install jup
-000017a0: 7974 6572 6020 6f72 2060 7069 7033 2069  yter` or `pip3 i
-000017b0: 6e73 7461 6c6c 206a 7570 7974 6572 6020  nstall jupyter` 
-000017c0: 616e 6420 6c61 756e 6368 6564 2075 7369  and launched usi
-000017d0: 6e67 2060 6a75 7079 7465 7220 6e6f 7465  ng `jupyter note
-000017e0: 626f 6f6b 602e 2059 6f75 7220 6465 7669  book`. Your devi
-000017f0: 6365 206d 6179 2061 6c72 6561 6479 2062  ce may already b
-00001800: 6520 6571 7569 7070 6564 2074 6f20 7669  e equipped to vi
-00001810: 6577 2060 2e69 7079 6e62 6020 6e6f 7465  ew `.ipynb` note
-00001820: 626f 6f6b 732e 200a 0a23 2320 2a2a 5265  books. ..## **Re
-00001830: 736f 7572 6365 732a 2a0a 2a20 5b60 706f  sources**.* [`po
-00001840: 6c61 7273 6020 7573 6572 2067 7569 6465  lars` user guide
-00001850: 5d28 6874 7470 733a 2f2f 706f 6c61 2d72  ](https://pola-r
-00001860: 732e 6769 7468 7562 2e69 6f2f 706f 6c61  s.github.io/pola
-00001870: 7273 2d62 6f6f 6b2f 7573 6572 2d67 7569  rs-book/user-gui
-00001880: 6465 2f69 6e64 6578 2e68 746d 6c29 0a2a  de/index.html).*
-00001890: 205b 7265 6765 7820 6368 6561 7420 7368   [regex cheat sh
-000018a0: 6565 745d 2868 7474 7073 3a2f 2f77 7777  eet](https://www
-000018b0: 2e72 6578 6567 672e 636f 6d2f 7265 6765  .rexegg.com/rege
-000018c0: 782d 7175 6963 6b73 7461 7274 2e68 746d  x-quickstart.htm
-000018d0: 6c29 0a2a 205b 416e 6163 6f6e 6461 2028  l).* [Anaconda (
-000018e0: 7475 746f 7269 616c 7320 6f6e 2070 7974  tutorials on pyt
-000018f0: 686f 6e20 6461 7461 2061 6e61 6c79 7369  hon data analysi
-00001900: 7329 5d28 6874 7470 733a 2f2f 7777 772e  s)](https://www.
-00001910: 616e 6163 6f6e 6461 2e63 6f6d 2f6f 7065  anaconda.com/ope
-00001920: 6e2d 736f 7572 6365 290a 2a20 5b54 6865  n-source).* [The
-00001930: 2050 7974 686f 6e20 5475 746f 7269 616c   Python Tutorial
-00001940: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
-00001950: 7974 686f 6e2e 6f72 672f 332f 7475 746f  ython.org/3/tuto
-00001960: 7269 616c 2f29 0a2a 205b 4a75 7079 7465  rial/).* [Jupyte
-00001970: 7220 4e6f 7465 626f 6f6b 2069 6e74 726f  r Notebook intro
-00001980: 6475 6374 696f 6e5d 2868 7474 7073 3a2f  duction](https:/
-00001990: 2f72 6561 6c70 7974 686f 6e2e 636f 6d2f  /realpython.com/
-000019a0: 6a75 7079 7465 722d 6e6f 7465 626f 6f6b  jupyter-notebook
-000019b0: 2d69 6e74 726f 6475 6374 696f 6e2f 290a  -introduction/).
+00001000: 6e2c 202d 2d6e 6f2d 6d61 726b 2020 2020  n, --no-mark    
+00001010: 2020 2020 2020 2020 2020 2044 6f20 6e6f             Do no
+00001020: 7420 7570 6461 7465 2071 7565 7279 2074  t update query t
+00001030: 656d 706c 6174 6520 6166 7465 7220 636f  emplate after co
+00001040: 6d70 6c65 7469 6f6e 0a20 202d 2d64 6562  mpletion.  --deb
+00001050: 7567 2020 2020 2020 2020 2020 2020 2020  ug              
+00001060: 2020 2020 2020 2050 7269 6e74 2064 6574         Print det
+00001070: 6169 6c65 6420 7275 6e74 696d 6520 696e  ailed runtime in
+00001080: 666f 726d 6174 696f 6e20 746f 2063 6f6e  formation to con
+00001090: 736f 6c65 0a20 202d 682c 202d 2d68 656c  sole.  -h, --hel
+000010a0: 7020 2020 2020 2020 2020 2020 2020 2020  p               
+000010b0: 2020 2053 686f 7720 7468 6973 206d 6573     Show this mes
+000010c0: 7361 6765 2061 6e64 2065 7869 742e 0a60  sage and exit..`
+000010d0: 6060 0a0a 0a23 2320 2a2a 576f 726b 2077  ``...## **Work w
+000010e0: 6974 6820 6361 7365 2064 6174 6120 696e  ith case data in
+000010f0: 2050 7974 686f 6e2a 2a0a 0a0a 4f75 7420   Python**...Out 
+00001100: 6f66 2074 6865 2062 6f78 2c20 416c 6163  of the box, Alac
+00001110: 6f72 6465 7220 6578 706f 7274 7320 746f  order exports to
+00001120: 2060 2e78 6c73 7860 2c20 602e 786c 7360   `.xlsx`, `.xls`
+00001130: 2c20 602e 6373 7660 2c20 602e 6a73 6f6e  , `.csv`, `.json
+00001140: 602c 2061 6e64 2060 2e70 6172 7175 6574  `, and `.parquet
+00001150: 602e 2042 7574 2079 6f75 2063 616e 2075  `. But you can u
+00001160: 7365 2060 706f 6c61 7273 6020 616e 6420  se `polars` and 
+00001170: 6f74 6865 7220 7079 7468 6f6e 206c 6962  other python lib
+00001180: 7261 7269 6573 2074 6f20 6372 6561 7465  raries to create
+00001190: 2079 6f75 7220 6f77 6e20 6461 7461 2063   your own data c
+000011a0: 6f6c 6c65 6374 696f 6e20 776f 726b 666c  ollection workfl
+000011b0: 6f77 7320 616e 6420 6375 7374 6f6d 697a  ows and customiz
+000011c0: 6520 416c 6163 6f72 6465 7220 6578 706f  e Alacorder expo
+000011d0: 7274 732e 200a 0a0a 6060 6070 7974 686f  rts. ...```pytho
+000011e0: 6e0a 6672 6f6d 2061 6c61 636f 7264 6572  n.from alacorder
+000011f0: 2069 6d70 6f72 7420 616c 6163 0a69 6d70   import alac.imp
+00001200: 6f72 7420 706f 6c61 7273 2061 7320 706c  ort polars as pl
+00001210: 0a0a 7175 6575 6520 3d20 616c 6163 2e67  ..queue = alac.g
+00001220: 6574 5f70 6174 6873 2822 2f55 7365 7273  et_paths("/Users
+00001230: 2f63 7269 6d73 6f6e 2f44 6573 6b74 6f70  /crimson/Desktop
+00001240: 2f54 7574 7769 6c65 722f 2229 2023 202d  /Tutwiler/") # -
+00001250: 3e20 5b73 7472 5d0a 0a72 6f77 7320 3d20  > [str]..rows = 
+00001260: 5b5d 0a0a 666f 7220 692c 2070 6174 6820  []..for i, path 
+00001270: 696e 2065 6e75 6d65 7261 7465 2871 7565  in enumerate(que
+00001280: 7565 293a 0a20 2020 2074 6578 7420 3d20  ue):.    text = 
+00001290: 616c 6163 2e65 7874 7261 6374 5f74 6578  alac.extract_tex
+000012a0: 7428 7061 7468 290a 2020 2020 636e 756d  t(path).    cnum
+000012b0: 203d 2061 6c61 632e 6765 7443 6173 654e   = alac.getCaseN
+000012c0: 756d 6265 7228 7465 7874 290a 2020 2020  umber(text).    
+000012d0: 6374 7920 3d20 616c 6163 2e67 6574 436f  cty = alac.getCo
+000012e0: 756e 7479 2874 6578 7429 0a20 2020 2074  unty(text).    t
+000012f0: 6261 6c20 3d20 616c 6163 2e67 6574 546f  bal = alac.getTo
+00001300: 7461 6c42 616c 616e 6365 2874 6578 7429  talBalance(text)
+00001310: 0a20 2020 2070 7472 203d 2061 6c61 632e  .    ptr = alac.
+00001320: 6765 7450 6179 6d65 6e74 546f 5265 7374  getPaymentToRest
+00001330: 6f72 6528 7465 7874 2920 2320 692e 652e  ore(text) # i.e.
+00001340: 2076 6f74 696e 6720 7269 6768 7473 0a20   voting rights. 
+00001350: 2020 2072 6f77 7320 2b3d 205b 5b63 6e75     rows += [[cnu
+00001360: 6d2c 2063 7479 2c20 7462 616c 2c20 7074  m, cty, tbal, pt
+00001370: 725d 5d0a 0a63 6173 6573 203d 2070 6c2e  r]]..cases = pl.
+00001380: 4461 7461 4672 616d 6528 726f 7773 290a  DataFrame(rows).
+00001390: 0a63 6173 6573 2e77 7269 7465 5f65 7863  .cases.write_exc
+000013a0: 656c 2822 2f55 7365 7273 2f63 7269 6d73  el("/Users/crims
+000013b0: 6f6e 2f44 6573 6b74 6f70 2f54 7574 7769  on/Desktop/Tutwi
+000013c0: 6c65 722f 7375 6d6d 6172 792e 786c 7378  ler/summary.xlsx
+000013d0: 2229 0a0a 6060 600a 0a23 2320 4578 7465  ")..```..## Exte
+000013e0: 6e64 2041 6c61 636f 7264 6572 2077 6974  nd Alacorder wit
+000013f0: 6820 6070 6f6c 6172 7360 2061 6e64 206f  h `polars` and o
+00001400: 7468 6572 2074 6f6f 6c73 0a0a 416c 6163  ther tools..Alac
+00001410: 6f72 6465 7220 7275 6e73 206f 6e20 5b60  order runs on [`
+00001420: 706f 6c61 7273 605d 2868 7474 7073 3a2f  polars`](https:/
+00001430: 2f67 6974 6875 622e 636f 6d2f 706f 6c61  /github.com/pola
+00001440: 2d72 732f 706f 6c61 7273 292c 2061 2064  -rs/polars), a d
+00001450: 6174 6166 7261 6d65 7320 6c69 6272 6172  ataframes librar
+00001460: 7920 796f 7520 6361 6e20 7573 6520 746f  y you can use to
+00001470: 2077 6f72 6b20 7769 7468 2061 6e64 2061   work with and a
+00001480: 6e61 6c79 7a65 2074 6162 756c 6172 2064  nalyze tabular d
+00001490: 6174 612e 2060 706f 6c61 7273 6020 6361  ata. `polars` ca
+000014a0: 6e20 7265 6164 2066 726f 6d20 616e 6420  n read from and 
+000014b0: 7772 6974 6520 746f 2061 6c6c 206d 616a  write to all maj
+000014c0: 6f72 2064 6174 6120 7374 6f72 6167 6520  or data storage 
+000014d0: 666f 726d 6174 732e 2049 7420 6361 6e20  formats. It can 
+000014e0: 636f 6e6e 6563 7420 746f 2061 2077 6964  connect to a wid
+000014f0: 6520 7661 7269 6574 7920 6f66 2073 6572  e variety of ser
+00001500: 7669 6365 7320 746f 2070 726f 7669 6465  vices to provide
+00001510: 2066 6f72 2065 6173 7920 696d 706f 7274   for easy import
+00001520: 2061 6e64 2065 7870 6f72 742e 0a0a 6060   and export...``
+00001530: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
+00001540: 6f6c 6172 7320 6173 2070 6c0a 636f 6e74  olars as pl.cont
+00001550: 656e 7473 203d 2070 6c2e 7265 6164 5f6a  ents = pl.read_j
+00001560: 736f 6e28 222f 7061 7468 2f74 6f2f 6172  son("/path/to/ar
+00001570: 6368 6976 652e 6a73 6f6e 2229 0a60 6060  chive.json").```
+00001580: 0a0a 4966 2079 6f75 2077 6f75 6c64 206c  ..If you would l
+00001590: 696b 6520 746f 2076 6973 7561 6c69 7a65  ike to visualize
+000015a0: 2064 6174 6120 7769 7468 6f75 7420 6578   data without ex
+000015b0: 706f 7274 696e 6720 746f 2045 7863 656c  porting to Excel
+000015c0: 206f 7220 616e 6f74 6865 7220 666f 726d   or another form
+000015d0: 6174 2c20 6372 6561 7465 2061 2060 6a75  at, create a `ju
+000015e0: 7079 7465 7220 6e6f 7465 626f 6f6b 6020  pyter notebook` 
+000015f0: 616e 6420 696e 7374 616c 6c20 746f 6f6c  and install tool
+00001600: 7320 6c69 6b65 2060 6d61 7470 6c6f 746c  s like `matplotl
+00001610: 6962 602c 2060 7461 6275 6c61 7465 602c  ib`, `tabulate`,
+00001620: 2061 6e64 2060 6974 6162 6c65 7360 2074   and `itables` t
+00001630: 6f20 6765 7420 7374 6172 7465 642e 205b  o get started. [
+00001640: 4a75 7079 7465 7220 4e6f 7465 626f 6f6b  Jupyter Notebook
+00001650: 5d28 6874 7470 733a 2f2f 646f 6373 2e6a  ](https://docs.j
+00001660: 7570 7974 6572 2e6f 7267 2f65 6e2f 6c61  upyter.org/en/la
+00001670: 7465 7374 2f73 7461 7274 2f69 6e64 6578  test/start/index
+00001680: 2e68 746d 6c29 2069 7320 6120 5079 7468  .html) is a Pyth
+00001690: 6f6e 2070 726f 6a65 6374 2079 6f75 2063  on project you c
+000016a0: 616e 2075 7365 2074 6f20 6372 6561 7465  an use to create
+000016b0: 2069 6e74 6572 6163 7469 7665 206e 6f74   interactive not
+000016c0: 6562 6f6f 6b73 2066 6f72 2064 6174 6120  ebooks for data 
+000016d0: 616e 616c 7973 6973 2061 6e64 206f 7468  analysis and oth
+000016e0: 6572 2070 7572 706f 7365 732e 2049 7420  er purposes. It 
+000016f0: 6361 6e20 6265 2069 6e73 7461 6c6c 6564  can be installed
+00001700: 2075 7369 6e67 2060 7069 7020 696e 7374   using `pip inst
+00001710: 616c 6c20 6a75 7079 7465 7260 206f 7220  all jupyter` or 
+00001720: 6070 6970 3320 696e 7374 616c 6c20 6a75  `pip3 install ju
+00001730: 7079 7465 7260 2061 6e64 206c 6175 6e63  pyter` and launc
+00001740: 6865 6420 7573 696e 6720 606a 7570 7974  hed using `jupyt
+00001750: 6572 206e 6f74 6562 6f6f 6b60 2e20 596f  er notebook`. Yo
+00001760: 7572 2064 6576 6963 6520 6d61 7920 616c  ur device may al
+00001770: 7265 6164 7920 6265 2065 7175 6970 7065  ready be equippe
+00001780: 6420 746f 2076 6965 7720 602e 6970 796e  d to view `.ipyn
+00001790: 6260 206e 6f74 6562 6f6f 6b73 2e20 0a0a  b` notebooks. ..
+000017a0: 2323 202a 2a52 6573 6f75 7263 6573 2a2a  ## **Resources**
+000017b0: 0a2a 205b 6070 6f6c 6172 7360 2075 7365  .* [`polars` use
+000017c0: 7220 6775 6964 655d 2868 7474 7073 3a2f  r guide](https:/
+000017d0: 2f70 6f6c 612d 7273 2e67 6974 6875 622e  /pola-rs.github.
+000017e0: 696f 2f70 6f6c 6172 732d 626f 6f6b 2f75  io/polars-book/u
+000017f0: 7365 722d 6775 6964 652f 696e 6465 782e  ser-guide/index.
+00001800: 6874 6d6c 290a 2a20 5b72 6567 6578 2063  html).* [regex c
+00001810: 6865 6174 2073 6865 6574 5d28 6874 7470  heat sheet](http
+00001820: 733a 2f2f 7777 772e 7265 7865 6767 2e63  s://www.rexegg.c
+00001830: 6f6d 2f72 6567 6578 2d71 7569 636b 7374  om/regex-quickst
+00001840: 6172 742e 6874 6d6c 290a 2a20 5b41 6e61  art.html).* [Ana
+00001850: 636f 6e64 6120 2874 7574 6f72 6961 6c73  conda (tutorials
+00001860: 206f 6e20 7079 7468 6f6e 2064 6174 6120   on python data 
+00001870: 616e 616c 7973 6973 295d 2868 7474 7073  analysis)](https
+00001880: 3a2f 2f77 7777 2e61 6e61 636f 6e64 612e  ://www.anaconda.
+00001890: 636f 6d2f 6f70 656e 2d73 6f75 7263 6529  com/open-source)
+000018a0: 0a2a 205b 5468 6520 5079 7468 6f6e 2054  .* [The Python T
+000018b0: 7574 6f72 6961 6c5d 2868 7474 7073 3a2f  utorial](https:/
+000018c0: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
+000018d0: 2f33 2f74 7574 6f72 6961 6c2f 290a 2a20  /3/tutorial/).* 
+000018e0: 5b4a 7570 7974 6572 204e 6f74 6562 6f6f  [Jupyter Noteboo
+000018f0: 6b20 696e 7472 6f64 7563 7469 6f6e 5d28  k introduction](
+00001900: 6874 7470 733a 2f2f 7265 616c 7079 7468  https://realpyth
+00001910: 6f6e 2e63 6f6d 2f6a 7570 7974 6572 2d6e  on.com/jupyter-n
+00001920: 6f74 6562 6f6f 6b2d 696e 7472 6f64 7563  otebook-introduc
+00001930: 7469 6f6e 2f29 0a                        tion/).
```

### Comparing `alacorder-80.6.0/pyproject.toml` & `alacorder-80.6.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.0"
+version = "80.6.0.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.0/src/alacorder/.DS_Store` & `alacorder-80.6.0.1/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.0/src/alacorder/__main__.py` & `alacorder-80.6.0.1/src/alacorder/__main__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.0/src/alacorder/alac.py` & `alacorder-80.6.0.1/src/alacorder/alac.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.0/PKG-INFO` & `alacorder-80.6.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.0
+Version: 80.6.0.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -99,16 +99,14 @@
   -in, --input-path PATH      Path to query table/spreadsheet (.xls, .xlsx)
                               [required]
   -out, --output-path PATH    Desired PDF output directory  [required]
   -c, --customer-id TEXT      Customer ID on Alacourt.com  [required]
   -u, --user-id TEXT          User ID on Alacourt.com  [required]
   -p, --password TEXT         Password on Alacourt.com  [required]
   -criminal, --criminal-only  Only search criminal cases
-  -max, --max INTEGER         Maximum queries to conduct on Alacourt.com
-  -skip, --skip INTEGER       Skip entries at top of query file
   -n, --no-mark               Do not update query template after completion
   --debug                     Print detailed runtime information to console
   -h, --help                  Show this message and exit.
 ```
 
 
 ## **Work with case data in Python**
```

