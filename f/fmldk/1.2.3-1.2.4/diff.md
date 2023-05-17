# Comparing `tmp/fmldk-1.2.3.tar.gz` & `tmp/fmldk-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmldk-1.2.3.tar", last modified: Tue May  9 12:55:30 2023, max compression
+gzip compressed data, was "fmldk-1.2.4.tar", last modified: Wed May 17 16:49:43 2023, max compression
```

## Comparing `fmldk-1.2.3.tar` & `fmldk-1.2.4.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.846187 fmldk-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-09 12:55:30.846187 fmldk-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-05-09 12:55:13.000000 fmldk-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.826187 fmldk-1.2.3/ctfr/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfr/ctfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfr/ctfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfr/ctfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfr/ctfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfr/ctfr_models_v0.1.29.py
--rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfr/ctfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.830187 fmldk-1.2.3/ctfrv2/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2/ctfrv2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2/ctfrv2_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2/ctfrv2_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2/ctfrv2_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.830187 fmldk-1.2.3/ctfrv2_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2_gpu/ctfrv2_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2_gpu/ctfrv2_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    78757 2023-05-09 12:55:13.000000 fmldk-1.2.3/ctfrv2_gpu/ctfrv2_model_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.830187 fmldk-1.2.3/eda/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 12:55:13.000000 fmldk-1.2.3/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-05-09 12:55:13.000000 fmldk-1.2.3/eda/eda_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-09 12:55:13.000000 fmldk-1.2.3/eda/eda_lib_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-05-09 12:55:13.000000 fmldk-1.2.3/eda/eda_lib_v0.1.19.py
--rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-05-09 12:55:13.000000 fmldk-1.2.3/eda/eda_lib_v0.1.37.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.834187 fmldk-1.2.3/fmldk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-09 12:55:30.000000 fmldk-1.2.3/fmldk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-09 12:55:30.000000 fmldk-1.2.3/fmldk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:55:30.000000 fmldk-1.2.3/fmldk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 12:55:30.000000 fmldk-1.2.3/fmldk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 12:55:30.000000 fmldk-1.2.3/fmldk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.834187 fmldk-1.2.3/sage/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46655 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/sage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/sage_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/sage_global_scaled_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/sage_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/sage_losses_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/sage_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage/sage_model_old.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.834187 fmldk-1.2.3/sage_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36569 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage_gpu/sage_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage_gpu/sage_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    87795 2023-05-09 12:55:13.000000 fmldk-1.2.3/sage_gpu/sage_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:55:30.846187 fmldk-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-09 12:55:13.000000 fmldk-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.838188 fmldk-1.2.3/stctn/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 12:55:13.000000 fmldk-1.2.3/stctn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-05-09 12:55:13.000000 fmldk-1.2.3/stctn/stctn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-09 12:55:13.000000 fmldk-1.2.3/stctn/stctn_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-09 12:55:13.000000 fmldk-1.2.3/stctn/stctn_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-05-09 12:55:13.000000 fmldk-1.2.3/stctn/stctn_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.842188 fmldk-1.2.3/tfr/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data_v0.1.14.py
--rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data_v0.1.15.py
--rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data_v0.1.16.py
--rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_data_v0.1.21.py
--rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_local_block_sparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_local_block_sparse_attention_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_local_block_sparse_attention_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_models_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_models_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_models_v0.1.23.py
--rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-05-09 12:55:13.000000 fmldk-1.2.3/tfr/tfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.846187 fmldk-1.2.3/tft/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46653 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_data_v1.1.3.py
--rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_data_v1.1.7.py
--rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_model_v0.1.26.py
--rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_model_v0.1.31.py
--rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft/tft_model_v1.1.3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:55:30.846187 fmldk-1.2.3/tft_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36585 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft_gpu/tft_data_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft_gpu/tft_losses_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-05-09 12:55:13.000000 fmldk-1.2.3/tft_gpu/tft_model_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.485812 fmldk-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-17 16:49:43.485812 fmldk-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-05-17 16:49:32.000000 fmldk-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/ctfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_models_v0.1.29.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfr/ctfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/ctfrv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2/ctfrv2_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/ctfrv2_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/ctfrv2_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/ctfrv2_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78757 2023-05-17 16:49:32.000000 fmldk-1.2.4/ctfrv2_gpu/ctfrv2_model_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.473812 fmldk-1.2.4/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib_v0.1.19.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-05-17 16:49:32.000000 fmldk-1.2.4/eda/eda_lib_v0.1.37.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/fmldk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 16:49:43.000000 fmldk-1.2.4/fmldk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/sage/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46655 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_global_scaled_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_losses_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage/sage_model_old.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/sage_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36569 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90885 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87795 2023-05-17 16:49:32.000000 fmldk-1.2.4/sage_gpu/sage_model_gpu_v1.2.3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:49:43.485812 fmldk-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-17 16:49:32.000000 fmldk-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.477812 fmldk-1.2.4/stctn/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-05-17 16:49:32.000000 fmldk-1.2.4/stctn/stctn_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.481812 fmldk-1.2.4/tfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_data_v0.1.21.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_local_block_sparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.23.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-05-17 16:49:32.000000 fmldk-1.2.4/tfr/tfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.485812 fmldk-1.2.4/tft/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46653 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data_v1.1.3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_data_v1.1.7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model_v0.1.26.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model_v0.1.31.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft/tft_model_v1.1.3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:49:43.485812 fmldk-1.2.4/tft_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36585 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/tft_data_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/tft_losses_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78604 2023-05-17 16:49:32.000000 fmldk-1.2.4/tft_gpu/tft_model_gpu.py
```

### Comparing `fmldk-1.2.3/PKG-INFO` & `fmldk-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.2.3
+Version: 1.2.4
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.2.3/README.md` & `fmldk-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfr/ctfr_data.py` & `fmldk-1.2.4/ctfr/ctfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfr/ctfr_losses.py` & `fmldk-1.2.4/ctfr/ctfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfr/ctfr_losses_bkp.py` & `fmldk-1.2.4/ctfr/ctfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfr/ctfr_models.py` & `fmldk-1.2.4/ctfr/ctfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfr/ctfr_models_v0.1.29.py` & `fmldk-1.2.4/ctfr/ctfr_models_v0.1.29.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfr/ctfr_models_v0.1.31.py` & `fmldk-1.2.4/ctfr/ctfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfrv2/ctfrv2_data.py` & `fmldk-1.2.4/ctfrv2/ctfrv2_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfrv2/ctfrv2_global_scaled_data.py` & `fmldk-1.2.4/ctfrv2/ctfrv2_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfrv2/ctfrv2_losses.py` & `fmldk-1.2.4/ctfrv2/ctfrv2_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfrv2/ctfrv2_models.py` & `fmldk-1.2.4/ctfrv2/ctfrv2_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfrv2_gpu/ctfrv2_data_gpu.py` & `fmldk-1.2.4/ctfrv2_gpu/ctfrv2_data_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfrv2_gpu/ctfrv2_losses_gpu.py` & `fmldk-1.2.4/ctfrv2_gpu/ctfrv2_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/ctfrv2_gpu/ctfrv2_model_gpu.py` & `fmldk-1.2.4/ctfrv2_gpu/ctfrv2_model_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/eda/eda_lib.py` & `fmldk-1.2.4/eda/eda_lib.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/eda/eda_lib_v0.1.18.py` & `fmldk-1.2.4/eda/eda_lib_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/eda/eda_lib_v0.1.19.py` & `fmldk-1.2.4/eda/eda_lib_v0.1.19.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/eda/eda_lib_v0.1.37.py` & `fmldk-1.2.4/eda/eda_lib_v0.1.37.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/fmldk.egg-info/PKG-INFO` & `fmldk-1.2.4/fmldk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.2.3
+Version: 1.2.4
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.2.3/fmldk.egg-info/SOURCES.txt` & `fmldk-1.2.4/fmldk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 sage/sage_losses_old.py
 sage/sage_model.py
 sage/sage_model_old.py
 sage_gpu/__init__.py
 sage_gpu/sage_data_gpu.py
 sage_gpu/sage_losses_gpu.py
 sage_gpu/sage_model_gpu.py
+sage_gpu/sage_model_gpu_v1.2.3.py
 stctn/__init__.py
 stctn/stctn_data.py
 stctn/stctn_losses.py
 stctn/stctn_losses_bkp.py
 stctn/stctn_models.py
 tfr/__init__.py
 tfr/tfr_data.py
```

### Comparing `fmldk-1.2.3/sage/sage_data.py` & `fmldk-1.2.4/sage/sage_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage/sage_data_old.py` & `fmldk-1.2.4/sage/sage_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage/sage_global_scaled_data_old.py` & `fmldk-1.2.4/sage/sage_global_scaled_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage/sage_losses.py` & `fmldk-1.2.4/sage/sage_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage/sage_losses_old.py` & `fmldk-1.2.4/sage/sage_losses_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage/sage_model.py` & `fmldk-1.2.4/sage/sage_model.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage/sage_model_old.py` & `fmldk-1.2.4/sage/sage_model_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage_gpu/sage_data_gpu.py` & `fmldk-1.2.4/sage_gpu/sage_data_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage_gpu/sage_losses_gpu.py` & `fmldk-1.2.4/sage_gpu/sage_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/sage_gpu/sage_model_gpu.py` & `fmldk-1.2.4/sage_gpu/sage_model_gpu_v1.2.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/setup.py` & `fmldk-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 # The directory containing this file
 this_directory = Path(__file__).parent
 long_description  = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="fmldk",
-    version="1.2.3",
+    version="1.2.4",
     description="Forecast ML library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rahul Sinha",
     author_email="rahul.sinha@unilever.com",
     packages=["sage","sage_gpu","tfr","tft","tft_gpu","stctn","ctfr","ctfrv2","ctfrv2_gpu","eda"],
     include_package_data=True,
-    install_requires=["tensorflow", "tensorflow_probability", "numpy", "statsmodels", "pandas", "joblib", "pathlib",
-                      "bokeh", "holoviews", "hvplot", "ennemi"]
+    install_requires=["tensorflow", "tensorflow_probability", "numpy", "statsmodels", "pandas", "joblib", "pathlib", "bokeh", "holoviews", "hvplot", "ennemi"]
 )
```

### Comparing `fmldk-1.2.3/stctn/stctn_data.py` & `fmldk-1.2.4/stctn/stctn_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/stctn/stctn_losses.py` & `fmldk-1.2.4/stctn/stctn_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/stctn/stctn_losses_bkp.py` & `fmldk-1.2.4/stctn/stctn_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/stctn/stctn_models.py` & `fmldk-1.2.4/stctn/stctn_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data.py` & `fmldk-1.2.4/tfr/tfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data_v0.1.11.py` & `fmldk-1.2.4/tfr/tfr_data_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data_v0.1.12.py` & `fmldk-1.2.4/tfr/tfr_data_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data_v0.1.14.py` & `fmldk-1.2.4/tfr/tfr_data_v0.1.14.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data_v0.1.15.py` & `fmldk-1.2.4/tfr/tfr_data_v0.1.15.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data_v0.1.16.py` & `fmldk-1.2.4/tfr/tfr_data_v0.1.16.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data_v0.1.18.py` & `fmldk-1.2.4/tfr/tfr_data_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_data_v0.1.21.py` & `fmldk-1.2.4/tfr/tfr_data_v0.1.21.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_local_block_sparse_attention.py` & `fmldk-1.2.4/tfr/tfr_local_block_sparse_attention.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_local_block_sparse_attention_v0.1.10.py` & `fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_local_block_sparse_attention_v0.1.12.py` & `fmldk-1.2.4/tfr/tfr_local_block_sparse_attention_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_losses.py` & `fmldk-1.2.4/tfr/tfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_losses_bkp.py` & `fmldk-1.2.4/tfr/tfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_models.py` & `fmldk-1.2.4/tfr/tfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_models_v0.1.10.py` & `fmldk-1.2.4/tfr/tfr_models_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_models_v0.1.11.py` & `fmldk-1.2.4/tfr/tfr_models_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_models_v0.1.23.py` & `fmldk-1.2.4/tfr/tfr_models_v0.1.23.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tfr/tfr_models_v0.1.31.py` & `fmldk-1.2.4/tfr/tfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_data.py` & `fmldk-1.2.4/tft/tft_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_data_old.py` & `fmldk-1.2.4/tft/tft_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_data_v1.1.3.py` & `fmldk-1.2.4/tft/tft_data_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_data_v1.1.7.py` & `fmldk-1.2.4/tft/tft_data_v1.1.7.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_global_scaled_data.py` & `fmldk-1.2.4/tft/tft_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_losses.py` & `fmldk-1.2.4/tft/tft_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_model.py` & `fmldk-1.2.4/tft/tft_model.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_model_v0.1.26.py` & `fmldk-1.2.4/tft/tft_model_v0.1.26.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_model_v0.1.31.py` & `fmldk-1.2.4/tft/tft_model_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft/tft_model_v1.1.3.py` & `fmldk-1.2.4/tft/tft_model_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft_gpu/tft_data_gpu.py` & `fmldk-1.2.4/tft_gpu/tft_data_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft_gpu/tft_losses_gpu.py` & `fmldk-1.2.4/tft_gpu/tft_losses_gpu.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.2.3/tft_gpu/tft_model_gpu.py` & `fmldk-1.2.4/tft_gpu/tft_model_gpu.py`

 * *Files identical despite different names*

