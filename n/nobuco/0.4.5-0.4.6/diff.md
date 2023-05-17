# Comparing `tmp/nobuco-0.4.5.tar.gz` & `tmp/nobuco-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.5.tar", last modified: Thu May  4 09:36:08 2023, max compression
+gzip compressed data, was "nobuco-0.4.6.tar", last modified: Wed May 17 10:53:17 2023, max compression
```

## Comparing `nobuco-0.4.5.tar` & `nobuco-0.4.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.662879 nobuco-0.4.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.5/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22073 2023-05-04 09:36:08.662879 nobuco-0.4.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20239 2023-05-04 09:35:08.000000 nobuco-0.4.5/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.658878 nobuco-0.4.5/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.5/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.658878 nobuco-0.4.5/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.658878 nobuco-0.4.5/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.658878 nobuco-0.4.5/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.658878 nobuco-0.4.5/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.662879 nobuco-0.4.5/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.5/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.5/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.5/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11116 2023-05-04 09:33:42.000000 nobuco-0.4.5/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-01 14:05:35.000000 nobuco-0.4.5/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10637 2023-05-01 11:14:44.000000 nobuco-0.4.5/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.662879 nobuco-0.4.5/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.662879 nobuco-0.4.5/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.5/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:36:08.658878 nobuco-0.4.5/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22073 2023-05-04 09:36:08.000000 nobuco-0.4.5/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-05-04 09:36:08.000000 nobuco-0.4.5/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-04 09:36:08.000000 nobuco-0.4.5/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-05-04 09:36:08.000000 nobuco-0.4.5/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-05-04 09:36:08.000000 nobuco-0.4.5/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-05-04 09:35:54.000000 nobuco-0.4.5/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-04 09:36:08.662879 nobuco-0.4.5/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.6/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-05-17 10:53:17.679828 nobuco-0.4.6/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.6/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.6/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.6/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.6/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.6/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.6/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11116 2023-05-04 09:33:42.000000 nobuco-0.4.6/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.6/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.6/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-16 10:06:21.000000 nobuco-0.4.6/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-05-17 10:49:15.000000 nobuco-0.4.6/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-05-17 10:51:39.000000 nobuco-0.4.6/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-17 10:53:17.679828 nobuco-0.4.6/setup.cfg
```

### Comparing `nobuco-0.4.5/LICENSE` & `nobuco-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/PKG-INFO` & `nobuco-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.5
+Version: 0.4.6
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,15 @@
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
-<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch">
-<img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
+<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch"> <img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
 ```bash
 pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
@@ -547,15 +546,15 @@
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
 and there's a utility function to help you find what you need:
 
 
 ```python
 node = torch.Tensor.repeat
 # node = F.relu_
-# node = nn.Conv2d
+# node = nn.LSTM
 
 location_link, source_code = nobuco.locate_converter(node)
 print('Converter location:')
 print(location_link)
 print('Converter source code:')
 print(source_code)
 ```
```

### Comparing `nobuco-0.4.5/README.md` & `nobuco-0.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
-<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch">
-<img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
+<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch"> <img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
 ```bash
 pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
@@ -511,15 +510,15 @@
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
 and there's a utility function to help you find what you need:
 
 
 ```python
 node = torch.Tensor.repeat
 # node = F.relu_
-# node = nn.Conv2d
+# node = nn.LSTM
 
 location_link, source_code = nobuco.locate_converter(node)
 print('Converter location:')
 print(location_link)
 print('Converter source code:')
 print(source_code)
 ```
```

### Comparing `nobuco-0.4.5/nobuco/__init__.py` & `nobuco-0.4.6/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/commons.py` & `nobuco-0.4.6/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/convert.py` & `nobuco-0.4.6/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/converters/channel_ordering.py` & `nobuco-0.4.6/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/converters/node_converter.py` & `nobuco-0.4.6/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/converters/tensor.py` & `nobuco-0.4.6/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/converters/type_cast.py` & `nobuco-0.4.6/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/converters/validation.py` & `nobuco-0.4.6/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/entity/keras.py` & `nobuco-0.4.6/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/entity/pytorch.py` & `nobuco-0.4.6/nobuco/entity/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import inspect
 import time
 from typing import Collection, List
 
 import torch
 from nobuco.locate.link import get_link_to_obj
 from torch import nn
```

### Comparing `nobuco-0.4.5/nobuco/funcs.py` & `nobuco-0.4.6/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/layers/channel_order.py` & `nobuco-0.4.6/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/layers/container.py` & `nobuco-0.4.6/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/layers/weight.py` & `nobuco-0.4.6/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/locate/link.py` & `nobuco-0.4.6/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/locate/locate.py` & `nobuco-0.4.6/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/activation.py` & `nobuco-0.4.6/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/boolean.py` & `nobuco-0.4.6/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.6/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/comparison.py` & `nobuco-0.4.6/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/convolution.py` & `nobuco-0.4.6/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/dropout.py` & `nobuco-0.4.6/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/interpolation.py` & `nobuco-0.4.6/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/linear.py` & `nobuco-0.4.6/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/math.py` & `nobuco-0.4.6/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/misc.py` & `nobuco-0.4.6/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/normalization.py` & `nobuco-0.4.6/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/padding.py` & `nobuco-0.4.6/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/pooling.py` & `nobuco-0.4.6/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/recurrent.py` & `nobuco-0.4.6/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/slice.py` & `nobuco-0.4.6/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.6/nobuco/node_converters/tensor_cast.py`

 * *Files 20% similar despite different names*

```diff
@@ -52,19 +52,39 @@
 
 
 @converter(torch.Tensor.type, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_type(self, dtype=None, non_blocking=False, **kwargs):
     return type_func
 
 
+@converter(torch.Tensor.bool, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_bool(self, memory_format=None):
+    return lambda x: type_func(x, dtype=torch.bool)
+
+
+@converter(torch.Tensor.int, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_int(self, memory_format=None):
+    return lambda x: type_func(x, dtype=torch.int32)
+
+
+@converter(torch.Tensor.long, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_long(self, memory_format=None):
+    return lambda x: type_func(x, dtype=torch.int64)
+
+
 @converter(torch.Tensor.float, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_type(self, memory_format=None):
+def converter_float(self, memory_format=None):
     return lambda x: type_func(x, dtype=torch.float32)
 
 
+@converter(torch.Tensor.double, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_double(self, memory_format=None):
+    return lambda x: type_func(x, dtype=torch.float64)
+
+
 @converter(torch.Tensor.to, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_to(self, device=None, dtype=None, non_blocking=False, copy=False, memory_format=torch.preserve_format):
     def func(self, device=None, dtype=None, non_blocking=False, copy=False, memory_format=torch.preserve_format):
         if dtype is not None:
             return type_func(self, dtype=dtype, non_blocking=non_blocking)
         elif isinstance(device, torch._C.dtype):
             return type_func(self, dtype=device, non_blocking=non_blocking)
```

### Comparing `nobuco-0.4.5/nobuco/node_converters/tensor_creation.py` & `nobuco-0.4.6/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.6/nobuco/node_converters/tensor_manipulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,26 +270,37 @@
             x = _permute(perm)(x)
         x = tf.expand_dims(x, axis=dim)
         x = set_channel_order(x, ChannelOrder.PYTORCH)
         return x
     return func
 
 
-# @converter(torch.Tensor.unfold, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
-# def converter_unfold(self, dimension, size, step):
-#     n_dims = self.dim()
-#
-#     def func(self, dimension, size, step):
-#         sizes = [1]*n_dims
-#         strides = [1]*n_dims
-#         rates = [1]*n_dims
-#
-#         sizes[dimension] = size
-#         strides[dimension] = step
-#         x = self
-#         x = tf.image.extract_patches(x, sizes=sizes, strides=strides, rates=rates, padding='VALID')
-#
-#         b, c, h, w = x.shape
-#         x = tf.reshape(x, shape=[b, c, h, size, -1])
-#         x = tf.transpose(x, (0, 1, 2, 4, 3))
-#         return x
-#     return func
+def torch_gather(x, indices, gather_axis):
+    """
+    See: https://stackoverflow.com/a/71037111/4850610
+    """
+
+    all_indices = tf.where(tf.fill(indices.shape, True))
+    gather_locations = tf.reshape(indices, [indices.shape.num_elements()])
+
+    gather_indices = []
+    for axis in range(len(indices.shape)):
+        if axis == gather_axis:
+            gather_indices.append(tf.cast(gather_locations, dtype=tf.int64))
+        else:
+            gather_indices.append(tf.cast(all_indices[:, axis], dtype=tf.int64))
+
+    gather_indices = tf.stack(gather_indices, axis=-1)
+    gathered = tf.gather_nd(x, gather_indices)
+    reshaped = tf.reshape(gathered, indices.shape)
+    return reshaped
+
+
+@converter(torch.gather, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_gather(input: Tensor, dim, index: Tensor, *, sparse_grad: _bool=False, out: Optional[Tensor]=None):
+    n_dims = input.dim()
+
+    def func(input, dim, index, *, sparse_grad=False, out=None):
+        if get_channel_order(input) == ChannelOrder.TENSORFLOW:
+            dim = dim_pytorch2keras(dim, n_dims)
+        return torch_gather(input, index, dim)
+    return func
```

### Comparing `nobuco-0.4.5/nobuco/trace/tensor_storage.py` & `nobuco-0.4.6/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/trace/trace.py` & `nobuco-0.4.6/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/util.py` & `nobuco-0.4.6/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/vis/console_stylizer.py` & `nobuco-0.4.6/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco/vis/html_stylizer.py` & `nobuco-0.4.6/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.6/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.5
+Version: 0.4.6
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,15 @@
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
-<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch">
-<img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
+<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch"> <img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
 ```bash
 pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
@@ -547,15 +546,15 @@
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
 and there's a utility function to help you find what you need:
 
 
 ```python
 node = torch.Tensor.repeat
 # node = F.relu_
-# node = nn.Conv2d
+# node = nn.LSTM
 
 location_link, source_code = nobuco.locate_converter(node)
 print('Converter location:')
 print(location_link)
 print('Converter source code:')
 print(source_code)
 ```
```

### Comparing `nobuco-0.4.5/nobuco.egg-info/SOURCES.txt` & `nobuco-0.4.6/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.5/pyproject.toml` & `nobuco-0.4.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.5"
+version = "0.4.6"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

