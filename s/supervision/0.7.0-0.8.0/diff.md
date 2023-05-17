# Comparing `tmp/supervision-0.7.0.tar.gz` & `tmp/supervision-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervision-0.7.0.tar", last modified: Wed May 10 22:44:27 2023, max compression
+gzip compressed data, was "supervision-0.8.0.tar", last modified: Wed May 17 19:36:51 2023, max compression
```

## Comparing `supervision-0.7.0.tar` & `supervision-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.936566 supervision-0.7.0/
--rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.7.0/LICENSE.md
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-05-10 22:44:27.936430 supervision-0.7.0/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.7.0/README.md
--rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-05-10 22:44:27.936620 supervision-0.7.0/setup.cfg
--rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.7.0/setup.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.929311 supervision-0.7.0/supervision/
--rw-r--r--   0 skalskip   (501) staff       (20)     1044 2023-05-10 13:02:27.000000 supervision-0.7.0/supervision/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.930746 supervision-0.7.0/supervision/dataset/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/dataset/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     8641 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/core.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.931360 supervision-0.7.0/supervision/dataset/formats/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/dataset/formats/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5564 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/formats/pascal_voc.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5633 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/formats/yolo.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1094 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/ultils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.932461 supervision-0.7.0/supervision/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6799 2023-05-09 10:13:33.000000 supervision-0.7.0/supervision/detection/annotate.py
--rw-r--r--   0 skalskip   (501) staff       (20)    20838 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/detection/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     7589 2023-05-10 16:45:50.000000 supervision-0.7.0/supervision/detection/line_counter.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.932884 supervision-0.7.0/supervision/detection/tools/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.7.0/supervision/detection/tools/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5056 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/detection/tools/polygon_zone.py
--rw-r--r--   0 skalskip   (501) staff       (20)     9634 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/detection/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.933487 supervision-0.7.0/supervision/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/supervision/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/draw/color.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.7.0/supervision/draw/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1734 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/file.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934052 supervision-0.7.0/supervision/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.7.0/supervision/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/geometry/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/geometry/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)      421 2023-05-03 22:43:10.000000 supervision-0.7.0/supervision/internal.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934382 supervision-0.7.0/supervision/notebook/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/supervision/notebook/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2839 2023-05-03 22:43:10.000000 supervision-0.7.0/supervision/notebook/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/video.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.930175 supervision-0.7.0/supervision.egg-info/
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     1286 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/SOURCES.txt
--rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/dependency_links.txt
--rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/requires.txt
--rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/top_level.txt
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934625 supervision-0.7.0/test/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/test/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934749 supervision-0.7.0/test/dataset/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.7.0/test/dataset/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934973 supervision-0.7.0/test/dataset/formats/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.7.0/test/dataset/formats/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6532 2023-05-10 12:01:26.000000 supervision-0.7.0/test/dataset/formats/test_yolo.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.935524 supervision-0.7.0/test/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.7.0/test/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6749 2023-05-04 15:46:53.000000 supervision-0.7.0/test/detection/test_core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     8054 2023-04-19 14:17:19.000000 supervision-0.7.0/test/detection/test_utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.935791 supervision-0.7.0/test/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/test/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.7.0/test/draw/test_color.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.936169 supervision-0.7.0/test/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.7.0/test/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.7.0/test/geometry/test_dataclasses.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.562546 supervision-0.8.0/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.8.0/LICENSE.md
+-rw-r--r--   0 skalskip   (501) staff       (20)     6201 2023-05-17 19:36:51.562405 supervision-0.8.0/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     4874 2023-05-17 19:02:43.000000 supervision-0.8.0/README.md
+-rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-05-17 19:36:51.562599 supervision-0.8.0/setup.cfg
+-rw-r--r--   0 skalskip   (501) staff       (20)     2238 2023-05-17 17:05:52.000000 supervision-0.8.0/setup.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.554722 supervision-0.8.0/supervision/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1066 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.555997 supervision-0.8.0/supervision/dataset/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.8.0/supervision/dataset/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    13623 2023-05-17 19:34:46.000000 supervision-0.8.0/supervision/dataset/core.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.556667 supervision-0.8.0/supervision/dataset/formats/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.8.0/supervision/dataset/formats/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5396 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/dataset/formats/pascal_voc.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9267 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/dataset/formats/yolo.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2357 2023-05-17 18:23:25.000000 supervision-0.8.0/supervision/dataset/ultils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.558026 supervision-0.8.0/supervision/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6799 2023-05-09 10:13:33.000000 supervision-0.8.0/supervision/detection/annotate.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    20838 2023-05-16 14:15:01.000000 supervision-0.8.0/supervision/detection/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     7667 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/detection/line_counter.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.558342 supervision-0.8.0/supervision/detection/tools/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.8.0/supervision/detection/tools/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5056 2023-04-19 14:17:19.000000 supervision-0.8.0/supervision/detection/tools/polygon_zone.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9949 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/detection/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.558971 supervision-0.8.0/supervision/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/supervision/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/draw/color.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.8.0/supervision/draw/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2116 2023-05-17 17:05:52.000000 supervision-0.8.0/supervision/file.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.559513 supervision-0.8.0/supervision/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.8.0/supervision/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/geometry/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/geometry/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      421 2023-05-03 22:43:10.000000 supervision-0.8.0/supervision/internal.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.559823 supervision-0.8.0/supervision/notebook/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/supervision/notebook/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2839 2023-05-03 22:43:10.000000 supervision-0.8.0/supervision/notebook/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.8.0/supervision/video.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.555583 supervision-0.8.0/supervision.egg-info/
+-rw-r--r--   0 skalskip   (501) staff       (20)     6201 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     1313 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/SOURCES.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/dependency_links.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)      145 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/requires.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-05-17 19:36:51.000000 supervision-0.8.0/supervision.egg-info/top_level.txt
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.560095 supervision-0.8.0/test/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/test/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.560312 supervision-0.8.0/test/dataset/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.8.0/test/dataset/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.560699 supervision-0.8.0/test/dataset/formats/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.8.0/test/dataset/formats/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9650 2023-05-17 17:05:52.000000 supervision-0.8.0/test/dataset/formats/test_yolo.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2344 2023-05-17 18:23:25.000000 supervision-0.8.0/test/dataset/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.561378 supervision-0.8.0/test/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.8.0/test/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6749 2023-05-04 15:46:53.000000 supervision-0.8.0/test/detection/test_core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     8054 2023-04-19 14:17:19.000000 supervision-0.8.0/test/detection/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.561746 supervision-0.8.0/test/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.8.0/test/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.8.0/test/draw/test_color.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-17 19:36:51.562128 supervision-0.8.0/test/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.8.0/test/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.8.0/test/geometry/test_dataclasses.py
```

### Comparing `supervision-0.7.0/LICENSE.md` & `supervision-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/PKG-INFO` & `supervision-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.7.0
+Version: 0.8.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
@@ -84,14 +84,18 @@
           />
       </a>
       </a>
   </div>
 
   <br>
 
+[![version](https://badge.fury.io/py/supervision.svg)](https://badge.fury.io/py/supervision)
+[![downloads](https://img.shields.io/pypi/dm/supervision)](https://pypistats.org/packages/supervision)
+[![license](https://img.shields.io/pypi/l/supervision)](https://github.com/roboflow/supervision/blob/main/LICENSE.md)
+[![python-version](https://img.shields.io/pypi/pyversions/supervision)](https://badge.fury.io/py/supervision)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-detect-and-count-objects-in-polygon-zone.ipynb)
 
 </div>
 
 ## 👋 hello
 
 A set of easy-to-use utils that will come in handy in any computer vision project. **Supervision is still in
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.7.0 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.8.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -33,15 +33,21 @@
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
  [https://media.roboflow.com/notebooks/template/icons/purple/forum.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949633584]_[https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]_
  [https://media.roboflow.com/notebooks/template/icons/purple/blog.png?ik-sdk-
                version=javascript-1.4.3&updatedAt=1672949633605]
 
- [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+ [![version](https://badge.fury.io/py/supervision.svg)](https://badge.fury.io/
+  py/supervision) [![downloads](https://img.shields.io/pypi/dm/supervision)]
+       (https://pypistats.org/packages/supervision) [![license](https://
+ img.shields.io/pypi/l/supervision)](https://github.com/roboflow/supervision/
+     blob/main/LICENSE.md) [![python-version](https://img.shields.io/pypi/
+pyversions/supervision)](https://badge.fury.io/py/supervision) [![Colab](https:
+         //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-
               to-detect-and-count-objects-in-polygon-zone.ipynb)
 ## ð hello A set of easy-to-use utils that will come in handy in any
 computer vision project. **Supervision is still in pre-release stage. ð§ Keep
 your eyes open for potential bugs and be aware that at this stage our API is
 still fluid and may change.** ## ð» install Pip install the supervision
 package in a [**3.10>=Python>=3.7**](https://www.python.org/) environment.
```

### Comparing `supervision-0.7.0/README.md` & `supervision-0.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,18 @@
           />
       </a>
       </a>
   </div>
 
   <br>
 
+[![version](https://badge.fury.io/py/supervision.svg)](https://badge.fury.io/py/supervision)
+[![downloads](https://img.shields.io/pypi/dm/supervision)](https://pypistats.org/packages/supervision)
+[![license](https://img.shields.io/pypi/l/supervision)](https://github.com/roboflow/supervision/blob/main/LICENSE.md)
+[![python-version](https://img.shields.io/pypi/pyversions/supervision)](https://badge.fury.io/py/supervision)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-detect-and-count-objects-in-polygon-zone.ipynb)
 
 </div>
 
 ## 👋 hello
 
 A set of easy-to-use utils that will come in handy in any computer vision project. **Supervision is still in
```

#### html2text {}

```diff
@@ -15,15 +15,21 @@
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
  [https://media.roboflow.com/notebooks/template/icons/purple/forum.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949633584]_[https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]_
  [https://media.roboflow.com/notebooks/template/icons/purple/blog.png?ik-sdk-
                version=javascript-1.4.3&updatedAt=1672949633605]
 
- [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+ [![version](https://badge.fury.io/py/supervision.svg)](https://badge.fury.io/
+  py/supervision) [![downloads](https://img.shields.io/pypi/dm/supervision)]
+       (https://pypistats.org/packages/supervision) [![license](https://
+ img.shields.io/pypi/l/supervision)](https://github.com/roboflow/supervision/
+     blob/main/LICENSE.md) [![python-version](https://img.shields.io/pypi/
+pyversions/supervision)](https://badge.fury.io/py/supervision) [![Colab](https:
+         //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-
               to-detect-and-count-objects-in-polygon-zone.ipynb)
 ## ð hello A set of easy-to-use utils that will come in handy in any
 computer vision project. **Supervision is still in pre-release stage. ð§ Keep
 your eyes open for potential bugs and be aware that at this stage our API is
 still fluid and may change.** ## ð» install Pip install the supervision
 package in a [**3.10>=Python>=3.7**](https://www.python.org/) environment.
```

### Comparing `supervision-0.7.0/setup.py` & `supervision-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     description='A set of easy-to-use utils that will come in handy in any Computer Vision project',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/roboflow/supervision',
     install_requires=[
         'numpy>=1.20.0',
         'opencv-python',
-        'matplotlib'
+        'matplotlib',
+        'pyyaml'
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         'dev': [
             'flake8',
             'black==22.3.0',
             'isort',
```

### Comparing `supervision-0.7.0/supervision/__init__.py` & `supervision-0.8.0/supervision/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
-from supervision.dataset.core import Dataset
+from supervision.dataset.core import BaseDataset, DetectionDataset
 from supervision.detection.annotate import BoxAnnotator, MaskAnnotator
 from supervision.detection.core import Detections
 from supervision.detection.line_counter import LineZone, LineZoneAnnotator
 from supervision.detection.tools.polygon_zone import PolygonZone, PolygonZoneAnnotator
 from supervision.detection.utils import (
     box_iou_batch,
     filter_polygons_by_area,
```

### Comparing `supervision-0.7.0/supervision/dataset/core.py` & `supervision-0.8.0/supervision/dataset/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 from __future__ import annotations
 
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Iterator
+from typing import Dict, Iterator, List, Optional, Tuple
 
 import cv2
 import numpy as np
 
 from supervision.dataset.formats.pascal_voc import (
     detections_to_pascal_voc,
     load_pascal_voc_annotations,
 )
-from supervision.dataset.formats.yolo import load_yolo_annotations
+from supervision.dataset.formats.yolo import (
+    load_yolo_annotations,
+    save_data_yaml,
+    save_yolo_annotations,
+)
+from supervision.dataset.ultils import save_dataset_images, train_test_split
 from supervision.detection.core import Detections
 from supervision.file import list_files_with_extensions
 
 
 @dataclass
-class Dataset:
+class BaseDataset(ABC):
+    @abstractmethod
+    def __len__(self) -> int:
+        pass
+
+    @abstractmethod
+    def split(
+        self, split_ratio=0.8, random_state=None, shuffle: bool = True
+    ) -> Tuple[BaseDataset, BaseDataset]:
+        pass
+
+
+@dataclass
+class DetectionDataset(BaseDataset):
     """
-    Dataclass containing information about the dataset.
+    Dataclass containing information about object detection dataset.
 
     Attributes:
         classes (List[str]): List containing dataset class names.
         images (Dict[str, np.ndarray]): Dictionary mapping image name to image.
         annotations (Dict[str, Detections]): Dictionary mapping image name to annotations.
     """
 
@@ -47,21 +66,66 @@
         Yields:
             Iterator[Tuple[str, np.ndarray, Detections]]: An iterator that yields tuples containing the image name,
                                                           the image data, and its corresponding annotation.
         """
         for image_name, image in self.images.items():
             yield image_name, image, self.annotations.get(image_name, None)
 
+    def split(
+        self, split_ratio=0.8, random_state=None, shuffle: bool = True
+    ) -> Tuple[DetectionDataset, DetectionDataset]:
+        """
+        Splits the dataset into two parts (training and testing) using the provided split_ratio.
+
+        Args:
+            split_ratio (float, optional): The ratio of the training set to the entire dataset. Default is 0.8.
+            random_state (int, optional): The seed for the random number generator. This is used for reproducibility. Default is None.
+            shuffle (bool, optional): Whether to shuffle the data before splitting. Default is True.
+
+        Returns:
+            Tuple[DetectionDataset, DetectionDataset]: A tuple containing the training and testing datasets.
+
+        Example:
+            ```python
+            >>> import supervision as sv
+
+            >>> ds = sv.DetectionDataset(...)
+            >>> train_ds, test_ds = ds.split(split_ratio=0.7, random_state=42, shuffle=True)
+            >>> len(train_ds), len(test_ds)
+            (700, 300)
+            ```
+        """
+
+        image_names = list(self.images.keys())
+        train_names, test_names = train_test_split(
+            data=image_names,
+            train_ratio=split_ratio,
+            random_state=random_state,
+            shuffle=shuffle,
+        )
+
+        train_dataset = DetectionDataset(
+            classes=self.classes,
+            images={name: self.images[name] for name in train_names},
+            annotations={name: self.annotations[name] for name in train_names},
+        )
+        test_dataset = DetectionDataset(
+            classes=self.classes,
+            images={name: self.images[name] for name in test_names},
+            annotations={name: self.annotations[name] for name in test_names},
+        )
+        return train_dataset, test_dataset
+
     def as_pascal_voc(
         self,
         images_directory_path: Optional[str] = None,
         annotations_directory_path: Optional[str] = None,
         min_image_area_percentage: float = 0.0,
         max_image_area_percentage: float = 1.0,
-        approximation_percentage: float = 0.75,
+        approximation_percentage: float = 0.0,
     ) -> None:
         """
         Exports the dataset to PASCAL VOC format. This method saves the images and their corresponding annotations in
         PASCAL VOC format, which consists of XML files. The method allows filtering the detections based on their area
         percentage.
 
         Args:
@@ -103,44 +167,44 @@
 
                 with open(annotations_path / f"{annotation_name}.xml", "w") as f:
                     f.write(pascal_voc_xml)
 
     @classmethod
     def from_pascal_voc(
         cls, images_directory_path: str, annotations_directory_path: str
-    ) -> Dataset:
+    ) -> DetectionDataset:
         """
         Creates a Dataset instance from PASCAL VOC formatted data.
 
         Args:
             images_directory_path (str): The path to the directory containing the images.
             annotations_directory_path (str): The path to the directory containing the PASCAL VOC XML annotations.
 
         Returns:
-            Dataset: A Dataset instance containing the loaded images and annotations.
+            DetectionDataset: A DetectionDataset instance containing the loaded images and annotations.
 
         Example:
             ```python
             >>> import roboflow
             >>> from roboflow import Roboflow
             >>> import supervision as sv
 
             >>> roboflow.login()
 
             >>> rf = Roboflow()
 
             >>> project = rf.workspace(WORKSPACE_ID).project(PROJECT_ID)
             >>> dataset = project.version(PROJECT_VERSION).download("voc")
 
-            >>> train_dataset = sv.Dataset.from_yolo(
+            >>> ds = sv.DetectionDataset.from_yolo(
             ...     images_directory_path=f"{dataset.location}/train/images",
             ...     annotations_directory_path=f"{dataset.location}/train/labels"
             ... )
 
-            >>> dataset.classes
+            >>> ds.classes
             ['dog', 'person']
             ```
         """
         image_paths = list_files_with_extensions(
             directory=images_directory_path, extensions=["jpg", "jpeg", "png"]
         )
         annotation_paths = list_files_with_extensions(
@@ -164,59 +228,105 @@
         images = {
             image_path.name: cv2.imread(str(image_path)) for image_path in image_paths
         }
 
         annotations = {
             image_name: detections for image_name, detections, _ in raw_annotations
         }
-        return Dataset(classes=classes, images=images, annotations=annotations)
+        return DetectionDataset(classes=classes, images=images, annotations=annotations)
 
     @classmethod
     def from_yolo(
         cls,
         images_directory_path: str,
         annotations_directory_path: str,
         data_yaml_path: str,
         force_masks: bool = False,
-    ) -> Dataset:
+    ) -> DetectionDataset:
         """
         Creates a Dataset instance from YOLO formatted data.
 
         Args:
             images_directory_path (str): The path to the directory containing the images.
             annotations_directory_path (str): The path to the directory containing the YOLO annotation files.
             data_yaml_path (str): The path to the data YAML file containing class information.
             force_masks (bool, optional): If True, forces masks to be loaded for all annotations, regardless of whether they are present.
 
         Returns:
-            Dataset: A Dataset instance containing the loaded images and annotations.
+            DetectionDataset: A DetectionDataset instance containing the loaded images and annotations.
 
         Example:
             ```python
             >>> import roboflow
             >>> from roboflow import Roboflow
             >>> import supervision as sv
 
             >>> roboflow.login()
 
             >>> rf = Roboflow()
 
             >>> project = rf.workspace(WORKSPACE_ID).project(PROJECT_ID)
             >>> dataset = project.version(PROJECT_VERSION).download("yolov5")
 
-            >>> train_dataset = sv.Dataset.from_yolo(
+            >>> ds = sv.DetectionDataset.from_yolo(
             ...     images_directory_path=f"{dataset.location}/train/images",
             ...     annotations_directory_path=f"{dataset.location}/train/labels",
             ...     data_yaml_path=f"{dataset.location}/data.yaml"
             ... )
 
-            >>> dataset.classes
+            >>> ds.classes
             ['dog', 'person']
             ```
         """
         classes, images, annotations = load_yolo_annotations(
             images_directory_path=images_directory_path,
             annotations_directory_path=annotations_directory_path,
             data_yaml_path=data_yaml_path,
             force_masks=force_masks,
         )
-        return Dataset(classes=classes, images=images, annotations=annotations)
+        return DetectionDataset(classes=classes, images=images, annotations=annotations)
+
+    def as_yolo(
+        self,
+        images_directory_path: Optional[str] = None,
+        annotations_directory_path: Optional[str] = None,
+        data_yaml_path: Optional[str] = None,
+        min_image_area_percentage: float = 0.0,
+        max_image_area_percentage: float = 1.0,
+        approximation_percentage: float = 0.0,
+    ) -> None:
+        """
+        Exports the dataset to YOLO format. This method saves the images and their corresponding
+        annotations in YOLO format, which is a simple text file that describes an object in the image. It also allows
+        for the optional saving of a data.yaml file, used in YOLOv5, that contains metadata about the dataset.
+
+        The method allows filtering the detections based on their area percentage and offers an option for polygon approximation.
+
+        Args:
+            images_directory_path (Optional[str]): The path to the directory where the images should be saved.
+                If not provided, images will not be saved.
+            annotations_directory_path (Optional[str]): The path to the directory where the annotations in
+                YOLO format should be saved. If not provided, annotations will not be saved.
+            data_yaml_path (Optional[str]): The path where the data.yaml file should be saved.
+                If not provided, the file will not be saved.
+            min_image_area_percentage (float): The minimum percentage of detection area relative to
+                the image area for a detection to be included.
+            max_image_area_percentage (float): The maximum percentage of detection area relative to
+                the image area for a detection to be included.
+            approximation_percentage (float): The percentage of polygon points to be removed from the input polygon,
+                in the range [0, 1). This is useful for simplifying the annotations.
+        """
+        if images_directory_path is not None:
+            save_dataset_images(
+                images_directory_path=images_directory_path, images=self.images
+            )
+        if annotations_directory_path is not None:
+            save_yolo_annotations(
+                annotations_directory_path=annotations_directory_path,
+                images=self.images,
+                annotations=self.annotations,
+                min_image_area_percentage=min_image_area_percentage,
+                max_image_area_percentage=max_image_area_percentage,
+                approximation_percentage=approximation_percentage,
+            )
+        if data_yaml_path is not None:
+            save_data_yaml(data_yaml_path=data_yaml_path, classes=self.classes)
```

### Comparing `supervision-0.7.0/supervision/dataset/formats/pascal_voc.py` & `supervision-0.8.0/supervision/dataset/formats/pascal_voc.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,14 @@
         min_image_area_percentage (float): Minimum detection area relative to area of image associated with it.
         max_image_area_percentage (float): Maximum detection area relative to area of image associated with it.
         approximation_percentage (float): The percentage of polygon points to be removed from the input polygon, in the range [0, 1).
     Returns:
         str: An XML string in Pascal VOC format representing the detections.
     """
     height, width, depth = image_shape
-    image_area = height * width
-    minimum_detection_area = min_image_area_percentage * image_area
-    maximum_detection_area = max_image_area_percentage * image_area
 
     # Create root element
     annotation = Element("annotation")
 
     # Add folder element
     folder = SubElement(annotation, "folder")
     folder.text = "VOC"
```

### Comparing `supervision-0.7.0/supervision/dataset/formats/yolo.py` & `supervision-0.8.0/supervision/dataset/formats/yolo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import os
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
+import yaml
 
+from supervision.dataset.ultils import approximate_mask_with_polygons
 from supervision.detection.core import Detections
 from supervision.detection.utils import polygon_to_mask, polygon_to_xyxy
-from supervision.file import list_files_with_extensions, read_txt_file
+from supervision.file import list_files_with_extensions, read_txt_file, save_text_file
 
 
 def _parse_box(values: List[str]) -> np.ndarray:
     x_center, y_center, width, height = values
     return np.array(
         [
             float(x_center) - float(width) / 2,
@@ -74,14 +77,19 @@
                 names.append(line.strip().replace("-", "").strip())
             else:
                 break
 
     return names
 
 
+def _image_name_to_annotation_name(image_name: str) -> str:
+    base_name, _ = os.path.splitext(image_name)
+    return base_name + ".txt"
+
+
 def yolo_annotations_to_detections(
     lines: List[str], resolution_wh: Tuple[int, int], with_masks: bool
 ) -> Detections:
     if len(lines) == 0:
         return Detections.empty()
 
     class_id, relative_xyxy, relative_polygon = [], [], []
@@ -126,15 +134,15 @@
     Args:
         images_directory_path (str): The path to the directory containing the images.
         annotations_directory_path (str): The path to the directory containing the YOLO annotation files.
         data_yaml_path (str): The path to the data YAML file containing class information.
         force_masks (bool, optional): If True, forces masks to be loaded for all annotations, regardless of whether they are present.
 
     Returns:
-        Tuple[List[str], Dict[str, np.ndarray], Dict[str, Detections]]: A tuple containing a list of class names, a dictionary with image paths as keys and images as values, and a dictionary with image paths as keys and corresponding Detections instances as values.
+        Tuple[List[str], Dict[str, np.ndarray], Dict[str, Detections]]: A tuple containing a list of class names, a dictionary with image names as keys and images as values, and a dictionary with image names as keys and corresponding Detections instances as values.
     """
     image_paths = list_files_with_extensions(
         directory=images_directory_path, extensions=["jpg", "jpeg", "png"]
     )
     annotation_paths = list_files_with_extensions(
         directory=annotations_directory_path, extensions=["txt"]
     )
@@ -152,10 +160,97 @@
 
         with_masks = _with_mask(lines=lines)
         with_masks = force_masks if force_masks else with_masks
         annotation = yolo_annotations_to_detections(
             lines=lines, resolution_wh=resolution_wh, with_masks=with_masks
         )
 
-        images[str(image_path)] = image
-        annotations[str(image_path)] = annotation
+        images[image_path.name] = image
+        annotations[image_path.name] = annotation
     return classes, images, annotations
+
+
+def object_to_yolo(
+    xyxy: np.ndarray,
+    class_id: int,
+    image_shape: Tuple[int, int, int],
+    polygon: Optional[np.ndarray] = None,
+) -> str:
+    h, w, _ = image_shape
+    if polygon is None:
+        xyxy_relative = xyxy / np.array([w, h, w, h], dtype=np.float32)
+        x_min, y_min, x_max, y_max = xyxy_relative
+        x_center = (x_min + x_max) / 2
+        y_center = (y_min + y_max) / 2
+        width = x_max - x_min
+        height = y_max - y_min
+        return f"{int(class_id)} {x_center:.5f} {y_center:.5f} {width:.5f} {height:.5f}"
+    else:
+        polygon_relative = polygon / np.array([w, h], dtype=np.float32)
+        polygon_relative = polygon_relative.reshape(-1)
+        polygon_parsed = " ".join([f"{value:.5f}" for value in polygon_relative])
+        return f"{int(class_id)} {polygon_parsed}"
+
+
+def detections_to_yolo_annotations(
+    detections: Detections,
+    image_shape: Tuple[int, int, int],
+    min_image_area_percentage: float = 0.0,
+    max_image_area_percentage: float = 1.0,
+    approximation_percentage: float = 0.75,
+) -> List[str]:
+    annotation = []
+    for xyxy, mask, _, class_id, _ in detections:
+        if mask is not None:
+            polygons = approximate_mask_with_polygons(
+                mask=mask,
+                min_image_area_percentage=min_image_area_percentage,
+                max_image_area_percentage=max_image_area_percentage,
+                approximation_percentage=approximation_percentage,
+            )
+            for polygon in polygons:
+                xyxy = polygon_to_xyxy(polygon=polygon)
+                next_object = object_to_yolo(
+                    xyxy=xyxy,
+                    class_id=class_id,
+                    image_shape=image_shape,
+                    polygon=polygon,
+                )
+                annotation.append(next_object)
+        else:
+            next_object = object_to_yolo(
+                xyxy=xyxy, class_id=class_id, image_shape=image_shape
+            )
+            annotation.append(next_object)
+    return annotation
+
+
+def save_yolo_annotations(
+    annotations_directory_path: str,
+    images: Dict[str, np.ndarray],
+    annotations: Dict[str, Detections],
+    min_image_area_percentage: float = 0.0,
+    max_image_area_percentage: float = 1.0,
+    approximation_percentage: float = 0.75,
+) -> None:
+    Path(annotations_directory_path).mkdir(parents=True, exist_ok=True)
+    for image_name, image in images.items():
+        detections = annotations[image_name]
+        yolo_annotations_name = _image_name_to_annotation_name(image_name=image_name)
+        yolo_annotations_path = os.path.join(
+            annotations_directory_path, yolo_annotations_name
+        )
+        lines = detections_to_yolo_annotations(
+            detections=detections,
+            image_shape=image.shape,
+            min_image_area_percentage=min_image_area_percentage,
+            max_image_area_percentage=max_image_area_percentage,
+            approximation_percentage=approximation_percentage,
+        )
+        save_text_file(lines=lines, file_path=yolo_annotations_path)
+
+
+def save_data_yaml(data_yaml_path: str, classes: List[str]) -> None:
+    data = {"nc": len(classes), "names": classes}
+    Path(data_yaml_path).parent.mkdir(parents=True, exist_ok=True)
+    with open(data_yaml_path, "w") as outfile:
+        yaml.dump(data, outfile, default_flow_style=False)
```

### Comparing `supervision-0.7.0/supervision/detection/annotate.py` & `supervision-0.8.0/supervision/detection/annotate.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/detection/core.py` & `supervision-0.8.0/supervision/detection/core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/detection/line_counter.py` & `supervision-0.8.0/supervision/detection/line_counter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Dict
+from typing import Dict, Optional
 
 import cv2
 import numpy as np
 
 from supervision.detection.core import Detections
 from supervision.draw.color import Color
 from supervision.geometry.core import Point, Rect, Vector
-from typing import Optional
 
 
 class LineZone:
     """
     Count the number of objects that cross a line.
     """
 
@@ -67,14 +66,15 @@
 
             self.tracker_state[tracker_id] = tracker_state
             if tracker_state:
                 self.in_count += 1
             else:
                 self.out_count += 1
 
+
 class LineZoneAnnotator:
     def __init__(
         self,
         thickness: float = 2,
         color: Color = Color.white(),
         text_thickness: float = 2,
         text_color: Color = Color.black(),
@@ -141,17 +141,24 @@
             line_counter.vector.end.as_xy_int_tuple(),
             radius=5,
             color=self.text_color.as_bgr(),
             thickness=-1,
             lineType=cv2.LINE_AA,
         )
 
-        in_text = f"{self.custom_in_text}: {line_counter.in_count}" if self.custom_in_text is not None else f"in: {line_counter.in_count}"
-        out_text = f"{self.custom_out_text}: {line_counter.out_count}" if self.custom_out_text is not None else f"out: {line_counter.out_count}"
-
+        in_text = (
+            f"{self.custom_in_text}: {line_counter.in_count}"
+            if self.custom_in_text is not None
+            else f"in: {line_counter.in_count}"
+        )
+        out_text = (
+            f"{self.custom_out_text}: {line_counter.out_count}"
+            if self.custom_out_text is not None
+            else f"out: {line_counter.out_count}"
+        )
 
         (in_text_width, in_text_height), _ = cv2.getTextSize(
             in_text, cv2.FONT_HERSHEY_SIMPLEX, self.text_scale, self.text_thickness
         )
         (out_text_width, out_text_height), _ = cv2.getTextSize(
             out_text, cv2.FONT_HERSHEY_SIMPLEX, self.text_scale, self.text_thickness
         )
```

### Comparing `supervision-0.7.0/supervision/detection/tools/polygon_zone.py` & `supervision-0.8.0/supervision/detection/tools/polygon_zone.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/detection/utils.py` & `supervision-0.8.0/supervision/detection/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -216,38 +216,45 @@
         np.ndarray: A 1D NumPy array containing the bounding box `(x_min, y_min, x_max, y_max)` of the input polygon.
     """
     x_min, y_min = np.min(polygon, axis=0)
     x_max, y_max = np.max(polygon, axis=0)
     return np.array([x_min, y_min, x_max, y_max])
 
 
-def approximate_polygon(polygon: np.ndarray, percentage: float) -> np.ndarray:
+def approximate_polygon(
+    polygon: np.ndarray, percentage: float, epsilon_step: float = 0.05
+) -> np.ndarray:
     """
     Approximates a given polygon by reducing a certain percentage of points.
 
     This function uses the Ramer-Douglas-Peucker algorithm to simplify the input polygon by reducing the number of points
     while preserving the general shape.
 
     Parameters:
-        polygon (np.ndarray): A 2D NumPy array of shape (N, 2) containing the x, y coordinates of the input polygon's points.
-        percentage (float): The percentage of points to be removed from the input polygon, in the range [0, 1).
+        polygon (np.ndarray): A 2D NumPy array of shape `(N, 2)` containing the `x`, `y` coordinates of the input polygon's points.
+        percentage (float): The percentage of points to be removed from the input polygon, in the range `[0, 1)`.
+        epsilon_step (float): Approximation accuracy step. Epsilon is the maximum distance between the original curve and its approximation.
 
     Returns:
-        np.ndarray: A new 2D NumPy array of shape (M, 2), where M <= N * (1 - percentage), containing the x, y coordinates of the
+        np.ndarray: A new 2D NumPy array of shape `(M, 2)`, where `M <= N * (1 - percentage)`, containing the `x`, `y` coordinates of the
             approximated polygon's points.
     """
 
     if percentage < 0 or percentage >= 1:
         raise ValueError("Percentage must be in the range [0, 1).")
 
     target_points = max(int(len(polygon) * (1 - percentage)), 3)
 
     if len(polygon) <= target_points:
         return polygon
 
     epsilon = 0
     approximated_points = polygon
-    while len(approximated_points) > target_points:
-        epsilon += 0.1
-        approximated_points = cv2.approxPolyDP(polygon, epsilon, closed=True)
+    while True:
+        epsilon += epsilon_step
+        new_approximated_points = cv2.approxPolyDP(polygon, epsilon, closed=True)
+        if len(new_approximated_points) > target_points:
+            approximated_points = new_approximated_points
+        else:
+            break
 
     return np.squeeze(approximated_points, axis=1)
```

### Comparing `supervision-0.7.0/supervision/draw/color.py` & `supervision-0.8.0/supervision/draw/color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/draw/utils.py` & `supervision-0.8.0/supervision/draw/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/file.py` & `supervision-0.8.0/supervision/file.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,7 +49,20 @@
         List[str]: A list of strings representing the lines in the text file.
     """
     with open(file_path, "r") as file:
         lines = file.readlines()
         lines = [line.rstrip("\n") for line in lines]
 
     return lines
+
+
+def save_text_file(lines: List[str], file_path: str):
+    """
+    Write a list of strings to a text file, each string on a new line.
+
+    Args:
+        lines (List[str]): The list of strings to be written to the file.
+        file_path (str): The path to the text file.
+    """
+    with open(file_path, "w") as file:
+        for line in lines:
+            file.write(line + "\n")
```

### Comparing `supervision-0.7.0/supervision/geometry/core.py` & `supervision-0.8.0/supervision/geometry/core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/geometry/utils.py` & `supervision-0.8.0/supervision/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/notebook/utils.py` & `supervision-0.8.0/supervision/notebook/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision/video.py` & `supervision-0.8.0/supervision/video.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/supervision.egg-info/PKG-INFO` & `supervision-0.8.0/supervision.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.7.0
+Version: 0.8.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
@@ -84,14 +84,18 @@
           />
       </a>
       </a>
   </div>
 
   <br>
 
+[![version](https://badge.fury.io/py/supervision.svg)](https://badge.fury.io/py/supervision)
+[![downloads](https://img.shields.io/pypi/dm/supervision)](https://pypistats.org/packages/supervision)
+[![license](https://img.shields.io/pypi/l/supervision)](https://github.com/roboflow/supervision/blob/main/LICENSE.md)
+[![python-version](https://img.shields.io/pypi/pyversions/supervision)](https://badge.fury.io/py/supervision)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-detect-and-count-objects-in-polygon-zone.ipynb)
 
 </div>
 
 ## 👋 hello
 
 A set of easy-to-use utils that will come in handy in any computer vision project. **Supervision is still in
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.7.0 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.8.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -33,15 +33,21 @@
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
  [https://media.roboflow.com/notebooks/template/icons/purple/forum.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949633584]_[https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]_
  [https://media.roboflow.com/notebooks/template/icons/purple/blog.png?ik-sdk-
                version=javascript-1.4.3&updatedAt=1672949633605]
 
- [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+ [![version](https://badge.fury.io/py/supervision.svg)](https://badge.fury.io/
+  py/supervision) [![downloads](https://img.shields.io/pypi/dm/supervision)]
+       (https://pypistats.org/packages/supervision) [![license](https://
+ img.shields.io/pypi/l/supervision)](https://github.com/roboflow/supervision/
+     blob/main/LICENSE.md) [![python-version](https://img.shields.io/pypi/
+pyversions/supervision)](https://badge.fury.io/py/supervision) [![Colab](https:
+         //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-
               to-detect-and-count-objects-in-polygon-zone.ipynb)
 ## ð hello A set of easy-to-use utils that will come in handy in any
 computer vision project. **Supervision is still in pre-release stage. ð§ Keep
 your eyes open for potential bugs and be aware that at this stage our API is
 still fluid and may change.** ## ð» install Pip install the supervision
 package in a [**3.10>=Python>=3.7**](https://www.python.org/) environment.
```

### Comparing `supervision-0.7.0/supervision.egg-info/SOURCES.txt` & `supervision-0.8.0/supervision.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 supervision/geometry/__init__.py
 supervision/geometry/core.py
 supervision/geometry/utils.py
 supervision/notebook/__init__.py
 supervision/notebook/utils.py
 test/__init__.py
 test/dataset/__init__.py
+test/dataset/test_utils.py
 test/dataset/formats/__init__.py
 test/dataset/formats/test_yolo.py
 test/detection/__init__.py
 test/detection/test_core.py
 test/detection/test_utils.py
 test/draw/__init__.py
 test/draw/test_color.py
```

### Comparing `supervision-0.7.0/test/dataset/formats/test_yolo.py` & `supervision-0.8.0/test/dataset/formats/test_yolo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from contextlib import ExitStack as DoesNotRaise
 from typing import List, Tuple, Optional
 
 import pytest
 import numpy as np
 
 from supervision.detection.core import Detections
-from supervision.dataset.formats.yolo import yolo_annotations_to_detections, _with_mask
+from supervision.dataset.formats.yolo import yolo_annotations_to_detections, _with_mask, _image_name_to_annotation_name, \
+    object_to_yolo
 
 
 def _mock_simple_mask(resolution_wh: Tuple[int, int], box: List[int]) -> np.array:
     x_min, y_min, x_max, y_max = box
     mask = np.full(resolution_wh, False, dtype=bool)
     mask[y_min:y_max, x_min:x_max] = True
     return mask
@@ -198,7 +199,106 @@
         result = yolo_annotations_to_detections(
             lines=lines,
             resolution_wh=resolution_wh,
             with_masks=with_masks)
         assert np.array_equal(result.xyxy, expected_result.xyxy)
         assert np.array_equal(result.class_id, expected_result.class_id)
         assert (result.mask is None and expected_result.mask is None) or _arrays_almost_equal(result.mask, expected_result.mask)
+
+
+@pytest.mark.parametrize(
+    'image_name, expected_result, exception',
+    [
+        (
+            'image.png',
+            'image.txt',
+            DoesNotRaise()
+        ),  # simple png image
+        (
+            'image.jpeg',
+            'image.txt',
+            DoesNotRaise()
+        ),  # simple jpeg image
+        (
+            'image.jpg',
+            'image.txt',
+            DoesNotRaise()
+        ),  # simple jpg image
+        (
+            'image.000.jpg',
+            'image.000.txt',
+            DoesNotRaise()
+        ),  # jpg image with multiple dots in name
+    ]
+)
+def test_image_name_to_annotation_name(
+    image_name: str,
+    expected_result: Optional[str],
+    exception: Exception
+) -> None:
+    with exception:
+        result = _image_name_to_annotation_name(image_name=image_name)
+        assert result == expected_result
+
+
+@pytest.mark.parametrize(
+    'xyxy, class_id, image_shape, polygon, expected_result, exception',
+    [
+        (
+            np.array([100, 100, 200, 200], dtype=np.float32),
+            1,
+            (1000, 1000, 3),
+            None,
+            '1 0.15000 0.15000 0.10000 0.10000',
+            DoesNotRaise()
+        ),  # square bounding box on square image
+        (
+            np.array([100, 100, 200, 200], dtype=np.float32),
+            1,
+            (800, 1000, 3),
+            None,
+            '1 0.15000 0.18750 0.10000 0.12500',
+            DoesNotRaise()
+        ),  # square bounding box on horizontal image
+        (
+            np.array([100, 100, 200, 200], dtype=np.float32),
+            1,
+            (1000, 800, 3),
+            None,
+            '1 0.18750 0.15000 0.12500 0.10000',
+            DoesNotRaise()
+        ),  # square bounding box on vertical image
+        (
+            np.array([100, 200, 200, 400], dtype=np.float32),
+            1,
+            (1000, 1000, 3),
+            None,
+            '1 0.15000 0.30000 0.10000 0.20000',
+            DoesNotRaise()
+        ),  # horizontal bounding box on square image
+        (
+            np.array([200, 100, 400, 200], dtype=np.float32),
+            1,
+            (1000, 1000, 3),
+            None,
+            '1 0.30000 0.15000 0.20000 0.10000',
+            DoesNotRaise()
+        ),  # vertical bounding box on square image
+        (
+            np.array([100, 100, 200, 200], dtype=np.float32),
+            1,
+            (1000, 1000, 3),
+            np.array([
+                [100, 100],
+                [200, 100],
+                [200, 200],
+                [100, 100]
+            ], dtype=np.float32),
+            '1 0.10000 0.10000 0.20000 0.10000 0.20000 0.20000 0.10000 0.10000',
+            DoesNotRaise()
+        ),  # square mask on square image
+    ]
+)
+def test_object_to_yolo(xyxy: np.ndarray, class_id: int, image_shape: Tuple[int, int, int], polygon: Optional[np.ndarray], expected_result: Optional[str], exception: Exception) -> None:
+    with exception:
+        result = object_to_yolo(xyxy=xyxy, class_id=class_id, image_shape=image_shape, polygon=polygon)
+        assert result == expected_result
```

### Comparing `supervision-0.7.0/test/detection/test_core.py` & `supervision-0.8.0/test/detection/test_core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/test/detection/test_utils.py` & `supervision-0.8.0/test/detection/test_utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/test/draw/test_color.py` & `supervision-0.8.0/test/draw/test_color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.7.0/test/geometry/test_dataclasses.py` & `supervision-0.8.0/test/geometry/test_dataclasses.py`

 * *Files identical despite different names*

