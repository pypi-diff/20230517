# Comparing `tmp/hcai-datasets-nightly-0.1.7.dev202305040643.tar.gz` & `tmp/hcai-datasets-nightly-0.1.7.dev202305170919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202305040643.tar", last modified: Thu May  4 06:43:54 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202305170919.tar", last modified: Wed May 17 09:19:08 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.7.dev202305040643.tar` & `hcai-datasets-nightly-0.1.7.dev202305170919.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.823663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.823663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.823663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.827663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20593 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    24935 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12645 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    13914 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-04 06:43:54.000000 hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 06:43:54.831663 hcai-datasets-nightly-0.1.7.dev202305040643/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-04 06:43:39.000000 hcai-datasets-nightly-0.1.7.dev202305040643/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.384163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.384163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.388163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22727 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24935 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12645 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18990 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-17 09:19:08.000000 hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 09:19:08.392163 hcai-datasets-nightly-0.1.7.dev202305170919/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-17 09:18:57.000000 hcai-datasets-nightly-0.1.7.dev202305170919/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202305170919/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202305040643
+Version: 0.1.7.dev202305170919
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/README.md` & `hcai-datasets-nightly-0.1.7.dev202305170919/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

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

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

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

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

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

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import sys
 
 import numpy as np
 import os
 import copy
 
 import nova_utils.db_utils.nova_types as nt
 import hcai_datasets.hcai_nova_dynamic.utils.nova_data_utils as ndu
@@ -73,14 +74,27 @@
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
 
         if self.frame_size_ms == 0:
@@ -95,15 +109,15 @@
 
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
         self.fake_missing_data = fake_missing_data
         self.nova_db_handler = NovaDBHandler(db_config_path, db_config_dict)
 
@@ -276,15 +290,15 @@
                 sample_data_path = os.path.join(
                     self.nova_data_dir,
                     self.dataset,
                     self.sessions[0],
                     sample_stream_name,
                 )
                 dtype = nt.string_to_enum(nt.DataTypes, data_stream["type"])
-                window_size = (self.left_context_ms + self.frame_size_ms + self.right_context_ms) / (1 / data_stream["sr"])
+                #window_size = (self.left_context_ms + self.frame_size_ms + self.right_context_ms) / (1 / data_stream["sr"])
                 # TODO
                 try:
                     if dtype == nt.DataTypes.VIDEO:
                         data = VideoData(
                             role=role,
                             name=data_stream["name"],
                             file_ext=data_stream["fileExt"],
@@ -358,130 +372,160 @@
                 data.open_file_reader(data_path)
             except FileNotFoundError as fnf:
                 if self.fake_missing_data:
                     print(f"WARNING: {fnf} - Providing dummy data")
                 else:
                     raise fnf
 
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
+
     def _yield_sample(self):
         """Yields examples."""
 
         # Needed to sort the samples later and assure that the order is the same as in nova. Necessary for CML till the tfds can be returned in order.
         sample_counter = 1
 
         for session in self.sessions:
 
             self._init_session(session)
 
-            session_info = self.session_info[session]
-            dur = session_info["duration"]
-            _frame_size_ms = self.frame_size_ms
-            _stride_ms = self.stride_ms
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
-                _frame_size_ms = min(dur_ms, self.end_ms - self.start_ms)
-                _stride_ms = _frame_size_ms
-
-            # Starting position of the first frame in seconds
-            # c_pos_ms = self.left_context_ms + self.start_ms
-            c_pos_ms = max(self.left_context_ms, self.start_ms)
-
-            # Generate samples for this session
-            while c_pos_ms + _stride_ms + self.right_context_ms <= min(
-                self.end_ms, dur_ms
-            ):
-                frame_start_ms = c_pos_ms - self.left_context_ms
-                frame_end_ms = c_pos_ms + _frame_size_ms + self.right_context_ms
-
-                key = (
-                    session
-                    + "_"
-                    + str(frame_start_ms / 1000)
-                    + "_"
-                    + str(frame_end_ms / 1000)
-                )
-
-                labels_for_frame = [
-                    (k, v.get_label_for_frame(frame_start_ms, frame_end_ms))
-                    for k, v in self.annos.items()
-                ]
-
-                data_for_frame = []
-
-                for k, v in self.data_info.items():
-                    sample = v.get_sample(frame_start_ms, frame_end_ms)
-                    if sample.shape[0] == 0:
-                        print(f"Sample{frame_start_ms}-{frame_end_ms} is empty")
-                        c_pos_ms += _stride_ms
-                        continue
-                    data_for_frame.append({k: sample})
-
-                sample_dict = {}
-
-                garbage_detected = False
-                for label_id, label_value in labels_for_frame:
-                    # check for nan
-                    if (
-                        type(label_value) != list
-                        and type(label_value) != str
-                        and type(label_value) != np.ndarray
-                    ):
-                        try:
-                            if label_value != label_value:
-                                garbage_detected = True
-                        except:
-                            breakpoint()
-                    sample_dict.update({label_id: label_value})
-
-                # If at least one label is a garbage label we skip this iteration
-                if garbage_detected:
-                    c_pos_ms += _stride_ms
-                    sample_counter += 1
-                    continue
-
-                for d in data_for_frame:
-                    sample_dict.update(d)
+            # Iterate through the session using frame based indices
+            if self.stride_unit == ndu.StrideUnit.FRAMES:
 
-                if self.flatten_samples:
-
-                    # grouping labels and data according to roles
-                    for role in self.roles:
-                        # filter dictionary to contain values for role
-                        sample_dict_for_role = dict(
-                            filter(lambda elem: role in elem[0], sample_dict.items())
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
 
-                        # remove role from dictionary keys
-                        sample_dict_for_role = dict(
-                            map(
-                                lambda elem: (elem[0].replace(role + ".", ""), elem[1]),
-                                sample_dict_for_role.items(),
-                            )
-                        )
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
 
-                        sample_dict_for_role["frame"] = (
-                            str(sample_counter) + "_" + key + "_" + role
-                        )
-                        # yield key + '_' + role, sample_dict_for_role
-                        yield sample_dict_for_role
+                    sample_dict = self._build_sample_dict(labels_for_frame, data_for_frame)
+                    if not sample_dict:
+                        c_pos_ms += _stride_ms
                         sample_counter += 1
-                    c_pos_ms += _stride_ms
+                        continue
 
-                else:
-                    sample_dict["frame"] = str(sample_counter) + "_" + key
                     yield sample_dict
                     c_pos_ms += _stride_ms
                     sample_counter += 1
 
             # closing file readers for this session
             for k, v in self.data_info.items():
                 v.close_file_reader()
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,50 +9,59 @@
 from nova_utils.db_utils import nova_types as nt
 from nova_utils.ssi_utils.ssi_stream_utils import Stream
 from hcai_datasets.hcai_nova_dynamic.utils.nova_string_utils import (
     merge_role_key,
 )
 from typing import Union
 from abc import ABC, abstractmethod
+from enum import Enum
+
+
+class StrideUnit(Enum):
+    MILLISECONDS = (0,)
+    SECONDS = (1,)
+    FRAMES = 2
 
 
 class Data(ABC):
     def __init__(
         self,
         role: str = "",
         name: str = "",
         file_ext: str = "stream",
         sr: int = 0,
         data_type: nt.DataTypes = None,
         is_valid: bool = True,
         sample_data_path: str = "",
+        sample_data_shape: tuple = None,
         lazy_loading: bool = False,
     ):
         """
         Abstract base class for all data types
         Args:
             role (str): Role to which the datastream belongs
             name (str): Filename of the datastream without the role
             file_ext (str): File extension of the datastream
             sr (int): Samplerate of the datastream
             data_type (DataTypes): Type of the datastream as specified in the nova_utils package under db_utils.nova_types.novDataTypes
             is_valid (bool): Whether the datastream is valid or not
             sample_data_path (str): A path to an example data file from which all meta information that is not saved in the Nova database can be read
+            sample_data_shape (tuple): The default shape of one data sample. Will be overwritten by populate_meta_info if a valid datastream can be found.
             lazy_loading (bool): If set to true only the respective timestamps and filenames will be returned for each window. Not the actual data.
         """
         self.role = role
         self.name = name
         self.is_valid = is_valid
         self.sr = sr
         self.file_ext = file_ext
         self.lazy_loading = lazy_loading
         self.data_type = data_type
 
         # Set when populate_meta_info is called
-        self.sample_data_shape = None
+        self.sample_data_shape = sample_data_shape
         self.np_data_type = None
         self.meta_loaded = False
         # self.n_frames_per_window = n_samples_per_window
 
         # Set when open_file_reader is called
         self.file_path = None
         self.file_reader = None
@@ -89,31 +98,37 @@
         else:
             print(
                 "Meta data has not been loaded for file {}. Call get_meta_info() first.".format(
                     merge_role_key(self.role, self.name)
                 )
             )
 
-    def get_sample(self, frame_start_ms: int, frame_end_ms: int):
+    def get_sample(
+        self,
+        window_start: int,
+        window_end: int,
+        stride_unit: StrideUnit = StrideUnit.MILLISECONDS,
+    ):
         """
         Returns the sample for the respective frames. If lazy loading is true, only the filepath and frame_start, frame_end will be returned.
         """
 
         if not self.file_reader:
-            start_frame = milli_seconds_to_sample_nr(self.sr, frame_start_ms)
-            end_frame = milli_seconds_to_sample_nr(self.sr, frame_end_ms)
-            return np.zeros(self.sample_data_shape + (end_frame - start_frame,))
+            start_frame, end_frame = sample_window_from_time_interval(
+                window_start, window_end, self.sr
+            )
+            return np.zeros((end_frame - start_frame,), self.sample_data_shape)
         elif self.lazy_loading:
             return {
-                "frame_start": frame_start_ms,
-                "frame_end": frame_end_ms,
+                "frame_start": window_start,
+                "frame_end": window_end,
                 "file_path": self.file_path,
             }
         else:
-            return self._get_sample_hook(frame_start_ms, frame_end_ms)
+            return self._get_sample_hook(window_start, window_end, stride_unit)
 
     def open_file_reader(self, path: str):
         """
         Args:
             path ():
         Raises:
             FileNotFoundError: If path is not a file
@@ -129,17 +144,25 @@
     def _get_info_hook(self):
         """
         Returns the features for this datastream to create the DatasetInfo for tensorflow
         """
         ...
 
     @abstractmethod
-    def _get_sample_hook(self, window_start_ms: int, window_end_ms: int):
+    def _get_sample_hook(
+        self,
+        window_start: int,
+        window_end: int,
+        stride_unit: StrideUnit = StrideUnit.MILLISECONDS,
+    ):
         """
         Returns a data chunk from window start to window end. The window is automatically adjusted to always provide the same number of data samples.
+
+        Args:
+            stride_unit ():
         """
         ...
 
     @abstractmethod
     def _open_file_reader_hook(self, path: str):
         """
         Opens a filereader for the respective datastream. Sets attributes self.file_reader and self.dur
@@ -164,37 +187,48 @@
 class AudioData(Data):
     def __init__(self, **kwargs):
         """
 
         Args:
             **kwargs ():
         """
-        super().__init__(**kwargs)
-
         # Overwrite default
-        self.sample_data_shape = (1,)
+        if kwargs.get("sample_data_shape") is None:
+            self.sample_data_shape = (1,)
+        super().__init__(**kwargs)
 
     def _get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
             "dtype": np.float32,
         }
 
-    def _get_sample_hook(self, window_start_ms: int, window_end_ms: int):
-        windows_start_sample, window_end_sample = sample_window_from_interval(
-            window_start_ms, window_end_ms, self.sr
-        )
+    def _get_sample_hook(
+        self,
+        window_start: int,
+        window_end: int,
+        stride_unit: StrideUnit = StrideUnit.FRAMES,
+    ):
+
+        if stride_unit == StrideUnit.FRAMES:
+            window_start_sample = window_start
+            window_end_sample = window_end
+        else:
+            window_start_sample, window_end_sample = sample_window_from_time_interval(
+                window_start, window_end, self.sr
+            )
         chunk = self.file_reader.get_batch(
-            list(range(windows_start_sample, window_end_sample))
+            list(range(window_start_sample, window_end_sample))
         ).asnumpy()
         return chunk
 
     def _open_file_reader_hook(self, path: str):
         self.file_reader = AudioReader(path, ctx=cpu(0), mono=False)
         self.dur = self.file_reader.duration()
+        self.n_frames = len(self.file_reader)
 
     def populate_meta_info(self, path: str):
         """
 
         Args:
             path ():
         """
@@ -211,39 +245,51 @@
 class VideoData(Data):
     def __init__(self, **kwargs: object) -> object:
         """
 
         Args:
             **kwargs ():
         """
-        super().__init__(**kwargs)
-
         # Overwrite default
-        self.sample_data_shape = (480, 640, 3)
+        if kwargs.get("sample_data_shape") is None:
+            sample_data_shape = (480, 640, 3)
+            kwargs.update({"sample_data_shape": sample_data_shape})
+        super().__init__(**kwargs)
 
     def _get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
             "dtype": np.float32,
         }
 
-    def _get_sample_hook(self, window_start_ms: int, window_end_ms: int):
-        windows_start_sample, window_end_sample = sample_window_from_interval(
-            window_start_ms, window_end_ms, self.sr
-        )
+    def _get_sample_hook(
+        self,
+        window_start: int,
+        window_end: int,
+        stride_unit: StrideUnit = StrideUnit.FRAMES,
+    ):
+        if stride_unit == StrideUnit.FRAMES:
+            window_start_sample = window_start
+            window_end_sample = window_end
+        else:
+            window_start_sample, window_end_sample = sample_window_from_time_interval(
+                window_start, window_end, self.sr
+            )
+
         chunk = self.file_reader.get_batch(
-            list(range(windows_start_sample, window_end_sample))
+            list(range(window_start_sample, window_end_sample))
         ).asnumpy()
         return chunk
 
     def _open_file_reader_hook(self, path: str):
         self.file_reader = VideoReader(path, ctx=cpu(0))
         fps = self.file_reader.get_avg_fps()
         frame_count = len(self.file_reader)
         self.dur = frame_count / fps
+        self.n_frames = len(self.file_reader)
 
     def populate_meta_info(self, path: str):
         file_reader = VideoReader(path)
         self.sample_data_shape = file_reader[0].shape
         self.meta_loaded = True
 
     def close_file_reader(self):
@@ -253,44 +299,58 @@
 class StreamData(Data):
     def __init__(self, **kwargs: object) -> object:
         """
 
         Args:
             **kwargs ():
         """
-        super().__init__(**kwargs)
         # Overwrite default
-        self.sample_data_shape = (1,)
+        if kwargs.get("sample_data_shape") is None:
+            sample_data_shape = (1,)
+            kwargs.update({"sample_data_shape": sample_data_shape})
+
+        super().__init__(**kwargs)
 
     def _get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
             "dtype": self.np_data_type,
         }
 
-    def _get_sample_hook(self, window_start_ms: int, window_end_ms: int):
+    def _get_sample_hook(
+        self,
+        window_start: int,
+        window_end: int,
+        stride_unit: StrideUnit = StrideUnit.FRAMES,
+    ):
         try:
             self.data_stream_opend()
-            windows_start_sample, window_end_sample = sample_window_from_interval(
-                window_start_ms, window_end_ms, self.sr
-            )
+            if stride_unit == StrideUnit.FRAMES:
+                window_start_sample = window_start
+                window_end_sample = window_end
+            else:
+                (
+                    window_start_sample,
+                    window_end_sample,
+                ) = sample_window_from_time_interval(window_start, window_end, self.sr)
 
-            return self.file_reader.data[windows_start_sample:window_end_sample]
+            return self.file_reader.data[window_start_sample:window_end_sample]
         except RuntimeError:
             print(
                 "Could not get chunk {}-{} from data stream {}".format(
-                    window_start_ms, window_end_ms, merge_role_key(self.role, self.name)
+                    window_start, window_end, merge_role_key(self.role, self.name)
                 )
             )
 
     def _open_file_reader_hook(self, path: Path) -> bool:
         stream = Stream(path=path)
         if stream:
             self.file_reader = stream
-            self.dur = stream.data.shape[0] / stream.sr
+            self.n_frames = stream.data.shape[0]
+            self.dur = self.n_frames / stream.sr
             return True
         else:
             print("Could not open Stream {}".format(str))
             return False
 
     def close_file_reader(self):
         return True
@@ -336,15 +396,41 @@
     Returns:
         float: Unrounded index of the sample in the stream for a given time
 
     """
     return seconds_to_sample_nr(sr=sr, time_s=time_ms / 1000.0)
 
 
-def sample_window_from_interval(
+def sample_nr_to_seconds(sample_nr: float, sr: float) -> float:
+    """
+    Calculates the specific time in seconds in a data stream that corresponds to given sample number
+    Args:
+        sample_nr (float): The unrounded sample number. Might represent a value between to actual samples of the stream.
+        sr (float): The average numbers of samples per second.
+
+    Returns:
+        float: Unrounded time representation of sample_nr specified in seconds
+    """
+    return sample_nr * sr
+
+
+def sample_nr_to_milli_seconds(sample_nr: float, sr: float) -> float:
+    """
+    Calculates the specific time in milli in a data stream that corresponds to given sample number
+    Args:
+        sample_nr (float): The unrounded sample number. Might represent a value between to actual samples of the stream.
+        sr (float): The average numbers of samples per second.
+
+     Returns:
+         float: Unrounded time representation of sample_nr specified in milliseconds
+    """
+    return sample_nr_to_seconds(sample_nr, sr) * 1000.0
+
+
+def sample_window_from_time_interval(
     start_time_ms: int, end_time_ms: int, sr: float
 ) -> tuple[int, int]:
     """
     Calculates the start and end sample number of a sliding window.
     Args:
         start_time_ms (int): Start time of the window in milliseconds
         end_time_ms (int): End time of the window in milliseconds
@@ -364,16 +450,16 @@
     end_sample_nr = math.ceil(end_sample_nr)
 
     # Assert number of samples in window
     expected_number_of_samples = math.ceil(((end_time_ms - start_time_ms) / 1000) * sr)
     number_of_samples = end_sample_nr - start_sample_nr
     sample_diff = number_of_samples - expected_number_of_samples
 
-    # Fewer then expected samples: We pad with samples from the past
-    # More samples than expected: We cut samples from the beginning
+    # Fewer then expected samples: We move start_sample number to the left
+    # More samples than expected: We move start_sample number to the right
     start_sample_nr += sample_diff
 
     assert expected_number_of_samples == end_sample_nr - start_sample_nr
 
     return start_sample_nr, end_sample_nr
 
 
@@ -417,7 +503,70 @@
             return int(frame)
         except ValueError:
             raise ValueError("Invalid input format for frame: {}".format(frame))
 
     print(
         f'WARNING: Could  not automatically parse time "{frame}" to seconds. Returning None '
     )
+
+
+def parse_time_str(frame: Union[str, int, float]) -> (Union[int, float], StrideUnit):
+
+    if frame is None:
+        print(f"WARNING: No timestring to parse. Returning None ")
+        return None, StrideUnit.MILLISECONDS
+
+    # if frame is specified milliseconds
+    if str(frame).endswith("ms"):
+        try:
+            return int(frame[:-2]), StrideUnit.MILLISECONDS
+        except ValueError:
+            raise ValueError(
+                "Invalid input format for length specified in milliseconds: {}".format(
+                    frame
+                )
+            )
+
+    # if frame is specified in seconds
+    elif str(frame).endswith("s"):
+        try:
+            return float(frame[:-1]), StrideUnit.SECONDS
+        except ValueError:
+            raise ValueError(
+                "Invalid input format for length specified in seconds: {}".format(frame)
+            )
+
+    # if frame is specified in frames
+    elif str(frame).endswith("f"):
+        try:
+            return int(frame[:-1]), StrideUnit.FRAMES
+        except ValueError:
+            raise ValueError(
+                "Invalid input format for length specified in number of frames: {}".format(
+                    frame
+                )
+            )
+    # if type is float we assume the input will be seconds
+    elif isinstance(frame, float) or "." in str(frame):
+        try:
+            print(
+                "WARNING: Automatically inferred type for frame {} is float. Interpreting as seconds".format(
+                    frame
+                )
+            )
+            return float(frame), StrideUnit.SECONDS
+        except ValueError:
+            raise ValueError("Invalid input format for frame: {}".format(frame))
+    # if type is int we assume the input will be milliseconds
+    elif isinstance(frame, int) or (isinstance(frame, str) and frame.isdigit()):
+        try:
+            print(
+                "WARNING: Automatically inferred type for frame {} is int. Interpreting as milliseconds".format(
+                    frame
+                )
+            )
+            return int(frame), StrideUnit.MILLISECONDS
+        except ValueError:
+            raise ValueError("Invalid input format for frame: {}".format(frame))
+
+    print(f'WARNING: Could  not automatically parse time "{frame}". Returning None ')
+    return None, StrideUnit.MILLISECONDS
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202305040643
+Version: 0.1.7.dev202305170919
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.7.dev202305170919/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202305040643/setup.py` & `hcai-datasets-nightly-0.1.7.dev202305170919/setup.py`

 * *Files identical despite different names*

