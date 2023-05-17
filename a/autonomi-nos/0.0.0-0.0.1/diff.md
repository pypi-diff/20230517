# Comparing `tmp/autonomi_nos-0.0.0-py3-none-any.whl.zip` & `tmp/autonomi_nos-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,48 @@
-Zip file size: 4225 bytes, number of entries: 8
--rw-rw-r--  2.0 unx       22 b- defN 23-Apr-17 22:34 nos/_version.py
--rw-rw-r--  2.0 unx     1109 b- defN 23-Apr-17 22:30 nos/test_utils.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-Apr-17 22:34 autonomi_nos-0.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3016 b- defN 23-Apr-17 22:34 autonomi_nos-0.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 22:34 autonomi_nos-0.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Apr-17 22:34 autonomi_nos-0.0.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 23-Apr-17 22:34 autonomi_nos-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 23-Apr-17 22:34 autonomi_nos-0.0.0.dist-info/RECORD
-8 files, 6018 bytes uncompressed, 3073 bytes compressed:  48.9%
+Zip file size: 40342 bytes, number of entries: 46
+-rw-rw-r--  2.0 unx      119 b- defN 23-Apr-23 00:49 nos/__init__.py
+-rw-rw-r--  2.0 unx      561 b- defN 23-May-16 21:17 nos/constants.py
+-rw-rw-r--  2.0 unx       93 b- defN 23-May-01 21:40 nos/exceptions.py
+-rw-rw-r--  2.0 unx      940 b- defN 23-May-01 21:40 nos/logging.py
+-rw-rw-r--  2.0 unx     2716 b- defN 23-May-16 21:17 nos/protoc.py
+-rw-rw-r--  2.0 unx       22 b- defN 23-May-17 21:49 nos/version.py
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-23 00:49 nos/cli/benchmark.py
+-rw-rw-r--  2.0 unx      455 b- defN 23-May-16 21:17 nos/cli/cli.py
+-rw-rw-r--  2.0 unx     1983 b- defN 23-May-16 21:17 nos/cli/docker.py
+-rw-rw-r--  2.0 unx     1294 b- defN 23-Apr-23 00:49 nos/cli/hub.py
+-rw-rw-r--  2.0 unx     6244 b- defN 23-May-16 21:17 nos/cli/serve_grpc.py
+-rw-rw-r--  2.0 unx     5962 b- defN 23-May-16 21:17 nos/cli/serve_http.py
+-rw-rw-r--  2.0 unx     3479 b- defN 23-May-16 21:17 nos/cli/system.py
+-rw-rw-r--  2.0 unx      425 b- defN 23-May-05 01:05 nos/cli/utils.py
+-rw-rw-r--  2.0 unx      148 b- defN 23-May-16 21:17 nos/client/__init__.py
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-12 23:31 nos/client/exceptions.py
+-rw-rw-r--  2.0 unx     6048 b- defN 23-May-16 21:17 nos/client/grpc/client.py
+-rw-rw-r--  2.0 unx     6193 b- defN 23-May-12 23:31 nos/executors/ray.py
+-rw-rw-r--  2.0 unx     2087 b- defN 23-May-15 21:54 nos/hub/__init__.py
+-rw-rw-r--  2.0 unx     1812 b- defN 23-May-15 21:54 nos/hub/config.py
+-rw-rw-r--  2.0 unx      902 b- defN 23-May-12 23:31 nos/hub/spec.py
+-rw-rw-r--  2.0 unx      242 b- defN 23-May-15 21:54 nos/models/__init__.py
+-rw-rw-r--  2.0 unx     2370 b- defN 23-May-10 21:27 nos/models/clip.py
+-rw-rw-r--  2.0 unx     2028 b- defN 23-May-12 23:31 nos/models/faster_rcnn.py
+-rw-rw-r--  2.0 unx     2651 b- defN 23-May-01 21:36 nos/models/stable_diffusion.py
+-rw-rw-r--  2.0 unx       66 b- defN 23-May-13 02:32 nos/models/openmmlab/mmdetection/detection_tensorrt_dynamic-320x320-1344x1344.py
+-rw-rw-r--  2.0 unx     2589 b- defN 23-May-13 02:01 nos/models/openmmlab/mmdetection/mmdetection.py
+-rw-rw-r--  2.0 unx      370 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py
+-rw-rw-r--  2.0 unx     3187 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py
+-rw-rw-r--  2.0 unx     1765 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_instance.py
+-rw-rw-r--  2.0 unx     3828 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/models/faster-rcnn_r50_fpn.py
+-rw-rw-r--  2.0 unx      304 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py
+-rw-rw-r--  2.0 unx     5340 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py
+-rw-rw-r--  2.0 unx      177 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py
+-rw-rw-r--  2.0 unx      156 b- defN 23-May-16 21:17 nos/server/__init__.py
+-rw-rw-r--  2.0 unx     6235 b- defN 23-May-16 21:17 nos/server/docker.py
+-rw-rw-r--  2.0 unx     3047 b- defN 23-May-16 21:17 nos/server/runtime.py
+-rw-rw-r--  2.0 unx     8421 b- defN 23-May-16 21:17 nos/server/service.py
+-rw-rw-r--  2.0 unx      373 b- defN 23-Apr-23 00:49 nos/test/benchmark.py
+-rw-rw-r--  2.0 unx     1318 b- defN 23-May-01 21:36 nos/test/utils.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-17 21:49 autonomi_nos-0.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6095 b- defN 23-May-17 21:49 autonomi_nos-0.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-17 21:49 autonomi_nos-0.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-17 21:49 autonomi_nos-0.0.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-17 21:49 autonomi_nos-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4033 b- defN 23-May-17 21:49 autonomi_nos-0.0.1.dist-info/RECORD
+46 files, 97530 bytes uncompressed, 33836 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,25 +1,139 @@
-Filename: nos/_version.py
+Filename: nos/__init__.py
 Comment: 
 
-Filename: nos/test_utils.py
+Filename: nos/constants.py
 Comment: 
 
-Filename: autonomi_nos-0.0.0.dist-info/LICENSE
+Filename: nos/exceptions.py
 Comment: 
 
-Filename: autonomi_nos-0.0.0.dist-info/METADATA
+Filename: nos/logging.py
 Comment: 
 
-Filename: autonomi_nos-0.0.0.dist-info/WHEEL
+Filename: nos/protoc.py
 Comment: 
 
-Filename: autonomi_nos-0.0.0.dist-info/entry_points.txt
+Filename: nos/version.py
 Comment: 
 
-Filename: autonomi_nos-0.0.0.dist-info/top_level.txt
+Filename: nos/cli/benchmark.py
 Comment: 
 
-Filename: autonomi_nos-0.0.0.dist-info/RECORD
+Filename: nos/cli/cli.py
+Comment: 
+
+Filename: nos/cli/docker.py
+Comment: 
+
+Filename: nos/cli/hub.py
+Comment: 
+
+Filename: nos/cli/serve_grpc.py
+Comment: 
+
+Filename: nos/cli/serve_http.py
+Comment: 
+
+Filename: nos/cli/system.py
+Comment: 
+
+Filename: nos/cli/utils.py
+Comment: 
+
+Filename: nos/client/__init__.py
+Comment: 
+
+Filename: nos/client/exceptions.py
+Comment: 
+
+Filename: nos/client/grpc/client.py
+Comment: 
+
+Filename: nos/executors/ray.py
+Comment: 
+
+Filename: nos/hub/__init__.py
+Comment: 
+
+Filename: nos/hub/config.py
+Comment: 
+
+Filename: nos/hub/spec.py
+Comment: 
+
+Filename: nos/models/__init__.py
+Comment: 
+
+Filename: nos/models/clip.py
+Comment: 
+
+Filename: nos/models/faster_rcnn.py
+Comment: 
+
+Filename: nos/models/stable_diffusion.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/detection_tensorrt_dynamic-320x320-1344x1344.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/mmdetection.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_instance.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/configs/_base_/models/faster-rcnn_r50_fpn.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py
+Comment: 
+
+Filename: nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py
+Comment: 
+
+Filename: nos/server/__init__.py
+Comment: 
+
+Filename: nos/server/docker.py
+Comment: 
+
+Filename: nos/server/runtime.py
+Comment: 
+
+Filename: nos/server/service.py
+Comment: 
+
+Filename: nos/test/benchmark.py
+Comment: 
+
+Filename: nos/test/utils.py
+Comment: 
+
+Filename: autonomi_nos-0.0.1.dist-info/LICENSE
+Comment: 
+
+Filename: autonomi_nos-0.0.1.dist-info/METADATA
+Comment: 
+
+Filename: autonomi_nos-0.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: autonomi_nos-0.0.1.dist-info/entry_points.txt
+Comment: 
+
+Filename: autonomi_nos-0.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: autonomi_nos-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nos/test_utils.py` & `nos/test/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,45 @@
-#  Copyright 2022-  Autonomi AI , Inc. All rights reserved.
 """Various test utilities."""
 import os
 import unittest
+from enum import Enum
 from pathlib import Path
 
 import torch
 
-NOS_TEST_DATA_DIR = Path(__file__).parent.parent / "tests/test_data"
+
+NOS_TEST_DATA_DIR = Path(__file__).parent.parent.parent / "tests/test_data"
 NOS_TEST_IMAGE = NOS_TEST_DATA_DIR / "test.jpg"
 NOS_TEST_VIDEO = NOS_TEST_DATA_DIR / "test.mp4"
 NOS_TEST_AUDIO = NOS_TEST_DATA_DIR / "test_speech.flac"
 
 
+class PyTestGroup(Enum):
+    """pytest group for grouping model tests, benchmarks etc."""
+
+    UNIT = "unit"
+    INTEGRATION = "integration"
+    HUB = "hub"
+    BENCHMARK = "benchmark"
+    BENCHMARK_MODELS = "benchmark-models"
+
+
 def benchmark(test_case):
     """
     Decorator marking a test that is a benchmark (slow).
 
-    These tests are triggered when `NOS_TEST_BENCHMARKS=1`, and defaults to False.
+    These tests are triggered when `NOS_TEST_BENCHMARK=1`, and defaults to False.
     """
     return unittest.skipUnless(
-        os.getenv("NOS_TEST_BENCHMARK", default=False), "slow test requires NOS_TEST_BENCHMARK=1"
+        bool(os.getenv("NOS_TEST_BENCHMARK", default=False)),
+        "test requires NOS_TEST_BENCHMARK=1",
     )(test_case)
 
 
-def require_torch_cuda(test_case):
+def requires_torch_cuda(test_case):
     """
     Decorator marking a test that requires torch cuda devices.
 
     These tests are skipped when torch.cuda.is_available() is set to False. If
     `CUDA_VISIBLE_DEVICES=""` then, the decorated test is not run.
     """
     return unittest.skipUnless(torch.cuda.is_available(), "test requires torch.cuda.is_available() to be True")(
```

## Comparing `autonomi_nos-0.0.0.dist-info/LICENSE` & `autonomi_nos-0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

