# Comparing `tmp/saldet-0.5.1.tar.gz` & `tmp/saldet-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saldet-0.5.1.tar", max compression
+gzip compressed data, was "saldet-0.5.2.tar", max compression
```

## Comparing `saldet-0.5.1.tar` & `saldet-0.5.2.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.1/LICENSE
--rw-r--r--   0        0        0     3421 2023-05-11 09:18:21.911295 saldet-0.5.1/README.md
--rw-r--r--   0        0        0      917 2023-05-11 09:16:02.815493 saldet-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-05-11 09:14:44.361117 saldet-0.5.1/saldet/__init__.py
--rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.1/saldet/dataset/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.1/saldet/dataset/inference.py
--rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.1/saldet/dataset/saliency.py
--rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.1/saldet/experiment/__init__.py
--rw-r--r--   0        0        0     2915 2023-05-11 09:06:14.061549 saldet-0.5.1/saldet/experiment/inference.py
--rw-r--r--   0        0        0     2312 2023-05-10 20:46:44.791975 saldet-0.5.1/saldet/experiment/train.py
--rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.1/saldet/io/__init__.py
--rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.1/saldet/io/config.py
--rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.1/saldet/io/image.py
--rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.1/saldet/loss/__init__.py
--rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.1/saldet/loss/_factory.py
--rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.1/saldet/loss/attn_guided.py
--rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.1/saldet/loss/bce_iou_loss.py
--rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.5.1/saldet/loss/multi_bce.py
--rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.5.1/saldet/loss/pg.py
--rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.1/saldet/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.1/saldet/lr_scheduler/lr_scheduler.py
--rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.5.1/saldet/model/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-11 09:14:45.294803 saldet-0.5.1/saldet/model/_factory.py
--rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.1/saldet/model/models/__init__.py
--rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.1/saldet/model/models/pgnet.py
--rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.1/saldet/model/models/resnet.py
--rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.1/saldet/model/models/swin.py
--rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.1/saldet/model/models/u2net.py
--rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.1/saldet/ops/__init__.py
--rw-r--r--   0        0        0      930 2023-05-10 20:47:50.389781 saldet-0.5.1/saldet/ops/tensor.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.1/saldet/optimizer/__init__.py
--rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.1/saldet/optimizer/optimizer.py
--rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.1/saldet/pl/__init__.py
--rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.1/saldet/pl/data.py
--rw-r--r--   0        0        0     2370 2023-05-10 21:13:19.786920 saldet-0.5.1/saldet/pl/model.py
--rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.1/saldet/plot/__init__.py
--rw-r--r--   0        0        0     2525 2023-05-11 09:06:14.062100 saldet-0.5.1/saldet/plot/plot.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.1/saldet/trainer/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.1/saldet/trainer/callbacks.py
--rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.1/saldet/transform/__init__.py
--rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.1/saldet/transform/transform.py
--rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.1/saldet/utils/__init__.py
--rw-r--r--   0        0        0      225 2023-05-10 17:16:58.601910 saldet-0.5.1/saldet/utils/device.py
--rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.1/saldet/utils/time.py
--rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 saldet-0.5.1/setup.py
--rw-r--r--   0        0        0     4499 1970-01-01 00:00:00.000000 saldet-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3440 2023-05-11 09:22:36.999483 saldet-0.5.2/README.md
+-rw-r--r--   0        0        0      917 2023-05-17 16:12:22.485605 saldet-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-17 16:09:47.322673 saldet-0.5.2/saldet/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.2/saldet/dataset/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.2/saldet/dataset/inference.py
+-rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.2/saldet/dataset/saliency.py
+-rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.2/saldet/experiment/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-17 16:13:05.313542 saldet-0.5.2/saldet/experiment/inference.py
+-rw-r--r--   0        0        0     2312 2023-05-17 16:10:40.783399 saldet-0.5.2/saldet/experiment/train.py
+-rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.2/saldet/io/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.2/saldet/io/config.py
+-rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.2/saldet/io/image.py
+-rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.2/saldet/loss/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.2/saldet/loss/_factory.py
+-rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.2/saldet/loss/attn_guided.py
+-rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.2/saldet/loss/bce_iou_loss.py
+-rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.5.2/saldet/loss/multi_bce.py
+-rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.5.2/saldet/loss/pg.py
+-rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.2/saldet/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.2/saldet/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.5.2/saldet/model/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-11 09:14:45.294803 saldet-0.5.2/saldet/model/_factory.py
+-rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.2/saldet/model/models/__init__.py
+-rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.2/saldet/model/models/pgnet.py
+-rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.2/saldet/model/models/resnet.py
+-rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.2/saldet/model/models/swin.py
+-rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.2/saldet/model/models/u2net.py
+-rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.2/saldet/ops/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-17 15:23:24.394224 saldet-0.5.2/saldet/ops/tensor.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.2/saldet/optimizer/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.2/saldet/optimizer/optimizer.py
+-rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.2/saldet/pl/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.2/saldet/pl/data.py
+-rw-r--r--   0        0        0     2370 2023-05-16 13:40:17.705235 saldet-0.5.2/saldet/pl/model.py
+-rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.2/saldet/plot/__init__.py
+-rw-r--r--   0        0        0     2525 2023-05-17 16:10:06.920896 saldet-0.5.2/saldet/plot/plot.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.2/saldet/trainer/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.2/saldet/trainer/callbacks.py
+-rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.2/saldet/transform/__init__.py
+-rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.2/saldet/transform/transform.py
+-rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.2/saldet/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-11 09:34:56.451378 saldet-0.5.2/saldet/utils/device.py
+-rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.2/saldet/utils/time.py
+-rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 saldet-0.5.2/PKG-INFO
```

### Comparing `saldet-0.5.1/LICENSE` & `saldet-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/README.md` & `saldet-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # saldet
-> **Sal**iency **Det**ection (*saldet*) is a collection of models and tools to perform Saliency Detection with PyTorch.
+> **Sal**iency **Det**ection (*saldet*) is a collection of models and tools to perform Saliency Detection with PyTorch (cuda, mps, etc.).
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Build Status][build-image]][build-url]
 [![Code Coverage][coverage-image]][coverage-url]
 
 <!-- Badges: -->
 
@@ -18,14 +18,15 @@
 List of saliency detection models supported by saldet:
 
 * U2Net - https://arxiv.org/abs/2005.09007v3
 * PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet's repo](https://github.com/iCVTEAM/PGNet))
 
 
 ## **Train**
+
 ### **Easy Mode**
 The library comes with easy access to train models thanks to the amazing PyTorch Lightning support. 
 
 ```python
 from saldet.experiment import train
 
 train(
```

### Comparing `saldet-0.5.1/pyproject.toml` & `saldet-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saldet"
-version = "0.5.1"
+version = "0.5.2"
 description = "Saliency Detection library (models, loss, utils) with PyTorch"
 authors = ["Riccardo Musmeci"]
 repository = "https://github.com/riccardomusmeci/saldet"
 license = "MIT"
 readme = "README.md"
 keywords = ["computer vision", "saliency detection"]
```

### Comparing `saldet-0.5.1/saldet/dataset/inference.py` & `saldet-0.5.2/saldet/dataset/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/dataset/saliency.py` & `saldet-0.5.2/saldet/dataset/saliency.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/experiment/inference.py` & `saldet-0.5.2/saldet/experiment/inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,28 +16,26 @@
 
 
 def inference(
     images_dir: Path,
     config_path: Path,
     ckpt: Path,
     output_dir: Path,
-    normalize: bool = True,
     resize_to_original: bool = True,
-    threshold: float = 0.5,
+    threshold: float = None,
 ):
     """Inference entry point - create saliency maps and save them all in an output dir
 
     Args:
         images_dir (Path): path to folder with images
         config_path (Path): path to saldet configuration file
         ckpt (Path): path to model ckpt (.pth or .ckpt from pytorch_lightning)
         output_dir (Path): path to output dir where saliency maps will be saved
-        normalize (bool, optional): if True, normalizes saliency maps. Defaults to True.
         resize_to_original (bool, optional): if True, resize_to_original saliency maps. Defaults to True.
-        threshold (float, optional): if True, applies a threshold to saliency maps to be binary saliency maps. Defaults to .5.
+        threshold (float, optional): if True, applies a threshold to saliency maps to generate binary saliency maps. Defaults to None.
     """
     config = load_config(path=config_path)
 
     model = load_checkpoint(ckpt=ckpt, model_name=config["model"]["model_name"])
 
     os.makedirs(output_dir, exist_ok=True)
     print(f"> Loading images dataset")
@@ -55,23 +53,25 @@
             enumerate(data_loader), total=len(data_loader), desc="Inference"
         ):
             x, image_path = batch
             x = x.to(device())
             preds = model(x)
             if hasattr(preds, "__iter__"):
                 preds = preds[0]
-            if normalize:
-                preds = ops.normalize(preds)
+            preds = torch.sigmoid(preds)
             if resize_to_original:
                 w, h = Image.open(image_path[0]).size
                 preds = F.interpolate(preds, size=(h, w), mode="bilinear")
             for pred, image_path in zip(preds, image_path):
                 image_name = os.path.basename(image_path).split(".")[0]
                 file_path = os.path.join(output_dir, f"{image_name}.png")
-                pred = pred.squeeze().cpu().numpy()
+
                 if threshold is not None:
                     pred[pred >= threshold] = 255
                     pred[pred < threshold] = 0
                 else:
                     pred *= 255
+
+                pred = pred.squeeze().cpu().numpy()
                 pred = Image.fromarray(pred).convert("L")
+
                 pred.save(file_path)
```

### Comparing `saldet-0.5.1/saldet/experiment/train.py` & `saldet-0.5.2/saldet/experiment/train.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/io/image.py` & `saldet-0.5.2/saldet/io/image.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/loss/attn_guided.py` & `saldet-0.5.2/saldet/loss/attn_guided.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/loss/bce_iou_loss.py` & `saldet-0.5.2/saldet/loss/bce_iou_loss.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/loss/multi_bce.py` & `saldet-0.5.2/saldet/loss/multi_bce.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/loss/pg.py` & `saldet-0.5.2/saldet/loss/pg.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/lr_scheduler/lr_scheduler.py` & `saldet-0.5.2/saldet/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/model/_factory.py` & `saldet-0.5.2/saldet/model/_factory.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/model/models/pgnet.py` & `saldet-0.5.2/saldet/model/models/pgnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/model/models/resnet.py` & `saldet-0.5.2/saldet/model/models/resnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/model/models/swin.py` & `saldet-0.5.2/saldet/model/models/swin.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/model/models/u2net.py` & `saldet-0.5.2/saldet/model/models/u2net.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/ops/tensor.py` & `saldet-0.5.2/saldet/ops/tensor.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/optimizer/optimizer.py` & `saldet-0.5.2/saldet/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/pl/data.py` & `saldet-0.5.2/saldet/pl/data.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/pl/model.py` & `saldet-0.5.2/saldet/pl/model.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/plot/plot.py` & `saldet-0.5.2/saldet/plot/plot.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/trainer/callbacks.py` & `saldet-0.5.2/saldet/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/saldet/transform/transform.py` & `saldet-0.5.2/saldet/transform/transform.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.1/setup.py` & `saldet-0.5.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,143 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: saldet
+Version: 0.5.2
+Summary: Saliency Detection library (models, loss, utils) with PyTorch
+Home-page: https://github.com/riccardomusmeci/saldet
+License: MIT
+Keywords: computer vision,saliency detection
+Author: Riccardo Musmeci
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: albumentations (>=1.3.0,<2.0.0)
+Requires-Dist: lightning-bolts (>=0.5.0,<0.6.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: timm (>=0.6.13,<0.7.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: torchvision (>=0.15.2,<0.16.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Repository, https://github.com/riccardomusmeci/saldet
+Description-Content-Type: text/markdown
+
+# saldet
+> **Sal**iency **Det**ection (*saldet*) is a collection of models and tools to perform Saliency Detection with PyTorch (cuda, mps, etc.).
+
+[![PyPI Version][pypi-image]][pypi-url]
+[![Build Status][build-image]][build-url]
+[![Code Coverage][coverage-image]][coverage-url]
+
+<!-- Badges: -->
+
+[pypi-image]: https://img.shields.io/pypi/v/saldet
+[pypi-url]: https://pypi.org/project/saldet/
+[build-image]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml/badge.svg
+[build-url]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml
+[coverage-image]: https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg
+[coverage-url]: https://codecov.io/gh/riccardomusmeci/saldet/
+
+## **Models**
+List of saliency detection models supported by saldet:
+
+* U2Net - https://arxiv.org/abs/2005.09007v3
+* PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet's repo](https://github.com/iCVTEAM/PGNet))
+
+
+## **Train**
+
+### **Easy Mode**
+The library comes with easy access to train models thanks to the amazing PyTorch Lightning support. 
+
+```python
+from saldet.experiment import train
+
+train(
+    data_dir=...,
+    config_path="config/u2net_lite.yaml", # check the config folder with some configurations
+    output_dir=...,
+    resume_from=...,
+    seed=42
+)
+```
+
+Once the training is over, configuration file and checkpoints will be saved into the output dir.
+
+**[WARNING]** The dataset must be structured as follows:
+```
+dataset
+    ├── train                    
+    |       ├── images          
+    |       │   ├── img_1.jpg
+    |       │   └── img_2.jpg                
+    |       └── masks
+    |           ├── img_1.png
+    |           └── img_2.png   
+    └── val
+           ├── images          
+           │   ├── img_10.jpg
+           │   └── img_11.jpg                
+           └── masks
+               ├── img_10.png
+               └── img_11.png   
+```
+
+### **PyTorch Lighting Mode**
+The library provides utils for model and data PyTorch Lightning Modules.
+```python
+import pytorch_lightning as pl
+from saldet import create_model
+from saldet.pl import SaliencyPLDataModule, SaliencyPLModel
+from saldet.transform import SaliencyTransform
+
+# datamodule
+datamodule = SaliencyPLDataModule(
+    root_dir=data_dir,
+    train_transform=SaliencyTransform(train=True, **config["transform"]),
+    val_transform=SaliencyTransform(train=False, **config["transform"]),
+    **config["datamodule"],
+)
+
+model = create_model(...)
+criterion = ...
+optimizer = ...
+lr_scheduler = ...
+
+pl_model = SaliencyPLModel(
+    model=model, criterion=criterion, optimizer=optimizer, lr_scheduler=lr_scheduler
+)
+
+trainer = pl.Trainer(...)
+
+# fit
+print(f"Launching training...")
+trainer.fit(model=pl_model, datamodule=datamodule)
+```
+
+### **PyTorch Mode**
+Alternatively you can define your custom training process and use the ```create_model()``` util to use the model you like.
+
+
+## **Inference**
+The library comes with easy access to inference saliency maps from a folder with images.
+```python
+from saldet.experiment import inference
+
+inference(
+    images_dir=...,
+    ckpt=..., # path to ckpt/pth model file
+    config_path=..., # path to configuration file from saldet train
+    output_dir=..., # where to save saliency maps
+)
+```
 
-packages = \
-['saldet',
- 'saldet.dataset',
- 'saldet.experiment',
- 'saldet.io',
- 'saldet.loss',
- 'saldet.lr_scheduler',
- 'saldet.model',
- 'saldet.model.models',
- 'saldet.ops',
- 'saldet.optimizer',
- 'saldet.pl',
- 'saldet.plot',
- 'saldet.trainer',
- 'saldet.transform',
- 'saldet.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['albumentations>=1.3.0,<2.0.0',
- 'lightning-bolts>=0.5.0,<0.6.0',
- 'matplotlib>=3.7.1,<4.0.0',
- 'pytorch-lightning>=2.0.0,<3.0.0',
- 'pyyaml>=6.0,<7.0',
- 'timm>=0.6.13,<0.7.0',
- 'torch>=2.0.1,<3.0.0',
- 'torchvision>=0.15.2,<0.16.0',
- 'tqdm>=4.65.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'saldet',
-    'version': '0.5.1',
-    'description': 'Saliency Detection library (models, loss, utils) with PyTorch',
-    'long_description': '# saldet\n> **Sal**iency **Det**ection (*saldet*) is a collection of models and tools to perform Saliency Detection with PyTorch.\n\n[![PyPI Version][pypi-image]][pypi-url]\n[![Build Status][build-image]][build-url]\n[![Code Coverage][coverage-image]][coverage-url]\n\n<!-- Badges: -->\n\n[pypi-image]: https://img.shields.io/pypi/v/saldet\n[pypi-url]: https://pypi.org/project/saldet/\n[build-image]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml/badge.svg\n[build-url]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml\n[coverage-image]: https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg\n[coverage-url]: https://codecov.io/gh/riccardomusmeci/saldet/\n\n## **Models**\nList of saliency detection models supported by saldet:\n\n* U2Net - https://arxiv.org/abs/2005.09007v3\n* PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet\'s repo](https://github.com/iCVTEAM/PGNet))\n\n\n## **Train**\n### **Easy Mode**\nThe library comes with easy access to train models thanks to the amazing PyTorch Lightning support. \n\n```python\nfrom saldet.experiment import train\n\ntrain(\n    data_dir=...,\n    config_path="config/u2net_lite.yaml", # check the config folder with some configurations\n    output_dir=...,\n    resume_from=...,\n    seed=42\n)\n```\n\nOnce the training is over, configuration file and checkpoints will be saved into the output dir.\n\n**[WARNING]** The dataset must be structured as follows:\n```\ndataset\n    ├── train                    \n    |       ├── images          \n    |       │   ├── img_1.jpg\n    |       │   └── img_2.jpg                \n    |       └── masks\n    |           ├── img_1.png\n    |           └── img_2.png   \n    └── val\n           ├── images          \n           │   ├── img_10.jpg\n           │   └── img_11.jpg                \n           └── masks\n               ├── img_10.png\n               └── img_11.png   \n```\n\n### **PyTorch Lighting Mode**\nThe library provides utils for model and data PyTorch Lightning Modules.\n```python\nimport pytorch_lightning as pl\nfrom saldet import create_model\nfrom saldet.pl import SaliencyPLDataModule, SaliencyPLModel\nfrom saldet.transform import SaliencyTransform\n\n# datamodule\ndatamodule = SaliencyPLDataModule(\n    root_dir=data_dir,\n    train_transform=SaliencyTransform(train=True, **config["transform"]),\n    val_transform=SaliencyTransform(train=False, **config["transform"]),\n    **config["datamodule"],\n)\n\nmodel = create_model(...)\ncriterion = ...\noptimizer = ...\nlr_scheduler = ...\n\npl_model = SaliencyPLModel(\n    model=model, criterion=criterion, optimizer=optimizer, lr_scheduler=lr_scheduler\n)\n\ntrainer = pl.Trainer(...)\n\n# fit\nprint(f"Launching training...")\ntrainer.fit(model=pl_model, datamodule=datamodule)\n```\n\n### **PyTorch Mode**\nAlternatively you can define your custom training process and use the ```create_model()``` util to use the model you like.\n\n\n## **Inference**\nThe library comes with easy access to inference saliency maps from a folder with images.\n```python\nfrom saldet.experiment import inference\n\ninference(\n    images_dir=...,\n    ckpt=..., # path to ckpt/pth model file\n    config_path=..., # path to configuration file from saldet train\n    output_dir=..., # where to save saliency maps\n)\n```\n\n## **To-Dos**\n\n[ ] Improve code coverage\n\n[ ] Add new models\n',
-    'author': 'Riccardo Musmeci',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/riccardomusmeci/saldet',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## **To-Dos**
 
+[ ] Improve code coverage
+
+[ ] Add new models
 
-setup(**setup_kwargs)
```

