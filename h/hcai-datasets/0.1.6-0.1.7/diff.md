# Comparing `tmp/hcai-datasets-0.1.6.tar.gz` & `tmp/hcai-datasets-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-0.1.6.tar", last modified: Fri Mar 17 12:42:45 2023, max compression
+gzip compressed data, was "hcai-datasets-0.1.7.tar", last modified: Wed May 17 12:16:45 2023, max compression
```

## Comparing `hcai-datasets-0.1.6.tar` & `hcai-datasets-0.1.7.tar`

### file list

```diff
@@ -1,78 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.830348 hcai-datasets-0.1.6/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/dataset_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.830348 hcai-datasets-0.1.6/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.834348 hcai-datasets-0.1.6/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.834348 hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17265 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7833 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    22278 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12657 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9901 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/nova_types.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/nova_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/ssi_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/ssi_data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3828 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/ssi_sample_list_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/ssi_stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:42:45.834348 hcai-datasets-0.1.6/hcai_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-03-17 12:42:45.000000 hcai-datasets-0.1.6/hcai_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-03-17 12:42:45.000000 hcai-datasets-0.1.6/hcai_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 12:42:45.000000 hcai-datasets-0.1.6/hcai_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-03-17 12:42:45.000000 hcai-datasets-0.1.6/hcai_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-17 12:42:45.000000 hcai-datasets-0.1.6/hcai_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-17 12:42:45.838348 hcai-datasets-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-03-17 12:42:36.000000 hcai-datasets-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.148142 hcai-datasets-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-05-17 12:16:45.148142 hcai-datasets-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.136142 hcai-datasets-0.1.7/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.136142 hcai-datasets-0.1.7/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.136142 hcai-datasets-0.1.7/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-17 12:16:31.000000 hcai-datasets-0.1.7/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.140142 hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.140142 hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.140142 hcai-datasets-0.1.7/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.144142 hcai-datasets-0.1.7/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.144142 hcai-datasets-0.1.7/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.144142 hcai-datasets-0.1.7/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.144142 hcai-datasets-0.1.7/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.144142 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22727 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25025 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.144142 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12645 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19550 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.148142 hcai-datasets-0.1.7/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:16:45.136142 hcai-datasets-0.1.7/hcai_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-05-17 12:16:45.000000 hcai-datasets-0.1.7/hcai_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-05-17 12:16:45.000000 hcai-datasets-0.1.7/hcai_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:16:45.000000 hcai-datasets-0.1.7/hcai_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-17 12:16:45.000000 hcai-datasets-0.1.7/hcai_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-17 12:16:45.000000 hcai-datasets-0.1.7/hcai_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 12:16:45.148142 hcai-datasets-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-17 12:16:32.000000 hcai-datasets-0.1.7/setup.py
```

### Comparing `hcai-datasets-0.1.6/PKG-INFO` & `hcai-datasets-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets
-Version: 0.1.6
+Version: 0.1.7
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-0.1.6/README.md` & `hcai-datasets-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-0.1.7/hcai_dataset_utils/bridge_pytorch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import Iterator
 
 from torch.utils.data.dataset import T_co, IterableDataset
 
-import tensorflow as tf
-
 from hcai_dataset_utils.dataset_iterable import DatasetIterable
 
 
 class BridgePyTorch(IterableDataset):
     """
     Takes a dataset iterable and pytorch transforms
     can be fed directly to a pytorch DataLoader
```

### Comparing `hcai-datasets-0.1.6/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-0.1.7/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_dataset_utils/import_validator.py` & `hcai-datasets-0.1.7/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-0.1.7/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_dataset_utils/statistics.py` & `hcai-datasets-0.1.7/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/__init__.py` & `hcai-datasets-0.1.7/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-0.1.7/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import pandas as pd
 
 from pathlib import Path
 
-from hcai_dataset_utils.dataset_iterable import DatasetIterable
+from nova_utils.interfaces.dataset_iterable import DatasetIterable
 
 import numpy as np
 
 
 class HcaiAffectnetIterable(DatasetIterable):
 
     IMAGE_FOLDER_COL = "image_folder"
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from hcai_dataset_utils.dataset_iterable import DatasetIterable
+from nova_utils.interfaces.dataset_iterable import DatasetIterable
 import numpy as np
 
 
 class HcaiCkplusIterable(DatasetIterable):
     LABELS = [
         "neutral",
         "anger",
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from hcai_dataset_utils.dataset_iterable import DatasetIterable
+from nova_utils.interfaces.dataset_iterable import DatasetIterable
 import numpy as np
 
 
 class HcaiFacesIterable(DatasetIterable):
 
     CLASSES_AGE = ["y", "o", "m"]
     CLASSES_GENDER = ["m", "f"]
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-import warnings
+import logging
+import sys
 
 import numpy as np
 import os
-import shutil
-import sys
+import copy
 
-import hcai_datasets.hcai_nova_dynamic.utils.nova_types as nt
+import nova_utils.db_utils.nova_types as nt
 import hcai_datasets.hcai_nova_dynamic.utils.nova_data_utils as ndu
 import hcai_datasets.hcai_nova_dynamic.utils.nova_anno_utils as nau
-from hcai_dataset_utils.dataset_iterable import DatasetIterable
+from nova_utils.interfaces.dataset_iterable import DatasetIterable
 
 from hcai_datasets.hcai_nova_dynamic.utils.nova_data_utils import (
     AudioData,
     VideoData,
     StreamData,
 )
-from hcai_datasets.hcai_nova_dynamic.utils.nova_anno_utils import (
-    DiscreteAnnotation,
-    ContinuousAnnotation,
-    FreeAnnotation,
-)
 
 from hcai_datasets.hcai_nova_dynamic.nova_db_handler import NovaDBHandler
-from hcai_datasets.hcai_nova_dynamic.utils.nova_utils import *
+from hcai_datasets.hcai_nova_dynamic.utils.nova_string_utils import *
 
 
 class HcaiNovaDynamicIterable(DatasetIterable):
     def __init__(
         self,
-        *,
+        *args,
         db_config_path=None,
         db_config_dict=None,
         dataset=None,
         nova_data_dir=None,
         sessions=None,
         annotator=None,
         schemes=None,
@@ -40,18 +35,19 @@
         data_streams=None,
         start=None,
         end=None,
         left_context="0s",
         right_context="0s",
         frame_size=None,
         stride=None,
+        add_rest_class=True,
         flatten_samples=False,
         supervised_keys=None,
-        add_rest_class=True,
         lazy_loading=False,
+        fake_missing_data=True,
         **kwargs,
     ):
         """
         Initialize the HcaiNovaDynamic dataset builder
         Args:
           nova_data_dir: the directory to look for data. same as the directory specified in the nova gui.
           frame_size: the framesize to look at. the matching annotation will be calculated as majority vote from all annotations that are overlapping with the timeframe.
@@ -67,42 +63,66 @@
           sessions: list of sessions that should be loaded. must match the session names in nova.
           annotator: the name of the annotator that labeld the session. must match annotator names in nova.
           schemes: list of the annotation schemes to fetch
           roles: list of roles for which the annotation should be loaded.
           data_streams: list datastreams for which the annotation should be loaded. must match stream names in nova.
           start: optional start time_ms. use if only a specific chunk of a session should be retreived.
           end: optional end time_ms. use if only a specifc chunk of a session should be retreived.
+          fake_missing_data: If set to true missing datastreams will provide zero data and missing annotations will be empty. If set to false a session will be skipped if an expected data stream or annotation are not found.
           **kwargs: arguments that will be passed through to the dataset builder
         """
+        super().__init__(*args, **kwargs)
         self.dataset = dataset
         self.nova_data_dir = nova_data_dir
         self.sessions = sessions
         self.roles = roles
         self.schemes = schemes
         self.data_streams = data_streams
         self.annotator = annotator
+
+        # Sliding window parameters for the main stream
+        self.left_context, self.left_context_unit = ndu.parse_time_str(left_context)
+        self.right_context, self.right_context_unit = ndu.parse_time_str(right_context)
+        self.frame_size, self.frame_size_unit = ndu.parse_time_str(frame_size)
+        if self.frame_size == 0:
+            print(
+                "WARNING: Frame size 0 is invalid. Returning whole session as sample."
+            )
+            self.frame_size = None
+        self.stride, self.stride_unit = ndu.parse_time_str(stride) if stride else self.frame_size, self.frame_size_unit
+
+        #TODO: Remove time dependent variables after refactoring
         self.left_context_ms = ndu.parse_time_string_to_ms(left_context)
         self.right_context_ms = ndu.parse_time_string_to_ms(right_context)
         self.frame_size_ms = (
             ndu.parse_time_string_to_ms(frame_size) if frame_size else None
         )
+
+        if self.frame_size_ms == 0:
+            print(
+                "WARNING: Frame size 0 is invalid. Returning whole session as sample."
+            )
+            self.frame_size_ms = None
+
         self.stride_ms = (
             ndu.parse_time_string_to_ms(stride) if stride else self.frame_size_ms
         )
+
         self.start_ms = ndu.parse_time_string_to_ms(start)
         if not self.start_ms:
             self.start_ms = 0
 
         self.end_ms = ndu.parse_time_string_to_ms(end)
         if not self.end_ms:
-            self.end_ms = float("inf")
+            self.end_ms = sys.maxsize #float("inf")
 
         self.flatten_samples = flatten_samples
         self.add_rest_class = add_rest_class
         self.lazy_loading = lazy_loading
+        self.fake_missing_data = fake_missing_data
         self.nova_db_handler = NovaDBHandler(db_config_path, db_config_dict)
 
         # Retrieving meta information from the database
         mongo_schemes = self.nova_db_handler.get_schemes(
             dataset=dataset, schemes=schemes
         )
         mongo_data = self.nova_db_handler.get_data_streams(
@@ -111,14 +131,16 @@
         self.annos, self.anno_schemes = self._populate_label_info_from_mongo_doc(
             mongo_schemes
         )
         self.data_info, self.data_schemes = self._populate_data_info_from_mongo_doc(
             mongo_data
         )
 
+        self.session_info = {s: {} for s in self.sessions}
+
         # setting supervised keys
         if supervised_keys and self.flatten_samples:
             if supervised_keys[0] not in self.data_streams:
                 # remove <role> of supervised keys
                 _, data_stream = split_role_key(supervised_keys[0])
                 if not data_stream in self.data_streams:
                     print(
@@ -142,14 +164,51 @@
                 else:
                     supervised_keys[1] = scheme
 
         self.supervised_keys = tuple(supervised_keys) if supervised_keys else None
 
         self._iterable = self._yield_sample()
 
+    def to_single_session_iterator(self, session_id=""):
+        """Returns a copy of the iterator for a single session. All data objects and annotation objects will be initialized."""
+        ds_iter_copy = copy.copy(self)
+        if session_id not in self.sessions:
+            print(
+                f"WARNING: Session {session_id} not found in iterator session list. Using first session instead: {ds_iter_copy.sessions[0]}"
+            )
+            session_id = ds_iter_copy.sessions[0]
+        elif not session_id:
+            session_id = ds_iter_copy.sessions[0]
+
+        ds_iter_copy._init_session(session_id)
+        return ds_iter_copy
+
+    def _init_session(self, session):
+        """Opens all annotations and data readers"""
+
+        if (
+            not self.session_info[session]
+            or not self.session_info[session]["is_active"]
+        ):
+
+            # Gather all data we need for this session
+            self._load_annotation_for_session(session, time_to_ms=True)
+            self._open_data_reader_for_session(session)
+
+            session_info = self.nova_db_handler.get_session_info(self.dataset, session)[
+                0
+            ]
+
+            # Depricate other sessions
+            for id, s in self.session_info.items():
+                s["is_active"] = False
+
+            session_info["is_active"] = True
+            self.session_info[session] = session_info
+
     def _populate_label_info_from_mongo_doc(self, mongo_schemes):
         """
         Setting self.annos
         Args:
           mongo_schemes:
 
         Returns:
@@ -167,15 +226,15 @@
                 scheme_valid = scheme["isValid"]
                 anno_schemes[label_id] = scheme_type
 
                 if scheme_type == nt.AnnoTypes.DISCRETE:
                     labels = scheme["labels"]
                     annos[label_id] = nau.DiscreteAnnotation(
                         role=role,
-                        add_rest_class=True,
+                        add_rest_class=self.add_rest_class,
                         scheme=scheme_name,
                         is_valid=scheme_valid,
                         labels=labels,
                     )
 
                 elif scheme_type == nt.AnnoTypes.CONTINUOUS:
                     min_val = scheme["min"]
@@ -231,180 +290,244 @@
                 sample_data_path = os.path.join(
                     self.nova_data_dir,
                     self.dataset,
                     self.sessions[0],
                     sample_stream_name,
                 )
                 dtype = nt.string_to_enum(nt.DataTypes, data_stream["type"])
+                #window_size = (self.left_context_ms + self.frame_size_ms + self.right_context_ms) / (1 / data_stream["sr"])
+                # TODO
+                try:
+                    if dtype == nt.DataTypes.VIDEO:
+                        data = VideoData(
+                            role=role,
+                            name=data_stream["name"],
+                            file_ext=data_stream["fileExt"],
+                            sr=data_stream["sr"],
+                            is_valid=data_stream["isValid"],
+                            sample_data_path=sample_data_path,
+                            lazy_loading=self.lazy_loading,
+                        )
+                    elif dtype == nt.DataTypes.AUDIO:
+                        data = AudioData(
+                            role=role,
+                            name=data_stream["name"],
+                            file_ext=data_stream["fileExt"],
+                            sr=data_stream["sr"],
+                            is_valid=data_stream["isValid"],
+                            sample_data_path=sample_data_path,
+                            lazy_loading=self.lazy_loading,
+                        )
+                    elif dtype == nt.DataTypes.FEATURE:
+                        data = StreamData(
+                            role=role,
+                            name=data_stream["name"],
+                            sr=data_stream["sr"],
+                            data_type=dtype,
+                            is_valid=data_stream["isValid"],
+                            sample_data_path=sample_data_path,
+                            lazy_loading=self.lazy_loading,
+                        )
+                    else:
+                        raise ValueError(
+                            "Invalid data type".format(data_stream["type"])
+                        )
 
-                if dtype == nt.DataTypes.VIDEO:
-                    data = VideoData(
-                        role=role,
-                        name=data_stream["name"],
-                        file_ext=data_stream["fileExt"],
-                        sr=data_stream["sr"],
-                        is_valid=data_stream["isValid"],
-                        sample_data_path=sample_data_path,
-                        lazy_loading=self.lazy_loading,
-                    )
-                elif dtype == nt.DataTypes.AUDIO:
-                    data = AudioData(
-                        role=role,
-                        name=data_stream["name"],
-                        file_ext=data_stream["fileExt"],
-                        sr=data_stream["sr"],
-                        is_valid=data_stream["isValid"],
-                        sample_data_path=sample_data_path,
-                        lazy_loading=self.lazy_loading,
-                    )
-                elif dtype == nt.DataTypes.FEATURE:
-                    data = StreamData(
-                        role=role,
-                        name=data_stream["name"],
-                        sr=data_stream["sr"],
-                        data_type=dtype,
-                        is_valid=data_stream["isValid"],
-                        sample_data_path=sample_data_path,
-                        lazy_loading=self.lazy_loading,
-                    )
-                else:
-                    raise ValueError("Invalid data type {}".format(data_stream["type"]))
+                except FileNotFoundError as fnf:
+                    if self.fake_missing_data:
+                        raise FileNotFoundError
+                    else:
+                        print(f"WARNING: Ignoring exception - {fnf}")
+                        continue
 
                 data_id = merge_role_key(role=role, key=data_stream["name"])
                 data_info[data_id] = data
                 data_schemes[data_id] = dtype
 
         return data_info, data_schemes
 
     def _load_annotation_for_session(self, session, time_to_ms=False):
         for label_id, anno in self.annos.items():
-            mongo_anno = self.nova_db_handler.get_annos(
-                self.dataset, anno.scheme, session, self.annotator, anno.role
-            )
-            anno.set_annotation_from_mongo_doc(mongo_anno, time_to_ms=time_to_ms)
+            try:
+                mongo_anno = self.nova_db_handler.get_annos(
+                    self.dataset, anno.scheme, session, self.annotator, anno.role
+                )
+            except FileNotFoundError as fnf:
+                mongo_anno = []
+                if self.fake_missing_data:
+                    print(f"WARNING: {fnf} - Providing dummy data")
+                else:
+                    raise fnf
+            finally:
+                anno.set_annotation_from_mongo_doc(mongo_anno, time_to_ms=time_to_ms)
 
     def _open_data_reader_for_session(self, session):
         for data_id, data in self.data_info.items():
-            data_path = os.path.join(
-                self.nova_data_dir, self.dataset, session, data_id + "." + data.file_ext
-            )
-            data.open_file_reader(data_path)
+            try:
+                data_path = os.path.join(
+                    self.nova_data_dir,
+                    self.dataset,
+                    session,
+                    data_id + "." + data.file_ext,
+                )
+                data.open_file_reader(data_path)
+            except FileNotFoundError as fnf:
+                if self.fake_missing_data:
+                    print(f"WARNING: {fnf} - Providing dummy data")
+                else:
+                    raise fnf
+
+    def _build_sample_dict(self, labels_for_frame, data_for_frame):
+        sample_dict = {}
+
+        garbage_detected = False
+        for label_id, label_value in labels_for_frame:
+            # check for nan
+            if (
+                    type(label_value) != list
+                    and type(label_value) != str
+                    and type(label_value) != np.ndarray
+            ):
+                try:
+                    if label_value != label_value:
+                        garbage_detected = True
+                except:
+                    breakpoint()
+            sample_dict.update({label_id: label_value})
+
+        # If at least one label is a garbage label we skip this iteration
+        if garbage_detected:
+            return sample_dict
+
+        for d in data_for_frame:
+            sample_dict.update(d)
+
+        # if self.flatten_samples:
+        #
+        #     # grouping labels and data according to roles
+        #     for role in self.roles:
+        #         # filter dictionary to contain values for role
+        #         sample_dict_for_role = dict(
+        #             filter(lambda elem: role in elem[0], sample_dict.items())
+        #         )
+        #
+        #         # remove role from dictionary keys
+        #         sample_dict_for_role = dict(
+        #             map(
+        #                 lambda elem: (elem[0].replace(role + ".", ""), elem[1]),
+        #                 sample_dict_for_role.items(),
+        #             )
+        #         )
+        #
+        #         sample_dict_for_role["frame"] = (
+        #             str(sample_counter) + "_" + key + "_" + role
+        #         )
+        #         # yield key + '_' + role, sample_dict_for_role
+        #         yield sample_dict_for_role
+        #         sample_counter += 1
+        #     c_pos_ms += _stride_ms
+        #
+        # else:
+        return sample_dict
 
     def _yield_sample(self):
         """Yields examples."""
 
         # Needed to sort the samples later and assure that the order is the same as in nova. Necessary for CML till the tfds can be returned in order.
         sample_counter = 1
 
         for session in self.sessions:
 
-            # Gather all data we need for this session
-            self._load_annotation_for_session(session, time_to_ms=True)
-            self._open_data_reader_for_session(session)
+            self._init_session(session)
 
-            session_info = self.nova_db_handler.get_session_info(self.dataset, session)[
-                0
-            ]
-            dur = session_info["duration"]
-
-            # If we are loading any datastreams we check if any datastream is shorter than the duration stored in the database suggests
-            if self.data_info:
-                dur = min(*[v.dur for k, v in self.data_info.items()], dur)
-
-            if not dur:
-                raise ValueError("Session {} has no duration.".format(session))
-
-            dur_ms = int(dur * 1000)
-
-            # If framesize is not specified we return the whole session as one junk
-            if self.frame_size_ms is None:
-                self.frame_size_ms = min(dur_ms, self.end_ms - self.start_ms)
-                self.stride_ms = self.frame_size_ms
-
-            # Starting position of the first frame in seconds
-            # c_pos_ms = self.left_context_ms + self.start_ms
-            c_pos_ms = max(self.left_context_ms, self.start_ms)
-
-            # Generate samples for this session
-            while c_pos_ms + self.stride_ms + self.right_context_ms <= min(
-                self.end_ms, dur_ms
-            ):
-                frame_start_ms = c_pos_ms - self.left_context_ms
-                frame_end_ms = c_pos_ms + self.frame_size_ms + self.right_context_ms
+            # Iterate through the session using frame based indices
+            if self.stride_unit == ndu.StrideUnit.FRAMES:
 
-                key = (
-                    session
-                    + "_"
-                    + str(frame_start_ms / 1000)
-                    + "_"
-                    + str(frame_end_ms / 1000)
-                )
-
-                labels_for_frame = [
-                    {k: v.get_label_for_frame(frame_start_ms, frame_end_ms)}
-                    for k, v in self.annos.items()
-                ]
-
-
-                data_for_frame = []
-
-                for k, v in self.data_info.items():
-                    sample = v.get_sample(frame_start_ms, frame_end_ms)
-                    if sample.shape[0] == 0:
-                        print(f"Sample{frame_start_ms}-{frame_end_ms} is empty")
-                        c_pos_ms += self.stride_ms
-                        continue
-                    data_for_frame.append({k: sample})
-
-                sample_dict = {}
-
-                garbage_detected = False
-                for l in labels_for_frame:
-                    if np.isnan(list(l.values())[0]):
-                        garbage_detected = True
-                    sample_dict.update(l)
-
-                # If at least one label is a garbage label we skip this iteration
-                if garbage_detected:
-                    c_pos_ms += self.stride_ms
-                    sample_counter += 1
-                    continue
-
-                for d in data_for_frame:
-                    sample_dict.update(d)
-
-                if self.flatten_samples:
-
-                    # grouping labels and data according to roles
-                    for role in self.roles:
-                        # filter dictionary to contain values for role
-                        sample_dict_for_role = dict(
-                            filter(lambda elem: role in elem[0], sample_dict.items())
-                        )
-
-                        # remove role from dictionary keys
-                        sample_dict_for_role = dict(
-                            map(
-                                lambda elem: (elem[0].replace(role + ".", ""), elem[1]),
-                                sample_dict_for_role.items(),
-                            )
-                        )
+                # Setting the main stream as a reference
+                main_stream_id = self.roles[0] + '.' + self.data_streams[0]
+                if main_stream_id not in self.data_info.keys():
+                    print(f'WARNING: Framewise iteration has been requested but main stream "{main_stream_id}" could not be found. Skipping session.')
+                    break
+                print(f'Stride unit has been specified as number of frames. Using "{main_stream_id}" with a sr of {self.data_info[main_stream_id].sr} as main stream.')
+                main_stream = self.data_info[main_stream_id]
+                _frame_size = self.frame_size
+                _stride = self.stride
+
+                # Starting position of the first frame in seconds
+                c_pos = max(self.left_context, self.start_ms)
+
+                # If framesize is not specified we return the whole session as one junk
+                if self.frame_size is None:
+                    _frame_size = main_stream.n_frames
+                    _stride =  main_stream.n_frames
+
+                for i in range(0,main_stream.n_frames, _stride):
+                    print('')
+
+            else:
+                session_info = self.session_info[session]
+                dur = session_info["duration"]
+                _frame_size_ms = self.frame_size_ms
+                _stride_ms = self.stride_ms
+
+                # If we are loading any datastreams we check if any datastream is shorter than the duration stored in the database suggests
+                if self.data_info:
+                    dur = min(*[v.dur for k, v in self.data_info.items()], dur)
+
+                if not dur:
+                    raise ValueError("Session {} has no duration.".format(session))
+
+                dur_ms = int(dur * 1000)
+
+                # If framesize is not specified we return the whole session as one junk
+                if self.frame_size_ms is None:
+                    _frame_size_ms = min(dur_ms, self.end_ms - self.start_ms)
+                    _stride_ms = _frame_size_ms
+
+                # Starting position of the first frame in seconds
+                # c_pos_ms = self.left_context_ms + self.start_ms
+                c_pos_ms = max(self.left_context_ms, self.start_ms)
+
+                # Generate samples for this session
+                while c_pos_ms + _stride_ms + self.right_context_ms <= min(
+                    self.end_ms, dur_ms
+                ):
+                    frame_start_ms = c_pos_ms - self.left_context_ms
+                    frame_end_ms = c_pos_ms + _frame_size_ms + self.right_context_ms
+
+                    key = (
+                        session
+                        + "_"
+                        + str(frame_start_ms / 1000)
+                        + "_"
+                        + str(frame_end_ms / 1000)
+                    )
 
-                        sample_dict_for_role["frame"] = (
-                            str(sample_counter) + "_" + key + "_" + role
-                        )
-                        # yield key + '_' + role, sample_dict_for_role
-                        yield sample_dict_for_role
+                    labels_for_frame = [
+                        (k, v.get_label_for_frame(frame_start_ms, frame_end_ms))
+                        for k, v in self.annos.items()
+                    ]
+                    data_for_frame = []
+
+                    for k, v in self.data_info.items():
+                        sample = v.get_sample(frame_start_ms, frame_end_ms)
+                        if sample.shape[0] == 0:
+                            print(f"Sample{frame_start_ms}-{frame_end_ms} is empty")
+                            c_pos_ms += _stride_ms
+                            continue
+                        data_for_frame.append({k: sample})
+
+                    sample_dict = self._build_sample_dict(labels_for_frame, data_for_frame)
+                    if not sample_dict:
+                        c_pos_ms += _stride_ms
                         sample_counter += 1
-                    c_pos_ms += self.stride_ms
+                        continue
 
-                else:
-                    sample_dict["frame"] = str(sample_counter) + "_" + key
                     yield sample_dict
-                    c_pos_ms += self.stride_ms
+                    c_pos_ms += _stride_ms
                     sample_counter += 1
 
             # closing file readers for this session
             for k, v in self.data_info.items():
                 v.close_file_reader()
 
     def __iter__(self):
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 import shutil
 import tensorflow_datasets as tfds
 import tensorflow as tf
 from tensorflow_datasets.core import split_builder as split_builder_lib
 
 from hcai_dataset_utils.bridge_tf import BridgeTensorflow
 from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import HcaiNovaDynamicIterable
-import hcai_datasets.hcai_nova_dynamic.utils.nova_types as nt
-import hcai_datasets.hcai_nova_dynamic.utils.nova_data_utils as ndu
-import hcai_datasets.hcai_nova_dynamic.utils.nova_anno_utils as nau
+import nova_utils.db_utils.nova_types as nt
 
-from hcai_datasets.hcai_nova_dynamic.utils.nova_utils import *
+from hcai_datasets.hcai_nova_dynamic.utils.nova_string_utils import *
 
 # TODO(hcai_audioset): Markdown description  that will appear on the catalog page.
 _DESCRIPTION = """
 The Nova Dynamic dataset can be used to retrieve the data and labels for a certain session or a certain part of a session of a nova dataset. 
 This is part of the Nova CML Python backend (https://github.com/hcmlab/nova)
 To specify which data to load use the following format:
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
+import errno
 import copy
 import warnings
-import configparser
+import enum
 
+from configparser import ConfigParser
 from typing import Union
 from datetime import datetime
 from pymongo import MongoClient
 from pymongo.results import InsertOneResult, UpdateResult
 
 
 class NovaDBHandler:
@@ -51,74 +53,83 @@
                 )
             )
 
         self.client = MongoClient(
             host=self.ip, port=self.port, username=self.user, password=self.password
         )
 
-    def print_config(self, cfg, cfg_path):
+    def print_config(self, cfg: ConfigParser, cfg_path: str) -> None:
+        """
+        Prints the provided configuration on the console
+        Args:
+            cfg (ConfigParser): The main configuration parser
+            cfg_path (str): The file to load the configuration from
+        """
         print("Loaded config from {}:".format(cfg_path))
         print("---------------------")
         for sec_name, sec_dict in cfg._sections.items():
             print(sec_name)
             for k, v in sec_dict.items():
                 if k == "password":
                     continue
                 else:
                     print("\t{} : {}".format(k, v))
         print("---------------------")
 
-    def read_config(self, cfg_path):
-        config = configparser.RawConfigParser()
+    def read_config(self, cfg_path: str) -> ConfigParser:
+        """
+        Reads a NovaServer configuration from a file
+        Args:
+            cfg_path (str): The file to load the configuration from
+
+        Returns:
+            ConfigParser: The parsed configuration
+
+        """
+        config = ConfigParser()
         config.read(cfg_path)
         self.print_config(config, cfg_path)
         return config
 
     # Reading from database
     def get_docs_by_prop(
-            self, vals: Union[list, str], property: str, database: str, collection: str
-    ) -> list:
+        self, vals: Union[list[str], str], property: str, database: str, collection: str
+    ) -> list[dict]:
         """
         Fetching a document from the mongo db collection in the respective database where the passed values are matching a specific property in the collection.
-
         Args:
-          vals: The specific value of a property in the document
-          property: The property to look for the passed values
-          database: The name of the database to search
-          collection: The name of the collection within the database to search
+            vals (Union[list[str], str]): Value(s) of a property in the document. Might be a single value or list of values.
+            property (str): Property to look for the passed values
+            database (str): Name of the database to search
+            collection (str): Name of the collection within the database to search
 
         Returns:
-          list: List of documents that match the specified criteria
-
+            list[dict]: List of documents that match the specified criteria
         """
         filter = []
 
         if not type(vals) == type(list()):
             vals = [vals]
 
         for n in vals:
             filter.append({property: n})
 
         filter = {"$or": filter}
         ret = list(self.client[database][collection].find(filter))
         return ret
 
-    def get_schemes(self, dataset, schemes):
+    def get_schemes(self, dataset: str, schemes: list) -> list[dict]:
         """
-        Fetches the scheme object that matches the specified criteria from the nova database and returns them as a python readable dictionary.
+        Retreives all schemes matchin the provided criteria
         Args:
-          ip:
-          port:
-          user:
-          password:
-          dataset:
-          scheme:
+            dataset (str): Name of the dataset. Must match the respective entry in the MongoDB
+            schemes (str): List of schemes for which the mongo database entries are fetched
 
         Returns:
-
+            list[dict]: List of schemes that match the specified criteria
         """
 
         if not schemes:
             print("WARNING: No Schemes have been requested. Returning empty list.")
             return []
 
         # if not dataset in self.datasets:
@@ -126,35 +137,37 @@
 
         mongo_schemes = []
         for scheme in schemes:
             mongo_scheme = self.get_docs_by_prop(
                 scheme, "name", dataset, self.SCHEME_COLLECTION
             )
             if not mongo_scheme:
-                print(f"WARNING: No scheme {scheme} found in database for dataset {dataset}")
+                print(
+                    f"WARNING: No scheme {scheme} found in database for dataset {dataset}"
+                )
             else:
                 mongo_schemes.append(mongo_scheme[0])
 
         if not mongo_schemes:
             raise ValueError(
                 "No entries for schemes {} found in database".format(schemes)
             )
 
         return mongo_schemes
 
-    def get_session_info(self, dataset, session):
+    def get_session_info(self, dataset: str, session: Union[list, str]) -> list[dict]:
         """
         Fetches the session object that matches the specified criteria from the nova database and returns them as a python readable dictionary.
 
         Args:
-          dataset:
-          session:
+          dataset (str): Name of the dataset. Must match the respective entry in the MongoDB
+          session (Union[list, str]): Session or list of sessions for which the mongo database entries are fetched
 
         Returns:
-
+          list[dict]: List of sessions that match the specified criteria
         """
         mongo_session = self.get_docs_by_prop(
             session, "name", dataset, self.SESSION_COLLECTION
         )
         return mongo_session
 
     def get_data_streams(self, dataset, data_streams):
@@ -185,21 +198,21 @@
 
         if not mongo_streams:
             raise ValueError("no entries for datastream {} found".format(data_streams))
 
         return mongo_streams
 
     def get_annotation_docs(
-            self,
-            mongo_schemes,
-            mongo_sessions,
-            mongo_annotators,
-            mongo_roles,
-            database,
-            collection,
+        self,
+        mongo_schemes,
+        mongo_sessions,
+        mongo_annotators,
+        mongo_roles,
+        database,
+        collection,
     ):
         """
         Fetches all annotationobjects that match the specified criteria from the nova database
         Args:
           mongo_schemes:
           mongo_sessions:
           mongo_annotators:
@@ -237,20 +250,20 @@
             ]
         }
 
         ret = list(self.client[database][collection].find(filter))
         return ret
 
     def get_annos(
-            self,
-            dataset: str,
-            scheme: str,
-            session: str,
-            annotator: str,
-            roles: Union[list, str],
+        self,
+        dataset: str,
+        scheme: str,
+        session: str,
+        annotator: str,
+        roles: Union[list, str],
     ) -> list:
         """
         Fetches all annotations that matches the specified criteria from the nova database and returns them as a list of python readable dictionaries.
         Args:
           dataset:
           scheme:
           session:
@@ -268,15 +281,17 @@
             return []
         mongo_annotators = self.get_docs_by_prop(
             annotator, "name", dataset, self.ANNOTATOR_COLLECTION
         )
         if not mongo_annotators:
             warnings.warn(f"Unknown annotator {annotator} found")
             return []
-        mongo_roles = self.get_docs_by_prop(roles, "name", dataset, self.ROLE_COLLECTION)
+        mongo_roles = self.get_docs_by_prop(
+            roles, "name", dataset, self.ROLE_COLLECTION
+        )
         if not mongo_roles:
             warnings.warn(f"Unknown role {roles} found")
             return []
         mongo_sessions = self.get_docs_by_prop(
             session, "name", dataset, self.SESSION_COLLECTION
         )
         if not mongo_sessions:
@@ -290,30 +305,31 @@
             mongo_roles,
             dataset,
             self.ANNOTATION_COLLECTION,
         )
 
         # getting the annotation data and the session name
         if not mongo_annos:
-            print(
-                f"No annotations found for \n\t-annotator: {annotator}\n\t-scheme: {scheme}\n\t-session: {session}\n\t-role: {roles}"
+            raise FileNotFoundError(
+                errno.ENOENT,
+                "No such annotation",
+                f"annotator: {annotator} - scheme: {scheme} - session: {session} - role: {roles}",
             )
-            return []
 
         else:
             # TODO: adapt for multiple roles, annotators etc.
             label = self.get_data_docs_by_prop(
                 mongo_annos[0]["data_id"], "_id", dataset
             )
             label = label["labels"]
 
         return label
 
     def insert_doc_by_prop(
-            self, doc: dict, database: str, collection: str
+        self, doc: dict, database: str, collection: str
     ) -> InsertOneResult:
         """
         Uploading a document to the database using the specificed parameters
         Args:
           docs: List of dictionaries with objects to upload to the database
           database: The name of the database to search
           collection: The name of the collection within the database to search
@@ -321,15 +337,15 @@
         Returns:
           str: ObjectID of the inserted objects or an empty list in case of failure
         """
         ret = self.client[database][collection].insert_one(doc)
         return ret
 
     def update_doc_by_prop(
-            self, doc: dict, database: str, collection: str
+        self, doc: dict, database: str, collection: str
     ) -> UpdateResult:
         """
         Uploading a document to the database using the specificed parameters
         Args:
           docs: List of dictionaries with objects to upload to the database
           database: The name of the database to search
           collection: The name of the collection within the database to search
@@ -339,46 +355,44 @@
         """
         ret = self.client[database][collection].update_one(
             {"_id": doc["_id"]}, {"$set": doc}
         )
         return ret
 
     def update_doc_by_id(
-            self, _id: str, doc: dict, database: str, collection: str
+        self, _id: str, doc: dict, database: str, collection: str
     ) -> UpdateResult:
         """
         Uploading a document to the database using the specificed parameters
         Args:
           _id: ID of doc, which has to be updated
           docs: List of dictionaries with objects to upload to the database
           database: The name of the database to search
           collection: The name of the collection within the database to search
 
         Returns:
           str: ObjectID of the inserted objects or an empty list in case of failure
         """
-        ret = self.client[database][collection].update_one(
-            {"_id": _id}, {"$set": doc}
-        )
+        ret = self.client[database][collection].update_one({"_id": _id}, {"$set": doc})
         return ret
 
     # TODO: Remove Restclass Labels in discrete Cases
     # TODO: Consider "forced overwrite"
     # TODO: Add Backup case
     # TODO: Call preprocess of annotation
     def set_annos(
-            self,
-            database: str,
-            scheme: str,
-            session: str,
-            annotator: str,
-            role: str,
-            annos: list,
-            is_finished: bool = False,
-            is_locked: bool = False,
+        self,
+        database: str,
+        scheme: str,
+        session: str,
+        annotator: str,
+        role: str,
+        annos: list,
+        is_finished: bool = False,
+        is_locked: bool = False,
     ) -> str:
         """
         Uploading annotations to the database
         Args:
           database:
           scheme:
           session:
@@ -404,44 +418,52 @@
         )
 
         # Check for existing annotations
         mongo_anno_id = None
         mongo_data_id = None
         if mongo_annos:
             if mongo_annos[0]["isLocked"]:
-                warnings.warn(f"Can't overwrite locked annotation {str(mongo_annos[0]['_id'])}")
+                warnings.warn(
+                    f"Can't overwrite locked annotation {str(mongo_annos[0]['_id'])}"
+                )
                 return ""
             else:
-                warnings.warn(f"Overwriting existing annotation {str(mongo_annos[0]['_id'])}")
+                warnings.warn(
+                    f"Overwriting existing annotation {str(mongo_annos[0]['_id'])}"
+                )
                 mongo_anno_id = mongo_annos[0]["_id"]
                 mongo_data_id = mongo_annos[0]["data_id"]
 
         # Upload label data
         mongo_label_doc = {"labels": annos}
         if mongo_data_id:
             mongo_label_doc["_id"] = mongo_data_id
             success = self.update_doc_by_prop(
                 doc=mongo_label_doc,
                 database=database,
                 collection=self.ANNOTATION_DATA_COLLECTION,
             )
             if not success.acknowledged:
-                warnings.warn(f"Unknown error update database entries for Annotation data {mongo_data_id}")
+                warnings.warn(
+                    f"Unknown error update database entries for Annotation data {mongo_data_id}"
+                )
                 return ""
             else:
                 data_id = mongo_data_id
         else:
             success = self.insert_doc_by_prop(
                 doc=mongo_label_doc,
                 database=database,
                 collection=self.ANNOTATION_DATA_COLLECTION,
             )
             if not success.acknowledged:
-                warnings.warn(f"Unexpected error uploading annotation data for {database} - {session} - {scheme} - "
-                              f"{annotator}. Upload failed.")
+                warnings.warn(
+                    f"Unexpected error uploading annotation data for {database} - {session} - {scheme} - "
+                    f"{annotator}. Upload failed."
+                )
                 return ""
             else:
                 data_id = success.inserted_id
 
         # Upload annotation information
         mongo_anno_doc = {
             "data_id": data_id,
@@ -453,46 +475,104 @@
             "isLocked": is_locked,
             "date": datetime.today().replace(microsecond=0),
         }
 
         if mongo_anno_id:
             mongo_anno_doc["_id"] = mongo_anno_id
             success = self.update_doc_by_prop(
-                doc=mongo_anno_doc, database=database, collection=self.ANNOTATION_COLLECTION
+                doc=mongo_anno_doc,
+                database=database,
+                collection=self.ANNOTATION_COLLECTION,
             )
             if not success.acknowledged:
                 warnings.warn(
                     f"Unexpected error uploading annotations for {database} - {session} - {scheme} - {annotator}. Upload failed."
                 )
                 return ""
             else:
                 anno_id = mongo_anno_id
         else:
             success = self.insert_doc_by_prop(
-                doc=mongo_anno_doc, database=database, collection=self.ANNOTATION_COLLECTION
+                doc=mongo_anno_doc,
+                database=database,
+                collection=self.ANNOTATION_COLLECTION,
             )
             if not success.acknowledged:
                 warnings.warn(
                     f"Unexpected error uploading annotations for {database} - {session} - {scheme} - {annotator}. Upload failed."
                 )
                 return ""
             else:
                 anno_id = success.inserted_id
         return anno_id
 
+    def set_data_streams(
+        self,
+        database: str,
+        file_name: str,
+        file_ext: str,
+        stream_type: str,
+        is_valid: bool,
+        sr: float,
+        dimlabels: list,
+        overwrite: bool = False
+    ):
+
+        # check if datastream already exists
+        if not overwrite:
+            mongo_stream = self.get_docs_by_prop(
+                file_name, "name", database, self.STREAM_COLLECTION
+            )
+            if mongo_stream:
+                print(
+                    f"INFO: Stream {file_name} already exists in database. Skip adding stream."
+                )
+                return
+
+        # build doc
+        mongo_steam_doc = {
+            "name": file_name,
+            "fileExt": file_ext,
+            "type": stream_type,
+            "isValid": is_valid,
+            "sr": sr,
+            "dimlabels": dimlabels,
+        }
+
+        # insert datastream
+        success = self.insert_doc_by_prop(
+            doc=mongo_steam_doc,
+            database=database,
+            collection=self.STREAM_COLLECTION,
+        )
+
+        if not success.acknowledged:
+            warnings.warn(
+                f"Unexpected error adding stream for {database} - {file_name}.{file_ext}. Upload failed."
+            )
+            return ""
+        else:
+            stream_id = success.inserted_id
+
+        return stream_id
+
     def get_mongo_scheme(self, scheme, database):
-        mongo_scheme = self.get_docs_by_prop(scheme, "name", database, self.SCHEME_COLLECTION)
+        mongo_scheme = self.get_docs_by_prop(
+            scheme, "name", database, self.SCHEME_COLLECTION
+        )
         if not mongo_scheme:
             warnings.warn(f"Unknown scheme {scheme} found")
             return ""
 
         return mongo_scheme
 
     def get_mongo_annotator(self, annotator, database):
-        mongo_annotator = self.get_docs_by_prop(annotator, "name", database, self.ANNOTATOR_COLLECTION)
+        mongo_annotator = self.get_docs_by_prop(
+            annotator, "name", database, self.ANNOTATOR_COLLECTION
+        )
         if not mongo_annotator:
             warnings.warn(f"Unknown annotator {annotator} found")
             return ""
 
         return mongo_annotator
 
     def get_mongo_role(self, role, database):
@@ -500,65 +580,86 @@
         if not mongo_role:
             warnings.warn(f"Unknown role {role} found")
             return ""
 
         return mongo_role
 
     def get_mongo_session(self, session, database):
-        mongo_session = self.get_docs_by_prop(session, "name", database, self.SESSION_COLLECTION)
+        mongo_session = self.get_docs_by_prop(
+            session, "name", database, self.SESSION_COLLECTION
+        )
         if not mongo_session:
             warnings.warn(f"Unknown for session {session} found")
             return ""
 
         return mongo_session
 
     def delete_doc_with_tail(self, doc_id_to_remove, database):
         while doc_id_to_remove is not None:
             remove_id = copy.deepcopy(doc_id_to_remove)
-            result = self.get_fields_by_properties(doc_id_to_remove, "_id", "nextEntry", database,
-                                                   self.ANNOTATION_DATA_COLLECTION)
-            if result is not None and 'nextEntry' in result:
-                doc_id_to_remove = result['nextEntry']
+            result = self.get_fields_by_properties(
+                doc_id_to_remove,
+                "_id",
+                "nextEntry",
+                database,
+                self.ANNOTATION_DATA_COLLECTION,
+            )
+            if result is not None and "nextEntry" in result:
+                doc_id_to_remove = result["nextEntry"]
             else:
                 doc_id_to_remove = None
 
-            self.delete_doc_by_prop(remove_id, "_id", database, self.ANNOTATION_DATA_COLLECTION)
+            self.delete_doc_by_prop(
+                remove_id, "_id", database, self.ANNOTATION_DATA_COLLECTION
+            )
 
-    def delete_doc_by_prop(self, vals: Union[list, str], property: str, database: str, collection):
+    def delete_doc_by_prop(
+        self, vals: Union[list, str], property: str, database: str, collection
+    ):
         filter = []
 
         if not isinstance(vals, list):
             vals = [vals]
 
         for n in vals:
             filter.append({property: n})
 
         filter = {"$and": filter}
 
         return self.client[database][collection].delete_one(filter)
 
-    def get_data_docs_by_prop(self, vals: Union[list, str], property: str, database: str):
+    def get_data_docs_by_prop(
+        self, vals: Union[list, str], property: str, database: str
+    ):
         filter = []
 
         if not isinstance(vals, list):
             vals = [vals]
 
         for n in vals:
             filter.append({property: n})
 
         filter = {"$or": filter}
 
-        result = list(self.client[database][self.ANNOTATION_DATA_COLLECTION].find(filter))[0]
+        result = list(
+            self.client[database][self.ANNOTATION_DATA_COLLECTION].find(filter)
+        )[0]
         if "nextEntry" in result:
             return self.merge_collections(result, database)
 
         return result
 
-    def get_fields_by_properties(self, vals: Union[list, str], property, fields: Union[list, str], database: str,
-                                 collection: str):
+    def get_fields_by_properties(
+        self,
+        vals: Union[list, str],
+        property,
+        fields: Union[list, str],
+        database: str,
+        collection: str,
+    ):
         filter = []
         fields_dict = {}
 
         if not isinstance(fields, list):
             fields = [fields]
 
         for n in fields:
@@ -573,15 +674,15 @@
         filter = {"$or": filter}
 
         return self.client[database][collection].find_one(filter, fields_dict)
 
     def merge_collections(self, doc, database):
         next_id = doc["nextEntry"]
         new_doc = self.get_data_docs_by_prop(next_id, "_id", database)
-        doc['labels'] += new_doc['labels']
+        doc["labels"] += new_doc["labels"]
 
         return doc
 
 
 if __name__ == "__main__":
     db_handler = NovaDBHandler("../../local/nova_db_test.cfg")
 
@@ -654,17 +755,17 @@
             session=session,
             annotator=annotator,
             roles=roles,
         )
 
         new_annotator = "schildom"
         new_annos = [
-            {"from": 0, "to": 10, "conf": 1, "name": 'das'},
-            {"from": 20, "to": 25, "conf": 1, "name": 'geht'},
-            {"from": 30, "to": 35, "conf": 1, "name": 'ja'},
+            {"from": 0, "to": 10, "conf": 1, "name": "das"},
+            {"from": 20, "to": 25, "conf": 1, "name": "geht"},
+            {"from": 30, "to": 35, "conf": 1, "name": "ja"},
         ]
 
         db_handler.set_annos(
             dataset=dataset,
             scheme=scheme,
             session=session,
             annotator=new_annotator,
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-0.1.7/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import hcai_datasets.hcai_nova_dynamic.utils.nova_types as nt
 import numpy as np
 import pandas as pd
 from numba import njit
 from abc import ABC, abstractmethod
-from hcai_datasets.hcai_nova_dynamic.utils.nova_utils import merge_role_key
+from hcai_datasets.hcai_nova_dynamic.utils.nova_string_utils import merge_role_key
+from nova_utils.db_utils import nova_types as nt
 
 # TODO: Currently we do not take the rest class into account when calculating the label for the frame. Maybe we should do this
 @njit
 def _get_overlap(a, start, end):
     """
     Calculating all overlapping intervals between the given array of time intervals and the interval [start, end]
     Args:
@@ -144,15 +144,15 @@
         # Create
         if self.dataframe.empty:
             self.data_interval = np.empty((0, 2), int)
             self.data_values = np.empty((0, 2), int)
         else:
             # Creating numpy array of annotations for fast access
             # Splitting the annotations into interval and data array
-            self.data_interval = self.dataframe[["from", "to"]].values.astype(np.int)
+            self.data_interval = self.dataframe[["from", "to"]].values.astype(int)
             self.data_values = self.dataframe[["id", "conf"]].values
 
     def get_label_for_frame_legacy(self, start, end):
 
         # If we don't have any data we return the garbage label
         if self.data == -1:
             return -1
@@ -247,15 +247,15 @@
         # Create
         if self.dataframe.empty:
             self.data_interval = np.empty((0, 2), int)
             self.data_values = np.empty((0, 2), int)
         else:
             # Creating numpy array of annotations for fast access
             # Splitting the annotations into interval and data array
-            self.data_interval = self.dataframe[["from", "to"]].values.astype(np.int)
+            self.data_interval = self.dataframe[["from", "to"]].values.astype(int)
             self.data_values = self.dataframe[["name", "conf"]].values
 
     def get_label_for_frame_legacy(self, start, end):
 
         # If we don't have any data we return the garbage label
         if self.data == -1:
             return -1
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-0.1.7/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-0.1.7/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.6/hcai_datasets.egg-info/PKG-INFO` & `hcai-datasets-0.1.7/hcai_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets
-Version: 0.1.6
+Version: 0.1.7
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-0.1.6/hcai_datasets.egg-info/SOURCES.txt` & `hcai-datasets-0.1.7/hcai_datasets.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 pyproject.toml
 setup.py
 hcai_dataset_utils/__init__.py
 hcai_dataset_utils/bridge_pytorch.py
 hcai_dataset_utils/bridge_tf.py
 hcai_dataset_utils/dataset_indexed.py
-hcai_dataset_utils/dataset_iterable.py
 hcai_dataset_utils/import_validator.py
 hcai_dataset_utils/pytorch_dataset_wrapper.py
 hcai_dataset_utils/statistics.py
 hcai_datasets/__init__.py
 hcai_datasets.egg-info/PKG-INFO
 hcai_datasets.egg-info/SOURCES.txt
 hcai_datasets.egg-info/dependency_links.txt
@@ -46,16 +45,11 @@
 hcai_datasets/hcai_nova_dynamic/__init__.py
 hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
 hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
 hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
 hcai_datasets/hcai_nova_dynamic/utils/__init__.py
 hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
 hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
-hcai_datasets/hcai_nova_dynamic/utils/nova_types.py
-hcai_datasets/hcai_nova_dynamic/utils/nova_utils.py
-hcai_datasets/hcai_nova_dynamic/utils/ssi_anno_utils.py
-hcai_datasets/hcai_nova_dynamic/utils/ssi_data_types.py
-hcai_datasets/hcai_nova_dynamic/utils/ssi_sample_list_utils.py
-hcai_datasets/hcai_nova_dynamic/utils/ssi_stream_utils.py
+hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
 hcai_datasets/tests/__init__.py
 hcai_datasets/tests/dummy_set.py
 hcai_datasets/tests/test_bridge_pytorch.py
```

### Comparing `hcai-datasets-0.1.6/setup.py` & `hcai-datasets-0.1.7/setup.py`

 * *Files identical despite different names*

