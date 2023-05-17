# Comparing `tmp/saldet-0.5.2.tar.gz` & `tmp/saldet-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saldet-0.5.2.tar", max compression
+gzip compressed data, was "saldet-0.5.3.tar", max compression
```

## Comparing `saldet-0.5.2.tar` & `saldet-0.5.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.2/LICENSE
--rw-r--r--   0        0        0     3440 2023-05-11 09:22:36.999483 saldet-0.5.2/README.md
--rw-r--r--   0        0        0      917 2023-05-17 16:12:22.485605 saldet-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-17 16:09:47.322673 saldet-0.5.2/saldet/__init__.py
--rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.2/saldet/dataset/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.2/saldet/dataset/inference.py
--rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.2/saldet/dataset/saliency.py
--rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.2/saldet/experiment/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-17 16:13:05.313542 saldet-0.5.2/saldet/experiment/inference.py
--rw-r--r--   0        0        0     2312 2023-05-17 16:10:40.783399 saldet-0.5.2/saldet/experiment/train.py
--rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.2/saldet/io/__init__.py
--rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.2/saldet/io/config.py
--rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.2/saldet/io/image.py
--rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.2/saldet/loss/__init__.py
--rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.2/saldet/loss/_factory.py
--rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.2/saldet/loss/attn_guided.py
--rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.2/saldet/loss/bce_iou_loss.py
--rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.5.2/saldet/loss/multi_bce.py
--rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.5.2/saldet/loss/pg.py
--rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.2/saldet/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.2/saldet/lr_scheduler/lr_scheduler.py
--rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.5.2/saldet/model/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-11 09:14:45.294803 saldet-0.5.2/saldet/model/_factory.py
--rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.2/saldet/model/models/__init__.py
--rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.2/saldet/model/models/pgnet.py
--rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.2/saldet/model/models/resnet.py
--rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.2/saldet/model/models/swin.py
--rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.2/saldet/model/models/u2net.py
--rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.2/saldet/ops/__init__.py
--rw-r--r--   0        0        0      930 2023-05-17 15:23:24.394224 saldet-0.5.2/saldet/ops/tensor.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.2/saldet/optimizer/__init__.py
--rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.2/saldet/optimizer/optimizer.py
--rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.2/saldet/pl/__init__.py
--rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.2/saldet/pl/data.py
--rw-r--r--   0        0        0     2370 2023-05-16 13:40:17.705235 saldet-0.5.2/saldet/pl/model.py
--rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.2/saldet/plot/__init__.py
--rw-r--r--   0        0        0     2525 2023-05-17 16:10:06.920896 saldet-0.5.2/saldet/plot/plot.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.2/saldet/trainer/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.2/saldet/trainer/callbacks.py
--rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.2/saldet/transform/__init__.py
--rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.2/saldet/transform/transform.py
--rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.2/saldet/utils/__init__.py
--rw-r--r--   0        0        0      225 2023-05-11 09:34:56.451378 saldet-0.5.2/saldet/utils/device.py
--rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.2/saldet/utils/time.py
--rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 saldet-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3440 2023-05-11 09:22:36.999483 saldet-0.5.3/README.md
+-rw-r--r--   0        0        0      917 2023-05-17 16:47:15.304311 saldet-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-05-17 16:46:33.081338 saldet-0.5.3/saldet/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.3/saldet/dataset/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.3/saldet/dataset/inference.py
+-rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.3/saldet/dataset/saliency.py
+-rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.3/saldet/experiment/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-17 16:13:05.313542 saldet-0.5.3/saldet/experiment/inference.py
+-rw-r--r--   0        0        0     2312 2023-05-17 16:10:40.783399 saldet-0.5.3/saldet/experiment/train.py
+-rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.3/saldet/io/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.3/saldet/io/config.py
+-rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.3/saldet/io/image.py
+-rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.3/saldet/loss/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.3/saldet/loss/_factory.py
+-rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.3/saldet/loss/attn_guided.py
+-rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.3/saldet/loss/bce_iou_loss.py
+-rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.5.3/saldet/loss/multi_bce.py
+-rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.5.3/saldet/loss/pg.py
+-rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.3/saldet/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.3/saldet/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.5.3/saldet/model/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-11 09:14:45.294803 saldet-0.5.3/saldet/model/_factory.py
+-rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.3/saldet/model/models/__init__.py
+-rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.3/saldet/model/models/pgnet.py
+-rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.3/saldet/model/models/resnet.py
+-rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.3/saldet/model/models/swin.py
+-rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.3/saldet/model/models/u2net.py
+-rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.3/saldet/ops/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-17 15:23:24.394224 saldet-0.5.3/saldet/ops/tensor.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.3/saldet/optimizer/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.3/saldet/optimizer/optimizer.py
+-rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.3/saldet/pl/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.3/saldet/pl/data.py
+-rw-r--r--   0        0        0     2370 2023-05-16 13:40:17.705235 saldet-0.5.3/saldet/pl/model.py
+-rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.3/saldet/plot/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-17 16:46:33.116615 saldet-0.5.3/saldet/plot/plot.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.3/saldet/trainer/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.3/saldet/trainer/callbacks.py
+-rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.3/saldet/transform/__init__.py
+-rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.3/saldet/transform/transform.py
+-rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.3/saldet/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-11 09:34:56.451378 saldet-0.5.3/saldet/utils/device.py
+-rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.3/saldet/utils/time.py
+-rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 saldet-0.5.3/PKG-INFO
```

### Comparing `saldet-0.5.2/LICENSE` & `saldet-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/README.md` & `saldet-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/pyproject.toml` & `saldet-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saldet"
-version = "0.5.2"
+version = "0.5.3"
 description = "Saliency Detection library (models, loss, utils) with PyTorch"
 authors = ["Riccardo Musmeci"]
 repository = "https://github.com/riccardomusmeci/saldet"
 license = "MIT"
 readme = "README.md"
 keywords = ["computer vision", "saliency detection"]
```

### Comparing `saldet-0.5.2/saldet/dataset/inference.py` & `saldet-0.5.3/saldet/dataset/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/dataset/saliency.py` & `saldet-0.5.3/saldet/dataset/saliency.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/experiment/inference.py` & `saldet-0.5.3/saldet/experiment/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/experiment/train.py` & `saldet-0.5.3/saldet/experiment/train.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/io/image.py` & `saldet-0.5.3/saldet/io/image.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/loss/attn_guided.py` & `saldet-0.5.3/saldet/loss/attn_guided.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/loss/bce_iou_loss.py` & `saldet-0.5.3/saldet/loss/bce_iou_loss.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/loss/multi_bce.py` & `saldet-0.5.3/saldet/loss/multi_bce.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/loss/pg.py` & `saldet-0.5.3/saldet/loss/pg.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/lr_scheduler/lr_scheduler.py` & `saldet-0.5.3/saldet/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/model/_factory.py` & `saldet-0.5.3/saldet/model/_factory.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/model/models/pgnet.py` & `saldet-0.5.3/saldet/model/models/pgnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/model/models/resnet.py` & `saldet-0.5.3/saldet/model/models/resnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/model/models/swin.py` & `saldet-0.5.3/saldet/model/models/swin.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/model/models/u2net.py` & `saldet-0.5.3/saldet/model/models/u2net.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/ops/tensor.py` & `saldet-0.5.3/saldet/ops/tensor.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/optimizer/optimizer.py` & `saldet-0.5.3/saldet/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/pl/data.py` & `saldet-0.5.3/saldet/pl/data.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/pl/model.py` & `saldet-0.5.3/saldet/pl/model.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/plot/plot.py` & `saldet-0.5.3/saldet/plot/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 
 
 def apply_mask(image: np.array, mask: np.array, alpha: float = 1.0) -> np.array:
     """Apply segmentation masks to an image
 
     Args:
         image (np.array): image to be blended with the mask.
-        mask (np.array): mask to be blended with the image.
+        mask (np.array): binary mask to be blended with the image.
         alpha (float): relative weight of the mask, 1.0 means no transparency, 0.0 means the mask is completely transparent.
             Defaults to 1.0.
 
     Returns:
         np.array: image with masks applied
     """
+
+    assert np.unique(mask).shape[0] <= 2, "Mask must be binary"
     out = image.copy()
     cmap = plt.cm.tab10
     for cat_id in np.unique(mask)[1:]:
         bool_mask = mask == cat_id
         color = np.array(cmap(cat_id - 1)[:3]) * 255
         cat_mask = (np.expand_dims(mask, axis=2) * color)[bool_mask].astype(np.uint8)
         out[bool_mask] = cv2.addWeighted(
```

### Comparing `saldet-0.5.2/saldet/trainer/callbacks.py` & `saldet-0.5.3/saldet/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/saldet/transform/transform.py` & `saldet-0.5.3/saldet/transform/transform.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.2/PKG-INFO` & `saldet-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saldet
-Version: 0.5.2
+Version: 0.5.3
 Summary: Saliency Detection library (models, loss, utils) with PyTorch
 Home-page: https://github.com/riccardomusmeci/saldet
 License: MIT
 Keywords: computer vision,saliency detection
 Author: Riccardo Musmeci
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

