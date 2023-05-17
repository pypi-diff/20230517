# Comparing `tmp/autogluon.multimodal-0.7.1b20230515.tar.gz` & `tmp/autogluon.multimodal-0.7.1b20230516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.1b20230515.tar", last modified: Mon May 15 09:04:26 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.1b20230516.tar", last modified: Tue May 16 09:04:21 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.1b20230515.tar` & `autogluon.multimodal-0.7.1b20230516.tar`

### file list

```diff
@@ -1,145 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.026159 autogluon.multimodal-0.7.1b20230515/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-15 09:04:26.026159 autogluon.multimodal-0.7.1b20230515/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:04:26.026159 autogluon.multimodal-0.7.1b20230515/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.010159 autogluon.multimodal-0.7.1b20230515/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.018159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.018159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.018159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26476 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.018159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    85367 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.022159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.022159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.022159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30882 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   121528 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24352 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.026159 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    50614 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-15 09:03:46.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:04:26.014159 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:04:25.000000 autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.281023 autogluon.multimodal-0.7.1b20230516/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-16 09:04:21.277023 autogluon.multimodal-0.7.1b20230516/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:04:21.281023 autogluon.multimodal-0.7.1b20230516/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.253023 autogluon.multimodal-0.7.1b20230516/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.257023 autogluon.multimodal-0.7.1b20230516/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.261023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.265023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.265023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.265023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26706 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.269023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85367 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.269023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.273023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.273023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122269 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.277023 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22164 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-16 09:03:40.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:04:21.257023 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:04:21.000000 autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.1b20230515/PKG-INFO` & `autogluon.multimodal-0.7.1b20230516/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230515
+Version: 0.7.1b20230516
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230515/setup.py` & `autogluon.multimodal-0.7.1b20230516/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 DEFAULT_SHOT = "default_shot"
 DEPRECATED_ZERO_SHOT = "zero_shot"
 NER = "ner"
 NAMED_ENTITY_RECOGNITION = "named_entity_recognition"
 FEATURE_EXTRACTION = "feature_extraction"
 ZERO_SHOT_IMAGE_CLASSIFICATION = "zero_shot_image_classification"
 OBJECT_DETECTION = "object_detection"
+OPEN_VOCABULARY_OBJECT_DETECTION = "open_vocabulary_object_detection"
 OCR = "ocr"
 OCR_TEXT_DETECTION = f"{OCR}_text_detection"
 OCR_TEXT_RECOGNITION = f"{OCR}_text_recognition"
 IMAGE_SIMILARITY = "image_similarity"
 TEXT_SIMILARITY = "text_similarity"
 IMAGE_TEXT_SIMILARITY = "image_text_similarity"
 
 # Input keys
 IMAGE = "image"
+IMAGE_META = "image_meta"
 IMAGE_VALID_NUM = "image_valid_num"
 LABEL = "label"
 TEXT_TOKEN_IDS = "text_token_ids"
 CHOICES_IDS = "choices_ids"
 TEXT_VALID_LENGTH = "text_valid_length"
 TEXT_SEGMENT_IDS = "text_segment_ids"
 COLUMN = "column"
@@ -234,14 +236,15 @@
 FUSION = "fusion"
 FUSION_MLP = f"{FUSION}_mlp"
 FUSION_TRANSFORMER = f"{FUSION}_transformer"
 FUSION_NER = f"{FUSION}_{NER}"
 MMDET_IMAGE = "mmdet_image"
 MMOCR_TEXT_DET = "mmocr_text_detection"
 MMOCR_TEXT_RECOG = "mmocr_text_recognition"
+OVD = "ovd"
 NER_TEXT = "ner_text"
 DOCUMENT_TRANSFORMER = "document_transformer"
 HF_MODELS = (HF_TEXT, T_FEW, CLIP, NER_TEXT, DOCUMENT_TRANSFORMER)
 MMLAB_MODELS = (MMDET_IMAGE, MMOCR_TEXT_DET, MMOCR_TEXT_RECOG)
 
 # matcher loss type
 CONTRASTIVE_LOSS = "contrastive_loss"
@@ -281,14 +284,18 @@
 TRIPLET = "triplet"
 
 # mmdet
 XYWH = "xywh"
 XYXY = "xyxy"
 BBOX_FORMATS = [XYWH, XYXY]
 
+# open vocabulary detection
+PROMPT = "prompt"
+OVD_RET = "ovd_ret"
+
 # presets
 DEFAULT = "default"
 HIGH_QUALITY = "high_quality"
 MEDIUM_QUALITY = "medium_quality"
 BEST_QUALITY = "best_quality"
 ALL_MODEL_QUALITIES = [HIGH_QUALITY, MEDIUM_QUALITY, BEST_QUALITY, DEFAULT]
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 from .process_categorical import CategoricalProcessor
 from .process_document import DocumentProcessor
 from .process_image import ImageProcessor
 from .process_label import LabelProcessor
 from .process_mmlab import MMDetProcessor, MMOcrProcessor
 from .process_ner import NerProcessor
 from .process_numerical import NumericalProcessor
+from .process_ovd import OVDProcessor
 from .process_text import TextProcessor
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/infer_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     IMAGE_PATH,
     MULTICLASS,
     NER,
     NER_ANNOTATION,
     NULL,
     NUMERICAL,
     OBJECT_DETECTION,
+    OPEN_VOCABULARY_OBJECT_DETECTION,
     REGRESSION,
     ROIS,
     TEXT,
     TEXT_NER,
 )
 from .utils import is_rois_input
 
@@ -211,15 +212,14 @@
                 else:
                     raise ValueError(f"Unsupported image type: {image_type}")
             except:
                 success = False
                 break
 
             success = True
-
         if not success:
             failure_count += 1
     failure_ratio = failure_count / sample_num
     # Tolerate high failure rate in case that many image files may be corrupted.
     if failure_ratio <= 0.9:
         if failure_ratio > 0:
             warnings.warn(
@@ -637,15 +637,15 @@
             )
         if problem_type in [MULTICLASS, BINARY, CLASSIFICATION]:
             column_types[col_name] = CATEGORICAL
         elif problem_type == REGRESSION:
             column_types[col_name] = NUMERICAL
         elif problem_type == NER:
             column_types[col_name] = NER_ANNOTATION
-        elif problem_type == OBJECT_DETECTION:
+        elif problem_type in [OBJECT_DETECTION, OPEN_VOCABULARY_OBJECT_DETECTION]:
             column_types[col_name] = ROIS
 
         if column_types[col_name] not in allowable_label_types:
             column_types[col_name] = fallback_label_type
 
     return column_types
 
@@ -717,21 +717,23 @@
                 return MULTICLASS, class_num
         elif provided_problem_type == REGRESSION:
             return provided_problem_type, 1
         elif provided_problem_type == NER:
             return provided_problem_type, None
         elif provided_problem_type == OBJECT_DETECTION:
             return provided_problem_type, None
+        elif provided_problem_type == OPEN_VOCABULARY_OBJECT_DETECTION:
+            return provided_problem_type, None
         else:
             raise ValueError(
                 f"Problem type '{provided_problem_type}' doesn't have a valid output shape "
                 f"for training. The supported problem types are"
                 f" '{BINARY}', '{MULTICLASS}', '{REGRESSION}',"
                 f" '{CLASSIFICATION}', '{NER}',"
-                f" '{OBJECT_DETECTION}'"
+                f" '{OBJECT_DETECTION}', '{OPEN_VOCABULARY_OBJECT_DETECTION}'"
             )
     else:
         if column_types[label_column] == CATEGORICAL:
             class_num = len(data[label_column].unique())
             if class_num == 2:
                 return BINARY, 2
             else:
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     IMAGE_BYTEARRAY,
     IMAGE_PATH,
     LABEL,
     NER,
     NER_ANNOTATION,
     NULL,
     NUMERICAL,
+    OVD,
     ROIS,
     TEXT,
     TEXT_NER,
 )
 from .label_encoder import CustomLabelEncoder
 
 logger = logging.getLogger(__name__)
@@ -250,14 +251,19 @@
 
     def get_column_names(self, modality: str):
         if modality.startswith(IMAGE):
             if hasattr(self, "_image_path_names"):
                 return self._image_path_names
             else:
                 return self._image_feature_names
+        elif modality == OVD:
+            if hasattr(self, "_image_path_names"):
+                return self._image_path_names + self._text_feature_names
+            else:
+                return self._image_feature_names + self._text_feature_names
         elif modality == ROIS:
             return self._rois_feature_names
         elif modality == TEXT:
             return self._text_feature_names
         elif modality == CATEGORICAL:
             return self._categorical_feature_names
         elif modality == NUMERICAL:
@@ -481,14 +487,58 @@
                 raise ValueError(f"Unknown image type {col_type} for column {col_name}")
 
             ret_data[col_name] = processed_data
             ret_type[col_name] = self._column_types[col_name]
 
         return ret_data, ret_type
 
+    def transform_ovd(
+        self,
+        df: pd.DataFrame,
+    ) -> Tuple[Dict[str, List[List[str]]], Dict[str, str]]:
+        """
+        Preprocess image + prompt data.
+        For image data we preprocess them by collecting their paths together. If one sample has multiple images
+        in an image column, assume that their image paths are separated by ";".
+        For rois data we simply convert them from a column of pandas dataframe to a list.
+        This function needs to be called preceding the rois processor in "process_rois.py".
+
+        Parameters
+        ----------
+        df
+            The multimodal pd.DataFrame.
+
+        Returns
+        -------
+        image_features
+            All the image data stored in a dictionary.
+        image_types
+            The column types of these image data, e.g., image_path or image_identifier.
+        """
+        assert (
+            self._fit_called or self._fit_x_called
+        ), "You will need to first call preprocessor.fit_x() before calling preprocessor.transform_ovd."
+
+        x = self.transform_image(df)
+        ret_data = x[0]
+        ret_type = x[1]
+
+        for col_name in self._text_feature_names:
+            col_type = self._column_types[col_name]
+
+            if col_type == TEXT:
+                processed_data = df[col_name].tolist()
+            else:
+                raise ValueError(f"Unknown text type {col_type} for column {col_name}")
+
+            ret_data[col_name] = processed_data
+            ret_type[col_name] = self._column_types[col_name]
+
+        return ret_data, ret_type
+
     def transform_image(
         self,
         df: pd.DataFrame,
     ) -> Tuple[Dict[str, List[List[str]]], Dict[str, str]]:
         """
         Preprocess image data by collecting their paths together. If one sample has multiple images
         in an image column, assume that their image paths are separated by ";".
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/data/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 import ast
 import codecs
 import copy
 import re
 import warnings
+from io import BytesIO
 from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
+import PIL
 from omegaconf import ListConfig
 from text_unidecode import unidecode
 from timm.data.constants import (
     IMAGENET_DEFAULT_MEAN,
     IMAGENET_DEFAULT_STD,
     IMAGENET_INCEPTION_MEAN,
     IMAGENET_INCEPTION_STD,
 )
 from tokenizers import pre_tokenizers
 from torchvision import transforms
 
-from ..constants import CLIP_IMAGE_MEAN, CLIP_IMAGE_STD, IDENTIFIER, IMAGE, MMDET_IMAGE, MMLAB_MODELS
+from ..constants import (
+    CLIP_IMAGE_MEAN,
+    CLIP_IMAGE_STD,
+    IDENTIFIER,
+    IMAGE,
+    IMAGE_BYTEARRAY,
+    IMAGE_PATH,
+    MMDET_IMAGE,
+    MMLAB_MODELS,
+)
 from .collator import DictCollator
 from .preprocess_dataframe import MultiModalFeaturePreprocessor
 
 try:
     from torchvision.transforms import InterpolationMode
 
     BICUBIC = InterpolationMode.BICUBIC
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 from .huggingface_text import HFAutoModelForTextPrediction
 from .mmdet_image import MMDetAutoModelForObjectDetection
 from .mmocr_text_detection import MMOCRAutoModelForTextDetection
 from .mmocr_text_recognition import MMOCRAutoModelForTextRecognition
 from .ner_text import HFAutoModelForNER
 from .numerical_mlp import NumericalMLP
 from .numerical_transformer import NumericalTransformer
+from .ovd import OVDModel
 from .t_few import TFewModel
 from .timm_image import TimmAutoModelForImagePrediction
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/optimization/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     MEAN_AVERAGE_PRECISION,
     MULTI_NEGATIVES_SOFTMAX_LOSS,
     MULTICLASS,
     NER,
     NER_TOKEN_F1,
     NORM_FIT,
     OBJECT_DETECTION,
+    OPEN_VOCABULARY_OBJECT_DETECTION,
     OVERALL_ACCURACY,
     PAIR_MARGIN_MINER,
     PEARSONR,
     PEFT_STRATEGIES,
     QUADRATIC_KAPPA,
     R2,
     RECALL,
@@ -116,15 +117,15 @@
                 loss_func = nn.BCEWithLogitsLoss()
             else:
                 loss_func = nn.MSELoss()
         else:
             loss_func = nn.MSELoss()
     elif problem_type == NER:
         loss_func = nn.CrossEntropyLoss(ignore_index=0)
-    elif problem_type == OBJECT_DETECTION:
+    elif problem_type in [OBJECT_DETECTION, OPEN_VOCABULARY_OBJECT_DETECTION]:
         return None
     elif problem_type is None:
         return None
     else:
         raise NotImplementedError
 
     return loss_func
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     MULTICLASS,
     NER,
     NER_RET,
     NUMERICAL,
     OBJECT_DETECTION,
     OCR_TEXT_DETECTION,
     OCR_TEXT_RECOGNITION,
+    OPEN_VOCABULARY_OBJECT_DETECTION,
+    OVD_RET,
     OVERALL_F1,
     RAY_TUNE_CHECKPOINT,
     REGRESSION,
     ROIS,
     SCORE,
     TEXT,
     TEXT_NER,
@@ -146,14 +148,15 @@
     load_text_tokenizers,
     logits_to_prob,
     merge_bio_format,
     modify_duplicate_model_names,
     object_detection_data_to_df,
     predict,
     process_batch,
+    save_ovd_result_df,
     save_pretrained_model_configs,
     save_result_df,
     save_text_tokenizers,
     select_model,
     setup_detection_train_tuning_data,
     setup_save_path,
     split_hyperparameters,
@@ -211,14 +214,15 @@
             - 'multiclass': Multi-class classification
             - 'regression': Regression
             - 'classification': Classification problems include 'binary' and 'multiclass' classification.
 
             In addition, we support advanced problems such as
 
             - 'object_detection': Object detection
+            - 'open_vocabulry_object_detection': Zero-shot object detection (only support inference for now, finetuning TBC)
             - 'ner' or 'named_entity_recognition': Named entity extraction
             - 'text_similarity': Text-text similarity problem
             - 'image_similarity': Image-image similarity problem
             - 'image_text_similarity': Text-image similarity problem
             - 'feature_extraction': Extracting feature (only support inference)
             - 'zero_shot_image_classification': Zero-shot image classification (only support inference)
             - 'few_shot_text_classification': (experimental) Few-shot text classification
@@ -227,14 +231,15 @@
 
             For certain problem types, the default behavior is to load a pretrained model based on
             the presets / hyperparameters and the predictor will support zero-shot inference
             (running inference without .fit()). This includes the following
             problem types:
 
             - 'object_detection'
+            - 'open_vocabulry_object_detection'
             - 'text_similarity'
             - 'image_similarity'
             - 'image_text_similarity'
             - 'feature_extraction'
             - 'zero_shot_image_classification'
             - 'few_shot_text_classification' (experimental)
             - 'ocr_text_detection' (experimental)
@@ -1979,14 +1984,16 @@
                     metrics=metrics,
                     return_pred=return_pred,
                     eval_tool="torchmetrics",
                 )
 
         if self._problem_type == NER:
             ret_type = NER_RET
+        elif self._problem_type == OPEN_VOCABULARY_OBJECT_DETECTION:
+            ret_type = OVD_RET
         else:
             ret_type = LOGITS
 
         outputs = predict(
             predictor=self,
             data=data,
             requires_label=True,
@@ -2142,24 +2149,27 @@
             )
         if self._problem_type == OBJECT_DETECTION:
             data = object_detection_data_to_df(data)
 
             if self._label_column not in data:
                 self._label_column = None
 
-        if self._problem_type == OBJECT_DETECTION or self._problem_type == OCR_TEXT_DETECTION:
+        if self._problem_type in [OBJECT_DETECTION, OCR_TEXT_DETECTION]:
             ret_type = BBOX
         elif self._problem_type == OCR_TEXT_RECOGNITION:
             ret_type = [TEXT, SCORE]
         else:
             ret_type = LOGITS
 
         if self._problem_type == NER:
             ret_type = NER_RET
 
+        if self._problem_type == OPEN_VOCABULARY_OBJECT_DETECTION:
+            ret_type = OVD_RET
+
         if candidate_data:
             pred = self._match_queries_and_candidates(
                 query_data=data,
                 candidate_data=candidate_data,
                 return_prob=False,
             )
         else:
@@ -2221,14 +2231,22 @@
             if self._problem_type == OBJECT_DETECTION:
                 pred = save_result_df(
                     pred=pred,
                     data=data,
                     detection_classes=self._model.model.CLASSES,
                     result_path=None,
                 )
+            elif (
+                self._problem_type == OPEN_VOCABULARY_OBJECT_DETECTION
+            ):  # TODO: refactor and merge with OBJECT DETECTION
+                pred = save_ovd_result_df(
+                    pred=pred,
+                    data=data,
+                    result_path=None,
+                )
             else:
                 pred = self._as_pandas(data=data, to_be_converted=pred)
 
         return pred
 
     def predict_proba(
         self,
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,62 @@
     else:
         raise ValueError(f"Unknown preset type: {presets}")
 
     return hyperparameters, hyperparameter_tune_kwargs
 
 
 @automm_presets.register()
+def open_vocabulary_object_detection(presets: str = DEFAULT):
+    """
+    Register the presets for open_vocabulary_object_detection.
+
+    Parameters
+    ----------
+    presets
+        The preset name.
+
+    Returns
+    -------
+    hyperparameters
+        The hyperparameters for a given preset.
+    hyperparameter_tune_kwargs
+        The hyperparameter tuning kwargs.
+    """
+    hyperparameters = {
+        "model.names": ["ovd"],  # TODO: update with more preset hps
+        "env.num_gpus": 1,  # TODO: add multi gpu support and remove this
+        "env.eval_batch_size_ratio": 1,
+    }
+    hyperparameter_tune_kwargs = {}
+
+    if presets in [DEFAULT, BEST_QUALITY]:
+        hyperparameters.update(
+            {
+                "model.ovd.checkpoint_name": "GroundingDINO_SwinB",
+            }
+        )
+    elif presets == HIGH_QUALITY:
+        hyperparameters.update(
+            {
+                "model.ovd.checkpoint_name": "GroundingDINO_SwinT_OGC",
+            }
+        )
+    elif presets == MEDIUM_QUALITY:
+        hyperparameters.update(
+            {
+                "model.ovd.checkpoint_name": "GroundingDINO_SwinT_OGC",
+            }
+        )
+    else:
+        raise ValueError(f"Unknown preset type: {presets}")
+
+    return hyperparameters, hyperparameter_tune_kwargs
+
+
+@automm_presets.register()
 def object_detection(presets: str = DEFAULT):
     """
     Register the presets for object_detection.
 
     Parameters
     ----------
     presets
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/problem_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     NAMED_ENTITY_RECOGNITION,
     NER,
     NER_ANNOTATION,
     NUMERICAL,
     OBJECT_DETECTION,
     OCR_TEXT_DETECTION,
     OCR_TEXT_RECOGNITION,
+    OPEN_VOCABULARY_OBJECT_DETECTION,
     REGRESSION,
     ROIS,
     TEXT,
     TEXT_NER,
     TEXT_SIMILARITY,
     ZERO_SHOT_IMAGE_CLASSIFICATION,
 )
@@ -115,14 +116,27 @@
         support_zero_shot=True,
         supported_modality_type={IMAGE},
         supported_label_type={ROIS},
         force_exist_modality={IMAGE},
     ),
 )
 
+# Open Vocabulary Object detection: image --> bounding boxes
+PROBLEM_TYPES_REG.register(
+    OPEN_VOCABULARY_OBJECT_DETECTION,
+    ProblemTypeProperty(
+        name=OPEN_VOCABULARY_OBJECT_DETECTION,
+        support_zero_shot=True,
+        support_fit=False,  # TODO: future work
+        supported_modality_type={IMAGE, TEXT},
+        supported_label_type={ROIS},
+        force_exist_modality={IMAGE},
+    ),
+)
+
 # Matching: text <--> text, image <--> image, text <--> image
 PROBLEM_TYPES_REG.register(
     TEXT_SIMILARITY,
     ProblemTypeProperty(
         name=TEXT_SIMILARITY,
         support_zero_shot=True,
         is_matching=True,
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from .matcher import compute_semantic_similarity, convert_data_for_ranking, create_siamese_model, semantic_search
 from .metric import compute_ranking_score, compute_score, get_minmax_mode, get_stopping_threshold, infer_metrics
 from .misc import logits_to_prob, merge_bio_format, shopee_dataset, tensor_to_ndarray, visualize_ner
 from .mmcv import CollateMMDet, CollateMMOcr, send_datacontainers_to_device, unpack_datacontainers
 from .model import create_fusion_model, create_model, list_timm_models, modify_duplicate_model_names, select_model
 from .object_detection import (
     COCODataset,
+    bbox_ratio_xywh_to_index_xyxy,
     bbox_xyxy_to_xywh,
     cocoeval,
     convert_pred_to_xywh,
     evaluate_coco,
     from_coco,
     from_coco_or_voc,
     from_dict,
@@ -68,9 +69,10 @@
     save_result_coco_format,
     save_result_df,
     save_result_voc_format,
     setup_detection_train_tuning_data,
     visualize_detection,
 )
 from .object_detection_visualizer import Visualizer
+from .ovd import save_ovd_result_df
 from .pipeline import init_pretrained, init_pretrained_matcher
 from .save import process_save_path, save_text_tokenizers, setup_save_path
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/colormap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+# ------------------------------------------------------------------------
 # Copyright (c) Facebook, Inc. and its affiliates.
+# ------------------------------------------------------------------------
 
 """
 An awesome colormap for really neat visualizations.
 Copied from Detectron, and removed gray colors.
 """
 import random
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     IMAGE_PATH,
     LABEL,
     MMLAB_MODELS,
     NER,
     NER_ANNOTATION,
     NER_TEXT,
     NUMERICAL,
+    OVD,
     ROIS,
     TEXT,
     TEXT_NER,
 )
 from ..data import (
     CategoricalProcessor,
     DocumentProcessor,
@@ -41,14 +42,15 @@
     MixupModule,
     MMDetProcessor,
     MMOcrProcessor,
     MultiModalFeaturePreprocessor,
     NerLabelEncoder,
     NerProcessor,
     NumericalProcessor,
+    OVDProcessor,
     TextProcessor,
 )
 from ..data.infer_types import is_image_column
 
 logger = logging.getLogger(__name__)
 
 
@@ -175,14 +177,20 @@
         )
     elif data_type == ROIS:
         data_processor = MMDetProcessor(
             model=model,
             max_img_num_per_col=model_config.max_img_num_per_col,
             missing_value_strategy=config.data.image.missing_value_strategy,
         )
+    elif data_type == OVD:
+        data_processor = OVDProcessor(
+            model=model,
+            max_img_num_per_col=model_config.max_img_num_per_col,
+            missing_value_strategy=config.data.image.missing_value_strategy,
+        )
     elif data_type == DOCUMENT:
         train_transforms, val_transforms = get_image_transforms(
             model_config=model_config,
             model_name=model.prefix,
             advanced_hyperparameters=advanced_hyperparameters,
         )
         data_processor = DocumentProcessor(
@@ -233,14 +241,15 @@
         TEXT: [],
         CATEGORICAL: [],
         NUMERICAL: [],
         LABEL: [],
         ROIS: [],
         TEXT_NER: [],
         DOCUMENT: [],
+        OVD: [],
     }
 
     model_dict = {model.prefix: model}
 
     if model.prefix.lower().startswith("fusion"):
         for per_model in model.model:
             model_dict[per_model.prefix] = per_model
@@ -273,25 +282,36 @@
                     data_type=ROIS,
                     config=config,
                     model=per_model,
                 )
             )
             if data_types is not None and IMAGE in data_types:
                 data_types.remove(IMAGE)
+        elif per_name == OVD:
+            # create a multimodal processor for OVD.
+            data_processors[OVD].append(
+                create_data_processor(
+                    data_type=OVD,
+                    config=config,
+                    model=per_model,
+                )
+            )
+            if data_types is not None and IMAGE in data_types:
+                data_types.remove(IMAGE)
 
         if requires_label:
             # each model has its own label processor
             label_processor = create_data_processor(
                 data_type=LABEL,
                 config=config,
                 model=per_model,
             )
             data_processors[LABEL].append(label_processor)
 
-        if requires_data and data_types:
+        if requires_data and data_types and per_name != OVD:  # currently OVD does not require additional processors
             for data_type in data_types:
                 per_data_processor = create_data_processor(
                     data_type=data_type,
                     model=per_model,
                     config=config,
                     advanced_hyperparameters=advanced_hyperparameters,
                 )
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 
 from ..constants import (
     AUTOMM,
     BBOX,
     COLUMN_FEATURES,
     FEATURES,
     IMAGE,
+    IMAGE_META,
     LOGITS,
     MASKS,
     NER,
     NER_ANNOTATION,
     NER_RET,
     OBJECT_DETECTION,
+    OPEN_VOCABULARY_OBJECT_DETECTION,
+    OVD_RET,
     PROBABILITY,
+    PROMPT,
     QUERY,
     RESPONSE,
     SCORE,
     TEXT,
     TOKEN_WORD_MAPPING,
     WORD_OFFSETS,
 )
@@ -80,14 +84,36 @@
     elif ret_type == MASKS:
         ret = {}
         feature_masks = [ele[COLUMN_FEATURES][MASKS] for ele in outputs]  # a list of dicts
         for feature_name in feature_masks[0].keys():
             ret[feature_name] = torch.cat([ele[feature_name] for ele in feature_masks])
     elif ret_type == BBOX:
         return [ele[BBOX] for ele in outputs]
+    elif ret_type == OVD_RET:
+        from .object_detection import bbox_ratio_xywh_to_index_xyxy
+
+        ovd_pred = []
+        for ele in outputs:
+            curr_batch_size = len(ele[BBOX])
+            for i in range(curr_batch_size):
+                curr_pred = []
+                curr_pred_size = len(ele[BBOX][i])
+                for j in range(curr_pred_size):
+                    curr_pred.append(
+                        {
+                            "bbox": bbox_ratio_xywh_to_index_xyxy(
+                                xywh=ele[BBOX][i][j].detach().cpu().numpy(),
+                                image_wh=ele[IMAGE_META][i],
+                            )[0],
+                            "class": ele[PROMPT][i][j],
+                            "score": ele[LOGITS][i][j].detach().cpu().numpy(),
+                        }
+                    )
+                ovd_pred.append(curr_pred)
+        return ovd_pred
     elif ret_type == TEXT:
         return [ele[TEXT] for ele in outputs]  # single image
     elif ret_type == SCORE:
         return [ele[SCORE] for ele in outputs]
     elif ret_type == NER_RET:
         ner_pred = []
         as_ndarray = False
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     MAP,
     METRIC_MODE_MAP,
     MULTICLASS,
     NDCG,
     NER,
     NER_TOKEN_F1,
     OBJECT_DETECTION,
+    OPEN_VOCABULARY_OBJECT_DETECTION,
     OVERALL_ACCURACY,
     OVERALL_F1,
     PRECISION,
     RECALL,
     REGRESSION,
     RETRIEVAL_METRICS,
     RMSE,
@@ -106,15 +107,15 @@
     elif problem_type == BINARY:
         eval_metric_name = ROC_AUC
     elif problem_type == REGRESSION:
         if is_matching:
             eval_metric_name = SPEARMANR
         else:
             eval_metric_name = RMSE
-    elif problem_type == OBJECT_DETECTION:
+    elif problem_type in [OBJECT_DETECTION, OPEN_VOCABULARY_OBJECT_DETECTION]:
         if (not validation_metric_name) or validation_metric_name.lower() == MAP:
             return MAP, MAP
         elif validation_metric_name.lower() == DIRECT_LOSS:
             return DIRECT_LOSS, MAP
         else:
             raise ValueError(
                 f"Problem type: {problem_type}, validation_metric_name: {validation_metric_name} is not supported!"
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     MMOCR_TEXT_DET,
     MMOCR_TEXT_RECOG,
     NER,
     NER_TEXT,
     NUMERICAL,
     NUMERICAL_MLP,
     NUMERICAL_TRANSFORMER,
+    OVD,
     T_FEW,
     TEXT,
     TEXT_NER,
     TIMM_IMAGE,
     XYXY,
 )
 from ..data import MultiModalFeaturePreprocessor
@@ -47,14 +48,15 @@
     MMOCRAutoModelForTextDetection,
     MMOCRAutoModelForTextRecognition,
     MultimodalFusionMLP,
     MultimodalFusionNER,
     MultimodalFusionTransformer,
     NumericalMLP,
     NumericalTransformer,
+    OVDModel,
     TFewModel,
     TimmAutoModelForImagePrediction,
 )
 from ..models.utils import inject_adaptation_to_linear_layer
 
 logger = logging.getLogger(__name__)
 
@@ -309,14 +311,20 @@
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             config_file=OmegaConf.select(model_config, "config_file", default=None),
             classes=classes,
             pretrained=pretrained,
             output_bbox_format=OmegaConf.select(model_config, "output_bbox_format", default=XYXY),
         )
+    elif model_name.lower().startswith(OVD):
+        model = OVDModel(
+            prefix=model_name,
+            checkpoint_name=model_config.checkpoint_name,
+            pretrained=pretrained,
+        )
     elif model_name.lower().startswith(MMOCR_TEXT_DET):
         model = MMOCRAutoModelForTextDetection(
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
         )
     elif model_name.lower().startswith(MMOCR_TEXT_RECOG):
         model = MMOCRAutoModelForTextRecognition(
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/object_detection.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     MAR_10,
     MAR_100,
     MAR_LARGE,
     MAR_MEDIUM,
     MAR_SMALL,
     MEAN_AVERAGE_PRECISION,
     OBJECT_DETECTION,
+    OPEN_VOCABULARY_OBJECT_DETECTION,
 )
 from .download import download, is_url
 from .inference import predict
 from .save import setup_save_path
 
 logger = logging.getLogger(__name__)
 
@@ -479,14 +480,93 @@
             raise IndexError("Bounding boxes must have n * 4 elements, given {}".format(xywh.shape))
         xyxy = np.hstack((xywh[:, :2], xywh[:, :2] + np.maximum(0, xywh[:, 2:4] - 1)))
         return xyxy
     else:
         raise TypeError("Expect input xywh a list, tuple or numpy.ndarray, given {}".format(type(xywh)))
 
 
+def bbox_ratio_xywh_to_index_xyxy(
+    xywh: Optional[Union[list, tuple, np.ndarray]], image_wh: Optional[Union[list, tuple, np.ndarray]]
+):
+    """
+    Convert bounding boxes from format (x_center_ratio, y_center_ratio, w_ratio, h_ratio) to (xmin, ymin, xmax, ymax) in pixel index.
+
+    Parameters
+    ----------
+    xywh
+        The bbox in format (x_center_ratio, y_center_ratio, w_ratio, h_ratio).
+        If numpy.ndarray is provided, we expect multiple bounding boxes with
+        shape `(N, 4)`.
+
+    Returns
+    -------
+    A tuple or numpy.ndarray.
+    The converted bboxes in format (xmin, ymin, xmax, ymax).
+    If input is numpy.ndarray, return is numpy.ndarray correspondingly.
+    """
+    if isinstance(xywh, (tuple, list)):
+        assert isinstance(
+            image_wh, (tuple, list)
+        ), f"image_wh (type: {type(image_wh)} should have the same type with xywh (type: {type(xywh)})"
+
+        if not len(xywh) == 4:
+            raise IndexError("Bounding boxes must have 4 elements, given {}".format(len(xywh)))
+        if not len(image_wh) == 2:
+            raise IndexError("Image Width and Height must have 2 elements, given {}".format(len(image_wh)))
+
+        x, y = xywh[:2]
+        w, h = np.maximum(xywh[2] - 1, 0), np.maximum(xywh[3] - 1, 0)
+        W, H = np.maximum(image_wh[0] - 1, 0), np.maximum(image_wh[1] - 1, 0)
+
+        # ratio to index
+        x *= W
+        y *= H
+        W *= W
+        H *= H
+
+        # mid to upper left corner
+        x -= W / 2
+        y -= H / 2
+
+        return x, y, x + w, y + h  # xywh to xyxy
+    elif isinstance(xywh, np.ndarray):
+        if isinstance(image_wh, np.ndarray):
+
+            if not xywh.size % 4 == 0:
+                raise IndexError("Bounding boxes must have n * 4 elements, given {}".format(xywh.shape))
+            if not image_wh.size % 2 == 0:
+                raise IndexError("Image Width and Height must have n * 2 elements, given {}".format(image_wh.shape))
+
+            xywh = xywh * np.concat([image_wh, image_wh], axis=1)  # ratio to index
+
+            # mid to upper left corner
+            xywh[:, :2] -= xywh[:, 2:] / 2
+
+            # xywh to xyxy
+            xyxy = np.hstack((xywh[:, :2], xywh[:, :2] + np.maximum(0, xywh[:, 2:] - 1)))
+            return xyxy
+        elif isinstance(image_wh, (tuple, list)):
+
+            if not xywh.size % 4 == 0:
+                raise IndexError("Bounding boxes must have n * 4 elements, given {}".format(xywh.shape))
+
+            W, H = np.maximum(image_wh[0] - 1, 0), np.maximum(image_wh[1] - 1, 0)
+
+            xywh = xywh * np.array([[W, H, W, H]])  # ratio to index
+
+            # mid to upper left corner
+            xywh[:, :2] -= xywh[:, 2:] / 2
+
+            # xywh to xyxy
+            xyxy = np.hstack((xywh[:, :2], xywh[:, :2] + np.maximum(0, xywh[:, 2:] - 1)))
+            return xyxy
+    else:
+        raise TypeError("Expect input xywh a list, tuple or numpy.ndarray, given {}".format(type(xywh)))
+
+
 def bbox_xyxy_to_xywh(xyxy: Optional[Union[list, tuple, np.ndarray]]):
     """
     Convert bounding boxes from format (xmin, ymin, xmax, ymax) to (x, y, w, h). Modified from gluon cv.
 
     Parameters
     ----------
     xyxy
@@ -1496,16 +1576,18 @@
     anno_file
         The annotation file in COCO format
     return_pred
         Whether to return the prediction result of each row.
     eval_tool
         The eval_tool for object detection. Could be "pycocotools" or "torchmetrics".
     """
-    assert predictor._problem_type == OBJECT_DETECTION, (
-        f"predictor.evaluate_coco() is only supported when problem_type is {OBJECT_DETECTION}. "
+    assert (
+        predictor._problem_type == OBJECT_DETECTION or predictor._problem_type == OPEN_VOCABULARY_OBJECT_DETECTION
+    ), (
+        f"predictor.evaluate_coco() is only supported when problem_type is {OBJECT_DETECTION} or {OPEN_VOCABULARY_OBJECT_DETECTION}. "
         f"Received problem_type={predictor._problem_type}."
     )
     if isinstance(anno_file_or_df, str):
         anno_file = anno_file_or_df
         data = from_coco_or_voc(anno_file, "test")  # TODO: maybe remove default splits hardcoding (only used in VOC)
         if os.path.isdir(anno_file):
             eval_tool = "torchmetrics"  # we can only use torchmetrics for VOC format evaluation.
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.1b20230516/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230515
+Version: 0.7.1b20230516
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,33 @@
 src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
 src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8x8_300e_coco.py
 src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8x8_300e_coco.py
 src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8x8_300e_coco.py
 src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8x8_300e_coco.py
 src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8x8_300e_coco.py
 src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8x8_300e_coco.py
+src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
 src/autogluon/multimodal/data/__init__.py
 src/autogluon/multimodal/data/collator.py
 src/autogluon/multimodal/data/datamodule.py
 src/autogluon/multimodal/data/dataset.py
 src/autogluon/multimodal/data/infer_types.py
 src/autogluon/multimodal/data/label_encoder.py
 src/autogluon/multimodal/data/mixup.py
 src/autogluon/multimodal/data/preprocess_dataframe.py
 src/autogluon/multimodal/data/process_categorical.py
 src/autogluon/multimodal/data/process_document.py
 src/autogluon/multimodal/data/process_image.py
 src/autogluon/multimodal/data/process_label.py
 src/autogluon/multimodal/data/process_ner.py
 src/autogluon/multimodal/data/process_numerical.py
+src/autogluon/multimodal/data/process_ovd.py
 src/autogluon/multimodal/data/process_text.py
 src/autogluon/multimodal/data/randaug.py
 src/autogluon/multimodal/data/template_engine.py
 src/autogluon/multimodal/data/templates.py
 src/autogluon/multimodal/data/trivial_augmenter.py
 src/autogluon/multimodal/data/utils.py
 src/autogluon/multimodal/data/dataset_mmlab/__init__.py
@@ -72,14 +77,15 @@
 src/autogluon/multimodal/models/mlp.py
 src/autogluon/multimodal/models/mmdet_image.py
 src/autogluon/multimodal/models/mmocr_text_detection.py
 src/autogluon/multimodal/models/mmocr_text_recognition.py
 src/autogluon/multimodal/models/ner_text.py
 src/autogluon/multimodal/models/numerical_mlp.py
 src/autogluon/multimodal/models/numerical_transformer.py
+src/autogluon/multimodal/models/ovd.py
 src/autogluon/multimodal/models/t_few.py
 src/autogluon/multimodal/models/timm_image.py
 src/autogluon/multimodal/models/utils.py
 src/autogluon/multimodal/models/fusion/__init__.py
 src/autogluon/multimodal/models/fusion/base.py
 src/autogluon/multimodal/models/fusion/fusion_mlp.py
 src/autogluon/multimodal/models/fusion/fusion_ner.py
@@ -116,9 +122,10 @@
 src/autogluon/multimodal/utils/misc.py
 src/autogluon/multimodal/utils/mmcv.py
 src/autogluon/multimodal/utils/model.py
 src/autogluon/multimodal/utils/nlpaug.py
 src/autogluon/multimodal/utils/object_detection.py
 src/autogluon/multimodal/utils/object_detection_visualizer.py
 src/autogluon/multimodal/utils/onnx.py
+src/autogluon/multimodal/utils/ovd.py
 src/autogluon/multimodal/utils/pipeline.py
 src/autogluon/multimodal/utils/save.py
```

### Comparing `autogluon.multimodal-0.7.1b20230515/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.1b20230516/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.1b20230515
-autogluon.features==0.7.1b20230515
-autogluon.common==0.7.1b20230515
+autogluon.core[raytune]==0.7.1b20230516
+autogluon.features==0.7.1b20230516
+autogluon.common==0.7.1b20230516
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>0.1.5
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

