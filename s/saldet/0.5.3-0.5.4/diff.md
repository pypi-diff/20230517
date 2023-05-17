# Comparing `tmp/saldet-0.5.3.tar.gz` & `tmp/saldet-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saldet-0.5.3.tar", max compression
+gzip compressed data, was "saldet-0.5.4.tar", max compression
```

## Comparing `saldet-0.5.3.tar` & `saldet-0.5.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.3/LICENSE
--rw-r--r--   0        0        0     3440 2023-05-11 09:22:36.999483 saldet-0.5.3/README.md
--rw-r--r--   0        0        0      917 2023-05-17 16:47:15.304311 saldet-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       55 2023-05-17 16:46:33.081338 saldet-0.5.3/saldet/__init__.py
--rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.3/saldet/dataset/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.3/saldet/dataset/inference.py
--rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.3/saldet/dataset/saliency.py
--rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.3/saldet/experiment/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-17 16:13:05.313542 saldet-0.5.3/saldet/experiment/inference.py
--rw-r--r--   0        0        0     2312 2023-05-17 16:10:40.783399 saldet-0.5.3/saldet/experiment/train.py
--rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.3/saldet/io/__init__.py
--rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.3/saldet/io/config.py
--rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.3/saldet/io/image.py
--rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.3/saldet/loss/__init__.py
--rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.3/saldet/loss/_factory.py
--rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.3/saldet/loss/attn_guided.py
--rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.3/saldet/loss/bce_iou_loss.py
--rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.5.3/saldet/loss/multi_bce.py
--rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.5.3/saldet/loss/pg.py
--rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.3/saldet/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.3/saldet/lr_scheduler/lr_scheduler.py
--rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.5.3/saldet/model/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-11 09:14:45.294803 saldet-0.5.3/saldet/model/_factory.py
--rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.3/saldet/model/models/__init__.py
--rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.3/saldet/model/models/pgnet.py
--rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.3/saldet/model/models/resnet.py
--rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.3/saldet/model/models/swin.py
--rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.3/saldet/model/models/u2net.py
--rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.3/saldet/ops/__init__.py
--rw-r--r--   0        0        0      930 2023-05-17 15:23:24.394224 saldet-0.5.3/saldet/ops/tensor.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.3/saldet/optimizer/__init__.py
--rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.3/saldet/optimizer/optimizer.py
--rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.3/saldet/pl/__init__.py
--rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.3/saldet/pl/data.py
--rw-r--r--   0        0        0     2370 2023-05-16 13:40:17.705235 saldet-0.5.3/saldet/pl/model.py
--rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.3/saldet/plot/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-17 16:46:33.116615 saldet-0.5.3/saldet/plot/plot.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.3/saldet/trainer/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.3/saldet/trainer/callbacks.py
--rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.3/saldet/transform/__init__.py
--rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.3/saldet/transform/transform.py
--rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.3/saldet/utils/__init__.py
--rw-r--r--   0        0        0      225 2023-05-11 09:34:56.451378 saldet-0.5.3/saldet/utils/device.py
--rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.3/saldet/utils/time.py
--rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 saldet-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.4/LICENSE
+-rw-r--r--   0        0        0     4452 2023-05-17 17:43:12.582735 saldet-0.5.4/README.md
+-rw-r--r--   0        0        0      917 2023-05-17 17:43:28.129429 saldet-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-05-17 17:40:46.932866 saldet-0.5.4/saldet/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.4/saldet/dataset/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.4/saldet/dataset/inference.py
+-rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.4/saldet/dataset/saliency.py
+-rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.4/saldet/experiment/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-17 16:13:05.313542 saldet-0.5.4/saldet/experiment/inference.py
+-rw-r--r--   0        0        0     2312 2023-05-17 16:10:40.783399 saldet-0.5.4/saldet/experiment/train.py
+-rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.4/saldet/io/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.4/saldet/io/config.py
+-rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.4/saldet/io/image.py
+-rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.4/saldet/loss/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.4/saldet/loss/_factory.py
+-rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.4/saldet/loss/attn_guided.py
+-rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.4/saldet/loss/bce_iou_loss.py
+-rw-r--r--   0        0        0     1130 2023-05-17 16:56:43.163212 saldet-0.5.4/saldet/loss/multi_bce.py
+-rw-r--r--   0        0        0      858 2023-05-17 16:57:23.426213 saldet-0.5.4/saldet/loss/pg.py
+-rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.4/saldet/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.4/saldet/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0        0        0       65 2023-05-17 17:43:09.823099 saldet-0.5.4/saldet/model/__init__.py
+-rw-r--r--   0        0        0     2424 2023-05-17 17:43:09.733847 saldet-0.5.4/saldet/model/_factory.py
+-rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.4/saldet/model/models/__init__.py
+-rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.4/saldet/model/models/pgnet.py
+-rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.4/saldet/model/models/resnet.py
+-rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.4/saldet/model/models/swin.py
+-rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.4/saldet/model/models/u2net.py
+-rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.4/saldet/ops/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-17 15:23:24.394224 saldet-0.5.4/saldet/ops/tensor.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.4/saldet/optimizer/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.4/saldet/optimizer/optimizer.py
+-rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.4/saldet/pl/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.4/saldet/pl/data.py
+-rw-r--r--   0        0        0     2370 2023-05-16 13:40:17.705235 saldet-0.5.4/saldet/pl/model.py
+-rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.4/saldet/plot/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-17 16:46:33.116615 saldet-0.5.4/saldet/plot/plot.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.4/saldet/trainer/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.4/saldet/trainer/callbacks.py
+-rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.4/saldet/transform/__init__.py
+-rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.4/saldet/transform/transform.py
+-rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.4/saldet/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-11 09:34:56.451378 saldet-0.5.4/saldet/utils/device.py
+-rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.4/saldet/utils/time.py
+-rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 saldet-0.5.4/PKG-INFO
```

### Comparing `saldet-0.5.3/LICENSE` & `saldet-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/README.md` & `saldet-0.5.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -13,17 +13,29 @@
 [build-url]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml
 [coverage-image]: https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg
 [coverage-url]: https://codecov.io/gh/riccardomusmeci/saldet/
 
 ## **Models**
 List of saliency detection models supported by saldet:
 
-* U2Net - https://arxiv.org/abs/2005.09007v3
-* PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet's repo](https://github.com/iCVTEAM/PGNet))
+* U2Net - https://arxiv.org/abs/2005.09007v3 ([U2Net repo](https://github.com/xuebinqin/U-2-Net))
+* PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet repo](https://github.com/iCVTEAM/PGNet))
 
+### **Weights**
+* PGNet -> weights from [PGNet's repo](https://github.com/iCVTEAM/PGNet) converted to saldet version from [here](https://drive.google.com/file/d/1gr0lWZoCIucrV5-Z_QV23tUNd8826EjN/view?usp=share_link)
+* U2Net Lite -> weights from [here](https://drive.google.com/file/d/1rbSTGKAE-MTxBYHd-51l2hMOQPT_7EPy/view?usp=sharing) (U2Net repository)
+* U2Net Full -> weights from [here](https://drive.google.com/file/d/1ao1ovG1Qtx4b7EoskHXmi2E9rp5CHLcZ/view?usp=sharing) (U2Net repository)
+* U2Net Full - Portrait -> weights for portrait images from [here](https://drive.google.com/file/d/1IG3HdpcRiDoWNookbncQjeaPN28t90yW/view) (U2Net repository)
+* U2Net Full - Human Segmentation -> weights for segmenting humans from [here](https://drive.google.com/file/d/1-Yg0cxgrNhHP-016FPdp902BR-kSsA4P/view) (U2Net repository)
+
+To load pre-trained weights:
+```python
+from saldet import create_model
+model = create_model("pgnet", checkpoint_path=".../pgnet.pth")
+```
 
 ## **Train**
 
 ### **Easy Mode**
 The library comes with easy access to train models thanks to the amazing PyTorch Lightning support. 
 
 ```python
```

### Comparing `saldet-0.5.3/pyproject.toml` & `saldet-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saldet"
-version = "0.5.3"
+version = "0.5.4"
 description = "Saliency Detection library (models, loss, utils) with PyTorch"
 authors = ["Riccardo Musmeci"]
 repository = "https://github.com/riccardomusmeci/saldet"
 license = "MIT"
 readme = "README.md"
 keywords = ["computer vision", "saliency detection"]
```

### Comparing `saldet-0.5.3/saldet/dataset/inference.py` & `saldet-0.5.4/saldet/dataset/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/dataset/saliency.py` & `saldet-0.5.4/saldet/dataset/saliency.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/experiment/inference.py` & `saldet-0.5.4/saldet/experiment/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/experiment/train.py` & `saldet-0.5.4/saldet/experiment/train.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/io/image.py` & `saldet-0.5.4/saldet/io/image.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/loss/attn_guided.py` & `saldet-0.5.4/saldet/loss/attn_guided.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/loss/bce_iou_loss.py` & `saldet-0.5.4/saldet/loss/bce_iou_loss.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/loss/multi_bce.py` & `saldet-0.5.4/saldet/loss/multi_bce.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/loss/pg.py` & `saldet-0.5.4/saldet/loss/pg.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/lr_scheduler/lr_scheduler.py` & `saldet-0.5.4/saldet/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/model/_factory.py` & `saldet-0.5.4/saldet/model/_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,21 @@
             state_dict = torch.load(f=checkpoint_path, map_location="cpu")
         model.load_state_dict(state_dict=state_dict)
         print(f"> Loaded state dict for {model_name}.")
 
     return model
 
 
+def list_models():
+    """List all available models"""
+    print(f"saldet available models:")
+    for m in FACTORY:
+        print(f"> {m}")
+
+
 def load_checkpoint(
     ckpt: str,
     model_name: str = None,
 ) -> nn.Module:
     """Load either a checkpoint with pytorch-lightning support or a pth file
 
     Args:
```

### Comparing `saldet-0.5.3/saldet/model/models/pgnet.py` & `saldet-0.5.4/saldet/model/models/pgnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/model/models/resnet.py` & `saldet-0.5.4/saldet/model/models/resnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/model/models/swin.py` & `saldet-0.5.4/saldet/model/models/swin.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/model/models/u2net.py` & `saldet-0.5.4/saldet/model/models/u2net.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/ops/tensor.py` & `saldet-0.5.4/saldet/ops/tensor.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/optimizer/optimizer.py` & `saldet-0.5.4/saldet/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/pl/data.py` & `saldet-0.5.4/saldet/pl/data.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/pl/model.py` & `saldet-0.5.4/saldet/pl/model.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/plot/plot.py` & `saldet-0.5.4/saldet/plot/plot.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/trainer/callbacks.py` & `saldet-0.5.4/saldet/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/saldet/transform/transform.py` & `saldet-0.5.4/saldet/transform/transform.py`

 * *Files identical despite different names*

### Comparing `saldet-0.5.3/PKG-INFO` & `saldet-0.5.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saldet
-Version: 0.5.3
+Version: 0.5.4
 Summary: Saliency Detection library (models, loss, utils) with PyTorch
 Home-page: https://github.com/riccardomusmeci/saldet
 License: MIT
 Keywords: computer vision,saliency detection
 Author: Riccardo Musmeci
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -40,17 +40,29 @@
 [build-url]: https://github.com/riccardomusmeci/saldet/actions/workflows/build.yaml
 [coverage-image]: https://codecov.io/gh/riccardomusmeci/saldet/branch/main/graph/badge.svg
 [coverage-url]: https://codecov.io/gh/riccardomusmeci/saldet/
 
 ## **Models**
 List of saliency detection models supported by saldet:
 
-* U2Net - https://arxiv.org/abs/2005.09007v3
-* PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet's repo](https://github.com/iCVTEAM/PGNet))
+* U2Net - https://arxiv.org/abs/2005.09007v3 ([U2Net repo](https://github.com/xuebinqin/U-2-Net))
+* PGNet - https://arxiv.org/abs/2204.05041 (follow training instructions from [PGNet repo](https://github.com/iCVTEAM/PGNet))
 
+### **Weights**
+* PGNet -> weights from [PGNet's repo](https://github.com/iCVTEAM/PGNet) converted to saldet version from [here](https://drive.google.com/file/d/1gr0lWZoCIucrV5-Z_QV23tUNd8826EjN/view?usp=share_link)
+* U2Net Lite -> weights from [here](https://drive.google.com/file/d/1rbSTGKAE-MTxBYHd-51l2hMOQPT_7EPy/view?usp=sharing) (U2Net repository)
+* U2Net Full -> weights from [here](https://drive.google.com/file/d/1ao1ovG1Qtx4b7EoskHXmi2E9rp5CHLcZ/view?usp=sharing) (U2Net repository)
+* U2Net Full - Portrait -> weights for portrait images from [here](https://drive.google.com/file/d/1IG3HdpcRiDoWNookbncQjeaPN28t90yW/view) (U2Net repository)
+* U2Net Full - Human Segmentation -> weights for segmenting humans from [here](https://drive.google.com/file/d/1-Yg0cxgrNhHP-016FPdp902BR-kSsA4P/view) (U2Net repository)
+
+To load pre-trained weights:
+```python
+from saldet import create_model
+model = create_model("pgnet", checkpoint_path=".../pgnet.pth")
+```
 
 ## **Train**
 
 ### **Easy Mode**
 The library comes with easy access to train models thanks to the amazing PyTorch Lightning support. 
 
 ```python
```

