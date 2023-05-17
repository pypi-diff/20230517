# Comparing `tmp/PatryksAutoAI-1.0.9.tar.gz` & `tmp/PatryksAutoAI-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-1.0.9.tar", last modified: Wed May 17 16:31:08 2023, max compression
+gzip compressed data, was "PatryksAutoAI-1.1.0.tar", last modified: Wed May 17 17:04:18 2023, max compression
```

## Comparing `PatryksAutoAI-1.0.9.tar` & `PatryksAutoAI-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.605250 PatryksAutoAI-1.0.9/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.561250 PatryksAutoAI-1.0.9/KaggleAutoAI/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.561250 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.565250 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/algorithms/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/algorithms/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2168 2023-05-12 22:03:43.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.569250 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.573250 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.573250 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.573250 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     9091 2023-05-16 17:26:42.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7017 2023-05-17 16:30:46.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6221 2023-05-17 16:30:21.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6750 2023-05-17 16:30:15.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7952 2023-05-16 17:27:03.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5692 2023-05-16 17:27:10.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7080 2023-05-17 16:29:50.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2447 2023-05-16 13:31:51.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6718 2023-05-17 16:29:36.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.577250 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.577250 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/metrics.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5086 2023-05-17 16:29:16.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/text2number.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3969 2023-05-16 17:04:33.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.577250 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/models/baseline.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5085 2023-05-17 16:25:27.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/models/transformer_model.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.577250 PatryksAutoAI-1.0.9/KaggleAutoAI/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/model_data/animated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.577250 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.601250 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 16:31:08.605250 PatryksAutoAI-1.0.9/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 16:31:08.605250 PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 16:31:08.000000 PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-17 16:31:08.000000 PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-17 16:31:08.000000 PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-17 16:31:08.000000 PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-17 16:31:08.000000 PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-17 16:31:08.609250 PatryksAutoAI-1.0.9/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-17 16:30:56.000000 PatryksAutoAI-1.0.9/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.183647 PatryksAutoAI-1.1.0/KaggleAutoAI/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.183647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.183647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2168 2023-05-12 22:03:43.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.187647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.187647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.187647 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     9064 2023-05-17 16:38:48.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7017 2023-05-17 16:30:46.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6550 2023-05-17 16:44:45.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6740 2023-05-17 16:45:55.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     8076 2023-05-17 16:49:46.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5692 2023-05-16 17:27:10.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7080 2023-05-17 16:29:50.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2447 2023-05-16 13:31:51.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6701 2023-05-17 17:03:51.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/metrics.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5086 2023-05-17 16:29:16.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text2number.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4078 2023-05-17 16:36:27.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/baseline.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4971 2023-05-17 16:47:33.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/transformer_model.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/animated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-17 17:04:09.000000 PatryksAutoAI-1.1.0/setup.py
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/__init__.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/__init__.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/metrics.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/cat.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 "bootstrap_type": trial.suggest_categorical("bootstrap_type", params["bootstrap_type"]),
                 "used_ram_limit": trial.suggest_int("used_ram_limit", params["used_ram_limit"], params["used_ram_limit"]),
                 "verbose": trial.suggest_int("verbose", params["verbose"], params["verbose"]),
                 "thread_count": trial.suggest_int("thread_count", params["thread_count"], params["thread_count"]),
                 "random_state": trial.suggest_int("random_statep", params['random_state'], params['random_state']),
                 'num_boost_round': trial.suggest_int("num_boost_round", params['num_boost_round'], params['num_boost_round'])
             }
-            cat = CatBoostClassifier(**param,loss_function='MultiClass')
+            cat = CatBoostClassifier(**param)
             cat.fit(X_train,y_train)
             preds = cat.predict(X_test)
             loss = log_loss(y_test, preds)
             return loss
 
         def objective_multi(trial):
           param = {
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/extra_trees.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/gradient_boosting.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/gradient_boosting.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 
 class GradientBoosting(Metrics):
     def __init__(self):
         self.metric = Metrics()
         self.model = None
         self.parameters = None
 
+    def create(self, X, y, params=None):
+        if params == None:
+            cat = GradientBoostingClassifier()
+            cat.fit(X,y)
+            self.model = cat
+        else:
+            cat = GradientBoostingClassifier(**params)
+            cat.fit(X,y)
+            self.model = cat
+            self.parameters = params
+
     def create_grid(self, X, y, params=None, cv=2):
         params_columns = ["loss","learning_rate", "n_estimators",
                           "subsample","min_samples_split","max_depth",
                           "random_state","max_features","verbose",
                           "validation_fraction"]
         params_basic = {
                 'loss': ['log_loss'],
@@ -42,28 +53,28 @@
         grad = GradientBoostingClassifier()
         grid_search = GridSearchCV(grad,params,cv=cv)
         grid_search.fit(X,y)
         self.model = grid_search.best_estimator_
         self.parameters = grid_search.best_params_
 
 
-    def create_gb_optuna(self, X, y, params=None, n_trials=3, show_plot=False, show_features=False):
+    def create_optuna(self, X, y, params=None, n_trials=3, show_plot=False, show_features=False):
         params_columns = ["loss","learning_rate", "n_estimators",
                           "subsample","min_samples_split","max_depth",
                           "random_state","max_features","verbose",
                           "validation_fraction"]
         params_basic = {
-                'loss': 'log_loss',
+                'loss': ['log_loss'],
                 'learning_rate': [0.001,0.1],
                 'n_estimators': [10, 500],
                 'subsample': [0.8],
                 'min_samples_split': [3,10],
                 'max_depth': [1, 8],
-                'random_state': [42],
-                'max_features': 'sqrt',
+                'random_state': 42,
+                'max_features': ['sqrt'],
                 'verbose': 0,
                 'validation_fraction': 0.2
             }
         if params == None:
             params = params_basic
         else:
             for parameter in params_columns:
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/hist_gradient.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/hist_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             'loss': 'log_loss',
             'learning_rate': [0.01, 0.1],
             'max_iter': [200, 1000],
             'max_leaf_nodes': [13, 31],
             'max_depth': [1, 7],
             'min_samples_leaf': [10, 30],
             'l2_regularization': [0, 2],
-            'max_bins': [255],
-            'validation_fraction': [0.2],
+            'max_bins': 255,
+            'validation_fraction': 0.2,
             'verbose': 0,
             'random_state': 42
         }
         if params == None:
             params = params_basic
         else:
             for parameter in params_columns:
@@ -89,15 +89,15 @@
                 'loss': trial.suggest_categorical("loss", params['loss']),
                 'learning_rate': trial.suggest_loguniform('learning_rate', params['learning_rate'][0], params['learning_rate'][1]),
                 'max_iter': trial.suggest_int('max_iter', params['max_iter'][0], params['max_iter'][1]),
                 'max_leaf_nodes': trial.suggest_int('max_leaf_nodes', params['max_leaf_nodes'][0], params['max_leaf_nodes'][1]),
                 'max_depth': trial.suggest_int('max_depth', params['max_depth'][0], params['max_depth'][1]),
                 'min_samples_leaf': trial.suggest_int('min_samples_leaf', params['min_samples_leaf'][0], params['min_samples_leaf'][1]),
                 'l2_regularization': trial.suggest_float('l2_regularization', params["l2_regularization"][0], params["l2_regularization"][1]),
-                'max_bins': trial.suggest_int('max_bins', params['max_bins'][0], params['max_bins'][1]),
+                'max_bins': trial.suggest_int('max_bins', params['max_bins'], params['max_bins']),
                 'validation_fraction': trial.suggest_int("validation_fraction", params['validation_fraction'], params['validation_fraction']),
                 'verbose': trial.suggest_int("verbose", params['verbose'], params['verbose']),
                 'random_state': trial.suggest_int("random_state", params["random_state"], params["random_state"])
             }
             hist = HistGradientBoostingClassifier(**param)
             hist.fit(X_train, y_train)
             preds = hist.predict(X_test)
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/kneighbours.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/light_lgb.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/light_lgb.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,25 @@
 
 class LightLGB(Metrics):
     def __init__(self):
         self.metric = Metrics()
         self.model = None
         self.parameters = None
 
+    def create(self, X, y, params=None):
+        if params == None:
+            cat = lgb()
+            cat.fit(X,y)
+            self.model = cat
+        else:
+            cat = lgb(**params)
+            cat.fit(X,y)
+            self.model = cat
+            self.parameters = params
+
     def create_grid(self,X,y,params=None,cv=3,available_memory_gb=5):
         rows = len(X)
         memory_row = X.memory_usage(deep=True).sum() / rows
         max_bin = int(np.floor(available_memory_gb * 1024**3 / (rows * memory_row)))
 
         params_columns = ["max_bin","objective","metric","boosting_type",
                           "lambda_l1","lambda_l2","num_leaves","feature_fraction",
@@ -51,24 +62,24 @@
         lgb = lgb()
         grid_search = GridSearchCV(lgb, params, cv=cv)
         grid_search.fit(X, y)
         model = grid_search.best_estimator_
         self.model = model
         self.parameters = grid_search.best_params_
 
-    def create_lgb_optuna(self, X, y, params, n_trials=10,available_memory_gb=5, show_plot=False, show_features=False):
+    def create_optuna(self, X, y, params=None, n_trials=10,available_memory_gb=5, show_plot=False, show_features=False):
         ## Calculate processor usage 
         rows = len(X)
         memory_row = X.memory_usage(deep=True).sum() / rows
         max_bin = int(np.floor(available_memory_gb * 1024**3 / (rows * memory_row)))
 
         params_columns = ["max_bin","objective","metric","boosting_type",
                           "lambda_l1","lambda_l2","num_leaves","feature_fraction",
-                          "bagging_fraction","bagging_freq","min_child_samples",
-                          "max_depth","min_gain_to_split","seed","num_boost_round",
+                          "bagging_freq","min_child_samples","num_boost_round",
+                          "max_depth","min_gain_to_split","seed",
                           "verbosity"]
         params_basic ={
             "max_bin": max_bin,
             "objective": ["binary"],
             "metric": "binary_error",
             "boosting_type": ['gbdt', 'dart'],
             "lambda_l1": [0, 1],
@@ -99,15 +110,14 @@
                 'metric': trial.suggest_categorical('metric', params["metric"]),
                 'max_bin': trial.suggest_int("max_bin", params["max_bin"], params["max_bin"]),
                 'boosting_type': trial.suggest_categorical("boosting_type", param["boosting_type"]),
                 'lambda_l1': trial.suggest_float('lambda_l1', params["lambda_l1"][0], params["lambda_1"][1]),
                 'lambda_l2': trial.suggest_float('lambda_l2', params["lambda_l2"][0], params["lambda_2"][1]),
                 'num_leaves': trial.suggest_int('num_leaves', params["num_leaves"][0], params["num_leaves"][1]),
                 'feature_fraction': trial.suggest_uniform('feature_fraction', params["feature_fraction"][0], params["feature_fraction"][1]),
-                'bagging_fraction': trial.suggest_uniform('bagging_fraction', params["bagging_freaction"][0], params["bagging_fraction"][1]),
                 'bagging_freq': trial.suggest_int('bagging_freq', params["bagging_freq"][0], params["bagging_freq"][1]),
                 'min_child_samples': trial.suggest_int('min_child_samples', params["min_child_samples"][0], params["min_child_samples"][0]),
                 'max_depth': trial.suggest_int('max_depth', params["max_depth"][0], params["max_depth"][1]),
                 'min_gain_to_split': trial.suggest_loguniform('min_gain_to_split', params["min_gain_to_split"][0], params["min_gain_to_split"][1]),
                 'seed': trial.suggest_int("seed", params["seed"], params["seed"]),
                 'num_boost_round': trial.suggest_int("num_boost_round", params["num_boost_round"], params["num_boost_round"]),
                 'verbosity': params["verbosity"]
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/linear_svc.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/logistic_regression.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/random_forest.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/sgd_classifier.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/svc.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/classification/models/xgb.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/xgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if params == None:
             params = params_basic
         else:
             for parameter in params_columns:
                 if parameter not in params.keys():
                     params[parameter] = params_basic[parameter]
 
-        X_train, X_test, y_train, y_test = train_test_split(X,y,test_size=0.2,random_state=42, show_plot=False)
+        X_train, X_test, y_train, y_test = train_test_split(X,y,test_size=0.2,random_state=42)
         def objective(trial):
             param = {
                 'n_estimators': trial.suggest_int('n_estimators', params['n_estimators'][0], params['n_estimators'][1]),
                 'learning_rate': trial.suggest_float('learning_rate', params['learning_rate'][0], params['learning_rate'][1]),
                 'max_depth': trial.suggest_int('max_depth', params['max_depth'][0], params['max_depth'][1]),
                 'min_child_weight': trial.suggest_int('min_child_weight', params['min_child_weight'][0], params['min_child_weight'][1]),
                 'subsample': trial.suggest_float("subsample", params['subsample'], params['subsample']),
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/helper_function.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/metrics.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/text2number.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text2number.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 from spellchecker import SpellChecker
 import nltk
 import pandas as pd
 import emoji
 import string
 import re
 
-nltk.download('stopwords')
-
 
 class TextPreprocessing():
     def __init__(self, text:pd.DataFrame):
         self.text = text
 
     def lowercase(self):
         self.text = self.text.apply(lambda x: lower(x))
 
     def punctuation(self):
         self.text = self.text.apply(lambda x: remove_punctuation(x))
 
     def stopwords(self, language='english'):
+        try:
+            nltk.data.find('corpora/stopwords')
+        except LookupError:
+            nltk.download('stopwords')
+        
         stopword = set(stopwords.words(language))
         self.text = self.text.apply(lambda x: remove_stopwords(x, stopword))
 
     def frequent_words(self, most_common=10):
         words = Counter()
         for text in self.text:
             for word in text.split():
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/models/baseline.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/baseline.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/language_processing/models/transformer_model.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/transformer_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,18 +74,16 @@
             self.reset_layers()
             layers = trial.suggest_int("num_layers", params["layers"][0], params["layers"][1])
             for i in range(layers):
                 self.add_layer(
                     trial.suggest_int(f"Layer_{i}", params["layers_dimensions"][0], params["layers_dimensions"][1]),
                     activation="relu"
                 )
-            self.fit(train, val, epochs=2)
-            print("here:", test_data)
+            self.fit(train, val, epochs=1)
             preds = self.model.predict(test_data)
-            print("preds", preds)
             loss = log_loss(test_labels, preds)
             return loss
 
         study = optuna.create_study(direction='minimize', pruner=optuna.pruners.MedianPruner())
         study.optimize(objective, n_trials=n_trials)
         if show_plot:
             optimization_history_plot = optuna.visualization.plot_optimization_history(study)
@@ -107,17 +105,16 @@
             for input_ids, attention_mask, labels in X:
                 batch_predictions = self.model.predict([input_ids, attention_mask])
                 predictions.append(batch_predictions)
             predictions = np.concatenate(predictions, axis=0)
             return predictions
 
         for input_ids, attention_mask in X:
-            print("here:", input_ids, attention_mask)
             batch_predictions = self.model.predict([input_ids, attention_mask])
-            predictions.append(batch_predictions)
+            predictions.append(batch_predictions.reshape(-1))
         predictions = np.concatenate(predictions, axis=0)
         return predictions
     
     def reset_layers(self):
         self.layers = []
 
     def show_layer(self):
```

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/model_data/animated.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/animated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/model_data/model_data.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/metrics_regression.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/cat.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/elastic_net.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/gradient_boosting.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/lasso.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/lgb.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/sgd.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/svr.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/KaggleAutoAI/regression/models/xgb.py` & `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/PKG-INFO` & `PatryksAutoAI-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 1.0.9
+Version: 1.1.0
 Summary: Auto_AI_patryk
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 Keywords: python,machine_learning,auto
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 1.0.9
+Version: 1.1.0
 Summary: Auto_AI_patryk
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 Keywords: python,machine_learning,auto
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PatryksAutoAI-1.0.9/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.0.9/setup.py` & `PatryksAutoAI-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./KaggleAutoAI/requirements.txt') as f:
     requirements = f.read().splitlines()
```

