# Comparing `tmp/neuralhydrology-1.6.0.tar.gz` & `tmp/neuralhydrology-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralhydrology-1.6.0.tar", last modified: Tue Apr  4 07:51:59 2023, max compression
+gzip compressed data, was "neuralhydrology-1.7.0.tar", last modified: Wed May 17 12:27:12 2023, max compression
```

## Comparing `neuralhydrology-1.6.0.tar` & `neuralhydrology-1.7.0.tar`

### file list

```diff
@@ -1,85 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.327079 neuralhydrology-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-04 07:51:59.327079 neuralhydrology-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.311079 neuralhydrology-1.6.0/neuralhydrology/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.315079 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/basedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsaus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelscl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/caravan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/genericdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/hourlycamelsus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/lamah.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datasetzoo/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.315079 neuralhydrology-1.6.0/neuralhydrology/datautils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datautils/climateindices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datautils/dischargeinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datautils/pet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/datautils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.315079 neuralhydrology-1.6.0/neuralhydrology/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/evaluation/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/evaluation/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/evaluation/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.323079 neuralhydrology-1.6.0/neuralhydrology/modelzoo/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/arlstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/cudalstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/customlstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/ealstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/embcudalstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/fc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/gru.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/inputlayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/mclstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/mtslstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/odelstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/modelzoo/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/nh_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/nh_run_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.323079 neuralhydrology-1.6.0/neuralhydrology/training/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/basetrainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/umaltrainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.327079 neuralhydrology-1.6.0/neuralhydrology/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/configutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/nh_results_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/ratingcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/neuralhydrology/utils/samplingutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.311079 neuralhydrology-1.6.0/neuralhydrology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-04 07:51:59.000000 neuralhydrology-1.6.0/neuralhydrology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-04 07:51:59.000000 neuralhydrology-1.6.0/neuralhydrology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:51:59.000000 neuralhydrology-1.6.0/neuralhydrology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-04 07:51:59.000000 neuralhydrology-1.6.0/neuralhydrology.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-04 07:51:59.000000 neuralhydrology-1.6.0/neuralhydrology.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 07:51:59.000000 neuralhydrology-1.6.0/neuralhydrology.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:51:59.327079 neuralhydrology-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:51:59.327079 neuralhydrology-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/test/test_config_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/test/test_custom_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/test/test_datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-04 07:51:50.000000 neuralhydrology-1.6.0/test/test_mclstm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.620346 neuralhydrology-1.7.0/neuralhydrology/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.624346 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/basedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsaus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelscl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/caravan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/genericdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/hourlycamelsus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/lamah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datasetzoo/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.624346 neuralhydrology-1.7.0/neuralhydrology/datautils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/climateindices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/dischargeinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/pet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/datautils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.624346 neuralhydrology-1.7.0/neuralhydrology/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26358 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/neuralhydrology/modelzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/arlstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/cudalstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/customlstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/ealstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/embcudalstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/inputlayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/mclstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/mtslstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/odelstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/modelzoo/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/nh_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/nh_run_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/neuralhydrology/training/
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/basetrainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/neuralhydrology/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/configutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/nh_results_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/ratingcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30861 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/neuralhydrology/utils/samplingutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.620346 neuralhydrology-1.7.0/neuralhydrology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 12:27:12.000000 neuralhydrology-1.7.0/neuralhydrology.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:27:12.632346 neuralhydrology-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:27:12.628346 neuralhydrology-1.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_config_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_custom_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-17 12:27:02.000000 neuralhydrology-1.7.0/test/test_mclstm.py
```

### Comparing `neuralhydrology-1.6.0/LICENSE` & `neuralhydrology-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/PKG-INFO` & `neuralhydrology-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralhydrology
-Version: 1.6.0
+Version: 1.7.0
 Summary: Library for training deep learning models with environmental focus
 Home-page: https://neuralhydrology.readthedocs.io
 Author: Frederik Kratzert, Daniel Klotz, Martin Gauch
 Author-email: neuralhydrology@googlegroups.com
 Project-URL: Documentation, https://neuralhydrology.readthedocs.io
 Project-URL: Source, https://github.com/neuralhydrology/neuralhydrology
 Project-URL: Research Blog, https://neuralhydrology.github.io/
```

### Comparing `neuralhydrology-1.6.0/README.md` & `neuralhydrology-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/__init__.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/basedataset.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/basedataset.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsaus.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsaus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsbr.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsbr.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelscl.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelscl.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsgb.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsgb.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/camelsus.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/camelsus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/caravan.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/caravan.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/genericdataset.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/genericdataset.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/hourlycamelsus.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/hourlycamelsus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/lamah.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/lamah.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datasetzoo/template.py` & `neuralhydrology-1.7.0/neuralhydrology/datasetzoo/template.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datautils/climateindices.py` & `neuralhydrology-1.7.0/neuralhydrology/datautils/climateindices.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datautils/dischargeinput.py` & `neuralhydrology-1.7.0/neuralhydrology/datautils/dischargeinput.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datautils/pet.py` & `neuralhydrology-1.7.0/neuralhydrology/datautils/pet.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/datautils/utils.py` & `neuralhydrology-1.7.0/neuralhydrology/datautils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,20 @@
     """
     native_frequency = pd.infer_freq(index)
     if native_frequency is None:
         raise ValueError(f'Cannot infer a legal frequency from dataset: {native_frequency}.')
     if native_frequency[0] not in '0123456789':  # add a value to the unit so to_timedelta works
         native_frequency = f'1{native_frequency}'
 
+    # pd.Timedelta doesn't understand weekly (W) frequencies, so we convert them to the equivalent multiple of 7D.
+    weekly_freq = re.match('(\d+)W(-(MON|TUE|WED|THU|FRI|SAT|SUN))?$', native_frequency)
+    if weekly_freq is not None:
+        n = int(weekly_freq[1]) * 7
+        native_frequency = f'{n}D'
+
     # Assert that the frequency corresponds to a positive time delta. We first add one offset to the base datetime
     # to make sure it's aligned with the frequency. Otherwise, adding an offset of e.g. 0Y would round up to the
     # nearest year-end, so we'd incorrectly miss a frequency of zero.
     base_datetime = pd.to_datetime('2001-01-01 00:00:00') + to_offset(native_frequency)
     if base_datetime >= base_datetime + to_offset(native_frequency):
         raise ValueError('Inferred dataset frequency is zero or negative.')
     return native_frequency
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology/evaluation/__init__.py` & `neuralhydrology-1.7.0/neuralhydrology/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/evaluation/evaluate.py` & `neuralhydrology-1.7.0/neuralhydrology/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/evaluation/metrics.py` & `neuralhydrology-1.7.0/neuralhydrology/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/evaluation/plots.py` & `neuralhydrology-1.7.0/neuralhydrology/evaluation/plots.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/evaluation/signatures.py` & `neuralhydrology-1.7.0/neuralhydrology/evaluation/signatures.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/evaluation/tester.py` & `neuralhydrology-1.7.0/neuralhydrology/evaluation/tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,14 +418,15 @@
         losses = []
         with torch.no_grad():
             for data in loader:
 
                 for key in data:
                     if not key.startswith('date'):
                         data[key] = data[key].to(self.device)
+                data = model.pre_model_hook(data, is_train=False)
                 predictions, loss = self._get_predictions_and_loss(model, data)
 
                 for freq in frequencies:
                     if predict_last_n[freq] == 0:
                         continue  # no predictions for this frequency
                     freq_key = '' if len(frequencies) == 1 else f'_{freq}'
                     y_hat_sub, y_sub = self._subset_targets(model, data, predictions, predict_last_n[freq], freq_key)
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology/evaluation/utils.py` & `neuralhydrology-1.7.0/neuralhydrology/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/__init__.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/arlstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/arlstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/basemodel.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/basemodel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Optional, Callable
 
 import torch
 import torch.nn as nn
 
 from neuralhydrology.utils.config import Config
-from neuralhydrology.utils.samplingutils import sample_pointpredictions
+from neuralhydrology.utils.samplingutils import sample_pointpredictions, umal_extend_batch
 
 
 class BaseModel(nn.Module):
     """Abstract base model class, don't use this class for model training.
 
     Use subclasses of this class for training/evaluating different models, e.g. use `CudaLSTM` for training a standard
     LSTM model or `EA-LSTM` for training an Entity-Aware-LSTM. Refer to  :doc:`Documentation/Modelzoo </usage/models>` 
@@ -65,7 +65,31 @@
 
         Returns
         -------
         Dict[str, torch.Tensor]
             Model output and potentially any intermediate states and activations as a dictionary.
         """
         raise NotImplementedError
+    
+    def pre_model_hook(self, data: Dict[str, torch.Tensor], is_train: bool) -> Dict[str, torch.Tensor]:
+        """A function to execute before the model in training, validaton and test. 
+        The beahvior can be adapted depending on the run configuration and the provided arguments.
+
+        Parameters
+        ----------
+        data : Dict[str, torch.Tensor]
+            Dictionary, containing input features as key-value pairs and labels y.
+        is_train : bool
+            Defines if the hook is executed in train mode or in validation/test mode.
+
+        Returns
+        -------
+        data : Dict[str, torch.Tensor]
+            The modified (or unmodified) data that are used for the training or evaluation.
+        """
+        if self.cfg.head.lower() == "umal":
+            data = umal_extend_batch(data, self.cfg, n_taus=self.cfg.n_taus, extend_y=True)
+        else:
+            # here one can implement additional pre model hooks
+            pass 
+
+        return data
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/cudalstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/cudalstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/customlstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/customlstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/ealstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/ealstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/embcudalstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/embcudalstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/fc.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/fc.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/gru.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/gru.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/head.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/head.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/inputlayer.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/inputlayer.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/mclstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/mclstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/mtslstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/mtslstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/odelstm.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/odelstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/template.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/template.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/modelzoo/transformer.py` & `neuralhydrology-1.7.0/neuralhydrology/modelzoo/transformer.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/nh_run.py` & `neuralhydrology-1.7.0/neuralhydrology/nh_run.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/nh_run_scheduler.py` & `neuralhydrology-1.7.0/neuralhydrology/nh_run_scheduler.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/training/__init__.py` & `neuralhydrology-1.7.0/neuralhydrology/training/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/training/basetrainer.py` & `neuralhydrology-1.7.0/neuralhydrology/training/basetrainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,16 +280,16 @@
         nan_count = 0
         for data in pbar:
 
             for key in data.keys():
                 if not key.startswith('date'):
                     data[key] = data[key].to(self.device)
 
-            # apply possible subclass pre-processing
-            data = self._pre_model_hook(data)
+            # apply possible pre-processing to the batch before the forward pass
+            data = self.model.pre_model_hook(data, is_train=True)
 
             # get predictions
             predictions = self.model(data)
 
             if self.noise_sampler_y is not None:
                 for key in filter(lambda k: 'y' in k, data.keys()):
                     noise = self.noise_sampler_y.sample(data[key].shape)
@@ -378,9 +378,7 @@
             self.cfg.train_dir.mkdir(parents=True)
         else:
             raise RuntimeError(f"There is already a folder at {self.cfg.run_dir}")
         if self.cfg.log_n_figures is not None:
             self.cfg.img_log_dir = self.cfg.run_dir / "img_log"
             self.cfg.img_log_dir.mkdir(parents=True)
 
-    def _pre_model_hook(self, data: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
-        return data
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology/training/logger.py` & `neuralhydrology-1.7.0/neuralhydrology/training/logger.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/training/loss.py` & `neuralhydrology-1.7.0/neuralhydrology/training/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,23 +356,23 @@
     eps : float, optional
         Small constant for numeric stability.
     """
 
     def __init__(self, cfg, eps: float = 1e-5):
         super(MaskedUMALLoss, self).__init__(cfg,
                                              prediction_keys=['mu', 'b'],
-                                             ground_truth_keys=['y', 'tau'],
+                                             ground_truth_keys=['y_extended', 'tau'],
                                              output_size_per_target=2)
         self.eps = eps
         self._n_taus_count = cfg.n_taus
         self._n_taus_log = torch.as_tensor(np.log(cfg.n_taus).astype('float32'))
 
     def _get_loss(self, prediction: Dict[str, torch.Tensor], ground_truth: Dict[str, torch.Tensor], **kwargs):
-        mask = ~torch.isnan(ground_truth['y']).any(1).any(1)
-        y = ground_truth['y'][mask]
+        mask = ~torch.isnan(ground_truth['y_extended']).any(1).any(1)
+        y = ground_truth['y_extended'][mask]
         t = ground_truth['tau'][mask]
         m = prediction['mu'][mask]
         b = prediction['b'][mask]
 
         # compute log likelihood
         error = y - m
         log_like = torch.log(t) + \
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology/training/regularization.py` & `neuralhydrology-1.7.0/neuralhydrology/training/regularization.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/training/train.py` & `neuralhydrology-1.7.0/neuralhydrology/training/train.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from neuralhydrology.training.basetrainer import BaseTrainer
-from neuralhydrology.training.umaltrainer import UMALTrainer
 from neuralhydrology.utils.config import Config
 
 
 def start_training(cfg: Config):
     """Start model training.
     
     Parameters
     ----------
     cfg : Config
         The run configuration.
 
     """
     # MC-LSTM is a special case, where the head returns an empty string but the model is trained as regression model.
-    if cfg.head.lower() in ['regression', 'gmm', 'cmal', '']:
+    if cfg.head.lower() in ['regression', 'gmm', 'umal', 'cmal', '']:
         trainer = BaseTrainer(cfg=cfg)
-    elif cfg.head.lower() == 'umal':
-        trainer = UMALTrainer(cfg=cfg)
     else:
         raise ValueError(f"Unknown head {cfg.head}.")
     trainer.initialize_training()
     trainer.train_and_validate()
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology/utils/config.py` & `neuralhydrology-1.7.0/neuralhydrology/utils/config.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/utils/configutils.py` & `neuralhydrology-1.7.0/neuralhydrology/utils/configutils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/utils/logging_utils.py` & `neuralhydrology-1.7.0/neuralhydrology/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/utils/nh_results_ensemble.py` & `neuralhydrology-1.7.0/neuralhydrology/utils/nh_results_ensemble.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/utils/ratingcurve.py` & `neuralhydrology-1.7.0/neuralhydrology/utils/ratingcurve.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/neuralhydrology/utils/samplingutils.py` & `neuralhydrology-1.7.0/neuralhydrology/utils/samplingutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import numpy as np
 from numba import njit
 import torch
 from torch.distributions import Categorical, Uniform
 
 from neuralhydrology.utils.config import Config
-from neuralhydrology.training.utils import umal_extend_batch
 
 
 def sample_pointpredictions(model: 'BaseModel', data: Dict[str, torch.Tensor],
                             n_samples: int) -> Dict[str, torch.Tensor]:
     """Point prediction samplers for the different uncertainty estimation approaches.
     
     This function provides different point sampling functions for the different uncertainty estimation approaches 
@@ -182,15 +181,15 @@
 
         # determine appropriate frequency suffix:
         if self.cfg.use_frequencies:
             self.freq_suffixes = [f'_{freq}' for freq in cfg.use_frequencies]
         else:
             self.freq_suffixes = ['']
 
-        self.batch_size_data = data[f'x_d{self.freq_suffixes[0]}'].shape[0]
+        self.batch_size_data = data[f'y{self.freq_suffixes[0]}'].shape[0]
 
     def _get_frequency_last_n(self, freq_suffix: str):
         if isinstance(self.predict_last_n, int):
             frequency_last_n = self.predict_last_n
         else:
             frequency_last_n = self.predict_last_n[freq_suffix[1:]]
         return frequency_last_n
@@ -482,15 +481,16 @@
     setup = _SamplingSetup(model, data, "umal")
 
     # force model into train mode if mc_dropout:
     if setup.mc_dropout:
         model.train()
 
     # n_taus expands the batch by itself and adds a sampled tau as input (new_batch_size = n_taus*batch_size):
-    data = umal_extend_batch(data, setup.cfg, n_taus=setup.cfg.n_taus)
+    if 'y_extended' not in data:
+        data = model.pre_model_hook(data, is_train=False)
 
     # make predictions:
     pred = model(data)
 
     # sample:
     samples = {}
     for freq_suffix in setup.freq_suffixes:
@@ -539,14 +539,74 @@
                     sample_points[mask_nan, -frequency_last_n:, nth_target, nth_sample] = values
 
         # add sample_points to dictionary of samples:
         freq_key = f'y_hat{freq_suffix}'
         samples.update({freq_key: sample_points})
     return samples
 
+def umal_extend_batch(data: Dict[str, torch.Tensor], cfg: Config, n_taus: int = 1, extend_y: bool = False) \
+        -> Dict[str, torch.Tensor]:
+    """This function extends the batch for the usage in UMAL (see: [#]_). 
+    
+    UMAL makes an MC approximation to a mixture integral by sampling random asymmetry parameters (tau). This can be 
+    parallelized by expanding the batch for each tau.  
+    
+    Parameters
+    ----------
+    data : Dict[str, torch.Tensor]
+        Dictionary, containing input features as key-value pairs.
+    cfg : Config
+        The run configuration.
+    n_taus : int
+        Number of taus to expand the batch.
+    extend_y : bool
+        Option to also extend the labels/y. 
+    
+    Returns
+    -------
+    Dict[str, torch.Tensor]
+        Dictionary, containing expanded input features and tau samples as key-value pairs.
+
+    References
+    ----------
+    .. [#] A. Brando, J. A. Rodriguez, J. Vitria, and A. R. Munoz: Modelling heterogeneous distributions 
+        with an Uncountable Mixture of Asymmetric Laplacians. Advances in Neural Information Processing Systems, 
+        pp. 8838-8848, 2019.
+    """
+    # setup:
+    if cfg.use_frequencies:
+        freq_suffixes = [f'_{freq}' for freq in cfg.use_frequencies]
+    else:
+        freq_suffixes = ['']
+
+    for freq_suffix in freq_suffixes:
+        batch_size, seq_length, input_size = data[f'x_d{freq_suffix}'].shape
+
+        if isinstance(cfg.predict_last_n, int):
+            predict_last_n = cfg.predict_last_n
+        else:
+            predict_last_n = cfg.predict_last_n[freq_suffix[1:]]
+
+        # sample tau within [tau_down, tau_up] and add to data:
+        tau = (cfg.tau_up - cfg.tau_down) * torch.rand(batch_size * n_taus, 1, 1) + cfg.tau_down
+        tau = tau.repeat(1, seq_length, 1)  # in our convention tau remains the same over all inputs
+        tau = tau.to(data[f'x_d{freq_suffix}'].device)
+        data[f'tau{freq_suffix}'] = tau[:, -predict_last_n:, :]
+
+        # extend dynamic inputs with tau and expand batch:
+        x_d = data[f'x_d{freq_suffix}'].repeat(n_taus, 1, 1)
+        data[f'x_d{freq_suffix}'] = torch.cat([x_d, tau], dim=-1)
+        data[f'y_extended{freq_suffix}'] = data[f'y{freq_suffix}'].repeat(n_taus, 1, 1)
+        if f'x_s{freq_suffix}' in data:
+            data[f'x_s{freq_suffix}'] = data[f'x_s{freq_suffix}'].repeat(n_taus, 1)
+        if f'x_one_hot{freq_suffix}' in data:
+            data[f'x_one_hot{freq_suffix}'] = data[f'x_one_hot{freq_suffix}'].repeat(n_taus, 1)
+
+    return data
+
 
 @njit
 def bernoulli_subseries_sampler(
     data: np.ndarray, 
     missing_fraction: float, 
     mean_missing_length: float,
     start_sampling_on: bool = True,
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology.egg-info/PKG-INFO` & `neuralhydrology-1.7.0/neuralhydrology.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralhydrology
-Version: 1.6.0
+Version: 1.7.0
 Summary: Library for training deep learning models with environmental focus
 Home-page: https://neuralhydrology.readthedocs.io
 Author: Frederik Kratzert, Daniel Klotz, Martin Gauch
 Author-email: neuralhydrology@googlegroups.com
 Project-URL: Documentation, https://neuralhydrology.readthedocs.io
 Project-URL: Source, https://github.com/neuralhydrology/neuralhydrology
 Project-URL: Research Blog, https://neuralhydrology.github.io/
```

### Comparing `neuralhydrology-1.6.0/neuralhydrology.egg-info/SOURCES.txt` & `neuralhydrology-1.7.0/neuralhydrology.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,14 @@
 neuralhydrology/modelzoo/transformer.py
 neuralhydrology/training/__init__.py
 neuralhydrology/training/basetrainer.py
 neuralhydrology/training/logger.py
 neuralhydrology/training/loss.py
 neuralhydrology/training/regularization.py
 neuralhydrology/training/train.py
-neuralhydrology/training/umaltrainer.py
-neuralhydrology/training/utils.py
 neuralhydrology/utils/__init__.py
 neuralhydrology/utils/config.py
 neuralhydrology/utils/configutils.py
 neuralhydrology/utils/errors.py
 neuralhydrology/utils/logging_utils.py
 neuralhydrology/utils/nh_results_ensemble.py
 neuralhydrology/utils/ratingcurve.py
```

### Comparing `neuralhydrology-1.6.0/setup.py` & `neuralhydrology-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/test/test_config_runs.py` & `neuralhydrology-1.7.0/test/test_config_runs.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/test/test_custom_lstm.py` & `neuralhydrology-1.7.0/test/test_custom_lstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.6.0/test/test_datautils.py` & `neuralhydrology-1.7.0/test/test_datautils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     pytest.raises(ValueError, sort_frequencies, ['1D', '1XYZ'])  # not a frequency
 
 
 def test_infer_frequency():
     """Test the logic to infer frequencies. """
     assert infer_frequency(pd.date_range('2000-01-01', '2000-01-10', freq='D')) == '1D'
     assert infer_frequency(pd.date_range('2000-01-01', '2000-01-10', freq='48H')) == '2D'
-    assert infer_frequency(pd.date_range('2000-01-01', '2000-03-01', freq='W-MON')) == '1W-MON'
+    assert infer_frequency(pd.date_range('2000-01-01', '2000-03-01', freq='W-MON')) == '7D'
 
     # just a single date
     pytest.raises(ValueError, infer_frequency, [pd.to_datetime('2000-01-01')])
     # frequency of zero
     pytest.raises(ValueError, infer_frequency,
                   [pd.to_datetime('2000-01-01'),
                    pd.to_datetime('2000-01-01'),
```

### Comparing `neuralhydrology-1.6.0/test/test_mclstm.py` & `neuralhydrology-1.7.0/test/test_mclstm.py`

 * *Files identical despite different names*

