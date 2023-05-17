# Comparing `tmp/cnn2snn-2.3.5.tar.gz` & `tmp/cnn2snn-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnn2snn-2.3.5.tar", last modified: Fri Apr 28 06:59:14 2023, max compression
+gzip compressed data, was "dist/cnn2snn-2.3.6.tar", last modified: Wed May 17 14:19:31 2023, max compression
```

## Comparing `cnn2snn-2.3.5.tar` & `cnn2snn-2.3.6.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/
--rw-r--r--   0 root         (0) root         (0)     1483 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/akida_versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/calibration/
--rw-r--r--   0 root         (0) root         (0)      958 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16847 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/adaround.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)    12381 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/calibration.py
--rw-r--r--   0 root         (0) root         (0)    10739 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/cli.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/cnn2snn_objects.py
--rw-r--r--   0 root         (0) root         (0)    12382 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/converter.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/min_value_constraint.py
--rw-r--r--   0 root         (0) root         (0)    14077 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/model_generator.py
--rw-r--r--   0 root         (0) root         (0)    13749 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantization.py
--rw-r--r--   0 root         (0) root         (0)    26028 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantization_layers.py
--rw-r--r--   0 root         (0) root         (0)    12977 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantization_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/
--rw-r--r--   0 root         (0) root         (0)      882 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3229 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/activations.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/add.py
--rw-r--r--   0 root         (0) root         (0)     4489 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/attention.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/batchnorm.py
--rw-r--r--   0 root         (0) root         (0)     8996 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13938 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/concatenate.py
--rw-r--r--   0 root         (0) root         (0)     6573 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     8073 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/convolution.py
--rw-r--r--   0 root         (0) root         (0)     8514 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/dense.py
--rw-r--r--   0 root         (0) root         (0)     6266 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     6342 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/dequantizer.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/extract_token.py
--rw-r--r--   0 root         (0) root         (0)     3442 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/input_data.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/layer_utils.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/madnorm.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/model_generator.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/outputs.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/padding.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/pooling.py
--rw-r--r--   0 root         (0) root         (0)     5549 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/separable_convolution.py
--rw-r--r--   0 root         (0) root         (0)     3083 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/shiftmax.py
--rw-r--r--   0 root         (0) root         (0)     7990 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/stem.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/transforms/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/batch_normalization.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/clone.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/equalization.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/reshape.py
--rw-r--r--   0 root         (0) root         (0)    14261 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/sequential.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/utils.py
--rw-r--r--   0 root         (0) root         (0)    11223 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/weights_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1760 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2023-04-28 06:59:06.000000 cnn2snn-2.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      520 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/akida_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/cnn2snn/calibration/
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16847 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/adaround.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/calibration/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    10739 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/cnn2snn_objects.py
+-rw-r--r--   0 root         (0) root         (0)    12382 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/converter.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/min_value_constraint.py
+-rw-r--r--   0 root         (0) root         (0)    14077 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)    13749 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    26028 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantization_layers.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantization_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/activations.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/add.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/attention.py
+-rw-r--r--   0 root         (0) root         (0)     5283 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/block_converter.py
+-rw-r--r--   0 root         (0) root         (0)     9312 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    13554 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/concatenate.py
+-rw-r--r--   0 root         (0) root         (0)     6579 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/convolution.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/dense.py
+-rw-r--r--   0 root         (0) root         (0)     6272 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/dequantizer.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/extract_token.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/layer_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4981 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/madnorm.py
+-rw-r--r--   0 root         (0) root         (0)     6321 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/outputs.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/padding.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/separable_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/shiftmax.py
+-rw-r--r--   0 root         (0) root         (0)     7996 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/stem.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/quantizeml/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/cnn2snn/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/batch_normalization.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/clone.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/equalization.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/reshape.py
+-rw-r--r--   0 root         (0) root         (0)    14261 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/transforms/sequential.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11223 2023-05-17 14:19:28.000000 cnn2snn-2.3.6/cnn2snn/weights_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-17 14:19:30.000000 cnn2snn-2.3.6/cnn2snn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 14:19:31.000000 cnn2snn-2.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-05-17 14:19:24.000000 cnn2snn-2.3.6/setup.py
```

### Comparing `cnn2snn-2.3.5/LICENSE` & `cnn2snn-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/PKG-INFO` & `cnn2snn-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.5
+Version: 2.3.6
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.5/cnn2snn/__init__.py` & `cnn2snn-2.3.6/cnn2snn/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/akida_versions.py` & `cnn2snn-2.3.6/cnn2snn/akida_versions.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/calibration/__init__.py` & `cnn2snn-2.3.6/cnn2snn/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/calibration/adaround.py` & `cnn2snn-2.3.6/cnn2snn/calibration/adaround.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/calibration/bias_correction.py` & `cnn2snn-2.3.6/cnn2snn/calibration/bias_correction.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/calibration/calibration.py` & `cnn2snn-2.3.6/cnn2snn/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/cli.py` & `cnn2snn-2.3.6/cnn2snn/cli.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/cnn2snn_objects.py` & `cnn2snn-2.3.6/cnn2snn/cnn2snn_objects.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/compatibility_checks.py` & `cnn2snn-2.3.6/cnn2snn/compatibility_checks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/converter.py` & `cnn2snn-2.3.6/cnn2snn/converter.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/min_value_constraint.py` & `cnn2snn-2.3.6/cnn2snn/min_value_constraint.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/model_generator.py` & `cnn2snn-2.3.6/cnn2snn/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantization.py` & `cnn2snn-2.3.6/cnn2snn/quantization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantization_layers.py` & `cnn2snn-2.3.6/cnn2snn/quantization_layers.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantization_ops.py` & `cnn2snn-2.3.6/cnn2snn/quantization_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/__init__.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ******************************************************************************
 """Helper functions to convert to akida models, models quantized with quantizeml API.
 """
 from .model_generator import generate_model
+from .dense import *
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/activations.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/activations.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,55 +18,77 @@
 """
 import numpy as np
 from quantizeml.layers import QuantizedReLU, AlignedWeightQuantizer, OutputQuantizer
 from .weights import broadcast_and_set_variable
 from ..akida_versions import AkidaVersion, get_akida_version
 
 
-def parse_relu(layer_k):
-    """Parses the quantizeml.QuantizedReLU parameters.
+def v1_relu_checks(layer):
+    """Additionnal checks on QuantizedReLU layers of akida v1 models.
 
     Args:
-        layer_k (:obj:`tf.keras.Layer`): the InputLayer to parser.
+        layer (:obj:`tf.keras.Layer`): the QuantizedReLU layer to check.
+    """
+    assert isinstance(layer.max_value_quantizer, AlignedWeightQuantizer)
+    lname = layer.name
+    # Check if there is an output_quantizer
+    out_quantizer = getattr(layer, "out_quantizer", None)
+    if not out_quantizer:
+        raise ValueError(f"{lname}: in AkidaVersion.v1, output_quantizer is mandatory.")
+    assert isinstance(out_quantizer, OutputQuantizer)
+    if out_quantizer._axis == "per-axis":
+        raise ValueError(f"{lname}: in AkidaVersion.v1, output_quantizer must be per-tensor.")
+
+
+def parse_relu_v1(layer_k):
+    """Parses the quantizeml.QuantizedReLU parameters for Akida v1 layers.
+
+    Args:
+        layer_k (:obj:`tf.keras.Layer`): the QuantizedReLU layer to parse.
+
+    Returns:
+        dict: the corresponding akida parameters.
+    """
+    # Check if there is an output_quantizer
+    out_quantizer = getattr(layer_k, "out_quantizer", None)
+
+    return {'activation': True, 'act_bits': out_quantizer.bitwidth}
+
+
+def parse_relu_v2(layer_k):
+    """Parses the quantizeml.QuantizedReLU parameters for Akida v2 layers.
+
+    Args:
+        layer_k (:obj:`tf.keras.Layer`): the QuantizedReLU layer to parse.
 
     Returns:
         dict: the corresponding akida parameters.
     """
-    assert isinstance(layer_k, QuantizedReLU)
     assert isinstance(layer_k.max_value_quantizer, AlignedWeightQuantizer)
 
     # Check if there is an output_quantizer
     out_quantizer = getattr(layer_k, "out_quantizer", None)
-    lname = layer_k.name
 
     if not out_quantizer:
-        if get_akida_version() == AkidaVersion.v1:
-            raise ValueError(f"{lname}: in AkidaVersion.v1, output_quantizer is mandatory.")
         return {'activation': True}
 
     assert isinstance(out_quantizer, OutputQuantizer)
-    bitwidth = out_quantizer.bitwidth
-    if get_akida_version() == AkidaVersion.v2:
-        bitwidth_param = 'output_bits'
-    else:
-        bitwidth_param = 'act_bits'
-        if out_quantizer._axis == "per-axis":
-            raise ValueError(f"{lname}: in AkidaVersion.v1, output_quantizer must be per-tensor.")
-    return {'activation': True, bitwidth_param: bitwidth}
+    return {'activation': True, 'output_bits': out_quantizer.bitwidth}
 
 
 def set_relu_variables(layer_ak, layer_k):
     """Computes and sets the activation variables in an akida layer.
 
     Args:
         layer_ak (:obj:`akida.Layer`): the targeted akida layer.
         layer_k (:obj:`quantizeml.QuantizedRelu`): the source QuantizedReLU layer.
     """
     # Nothing to do in AkidaVersion.v1 : the values will be modified by
-    # :func:`set_output_variables`.
+    # :func:`set_output_v1_variables`.
+    # TODO: remove this checks once the conversion pipeline uses only BlockConverter
     if get_akida_version() == AkidaVersion.v1:
         return
 
     assert isinstance(layer_k, QuantizedReLU)
 
     variables_ak = layer_ak.variables
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/add.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/add.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/attention.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/attention.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/batchnorm.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/batchnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 """Functions to convert QuantizedBatchNormalization to Akida.
 """
 from akida import LayerType, BatchNormalization
 import quantizeml.layers as qlayers
 import numpy as np
 
 from .weights import broadcast_and_set_variable
-from .outputs import set_output_variables
-from .activations import parse_relu, set_relu_variables
+from .outputs import set_output_v2_variables
+from .activations import parse_relu_v2, set_relu_variables
 from .layer_utils import get_inbound_layers
 
 
 def _set_batchnorm_variables(ak_layer, block):
     """Computes and sets the variables for an Akida BatchNormalization layer.
 
     This function converts the variables of a Keras layer and sets them into
@@ -64,15 +64,15 @@
     if len(block) > 1:
         relu_layer = block[1]
         set_relu_variables(ak_layer, relu_layer)
         # the effective output_quantizer should be the relu one
         out_quantizer = getattr(relu_layer, "out_quantizer", False)
 
     if out_quantizer:
-        set_output_variables(ak_layer, out_quantizer)
+        set_output_v2_variables(ak_layer, out_quantizer)
 
 
 def _create_batchnorm(layer_block):
     """Parses a quantizeml QuantizedBatchNormalization layer and returns the
     params to create the corresponding Akida BatchNormalization layer.
 
     Args:
@@ -82,15 +82,15 @@
     Returns:
         :obj:`akida.BatchNormalization`: The created akida layer.
     """
     layer = layer_block[0]
     assert isinstance(layer, qlayers.QuantizedBatchNormalization)
     act_params = {}
     if len(layer_block) > 1:
-        act_params = parse_relu(layer_block[1])
+        act_params = parse_relu_v2(layer_block[1])
     # In quantizeml one bit is reserved for the sign in the buffer bitwidth
     # variable, but in akida this value has to be added back to have the
     # correct clipping.
     buffer_bits = layer.buffer_bitwidth + 1
     # If there is no activation, find out output_bits
     if not act_params:
         out_quantizer = getattr(layer, "out_quantizer", False)
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/blocks.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from quantizeml.layers import (QuantizedMaxPool2D,
                                QuantizedGlobalAveragePooling2D,
                                QuantizedReLU,
                                QuantizedExtractToken,
                                Dequantizer)
 
 from .pooling import parse_max_pooling, parse_global_average_pooling
-from .activations import parse_relu
+from .activations import parse_relu_v1, parse_relu_v2
 from ..akida_versions import AkidaVersion, get_akida_version
 
 
 def parse_block_additional_layers(layers, block_params):
     """Parse block additional layers into the parameters of one.
 
     In Akida v1, we are able to manage this sequence of layers:
@@ -50,15 +50,16 @@
         block_params (dict): the current block parameters.
 
     Returns:
         dict: additional layers found in the process, with layer type as key
     """
     # Identify the next layers
     next_layers = {}
-    if get_akida_version() == AkidaVersion.v1:
+    akida_version = get_akida_version()
+    if akida_version == AkidaVersion.v1:
         layer_types = [QuantizedMaxPool2D, QuantizedGlobalAveragePooling2D, QuantizedReLU]
     else:
         layer_types = [QuantizedMaxPool2D, QuantizedReLU, QuantizedGlobalAveragePooling2D]
     index = 1
     while index < len(layers) and layer_types:
         layer_type = layer_types.pop(0)
         layer = layers[index]
@@ -83,15 +84,20 @@
         pool_params = parse_max_pooling(max_pool_layer)
         # Padding checked on check_compatibility_model()
         block_params.update(pool_params)
     if global_average_pool_layer:
         pool_params = parse_global_average_pooling(global_average_pool_layer)
         block_params.update(pool_params)
     if relu_layer:
-        act_params = parse_relu(relu_layer)
+        # TODO: Remove the dependence to the akida_version when the conv block conversion
+        # will be done with it proper ConvBlockConverter
+        if akida_version == AkidaVersion.v1:
+            act_params = parse_relu_v1(relu_layer)
+        else:
+            act_params = parse_relu_v2(relu_layer)
         block_params.update(act_params)
 
     return next_layers
 
 
 def split_model_into_blocks(model):
     """Search into the model the sets of possible blocks and return them.
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/compatibility_checks.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/compatibility_checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 """
 from keras import layers
 from quantizeml import layers as qlayers
 
 from .blocks import split_model_into_blocks
 from .padding import check_same_valid_compatibility
 from ..transforms.sequential import _check_layers_data_format, _check_layer_inbounds
-from ..compatibility_checks import _check_reshape_layer
 from ..akida_versions import get_akida_version, AkidaVersion
+from .block_converter import _V1_PATTERN_CONVERTERS, _V2_PATTERN_CONVERTERS
 
 neural_layers = (qlayers.QuantizedConv2D, qlayers.QuantizedSeparableConv2D,
                  qlayers.QuantizedDense, qlayers.QuantizedDepthwiseConv2D,
                  qlayers.QuantizedConv2DTranspose, qlayers.QuantizedDepthwiseConv2DTranspose)
-skippable_layers = (layers.InputLayer, layers.Reshape, layers.Flatten, layers.Rescaling,
-                    layers.Activation, layers.Softmax, layers.Dropout)
+skippable_layers = (layers.InputLayer, layers.Rescaling, layers.Activation, layers.Softmax,
+                    layers.Dropout)
 pooling_layers = (qlayers.QuantizedGlobalAveragePooling2D, qlayers.QuantizedMaxPool2D)
 norm_layers = (qlayers.LayerMadNormalization, qlayers.QuantizedBatchNormalization)
 activation_layers = (qlayers.QuantizedReLU,)
 stem_layers = (qlayers.ClassToken, qlayers.AddPositionEmbs)
+reshape_layers = (qlayers.QuantizedReshape, qlayers.QuantizedFlatten)
 
 
 class CompatibilityMessage:
     """Helper to represent an error message
 
     Args:
         message (str): main error message.
@@ -83,14 +84,45 @@
         return err_msg
 
     def __call__(self):
         if self.status:
             raise RuntimeError(str(self))
 
 
+def _block_pattern(block):
+    """Method that returns the pattern of a block of layers.
+
+    Args:
+        block (list): list of quantized quantizeml layers.
+
+    Returns:
+        tuple: list of layer types representing the block pattern.
+    """
+    return tuple([layer.__class__ for layer in block])
+
+
+def _get_block_converter(block):
+    """Helper to get the BlockConverter of a block of layers.
+
+    Args:
+        block (list): list of quantized quantizeml layers.
+
+    Returns:
+        (:obj:`BlockConverter`): the BlockConverter corresponding to the block of layers or None.
+    """
+    pattern = _block_pattern(block)
+
+    if get_akida_version() == AkidaVersion.v1:
+        block_converter = _V1_PATTERN_CONVERTERS.get(pattern, None)
+    else:
+        block_converter = _V2_PATTERN_CONVERTERS.get(pattern, None)
+
+    return block_converter
+
+
 def check_model_compatibility(model):
     r"""Checks if a QuantizeML model is compatible for Akida conversion.
 
     This function does NOT:
 
     - convert the QuantizeML model to an Akida model,
     - check if the model is compatible with Akida hardware
@@ -111,27 +143,34 @@
     _check_layers_data_format(model)
     if get_akida_version() == AkidaVersion.v1:
         _check_layer_inbounds(model)
 
     # Split model into theirs blocks:
     blocks = split_model_into_blocks(model)
 
-    non_skippable_layers = []
+    # This list will contains either a block converter instance,
+    # or a list of non-skippable layers.
+    straight_blocks = []
     # Evaluate block-by-block integrity
     for block in blocks:
-        # Check reshape/flatten layers
-        skippable, block = _extract_skippable_layers(block)
-        _check_skippable_compatibility(skippable)
+        # Split blocks into skippable and none skippable blocks
+        _, non_skippable = _extract_skippable_layers(block)
+        # Get the corresponding BlockConverter of the layers block if available.
+        block_converter = _get_block_converter(non_skippable)
+        if block_converter:
+            straight_blocks.append(block_converter(non_skippable))
+            continue
+        # TODO: remove this part once all conversion uses BlockConverter classes
         # Check pooling layers
-        _check_pooling_compatibility(block)
+        _check_pooling_compatibility(non_skippable)
         # Check other rules
-        _check_block_integrity(block)
-        if len(block) > 0:
-            non_skippable_layers.append(block)
-    return non_skippable_layers
+        _check_block_integrity(non_skippable)
+        if len(non_skippable) > 0:
+            straight_blocks.append(non_skippable)
+    return straight_blocks
 
 
 def _split_block_into_layer_types(block):
     """Split input block into the following categories:
 
     - neural (processing) layers,
     - activation layers,
@@ -150,14 +189,16 @@
             neurals.append(layer)
         elif isinstance(layer, activation_layers):
             acts.append(layer)
         elif isinstance(layer, norm_layers):
             norms.append(layer)
         elif isinstance(layer, stem_layers):
             stems.append(layer)
+        elif isinstance(layer, reshape_layers):
+            continue
         elif not isinstance(layer, pooling_layers):
             raise RuntimeError(f"Unrecognizable layer in block: {layer.name}")
     return neurals, acts, norms, stems
 
 
 def _check_block_integrity(block):
     """Check integrity of one block.
@@ -201,16 +242,17 @@
             errors.push("A block must end by an activation layer", block[-1])
 
     # General limitations
     if len(block) > 1:
         neurals, acts, norms, stems = _split_block_into_layer_types(block)
         if len(neurals) != 1:
             errors.push("A block must have one neural layer", neurals)
-        if block[0] != neurals[0]:
-            errors.push("A block must start by a neural layer", block[0])
+        if len(neurals) > 0:
+            if block[0] != neurals[0]:
+                errors.push("A block must start by a neural layer", block[0])
         if len(acts) > 1:
             errors.push("A block could have up to only one activation layer", acts)
         if len(norms) != 0:
             errors.push("A block should not have normalization layers: "
                         "these must be folded into previous neural layers", norms)
         if len(stems) > 0:
             if ak_version == AkidaVersion.v1:
@@ -270,52 +312,14 @@
         if isinstance(layer, skippable_layers):
             skippable.append(layer)
         else:
             non_skippable.append(layer)
     return skippable, non_skippable
 
 
-def _check_skippable_compatibility(skippables):
-    """Check rules over quantized skippable layers
-
-    Args:
-        skippables (list(tf.keras.Layer)): layers list to check.
-    """
-    def _find_next_non_skippable_outbounds(layer):
-        outbound = layer.outbound_nodes
-        if len(outbound) == 1:
-            outbound_layer = outbound[0].outbound_layer
-            if isinstance(outbound_layer, skippable_layers):
-                return _find_next_non_skippable_outbounds(outbound_layer)
-            # If outbound layer is a Dequantizer, target is considered as the final quantized layer
-            if isinstance(outbound_layer, qlayers.Dequantizer):
-                outbound = []
-        return outbound
-
-    for layer in skippables:
-        if isinstance(layer, qlayers.QuantizedReshape):
-            # There are not rules on Akida 2.0 about QuantizedReshape.
-            if get_akida_version() == AkidaVersion.v1:
-                _check_reshape_layer(layer)
-            continue
-        # For the next layer types, we can skip checks if they are the last ones in the model
-        outbound = _find_next_non_skippable_outbounds(layer)
-        if len(outbound) == 0:
-            continue
-        elif isinstance(layer, qlayers.QuantizedFlatten):
-            # QuantizedFlatten outbound must be one QuantizedDense
-            outbound_layer = outbound[0].outbound_layer
-            if len(outbound) > 1 or not isinstance(outbound_layer, qlayers.QuantizedDense):
-                raise RuntimeError("A QuantizedFlatten layer is only supported at the end of "
-                                   "the model or before a QuantizedDense. "
-                                   f"Layer: {layer.name}")
-        elif not isinstance(layer, skippable_layers):
-            raise RuntimeError(f"Incompatible {layer.name} skippable layer.")
-
-
 def _check_pooling_compatibility(block):
     """Asserts pooling layer is compatible for conversion.
 
     Args:
         block (list): the layers block.
     """
     errors = CompatibilityBlockError()
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/concatenate.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/concatenate.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/conv2d_transpose.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/conv2d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from quantizeml.layers import (QuantizedConv2DTranspose, QuantizedReLU,
                                QuantizedMaxPool2D, WeightQuantizer, AlignedWeightQuantizer)
 from akida import Conv2DTranspose
 
 from ..akida_versions import AkidaVersion, get_akida_version
 from .activations import set_relu_variables
 from .weights import broadcast_and_set_variable
-from .outputs import set_output_variables
+from .outputs import set_output_v2_variables
 from .blocks import parse_block_additional_layers, get_block_out_quantizer
 
 
 def _set_conv2d_transpose_variables(layer_ak, layer_k):
     """Computes and sets the variables for an Akida Conv2DTranspose layer.
 
     This function converts the variables of a Keras layer and sets them into
@@ -162,10 +162,10 @@
 
     # Set optional activation variables
     if relu_layer:
         set_relu_variables(conv_transpose_ak, relu_layer)
 
     # Set optional output_quantizer variables
     if out_quantizer:
-        set_output_variables(conv_transpose_ak, out_quantizer)
+        set_output_v2_variables(conv_transpose_ak, out_quantizer)
 
     return 1 + len(next_layers)
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/convolution.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/convolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from quantizeml.layers import (QuantizedConv2D, QuantizedReLU, QuantizedGlobalAveragePooling2D,
                                WeightQuantizer, AlignedWeightQuantizer)
 from akida import InputConvolutional, Convolutional, LayerType, Conv2D, InputConv2D
 
 from ..akida_versions import AkidaVersion, get_akida_version
 from .activations import set_relu_variables
 from .pooling import set_pooling_variables
-from .outputs import set_output_variables
+from .outputs import set_output_v1_variables, set_output_v2_variables
 from .padding import get_padding_info
 from .blocks import parse_block_additional_layers, get_block_out_quantizer
 from .weights import broadcast_and_set_variable
 
 
 def _set_conv2d_variables(layer_ak, layer_k):
     """Computes and sets the variables for an Akida convolutional layer.
@@ -190,10 +190,13 @@
             # Set the optional activation variables
             set_relu_variables(conv_ak, relu_layer)
 
     # Get out_quantizer of the block.
     out_quantizer = get_block_out_quantizer([conv] + list(next_layers.values()))
 
     if out_quantizer:
-        set_output_variables(conv_ak, out_quantizer)
+        if isinstance(conv_ak, (InputConvolutional, Convolutional)):
+            set_output_v1_variables(conv_ak, out_quantizer)
+        else:
+            set_output_v2_variables(conv_ak, out_quantizer)
 
     return 1 + len(next_layers)
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from quantizeml.layers import (QuantizedDepthwiseConv2D, QuantizedReLU,
                                WeightQuantizer, AlignedWeightQuantizer)
 from akida import DepthwiseConv2D
 
 from ..akida_versions import AkidaVersion, get_akida_version
 from .activations import set_relu_variables
 from .weights import broadcast_and_set_variable
-from .outputs import set_output_variables
+from .outputs import set_output_v2_variables
 from .padding import get_padding_info
 from .blocks import parse_block_additional_layers
 
 
 def _set_depthwise_conv2d_variables(layer_ak, layer_k):
     """Computes and sets the variables for an Akida DepthwiseConv2D layer.
 
@@ -165,10 +165,10 @@
 
     # Set optional activation variables
     if relu_layer:
         set_relu_variables(dw_conv_ak, relu_layer)
 
     # Set optional output_quantizer variables
     if out_quantizer:
-        set_output_variables(dw_conv_ak, out_quantizer)
+        set_output_v2_variables(dw_conv_ak, out_quantizer)
 
     return 1 + len(next_layers)
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d_transpose.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/depthwise_conv2d_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from quantizeml.layers import (QuantizedDepthwiseConv2DTranspose, QuantizedReLU,
                                WeightQuantizer, AlignedWeightQuantizer)
 from akida import DepthwiseConv2DTranspose
 
 from ..akida_versions import AkidaVersion, get_akida_version
 from .activations import set_relu_variables
 from .weights import broadcast_and_set_variable
-from .outputs import set_output_variables
+from .outputs import set_output_v2_variables
 from .blocks import parse_block_additional_layers, get_block_out_quantizer
 
 
 def _set_depthwise_conv2d_transpose_variables(layer_ak, layer_k):
     """Computes and sets the variables for an Akida DepthwiseConv2DTranspose layer.
 
     This function converts the variables of a Keras layer and sets them into
@@ -158,10 +158,10 @@
     # Set optional activation variables if we have a ReLU
     relu_layer = next_layers.get(QuantizedReLU, None)
     if relu_layer:
         set_relu_variables(dw_conv_ak, relu_layer)
 
     # Set optional output_quantizer variables
     if out_quantizer:
-        set_output_variables(dw_conv_ak, out_quantizer)
+        set_output_v2_variables(dw_conv_ak, out_quantizer)
 
     return len(layer_block)
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/dequantizer.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/dequantizer.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/extract_token.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/extract_token.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/input_data.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/input_data.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/layer_utils.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/layer_utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/madnorm.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/madnorm.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 from akida import LayerType, MadNorm
 import quantizeml.layers as qlayers
 import numpy as np
 
 from .layer_utils import get_inbound_layers
 from .weights import broadcast_and_set_variable
-from .outputs import set_output_variables
+from .outputs import set_output_v2_variables
 
 
 def _set_madnorm_variables(ak_layer, k_layer):
     """Computes and sets the variables for an Akida MadNorm layer.
 
     This function converts the variables of a Keras layer and sets them into
     the corresponding variables of the equivalent Akida layer.
@@ -61,15 +61,15 @@
                                    input_shift.value.numpy().astype(np.uint8))
     variables_ak["gamma"] = gamma_ak.astype(np.int8)
     broadcast_and_set_variable(variables_ak, "gamma_shift", gamma_shift)
     variables_ak["beta"] = beta_ak.astype(np.int8)
     broadcast_and_set_variable(variables_ak, "beta_shift", beta_shift)
     out_quantizer = getattr(k_layer, "out_quantizer", False)
     if out_quantizer:
-        set_output_variables(ak_layer, out_quantizer)
+        set_output_v2_variables(ak_layer, out_quantizer)
 
 
 def _create_madnorm(layer):
     """Parses a quantizeml QuantizedLayerNormalization layer and returns the
     params to create the corresponding Akida MadNorm layer.
 
     Args:
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/model_generator.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/model_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 import quantizeml.layers as qlayers
 from quantizeml.models import record_quantization_variables
 from akida import Model
 
 from .depthwise_conv2d import convert_depthwise_conv_block
 from .depthwise_conv2d_transpose import convert_depthwise_conv2d_transpose_block
-from .dense import convert_dense_block
 from .add import convert_quantized_add
 from .input_data import convert_input
 from .shiftmax import convert_quantized_shiftmax
 from .attention import convert_quantized_attention
 from .madnorm import convert_quantized_madnorm
 from .stem import convert_quantized_stem_layers
 from .concatenate import convert_quantized_concatenate
@@ -35,14 +34,15 @@
 from .separable_convolution import convert_sepconv_block
 from .batchnorm import convert_batchnorm_block
 from .extract_token import convert_extract_token
 from .conv2d_transpose import convert_conv_transpose_block
 from .dequantizer import convert_dequantizer
 from ..akida_versions import AkidaVersion, get_akida_version
 from .compatibility_checks import check_model_compatibility
+from .block_converter import BlockConverter
 
 
 def _raise_block_error(block):
     """ Raise error due to non convertible layers block"""
     block_layers_name = ""
     block_layers_type = ""
     for layer in block:
@@ -73,61 +73,55 @@
 
     model_ak = Model()
 
     # Identify the input block
     ak_version = get_akida_version()
     # Flag to identify if the current block has been converted
     converted = False
-    if ak_version == AkidaVersion.v2 and input_is_image:
-        # Convert the akida 2.0 stem block layer if the keras model has one.
-        converted = convert_quantized_stem_layers(model_ak, blocks[0])
-    if not converted and input_is_image:
-        # Look for an input convolution layer
-        converted = convert_conv_block(model_ak, blocks[0])
+    if not isinstance(blocks[0], BlockConverter) and input_is_image:
+        if ak_version == AkidaVersion.v2:
+            # Convert the akida 2.0 stem block layer if the keras model has one.
+            converted = convert_quantized_stem_layers(model_ak, blocks[0])
+        if not converted:
+            # Look for an input convolution layer
+            converted = convert_conv_block(model_ak, blocks[0])
     if not converted:
         # Convert the keras InputLayer into an InputData layer
         convert_input(model_ak, model.layers[0], input_is_image)
-
-    if converted:
+    else:
         blocks.pop(0)
 
     for block in blocks:
         # Create and add layer to the akida model
-        # The next check converts the potential dense_block layers to a QuantizedDense,
-        converted = convert_dense_block(model_ak, block)
-        if converted:
-            continue
+        # The next check converts the potential dense_block layers to a QuantizedDense
+        if isinstance(block, BlockConverter):
+            if block.convert(model_ak):
+                continue
         # conv_block layers to a QuantizedConv2D
-        converted = convert_conv_block(model_ak, block)
-        if converted:
+        if convert_conv_block(model_ak, block):
             continue
         # and sepconv_block to a QuantizedSeparableConv2D
-        converted = convert_sepconv_block(model_ak, block)
-        if converted:
+        if convert_sepconv_block(model_ak, block):
             continue
         # Dequantizer conversion applies in both version
         if isinstance(block[0], qlayers.Dequantizer):
             convert_dequantizer(model_ak, block[0])
             continue
         # The other modules are for v2 only
         if get_akida_version() != AkidaVersion.v2:
             # If you got here, the layer is not supported: raise an error.
             _raise_block_error(block)
-        converted = convert_batchnorm_block(model_ak, block)
-        if converted:
+        if convert_batchnorm_block(model_ak, block):
             continue
-        converted = convert_depthwise_conv_block(model_ak, block)
-        if converted:
+        if convert_depthwise_conv_block(model_ak, block):
             continue
         # convert conv_transpose_block to a QuantizedConv2DTranspose
-        converted = convert_conv_transpose_block(model_ak, block)
-        if converted:
+        if convert_conv_transpose_block(model_ak, block):
             continue
-        converted = convert_depthwise_conv2d_transpose_block(model_ak, block)
-        if converted:
+        if convert_depthwise_conv2d_transpose_block(model_ak, block):
             continue
         if len(block) == 1:
             layer = block[0]
             if isinstance(layer, qlayers.QuantizedAdd):
                 convert_quantized_add(model_ak, layer)
             elif isinstance(layer, qlayers.QuantizedShiftmax):
                 convert_quantized_shiftmax(model_ak, layer)
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/outputs.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/outputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,44 +15,55 @@
 # limitations under the License.
 # ******************************************************************************
 """Functions to update akida layer output variables from a keras OutputQuantizer.
 """
 import numpy as np
 from quantizeml.layers import OutputQuantizer
 from quantizeml.tensors import pow2
-
-from ..akida_versions import AkidaVersion, get_akida_version
 from .weights import broadcast_and_set_variable
 
 
-def set_output_variables(layer_ak, out_quantizer):
-    """Computes and sets the output variables in an akida layer.
+def set_output_v1_variables(layer_ak, out_quantizer):
+    """Computes and sets the output variables in an akida v1 layer.
 
     Args:
-        layer_ak (:obj:`akida.Layer`): the targeted akida layer.
+        layer_ak (:obj:`akida.Layer`): the targeted akida v1 layer.
         out_quantizer (:obj:`quantizeml.OutputQuantizer`): the source output quantizer.
     """
     assert isinstance(out_quantizer, OutputQuantizer)
 
     # Extract the OutputQuantizer variables
     scales = out_quantizer.qscales.value.values
     shift = out_quantizer.shift.value
 
     # Quantizeml evaluates the outputs as: y = x * scales * 2^shift
-    if get_akida_version() == AkidaVersion.v1:
-        # Calculate the float activation step, as the reciprocal of (scales * 2^shift)
-        scales_rec = (pow2(-shift) / scales).numpy().astype(np.float32)
-        # In akida 1.0, the outputs are evaluated as: y = x / act_step
-        layer_ak.variables["act_step"] = scales_rec
-        if layer_ak.parameters.activation:
-            # For activations, x is decreased by half the activations step before division
-            # to increase the precision. This is obtained by increasing the threshold.
-            layer_ak.variables["threshold"] += np.round(0.5 * scales_rec).astype(np.int32)
-            # Adjust activation step to match activation formula
-            act_bits = layer_ak.parameters.act_bits
-            layer_ak.variables["act_step"] *= 2 ** (act_bits - 4)
-    else:
-        output_scales = scales.numpy().astype(np.uint8)
-        broadcast_and_set_variable(layer_ak.variables, "output_scales",
-                                   output_scales)
-        broadcast_and_set_variable(layer_ak.variables, "output_shift",
-                                   shift.numpy().astype(np.int8))
+    # Calculate the float activation step, as the reciprocal of (scales * 2^shift)
+    scales_rec = (pow2(-shift) / scales).numpy().astype(np.float32)
+    # In akida 1.0, the outputs are evaluated as: y = x / act_step
+    layer_ak.variables["act_step"] = scales_rec
+    if layer_ak.parameters.activation:
+        # For activations, x is decreased by half the activations step before division
+        # to increase the precision. This is obtained by increasing the threshold.
+        layer_ak.variables["threshold"] += np.round(0.5 * scales_rec).astype(np.int32)
+        # Adjust activation step to match activation formula
+        act_bits = layer_ak.parameters.act_bits
+        layer_ak.variables["act_step"] *= 2 ** (act_bits - 4)
+
+
+def set_output_v2_variables(layer_ak, out_quantizer):
+    """Computes and sets the output variables in an akida v2 layer.
+
+    Args:
+        layer_ak (:obj:`akida.Layer`): the targeted akida v2 layer.
+        out_quantizer (:obj:`quantizeml.OutputQuantizer`): the source output quantizer.
+    """
+    assert isinstance(out_quantizer, OutputQuantizer)
+
+    # Extract the OutputQuantizer variables
+    scales = out_quantizer.qscales.value.values
+    shift = out_quantizer.shift.value
+
+    output_scales = scales.numpy().astype(np.uint8)
+    broadcast_and_set_variable(layer_ak.variables, "output_scales",
+                               output_scales)
+    broadcast_and_set_variable(layer_ak.variables, "output_shift",
+                               shift.numpy().astype(np.int8))
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/padding.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/padding.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/pooling.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/pooling.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/separable_convolution.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/separable_convolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from akida import LayerType, SeparableConvolutional
 from quantizeml.layers import (QuantizedSeparableConv2D, QuantizedGlobalAveragePooling2D,
                                WeightQuantizer, AlignedWeightQuantizer)
 
 from ..akida_versions import AkidaVersion, get_akida_version
 from .pooling import set_pooling_variables
-from .outputs import set_output_variables
+from .outputs import set_output_v1_variables
 from .padding import get_padding_info
 from .blocks import parse_block_additional_layers, get_block_out_quantizer
 
 
 def _set_sepconv_variables(ak_layer, k_layer):
     """Computes and sets the variables for an Akida SeparableConvolutional layer.
 
@@ -134,10 +134,10 @@
     # Set variables
     _set_sepconv_variables(sepconv_ak, sepconv)
     pool_layer = next_layers.get(QuantizedGlobalAveragePooling2D, None)
     if pool_layer:
         set_pooling_variables(sepconv_ak, pool_layer)
     out_quantizer = get_block_out_quantizer([sepconv] + list(next_layers.values()))
     if out_quantizer:
-        set_output_variables(sepconv_ak, out_quantizer)
+        set_output_v1_variables(sepconv_ak, out_quantizer)
 
     return 1 + len(next_layers)
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/shiftmax.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/shiftmax.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/stem.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/stem.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     - The ClassToken (+ the DistToken for distilled models) layer(s)
     - The AddPosEmbedding layer
 """
 from akida import LayerType, Stem
 import quantizeml.layers as qlayers
 import numpy as np
 from .blocks import get_block_out_quantizer
-from .outputs import set_output_variables
+from .outputs import set_output_v2_variables
 from .weights import broadcast_and_set_variables
 
 
 def _set_stem_variables(ak_layer, layers):
     """Computes and sets the variables for an Akida Stem layer.
 
     This function converts the variables of a Keras layers and sets them into
@@ -197,10 +197,10 @@
     model_ak.add(layer_ak)
     _set_stem_variables(layer_ak, block)
     # Get out_quantizer of the block.
     out_quantizer = get_block_out_quantizer(block)
     # OutputQuantizer is mandatory at the end of the block
     assert isinstance(out_quantizer, qlayers.OutputQuantizer)
 
-    set_output_variables(layer_ak, out_quantizer)
+    set_output_v2_variables(layer_ak, out_quantizer)
 
     return True
```

### Comparing `cnn2snn-2.3.5/cnn2snn/quantizeml/weights.py` & `cnn2snn-2.3.6/cnn2snn/quantizeml/weights.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/transforms/__init__.py` & `cnn2snn-2.3.6/cnn2snn/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/transforms/batch_normalization.py` & `cnn2snn-2.3.6/cnn2snn/transforms/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/transforms/clone.py` & `cnn2snn-2.3.6/cnn2snn/transforms/clone.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/transforms/equalization.py` & `cnn2snn-2.3.6/cnn2snn/transforms/equalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/transforms/reshape.py` & `cnn2snn-2.3.6/cnn2snn/transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/transforms/sequential.py` & `cnn2snn-2.3.6/cnn2snn/transforms/sequential.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/utils.py` & `cnn2snn-2.3.6/cnn2snn/utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn/weights_ops.py` & `cnn2snn-2.3.6/cnn2snn/weights_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.5/cnn2snn.egg-info/PKG-INFO` & `cnn2snn-2.3.6/cnn2snn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.5
+Version: 2.3.6
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.5/cnn2snn.egg-info/SOURCES.txt` & `cnn2snn-2.3.6/cnn2snn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 cnn2snn/calibration/bias_correction.py
 cnn2snn/calibration/calibration.py
 cnn2snn/quantizeml/__init__.py
 cnn2snn/quantizeml/activations.py
 cnn2snn/quantizeml/add.py
 cnn2snn/quantizeml/attention.py
 cnn2snn/quantizeml/batchnorm.py
+cnn2snn/quantizeml/block_converter.py
 cnn2snn/quantizeml/blocks.py
 cnn2snn/quantizeml/compatibility_checks.py
 cnn2snn/quantizeml/concatenate.py
 cnn2snn/quantizeml/conv2d_transpose.py
 cnn2snn/quantizeml/convolution.py
 cnn2snn/quantizeml/dense.py
 cnn2snn/quantizeml/depthwise_conv2d.py
```

### Comparing `cnn2snn-2.3.5/setup.py` & `cnn2snn-2.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cnn2snn',
-    version='2.3.5',
+    version='2.3.6',
     description='Keras to Akida CNN Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alvaro Moran',
     author_email='amoran@brainchip.com',
     url='https://doc.brainchipinc.com',
     license='Apache 2.0',
     packages=['cnn2snn', 'cnn2snn.transforms', 'cnn2snn.calibration', 'cnn2snn.quantizeml'],
     entry_points={
         'console_scripts': [ 'cnn2snn = cnn2snn.cli:main' ]
     },
     install_requires=[get_tf_dep(), 'keras~=2.10.0',
-        'akida==2.3.5', 'quantizeml~=0.4.1'],
+        'akida==2.3.6', 'quantizeml~=0.4.1'],
 )
```

