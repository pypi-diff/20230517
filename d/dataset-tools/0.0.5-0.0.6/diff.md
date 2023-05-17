# Comparing `tmp/dataset-tools-0.0.5.tar.gz` & `tmp/dataset-tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-tools-0.0.5.tar", last modified: Tue May 16 17:55:00 2023, max compression
+gzip compressed data, was "dataset-tools-0.0.6.tar", last modified: Wed May 17 08:11:59 2023, max compression
```

## Comparing `dataset-tools-0.0.5.tar` & `dataset-tools-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.185549 dataset-tools-0.0.5/dataset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.185549 dataset-tools-0.0.5/dataset_tools/image/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/dataset_tools/image/renders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/poster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/separated_anns_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/dataset_tools/image/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/basestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/class_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/class_cooccurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/classes_per_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/heatmaps_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/object_and_class_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/objects_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.185549 dataset-tools-0.0.5/dataset_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:59.468696 dataset-tools-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 08:11:59.468696 dataset-tools-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:59.464695 dataset-tools-0.0.6/dataset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:59.468696 dataset-tools-0.0.6/dataset_tools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:59.468696 dataset-tools-0.0.6/dataset_tools/image/renders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/renders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/renders/poster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/renders/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/renders/separated_anns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/renders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:59.468696 dataset-tools-0.0.6/dataset_tools/image/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/basestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/class_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/class_cooccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/classes_per_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/heatmaps_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/object_and_class_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/objects_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/dataset_tools/image/stats/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:11:59.468696 dataset-tools-0.0.6/dataset_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 08:11:59.000000 dataset-tools-0.0.6/dataset_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 08:11:59.000000 dataset-tools-0.0.6/dataset_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:11:59.000000 dataset-tools-0.0.6/dataset_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-17 08:11:59.000000 dataset-tools-0.0.6/dataset_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 08:11:59.000000 dataset-tools-0.0.6/dataset_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 08:11:59.468696 dataset-tools-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-17 08:09:10.000000 dataset-tools-0.0.6/setup.py
```

### Comparing `dataset-tools-0.0.5/LICENSE` & `dataset-tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.5/PKG-INFO` & `dataset-tools-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.5/dataset_tools/__init__.py` & `dataset-tools-0.0.6/dataset_tools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 from dataset_tools.image.stats.object_and_class_sizes import ObjectSizes, ClassSizes
 
 from dataset_tools.image.stats.wrapper import count_stats  # , initialize
 
 
 from dataset_tools.image.renders.wrapper import prepare_renders
 from dataset_tools.image.renders.separated_anns_grid import SideAnnotationsGrid
+from dataset_tools.image.renders.poster import Poster
```

### Comparing `dataset-tools-0.0.5/dataset_tools/image/renders/previews.py` & `dataset-tools-0.0.6/dataset_tools/image/renders/previews.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.5/dataset_tools/image/renders/separated_anns_grid.py` & `dataset-tools-0.0.6/dataset_tools/image/renders/separated_anns_grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import os
 import random
+from typing import Union
 
 import numpy as np
-from dotenv import load_dotenv
 from tqdm import tqdm
 
 import supervisely as sly
 
 
 class SideAnnotationsGrid:
-    def __init__(self, project_meta: sly.ProjectMeta, api: sly.Api = None, rows: int = 3, cols: int = 3):
+    def __init__(
+        self,
+        project: Union[str, int],
+        project_meta: sly.ProjectMeta,
+        api: sly.Api = None,
+        rows: int = 3,
+        cols: int = 3,
+    ):
         self.project_meta = project_meta
 
         self._max_size = 1920
         self._rows = rows
         self._cols = cols
         self._aspect_ratio = 9 / 16
 
@@ -23,31 +30,31 @@
 
         self._all_image_infos = []
         self._all_anns = []
         self.np_images = []
         self.original_masks = []
         self._grid = None
 
+        self._local = False if isinstance(project, int) else True
         self._api = api if api is not None else sly.Api.from_env()
 
     def update(self, data: tuple):
         cnt = self._cols * self._rows
-        temp_imgs = []
-        temp_anns = []
-        for dataset_id, image_infos, anns in data:
-            temp_imgs.extend(image_infos)
-            temp_anns.extend(anns)
-        temp_data = list(zip(temp_imgs, temp_anns))
+        join_data = [(ds, img, ann) for ds, list1, list2 in data for img, ann in zip(list1, list2)]
 
-        random.shuffle(temp_data)
+        random.shuffle(join_data)
         with tqdm(desc="Downloading images", total=cnt) as p:
-            for img_info, ann in temp_data[:cnt]:
+            for ds, img_info, ann in join_data[:cnt]:
                 self._all_image_infos.append(img_info)
                 self._all_anns.append(ann)
-                self.np_images.append(self._api.image.download_np(img_info.id))
+                self.np_images.append(
+                    sly.image.read(ds.get_img_path(img_info.name))
+                    if self._local
+                    else self._api.image.download_np(img_info.id)
+                )
                 p.update(1)
 
                 self.original_masks.append(self._draw_masks_on_single_image(ann, img_info))
 
         resized_images = self._resize_images(self.np_images)
         resized_masks = self._resize_images(self.original_masks)
 
@@ -131,44 +138,7 @@
         )
         for idx in range(num):
             x = (idx % (self._cols * 2)) * img_w
             y = (idx // (self._cols * 2)) * img_h
             grid[y : y + img_h, x : x + img_w, ...] = images[idx][:, :, ...]
 
         return grid
-
-
-###########################################################################
-############################# for local debug #############################
-###########################################################################
-
-# if sly.is_development():
-#     load_dotenv(os.path.expanduser("~/ninja.env"))
-#     load_dotenv("local.env")
-
-# project_id = sly.env.project_id(raise_not_found=False)
-
-# api = sly.Api.from_env()
-
-# project_meta = sly.ProjectMeta.from_json(api.project.get_meta(project_id))
-# grid = SideAnnotationsGrid(project_meta=project_meta, rows=5, cols=2)
-
-# limit = 30
-# samples = []
-# for dataset in api.dataset.get_list(project_id):
-#     ds_images = api.image.get_list(
-#         dataset.id,
-#         filters=[{"field": "labelsCount", "operator": ">", "value": "0"}],
-#     )
-#     if len(ds_images) == 0:
-#         continue
-#     sample_image_infos = random.sample(ds_images, limit)
-#     ds_anns_infos = api.annotation.download_json_batch(
-#         dataset.id, [s.id for s in sample_image_infos]
-#     )
-#     ds_anns = [sly.Annotation.from_json(a, project_meta) for a in ds_anns_infos]
-#     samples.append((dataset.id, sample_image_infos, ds_anns))
-
-# # for dataset_id, ds_images, ds_anns in samples:
-# grid.update(samples)
-
-# grid.to_image("/tmp/grid.png")
```

### Comparing `dataset-tools-0.0.5/dataset_tools/image/stats/basestats.py` & `dataset-tools-0.0.6/dataset_tools/image/stats/basestats.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.5/dataset_tools/image/stats/class_balance.py` & `dataset-tools-0.0.6/dataset_tools/image/stats/class_balance.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 UNLABELED_COLOR = [0, 0, 0]
 
 
 class ClassBalance(BaseStats):
     """
     Columns:
-        class,
-        images,
-        objects,
-        avg count per image,
-        avg area per image,
+        class name
+        images
+        objects
+        avg count per image
+        avg area per image
     """
 
     def __init__(self, project_meta: sly.ProjectMeta) -> None:
         self._meta = project_meta
         self._stats = {}
 
         self._class_names = ["unlabeled"]
@@ -94,15 +94,21 @@
 
             # TODO: implement later
             # if stat_count[class_name] > 0:
             # obj_ids = [obj[0] for obj in ann_objects if obj[1] == class_name]
             # self._stats["object_counts_filter_by_id"][idx].extend(obj_ids)
 
     def to_json(self) -> dict:
-        columns = ["class", "images", "objects", "avg count per image", "avg area per image"]
+        columns = [
+            "class name",
+            "num images",
+            "num objects",
+            "avg count per image",
+            "avg area per image",
+        ]
         rows = []
         for name, idx in self._name_to_index.items():
             rows.append(
                 [
                     name,
                     self._stats["images_count"][idx],
                     self._stats["objects_count"][idx],
```

### Comparing `dataset-tools-0.0.5/dataset_tools/image/stats/class_cooccurrence.py` & `dataset-tools-0.0.6/dataset_tools/image/stats/class_cooccurrence.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 
 from dataset_tools.image.stats.basestats import BaseStats
 from supervisely.app.widgets import ConfusionMatrix
 
 
 class ClassCooccurrence(BaseStats):
     """
-    Classes co-occurrence matrix.
-    Column names depends on the number of classes
+    Columns:
+        class name
+        class 1
+        class 2
+        etc.
     """
 
     def __init__(self, project_meta: sly.ProjectMeta) -> None:
         self._meta = project_meta
         self._stats = {}
 
         self._class_names = [cls.name for cls in project_meta.obj_classes]
@@ -63,15 +66,15 @@
 
         data = [
             [value] + sublist
             for value, sublist in zip(self._class_names, self.co_occurrence_matrix.tolist())
         ]
 
         res = {
-            "columns": ["class"] + self._class_names,
+            "columns": ["class name"] + self._class_names,
             "data": data,
             "referencesRow": self._references,
             "options": options,
             "colomnsOptions": colomns_options,
         }
         return res
```

### Comparing `dataset-tools-0.0.5/dataset_tools/image/stats/classes_per_image.py` & `dataset-tools-0.0.6/dataset_tools/image/stats/classes_per_image.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.5/dataset_tools/image/stats/heatmaps_for_classes.py` & `dataset-tools-0.0.6/dataset_tools/image/stats/heatmaps_for_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import cv2
 import math
 import supervisely as sly
 from skimage.transform import resize
 
 
 class ClassesHeatmaps:
+    """
+    Get heatmap of visual density of aggregated annotations for every class
+    """
+
     def __init__(self, project_meta: sly.ProjectMeta, heatmap_img_size: tuple = None):
         self._meta = project_meta
         self.classname_heatmap = {}
         self._ds_image_sizes = []
         self.heatmap_image_paths = []
 
         if heatmap_img_size:
```

### Comparing `dataset-tools-0.0.5/dataset_tools/image/stats/object_and_class_sizes.py` & `dataset-tools-0.0.6/dataset_tools/image/stats/object_and_class_sizes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 from collections import defaultdict
-from dataset_tools.image.stats.basestats import BaseStats
 
-import pandas as pd
 import supervisely as sly
 
+from dataset_tools.image.stats.basestats import BaseStats
+
 
 class ObjectSizes(BaseStats):
+    """
+    Columns:
+        Class name
+        Dataset ID
+        Image name
+        Image size
+        Height px
+        Height %
+        Width px
+        Width %
+        Area px
+        Area %
+    """
+
     def __init__(self, project_meta: sly.ProjectMeta):
         self.project_meta = project_meta
         self._stats = []
 
     def update(self, image: sly.ImageInfo, ann: sly.Annotation):
         image_height, image_width = ann.img_size
 
         for label in ann.labels:
             if type(label.geometry) not in [sly.Bitmap, sly.Rectangle, sly.Polygon]:
                 continue
 
             object_data = {
                 "class_name": label.obj_class.name,
+                "dataset_id": image.dataset_id,
                 "image_name": image.name,
                 "image_size_hw": f"{image_height}x{image_width}",
             }
 
             object_data.update(calculate_obj_sizes(label, image_height, image_width))
 
             object_data = list(object_data.values())
@@ -31,27 +46,29 @@
 
     def to_json(self):
         options = {"fixColumns": 1}
 
         res = {
             "columns": [
                 "Class name",
+                "Dataset ID",
                 "Image name",
                 "Image size",
                 "Height",
                 "Height",
                 "Width",
                 "Width",
                 "Area",
                 "Area",
             ],
             "columnsOptions": [
                 {},
                 {},
                 {},
+                {},
                 {"postfix": "px"},
                 {"postfix": "%"},
                 {"postfix": "px"},
                 {"postfix": "%"},
                 {"postfix": "px"},
                 {"postfix": "%"},
             ],
@@ -59,101 +76,125 @@
             "options": options,
         }
 
         return res
 
 
 class ClassSizes(BaseStats):
+    """
+    Columns:
+        Class name
+        Object count
+        Min height px
+        Min height %
+        Max height px
+        Max height %
+        Avg height px
+        Avg height %
+        Min width px
+        Min width %
+        Max width px
+        Max width %
+        Avg width px
+        Avg width %
+        Min area px
+        Min area %
+        Max area px
+        Max area %
+        Avg area px
+        Avg area %
+    """
+
     def __init__(self, project_meta):
         self.project_meta = project_meta
         self._class_titles = [obj_class.name for obj_class in project_meta.obj_classes]
 
         self._stats = []
-
-        self._class_heights_px = defaultdict(list)
-        self._class_heights_pc = defaultdict(list)
-        self._class_widths_px = defaultdict(list)
-        self._class_widths_pc = defaultdict(list)
-        self._class_areas_px = defaultdict(list)
-        self._class_areas_pc = defaultdict(list)
-        self._class_object_counts = defaultdict(int)
+        self._data = []
 
     def update(self, image: sly.ImageInfo, ann: sly.Annotation):
-        image_height, image_width = ann.img_size
-        for label in ann.labels:
-            if type(label.geometry) not in [sly.Bitmap, sly.Rectangle, sly.Polygon]:
-                continue
-
-            self._class_object_counts[label.obj_class.name] += 1
+        self._data.append(ann)
 
-            obj_sizes = calculate_obj_sizes(label, image_height, image_width)
-
-            self._class_heights_px[label.obj_class.name].append(obj_sizes["height_px"])
-            self._class_heights_pc[label.obj_class.name].append(obj_sizes["height_pc"])
-            self._class_widths_px[label.obj_class.name].append(obj_sizes["width_px"])
-            self._class_widths_pc[label.obj_class.name].append(obj_sizes["width_pc"])
-            self._class_areas_px[label.obj_class.name].append(obj_sizes["area_px"])
-            self._class_areas_pc[label.obj_class.name].append(obj_sizes["area_pc"])
+    def to_json(self):
+        class_heights_px = defaultdict(list)
+        class_heights_pc = defaultdict(list)
+        class_widths_px = defaultdict(list)
+        class_widths_pc = defaultdict(list)
+        class_areas_px = defaultdict(list)
+        class_areas_pc = defaultdict(list)
+        class_object_counts = defaultdict(int)
+
+        for ann in self._data:
+            image_height, image_width = ann.img_size
+            for label in ann.labels:
+                if type(label.geometry) not in [sly.Bitmap, sly.Rectangle, sly.Polygon]:
+                    continue
+
+                class_object_counts[label.obj_class.name] += 1
+
+                obj_sizes = calculate_obj_sizes(label, image_height, image_width)
+
+                class_heights_px[label.obj_class.name].append(obj_sizes["height_px"])
+                class_heights_pc[label.obj_class.name].append(obj_sizes["height_pc"])
+                class_widths_px[label.obj_class.name].append(obj_sizes["width_px"])
+                class_widths_pc[label.obj_class.name].append(obj_sizes["width_pc"])
+                class_areas_px[label.obj_class.name].append(obj_sizes["area_px"])
+                class_areas_pc[label.obj_class.name].append(obj_sizes["area_pc"])
 
         for class_title in self._class_titles:
-            object_count = self._class_object_counts[class_title]
+            object_count = class_object_counts[class_title]
 
             if object_count < 1:
                 continue
 
             class_data = {
                 "class_name": class_title,
                 "object_count": object_count,
-                "min_height_px": min(self._class_heights_px[class_title]),
-                "min_height_pc": min(self._class_heights_pc[class_title]),
-                "max_height_px": max(self._class_heights_px[class_title]),
-                "max_height_pc": max(self._class_heights_pc[class_title]),
+                "min_height_px": min(class_heights_px[class_title]),
+                "min_height_pc": min(class_heights_pc[class_title]),
+                "max_height_px": max(class_heights_px[class_title]),
+                "max_height_pc": max(class_heights_pc[class_title]),
                 "avg_height_px": round(
-                    sum(self._class_heights_px[class_title])
-                    / len(self._class_heights_px[class_title]),
+                    sum(class_heights_px[class_title]) / len(class_heights_px[class_title]),
                     2,
                 ),
                 "avg_height_pc": round(
-                    sum(self._class_heights_pc[class_title])
-                    / len(self._class_heights_pc[class_title]),
+                    sum(class_heights_pc[class_title]) / len(class_heights_pc[class_title]),
                     2,
                 ),
-                "min_width_px": min(self._class_widths_px[class_title]),
-                "min_width_pc": min(self._class_widths_pc[class_title]),
-                "max_width_px": max(self._class_widths_px[class_title]),
-                "max_width_pc": max(self._class_widths_pc[class_title]),
+                "min_width_px": min(class_widths_px[class_title]),
+                "min_width_pc": min(class_widths_pc[class_title]),
+                "max_width_px": max(class_widths_px[class_title]),
+                "max_width_pc": max(class_widths_pc[class_title]),
                 "avg_width_px": round(
-                    sum(self._class_widths_px[class_title])
-                    / len(self._class_widths_px[class_title]),
+                    sum(class_widths_px[class_title]) / len(class_widths_px[class_title]),
                     2,
                 ),
                 "avg_width_pc": round(
-                    sum(self._class_widths_pc[class_title])
-                    / len(self._class_widths_pc[class_title]),
+                    sum(class_widths_pc[class_title]) / len(class_widths_pc[class_title]),
                     2,
                 ),
-                "min_area_px": min(self._class_areas_px[class_title]),
-                "min_area_pc": min(self._class_areas_pc[class_title]),
-                "max_area_px": max(self._class_areas_px[class_title]),
-                "max_area_pc": max(self._class_areas_pc[class_title]),
+                "min_area_px": min(class_areas_px[class_title]),
+                "min_area_pc": min(class_areas_pc[class_title]),
+                "max_area_px": max(class_areas_px[class_title]),
+                "max_area_pc": max(class_areas_pc[class_title]),
                 "avg_area_px": round(
-                    sum(self._class_areas_px[class_title]) / len(self._class_areas_px[class_title]),
+                    sum(class_areas_px[class_title]) / len(class_areas_px[class_title]),
                     2,
                 ),
                 "avg_area_pc": round(
-                    sum(self._class_areas_pc[class_title]) / len(self._class_areas_pc[class_title]),
+                    sum(class_areas_pc[class_title]) / len(class_areas_pc[class_title]),
                     2,
                 ),
             }
 
             class_data = list(class_data.values())
 
             self._stats.append(class_data)
 
-    def to_json(self):
         options = {"fixColumns": 1}
 
         res = {
             "columns": [
                 "Class name",
                 "Object count",
                 "Min height",
```

### Comparing `dataset-tools-0.0.5/dataset_tools/image/stats/wrapper.py` & `dataset-tools-0.0.6/dataset_tools/image/stats/wrapper.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.5/dataset_tools.egg-info/PKG-INFO` & `dataset-tools-0.0.6/dataset_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.5/dataset_tools.egg-info/SOURCES.txt` & `dataset-tools-0.0.6/dataset_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.5/dataset_tools.egg-info/requires.txt` & `dataset-tools-0.0.6/dataset_tools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.5/setup.py` & `dataset-tools-0.0.6/setup.py`

 * *Files identical despite different names*

