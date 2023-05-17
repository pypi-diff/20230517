# Comparing `tmp/dataset-tools-0.0.7.tar.gz` & `tmp/dataset-tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-tools-0.0.7.tar", last modified: Wed May 17 10:14:54 2023, max compression
+gzip compressed data, was "dataset-tools-0.0.8.tar", last modified: Wed May 17 10:26:01 2023, max compression
```

## Comparing `dataset-tools-0.0.7.tar` & `dataset-tools-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/dataset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/dataset_tools/image/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/dataset_tools/image/renders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/renders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/renders/poster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/renders/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/renders/separated_anns_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/renders/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/dataset_tools/image/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/basestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/class_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/class_cooccurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/classes_per_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/heatmaps_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/object_and_class_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/objects_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/dataset_tools/image/stats/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/dataset_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 10:14:54.000000 dataset-tools-0.0.7/dataset_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 10:14:54.000000 dataset-tools-0.0.7/dataset_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:14:54.000000 dataset-tools-0.0.7/dataset_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-17 10:14:54.000000 dataset-tools-0.0.7/dataset_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 10:14:54.000000 dataset-tools-0.0.7/dataset_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:14:54.056050 dataset-tools-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-17 10:12:11.000000 dataset-tools-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.428417 dataset-tools-0.0.8/dataset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools/image/renders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/poster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/separated_anns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/renders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools/image/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/basestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/class_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/class_cooccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/classes_per_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/heatmaps_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/object_and_class_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/objects_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/dataset_tools/image/stats/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/dataset_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 10:26:01.000000 dataset-tools-0.0.8/dataset_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:26:01.432417 dataset-tools-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-17 10:23:16.000000 dataset-tools-0.0.8/setup.py
```

### Comparing `dataset-tools-0.0.7/LICENSE` & `dataset-tools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/PKG-INFO` & `dataset-tools-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.7/dataset_tools/__init__.py` & `dataset-tools-0.0.8/dataset_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/renders/poster.py` & `dataset-tools-0.0.8/dataset_tools/image/renders/poster.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import random
 from typing import List, Union
 
 import cv2
 import numpy as np
-from dotenv import load_dotenv
+from PIL import Image, ImageDraw
 from tqdm import tqdm
 
 import supervisely as sly
 from supervisely.imaging import font as sly_font
 
 
 class Poster:
@@ -57,14 +57,16 @@
         self._size_line_2 = (
             (self._size[0] - 3 * self._GAP) // 5 * 2,
             (self._size[1] - 5 * self._GAP) // 4,
         )
 
         self._poster = np.ones((*self._size, 4), dtype=np.uint8) * 255  # result poster
 
+        self._logo_text = "logo.png"
+
     def update(self, data: tuple):
         np_images = []
         join_data = [(ds, img, ann) for ds, list1, list2 in data for img, ann in zip(list1, list2)]
         random.shuffle(join_data)
         i = 0
         with tqdm(desc="Downloading 7 sample images.", total=7) as pbar:
             while len(np_images) < 7:
@@ -94,14 +96,15 @@
                 np_images.append(np_img)
                 i += 1
                 pbar.update(1)
 
         self._resize_images(np_images)
         self._create_frame(np_images)
         self._draw_text_and_bboxes()
+        self._put_watermark(self._logo_text)
 
     def to_image(self, path: str = None):
         if path is None:
             storage_dir = sly.app.get_data_dir()
             sly.fs.clean_dir(storage_dir)
             path = os.path.join(storage_dir, "poster.jpeg")
         sly.image.write(path, self._poster)
@@ -216,7 +219,37 @@
 
         y = y_end + self._GAP
         x = self._GAP
         for img in images[3:]:
             x_end, y_end = x + img.shape[1], y + img.shape[0]
             self._poster[y:y_end, x:x_end] = img
             x = x_end + self._GAP
+
+    def _put_watermark(self, path):
+        img = sly.image.read(path)
+        poster_h, poster_w = self._size
+
+        # resize logo to poster size
+        mark_w = int(self._size_line_2[0] * 0.9)
+        mark_h = mark_w * img.shape[0] // img.shape[1]
+        img = cv2.resize(img, (mark_w, mark_h), interpolation=cv2.INTER_NEAREST)
+        # img = sly.image.resize_inter_nearest(img, (mark_h, mark_w))
+        img_h, img_w = img.shape[:2]
+
+        # calculate coords
+        offset_x = (self._size_line_2[1] - img_w) // 2
+        x = 3 * self._size_line_2[1] + 4 * self._GAP + offset_x
+        y = int(poster_h - 1.2 * self._GAP - img_h)
+
+        # add logo
+        logo = np.zeros((poster_h, poster_w, 4), dtype=np.uint8)
+        logo[y : y + img_h, x : x + img.shape[1], :3] = img[:, :, :3]
+        logo[y : y + img_h, x : x + img.shape[1], 3] = 255
+
+        self._poster = cv2.addWeighted(self._poster, 0.9, logo, 0.5, 0)
+
+        # or
+        # background = Image.fromarray(self._poster, mode="RGBA")
+        # overlay = Image.fromarray(logo, mode="RGBA")
+        # overlay = overlay.resize(background.size)
+        # new_image = Image.blend(background, overlay, alpha=0.15)
+        # self._poster = np.array(new_image, dtype=np.uint8)
```

### Comparing `dataset-tools-0.0.7/dataset_tools/image/renders/previews.py` & `dataset-tools-0.0.8/dataset_tools/image/renders/previews.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/renders/separated_anns_grid.py` & `dataset-tools-0.0.8/dataset_tools/image/renders/separated_anns_grid.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/renders/wrapper.py` & `dataset-tools-0.0.8/dataset_tools/image/renders/wrapper.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/basestats.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/basestats.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/class_balance.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/class_balance.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,19 @@
         }
         colomns_options[4] = {
             "postfix": "%",
             "maxValue": round(max(notnonearea), 2),
             "subtitle": "average",
             "tooltip": "Average image area of corresponding class. Images without such objects are not taking into account",
         }
-        options = {"fixColumns": 1, "sort": {"columnIndex": 1, "order": "desc"}}  # asc
+        options = {
+            "fixColumns": 1,
+            "sort": {"columnIndex": 1, "order": "desc"},
+            "pageSize": len(self._class_names),
+        }  # asc
 
         res = {
             "columns": columns,
             "data": rows,
             "referencesRow": self._stats["image_counts_filter_by_id"],
             "options": options,
             "columnsOptions": colomns_options,
```

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/class_cooccurrence.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/class_cooccurrence.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/classes_per_image.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/classes_per_image.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/heatmaps_for_classes.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/heatmaps_for_classes.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/object_and_class_sizes.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/object_and_class_sizes.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/objects_distribution.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/objects_distribution.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools/image/stats/wrapper.py` & `dataset-tools-0.0.8/dataset_tools/image/stats/wrapper.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools.egg-info/PKG-INFO` & `dataset-tools-0.0.8/dataset_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.7/dataset_tools.egg-info/SOURCES.txt` & `dataset-tools-0.0.8/dataset_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/dataset_tools.egg-info/requires.txt` & `dataset-tools-0.0.8/dataset_tools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.7/setup.py` & `dataset-tools-0.0.8/setup.py`

 * *Files identical despite different names*

