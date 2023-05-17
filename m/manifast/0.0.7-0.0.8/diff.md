# Comparing `tmp/manifast-0.0.7.tar.gz` & `tmp/manifast-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manifast-0.0.7.tar", last modified: Thu Apr 20 07:06:05 2023, max compression
+gzip compressed data, was "manifast-0.0.8.tar", last modified: Wed May 17 06:15:16 2023, max compression
```

## Comparing `manifast-0.0.7.tar` & `manifast-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/
--rw-rw-r--   0 knight    (1000) knight    (1000)       33 2023-02-24 15:52:08.000000 manifast-0.0.7/MANIFEST.in
--rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-04-20 07:06:05.000000 manifast-0.0.7/PKG-INFO
--rw-rw-r--   0 knight    (1000) knight    (1000)       11 2023-02-24 09:21:56.000000 manifast-0.0.7/README.md
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/
--rw-rw-r--   0 knight    (1000) knight    (1000)      367 2023-02-24 15:58:02.000000 manifast-0.0.7/manifast/__init__.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/gui_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      321 2023-02-27 01:41:55.000000 manifast-0.0.7/manifast/gui_utils/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      422 2023-02-27 10:18:34.000000 manifast-0.0.7/manifast/gui_utils/counter.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      992 2023-04-04 08:48:51.000000 manifast-0.0.7/manifast/import_pkg.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/iostream/
--rw-rw-r--   0 knight    (1000) knight    (1000)      498 2023-04-20 07:01:48.000000 manifast-0.0.7/manifast/iostream/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1904 2023-04-20 07:05:50.000000 manifast-0.0.7/manifast/iostream/envstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3789 2023-04-15 15:56:19.000000 manifast-0.0.7/manifast/iostream/filestream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     2217 2023-04-09 04:26:57.000000 manifast-0.0.7/manifast/iostream/imagestream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      773 2023-04-06 02:01:32.000000 manifast-0.0.7/manifast/iostream/logstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      680 2023-04-04 07:04:06.000000 manifast-0.0.7/manifast/iostream/pdstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1631 2023-04-09 04:32:18.000000 manifast-0.0.7/manifast/iostream/pltstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1305 2023-04-06 02:33:09.000000 manifast-0.0.7/manifast/iostream/processsing.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/label_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      329 2023-02-24 15:52:38.000000 manifast-0.0.7/manifast/label_utils/__init__.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/label_utils/classify/
--rw-rw-r--   0 knight    (1000) knight    (1000)      338 2023-02-24 15:53:30.000000 manifast-0.0.7/manifast/label_utils/classify/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      344 2023-02-24 15:40:14.000000 manifast-0.0.7/manifast/label_utils/classify/gen_split_data.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/label_utils/detect/
--rw-rw-r--   0 knight    (1000) knight    (1000)      336 2023-02-24 15:53:26.000000 manifast-0.0.7/manifast/label_utils/detect/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      985 2023-02-25 14:16:00.000000 manifast-0.0.7/manifast/label_utils/detect/convert_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1903 2023-02-25 14:16:04.000000 manifast-0.0.7/manifast/label_utils/detect/gen_split_data.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     5031 2023-02-25 14:16:06.000000 manifast-0.0.7/manifast/label_utils/detect/vis_label.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/label_utils/segment/
--rw-rw-r--   0 knight    (1000) knight    (1000)      337 2023-02-24 15:53:21.000000 manifast-0.0.7/manifast/label_utils/segment/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     4301 2023-02-25 01:34:19.000000 manifast-0.0.7/manifast/label_utils/segment/colorize_mask.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     7247 2023-02-25 14:16:31.000000 manifast-0.0.7/manifast/label_utils/segment/convert_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1644 2023-02-25 02:17:38.000000 manifast-0.0.7/manifast/label_utils/segment/convert_utils.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3977 2023-02-25 14:17:05.000000 manifast-0.0.7/manifast/label_utils/segment/gen_split_data.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1236 2023-02-25 14:17:11.000000 manifast-0.0.7/manifast/label_utils/segment/vis_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     4864 2023-02-25 14:20:53.000000 manifast-0.0.7/manifast/label_utils/segment/vis_utils.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast/model_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      331 2023-02-24 14:27:00.000000 manifast-0.0.7/manifast/model_utils/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     2043 2023-02-25 01:29:23.000000 manifast-0.0.7/manifast/model_utils/eval_runtime.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     5513 2023-02-25 01:19:07.000000 manifast-0.0.7/manifast/model_utils/grad_cam.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3033 2023-02-24 13:01:54.000000 manifast-0.0.7/manifast/model_utils/summary.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast.egg-info/
--rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast.egg-info/PKG-INFO
--rw-rw-r--   0 knight    (1000) knight    (1000)     1264 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast.egg-info/SOURCES.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)        1 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast.egg-info/dependency_links.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)        9 2023-04-20 07:06:05.000000 manifast-0.0.7/manifast.egg-info/top_level.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)      107 2023-04-20 07:06:05.000000 manifast-0.0.7/setup.cfg
--rw-rw-r--   0 knight    (1000) knight    (1000)     1442 2023-04-15 16:15:43.000000 manifast-0.0.7/setup.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/
+-rw-rw-r--   0 knight    (1000) knight    (1000)       33 2023-02-24 15:52:08.000000 manifast-0.0.8/MANIFEST.in
+-rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-17 06:15:16.659279 manifast-0.0.8/PKG-INFO
+-rw-rw-r--   0 knight    (1000) knight    (1000)       11 2023-02-24 09:21:56.000000 manifast-0.0.8/README.md
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.655279 manifast-0.0.8/manifast/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      367 2023-02-24 15:58:02.000000 manifast-0.0.8/manifast/__init__.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.655279 manifast-0.0.8/manifast/gui_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      321 2023-02-27 01:41:55.000000 manifast-0.0.8/manifast/gui_utils/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      422 2023-02-27 10:18:34.000000 manifast-0.0.8/manifast/gui_utils/counter.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      994 2023-05-17 06:15:00.000000 manifast-0.0.8/manifast/import_pkg.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/iostream/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      498 2023-04-20 07:01:48.000000 manifast-0.0.8/manifast/iostream/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1904 2023-04-20 07:05:50.000000 manifast-0.0.8/manifast/iostream/envstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     3882 2023-05-08 02:35:21.000000 manifast-0.0.8/manifast/iostream/filestream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     2217 2023-04-09 04:26:57.000000 manifast-0.0.8/manifast/iostream/imagestream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      773 2023-04-06 02:01:32.000000 manifast-0.0.8/manifast/iostream/logstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      680 2023-04-04 07:04:06.000000 manifast-0.0.8/manifast/iostream/pdstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1631 2023-04-09 04:32:18.000000 manifast-0.0.8/manifast/iostream/pltstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1307 2023-05-08 02:31:43.000000 manifast-0.0.8/manifast/iostream/processsing.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      329 2023-02-24 15:52:38.000000 manifast-0.0.8/manifast/label_utils/__init__.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/classify/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      338 2023-02-24 15:53:30.000000 manifast-0.0.8/manifast/label_utils/classify/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      344 2023-02-24 15:40:14.000000 manifast-0.0.8/manifast/label_utils/classify/gen_split_data.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/detect/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      336 2023-02-24 15:53:26.000000 manifast-0.0.8/manifast/label_utils/detect/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      985 2023-02-25 14:16:00.000000 manifast-0.0.8/manifast/label_utils/detect/convert_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1903 2023-02-25 14:16:04.000000 manifast-0.0.8/manifast/label_utils/detect/gen_split_data.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     5031 2023-02-25 14:16:06.000000 manifast-0.0.8/manifast/label_utils/detect/vis_label.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/segment/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      337 2023-02-24 15:53:21.000000 manifast-0.0.8/manifast/label_utils/segment/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4301 2023-02-25 01:34:19.000000 manifast-0.0.8/manifast/label_utils/segment/colorize_mask.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     7247 2023-02-25 14:16:31.000000 manifast-0.0.8/manifast/label_utils/segment/convert_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1644 2023-02-25 02:17:38.000000 manifast-0.0.8/manifast/label_utils/segment/convert_utils.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     3977 2023-02-25 14:17:05.000000 manifast-0.0.8/manifast/label_utils/segment/gen_split_data.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1236 2023-02-25 14:17:11.000000 manifast-0.0.8/manifast/label_utils/segment/vis_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4864 2023-02-25 14:20:53.000000 manifast-0.0.8/manifast/label_utils/segment/vis_utils.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/model_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      331 2023-02-24 14:27:00.000000 manifast-0.0.8/manifast/model_utils/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     2043 2023-02-25 01:29:23.000000 manifast-0.0.8/manifast/model_utils/eval_runtime.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     5513 2023-02-25 01:19:07.000000 manifast-0.0.8/manifast/model_utils/grad_cam.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     3033 2023-02-24 13:01:54.000000 manifast-0.0.8/manifast/model_utils/summary.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.655279 manifast-0.0.8/manifast.egg-info/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/PKG-INFO
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1264 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/SOURCES.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)        1 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/dependency_links.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)        9 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/top_level.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)      107 2023-05-17 06:15:16.659279 manifast-0.0.8/setup.cfg
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1442 2023-05-17 06:13:50.000000 manifast-0.0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `manifast-0.0.7/manifast/import_pkg.py` & `manifast-0.0.8/manifast/import_pkg.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 18:22:41
 FilePath     : /manifast/manifast/import_pkg.py
 Description  : 
-LastEditTime : 2023-04-04 16:48:43
+LastEditTime : 2023-05-17 14:14:59
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 import os
 import re
 import cv2
@@ -27,14 +27,14 @@
 from tqdm import tqdm
 from loguru import logger
 from easydict import EasyDict as edict
 from PIL import Image, ImageDraw
 from multiprocessing import Pool
 from argparse import ArgumentParser
 import matplotlib.pyplot as plt
-from labelme.utils import draw_label
+# from labelme.utils import draw_label
 from easydict import EasyDict as edict
 plt.rcParams['font.sans-serif'] = ['SimHei']
 plt.rcParams['axes.unicode_minus'] = False
 if not os.getcwd().split('\\')[-1].find('notebooks') == -1:
     os.chdir('../')
 sys.path.append(os.getcwd())
```

### Comparing `manifast-0.0.7/manifast/iostream/envstream.py` & `manifast-0.0.8/manifast/iostream/envstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/iostream/filestream.py` & `manifast-0.0.8/manifast/iostream/filestream.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 16:57:43
 FilePath     : /manifast/manifast/iostream/filestream.py
 Description  : 
-LastEditTime : 2023-04-15 23:56:19
+LastEditTime : 2023-05-08 10:35:21
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 import os
 import time
 import json
@@ -48,15 +48,18 @@
                 for filename in filenames:
                     if (os.path.splitext(filename)[1] in extention):
                         path_list.append(os.path.join(dirpath, filename))
     return path_list
 
 
 def make_path_dirs(path):
-    os.makedirs(os.path.dirname(path), exist_ok=True)
+    if '.' in os.path.basename(path):
+        os.makedirs(os.path.dirname(path), exist_ok=True)
+    else:
+        os.makedirs(path, exist_ok=True)
 
 
 def save_dict2json(data={}, save_path='./results.json'):
     """
      description: 将data保存到指定的json文件下
      param       {*} data 
      param       {*} save_path
```

### Comparing `manifast-0.0.7/manifast/iostream/imagestream.py` & `manifast-0.0.8/manifast/iostream/imagestream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/iostream/logstream.py` & `manifast-0.0.8/manifast/iostream/logstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/iostream/pdstream.py` & `manifast-0.0.8/manifast/iostream/pdstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/iostream/pltstream.py` & `manifast-0.0.8/manifast/iostream/pltstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/iostream/processsing.py` & `manifast-0.0.8/manifast/iostream/processsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 21:58:02
 FilePath     : /manifast/manifast/iostream/processsing.py
 Description  : 
-LastEditTime : 2023-04-06 10:32:30
+LastEditTime : 2023-05-08 10:31:40
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 from multiprocessing import Pool
 from tqdm import tqdm
-from logstream import LOG_INFO
+from .logstream import LOG_INFO
 
 
 def run(image_path):
     print(image_path, end='')
-    return(image_path)
+    return (image_path)
 
 
 def run_multi_threading(data_list, func):
     '''
     description: 多线程运行函数
     param       {*} data_list 所要处理数据 list
     param       {*} func 处理单条数据函数
```

### Comparing `manifast-0.0.7/manifast/label_utils/detect/convert_label.py` & `manifast-0.0.8/manifast/label_utils/detect/convert_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/detect/gen_split_data.py` & `manifast-0.0.8/manifast/label_utils/detect/gen_split_data.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/detect/vis_label.py` & `manifast-0.0.8/manifast/label_utils/detect/vis_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/segment/colorize_mask.py` & `manifast-0.0.8/manifast/label_utils/segment/colorize_mask.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/segment/convert_label.py` & `manifast-0.0.8/manifast/label_utils/segment/convert_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/segment/convert_utils.py` & `manifast-0.0.8/manifast/label_utils/segment/convert_utils.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/segment/gen_split_data.py` & `manifast-0.0.8/manifast/label_utils/segment/gen_split_data.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/segment/vis_label.py` & `manifast-0.0.8/manifast/label_utils/segment/vis_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/label_utils/segment/vis_utils.py` & `manifast-0.0.8/manifast/label_utils/segment/vis_utils.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/model_utils/eval_runtime.py` & `manifast-0.0.8/manifast/model_utils/eval_runtime.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/model_utils/grad_cam.py` & `manifast-0.0.8/manifast/model_utils/grad_cam.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast/model_utils/summary.py` & `manifast-0.0.8/manifast/model_utils/summary.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/manifast.egg-info/SOURCES.txt` & `manifast-0.0.8/manifast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manifast-0.0.7/setup.py` & `manifast-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 15:48:13
 FilePath     : /manifast/setup.py
 Description  : 
-LastEditTime : 2023-04-16 00:15:43
+LastEditTime : 2023-05-17 14:13:49
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 
 from os import path
 from setuptools import setup, find_packages
@@ -25,15 +25,15 @@
 install_requires = [x.strip() for x in all_reqs if 'git+' not in x]
 
 # 读取readme文件
 with open("README.md", "r", encoding='utf-8') as f:
     readme = f.read()
 setup(
     name="manifast",  # 包名称
-    version="0.0.7",  # 版本
+    version="0.0.8",  # 版本
     author="Knight",  # 包邮箱
     author_email="knightdby@163.com",  # 作者邮箱
     description="A small example package",  # 包描述
     license='MIT License',
     # 长描述，通常是readme ,打包到PiPy需要 。
     long_description=long_description,
     long_description_content_type='text/markdown',
```

