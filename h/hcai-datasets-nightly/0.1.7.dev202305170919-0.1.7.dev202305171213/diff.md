# Comparing `tmp/hcai-datasets-nightly-0.1.7.dev202305170919.tar.gz` & `tmp/hcai-datasets-nightly-0.1.7.dev202305171213.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202305170919.tar", last modified: Wed May 17 09:19:08 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202305171213.tar", last modified: Wed May 17 12:13:48 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.7.dev202305170919.tar` & `hcai-datasets-nightly-0.1.7.dev202305171213.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.384163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.384163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22727 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    24935 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12645 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18990 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.232938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.232938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.232938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-17 12:13:35.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.236938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.236938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.236938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.236938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.236938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.236938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22727 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25025 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12645 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19550 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-17 12:13:48.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-05-17 12:13:48.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:13:48.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-17 12:13:48.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-17 12:13:48.000000 hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 12:13:48.240938 hcai-datasets-nightly-0.1.7.dev202305171213/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-17 12:13:36.000000 hcai-datasets-nightly-0.1.7.dev202305171213/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202305171213/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202305170919
+Version: 0.1.7.dev202305171213
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/README.md` & `hcai-datasets-nightly-0.1.7.dev202305171213/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,25 +510,27 @@
         database: str,
         file_name: str,
         file_ext: str,
         stream_type: str,
         is_valid: bool,
         sr: float,
         dimlabels: list,
+        overwrite: bool = False
     ):
 
         # check if datastream already exists
-        mongo_stream = self.get_docs_by_prop(
-            file_name, "name", database, self.STREAM_COLLECTION
-        )
-        if mongo_stream:
-            print(
-                f"INFO: Stream {file_name} already exists in database. Skip adding stream."
+        if not overwrite:
+            mongo_stream = self.get_docs_by_prop(
+                file_name, "name", database, self.STREAM_COLLECTION
             )
-            return
+            if mongo_stream:
+                print(
+                    f"INFO: Stream {file_name} already exists in database. Skip adding stream."
+                )
+                return
 
         # build doc
         mongo_steam_doc = {
             "name": file_name,
             "fileExt": file_ext,
             "type": stream_type,
             "isValid": is_valid,
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     def __init__(
         self,
         role: str = "",
         name: str = "",
         file_ext: str = "stream",
         sr: int = 0,
         data_type: nt.DataTypes = None,
+        np_data_type: np.dtype = np.float,
         is_valid: bool = True,
         sample_data_path: str = "",
         sample_data_shape: tuple = None,
         lazy_loading: bool = False,
     ):
         """
         Abstract base class for all data types
@@ -51,18 +52,18 @@
         self.role = role
         self.name = name
         self.is_valid = is_valid
         self.sr = sr
         self.file_ext = file_ext
         self.lazy_loading = lazy_loading
         self.data_type = data_type
+        self.np_data_type = np_data_type
 
         # Set when populate_meta_info is called
         self.sample_data_shape = sample_data_shape
-        self.np_data_type = None
         self.meta_loaded = False
         # self.n_frames_per_window = n_samples_per_window
 
         # Set when open_file_reader is called
         self.file_path = None
         self.file_reader = None
         self.dur = sys.maxsize
@@ -112,15 +113,15 @@
         Returns the sample for the respective frames. If lazy loading is true, only the filepath and frame_start, frame_end will be returned.
         """
 
         if not self.file_reader:
             start_frame, end_frame = sample_window_from_time_interval(
                 window_start, window_end, self.sr
             )
-            return np.zeros((end_frame - start_frame,), self.sample_data_shape)
+            return np.zeros((end_frame - start_frame,) + self.sample_data_shape).astype(self.np_data_type)
         elif self.lazy_loading:
             return {
                 "frame_start": window_start,
                 "frame_end": window_end,
                 "file_path": self.file_path,
             }
         else:
@@ -190,14 +191,18 @@
 
         Args:
             **kwargs ():
         """
         # Overwrite default
         if kwargs.get("sample_data_shape") is None:
             self.sample_data_shape = (1,)
+        if kwargs.get("np_data_type") is None:
+            kwargs.update({"np_data_type": np.float32})
+        kwargs.update({"data_type": nt.DataTypes.AUDIO})
+
         super().__init__(**kwargs)
 
     def _get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
             "dtype": np.float32,
         }
@@ -249,14 +254,18 @@
         Args:
             **kwargs ():
         """
         # Overwrite default
         if kwargs.get("sample_data_shape") is None:
             sample_data_shape = (480, 640, 3)
             kwargs.update({"sample_data_shape": sample_data_shape})
+        if kwargs.get("np_data_type") is None:
+            kwargs.update({"np_data_type": np.uint8})
+        kwargs.update({"data_type": nt.DataTypes.VIDEO})
+
         super().__init__(**kwargs)
 
     def _get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
             "dtype": np.float32,
         }
@@ -303,14 +312,17 @@
         Args:
             **kwargs ():
         """
         # Overwrite default
         if kwargs.get("sample_data_shape") is None:
             sample_data_shape = (1,)
             kwargs.update({"sample_data_shape": sample_data_shape})
+        if kwargs.get("np_data_type") is None:
+            kwargs.update({"np_data_type": np.float32})
+        kwargs.update({"data_type": nt.DataTypes.FEATURE})
 
         super().__init__(**kwargs)
 
     def _get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
             "dtype": self.np_data_type,
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202305170919
+Version: 0.1.7.dev202305171213
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.7.dev202305171213/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305170919/setup.py` & `hcai-datasets-nightly-0.1.7.dev202305171213/setup.py`

 * *Files identical despite different names*

