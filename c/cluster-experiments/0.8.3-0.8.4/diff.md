# Comparing `tmp/cluster_experiments-0.8.3.tar.gz` & `tmp/cluster_experiments-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluster_experiments-0.8.3.tar", last modified: Wed May 17 10:45:08 2023, max compression
+gzip compressed data, was "cluster_experiments-0.8.4.tar", last modified: Wed May 17 12:32:52 2023, max compression
```

## Comparing `cluster_experiments-0.8.3.tar` & `cluster_experiments-0.8.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.875046 cluster_experiments-0.8.3/cluster_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/cupac.py
--rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/perturbator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/power_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/power_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/random_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/cluster_experiments/washover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.875046 cluster_experiments-0.8.3/cluster_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 10:45:08.000000 cluster_experiments-0.8.3/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.875046 cluster_experiments-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/analysis/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/cupac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/cupac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/cupac/test_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/perturbator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/perturbator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.879046 cluster_experiments-0.8.3/tests/power_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:45:08.883046 cluster_experiments-0.8.3/tests/splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_time_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/splitter/test_washover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/test_non_clustered.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 10:43:50.000000 cluster_experiments-0.8.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.387857 cluster_experiments-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 12:32:52.387857 cluster_experiments-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.383857 cluster_experiments-0.8.4/cluster_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/cupac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/perturbator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/power_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/random_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/cluster_experiments/washover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.383857 cluster_experiments-0.8.4/cluster_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 12:32:52.000000 cluster_experiments-0.8.4/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 12:32:52.000000 cluster_experiments-0.8.4/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:32:52.000000 cluster_experiments-0.8.4/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 12:32:52.000000 cluster_experiments-0.8.4/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 12:32:52.000000 cluster_experiments-0.8.4/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:32:52.387857 cluster_experiments-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.383857 cluster_experiments-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.383857 cluster_experiments-0.8.4/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/analysis/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.383857 cluster_experiments-0.8.4/tests/cupac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/cupac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/cupac/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.383857 cluster_experiments-0.8.4/tests/perturbator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/perturbator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.387857 cluster_experiments-0.8.4/tests/power_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:52.387857 cluster_experiments-0.8.4/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/splitter/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/splitter/test_time_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/splitter/test_washover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/test_non_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 12:31:44.000000 cluster_experiments-0.8.4/tests/utils.py
```

### Comparing `cluster_experiments-0.8.3/LICENSE` & `cluster_experiments-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/PKG-INFO` & `cluster_experiments-0.8.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster_experiments
-Version: 0.8.3
+Version: 0.8.4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.8.3/README.md` & `cluster_experiments-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments/__init__.py` & `cluster_experiments-0.8.4/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments/cupac.py` & `cluster_experiments-0.8.4/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.8.4/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments/perturbator.py` & `cluster_experiments-0.8.4/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments/power_analysis.py` & `cluster_experiments-0.8.4/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments/power_config.py` & `cluster_experiments-0.8.4/cluster_experiments/power_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import annotations
-
 import datetime
 import logging
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Union
 
 from cluster_experiments.cupac import EmptyRegressor, TargetAggregation
 from cluster_experiments.experiment_analysis import (
     ClusteredOLSAnalysis,
     GeeExperimentAnalysis,
     MLMExperimentAnalysis,
     OLSAnalysis,
@@ -106,15 +104,15 @@
     # Splitter
     treatments: Optional[List[str]] = None
     strata_cols: Optional[List[str]] = None
     splitter_weights: Optional[List[float]] = None
     switch_frequency: Optional[str] = None
     # Switchback
     time_col: Optional[str] = None
-    washover_time_delta: Optional[datetime.timedelta | int] = None
+    washover_time_delta: Optional[Union[datetime.timedelta, int]] = None
 
     # Analysis
     covariates: Optional[List[str]] = None
 
     # Power analysis
     n_simulations: int = 100
     alpha: float = 0.05
```

### Comparing `cluster_experiments-0.8.3/cluster_experiments/random_splitter.py` & `cluster_experiments-0.8.4/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments/washover.py` & `cluster_experiments-0.8.4/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments.egg-info/PKG-INFO` & `cluster_experiments-0.8.4/cluster_experiments.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-experiments
-Version: 0.8.3
+Version: 0.8.4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.8.3/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.8.4/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.8.4/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/setup.py` & `cluster_experiments-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.8.3",
+    version="0.8.4",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.8.3/tests/analysis/test_analysis.py` & `cluster_experiments-0.8.4/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/cupac/test_aggregator.py` & `cluster_experiments-0.8.4/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.8.4/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/examples.py` & `cluster_experiments-0.8.4/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.8.4/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/conftest.py` & `cluster_experiments-0.8.4/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.8.4/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.8.4/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.8.4/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.8.4/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.8.4/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/test_seed.py` & `cluster_experiments-0.8.4/tests/power_analysis/test_seed.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.8.4/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/splitter/conftest.py` & `cluster_experiments-0.8.4/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/splitter/test_splitter.py` & `cluster_experiments-0.8.4/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.8.4/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/splitter/test_time_col.py` & `cluster_experiments-0.8.4/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/splitter/test_washover.py` & `cluster_experiments-0.8.4/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/test_docs.py` & `cluster_experiments-0.8.4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/test_non_clustered.py` & `cluster_experiments-0.8.4/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.3/tests/utils.py` & `cluster_experiments-0.8.4/tests/utils.py`

 * *Files identical despite different names*

