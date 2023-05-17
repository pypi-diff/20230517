# Comparing `tmp/prophet-1.1.2.tar.gz` & `tmp/prophet-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet-1.1.2.tar", last modified: Fri Jan 20 11:05:34 2023, max compression
+gzip compressed data, was "prophet-1.1.3.tar", last modified: Wed May 17 14:46:58 2023, max compression
```

## Comparing `prophet-1.1.2.tar` & `prophet-1.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 11:05:34.075203 prophet-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-20 11:05:12.000000 prophet-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-20 11:05:12.000000 prophet-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-01-20 11:05:34.075203 prophet-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-01-20 11:05:12.000000 prophet-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 11:05:34.071203 prophet-1.1.2/prophet/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22557 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    76141 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/forecaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    33593 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/hdays.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/make_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    36757 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 11:05:34.071203 prophet-1.1.2/prophet/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/data2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/serialized_model_v0.6.1.dev0.json
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/serialized_model_v0.7.1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/serialized_model_v1.0.1.json
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34045 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/test_prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-01-20 11:05:12.000000 prophet-1.1.2/prophet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 11:05:34.071203 prophet-1.1.2/prophet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-01-20 11:05:34.000000 prophet-1.1.2/prophet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-01-20 11:05:34.000000 prophet-1.1.2/prophet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 11:05:34.000000 prophet-1.1.2/prophet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 11:05:33.000000 prophet-1.1.2/prophet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-20 11:05:34.000000 prophet-1.1.2/prophet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-20 11:05:34.000000 prophet-1.1.2/prophet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-01-20 11:05:12.000000 prophet-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 11:05:34.075203 prophet-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-01-20 11:05:12.000000 prophet-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 11:05:34.071203 prophet-1.1.2/stan/
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-01-20 11:05:12.000000 prophet-1.1.2/stan/prophet.stan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.588314 prophet-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:46:39.000000 prophet-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 14:46:39.000000 prophet-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-17 14:46:58.588314 prophet-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-17 14:46:39.000000 prophet-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.584313 prophet-1.1.3/prophet/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22557 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76155 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/hdays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/make_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36757 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.588314 prophet-1.1.3/prophet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/data2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/serialized_model_v0.6.1.dev0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/serialized_model_v0.7.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/serialized_model_v1.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37362 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.584313 prophet-1.1.3/prophet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-17 14:46:39.000000 prophet-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:46:58.588314 prophet-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-17 14:46:39.000000 prophet-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.588314 prophet-1.1.3/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-17 14:46:39.000000 prophet-1.1.3/stan/prophet.stan
```

### Comparing `prophet-1.1.2/LICENSE` & `prophet-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/PKG-INFO` & `prophet-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: prophet
-Version: 1.1.2
+Version: 1.1.3
 Summary: Automatic Forecasting Procedure
 Author-email: "Sean J. Taylor" <sjtz@pm.me>, Ben Letham <bletham@fb.com>
 Maintainer-email: Cuong Duong <cuong.duong242@gmail.com>
 License: MIT
-Project-URL: homepage, https://facebook.github.io/prophet/
-Project-URL: documentation, https://facebook.github.io/prophet/
-Project-URL: repository, https://github.com/facebook/prophet
+Project-URL: Homepage, https://facebook.github.io/prophet/
+Project-URL: Documentation, https://facebook.github.io/prophet/
+Project-URL: Repository, https://github.com/facebook/prophet
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `prophet-1.1.2/README.md` & `prophet-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/__init__.py` & `prophet-1.1.3/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/diagnostics.py` & `prophet-1.1.3/prophet/diagnostics.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/forecaster.py` & `prophet-1.1.3/prophet/forecaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,16 +363,16 @@
                 standardize = False
             if standardize == 'auto':
                 if set(df[name].unique()) == {1, 0}:
                     standardize = False #  Don't standardize binary variables.
                 else:
                     standardize = True
             if standardize:
-                mu = df[name].mean()
-                std = df[name].std()
+                mu = float(df[name].mean())
+                std = float(df[name].std())
                 self.extra_regressors[name]['mu'] = mu
                 self.extra_regressors[name]['std'] = std
 
     def set_changepoints(self):
         """Set changepoints
 
         Sets m$changepoints to the dates of changepoints. Either:
```

### Comparing `prophet-1.1.2/prophet/hdays.py` & `prophet-1.1.3/prophet/hdays.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 import warnings
 from datetime import date, timedelta
 
 from convertdate.islamic import from_gregorian, to_gregorian
 from lunarcalendar import Lunar, Converter
 
-from holidays import WEEKEND, HolidayBase, Turkey
+from holidays import WEEKEND, HolidayBase
+from holidays.countries import Turkey
 from dateutil.easter import easter, EASTER_ORTHODOX
 from dateutil.relativedelta import relativedelta as rd
 
 
 # Official public holidays at a country level
 # ------------ Holidays in Indonesia---------------------
 class Indonesia(HolidayBase):
```

### Comparing `prophet-1.1.2/prophet/make_holidays.py` & `prophet-1.1.3/prophet/make_holidays.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/models.py` & `prophet-1.1.3/prophet/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import absolute_import, division, print_function
 from abc import abstractmethod, ABC
 from typing import Tuple
 from collections import OrderedDict
 from enum import Enum
-from pathlib import Path
-import pkg_resources
+import importlib_resources
 import platform
 
 import logging
 logger = logging.getLogger('prophet.models')
 
 PLATFORM = "win" if platform.platform().startswith("Win") else "unix"
 
@@ -55,32 +54,27 @@
 
 
 class CmdStanPyBackend(IStanBackend):
     CMDSTAN_VERSION = "2.26.1"
     def __init__(self):
         import cmdstanpy
         # this must be set before super.__init__() for load_model to work on Windows
-        local_cmdstan = pkg_resources.resource_filename(
-            "prophet", f"stan_model/cmdstan-{self.CMDSTAN_VERSION}"
-        )
-        if Path(local_cmdstan).exists():
-            cmdstanpy.set_cmdstan_path(local_cmdstan)
+        local_cmdstan = importlib_resources.files("prophet") / "stan_model" / f"cmdstan-{self.CMDSTAN_VERSION}"
+        if local_cmdstan.exists():
+            cmdstanpy.set_cmdstan_path(str(local_cmdstan))
         super().__init__()
 
     @staticmethod
     def get_type():
         return StanBackendEnum.CMDSTANPY.name
 
     def load_model(self):
         import cmdstanpy
-        model_file = pkg_resources.resource_filename(
-            'prophet',
-            'stan_model/prophet_model.bin',
-        )
-        return cmdstanpy.CmdStanModel(exe_file=model_file)
+        model_file = importlib_resources.files("prophet") / "stan_model" / "prophet_model.bin"
+        return cmdstanpy.CmdStanModel(exe_file=str(model_file))
 
     def fit(self, stan_init, stan_data, **kwargs):
         if 'inits' not in kwargs and 'init' in kwargs:
             stan_init = self.sanitize_custom_inits(stan_init, kwargs['init'])
             del kwargs['init']
 
         inits_list, data_list = self.prepare_data(stan_init, stan_data)
```

### Comparing `prophet-1.1.2/prophet/plot.py` & `prophet-1.1.3/prophet/plot.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/serialize.py` & `prophet-1.1.3/prophet/serialize.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/tests/data.csv` & `prophet-1.1.3/prophet/tests/data.csv`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/tests/data2.csv` & `prophet-1.1.3/prophet/tests/data2.csv`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/tests/serialized_model_v0.6.1.dev0.json` & `prophet-1.1.3/prophet/tests/serialized_model_v0.6.1.dev0.json`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/tests/serialized_model_v0.7.1.json` & `prophet-1.1.3/prophet/tests/serialized_model_v0.7.1.json`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/tests/serialized_model_v1.0.1.json` & `prophet-1.1.3/prophet/tests/serialized_model_v1.0.1.json`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet/tests/test_diagnostics.py` & `prophet-1.1.3/prophet/tests/test_diagnostics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,358 +1,361 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
-
+import datetime
 import itertools
-import os
-from unittest import TestCase
-from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
-import datetime
+import pytest
+
+from prophet import Prophet, diagnostics
 
-from prophet import Prophet
-from prophet import diagnostics
 
-DATA_all = pd.read_csv(
-    os.path.join(os.path.dirname(__file__), 'data.csv'), parse_dates=['ds']
-)
-DATA = DATA_all.head(100)
+@pytest.fixture(scope="module")
+def ts_short(daily_univariate_ts):
+    return daily_univariate_ts.head(100)
 
 
 class CustomParallelBackend:
     def map(self, func, *iterables):
         results = [func(*args) for args in zip(*iterables)]
         return results
 
 
-class TestDiagnostics(TestCase):
+PARALLEL_METHODS = [None, "processes", "threads", CustomParallelBackend()]
+try:
+    from dask.distributed import Client
+
+    client = Client(processes=False)  # noqa
+    PARALLEL_METHODS.append("dask")
+except ImportError:
+    pass
 
-    def __init__(self, *args, **kwargs):
-        super(TestDiagnostics, self).__init__(*args, **kwargs)
-        # Use first 100 record in data.csv
-        self.__df = DATA
-
-    def test_cross_validation(self):
-        m = Prophet()
-        m.fit(self.__df)
-        # Calculate the number of cutoff points(k)
-        horizon = pd.Timedelta('4 days')
-        period = pd.Timedelta('10 days')
-        initial = pd.Timedelta('115 days')
-        methods = [None, 'processes', 'threads', CustomParallelBackend()]
-
-        try:
-            from dask.distributed import Client
-            client = Client(processes=False)  # noqa
-            methods.append("dask")
-        except ImportError:
-            pass
-
-        for parallel in methods:
-            with self.subTest(i=parallel):
-                df_cv = diagnostics.cross_validation(
-                    m, horizon='4 days', period='10 days', initial='115 days',
-                    parallel=parallel)
-                self.assertEqual(len(np.unique(df_cv['cutoff'])), 3)
-                self.assertEqual(max(df_cv['ds'] - df_cv['cutoff']), horizon)
-                self.assertTrue(min(df_cv['cutoff']) >= min(self.__df['ds']) + initial)
-                dc = df_cv['cutoff'].diff()
-                dc = dc[dc > pd.Timedelta(0)].min()
-                self.assertTrue(dc >= period)
-                self.assertTrue((df_cv['cutoff'] < df_cv['ds']).all())
-                # Each y in df_cv and self.__df with same ds should be equal
-                df_merged = pd.merge(df_cv, self.__df, 'left', on='ds')
-                self.assertAlmostEqual(
-                    np.sum((df_merged['y_x'] - df_merged['y_y']) ** 2), 0.0)
-                df_cv = diagnostics.cross_validation(
-                    m, horizon='4 days', period='10 days', initial='135 days')
-                self.assertEqual(len(np.unique(df_cv['cutoff'])), 1)
-                with self.assertRaises(ValueError):
-                    diagnostics.cross_validation(
-                        m, horizon='10 days', period='10 days', initial='140 days')
 
+class TestCrossValidation:
+    @pytest.mark.parametrize("parallel_method", PARALLEL_METHODS)
+    def test_cross_validation(self, ts_short, parallel_method, backend):
+        m = Prophet(stan_backend=backend)
+        m.fit(ts_short)
+        # Calculate the number of cutoff points(k)
+        horizon = pd.Timedelta("4 days")
+        period = pd.Timedelta("10 days")
+        initial = pd.Timedelta("115 days")
+        df_cv = diagnostics.cross_validation(
+            m, horizon="4 days", period="10 days", initial="115 days", parallel=parallel_method
+        )
+        assert len(np.unique(df_cv["cutoff"])) == 3
+        assert max(df_cv["ds"] - df_cv["cutoff"]) == horizon
+        assert min(df_cv["cutoff"]) >= min(ts_short["ds"]) + initial
+        dc = df_cv["cutoff"].diff()
+        dc = dc[dc > pd.Timedelta(0)].min()
+        assert dc >= period
+        assert (df_cv["cutoff"] < df_cv["ds"]).all()
+        # Each y in df_cv and ts_short with same ds should be equal
+        df_merged = pd.merge(df_cv, ts_short, "left", on="ds")
+        assert np.sum((df_merged["y_x"] - df_merged["y_y"]) ** 2) == pytest.approx(0.0)
+        df_cv = diagnostics.cross_validation(
+            m, horizon="4 days", period="10 days", initial="135 days"
+        )
+        assert len(np.unique(df_cv["cutoff"])) == 1
+        with pytest.raises(ValueError):
+            diagnostics.cross_validation(m, horizon="10 days", period="10 days", initial="140 days")
+
+    def test_bad_parallel_methods(self, ts_short, backend):
+        m = Prophet(stan_backend=backend)
+        m.fit(ts_short)
         # invalid alias
-        with self.assertRaisesRegex(ValueError, "'parallel' should be one"):
+        with pytest.raises(ValueError, match="'parallel' should be one"):
             diagnostics.cross_validation(m, horizon="4 days", parallel="bad")
-
         # no map method
-        with self.assertRaisesRegex(ValueError, "'parallel' should be one"):
+        with pytest.raises(ValueError, match="'parallel' should be one"):
             diagnostics.cross_validation(m, horizon="4 days", parallel=object())
 
+    def test_check_single_cutoff_forecast_func_calls(self, ts_short, monkeypatch, backend):
+        m = Prophet(stan_backend=backend)
+        m.fit(ts_short)
+
+        def mock_predict(df, model, cutoff, horizon, predict_columns):
+            nonlocal n_calls
+            n_calls = n_calls + 1
+            return pd.DataFrame(
+                {
+                    "ds": pd.date_range(start="2012-09-17", periods=3),
+                    "yhat": np.arange(16, 19),
+                    "yhat_lower": np.arange(15, 18),
+                    "yhat_upper": np.arange(17, 20),
+                    "y": np.arange(16.5, 19.5),
+                    "cutoff": [datetime.date(2012, 9, 15)] * 3,
+                }
+            )
 
-    def test_check_single_cutoff_forecast_func_calls(self):
-        m = Prophet()
-        m.fit(self.__df)
-        mock_predict = pd.DataFrame({'ds':pd.date_range(start='2012-09-17', periods=3),
-                                     'yhat':np.arange(16, 19),
-                                     'yhat_lower':np.arange(15, 18),
-                                     'yhat_upper': np.arange(17, 20),
-                                      'y': np.arange(16.5, 19.5),
-                                     'cutoff': [datetime.date(2012, 9, 15)]*3})
-
+        monkeypatch.setattr(diagnostics, "single_cutoff_forecast", mock_predict)
         # cross validation  with 3 and 7 forecasts
-        for args, forecasts in ((['4 days', '10 days', '115 days'], 3),
-                            (['4 days', '4 days', '115 days'], 7)):
-            with patch('prophet.diagnostics.single_cutoff_forecast') as mock_func:
-                mock_func.return_value = mock_predict
-                df_cv = diagnostics.cross_validation(m, *args)
-                # check single forecast function called expected number of times
-                self.assertEqual(diagnostics.single_cutoff_forecast.call_count,
-                                 forecasts)
-
-    def test_cross_validation_logistic_or_flat_growth(self):
-        params = (x for x in ['logistic', 'flat'])
-        for growth in params:
-            with self.subTest(i=growth):
-                df = self.__df.copy()
-                if growth == "logistic":
-                    df['cap'] = 40
-                m = Prophet(growth=growth).fit(df)
-                df_cv = diagnostics.cross_validation(
-                    m, horizon='1 days', period='1 days', initial='140 days')
-                self.assertEqual(len(np.unique(df_cv['cutoff'])), 2)
-                self.assertTrue((df_cv['cutoff'] < df_cv['ds']).all())
-                df_merged = pd.merge(df_cv, self.__df, 'left', on='ds')
-                self.assertAlmostEqual(
-                    np.sum((df_merged['y_x'] - df_merged['y_y']) ** 2), 0.0)
-
-    def test_cross_validation_extra_regressors(self):
-        df = self.__df.copy()
-        df['extra'] = range(df.shape[0])
-        df['is_conditional_week'] = np.arange(df.shape[0]) // 7 % 2
-        m = Prophet()
-        m.add_seasonality(name='monthly', period=30.5, fourier_order=5)
-        m.add_seasonality(name='conditional_weekly', period=7, fourier_order=3,
-                          prior_scale=2., condition_name='is_conditional_week')
-        m.add_regressor('extra')
+        for args, forecasts in (
+            (["4 days", "10 days", "115 days"], 3),
+            (["4 days", "4 days", "115 days"], 7),
+        ):
+            n_calls = 0
+            _ = diagnostics.cross_validation(m, *args)
+            # check single forecast function called expected number of times
+            assert n_calls == forecasts
+
+    @pytest.mark.parametrize("growth", ["logistic", "flat"])
+    def test_cross_validation_logistic_or_flat_growth(self, growth, ts_short, backend):
+        df = ts_short.copy()
+        if growth == "logistic":
+            df["cap"] = 40
+        m = Prophet(growth=growth, stan_backend=backend).fit(df)
+        df_cv = diagnostics.cross_validation(
+            m, horizon="1 days", period="1 days", initial="140 days"
+        )
+        assert len(np.unique(df_cv["cutoff"])) == 2
+        assert (df_cv["cutoff"] < df_cv["ds"]).all()
+        df_merged = pd.merge(df_cv, ts_short, "left", on="ds")
+        assert np.sum((df_merged["y_x"] - df_merged["y_y"]) ** 2) == pytest.approx(0.0)
+
+    def test_cross_validation_extra_regressors(self, ts_short, backend):
+        df = ts_short.copy()
+        df["extra"] = range(df.shape[0])
+        df["is_conditional_week"] = np.arange(df.shape[0]) // 7 % 2
+        m = Prophet(stan_backend=backend)
+        m.add_seasonality(name="monthly", period=30.5, fourier_order=5)
+        m.add_seasonality(
+            name="conditional_weekly",
+            period=7,
+            fourier_order=3,
+            prior_scale=2.0,
+            condition_name="is_conditional_week",
+        )
+        m.add_regressor("extra")
         m.fit(df)
         df_cv = diagnostics.cross_validation(
-            m, horizon='4 days', period='4 days', initial='135 days')
-        self.assertEqual(len(np.unique(df_cv['cutoff'])), 2)
-        period = pd.Timedelta('4 days')
-        dc = df_cv['cutoff'].diff()
+            m, horizon="4 days", period="4 days", initial="135 days"
+        )
+        assert len(np.unique(df_cv["cutoff"])) == 2
+        period = pd.Timedelta("4 days")
+        dc = df_cv["cutoff"].diff()
         dc = dc[dc > pd.Timedelta(0)].min()
-        self.assertTrue(dc >= period)
-        self.assertTrue((df_cv['cutoff'] < df_cv['ds']).all())
-        df_merged = pd.merge(df_cv, self.__df, 'left', on='ds')
-        self.assertAlmostEqual(
-            np.sum((df_merged['y_x'] - df_merged['y_y']) ** 2), 0.0)
-
-    def test_cross_validation_default_value_check(self):
-        m = Prophet()
-        m.fit(self.__df)
+        assert dc >= period
+        assert (df_cv["cutoff"] < df_cv["ds"]).all()
+        df_merged = pd.merge(df_cv, ts_short, "left", on="ds")
+        assert np.sum((df_merged["y_x"] - df_merged["y_y"]) ** 2) == pytest.approx(0.0)
+
+    def test_cross_validation_default_value_check(self, ts_short, backend):
+        m = Prophet(stan_backend=backend)
+        m.fit(ts_short)
         # Default value of initial should be equal to 3 * horizon
-        df_cv1 = diagnostics.cross_validation(
-            m, horizon='32 days', period='10 days')
+        df_cv1 = diagnostics.cross_validation(m, horizon="32 days", period="10 days")
         df_cv2 = diagnostics.cross_validation(
-            m, horizon='32 days', period='10 days', initial='96 days')
-        self.assertAlmostEqual(
-            ((df_cv1['y'] - df_cv2['y']) ** 2).sum(), 0.0)
-        self.assertAlmostEqual(
-            ((df_cv1['yhat'] - df_cv2['yhat']) ** 2).sum(), 0.0)
-
-    def test_cross_validation_custom_cutoffs(self):
-        m = Prophet()
-        m.fit(self.__df)
+            m, horizon="32 days", period="10 days", initial="96 days"
+        )
+        assert ((df_cv1["y"] - df_cv2["y"]) ** 2).sum() == pytest.approx(0.0)
+        assert ((df_cv1["yhat"] - df_cv2["yhat"]) ** 2).sum() == pytest.approx(0.0)
+
+    def test_cross_validation_custom_cutoffs(self, ts_short, backend):
+        m = Prophet(stan_backend=backend)
+        m.fit(ts_short)
         # When specify a list of cutoffs
         #  the cutoff dates in df_cv are those specified
         df_cv1 = diagnostics.cross_validation(
             m,
-            horizon='32 days',
-            period='10 days',
-            cutoffs=[pd.Timestamp('2012-07-31'), pd.Timestamp('2012-08-31')])
-        self.assertEqual(len(df_cv1['cutoff'].unique()), 2)
+            horizon="32 days",
+            period="10 days",
+            cutoffs=[pd.Timestamp("2012-07-31"), pd.Timestamp("2012-08-31")],
+        )
+        assert len(df_cv1["cutoff"].unique()) == 2
 
-    def test_cross_validation_uncertainty_disabled(self):
-        df = self.__df.copy()
+    def test_cross_validation_uncertainty_disabled(self, ts_short, backend):
+        df = ts_short.copy()
         for uncertainty in [0, False]:
-            m = Prophet(uncertainty_samples=uncertainty)
-            m.fit(df, algorithm='Newton')
+            m = Prophet(uncertainty_samples=uncertainty, stan_backend=backend)
+            m.fit(df, algorithm="Newton")
             df_cv = diagnostics.cross_validation(
-                m, horizon='4 days', period='4 days', initial='115 days')
-            expected_cols = ['ds', 'yhat', 'y', 'cutoff']
-            self.assertTrue(all(col in expected_cols for col in df_cv.columns.tolist()))
+                m, horizon="4 days", period="4 days", initial="115 days"
+            )
+            expected_cols = ["ds", "yhat", "y", "cutoff"]
+            assert all(col in expected_cols for col in df_cv.columns.tolist())
             df_p = diagnostics.performance_metrics(df_cv)
-            self.assertTrue('coverage' not in df_p.columns)
+            assert "coverage" not in df_p.columns
 
-    def test_performance_metrics(self):
-        m = Prophet()
-        m.fit(self.__df)
+
+class TestPerformanceMetrics:
+    def test_performance_metrics(self, ts_short, backend):
+        m = Prophet(stan_backend=backend)
+        m.fit(ts_short)
         df_cv = diagnostics.cross_validation(
-            m, horizon='4 days', period='10 days', initial='90 days')
+            m, horizon="4 days", period="10 days", initial="90 days"
+        )
         # Aggregation level none
         df_none = diagnostics.performance_metrics(df_cv, rolling_window=-1)
-        self.assertEqual(
-            set(df_none.columns),
-            {'horizon', 'coverage', 'mae', 'mape', 'mdape', 'mse', 'rmse', 'smape'},
-        )
-        self.assertEqual(df_none.shape[0], 16)
+        assert set(df_none.columns) == {
+            "horizon",
+            "coverage",
+            "mae",
+            "mape",
+            "mdape",
+            "mse",
+            "rmse",
+            "smape",
+        }
+        assert df_none.shape[0] == 16
         # Aggregation level 0
         df_0 = diagnostics.performance_metrics(df_cv, rolling_window=0)
-        self.assertEqual(len(df_0), 4)
-        self.assertEqual(len(df_0['horizon'].unique()), 4)
+        assert len(df_0) == 4
+        assert len(df_0["horizon"].unique()) == 4
         # Aggregation level 0.2
         df_horizon = diagnostics.performance_metrics(df_cv, rolling_window=0.2)
-        self.assertEqual(len(df_horizon), 4)
-        self.assertEqual(len(df_horizon['horizon'].unique()), 4)
+        assert len(df_horizon) == 4
+        assert len(df_horizon["horizon"].unique()) == 4
         # Aggregation level all
         df_all = diagnostics.performance_metrics(df_cv, rolling_window=1)
-        self.assertEqual(df_all.shape[0], 1)
-        for metric in ['mse', 'mape', 'mae', 'coverage']:
-            self.assertAlmostEqual(df_all[metric].values[0], df_none[metric].mean())
-        self.assertAlmostEqual(df_all['mdape'].values[0], df_none['mdape'].median())
+        assert df_all.shape[0] == 1
+        for metric in ["mse", "mape", "mae", "coverage"]:
+            assert df_all[metric].values[0] == pytest.approx(df_none[metric].mean())
+        assert df_all["mdape"].values[0] == pytest.approx(df_none["mdape"].median())
         # Custom list of metrics
         df_horizon = diagnostics.performance_metrics(
-            df_cv, metrics=['coverage', 'mse'],
-        )
-        self.assertEqual(
-            set(df_horizon.columns),
-            {'coverage', 'mse', 'horizon'},
+            df_cv,
+            metrics=["coverage", "mse"],
         )
+        assert set(df_horizon.columns) == {"coverage", "mse", "horizon"}
         # Skip MAPE
-        df_cv.loc[0, 'y'] = 0.
+        df_cv.loc[0, "y"] = 0.0
         df_horizon = diagnostics.performance_metrics(
-            df_cv, metrics=['coverage', 'mape'],
-        )
-        self.assertEqual(
-            set(df_horizon.columns),
-            {'coverage', 'horizon'},
+            df_cv,
+            metrics=["coverage", "mape"],
         )
+        assert set(df_horizon.columns) == {"coverage", "horizon"}
         df_horizon = diagnostics.performance_metrics(
-            df_cv, metrics=['mape'],
+            df_cv,
+            metrics=["mape"],
         )
-        self.assertIsNone(df_horizon)
+        assert df_horizon is None
         # List of metrics containing non-valid metrics
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             diagnostics.performance_metrics(
-                df_cv, metrics=['mse', 'error_metric'],
+                df_cv,
+                metrics=["mse", "error_metric"],
             )
 
     def test_rolling_mean(self):
         x = np.arange(10)
         h = np.arange(10)
-        df = diagnostics.rolling_mean_by_h(x=x, h=h, w=1, name='x')
-        self.assertTrue(np.array_equal(x, df['x'].values))
-        self.assertTrue(np.array_equal(h, df['horizon'].values))
-
-        df = diagnostics.rolling_mean_by_h(x, h, w=4, name='x')
-        self.assertTrue(np.allclose(x[3:] - 1.5, df['x'].values))
-        self.assertTrue(np.array_equal(np.arange(3, 10), df['horizon'].values))
-
-        h = np.array([1., 2., 3., 4., 4., 4., 4., 4., 7., 7.])
-        x_true = np.array([1.0, 5.0 , 22. / 3])
-        h_true = np.array([3., 4., 7.])
-        df = diagnostics.rolling_mean_by_h(x, h, w=3, name='x')
-        self.assertTrue(np.allclose(x_true, df['x'].values))
-        self.assertTrue(np.array_equal(h_true, df['horizon'].values))
-
-        df = diagnostics.rolling_mean_by_h(x, h, w=10, name='x')
-        self.assertTrue(np.allclose(np.array([7.]), df['horizon'].values))
-        self.assertTrue(np.allclose(np.array([4.5]), df['x'].values))
+        df = diagnostics.rolling_mean_by_h(x=x, h=h, w=1, name="x")
+        assert np.array_equal(x, df["x"].values)
+        assert np.array_equal(h, df["horizon"].values)
+
+        df = diagnostics.rolling_mean_by_h(x, h, w=4, name="x")
+        assert np.allclose(x[3:] - 1.5, df["x"].values)
+        assert np.array_equal(np.arange(3, 10), df["horizon"].values)
+
+        h = np.array([1.0, 2.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0, 7.0, 7.0])
+        x_true = np.array([1.0, 5.0, 22.0 / 3])
+        h_true = np.array([3.0, 4.0, 7.0])
+        df = diagnostics.rolling_mean_by_h(x, h, w=3, name="x")
+        assert np.allclose(x_true, df["x"].values)
+        assert np.array_equal(h_true, df["horizon"].values)
+
+        df = diagnostics.rolling_mean_by_h(x, h, w=10, name="x")
+        assert np.allclose(np.array([7.0]), df["horizon"].values)
+        assert np.allclose(np.array([4.5]), df["x"].values)
 
     def test_rolling_median(self):
         x = np.arange(10)
         h = np.arange(10)
-        df = diagnostics.rolling_median_by_h(x=x, h=h, w=1, name='x')
-        self.assertTrue(np.array_equal(x, df['x'].values))
-        self.assertTrue(np.array_equal(h, df['horizon'].values))
+        df = diagnostics.rolling_median_by_h(x=x, h=h, w=1, name="x")
+        assert np.array_equal(x, df["x"].values)
+        assert np.array_equal(h, df["horizon"].values)
 
-        df = diagnostics.rolling_median_by_h(x, h, w=4, name='x')
+        df = diagnostics.rolling_median_by_h(x, h, w=4, name="x")
         x_true = x[3:] - 1.5
-        self.assertTrue(np.allclose(x_true, df['x'].values))
-        self.assertTrue(np.array_equal(np.arange(3, 10), df['horizon'].values))
+        assert np.allclose(x_true, df["x"].values)
+        assert np.array_equal(np.arange(3, 10), df["horizon"].values)
 
-        h = np.array([1., 2., 3., 4., 4., 4., 4., 4., 7., 7.])
+        h = np.array([1.0, 2.0, 3.0, 4.0, 4.0, 4.0, 4.0, 4.0, 7.0, 7.0])
         x_true = np.array([1.0, 5.0, 8.0])
-        h_true = np.array([3., 4., 7.])
-        df = diagnostics.rolling_median_by_h(x, h, w=3, name='x')
-        self.assertTrue(np.allclose(x_true, df['x'].values))
-        self.assertTrue(np.array_equal(h_true, df['horizon'].values))
-
-        df = diagnostics.rolling_median_by_h(x, h, w=10, name='x')
-        self.assertTrue(np.allclose(np.array([7.]), df['horizon'].values))
-        self.assertTrue(np.allclose(np.array([4.5]), df['x'].values))
-
-    def test_copy(self):
-        df = DATA_all.copy()
-        df['cap'] = 200.
-        df['binary_feature'] = [0] * 255 + [1] * 255
+        h_true = np.array([3.0, 4.0, 7.0])
+        df = diagnostics.rolling_median_by_h(x, h, w=3, name="x")
+        assert np.allclose(x_true, df["x"].values)
+        assert np.array_equal(h_true, df["horizon"].values)
+
+        df = diagnostics.rolling_median_by_h(x, h, w=10, name="x")
+        assert np.allclose(np.array([7.0]), df["horizon"].values)
+        assert np.allclose(np.array([4.5]), df["x"].values)
+
+
+class TestProphetCopy:
+    @pytest.fixture(scope="class")
+    def data(self, daily_univariate_ts):
+        df = daily_univariate_ts.copy()
+        df["cap"] = 200.0
+        df["binary_feature"] = [0] * 255 + [1] * 255
+        return df
+
+    def test_prophet_copy(self, data, backend):
         # These values are created except for its default values
-        holiday = pd.DataFrame(
-            {'ds': pd.to_datetime(['2016-12-25']), 'holiday': ['x']})
+        holiday = pd.DataFrame({"ds": pd.to_datetime(["2016-12-25"]), "holiday": ["x"]})
         products = itertools.product(
-            ['linear', 'logistic'],  # growth
-            [None, pd.to_datetime(['2016-12-25'])],  # changepoints
+            ["linear", "logistic"],  # growth
+            [None, pd.to_datetime(["2016-12-25"])],  # changepoints
             [3],  # n_changepoints
             [0.9],  # changepoint_range
             [True, False],  # yearly_seasonality
             [True, False],  # weekly_seasonality
             [True, False],  # daily_seasonality
             [None, holiday],  # holidays
-            ['additive', 'multiplicative'],  # seasonality_mode
+            ["additive", "multiplicative"],  # seasonality_mode
             [1.1],  # seasonality_prior_scale
             [1.1],  # holidays_prior_scale
             [0.1],  # changepoint_prior_scale
             [100],  # mcmc_samples
             [0.9],  # interval_width
-            [200]  # uncertainty_samples
+            [200],  # uncertainty_samples
         )
         # Values should be copied correctly
         for product in products:
-            m1 = Prophet(*product)
-            m1.country_holidays = 'US'
-            m1.history = m1.setup_dataframe(
-                df.copy(), initialize_scales=True)
+            m1 = Prophet(*product, stan_backend=backend)
+            m1.country_holidays = "US"
+            m1.history = m1.setup_dataframe(data.copy(), initialize_scales=True)
             m1.set_auto_seasonalities()
             m2 = diagnostics.prophet_copy(m1)
-            self.assertEqual(m1.growth, m2.growth)
-            self.assertEqual(m1.n_changepoints, m2.n_changepoints)
-            self.assertEqual(m1.changepoint_range, m2.changepoint_range)
+            assert m1.growth == m2.growth
+            assert m1.n_changepoints == m2.n_changepoints
+            assert m1.changepoint_range == m2.changepoint_range
             if m1.changepoints is None:
-                self.assertEqual(m1.changepoints, m2.changepoints)
+                assert m1.changepoints == m2.changepoints
             else:
-                self.assertTrue(m1.changepoints.equals(m2.changepoints))
-            self.assertEqual(False, m2.yearly_seasonality)
-            self.assertEqual(False, m2.weekly_seasonality)
-            self.assertEqual(False, m2.daily_seasonality)
-            self.assertEqual(
-                m1.yearly_seasonality, 'yearly' in m2.seasonalities)
-            self.assertEqual(
-                m1.weekly_seasonality, 'weekly' in m2.seasonalities)
-            self.assertEqual(
-                m1.daily_seasonality, 'daily' in m2.seasonalities)
+                assert m1.changepoints.equals(m2.changepoints)
+            assert False == m2.yearly_seasonality
+            assert False == m2.weekly_seasonality
+            assert False == m2.daily_seasonality
+            assert m1.yearly_seasonality == ("yearly" in m2.seasonalities)
+            assert m1.weekly_seasonality == ("weekly" in m2.seasonalities)
+            assert m1.daily_seasonality == ("daily" in m2.seasonalities)
             if m1.holidays is None:
-                self.assertEqual(m1.holidays, m2.holidays)
+                assert m1.holidays == m2.holidays
             else:
-                self.assertTrue((m1.holidays == m2.holidays).values.all())
-            self.assertEqual(m1.country_holidays, m2.country_holidays)
-            self.assertEqual(m1.seasonality_mode, m2.seasonality_mode)
-            self.assertEqual(m1.seasonality_prior_scale,
-                             m2.seasonality_prior_scale)
-            self.assertEqual(m1.changepoint_prior_scale,
-                             m2.changepoint_prior_scale)
-            self.assertEqual(m1.holidays_prior_scale, m2.holidays_prior_scale)
-            self.assertEqual(m1.mcmc_samples, m2.mcmc_samples)
-            self.assertEqual(m1.interval_width, m2.interval_width)
-            self.assertEqual(m1.uncertainty_samples, m2.uncertainty_samples)
-
-        # Check for cutoff and custom seasonality and extra regressors
-        changepoints = pd.date_range('2012-06-15', '2012-09-15')
-        cutoff = pd.Timestamp('2012-07-25')
-        m1 = Prophet(changepoints=changepoints)
-        m1.add_seasonality('custom', 10, 5)
-        m1.add_regressor('binary_feature')
-        m1.fit(df)
+                assert (m1.holidays == m2.holidays).values.all()
+            assert m1.country_holidays == m2.country_holidays
+            assert m1.seasonality_mode == m2.seasonality_mode
+            assert m1.seasonality_prior_scale == m2.seasonality_prior_scale
+            assert m1.changepoint_prior_scale == m2.changepoint_prior_scale
+            assert m1.holidays_prior_scale == m2.holidays_prior_scale
+            assert m1.mcmc_samples == m2.mcmc_samples
+            assert m1.interval_width == m2.interval_width
+            assert m1.uncertainty_samples == m2.uncertainty_samples
+
+    def test_prophet_copy_custom(self, data, backend):
+        changepoints = pd.date_range("2012-06-15", "2012-09-15")
+        cutoff = pd.Timestamp("2012-07-25")
+        m1 = Prophet(changepoints=changepoints, stan_backend=backend)
+        m1.add_seasonality("custom", 10, 5)
+        m1.add_regressor("binary_feature")
+        m1.fit(data)
         m2 = diagnostics.prophet_copy(m1, cutoff=cutoff)
         changepoints = changepoints[changepoints < cutoff]
-        self.assertTrue((changepoints == m2.changepoints).all())
-        self.assertTrue('custom' in m2.seasonalities)
-        self.assertTrue('binary_feature' in m2.extra_regressors)
-
+        assert (changepoints == m2.changepoints).all()
+        assert "custom" in m2.seasonalities
+        assert "binary_feature" in m2.extra_regressors
```

### Comparing `prophet-1.1.2/prophet/tests/test_serialize.py` & `prophet-1.1.3/prophet/tests/test_serialize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,143 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
-
 import json
-import os
-import sys
-from unittest import TestCase, skipUnless
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
-from prophet import Prophet
-from prophet.serialize import model_to_json, model_from_json, PD_SERIES, PD_DATAFRAME
-
-
-DATA = pd.read_csv(
-    os.path.join(os.path.dirname(__file__), 'data.csv'),
-    parse_dates=['ds'],
-)
+import pytest
 
+from prophet import Prophet
+from prophet.serialize import PD_DATAFRAME, PD_SERIES, model_from_json, model_to_json
 
-class TestSerialize(TestCase):
 
-    def test_simple_serialize(self):
-        m = Prophet()
-        days = 30
-        N = DATA.shape[0]
-        df = DATA.head(N - days)
+class TestSerialize:
+    def test_simple_serialize(self, daily_univariate_ts, backend):
+        m = Prophet(stan_backend=backend)
+        df = daily_univariate_ts.head(daily_univariate_ts.shape[0] - 30)
         m.fit(df)
 
         future = m.make_future_dataframe(2, include_history=False)
         fcst = m.predict(future)
 
         model_str = model_to_json(m)
         # Make sure json doesn't get too large in the future
-        self.assertTrue(len(model_str) < 200000)
+        assert len(model_str) < 200000
         m2 = model_from_json(model_str)
 
         # Check that m and m2 are equal
-        self.assertEqual(m.__dict__.keys(), m2.__dict__.keys())
+        assert m.__dict__.keys() == m2.__dict__.keys()
         for k, v in m.__dict__.items():
-            if k in ['stan_fit', 'stan_backend']:
+            if k in ["stan_fit", "stan_backend"]:
                 continue
-            if k == 'params':
-                self.assertEqual(v.keys(), m2.params.keys())
+            if k == "params":
+                assert v.keys() == m2.params.keys()
                 for kk, vv in v.items():
-                    self.assertTrue(np.array_equal(vv, m2.params[kk]))
+                    assert np.array_equal(vv, m2.params[kk])
             elif k in PD_SERIES and v is not None:
-                self.assertTrue(v.equals(m2.__dict__[k]))
+                assert v.equals(m2.__dict__[k])
             elif k in PD_DATAFRAME and v is not None:
-                pd.testing.assert_frame_equal(v, m2.__dict__[k])
-            elif k == 'changepoints_t':
-                self.assertTrue(np.array_equal(v, m.__dict__[k]))
+                pd.testing.assert_frame_equal(v, m2.__dict__[k], check_index_type=False)
+            elif k == "changepoints_t":
+                assert np.array_equal(v, m.__dict__[k])
             else:
-                self.assertEqual(v, m2.__dict__[k])
-        self.assertTrue(m2.stan_fit is None)
-        self.assertTrue(m2.stan_backend is None)
+                assert v == m2.__dict__[k]
+        assert m2.stan_fit is None
+        assert m2.stan_backend is None
 
         # Check that m2 makes the same forecast
         future2 = m2.make_future_dataframe(2, include_history=False)
         fcst2 = m2.predict(future2)
 
-        self.assertTrue(np.array_equal(fcst['yhat'].values, fcst2['yhat'].values))
+        assert np.array_equal(fcst["yhat"].values, fcst2["yhat"].values)
 
-    def test_full_serialize(self):
+    def test_full_serialize(self, daily_univariate_ts, backend):
         # Construct a model with all attributes
-        holidays = pd.DataFrame({
-            'ds': pd.to_datetime(['2012-06-06', '2013-06-06']),
-            'holiday': ['seans-bday'] * 2,
-            'lower_window': [0] * 2,
-            'upper_window': [1] * 2,
-        })
+        holidays = pd.DataFrame(
+            {
+                "ds": pd.to_datetime(["2012-06-06", "2013-06-06"]),
+                "holiday": ["seans-bday"] * 2,
+                "lower_window": [0] * 2,
+                "upper_window": [1] * 2,
+            }
+        )
         # Test with holidays and country_holidays
         m = Prophet(
             holidays=holidays,
-            seasonality_mode='multiplicative',
-            changepoints=['2012-07-01', '2012-10-01', '2013-01-01'],
+            seasonality_mode="multiplicative",
+            changepoints=["2012-07-01", "2012-10-01", "2013-01-01"],
+            stan_backend=backend,
         )
-        m.add_country_holidays(country_name='US')
-        m.add_seasonality(name='conditional_weekly', period=7, fourier_order=3,
-                          prior_scale=2., condition_name='is_conditional_week')
-        m.add_seasonality(name='normal_monthly', period=30.5, fourier_order=5,
-                          prior_scale=2.)
-        df = DATA.copy()
-        df['is_conditional_week'] = [0] * 255 + [1] * 255
-        m.add_regressor('binary_feature', prior_scale=0.2)
-        m.add_regressor('numeric_feature', prior_scale=0.5)
-        m.add_regressor(
-            'numeric_feature2', prior_scale=0.5, mode='multiplicative'
+        m.add_country_holidays(country_name="US")
+        m.add_seasonality(
+            name="conditional_weekly",
+            period=7,
+            fourier_order=3,
+            prior_scale=2.0,
+            condition_name="is_conditional_week",
         )
-        m.add_regressor('binary_feature2', standardize=True)
-        df['binary_feature'] = ['0'] * 255 + ['1'] * 255
-        df['numeric_feature'] = range(510)
-        df['numeric_feature2'] = range(510)
-        df['binary_feature2'] = [1] * 100 + [0] * 410
+        m.add_seasonality(name="normal_monthly", period=30.5, fourier_order=5, prior_scale=2.0)
+        df = daily_univariate_ts.copy()
+        df["is_conditional_week"] = [0] * 255 + [1] * 255
+        m.add_regressor("binary_feature", prior_scale=0.2)
+        m.add_regressor("numeric_feature", prior_scale=0.5)
+        m.add_regressor("numeric_feature2", prior_scale=0.5, mode="multiplicative")
+        m.add_regressor("binary_feature2", standardize=True)
+        df["binary_feature"] = ["0"] * 255 + ["1"] * 255
+        df["numeric_feature"] = range(510)
+        df["numeric_feature2"] = range(510)
+        df["binary_feature2"] = [1] * 100 + [0] * 410
 
         train = df.head(400)
         test = df.tail(100)
 
         m.fit(train)
-        future = m.make_future_dataframe(periods=100, include_history=False)
         fcst = m.predict(test)
         # Serialize!
         m2 = model_from_json(model_to_json(m))
 
         # Check that m and m2 are equal
-        self.assertEqual(m.__dict__.keys(), m2.__dict__.keys())
+        assert m.__dict__.keys() == m2.__dict__.keys()
         for k, v in m.__dict__.items():
-            if k in ['stan_fit', 'stan_backend']:
+            if k in ["stan_fit", "stan_backend"]:
                 continue
-            if k == 'params':
-                self.assertEqual(v.keys(), m2.params.keys())
+            if k == "params":
+                assert v.keys() == m2.params.keys()
                 for kk, vv in v.items():
-                    self.assertTrue(np.array_equal(vv, m2.params[kk]))
+                    assert np.array_equal(vv, m2.params[kk])
             elif k in PD_SERIES and v is not None:
-                self.assertTrue(v.equals(m2.__dict__[k]))
+                assert v.equals(m2.__dict__[k])
             elif k in PD_DATAFRAME and v is not None:
-                pd.testing.assert_frame_equal(v, m2.__dict__[k])
-            elif k == 'changepoints_t':
-                self.assertTrue(np.array_equal(v, m.__dict__[k]))
+                pd.testing.assert_frame_equal(v, m2.__dict__[k], check_index_type=False)
+            elif k == "changepoints_t":
+                assert np.array_equal(v, m.__dict__[k])
             else:
-                self.assertEqual(v, m2.__dict__[k])
-        self.assertTrue(m2.stan_fit is None)
-        self.assertTrue(m2.stan_backend is None)
+                assert v == m2.__dict__[k]
+        assert m2.stan_fit is None
+        assert m2.stan_backend is None
 
         # Check that m2 makes the same forecast
-        future = m2.make_future_dataframe(periods=100, include_history=False)
         fcst2 = m2.predict(test)
+        assert np.array_equal(fcst["yhat"].values, fcst2["yhat"].values)
 
-        self.assertTrue(np.array_equal(fcst['yhat'].values, fcst2['yhat'].values))
-
+    @pytest.mark.skip(reason="skipping until json serialization issue in pandas 2.0 is resolved.")
     def test_backwards_compatibility(self):
         old_versions = {
-            '0.6.1.dev0': (29.3669923968994, 'fb'),
-            '0.7.1': (29.282810844704414, 'fb'),
-            '1.0.1': (29.282810844704414, ''),
+            "0.6.1.dev0": (29.3669923968994, "fb"),
+            "0.7.1": (29.282810844704414, "fb"),
+            "1.0.1": (29.282810844704414, ""),
         }
         for v, (pred_val, v_str) in old_versions.items():
-            fname = os.path.join(
-                os.path.dirname(__file__),
-                'serialized_model_v{}.json'.format(v)
-            )
-            with open(fname, 'r') as fin:
+            fname = Path(__file__).parent / f"serialized_model_v{v}.json"
+            with open(fname, "r") as fin:
                 model_str = json.load(fin)
             # Check that deserializes
             m = model_from_json(model_str)
-            self.assertEqual(json.loads(model_str)[f'__{v_str}prophet_version'], v)
+            assert json.loads(model_str)[f"__{v_str}prophet_version"] == v
             # Predict
             future = m.make_future_dataframe(10)
             fcst = m.predict(future)
-            self.assertAlmostEqual(fcst['yhat'].values[-1], pred_val)
+            assert fcst["yhat"].values[-1] == pytest.approx(pred_val)
```

### Comparing `prophet-1.1.2/prophet/tests/test_utilities.py` & `prophet-1.1.3/prophet/tests/test_utilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
-
-import os
-from unittest import TestCase
-
 import numpy as np
-import pandas as pd
+
 from prophet import Prophet
 from prophet.utilities import regressor_coefficients
 
 
-DATA = pd.read_csv(
-    os.path.join(os.path.dirname(__file__), 'data.csv'),
-    parse_dates=['ds'],
-)
-
-class TestUtilities(TestCase):
-    def test_regressor_coefficients(self):
-        m = Prophet()
-        N = DATA.shape[0]
-        df = DATA.copy()
+class TestUtilities:
+    def test_regressor_coefficients(self, daily_univariate_ts, backend):
+        m = Prophet(stan_backend=backend)
+        df = daily_univariate_ts.copy()
         np.random.seed(123)
-        df['regr1'] = np.random.normal(size=N)
-        df['regr2'] = np.random.normal(size=N)
-        m.add_regressor('regr1', mode='additive')
-        m.add_regressor('regr2', mode='multiplicative')
+        df["regr1"] = np.random.normal(size=df.shape[0])
+        df["regr2"] = np.random.normal(size=df.shape[0])
+        m.add_regressor("regr1", mode="additive")
+        m.add_regressor("regr2", mode="multiplicative")
         m.fit(df)
 
         coefs = regressor_coefficients(m)
-        self.assertTrue(coefs.shape == (2, 6))
+        assert coefs.shape == (2, 6)
         # No MCMC sampling, so lower and upper should be the same as mean
-        self.assertTrue(np.array_equal(coefs['coef_lower'].values, coefs['coef'].values))
-        self.assertTrue(np.array_equal(coefs['coef_upper'].values, coefs['coef'].values))
+        assert np.array_equal(coefs["coef_lower"].values, coefs["coef"].values)
+        assert np.array_equal(coefs["coef_upper"].values, coefs["coef"].values)
```

### Comparing `prophet-1.1.2/prophet/utilities.py` & `prophet-1.1.3/prophet/utilities.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/prophet.egg-info/PKG-INFO` & `prophet-1.1.3/prophet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: prophet
-Version: 1.1.2
+Version: 1.1.3
 Summary: Automatic Forecasting Procedure
 Author-email: "Sean J. Taylor" <sjtz@pm.me>, Ben Letham <bletham@fb.com>
 Maintainer-email: Cuong Duong <cuong.duong242@gmail.com>
 License: MIT
-Project-URL: homepage, https://facebook.github.io/prophet/
-Project-URL: documentation, https://facebook.github.io/prophet/
-Project-URL: repository, https://github.com/facebook/prophet
+Project-URL: Homepage, https://facebook.github.io/prophet/
+Project-URL: Documentation, https://facebook.github.io/prophet/
+Project-URL: Repository, https://github.com/facebook/prophet
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `prophet-1.1.2/prophet.egg-info/SOURCES.txt` & `prophet-1.1.3/prophet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/pyproject.toml` & `prophet-1.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   "matplotlib>=2.0.0",
   "pandas>=1.0.4",
   "LunarCalendar>=0.0.9",
   "convertdate>=2.1.2",
   "holidays>=0.14.2",
   "python-dateutil>=2.8.0",
   "tqdm>=4.36.1",
+  "importlib_resources",
 ]
 authors = [
   {name = "Sean J. Taylor", email = "sjtz@pm.me"},
   {name = "Ben Letham", email = "bletham@fb.com"},
 ]
 maintainers = [
   {name = "Cuong Duong", email = "cuong.duong242@gmail.com"},
@@ -52,10 +53,10 @@
 ]
 parallel = [
   "dask[dataframe]",
   "distributed",
 ]
 
 [project.urls]
-homepage = "https://facebook.github.io/prophet/"
-documentation = "https://facebook.github.io/prophet/"
-repository = "https://github.com/facebook/prophet"
+Homepage = "https://facebook.github.io/prophet/"
+Documentation = "https://facebook.github.io/prophet/"
+Repository = "https://github.com/facebook/prophet"
```

### Comparing `prophet-1.1.2/setup.py` & `prophet-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.2/stan/prophet.stan` & `prophet-1.1.3/stan/prophet.stan`

 * *Files identical despite different names*

