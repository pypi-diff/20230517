# Comparing `tmp/ml-stars-0.1.1.dev0.tar.gz` & `tmp/ml-stars-0.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml-stars-0.1.1.dev0.tar", last modified: Mon Feb  6 18:59:41 2023, max compression
+gzip compressed data, was "ml-stars-0.1.1.dev1.tar", last modified: Tue May 16 21:58:52 2023, max compression
```

## Comparing `ml-stars-0.1.1.dev0.tar` & `ml-stars-0.1.1.dev1.tar`

### file list

```diff
@@ -1,49 +1,111 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/
--rw-r--r--   0 sarah      (501) staff       (20)     4489 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     1070 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)     8324 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)       10 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/HISTORY.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)      217 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/tests/test_utils.py
--rw-r--r--   0 sarah      (501) staff       (20)    10244 2022-10-24 17:51:05.000000 ml-stars-0.1.1.dev0/tests/.DS_Store
--rw-r--r--   0 sarah      (501) staff       (20)      442 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/tests/test_mlstars.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/tests/adapters/
--rw-r--r--   0 sarah      (501) staff       (20)     6148 2022-10-24 17:48:29.000000 ml-stars-0.1.1.dev0/tests/adapters/.DS_Store
--rw-r--r--   0 sarah      (501) staff       (20)     1961 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/tests/adapters/test_statsmodels.py
--rw-r--r--   0 sarah      (501) staff       (20)     1836 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/tests/adapters/test_keras.py
--rw-r--r--   0 sarah      (501) staff       (20)     5027 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/tests/adapters/test_pandas.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/tests/custom/
--rw-r--r--   0 sarah      (501) staff       (20)    15169 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/tests/custom/test_timeseries_preprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)     7362 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/tests/custom/test_timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)      265 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/MANIFEST.in
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      994 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/docs/index.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)    33432 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/docs/images/dai-logo-white-200.png
--rw-r--r--   0 sarah      (501) staff       (20)      608 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/docs/Makefile
--rw-r--r--   0 sarah      (501) staff       (20)     6403 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)      805 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/docs/make.bat
--rw-r--r--   0 sarah      (501) staff       (20)     2924 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/README.md
--rw-r--r--   0 sarah      (501) staff       (20)     2796 2023-02-06 18:59:29.000000 ml-stars-0.1.1.dev0/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)     4489 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)      929 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)       92 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)      678 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)        8 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/top_level.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/ml_stars.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)      108 2022-10-13 18:43:25.000000 ml-stars-0.1.1.dev0/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)      988 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/setup.cfg
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/mlstars/
--rw-r--r--   0 sarah      (501) staff       (20)      441 2023-02-06 18:59:29.000000 ml-stars-0.1.1.dev0/mlstars/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/mlstars/adapters/
--rw-r--r--   0 sarah      (501) staff       (20)     3453 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/adapters/pandas.py
--rw-r--r--   0 sarah      (501) staff       (20)     4088 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/adapters/keras.py
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/adapters/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     1731 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/adapters/statsmodels.py
--rw-r--r--   0 sarah      (501) staff       (20)     2941 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/utils.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-02-06 18:59:41.000000 ml-stars-0.1.1.dev0/mlstars/custom/
--rw-r--r--   0 sarah      (501) staff       (20)    16626 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/custom/timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/custom/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     9481 2023-02-02 21:54:57.000000 ml-stars-0.1.1.dev0/mlstars/custom/timeseries_preprocessing.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.777452 ml-stars-0.1.1.dev1/
+-rw-r--r--   0 sarah      (501) staff       (20)      108 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8324 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      109 2023-04-18 19:20:35.000000 ml-stars-0.1.1.dev1/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1070 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      299 2023-04-18 19:20:35.000000 ml-stars-0.1.1.dev1/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)     5275 2023-05-16 21:58:52.777682 ml-stars-0.1.1.dev1/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     4361 2023-04-18 19:20:35.000000 ml-stars-0.1.1.dev1/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.670988 ml-stars-0.1.1.dev1/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      608 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/Makefile
+-rw-r--r--   0 sarah      (501) staff       (20)     6403 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/conf.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.674231 ml-stars-0.1.1.dev1/docs/developer_guides/
+-rw-r--r--   0 sarah      (501) staff       (20)     8504 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/developer_guides/adapters.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7667 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/docs/developer_guides/annotations.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5116 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/developer_guides/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7925 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/developer_guides/custom.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3414 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/docs/developer_guides/index.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.676652 ml-stars-0.1.1.dev1/docs/getting_started/
+-rw-r--r--   0 sarah      (501) staff       (20)     6296 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/concepts.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      126 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1589 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/install.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1920 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/quickstart.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/history.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.677263 ml-stars-0.1.1.dev1/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)    33432 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/images/dai-logo-white-200.png
+-rw-r--r--   0 sarah      (501) staff       (20)     1505 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      805 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/make.bat
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.682451 ml-stars-0.1.1.dev1/ml_stars.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)     5275 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     4156 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       91 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      683 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        8 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/top_level.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.683611 ml-stars-0.1.1.dev1/mlstars/
+-rw-r--r--   0 sarah      (501) staff       (20)      441 2023-05-16 21:58:43.000000 ml-stars-0.1.1.dev1/mlstars/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.687152 ml-stars-0.1.1.dev1/mlstars/adapters/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/adapters/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4088 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/adapters/keras.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3449 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/mlstars/adapters/pandas.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1731 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/adapters/statsmodels.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.690023 ml-stars-0.1.1.dev1/mlstars/custom/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/custom/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    16626 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/custom/timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)     9471 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/mlstars/custom/timeseries_preprocessing.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.770526 ml-stars-0.1.1.dev1/mlstars/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)     5005 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4499 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5176 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1902 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_anomalies.find_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1244 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_anomalies.regression_errors.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1173 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.cutoff_window_sequences.json
+-rw-r--r--   0 sarah      (501) staff       (20)      870 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.intervals_to_mask.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2027 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.rolling_window_sequences.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1524 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_aggregate.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1099 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_average.json
+-rw-r--r--   0 sarah      (501) staff       (20)      847 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/numpy.argmax.json
+-rw-r--r--   0 sarah      (501) staff       (20)      821 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/numpy.ravel.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/numpy.reshape.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1607 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.append.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1621 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.drop.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1399 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.drop_duplicates.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1579 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.dropna.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1738 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.fillna.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1686 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.filter.json
+-rw-r--r--   0 sarah      (501) staff       (20)      998 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.get.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1948 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.join.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1521 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.json
+-rw-r--r--   0 sarah      (501) staff       (20)      947 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.pop.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2273 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.resample.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.select_dtypes.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1047 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.set.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1817 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.set_index.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.to_numpy.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1243 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.unstack.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1224 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.Series.filter.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2238 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.decomposition.PCA.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1890 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.AdaBoostClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1914 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.AdaBoostRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4782 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.GradientBoostingClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5015 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.GradientBoostingRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2565 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.IsolationForest.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3721 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.RandomForestClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3909 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.RandomForestRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1765 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.impute.SimpleImputer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5411 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.Lasso.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2378 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.LinearRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)     7498 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.LogisticRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4365 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.Ridge.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2459 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.neighbors.KNeighborsClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2401 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.neighbors.KNeighborsRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1663 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.MinMaxScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1321 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.OneHotEncoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1262 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.StandardScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1366 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/mlstars/primitives/statsmodels.tsa.arima_model.Arima.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2226 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/xgboost.XGBClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2220 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/xgboost.XGBRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2941 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/utils.py
+-rw-r--r--   0 sarah      (501) staff       (20)      988 2023-05-16 21:58:52.779336 ml-stars-0.1.1.dev1/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     2801 2023-05-16 21:58:43.000000 ml-stars-0.1.1.dev1/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.772229 ml-stars-0.1.1.dev1/tests/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.774916 ml-stars-0.1.1.dev1/tests/adapters/
+-rw-r--r--   0 sarah      (501) staff       (20)     1836 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/adapters/test_keras.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5027 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/adapters/test_pandas.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1961 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/adapters/test_statsmodels.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.776696 ml-stars-0.1.1.dev1/tests/custom/
+-rw-r--r--   0 sarah      (501) staff       (20)     7362 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/custom/test_timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)    15169 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/custom/test_timeseries_preprocessing.py
+-rw-r--r--   0 sarah      (501) staff       (20)      442 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/test_mlstars.py
+-rw-r--r--   0 sarah      (501) staff       (20)      217 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ml-stars-0.1.1.dev0/LICENSE` & `ml-stars-0.1.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/CONTRIBUTING.rst` & `ml-stars-0.1.1.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/tests/adapters/test_statsmodels.py` & `ml-stars-0.1.1.dev1/tests/adapters/test_statsmodels.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/tests/adapters/test_keras.py` & `ml-stars-0.1.1.dev1/tests/adapters/test_keras.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/tests/adapters/test_pandas.py` & `ml-stars-0.1.1.dev1/tests/adapters/test_pandas.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/tests/custom/test_timeseries_preprocessing.py` & `ml-stars-0.1.1.dev1/tests/custom/test_timeseries_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/tests/custom/test_timeseries_anomalies.py` & `ml-stars-0.1.1.dev1/tests/custom/test_timeseries_anomalies.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/docs/images/dai-logo-white-200.png` & `ml-stars-0.1.1.dev1/docs/images/dai-logo-white-200.png`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/docs/Makefile` & `ml-stars-0.1.1.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/docs/conf.py` & `ml-stars-0.1.1.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/docs/make.bat` & `ml-stars-0.1.1.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/setup.py` & `ml-stars-0.1.1.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     history = history_file.read()
 
 install_requires = [
     'Keras>=2.4,<2.5',
     'mlblocks>=0.4,<0.6',
     'numpy<1.21.0,>=1.16.0',
     'pandas>=1,<2',
-    'scikit-learn>=0.21',
+    'scikit-learn>=0.21,<1.2',
     'scipy>=1.1.0,<2',
     'statsmodels>=0.9.0,<0.13',
     'tensorflow>=2,<2.5',
     'xgboost>=0.72.1,<1',
 
     # fix google/protobuf/descriptor
     'protobuf<4',
@@ -104,10 +104,10 @@
     name='ml-stars',
     packages=find_packages(include=['mlstars', 'mlstars.*']),
     python_requires='>=3.6,<3.9',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/ml-stars',
-    version='0.1.1.dev0',
+    version='0.1.1.dev1',
     zip_safe=False,
 )
```

### Comparing `ml-stars-0.1.1.dev0/ml_stars.egg-info/requires.txt` & `ml-stars-0.1.1.dev1/ml_stars.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Keras<2.5,>=2.4
 mlblocks<0.6,>=0.4
 numpy<1.21.0,>=1.16.0
 pandas<2,>=1
-scikit-learn>=0.21
+scikit-learn<1.2,>=0.21
 scipy<2,>=1.1.0
 statsmodels<0.13,>=0.9.0
 tensorflow<2.5,>=2
 xgboost<1,>=0.72.1
 protobuf<4
 
 [dev]
```

### Comparing `ml-stars-0.1.1.dev0/setup.cfg` & `ml-stars-0.1.1.dev1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1.dev0
+current_version = 0.1.1.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `ml-stars-0.1.1.dev0/mlstars/adapters/pandas.py` & `ml-stars-0.1.1.dev1/mlstars/adapters/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     Returns:
         pandas.Dataframe:
             resampled dataframe
     """
     if on is None and time_index is not None:
         message = (
             'resample `time_series` argument deprecated and will be removed'
-            ' in future versions of MLPrimitives. Please use `on` instead.'
+            ' in future versions of ml-stars. Please use `on` instead.'
         )
         warnings.warn(message, DeprecationWarning, stacklevel=2)
         on = time_index
 
     if groupby:
         df = df.groupby(groupby)
```

### Comparing `ml-stars-0.1.1.dev0/mlstars/adapters/keras.py` & `ml-stars-0.1.1.dev1/mlstars/adapters/keras.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/mlstars/adapters/statsmodels.py` & `ml-stars-0.1.1.dev1/mlstars/adapters/statsmodels.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/mlstars/utils.py` & `ml-stars-0.1.1.dev1/mlstars/utils.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/mlstars/custom/timeseries_anomalies.py` & `ml-stars-0.1.1.dev1/mlstars/custom/timeseries_anomalies.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev0/mlstars/custom/timeseries_preprocessing.py` & `ml-stars-0.1.1.dev1/mlstars/custom/timeseries_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,17 +108,17 @@
         y_index.append(index[end + offset])
         start = start + step_size
 
     return np.asarray(out_X), np.asarray(out_y), np.asarray(X_index), np.asarray(y_index)
 
 
 _TIME_SEGMENTS_AVERAGE_DEPRECATION_WARNING = (
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_average "
+    "mlstars.custom.timeseries_preprocessing.time_segments_average "
     "is deprecated and will be removed in a future version. Please use "
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate instead."
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate instead."
 )
 
 
 def time_segments_average(X, interval, time_column):
     """Compute average of values over given time span.
 
     Args:
```

