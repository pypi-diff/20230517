# Comparing `tmp/scrapautoscout-1.2.0.tar.gz` & `tmp/scrapautoscout-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapautoscout-1.2.0.tar", last modified: Tue Apr 11 09:14:54 2023, max compression
+gzip compressed data, was "scrapautoscout-1.3.0.tar", last modified: Wed May 17 13:11:45 2023, max compression
```

## Comparing `scrapautoscout-1.2.0.tar` & `scrapautoscout-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,52 @@
-drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-04-11 09:14:54.985763 scrapautoscout-1.2.0/
--rw-r--r--   0 vicolc     (501) staff       (20)     1068 2023-03-16 13:16:28.000000 scrapautoscout-1.2.0/LICENSE
--rw-r--r--   0 vicolc     (501) staff       (20)       39 2023-03-16 13:16:28.000000 scrapautoscout-1.2.0/MANIFEST.in
--rw-r--r--   0 vicolc     (501) staff       (20)     1718 2023-04-11 09:14:54.985587 scrapautoscout-1.2.0/PKG-INFO
--rw-r--r--   0 vicolc     (501) staff       (20)     1108 2023-04-06 11:54:53.000000 scrapautoscout-1.2.0/README.md
-drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-04-11 09:14:54.979871 scrapautoscout-1.2.0/scrapautoscout/
--rw-r--r--   0 vicolc     (501) staff       (20)        1 2023-03-16 13:16:28.000000 scrapautoscout-1.2.0/scrapautoscout/__init__.py
-drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-04-11 09:14:54.984963 scrapautoscout-1.2.0/scrapautoscout/__pycache__/
--rw-r--r--   0 vicolc     (501) staff       (20)      154 2023-03-16 14:55:35.000000 scrapautoscout-1.2.0/scrapautoscout/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 vicolc     (501) staff       (20)     8877 2023-04-05 10:11:26.000000 scrapautoscout-1.2.0/scrapautoscout/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 vicolc     (501) staff       (20)     2323 2023-04-10 10:43:41.000000 scrapautoscout-1.2.0/scrapautoscout/__pycache__/pipeline.cpython-310.pyc
--rw-r--r--   0 vicolc     (501) staff       (20)     3094 2023-04-07 09:58:17.000000 scrapautoscout-1.2.0/scrapautoscout/__pycache__/proxies.cpython-310.pyc
--rw-r--r--   0 vicolc     (501) staff       (20)    21434 2023-04-10 10:43:41.000000 scrapautoscout-1.2.0/scrapautoscout/__pycache__/scrapper.cpython-310.pyc
--rw-r--r--   0 vicolc     (501) staff       (20)     5771 2023-04-05 10:45:15.000000 scrapautoscout-1.2.0/scrapautoscout/__pycache__/transform.cpython-310.pyc
--rw-r--r--   0 vicolc     (501) staff       (20)     1815 2023-03-28 11:38:09.000000 scrapautoscout-1.2.0/scrapautoscout/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 vicolc     (501) staff       (20)    12415 2023-04-05 09:33:57.000000 scrapautoscout-1.2.0/scrapautoscout/config.py
--rw-r--r--   0 vicolc     (501) staff       (20)     2165 2023-04-10 11:48:23.000000 scrapautoscout-1.2.0/scrapautoscout/pipeline.py
--rw-r--r--   0 vicolc     (501) staff       (20)     3459 2023-04-07 09:58:17.000000 scrapautoscout-1.2.0/scrapautoscout/proxies.py
--rw-r--r--   0 vicolc     (501) staff       (20)    30571 2023-04-11 08:44:20.000000 scrapautoscout-1.2.0/scrapautoscout/scrapper.py
--rw-r--r--   0 vicolc     (501) staff       (20)     7592 2023-04-05 09:33:57.000000 scrapautoscout-1.2.0/scrapautoscout/transform.py
--rw-r--r--   0 vicolc     (501) staff       (20)     1416 2023-03-28 11:10:05.000000 scrapautoscout-1.2.0/scrapautoscout/utils.py
-drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-04-11 09:14:54.981814 scrapautoscout-1.2.0/scrapautoscout.egg-info/
--rw-r--r--   0 vicolc     (501) staff       (20)     1718 2023-04-11 09:14:54.000000 scrapautoscout-1.2.0/scrapautoscout.egg-info/PKG-INFO
--rw-r--r--   0 vicolc     (501) staff       (20)      811 2023-04-11 09:14:54.000000 scrapautoscout-1.2.0/scrapautoscout.egg-info/SOURCES.txt
--rw-r--r--   0 vicolc     (501) staff       (20)        1 2023-04-11 09:14:54.000000 scrapautoscout-1.2.0/scrapautoscout.egg-info/dependency_links.txt
--rw-r--r--   0 vicolc     (501) staff       (20)       64 2023-04-11 09:14:54.000000 scrapautoscout-1.2.0/scrapautoscout.egg-info/entry_points.txt
--rw-r--r--   0 vicolc     (501) staff       (20)       88 2023-04-11 09:14:54.000000 scrapautoscout-1.2.0/scrapautoscout.egg-info/requires.txt
--rw-r--r--   0 vicolc     (501) staff       (20)       15 2023-04-11 09:14:54.000000 scrapautoscout-1.2.0/scrapautoscout.egg-info/top_level.txt
--rw-r--r--   0 vicolc     (501) staff       (20)       38 2023-04-11 09:14:54.985817 scrapautoscout-1.2.0/setup.cfg
--rw-r--r--   0 vicolc     (501) staff       (20)     1138 2023-04-11 09:14:51.000000 scrapautoscout-1.2.0/setup.py
+drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-05-17 13:11:45.535132 scrapautoscout-1.3.0/
+-rw-r--r--   0 vicolc     (501) staff       (20)     1068 2023-03-16 13:16:28.000000 scrapautoscout-1.3.0/LICENSE
+-rw-r--r--   0 vicolc     (501) staff       (20)       39 2023-03-16 13:16:28.000000 scrapautoscout-1.3.0/MANIFEST.in
+-rw-r--r--   0 vicolc     (501) staff       (20)     1698 2023-05-17 13:11:45.534919 scrapautoscout-1.3.0/PKG-INFO
+-rw-r--r--   0 vicolc     (501) staff       (20)     1108 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/README.md
+drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-05-17 13:11:45.517312 scrapautoscout-1.3.0/db/
+-rw-r--r--   0 vicolc     (501) staff       (20)        1 2023-03-16 13:16:28.000000 scrapautoscout-1.3.0/db/__init__.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     1077 2023-05-17 13:09:23.000000 scrapautoscout-1.3.0/db/connect.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     4274 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/db/create_tables.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      733 2023-05-17 13:10:29.000000 scrapautoscout-1.3.0/db/db_config.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     1340 2023-05-17 13:04:51.000000 scrapautoscout-1.3.0/db/extract_data.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     1201 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/db/insert_data.py
+drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-05-17 13:11:45.525382 scrapautoscout-1.3.0/scrapautoscout/
+-rw-r--r--   0 vicolc     (501) staff       (20)        1 2023-03-16 13:16:28.000000 scrapautoscout-1.3.0/scrapautoscout/__init__.py
+drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-05-17 13:11:45.529774 scrapautoscout-1.3.0/scrapautoscout/__pycache__/
+-rw-r--r--   0 vicolc     (501) staff       (20)      154 2023-03-16 14:55:35.000000 scrapautoscout-1.3.0/scrapautoscout/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 vicolc     (501) staff       (20)     8877 2023-04-05 10:11:26.000000 scrapautoscout-1.3.0/scrapautoscout/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 vicolc     (501) staff       (20)     2323 2023-04-10 10:43:41.000000 scrapautoscout-1.3.0/scrapautoscout/__pycache__/pipeline.cpython-310.pyc
+-rw-r--r--   0 vicolc     (501) staff       (20)     3094 2023-04-07 09:58:17.000000 scrapautoscout-1.3.0/scrapautoscout/__pycache__/proxies.cpython-310.pyc
+-rw-r--r--   0 vicolc     (501) staff       (20)    21488 2023-05-03 15:23:55.000000 scrapautoscout-1.3.0/scrapautoscout/__pycache__/scrapper.cpython-310.pyc
+-rw-r--r--   0 vicolc     (501) staff       (20)     5771 2023-04-05 10:45:15.000000 scrapautoscout-1.3.0/scrapautoscout/__pycache__/transform.cpython-310.pyc
+-rw-r--r--   0 vicolc     (501) staff       (20)     1815 2023-03-28 11:38:09.000000 scrapautoscout-1.3.0/scrapautoscout/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 vicolc     (501) staff       (20)    12415 2023-05-17 12:38:18.000000 scrapautoscout-1.3.0/scrapautoscout/config.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     2224 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/scrapautoscout/pipeline.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     3459 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/scrapautoscout/proxies.py
+-rw-r--r--   0 vicolc     (501) staff       (20)    30571 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/scrapautoscout/scrapper.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     7592 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/scrapautoscout/transform.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     1416 2023-03-28 11:10:05.000000 scrapautoscout-1.3.0/scrapautoscout/utils.py
+drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-05-17 13:11:45.526817 scrapautoscout-1.3.0/scrapautoscout.egg-info/
+-rw-r--r--   0 vicolc     (501) staff       (20)     1698 2023-05-17 13:11:45.000000 scrapautoscout-1.3.0/scrapautoscout.egg-info/PKG-INFO
+-rw-r--r--   0 vicolc     (501) staff       (20)     1495 2023-05-17 13:11:45.000000 scrapautoscout-1.3.0/scrapautoscout.egg-info/SOURCES.txt
+-rw-r--r--   0 vicolc     (501) staff       (20)        1 2023-05-17 13:11:45.000000 scrapautoscout-1.3.0/scrapautoscout.egg-info/dependency_links.txt
+-rw-r--r--   0 vicolc     (501) staff       (20)       63 2023-05-17 13:11:45.000000 scrapautoscout-1.3.0/scrapautoscout.egg-info/entry_points.txt
+-rw-r--r--   0 vicolc     (501) staff       (20)       88 2023-05-17 13:11:45.000000 scrapautoscout-1.3.0/scrapautoscout.egg-info/requires.txt
+-rw-r--r--   0 vicolc     (501) staff       (20)       18 2023-05-17 13:11:45.000000 scrapautoscout-1.3.0/scrapautoscout.egg-info/top_level.txt
+-rw-r--r--   0 vicolc     (501) staff       (20)       38 2023-05-17 13:11:45.535199 scrapautoscout-1.3.0/setup.cfg
+-rw-r--r--   0 vicolc     (501) staff       (20)     1144 2023-05-17 13:11:33.000000 scrapautoscout-1.3.0/setup.py
+drwxr-xr-x   0 vicolc     (501) staff       (20)        0 2023-05-17 13:11:45.534176 scrapautoscout-1.3.0/tests/
+-rw-r--r--   0 vicolc     (501) staff       (20)      504 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_calculate_nr_of_pages.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     2134 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_compose_search_url.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      532 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/tests/test_find_all_json_files_with_ids.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      509 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/tests/test_find_ids_left_to_extract.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     5638 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/tests/test_get_all_article_ids.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      743 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_get_all_ids_for_search_url.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     1227 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_get_content_for_article_ids.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      661 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_get_content_from_all_pages.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      970 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_get_details_from_raw_json.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      371 2023-03-23 15:41:35.000000 scrapautoscout-1.3.0/tests/test_get_hash_from_string.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      545 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_get_number_of_articles_from_url.py
+-rw-r--r--   0 vicolc     (501) staff       (20)     1168 2023-04-05 09:33:57.000000 scrapautoscout-1.3.0/tests/test_get_valid_proxies_multithreading.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      364 2023-05-17 12:50:02.000000 scrapautoscout-1.3.0/tests/test_main_extract_json_txt_for_all_known_ids.py
+-rw-r--r--   0 vicolc     (501) staff       (20)      638 2023-03-24 12:41:39.000000 scrapautoscout-1.3.0/tests/test_truncate_useless_date_from_json_text.py
```

### Comparing `scrapautoscout-1.2.0/LICENSE` & `scrapautoscout-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/PKG-INFO` & `scrapautoscout-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: scrapautoscout
-Version: 1.2.0
+Version: 1.3.0
 Summary: autoscout24 web scrapper
 Home-page: https://github.com/viggleUnik/scrapautoscout
 Author: Vicol Cristian
 Author-email: vicol.cristianken@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
@@ -51,9 +50,7 @@
  + --LOGS_LEVEL LOGS_LEVEL - Log level, e.g. 'debug', 'info', 'error'
 
 **After this you can run it with specified parameters, example:**
 
 ```shell
 scrapautoscout --LOCATION 's3' 
 ```
-
-
```

### Comparing `scrapautoscout-1.2.0/README.md` & `scrapautoscout-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/__pycache__/config.cpython-310.pyc` & `scrapautoscout-1.3.0/scrapautoscout/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/__pycache__/pipeline.cpython-310.pyc` & `scrapautoscout-1.3.0/scrapautoscout/__pycache__/pipeline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/__pycache__/proxies.cpython-310.pyc` & `scrapautoscout-1.3.0/scrapautoscout/__pycache__/proxies.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/__pycache__/scrapper.cpython-310.pyc` & `scrapautoscout-1.3.0/scrapautoscout/__pycache__/scrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 10:37:59 2023 UTC, .py size: 30518 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 07e7 3364 3677 0000  o.........3d6w..
+00000000: 6f0d 0d0a 0000 0000 e41d 3564 6b77 0000  o.........5dkw..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0013 0000 0040 0000 0073 a803 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c06 5a06 6400 6401 6c07  ..d.d.l.Z.d.d.l.
 00000060: 5a07 6400 6403 6c08 6d09 5a09 6d0a 5a0a  Z.d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6401 6c0c 5a0c 6400  m.Z...d.d.l.Z.d.
@@ -994,347 +994,350 @@
 00003e10: 0200 0000 2000 7a30 6669 6e64 5f61 6c6c  .... .z0find_all
 00003e20: 5f6a 736f 6e5f 6669 6c65 735f 7769 7468  _json_files_with
 00003e30: 5f69 6473 2e3c 6c6f 6361 6c73 3e2e 3c6c  _ids.<locals>.<l
 00003e40: 6973 7463 6f6d 703e 727f 0000 0072 7a00  istcomp>r....rz.
 00003e50: 0000 da0c 6c69 7374 5f6f 626a 6563 7473  ....list_objects
 00003e60: a902 7281 0000 005a 0650 7265 6669 78da  ..r....Z.Prefix.
 00003e70: 0843 6f6e 7465 6e74 7372 8200 0000 72b9  .Contentsr....r.
-00003e80: 0000 0072 7e00 0000 7232 0000 007a 0745  ...r~...r2...z.E
-00003e90: 7272 6f72 3a20 fa09 6c6f 6361 7469 6f6e  rror: ..location
-00003ea0: 3dfa 0f20 6e6f 7420 7265 636f 676e 697a  =.. not recogniz
-00003eb0: 6564 2913 da04 676c 6f62 7207 0000 0072  ed)...globr....r
-00003ec0: 8f00 0000 7290 0000 0072 8c00 0000 728d  ....r....r....r.
-00003ed0: 0000 0072 8e00 0000 7298 0000 00da 0d67  ...r....r......g
-00003ee0: 6574 5f70 6167 696e 6174 6f72 da08 7061  et_paginator..pa
-00003ef0: 6769 6e61 7465 7299 0000 0072 3f00 0000  ginater....r?...
-00003f00: da05 7370 6c69 7472 5500 0000 722a 0000  ..splitrU...r*..
-00003f10: 0072 a500 0000 7241 0000 0072 a600 0000  .r....rA...r....
-00003f20: 7265 0000 0029 0b72 ec00 0000 da0a 6669  re...).r......fi
-00003f30: 6c65 735f 6a73 6f6e 72a7 0000 0072 7f00  les_jsonr....r..
-00003f40: 0000 da09 7061 6769 6e61 746f 72da 0d70  ....paginator..p
-00003f50: 6167 655f 6974 6572 6174 6f72 7246 0000  age_iteratorrF..
-00003f60: 0072 bd00 0000 72aa 0000 00da 0e66 696c  .r....r......fil
-00003f70: 655f 6261 7365 5f6e 616d 6572 4700 0000  e_base_namerG...
-00003f80: 721b 0000 0072 1b00 0000 7220 0000 0072  r....r....r ...r
-00003f90: ce00 0000 6102 0000 7332 0000 0008 021a  ....a...s2......
-00003fa0: 010e 0104 0108 0104 010e 010a 010a 0112  ................
-00003fb0: 0102 0108 010c 010a 010e 0114 0102 fd02  ................
-00003fc0: ff04 070e fe1a 0104 0108 8002 fe10 0472  ...............r
-00003fd0: ce00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00003fe0: 0005 0000 0009 0000 0043 0000 0073 6a00  .........C...sj.
-00003ff0: 0000 7400 a000 7401 6a02 9b00 6401 7401  ..t...t.j...d.t.
-00004000: 6a03 9b00 6402 9d04 a101 7d00 6700 7d01  j...d.....}.g.}.
-00004010: 7c00 4400 5d21 7d02 7404 7c02 6403 8302  |.D.]!}.t.|.d...
-00004020: 8f12 7d03 7405 a006 7c03 a101 7d04 7c01  ..}.t...|...}.|.
-00004030: a007 7c04 a101 0100 5700 6400 0400 0400  ..|.....W.d.....
-00004040: 8303 0100 6e08 3100 732d 7701 0100 0100  ....n.1.s-w.....
-00004050: 0100 5900 0100 7111 7c01 5300 2904 4e72  ..Y...q.|.S.).Nr
-00004060: 1800 0000 72ed 0000 00da 0172 2908 72f9  ....r......r).r.
-00004070: 0000 0072 0700 0000 728f 0000 0072 9000  ...r....r....r..
-00004080: 0000 7295 0000 0072 9600 0000 7297 0000  ..r....r....r...
-00004090: 0072 d100 0000 2905 72fd 0000 0072 d200  .r....).r....r..
-000040a0: 0000 5a09 6669 6c65 5f6a 736f 6eda 0466  ..Z.file_json..f
-000040b0: 696c 6572 a900 0000 721b 0000 0072 1b00  iler....r....r..
-000040c0: 0000 7220 0000 00da 186c 6f61 645f 616c  ..r .....load_al
-000040d0: 6c5f 6b6e 6f77 6e5f 6964 735f 6c6f 6361  l_known_ids_loca
-000040e0: 6c7a 0200 0073 1200 0000 1a01 0401 0802  lz...s..........
-000040f0: 0c01 0a01 0c01 1cfe 0280 0404 7203 0100  ............r...
-00004100: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
-00004110: 0000 0600 0000 4300 0000 732c 0000 0074  ......C...s,...t
-00004120: 00a0 0074 016a 029b 0064 0174 016a 039b  ...t.j...d.t.j..
-00004130: 0064 029d 04a1 017d 0064 0364 0484 007c  .d.....}.d.d...|
-00004140: 0044 0083 017d 017c 0153 0029 054e 7218  .D...}.|.S.).Nr.
-00004150: 0000 0072 ed00 0000 6301 0000 0000 0000  ...r....c.......
-00004160: 0000 0000 0002 0000 0006 0000 0053 0000  .............S..
-00004170: 0072 ee00 0000 72ef 0000 0072 f000 0000  .r....r....r....
-00004180: 72f2 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00004190: 2000 0000 7226 0000 0088 0200 0072 f300   ...r&.......r..
-000041a0: 0000 7a3c 6c6f 6164 5f69 6473 5f6f 665f  ..z<load_ids_of_
-000041b0: 616c 6c5f 6578 7472 6163 7465 645f 6172  all_extracted_ar
-000041c0: 7469 636c 6573 5f6c 6f63 616c 2e3c 6c6f  ticles_local.<lo
-000041d0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000041e0: 2904 72f9 0000 0072 0700 0000 728f 0000  ).r....r....r...
-000041f0: 00da 0f46 4f4c 4445 525f 4152 5449 434c  ...FOLDER_ARTICL
-00004200: 4553 2902 72fd 0000 005a 1361 6c6c 5f69  ES).r....Z.all_i
-00004210: 6473 5f6f 665f 6172 7469 636c 6573 721b  ds_of_articlesr.
-00004220: 0000 0072 1b00 0000 7220 0000 00da 286c  ...r....r ....(l
-00004230: 6f61 645f 6964 735f 6f66 5f61 6c6c 5f65  oad_ids_of_all_e
-00004240: 7874 7261 6374 6564 5f61 7274 6963 6c65  xtracted_article
-00004250: 735f 6c6f 6361 6c86 0200 0073 0600 0000  s_local....s....
-00004260: 1a01 0e01 0401 7205 0100 0063 0000 0000  ......r....c....
-00004270: 0000 0000 0000 0000 0b00 0000 0a00 0000  ................
-00004280: 4300 0000 73e0 0000 0074 006a 0174 026a  C...s....t.j.t.j
-00004290: 0364 018d 017d 007c 00a0 0464 02a1 017d  .d...}.|...d...}
-000042a0: 017c 01a0 0564 03a1 017d 027c 026a 0674  .|...d...}.|.j.t
-000042b0: 026a 0774 026a 0864 048d 027d 0367 007d  .j.t.j.d...}.g.}
-000042c0: 047a 2c7c 0344 005d 277d 057c 0564 0519  .z,|.D.]'}.|.d..
-000042d0: 0044 005d 207d 067c 06a0 0964 06a1 017d  .D.] }.|...d...}
-000042e0: 077c 016a 0a74 026a 077c 0764 078d 027d  .|.j.t.j.|.d...}
-000042f0: 0874 0ba0 0c7c 0864 0819 00a0 0da1 00a0  .t...|.d........
-00004300: 0e64 09a1 01a1 017d 097c 04a0 0f7c 09a1  .d.....}.|...|..
-00004310: 0101 0071 2571 1f57 006e 1a04 0074 1079  ...q%q.W.n...t.y
-00004320: 6201 007d 0a01 007a 0e74 11a0 1264 0a7c  b..}...z.t...d.|
-00004330: 0a9b 009d 02a1 0101 0057 0059 0064 007d  .........W.Y.d.}
-00004340: 0a7e 0a6e 0564 007d 0a7e 0a77 0177 0074  .~.n.d.}.~.w.w.t
-00004350: 11a0 1364 0b74 147c 0483 019b 0064 0c9d  ...d.t.|.....d..
-00004360: 03a1 0101 007c 0453 0029 0d4e 727a 0000  .....|.S.).Nrz..
-00004370: 0072 7f00 0000 72f4 0000 0072 f500 0000  .r....r....r....
-00004380: 72f6 0000 0072 8200 0000 7280 0000 0072  r....r....r....r
-00004390: 8400 0000 7285 0000 007a 1a45 7272 6f72  ....r....z.Error
-000043a0: 2067 6574 7469 6e67 206f 626a 2066 726f   getting obj fro
-000043b0: 6d20 7333 207a 0e41 6c6c 204b 6e6f 776e  m s3 z.All Known
-000043c0: 2049 6473 2072 1600 0000 2915 728c 0000   Ids r....).r...
-000043d0: 0072 8d00 0000 7207 0000 0072 8e00 0000  .r....r....r....
-000043e0: 7298 0000 0072 fa00 0000 72fb 0000 0072  r....r....r....r
-000043f0: 9900 0000 7290 0000 0072 3f00 0000 729b  ....r....r?...r.
-00004400: 0000 0072 9600 0000 729c 0000 0072 9d00  ...r....r....r..
-00004410: 0000 729e 0000 0072 d100 0000 72a5 0000  ..r....r....r...
-00004420: 0072 4100 0000 72a6 0000 0072 9a00 0000  .rA...r....r....
-00004430: 724d 0000 0029 0b72 a700 0000 727f 0000  rM...).r....r...
-00004440: 0072 fe00 0000 72ff 0000 0072 d200 0000  .r....r....r....
-00004450: 7246 0000 0072 bd00 0000 72aa 0000 005a  rF...r....r....Z
-00004460: 0872 6573 706f 6e73 6572 a900 0000 7247  .responser....rG
-00004470: 0000 0072 1b00 0000 721b 0000 0072 2000  ...r....r....r .
-00004480: 0000 da15 6c6f 6164 5f61 6c6c 5f6b 6e6f  ....load_all_kno
-00004490: 776e 5f69 6473 5f73 338c 0200 0073 2800  wn_ids_s3....s(.
-000044a0: 0000 0e01 0a01 0a02 1201 0401 0201 0801  ................
-000044b0: 0c01 0a01 1001 1801 0c01 02fc 04ff 0e06  ................
-000044c0: 1c01 0880 02ff 1603 0401 7206 0100 0063  ..........r....c
-000044d0: 0000 0000 0000 0000 0000 0000 0900 0000  ................
-000044e0: 0a00 0000 4300 0000 73c8 0000 0074 006a  ....C...s....t.j
-000044f0: 0174 026a 0364 018d 017d 007c 00a0 0464  .t.j.d...}.|...d
-00004500: 02a1 017d 017c 01a0 0564 03a1 017d 0267  ...}.|...d...}.g
-00004510: 007d 037a 2a7c 026a 0674 026a 0774 026a  .}.z*|.j.t.j.t.j
-00004520: 0864 048d 0244 005d 1e7d 047c 0464 0519  .d...D.].}.|.d..
-00004530: 0044 005d 177d 057c 05a0 0964 06a1 017d  .D.].}.|...d...}
-00004540: 067c 06a0 0a64 07a1 0164 0819 007d 077c  .|...d...d...}.|
-00004550: 03a0 0b7c 07a0 0c64 0964 0aa1 02a1 0101  ...|...d.d......
-00004560: 0071 2371 1d57 006e 1a04 0074 0d79 5701  .q#q.W.n...t.yW.
-00004570: 007d 0801 007a 0e74 0ea0 0f64 0b7c 089b  .}...z.t...d.|..
-00004580: 009d 02a1 0101 0057 0059 0064 007d 087e  .......W.Y.d.}.~
-00004590: 086e 0564 007d 087e 0877 0177 0074 0ea0  .n.d.}.~.w.w.t..
-000045a0: 1064 0c74 117c 0383 019b 009d 02a1 0101  .d.t.|..........
-000045b0: 007c 0353 0029 0d4e 727a 0000 0072 7f00  .|.S.).Nrz...r..
-000045c0: 0000 72f4 0000 0072 f500 0000 72f6 0000  ..r....r....r...
-000045d0: 0072 8200 0000 7218 0000 0072 b900 0000  .r....r....r....
-000045e0: 727e 0000 0072 3200 0000 7a1d 4572 726f  r~...r2...z.Erro
-000045f0: 7220 6c69 7374 696e 6720 6f62 6a65 6374  r listing object
-00004600: 7320 696e 2073 333a 207a 0e45 7874 7261  s in s3: z.Extra
-00004610: 6374 6564 2049 6473 2029 1272 8c00 0000  cted Ids ).r....
-00004620: 728d 0000 0072 0700 0000 728e 0000 0072  r....r....r....r
-00004630: 9800 0000 72fa 0000 0072 fb00 0000 7299  ....r....r....r.
-00004640: 0000 0072 0401 0000 723f 0000 0072 fc00  ...r....r?...r..
-00004650: 0000 7255 0000 0072 2a00 0000 72a5 0000  ..rU...r*...r...
-00004660: 0072 4100 0000 72a6 0000 0072 9a00 0000  .rA...r....r....
-00004670: 724d 0000 0029 0972 a700 0000 727f 0000  rM...).r....r...
-00004680: 0072 fe00 0000 5a11 616c 6c5f 6964 735f  .r....Z.all_ids_
-00004690: 6578 7472 6163 7465 6472 4600 0000 72bd  extractedrF...r.
-000046a0: 0000 0072 aa00 0000 7200 0100 0072 4700  ...r....r....rG.
-000046b0: 0000 721b 0000 0072 1b00 0000 7220 0000  ..r....r....r ..
-000046c0: 00da 256c 6f61 645f 6964 735f 6f66 5f61  ..%load_ids_of_a
-000046d0: 6c6c 5f65 7874 7261 6374 6564 5f61 7274  ll_extracted_art
-000046e0: 6963 6c65 735f 7333 a102 0000 7324 0000  icles_s3....s$..
-000046f0: 000e 010a 010a 0204 0102 0116 010c 010a  ................
-00004700: 010e 0114 0102 fd04 ff0e 051c 0108 8002  ................
-00004710: ff14 0304 0172 0701 0000 6301 0000 0000  .....r....c.....
-00004720: 0000 0000 0000 0004 0000 0009 0000 0043  ...............C
-00004730: 0000 0073 9600 0000 7c00 6400 7500 7207  ...s....|.d.u.r.
-00004740: 7400 6a01 7d00 7c00 6401 6b02 7212 7402  t.j.}.|.d.k.r.t.
-00004750: 8300 7d01 7403 8300 7d02 6e13 7c00 6402  ..}.t...}.n.|.d.
-00004760: 6b02 721d 7404 8300 7d01 7405 8300 7d02  k.r.t...}.t...}.
-00004770: 6e08 7406 6403 7c00 9b00 6404 9d03 8301  n.t.d.|...d.....
-00004780: 8201 7407 7c01 8301 7d01 7407 7c02 8301  ..t.|...}.t.|...
-00004790: 7d02 7408 7c01 a009 7c02 a101 8301 7d03  }.t.|...|.....}.
-000047a0: 740a a00b 6405 740c 7c03 8301 9b00 6406  t...d.t.|.....d.
-000047b0: 740c 7c01 8301 9b00 6407 740c 7c02 8301  t.|.....d.t.|...
-000047c0: 9b00 6408 9d07 a101 0100 7c03 5300 2909  ..d.......|.S.).
-000047d0: 4e72 7700 0000 727f 0000 0072 f700 0000  Nrw...r....r....
-000047e0: 72f8 0000 007a 0666 6f75 6e64 207a 1620  r....z.found z. 
-000047f0: 4944 7320 6c65 6674 2074 6f20 6578 7472  IDs left to extr
-00004800: 6163 7420 287a 0820 6b6e 6f77 6e2c 207a  act (z. known, z
-00004810: 0b20 6578 7472 6163 7465 6429 290d 7207  . extracted)).r.
-00004820: 0000 0072 c900 0000 7203 0100 0072 0501  ...r....r....r..
-00004830: 0000 7206 0100 0072 0701 0000 7265 0000  ..r....r....re..
-00004840: 0072 a100 0000 723c 0000 00da 0a64 6966  .r....r<.....dif
-00004850: 6665 7265 6e63 6572 4100 0000 7242 0000  ferencerA...rB..
-00004860: 0072 4d00 0000 2904 72ec 0000 005a 0969  .rM...).r....Z.i
-00004870: 6473 5f6b 6e6f 776e 5a0d 6964 735f 6578  ds_knownZ.ids_ex
-00004880: 7472 6163 7465 645a 1369 6473 5f6c 6566  tractedZ.ids_lef
-00004890: 745f 746f 5f65 7874 7261 6374 721b 0000  t_to_extractr...
-000048a0: 0072 1b00 0000 7220 0000 00da 1866 696e  .r....r .....fin
-000048b0: 645f 6964 735f 6c65 6674 5f74 6f5f 6578  d_ids_left_to_ex
-000048c0: 7472 6163 74b4 0200 0073 2400 0000 0801  tract....s$.....
-000048d0: 0601 0802 0601 0801 0801 0601 0801 1002  ................
-000048e0: 0802 0801 0e01 1001 0601 04ff 0601 0aff  ................
-000048f0: 0403 7209 0100 0063 0200 0000 0000 0000  ..r....c........
-00004900: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
-00004910: 7366 0000 0074 006a 019b 0064 0174 006a  sf...t.j...d.t.j
-00004920: 029b 009d 037d 0274 036a 047c 0264 0264  .....}.t.j.|.d.d
-00004930: 038d 0201 0074 057c 029b 0064 017c 019b  .....t.|...d.|..
-00004940: 0064 049d 0464 0583 028f 0e7d 037c 03a0  .d...d.....}.|..
-00004950: 067c 00a1 0101 0057 0064 0004 0004 0083  .|.....W.d......
-00004960: 0301 0064 0053 0031 0073 2c77 0101 0001  ...d.S.1.s,w....
-00004970: 0001 0059 0001 0064 0053 0029 064e 7218  ...Y...d.S.).Nr.
-00004980: 0000 0054 727c 0000 0072 7e00 0000 7287  ...Tr|...r~...r.
-00004990: 0000 0029 0772 0700 0000 728f 0000 0072  ...).r....r....r
-000049a0: 0401 0000 7291 0000 0072 9200 0000 7295  ....r....r....r.
-000049b0: 0000 00da 0577 7269 7465 2904 72db 0000  .....write).r...
-000049c0: 00da 0a69 645f 6172 7469 636c 655a 0964  ...id_articleZ.d
-000049d0: 6972 5f6c 6f63 616c 72a8 0000 0072 1b00  ir_localr....r..
-000049e0: 0000 721b 0000 0072 2000 0000 da16 7361  ..r....r .....sa
-000049f0: 7665 5f6a 736f 6e5f 7478 745f 746f 5f6c  ve_json_txt_to_l
-00004a00: 6f63 616c ca02 0000 730a 0000 0012 010e  ocal....s.......
-00004a10: 0118 020c 0122 ff72 0c01 0000 6302 0000  .....".r....c...
-00004a20: 0000 0000 0000 0000 0007 0000 000a 0000  ................
-00004a30: 0043 0000 0073 8400 0000 7400 6a01 7402  .C...s....t.j.t.
-00004a40: 6a03 6401 8d01 7d02 7c02 a004 6402 a101  j.d...}.|...d...
-00004a50: 7d03 7405 a006 7c00 a101 7d04 7402 6a07  }.t...|...}.t.j.
-00004a60: 9b00 6403 7c01 9b00 6404 9d04 7d05 7a0c  ..d.|...d...}.z.
-00004a70: 7c03 6a08 7402 6a09 7c05 7c04 6405 8d03  |.j.t.j.|.|.d...
-00004a80: 0100 5700 6400 5300 0400 740a 7941 0100  ..W.d.S...t.yA..
-00004a90: 7d06 0100 7a0f 740b a00c 6406 7c06 9b00  }...z.t...d.|...
-00004aa0: 9d02 a101 0100 5700 5900 6400 7d06 7e06  ......W.Y.d.}.~.
-00004ab0: 6400 5300 6400 7d06 7e06 7701 7700 2907  d.S.d.}.~.w.w.).
-00004ac0: 4e72 7a00 0000 727f 0000 0072 1800 0000  Nrz...r....r....
-00004ad0: 727e 0000 0072 8a00 0000 728b 0000 0029  r~...r....r....)
-00004ae0: 0d72 8c00 0000 728d 0000 0072 0700 0000  .r....r....r....
-00004af0: 728e 0000 0072 9800 0000 7296 0000 0072  r....r....r....r
-00004b00: a300 0000 7204 0100 0072 a400 0000 7299  ....r....r....r.
-00004b10: 0000 0072 a500 0000 7241 0000 0072 a600  ...r....rA...r..
-00004b20: 0000 2907 72db 0000 0072 0b01 0000 72a7  ..).r....r....r.
-00004b30: 0000 0072 7f00 0000 72ab 0000 0072 aa00  ...r....r....r..
-00004b40: 0000 7247 0000 0072 1b00 0000 721b 0000  ..rG...r....r...
-00004b50: 0072 2000 0000 da13 7361 7665 5f6a 736f  .r .....save_jso
-00004b60: 6e5f 7478 745f 746f 5f73 33d2 0200 0073  n_txt_to_s3....s
-00004b70: 1400 0000 0e01 0a01 0a01 1201 0201 1801  ................
-00004b80: 0e01 1e01 0880 02ff 720d 0100 0063 0300  ........r....c..
-00004b90: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00004ba0: 0000 4300 0000 7334 0000 007c 0264 016b  ..C...s4...|.d.k
-00004bb0: 0272 0974 007c 007c 0183 0253 007c 0264  .r.t.|.|...S.|.d
-00004bc0: 026b 0272 1274 017c 007c 0183 0253 0074  .k.r.t.|.|...S.t
-00004bd0: 0264 037c 029b 0064 049d 0383 0182 0129  .d.|...d.......)
-00004be0: 054e 7277 0000 0072 7f00 0000 72f7 0000  .Nrw...r....r...
-00004bf0: 0072 f800 0000 2903 720c 0100 0072 0d01  .r....).r....r..
-00004c00: 0000 7265 0000 00a9 0372 db00 0000 720b  ..re.....r....r.
-00004c10: 0100 0072 ec00 0000 721b 0000 0072 1b00  ...r....r....r..
-00004c20: 0000 7220 0000 00da 0d73 6176 655f 6a73  ..r .....save_js
-00004c30: 6f6e 5f74 7874 df02 0000 730a 0000 0008  on_txt....s.....
-00004c40: 010a 0108 010a 0110 0272 0f01 0000 e9e8  .........r......
-00004c50: 0300 00da 0a63 6875 6e6b 5f73 697a 6563  .....chunk_sizec
-00004c60: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
-00004c70: 0800 0000 4300 0000 732c 0100 0074 00a0  ....C...s,...t..
-00004c80: 0164 01a1 0101 007c 0064 0075 0072 0c74  .d.....|.d.u.r.t
-00004c90: 026a 037d 0074 047c 0083 017d 0264 027d  .j.}.t.|...}.d.}
-00004ca0: 0364 027d 0474 057c 0283 017d 0574 067c  .d.}.t.|...}.t.|
-00004cb0: 0564 0364 0464 0564 068d 047d 0674 057c  .d.d.d.d...}.t.|
-00004cc0: 0283 0164 026b 0472 877c 0264 007c 0185  ...d.k.r.|.d.|..
-00004cd0: 0219 007c 027c 0164 0085 0219 0002 027d  ...|.|.d.......}
-00004ce0: 077d 0274 077c 0783 017d 087c 0374 057c  .}.t.|...}.|.t.|
-00004cf0: 0783 0137 007d 037c 08a0 08a1 0044 005d  ...7.}.|.....D.]
-00004d00: 235c 027d 097d 0a7a 0674 097c 0a83 017d  #\.}.}.z.t.|...}
-00004d10: 0b57 006e 0d01 0001 0001 0074 00a0 0a64  .W.n.......t...d
-00004d20: 077c 099b 009d 02a1 0101 0059 0071 4174  .|.........Y.qAt
-00004d30: 0b7c 0b7c 097c 0064 088d 0301 007c 0464  .|.|.|.d.....|.d
-00004d40: 0937 007d 0471 4174 00a0 0c7c 037c 051b  .7.}.qAt...|.|..
-00004d50: 0064 0514 0064 0a9b 0464 0b7c 047c 031b  .d...d...d.|.|..
-00004d60: 0064 0514 0064 0a9b 0464 0c9d 04a1 0101  .d...d...d......
-00004d70: 007c 06a0 0d74 057c 0783 01a1 0101 0074  .|...t.|.......t
-00004d80: 057c 0283 0164 026b 0473 267c 06a0 0ea1  .|...d.k.s&|....
-00004d90: 0001 007c 06a0 0fa1 0001 0074 00a0 0164  ...|.......t...d
-00004da0: 0da1 0101 0064 0053 0029 0e4e 7a36 6d61  .....d.S.).Nz6ma
-00004db0: 696e 5f65 7874 7261 6374 5f6a 736f 6e5f  in_extract_json_
-00004dc0: 7478 745f 666f 725f 616c 6c5f 6b6e 6f77  txt_for_all_know
-00004dd0: 6e5f 6964 7328 293a 2053 7461 7274 696e  n_ids(): Startin
-00004de0: 672e 2e2e 7201 0000 005a 0249 44e9 1e00  g...r....Z.ID...
-00004df0: 0000 7257 0000 0029 04da 0574 6f74 616c  ..rW...)...total
-00004e00: 5a04 756e 6974 5a0b 6d69 6e69 6e74 6572  Z.unitZ.mininter
-00004e10: 7661 6c5a 086d 696e 6974 6572 737a 4246  valZ.miniterszBF
-00004e20: 6169 6c65 6420 746f 2067 6574 206a 736f  ailed to get jso
-00004e30: 6e20 7478 7420 6672 6f6d 2042 6561 7574  n txt from Beaut
-00004e40: 6966 756c 536f 7570 206f 626a 206f 6620  ifulSoup obj of 
-00004e50: 6172 7469 636c 6520 7769 7468 2049 443a  article with ID:
-00004e60: 2072 0e01 0000 725d 0000 0072 5e00 0000   r....r]...r^...
-00004e70: 7a22 2520 6f66 2049 4473 2061 7474 656d  z"% of IDs attem
-00004e80: 7074 6564 2c20 7375 6363 6573 7320 7261  pted, success ra
-00004e90: 7465 3a20 fa01 257a 306d 6169 6e5f 6578  te: ..%z0main_ex
-00004ea0: 7472 6163 745f 6a73 6f6e 5f74 7874 5f66  tract_json_txt_f
-00004eb0: 6f72 5f61 6c6c 5f6b 6e6f 776e 5f69 6473  or_all_known_ids
-00004ec0: 2829 3a20 446f 6e65 2e29 1072 4100 0000  (): Done.).rA...
-00004ed0: 729a 0000 0072 0700 0000 72c9 0000 0072  r....r....r....r
-00004ee0: 0901 0000 724d 0000 0072 0600 0000 72d8  ....rM...r....r.
-00004ef0: 0000 0072 2c00 0000 72dc 0000 0072 a600  ...r,...r....r..
-00004f00: 0000 720f 0100 0072 4200 0000 722b 0000  ..r....rB...r+..
-00004f10: 005a 0764 6973 706c 6179 da05 636c 6f73  .Z.display..clos
-00004f20: 6529 0c72 ec00 0000 7211 0100 0072 a900  e).r....r....r..
-00004f30: 0000 5a0b 6e5f 6174 7465 6d70 7465 645a  ..Z.n_attemptedZ
-00004f40: 0b6e 5f65 7874 7261 6374 6564 5a0a 6e5f  .n_extractedZ.n_
-00004f50: 696e 6974 5f69 6473 5a02 7062 5a08 6964  init_idsZ.pbZ.id
-00004f60: 735f 7061 7274 7267 0000 0072 0b01 0000  s_partrg...r....
-00004f70: 5a0f 636f 6e74 656e 745f 6172 7469 636c  Z.content_articl
-00004f80: 6572 db00 0000 721b 0000 0072 1b00 0000  er....r....r....
-00004f90: 7220 0000 00da 276d 6169 6e5f 6578 7472  r ....'main_extr
-00004fa0: 6163 745f 6a73 6f6e 5f74 7874 5f66 6f72  act_json_txt_for
-00004fb0: 5f61 6c6c 5f6b 6e6f 776e 5f69 6473 e802  _all_known_ids..
-00004fc0: 0000 7338 0000 000a 0108 0206 0108 0204  ..s8............
-00004fd0: 0104 0108 0110 010c 021a 0108 010c 0110  ................
-00004fe0: 0202 010c 0106 0110 0104 010e 020a 0114  ................
-00004ff0: 020c 010a ff0e 020c ef08 1308 010e 0172  ...............r
-00005000: 1601 0000 2902 4e72 3100 0000 2903 5454  ....).Nr1...).TT
-00005010: 7231 0000 0029 0572 5700 0000 544e 7231  r1...).rW...TNr1
-00005020: 0000 0072 3100 0000 721a 0000 0029 024e  ...r1...r....).N
-00005030: 7277 0000 0029 0372 b600 0000 5472 3100  rw...).r....Tr1.
-00005040: 0000 2901 7277 0000 0029 024e 7210 0100  ..).rw...).Nr...
-00005050: 0029 4672 e800 0000 5a07 6f73 2e70 6174  .)Fr....Z.os.pat
-00005060: 6872 9100 0000 723e 0000 005a 0362 7334  hr....r>...Z.bs4
-00005070: 7202 0000 0072 9600 0000 725f 0000 00da  r....r....r_....
-00005080: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
-00005090: 0072 0500 0000 da07 6c6f 6767 696e 6772  .r......loggingr
-000050a0: 4a00 0000 728c 0000 0072 bf00 0000 5a12  J...r....r....Z.
-000050b0: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-000050c0: 6573 7261 0000 0072 f900 0000 7206 0000  esra...r....r...
-000050d0: 00da 1573 6372 6170 6175 746f 7363 6f75  ...scrapautoscou
-000050e0: 742e 636f 6e66 6967 7207 0000 005a 1673  t.configr....Z.s
-000050f0: 6372 6170 6175 746f 7363 6f75 742e 7072  crapautoscout.pr
-00005100: 6f78 6965 7372 0800 0000 5a14 7363 7261  oxiesr....Z.scra
-00005110: 7061 7574 6f73 636f 7574 2e75 7469 6c73  pautoscout.utils
-00005120: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00005130: 0c00 0000 720d 0000 00da 0967 6574 4c6f  ....r......getLo
-00005140: 6767 6572 7293 0000 0072 f100 0000 da08  ggerr....r......
-00005150: 5f5f 6669 6c65 5f5f 7241 0000 0072 4e00  __file__rA...rN.
-00005160: 0000 da08 5349 5445 5f55 524c da03 7374  ....SITE_URL..st
-00005170: 7272 bb00 0000 7230 0000 0072 4800 0000  rr....r0...rH...
-00005180: 7253 0000 0072 5600 0000 da04 626f 6f6c  rS...rV.....bool
-00005190: 726a 0000 00da 094d 4158 5f50 4147 4553  rj.....MAX_PAGES
-000051a0: 7270 0000 0072 7600 0000 72ac 0000 0072  rp...rv...r....r
-000051b0: b500 0000 729f 0000 00da 144d 4158 5f52  ....r......MAX_R
-000051c0: 4553 554c 5453 5f50 4552 5f50 4147 4572  ESULTS_PER_PAGEr
-000051d0: a000 0000 da0b 4d41 585f 5245 5355 4c54  ......MAX_RESULT
-000051e0: 5372 d400 0000 72d5 0000 0072 d800 0000  Sr....r....r....
-000051f0: 72dc 0000 0072 e700 0000 72da 0000 0072  r....r....r....r
-00005200: ce00 0000 7203 0100 0072 0501 0000 7206  ....r....r....r.
-00005210: 0100 0072 0701 0000 7209 0100 0072 0c01  ...r....r....r..
-00005220: 0000 720d 0100 0072 0f01 0000 7216 0100  ..r....r....r...
-00005230: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
-00005240: 7220 0000 00da 083c 6d6f 6475 6c65 3e01  r .....<module>.
-00005250: 0000 0073 6201 0000 0800 0801 0801 0c01  ...sb...........
-00005260: 0801 0801 1401 0801 0801 0801 0801 0801  ................
-00005270: 0801 0c01 0c03 0c01 1c01 1203 0402 0404  ................
-00005280: 0201 0201 0201 0201 0201 0201 04f9 0201  ................
-00005290: 02ff 0202 02fe 0203 02fd 0204 02fc 0205  ................
-000052a0: 02fb 0206 02fa 0207 02f9 0209 0af7 0a2f  .............../
-000052b0: 100e 1c13 020c 0201 0201 0201 0201 04fa  ................
-000052c0: 0601 02ff 0202 02fe 0203 02fd 0204 02fc  ................
-000052d0: 0205 02fb 0206 02fa 0a07 0af9 0455 0201  .............U..
-000052e0: 0201 0201 04fb 0201 02ff 0202 02fe 0203  ................
-000052f0: 02fd 0204 02fc 0205 02fb 0606 0afa 201b  .............. .
-00005300: 0215 0201 04fd 0201 02ff 0202 02fe 0203  ................
-00005310: 0afd 0440 0201 0201 04fc 0201 02ff 0202  ...@............
-00005320: 02fe 0203 02fd 0204 0afc 1419 0429 0401  .............)..
-00005330: 04fd 0201 02ff 0202 02fe 0203 02fd 0204  ................
-00005340: 0afc 0209 0201 0201 0201 0401 0201 0201  ................
-00005350: 0201 0201 04f7 0601 02ff 0a02 02fe 0a03  ................
-00005360: 02fd 0204 02fc 0205 02fb 0206 02fa 0207  ................
-00005370: 02f9 0208 02f8 0209 0af7 007f 1417 0406  ................
-00005380: 0201 0201 0201 04fb 0601 02ff 0202 02fe  ................
-00005390: 0203 02fd 0204 02fc 0205 02fb 0a06 0afa  ................
-000053a0: 1223 0e07 0e09 1018 1219 120c 0806 0815  .#..............
-000053b0: 1013 0816 0808 100d 1809                 ..........
+00003e80: 0000 0072 7e00 0000 7232 0000 007a 1945  ...r~...r2...z.E
+00003e90: 7272 6f72 206e 6f20 6669 6c65 7320 7769  rror no files wi
+00003ea0: 7468 2069 6473 3a20 fa09 6c6f 6361 7469  th ids: ..locati
+00003eb0: 6f6e 3dfa 0f20 6e6f 7420 7265 636f 676e  on=.. not recogn
+00003ec0: 697a 6564 2913 da04 676c 6f62 7207 0000  ized)...globr...
+00003ed0: 0072 8f00 0000 7290 0000 0072 8c00 0000  .r....r....r....
+00003ee0: 728d 0000 0072 8e00 0000 7298 0000 00da  r....r....r.....
+00003ef0: 0d67 6574 5f70 6167 696e 6174 6f72 da08  .get_paginator..
+00003f00: 7061 6769 6e61 7465 7299 0000 0072 3f00  paginater....r?.
+00003f10: 0000 da05 7370 6c69 7472 5500 0000 722a  ....splitrU...r*
+00003f20: 0000 0072 a500 0000 7241 0000 0072 a600  ...r....rA...r..
+00003f30: 0000 7265 0000 0029 0b72 ec00 0000 da0a  ..re...).r......
+00003f40: 6669 6c65 735f 6a73 6f6e 72a7 0000 0072  files_jsonr....r
+00003f50: 7f00 0000 da09 7061 6769 6e61 746f 72da  ......paginator.
+00003f60: 0d70 6167 655f 6974 6572 6174 6f72 7246  .page_iteratorrF
+00003f70: 0000 0072 bd00 0000 72aa 0000 00da 0e66  ...r....r......f
+00003f80: 696c 655f 6261 7365 5f6e 616d 6572 4700  ile_base_namerG.
+00003f90: 0000 721b 0000 0072 1b00 0000 7220 0000  ..r....r....r ..
+00003fa0: 0072 ce00 0000 6102 0000 7332 0000 0008  .r....a...s2....
+00003fb0: 021a 010e 0104 0108 0104 010e 010a 010a  ................
+00003fc0: 0112 0102 0108 010c 010a 010e 0114 0102  ................
+00003fd0: fd02 ff04 070e fe1a 0104 0108 8002 fe10  ................
+00003fe0: 0472 ce00 0000 6300 0000 0000 0000 0000  .r....c.........
+00003ff0: 0000 0005 0000 0009 0000 0043 0000 0073  ...........C...s
+00004000: 6a00 0000 7400 a000 7401 6a02 9b00 6401  j...t...t.j...d.
+00004010: 7401 6a03 9b00 6402 9d04 a101 7d00 6700  t.j...d.....}.g.
+00004020: 7d01 7c00 4400 5d21 7d02 7404 7c02 6403  }.|.D.]!}.t.|.d.
+00004030: 8302 8f12 7d03 7405 a006 7c03 a101 7d04  ....}.t...|...}.
+00004040: 7c01 a007 7c04 a101 0100 5700 6400 0400  |...|.....W.d...
+00004050: 0400 8303 0100 6e08 3100 732d 7701 0100  ......n.1.s-w...
+00004060: 0100 0100 5900 0100 7111 7c01 5300 2904  ....Y...q.|.S.).
+00004070: 4e72 1800 0000 72ed 0000 00da 0172 2908  Nr....r......r).
+00004080: 72f9 0000 0072 0700 0000 728f 0000 0072  r....r....r....r
+00004090: 9000 0000 7295 0000 0072 9600 0000 7297  ....r....r....r.
+000040a0: 0000 0072 d100 0000 2905 72fd 0000 0072  ...r....).r....r
+000040b0: d200 0000 5a09 6669 6c65 5f6a 736f 6eda  ....Z.file_json.
+000040c0: 0466 696c 6572 a900 0000 721b 0000 0072  .filer....r....r
+000040d0: 1b00 0000 7220 0000 00da 186c 6f61 645f  ....r .....load_
+000040e0: 616c 6c5f 6b6e 6f77 6e5f 6964 735f 6c6f  all_known_ids_lo
+000040f0: 6361 6c7a 0200 0073 1200 0000 1a01 0401  calz...s........
+00004100: 0802 0c01 0a01 0c01 1cfe 0280 0404 7203  ..............r.
+00004110: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00004120: 0200 0000 0600 0000 4300 0000 732c 0000  ........C...s,..
+00004130: 0074 00a0 0074 016a 029b 0064 0174 016a  .t...t.j...d.t.j
+00004140: 039b 0064 029d 04a1 017d 0064 0364 0484  ...d.....}.d.d..
+00004150: 007c 0044 0083 017d 017c 0153 0029 054e  .|.D...}.|.S.).N
+00004160: 7218 0000 0072 ed00 0000 6301 0000 0000  r....r....c.....
+00004170: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
+00004180: 0000 0072 ee00 0000 72ef 0000 0072 f000  ...r....r....r..
+00004190: 0000 72f2 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+000041a0: 0072 2000 0000 7226 0000 0088 0200 0072  .r ...r&.......r
+000041b0: f300 0000 7a3c 6c6f 6164 5f69 6473 5f6f  ....z<load_ids_o
+000041c0: 665f 616c 6c5f 6578 7472 6163 7465 645f  f_all_extracted_
+000041d0: 6172 7469 636c 6573 5f6c 6f63 616c 2e3c  articles_local.<
+000041e0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000041f0: 703e 2904 72f9 0000 0072 0700 0000 728f  p>).r....r....r.
+00004200: 0000 00da 0f46 4f4c 4445 525f 4152 5449  .....FOLDER_ARTI
+00004210: 434c 4553 2902 72fd 0000 005a 1361 6c6c  CLES).r....Z.all
+00004220: 5f69 6473 5f6f 665f 6172 7469 636c 6573  _ids_of_articles
+00004230: 721b 0000 0072 1b00 0000 7220 0000 00da  r....r....r ....
+00004240: 286c 6f61 645f 6964 735f 6f66 5f61 6c6c  (load_ids_of_all
+00004250: 5f65 7874 7261 6374 6564 5f61 7274 6963  _extracted_artic
+00004260: 6c65 735f 6c6f 6361 6c86 0200 0073 0600  les_local....s..
+00004270: 0000 1a01 0e01 0401 7205 0100 0063 0000  ........r....c..
+00004280: 0000 0000 0000 0000 0000 0b00 0000 0a00  ................
+00004290: 0000 4300 0000 73e0 0000 0074 006a 0174  ..C...s....t.j.t
+000042a0: 026a 0364 018d 017d 007c 00a0 0464 02a1  .j.d...}.|...d..
+000042b0: 017d 017c 01a0 0564 03a1 017d 027c 026a  .}.|...d...}.|.j
+000042c0: 0674 026a 0774 026a 0864 048d 027d 0367  .t.j.t.j.d...}.g
+000042d0: 007d 047a 2c7c 0344 005d 277d 057c 0564  .}.z,|.D.]'}.|.d
+000042e0: 0519 0044 005d 207d 067c 06a0 0964 06a1  ...D.] }.|...d..
+000042f0: 017d 077c 016a 0a74 026a 077c 0764 078d  .}.|.j.t.j.|.d..
+00004300: 027d 0874 0ba0 0c7c 0864 0819 00a0 0da1  .}.t...|.d......
+00004310: 00a0 0e64 09a1 01a1 017d 097c 04a0 0f7c  ...d.....}.|...|
+00004320: 09a1 0101 0071 2571 1f57 006e 1a04 0074  .....q%q.W.n...t
+00004330: 1079 6201 007d 0a01 007a 0e74 11a0 1264  .yb..}...z.t...d
+00004340: 0a7c 0a9b 009d 02a1 0101 0057 0059 0064  .|.........W.Y.d
+00004350: 007d 0a7e 0a6e 0564 007d 0a7e 0a77 0177  .}.~.n.d.}.~.w.w
+00004360: 0074 11a0 1364 0b74 147c 0483 019b 0064  .t...d.t.|.....d
+00004370: 0c9d 03a1 0101 007c 0453 0029 0d4e 727a  .......|.S.).Nrz
+00004380: 0000 0072 7f00 0000 72f4 0000 0072 f500  ...r....r....r..
+00004390: 0000 72f6 0000 0072 8200 0000 7280 0000  ..r....r....r...
+000043a0: 0072 8400 0000 7285 0000 007a 2845 7272  .r....r....z(Err
+000043b0: 6f72 2067 6574 7469 6e67 2061 6c6c 206b  or getting all k
+000043c0: 6e6f 776e 2069 6473 2066 726f 6d20 7333  nown ids from s3
+000043d0: 2c20 6e6f 207a 0e41 6c6c 204b 6e6f 776e  , no z.All Known
+000043e0: 2049 6473 2072 1600 0000 2915 728c 0000   Ids r....).r...
+000043f0: 0072 8d00 0000 7207 0000 0072 8e00 0000  .r....r....r....
+00004400: 7298 0000 0072 fa00 0000 72fb 0000 0072  r....r....r....r
+00004410: 9900 0000 7290 0000 0072 3f00 0000 729b  ....r....r?...r.
+00004420: 0000 0072 9600 0000 729c 0000 0072 9d00  ...r....r....r..
+00004430: 0000 729e 0000 0072 d100 0000 72a5 0000  ..r....r....r...
+00004440: 0072 4100 0000 72a6 0000 0072 9a00 0000  .rA...r....r....
+00004450: 724d 0000 0029 0b72 a700 0000 727f 0000  rM...).r....r...
+00004460: 0072 fe00 0000 72ff 0000 0072 d200 0000  .r....r....r....
+00004470: 7246 0000 0072 bd00 0000 72aa 0000 005a  rF...r....r....Z
+00004480: 0872 6573 706f 6e73 6572 a900 0000 7247  .responser....rG
+00004490: 0000 0072 1b00 0000 721b 0000 0072 2000  ...r....r....r .
+000044a0: 0000 da15 6c6f 6164 5f61 6c6c 5f6b 6e6f  ....load_all_kno
+000044b0: 776e 5f69 6473 5f73 338c 0200 0073 2800  wn_ids_s3....s(.
+000044c0: 0000 0e01 0a01 0a02 1201 0401 0201 0801  ................
+000044d0: 0c01 0a01 1001 1801 0c01 02fc 04ff 0e06  ................
+000044e0: 1c01 0880 02ff 1603 0401 7206 0100 0063  ..........r....c
+000044f0: 0000 0000 0000 0000 0000 0000 0900 0000  ................
+00004500: 0a00 0000 4300 0000 73c8 0000 0074 006a  ....C...s....t.j
+00004510: 0174 026a 0364 018d 017d 007c 00a0 0464  .t.j.d...}.|...d
+00004520: 02a1 017d 017c 01a0 0564 03a1 017d 0267  ...}.|...d...}.g
+00004530: 007d 037a 2a7c 026a 0674 026a 0774 026a  .}.z*|.j.t.j.t.j
+00004540: 0864 048d 0244 005d 1e7d 047c 0464 0519  .d...D.].}.|.d..
+00004550: 0044 005d 177d 057c 05a0 0964 06a1 017d  .D.].}.|...d...}
+00004560: 067c 06a0 0a64 07a1 0164 0819 007d 077c  .|...d...d...}.|
+00004570: 03a0 0b7c 07a0 0c64 0964 0aa1 02a1 0101  ...|...d.d......
+00004580: 0071 2371 1d57 006e 1a04 0074 0d79 5701  .q#q.W.n...t.yW.
+00004590: 007d 0801 007a 0e74 0ea0 0f64 0b7c 089b  .}...z.t...d.|..
+000045a0: 009d 02a1 0101 0057 0059 0064 007d 087e  .......W.Y.d.}.~
+000045b0: 086e 0564 007d 087e 0877 0177 0074 0ea0  .n.d.}.~.w.w.t..
+000045c0: 1064 0c74 117c 0383 019b 009d 02a1 0101  .d.t.|..........
+000045d0: 007c 0353 0029 0d4e 727a 0000 0072 7f00  .|.S.).Nrz...r..
+000045e0: 0000 72f4 0000 0072 f500 0000 72f6 0000  ..r....r....r...
+000045f0: 0072 8200 0000 7218 0000 0072 b900 0000  .r....r....r....
+00004600: 727e 0000 0072 3200 0000 7a33 4572 726f  r~...r2...z3Erro
+00004610: 7220 6c6f 6164 696e 6720 6964 7320 6f66  r loading ids of
+00004620: 2065 7874 7261 6374 6564 2061 7274 6963   extracted artic
+00004630: 6c65 2066 726f 6d20 7333 2c20 6e6f 207a  le from s3, no z
+00004640: 0e45 7874 7261 6374 6564 2049 6473 2029  .Extracted Ids )
+00004650: 1272 8c00 0000 728d 0000 0072 0700 0000  .r....r....r....
+00004660: 728e 0000 0072 9800 0000 72fa 0000 0072  r....r....r....r
+00004670: fb00 0000 7299 0000 0072 0401 0000 723f  ....r....r....r?
+00004680: 0000 0072 fc00 0000 7255 0000 0072 2a00  ...r....rU...r*.
+00004690: 0000 72a5 0000 0072 4100 0000 72a6 0000  ..r....rA...r...
+000046a0: 0072 9a00 0000 724d 0000 0029 0972 a700  .r....rM...).r..
+000046b0: 0000 727f 0000 0072 fe00 0000 5a11 616c  ..r....r....Z.al
+000046c0: 6c5f 6964 735f 6578 7472 6163 7465 6472  l_ids_extractedr
+000046d0: 4600 0000 72bd 0000 0072 aa00 0000 7200  F...r....r....r.
+000046e0: 0100 0072 4700 0000 721b 0000 0072 1b00  ...rG...r....r..
+000046f0: 0000 7220 0000 00da 256c 6f61 645f 6964  ..r ....%load_id
+00004700: 735f 6f66 5f61 6c6c 5f65 7874 7261 6374  s_of_all_extract
+00004710: 6564 5f61 7274 6963 6c65 735f 7333 a102  ed_articles_s3..
+00004720: 0000 7324 0000 000e 010a 010a 0204 0102  ..s$............
+00004730: 0116 010c 010a 010e 0114 0102 fd04 ff0e  ................
+00004740: 051c 0108 8002 ff14 0304 0172 0701 0000  ...........r....
+00004750: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00004760: 0009 0000 0043 0000 0073 9600 0000 7c00  .....C...s....|.
+00004770: 6400 7500 7207 7400 6a01 7d00 7c00 6401  d.u.r.t.j.}.|.d.
+00004780: 6b02 7212 7402 8300 7d01 7403 8300 7d02  k.r.t...}.t...}.
+00004790: 6e13 7c00 6402 6b02 721d 7404 8300 7d01  n.|.d.k.r.t...}.
+000047a0: 7405 8300 7d02 6e08 7406 6403 7c00 9b00  t...}.n.t.d.|...
+000047b0: 6404 9d03 8301 8201 7407 7c01 8301 7d01  d.......t.|...}.
+000047c0: 7407 7c02 8301 7d02 7408 7c01 a009 7c02  t.|...}.t.|...|.
+000047d0: a101 8301 7d03 740a a00b 6405 740c 7c03  ....}.t...d.t.|.
+000047e0: 8301 9b00 6406 740c 7c01 8301 9b00 6407  ....d.t.|.....d.
+000047f0: 740c 7c02 8301 9b00 6408 9d07 a101 0100  t.|.....d.......
+00004800: 7c03 5300 2909 4e72 7700 0000 727f 0000  |.S.).Nrw...r...
+00004810: 0072 f700 0000 72f8 0000 007a 0666 6f75  .r....r....z.fou
+00004820: 6e64 207a 1620 4944 7320 6c65 6674 2074  nd z. IDs left t
+00004830: 6f20 6578 7472 6163 7420 287a 0820 6b6e  o extract (z. kn
+00004840: 6f77 6e2c 207a 0b20 6578 7472 6163 7465  own, z. extracte
+00004850: 6429 290d 7207 0000 0072 c900 0000 7203  d)).r....r....r.
+00004860: 0100 0072 0501 0000 7206 0100 0072 0701  ...r....r....r..
+00004870: 0000 7265 0000 0072 a100 0000 723c 0000  ..re...r....r<..
+00004880: 00da 0a64 6966 6665 7265 6e63 6572 4100  ...differencerA.
+00004890: 0000 7242 0000 0072 4d00 0000 2904 72ec  ..rB...rM...).r.
+000048a0: 0000 005a 0969 6473 5f6b 6e6f 776e 5a0d  ...Z.ids_knownZ.
+000048b0: 6964 735f 6578 7472 6163 7465 645a 1369  ids_extractedZ.i
+000048c0: 6473 5f6c 6566 745f 746f 5f65 7874 7261  ds_left_to_extra
+000048d0: 6374 721b 0000 0072 1b00 0000 7220 0000  ctr....r....r ..
+000048e0: 00da 1866 696e 645f 6964 735f 6c65 6674  ...find_ids_left
+000048f0: 5f74 6f5f 6578 7472 6163 74b4 0200 0073  _to_extract....s
+00004900: 2400 0000 0801 0601 0802 0601 0801 0801  $...............
+00004910: 0601 0801 1002 0802 0801 0e01 1001 0601  ................
+00004920: 04ff 0601 0aff 0403 7209 0100 0063 0200  ........r....c..
+00004930: 0000 0000 0000 0000 0000 0400 0000 0800  ................
+00004940: 0000 4300 0000 7366 0000 0074 006a 019b  ..C...sf...t.j..
+00004950: 0064 0174 006a 029b 009d 037d 0274 036a  .d.t.j.....}.t.j
+00004960: 047c 0264 0264 038d 0201 0074 057c 029b  .|.d.d.....t.|..
+00004970: 0064 017c 019b 0064 049d 0464 0583 028f  .d.|...d...d....
+00004980: 0e7d 037c 03a0 067c 00a1 0101 0057 0064  .}.|...|.....W.d
+00004990: 0004 0004 0083 0301 0064 0053 0031 0073  .........d.S.1.s
+000049a0: 2c77 0101 0001 0001 0059 0001 0064 0053  ,w.......Y...d.S
+000049b0: 0029 064e 7218 0000 0054 727c 0000 0072  .).Nr....Tr|...r
+000049c0: 7e00 0000 7287 0000 0029 0772 0700 0000  ~...r....).r....
+000049d0: 728f 0000 0072 0401 0000 7291 0000 0072  r....r....r....r
+000049e0: 9200 0000 7295 0000 00da 0577 7269 7465  ....r......write
+000049f0: 2904 72db 0000 00da 0a69 645f 6172 7469  ).r......id_arti
+00004a00: 636c 655a 0964 6972 5f6c 6f63 616c 72a8  cleZ.dir_localr.
+00004a10: 0000 0072 1b00 0000 721b 0000 0072 2000  ...r....r....r .
+00004a20: 0000 da16 7361 7665 5f6a 736f 6e5f 7478  ....save_json_tx
+00004a30: 745f 746f 5f6c 6f63 616c ca02 0000 730a  t_to_local....s.
+00004a40: 0000 0012 010e 0118 020c 0122 ff72 0c01  ...........".r..
+00004a50: 0000 6302 0000 0000 0000 0000 0000 0007  ..c.............
+00004a60: 0000 000a 0000 0043 0000 0073 8400 0000  .......C...s....
+00004a70: 7400 6a01 7402 6a03 6401 8d01 7d02 7c02  t.j.t.j.d...}.|.
+00004a80: a004 6402 a101 7d03 7405 a006 7c00 a101  ..d...}.t...|...
+00004a90: 7d04 7402 6a07 9b00 6403 7c01 9b00 6404  }.t.j...d.|...d.
+00004aa0: 9d04 7d05 7a0c 7c03 6a08 7402 6a09 7c05  ..}.z.|.j.t.j.|.
+00004ab0: 7c04 6405 8d03 0100 5700 6400 5300 0400  |.d.....W.d.S...
+00004ac0: 740a 7941 0100 7d06 0100 7a0f 740b a00c  t.yA..}...z.t...
+00004ad0: 6406 7c06 9b00 9d02 a101 0100 5700 5900  d.|.........W.Y.
+00004ae0: 6400 7d06 7e06 6400 5300 6400 7d06 7e06  d.}.~.d.S.d.}.~.
+00004af0: 7701 7700 2907 4e72 7a00 0000 727f 0000  w.w.).Nrz...r...
+00004b00: 0072 1800 0000 727e 0000 0072 8a00 0000  .r....r~...r....
+00004b10: 728b 0000 0029 0d72 8c00 0000 728d 0000  r....).r....r...
+00004b20: 0072 0700 0000 728e 0000 0072 9800 0000  .r....r....r....
+00004b30: 7296 0000 0072 a300 0000 7204 0100 0072  r....r....r....r
+00004b40: a400 0000 7299 0000 0072 a500 0000 7241  ....r....r....rA
+00004b50: 0000 0072 a600 0000 2907 72db 0000 0072  ...r....).r....r
+00004b60: 0b01 0000 72a7 0000 0072 7f00 0000 72ab  ....r....r....r.
+00004b70: 0000 0072 aa00 0000 7247 0000 0072 1b00  ...r....rG...r..
+00004b80: 0000 721b 0000 0072 2000 0000 da13 7361  ..r....r .....sa
+00004b90: 7665 5f6a 736f 6e5f 7478 745f 746f 5f73  ve_json_txt_to_s
+00004ba0: 33d2 0200 0073 1400 0000 0e01 0a01 0a01  3....s..........
+00004bb0: 1201 0201 1801 0e01 1e01 0880 02ff 720d  ..............r.
+00004bc0: 0100 0063 0300 0000 0000 0000 0000 0000  ...c............
+00004bd0: 0300 0000 0400 0000 4300 0000 7334 0000  ........C...s4..
+00004be0: 007c 0264 016b 0272 0974 007c 007c 0183  .|.d.k.r.t.|.|..
+00004bf0: 0253 007c 0264 026b 0272 1274 017c 007c  .S.|.d.k.r.t.|.|
+00004c00: 0183 0253 0074 0264 037c 029b 0064 049d  ...S.t.d.|...d..
+00004c10: 0383 0182 0129 054e 7277 0000 0072 7f00  .....).Nrw...r..
+00004c20: 0000 72f7 0000 0072 f800 0000 2903 720c  ..r....r....).r.
+00004c30: 0100 0072 0d01 0000 7265 0000 00a9 0372  ...r....re.....r
+00004c40: db00 0000 720b 0100 0072 ec00 0000 721b  ....r....r....r.
+00004c50: 0000 0072 1b00 0000 7220 0000 00da 0d73  ...r....r .....s
+00004c60: 6176 655f 6a73 6f6e 5f74 7874 df02 0000  ave_json_txt....
+00004c70: 730a 0000 0008 010a 0108 010a 0110 0272  s..............r
+00004c80: 0f01 0000 7237 0000 00da 0a63 6875 6e6b  ....r7.....chunk
+00004c90: 5f73 697a 6563 0200 0000 0000 0000 0000  _sizec..........
+00004ca0: 0000 0c00 0000 0800 0000 4300 0000 732c  ..........C...s,
+00004cb0: 0100 0074 00a0 0164 01a1 0101 007c 0064  ...t...d.....|.d
+00004cc0: 0075 0072 0c74 026a 037d 0074 047c 0083  .u.r.t.j.}.t.|..
+00004cd0: 017d 0264 027d 0364 027d 0474 057c 0283  .}.d.}.d.}.t.|..
+00004ce0: 017d 0574 067c 0564 0364 0464 0564 068d  .}.t.|.d.d.d.d..
+00004cf0: 047d 0674 057c 0283 0164 026b 0472 877c  .}.t.|...d.k.r.|
+00004d00: 0264 007c 0185 0219 007c 027c 0164 0085  .d.|.....|.|.d..
+00004d10: 0219 0002 027d 077d 0274 077c 0783 017d  .....}.}.t.|...}
+00004d20: 087c 0374 057c 0783 0137 007d 037c 08a0  .|.t.|...7.}.|..
+00004d30: 08a1 0044 005d 235c 027d 097d 0a7a 0674  ...D.]#\.}.}.z.t
+00004d40: 097c 0a83 017d 0b57 006e 0d01 0001 0001  .|...}.W.n......
+00004d50: 0074 00a0 0a64 077c 099b 009d 02a1 0101  .t...d.|........
+00004d60: 0059 0071 4174 0b7c 0b7c 097c 0064 088d  .Y.qAt.|.|.|.d..
+00004d70: 0301 007c 0464 0937 007d 0471 4174 00a0  ...|.d.7.}.qAt..
+00004d80: 0c7c 037c 051b 0064 0514 0064 0a9b 0464  .|.|...d...d...d
+00004d90: 0b7c 047c 031b 0064 0514 0064 0a9b 0464  .|.|...d...d...d
+00004da0: 0c9d 04a1 0101 007c 06a0 0d74 057c 0783  .......|...t.|..
+00004db0: 01a1 0101 0074 057c 0283 0164 026b 0473  .....t.|...d.k.s
+00004dc0: 267c 06a0 0ea1 0001 007c 06a0 0fa1 0001  &|.......|......
+00004dd0: 0074 00a0 0164 0da1 0101 0064 0053 0029  .t...d.....d.S.)
+00004de0: 0e4e 7a36 6d61 696e 5f65 7874 7261 6374  .Nz6main_extract
+00004df0: 5f6a 736f 6e5f 7478 745f 666f 725f 616c  _json_txt_for_al
+00004e00: 6c5f 6b6e 6f77 6e5f 6964 7328 293a 2053  l_known_ids(): S
+00004e10: 7461 7274 696e 672e 2e2e 7201 0000 005a  tarting...r....Z
+00004e20: 0249 44e9 1e00 0000 7257 0000 0029 04da  .ID.....rW...)..
+00004e30: 0574 6f74 616c 5a04 756e 6974 5a0b 6d69  .totalZ.unitZ.mi
+00004e40: 6e69 6e74 6572 7661 6c5a 086d 696e 6974  nintervalZ.minit
+00004e50: 6572 737a 4246 6169 6c65 6420 746f 2067  erszBFailed to g
+00004e60: 6574 206a 736f 6e20 7478 7420 6672 6f6d  et json txt from
+00004e70: 2042 6561 7574 6966 756c 536f 7570 206f   BeautifulSoup o
+00004e80: 626a 206f 6620 6172 7469 636c 6520 7769  bj of article wi
+00004e90: 7468 2049 443a 2072 0e01 0000 725d 0000  th ID: r....r]..
+00004ea0: 0072 5e00 0000 7a22 2520 6f66 2049 4473  .r^...z"% of IDs
+00004eb0: 2061 7474 656d 7074 6564 2c20 7375 6363   attempted, succ
+00004ec0: 6573 7320 7261 7465 3a20 fa01 257a 306d  ess rate: ..%z0m
+00004ed0: 6169 6e5f 6578 7472 6163 745f 6a73 6f6e  ain_extract_json
+00004ee0: 5f74 7874 5f66 6f72 5f61 6c6c 5f6b 6e6f  _txt_for_all_kno
+00004ef0: 776e 5f69 6473 2829 3a20 446f 6e65 2e29  wn_ids(): Done.)
+00004f00: 1072 4100 0000 729a 0000 0072 0700 0000  .rA...r....r....
+00004f10: 72c9 0000 0072 0901 0000 724d 0000 0072  r....r....rM...r
+00004f20: 0600 0000 72d8 0000 0072 2c00 0000 72dc  ....r....r,...r.
+00004f30: 0000 0072 a600 0000 720f 0100 0072 4200  ...r....r....rB.
+00004f40: 0000 722b 0000 005a 0764 6973 706c 6179  ..r+...Z.display
+00004f50: da05 636c 6f73 6529 0c72 ec00 0000 7210  ..close).r....r.
+00004f60: 0100 0072 a900 0000 5a0b 6e5f 6174 7465  ...r....Z.n_atte
+00004f70: 6d70 7465 645a 0b6e 5f65 7874 7261 6374  mptedZ.n_extract
+00004f80: 6564 5a0a 6e5f 696e 6974 5f69 6473 5a02  edZ.n_init_idsZ.
+00004f90: 7062 5a08 6964 735f 7061 7274 7267 0000  pbZ.ids_partrg..
+00004fa0: 0072 0b01 0000 5a0f 636f 6e74 656e 745f  .r....Z.content_
+00004fb0: 6172 7469 636c 6572 db00 0000 721b 0000  articler....r...
+00004fc0: 0072 1b00 0000 7220 0000 00da 276d 6169  .r....r ....'mai
+00004fd0: 6e5f 6578 7472 6163 745f 6a73 6f6e 5f74  n_extract_json_t
+00004fe0: 7874 5f66 6f72 5f61 6c6c 5f6b 6e6f 776e  xt_for_all_known
+00004ff0: 5f69 6473 e802 0000 7338 0000 000a 0108  _ids....s8......
+00005000: 0206 0108 0204 0104 0108 0110 010c 021a  ................
+00005010: 0108 010c 0110 0202 010c 0106 0110 0104  ................
+00005020: 010e 020a 0114 020c 010a ff0e 020c ef08  ................
+00005030: 1308 010e 0172 1501 0000 2902 4e72 3100  .....r....).Nr1.
+00005040: 0000 2903 5454 7231 0000 0029 0572 5700  ..).TTr1...).rW.
+00005050: 0000 544e 7231 0000 0072 3100 0000 721a  ..TNr1...r1...r.
+00005060: 0000 0029 024e 7277 0000 0029 0372 b600  ...).Nrw...).r..
+00005070: 0000 5472 3100 0000 2901 7277 0000 0029  ..Tr1...).rw...)
+00005080: 024e 7237 0000 0029 4672 e800 0000 5a07  .Nr7...)Fr....Z.
+00005090: 6f73 2e70 6174 6872 9100 0000 723e 0000  os.pathr....r>..
+000050a0: 005a 0362 7334 7202 0000 0072 9600 0000  .Z.bs4r....r....
+000050b0: 725f 0000 00da 0674 7970 696e 6772 0300  r_.....typingr..
+000050c0: 0000 7204 0000 0072 0500 0000 da07 6c6f  ..r....r......lo
+000050d0: 6767 696e 6772 4a00 0000 728c 0000 0072  ggingrJ...r....r
+000050e0: bf00 0000 5a12 636f 6e63 7572 7265 6e74  ....Z.concurrent
+000050f0: 2e66 7574 7572 6573 7261 0000 0072 f900  .futuresra...r..
+00005100: 0000 7206 0000 00da 1573 6372 6170 6175  ..r......scrapau
+00005110: 746f 7363 6f75 742e 636f 6e66 6967 7207  toscout.configr.
+00005120: 0000 005a 1673 6372 6170 6175 746f 7363  ...Z.scrapautosc
+00005130: 6f75 742e 7072 6f78 6965 7372 0800 0000  out.proxiesr....
+00005140: 5a14 7363 7261 7061 7574 6f73 636f 7574  Z.scrapautoscout
+00005150: 2e75 7469 6c73 7209 0000 0072 0a00 0000  .utilsr....r....
+00005160: 720b 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00005170: 0967 6574 4c6f 6767 6572 7293 0000 0072  .getLoggerr....r
+00005180: f100 0000 da08 5f5f 6669 6c65 5f5f 7241  ......__file__rA
+00005190: 0000 0072 4e00 0000 da08 5349 5445 5f55  ...rN.....SITE_U
+000051a0: 524c da03 7374 7272 bb00 0000 7230 0000  RL..strr....r0..
+000051b0: 0072 4800 0000 7253 0000 0072 5600 0000  .rH...rS...rV...
+000051c0: da04 626f 6f6c 726a 0000 00da 094d 4158  ..boolrj.....MAX
+000051d0: 5f50 4147 4553 7270 0000 0072 7600 0000  _PAGESrp...rv...
+000051e0: 72ac 0000 0072 b500 0000 729f 0000 00da  r....r....r.....
+000051f0: 144d 4158 5f52 4553 554c 5453 5f50 4552  .MAX_RESULTS_PER
+00005200: 5f50 4147 4572 a000 0000 da0b 4d41 585f  _PAGEr......MAX_
+00005210: 5245 5355 4c54 5372 d400 0000 72d5 0000  RESULTSr....r...
+00005220: 0072 d800 0000 72dc 0000 0072 e700 0000  .r....r....r....
+00005230: 72da 0000 0072 ce00 0000 7203 0100 0072  r....r....r....r
+00005240: 0501 0000 7206 0100 0072 0701 0000 7209  ....r....r....r.
+00005250: 0100 0072 0c01 0000 720d 0100 0072 0f01  ...r....r....r..
+00005260: 0000 7215 0100 0072 1b00 0000 721b 0000  ..r....r....r...
+00005270: 0072 1b00 0000 7220 0000 00da 083c 6d6f  .r....r .....<mo
+00005280: 6475 6c65 3e01 0000 0073 6201 0000 0800  dule>....sb.....
+00005290: 0801 0801 0c01 0801 0801 1401 0801 0801  ................
+000052a0: 0801 0801 0801 0801 0c01 0c03 0c01 1c01  ................
+000052b0: 1203 0402 0404 0201 0201 0201 0201 0201  ................
+000052c0: 0201 04f9 0201 02ff 0202 02fe 0203 02fd  ................
+000052d0: 0204 02fc 0205 02fb 0206 02fa 0207 02f9  ................
+000052e0: 0209 0af7 0a2f 100e 1c13 020c 0201 0201  ...../..........
+000052f0: 0201 0201 04fa 0601 02ff 0202 02fe 0203  ................
+00005300: 02fd 0204 02fc 0205 02fb 0206 02fa 0a07  ................
+00005310: 0af9 0455 0201 0201 0201 04fb 0201 02ff  ...U............
+00005320: 0202 02fe 0203 02fd 0204 02fc 0205 02fb  ................
+00005330: 0606 0afa 201b 0215 0201 04fd 0201 02ff  .... ...........
+00005340: 0202 02fe 0203 0afd 0440 0201 0201 04fc  .........@......
+00005350: 0201 02ff 0202 02fe 0203 02fd 0204 0afc  ................
+00005360: 1419 0429 0401 04fd 0201 02ff 0202 02fe  ...)............
+00005370: 0203 02fd 0204 0afc 0209 0201 0201 0201  ................
+00005380: 0401 0201 0201 0201 0201 04f7 0601 02ff  ................
+00005390: 0a02 02fe 0a03 02fd 0204 02fc 0205 02fb  ................
+000053a0: 0206 02fa 0207 02f9 0208 02f8 0209 0af7  ................
+000053b0: 007f 1417 0406 0201 0201 0201 04fb 0601  ................
+000053c0: 02ff 0202 02fe 0203 02fd 0204 02fc 0205  ................
+000053d0: 02fb 0a06 0afa 1223 0e07 0e09 1018 1219  .......#........
+000053e0: 120c 0806 0815 1013 0816 0808 100d 1809  ................
```

### Comparing `scrapautoscout-1.2.0/scrapautoscout/__pycache__/transform.cpython-310.pyc` & `scrapautoscout-1.3.0/scrapautoscout/__pycache__/transform.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/__pycache__/utils.cpython-310.pyc` & `scrapautoscout-1.3.0/scrapautoscout/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/config.py` & `scrapautoscout-1.3.0/scrapautoscout/config.py`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/pipeline.py` & `scrapautoscout-1.3.0/scrapautoscout/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     # nohup python3 -m scrapautoscout.pipeline >/dev/null 2>&1
     """
 
     parser = argparse.ArgumentParser(
         prog='Scrapper autoscout24',
         description='Full pipeline to extract articles from autoscout24'
     )
+    parser.add_argument('--ADAGE', help="Age of listings")
     parser.add_argument('--LOCATION', help="'local' or 's3'")
     parser.add_argument('--DIR_CACHE', help="Where to save artifacts. Default: 'cache' (relative to project root)")
     parser.add_argument('--AWS_PROFILE_NAME', help='AWS profile name')
     parser.add_argument('--AWS_S3_BUCKET', help='AWS S3 bucket')
     parser.add_argument('--MAKERS', nargs='+', help='List of makers delimited by space')
     parser.add_argument('--LOGS_LEVEL', help="Log level, e.g. 'debug', 'info', 'error'")
     args = parser.parse_args()
```

### Comparing `scrapautoscout-1.2.0/scrapautoscout/proxies.py` & `scrapautoscout-1.3.0/scrapautoscout/proxies.py`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/scrapper.py` & `scrapautoscout-1.3.0/scrapautoscout/scrapper.py`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/transform.py` & `scrapautoscout-1.3.0/scrapautoscout/transform.py`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout/utils.py` & `scrapautoscout-1.3.0/scrapautoscout/utils.py`

 * *Files identical despite different names*

### Comparing `scrapautoscout-1.2.0/scrapautoscout.egg-info/PKG-INFO` & `scrapautoscout-1.3.0/scrapautoscout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: scrapautoscout
-Version: 1.2.0
+Version: 1.3.0
 Summary: autoscout24 web scrapper
 Home-page: https://github.com/viggleUnik/scrapautoscout
 Author: Vicol Cristian
 Author-email: vicol.cristianken@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
@@ -51,9 +50,7 @@
  + --LOGS_LEVEL LOGS_LEVEL - Log level, e.g. 'debug', 'info', 'error'
 
 **After this you can run it with specified parameters, example:**
 
 ```shell
 scrapautoscout --LOCATION 's3' 
 ```
-
-
```

### Comparing `scrapautoscout-1.2.0/setup.py` & `scrapautoscout-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from io import open
 
-VERSION = '1.2.0'
+VERSION = '1.3.0'
 DESCRIPTION = 'autoscout24 web scrapper'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapautoscout",
@@ -13,15 +13,15 @@
     author='Vicol Cristian',
     author_email='vicol.cristianken@gmail.com',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/viggleUnik/scrapautoscout',
     license='MIT',
-    packages=['scrapautoscout'],
+    packages=['scrapautoscout', 'db'],
     install_requires=[
         'requests==2.28.2',
         'beautifulsoup4==4.11.1',
         'psycopg2-binary==2.9.5',
         'boto3==1.26.86',
         's3fs',
         'tqdm',
```

