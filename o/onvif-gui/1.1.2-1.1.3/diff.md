# Comparing `tmp/onvif-gui-1.1.2.tar.gz` & `tmp/onvif-gui-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.1.2.tar", last modified: Tue May  9 01:03:23 2023, max compression
+gzip compressed data, was "onvif-gui-1.1.3.tar", last modified: Wed May 17 14:59:50 2023, max compression
```

## Comparing `onvif-gui-1.1.2.tar` & `onvif-gui-1.1.3.tar`

### file list

```diff
@@ -1,284 +1,286 @@
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.932168 onvif-gui-1.1.2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)      217 2023-05-09 00:18:57.000000 onvif-gui-1.1.2/MANIFEST.in
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-09 01:03:23.932168 onvif-gui-1.1.2/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8170 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/README.md
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.900168 onvif-gui-1.1.2/detectron2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       67 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.900168 onvif-gui-1.1.2/detectron2/checkpoint/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/checkpoint/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17770 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/checkpoint/c2_model_loading.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5685 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/checkpoint/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5258 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/checkpoint/detection_checkpoint.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.900168 onvif-gui-1.1.2/detectron2/config/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      599 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/config/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7890 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/config/compat.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9211 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/config/config.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29512 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/config/defaults.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3015 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/config/instantiate.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15378 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/config/lazy.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.900168 onvif-gui-1.1.2/detectron2/configs/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1318 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/configs/Base-RCNN-FPN.yaml
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.900168 onvif-gui-1.1.2/detectron2/configs/COCO-InstanceSegmentation/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:42.000000 onvif-gui-1.1.2/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      192 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.900168 onvif-gui-1.1.2/detectron2/configs/COCO-Keypoints/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      527 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:42.000000 onvif-gui-1.1.2/detectron2/configs/COCO-Keypoints/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      182 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/configs/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.904168 onvif-gui-1.1.2/detectron2/data/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      644 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7378 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/benchmark.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21231 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7224 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9162 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8169 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/dataset_mapper.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.904168 onvif-gui-1.1.2/detectron2/data/datasets/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      523 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10174 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/builtin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21841 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/builtin_meta.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13167 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/cityscapes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7821 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/cityscapes_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23465 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8977 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/coco_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9623 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/lvis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   223757 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   219177 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/lvis_v1_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    39414 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3128 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/pascal_voc.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      169 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/datasets/register_coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    22841 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/detection_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.904168 onvif-gui-1.1.2/detectron2/data/samplers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      412 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/samplers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11789 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/samplers/distributed_sampler.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1944 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/samplers/grouped_batch_sampler.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.904168 onvif-gui-1.1.2/detectron2/data/transforms/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      466 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/transforms/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14112 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/transforms/augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23069 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/transforms/augmentation_impl.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12629 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/data/transforms/transform.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.908168 onvif-gui-1.1.2/detectron2/layers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      874 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5764 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/aspp.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12131 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/batch_norm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3024 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16978 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/deform_conv.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4202 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10879 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/mask_ops.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6490 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3098 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/roi_align.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3302 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/roi_align_rotated.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      652 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      537 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/shape_spec.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5123 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/layers/wrappers.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.908168 onvif-gui-1.1.2/detectron2/modeling/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1568 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15439 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/anchor_generator.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.912168 onvif-gui-1.1.2/detectron2/modeling/backbone/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      598 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2512 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/backbone.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1015 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10360 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15988 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/mvit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16656 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/regnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23658 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/resnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25095 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/swin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6360 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19338 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/backbone/vit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15123 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/box_regression.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/matcher.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.912168 onvif-gui-1.1.2/detectron2/modeling/meta_arch/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      508 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      814 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11651 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/dense_detector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13213 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/fcos.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10407 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13896 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18265 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9906 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/meta_arch/semantic_seg.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10832 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/mmdet_wrapper.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11316 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/poolers.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4045 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/postprocessing.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.912168 onvif-gui-1.1.2/detectron2/modeling/proposal_generator/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      231 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/proposal_generator/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      836 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/proposal_generator/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8128 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23814 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/proposal_generator/rpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8807 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/proposal_generator/rrpn.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.912168 onvif-gui-1.1.2/detectron2/modeling/roi_heads/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/box_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12990 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25390 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11156 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/keypoint_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12169 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/mask_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    37701 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/roi_heads.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11175 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2334 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/sampling.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12416 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/modeling/test_time_augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1780 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/predictor.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.916168 onvif-gui-1.1.2/detectron2/structures/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/structures/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14429 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/structures/boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5520 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/structures/image_list.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6613 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/structures/instances.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/structures/keypoints.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19802 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/structures/masks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18853 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/structures/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2707 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/tracker.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.916168 onvif-gui-1.1.2/detectron2/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       51 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6017 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/analysis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8391 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/collect_env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4096 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/colormap.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5608 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/comm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1852 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/develop.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5644 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17022 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/events.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1189 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/file_io.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7807 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/logger.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2583 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/memory.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1874 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/registry.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1064 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/serialize.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18113 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/testing.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11319 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/video_visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    51159 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/detectron2/utils/visualizer.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.916168 onvif-gui-1.1.2/gui/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.916168 onvif-gui-1.1.2/gui/components/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/components/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1738 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/components/comboselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2397 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/components/directoryselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2118 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/components/fileselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5315 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/components/labelselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/components/progress.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1918 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/components/thresholdslider.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1996 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/glwidget.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14377 2023-05-09 01:01:19.000000 onvif-gui-1.1.2/gui/main.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.920168 onvif-gui-1.1.2/gui/onvif/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      191 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/onvif/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5743 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/onvif/admintab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3959 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/onvif/imagetab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2425 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/onvif/logindialog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5247 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/onvif/networktab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5118 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/onvif/ptztab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4527 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/onvif/videotab.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.920168 onvif-gui-1.1.2/gui/panels/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      180 2023-05-03 01:49:37.000000 onvif-gui-1.1.2/gui/panels/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3624 2023-05-03 02:34:01.000000 onvif-gui-1.1.2/gui/panels/audiopanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13463 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/panels/camerapanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14483 2023-05-03 15:52:33.000000 onvif-gui-1.1.2/gui/panels/filepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12913 2023-05-02 23:52:13.000000 onvif-gui-1.1.2/gui/panels/settingspanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3627 2023-05-03 02:39:24.000000 onvif-gui-1.1.2/gui/panels/videopanel.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.928168 onvif-gui-1.1.2/gui/resources/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1936 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/apply.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/apply_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/apply_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/audio.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/audio_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/audio_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/branch_closed.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/branch_closed_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/branch_closed_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/branch_open.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/branch_open_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/branch_open_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/checked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/checked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/checked_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12716 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/darkstyle.qss
--rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/discover.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/discover_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/discover_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/fast-forward.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/fast-forward_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/fast-forward_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/mute.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/mute_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/mute_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/next.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/next_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/next_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/onvif-gui.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/pause.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/pause_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/pause_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/play.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/play_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/play_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/previous.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/previous_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/previous_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/radio-off.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/radio-off_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/radio-off_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/radio-on.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/radio-on_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/radio-on_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/record.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/record_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/record_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/recording.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/recording_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/recording_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/rewind.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/rewind_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/rewind_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/small_arrow_left.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/small_arrow_left_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/small_arrow_left_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/small_arrow_up.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/small_arrow_up_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/small_arrow_up_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/stop.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/stop_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/stop_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/unchecked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/unchecked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/gui/resources/unchecked_lo.png
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.928168 onvif-gui-1.1.2/modules/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:45:47.000000 onvif-gui-1.1.2/modules/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.928168 onvif-gui-1.1.2/modules/audio/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-03 02:36:19.000000 onvif-gui-1.1.2/modules/audio/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3404 2023-05-03 19:20:32.000000 onvif-gui-1.1.2/modules/audio/sample.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.928168 onvif-gui-1.1.2/modules/video/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.1.2/modules/video/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6757 2023-05-09 00:56:27.000000 onvif-gui-1.1.2/modules/video/keypoint.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4796 2023-05-09 00:54:17.000000 onvif-gui-1.1.2/modules/video/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3016 2023-05-03 02:51:12.000000 onvif-gui-1.1.2/modules/video/sample.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7345 2023-05-09 00:52:12.000000 onvif-gui-1.1.2/modules/video/segment.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11751 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/modules/video/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.928168 onvif-gui-1.1.2/onvif_gui.egg-info/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-09 01:03:23.000000 onvif-gui-1.1.2/onvif_gui.egg-info/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7976 2023-05-09 01:03:23.000000 onvif-gui-1.1.2/onvif_gui.egg-info/SOURCES.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-05-09 01:03:23.000000 onvif-gui-1.1.2/onvif_gui.egg-info/dependency_links.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       39 2023-05-09 01:03:23.000000 onvif-gui-1.1.2/onvif_gui.egg-info/entry_points.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-05-09 01:03:23.000000 onvif-gui-1.1.2/onvif_gui.egg-info/requires.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       29 2023-05-09 01:03:23.000000 onvif-gui-1.1.2/onvif_gui.egg-info/top_level.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1659 2023-05-09 01:01:10.000000 onvif-gui-1.1.2/pyproject.toml
--rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-05-09 01:03:23.932168 onvif-gui-1.1.2/setup.cfg
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1504 2023-05-09 01:01:05.000000 onvif-gui-1.1.2/setup.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.928168 onvif-gui-1.1.2/yolox/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.932168 onvif-gui-1.1.2/yolox/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      936 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4894 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6647 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/darknet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2305 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6720 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/network_blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3104 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/yolo_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25526 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/yolo_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4158 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/yolo_pafpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1992 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/models/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.932168 onvif-gui-1.1.2/yolox/tracker/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/tracker/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      951 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/tracker/basetrack.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12172 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/tracker/byte_tracker.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9547 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/tracker/kalman_filter.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6158 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/tracker/matching.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-09 01:03:23.932168 onvif-gui-1.1.2/yolox/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      126 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1580 2023-05-08 23:51:04.000000 onvif-gui-1.1.2/yolox/utils/utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.034966 onvif-gui-1.1.3/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11357 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      217 2023-05-09 22:10:02.000000 onvif-gui-1.1.3/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-17 14:59:50.034966 onvif-gui-1.1.3/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8170 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.010965 onvif-gui-1.1.3/detectron2/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       67 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.010965 onvif-gui-1.1.3/detectron2/checkpoint/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/checkpoint/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17770 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/checkpoint/c2_model_loading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5685 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/checkpoint/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5258 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.010965 onvif-gui-1.1.3/detectron2/config/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      599 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/config/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7890 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/config/compat.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9211 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/config/config.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    29512 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/config/defaults.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3015 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/config/instantiate.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15378 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/config/lazy.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.010965 onvif-gui-1.1.3/detectron2/configs/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1318 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/configs/Base-RCNN-FPN.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.010965 onvif-gui-1.1.3/detectron2/configs/COCO-InstanceSegmentation/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:40:11.000000 onvif-gui-1.1.3/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      192 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.014965 onvif-gui-1.1.3/detectron2/configs/COCO-Keypoints/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      527 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:40:01.000000 onvif-gui-1.1.3/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/configs/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.014965 onvif-gui-1.1.3/detectron2/data/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      644 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7378 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/benchmark.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21231 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7224 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9162 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8169 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/dataset_mapper.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.014965 onvif-gui-1.1.3/detectron2/data/datasets/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      523 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10174 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/builtin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21841 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/builtin_meta.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13167 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/cityscapes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7821 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23465 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8977 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/coco_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9623 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/lvis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   223757 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   219177 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/lvis_v1_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    39414 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3128 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/pascal_voc.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      169 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/datasets/register_coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    22841 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/detection_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.014965 onvif-gui-1.1.3/detectron2/data/samplers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      412 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/samplers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11789 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/samplers/distributed_sampler.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1944 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.014965 onvif-gui-1.1.3/detectron2/data/transforms/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      466 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/transforms/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14112 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/transforms/augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23069 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/transforms/augmentation_impl.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12629 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/data/transforms/transform.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.018966 onvif-gui-1.1.3/detectron2/layers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      874 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5764 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/aspp.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12131 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/batch_norm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3024 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16978 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/deform_conv.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4202 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10879 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/mask_ops.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6490 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3098 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/roi_align.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3302 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/roi_align_rotated.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      652 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      537 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/shape_spec.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5123 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/layers/wrappers.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.018966 onvif-gui-1.1.3/detectron2/modeling/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1568 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15439 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/anchor_generator.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.018966 onvif-gui-1.1.3/detectron2/modeling/backbone/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      598 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2512 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/backbone.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1015 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10360 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15988 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/mvit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16656 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/regnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23658 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/resnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25095 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/swin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6360 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19338 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/backbone/vit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15123 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/box_regression.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/matcher.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.018966 onvif-gui-1.1.3/detectron2/modeling/meta_arch/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      508 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      814 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11651 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/dense_detector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13213 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/fcos.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10407 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13896 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18265 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9906 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10832 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/mmdet_wrapper.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11316 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/poolers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4045 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/postprocessing.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.018966 onvif-gui-1.1.3/detectron2/modeling/proposal_generator/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      231 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/proposal_generator/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      836 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/proposal_generator/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8128 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23814 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/proposal_generator/rpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8807 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.018966 onvif-gui-1.1.3/detectron2/modeling/roi_heads/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4077 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/box_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12990 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25390 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11156 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12169 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/mask_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    37701 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/roi_heads.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11175 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2334 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/sampling.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12416 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/modeling/test_time_augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1780 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/predictor.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.022966 onvif-gui-1.1.3/detectron2/structures/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/structures/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14429 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/structures/boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5520 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/structures/image_list.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6613 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/structures/instances.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/structures/keypoints.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19802 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/structures/masks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18853 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/structures/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2707 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/tracker.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.022966 onvif-gui-1.1.3/detectron2/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       51 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6017 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/analysis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8391 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/collect_env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4096 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/colormap.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5608 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/comm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1852 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/develop.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5644 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17022 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/events.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1189 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/file_io.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7807 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/logger.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2583 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/memory.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1874 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/registry.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1064 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/serialize.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18113 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/testing.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11319 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/video_visualizer.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    51159 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/detectron2/utils/visualizer.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.022966 onvif-gui-1.1.3/gui/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.022966 onvif-gui-1.1.3/gui/components/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/components/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1777 2023-05-13 16:10:05.000000 onvif-gui-1.1.3/gui/components/comboselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2397 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/components/directoryselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2118 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/components/fileselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5393 2023-05-13 16:10:05.000000 onvif-gui-1.1.3/gui/components/labelselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4077 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/components/progress.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1918 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/components/thresholdslider.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1996 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/glwidget.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14379 2023-05-17 14:57:45.000000 onvif-gui-1.1.3/gui/main.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.022966 onvif-gui-1.1.3/gui/onvif/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      191 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/onvif/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/onvif/admintab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3959 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/onvif/imagetab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2425 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/onvif/logindialog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5247 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/onvif/networktab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5118 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/onvif/ptztab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4527 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/onvif/videotab.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.022966 onvif-gui-1.1.3/gui/panels/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      180 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/panels/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3624 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/panels/audiopanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13463 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/panels/camerapanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14483 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/panels/filepanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12913 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/panels/settingspanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3627 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/panels/videopanel.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.030966 onvif-gui-1.1.3/gui/resources/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1936 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/apply.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/apply_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/apply_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/audio.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/audio_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/audio_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/branch_closed.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/branch_closed_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/branch_closed_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/branch_open.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/branch_open_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/branch_open_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/checked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/checked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/checked_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12716 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/darkstyle.qss
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/discover.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/discover_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/discover_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/fast-forward.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/fast-forward_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/fast-forward_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/mute.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/mute_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/mute_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/next.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/next_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/next_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/onvif-gui.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/pause.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/pause_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/pause_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/play.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/play_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/play_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/previous.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/previous_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/previous_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/radio-off.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/radio-off_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/radio-off_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/radio-on.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/radio-on_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/radio-on_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/record.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/record_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/record_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/recording.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/recording_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/recording_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/rewind.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/rewind_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/rewind_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/small_arrow_left.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/small_arrow_left_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/small_arrow_left_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/small_arrow_up.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/small_arrow_up_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/small_arrow_up_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/stop.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/stop_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/stop_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/unchecked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/unchecked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/gui/resources/unchecked_lo.png
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.030966 onvif-gui-1.1.3/modules/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/modules/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.030966 onvif-gui-1.1.3/modules/audio/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/modules/audio/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3404 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/modules/audio/sample.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.030966 onvif-gui-1.1.3/modules/video/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.3/modules/video/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6913 2023-05-13 16:10:05.000000 onvif-gui-1.1.3/modules/video/keypoint.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4768 2023-05-13 16:10:05.000000 onvif-gui-1.1.3/modules/video/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3095 2023-05-13 16:10:05.000000 onvif-gui-1.1.3/modules/video/sample.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7423 2023-05-13 16:10:05.000000 onvif-gui-1.1.3/modules/video/segment.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10423 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/modules/video/yolov7.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8066 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/modules/video/yolov8.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12095 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/modules/video/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.030966 onvif-gui-1.1.3/onvif_gui.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-17 14:59:49.000000 onvif-gui-1.1.3/onvif_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7994 2023-05-17 14:59:50.000000 onvif-gui-1.1.3/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-17 14:59:49.000000 onvif-gui-1.1.3/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-17 14:59:49.000000 onvif-gui-1.1.3/onvif_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-17 14:59:49.000000 onvif-gui-1.1.3/onvif_gui.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       37 2023-05-17 14:59:49.000000 onvif-gui-1.1.3/onvif_gui.egg-info/top_level.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1659 2023-05-17 14:57:33.000000 onvif-gui-1.1.3/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-17 14:59:50.034966 onvif-gui-1.1.3/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1504 2023-05-17 14:57:27.000000 onvif-gui-1.1.3/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.034966 onvif-gui-1.1.3/tracker/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/tracker/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      951 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/tracker/basetrack.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12295 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/tracker/byte_tracker.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9547 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/tracker/kalman_filter.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6127 2023-05-16 21:11:27.000000 onvif-gui-1.1.3/tracker/matching.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.034966 onvif-gui-1.1.3/yolox/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.034966 onvif-gui-1.1.3/yolox/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      936 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4894 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6647 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/darknet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2305 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6720 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/network_blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3104 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/yolo_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25526 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/yolo_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4158 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/yolo_pafpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1992 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/models/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 14:59:50.034966 onvif-gui-1.1.3/yolox/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      126 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1580 2023-05-08 16:34:27.000000 onvif-gui-1.1.3/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.1.2/LICENSE` & `onvif-gui-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/PKG-INFO` & `onvif-gui-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.1.2
+Version: 1.1.3
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.1.2/README.md` & `onvif-gui-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.1.3/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/checkpoint/catalog.py` & `onvif-gui-1.1.3/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.1.3/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/config/__init__.py` & `onvif-gui-1.1.3/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/config/compat.py` & `onvif-gui-1.1.3/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/config/config.py` & `onvif-gui-1.1.3/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/config/defaults.py` & `onvif-gui-1.1.3/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/config/instantiate.py` & `onvif-gui-1.1.3/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/config/lazy.py` & `onvif-gui-1.1.3/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.1.3/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.1.3/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/__init__.py` & `onvif-gui-1.1.3/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/benchmark.py` & `onvif-gui-1.1.3/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/build.py` & `onvif-gui-1.1.3/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/catalog.py` & `onvif-gui-1.1.3/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/common.py` & `onvif-gui-1.1.3/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/dataset_mapper.py` & `onvif-gui-1.1.3/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/__init__.py` & `onvif-gui-1.1.3/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/builtin.py` & `onvif-gui-1.1.3/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.1.3/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.1.3/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.1.3/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/coco.py` & `onvif-gui-1.1.3/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.1.3/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/lvis.py` & `onvif-gui-1.1.3/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.1.3/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.1.3/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.1.3/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.1.3/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/detection_utils.py` & `onvif-gui-1.1.3/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.1.3/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.1.3/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.1.3/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.1.3/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/data/transforms/transform.py` & `onvif-gui-1.1.3/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/__init__.py` & `onvif-gui-1.1.3/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/aspp.py` & `onvif-gui-1.1.3/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/batch_norm.py` & `onvif-gui-1.1.3/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/blocks.py` & `onvif-gui-1.1.3/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/deform_conv.py` & `onvif-gui-1.1.3/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/losses.py` & `onvif-gui-1.1.3/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/mask_ops.py` & `onvif-gui-1.1.3/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/nms.py` & `onvif-gui-1.1.3/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/roi_align.py` & `onvif-gui-1.1.3/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.1.3/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.1.3/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/shape_spec.py` & `onvif-gui-1.1.3/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/layers/wrappers.py` & `onvif-gui-1.1.3/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/__init__.py` & `onvif-gui-1.1.3/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.1.3/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/build.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.1.3/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/box_regression.py` & `onvif-gui-1.1.3/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/matcher.py` & `onvif-gui-1.1.3/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.1.3/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.1.3/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.1.3/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.1.3/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.1.3/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.1.3/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.1.3/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.1.3/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/poolers.py` & `onvif-gui-1.1.3/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/postprocessing.py` & `onvif-gui-1.1.3/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.1.3/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.1.3/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.1.3/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.1.3/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.1.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/sampling.py` & `onvif-gui-1.1.3/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.1.3/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/predictor.py` & `onvif-gui-1.1.3/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/structures/__init__.py` & `onvif-gui-1.1.3/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/structures/boxes.py` & `onvif-gui-1.1.3/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/structures/image_list.py` & `onvif-gui-1.1.3/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/structures/instances.py` & `onvif-gui-1.1.3/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/structures/keypoints.py` & `onvif-gui-1.1.3/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/structures/masks.py` & `onvif-gui-1.1.3/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.1.3/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/tracker.py` & `onvif-gui-1.1.3/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/analysis.py` & `onvif-gui-1.1.3/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/collect_env.py` & `onvif-gui-1.1.3/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/colormap.py` & `onvif-gui-1.1.3/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/comm.py` & `onvif-gui-1.1.3/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/develop.py` & `onvif-gui-1.1.3/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/env.py` & `onvif-gui-1.1.3/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/events.py` & `onvif-gui-1.1.3/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/file_io.py` & `onvif-gui-1.1.3/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/logger.py` & `onvif-gui-1.1.3/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/memory.py` & `onvif-gui-1.1.3/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/registry.py` & `onvif-gui-1.1.3/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/serialize.py` & `onvif-gui-1.1.3/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/testing.py` & `onvif-gui-1.1.3/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/video_visualizer.py` & `onvif-gui-1.1.3/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/detectron2/utils/visualizer.py` & `onvif-gui-1.1.3/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/components/comboselector.py` & `onvif-gui-1.1.3/gui/components/comboselector.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.cmbBox.setCurrentText(self.mw.settings.value(self.selectKey, select))
         self.cmbBox.currentTextChanged.connect(self.cmbBoxChanged)
 
         lblBox = QLabel(name)
         lytBox = QGridLayout(self)
         lytBox.addWidget(lblBox,       0, 0, 1, 1)
         lytBox.addWidget(self.cmbBox,  0, 1, 1, 1)
+        lytBox.setColumnStretch(1, 10)
         lytBox.setContentsMargins(0, 0, 0, 0)
 
     def cmbBoxChanged(self, text):
         self.mw.settings.setValue(self.selectKey, text)
 
     def currentText(self):
         return self.cmbBox.currentText()
```

### Comparing `onvif-gui-1.1.2/gui/components/directoryselector.py` & `onvif-gui-1.1.3/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/components/fileselector.py` & `onvif-gui-1.1.3/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/components/labelselector.py` & `onvif-gui-1.1.3/gui/components/labelselector.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,30 @@
 
 from PyQt6.QtWidgets import QPushButton, QColorDialog, \
 QGridLayout, QWidget, QCheckBox, QLabel, QComboBox
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QColor
 
 class LabelSelector(QWidget):
-    def __init__(self, mw, name, index):
+    def __init__(self, mw, name, index, labels=None):
         super().__init__()
+
         self.labels = [ "person", "bicycle", "car", "motorcycle", "airplane", "bus", "train", "truck", 
                         "boat", "traffic light", "fire hydrant", "stop sign", "parking meter", "bench",
                         "bird", "cat", "dog", "horse", "sheep", "cow", "elephant", "bear",  "zebra",
                         "giraffe", "backpack", "umbrella", "handbag", "tie", "suitcase", "frisbee", "skis",
                         "snowboard", "sports ball", "kite", "baseball bat", "baseball glove", "skateboard",
                         "surfboard", "tennis racket", "bottle", "wine glass", "cup", "fork", "knife",
                         "spoon", "bowl", "banana", "apple", "sandwich", "orange", "broccoli", "carrot",
                         "hot dog", "pizza", "donut", "cake", "chair", "couch", "potted plant", "bed",
                         "dining table", "toilet", "tv", "laptop", "mouse", "remote", "keyboard",
                         "cell phone", "microwave", "oven", "toaster", "sink", "refrigerator", "book",
                         "clock", "vase", "scissors", "teddy bear", "hair drier", "toothbrush" ]
+        if labels is not None:
+            self.labels = labels
         
         self.mw = mw
         self.index = index
         self.colorKey = "Module/" + name + "/color" + str(index)
         self.enabledKey = "Module/" + name + "/enabled" + str(index)
         self.labelKey = "Module/" + name + "/label" + str(index)
         self.idleColor = QColor("#3B3B3B")
```

### Comparing `onvif-gui-1.1.2/gui/components/progress.py` & `onvif-gui-1.1.3/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/components/thresholdslider.py` & `onvif-gui-1.1.3/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/glwidget.py` & `onvif-gui-1.1.3/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/main.py` & `onvif-gui-1.1.3/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
         QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
-        self.program_name = "onvif gui version 1.1.2"
+        self.program_name = "onvif gui version 1.1.3"
         self.setWindowTitle(self.program_name)
         self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
@@ -156,15 +156,15 @@
     def loadVideoWorker(self, workerName):
         spec = importlib.util.spec_from_file_location("VideoWorker", self.videoPanel.dirModules.text() + "/" + workerName)
         self.videoHook = importlib.util.module_from_spec(spec)
         sys.modules["VideoWorker"] = self.videoHook
         spec.loader.exec_module(self.videoHook)
         self.worker = None
 
-    def pythonCallback(self, F):
+    def pyVideoCallback(self, F):
         if self.videoPanel.chkEngage.isChecked():
             if self.videoHook is not None:
                 if self.worker is None:
                     self.worker = self.videoHook.VideoWorker(self)
                 start = time.time()
                 self.worker(F)
                 finish = time.time()
@@ -238,15 +238,15 @@
                 self.player.renderCallback = lambda F : self.glWidget.renderCallback(F)
             else:
                 self.player.hWnd = self.glWidget.winId()
 
         self.player.disable_audio = self.settingsPanel.chkDisableAudio.isChecked()
         self.player.disable_video = self.settingsPanel.chkDisableVideo.isChecked()
 
-        self.player.pythonCallback = lambda F : self.pythonCallback(F)
+        self.player.pythonCallback = lambda F : self.pyVideoCallback(F)
         self.player.pyAudioCallback = lambda F: self.pyAudioCallback(F)
         self.player.cbMediaPlayingStarted = lambda n : self.mediaPlayingStarted(n)
         self.player.cbMediaPlayingStopped = lambda : self.mediaPlayingStopped()
         self.player.errorCallback = lambda s : self.errorCallback(s)
         self.player.infoCallback = lambda s : self.infoCallback(s)
         self.player.setVolume(int(self.volume))
         self.player.setMute(self.mute)
```

### Comparing `onvif-gui-1.1.2/gui/onvif/admintab.py` & `onvif-gui-1.1.3/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/onvif/imagetab.py` & `onvif-gui-1.1.3/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/onvif/logindialog.py` & `onvif-gui-1.1.3/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/onvif/networktab.py` & `onvif-gui-1.1.3/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/onvif/ptztab.py` & `onvif-gui-1.1.3/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/onvif/videotab.py` & `onvif-gui-1.1.3/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/panels/audiopanel.py` & `onvif-gui-1.1.3/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/panels/camerapanel.py` & `onvif-gui-1.1.3/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/panels/filepanel.py` & `onvif-gui-1.1.3/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/panels/settingspanel.py` & `onvif-gui-1.1.3/gui/panels/settingspanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/panels/videopanel.py` & `onvif-gui-1.1.3/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/LICENSE` & `onvif-gui-1.1.3/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/audio.png` & `onvif-gui-1.1.3/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/audio_hi.png` & `onvif-gui-1.1.3/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/audio_lo.png` & `onvif-gui-1.1.3/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/darkstyle.qss` & `onvif-gui-1.1.3/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/discover.png` & `onvif-gui-1.1.3/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/discover_hi.png` & `onvif-gui-1.1.3/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/discover_lo.png` & `onvif-gui-1.1.3/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/mute.png` & `onvif-gui-1.1.3/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/mute_lo.png` & `onvif-gui-1.1.3/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/onvif-gui.png` & `onvif-gui-1.1.3/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/gui/resources/recording_lo.png` & `onvif-gui-1.1.3/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/modules/audio/sample.py` & `onvif-gui-1.1.3/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/modules/video/keypoint.py` & `onvif-gui-1.1.3/modules/video/keypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 IMPORT_ERROR = ""
 try:
     import numpy as np
     import cv2
     import math
     import os
-    from distutils.sysconfig import get_python_lib
+    import sys
     from loguru import logger
-    from sys import platform
     from pathlib import Path
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
     from gui.components import ThresholdSlider
 
     import torch
     from detectron2.config import get_cfg
     from detectron2.predictor import Predictor
@@ -50,19 +49,18 @@
         self.sldThreshold.setEnabled(False)
 
     def enableThresholdSlider(self):
         self.sldThreshold.setEnabled(True)
 
 class VideoWorker:
     def __init__(self, mw):
-        self.mw = mw
-        self.last_ex = ""
-        self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
-
         try:
+            self.mw = mw
+            self.last_ex = ""
+            self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
             ckpt_file = "auto"
             fp16 = True
             self.no_back = True
             self.simple = True
 
             if ckpt_file is not None:
                 if ckpt_file.lower() == "auto":
@@ -71,18 +69,24 @@
                     cache = Path(ckpt_file)
 
                     if not cache.is_file():
                         cache.parent.mkdir(parents=True, exist_ok=True)
                         torch.hub.download_url_to_file("https://dl.fbaipublicfiles.com/detectron2/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x/137849621/model_final_a6e10b.pkl", ckpt_file)
 
             cfg = get_cfg()
-            working_dir = get_python_lib()
+            config_file = ""
             yaml_file = 'detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml'
-            config_file = os.path.join(working_dir, yaml_file)
-            assert(os.path.isfile(config_file))
+            if not os.path.isfile(yaml_file):
+                for path in sys.path:
+                    config_file = os.path.join(path, yaml_file)
+                    if os.path.isfile(config_file):
+                        break
+            else:
+                config_file = yaml_file
+
             cfg.merge_from_file(config_file)
             cfg.MODEL.RETINANET.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.WEIGHTS = ckpt_file
             cfg.MODEL.PANOPTIC_FPN.COMBINE.INSTANCES_CONFIDENCE_THRESH = self.CONFIDENCE_THRESHOLD
             cfg.freeze()
 
@@ -115,21 +119,21 @@
             if len(detected):
                 colors = np.asarray(self.tracker.assign_colors(detected)) * 255
                 colors = colors.astype(np.int32)
                 for idx, keypoint in enumerate(keypoints):
                     self.draw_keypoint(img, keypoint, colors[idx])
 
         except Exception as ex:
-            if self.last_ex != str(ex):
+            if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception("Keypoints runtime error")
             self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
         filename = None
-        if platform == "win32":
+        if sys.platform == "win32":
             filename = os.environ['HOMEPATH'] + "/.cache/torch/hub/checkpoints/model_final_a6e10b.pkl"
         else:
             filename = os.environ['HOME'] + "/.cache/torch/hub/checkpoints/model_final_a6e10b.pkl"
         return filename
 
     def draw_keypoint(self, img, keypoint, color):
         color = (int(color[0]), int(color[1]), int(color[2]))
```

### Comparing `onvif-gui-1.1.2/modules/video/retinanet.py` & `onvif-gui-1.1.3/modules/video/retinanet.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
                 QMessageBox.critical(None, "Retinanet Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
 
         except:
             logger.exception("retinanet configuration load error")
 
 class VideoWorker:
     def __init__(self, mw):
-        self.mw = mw
-        self.last_ex = ""
         try:
+            self.mw = mw
+            self.last_ex = ""
             self.model = torchvision.models.detection.retinanet_resnet50_fpn(weights=torchvision.models.detection.RetinaNet_ResNet50_FPN_Weights.DEFAULT)            
             self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
             self.model.eval().to(self.device)
         except:
             logger.exception("retinanet worker load error")
 
     def __call__(self, F):
@@ -91,17 +91,14 @@
             img = np.array(F, copy = False)
             tensor = transform(img).to(self.device)
             tensor = tensor.unsqueeze(0)
 
             with torch.no_grad():
                 outputs = self.model(tensor)
 
-            if self.mw.configure.name != MODULE_NAME:
-                return
-
             threshold = self.mw.configure.sldThreshold.value()
             scores = outputs[0]['scores'].detach().cpu().numpy()
             labels = outputs[0]['labels'].detach().cpu().numpy()
             boxes = outputs[0]['boxes'].detach().cpu().numpy()
 
             labels = labels[np.array(scores) >= threshold]
             boxes = boxes[np.array(scores) >= threshold].astype(np.int32)
@@ -114,11 +111,11 @@
                     b = lbl.color()[2]
                     lbl.setCount(lbl_boxes.shape[0])
 
                     for box in lbl_boxes:
                         cv2.rectangle(img, (box[0], box[1]), (box[2], box[3]), (r, g, b), 2)
 
         except Exception as ex:
-            if self.last_ex != str(ex):
+            if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception("retinanet worker call error")
             self.last_ex = str(ex)
```

### Comparing `onvif-gui-1.1.2/modules/video/sample.py` & `onvif-gui-1.1.3/modules/video/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,21 @@
     def chkShowBorderClicked(self, state):
         self.mw.settings.setValue(self.showBorderKey, state)
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
+            self.last_ex = ""
+
         except:
             logger.exception("sample worker failed to load")
 
     def __call__(self, F):
         try:
-            if self.mw.configure.name != MODULE_NAME:
-                return
-            
             img = np.array(F, copy = False)
             milliseconds = F.m_rts
             seconds, milliseconds = divmod(milliseconds, 1000)
             minutes, seconds = divmod(seconds, 60)
             timestamp = f'{int(minutes):02d}:{int(seconds):02d}.{int(milliseconds/100):01d}'
 
             imgWidth = img.shape[1]
@@ -72,9 +71,12 @@
             textY = max((imgHeight / 2) + (textHeight / 2), 0)
 
             color = (255, 255, 255)
             if self.mw.player.isRecording():
                 color = (255, 0, 0)
 
             cv2.putText(img, timestamp, (int(textX), int(textY)), cv2.FONT_HERSHEY_PLAIN, 12, color, 12)
-        except:
-            logger.exception("sample worker call error")
+
+        except Exception as ex:
+            if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
+                logger.exception("sample worker call error")
+            self.last_ex = str(ex)
```

### Comparing `onvif-gui-1.1.2/modules/video/segment.py` & `onvif-gui-1.1.3/modules/video/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 
 IMPORT_ERROR = ""
 try:
     import numpy as np
     import os
     import cv2
-    from distutils.sysconfig import get_python_lib
+    import sys
     from loguru import logger
-    from sys import platform
     from pathlib import Path
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QMessageBox
     from PyQt6.QtCore import Qt
     from gui.components import ThresholdSlider, LabelSelector
 
     import torch
     from detectron2.config import get_cfg
@@ -68,19 +67,18 @@
         self.sldThreshold.setEnabled(False)
 
     def enableThresholdSlider(self):
         self.sldThreshold.setEnabled(True)
 
 class VideoWorker:
     def __init__(self, mw):
-        self.mw = mw
-        self.last_ex = ""
-        self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
-
         try:
+            self.mw = mw
+            self.last_ex = ""
+            self.CONFIDENCE_THRESHOLD = self.mw.configure.sldThreshold.value()
             ckpt_file = 'auto'
             fp16 = True
             self.simple = True
             self.draw_overlay = False
             self.first_pass = True
 
             if ckpt_file is not None:
@@ -90,18 +88,24 @@
                     cache = Path(ckpt_file)
 
                     if not cache.is_file():
                         cache.parent.mkdir(parents=True, exist_ok=True)
                         torch.hub.download_url_to_file("https://dl.fbaipublicfiles.com/detectron2/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl", ckpt_file)
 
             cfg = get_cfg()
-            working_dir = get_python_lib()
+            config_file = ""
             yaml_file = 'detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml'
-            config_file = os.path.join(working_dir, yaml_file)
-            assert(os.path.isfile(config_file))
+            if not os.path.isfile(yaml_file):
+                for path in sys.path:
+                    config_file = os.path.join(path, yaml_file)
+                    if os.path.isfile(config_file):
+                        break
+            else:
+                config_file = yaml_file
+
             cfg.merge_from_file(config_file)
             cfg.MODEL.WEIGHTS = ckpt_file
 
             cfg.MODEL.RETINANET.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = self.CONFIDENCE_THRESHOLD
             cfg.MODEL.PANOPTIC_FPN.COMBINE.INSTANCES_CONFIDENCE_THRESH = self.CONFIDENCE_THRESHOLD
             cfg.freeze()
@@ -126,17 +130,14 @@
             img = np.array(F, copy=False)
 
             predictions = self.predictor(img)["instances"]
 
             test_classes = predictions.pred_classes.cpu().numpy()
             test_boxes = predictions.pred_boxes.tensor.cpu().numpy().astype(int)
 
-            if self.mw.configure.name != MODULE_NAME:
-                return
-
             masks = []
             classes = []
             boxes = []
             filter_classes = []
             counts = {}
             for lbl in self.mw.configure.labels:
                 if lbl.isChecked():
@@ -169,21 +170,21 @@
 
             for index, box in enumerate(boxes):
                 color = (colors[index] * 255).astype(int).tolist()
                 #cv2.rectangle(img, (box[0], box[1]), (box[2], box[3]), color, 2)
                 cv2.line(img, (box[0], box[3]), (box[2], box[3]), color, 2)
 
         except Exception as ex:
-            if self.last_ex != str(ex):
+            if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception("Instance Segmentation runtime error")
             self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
         filename = None
-        if platform == "win32":
+        if sys.platform == "win32":
             filename = os.environ['HOMEPATH'] + "/.cache/torch/hub/checkpoints/model_final_f10217.pkl"
         else:
             filename = os.environ['HOME'] + "/.cache/torch/hub/checkpoints/model_final_f10217.pkl"
         return filename
 
 
     def stopped(self):
```

### Comparing `onvif-gui-1.1.2/modules/video/yolox.py` & `onvif-gui-1.1.3/modules/video/yolox.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox
     from PyQt6.QtCore import Qt
 
     import torch
     from torchvision.transforms import functional
     import torch.nn as nn
-
+    
     from yolox.models import YOLOX, YOLOPAFPN, YOLOXHead
     from yolox.utils import postprocess
-    from yolox.tracker.byte_tracker import BYTETracker
+    from tracker.byte_tracker import BYTETracker
 
 except ModuleNotFoundError as ex:
     IMPORT_ERROR = str(ex)
     print("Import Error has occurred, missing modules need to be installed, please consult documentation: ", ex)
 
 os.environ['KMP_DUPLICATE_LIB_OK']='True'
 MODULE_NAME = "yolox"
@@ -70,15 +70,15 @@
             self.chkFP16.stateChanged.connect(self.chkFP16Clicked)
 
             self.chkTrack = QCheckBox("Track Objects")
             self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
             self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
-            self.sldConfThre.setEnabled(not self.chkTrack.isChecked())
+            #self.sldConfThre.setEnabled(not self.chkTrack.isChecked())
 
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
                 self.labels.append(LabelSelector(mw, MODULE_NAME, i+1))
             pnlLabels = QWidget()
             lytLabels = QGridLayout(pnlLabels)
@@ -87,40 +87,40 @@
             lytLabels.addWidget(lblPanel,        0, 0, 1, 1)
             for i in range(number_of_labels):
                 lytLabels.addWidget(self.labels[i], i+1, 0, 1, 1)
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.chkAuto,      0, 0, 1, 1)
-            lytMain.addWidget(self.txtFilename,  1, 0, 1, 1)
-            lytMain.addWidget(self.cmbRes,       2, 0, 1, 1)
-            lytMain.addWidget(self.cmbType,      3, 0, 1, 1)
+            lytMain.addWidget(self.cmbType,      1, 0, 1, 1)
+            lytMain.addWidget(self.txtFilename,  2, 0, 1, 1)
+            lytMain.addWidget(self.cmbRes,       3, 0, 1, 1)
             lytMain.addWidget(self.sldConfThre,  4, 0, 1, 1)
             lytMain.addWidget(self.chkFP16,      5, 0, 1, 1)
             lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
             lytMain.addWidget(pnlLabels,         7, 0, 1, 1)
             lytMain.addWidget(QLabel(),          8, 0, 1, 1)
             lytMain.setRowStretch(8, 10)
 
             if len(IMPORT_ERROR) > 0:
-                QMessageBox.critical(None, "YOLOX Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
+                QMessageBox.critical(None, MODULE_NAME + " Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
 
         except:
-            logger.exception("yolox configure failed to load")
+            logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
     def chkFP16Clicked(self, state):
         self.mw.settings.setValue(self.fp16Key, state)
 
     def chkTrackClicked(self, state):
         self.mw.settings.setValue(self.trackKey, state)
-        self.sldConfThre.setEnabled(not self.chkTrack.isChecked())
+        #self.sldConfThre.setEnabled(not self.chkTrack.isChecked())
 
 class VideoWorker:
     def __init__(self, mw):
         try:
             self.mw = mw
             self.last_ex = ""
             device_name = "cpu"
@@ -129,31 +129,26 @@
             self.device = torch.device(device_name)
 
             self.num_classes = 80
 
             self.fp16 = self.mw.configure.chkFP16.isChecked()
             self.track = self.mw.configure.chkTrack.isChecked()
 
-            track_thresh = 0.5
-            track_buffer = 30
-            match_thresh = 0.8
-
             size = {'yolox_s': [0.33, 0.50], 
                     'yolox_m': [0.67, 0.75],
                     'yolox_l': [1.00, 1.00],
                     'yolox_x': [1.33, 1.25]}[self.mw.configure.cmbType.currentText()]
 
             self.model = None
             self.model = self.get_model(self.num_classes, size[0], size[1], None).to(self.device)
             self.model.eval()
 
             self.ckpt_file = None
             if self.mw.configure.chkAuto.isChecked():
                 self.ckpt_file = self.get_auto_ckpt_filename()
-                print("cpkt_file:", self.ckpt_file)
                 cache = Path(self.ckpt_file)
 
                 if not cache.is_file():
                     cache.parent.mkdir(parents=True, exist_ok=True)
                     model_name = self.mw.configure.cmbType.currentText()
                     link = "https://github.com/Megvii-BaseDetection/YOLOX/releases/download/0.1.1rc0/" + model_name + ".pth"
                     torch.hub.download_url_to_file(link, self.ckpt_file)
@@ -161,18 +156,22 @@
                 self.ckpt_file = self.mw.configure.txtFilename.text()
 
             self.model.load_state_dict(torch.load(self.ckpt_file, map_location="cpu")["model"])
 
             if self.fp16:
                 self.model = self.model.half()
 
-            self.tracker = BYTETracker(track_thresh, track_buffer, match_thresh)
+            self.track_thresh = self.mw.configure.sldConfThre.value()
+            self.track_buffer = 30
+            self.match_thresh = 0.8
+
+            self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
 
         except:
-            logger.exception("yolox initialization failure")
+            logger.exception(MODULE_NAME + " initialization failure")
 
     def __call__(self, F):
         try:
             img = np.array(F, copy=False)
             
             res = int(self.mw.configure.cmbRes.currentText())
             test_size = (res, res)
@@ -195,15 +194,14 @@
             if self.mw.configure.chkAuto.isChecked():
                 tmp = self.get_auto_ckpt_filename()
             else:
                 tmp = self.mw.configure.txtFilename.text()
             if self.ckpt_file != tmp:
                 self.__init__(self.mw)
 
-
             if self.mw.configure.chkTrack.isChecked():
                 confthre = 0.001
             else:
                 confthre = self.mw.configure.sldConfThre.value()
             
             nmsthre = 0.65
 
@@ -212,31 +210,34 @@
                 if lbl.chkBox.isChecked():
                     label_filter.append(lbl.label())
 
             with torch.no_grad():
                 outputs = self.model(timg)
                 outputs = postprocess(outputs, self.num_classes, confthre, nmsthre)
 
-            if self.mw.configure.name != MODULE_NAME:
-                return
-            
             if outputs[0] is not None:
                 output = outputs[0].cpu()
                 if self.mw.configure.chkTrack.isChecked():
                     labels = output[:, 6].numpy().astype(int)
                     mask = np.in1d(labels, label_filter)
                     output = output[mask]
+                    output = output.cpu().numpy()
+                    
+                    if self.track_thresh != self.mw.configure.sldConfThre.value():
+                        self.track_thresh = self.mw.configure.sldConfThre.value()
+                        self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
+
                     online_targets = self.tracker.update(output, [img.shape[0], img.shape[1]], test_size)
                     self.draw_track_boxes(img, online_targets)
                 else:
                     self.draw_plain_boxes(img, output, ratio)
 
         except Exception as ex:
-            if self.last_ex != str(ex):
-                logger.exception("yolox runtime error")
+            if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
+                logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
 
     def draw_plain_boxes(self, img, output, ratio):
         boxes = output[:, 0:4] / ratio
         labels = output[:, 6].numpy().astype(int)
         for lbl in self.mw.configure.labels:
             if lbl.chkBox.isChecked():
```

### Comparing `onvif-gui-1.1.2/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.1.3/onvif_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.1.2
+Version: 1.1.3
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.1.2/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.1.3/onvif_gui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -220,31 +220,33 @@
 modules/audio/__init__.py
 modules/audio/sample.py
 modules/video/__init__.py
 modules/video/keypoint.py
 modules/video/retinanet.py
 modules/video/sample.py
 modules/video/segment.py
+modules/video/yolov7.py
+modules/video/yolov8.py
 modules/video/yolox.py
 onvif_gui.egg-info/PKG-INFO
 onvif_gui.egg-info/SOURCES.txt
 onvif_gui.egg-info/dependency_links.txt
 onvif_gui.egg-info/entry_points.txt
 onvif_gui.egg-info/requires.txt
 onvif_gui.egg-info/top_level.txt
+tracker/__init__.py
+tracker/basetrack.py
+tracker/byte_tracker.py
+tracker/kalman_filter.py
+tracker/matching.py
 yolox/__init__.py
 yolox/models/__init__.py
 yolox/models/build.py
 yolox/models/darknet.py
 yolox/models/losses.py
 yolox/models/network_blocks.py
 yolox/models/yolo_fpn.py
 yolox/models/yolo_head.py
 yolox/models/yolo_pafpn.py
 yolox/models/yolox.py
-yolox/tracker/__init__.py
-yolox/tracker/basetrack.py
-yolox/tracker/byte_tracker.py
-yolox/tracker/kalman_filter.py
-yolox/tracker/matching.py
 yolox/utils/__init__.py
 yolox/utils/utils.py
```

### Comparing `onvif-gui-1.1.2/pyproject.toml` & `onvif-gui-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.1.2"  
+version = "1.1.3"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.1.2/setup.py` & `onvif-gui-1.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.1.2",
+    version="1.1.3",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.1.2/yolox/models/__init__.py` & `onvif-gui-1.1.3/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/build.py` & `onvif-gui-1.1.3/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/darknet.py` & `onvif-gui-1.1.3/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/losses.py` & `onvif-gui-1.1.3/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/network_blocks.py` & `onvif-gui-1.1.3/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/yolo_fpn.py` & `onvif-gui-1.1.3/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/yolo_head.py` & `onvif-gui-1.1.3/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/yolo_pafpn.py` & `onvif-gui-1.1.3/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/models/yolox.py` & `onvif-gui-1.1.3/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/tracker/basetrack.py` & `onvif-gui-1.1.3/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/tracker/byte_tracker.py` & `onvif-gui-1.1.3/tracker/byte_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from .kalman_filter import KalmanFilter
-from yolox.tracker import matching
+from .matching import iou_distance, linear_assignment, fuse_score
 from .basetrack import BaseTrack, TrackState
 
 class STrack(BaseTrack):
     shared_kalman = KalmanFilter()
     def __init__(self, tlwh, score, label):
 
         # wait activate
@@ -156,19 +156,20 @@
     def update(self, output_results, img_info, img_size):
         self.frame_id += 1
         activated_starcks = []
         refind_stracks = []
         lost_stracks = []
         removed_stracks = []
 
-        if output_results.shape[1] == 5:
+        #output_results = output_results.cpu().numpy()
+        if output_results.shape[1] == 6:
             scores = output_results[:, 4]
             bboxes = output_results[:, :4]
+            labels = output_results[:, 5]
         else:
-            output_results = output_results.cpu().numpy()
             scores = output_results[:, 4] * output_results[:, 5]
             bboxes = output_results[:, :4]  # x1y1x2y2
             labels = output_results[:, 6].astype(int)
 
         img_h, img_w = img_info[0], img_info[1]
         scale = min(img_size[0] / float(img_h), img_size[1] / float(img_w))
         bboxes /= scale
@@ -201,20 +202,20 @@
             else:
                 tracked_stracks.append(track)
 
         ''' Step 2: First association, with high score detection boxes'''
         strack_pool = joint_stracks(tracked_stracks, self.lost_stracks)
         # Predict the current location with KF
         STrack.multi_predict(strack_pool)
-        dists = matching.iou_distance(strack_pool, detections)
+        dists = iou_distance(strack_pool, detections)
         
         #if not self.args.mot20:
-        dists = matching.fuse_score(dists, detections)
+        dists = fuse_score(dists, detections)
         
-        matches, u_track, u_detection = matching.linear_assignment(dists, thresh=self.match_thresh)
+        matches, u_track, u_detection = linear_assignment(dists, thresh=self.match_thresh)
 
         for itracked, idet in matches:
             track = strack_pool[itracked]
             det = detections[idet]
             if track.state == TrackState.Tracked:
                 track.update(detections[idet], self.frame_id)
                 activated_starcks.append(track)
@@ -227,16 +228,16 @@
         if len(dets_second) > 0:
             '''Detections'''
             detections_second = [STrack(STrack.tlbr_to_tlwh(tlbr), s, l) for
                           (tlbr, s, l) in zip(dets_second, scores_second, labels_second)]
         else:
             detections_second = []
         r_tracked_stracks = [strack_pool[i] for i in u_track if strack_pool[i].state == TrackState.Tracked]
-        dists = matching.iou_distance(r_tracked_stracks, detections_second)
-        matches, u_track, u_detection_second = matching.linear_assignment(dists, thresh=0.5)
+        dists = iou_distance(r_tracked_stracks, detections_second)
+        matches, u_track, u_detection_second = linear_assignment(dists, thresh=0.5)
         for itracked, idet in matches:
             track = r_tracked_stracks[itracked]
             det = detections_second[idet]
             if track.state == TrackState.Tracked:
                 track.update(det, self.frame_id)
                 activated_starcks.append(track)
             else:
@@ -247,20 +248,20 @@
             track = r_tracked_stracks[it]
             if not track.state == TrackState.Lost:
                 track.mark_lost()
                 lost_stracks.append(track)
 
         '''Deal with unconfirmed tracks, usually tracks with only one beginning frame'''
         detections = [detections[i] for i in u_detection]
-        dists = matching.iou_distance(unconfirmed, detections)
+        dists = iou_distance(unconfirmed, detections)
         
         #if not self.args.mot20:
-        dists = matching.fuse_score(dists, detections)
+        dists = fuse_score(dists, detections)
         
-        matches, u_unconfirmed, u_detection = matching.linear_assignment(dists, thresh=0.7)
+        matches, u_unconfirmed, u_detection = linear_assignment(dists, thresh=0.7)
         for itracked, idet in matches:
             unconfirmed[itracked].update(detections[idet], self.frame_id)
             activated_starcks.append(unconfirmed[itracked])
         for it in u_unconfirmed:
             track = unconfirmed[it]
             track.mark_removed()
             removed_stracks.append(track)
@@ -283,14 +284,15 @@
         self.tracked_stracks = [t for t in self.tracked_stracks if t.state == TrackState.Tracked]
         self.tracked_stracks = joint_stracks(self.tracked_stracks, activated_starcks)
         self.tracked_stracks = joint_stracks(self.tracked_stracks, refind_stracks)
         self.lost_stracks = sub_stracks(self.lost_stracks, self.tracked_stracks)
         self.lost_stracks.extend(lost_stracks)
         self.lost_stracks = sub_stracks(self.lost_stracks, self.removed_stracks)
         self.removed_stracks.extend(removed_stracks)
+        self.removed_stracks = [track for track in self.removed_stracks if self.frame_id - track.end_frame < 10 * self.max_time_lost]
         self.tracked_stracks, self.lost_stracks = remove_duplicate_stracks(self.tracked_stracks, self.lost_stracks)
         # get scores of lost tracks
         output_stracks = [track for track in self.tracked_stracks if track.is_activated]
 
         return output_stracks
 
 
@@ -316,15 +318,15 @@
         tid = t.track_id
         if stracks.get(tid, 0):
             del stracks[tid]
     return list(stracks.values())
 
 
 def remove_duplicate_stracks(stracksa, stracksb):
-    pdist = matching.iou_distance(stracksa, stracksb)
+    pdist = iou_distance(stracksa, stracksb)
     pairs = np.where(pdist < 0.15)
     dupa, dupb = list(), list()
     for p, q in zip(*pairs):
         timep = stracksa[p].frame_id - stracksa[p].start_frame
         timeq = stracksb[q].frame_id - stracksb[q].start_frame
         if timep > timeq:
             dupb.append(q)
```

### Comparing `onvif-gui-1.1.2/yolox/tracker/kalman_filter.py` & `onvif-gui-1.1.3/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.2/yolox/tracker/matching.py` & `onvif-gui-1.1.3/tracker/matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import scipy
 import lap
 from scipy.spatial.distance import cdist
 from cython_bbox import bbox_overlaps as bbox_ious
-from yolox.tracker import kalman_filter
+from .kalman_filter import chi2inv95
 
 def merge_matches(m1, m2, shape):
     O,P,Q = shape
     m1 = np.asarray(m1)
     m2 = np.asarray(m2)
 
     M1 = scipy.sparse.coo_matrix((np.ones(len(m1)), (m1[:, 0], m1[:, 1])), shape=(O, P))
@@ -126,28 +126,28 @@
     return cost_matrix
 
 
 def gate_cost_matrix(kf, cost_matrix, tracks, detections, only_position=False):
     if cost_matrix.size == 0:
         return cost_matrix
     gating_dim = 2 if only_position else 4
-    gating_threshold = kalman_filter.chi2inv95[gating_dim]
+    gating_threshold = chi2inv95[gating_dim]
     measurements = np.asarray([det.to_xyah() for det in detections])
     for row, track in enumerate(tracks):
         gating_distance = kf.gating_distance(
             track.mean, track.covariance, measurements, only_position)
         cost_matrix[row, gating_distance > gating_threshold] = np.inf
     return cost_matrix
 
 
 def fuse_motion(kf, cost_matrix, tracks, detections, only_position=False, lambda_=0.98):
     if cost_matrix.size == 0:
         return cost_matrix
     gating_dim = 2 if only_position else 4
-    gating_threshold = kalman_filter.chi2inv95[gating_dim]
+    gating_threshold = chi2inv95[gating_dim]
     measurements = np.asarray([det.to_xyah() for det in detections])
     for row, track in enumerate(tracks):
         gating_distance = kf.gating_distance(
             track.mean, track.covariance, measurements, only_position, metric='maha')
         cost_matrix[row, gating_distance > gating_threshold] = np.inf
         cost_matrix[row] = lambda_ * cost_matrix[row] + (1 - lambda_) * gating_distance
     return cost_matrix
```

### Comparing `onvif-gui-1.1.2/yolox/utils/utils.py` & `onvif-gui-1.1.3/yolox/utils/utils.py`

 * *Files identical despite different names*

