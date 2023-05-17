# Comparing `tmp/PatryksAutoAI-1.1.0.tar.gz` & `tmp/PatryksAutoAI-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-1.1.0.tar", last modified: Wed May 17 17:04:18 2023, max compression
+gzip compressed data, was "PatryksAutoAI-1.1.1.tar", last modified: Wed May 17 17:28:24 2023, max compression
```

## Comparing `PatryksAutoAI-1.1.0.tar` & `PatryksAutoAI-1.1.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.183647 PatryksAutoAI-1.1.0/KaggleAutoAI/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.183647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.183647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2168 2023-05-12 22:03:43.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.187647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.187647 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.187647 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     9064 2023-05-17 16:38:48.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7017 2023-05-17 16:30:46.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6550 2023-05-17 16:44:45.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6740 2023-05-17 16:45:55.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     8076 2023-05-17 16:49:46.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5692 2023-05-16 17:27:10.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7080 2023-05-17 16:29:50.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2447 2023-05-16 13:31:51.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6701 2023-05-17 17:03:51.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/metrics.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5086 2023-05-17 16:29:16.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text2number.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4078 2023-05-17 16:36:27.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/baseline.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4971 2023-05-17 16:47:33.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/transformer_model.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/animated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.191647 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-17 17:04:18.000000 PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-17 17:04:18.195647 PatryksAutoAI-1.1.0/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-17 17:04:09.000000 PatryksAutoAI-1.1.0/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.310174 PatryksAutoAI-1.1.1/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.298174 PatryksAutoAI-1.1.1/KaggleAutoAI/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.298174 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.298174 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/algorithms/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/algorithms/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2168 2023-05-12 22:03:43.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.302174 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.302174 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.302174 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.306174 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     9064 2023-05-17 16:38:48.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7017 2023-05-17 16:30:46.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6545 2023-05-17 17:23:11.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6742 2023-05-17 17:23:53.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     8077 2023-05-17 17:24:38.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5692 2023-05-16 17:27:10.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7080 2023-05-17 16:29:50.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2447 2023-05-16 13:31:51.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6701 2023-05-17 17:03:51.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.306174 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.306174 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/metrics.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5086 2023-05-17 16:29:16.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/text2number.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4078 2023-05-17 16:36:27.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.306174 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/models/baseline.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4999 2023-05-17 17:16:11.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/models/transformer_model.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.306174 PatryksAutoAI-1.1.1/KaggleAutoAI/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/model_data/animated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.306174 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.306174 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 17:28:24.310174 PatryksAutoAI-1.1.1/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-17 17:28:24.310174 PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-17 17:28:24.000000 PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-17 17:28:24.000000 PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-17 17:28:24.000000 PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-17 17:28:24.000000 PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-17 17:28:24.000000 PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-17 17:28:24.310174 PatryksAutoAI-1.1.1/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-17 17:28:09.000000 PatryksAutoAI-1.1.1/setup.py
```

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/__init__.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/__init__.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/metrics.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/cat.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/extra_trees.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/gradient_boosting.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/gradient_boosting.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                           "subsample","min_samples_split","max_depth",
                           "random_state","max_features","verbose",
                           "validation_fraction"]
         params_basic = {
                 'loss': ['log_loss'],
                 'learning_rate': [0.001,0.1],
                 'n_estimators': [10, 500],
-                'subsample': [0.8],
+                'subsample': 0.8,
                 'min_samples_split': [3,10],
                 'max_depth': [1, 8],
                 'random_state': 42,
                 'max_features': ['sqrt'],
                 'verbose': 0,
                 'validation_fraction': 0.2
             }
@@ -81,17 +81,17 @@
                 if parameter not in params.keys():
                     params[parameter] = params_basic[parameter]
 
         X_train, X_test, y_train, y_test = train_test_split(X,y, test_size=0.2, random_state=42)
         def objective(trail):
             param = {
                 'loss': trail.suggest_categorical("loss", params['loss']),
-                'learning_rate': trail.suggest_loguniform("learning_rate", params['learning_rate'][0], params['learning_rate'][1]),
+                'learning_rate': trail.suggest_float("learning_rate", params['learning_rate'][0], params['learning_rate'][1]),
                 'n_estimators': trail.suggest_int('n_estimators', params['n_estimators'][0], params['n_estimators'][1]),
-                'subsample': trail.suggest_int("subsample", params['subsample'], params['subsample']),
+                'subsample': trail.suggest_float("subsample", params['subsample'], params['subsample']),
                 'min_samples_split': trail.suggest_int('min_samples_split', params['min_samples_split'][0], params['min_samples_split'][1]),
                 'max_depth': trail.suggest_int('max_depth', params['max_depth'][0], params['max_depth'][1]),
                 'random_state': trail.suggest_int("random_state", params["random_state"], params["random_state"]),
                 'max_features': trail.suggest_categorical("max_features", params['max_features']),
                 'verbose': trail.suggest_int("verbose", params["verbose"], params["verbose"]),
                 'validation_fraction': trail.suggest_float('validation_fraction', params['validation_fraction'], params['validation_fraction']) 
             }
```

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/hist_gradient.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/hist_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     def create_optuna(self, X, y, params=None, n_trials=2, show_plot=False, show_features=False):
         params_columns = ["loss", "learning_rate", "max_iter",
                             "max_leaf_nodes","max_depth","min_samples_leaf"
                             ,"l2_regularization","max_bins","validation_fraction","verbose",
                             "random_state"]
         params_basic = {
-            'loss': 'log_loss',
+            'loss': ['log_loss'],
             'learning_rate': [0.01, 0.1],
             'max_iter': [200, 1000],
             'max_leaf_nodes': [13, 31],
             'max_depth': [1, 7],
             'min_samples_leaf': [10, 30],
             'l2_regularization': [0, 2],
             'max_bins': 255,
```

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/kneighbours.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/light_lgb.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/light_lgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         dtrain = lgb.Dataset(X_train, label=y_train)
         dval = lgb.Dataset(X_test, label=y_test)
         def objective(trial):
             param = {
                 'objective': trial.suggest_categorical('objective', params["objective"]),
                 'metric': trial.suggest_categorical('metric', params["metric"]),
                 'max_bin': trial.suggest_int("max_bin", params["max_bin"], params["max_bin"]),
-                'boosting_type': trial.suggest_categorical("boosting_type", param["boosting_type"]),
+                'boosting_type': trial.suggest_categorical("boosting_type", params["boosting_type"]),
                 'lambda_l1': trial.suggest_float('lambda_l1', params["lambda_l1"][0], params["lambda_1"][1]),
                 'lambda_l2': trial.suggest_float('lambda_l2', params["lambda_l2"][0], params["lambda_2"][1]),
                 'num_leaves': trial.suggest_int('num_leaves', params["num_leaves"][0], params["num_leaves"][1]),
                 'feature_fraction': trial.suggest_uniform('feature_fraction', params["feature_fraction"][0], params["feature_fraction"][1]),
                 'bagging_freq': trial.suggest_int('bagging_freq', params["bagging_freq"][0], params["bagging_freq"][1]),
                 'min_child_samples': trial.suggest_int('min_child_samples', params["min_child_samples"][0], params["min_child_samples"][0]),
                 'max_depth': trial.suggest_int('max_depth', params["max_depth"][0], params["max_depth"][1]),
```

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/linear_svc.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/logistic_regression.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/random_forest.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/sgd_classifier.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/svc.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/classification/models/xgb.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/helper_function.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/metrics.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text2number.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/text2number.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/baseline.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/models/baseline.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/language_processing/models/transformer_model.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/language_processing/models/transformer_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,16 +105,17 @@
             for input_ids, attention_mask, labels in X:
                 batch_predictions = self.model.predict([input_ids, attention_mask])
                 predictions.append(batch_predictions)
             predictions = np.concatenate(predictions, axis=0)
             return predictions
 
         for input_ids, attention_mask in X:
-            batch_predictions = self.model.predict([input_ids, attention_mask])
-            predictions.append(batch_predictions.reshape(-1))
+            preds = self.model.predict([input_ids, attention_mask])
+            squeezed = np.squeeze(preds, axis=1)
+            predictions.append(squeezed.reshape(-1))
         predictions = np.concatenate(predictions, axis=0)
         return predictions
     
     def reset_layers(self):
         self.layers = []
 
     def show_layer(self):
```

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/animated.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/model_data/animated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/model_data/model_data.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/metrics_regression.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/cat.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/elastic_net.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/gradient_boosting.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lasso.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/lgb.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/sgd.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/svr.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/KaggleAutoAI/regression/models/xgb.py` & `PatryksAutoAI-1.1.1/KaggleAutoAI/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/PKG-INFO` & `PatryksAutoAI-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 1.1.0
+Version: 1.1.1
 Summary: Auto_AI_patryk
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 Keywords: python,machine_learning,auto
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 1.1.0
+Version: 1.1.1
 Summary: Auto_AI_patryk
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 Keywords: python,machine_learning,auto
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PatryksAutoAI-1.1.0/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-1.1.1/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.1.0/setup.py` & `PatryksAutoAI-1.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./KaggleAutoAI/requirements.txt') as f:
     requirements = f.read().splitlines()
```

