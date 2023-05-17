# Comparing `tmp/becquerel-0.5.0.tar.gz` & `tmp/becquerel-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "becquerel-0.5.0.tar", last modified: Fri Feb 11 00:11:31 2022, max compression
+gzip compressed data, was "becquerel-0.6.0.tar", last modified: Wed May 17 19:45:27 2023, max compression
```

## Comparing `becquerel-0.5.0.tar` & `becquerel-0.6.0.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:31.492844 becquerel-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-02-11 00:11:10.000000 becquerel-0.5.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-02-11 00:11:10.000000 becquerel-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-02-11 00:11:10.000000 becquerel-0.5.0/COPYRIGHT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-02-11 00:11:10.000000 becquerel-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-02-11 00:11:10.000000 becquerel-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2022-02-11 00:11:31.492844 becquerel-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-02-11 00:11:10.000000 becquerel-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-02-11 00:11:10.000000 becquerel-0.5.0/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:31.488844 becquerel-0.5.0/becquerel/
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/__metadata__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:31.488844 becquerel-0.5.0/becquerel/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11001 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/autocal.py
--rw-r--r--   0 runner    (1001) docker     (121)    42755 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)    12493 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/energycal.py
--rw-r--r--   0 runner    (1001) docker     (121)    46122 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)    14451 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/peakfinder.py
--rw-r--r--   0 runner    (1001) docker     (121)    15520 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    14533 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/rebin.py
--rw-r--r--   0 runner    (1001) docker     (121)    51167 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:31.488844 becquerel-0.5.0/becquerel/io/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/io/h5.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:31.488844 becquerel-0.5.0/becquerel/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10784 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/parsers/cnf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/parsers/h5.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/parsers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/parsers/spc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4741 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/parsers/spe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:31.492844 becquerel-0.5.0/becquerel/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/_nndc_dummy_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/df_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    12311 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/element.py
--rw-r--r--   0 runner    (1001) docker     (121)    13763 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/isotope.py
--rw-r--r--   0 runner    (1001) docker     (121)    27100 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/isotope_qty.py
--rw-r--r--   0 runner    (1001) docker     (121)     8298 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/materials.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/materials_compendium.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/materials_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     6198 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/materials_nist.py
--rw-r--r--   0 runner    (1001) docker     (121)    32778 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/nndc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/wallet_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    17594 2022-02-11 00:11:10.000000 becquerel-0.5.0/becquerel/tools/xcom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 00:11:31.488844 becquerel-0.5.0/becquerel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2022-02-11 00:11:31.000000 becquerel-0.5.0/becquerel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-02-11 00:11:31.000000 becquerel-0.5.0/becquerel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 00:11:31.000000 becquerel-0.5.0/becquerel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-02-11 00:11:31.000000 becquerel-0.5.0/becquerel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-11 00:11:31.000000 becquerel-0.5.0/becquerel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-02-11 00:11:10.000000 becquerel-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-11 00:11:10.000000 becquerel-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-02-11 00:11:10.000000 becquerel-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-02-11 00:11:31.492844 becquerel-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-02-11 00:11:10.000000 becquerel-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.258156 becquerel-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-17 19:45:14.000000 becquerel-0.6.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-05-17 19:45:14.000000 becquerel-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-05-17 19:45:14.000000 becquerel-0.6.0/COPYRIGHT.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-05-17 19:45:14.000000 becquerel-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-17 19:45:14.000000 becquerel-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6674 2023-05-17 19:45:27.258156 becquerel-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-17 19:45:14.000000 becquerel-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-05-17 19:45:14.000000 becquerel-0.6.0/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.254156 becquerel-0.6.0/becquerel/
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/__metadata__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.258156 becquerel-0.6.0/becquerel/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10991 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/autocal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43601 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12418 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/energycal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51121 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15082 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/peakfinder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15510 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15485 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/rebin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52372 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.258156 becquerel-0.6.0/becquerel/io/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4053 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/io/h5.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.258156 becquerel-0.6.0/becquerel/parsers/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10977 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/parsers/cnf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/parsers/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9051 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/parsers/iec1455.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/parsers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12282 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/parsers/spc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/parsers/spe.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.258156 becquerel-0.6.0/becquerel/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1786 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/_nndc_dummy_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4326 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/df_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12271 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/element.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13753 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/isotope.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27740 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/isotope_qty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8298 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/materials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/materials_compendium.py
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/materials_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6198 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/materials_nist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32748 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/nndc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/wallet_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17513 2023-05-17 19:45:14.000000 becquerel-0.6.0/becquerel/tools/xcom.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.254156 becquerel-0.6.0/becquerel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6674 2023-05-17 19:45:27.000000 becquerel-0.6.0/becquerel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1291 2023-05-17 19:45:27.000000 becquerel-0.6.0/becquerel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 19:45:27.000000 becquerel-0.6.0/becquerel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-17 19:45:27.000000 becquerel-0.6.0/becquerel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-17 19:45:27.000000 becquerel-0.6.0/becquerel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-05-17 19:45:14.000000 becquerel-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-17 19:45:14.000000 becquerel-0.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-05-17 19:45:14.000000 becquerel-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-05-17 19:45:27.258156 becquerel-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-05-17 19:45:14.000000 becquerel-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 19:45:27.258156 becquerel-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-05-17 19:45:14.000000 becquerel-0.6.0/tests/test_utils.py
```

### Comparing `becquerel-0.5.0/CONTRIBUTING.md` & `becquerel-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/COPYRIGHT.txt` & `becquerel-0.6.0/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/LICENSE.txt` & `becquerel-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/PKG-INFO` & `becquerel-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: becquerel
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools for radiation spectral analysis.
 Home-page: https://github.com/lbl-anp/becquerel
 Maintainer: The Becquerel Development Team
 Maintainer-email: becquerel-dev@lbl.gov
 License: Other/Proprietary License (see LICENSE.txt)
 Download-URL: https://github.com/lbl-anp/becquerel/releases
 Platform: any
```

### Comparing `becquerel-0.5.0/README.md` & `becquerel-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/RELEASING.md` & `becquerel-0.6.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/becquerel/__init__.py` & `becquerel-0.6.0/becquerel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     __copyright__,
 )
 
 from . import core
 from .core import utils, fitting
 from .core.autocal import AutoCalibrator, AutoCalibratorError
 from .core.energycal import LinearEnergyCal, EnergyCalError, BadInput
-from .core.calibration import Calibration, CalibrationError
+from .core.calibration import Calibration, CalibrationError, CalibrationWarning
 from .core.fitting import Fitter
 from .core.peakfinder import (
     PeakFilter,
     PeakFilterError,
     GaussianPeakFilter,
     PeakFinder,
     PeakFinderError,
@@ -50,14 +50,15 @@
     "AutoCalibrator",
     "AutoCalibratorError",
     "LinearEnergyCal",
     "EnergyCalError",
     "BadInput",
     "Calibration",
     "CalibrationError",
+    "CalibrationWarning",
     "Fitter",
     "PeakFilter",
     "PeakFilterError",
     "GaussianPeakFilter",
     "PeakFinder",
     "PeakFinderError",
     "SpectrumPlotter",
```

### Comparing `becquerel-0.5.0/becquerel/__metadata__.py` & `becquerel-0.6.0/becquerel/__metadata__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __name__ = "becquerel"
 __author__ = "The Becquerel Development Team"
 __maintainer__ = __author__
 __email__ = "becquerel-dev@lbl.gov"
 __description__ = "Tools for radiation spectral analysis."
 __url__ = "https://github.com/lbl-anp/becquerel"
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 # classifiers from list at https://pypi.org/classifiers/
 __classifiers__ = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
```

### Comparing `becquerel-0.5.0/becquerel/core/autocal.py` & `becquerel-0.6.0/becquerel/core/autocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,14 @@
     186.21,
 ]
 
 
 class AutoCalibratorError(Exception):
     """Base class for errors in AutoCalibrator."""
 
-    pass
-
 
 def fit_gain(channels, snrs, energies):
     """Calculate the mean gain to relate channels to energies.
 
     Assume that the peak channel error scales like fwhm/snr,
     which is proportional to sqrt(x)/snr.
```

### Comparing `becquerel-0.5.0/becquerel/core/calibration.py` & `becquerel-0.6.0/becquerel/core/calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 """Class to describe a generic calibration function."""
 
 import ast
 import copy
+import warnings
 import asteval
 import black
 import blib2to3
 import numpy as np
 import scipy
 import scipy.optimize
 import matplotlib.pyplot as plt
 from .. import io
 
-DEFAULT_DOMAIN = (0, 1e5)
-DEFAULT_RANGE = (0, 1e5)
+# the default domain (x) and range (y) ranges over which a calibration is valid
+DEFAULT_DOMAIN = (-1e6, 1e6)
+DEFAULT_RANGE = (-1e6, 1e6)
 
 safe_eval = asteval.Interpreter(use_numpy=False)
 safe_eval.symtable["np"] = np
 safe_eval.symtable["numpy"] = np
 safe_eval.symtable["scipy"] = scipy
 
 
 class CalibrationError(Exception):
     """Base class for calibration errors."""
 
-    pass
+
+class CalibrationWarning(UserWarning):
+    """Warnings displayed by the Calibration class."""
 
 
 def _validate_domain_range(domain, rng):
     """Validate that domain and range contain finite values.
 
     Parameters
     ----------
     domain : array_like
         The domain of the function. Will raise an error if the independent
-        variable is outside this interval. Must be finite.
-        By default DEFAULT_DOMAIN.
+        variable is outside this interval. Must be finite. If None will use
+        the default. By default DEFAULT_DOMAIN.
     rng : array_like
         The range of the function. Expression outputs will be clipped to this
-        interval. Must be finite. By default DEFAULT_RANGE.
+        interval. Must be finite. If None will use the default. By default
+        DEFAULT_RANGE.
     """
+    if domain is None:
+        domain = DEFAULT_DOMAIN
+    if rng is None:
+        rng = DEFAULT_RANGE
     # must be length-2 iterables
     try:
         len(domain)
     except TypeError:
         raise CalibrationError(f"Domain must be length-2 iterable: {domain}")
     domain = np.asarray(domain)
     if not (len(domain) == 2 and domain.ndim == 1):
@@ -60,24 +69,25 @@
     if not np.isfinite(rng[0]) or not np.isfinite(rng[1]):
         raise CalibrationError(f"Range must contain finite values: {rng}")
     # must be in ascending order
     if not (domain[1] > domain[0]):
         raise CalibrationError(f"Domain must contain ascending values: {domain}")
     if not (rng[1] > rng[0]):
         raise CalibrationError(f"Range must contain ascending values: {rng}")
+    return domain, rng
 
 
 def _eval_expression(
     expression,
     params,
     x,
     ind_var="x",
     aux_params=None,
-    domain=DEFAULT_DOMAIN,
-    rng=DEFAULT_RANGE,
+    domain=None,
+    rng=None,
 ):
     """Evaluate the expression at x.
 
     Parameters
     ----------
     expression : string
         The expression that defines the calibration function.
@@ -100,15 +110,15 @@
         interval. Must be finite. By default DEFAULT_RANGE.
 
     Returns
     -------
     y : float or array_like
         Result of evaluating the expression for x.
     """
-    _validate_domain_range(domain, rng)
+    domain, rng = _validate_domain_range(domain, rng)
     x = np.asarray(x)
     if not np.all(x >= domain[0]):
         raise CalibrationError(f"{ind_var} must be >= {domain[0]}: {x}")
     if not np.all(x <= domain[1]):
         raise CalibrationError(f"{ind_var} must be <= {domain[1]}: {x}")
     if ind_var not in ["x", "y"]:
         raise CalibrationError(f"Independent variable {ind_var} must be 'x' or 'y'")
@@ -123,16 +133,28 @@
     if len(safe_eval.error) > 0:
         raise CalibrationError(
             "asteval failed with errors:\n"
             + "\n".join(str(err.get_error()) for err in safe_eval.error)
         )
     if not np.all(np.isreal(y)):
         raise CalibrationError(f"Function evaluation resulted in complex values: {y}")
-    # clip values of y to the range
-    y = np.clip(y, rng[0], rng[1])
+    # warn if y values outside range
+    y_low = np.any(y < rng[0])
+    y_high = np.any(y > rng[1])
+    if y_low or y_high:
+        msg = "Function values are "
+        msg_low = f"below the lower range ({rng[0]})"
+        msg_high = f"above the upper range ({rng[1]})"
+        if y_low and y_high:
+            msg = msg + msg_low + " and " + msg_high
+        elif y_low:
+            msg = msg + msg_low
+        else:
+            msg = msg + msg_high
+        warnings.warn(msg, CalibrationWarning)
     return y
 
 
 def _param_indices(expression):
     """Find all integer parameter indices of the expression.
 
     The expression must explicitly call each parameter as "p[j]", where
@@ -156,16 +178,16 @@
 
 
 def _validate_expression(
     expression,
     ind_var="x",
     params=None,
     aux_params=None,
-    domain=DEFAULT_DOMAIN,
-    rng=DEFAULT_RANGE,
+    domain=None,
+    rng=None,
     n_eval=100,
 ):
     """Perform checks on the expression.
 
     The expression must explicitly call each parameter as "p[j]", where
     j is the index of the parameter, and the indices for n parameters
     range from 0 to n - 1. The expression is checked for how many
@@ -197,15 +219,15 @@
         Number of points in the domain the evaluate at for testing.
 
     Returns
     -------
     expression : string
         Expression having been validated and reformatted using black.
     """
-    _validate_domain_range(domain, rng)
+    domain, rng = _validate_domain_range(domain, rng)
 
     # apply black formatting for consistency and error checking
     try:
         expression = black.format_str(expression, mode=black.FileMode())
     except (black.InvalidInput, blib2to3.pgen2.tokenize.TokenError):
         raise CalibrationError(
             f"Error while running black on expression:\n{expression}"
@@ -291,16 +313,16 @@
 def _fit_expression(
     expression,
     points_x,
     points_y,
     weights=None,
     params0=None,
     aux_params=None,
-    domain=DEFAULT_DOMAIN,
-    rng=DEFAULT_RANGE,
+    domain=None,
+    rng=None,
     **kwargs,
 ):
     """Fit the expression using the calibration points.
 
     Performs least squares via scipy.optimize.least_squares.
 
     Parameters
@@ -387,17 +409,15 @@
     )
     if not results.success:
         raise CalibrationError(results.message)
     params = results.x
     return params
 
 
-def _check_points(
-    points_x, points_y, weights=None, domain=DEFAULT_DOMAIN, rng=DEFAULT_RANGE
-):
+def _check_points(points_x, points_y, weights=None, domain=None, rng=None):
     """Perform various checks on the sets of calibration points.
 
     Ensure the arrays of points are both 1-D and have the same length,
     that all values are >= 0, that they fall within the domain and range,
     and then put them in the order of ascending x values.
 
     Parameters
@@ -458,14 +478,15 @@
         raise CalibrationError(f"Weights cannot be negative: {weights}")
     # sort points in increasing order of x
     i = np.argsort(points_x)
     points_x = points_x[i]
     points_y = points_y[i]
     weights = weights[i]
     # check domain and range
+    domain, rng = _validate_domain_range(domain, rng)
     if np.any((points_x < domain[0]) | (domain[1] < points_x)):
         raise CalibrationError(
             f"Some x points are outside of domain {domain}: {points_x}"
         )
     if np.any((points_y < rng[0]) | (rng[1] < points_y)):
         raise CalibrationError(f"Some y points are outside of range {rng}: {points_y}")
     return points_x, points_y, weights
@@ -508,16 +529,16 @@
 
     def __init__(
         self,
         expression: str,
         params,
         aux_params=None,
         inv_expression=None,
-        domain=DEFAULT_DOMAIN,
-        rng=DEFAULT_RANGE,
+        domain=None,
+        rng=None,
         **attrs,
     ):
         """Create a calibration described by the expression and parameters.
 
         Parameters
         ----------
         expression : string
@@ -658,26 +679,35 @@
 
     @property
     def domain(self):
         return self._domain
 
     @domain.setter
     def domain(self, domain):
-        _validate_domain_range(domain, (0, 1))
+        domain, _ = _validate_domain_range(domain, (0, 1))
         self._domain = tuple(domain)
 
     @property
     def range(self):
         return self._range
 
     @range.setter
     def range(self, rng):
-        _validate_domain_range((0, 1), rng)
+        _, rng = _validate_domain_range((0, 1), rng)
         self._range = tuple(rng)
 
+    # rng as an alias for range
+    @property
+    def rng(self):
+        return self.range
+
+    @rng.setter
+    def rng(self, rng):
+        self.range = rng
+
     @property
     def attrs(self):
         return self._attrs
 
     @attrs.setter
     def attrs(self, attrs):
         self._attrs = dict(copy.deepcopy(attrs))
@@ -998,16 +1028,16 @@
         cls,
         expression,
         points_x,
         points_y,
         weights=None,
         params0=None,
         aux_params=None,
-        domain=DEFAULT_DOMAIN,
-        rng=DEFAULT_RANGE,
+        domain=None,
+        rng=None,
         fit_kwargs={},
         **attrs,
     ):
         """Create a Calibration with the expression and fit the points.
 
         Parameters
         ----------
@@ -1064,15 +1094,15 @@
         cal = cls(
             expression, params, aux_params=aux_params, domain=domain, rng=rng, **attrs
         )
         cal.set_points(points_x, points_y, weights)
         return cal
 
     @classmethod
-    def from_linear(cls, params, domain=DEFAULT_DOMAIN, rng=DEFAULT_RANGE, **attrs):
+    def from_linear(cls, params, domain=None, rng=None, **attrs):
         """Create a Calibration with a linear function.
 
         Parameters
         ----------
         params : array_like
             Coefficients beginning with 0th order.
         attrs : dict
@@ -1080,15 +1110,15 @@
         """
         expr = "p[0] + p[1] * x"
         if len(params) != 2:
             raise CalibrationError("Linear calibration expects 2 parameters")
         return cls(expr, params, domain=domain, rng=rng, **attrs)
 
     @classmethod
-    def from_polynomial(cls, params, domain=DEFAULT_DOMAIN, rng=DEFAULT_RANGE, **attrs):
+    def from_polynomial(cls, params, domain=None, rng=None, **attrs):
         """Create a Calibration with a polynomial function of any order.
 
         The calibration function expression is
             "p[0] + p[1] * x + p[2] * x**2 + ..."
 
         Parameters
         ----------
@@ -1097,17 +1127,15 @@
         attrs : dict
             Other information to be stored with the calibration.
         """
         expr = _polynomial_expression(params)
         return cls(expr, params, domain=domain, rng=rng, **attrs)
 
     @classmethod
-    def from_sqrt_polynomial(
-        cls, params, domain=DEFAULT_DOMAIN, rng=DEFAULT_RANGE, **attrs
-    ):
+    def from_sqrt_polynomial(cls, params, domain=None, rng=None, **attrs):
         """Create a square root of a polynomial function of any order.
 
         The calibration function expression is
             "np.sqrt(p[0] + p[1] * x + p[2] * x**2 + ...)"
 
         Parameters
         ----------
@@ -1117,17 +1145,15 @@
             Other information to be stored with the calibration.
         """
         expr = _polynomial_expression(params)
         expr = "np.sqrt(" + expr + ")"
         return cls(expr, params, domain=domain, rng=rng, **attrs)
 
     @classmethod
-    def from_interpolation(
-        cls, points_x, points_y, domain=DEFAULT_DOMAIN, rng=DEFAULT_RANGE, **attrs
-    ):
+    def from_interpolation(cls, points_x, points_y, domain=None, rng=None, **attrs):
         """Create a Calibration that interpolates the calibration points.
 
         Parameters
         ----------
         points_x : float or array_like
             The x-value or values of calibration points
         points_y : float or array_like
```

### Comparing `becquerel-0.5.0/becquerel/core/energycal.py` & `becquerel-0.6.0/becquerel/core/energycal.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,18 @@
 import matplotlib.pyplot as plt
 import warnings
 
 
 class EnergyCalError(Exception):
     """Base class for errors in energycal.py"""
 
-    pass
-
 
 class BadInput(EnergyCalError):
     """Error related to energy cal input"""
 
-    pass
-
 
 class EnergyCalBase:
     """Abstract base class for energy calibration.
 
     A note on nomenclature: for historic reasons, 'channels' is used in
     energycal.py for generic uncalibrated x-axis values. A 'channel' is no
     longer necessarily an integer channel number (i.e., bin) from a
@@ -214,16 +210,14 @@
         Args:
           ch: an np.array, float, or int of channel values
 
         Returns:
           energy values, the same size/type as ch [keV]
         """
 
-        pass
-
     def kev2ch(self, kev):
         """Convert energy value(s) to channel(s).
 
         Args:
           kev: a scalar, np.array, list or tuple of energy values [keV]
 
         Returns:
@@ -247,26 +241,23 @@
 
         Returns:
           the channel value(s) corresponding to the input energies.
             a float if input is scalar. an np.array if input is iterable
         """
 
         # if this is not possible, raise a NotImplementedError ?
-        pass
 
     @abstractproperty
     def valid_coeffs(self):
         """A list of valid coefficients for the calibration curve.
 
         Returns:
           a tuple of strings, the names of the coefficients for this curve
         """
 
-        pass
-
     def _set_coeff(self, name, val):
         """Set a coefficient for the calibration curve.
 
         Args:
           name: a string, the name of the coefficient to set
           val: the value to set the coefficient to
 
@@ -297,16 +288,14 @@
         else:
             self._perform_fit()
 
     @abstractmethod
     def _perform_fit(self):
         """Do the actual curve fitting."""
 
-        pass
-
     def plot(self, ax=None):
         """Plot the calibration.
 
         Parameters
         ----------
         ax : np.ndarray of shape (2,), or matplotlib axes object, optional
             Plot axes to use. If None, create new axes.
```

### Comparing `becquerel-0.5.0/becquerel/core/fitting.py` & `becquerel-0.6.0/becquerel/core/fitting.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     for c in ["C0", "C2", "C4", "C5", "C6", "C7", "C8", "C9"]
 ]
 
 
 class FittingError(Exception):
     """Exception raised by Fitters."""
 
-    pass
-
 
 class FittingWarning(UserWarning):
     """Warning raised by Fitters."""
 
 
 # -----------------------------------------------------------------------------
 # Base functions
@@ -68,14 +66,76 @@
 def expgauss(x, amp=1, mu=0, sigma=1.0, gamma=1.0):
     gss = gamma * sigma * sigma
     arg1 = gamma * (mu + gss / 2.0 - x)
     arg2 = (mu + gss - x) / (SQRT_TWO * sigma)
     return amp * (gamma / 2) * np.exp(arg1) * scipy.special.erfc(arg2)
 
 
+def gauss_dbl_exp(
+    x: np.ndarray,
+    amp: float,
+    mu: float,
+    sigma: float,
+    ltail_ratio: float,
+    ltail_slope: float,
+    ltail_cutoff: float,
+    rtail_ratio: float,
+    rtail_slope: float,
+    rtail_cutoff: float,
+):
+    """A Gaussian with exponential tails added to either side of the peak. This
+    is an extension of the Gaussian with a low-side exponential tail described
+    by Namboodiri et al here: https://www.osti.gov/biblio/392720
+
+    The function is suitable for spectra with asymmetric peaks, such as those
+    from CZT crystals. The exponential tails are characterized by 3 parameters: a
+    tail-to-peak amplitude ratio, a slope, and a cutoff parameter.
+
+    Parameters
+    ----------
+    x : numpy.ndarray
+        X-data
+    amp : float
+        Amplitude parameter
+    mu: float
+        Mean parameter
+    sigma: float
+        Width parameter
+    ltail_ratio: float
+        Left-side exponential tail amplitude / Amplitude
+    ltail_slope: float
+        Left-side exponential tail slope, affects "steepness" of the tail
+    ltail_cutoff: float
+        Left-side exponential tail cutoff, affects "length" of the tail
+    rtail_ratio: float
+        Right-side exponential tail amplitude / Amplitude
+    rtail_slope: float
+        Right-side exponential tail slope, affects "steepness" of the tail
+    rtail_cutoff: float
+        Right-side exponential tail cutoff, affects "length" of the tail
+
+    Returns
+    -------
+    numpy.ndarray
+        Y-data
+    """
+    alpha = -1.0 / (2.0 * sigma**2)
+    ltail_func = np.zeros(shape=(len(x),))
+    rtail_func = np.zeros(shape=(len(x),))
+    # l and r tail_func are 0 when we're below/above the Gaussian mean
+    # "heavyside convolution"
+    mask = x < mu
+    ltail_func[mask] = amp * ltail_ratio * np.exp(ltail_slope * ((x[mask] - mu)))
+    ltail_func[mask] *= -np.expm1(ltail_cutoff * alpha * ((x[mask] - mu) ** 2))
+    mask = x > mu
+    rtail_func[mask] = amp * rtail_ratio * np.exp(rtail_slope * ((x[mask] - mu)))
+    rtail_func[mask] *= -np.expm1(rtail_cutoff * alpha * ((x[mask] - mu) ** 2))
+    return amp * np.exp(alpha * ((x - mu) ** 2)) + ltail_func + rtail_func
+
+
 # -----------------------------------------------------------------------------
 # Custom loss functions
 # -----------------------------------------------------------------------------
 
 
 def poisson_loss(y_eval, y_data):
     return np.sum(y_eval - scipy.special.xlogy(y_data, y_eval))
@@ -325,22 +385,75 @@
             (f"{self.prefix}sigma", "value", sigma),
             (f"{self.prefix}sigma", "min", 0.0),
             (f"{self.prefix}gamma", "value", 0.95),
             (f"{self.prefix}gamma", "min", 0.0),
         ]
 
 
+class GaussDblExpModel(Model):
+    """This model is a Gaussian combined with exponential tails on either side
+    of the center of the distribution. Each tail is characterized by 3 parameters:
+    an amplitude ratio, a slope, and a cutoff. This is an extension of the peak
+    shape described by Namboodiri et al here: https://www.osti.gov/biblio/392720
+    to fit CZT energy spectra. In their case, the exponential tail was only on
+    the low side of the peak.
+
+    A distribution with the exponential tail on only one side may be obtained by
+    fixing the undesired side's parameters to 0.
+
+    The tail amplitudes are expressed as ratios with respect to the peak
+    amplitude (tail_amplitude / amplitude).
+
+    The slope parameter impacts how steep the tail is, and the cutoff parameter
+    impacts how far out it goes.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(gauss_dbl_exp, **kwargs)
+        self.set_param_hint(f"{self.prefix}amp", min=0)
+        self.set_param_hint(f"{self.prefix}mu", min=0)
+        self.set_param_hint(f"{self.prefix}sigma", min=0)
+        self.set_param_hint(f"{self.prefix}ltail_ratio", min=0)
+        self.set_param_hint(f"{self.prefix}rtail_ratio", min=0)
+
+    def guess(self, y, x=None, dx=None):
+        if x is None:
+            x = np.arange(0, len(y))
+        if dx is None:
+            dx = np.ones_like(x)
+        mu = np.mean(x)
+        amp = np.max(y)
+        return [
+            (f"{self.prefix}amp", "value", amp),
+            (f"{self.prefix}amp", "min", 0.0),
+            (f"{self.prefix}mu", "value", mu),
+            (f"{self.prefix}mu", "min", x[0]),
+            (f"{self.prefix}mu", "max", x[-1]),
+            (f"{self.prefix}sigma", "value", 1.0),
+            (f"{self.prefix}sigma", "min", 0.0),
+            (f"{self.prefix}ltail_ratio", "value", 0.1),
+            (f"{self.prefix}ltail_ratio", "min", 0.0),
+            (f"{self.prefix}ltail_slope", "value", 0.05),
+            (f"{self.prefix}ltail_cutoff", "value", 1.0),
+            (f"{self.prefix}rtail_ratio", "value", 0.1),
+            (f"{self.prefix}rtail_ratio", "min", 0.0),
+            (f"{self.prefix}rtail_slope", "value", -0.05),
+            (f"{self.prefix}rtail_cutoff", "value", 1.0),
+        ]
+
+
 MODEL_STR_TO_CLS = {
     "constant": ConstantModel,
     "line": LineModel,
     "gauss": GaussModel,
     "gausserf": GaussErfModel,
     "erf": ErfModel,
     "exp": ExpModel,
     "expgauss": ExpGaussModel,
+    "gaussdblexp": GaussDblExpModel,
 }
 
 
 def _parameters_to_bq_guess(params: Parameters):
     """Convert a Parameters object to the tuple format becquerel expects for guess().
 
     Parameters
@@ -617,14 +730,16 @@
 
     def _guess_param_defaults(self, **kwargs):
         params = []
         for comp in self.model.components:
             p = comp.guess(self.y_roi, x=self.x_roi, dx=self.dx_roi)
             if isinstance(p, Parameters):
                 p = _parameters_to_bq_guess(p)
+            elif p is None:
+                raise TypeError()
             params += p
         return params
 
     def guess_param_defaults(self, update=False, **kwargs):
         defaults = self._guess_param_defaults(**kwargs)
         if update:
             if defaults is not None:
@@ -826,15 +941,15 @@
                     "like this, using \"nan_policy='omit'\" will probably "
                     "not work."
                 )
                 raise ValueError(msg)
             mask = model <= 0  # This should not be necessary
             diff = model - scipy.special.xlogy(data, model)
             diff[mask] = 1e32
-            if diff.dtype == np.complex:
+            if np.issubdtype(diff.dtype, complex):
                 # data/model are complex
                 diff = diff.ravel().view(float)
             return np.asarray(diff).ravel()  # for compatibility with pandas.Series
 
         # This overwrites the  model residual method, is an ugly hack to make
         # poisson fitting possible. This is not undone for now.
         self.model._residual = _likelihood_residual.__get__(self.model, Model)
@@ -936,95 +1051,104 @@
         Value of fit parameter `param`
         """
         if self.result is None:
             return None
         if "lmfit" in self.backend:
             if param in self.result.params:
                 return self.result.params[param].value
-            elif param in self.fit.best_values:
+            elif param in self.result.best_values:
                 return self.result.best_values[param]
             else:
-                raise FittingError("Unknown param: {}", param)
+                raise FittingError(f"Unknown param: {param}")
         elif "minuit" in self.backend:
-            return self.result.params[param].value
-        else:
-            raise FittingError("Unknown backend: {}", self.backend)
+            if param in self.result.parameters:
+                return self.result.params[param].value
+            raise FittingError(f"Unknown param: {param}")
+        raise FittingError(f"Unknown backend: {self.backend}")
 
     def param_unc(self, param):
         """
         Fit error of fit parameter `param`
         """
         if self.result is None:
             return None
         if "lmfit" in self.backend:
             if param in self.result.params:
                 return self.result.params[param].stderr
             elif param in self.result.best_values:
                 # This is the case for the `erf_form` key
                 return np.nan
             else:
-                raise FittingError("Unknown param: {}", param)
+                raise FittingError(f"Unknown param: {param}")
         elif "minuit" in self.backend:
-            return self.result.params[param].error  # TODO minos vs hesse?
-        else:
-            raise FittingError("Unknown backend: {}", self.backend)
+            if param in self.result.parameters:
+                return self.result.params[param].error  # TODO minos vs hesse?
+            raise FittingError(f"Unknown param: {param}")
+        raise FittingError(f"Unknown backend: {self.backend}")
+
+    def param_rel_unc(self, param):
+        """
+        Relative error of fit parameter `param`
+        """
+        if self.param_unc(param):
+            return self.param_unc(param) / self.param_val(param)
+        return None
 
     @property
     def best_values(self):
         """Wrapper for dictionary of best_values."""
         if "lmfit" in self.backend:
             return self.result.best_values
         elif "minuit" in self.backend:
             return self._best_values
-        else:
-            raise FittingError("Unknown backend: {}", self.backend)
+        raise FittingError(f"Unknown backend: {self.backend}")
 
     @property
     def init_values(self):
         """Wrapper for dictionary of init_values."""
         if "lmfit" in self.backend:
             return self.result.init_values
         elif "minuit" in self.backend:
             return self._init_values
-        else:
-            raise FittingError("Unknown backend: {}", self.backend)
+        raise FittingError(f"Unknown backend: {self.backend}")
 
     @property
     def success(self):
         if "lmfit" in self.backend:
             return self.result.success
         elif "minuit" in self.backend:
             return self.result.valid
-        else:
-            raise FittingError("Unknown backend: {}", self.backend)
+        raise FittingError(f"Unknown backend: {self.backend}")
 
     @property
     def covariance(self):
         """Wrapper for fit covariance matrix."""
         if "lmfit" in self.backend:
             return self.result.covar
         elif "minuit" in self.backend:
             return self.result.covariance
-        else:
-            raise FittingError("Unknown backend: {}", self.backend)
+        raise FittingError(f"Unknown backend: {self.backend}")
 
     def param_dataframe(self, sort_by_model=False):
         """
         Dataframe of all fit parameters value and fit error
         """
         if self.result is None:
             return None
         df = pd.DataFrame(columns=["val", "unc"], dtype=float)
         for k in self.param_names:
             df.loc[k, "val"] = self.param_val(k)
             df.loc[k, "unc"] = self.param_unc(k)
         if sort_by_model:
             df.set_index(
                 pd.MultiIndex.from_tuples(
-                    [tuple(p.split("_")) for p in df.index], names=["model", "param"]
+                    # Only split on the first underscore, in case the param name
+                    # has an underscore in it
+                    [tuple(p.split("_", maxsplit=1)) for p in df.index],
+                    names=["model", "param"],
                 ),
                 inplace=True,
             )
         return df
 
     def compute_residuals(self, residual_type="abs"):
         """Compute residuals between the data and the fit.
```

### Comparing `becquerel-0.5.0/becquerel/core/peakfinder.py` & `becquerel-0.6.0/becquerel/core/peakfinder.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import warnings
 from .spectrum import Spectrum
 
 
 class PeakFilterError(Exception):
     """Base class for errors in PeakFilter."""
 
-    pass
-
 
 class PeakFilter:
     """An energy-dependent kernel that can be convolved with a spectrum.
 
     To detect lines, a kernel should have a positive component in the center
     and negative wings to subtract the continuum, e.g., a Gaussian or a boxcar:
 
@@ -144,22 +142,18 @@
         kernel = g1_x0 - g1_x1
         return kernel
 
 
 class PeakFinderError(Exception):
     """Base class for errors in PeakFinder."""
 
-    pass
-
 
 class PeakFinderWarning(UserWarning):
     """Warnings displayed during peak fitting."""
 
-    pass
-
 
 class PeakFinder:
     """Find peaks in a spectrum after convolving it with a kernel."""
 
     def __init__(self, spectrum, kernel, min_sep=5, fwhm_tol=(0.5, 1.5)):
         """Initialize with a spectrum and kernel."""
         if min_sep <= 0:
@@ -349,16 +343,39 @@
             )
 
         peak_index = np.where((self.snr == peak_snr) & x_range)[0][0]
         peak_x = bin_centers[peak_index]
         self.add_peak(peak_x)
         return peak_x
 
-    def find_peaks(self, xmin=None, xmax=None, min_snr=2, max_num=40):
-        """Find the highest SNR peaks in the data."""
+    def find_peaks(self, xmin=None, xmax=None, min_snr=2, max_num=40, reset=False):
+        """Find the highest SNR peaks in the data.
+
+        Parameters
+        ----------
+        xmin
+            Left edge of the x-range that should be scanned for
+            peaks. Uses min(x-range) if not given.
+        xmax
+            Right edge of the x-range that should be scanned for
+            peaks. Uses max(x-range) if not given.
+        min_snr
+            Minium SNR for a peak to be added
+        max_num
+            Maximum number of peaks to be added
+        reset
+            If true, reset the already found peaks. Useful when
+            changing `min_snr` and calling find_peaks again on the
+            same x-range.
+
+        """
+
+        if reset:
+            self.reset()
+
         bin_edges = self.spectrum.bin_edges_raw
         bin_centers = self.spectrum.bin_centers_raw
 
         if xmin is None:
             xmin = bin_edges.min()
         if xmax is None:
             xmax = bin_edges.max()
```

### Comparing `becquerel-0.5.0/becquerel/core/plotting.py` & `becquerel-0.6.0/becquerel/core/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from uncertainties import unumpy
 import warnings
 
 
 class PlottingError(Exception):
     """General exception for plotting.py"""
 
-    pass
-
 
 class SpectrumPlotter:
     """Class for handling spectrum plotting."""
 
     def __init__(self, spec, *fmt, **kwargs):
         """
         Args:
```

### Comparing `becquerel-0.5.0/becquerel/core/rebin.py` & `becquerel-0.6.0/becquerel/core/rebin.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 import numpy as np
 import warnings
 
 
 class RebinError(Exception):
     """Exception raised by rebin operations."""
 
-    pass
-
 
 class RebinWarning(UserWarning):
     """Warnings displayed by rebin operations."""
 
-    pass
-
 
 def _check_monotonic_increasing(arr, arr_name="array"):
     """Check that a numpy array is monotonically increasing.
 
     Args:
       arr: numpy array for checking
       arr_name: name of array, just for use in the AssertionError message
@@ -160,15 +156,15 @@
 
     N.B. Does not keep Poisson statistics
 
     Args:
       in_spectrum: iterable of input spectrum counts in each bin
       in_edges: iterable of input bin edges (len = len(in_spectrum) + 1)
       out_edges_no_rightmost: iterable of output bin edges
-                              (sans the rightmost bin)
+                              (sans the rightmost bin edge)
       slopes: the slopes of each histogram bin, with the lines drawn between
               each bin edge. (len = len(in_spectrum))
       out_spectrum: for nb.guvectorize; This is the return array, do not
                     actually give this as an arg when calling the function.
                     Same length as out_edges_no_rightmost due to signature.
 
     Returns:
@@ -274,14 +270,15 @@
 def rebin(
     in_spectra,
     in_edges,
     out_edges,
     method="interpolation",
     slopes=None,
     zero_pad_warnings=True,
+    include_overflows=False,
 ):
     """
     Spectra rebinning via deterministic or stochastic methods.
 
     Args:
         in_spectrum (np.ndarray): an ND array of input counts spectra
             [..., num_bins_in]
@@ -303,14 +300,17 @@
                 conversion results in a decimal precision loss.
         slopes (np.ndarray|None): (optional) an array of input bin slopes for
             quadratic interpolation (1D or 2D)
             (only applies for "interpolation" method)
             [num_spectra, num_bins_in + 1] or [num_bins_in + 1]
         zero_pad_warnings (boolean): warn when edge overlap results in
             appending empty bins
+        include_overflows (boolean): whether to include counts below
+            out_edges[0] and above out_edges[-1] in the first and last
+            of the "out" bins, respectively, or to discard them (default).
 
     Raises:
         AssertionError: for bad input arguments
 
     Returns:
         The rebinned spectrum/a
     """
@@ -358,16 +358,39 @@
     # Check for increasing bin structure
     _check_monotonic_increasing(in_edges, "in_edges")
     _check_monotonic_increasing(out_edges, "out_edges")
     # Check for bin structure overlap
     _check_any_overlap(in_edges, out_edges)
     if zero_pad_warnings:
         _check_partial_overlap(in_edges, out_edges)
+
+    # add an extra bin at each end if we don't want overflow counts in
+    # the first and last bins
+    if not include_overflows:
+        if not np.isfinite(out_edges[0]):
+            raise RebinError(
+                "Lowest output edge must be finite if not including overflows"
+            )
+        if not np.isfinite(out_edges[-1]):
+            raise RebinError(
+                "Highest output edge must be finite if not including overflows"
+            )
+        out_edges_temp = np.concatenate(
+            (np.array([-np.inf]), out_edges, np.array([np.inf]))
+        )
+    else:
+        out_edges_temp = out_edges
+
     # Remove highest output edge, necessary for guvectorize
-    out_edges = out_edges[..., :-1]
+    out_edges = out_edges_temp[..., :-1]
 
     # Specific calls to (wrapped) nb.guvectorize'd rebinning methods
     if method == "interpolation":
-        return _rebin_interpolation(in_spectra, in_edges, out_edges, slopes)
+        hist = _rebin_interpolation(in_spectra, in_edges, out_edges, slopes)
     elif method == "listmode":
-        return _rebin_listmode(in_spectra, in_edges, out_edges)
-    raise ValueError(f"{method} is not a valid rebinning method")
+        hist = _rebin_listmode(in_spectra, in_edges, out_edges)
+    else:
+        raise ValueError(f"{method} is not a valid rebinning method")
+
+    if not include_overflows:
+        hist = hist[..., 1:-1]
+    return hist
```

### Comparing `becquerel-0.5.0/becquerel/core/spectrum.py` & `becquerel-0.6.0/becquerel/core/spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,22 @@
 from . import fitting
 import warnings
 
 
 class SpectrumError(Exception):
     """Exception raised by Spectrum."""
 
-    pass
-
 
 class SpectrumWarning(UserWarning):
     """Warnings displayed by Spectrum."""
 
-    pass
-
 
 class UncalibratedError(SpectrumError):
     """Raised when an uncalibrated spectrum is treated as calibrated."""
 
-    pass
-
 
 class Spectrum:
     """
     Represents an energy spectrum.
 
     Initialize a Spectrum directly, or with Spectrum.from_file(filename), or
     with Spectrum.from_listmode(listmode_data).
@@ -563,37 +557,60 @@
             raise SpectrumError("Bad length of bin edges vector")
         elif np.any(np.diff(bin_edges_raw) <= 0):
             raise ValueError("Raw bin edges must be strictly increasing")
         else:
             self._bin_edges_raw = np.array(bin_edges_raw, dtype=float)
 
     @classmethod
-    def from_file(cls, infilename, verbose=False):
+    def from_file(cls, infilename, verbose=False, cal_kwargs=None):
         """Construct a Spectrum object from a filename.
 
         Args:
           infilename: a string representing the path to a parsable file
           verbose: (optional) whether to print debugging information.
+          cal_kwargs: (optional) kwargs to override the file Calibration.
 
         Returns:
           A Spectrum object
 
         Raises:
           AssertionError: for a bad filename  # TODO make this an IOError
         """
         # read the data using one of the low-level parsers
         _, ext = os.path.splitext(infilename)
         if io.h5.is_h5_filename(infilename):
-            data, cal = parsers.h5.read(infilename, verbose=verbose)
+            data, cal = parsers.h5.read(
+                infilename,
+                verbose=verbose,
+                cal_kwargs=cal_kwargs,
+            )
         elif ext.lower() == ".cnf":
-            data, cal = parsers.cnf.read(infilename, verbose=verbose)
+            data, cal = parsers.cnf.read(
+                infilename,
+                verbose=verbose,
+                cal_kwargs=cal_kwargs,
+            )
         elif ext.lower() == ".spc":
-            data, cal = parsers.spc.read(infilename, verbose=verbose)
+            data, cal = parsers.spc.read(
+                infilename,
+                verbose=verbose,
+                cal_kwargs=cal_kwargs,
+            )
         elif ext.lower() == ".spe":
-            data, cal = parsers.spe.read(infilename, verbose=verbose)
+            data, cal = parsers.spe.read(
+                infilename,
+                verbose=verbose,
+                cal_kwargs=cal_kwargs,
+            )
+        elif ext.lower() == ".iec":
+            data, cal = parsers.iec1455.read(
+                infilename,
+                verbose=verbose,
+                cal_kwargs=cal_kwargs,
+            )
         else:
             raise NotImplementedError(f"File type {ext} can not be read")
 
         # create the object and apply the calibration
         spec = cls(**data)
         spec.attrs["infilename"] = infilename
         if cal is not None:
@@ -630,14 +647,19 @@
         attrs = deepcopy(self.attrs)
         # convert time attributes to strings
         for key in ["start_time", "stop_time"]:
             val = getattr(self, key)
             if val is not None:
                 iso8601 = f"{val:%Y-%m-%dT%H:%M:%S.%f%z}"
                 attrs.update({key: iso8601})
+        for key in ["sample_collection_time"]:
+            if key in attrs:
+                val = attrs[key]
+                iso8601 = f"{val:%Y-%m-%dT%H:%M:%S.%f%z}"
+                attrs.update({key: iso8601})
         for key in ["livetime", "realtime"]:
             val = getattr(self, key)
             if val is not None:
                 attrs.update({key: val})
         # cannot specify all three of start, stop, and real time
         if "start_time" in attrs and "stop_time" in attrs and "realtime" in attrs:
             attrs.pop("realtime")
@@ -1135,23 +1157,23 @@
     def apply_calibration(self, cal):
         """Use a Calibration to generate bin edge energies for this spectrum.
 
         Args:
           cal: a Calibration object
         """
 
-        try:
+        if hasattr(cal, "ch2kev") and callable(getattr(cal, "ch2kev")):
             self.bin_edges_kev = cal.ch2kev(self.bin_edges_raw)
             warnings.warn(
                 "The use of bq.EnergyCalBase classes is deprecated "
                 "and will be removed in a future release; "
                 "use bq.Calibration instead",
                 DeprecationWarning,
             )
-        except AttributeError:
+        else:
             self.bin_edges_kev = cal(self.bin_edges_raw)
         self.energy_cal = cal
 
     def calibrate_like(self, other):
         """Apply another Spectrum object's calibration (bin edges vector).
 
         Bin edges are copied, so the two spectra do not have the same object
@@ -1220,15 +1242,20 @@
             "bin_edges_kev": combined_bin_edges,
             "livetime": self.livetime,
         }
         obj = Spectrum(**kwargs)
         return obj
 
     def rebin(
-        self, out_edges, method="interpolation", slopes=None, zero_pad_warnings=True
+        self,
+        out_edges,
+        method="interpolation",
+        slopes=None,
+        zero_pad_warnings=True,
+        include_overflows=False,
     ):
         """
         Spectra rebinning via deterministic or stochastic methods.
 
         Args:
             out_edges (np.ndarray): an array of the output bin edges
                 [num_bins_out]
@@ -1237,16 +1264,19 @@
                     Deterministic interpolation
                 "listmode"
                     Stochastic rebinning via conversion to listmode of energies
             slopes (np.ndarray|None): (optional) an array of input bin slopes
                 for quadratic interpolation
                 (only applies for "interpolation" method)
                 [len(spectrum) + 1]
-        zero_pad_warnings (boolean): warn when edge overlap results in
-            appending empty bins
+            zero_pad_warnings (boolean): warn when edge overlap results in
+                appending empty bins
+            include_overflows (boolean): whether to include counts below
+                out_edges[0] and above out_edges[-1] in the first and last
+                of the "out" bins, respectively, or to discard them (default).
 
         Raises:
             SpectrumError: for bad input arguments
 
         Returns:
             A new Spectrum object with the rebinned data.
         """
@@ -1265,14 +1295,15 @@
         out_spec = rebin(
             in_spec,
             self.bin_edges_kev,
             out_edges,
             method=method,
             slopes=slopes,
             zero_pad_warnings=zero_pad_warnings,
+            include_overflows=include_overflows,
         )
         return Spectrum(
             counts=out_spec,
             uncs=np.sqrt(out_spec),
             bin_edges_kev=out_edges,
             livetime=self.livetime,
         )
```

### Comparing `becquerel-0.5.0/becquerel/core/utils.py` & `becquerel-0.6.0/becquerel/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 VECTOR_TYPES = (list, tuple, np.ndarray)
 
 
 class UncertaintiesError(Exception):
     """Raised when uncertainties are badly specified in an input."""
 
-    pass
-
 
 def all_ufloats(x):
     """Check if every element of x is a UFloat.
 
     Args:
       x: an iterable or scalar to check
```

### Comparing `becquerel-0.5.0/becquerel/io/h5.py` & `becquerel-0.6.0/becquerel/io/h5.py`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/becquerel/parsers/cnf.py` & `becquerel-0.6.0/becquerel/parsers/cnf.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,23 +71,25 @@
     for i in range(4):
         coeff[i] = _from_pdp11(data, index + 2 * 4 + 28 + 4 * i)
     if coeff[1] == 0.0:
         return None
     return coeff
 
 
-def read(filename, verbose=False):
+def read(filename, verbose=False, cal_kwargs=None):
     """Parse the CNF file and return a dictionary of data.
 
     Parameters
     ----------
     filename : str
         The filename of the CNF file to read.
     verbose : bool (optional)
         Whether to print out debugging information. By default False.
+    cal_kwargs : dict or None (optional)
+        Kwargs to override the Calibration parameters read from file.
 
     Returns
     -------
     data : dict
         Dictionary of data that can be used to instantiate a Spectrum.
     cal : Calibration
         Energy calibration stored in the file.
@@ -294,10 +296,12 @@
     for key in data.keys():
         if isinstance(data[key], str):
             data[key] = data[key].replace("\x00", " ")
             data[key] = data[key].replace("\x01", " ")
             data[key] = data[key].strip()
 
     # create an energy calibration object
-    cal = calibration.Calibration.from_polynomial(cal_coeff)
+    if cal_kwargs is None:
+        cal_kwargs = {}
+    cal = calibration.Calibration.from_polynomial(cal_coeff, **cal_kwargs)
 
     return data, cal
```

### Comparing `becquerel-0.5.0/becquerel/parsers/h5.py` & `becquerel-0.6.0/becquerel/parsers/h5.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Read in a becquerel Spectrum HDF5 file."""
 
 from .. import io
 from ..core import calibration
-from .parsers import BecquerelParserError
+from .parsers import BecquerelParserError, override_calibration
 
 
-def read(filename, verbose=False):
+def read(filename, verbose=False, cal_kwargs=None):
     """Parse the becquerel Spectrum HDF5 file and return a dictionary of data.
 
     Parameters
     ----------
     filename : str
         The filename of the HDF5 file to read.
     verbose : bool (optional)
         Whether to print out debugging information. By default False.
+    cal_kwargs : dict or None (optional)
+        Kwargs to override the Calibration parameters read from file.
 
     Returns
     -------
     data : dict
         Dictionary of data that can be used to instantiate a Spectrum.
     cal : Calibration
         Energy calibration stored in the file.
@@ -27,15 +29,18 @@
         raise BecquerelParserError("File is not an HDF5: " + filename)
 
     # group datasets and attributes into one dictionary
     dsets, attrs, skipped = io.h5.read_h5(filename)
     data = {**dsets, **attrs}
 
     # read energy calibration from file
+    if cal_kwargs is None:
+        cal_kwargs = {}
     if "energy_cal" in skipped:
         with io.h5.open_h5(filename, "r") as h5:
             group = h5["energy_cal"]
             cal = calibration.Calibration.read(group)
+            cal = override_calibration(cal, **cal_kwargs)
     else:
         cal = None
 
     return data, cal
```

### Comparing `becquerel-0.5.0/becquerel/parsers/spc.py` & `becquerel-0.6.0/becquerel/parsers/spc.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         ["Calibration parameter 0", "f"],
         ["Calibration parameter 1", "f"],
         ["Calibration parameter 2", "f116x"],
     ],
 ]
 
 
-def read(filename, verbose=False):
+def read(filename, verbose=False, cal_kwargs=None):
     """Parse the binary SPC file and return a dictionary of data.
 
     ORTEC's SPC file format is divided into records of 128 bytes each. The
     specifications for what each record should contain can be found on pages
     29--44 of this document:
         http://www.ortec-online.com/download/ortec-software-file-structure-manual.pdf
 
@@ -193,14 +193,16 @@
 
     Parameters
     ----------
     filename : str
         The filename of the CNF file to read.
     verbose : bool (optional)
         Whether to print out debugging information. By default False.
+    cal_kwargs : dict or None (optional)
+        Kwargs to override the Calibration parameters read from file.
 
     Returns
     -------
     data : dict
         Dictionary of data that can be used to instantiate a Spectrum.
     cal : Calibration
         Energy calibration stored in the file.
@@ -389,10 +391,12 @@
     for key in data.keys():
         if isinstance(data[key], str):
             data[key] = data[key].replace("\x00", " ")
             data[key] = data[key].replace("\x01", " ")
             data[key] = data[key].strip()
 
     # create an energy calibration object
-    cal = calibration.Calibration.from_polynomial(cal_coeff)
+    if cal_kwargs is None:
+        cal_kwargs = {}
+    cal = calibration.Calibration.from_polynomial(cal_coeff, **cal_kwargs)
 
     return data, cal
```

### Comparing `becquerel-0.5.0/becquerel/parsers/spe.py` & `becquerel-0.6.0/becquerel/parsers/spe.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import warnings
 import dateutil.parser
 import numpy as np
 from ..core import calibration
 from .parsers import BecquerelParserError, BecquerelParserWarning
 
 
-def read(filename, verbose=False):
+def read(filename, verbose=False, cal_kwargs=None):
     """Parse the ASCII SPE file and return a dictionary of data.
 
     ORTEC's SPE file format is given on page 73 of this document:
         http://www.ortec-online.com/download/ortec-software-file-structure-manual.pdf
 
     Parameters
     ----------
     filename : str
         The filename of the CNF file to read.
     verbose : bool (optional)
         Whether to print out debugging information. By default False.
+    cal_kwargs : dict or None (optional)
+        Kwargs to override the Calibration parameters read from file.
 
     Returns
     -------
     data : dict
         Dictionary of data that can be used to instantiate a Spectrum.
     cal : Calibration
         Energy calibration stored in the file.
@@ -123,12 +125,14 @@
     # finish populating data dict
     data["realtime"] = realtime
     data["livetime"] = livetime
     data["start_time"] = collection_start
     data["counts"] = counts
 
     # create an energy calibration object
+    if cal_kwargs is None:
+        cal_kwargs = {}
     cal = None
     if len(cal_coeff) > 0 and not np.allclose(cal_coeff, 0):
-        cal = calibration.Calibration.from_polynomial(cal_coeff)
+        cal = calibration.Calibration.from_polynomial(cal_coeff, **cal_kwargs)
 
     return data, cal
```

### Comparing `becquerel-0.5.0/becquerel/tools/__init__.py` & `becquerel-0.6.0/becquerel/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/becquerel/tools/_nndc_dummy_text.py` & `becquerel-0.6.0/becquerel/tools/_nndc_dummy_text.py`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/becquerel/tools/df_cache.py` & `becquerel-0.6.0/becquerel/tools/df_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import os
 import pandas as pd
 
 
 class CacheError(Exception):
     """Problem fetching, saving, or retrieving cached data."""
 
-    pass
-
 
 class DataFrameCache:
     """Abstract base class for downloading, saving, and retrieving a DataFrame.
 
     Abstract methods:
       fetch: retrieve the DataFrame from a source.
```

### Comparing `becquerel-0.5.0/becquerel/tools/element.py` & `becquerel-0.6.0/becquerel/tools/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,34 +152,26 @@
 _MASS_FROM_Z = {d[0]: d[3] for d in _Z_SYMBOL_NAME_MASS}
 _MASS_FROM_SYMBOL = {d[1]: d[3] for d in _Z_SYMBOL_NAME_MASS}
 
 
 class ElementError(Exception):
     """Problem with element properties."""
 
-    pass
-
 
 class ElementZError(ElementError):
     """Bad element Z value."""
 
-    pass
-
 
 class ElementSymbolError(ElementError):
     """Bad element symbol."""
 
-    pass
-
 
 class ElementNameError(ElementError):
     """Bad element name."""
 
-    pass
-
 
 def validated_z(z):
     """Convert z into a valid element atomic number.
 
     Args:
       z: numeric or string type representing the atomic number Z.
```

### Comparing `becquerel-0.5.0/becquerel/tools/isotope.py` & `becquerel-0.6.0/becquerel/tools/isotope.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 N_AV = 6.022141e23  # mol^-1
 
 
 class IsotopeError(element.ElementError):
     """Problem with isotope properties."""
 
-    pass
-
 
 def _split_element_mass(arg):
     """Split a string into an element name/symbol plus a mass number/isomer.
 
     For example, the string 'TC99M' would be split into ('TC', '99M'), the
     string '238U' would be split into ('U', '238'), and the string 'Hf-178m3'
     would be split into ('Hf', '178m3').
```

### Comparing `becquerel-0.5.0/becquerel/tools/isotope_qty.py` & `becquerel-0.6.0/becquerel/tools/isotope_qty.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 UCI_TO_BQ = 3.7e4
 N_AV = 6.022141e23
 
 
 class IsotopeQuantityError(Exception):
     """Raised by the IsotopeQuantity class"""
 
-    pass
-
 
 def handle_isotope(isotope, error_name=None):
     """Handle string or Isotope input.
 
     Args:
       isotope: either a string of an isotope name, or an Isotope object
 
@@ -60,24 +58,26 @@
       half_life: the half life of the isotope, in seconds
       decay_const: the decay constant of the isotope, in 1/seconds
       is_stable: bool representing whether the isotope is considered stable
       ref_date: a datetime object representing the reference date/time
       ref_atoms: the number of atoms of the isotope, at the reference time.
 
     Methods:
-      atoms_at: number of atoms at given time
-      bq_at: activity in Bq at given time
-      uci_at: activity in uCi at given time
-      g_at: mass in grams at given time
-      atoms_now, bq_now, uci_now, g_now: quantity at current time
+      atoms_at: number of atoms at given time, defaults to system time
+      bq_at: activity in Bq at given time, defaults to system time
+      uci_at: activity in uCi at given time, defaults to system time
+      g_at: mass in grams at given time, defaults to system time
       decays_from: number of decays during a time interval
       bq_from, uci_from: average activity during a time interval
       decays_during: number of decays during a Spectrum measurement
       bq_during, uci_during: average activity during a Spectrum measurement
       time_when: time at which activity or mass equals a given value
+
+    Deprecated:
+      atoms_now, bq_now, uci_now, g_now: quantity at current time (use *_at(None))
     """
 
     def __init__(self, isotope, date=None, stability=1e18, **kwargs):
         """Initialize.
 
         Specify one of bq, uci, atoms, g to define the quantity.
 
@@ -157,24 +157,32 @@
         if ("bq" in kwargs or "uci" in kwargs) and self.is_stable:
             raise IsotopeQuantityError(
                 "Cannot initialize a stable IsotopeQuantity from activity"
             )
 
         # dictionary with functions that define how to calculate all quantities
         # in a circular manner
-        conversions = dict(
-            atoms=lambda: ref_quantities["g"] / self.isotope.A * N_AV,
-            bq=lambda: ref_quantities["atoms"] * self.decay_const,
-            uci=lambda: ref_quantities["bq"] / UCI_TO_BQ,
-            g=lambda: ref_quantities["uci"]
-            * UCI_TO_BQ
-            / self.decay_const
-            / N_AV
-            * self.isotope.A,
-        )
+        if self.is_stable:
+            conversions = dict(
+                atoms=lambda: ref_quantities["g"] / self.isotope.A * N_AV,
+                g=lambda: ref_quantities["atoms"] * self.isotope.A / N_AV,
+                bq=lambda: 0,
+                uci=lambda: 0,
+            )
+        else:
+            conversions = dict(
+                atoms=lambda: ref_quantities["g"] / self.isotope.A * N_AV,
+                bq=lambda: ref_quantities["atoms"] * self.decay_const,
+                uci=lambda: ref_quantities["bq"] / UCI_TO_BQ,
+                g=lambda: ref_quantities["uci"]
+                * UCI_TO_BQ
+                / self.decay_const
+                / N_AV
+                * self.isotope.A,
+            )
 
         # rotates the order of the list so that the provided kwarg is at [0]
         order = ["atoms", "bq", "uci", "g"]
         if next(iter(kwargs)) not in order:
             raise IsotopeQuantityError("Unknown isotope quantity.")
         while order[0] not in kwargs:
             order.append(order.pop(0))
@@ -279,15 +287,17 @@
 
         Raises:
           TypeError: if date is not recognized
         """
         date = date if date is not None else datetime.datetime.now()
         t1 = utils.handle_datetime(date)
         dt = (t1 - self.ref_date).total_seconds()
-        return self._ref_quantities[quantity] * np.exp(-dt * self.decay_const)
+        # here we use expm1, to use the same function consistently
+        # different numpy functions that could have different numerical precisions
+        return self._ref_quantities[quantity] * (np.expm1(-dt * self.decay_const) + 1.0)
 
     def atoms_at(self, date=None):
         """Calculate the number of atoms at a given time.
 
         Args:
           date: the date to calculate for (default now)
 
@@ -548,16 +558,14 @@
                 abs(a), abs(b)
             )
 
 
 class NeutronIrradiationError(Exception):
     """Exception from NeutronIrradiation class."""
 
-    pass
-
 
 class NeutronIrradiation:
     """Represents an irradiation period with thermal neutrons.
 
     Data attributes:
       start_time: beginning of irradiation
       stop_time: end of irradiation
@@ -622,15 +630,15 @@
         if self.duration == 0:
             return f"{self.n_cm2} neutrons/cm2 at {self.start_time}"
         else:
             return "{} n/cm2/s from {} to {}".format(
                 self.n_cm2_s, self.start_time, self.stop_time
             )
 
-    def activate(self, barns, initial, activated):
+    def activate(self, barns, initial, activated, stability=1e18):
         """
         Calculate an IsotopeQuantity from before or after a neutron activation.
 
         For a forward calculation (known initial quantity, to calculate the
         activated result), specify an initial IsotopeQuantity and an
         activated Isotope.
 
@@ -692,15 +700,15 @@
             )
         else:
             raise TypeError(
                 "Input args should be Isotope or IsotopeQuantity objects: "
                 + f"{initial}, {activated}"
             )
 
-        if not initial.is_stable:
+        if not initial.half_life > stability:
             raise NotImplementedError(
                 "Activation not implemented for a radioactive initial isotope"
             )
 
         cross_section = barns * 1.0e-24
 
         if forward:
```

### Comparing `becquerel-0.5.0/becquerel/tools/materials.py` & `becquerel-0.6.0/becquerel/tools/materials.py`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/becquerel/tools/materials_compendium.py` & `becquerel-0.6.0/becquerel/tools/materials_compendium.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 import json
 import os
 import warnings
 import numpy as np
 import pandas as pd
-from .materials_error import MaterialsWarning
+from .materials_error import MaterialsWarning, MaterialsError
 
 FNAME = os.path.join(os.path.split(__file__)[0], "MaterialsCompendium.json")
 
 
 def json_elements_to_weight_fractions(elements):
     """Calculate element weight fractions from the Elements data."""
     results = []
@@ -56,14 +56,31 @@
         )
         data = []
     else:
         with open(FNAME, "r") as f:
             data = json.load(f)
 
     # extract relevant data
+    if isinstance(data, list):
+        print("Pre-March 2022 JSON detected")
+    elif isinstance(data, dict):
+        print("Post-March 2022 JSON detected")
+        if "siteVersion" not in data.keys() or "data" not in data.keys():
+            raise MaterialsError(
+                "Attempt to read Compendium JSON failed; "
+                "dictionary must have keys 'siteVersion' "
+                "and 'data' but have keys " + str(list(data.keys()))
+            )
+        print(f"Compendium data - site version: {data['siteVersion']}")
+        data = data["data"]
+    else:
+        raise MaterialsError(
+            "Attempt to read Compendium JSON failed; "
+            "object must be a list or dict but is a " + str(type(data))
+        )
     names = [datum["Name"] for datum in data]
     formulae = [datum["Formula"] if "Formula" in datum else "-" for datum in data]
     densities = [datum["Density"] for datum in data]
     weight_fracs = [
         json_elements_to_weight_fractions(datum["Elements"]) for datum in data
     ]
```

### Comparing `becquerel-0.5.0/becquerel/tools/materials_nist.py` & `becquerel-0.6.0/becquerel/tools/materials_nist.py`

 * *Files identical despite different names*

### Comparing `becquerel-0.5.0/becquerel/tools/nndc.py` & `becquerel-0.6.0/becquerel/tools/nndc.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,32 +85,26 @@
     "a": "A",
 }
 
 
 class NNDCError(Exception):
     """General NNDC request error."""
 
-    pass
-
 
 class NoDataFound(NNDCError):
     """No datasets were found within the specified search."""
 
 
 class NNDCInputError(NNDCError):
     """Error related to the user input to an NNDC query."""
 
-    pass
-
 
 class NNDCRequestError(NNDCError):
     """Error related to communicating with NNDC or parsing the result."""
 
-    pass
-
 
 def _parse_headers(headers):
     """Parse table headers and ensure they are unique.
 
     Args:
       headers: a list of column header strings.
```

### Comparing `becquerel-0.5.0/becquerel/tools/wallet_cache.py` & `becquerel-0.6.0/becquerel/tools/wallet_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,16 +53,17 @@
         super().read_file()
         for col in ["Abundance (%)", "Mass Excess (MeV)"]:
             self.df[col] = self.df[col].apply(convert_float_ufloat)
 
     def fetch(self):
         """Fetch wallet card data from NNDC for all isotopes."""
 
-        self.df = pd.DataFrame()
+        dfs = []
         z_edges = (0, 40, 80, 120)
         for z0, z1 in zip(z_edges[:-1], z_edges[1:]):
             df_chunk = nndc.fetch_wallet_card(z_range=(z0, z1 - 1))
-            self.df = self.df.append(df_chunk)
+            dfs.append(df_chunk)
+        self.df = pd.concat(dfs)
         self.loaded = True
 
 
 wallet_cache = WalletCardCache()
```

### Comparing `becquerel-0.5.0/becquerel/tools/xcom.py` & `becquerel-0.6.0/becquerel/tools/xcom.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
 # Dictionary of data that will be posted to URL
 _DATA = {
     "NumAdd": "1",  # always '1'?
     "Energies": "",  # additional energies separated by ; (MeV)
     "WindowXmin": "0.001",  # lower limit of energy grid (MeV)
     "WindowXmax": "100",  # upper limit of energy grid (MeV)
-    "Output": "",  # 'on' for standard energy grid
     "OutOpt": "PIC",  # return cross sections in cm^2/g
     "ResizeFlag": "on",  # seems to determine whether Xmin and Xmax are used
 }
 
 # abbreviated names for the table columns (these are used in the dataframe)
 COLUMNS_SHORT = [
     "energy",
@@ -100,28 +99,22 @@
     "total_wo_coh": "Total Attenuation without Coherent Scattering",
 }
 
 
 class XCOMError(Exception):
     """General XCOM error."""
 
-    pass
-
 
 class XCOMInputError(XCOMError):
     """Error related to the user input to XCOMQuery."""
 
-    pass
-
 
 class XCOMRequestError(XCOMError):
     """Error related to communicating with XCOM or parsing the result."""
 
-    pass
-
 
 class _XCOMQuery:
     """Query photon cross section data from NIST XCOM database.
 
     After the data have been successfully queried, they are stored in a
     pandas DataFrame that is accessible through this class's methods.
 
@@ -433,15 +426,15 @@
             a problem parsing the data.
 
         """
         if self._method not in ["1", "2", "3"]:
             raise XCOMInputError(
                 "XCOM search method not set. Need to call update() method."
             )
-        if self._data["Energies"] == "" and self._data["Output"] == "":
+        if self._data["Energies"] == "" and "Output" not in self._data:
             raise XCOMInputError("No energies_kev or e_range_kev requested.")
         # submit the query
         self._request()
         # package the output into a pandas DataFrame
         self._parse_text()
         # convert energy from MeV to keV
         self.df["energy"] *= 1000.0
```

### Comparing `becquerel-0.5.0/becquerel.egg-info/PKG-INFO` & `becquerel-0.6.0/becquerel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: becquerel
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools for radiation spectral analysis.
 Home-page: https://github.com/lbl-anp/becquerel
 Maintainer: The Becquerel Development Team
 Maintainer-email: becquerel-dev@lbl.gov
 License: Other/Proprietary License (see LICENSE.txt)
 Download-URL: https://github.com/lbl-anp/becquerel/releases
 Platform: any
```

### Comparing `becquerel-0.5.0/becquerel.egg-info/SOURCES.txt` & `becquerel-0.6.0/becquerel.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 becquerel/core/spectrum.py
 becquerel/core/utils.py
 becquerel/io/__init__.py
 becquerel/io/h5.py
 becquerel/parsers/__init__.py
 becquerel/parsers/cnf.py
 becquerel/parsers/h5.py
+becquerel/parsers/iec1455.py
 becquerel/parsers/parsers.py
 becquerel/parsers/spc.py
 becquerel/parsers/spe.py
 becquerel/tools/__init__.py
 becquerel/tools/_nndc_dummy_text.py
 becquerel/tools/df_cache.py
 becquerel/tools/element.py
@@ -43,8 +44,9 @@
 becquerel/tools/isotope_qty.py
 becquerel/tools/materials.py
 becquerel/tools/materials_compendium.py
 becquerel/tools/materials_error.py
 becquerel/tools/materials_nist.py
 becquerel/tools/nndc.py
 becquerel/tools/wallet_cache.py
-becquerel/tools/xcom.py
+becquerel/tools/xcom.py
+tests/test_utils.py
```

### Comparing `becquerel-0.5.0/setup.py` & `becquerel-0.6.0/setup.py`

 * *Files identical despite different names*

