# Comparing `tmp/cluster_experiments-0.8.2.tar.gz` & `tmp/cluster_experiments-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.8.2.tar", last modified: Fri May 12 13:15:15 2023, max compression
+gzip compressed data, was "cluster_experiments-0.8.3.tar", last modified: Wed May 17 10:45:08 2023, max compression
```

## Comparing `cluster_experiments-0.8.2.tar` & `cluster_experiments-0.8.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.868112 cluster_experiments-0.8.2/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.8.2/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.8.2/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      659 2023-05-12 13:15:15.866697 cluster_experiments-0.8.2/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7603 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.755470 cluster_experiments-0.8.2/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1760 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.8.2/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    21014 2023-05-09 15:17:29.000000 cluster_experiments-0.8.2/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    16391 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4748 2023-05-10 12:56:47.000000 cluster_experiments-0.8.2/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.8.2/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.8.2/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.8.2/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.771010 cluster_experiments-0.8.2/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      659 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-12 13:15:15.868781 cluster_experiments-0.8.2/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1724 2023-05-12 13:12:21.000000 cluster_experiments-0.8.2/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.785893 cluster_experiments-0.8.2/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.8.2/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.791983 cluster_experiments-0.8.2/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-05-09 15:17:29.000000 cluster_experiments-0.8.2/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.8.2/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.813541 cluster_experiments-0.8.2/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.8.2/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.8.2/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.817396 cluster_experiments-0.8.2/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9410 2023-05-10 12:56:47.000000 cluster_experiments-0.8.2/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.844657 cluster_experiments-0.8.2/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.8.2/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.8.2/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/power_analysis/test_seed.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.864427 cluster_experiments-0.8.2/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.8.2/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.8.2/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.8.2/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.8.2/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2282 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.8.2/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.8.2/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.8.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.875046 cluster_experiments-0.8.3/cluster_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/cupac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/perturbator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/power_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/random_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/washover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.875046 cluster_experiments-0.8.3/cluster_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.875046 cluster_experiments-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/analysis/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/cupac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/cupac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/cupac/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/perturbator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/perturbator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/power_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_time_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_washover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/test_non_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/utils.py
```

### Comparing `cluster_experiments-0.8.2/LICENSE` & `cluster_experiments-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/PKG-INFO` & `cluster_experiments-0.8.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster_experiments
-Version: 0.8.2
+Version: 0.8.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.8.2/README.md` & `cluster_experiments-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 https://pepy.tech/project/cluster-experiments)
 [![PyPI](https://img.shields.io/pypi/v/cluster-experiments)](
 https://pypi.org/project/cluster-experiments/)
 [![Unit tests](https://github.com/david26694/cluster-experiments/workflows/Release%20unit%20Tests/badge.svg)](https://github.com/david26694/cluster-experiments/actions)
 [![CodeCov](
 https://codecov.io/gh/david26694/cluster-experiments/branch/main/graph/badge.svg)](https://app.codecov.io/gh/david26694/cluster-experiments/)
 ![License](https://img.shields.io/github/license/david26694/cluster-experiments)
+[![Pypi version](https://img.shields.io/pypi/pyversions/cluster-experiments.svg)](https://pypi.python.org/pypi/cluster-experiments)
 
 A library to run simulation-based power analysis, including clustered data. Also useful to design and analyse clustered and switchback experiments.
 
 
 <img src="theme/flow.png">
 
 ## Examples
```

### Comparing `cluster_experiments-0.8.2/cluster_experiments/__init__.py` & `cluster_experiments-0.8.3/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/cluster_experiments/cupac.py` & `cluster_experiments-0.8.3/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.8.3/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/cluster_experiments/perturbator.py` & `cluster_experiments-0.8.3/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/cluster_experiments/power_analysis.py` & `cluster_experiments-0.8.3/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/cluster_experiments/random_splitter.py` & `cluster_experiments-0.8.3/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/cluster_experiments/washover.py` & `cluster_experiments-0.8.3/cluster_experiments/washover.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,14 +171,16 @@
 
     @classmethod
     def from_config(cls, config) -> "Washover":
         if not config.washover_time_delta:
             raise ValueError(
                 f"Washover time delta must be specified for ConstantWashover, while it is {config.washover_time_delta = }"
             )
-        return cls(
-            washover_time_delta=config.washover_time_delta,
-        )
+
+        washover_time_delta = config.washover_time_delta
+        if isinstance(washover_time_delta, int):
+            washover_time_delta = datetime.timedelta(minutes=config.washover_time_delta)
+        return cls(washover_time_delta=washover_time_delta)
 
 
 # This is kept in here because of circular imports, need to rethink this
 washover_mapping = {"": EmptyWashover, "constant_washover": ConstantWashover}
```

### Comparing `cluster_experiments-0.8.2/cluster_experiments.egg-info/PKG-INFO` & `cluster_experiments-0.8.3/cluster_experiments.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-experiments
-Version: 0.8.2
+Version: 0.8.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.8.2/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.8.3/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.8.3/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/setup.py` & `cluster_experiments-0.8.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.8.2",
+    version="0.8.3",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.8.2/tests/analysis/test_analysis.py` & `cluster_experiments-0.8.3/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/cupac/test_aggregator.py` & `cluster_experiments-0.8.3/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.8.3/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/examples.py` & `cluster_experiments-0.8.3/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.8.3/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/conftest.py` & `cluster_experiments-0.8.3/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.8.3/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.8.3/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.8.3/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.8.3/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.8.3/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/test_seed.py` & `cluster_experiments-0.8.3/tests/power_analysis/test_seed.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.8.3/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/splitter/conftest.py` & `cluster_experiments-0.8.3/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/splitter/test_splitter.py` & `cluster_experiments-0.8.3/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.8.3/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/splitter/test_time_col.py` & `cluster_experiments-0.8.3/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/splitter/test_washover.py` & `cluster_experiments-0.8.3/tests/splitter/test_washover.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from dataclasses import dataclass
 from datetime import timedelta
 
 import pytest
 
 from cluster_experiments import SwitchbackSplitter
 from cluster_experiments.washover import ConstantWashover, EmptyWashover
 
 
 @pytest.mark.parametrize("minutes, n_rows", [(30, 2), (10, 4), (15, 3)])
 def test_constant_washover_base(minutes, n_rows, washover_base_df):
-
     out_df = ConstantWashover(washover_time_delta=timedelta(minutes=minutes)).washover(
         df=washover_base_df,
         truncated_time_col="time",
         cluster_cols=["city", "time"],
         treatment_col="treatment",
         original_time_col="original___time",
     )
@@ -25,15 +25,14 @@
     "minutes, n_rows, df",
     [
         (30, 4, "washover_df_no_switch"),
         (30, 4 + 4, "washover_df_multi_city"),
     ],
 )
 def test_constant_washover_no_switch(minutes, n_rows, df, request):
-
     washover_df = request.getfixturevalue(df)
 
     out_df = ConstantWashover(washover_time_delta=timedelta(minutes=minutes)).washover(
         df=washover_df,
         truncated_time_col="time",
         cluster_cols=["city", "time"],
         treatment_col="treatment",
@@ -101,7 +100,42 @@
     out_df = splitter.assign_treatment_df(df=washover_split_df)
 
     # Assert A and B in out_df
     assert set(out_df["treatment"].unique()) == {"A", "B"}
 
     # We need to have exactly 1000 rows
     assert len(out_df) == n
+
+
+@pytest.mark.parametrize(
+    "minutes, n_rows, df",
+    [
+        (30, 4, "washover_df_no_switch"),
+        (30, 4 + 4, "washover_df_multi_city"),
+    ],
+)
+def test_constant_washover_no_switch_instantiated_int(minutes, n_rows, df, request):
+    washover_df = request.getfixturevalue(df)
+
+    @dataclass
+    class Cfg:
+        washover_time_delta: int
+
+    cw = ConstantWashover.from_config(Cfg(minutes))
+    out_df = cw.washover(
+        df=washover_df,
+        truncated_time_col="time",
+        cluster_cols=["city", "time"],
+        treatment_col="treatment",
+    )
+    assert len(out_df) == n_rows
+    if df == "washover_df_no_switch":
+        # Check that, after 2022-01-01 02:00:00, we keep all the rows of the original
+        # dataframe
+        assert washover_df.query("time >= '2022-01-01 02:00:00'").equals(
+            out_df.query("time >= '2022-01-01 02:00:00'")
+        )
+        # Check that, after 2022-01-01 01:00:00, we don't have the same rows as the
+        # original dataframe
+        assert not washover_df.query("time >= '2022-01-01 01:00:00'").equals(
+            out_df.query("time >= '2022-01-01 01:00:00'")
+        )
```

### Comparing `cluster_experiments-0.8.2/tests/test_docs.py` & `cluster_experiments-0.8.3/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/test_non_clustered.py` & `cluster_experiments-0.8.3/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.2/tests/utils.py` & `cluster_experiments-0.8.3/tests/utils.py`

 * *Files identical despite different names*

