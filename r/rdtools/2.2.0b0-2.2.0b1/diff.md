# Comparing `tmp/rdtools-2.2.0b0.tar.gz` & `tmp/rdtools-2.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdtools-2.2.0b0.tar", last modified: Wed Sep 14 13:17:37 2022, max compression
+gzip compressed data, was "rdtools-2.2.0b1.tar", last modified: Wed Dec  7 18:42:24 2022, max compression
```

## Comparing `rdtools-2.2.0b0.tar` & `rdtools-2.2.0b1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:17:37.377779 rdtools-2.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-09-14 13:17:37.377779 rdtools-2.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4582 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:17:37.377779 rdtools-2.2.0b0/rdtools/
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13152 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-14 13:17:37.377779 rdtools-2.2.0b0/rdtools/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)    38558 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/analysis_chains.py
--rw-r--r--   0 runner    (1001) docker     (121)    30022 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/availability.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/clearsky_temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:17:37.369779 rdtools-2.2.0b0/rdtools/data/
--rw-r--r--   0 runner    (1001) docker     (121)  6223504 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/data/temperature.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)    15997 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/degradation.py
--rw-r--r--   0 runner    (1001) docker     (121)    32728 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:17:37.377779 rdtools-2.2.0b0/rdtools/models/
--rw-r--r--   0 runner    (1001) docker     (121)   605196 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/models/xgboost_clipping_model.json
--rw-r--r--   0 runner    (1001) docker     (121)    31477 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)    18180 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)   134157 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/rdtools/soiling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:17:37.369779 rdtools-2.2.0b0/rdtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-09-14 13:17:37.000000 rdtools-2.2.0b0/rdtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-09-14 13:17:37.000000 rdtools-2.2.0b0/rdtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 13:17:37.000000 rdtools-2.2.0b0/rdtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 13:17:37.000000 rdtools-2.2.0b0/rdtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-09-14 13:17:37.000000 rdtools-2.2.0b0/rdtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-14 13:17:37.000000 rdtools-2.2.0b0/rdtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-14 13:17:37.377779 rdtools-2.2.0b0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3398 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-09-14 13:17:26.000000 rdtools-2.2.0b0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 18:42:24.190437 rdtools-2.2.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-07 18:42:24.190437 rdtools-2.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 18:42:24.190437 rdtools-2.2.0b1/rdtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2022-12-07 18:42:24.190437 rdtools-2.2.0b1/rdtools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43619 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/analysis_chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30022 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/clearsky_temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 18:42:24.182437 rdtools-2.2.0b1/rdtools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  6223504 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/data/temperature.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    16558 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/degradation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32728 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 18:42:24.190437 rdtools-2.2.0b1/rdtools/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   605196 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/models/xgboost_clipping_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31477 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18252 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134157 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/rdtools/soiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 18:42:24.182437 rdtools-2.2.0b1/rdtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-07 18:42:24.000000 rdtools-2.2.0b1/rdtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-07 18:42:24.000000 rdtools-2.2.0b1/rdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 18:42:24.000000 rdtools-2.2.0b1/rdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 18:42:24.000000 rdtools-2.2.0b1/rdtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-07 18:42:24.000000 rdtools-2.2.0b1/rdtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-07 18:42:24.000000 rdtools-2.2.0b1/rdtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-07 18:42:24.190437 rdtools-2.2.0b1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2022-12-07 18:42:15.000000 rdtools-2.2.0b1/versioneer.py
```

### Comparing `rdtools-2.2.0b0/LICENSE` & `rdtools-2.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/PKG-INFO` & `rdtools-2.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdtools
-Version: 2.2.0b0
+Version: 2.2.0b1
 Summary: Functions for reproducible timeseries analysis of photovoltaic systems.
 Home-page: https://github.com/NREL/rdtools
 Author: Rdtools Python Developers
 Author-email: RdTools@nrel.gov
 Maintainer-email: RdTools@nrel.gov
 License: MIT
 Project-URL: Bug Tracker, https://github.com/NREL/rdtools/issues
```

### Comparing `rdtools-2.2.0b0/README.md` & `rdtools-2.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/__init__.py` & `rdtools-2.2.0b1/rdtools/__init__.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/_deprecation.py` & `rdtools-2.2.0b1/rdtools/_deprecation.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/aggregation.py` & `rdtools-2.2.0b1/rdtools/aggregation.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/analysis_chains.py` & `rdtools-2.2.0b1/rdtools/analysis_chains.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,14 +71,22 @@
         parameters to be passed to rdtools.filtering functions. Keys are the
         names of the rdtools.filtering functions. Values are dicts of parameters
         to be passed to those functions. Also has a special key `ad_hoc_filter`
         the associated value is a boolean mask joined with the rest of the filters.
         filter_params defaults to empty dicts for each function in rdtools.filtering,
         in which case those functions use default parameter values,  `ad_hoc_filter`
         defaults to None. See examples for more information.
+    filter_params_aggregated: dict
+        parameters to be passed to rdtools.filtering functions that specifically handle
+        aggregated data (dily filters, etc). Keys are the names of the rdtools.filtering functions.
+        Values are dicts of parameters to be passed to those functions. Also has a special key
+        `ad_hoc_filter`; this filter is a boolean mask joined with the rest of the filters.
+        filter_params_aggregated defaults to empty dicts for each function in rdtools.filtering,
+        in which case those functions use default parameter values,  `ad_hoc_filter`
+        defaults to None. See examples for more information.
     results : dict
         Nested dict used to store the results of methods ending with `_analysis`
     '''
 
     def __init__(self, pv, poa_global=None, temperature_cell=None, temperature_ambient=None,
                  gamma_pdc=None, aggregation_freq='D', pv_input='power',
                  windspeed=0, power_expected=None, temperature_model=None,
@@ -129,14 +137,17 @@
             'normalized_filter': {},
             'poa_filter': {},
             'tcell_filter': {},
             'clip_filter': {},
             'csi_filter': {},
             'ad_hoc_filter': None  # use this to include an explict filter
         }
+        self.filter_params_aggregated = {
+            'ad_hoc_filter': None
+        }
         # remove tcell_filter from list if power_expected is passed in
         if power_expected is not None and temperature_cell is None:
             del self.filter_params['tcell_filter']
 
     def set_clearsky(self, pvlib_location=None, pv_azimuth=None, pv_tilt=None,
                      poa_global_clearsky=None, temperature_cell_clearsky=None,
                      temperature_ambient_clearsky=None, albedo=0.25,
@@ -248,15 +259,16 @@
             clearsky['ghi'],
             clearsky['dhi'],
             albedo=self.albedo,
             **kwargs)
         clearsky_poa = clearsky_poa['poa_global']
 
         if aggregate:
-            interval_id = pd.Series(range(len(self.poa_global)), index=self.poa_global.index)
+            interval_id = pd.Series(
+                range(len(self.poa_global)), index=self.poa_global.index)
             interval_id = interval_id.reindex(times, method='backfill')
             clearsky_poa = clearsky_poa.groupby(interval_id).mean()
             clearsky_poa.index = self.poa_global.index
             clearsky_poa.iloc[0] = np.nan
 
         if rescale is True:
             if not clearsky_poa.index.equals(self.poa_global.index):
@@ -379,15 +391,16 @@
 
     def _filter(self, energy_normalized, case):
         '''
         Calculate filters based on those in rdtools.filtering. Uses
         self.filter_params, which is a dict, the keys of which are names of
         functions in rdtools.filtering, and the values of which are dicts
         containing the associated parameters with which to run the filtering
-        functions. See examples for details on how to modify filter parameters.
+        functions. This private method is specifically for the original indexed
+        data. See examples for details on how to modify filter parameters.
 
         Parameters
         ----------
         energy_normalized : pandas.Series
             Time series of normalized PV energy
         case : str
             'sensor' or 'clearsky' which filtering protocol to apply. Affects
@@ -401,15 +414,16 @@
         # Combining filters is non-trivial because of the possibility of index
         # mismatch.  Adding columns to an existing dataframe performs a left index
         # join, but probably we actually want an outer join.  We can get an outer
         # join by keeping this as a dictionary and converting it to a dataframe all
         # at once.  However, we add a default value of True, with the same index as
         # energy_normalized, so that the output is still correct even when all
         # filters have been disabled.
-        filter_components = {'default': pd.Series(True, index=energy_normalized.index)}
+        filter_components = {'default': pd.Series(
+            True, index=energy_normalized.index)}
 
         if case == 'sensor':
             poa = self.poa_global
             cell_temp = self.temperature_cell
         if case == 'clearsky':
             poa = self.poa_global_clearsky
             cell_temp = self.temperature_cell_clearsky
@@ -451,34 +465,93 @@
         filter_components = pd.DataFrame(filter_components).fillna(False)
 
         # apply special checks to ad_hoc_filter, as it is likely more prone to user error
         if self.filter_params.get('ad_hoc_filter', None) is not None:
             ad_hoc_filter = self.filter_params['ad_hoc_filter']
 
             if ad_hoc_filter.isnull().any():
-                warnings.warn('ad_hoc_filter contains NaN values; setting to False (excluding)')
+                warnings.warn(
+                    'ad_hoc_filter contains NaN values; setting to False (excluding)')
                 ad_hoc_filter = ad_hoc_filter.fillna(False)
 
             if not filter_components.index.equals(ad_hoc_filter.index):
                 warnings.warn('ad_hoc_filter index does not match index of other filters; missing '
                               'values will be set to True (kept). Align the index with the index '
                               'of the filter_components attribute to prevent this warning')
-                ad_hoc_filter = ad_hoc_filter.reindex(filter_components.index).fillna(True)
+                ad_hoc_filter = ad_hoc_filter.reindex(
+                    filter_components.index).fillna(True)
 
             filter_components['ad_hoc_filter'] = ad_hoc_filter
 
         bool_filter = filter_components.all(axis=1)
         filter_components = filter_components.drop(columns=['default'])
         if case == 'sensor':
             self.sensor_filter = bool_filter
             self.sensor_filter_components = filter_components
         elif case == 'clearsky':
             self.clearsky_filter = bool_filter
             self.clearsky_filter_components = filter_components
 
+    def _aggregated_filter(self, aggregated, case):
+        """
+        Mirrors the _filter private function, but with aggregated filters applied.
+        These aggregated filters are based on those in rdtools.filtering. Uses
+        self.filter_params_aggregated, which is a dict, the keys of which are names of
+        functions in rdtools.filtering, and the values of which are dicts
+        containing the associated parameters with which to run the filtering
+        functions. See examples for details on how to modify filter parameters.
+
+        Parameters
+        ----------
+        aggregated : pandas.Series
+            Time series of aggregated normalized AC energy
+        case : str
+            'sensor' or 'clearsky' which filtering protocol to apply. Affects
+            whether result is stored in self.sensor_filter_aggregated or
+            self.clearsky_filter_aggregated)
+
+        Returns
+        -------
+        None
+        """
+        filter_components_aggregated = {'default':
+                                        pd.Series(True, index=aggregated.index)}
+        # Add daily aggregate filters as they come online here.
+        # Convert the dictionary into a dataframe (after running filters)
+        filter_components_aggregated = pd.DataFrame(
+            filter_components_aggregated).fillna(False)
+        # Run the ad-hoc filter from filter_params_aggregated, if available
+        if self.filter_params_aggregated.get('ad_hoc_filter', None) is not None:
+            ad_hoc_filter_aggregated = self.filter_params_aggregated['ad_hoc_filter']
+
+            if ad_hoc_filter_aggregated.isnull().any():
+                warnings.warn(
+                    'aggregated ad_hoc_filter contains NaN values; setting to False (excluding)')
+                ad_hoc_filter_aggregated = ad_hoc_filter_aggregated.fillna(False)
+
+            if not filter_components_aggregated.index.equals(ad_hoc_filter_aggregated.index):
+                warnings.warn('Aggregated ad_hoc_filter index does not match index of other '
+                              'filters; missing values will be set to True (kept). '
+                              'Align the index with the index of the '
+                              'filter_components_aggregated attribute to prevent this warning')
+                ad_hoc_filter_aggregated = ad_hoc_filter_aggregated.reindex(
+                    filter_components_aggregated.index).fillna(True)
+
+            filter_components_aggregated['ad_hoc_filter'] = ad_hoc_filter_aggregated
+
+        bool_filter_aggregated = filter_components_aggregated.all(axis=1)
+        filter_components_aggregated = filter_components_aggregated.drop(
+            columns=['default'])
+        if case == 'sensor':
+            self.sensor_filter_aggregated = bool_filter_aggregated
+            self.sensor_filter_components_aggregated = filter_components_aggregated
+        elif case == 'clearsky':
+            self.clearsky_filter_aggregated = bool_filter_aggregated
+            self.clearsky_filter_components_aggregated = filter_components_aggregated
+
     def _filter_check(self, post_filter):
         '''
         post-filter check for requisite 730 days of data
 
         Parameters
         ----------
         post_filter : pandas.Series
@@ -617,16 +690,24 @@
                 self.poa_global, self.temperature_cell)
         else:  # self.power_expected passed in by user
             energy_normalized, insolation = normalization.normalize_with_expected_power(
                 self.pv_energy, self.power_expected, self.poa_global, pv_input='energy')
         self._filter(energy_normalized, 'sensor')
         aggregated, aggregated_insolation = self._aggregate(
             energy_normalized[self.sensor_filter], insolation[self.sensor_filter])
-        self.sensor_aggregated_performance = aggregated
-        self.sensor_aggregated_insolation = aggregated_insolation
+        # Run daily filters on aggregated data
+        self._aggregated_filter(aggregated, 'sensor')
+        # Apply filter to aggregated data and store
+        self.sensor_aggregated_performance = aggregated[self.sensor_filter_aggregated]
+        self.sensor_aggregated_insolation = aggregated_insolation[self.sensor_filter_aggregated]
+        # Reindex the data after the fact, so it's on the aggregated interval
+        self.sensor_aggregated_performance = self.sensor_aggregated_performance.asfreq(
+            self.aggregation_freq)
+        self.sensor_aggregated_insolation = self.sensor_aggregated_insolation.asfreq(
+            self.aggregation_freq)
 
     def _clearsky_preprocess(self):
         '''
         Perform clear-sky-based normalization, filtering, and aggregation.
         If optional parameter self.power_expected is passed in,
         normalize_with_expected_power will be used instead of pvwatts.
         '''
@@ -647,16 +728,25 @@
                 self.poa_global_clearsky, self.temperature_cell_clearsky)
         else:  # self.power_expected passed in by user
             cs_normalized, cs_insolation = normalization.normalize_with_expected_power(
                 self.pv_energy, self.power_expected, self.poa_global_clearsky, pv_input='energy')
         self._filter(cs_normalized, 'clearsky')
         cs_aggregated, cs_aggregated_insolation = self._aggregate(
             cs_normalized[self.clearsky_filter], cs_insolation[self.clearsky_filter])
-        self.clearsky_aggregated_performance = cs_aggregated
-        self.clearsky_aggregated_insolation = cs_aggregated_insolation
+        # Run daily filters on aggregated data
+        self._aggregated_filter(cs_aggregated, 'clearsky')
+        # Apply daily filter to aggregated data and store
+        self.clearsky_aggregated_performance = cs_aggregated[self.clearsky_filter_aggregated]
+        self.clearsky_aggregated_insolation = \
+            cs_aggregated_insolation[self.clearsky_filter_aggregated]
+        # Reindex the data after the fact, so it's on the aggregated interval
+        self.clearsky_aggregated_performance = self.clearsky_aggregated_performance.asfreq(
+            self.aggregation_freq)
+        self.clearsky_aggregated_insolation = self.clearsky_aggregated_insolation.asfreq(
+            self.aggregation_freq)
 
     def sensor_analysis(self, analyses=['yoy_degradation'], yoy_kwargs={}, srr_kwargs={}):
         '''
         Perform entire sensor-based analysis workflow.
         Results are stored in self.results['sensor']
 
         Parameters
```

### Comparing `rdtools-2.2.0b0/rdtools/availability.py` & `rdtools-2.2.0b1/rdtools/availability.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/bootstrap.py` & `rdtools-2.2.0b1/rdtools/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/clearsky_temperature.py` & `rdtools-2.2.0b1/rdtools/clearsky_temperature.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/data/temperature.hdf5` & `rdtools-2.2.0b1/rdtools/data/temperature.hdf5`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/degradation.py` & `rdtools-2.2.0b1/rdtools/degradation.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,19 +240,27 @@
 
     # Detect sub-daily data:
     if min(np.diff(energy_normalized.index.values, n=1)) < \
             np.timedelta64(23, 'h'):
         raise ValueError('energy_normalized must not be '
                          'more frequent than daily')
 
-    # Detect less than 2 years of data
-    if energy_normalized.index[-1] - energy_normalized.index[0] < \
-            pd.Timedelta('730d'):
-        raise ValueError('must provide at least two years of '
-                         'normalized energy')
+    # Detect less than 2 years of data. This is complicated by two things:
+    #   - leap days muddle the precise meaning of "two years of data".
+    #   - can't just check the number of days between the first and last
+    #     index values, since non-daily (e.g. weekly) inputs span
+    #     a longer period than their index values directly indicate.
+    # See the unit tests for several motivating cases.
+    if energy_normalized.index.inferred_freq is not None:
+        step = pd.tseries.frequencies.to_offset(energy_normalized.index.inferred_freq)
+    else:
+        step = energy_normalized.index.to_series().diff().median()
+
+    if energy_normalized.index[-1] < energy_normalized.index[0] + pd.DateOffset(years=2) - step:
+        raise ValueError('must provide at least two years of normalized energy')
 
     # If circular block bootstrapping...
     if uncertainty_method == 'circular_block':
         # ... require regular logging frequency
         freq = pd.infer_freq(energy_normalized.index)
         if isinstance(freq, type(None)):
             raise ValueError('energy_normalized must have a fixed frequency')
@@ -283,14 +291,15 @@
                        )
 
     df['time_diff_years'] = (df.dt - df.dt_right).astype('timedelta64[h]') / 8760.0
     df['yoy'] = 100.0 * (df.energy - df.energy_right) / (df.time_diff_years)
     df.index = df.dt
 
     yoy_result = df.yoy.dropna()
+
     df_right = df.set_index(df.dt_right).drop_duplicates('dt_right')
     df['usage_of_points'] = df.yoy.notnull().astype(int).add(
                 df_right.yoy.notnull().astype(int), fill_value=0)
 
     if not len(yoy_result):
         raise ValueError('no year-over-year aggregated data pairs found')
```

### Comparing `rdtools-2.2.0b0/rdtools/filtering.py` & `rdtools-2.2.0b1/rdtools/filtering.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/models/xgboost_clipping_model.json` & `rdtools-2.2.0b1/rdtools/models/xgboost_clipping_model.json`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/normalization.py` & `rdtools-2.2.0b1/rdtools/normalization.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools/plotting.py` & `rdtools-2.2.0b1/rdtools/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,16 +234,16 @@
         'and default behaviors may change in future releases (including MINOR '
         'and PATCH releases) as the code matures.'
     )
 
     sratio = soiling_info['soiling_ratio_perfect_clean']
     fig, ax = plt.subplots()
     renormalized = normalized_yield / soiling_info['renormalizing_factor']
-    ax.plot(renormalized.index, renormalized, 'o')
-    ax.plot(sratio.index, sratio, 'o')
+    ax.plot(renormalized.index, renormalized, 'o', c=point_color, alpha=point_alpha)
+    ax.plot(sratio.index, sratio, 'o', c=profile_color, alpha=profile_alpha)
     ax.set_ylim(ymin, ymax)
     ax.set_ylabel('Renormalized energy')
 
     fig.autofmt_xdate()
 
     return fig
```

### Comparing `rdtools-2.2.0b0/rdtools/soiling.py` & `rdtools-2.2.0b1/rdtools/soiling.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools.egg-info/PKG-INFO` & `rdtools-2.2.0b1/rdtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdtools
-Version: 2.2.0b0
+Version: 2.2.0b1
 Summary: Functions for reproducible timeseries analysis of photovoltaic systems.
 Home-page: https://github.com/NREL/rdtools
 Author: Rdtools Python Developers
 Author-email: RdTools@nrel.gov
 Maintainer-email: RdTools@nrel.gov
 License: MIT
 Project-URL: Bug Tracker, https://github.com/NREL/rdtools/issues
```

### Comparing `rdtools-2.2.0b0/rdtools.egg-info/SOURCES.txt` & `rdtools-2.2.0b1/rdtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/rdtools.egg-info/requires.txt` & `rdtools-2.2.0b1/rdtools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/setup.py` & `rdtools-2.2.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `rdtools-2.2.0b0/versioneer.py` & `rdtools-2.2.0b1/versioneer.py`

 * *Files identical despite different names*

