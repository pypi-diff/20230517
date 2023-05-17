# Comparing `tmp/baysalt_christmas-0.1.7.2.tar.gz` & `tmp/baysalt_christmas-0.1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.2.tar", last modified: Wed Apr 26 03:44:06 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.3.tar", last modified: Wed May 17 09:02:38 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.2.tar` & `baysalt_christmas-0.1.7.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.938433 baysalt_christmas-0.1.7.2/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-19 08:43:20.000000 baysalt_christmas-0.1.7.2/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.2/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-26 03:44:06.938308 baysalt_christmas-0.1.7.2/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.2/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.932340 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.934481 baysalt_christmas-0.1.7.2/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    20519 2023-04-26 03:41:40.000000 baysalt_christmas-0.1.7.2/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.2/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.2/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4526 2023-04-24 06:14:31.000000 baysalt_christmas-0.1.7.2/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.2/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.935982 baysalt_christmas-0.1.7.2/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.937952 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.2/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.2/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.2/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.2/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-26 03:44:06.938481 baysalt_christmas-0.1.7.2/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-26 03:44:02.000000 baysalt_christmas-0.1.7.2/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.199330 baysalt_christmas-0.1.7.3/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-09 03:21:44.000000 baysalt_christmas-0.1.7.3/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.3/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-17 09:02:38.199168 baysalt_christmas-0.1.7.3/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.3/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.193191 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-05-17 09:02:38.000000 baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.196340 baysalt_christmas-0.1.7.3/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    20792 2023-05-10 02:26:31.000000 baysalt_christmas-0.1.7.3/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.3/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.3/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.3/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.3/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.197982 baysalt_christmas-0.1.7.3/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-05-17 09:02:38.198836 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.3/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.3/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.3/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.3/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.3/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-05-17 09:02:38.199396 baysalt_christmas-0.1.7.3/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-05-17 09:02:36.000000 baysalt_christmas-0.1.7.3/setup.py
```

### Comparing `baysalt_christmas-0.1.7.2/.DS_Store` & `baysalt_christmas-0.1.7.3/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -266,37 +266,37 @@
 00001090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000010b0: 636f 6d70 0000 0000 0000 0000 0000 001a  comp............
 000010c0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000010d0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000010e0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000010f0: 0066 006f 6c67 3153 636f 6d70 0000 0000  .f.olg1Scomp....
-00001100: 0000 12f4 0000 001a 0062 0061 0079 0073  .........b.a.y.s
+00001100: 0000 1301 0000 001a 0062 0061 0079 0073  .........b.a.y.s
 00001110: 0061 006c 0074 005f 0063 0068 0072 0069  .a.l.t._.c.h.r.i
 00001120: 0073 0074 006d 0061 0073 002e 0065 0067  .s.t.m.a.s...e.g
 00001130: 0067 002d 0069 006e 0066 006f 6d6f 4444  .g.-.i.n.f.omoDD
-00001140: 626c 6f62 0000 0008 2733 7c67 30f7 c441  blob....'3|g0..A
+00001140: 626c 6f62 0000 0008 745c 6dc3 6afc c441  blob....t\m.j..A
 00001150: 0000 001a 0062 0061 0079 0073 0061 006c  .....b.a.y.s.a.l
 00001160: 0074 005f 0063 0068 0072 0069 0073 0074  .t._.c.h.r.i.s.t
 00001170: 006d 0061 0073 002e 0065 0067 0067 002d  .m.a.s...e.g.g.-
 00001180: 0069 006e 0066 006f 6d6f 6444 626c 6f62  .i.n.f.omodDblob
-00001190: 0000 0008 234e 55f2 c7eb c441 0000 001a  ....#NU....A....
+00001190: 0000 0008 745c 6dc3 6afc c441 0000 001a  ....t\m.j..A....
 000011a0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000011b0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000011c0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000011d0: 0066 006f 7068 3153 636f 6d70 0000 0000  .f.oph1Scomp....
 000011e0: 0000 5000 0000 0005 0062 0075 0069 006c  ..P......b.u.i.l
 000011f0: 0064 6c67 3153 636f 6d70 0000 0000 0001  .dlg1Scomp......
-00001200: 71dc 0000 0005 0062 0075 0069 006c 0064  q......b.u.i.l.d
-00001210: 6d6f 4444 626c 6f62 0000 0008 ed3c c3dd  moDDblob.....<..
-00001220: 4ef7 c441 0000 0005 0062 0075 0069 006c  N..A.....b.u.i.l
-00001230: 0064 6d6f 6444 626c 6f62 0000 0008 ed3c  .dmodDblob.....<
-00001240: c3dd 4ef7 c441 0000 0005 0062 0075 0069  ..N..A.....b.u.i
+00001200: 9651 0000 0005 0062 0075 0069 006c 0064  .Q.....b.u.i.l.d
+00001210: 6d6f 4444 626c 6f62 0000 0008 3414 94c3  moDDblob....4...
+00001220: 6afc c441 0000 0005 0062 0075 0069 006c  j..A.....b.u.i.l
+00001230: 0064 6d6f 6444 626c 6f62 0000 0008 3414  .dmodDblob....4.
+00001240: 94c3 6afc c441 0000 0005 0062 0075 0069  ..j..A.....b.u.i
 00001250: 006c 0064 7068 3153 636f 6d70 0000 0000  .l.dph1Scomp....
-00001260: 0002 1000 0000 0009 0063 0068 0072 0069  .........c.h.r.i
+00001260: 0002 4000 0000 0009 0063 0068 0072 0069  ..@......c.h.r.i
 00001270: 0073 0074 006d 0061 0073 6277 7370 626c  .s.t.m.a.sbwspbl
 00001280: 6f62 0000 00ba 6270 6c69 7374 3030 d601  ob....bplist00..
 00001290: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 000012a0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 000012b0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000012c0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000012d0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
@@ -306,15 +306,15 @@
 00001310: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8c  }}...#/;R_klmno.
 00001320: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001330: 0000 0000 0000 0000 0000 0000 0000 008d  ................
 00001340: 0000 0009 0063 0068 0072 0069 0073 0074  .....c.h.r.i.s.t
 00001350: 006d 0061 0073 6473 636c 626f 6f6c 0100  .m.a.sdsclbool..
 00001360: 0000 0900 6300 6800 7200 6900 7300 7400  ....c.h.r.i.s.t.
 00001370: 6d00 6100 736c 6731 5363 6f6d 7000 0000  m.a.slg1Scomp...
-00001380: 0000 01ba cf00 0000 0900 6300 6800 7200  ..........c.h.r.
+00001380: 0000 0219 f200 0000 0900 6300 6800 7200  ..........c.h.r.
 00001390: 6900 7300 7400 6d00 6100 736c 7376 4362  i.s.t.m.a.slsvCb
 000013a0: 6c6f 6200 0003 0062 706c 6973 7430 30d8  lob....bplist00.
 000013b0: 0102 0304 0506 0708 090a 0b16 5354 550a  ............STU.
 000013c0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
 000013d0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
 000013e0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
 000013f0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
@@ -400,20 +400,20 @@
 000018f0: 0169 0172 0174 0175 0176 017f 0181 0182  .i.r.t.u.v......
 00001900: 0184 0185 018e 0190 0191 0194 0195 019e  ................
 00001910: 01a0 01a1 01a2 01a3 01ac 01b9 01c2 0000  ................
 00001920: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00001930: 0000 0000 0000 0000 0000 0000 01c3 0000  ................
 00001940: 0009 0063 0068 0072 0069 0073 0074 006d  ...c.h.r.i.s.t.m
 00001950: 0061 0073 6d6f 4444 626c 6f62 0000 0008  .a.smoDDblob....
-00001960: f506 df8d f0f7 c441 0000 0009 0063 0068  .......A.....c.h
+00001960: 29ca 80d6 f904 c541 0000 0009 0063 0068  )......A.....c.h
 00001970: 0072 0069 0073 0074 006d 0061 0073 6d6f  .r.i.s.t.m.a.smo
-00001980: 6444 626c 6f62 0000 0008 f506 df8d f0f7  dDblob..........
-00001990: c441 0000 0009 0063 0068 0072 0069 0073  .A.....c.h.r.i.s
+00001980: 6444 626c 6f62 0000 0008 29ca 80d6 f904  dDblob....).....
+00001990: c541 0000 0009 0063 0068 0072 0069 0073  .A.....c.h.r.i.s
 000019a0: 0074 006d 0061 0073 7068 3153 636f 6d70  .t.m.a.sph1Scomp
-000019b0: 0000 0000 0003 2000 0000 0009 0063 0068  ...... ......c.h
+000019b0: 0000 0000 0003 8000 0000 0009 0063 0068  .............c.h
 000019c0: 0072 0069 0073 0074 006d 0061 0073 7653  .r.i.s.t.m.a.svS
 000019d0: 726e 6c6f 6e67 0000 0001 0000 0004 0064  rnlong.........d
 000019e0: 0069 0073 0074 6277 7370 626c 6f62 0000  .i.s.tbwspblob..
 000019f0: 00b9 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 00001a00: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 00001a10: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001a20: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
@@ -422,21 +422,21 @@
 00001a50: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
 00001a60: 095f 1019 7b7b 3430 342c 2034 3738 7d2c  ._..{{404, 478},
 00001a70: 207b 3132 3338 2c20 3436 377d 7d09 0815   {1238, 467}}...
 00001a80: 232f 3b52 5f6b 6c6d 6e6f 8b00 0000 0000  #/;R_klmno......
 00001a90: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00001aa0: 0000 0000 0000 0000 0000 8c00 0000 0400  ................
 00001ab0: 6400 6900 7300 746c 6731 5363 6f6d 7000  d.i.s.tlg1Scomp.
-00001ac0: 0000 0000 011b c600 0000 0400 6400 6900  ............d.i.
-00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 0893  s.tmoDDblob.....
-00001ae0: 94ab 6730 f7c4 4100 0000 0400 6400 6900  ..g0..A.....d.i.
-00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 0893  s.tmodDblob.....
-00001b00: 94ab 6730 f7c4 4100 0000 0400 6400 6900  ..g0..A.....d.i.
+00001ac0: 0000 0000 0139 1c00 0000 0400 6400 6900  .....9......d.i.
+00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 08d7  s.tmoDDblob.....
+00001ae0: 0398 c36a fcc4 4100 0000 0400 6400 6900  ...j..A.....d.i.
+00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 08d7  s.tmodDblob.....
+00001b00: 0398 c36a fcc4 4100 0000 0400 6400 6900  ...j..A.....d.i.
 00001b10: 7300 7470 6831 5363 6f6d 7000 0000 0000  s.tph1Scomp.....
-00001b20: 0130 0000 0000 0400 6400 6900 7300 7476  .0......d.i.s.tv
+00001b20: 0150 0000 0000 0400 6400 6900 7300 7476  .P......d.i.s.tv
 00001b30: 5372 6e6c 6f6e 6700 0000 0100 0000 0000  Srnlong.........
 00001b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `baysalt_christmas-0.1.7.2/PKG-INFO` & `baysalt_christmas-0.1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.2
+Version: 0.1.7.3
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.2/README.md` & `baysalt_christmas-0.1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.2
+Version: 0.1.7.3
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.3/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/Blogging.py` & `baysalt_christmas-0.1.7.3/christmas/Blogging.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             self.PARA_DEFAULT['debug_log_filename'] = f'{self.logfile_name}_debug.log'
             self.PARA_DEFAULT['info_log_filename'] = f'{self.logfile_name}_info.log'
             self.PARA_DEFAULT['warning_log_filename'] = f'{self.logfile_name}_warning.log'
             self.PARA_DEFAULT['error_log_filename'] = f'{self.logfile_name}_error.log'
             self.PARA_DEFAULT['critical_log_filename'] = f'{self.logfile_name}_critical.log'
         
         self.PARA = self.PARA_DEFAULT
-        self.console
+        self.console()
     
     def setup_Blog(self, **kwargs):
         
         self.PARA.update(kwargs)
         self.maxBytes = self.PARA['maxBytes']
         self.backupCount = self.PARA['backupCount']
         self.colors_config = self.PARA['colors_config']
@@ -253,15 +253,19 @@
         """
         logger_handler.close()
     
     def console(self):
         """构造日志收集器"""
         self.setup_Blog()  # 初始化
         self.logger.setLevel(self.log_level)  # 设置日志收集器级别
-        
+
+        if self.logger.hasHandlers():  # 如果已经有日志记录器，先关闭
+            self.logger.handlers.clear()
+        if self.logger.filters:  # 如果已经有日志过滤器，先关闭
+            self.logger.filters.clear()
         if self.switch_write_all_log:  # 是否写入全部日志
             self.__write_all_log()
         if self.switch_write_error_plus_log:  # 是否写入错误日志
             self.__write_error_plus_log()
         if self.switch_print_log:  # 是否打印日志
             self.__print_log()
         if self.switch_write_debug_log:
@@ -309,21 +313,36 @@
     def addLevelName(level, levelName):
         logging.addLevelName(level, levelName)
     
     @staticmethod
     def getLevelName(level):
         return logging.getLevelName(level)
 
+    def __getitem__(self, item):
+        return getattr(self, item)
+
+    def __del__(self):
+        # self.logger.handlers.clear()
+        # self.logger.filters.clear()
+        # del self.logger
+        pass
+
+    def __str__(self):
+        return 'Blog()'
+
+    def __call__(self, *args, **kwargs):
+        return self.logger
+
 
-def debug(msg, *args, **kwargs):
+def debug(self, *args, **kwargs):
     TF, instanced = whether_instanced(Blog)
     if TF:
-        instanced[instanced.keys()[0]].logger.debug(msg, *args, **kwargs)
+        instanced[instanced.keys()[0]].logger.debug(self, *args, **kwargs)
     else:
-        Blog().logger.debug(msg, *args, **kwargs)
+        Blog().logger.debug(self, *args, **kwargs)
 
 
 def info(msg, *args, **kwargs):
     TF, instanced = whether_instanced(Blog)
     if TF:
         instanced[instanced.keys()[0]].logger.info(msg, *args, **kwargs)
     else:
@@ -331,31 +350,23 @@
 
 
 def warning(msg, *args, **kwargs):
     TF, instanced = whether_instanced(Blog)
     if TF:
         instanced[instanced.keys()[0]].logger.warning(msg, *args, **kwargs)
     else:
-        Blog().logger.warning(msg, *args, **kwargs)
+        Blog().console().warning(msg, *args, **kwargs)
 
 
 def error(msg, *args, **kwargs):
-    TF, instanced = whether_instanced(Blog)
-    if TF:
-        instanced[instanced.keys()[0]].logger.error(msg, *args, **kwargs)
-    else:
-        Blog().logger.error(msg, *args, **kwargs)
+    Blog().logger.error(msg, *args, **kwargs)
 
 
 def critical(msg, *args, **kwargs):
-    TF, instanced = whether_instanced(Blog)
-    if TF:
-        instanced[instanced.keys()[0]].logger.critical(msg, *args, **kwargs)
-    else:
-        Blog().logger.critical(msg, *args, **kwargs)
+    Blog().logger.critical(msg, *args, **kwargs)
 
 
 def exception(msg, *args, **kwargs):
     TF, instanced = whether_instanced(Blog)
     if TF:
         instanced[instanced.keys()[0]].logger.exception(msg, *args, **kwargs)
     else:
@@ -405,18 +416,19 @@
     x.info("这是日志信息")  # 日志输出
     x.warning("这是警告信息")  # 日志输出
     x.error("这是错误日志信息")  # 日志输出
     x.critical("这是严重级别信息")  # 日志输出
 
 
 def example_Blog_simple():
-    log1 = Blog()
-    log1.logger.debug("这是debug信息")
-    log1.logger.info("这是日志信息")
-    log1.logger.warning("这是警告信息")
-    log1.logger.error("这是错误日志信息")
-    log1.logger.critical("这是严重级别信息")
+    log_1 = Blog()
+    log1 = log_1.console()
+    log1.debug("这是debug信息")
+    log1.info("这是日志信息")
+    log1.warning("这是警告信息")
+    log1.error("这是错误日志信息")
+    log1.critical("这是严重级别信息")
 
 
 if __name__ == '__main__':
     # example_Blog_simple()
     example_Blog()
```

### Comparing `baysalt_christmas-0.1.7.2/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.3/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/commonCode.py` & `baysalt_christmas-0.1.7.3/christmas/commonCode.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,14 +112,25 @@
     :return:
     """
     for p in path:
         if os.path.exists(p):
             os.remove(p)
 
 
+def rmdirs(*path):
+    """
+    删除文件夹
+    :param path: 文件夹路径
+    :return:
+    """
+    for p in path:
+        if os.path.exists(p):
+            os.removedirs(p)
+
+
 class FtpUploadTracker:
     sizeWritten = 0
     totalSize = 0
     lastShownPercent = 0
 
     def __init__(self, totalSize, sizeWritten):
         self.totalSize = totalSize
@@ -131,22 +142,22 @@
         if self.lastShownPercent != percentComplete:
             self.lastShownPercent = percentComplete
             if percentComplete % 10 == 0:
                 print(f'{str(percentComplete)}% complete')
             # print(str(percentComplete) +"% complete")
 
 
-def split_path(_path):
+def split_path(_path, _split='/'):
     """
     如果路径名最后一位是'/'，则去掉
     :param _path: 路径名
     :return: 路径名
     """
     with contextlib.suppress(IndexError):
-        if _path[-1] == '/':
+        if _path[-1] == _split:
             _path = _path[:-1]
     return _path
 
 
 def timer(func):
     def inside(self):
         t1 = time.time()
@@ -161,15 +172,14 @@
     """
     判断是否被实例化
     :param _class: 类名
     """
     has_instance = False
     instanced = {}
     instances = globals().copy()
+
     for var_name, var_value in instances.items():
         if isinstance(var_value, _class):
             has_instance = True
             instanced[var_name] = var_value
-        else:
-            has_instance = False
 
     return has_instance, instanced
```

### Comparing `baysalt_christmas-0.1.7.2/christmas/cprintf.py` & `baysalt_christmas-0.1.7.3/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.3/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.3/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.3/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.3/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.3/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/processBar.py` & `baysalt_christmas-0.1.7.3/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/read_conf.py` & `baysalt_christmas-0.1.7.3/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/christmas/server_info.py` & `baysalt_christmas-0.1.7.3/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.2/setup.py` & `baysalt_christmas-0.1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.2",
+    version="0.1.7.3",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

