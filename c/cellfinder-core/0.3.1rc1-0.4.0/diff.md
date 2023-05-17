# Comparing `tmp/cellfinder-core-0.3.1rc1.tar.gz` & `tmp/cellfinder-core-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-core-0.3.1rc1.tar", last modified: Tue Dec 13 10:56:48 2022, max compression
+gzip compressed data, was "cellfinder-core-0.4.0.tar", last modified: Wed May 17 09:39:26 2023, max compression
```

## Comparing `cellfinder-core-0.3.1rc1.tar` & `cellfinder-core-0.4.0.tar`

### file list

```diff
@@ -1,72 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.936524 cellfinder-core-0.3.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2022-12-13 10:56:48.936524 cellfinder-core-0.3.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-13 10:56:48.936524 cellfinder-core-0.3.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.920523 cellfinder-core-0.3.1rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.920523 cellfinder-core-0.3.1rc1/src/cellfinder_core/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.924523 cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    14993 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.924523 cellfinder-core-0.3.1rc1/src/cellfinder_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.924523 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.924523 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.928523 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1161992 2022-12-13 10:56:45.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/base_tile_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/base_tile_filter.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/setup_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/typedefs.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.932524 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1035849 2022-12-13 10:56:46.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/ball_filter.c
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/ball_filter.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1238960 2022-12-13 10:56:47.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/structure_detection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/structure_detection.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.932524 cellfinder-core-0.3.1rc1/src/cellfinder_core/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/download/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.936524 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/IO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.936524 cellfinder-core-0.3.1rc1/src/cellfinder_core/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2022-12-13 10:56:29.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core/train/train_yml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:56:48.924523 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2022-12-13 10:56:48.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2022-12-13 10:56:48.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 10:56:48.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-13 10:56:48.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 10:56:48.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      372 2022-12-13 10:56:48.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-13 10:56:48.000000 cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.721206 cellfinder-core-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.729206 cellfinder-core-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.github/workflows/test_numba_off.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.729206 cellfinder-core-0.4.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/detect_and_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/filter_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/filter_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/cell_detection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.721206 cellfinder-core-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.729206 cellfinder-core-0.4.0/src/cellfinder_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.733206 cellfinder-core-0.4.0/src/cellfinder_core/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.733206 cellfinder-core-0.4.0/src/cellfinder_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/src/cellfinder_core/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/src/cellfinder_core/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/src/cellfinder_core/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.733206 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-17 09:39:26.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/test_detection_structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.725206 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_tools_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tox.ini
```

### Comparing `cellfinder-core-0.3.1rc1/LICENSE` & `cellfinder-core-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/PKG-INFO` & `cellfinder-core-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cellfinder-core
-Version: 0.3.1rc1
+Version: 0.4.0
 Summary: Automated 3D cell detection in large microscopy images
-Home-page: https://brainglobe.info/cellfinder
-Author: Adam Tyson, Christian Niedworok, Charly Rousseau
-Author-email: code@adamltyson.com
+Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
+Project-URL: Homepage, https://brainglobe.info/cellfinder
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
 Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
 Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
@@ -74,15 +73,15 @@
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
 [here](https://docs.brainglobe.info/cellfinder/installation/using-gpu).
 
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
-[preprint](https://www.biorxiv.org/content/10.1101/2020.10.21.348771v2) which
+[paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
 command-line tool ([cell candidate detection](https://docs.brainglobe.info/cellfinder/user-guide/command-line/candidate-detection),
 [cell candidate classification](https://docs.brainglobe.info/cellfinder/user-guide/command-line/classification)).
 It may also be useful to try the
@@ -313,15 +312,15 @@
 **Cassified cell candidates. Yellow - cells, Blue - artefacts**
 
 ## Contributing
 Contributions to cellfinder-core are more than welcome. Please see the [contributing guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
 
 ---
 ## Citing cellfinder
-If you find this plugin useful, and use it in your research, please cite the preprint outlining the cell detection algorithm:
+If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
  [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-core-0.3.1rc1/README.md` & `cellfinder-core-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
 [here](https://docs.brainglobe.info/cellfinder/installation/using-gpu).
 
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
-[preprint](https://www.biorxiv.org/content/10.1101/2020.10.21.348771v2) which
+[paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
 command-line tool ([cell candidate detection](https://docs.brainglobe.info/cellfinder/user-guide/command-line/candidate-detection),
 [cell candidate classification](https://docs.brainglobe.info/cellfinder/user-guide/command-line/classification)).
 It may also be useful to try the
@@ -289,15 +289,15 @@
 **Cassified cell candidates. Yellow - cells, Blue - artefacts**
 
 ## Contributing
 Contributions to cellfinder-core are more than welcome. Please see the [contributing guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
 
 ---
 ## Citing cellfinder
-If you find this plugin useful, and use it in your research, please cite the preprint outlining the cell detection algorithm:
+If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
  [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/augment.py` & `cellfinder-core-0.4.0/src/cellfinder_core/classify/augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
             normalised_pixel_sizes,
             augmentation_parameters.interpolation_order,
         )
     return image
 
 
 def rescale_to_isotropic(image, relative_pixel_sizes, interpolation_order):
-
     if not all_elements_equal(relative_pixel_sizes):
         min_pixel_size = min(relative_pixel_sizes)
         normalised_pixel_sizes = []
         for pixel_size in relative_pixel_sizes:
             normalised_pixel_sizes.append(
                 round(pixel_size / min_pixel_size, 2)
             )
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/classify.py` & `cellfinder-core-0.4.0/src/cellfinder_core/classify/classify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import Callable, Optional
+from typing import Callable, List, Optional
 
 import numpy as np
 from imlib.general.system import get_num_processes
 from tensorflow import keras
 
-from cellfinder_core import logger
+from cellfinder_core import logger, types
 from cellfinder_core.classify.cube_generator import CubeGeneratorFromFile
 from cellfinder_core.classify.tools import get_model
 from cellfinder_core.train.train_yml import models
 
 
 def main(
     points,
-    signal_array,
-    background_array,
-    n_free_cpus,
+    signal_array: types.array,
+    background_array: types.array,
+    n_free_cpus: int,
     voxel_sizes,
     network_voxel_sizes,
     batch_size,
     cube_height,
     cube_width,
     cube_depth,
     trained_model,
     model_weights,
     network_depth,
     max_workers=3,
     *,
     callback: Optional[Callable[[int], None]] = None,
-):
+) -> List:
     """
     Parameters
     ----------
     callback : Callable[int], optional
         A callback function that is called during classification. Called with
         the batch number once that batch has been classified.
     """
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/cube_generator.py` & `cellfinder-core-0.4.0/src/cellfinder_core/classify/cube_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from random import shuffle
+from typing import Optional, Tuple
 
 import numpy as np
 import tensorflow as tf
 from imlib.cells.cells import group_cells_by_z
 from imlib.general.numerical import is_even
 from scipy.ndimage import zoom
 from skimage.io import imread
 from tensorflow.keras.utils import Sequence
 
+from cellfinder_core import types
 from cellfinder_core.classify.augment import AugmentationParameters, augment
 
 # TODO: rename, as now using dask arrays -
 #  actually should combine to one generator
 
 
 class StackSizeError(Exception):
@@ -29,34 +31,34 @@
 
     # TODO: shuffle within (and maybe between) batches
     # TODO: limit workers based on RAM
 
     def __init__(
         self,
         points,
-        signal_array,
-        background_array,
+        signal_array: types.array,
+        background_array: types.array,
         voxel_sizes,
         network_voxel_sizes,
-        batch_size=16,
-        cube_width=50,
-        cube_height=50,
-        cube_depth=20,
-        channels=2,  # No other option currently
-        classes=2,
-        extract=False,
-        train=False,
-        augment=False,
-        augment_likelihood=0.1,
-        flip_axis=[0, 1, 2],
-        rotate_max_axes=[1, 1, 1],  # degrees
+        batch_size: Optional[int] = 16,
+        cube_width: Optional[int] = 50,
+        cube_height: Optional[int] = 50,
+        cube_depth: Optional[int] = 20,
+        channels: Optional[int] = 2,  # No other option currently
+        classes: Optional[int] = 2,
+        extract: Optional[bool] = False,
+        train: Optional[bool] = False,
+        augment: Optional[bool] = False,
+        augment_likelihood: Optional[float] = 0.1,
+        flip_axis: Tuple[int, int, int] = (0, 1, 2),
+        rotate_max_axes: Tuple[float, float, float] = (1, 1, 1),  # degrees
         # scale=[0.5, 2],  # min, max
-        translate=[0.05, 0.05, 0.05],
-        shuffle=False,
-        interpolation_order=2,
+        translate: Tuple[float, float, float] = (0.05, 0.05, 0.05),
+        shuffle: Optional[bool] = False,
+        interpolation_order: Optional[int] = 2,
     ):
         self.points = points
         self.signal_array = signal_array
         self.background_array = background_array
         self.batch_size = batch_size
         self.axis_2_pixel_um = float(voxel_sizes[2])
         self.axis_1_pixel_um = float(voxel_sizes[1])
@@ -98,15 +100,15 @@
         self.__get_batches()
         if shuffle:
             self.on_epoch_end()
 
     def __check_image_sizes(self):
         if len(self.signal_array) != len(self.background_array):
             raise ValueError(
-                f"Number of signal images ({len(self.signal_array)} does not"
+                f"Number of signal images ({len(self.signal_array)}) does not "
                 f"match the number of background images "
                 f"({len(self.background_array)}"
             )
 
     def __get_image_size(self):
         self.image_z_size = len(self.signal_array)
         self.image_height, self.image_width = self.signal_array[0].shape
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/resnet.py` & `cellfinder-core-0.4.0/src/cellfinder_core/classify/resnet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from typing import Dict, List, Literal, Tuple, Union
+
 from tensorflow.keras import Model
+from tensorflow.keras.initializers import Initializer
 from tensorflow.keras.layers import (
     Activation,
     Add,
     BatchNormalization,
     Conv3D,
     Dense,
     GlobalAveragePooling3D,
@@ -11,58 +14,48 @@
     ZeroPadding3D,
 )
 from tensorflow.keras.optimizers import Adam
 
 #####################################################################
 # Define the types of ResNet
 
-resnet_unit_blocks = {
+layer_type = Literal[
+    "18-layer", "34-layer", "50-layer", "101-layer", "152-layer"
+]
+
+resnet_unit_blocks: Dict[layer_type, List[int]] = {
     "18-layer": [2, 2, 2, 2],
     "34-layer": [3, 4, 6, 3],
     "50-layer": [3, 4, 6, 3],
     "101-layer": [3, 4, 23, 3],
     "152-layer": [3, 6, 36, 3],
 }
 
-network_residual_bottleneck = {
+network_residual_bottleneck: Dict[layer_type, bool] = {
     "18-layer": False,
     "34-layer": False,
     "50-layer": True,
     "101-layer": True,
     "152-layer": True,
 }
 #####################################################################
 
 
 def build_model(
-    shape=(50, 50, 20, 2),
-    network_depth="18-layer",
+    shape: Tuple[int, int, int, int] = (50, 50, 20, 2),
+    network_depth: layer_type = "18-layer",
     optimizer=None,
-    learning_rate=0.0005,  # higher rates don't always converge
+    learning_rate: float = 0.0005,  # higher rates don't always converge
     loss="categorical_crossentropy",
     metrics=["accuracy"],
-    number_classes=2,
-    axis=3,
-    starting_features=64,
+    number_classes: int = 2,
+    axis: int = 3,
+    starting_features: int = 64,
     classification_activation="softmax",
-):
-    """
-
-    :param shape:
-    :param network_depth:
-    :param optimizer:
-    :param learning_rate:
-    :param loss:
-    :param metrics:
-    :param number_classes:
-    :param int axis: Default: 3. Assumed channels are last
-    :param starting_features: # increases in each set of residual units
-    :param classification_activation:
-    :return:
-    """
+) -> Model:
     blocks, bottleneck = get_resnet_blocks_and_bottleneck(network_depth)
 
     inputs = Input(shape)
     x = non_residual_block(inputs, starting_features, axis=axis)
 
     features = starting_features
     for resnet_unit_id, iterations in enumerate(blocks):
@@ -90,15 +83,15 @@
     if optimizer is None:
         optimizer = Adam(learning_rate=learning_rate)
 
     model.compile(optimizer, loss=loss, metrics=metrics)
     return model
 
 
-def get_resnet_blocks_and_bottleneck(network_depth):
+def get_resnet_blocks_and_bottleneck(network_depth: layer_type):
     """
     Parses dicts, and returns how many resnet blocks are in each unit, along
     with whether they are bottlneck blocks or not
 
     :param network_depth:
     :return:
     """
@@ -167,15 +160,14 @@
     bottleneck=False,
     activation="relu",
     use_bias=False,
     kernel_initializer="he_normal",
     bn_epsilon=1e-5,
     axis=3,
 ):
-
     """
     Residual unit from He et al. (2015)
 
 
     :param int output_features: How many output features
     :param int resnet_unit_id: Which resnet unit
     (e.g. 0 is conv2_x, 1 is conv3_x)
@@ -301,24 +293,23 @@
         return y
 
     return f
 
 
 def get_shortcut(
     inputs,
-    resnet_unit_label,
-    block_id,
-    features,
-    stride,
-    use_bias=False,
-    kernel_initializer="he_normal",
-    bn_epsilon=1e-5,
-    axis=3,
+    resnet_unit_label: int,
+    block_id: int,
+    features: int,
+    stride: int,
+    use_bias: bool = False,
+    kernel_initializer: Union[str, Initializer] = "he_normal",
+    bn_epsilon: float = 1e-5,
+    axis: int = 3,
 ):
-
     """
     Create shortcut. For none-bottleneck residual units, this is just the
     identity. Otherwise, the input is reshaped to match the output of the
     bottleneck unit
 
     :param inputs: Input to the residual unit
     :param int resnet_unit_label: Which resnet unit (i.e. 2 is conv2_x)
@@ -349,15 +340,15 @@
             name=f"resunit{resnet_unit_label}_block{block_id}_shortcut_bn",
         )(shortcut)
         return shortcut
     else:
         return inputs
 
 
-def get_stride(resnet_unit_id, block_id):
+def get_stride(resnet_unit_id: int, block_id: int) -> int:
     """
     Determines the convolution stride.
 
     :param int resnet_unit_id: Which resnet unit
     (e.g. 0 is conv2_x, 1 is conv3_x)
     :param int block_id: Which block in the resnet unit (i.e. in the third
     unit of a 152-layer resnet, block_id=36)
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/classify/tools.py` & `cellfinder-core-0.4.0/src/cellfinder_core/classify/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import os
+from typing import Optional
+
 import numpy as np
 import tensorflow as tf
 
 from cellfinder_core import logger
 from cellfinder_core.classify.resnet import build_model
 
 
 def get_model(
-    existing_model=None,
-    model_weights=None,
+    existing_model: Optional[os.PathLike] = None,
+    model_weights: Optional[os.PathLike] = None,
     network_depth=None,
     learning_rate=0.0001,
     inference=False,
     continue_training=False,
 ):
     """
     Returns the correct model based on the arguments passed
@@ -44,15 +47,14 @@
             if model_weights is None:
                 raise IOError("`model_weights` must be provided")
             model.load_weights(model_weights)
         return model
 
 
 def make_lists(tiff_files, train=True):
-
     signal_list = []
     background_list = []
     if train:
         labels = []
 
     for group in tiff_files:
         for image in group:
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/plane/classical_filter.py` & `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/classical_filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 from scipy.ndimage import gaussian_filter, laplace
 from scipy.signal import medfilt2d
 
 
-def enhance_peaks(img, clipping_value, gaussian_sigma=2.5):
+def enhance_peaks(
+    img: np.ndarray, clipping_value: float, gaussian_sigma: float = 2.5
+) -> np.ndarray:
     type_in = img.dtype
     filtered_img = medfilt2d(img.astype(np.float64))
     filtered_img = gaussian_filter(filtered_img, gaussian_sigma)
     filtered_img = laplace(filtered_img)
     filtered_img *= -1
 
     filtered_img -= filtered_img.min()
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/structure_splitting.py` & `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+from typing import List, Tuple
+
 import numpy as np
 
 from cellfinder_core import logger
 from cellfinder_core.detect.filters.volume.ball_filter import BallFilter
 from cellfinder_core.detect.filters.volume.structure_detection import (
     CellDetector,
-    get_structure_centre_wrapper,
+    get_structure_centre,
 )
 
 
 class StructureSplitException(Exception):
     pass
 
 
-def get_shape(xs, ys, zs):
+def get_shape(xs: np.ndarray, ys: np.ndarray, zs: np.ndarray) -> List[int]:
     # +1 because difference. TEST:
     shape = [int((dim.max() - dim.min()) + 1) for dim in (xs, ys, zs)]
     return shape
 
 
-def coords_to_volume(xs, ys, zs, ball_radius=1):
+def coords_to_volume(
+    xs: np.ndarray, ys: np.ndarray, zs: np.ndarray, ball_radius: int = 1
+) -> np.ndarray:
     ball_diameter = ball_radius * 2
     # Expanded to ensure the ball fits even at the border
     expanded_shape = [
         dim_size + ball_diameter for dim_size in get_shape(xs, ys, zs)
     ]
     volume = np.zeros(expanded_shape, dtype=np.uint16)
 
@@ -35,51 +39,60 @@
     # OPTIMISE: vectorize
     for rel_x, rel_y, rel_z in zip(relative_xs, relative_ys, relative_zs):
         volume[rel_x, rel_y, rel_z] = 65534
     return volume
 
 
 def ball_filter_imgs(
-    volume, threshold_value, soma_centre_value, ball_xy_size=3, ball_z_size=3
-):
+    volume: np.ndarray,
+    threshold_value: int,
+    soma_centre_value: int,
+    ball_xy_size: int = 3,
+    ball_z_size: int = 3,
+) -> Tuple[np.ndarray, np.ndarray]:
     # OPTIMISE: reuse ball filter instance
 
-    good_tiles_mask = np.ones((1, 1, volume.shape[2]), dtype=np.uint8)
+    good_tiles_mask = np.ones((1, 1, volume.shape[2]), dtype=bool)
 
-    layer_width, layer_height = volume.shape[:2]
+    plane_width, plane_height = volume.shape[:2]
 
     bf = BallFilter(
-        layer_width,
-        layer_height,
+        plane_width,
+        plane_height,
         ball_xy_size,
         ball_z_size,
         overlap_fraction=0.8,
-        tile_step_width=layer_width,
-        tile_step_height=layer_height,
+        tile_step_width=plane_width,
+        tile_step_height=plane_height,
         threshold_value=threshold_value,
         soma_centre_value=soma_centre_value,
     )
     cell_detector = CellDetector(
-        layer_width, layer_height, start_z=ball_z_size // 2
+        plane_width, plane_height, start_z=ball_z_size // 2
     )
 
     # FIXME: hard coded type
     ball_filtered_volume = np.zeros(volume.shape, dtype=np.uint16)
+    previous_plane = None
     for z in range(volume.shape[2]):
         bf.append(volume[:, :, z].astype(np.uint16), good_tiles_mask[:, :, z])
         if bf.ready:
             bf.walk()
             middle_plane = bf.get_middle_plane()
             ball_filtered_volume[:, :, z] = middle_plane[:]
             # DEBUG: TEST: transpose
-            cell_detector.process(middle_plane.copy())
+            previous_plane = cell_detector.process(
+                middle_plane.copy(), previous_plane
+            )
     return ball_filtered_volume, cell_detector.get_cell_centres()
 
 
-def iterative_ball_filter(volume, n_iter=10):
+def iterative_ball_filter(
+    volume: np.ndarray, n_iter: int = 10
+) -> Tuple[List[int], List[np.ndarray]]:
     ns = []
     centres = []
 
     threshold_value = 65534
     soma_centre_value = 65535
 
     vol = volume.copy()  # TODO: check if required
@@ -93,76 +106,83 @@
         ns.append(n_structures)
         centres.append(cell_centres)
         if n_structures == 0:
             break
     return ns, centres
 
 
-def check_centre_in_cuboid(centre, max_coords):
+def check_centre_in_cuboid(centre: np.ndarray, max_coords: np.ndarray) -> bool:
     """
     Checks whether a coordinate is in a cuboid
     :param centre: x,y,z coordinate
     :param max_coords: far corner of cuboid
     :return: True if within cuboid, otherwise False
     """
-    relative_coords = np.array([centre[k] for k in ("x", "y", "z")])
+    relative_coords = centre
     if (relative_coords > max_coords).all():
         logger.info(
             'Relative coordinates "{}" exceed maximum volume '
             'dimension of "{}"'.format(relative_coords, max_coords)
         )
         return False
     else:
         return True
 
 
-def split_cells(cell_points, outlier_keep=False):
-    orig_centre = get_structure_centre_wrapper(cell_points)
+def split_cells(
+    cell_points: np.ndarray, outlier_keep: bool = False
+) -> np.ndarray:
+    orig_centre = get_structure_centre(cell_points)
+
+    xs = cell_points[:, 0]
+    ys = cell_points[:, 1]
+    zs = cell_points[:, 2]
+
+    orig_corner = np.array(
+        [
+            orig_centre[0] - (orig_centre[0] - xs.min()),
+            orig_centre[1] - (orig_centre[1] - ys.min()),
+            orig_centre[2] - (orig_centre[2] - zs.min()),
+        ]
+    )
 
-    xs = np.array([p["x"] for p in cell_points])  # TODO: use dataframe
-    ys = np.array([p["y"] for p in cell_points])
-    zs = np.array([p["z"] for p in cell_points])
-
-    orig_corner = {
-        "x": orig_centre["x"] - (orig_centre["x"] - xs.min()),
-        "y": orig_centre["y"] - (orig_centre["y"] - ys.min()),
-        "z": orig_centre["z"] - (orig_centre["z"] - zs.min()),
-    }
-    relative_orig_centre = {
-        k: orig_centre[k] - orig_corner[k] for k in ("x", "y", "z")
-    }
+    relative_orig_centre = np.array(
+        [
+            orig_centre[0] - orig_corner[0],
+            orig_centre[1] - orig_corner[1],
+            orig_centre[2] - orig_corner[2],
+        ]
+    )
 
     original_bounding_cuboid_shape = get_shape(xs, ys, zs)
 
     ball_radius = 1
     vol = coords_to_volume(xs, ys, zs, ball_radius=ball_radius)
 
-    # centres is a list of lists of centres (1 list of centres per ball run)
+    # centres is a list of arrays of centres (1 array of centres per ball run)
     ns, centres = iterative_ball_filter(vol)
     ns.insert(0, 1)
-    centres.insert(0, [relative_orig_centre])
+    centres.insert(0, np.array([relative_orig_centre]))
 
     best_iteration = ns.index(max(ns))
 
     # TODO: put constraint on minimum centres distance ?
     relative_centres = centres[best_iteration]
 
     if not outlier_keep:
         # TODO: change to checking whether in original cluster shape
         original_max_coords = np.array(original_bounding_cuboid_shape)
-        relative_centres = [
-            x
-            for x in relative_centres
-            if check_centre_in_cuboid(x, original_max_coords)
-        ]
+        relative_centres = np.array(
+            [
+                x
+                for x in relative_centres
+                if check_centre_in_cuboid(x, original_max_coords)
+            ]
+        )
 
-    absolute_centres = []
+    absolute_centres = np.empty((len(relative_centres), 3))
     # FIXME: extract functionality
-    for relative_centre in relative_centres:
-        absolute_centre = {
-            "x": orig_corner["x"] + relative_centre["x"],
-            "y": orig_corner["y"] + relative_centre["y"],
-            "z": orig_corner["z"] + relative_centre["z"],
-        }
-        absolute_centres.append(absolute_centre)
+    absolute_centres[:, 0] = orig_corner[0] + relative_centres[:, 0]
+    absolute_centres[:, 1] = orig_corner[1] + relative_centres[:, 1]
+    absolute_centres[:, 2] = orig_corner[2] + relative_centres[:, 2]
 
-        return absolute_centres
+    return absolute_centres
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/detect/filters/volume/volume_filter.py` & `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/volume_filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,139 +1,163 @@
 import math
 import os
 from queue import Queue
-from typing import Callable, Optional, Sequence
+from threading import Lock
+from typing import Any, Callable, List, Optional, Tuple
 
+import numpy as np
 from imlib.cells.cells import Cell
 from tifffile import tifffile
 from tqdm import tqdm
 
 from cellfinder_core import logger
-from cellfinder_core.detect.filters.setup_filters import setup
+from cellfinder_core.detect.filters.setup_filters import (
+    get_ball_filter,
+    get_cell_detector,
+)
 from cellfinder_core.detect.filters.volume.structure_detection import (
-    get_structure_centre_wrapper,
+    get_structure_centre,
 )
 from cellfinder_core.detect.filters.volume.structure_splitting import (
     StructureSplitException,
     split_cells,
 )
 
 
 class VolumeFilter(object):
     def __init__(
         self,
         *,
         soma_diameter: float,
         soma_size_spread_factor: float = 1.4,
-        setup_params: Sequence,
-        planes_paths_range: Sequence,
+        setup_params: Tuple[np.ndarray, Any, int, int, float, Any],
+        n_planes: int,
+        n_locks_release: int,
         save_planes: bool = False,
         plane_directory: Optional[str] = None,
         start_plane: int = 0,
         max_cluster_size: int = 5000,
         outlier_keep: bool = False,
         artifact_keep: bool = True,
     ):
         self.soma_diameter = soma_diameter
         self.soma_size_spread_factor = soma_size_spread_factor
-        self.planes_paths_range = planes_paths_range
+        self.n_planes = n_planes
         self.z = start_plane
         self.save_planes = save_planes
         self.plane_directory = plane_directory
         self.max_cluster_size = max_cluster_size
         self.outlier_keep = outlier_keep
+        self.n_locks_release = n_locks_release
 
         self.artifact_keep = artifact_keep
 
         self.clipping_val = None
         self.threshold_value = None
         self.setup_params = setup_params
 
-        self.ball_filter, self.cell_detector = setup(
-            self.setup_params[0],
-            self.setup_params[1],
-            self.setup_params[2],
-            self.setup_params[3],
+        self.previous_plane: Optional[np.ndarray] = None
+
+        self.ball_filter = get_ball_filter(
+            plane=self.setup_params[0],
+            soma_diameter=self.setup_params[1],
+            ball_xy_size=self.setup_params[2],
+            ball_z_size=self.setup_params[3],
             ball_overlap_fraction=self.setup_params[4],
+        )
+
+        self.cell_detector = get_cell_detector(
+            plane_shape=self.setup_params[0].shape,  # type: ignore
+            ball_z_size=self.setup_params[3],
             z_offset=self.setup_params[5],
         )
 
     def process(
         self,
         async_result_queue: Queue,
+        locks: List[Lock],
         *,
         callback: Callable[[int], None],
-    ):
-        progress_bar = tqdm(
-            total=len(self.planes_paths_range), desc="Processing planes"
-        )
-        while not async_result_queue.empty():
+    ) -> List[Cell]:
+        progress_bar = tqdm(total=self.n_planes, desc="Processing planes")
+        for z in range(self.n_planes):
             # Get result from the queue.
             #
             # It is important to remove the result from the queue here
             # to free up memory once this plane has been processed by
             # the 3D filter here
+            logger.debug(f"🏐 Waiting for plane {z}")
             result = async_result_queue.get()
             # .get() blocks until the result is available
             plane, mask = result.get()
+            logger.debug(f"🏐 Got plane {z}")
 
-            logger.debug(f"Plane {self.z} received for 3D filtering")
-            print(f"Plane {self.z} received for 3D filtering")
-
-            logger.debug(f"Adding plane {self.z} for 3D filtering")
             self.ball_filter.append(plane, mask)
 
             if self.ball_filter.ready:
-                logger.debug(f"Ball filtering plane {self.z}")
-                self.ball_filter.walk()
+                # Let the next 2D filter run
+                z_release = z + self.n_locks_release + 1
+                if z_release < len(locks):
+                    logger.debug(f"🔓 Releasing lock for plane {z_release}")
+                    locks[z_release].release()
 
-                middle_plane = self.ball_filter.get_middle_plane()
-                if self.save_planes:
-                    self.save_plane(middle_plane)
-
-                logger.debug(f"Detecting structures for plane {self.z}")
-                self.cell_detector.process(middle_plane)
-
-                logger.debug(f"Structures done for plane {self.z}")
-                logger.debug(
-                    f"Skipping plane {self.z} for 3D filter" " (out of bounds)"
-                )
+                self._run_filter()
 
             callback(self.z)
             self.z += 1
             progress_bar.update()
 
         progress_bar.close()
         logger.debug("3D filter done")
         return self.get_results()
 
-    def save_plane(self, plane):
+    def _run_filter(self) -> None:
+        logger.debug(f"🏐 Ball filtering plane {self.z}")
+        self.ball_filter.walk()
+
+        middle_plane = self.ball_filter.get_middle_plane()
+        if self.save_planes:
+            self.save_plane(middle_plane)
+
+        logger.debug(f"🏫 Detecting structures for plane {self.z}")
+        self.previous_plane = self.cell_detector.process(
+            middle_plane, self.previous_plane
+        )
+
+        logger.debug(f"🏫 Structures done for plane {self.z}")
+
+    def save_plane(self, plane: np.ndarray) -> None:
+        if self.plane_directory is None:
+            raise ValueError(
+                "plane_directory must be set to save planes to file"
+            )
         plane_name = f"plane_{str(self.z).zfill(4)}.tif"
         f_path = os.path.join(self.plane_directory, plane_name)
         tifffile.imsave(f_path, plane.T)
 
-    def get_results(self):
+    def get_results(self) -> List[Cell]:
         logger.info("Splitting cell clusters and writing results")
 
         max_cell_volume = sphere_volume(
             self.soma_size_spread_factor * self.soma_diameter / 2
         )
 
         cells = []
-        for (
-            cell_id,
-            cell_points,
-        ) in self.cell_detector.get_coords_list().items():
+        for cell_id, cell_points in self.cell_detector.coords_maps.items():
             cell_volume = len(cell_points)
 
             if cell_volume < max_cell_volume:
-                cell_centre = get_structure_centre_wrapper(cell_points)
+                cell_centre = get_structure_centre(cell_points)
                 cells.append(
                     Cell(
-                        (cell_centre["x"], cell_centre["y"], cell_centre["z"]),
+                        (
+                            cell_centre[0],
+                            cell_centre[1],
+                            cell_centre[2],
+                        ),
                         Cell.UNKNOWN,
                     )
                 )
             else:
                 if cell_volume < self.max_cluster_size:
                     try:
                         cell_centres = split_cells(
@@ -143,32 +167,32 @@
                         raise StructureSplitException(
                             f"Cell {cell_id}, error; {err}"
                         )
                     for cell_centre in cell_centres:
                         cells.append(
                             Cell(
                                 (
-                                    cell_centre["x"],
-                                    cell_centre["y"],
-                                    cell_centre["z"],
+                                    cell_centre[0],
+                                    cell_centre[1],
+                                    cell_centre[2],
                                 ),
                                 Cell.UNKNOWN,
                             )
                         )
                 else:
-                    cell_centre = get_structure_centre_wrapper(cell_points)
+                    cell_centre = get_structure_centre(cell_points)
                     cells.append(
                         Cell(
                             (
-                                cell_centre["x"],
-                                cell_centre["y"],
-                                cell_centre["z"],
+                                cell_centre[0],
+                                cell_centre[1],
+                                cell_centre[2],
                             ),
                             Cell.ARTIFACT,
                         )
                     )
 
         return cells
 
 
-def sphere_volume(radius):
+def sphere_volume(radius: float) -> float:
     return (4 / 3) * math.pi * radius**3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/download/cli.py` & `cellfinder-core-0.4.0/src/cellfinder_core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/download/download.py` & `cellfinder-core-0.4.0/src/cellfinder_core/download/download.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/download/models.py` & `cellfinder-core-0.4.0/src/cellfinder_core/download/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from pathlib import Path
+from typing import Literal
 
 from cellfinder_core import logger
 from cellfinder_core.download.download import download
 
 model_weight_urls = {
     "resnet50_tv": "https://gin.g-node.org/cellfinder/models/raw/"
     "master/resnet50_tv.h5",
@@ -12,16 +13,18 @@
 }
 
 download_requirements_gb = {
     "resnet50_tv": 0.18,
     "resnet50_all": 0.18,
 }
 
+model_type = Literal["resnet50_tv", "resnet50_all"]
 
-def main(model_name: str, download_path: os.PathLike) -> Path:
+
+def main(model_name: model_type, download_path: os.PathLike) -> Path:
     """
     For a given model name and download path, download the model file
     and return the path to the downloaded file.
     """
     download_path = Path(download_path)
 
     model_weight_dir = download_path / "model_weights"
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/main.py` & `cellfinder-core-0.4.0/src/cellfinder_core/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 """
 N.B imports are within functions to prevent tensorflow being imported before
 it's warnings are silenced
 """
-
 import os
+from typing import Callable, Optional, Tuple
 
+import numpy as np
 from imlib.general.logging import suppress_specific_logs
 
 from cellfinder_core import logger
+from cellfinder_core.download.models import model_type
+from cellfinder_core.train.train_yml import depth_type
 
 tf_suppress_log_messages = [
     "multiprocessing can interact badly with TensorFlow"
 ]
 
 
 def main(
-    signal_array,
-    background_array,
-    voxel_sizes,
-    start_plane=0,
-    end_plane=-1,
-    trained_model=None,
-    model_weights=None,
-    model="resnet50_tv",
-    batch_size=32,
-    n_free_cpus=2,
-    network_voxel_sizes=[5, 1, 1],
-    soma_diameter=16,
-    ball_xy_size=6,
-    ball_z_size=15,
-    ball_overlap_fraction=0.6,
-    log_sigma_size=0.2,
-    n_sds_above_mean_thresh=10,
-    soma_spread_factor=1.4,
-    max_cluster_size=100000,
-    cube_width=50,
-    cube_height=50,
-    cube_depth=20,
-    network_depth="50",
+    signal_array: np.ndarray,
+    background_array: np.ndarray,
+    voxel_sizes: Tuple[int, int, int],
+    start_plane: int = 0,
+    end_plane: int = -1,
+    trained_model: Optional[os.PathLike] = None,
+    model_weights: Optional[os.PathLike] = None,
+    model: model_type = "resnet50_tv",
+    batch_size: int = 32,
+    n_free_cpus: int = 2,
+    network_voxel_sizes: Tuple[int, int, int] = (5, 1, 1),
+    soma_diameter: int = 16,
+    ball_xy_size: int = 6,
+    ball_z_size: int = 15,
+    ball_overlap_fraction: float = 0.6,
+    log_sigma_size: float = 0.2,
+    n_sds_above_mean_thresh: int = 10,
+    soma_spread_factor: float = 1.4,
+    max_cluster_size: int = 100000,
+    cube_width: int = 50,
+    cube_height: int = 50,
+    cube_depth: int = 20,
+    network_depth: depth_type = "50",
     *,
-    detect_callback=None,
-    classify_callback=None,
-    detect_finished_callback=None,
+    detect_callback: Optional[Callable[[int], None]] = None,
+    classify_callback: Optional[Callable[[int], None]] = None,
+    detect_finished_callback: Optional[Callable[[list], None]] = None,
 ):
     """
     Parameters
     ----------
     detect_callback : Callable[int], optional
         Called every time a plane has finished being processed during the
         detection stage. Called with the plane number that has finished.
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/IO.py` & `cellfinder-core-0.4.0/src/cellfinder_core/tools/IO.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/image_processing.py` & `cellfinder-core-0.4.0/src/cellfinder_core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/prep.py` & `cellfinder-core-0.4.0/src/cellfinder_core/tools/prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DEFAULT_INSTALL_PATH = home / ".cellfinder"
 
 
 def prep_classification(
     trained_model: Optional[os.PathLike],
     model_weights: Optional[os.PathLike],
     install_path: Optional[os.PathLike],
-    model_name: str,
+    model_name: model_download.model_type,
     n_free_cpus: int,
 ) -> Path:
     n_processes = get_num_processes(min_free_cpu_cores=n_free_cpus)
     prep_tensorflow(n_processes)
     model_weights = prep_models(
         trained_model, model_weights, install_path, model_name
     )
@@ -37,15 +37,15 @@
 
 
 def prep_training(
     n_free_cpus: int,
     trained_model: Optional[os.PathLike],
     model_weights: Optional[os.PathLike],
     install_path: Optional[os.PathLike],
-    model_name: str,
+    model_name: model_download.model_type,
 ) -> Path:
     n_processes = get_num_processes(min_free_cpu_cores=n_free_cpus)
     prep_tensorflow(n_processes)
     model_weights = prep_models(
         trained_model, model_weights, install_path, model_name
     )
     return model_weights
@@ -56,15 +56,15 @@
     tf_tools.allow_gpu_memory_growth()
 
 
 def prep_models(
     trained_model_path: Optional[os.PathLike],
     model_weights_path: Optional[os.PathLike],
     install_path: Optional[os.PathLike],
-    model_name: str,
+    model_name: model_download.model_type,
 ) -> Path:
     install_path = install_path or DEFAULT_INSTALL_PATH
     # if no model or weights, set default weights
     if model_weights_path is None:
         logger.debug("No model supplied, so using the default")
 
         config_file = source_custom_config_cellfinder()
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/system.py` & `cellfinder-core-0.4.0/src/cellfinder_core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/tf.py` & `cellfinder-core-0.4.0/src/cellfinder_core/tools/tf.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/tiff.py` & `cellfinder-core-0.4.0/src/cellfinder_core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/tools/tools.py` & `cellfinder-core-0.4.0/src/cellfinder_core/tools/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from random import getrandbits, uniform
 
 import numpy as np
 from natsort import natsorted
 
 
-def get_max_value(obj_in: np.ndarray) -> int:
+def get_max_possible_value(obj_in: np.ndarray) -> int:
     """
     Returns the maximum allowed value for a numpy array of integer data type.
     """
     dtype = obj_in.dtype
     if np.issubdtype(dtype, np.integer):
         return np.iinfo(dtype).max
     else:
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core/train/train_yml.py` & `cellfinder-core-0.4.0/src/cellfinder_core/train/train_yml.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from argparse import (
     ArgumentDefaultsHelpFormatter,
     ArgumentParser,
     ArgumentTypeError,
 )
 from datetime import datetime
 from pathlib import Path
+from typing import Literal
 
 from fancylog import fancylog
 from imlib.general.numerical import check_positive_float, check_positive_int
 from imlib.general.system import ensure_directory_exists
 from imlib.IO.cells import find_relevant_tiffs
 from imlib.IO.yaml import read_yaml_section
 from sklearn.model_selection import train_test_split
@@ -37,14 +38,16 @@
     "18": "18-layer",
     "34": "34-layer",
     "50": "50-layer",
     "101": "101-layer",
     "152": "152-layer",
 }
 
+depth_type = Literal["18", "34", "50", "101", "152"]
+
 
 def valid_model_depth(depth):
     """
     Ensures a correct existing_model is chosen
     :param value: Input value
     :param models: Dict of allowed models
     :return: Input value, if it corresponds to a valid existing_model
@@ -309,15 +312,14 @@
     no_augment=False,
     tensorboard=False,
     save_weights=False,
     no_save_checkpoints=False,
     save_progress=False,
     epochs=100,
 ):
-
     from cellfinder_core.main import suppress_tf_logging
 
     suppress_tf_logging(tf_suppress_log_messages)
 
     from tensorflow.keras.callbacks import (
         CSVLogger,
         ModelCheckpoint,
```

### Comparing `cellfinder-core-0.3.1rc1/src/cellfinder_core.egg-info/PKG-INFO` & `cellfinder-core-0.4.0/src/cellfinder_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cellfinder-core
-Version: 0.3.1rc1
+Version: 0.4.0
 Summary: Automated 3D cell detection in large microscopy images
-Home-page: https://brainglobe.info/cellfinder
-Author: Adam Tyson, Christian Niedworok, Charly Rousseau
-Author-email: code@adamltyson.com
+Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
+Project-URL: Homepage, https://brainglobe.info/cellfinder
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
 Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
 Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
@@ -74,15 +73,15 @@
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
 [here](https://docs.brainglobe.info/cellfinder/installation/using-gpu).
 
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
-[preprint](https://www.biorxiv.org/content/10.1101/2020.10.21.348771v2) which
+[paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
 command-line tool ([cell candidate detection](https://docs.brainglobe.info/cellfinder/user-guide/command-line/candidate-detection),
 [cell candidate classification](https://docs.brainglobe.info/cellfinder/user-guide/command-line/classification)).
 It may also be useful to try the
@@ -313,15 +312,15 @@
 **Cassified cell candidates. Yellow - cells, Blue - artefacts**
 
 ## Contributing
 Contributions to cellfinder-core are more than welcome. Please see the [contributing guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
 
 ---
 ## Citing cellfinder
-If you find this plugin useful, and use it in your research, please cite the preprint outlining the cell detection algorithm:
+If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
  [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
```

