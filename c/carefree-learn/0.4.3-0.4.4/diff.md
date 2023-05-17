# Comparing `tmp/carefree-learn-0.4.3.tar.gz` & `tmp/carefree-learn-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-learn-0.4.3.tar", last modified: Fri May 12 11:21:40 2023, max compression
+gzip compressed data, was "carefree-learn-0.4.4.tar", last modified: Wed May 17 13:23:16 2023, max compression
```

## Comparing `carefree-learn-0.4.3.tar` & `carefree-learn-0.4.4.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.094033 carefree-learn-0.4.3/
--rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/LICENSE
--rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7575 2023-05-12 11:21:40.095033 carefree-learn-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.967523 carefree-learn-0.4.3/carefree_learn.egg-info/
--rw-rw-rw-   0        0        0     7575 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10736 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      635 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.971523 carefree-learn-0.4.3/cflearn/
--rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.973523 carefree-learn-0.4.3/cflearn/api/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/api/__init__.py
--rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.3/cflearn/api/api.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.974523 carefree-learn-0.4.3/cflearn/api/cv/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/api/cv/__init__.py
--rw-rw-rw-   0        0        0    61743 2023-05-09 10:43:21.000000 carefree-learn-0.4.3/cflearn/api/cv/diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.976523 carefree-learn-0.4.3/cflearn/api/cv/third_party/
--rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/blip.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.977523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/__init__.py
--rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/api.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.978523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/predictor.py
--rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/transforms.py
--rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.980523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/
--rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
--rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/base.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.981523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.982524 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/
--rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
--rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
--rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
--rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.984523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/
--rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
--rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
--rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.991524 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
--rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
--rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
--rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
--rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
--rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
--rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
--rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
--rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
--rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modifiers.py
--rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/ops.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.992524 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/utils/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/utils/__init__.py
--rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/utils/misc.py
--rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/isnet.py
--rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/lama.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.995524 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/__init__.py
--rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/api.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.002524 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/__init__.py
--rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/base_model.py
--rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/blocks.py
--rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/dpt_depth.py
--rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net.py
--rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
--rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/transforms.py
--rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/vit.py
--rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.004524 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/__init__.py
--rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/api.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.006524 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/__init__.py
--rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
--rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.009525 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/api.py
--rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/body.py
--rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/hand.py
--rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/model.py
--rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/util.py
--rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/prompt.py
--rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.3/cflearn/api/cv/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.010525 carefree-learn-0.4.3/cflearn/api/ml/
--rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/api/ml/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/api/ml/ddr.py
--rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/api/schema.py
--rw-rw-rw-   0        0        0     5513 2023-04-20 04:16:04.000000 carefree-learn-0.4.3/cflearn/api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.010525 carefree-learn-0.4.3/cflearn/api/zoo/
--rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.3/cflearn/api/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.013526 carefree-learn-0.4.3/cflearn/callbacks/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.3/cflearn/callbacks/classification.py
--rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.3/cflearn/callbacks/general.py
--rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.3/cflearn/callbacks/generator.py
--rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.014525 carefree-learn-0.4.3/cflearn/data/
--rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.3/cflearn/data/__init__.py
--rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.3/cflearn/data/array.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.015525 carefree-learn-0.4.3/cflearn/data/blocks/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.019526 carefree-learn-0.4.3/cflearn/data/blocks/cv/
--rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/crop.py
--rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/hwc_to_chw.py
--rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/image_folder.py
--rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/normalize.py
--rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/to_numpy.py
--rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/tuple_to_batch.py
--rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/flatten.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.022525 carefree-learn-0.4.3/cflearn/data/blocks/ml/
--rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/__init__.py
--rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/file.py
--rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/gather.py
--rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/nan_handler.py
--rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/preprocessor.py
--rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/recognizer.py
--rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/schema.py
--rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/splitter.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.024031 carefree-learn-0.4.3/cflearn/data/ml/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/ml/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.3/cflearn/data/ml/api.py
--rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/ml/datasets.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.026034 carefree-learn-0.4.3/cflearn/data/pytorch/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/pytorch/__init__.py
--rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.3/cflearn/data/pytorch/api.py
--rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.3/cflearn/data/pytorch/datasets.py
--rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.3/cflearn/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.026034 carefree-learn-0.4.3/cflearn/dist/
--rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/dist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.027034 carefree-learn-0.4.3/cflearn/dist/ml/
--rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/dist/ml/__init__.py
--rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/experiment.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.028034 carefree-learn-0.4.3/cflearn/dist/ml/runs/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/dist/ml/runs/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/runs/_utils.py
--rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/runs/basic.py
--rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/task.py
--rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/inference.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.030033 carefree-learn-0.4.3/cflearn/losses/
--rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/losses/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.3/cflearn/losses/basic.py
--rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/losses/gan.py
--rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.3/cflearn/losses/lpips.py
--rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/losses/vae.py
--rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.031033 carefree-learn-0.4.3/cflearn/misc/
--rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.3/cflearn/misc/__init__.py
--rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.3/cflearn/misc/available.json
--rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/misc/mixins.py
--rw-rw-rw-   0        0        0    44325 2023-05-08 12:35:20.000000 carefree-learn-0.4.3/cflearn/misc/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.032033 carefree-learn-0.4.3/cflearn/models/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/__init__.py
--rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/bases.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.033034 carefree-learn-0.4.3/cflearn/models/cv/
--rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.035035 carefree-learn-0.4.3/cflearn/models/cv/ae/
--rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/__init__.py
--rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/common.py
--rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/kl.py
--rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/vq.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.036034 carefree-learn-0.4.3/cflearn/models/cv/classifier/
--rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/classifier/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/classifier/vanilla.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.039034 carefree-learn-0.4.3/cflearn/models/cv/decoder/
--rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/__init__.py
--rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/attn.py
--rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/schema.py
--rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan.py
--rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan_v2.py
--rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/vanilla.py
--rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.042034 carefree-learn-0.4.3/cflearn/models/cv/diffusion/
--rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.044034 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/
--rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/clip.py
--rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/rescaler.py
--rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/schema.py
--rw-rw-rw-   0        0        0    28538 2023-05-06 05:26:10.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/ddpm.py
--rw-rw-rw-   0        0        0    10578 2023-05-08 12:33:49.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/ldm.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.047033 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/
--rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/basic.py
--rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/ddim.py
--rw-rw-rw-   0        0        0    13157 2023-04-20 02:12:01.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/k_samplers.py
--rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/plms.py
--rw-rw-rw-   0        0        0     7804 2023-05-04 11:20:31.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/schema.py
--rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/solver.py
--rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/utils.py
--rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/unet.py
--rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.051033 carefree-learn-0.4.3/cflearn/models/cv/encoder/
--rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/__init__.py
--rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/attn.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.053034 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/
--rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/api.py
--rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/core.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.055034 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/
--rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/__init__.py
--rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/mobilenet.py
--rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/resnet.py
--rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/transformer.py
--rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/vgg.py
--rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/register.py
--rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/fnet.py
--rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/mixer.py
--rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/perceiver.py
--rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/pool_former.py
--rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/schema.py
--rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/transformer.py
--rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/vanilla.py
--rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.057034 carefree-learn-0.4.3/cflearn/models/cv/gan/
--rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/__init__.py
--rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/discriminators.py
--rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/schema.py
--rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/vanilla.py
--rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/general.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.058033 carefree-learn-0.4.3/cflearn/models/cv/translator/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/translator/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/translator/rrdb.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.058033 carefree-learn-0.4.3/cflearn/models/implicit/
--rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/implicit/__init__.py
--rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/implicit/siren.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.063034 carefree-learn-0.4.3/cflearn/models/ml/
--rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/base.py
--rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.3/cflearn/models/ml/ddr.py
--rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.3/cflearn/models/ml/encoders.py
--rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/fcnn.py
--rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/linear.py
--rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/mixed_stacked.py
--rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/nbm.py
--rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/ndt.py
--rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/rnn.py
--rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/wnd.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.064033 carefree-learn-0.4.3/cflearn/models/multimodal/
--rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/multimodal/__init__.py
--rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.3/cflearn/models/multimodal/clip.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/multimodal/constants.py
--rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.3/cflearn/models/multimodal/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.064033 carefree-learn-0.4.3/cflearn/models/nlp/
--rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.066033 carefree-learn-0.4.3/cflearn/models/nlp/encoder/
--rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/encoder/__init__.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/encoder/constants.py
--rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/encoder/transformer.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.067033 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/clip.py
--rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.069035 carefree-learn-0.4.3/cflearn/models/nlp/transformers/
--rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/__init__.py
--rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/core.py
--rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/opus.py
--rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/simbert.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.070033 carefree-learn-0.4.3/cflearn/models/schemas/
--rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.3/cflearn/models/schemas/__init__.py
--rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/models/schemas/custom.py
--rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/schemas/cv.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.071033 carefree-learn-0.4.3/cflearn/modules/
--rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.076033 carefree-learn-0.4.3/cflearn/modules/blocks/
--rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.3/cflearn/modules/blocks/__init__.py
--rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.3/cflearn/modules/blocks/activations.py
--rw-rw-rw-   0        0        0    21356 2023-05-08 11:16:44.000000 carefree-learn-0.4.3/cflearn/modules/blocks/attentions.py
--rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.3/cflearn/modules/blocks/common.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.077033 carefree-learn-0.4.3/cflearn/modules/blocks/convs/
--rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/convs/__init__.py
--rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.3/cflearn/modules/blocks/convs/basic.py
--rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.3/cflearn/modules/blocks/convs/residual.py
--rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.3/cflearn/modules/blocks/customs.py
--rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/modules/blocks/high_level.py
--rw-rw-rw-   0        0        0    14999 2023-04-12 13:33:59.000000 carefree-learn-0.4.3/cflearn/modules/blocks/hijacks.py
--rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.3/cflearn/modules/blocks/hooks.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.078033 carefree-learn-0.4.3/cflearn/modules/blocks/implementations/
--rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/implementations/__init__.py
--rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/implementations/perceiver.py
--rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mappings.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.080033 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/
--rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/__init__.py
--rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/api.py
--rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
--rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/poolers.py
--rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/schema.py
--rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/token_mixers.py
--rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/norms.py
--rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.3/cflearn/modules/blocks/utils.py
--rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/optimizers.py
--rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.3/cflearn/modules/schedulers.py
--rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/monitors.py
--rw-rw-rw-   0        0        0      634 2023-02-16 10:09:59.000000 carefree-learn-0.4.3/cflearn/parameters.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.082034 carefree-learn-0.4.3/cflearn/pipeline/
--rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/__init__.py
--rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.3/cflearn/pipeline/api.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.084033 carefree-learn-0.4.3/cflearn/pipeline/blocks/
--rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/__init__.py
--rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/basic.py
--rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/ml.py
--rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/utils.py
--rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.3/cflearn/pipeline/core.py
--rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/schema.py
--rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/third_party.py
--rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/register.py
--rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.3/cflearn/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.084033 carefree-learn-0.4.3/cflearn/scripts/
--rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.3/cflearn/scripts/__init__.py
--rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/scripts/sd.py
--rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/trainer.py
--rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/types.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.085034 carefree-learn-0.4.3/cflearn/zoo/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.956523 carefree-learn-0.4.3/cflearn/zoo/configs/ae/
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.087034 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/
--rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f16.json
--rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f4.json
--rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.088033 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/
--rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/f4.json
--rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/f4_no_attn.json
--rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.088033 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ddpm/
--rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ddpm/default.json
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.091033 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/
--rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/default.json
--rw-rw-rw-   0        0        0      451 2023-05-08 10:29:54.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd.json
--rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
--rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
--rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
--rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/vq.json
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.092033 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/
--rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/chinese.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/default.json
--rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/large.json
--rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/sr/
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.093033 carefree-learn-0.4.3/cflearn/zoo/configs/sr/esr/
--rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/sr/esr/anime.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/sr/esr/default.json
--rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.3/cflearn/zoo/core.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.094033 carefree-learn-0.4.3/cflearn/zoo/models/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/models/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/models/clip.py
--rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/models/schema.py
--rw-rw-rw-   0        0        0      383 2023-05-12 11:21:40.096033 carefree-learn-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-05-12 11:17:01.000000 carefree-learn-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.885306 carefree-learn-0.4.4/
+-rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7575 2023-05-17 13:23:16.885306 carefree-learn-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.740221 carefree-learn-0.4.4/carefree_learn.egg-info/
+-rw-rw-rw-   0        0        0     7575 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10736 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      635 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.744210 carefree-learn-0.4.4/cflearn/
+-rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.746203 carefree-learn-0.4.4/cflearn/api/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/api/__init__.py
+-rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.4/cflearn/api/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.747200 carefree-learn-0.4.4/cflearn/api/cv/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/api/cv/__init__.py
+-rw-rw-rw-   0        0        0    63199 2023-05-16 07:51:40.000000 carefree-learn-0.4.4/cflearn/api/cv/diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.750190 carefree-learn-0.4.4/cflearn/api/cv/third_party/
+-rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/blip.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.751187 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.753180 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/__init__.py
+-rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/predictor.py
+-rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/transforms.py
+-rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.754177 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/
+-rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
+-rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/base.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.756170 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.758164 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/
+-rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
+-rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
+-rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
+-rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.760156 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/
+-rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
+-rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
+-rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.765140 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
+-rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
+-rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
+-rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
+-rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
+-rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
+-rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
+-rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
+-rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
+-rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modifiers.py
+-rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/ops.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.766137 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/utils/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/utils/misc.py
+-rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/isnet.py
+-rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/lama.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.767134 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/__init__.py
+-rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.772117 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/base_model.py
+-rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/blocks.py
+-rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/dpt_depth.py
+-rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net.py
+-rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/transforms.py
+-rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/vit.py
+-rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.773113 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.775107 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.778097 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/api.py
+-rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/body.py
+-rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/hand.py
+-rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/model.py
+-rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/util.py
+-rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/prompt.py
+-rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.4/cflearn/api/cv/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.779094 carefree-learn-0.4.4/cflearn/api/ml/
+-rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/api/ml/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/api/ml/ddr.py
+-rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/api/schema.py
+-rw-rw-rw-   0        0        0     2983 2023-05-17 13:13:35.000000 carefree-learn-0.4.4/cflearn/api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.780090 carefree-learn-0.4.4/cflearn/api/zoo/
+-rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.4/cflearn/api/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.782084 carefree-learn-0.4.4/cflearn/callbacks/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.4/cflearn/callbacks/classification.py
+-rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.4/cflearn/callbacks/general.py
+-rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.4/cflearn/callbacks/generator.py
+-rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.783080 carefree-learn-0.4.4/cflearn/data/
+-rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.4/cflearn/data/__init__.py
+-rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.4/cflearn/data/array.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.784077 carefree-learn-0.4.4/cflearn/data/blocks/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.787067 carefree-learn-0.4.4/cflearn/data/blocks/cv/
+-rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/crop.py
+-rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/hwc_to_chw.py
+-rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/image_folder.py
+-rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/normalize.py
+-rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/to_numpy.py
+-rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/tuple_to_batch.py
+-rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/flatten.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.791054 carefree-learn-0.4.4/cflearn/data/blocks/ml/
+-rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/__init__.py
+-rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/file.py
+-rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/gather.py
+-rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/nan_handler.py
+-rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/preprocessor.py
+-rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/recognizer.py
+-rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/schema.py
+-rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/splitter.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.792050 carefree-learn-0.4.4/cflearn/data/ml/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/ml/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.4/cflearn/data/ml/api.py
+-rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/ml/datasets.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.793047 carefree-learn-0.4.4/cflearn/data/pytorch/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.4/cflearn/data/pytorch/api.py
+-rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.4/cflearn/data/pytorch/datasets.py
+-rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.4/cflearn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.794044 carefree-learn-0.4.4/cflearn/dist/
+-rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/dist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.795040 carefree-learn-0.4.4/cflearn/dist/ml/
+-rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/dist/ml/__init__.py
+-rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/experiment.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.797034 carefree-learn-0.4.4/cflearn/dist/ml/runs/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/dist/ml/runs/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/runs/_utils.py
+-rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/runs/basic.py
+-rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/task.py
+-rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/inference.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.799027 carefree-learn-0.4.4/cflearn/losses/
+-rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/losses/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.4/cflearn/losses/basic.py
+-rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/losses/gan.py
+-rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.4/cflearn/losses/lpips.py
+-rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/losses/vae.py
+-rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.801020 carefree-learn-0.4.4/cflearn/misc/
+-rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.4/cflearn/misc/__init__.py
+-rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.4/cflearn/misc/available.json
+-rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/misc/mixins.py
+-rw-rw-rw-   0        0        0    44325 2023-05-16 10:13:20.000000 carefree-learn-0.4.4/cflearn/misc/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.802017 carefree-learn-0.4.4/cflearn/models/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/__init__.py
+-rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/bases.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.803013 carefree-learn-0.4.4/cflearn/models/cv/
+-rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.805007 carefree-learn-0.4.4/cflearn/models/cv/ae/
+-rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/__init__.py
+-rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/common.py
+-rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/kl.py
+-rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/vq.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.806003 carefree-learn-0.4.4/cflearn/models/cv/classifier/
+-rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/classifier/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/classifier/vanilla.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.808993 carefree-learn-0.4.4/cflearn/models/cv/decoder/
+-rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/__init__.py
+-rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/attn.py
+-rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/schema.py
+-rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan.py
+-rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan_v2.py
+-rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/vanilla.py
+-rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.811983 carefree-learn-0.4.4/cflearn/models/cv/diffusion/
+-rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.813977 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/
+-rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/clip.py
+-rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/rescaler.py
+-rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/schema.py
+-rw-rw-rw-   0        0        0    28538 2023-05-06 05:26:10.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/ddpm.py
+-rw-rw-rw-   0        0        0    10675 2023-05-16 07:51:34.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/ldm.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.818960 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/
+-rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/__init__.py
+-rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/basic.py
+-rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/ddim.py
+-rw-rw-rw-   0        0        0    13157 2023-04-20 02:12:01.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/k_samplers.py
+-rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/plms.py
+-rw-rw-rw-   0        0        0     7804 2023-05-04 11:20:31.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/schema.py
+-rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/solver.py
+-rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/utils.py
+-rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/unet.py
+-rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.823943 carefree-learn-0.4.4/cflearn/models/cv/encoder/
+-rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/__init__.py
+-rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/attn.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.824941 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/
+-rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/api.py
+-rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/core.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.827930 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/
+-rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/__init__.py
+-rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/mobilenet.py
+-rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/resnet.py
+-rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/transformer.py
+-rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/vgg.py
+-rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/register.py
+-rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/fnet.py
+-rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/mixer.py
+-rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/perceiver.py
+-rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/pool_former.py
+-rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/schema.py
+-rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/transformer.py
+-rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/vanilla.py
+-rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.830921 carefree-learn-0.4.4/cflearn/models/cv/gan/
+-rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/__init__.py
+-rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/discriminators.py
+-rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/schema.py
+-rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/vanilla.py
+-rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/general.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.831918 carefree-learn-0.4.4/cflearn/models/cv/translator/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/translator/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/translator/rrdb.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.833911 carefree-learn-0.4.4/cflearn/models/implicit/
+-rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/implicit/__init__.py
+-rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/implicit/siren.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.839890 carefree-learn-0.4.4/cflearn/models/ml/
+-rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/__init__.py
+-rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/base.py
+-rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.4/cflearn/models/ml/ddr.py
+-rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.4/cflearn/models/ml/encoders.py
+-rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/fcnn.py
+-rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/linear.py
+-rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/mixed_stacked.py
+-rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/nbm.py
+-rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/ndt.py
+-rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/rnn.py
+-rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/wnd.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.841884 carefree-learn-0.4.4/cflearn/models/multimodal/
+-rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/multimodal/__init__.py
+-rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.4/cflearn/models/multimodal/clip.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/multimodal/constants.py
+-rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.4/cflearn/models/multimodal/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.841884 carefree-learn-0.4.4/cflearn/models/nlp/
+-rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.843877 carefree-learn-0.4.4/cflearn/models/nlp/encoder/
+-rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/encoder/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/encoder/constants.py
+-rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/encoder/transformer.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.846868 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/clip.py
+-rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.849857 carefree-learn-0.4.4/cflearn/models/nlp/transformers/
+-rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/__init__.py
+-rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/core.py
+-rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/opus.py
+-rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/simbert.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.850855 carefree-learn-0.4.4/cflearn/models/schemas/
+-rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.4/cflearn/models/schemas/__init__.py
+-rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/models/schemas/custom.py
+-rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/schemas/cv.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.852847 carefree-learn-0.4.4/cflearn/modules/
+-rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.858828 carefree-learn-0.4.4/cflearn/modules/blocks/
+-rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.4/cflearn/modules/blocks/__init__.py
+-rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.4/cflearn/modules/blocks/activations.py
+-rw-rw-rw-   0        0        0    21356 2023-05-08 11:16:44.000000 carefree-learn-0.4.4/cflearn/modules/blocks/attentions.py
+-rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.4/cflearn/modules/blocks/common.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.860821 carefree-learn-0.4.4/cflearn/modules/blocks/convs/
+-rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/convs/__init__.py
+-rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.4/cflearn/modules/blocks/convs/basic.py
+-rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.4/cflearn/modules/blocks/convs/residual.py
+-rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.4/cflearn/modules/blocks/customs.py
+-rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/modules/blocks/high_level.py
+-rw-rw-rw-   0        0        0    15078 2023-05-16 07:51:00.000000 carefree-learn-0.4.4/cflearn/modules/blocks/hijacks.py
+-rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.4/cflearn/modules/blocks/hooks.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.861817 carefree-learn-0.4.4/cflearn/modules/blocks/implementations/
+-rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/implementations/__init__.py
+-rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/implementations/perceiver.py
+-rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.865804 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/
+-rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/__init__.py
+-rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/api.py
+-rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
+-rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/poolers.py
+-rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/schema.py
+-rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/token_mixers.py
+-rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/norms.py
+-rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.4/cflearn/modules/blocks/utils.py
+-rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/optimizers.py
+-rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.4/cflearn/modules/schedulers.py
+-rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/monitors.py
+-rw-rw-rw-   0        0        0      634 2023-02-16 10:09:59.000000 carefree-learn-0.4.4/cflearn/parameters.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.868794 carefree-learn-0.4.4/cflearn/pipeline/
+-rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/__init__.py
+-rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.4/cflearn/pipeline/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.870787 carefree-learn-0.4.4/cflearn/pipeline/blocks/
+-rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/__init__.py
+-rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/basic.py
+-rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/ml.py
+-rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/utils.py
+-rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.4/cflearn/pipeline/core.py
+-rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/schema.py
+-rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/third_party.py
+-rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/register.py
+-rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.4/cflearn/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.871784 carefree-learn-0.4.4/cflearn/scripts/
+-rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.4/cflearn/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/scripts/sd.py
+-rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/trainer.py
+-rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/types.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.872780 carefree-learn-0.4.4/cflearn/zoo/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.717081 carefree-learn-0.4.4/cflearn/zoo/configs/ae/
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.873777 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/
+-rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f16.json
+-rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f4.json
+-rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.875331 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/
+-rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/f4.json
+-rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/f4_no_attn.json
+-rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.876333 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ddpm/
+-rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ddpm/default.json
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.879325 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/
+-rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/default.json
+-rw-rw-rw-   0        0        0      451 2023-05-08 10:29:54.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd.json
+-rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
+-rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
+-rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
+-rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/vq.json
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.882316 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/
+-rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/chinese.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/default.json
+-rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/large.json
+-rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/sr/
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.883312 carefree-learn-0.4.4/cflearn/zoo/configs/sr/esr/
+-rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/sr/esr/anime.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/sr/esr/default.json
+-rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.4/cflearn/zoo/core.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.884310 carefree-learn-0.4.4/cflearn/zoo/models/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/models/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/models/clip.py
+-rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/models/schema.py
+-rw-rw-rw-   0        0        0      383 2023-05-17 13:23:16.888297 carefree-learn-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-05-17 13:22:51.000000 carefree-learn-0.4.4/setup.py
```

### Comparing `carefree-learn-0.4.3/LICENSE` & `carefree-learn-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/PKG-INFO` & `carefree-learn-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.3
+Version: 0.4.4
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.3.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.4.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.3/README.md` & `carefree-learn-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/carefree_learn.egg-info/PKG-INFO` & `carefree-learn-0.4.4/carefree_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.3
+Version: 0.4.4
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.3.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.4.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.3/carefree_learn.egg-info/SOURCES.txt` & `carefree-learn-0.4.4/carefree_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/carefree_learn.egg-info/requires.txt` & `carefree-learn-0.4.4/carefree_learn.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 accelerate
 safetensors
-carefree-toolkit>=0.3.4
+carefree-toolkit>=0.3.5
 
 [cv]
 ftfy
 lmdb
 regex
 transformers
 albumentations
```

### Comparing `carefree-learn-0.4.3/cflearn/__init__.py` & `carefree-learn-0.4.4/cflearn/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/api.py` & `carefree-learn-0.4.4/cflearn/api/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/diffusion.py` & `carefree-learn-0.4.4/cflearn/api/cv/diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import Tuple
 from typing import Union
 from typing import TypeVar
 from typing import Callable
 from typing import Optional
 from typing import NamedTuple
 from typing import ContextManager
+from cftool.cv import to_rgb
 from cftool.cv import read_image
 from cftool.cv import save_images
 from cftool.cv import restrict_wh
 from cftool.cv import get_suitable_size
 from cftool.cv import ReadImageResponse
 from cftool.misc import safe_execute
 from cftool.misc import print_warning
@@ -629,117 +630,145 @@
         reference_fidelity: float = 0.2,
         anchor: int = 64,
         max_wh: int = 512,
         num_samples: Optional[int] = None,
         num_steps: Optional[int] = None,
         clip_output: bool = True,
         keep_original: bool = False,
+        ref_mask_smooth: int = 0,
         use_raw_inpainting: bool = False,
+        raw_inpainting_use_ref: bool = False,
         raw_inpainting_fidelity: float = 0.2,
         callback: Optional[Callable[[Tensor], Tensor]] = None,
         use_latent_guidance: bool = False,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
-        if use_raw_inpainting:
-            image_res = read_image(image, max_wh, anchor=anchor)
-            mask = read_image(mask, max_wh, anchor=anchor, to_mask=True).image
-            z = z_ref = self._get_z(image_res.image)
-            z_ref_mask = F.interpolate(
-                torch.from_numpy(mask).to(z_ref),
+        def get_z_ref_pack(
+            res_: ReadImageResponse,
+            mask_: np.ndarray,
+        ) -> Tuple[Tensor, Tensor, Tensor]:
+            z_ref = self._get_z(res_.image)
+            if ref_mask_smooth > 0:
+                mask_ = cv2.blur(mask_[0][0], (ref_mask_smooth, ref_mask_smooth))
+                mask_ = mask_[None, None]
+            z_ref_mask = 1.0 - F.interpolate(
+                torch.from_numpy(mask_).to(z_ref),
                 z_ref.shape[-2:],
                 mode="bicubic",
             )
-            return self._img2img(
-                z,
-                export_path,
-                z_ref=z_ref,
-                z_ref_mask=z_ref_mask,
-                fidelity=raw_inpainting_fidelity,
-                original_size=image_res.original_size,
-                alpha=None,
-                cond=[txt],
-                num_steps=num_steps,
-                clip_output=clip_output,
-                verbose=verbose,
-                **kwargs,
-            )
+            if seed is not None:
+                seed_everything(seed)
+            z_ref_noise = torch.randn_like(z_ref)
+            return z_ref, z_ref_mask, z_ref_noise
+
+        def get_z_info_from(
+            reference_: Optional[Union[str, Image.Image]],
+            fidelity_: float,
+            shape_: Tuple[int, int],
+        ) -> Tuple[Optional[Tensor], Optional[Tuple[int, int]], Dict[str, Any]]:
+            if reference_ is None:
+                z = None
+                new_kw = kwargs
+                size = tuple(map(lambda n: n * self.size_info.factor, shape_))
+            else:
+                size = None
+                z = self._get_z(read_image(reference_, max_wh, anchor=anchor).image)
+                if z_ref_mask is not None and z_ref_noise is not None:
+                    z = z * z_ref_mask + z_ref_noise * (1.0 - z_ref_mask)
+                z, _, new_kw = self._q_sample(z, num_steps, fidelity_, seed, **kwargs)
+            return z, size, new_kw  # type: ignore
+
+        def paste_original(
+            original_: Image.Image,
+            mask_: Image.Image,
+            sampled_: Tensor,
+        ) -> Tensor:
+            rgb = to_rgb(original_)
+            rgb_normalized = np.array(rgb).astype(np.float32) / 127.5 - 1.0
+            rgb_normalized = rgb_normalized.transpose([2, 0, 1])[None]
+            mask_res_ = read_image(mask_, None, anchor=None, to_mask=True)
+            remained_mask_ = ~(mask_res_.image >= 0.5)
+            pasted = np.where(remained_mask_, rgb_normalized, sampled_.numpy())
+            return torch.from_numpy(pasted)
+
         txt_list, num_samples = get_txt_cond(txt, num_samples)
+        if use_raw_inpainting:
+            image_res = read_image(image, max_wh, anchor=anchor)
+            mask_res = read_image(mask, max_wh, anchor=anchor, to_mask=True)
+            z_ref, z_ref_mask, z_ref_noise = get_z_ref_pack(image_res, mask_res.image)
+            z, size, kwargs = get_z_info_from(
+                image_res.image if raw_inpainting_use_ref else None,
+                raw_inpainting_fidelity,
+                z_ref.shape[-2:][::-1],
+            )
+            kw = shallow_copy_dict(kwargs)
+            kw.update(
+                dict(
+                    z=z,
+                    size=size,
+                    export_path=export_path,
+                    z_ref=z_ref,
+                    z_ref_mask=z_ref_mask,
+                    z_ref_noise=z_ref_noise,
+                    original_size=image_res.original_size,
+                    alpha=None,
+                    cond=txt_list,
+                    num_steps=num_steps,
+                    clip_output=clip_output,
+                    verbose=verbose,
+                )
+            )
+            sampled = self.sample(num_samples, **kw)
+            if keep_original:
+                original = image_res.original
+                sampled = paste_original(original, mask_res.original, sampled)
+            return sampled
         res = self._get_masked_cond(
             image,
             mask,
             max_wh,
             anchor,
             lambda remained_mask, img: np.where(remained_mask, img, 0.5),
             lambda bool_mask: torch.from_numpy(bool_mask),
         )
         # sampling
         with switch_sampler_context(self, kwargs.get("sampler")):
             # calculate `z_ref` stuffs based on `use_image_guidance`
             if not use_latent_guidance:
                 z_ref = z_ref_mask = z_ref_noise = None
             else:
-                z_ref = self._get_z(res.image_res.image)
-                z_ref_mask = 1.0 - F.interpolate(
-                    torch.from_numpy(res.mask).to(z_ref),
-                    z_ref.shape[-2:],
-                    mode="bicubic",
-                )
-                if seed is not None:
-                    seed_everything(seed)
-                z_ref_noise = torch.randn_like(z_ref)
+                z_ref, z_ref_mask, z_ref_noise = get_z_ref_pack(res.image_res, res.mask)
                 reference = res.image_res.original
             # calculate `z` based on `reference`
-            if reference is None:
-                z = None
-                size = tuple(
-                    map(
-                        lambda n: n * self.size_info.factor,
-                        res.remained_image_cond.shape[-2:][::-1],
-                    )
-                )
-            else:
-                size = None
-                z = self._get_z(read_image(reference, max_wh, anchor=anchor).image)
-                if z_ref_mask is not None and z_ref_noise is not None:
-                    z = z * z_ref_mask + z_ref_noise * (1.0 - z_ref_mask)
-                z, _, kwargs = self._q_sample(
-                    z,
-                    num_steps,
-                    reference_fidelity,
-                    seed,
-                    **kwargs,
-                )
+            z_shape = res.remained_image_cond.shape[-2:][::-1]
+            z, size, kwargs = get_z_info_from(reference, reference_fidelity, z_shape)
             # core
             sampled = self.sample(
                 num_samples,
                 export_path,
                 seed=seed,
                 z=z,
                 z_ref=z_ref,
                 z_ref_mask=z_ref_mask,
                 z_ref_noise=z_ref_noise,
                 size=size,  # type: ignore
                 original_size=res.image_res.original_size,
-                alpha=res.image_res.alpha,
+                alpha=None,
                 cond=txt_list,
                 cond_concat=torch.cat([res.mask_cond, res.remained_image_cond], dim=1),
                 num_steps=num_steps,
                 clip_output=clip_output,
                 callback=callback,
                 verbose=verbose,
                 **kwargs,
             )
         if keep_original:
-            original = np.array(res.image_res.original).astype(np.float32) / 127.5 - 1.0
-            original = original.transpose([2, 0, 1])[None]
-            mask_ = read_image(res.mask_res.original, None, anchor=None, to_mask=True)
-            remained_mask = ~(mask_.image >= 0.5)
-            sampled = np.where(remained_mask, original, sampled.numpy())
-            sampled = torch.from_numpy(sampled)
+            original = res.image_res.original
+            sampled = paste_original(original, res.mask_res.original, sampled)
         return sampled
 
     def outpainting(
         self,
         txt: str,
         image: Union[str, Image.Image],
         export_path: Optional[str] = None,
```

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/blip.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/blip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/api.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/predictor.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/predictor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/transforms.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/base.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/dih_model.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/dih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/unet.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/ops.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/ops.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/isnet.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/isnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/lama.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/lama.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/api.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/blocks.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/dpt_depth.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net_custom.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/transforms.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/vit.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/vit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/utils.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/api.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/utils.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/api.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/body.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/body.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/hand.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/model.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/util.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/util.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/third_party/prompt.py` & `carefree-learn-0.4.4/cflearn/api/cv/third_party/prompt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/cv/translator.py` & `carefree-learn-0.4.4/cflearn/api/cv/translator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/ml/ddr.py` & `carefree-learn-0.4.4/cflearn/api/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/schema.py` & `carefree-learn-0.4.4/cflearn/api/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/api/utils.py` & `carefree-learn-0.4.4/cflearn/models/bases.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,181 +1,168 @@
-import gc
-import time
+import os
 import torch
 
-import torch.nn as nn
+import torch.nn.functional as F
 
 from abc import abstractmethod
 from abc import ABCMeta
 from typing import Any
 from typing import Dict
-from typing import Type
-from typing import Generic
-from typing import TypeVar
-from typing import Callable
 from typing import Optional
-from cftool.misc import TIME_FORMAT
-from cftool.misc import print_info
-from cftool.misc import sort_dict_by_value
+from typing import NamedTuple
+from cftool.misc import print_warning
 from cftool.types import tensor_dict_type
-from torch.cuda.amp.autocast_mode import autocast
 
-from .zoo import TPipeline
-from ..misc.toolkit import is_cpu
-from ..misc.toolkit import get_device
-from ..misc.toolkit import empty_cuda_cache
+from ..schema import ITrainer
+from ..schema import ILoss
+from ..schema import IDLModel
+from ..constants import LOSS_KEY
+from ..constants import LABEL_KEY
+from ..constants import LATENT_KEY
+from ..constants import PREDICTIONS_KEY
+from ..misc.toolkit import set_requires_grad
+
+
+class ICustomLossOutput(NamedTuple):
+    forward_results: tensor_dict_type
+    loss_dict: tensor_dict_type
+
+
+class ICustomLossModule(torch.nn.Module):
+    @abstractmethod
+    def get_losses(
+        self,
+        batch_idx: int,
+        batch: tensor_dict_type,
+        trainer: ITrainer,
+        forward_kwargs: Dict[str, Any],
+        loss_kwargs: Dict[str, Any],
+    ) -> ICustomLossOutput:
+        pass
+
+    @abstractmethod
+    def forward(self, *args: Any, **kwargs: Any) -> Any:
+        pass
+
+
+class IBAKE(ICustomLossModule, metaclass=ABCMeta):
+    lb: float
+    bake_loss: ILoss
+    w_ensemble: float
+    is_classification: bool
 
+    def _init_bake(
+        self,
+        lb: float,
+        bake_loss: str,
+        bake_loss_config: Optional[Dict[str, Any]],
+        w_ensemble: float,
+        is_classification: bool,
+    ) -> None:
+        self.lb = lb
+        self.w_ensemble = w_ensemble
+        self.is_classification = is_classification
+        if bake_loss == "auto":
+            bake_loss = "focal" if is_classification else "mae"
+        self.bake_loss = ILoss.make(bake_loss, bake_loss_config or {})
 
-TAPI = TypeVar("TAPI", bound="APIMixin")
-TItem = TypeVar("TItem")
+    def get_losses(
+        self,
+        batch_idx: int,
+        batch: tensor_dict_type,
+        trainer: ITrainer,
+        forward_kwargs: Dict[str, Any],
+        loss_kwargs: Dict[str, Any],
+    ) -> ICustomLossOutput:
+        state = trainer.state
+        forward_results = self(batch_idx, batch, state, **forward_kwargs)
+        loss_dict = trainer.loss(forward_results, batch, state, **loss_kwargs)
+        loss = loss_dict[LOSS_KEY]
+        predictions = forward_results[PREDICTIONS_KEY]
+        # BAKE
+        latent = F.normalize(forward_results[LATENT_KEY])
+        batch_size = latent.shape[0]
+        eye = torch.eye(batch_size, device=latent.device)
+        similarities = F.softmax(latent.mm(latent.t()) - eye * 1.0e9, dim=1)
+        inv = (eye - self.w_ensemble * similarities).inverse()
+        weights = (1.0 - self.w_ensemble) * inv
+        if not self.is_classification:
+            bake_inp = predictions
+            soft_labels = weights.mm(predictions).detach()
+        else:
+            bake_inp = F.log_softmax(predictions)
+            soft_labels = weights.mm(F.softmax(predictions, dim=1)).detach()
+        bake_loss = self.bake_loss(
+            {PREDICTIONS_KEY: bake_inp},
+            {LABEL_KEY: soft_labels},
+            state,
+            **loss_kwargs,
+        )[LOSS_KEY]
+        loss_dict["bake"] = bake_loss
+        loss_dict[LOSS_KEY] = loss + self.lb * bake_loss
+        return ICustomLossOutput(forward_results, loss_dict)
+
+
+class IRDropout(ICustomLossModule, metaclass=ABCMeta):
+    lb: float
+    is_classification: bool
 
+    def get_losses(
+        self,
+        batch_idx: int,
+        batch: tensor_dict_type,
+        trainer: ITrainer,
+        forward_kwargs: Dict[str, Any],
+        loss_kwargs: Dict[str, Any],
+    ) -> ICustomLossOutput:
+        state = trainer.state
+        fr1 = self(batch_idx, batch, state, **forward_kwargs)
+        fr2 = self(batch_idx, batch, state, **forward_kwargs)
+        loss_dict = trainer.loss(fr1, batch, state, **loss_kwargs)
+        for k, v in trainer.loss(fr2, batch, state, **loss_kwargs).items():
+            loss_dict[k] = loss_dict[k] + v
+        loss = loss_dict[LOSS_KEY]
+        # R-Dropout loss
+        p1 = fr1[PREDICTIONS_KEY]
+        p2 = fr2[PREDICTIONS_KEY]
+        if not self.is_classification:
+            r_dropout = ((p1 - p2) ** 2).mean()
+        else:
+            p1_loss = F.kl_div(F.log_softmax(p1, dim=-1), F.softmax(p2, dim=-1))
+            p2_loss = F.kl_div(F.log_softmax(p2, dim=-1), F.softmax(p1, dim=-1))
+            r_dropout = 0.5 * (p1_loss + p2_loss)
+        loss_dict["r_dropout"] = r_dropout
+        loss_dict[LOSS_KEY] = loss + self.lb * r_dropout
+        return ICustomLossOutput(fr1, loss_dict)
 
-class APIMixin:
-    m: nn.Module
-    device: torch.device
-    use_amp: bool
-    use_half: bool
 
-    def __init__(
-        self,
-        m: nn.Module,
-        device: torch.device,
-        *,
-        use_amp: bool = False,
-        use_half: bool = False,
-    ):
-        if use_amp and use_half:
-            raise ValueError("`use_amp` & `use_half` should not be True simultaneously")
-        self.m = m.eval().requires_grad_(False)
-        self.device = device
-        self.use_amp = use_amp
-        self.use_half = use_half
+class CascadeMixin:
+    lv1_net: IDLModel
+    lv2_net: IDLModel
 
-    def to(
+    def _construct(
         self,
-        device: torch.device,
-        *,
-        use_amp: bool = False,
-        use_half: bool = False,
+        lv1_model_name: str,
+        lv2_model_name: str,
+        lv1_model_config: Dict[str, Any],
+        lv2_model_config: Dict[str, Any],
+        lv1_model_ckpt_path: Optional[str],
+        lv1_model_trainable: bool,
     ) -> None:
-        if use_amp and use_half:
-            raise ValueError("`use_amp` & `use_half` should not be True simultaneously")
-        self.device = device
-        self.use_amp = use_amp
-        self.use_half = use_half
-        device_is_cpu = is_cpu(device)
-        if device_is_cpu:
-            self.m.to(device)
-        if use_half:
-            self.m.half()
-        else:
-            self.m.float()
-        if not device_is_cpu:
-            self.m.to(device)
-
-    def empty_cuda_cache(self) -> None:
-        empty_cuda_cache(self.device)
-
-    @property
-    def amp_context(self) -> autocast:
-        return autocast(enabled=self.use_amp)
-
-    @classmethod
-    def from_pipeline(
-        cls: Type[TAPI],
-        m: TPipeline,
-        device: Optional[str] = None,
-        *,
-        use_amp: bool = False,
-        use_half: bool = False,
-        **kwargs: Any,
-    ) -> TAPI:
-        if use_amp and use_half:
-            raise ValueError("`use_amp` & `use_half` should not be True simultaneously")
-        model = m.build_model.model
-        if use_half:
-            model.half()
-        if device is not None:
-            model.to(device)
-        return cls(
-            model,
-            get_device(model),
-            use_amp=use_amp,
-            use_half=use_half,
-            **kwargs,
-        )
-
-
-class ILoadableItem(Generic[TItem]):
-    _item: Optional[TItem]
-
-    def __init__(self, init_fn: Callable[[], TItem], *, init: bool = False):
-        self.init_fn = init_fn
-        self.load_time = time.time()
-        self._item = init_fn() if init else None
-
-    def load(self, **kwargs: Any) -> TItem:
-        self.load_time = time.time()
-        if self._item is None:
-            self._item = self.init_fn()
-        return self._item
-
-    def unload(self) -> None:
-        self._item = None
-        gc.collect()
-
-
-class ILoadablePool(Generic[TItem], metaclass=ABCMeta):
-    pool: Dict[str, ILoadableItem]
-    activated: Dict[str, ILoadableItem]
-
-    # set `limit` to negative values to indicate 'no limit'
-    def __init__(self, limit: int = -1):
-        self.pool = {}
-        self.activated = {}
-        self.limit = limit
-        if limit == 0:
-            raise ValueError(
-                "limit should either be negative "
-                "(which indicates 'no limit') or be positive"
-            )
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.pool
-
-    def register(self, key: str, init_fn: Callable[[bool], ILoadableItem]) -> None:
-        if key in self.pool:
-            raise ValueError(f"key '{key}' already exists")
-        init = self.limit < 0 or len(self.activated) < self.limit
-        loadable_item = init_fn(init)
-        self.pool[key] = loadable_item
-        if init:
-            self.activated[key] = loadable_item
-
-    def get(self, key: str, **kwargs: Any) -> TItem:
-        loadable_item = self.pool.get(key)
-        if loadable_item is None:
-            raise ValueError(f"key '{key}' does not exist")
-        item = loadable_item.load(**kwargs)
-        if key in self.activated:
-            return item
-        load_times = {k: v.load_time for k, v in self.activated.items()}
-        earliest_key = list(sort_dict_by_value(load_times).keys())[0]
-        self.activated.pop(earliest_key).unload()
-        self.activated[key] = loadable_item
-
-        time_format = "-".join(TIME_FORMAT.split("-")[:-1])
-        print_info(
-            f"'{earliest_key}' is unloaded to make room for '{key}' "
-            f"(last updated: {time.strftime(time_format, time.localtime(loadable_item.load_time))})"
-        )
-        return item
-
-
-class Weights(ILoadableItem[tensor_dict_type]):
-    def __init__(self, path: str, *, init: bool = False):
-        super().__init__(lambda: torch.load(path), init=init)
-
-
-class WeightsPool(ILoadablePool[tensor_dict_type]):
-    def register(self, key: str, path: str) -> None:  # type: ignore
-        super().register(key, lambda init: Weights(path, init=init))
+        self.lv1_net = IDLModel.make(lv1_model_name, lv1_model_config)
+        if lv1_model_ckpt_path is not None:
+            if not os.path.isfile(lv1_model_ckpt_path):
+                print_warning(f"'{lv1_model_ckpt_path}' does not exist")
+            else:
+                state_dict = torch.load(lv1_model_ckpt_path, map_location="cpu")
+                self.lv1_net.load_state_dict(state_dict)
+        if not lv1_model_trainable:
+            set_requires_grad(self.lv1_net, False)
+        self.lv2_net = IDLModel.make(lv2_model_name, lv2_model_config)
+
+
+__all__ = [
+    "ICustomLossModule",
+    "IBAKE",
+    "IRDropout",
+    "CascadeMixin",
+]
```

### Comparing `carefree-learn-0.4.3/cflearn/api/zoo/__init__.py` & `carefree-learn-0.4.4/cflearn/api/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/callbacks/classification.py` & `carefree-learn-0.4.4/cflearn/callbacks/classification.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/callbacks/general.py` & `carefree-learn-0.4.4/cflearn/callbacks/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/callbacks/generator.py` & `carefree-learn-0.4.4/cflearn/callbacks/generator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/constants.py` & `carefree-learn-0.4.4/cflearn/constants.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/array.py` & `carefree-learn-0.4.4/cflearn/data/array.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/cv/crop.py` & `carefree-learn-0.4.4/cflearn/data/blocks/cv/crop.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/cv/image_folder.py` & `carefree-learn-0.4.4/cflearn/data/blocks/cv/image_folder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/cv/normalize.py` & `carefree-learn-0.4.4/cflearn/data/blocks/cv/normalize.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/cv/to_numpy.py` & `carefree-learn-0.4.4/cflearn/data/blocks/cv/to_numpy.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/cv/tuple_to_batch.py` & `carefree-learn-0.4.4/cflearn/data/blocks/cv/tuple_to_batch.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/ml/file.py` & `carefree-learn-0.4.4/cflearn/data/blocks/ml/file.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/ml/gather.py` & `carefree-learn-0.4.4/cflearn/data/blocks/ml/gather.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/ml/nan_handler.py` & `carefree-learn-0.4.4/cflearn/data/blocks/ml/nan_handler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/ml/preprocessor.py` & `carefree-learn-0.4.4/cflearn/data/blocks/ml/preprocessor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/ml/recognizer.py` & `carefree-learn-0.4.4/cflearn/data/blocks/ml/recognizer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/blocks/ml/splitter.py` & `carefree-learn-0.4.4/cflearn/data/blocks/ml/splitter.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/ml/api.py` & `carefree-learn-0.4.4/cflearn/data/ml/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/ml/datasets.py` & `carefree-learn-0.4.4/cflearn/data/ml/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/pytorch/api.py` & `carefree-learn-0.4.4/cflearn/data/pytorch/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/pytorch/datasets.py` & `carefree-learn-0.4.4/cflearn/data/pytorch/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/data/utils.py` & `carefree-learn-0.4.4/cflearn/data/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/dist/ml/experiment.py` & `carefree-learn-0.4.4/cflearn/dist/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/dist/ml/runs/_utils.py` & `carefree-learn-0.4.4/cflearn/dist/ml/runs/_utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/dist/ml/task.py` & `carefree-learn-0.4.4/cflearn/dist/ml/task.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/inference.py` & `carefree-learn-0.4.4/cflearn/inference.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/losses/basic.py` & `carefree-learn-0.4.4/cflearn/losses/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/losses/gan.py` & `carefree-learn-0.4.4/cflearn/losses/gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/losses/lpips.py` & `carefree-learn-0.4.4/cflearn/losses/lpips.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/losses/vae.py` & `carefree-learn-0.4.4/cflearn/losses/vae.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/metrics.py` & `carefree-learn-0.4.4/cflearn/metrics.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/misc/available.json` & `carefree-learn-0.4.4/cflearn/misc/available.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/misc/mixins.py` & `carefree-learn-0.4.4/cflearn/misc/mixins.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/misc/toolkit.py` & `carefree-learn-0.4.4/cflearn/misc/toolkit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/ae/common.py` & `carefree-learn-0.4.4/cflearn/models/cv/ae/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/ae/kl.py` & `carefree-learn-0.4.4/cflearn/models/cv/ae/kl.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/ae/vq.py` & `carefree-learn-0.4.4/cflearn/models/cv/ae/vq.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/classifier/vanilla.py` & `carefree-learn-0.4.4/cflearn/models/cv/classifier/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/decoder/attn.py` & `carefree-learn-0.4.4/cflearn/models/cv/decoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/decoder/schema.py` & `carefree-learn-0.4.4/cflearn/models/cv/decoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan.py` & `carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan_v2.py` & `carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan_v2.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/decoder/vanilla.py` & `carefree-learn-0.4.4/cflearn/models/cv/decoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/decoder/vqgan.py` & `carefree-learn-0.4.4/cflearn/models/cv/decoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/clip.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/rescaler.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/rescaler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/schema.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/ddpm.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/ldm.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/ldm.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,17 @@
 
     def get_lora_checkpoints(self) -> Dict[str, Optional[IHook]]:
         return self.lora_manager.checkpoint(self)
 
     def restore_lora_from(self, hooks: Dict[str, Optional[IHook]]) -> None:
         return self.lora_manager.restore(self, hooks)
 
+    def check_lora_exists(self, key: str) -> bool:
+        return self.lora_manager.has(key)
+
 
 __all__ = [
     "LDM",
     "SDLoRAMode",
     "StableDiffusion",
     "convert_lora",
 ]
```

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/basic.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/ddim.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/ddim.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/k_samplers.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/k_samplers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/plms.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/plms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/schema.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/solver.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/solver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/utils.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/unet.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/diffusion/utils.py` & `carefree-learn-0.4.4/cflearn/models/cv/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/attn.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/api.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/core.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/resnet.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/transformer.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/vgg.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/vgg.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/register.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/register.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/fnet.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/fnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/mixer.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/mixer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/perceiver.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/pool_former.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/pool_former.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/schema.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/transformer.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/vanilla.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/encoder/vqgan.py` & `carefree-learn-0.4.4/cflearn/models/cv/encoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/gan/discriminators.py` & `carefree-learn-0.4.4/cflearn/models/cv/gan/discriminators.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/gan/schema.py` & `carefree-learn-0.4.4/cflearn/models/cv/gan/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/gan/vanilla.py` & `carefree-learn-0.4.4/cflearn/models/cv/gan/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/general.py` & `carefree-learn-0.4.4/cflearn/models/cv/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/cv/translator/rrdb.py` & `carefree-learn-0.4.4/cflearn/models/cv/translator/rrdb.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/implicit/siren.py` & `carefree-learn-0.4.4/cflearn/models/implicit/siren.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/base.py` & `carefree-learn-0.4.4/cflearn/models/ml/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/ddr.py` & `carefree-learn-0.4.4/cflearn/models/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/encoders.py` & `carefree-learn-0.4.4/cflearn/models/ml/encoders.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/fcnn.py` & `carefree-learn-0.4.4/cflearn/models/ml/fcnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/linear.py` & `carefree-learn-0.4.4/cflearn/models/ml/linear.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/mixed_stacked.py` & `carefree-learn-0.4.4/cflearn/models/ml/mixed_stacked.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/nbm.py` & `carefree-learn-0.4.4/cflearn/models/ml/nbm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/ndt.py` & `carefree-learn-0.4.4/cflearn/models/ml/ndt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/rnn.py` & `carefree-learn-0.4.4/cflearn/models/ml/rnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/ml/wnd.py` & `carefree-learn-0.4.4/cflearn/models/ml/wnd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/multimodal/clip.py` & `carefree-learn-0.4.4/cflearn/models/multimodal/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/multimodal/schema.py` & `carefree-learn-0.4.4/cflearn/models/multimodal/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/nlp/encoder/transformer.py` & `carefree-learn-0.4.4/cflearn/models/nlp/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/clip.py` & `carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/schema.py` & `carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/nlp/transformers/core.py` & `carefree-learn-0.4.4/cflearn/models/nlp/transformers/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/nlp/transformers/opus.py` & `carefree-learn-0.4.4/cflearn/models/nlp/transformers/opus.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/nlp/transformers/simbert.py` & `carefree-learn-0.4.4/cflearn/models/nlp/transformers/simbert.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/schemas/custom.py` & `carefree-learn-0.4.4/cflearn/models/schemas/custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/models/schemas/cv.py` & `carefree-learn-0.4.4/cflearn/models/schemas/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/__init__.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/activations.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/activations.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/attentions.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/attentions.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/common.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/convs/basic.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/convs/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/convs/residual.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/convs/residual.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/customs.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/customs.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/high_level.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/high_level.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/hijacks.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/hijacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,17 @@
     def __init__(self) -> None:
         self.m = None
         self.injected = False
         self.lora_packs: Dict[str, LoRAPack] = {}
 
     # api
 
+    def has(self, key: str) -> bool:
+        return key in self.lora_packs
+
     def build_pack(self, *keys: str) -> Optional[LoRAPack]:
         if not keys:
             return None
         if len(keys) == 1:
             return self.lora_packs.get(keys[0])
         selected = [self.lora_packs.get(key) for key in keys]
         not_none = [pack for pack in selected if pack is not None]
```

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/hooks.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/hooks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/implementations/perceiver.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/implementations/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/mappings.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/mappings.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/api.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/channel_mixers.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/channel_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/poolers.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/poolers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/schema.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/token_mixers.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/token_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/norms.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/norms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/blocks/utils.py` & `carefree-learn-0.4.4/cflearn/modules/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/optimizers.py` & `carefree-learn-0.4.4/cflearn/modules/optimizers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/modules/schedulers.py` & `carefree-learn-0.4.4/cflearn/modules/schedulers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/monitors.py` & `carefree-learn-0.4.4/cflearn/monitors.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/parameters.py` & `carefree-learn-0.4.4/cflearn/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/pipeline/api.py` & `carefree-learn-0.4.4/cflearn/pipeline/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/pipeline/blocks/basic.py` & `carefree-learn-0.4.4/cflearn/pipeline/blocks/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/pipeline/blocks/ml.py` & `carefree-learn-0.4.4/cflearn/pipeline/blocks/ml.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/pipeline/blocks/utils.py` & `carefree-learn-0.4.4/cflearn/pipeline/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/pipeline/core.py` & `carefree-learn-0.4.4/cflearn/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/pipeline/third_party.py` & `carefree-learn-0.4.4/cflearn/pipeline/third_party.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/schema.py` & `carefree-learn-0.4.4/cflearn/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/scripts/sd.py` & `carefree-learn-0.4.4/cflearn/scripts/sd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/trainer.py` & `carefree-learn-0.4.4/cflearn/trainer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/types.py` & `carefree-learn-0.4.4/cflearn/types.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f4.json` & `carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f4.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ddpm/default.json` & `carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ddpm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/default.json` & `carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/vq.json` & `carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/vq.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/chinese.json` & `carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/chinese.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/zoo/core.py` & `carefree-learn-0.4.4/cflearn/zoo/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/cflearn/zoo/models/clip.py` & `carefree-learn-0.4.4/cflearn/zoo/models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.3/setup.py` & `carefree-learn-0.4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.4.3"
+VERSION = "0.4.4"
 DESCRIPTION = "Deep Learning with PyTorch made easy"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 cv_requires = [
     "ftfy",
     "lmdb",
@@ -32,15 +32,15 @@
 setup(
     name="carefree-learn",
     version=VERSION,
     packages=find_packages(exclude=("tests",)),
     install_requires=[
         "accelerate",
         "safetensors",
-        "carefree-toolkit>=0.3.4",
+        "carefree-toolkit>=0.3.5",
     ],
     extras_require={
         "onnx": onnx_requires,
         "cv": cv_requires,
         "cv_full": cv_full_requires,
         "full": cv_full_requires
         + onnx_requires
```

