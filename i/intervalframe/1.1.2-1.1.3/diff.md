# Comparing `tmp/intervalframe-1.1.2.tar.gz` & `tmp/intervalframe-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intervalframe-1.1.2.tar", max compression
+gzip compressed data, was "intervalframe-1.1.3.tar", max compression
```

## Comparing `intervalframe-1.1.2.tar` & `intervalframe-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 intervalframe-1.1.2/LICENSE.md
--rwxr-xr-x   0        0        0     1017 2022-01-03 18:58:56.000000 intervalframe-1.1.2/README.md
--rw-r--r--   0        0        0     6148 2023-05-08 14:50:48.246993 intervalframe-1.1.2/intervalframe/.DS_Store
--rw-r--r--   0        0        0      444 2023-05-08 14:58:49.487881 intervalframe-1.1.2/intervalframe/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-02 16:32:30.612368 intervalframe-1.1.2/intervalframe/core/.DS_Store
--rw-r--r--   0        0        0    36691 2023-05-08 14:56:39.086479 intervalframe-1.1.2/intervalframe/core/IntervalFrame.py
--rw-r--r--   0        0        0    18564 2023-05-08 14:58:21.201049 intervalframe-1.1.2/intervalframe/core/IntervalSeries.py
--rw-r--r--   0        0        0     1244 2020-06-30 16:23:05.000000 intervalframe-1.1.2/intervalframe/core/groupby.py
--rw-r--r--   0        0        0     4299 2022-01-10 22:35:34.000000 intervalframe-1.1.2/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc
--rw-r--r--   0        0        0     6980 2023-02-02 17:51:34.367876 intervalframe-1.1.2/intervalframe/core/index/indexers.py
--rw-r--r--   0        0        0     2473 2021-09-21 15:04:53.000000 intervalframe-1.1.2/intervalframe/read/__pycache__/read_h5.cpython-39.pyc
--rw-r--r--   0        0        0     1191 2022-01-10 22:35:34.000000 intervalframe-1.1.2/intervalframe/read/__pycache__/read_text.cpython-39.pyc
--rw-r--r--   0        0        0    20974 2021-02-11 01:01:08.000000 intervalframe-1.1.2/intervalframe/read/h5_utilities.py
--rw-r--r--   0        0        0     6848 2023-03-25 17:26:19.423023 intervalframe-1.1.2/intervalframe/read/read_h5.py
--rw-r--r--   0        0        0      815 2023-01-26 17:56:39.789523 intervalframe-1.1.2/intervalframe/read/read_parquet.py
--rw-r--r--   0        0        0     2453 2023-01-26 20:00:28.520286 intervalframe-1.1.2/intervalframe/read/read_text.py
--rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.2/intervalframe/utilities/h5_utilities.py
--rw-r--r--   0        0        0     2856 2021-09-21 15:04:53.000000 intervalframe-1.1.2/intervalframe/write/__pycache__/write_h5.cpython-39.pyc
--rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.2/intervalframe/write/h5_utilities.py
--rw-r--r--   0        0        0     7192 2023-03-25 13:52:13.113838 intervalframe-1.1.2/intervalframe/write/write_h5.py
--rw-r--r--   0        0        0      736 2023-01-30 21:43:29.435395 intervalframe-1.1.2/intervalframe/write/write_parquet.py
--rw-r--r--   0        0        0        0 2020-07-22 20:58:51.000000 intervalframe-1.1.2/intervalframe/write/write_text.py
--rw-r--r--   0        0        0     2008 2023-05-08 14:58:59.689426 intervalframe-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 intervalframe-1.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 intervalframe-1.1.3/LICENSE.md
+-rwxr-xr-x   0        0        0     1017 2022-01-03 18:58:56.000000 intervalframe-1.1.3/README.md
+-rw-r--r--   0        0        0     6148 2023-05-12 20:29:56.068870 intervalframe-1.1.3/intervalframe/.DS_Store
+-rw-r--r--   0        0        0      444 2023-05-17 13:18:57.473103 intervalframe-1.1.3/intervalframe/__init__.py
+-rw-r--r--   0        0        0     6148 2023-05-08 15:06:34.044574 intervalframe-1.1.3/intervalframe/core/.DS_Store
+-rw-r--r--   0        0        0    37043 2023-05-12 20:34:03.525928 intervalframe-1.1.3/intervalframe/core/IntervalFrame.py
+-rw-r--r--   0        0        0    18564 2023-05-08 14:58:21.201049 intervalframe-1.1.3/intervalframe/core/IntervalSeries.py
+-rw-r--r--   0        0        0     1244 2020-06-30 16:23:05.000000 intervalframe-1.1.3/intervalframe/core/groupby.py
+-rw-r--r--   0        0        0     4299 2022-01-10 22:35:34.000000 intervalframe-1.1.3/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc
+-rw-r--r--   0        0        0     6980 2023-02-02 17:51:34.367876 intervalframe-1.1.3/intervalframe/core/index/indexers.py
+-rw-r--r--   0        0        0     2473 2021-09-21 15:04:53.000000 intervalframe-1.1.3/intervalframe/read/__pycache__/read_h5.cpython-39.pyc
+-rw-r--r--   0        0        0     1191 2022-01-10 22:35:34.000000 intervalframe-1.1.3/intervalframe/read/__pycache__/read_text.cpython-39.pyc
+-rw-r--r--   0        0        0    20974 2021-02-11 01:01:08.000000 intervalframe-1.1.3/intervalframe/read/h5_utilities.py
+-rw-r--r--   0        0        0     6848 2023-03-25 17:26:19.423023 intervalframe-1.1.3/intervalframe/read/read_h5.py
+-rw-r--r--   0        0        0      815 2023-01-26 17:56:39.789523 intervalframe-1.1.3/intervalframe/read/read_parquet.py
+-rw-r--r--   0        0        0     2453 2023-01-26 20:00:28.520286 intervalframe-1.1.3/intervalframe/read/read_text.py
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.3/intervalframe/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2856 2021-09-21 15:04:53.000000 intervalframe-1.1.3/intervalframe/write/__pycache__/write_h5.cpython-39.pyc
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.3/intervalframe/write/h5_utilities.py
+-rw-r--r--   0        0        0     7192 2023-03-25 13:52:13.113838 intervalframe-1.1.3/intervalframe/write/write_h5.py
+-rw-r--r--   0        0        0      736 2023-01-30 21:43:29.435395 intervalframe-1.1.3/intervalframe/write/write_parquet.py
+-rw-r--r--   0        0        0        0 2020-07-22 20:58:51.000000 intervalframe-1.1.3/intervalframe/write/write_text.py
+-rw-r--r--   0        0        0     2066 2023-05-17 13:19:08.765570 intervalframe-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 intervalframe-1.1.3/PKG-INFO
```

### Comparing `intervalframe-1.1.2/LICENSE.md` & `intervalframe-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/README.md` & `intervalframe-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/.DS_Store` & `intervalframe-1.1.3/intervalframe/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 00000420: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
 00000430: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 00000440: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 00000450: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00000460: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00000470: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00000480: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00000490: 0908 095f 1018 7b7b 3434 332c 2033 3938  ..._..{{443, 398
+00000490: 0908 095f 1018 7b7b 3338 352c 2034 3233  ..._..{{385, 423
 000004a0: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
 000004b0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
 000004c0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
 000004d0: 0000 0000 0000 0000 0000 008b 0000 0004  ................
 000004e0: 0063 006f 0072 0065 7653 726e 6c6f 6e67  .c.o.r.evSrnlong
 000004f0: 0000 0001 0000 0004 0072 0065 0061 0064  .........r.e.a.d
 00000500: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
```

### Comparing `intervalframe-1.1.2/intervalframe/core/.DS_Store` & `intervalframe-1.1.3/intervalframe/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/core/IntervalFrame.py` & `intervalframe-1.1.3/intervalframe/core/IntervalFrame.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,16 +655,28 @@
 
         return nhits_iframe
 
 
     def iter_intersect(self,
                        iframe):
         """
+        Iterate over intersections
+
+        Parameters
+        ----------
+            iframe : IntervalFrame
+                Intervals to intersect with
+        
+        Returns
+        -------
+            intersected_iframe : Generator[IntervalFrame]
+                Generator of intervals that intersect
         """
 
+        # Iterate over intersecting intervals
         for index in iframe.index.iter_intersect(self.index, return_intervals=False, return_index=True):
             if len(index) > 0:
                 new_iframe = iframe.iloc[index,:]
             else:
                 new_iframe = IntervalFrame(columns=[iframe.columns])
             
             yield new_iframe
```

### Comparing `intervalframe-1.1.2/intervalframe/core/IntervalSeries.py` & `intervalframe-1.1.3/intervalframe/core/IntervalSeries.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/core/groupby.py` & `intervalframe-1.1.3/intervalframe/core/groupby.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc` & `intervalframe-1.1.3/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/core/index/indexers.py` & `intervalframe-1.1.3/intervalframe/core/index/indexers.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/read/__pycache__/read_h5.cpython-39.pyc` & `intervalframe-1.1.3/intervalframe/read/__pycache__/read_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/read/__pycache__/read_text.cpython-39.pyc` & `intervalframe-1.1.3/intervalframe/read/__pycache__/read_text.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/read/h5_utilities.py` & `intervalframe-1.1.3/intervalframe/read/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/read/read_h5.py` & `intervalframe-1.1.3/intervalframe/read/read_h5.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/read/read_parquet.py` & `intervalframe-1.1.3/intervalframe/read/read_parquet.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/read/read_text.py` & `intervalframe-1.1.3/intervalframe/read/read_text.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/utilities/h5_utilities.py` & `intervalframe-1.1.3/intervalframe/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/write/__pycache__/write_h5.cpython-39.pyc` & `intervalframe-1.1.3/intervalframe/write/__pycache__/write_h5.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/write/h5_utilities.py` & `intervalframe-1.1.3/intervalframe/write/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/write/write_h5.py` & `intervalframe-1.1.3/intervalframe/write/write_h5.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/intervalframe/write/write_parquet.py` & `intervalframe-1.1.3/intervalframe/write/write_parquet.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.1.2/pyproject.toml` & `intervalframe-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "intervalframe"
-version = "1.1.2"
+version = "1.1.3"
 description = "Python package for interval manipulation"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/intervalframe"
 documentation = "https://www.biosciencestack.com/static/intervalframe/docs/index.html"
 keywords = ["cython", "interval", "ailist", "frame"]
 readme = 'README.md'
@@ -31,14 +31,17 @@
 numpy = "^1.23.5"
 cython = "^0.29.32"
 pandas = "^1.5.2"
 ailist = "^2.1.0"
 tabulate = "^0.9.0"
 linear_segment = "^1.0.0"
 h5py = "^3.8.0"
+scipy = "^1.9.1"
+requests = "^2.28.2"
+pyarrow = "^11.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
             "cython>=0.29.32",
```

### Comparing `intervalframe-1.1.2/PKG-INFO` & `intervalframe-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intervalframe
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python package for interval manipulation
 Home-page: https://github.com/kylessmith/intervalframe
 License: GPL-2.0-or-later
 Keywords: cython,interval,ailist,frame
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -30,14 +30,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ailist (>=2.1.0,<3.0.0)
 Requires-Dist: cython (>=0.29.32,<0.30.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: linear_segment (>=1.0.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/intervalframe/docs/index.html
 Project-URL: Repository, https://github.com/kylessmith/intervalframe
 Description-Content-Type: text/markdown
 
 # IntervalFrame for interval manipulation
```

