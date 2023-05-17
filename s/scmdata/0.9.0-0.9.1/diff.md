# Comparing `tmp/scmdata-0.9.0.tar.gz` & `tmp/scmdata-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scmdata-0.9.0.tar", last modified: Thu Feb 18 23:25:25 2021, max compression
+gzip compressed data, was "dist/scmdata-0.9.1.tar", last modified: Wed Feb 24 05:07:20 2021, max compression
```

## Comparing `scmdata-0.9.0.tar` & `scmdata-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-18 23:25:25.000000 scmdata-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)    14877 2021-02-18 23:24:26.000000 scmdata-0.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1503 2021-02-18 23:24:26.000000 scmdata-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      112 2021-02-18 23:24:26.000000 scmdata-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1982 2021-02-18 23:25:25.000000 scmdata-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4196 2021-02-18 23:24:26.000000 scmdata-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      907 2021-02-18 23:25:25.000000 scmdata-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4079 2021-02-18 23:24:26.000000 scmdata-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata/
--rw-r--r--   0 runner    (1001) docker     (116)      323 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     9001 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/database.py
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)    11397 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/filters.py
--rw-r--r--   0 runner    (1001) docker     (116)     5636 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/groupby.py
--rw-r--r--   0 runner    (1001) docker     (116)    11559 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     4079 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/offsets.py
--rw-r--r--   0 runner    (1001) docker     (116)    34504 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/ops.py
--rw-r--r--   0 runner    (1001) docker     (116)    13224 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/plotting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1791 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/pyam_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)    76585 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     2551 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/testing.py
--rw-r--r--   0 runner    (1001) docker     (116)    11095 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/time.py
--rw-r--r--   0 runner    (1001) docker     (116)     8364 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (116)     3403 2021-02-18 23:24:26.000000 scmdata-0.9.0/src/scmdata/units.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1982 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      615 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      775 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2021-02-18 23:25:25.000000 scmdata-0.9.0/src/scmdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    68611 2021-02-18 23:24:26.000000 scmdata-0.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 05:07:20.000000 scmdata-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)    15136 2021-02-24 05:06:17.000000 scmdata-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1503 2021-02-24 05:06:17.000000 scmdata-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      112 2021-02-24 05:06:17.000000 scmdata-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1982 2021-02-24 05:07:20.000000 scmdata-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4196 2021-02-24 05:06:17.000000 scmdata-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      907 2021-02-24 05:07:20.000000 scmdata-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     4079 2021-02-24 05:06:17.000000 scmdata-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata/
+-rw-r--r--   0 runner    (1001) docker     (116)      323 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9001 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/database.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11397 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/filters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5636 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11559 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4079 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/offsets.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34504 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/ops.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13284 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1791 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/pyam_compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)    76585 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2551 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/testing.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11095 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/time.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8364 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3403 2021-02-24 05:06:17.000000 scmdata-0.9.1/src/scmdata/units.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1982 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      615 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      775 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2021-02-24 05:07:20.000000 scmdata-0.9.1/src/scmdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    68611 2021-02-24 05:06:17.000000 scmdata-0.9.1/versioneer.py
```

### Comparing `scmdata-0.9.0/CHANGELOG.rst` & `scmdata-0.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Changelog
 =========
 
 master
 ------
 
+v0.9.1
+------
+
+- (`#144 <https://github.com/openscm/scmdata/pull/144>`_) Fix :meth:`ScmRun.plumeplot` style handling (previously, if ``dashes`` was not supplied each line would be a different style even if all the lines had the same value for ``style_var``)
+
 v0.9.0
 ------
 
 - (`#143 <https://github.com/openscm/scmdata/pull/143>`_) Alter time axis when serialising to netCDF so that time axis is easily read by other tools (e.g. xarray)
 
 v0.8.0
 ------
```

### Comparing `scmdata-0.9.0/LICENSE` & `scmdata-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/PKG-INFO` & `scmdata-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmdata
-Version: 0.9.0
+Version: 0.9.1
 Summary: Data handling for simple climate model data
 Home-page: https://github.com/openscm/scmdata
 Author: Jared Lewis, Zeb Nicholls
 Author-email: jared.lewis@climate-energy-college.org, zebedee.nicholls@climate-energy-college.org
 License: 3-Clause BSD License
 Project-URL: Bug Reports, https://github.com/openscm/scmdata/issues
 Project-URL: Documentation, https://scmdata.readthedocs.io/en/latest
```

### Comparing `scmdata-0.9.0/README.rst` & `scmdata-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/setup.cfg` & `scmdata-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/setup.py` & `scmdata-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/database.py` & `scmdata-0.9.1/src/scmdata/database.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/errors.py` & `scmdata-0.9.1/src/scmdata/errors.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/filters.py` & `scmdata-0.9.1/src/scmdata/filters.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/groupby.py` & `scmdata-0.9.1/src/scmdata/groupby.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/netcdf.py` & `scmdata-0.9.1/src/scmdata/netcdf.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/offsets.py` & `scmdata-0.9.1/src/scmdata/offsets.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/ops.py` & `scmdata-0.9.1/src/scmdata/ops.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/plotting.py` & `scmdata-0.9.1/src/scmdata/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,17 @@
                             pkwargs["linestyle"] = _dashes[style_value]
                         except KeyError as exc:
                             error_msg = "{} not in dashes: {}".format(
                                 style_value, dashes
                             )
                             raise KeyError(error_msg) from exc
                     else:
-                        _dashes[style_value] = next(linestyle_cycler)
+                        if style_value not in _dashes:
+                            _dashes[style_value] = next(linestyle_cycler)
+
                         pkwargs["linestyle"] = _dashes[style_value]
 
                     if isinstance(q[0], str):
                         label = q[0]
                     else:
                         label = "{:.0f}th".format(q[0] * 100)
```

### Comparing `scmdata-0.9.0/src/scmdata/pyam_compat.py` & `scmdata-0.9.1/src/scmdata/pyam_compat.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/run.py` & `scmdata-0.9.1/src/scmdata/run.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/testing.py` & `scmdata-0.9.1/src/scmdata/testing.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/time.py` & `scmdata-0.9.1/src/scmdata/time.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/timeseries.py` & `scmdata-0.9.1/src/scmdata/timeseries.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata/units.py` & `scmdata-0.9.1/src/scmdata/units.py`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata.egg-info/PKG-INFO` & `scmdata-0.9.1/src/scmdata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmdata
-Version: 0.9.0
+Version: 0.9.1
 Summary: Data handling for simple climate model data
 Home-page: https://github.com/openscm/scmdata
 Author: Jared Lewis, Zeb Nicholls
 Author-email: jared.lewis@climate-energy-college.org, zebedee.nicholls@climate-energy-college.org
 License: 3-Clause BSD License
 Project-URL: Bug Reports, https://github.com/openscm/scmdata/issues
 Project-URL: Documentation, https://scmdata.readthedocs.io/en/latest
```

### Comparing `scmdata-0.9.0/src/scmdata.egg-info/SOURCES.txt` & `scmdata-0.9.1/src/scmdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/src/scmdata.egg-info/requires.txt` & `scmdata-0.9.1/src/scmdata.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scmdata-0.9.0/versioneer.py` & `scmdata-0.9.1/versioneer.py`

 * *Files identical despite different names*

