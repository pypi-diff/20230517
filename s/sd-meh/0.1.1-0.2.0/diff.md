# Comparing `tmp/sd_meh-0.1.1.tar.gz` & `tmp/sd_meh-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.1.1.tar", max compression
+gzip compressed data, was "sd_meh-0.2.0.tar", max compression
```

## Comparing `sd_meh-0.1.1.tar` & `sd_meh-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-05-10 14:42:40.197057 sd_meh-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1359 2023-05-12 08:39:24.814256 sd_meh-0.1.1/README.md
--rw-r--r--   0        0        0      390 2023-05-12 08:38:00.548569 sd_meh-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 13:19:22.947635 sd_meh-0.1.1/sd_meh/__init__.py
--rw-r--r--   0        0        0     5804 2023-05-12 08:32:12.808921 sd_meh-0.1.1/sd_meh/merge.py
--rw-r--r--   0        0        0     1465 2023-05-10 13:19:22.948414 sd_meh-0.1.1/sd_meh/model.py
--rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 sd_meh-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 14:42:40.197057 sd_meh-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1359 2023-05-12 08:39:24.814256 sd_meh-0.2.0/README.md
+-rw-r--r--   0        0        0      390 2023-05-17 11:14:54.463646 sd_meh-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-17 11:14:54.463955 sd_meh-0.2.0/sd_meh/__init__.py
+-rw-r--r--   0        0        0     6236 2023-05-17 11:14:54.464545 sd_meh-0.2.0/sd_meh/merge.py
+-rw-r--r--   0        0        0     1465 2023-05-10 13:19:22.948414 sd_meh-0.2.0/sd_meh/model.py
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 sd_meh-0.2.0/PKG-INFO
```

### Comparing `sd_meh-0.1.1/LICENSE.txt` & `sd_meh-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.1.1/README.md` & `sd_meh-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sd_meh-0.1.1/sd_meh/merge.py` & `sd_meh-0.2.0/sd_meh/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
 from pathlib import Path
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
 
 from sd_meh.model import SDModel
 
@@ -55,35 +55,40 @@
 # https://github.com/j4ded/sdweb-merge-block-weighted-gui/blob/master/scripts/mbw/merge_block_weighted.py#L115
 def fix_model(model: Dict) -> Dict:
     for k in model:
         model = fix_key(model, k)
     return fix_clip(model)
 
 
-def load_sd_model(model_path: os.PathLike, device: str = "cpu") -> SDModel:
-    return SDModel(model_path, device).load_model()
+def load_sd_model(model: os.PathLike | str, device: str = "cpu") -> Dict:
+    if isinstance(model, str):
+        model = Path(model)
+
+    return SDModel(model, device).load_model()
 
 
 def merge_models(
-    models: Dict[str, os.PathLike],
+    models: Dict[str, os.PathLike | str],
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
-) -> None:
-    thetas = {k: load_sd_model(Path(m)) for k, m in models.items()}
+    weights_clip: bool = False,
+) -> Dict:
+    thetas = {k: load_sd_model(m) for k, m in models.items()}
 
     for key in tqdm(thetas["model_a"].keys(), desc="stage 1"):
         if result := merge_key(
             key,
             thetas,
             weights,
             bases,
             merge_mode,
             precision,
+            weights_clip,
         ):
             thetas["model_a"][key] = result[1]
 
     for key in tqdm(thetas["model_b"].keys(), desc="stage 2"):
         if KEY_POSITION_IDS in key:
             continue
         if "model" in key and key not in thetas["model_a"]:
@@ -97,15 +102,16 @@
 def merge_key(
     key: str,
     thetas: Dict,
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
-) -> Tuple[str, Dict]:
+    weights_clip: bool = False,
+) -> Optional[Tuple[str, Dict]]:
     if KEY_POSITION_IDS in key:
         return
 
     for theta in thetas.values():
         if key not in theta:
             return
 
@@ -134,21 +140,27 @@
                 raise ValueError(f"illegal block index {key}")
 
             if weight_index >= 0:
                 current_bases = {k: w[weight_index] for k, w in weights.items()}
 
         merged_key = merge(current_bases, thetas, key, merge_mode)
 
+        if weights_clip:
+            t0 = thetas["model_a"][key]
+            t1 = thetas["model_b"][key]
+            threshold = torch.maximum(torch.abs(t0), torch.abs(t1))
+            merged_key = torch.minimum(torch.maximum(merged_key, -threshold), threshold)
+
         if precision == 16:
             merged_key = merged_key.half()
 
-        return (key, merged_key)
+        return key, merged_key
 
 
-def merge(current_bases: Dict, thetas: Dict, key: str, merge_mode: str) -> Dict:
+def merge(current_bases: Dict, thetas: Dict, key: str, merge_mode: str) -> torch.Tensor:
     t0 = thetas["model_a"][key]
     t1 = thetas["model_b"][key]
     alpha = current_bases["alpha"]
     if merge_mode == "weighted_sum":
         return (1 - alpha) * t0 + alpha * t1
     elif merge_mode == "weighted_subtraction":
         beta = current_bases["beta"]
```

### Comparing `sd_meh-0.1.1/sd_meh/model.py` & `sd_meh-0.2.0/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.1.1/PKG-INFO` & `sd_meh-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.1.1
+Version: 0.2.0
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

