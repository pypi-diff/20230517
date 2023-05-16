# Comparing `tmp/QETpy-1.6.2.tar.gz` & `tmp/QETpy-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QETpy-1.6.2.tar", last modified: Wed Mar  1 20:18:35 2023, max compression
+gzip compressed data, was "QETpy-1.6.3.tar", last modified: Tue May 16 23:37:54 2023, max compression
```

## Comparing `QETpy-1.6.2.tar` & `QETpy-1.6.3.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.702039 QETpy-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-01 20:18:26.000000 QETpy-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-01 20:18:35.702039 QETpy-1.6.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.698039 QETpy-1.6.2/QETpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-01 20:18:35.000000 QETpy-1.6.2/QETpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-01 20:18:35.000000 QETpy-1.6.2/QETpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:18:35.000000 QETpy-1.6.2/QETpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:18:35.000000 QETpy-1.6.2/QETpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-01 20:18:35.000000 QETpy-1.6.2/QETpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 20:18:35.000000 QETpy-1.6.2/QETpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-03-01 20:18:26.000000 QETpy-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-01 20:18:26.000000 QETpy-1.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.698039 QETpy-1.6.2/qetpy/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.698039 QETpy-1.6.2/qetpy/core/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_de_pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)    87160 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    30711 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_iv.py
--rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_of_1x1.py
--rw-r--r--   0 runner    (1001) docker     (123)    35613 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_of_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33107 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_of_nonlin.py
--rw-r--r--   0 runner    (1001) docker     (123)    49337 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_of_nsmb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/_of_pileup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.698039 QETpy-1.6.2/qetpy/core/didv/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/didv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36620 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/didv/_base_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    29423 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/didv/_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/didv/_didv_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/core/didv/_plot_didv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.702039 QETpy-1.6.2/qetpy/cut/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/cut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/cut/_cut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.702039 QETpy-1.6.2/qetpy/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/plotting/_fitting_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/plotting/_ibis_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/plotting/_iv_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/plotting/_noise_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/plotting/_of_nsmb_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.702039 QETpy-1.6.2/qetpy/sim/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28269 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/sim/_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.702039 QETpy-1.6.2/qetpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-03-01 20:18:26.000000 QETpy-1.6.2/qetpy/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 20:18:35.702039 QETpy-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-01 20:18:26.000000 QETpy-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:18:35.702039 QETpy-1.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-03-01 20:18:27.000000 QETpy-1.6.2/test/test_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-03-01 20:18:27.000000 QETpy-1.6.2/test/test_detcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-03-01 20:18:27.000000 QETpy-1.6.2/test/test_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-03-01 20:18:27.000000 QETpy-1.6.2/test/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-03-01 20:18:27.000000 QETpy-1.6.2/test/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-03-01 20:18:27.000000 QETpy-1.6.2/test/test_ofnsmb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-03-01 20:18:27.000000 QETpy-1.6.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-16 23:37:42.000000 QETpy-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-16 23:37:54.079904 QETpy-1.6.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.075904 QETpy-1.6.3/QETpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-16 23:37:54.000000 QETpy-1.6.3/QETpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-16 23:37:54.000000 QETpy-1.6.3/QETpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:37:54.000000 QETpy-1.6.3/QETpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:37:54.000000 QETpy-1.6.3/QETpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 23:37:54.000000 QETpy-1.6.3/QETpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 23:37:54.000000 QETpy-1.6.3/QETpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-16 23:37:42.000000 QETpy-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 23:37:43.000000 QETpy-1.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.075904 QETpy-1.6.3/qetpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/qetpy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_de_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87160 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30711 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_iv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_of_1x1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35613 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_of_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33107 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_of_nonlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49337 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_of_nsmb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/_of_pileup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/qetpy/core/didv/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/didv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46735 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/didv/_base_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34615 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/didv/_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/didv/_didv_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/didv/_plot_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/didv/_templates_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56290 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/core/didv/_uncertainties_didv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/qetpy/cut/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/cut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83142 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/cut/_cut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/qetpy/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/plotting/_fitting_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/plotting/_ibis_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/plotting/_iv_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/plotting/_noise_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/plotting/_of_nsmb_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/qetpy/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28269 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/sim/_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/qetpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32582 2023-05-16 23:37:43.000000 QETpy-1.6.3/qetpy/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:37:54.079904 QETpy-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-16 23:37:43.000000 QETpy-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:37:54.079904 QETpy-1.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-16 23:37:44.000000 QETpy-1.6.3/test/test_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-16 23:37:44.000000 QETpy-1.6.3/test/test_detcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-16 23:37:44.000000 QETpy-1.6.3/test/test_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-05-16 23:37:44.000000 QETpy-1.6.3/test/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-16 23:37:44.000000 QETpy-1.6.3/test/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-16 23:37:44.000000 QETpy-1.6.3/test/test_ofnsmb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-16 23:37:44.000000 QETpy-1.6.3/test/test_utils.py
```

### Comparing `QETpy-1.6.2/LICENSE` & `QETpy-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/PKG-INFO` & `QETpy-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QETpy
-Version: 1.6.2
+Version: 1.6.3
 Summary: TES Detector Calibration and Analysis Python Tools
 Home-page: https://github.com/spice-herald/QETpy
 Author: Samuel Watkins, Caleb Fink
 Author-email: samwatkins@berkeley.edu, cwfink@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `QETpy-1.6.2/QETpy.egg-info/PKG-INFO` & `QETpy-1.6.3/QETpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QETpy
-Version: 1.6.2
+Version: 1.6.3
 Summary: TES Detector Calibration and Analysis Python Tools
 Home-page: https://github.com/spice-herald/QETpy
 Author: Samuel Watkins, Caleb Fink
 Author-email: samwatkins@berkeley.edu, cwfink@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `QETpy-1.6.2/QETpy.egg-info/SOURCES.txt` & `QETpy-1.6.3/QETpy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 qetpy/core/_of_nsmb.py
 qetpy/core/_of_pileup.py
 qetpy/core/didv/__init__.py
 qetpy/core/didv/_base_didv.py
 qetpy/core/didv/_didv.py
 qetpy/core/didv/_didv_priors.py
 qetpy/core/didv/_plot_didv.py
+qetpy/core/didv/_templates_didv.py
+qetpy/core/didv/_uncertainties_didv.py
 qetpy/cut/__init__.py
 qetpy/cut/_cut.py
 qetpy/plotting/__init__.py
 qetpy/plotting/_fitting_plotting.py
 qetpy/plotting/_ibis_plotting.py
 qetpy/plotting/_iv_plotting.py
 qetpy/plotting/_noise_plotting.py
```

### Comparing `QETpy-1.6.2/README.md` & `QETpy-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_de_pileup.py` & `QETpy-1.6.3/qetpy/core/_de_pileup.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_fitting.py` & `QETpy-1.6.3/qetpy/core/_fitting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_ibis.py` & `QETpy-1.6.3/qetpy/core/_ibis.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_iv.py` & `QETpy-1.6.3/qetpy/core/_iv.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_noise.py` & `QETpy-1.6.3/qetpy/core/_noise.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_of_1x1.py` & `QETpy-1.6.3/qetpy/core/_of_1x1.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_of_base.py` & `QETpy-1.6.3/qetpy/core/_of_base.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_of_nonlin.py` & `QETpy-1.6.3/qetpy/core/_of_nonlin.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_of_nsmb.py` & `QETpy-1.6.3/qetpy/core/_of_nsmb.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/_of_pileup.py` & `QETpy-1.6.3/qetpy/core/_of_pileup.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/didv/_base_didv.py` & `QETpy-1.6.3/qetpy/core/didv/_base_didv.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 __all__ = [
     "stdcomplex",
     "compleximpedance",
     "complexadmittance",
     "squarewaveresponse",
+    "get_i0",
+    "get_ibias",
+    "get_tes_bias_parameters_dict"
 ]
 
 
 def _pole_extractor(arg_dict):
     """
     Hidden helper function for aiding in determining which model to
     use when calculating the complex impedance or admittance.
@@ -371,14 +374,344 @@
         )
         return _BaseDIDV._convolvedidv(
             t, A, B, C, tau1, tau2, tau3, sgamp, rsh, sgfreq, dutycycle,
         )
 
 
 
+def _get_current_offset(metadata, channel_name):
+    """
+    Gets and returns the changable current offset (i.e. the current offset set
+    from the FEB control labview tool)
+    
+    Parameters
+    ----------        
+    metadata : dict
+        Metadata returned when loading the dIdV traces.  Used to get
+        the voltage/current offset set with the slider on the FEB controller
+        labview script, so that we can compensate for it. Can be just for 
+        one event
+        
+    channel_name : str
+        Channel name, e.g. 'Melange025pcRight'
+    
+    """
+    
+    voltage_offset = metadata[0]['detector_config'][channel_name]['output_offset']
+    close_loop_norm = metadata[0]['detector_config'][channel_name]['close_loop_norm']
+    return voltage_offset/close_loop_norm
+
+
+def get_i0(offset, offset_err, offset_dict, output_offset, closed_loop_norm,
+           lgcdiagnostics=False):
+    """
+    Gets and returns the current and uncertainty in the current
+    through the TES from a didv_fitresult dictonary (which
+    includes a parameter for the offset of the didv and the offset)
+    
+    Parameters
+    ----------
+    offset: float
+        The current offset of the dIdV as fit (i.e. as measured, without
+        any corrections)
+        
+    offset_err: float
+        The uncertainty in the current offset of the dIdV fit
+        
+    offset_dict: dict
+        Dictionary of offsets gotten from the IV sweep.
+        
+    output_offset: float, volts
+        The output offset gotten from the event metadata. In units of volts,
+        we correct for volts to amps conversion with the closed loop norm.
+        
+    closed_loop_norm: float, volts/amp=ohms
+        The constant from the metadata used to translate the voltage measured by
+        the DAQ into a current coming into the input coil of the SQUIDs. In units of
+        volts/amp = ohms.
+        
+    lgcdiagnostics : bool, optional
+        Used if you want to see the raw currents and offsets and how they're
+        added together. Prints these out
+        
+    Returns
+    -------
+    i0 : float
+        The calculated absolute current through the TES
+    i0_err : float
+        The uncertainty in the absolute current through the TES
+        
+    """
+    
+    current_didv = offset
+    current_err_didv = offset_err
+    
+    offset_changable = output_offset/closed_loop_norm
+    delta_i_changable = (offset_changable - offset_dict['i0_changable_offset'])
+    
+    i0 = current_didv - offset_dict['i0_off'] - delta_i_changable
+    
+    if lgcdiagnostics:
+        print("Current as measured from dIdV: " + str(current_didv) + " amps")
+        print("Changable current as meaured from metadata for this dIdV: " + str(offset_changable) + " amps")
+        print(" ")
+        print("Changable current as measured during IV when offsets were measured: " + 
+              str(offset_dict['i0_changable_offset']) + " amps")
+        print("Current offset as measured from IV: " + str(offset_dict['i0_off']) + " amps")
+        print(" ")
+        print("Delta changable current: " + str(offset_changable) + " - " + 
+             str(offset_dict['i0_changable_offset']) + " = \n " + str(delta_i_changable) + " amps")
+        print(" ")
+        print("True current through TES: " + str(current_didv) + " - " + str(delta_i_changable) + " - \n" + 
+             str(offset_dict['i0_off']) + " = " + str(i0) + " amps")
+    
+    i0_err = np.sqrt((current_err_didv)**2.0 + (offset_dict['i0_off_err'])**2.0)
+    
+    if lgcdiagnostics:
+        print(" ")
+        print(" --------- ")
+        print(" ")
+        print("Current uncertainty from dIdV: " + str(current_err_didv) + " amps")
+        print("Current offset uncertainty from IV: " + str(offset_dict['i0_off_err']) + " amps")
+        print(" ")
+        print("Total current uncetainty: (("  + str(current_err_didv) + ")**2.0 + (" +
+             str(offset_dict['i0_off_err']) + ")**2.0 )**0.5 = \n" + 
+              str(i0_err) + " amps")
+    
+    return i0, i0_err
+
+def get_ibias(ibias_metadata, offset_dict, lgcdiagnostics=False):
+    """
+    Gets and returns the current and uncertainty in the current
+    used to bias the TES from a metadata list
+    
+    Parameters
+    ----------
+        
+    ibias_metadata: float
+        The ibias gotten from the event metadata, i.e. without correcting for
+        the ibias offset calculated from the IV curve
+        
+    offset_dict: dict
+        Dictionary of offsets gotten from the IV sweep.
+        
+    lgcdiagnostics : bool, optional
+        Used if you want to see the raw currents and offsets and how they're
+        added together. Prints these out
+        
+    Returns
+    -------
+    ibias : float
+        The calculated absolute current used to bias the TES
+    ibias_err : float
+        The uncertainty in the absolute current used to bias the TES
+        
+    """
+    
+    ibias = ibias_metadata - offset_dict['ibias_off']
+    ibias_err = offset_dict['ibias_off_err']
+    
+    if lgcdiagnostics:
+        print("Bias current from metadata: " + str(ibias_metadata) + " amps")
+        print("Bias current offset from IV: " + str(offset_dict['ibias_off']) + " amps")
+        print("True bias current: " + str(ibias_metadata) + " - " + str(offset_dict['ibias_off']) + 
+             " = \n" + str(ibias) + " amps")
+        print(" ")
+        
+        print("Bias current uncertainty from IV: " + str(offset_dict['ibias_off_err']) + " amps")
+        
+    return np.absolute(ibias), ibias_err
+
+
+def _get_v0(i0, i0_err, ibias, ibias_err, rsh, rp):
+    """
+    Gets and returns voltage and uncertainty in voltage across the
+    TES at a given bias point.
+    
+    Parameters
+    ----------
+        
+    i0 : float
+        The current through the TES at a given bias point
+        
+    i0_err: float
+        The uncertainty in the current through the TES at a given
+        bias point
+        
+    ibias: float
+        The bias current applied to the TES/shunt system
+        
+    ibias_err: float
+        The uncertainty in the bias current applied to the TES/shunt
+        system
+        
+    rsh: float
+        The shunt resistance in ohms
+        
+    rp: float
+        The parasitic resistance in ohms
+        
+    Returns
+    -------
+    v0 : float
+        The calculated voltage across the TES in volts
+        
+    v0_err : float
+        The calculated uncertainty in the voltage across the TES
+        in volts
+        
+    """
+    
+    vb = rsh * (ibias - i0) #voltage across the shunt resistor
+    vb_err = rsh * np.sqrt(i0_err**2 + ibias_err**2)
+    
+    v0 = np.absolute(vb - rp * i0) #the voltage across the shunt resistor minus
+                      #the voltage across the parasitic resistance
+    v0_err = np.sqrt(vb_err**2 + rp**2 * i0_err**2)
+    
+    return v0, v0_err
+
+def _get_r0(i0, i0_err, v0, v0_err):
+    """
+    Gets and returns the resistance and uncertainty in resistance
+    of a TES at a given bias point
+    
+    Parameters
+    ----------
+        
+    i0 : float
+        The current through the TES at a given bias point
+        
+    i0_err: float
+        The uncertainty in the current through the TES at a given
+        bias point
+        
+    v0: float
+        The voltage across the TES at the bias point
+        
+    v0_err: float
+        The uncertainty in the voltage across the TES at the bias
+        point
+        
+    Returns
+    -------
+    r0 : float
+        The calculated resistance of the TES at the bias point
+        in ohms
+        
+    r0_err : float
+        The calculated uncertainty in the resistance of the TES at
+        the bias point in ohms
+        
+    """
+    
+    r0 = np.absolute(v0/i0)
+    r0_err = np.sqrt(v0_err**2 * i0**-2 + v0**2 * i0_err**2 * i0**-4)
+    
+    return r0, r0_err
+
+def _get_p0(i0, i0_err, v0, v0_err):
+    """
+    Gets and returns the bias power and uncertainty in bias power
+    of a TES at a given bias point
+    
+    Parameters
+    ----------
+        
+    i0 : float
+        The current through the TES at a given bias point
+        
+    i0_err: float
+        The uncertainty in the current through the TES at a given
+        bias point
+        
+    v0: float
+        The voltage across the TES at the bias point
+        
+    v0_err: float
+        The uncertainty in the voltage across the TES at the bias
+        point
+        
+    Returns
+    -------
+    p0 : float
+        The calculated bias power of the TES at the bias point
+        in watts
+        
+    p0_err : float
+        The calculated uncertainty in the bias power of the TES at
+        the bias point in watts
+        
+    """
+    
+    p0 = np.absolute(v0*i0)
+    p0_err = np.sqrt(v0_err**2 * i0**2 + v0**2 * i0_err**2)
+    
+    return p0, p0_err
+
+def get_tes_bias_parameters_dict(i0, i0_err, ibias, ibias_err, rsh, rp):
+    """
+    Gets and returns a dictonary of i0, v0, r0, and p0 with uncertainties
+    from the measured TES bias current and i0
+    
+    Parameters
+    ----------
+        
+    i0 : float
+        The current through the TES at a given bias point
+        
+    i0_err: float
+        The uncertainty in the current through the TES at a given
+        bias point
+        
+    ibias: float
+        The bias current applied to the TES/shunt system
+        
+    ibias_err: float
+        The uncertainty in the bias current applied to the TES/shunt
+        system
+        
+    rsh: float
+        The shunt resistance in ohms
+        
+    rp: float
+        The parasitic resistance in ohms
+        
+    Returns
+    -------
+    bias_parameters_dict : dict
+        A dictonary of bias parameters and uncertainties, including i0, r0,
+        v0, and p0
+        
+    """
+    
+    i0 = np.absolute(i0)
+    
+    v0, v0_err = _get_v0(i0, i0_err, ibias, ibias_err, rsh, rp)
+    r0, r0_err = _get_r0(i0, i0_err, v0, v0_err)
+    p0, p0_err = _get_p0(i0, i0_err, v0, v0_err)
+    
+    bias_parameter_dict = {
+        'i0': i0,
+        'i0_err': i0_err,
+        'v0': v0,
+        'v0_err': v0_err,
+        'r0': r0,
+        'r0_err': r0_err,
+        'p0': p0,
+        'p0_err': p0_err,
+    }
+    
+    return bias_parameter_dict
+
+
+
+
+
+
 class _BaseDIDV(object):
     """
     Class for fitting a didv curve for different types of models of the
     didv. Also gives various other useful values pertaining to the
     didv. This class supports doing 1, 2, and 3 pole fits. This is
     supported in a way that does one dataset at a time.
```

### Comparing `QETpy-1.6.2/qetpy/core/didv/_didv.py` & `QETpy-1.6.3/qetpy/core/didv/_didv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import numpy as np
 from scipy.optimize import least_squares, fsolve
 from scipy.fftpack import fft, ifft, fftfreq
 
-from ._base_didv import _BaseDIDV, complexadmittance
+from ._base_didv import _BaseDIDV, complexadmittance, get_i0, get_ibias, get_tes_bias_parameters_dict
 from ._plot_didv import _PlotDIDV
+from ._uncertainties_didv import get_power_noise_with_uncertainties, get_dPdI_with_uncertainties
+from ._uncertainties_didv import get_smallsignalparams_cov, get_smallsignalparams_sigmas
+
 
 
 __all__ = [
     "didvinitfromdata",
     "DIDV",
 ]
 
@@ -450,15 +453,16 @@
 
         return popt, pcov, cost
 
 
     def dofit(self, poles, fcutoff=np.inf,
               bounds=None, guess_params=None,
               guess_isloopgainsub1=None,
-              lgcfix=None,
+              biasparams_dict=None,
+              lgcfix=None, lgc_ssp_light=False,
               verbose=0, max_nfev=1000,
               method='trf', loss='linear',
               ftol=1e-15, xtol=1e-15):
         """
         This method does the fit that is specified by the variable
         poles. If the `processtraces` method has not been run yet, then
         this method will run that first.
@@ -468,14 +472,18 @@
         poles : int
             The fit that should be run. Should be 1, 2, or 3.
         fcutoff : float, optional
             The cutoff frequency in Hz, above which data is ignored in
             the specified fitting routine. Default is `np.inf`, which
             is equivalent to no cutoff frequency.
         bounds: 
+        lgc_ssp_light : bool, optional
+            Used to tell dofit that the smallsignalparams light (only
+            beta, l, L, tau0, gratio) result dictionary including
+            uncertainties and covaraiance matrix should be calculted
 
         Raises
         ------
         ValueError
             If the inputted `poles` is not 1, 2, or 3.
 
         Notes
@@ -566,15 +574,18 @@
                 fitparams1,
                 fitcov1,
                 falltimes1,
                 fitcost1,
                 self._rsh,
                 self._rp,
                 self._r0,
+                self._offset,
+                self._offset_err, 
                 lgcfix=lgcfix,
+                biasparams_dict=biasparams_dict,
             )
 
         elif poles==2:
   
             
             # Guess the starting parameters for 2 pole fitting
             A0, B0, tau10, tau20, isloopgainsub1 = DIDV._guessdidvparams(
@@ -645,15 +656,18 @@
                 fitparams2,
                 fitcov2,
                 falltimes2,
                 fitcost2,
                 self._rsh,
                 self._rp,
                 self._r0,
+                self._offset, 
+                self._offset_err, 
                 lgcfix=lgcfix,
+                biasparams_dict=biasparams_dict,
             )
 
         elif poles==3:
             
             if self._2poleresult is None:
                 # Guess the 3-pole fit starting parameters from
                 # 2-pole fit guess
@@ -751,34 +765,125 @@
                 fitparams3,
                 fitcov3,
                 falltimes3,
                 fitcost3,
                 self._rsh,
                 self._rp,
                 self._r0,
+                self._offset,
+                self._offset_err,
                 lgcfix=lgcfix,
+                biasparams_dict=biasparams_dict,
             )
+            
+            if lgc_ssp_light:
+                ssp_light_cov = get_smallsignalparams_cov(self._3poleresult)
+                ssp_light_sigmas = get_smallsignalparams_sigmas(self._3poleresult)
+                
+                self._3poleresult = DIDV._fitresult(
+                    poles,
+                    fitparams3,
+                    fitcov3,
+                    falltimes3,
+                    fitcost3,
+                    self._rsh,
+                    self._rp,
+                    self._r0,
+                    self._offset,
+                    self._offset_err,
+                    lgcfix=lgcfix,
+                    biasparams_dict=biasparams_dict,
+                    ssp_light_cov=ssp_light_cov,
+                    ssp_light_sigmas=ssp_light_sigmas,
+                )
+            
 
         else:
             raise ValueError("The number of poles should be 1, 2, or 3.")
 
+    def dofit_with_true_current(self, offset_dict, output_offset, closed_loop_norm, ibias_metadata,
+                            bounds=None, guess=None, lgcdiagnostics=False):
+        """
+        Given the offset dictionary used to store the various current
+        current offsets used to reconstruct the true current through the 
+        TES and the trace metadata, finds the true current through the TES,
+        makes a biasparams dict, and recalculates the smallsignalparams
+        from the newly found true bias point.
+        
+        
+        Parameters:
+        ----------
+        
+        offset_dict: dict
+            Where are the relevant offsets are stored. Generated from the IV
+            sweep.
+            
+        output_offset: float, volts
+            The output offset gotten from the event metadata. In units of volts,
+            we correct for volts to amps conversion with the closed loop norm.
+            
+        closed_loop_norm: float, volts/amp=ohms
+            The constant from the metadata used to translate the voltage measured by
+            the DAQ into a current coming into the input coil of the SQUIDs. In units of
+            volts/amp = ohms.
+            
+        ibias_metadata: float
+            The ibias gotten from the event metadata, i.e. without correcting for
+            the ibias offset calculated from the IV curve
+            
+        bounds: array, optional
+            Passed to dofit.
+            
+        guess: array, optional
+            Passed to dofit
+            
+        
+        
+        Returns:
+        --------
+            
+        retult3: fitresult_dict
+            3 pole fit result with biasparams calculated, and the smallsignalparams
+            correctly calculated from the r0 calculated for the biasparams
+        
+        """
+
+        self._rp = offset_dict['rp']
+
+        rsh = self._rsh
+        rp = self._rp
+
+        offset = self._offset
+        offset_err = self._offset_err
+
+        i0, i0_err = get_i0(offset, offset_err, offset_dict, output_offset, closed_loop_norm, lgcdiagnostics)
+        ibias, ibias_err = get_ibias(ibias_metadata, offset_dict, lgcdiagnostics)
+        biasparams_dict = get_tes_bias_parameters_dict(i0, i0_err, ibias, ibias_err, rsh, rp)
+        self._r0 = biasparams_dict['r0']
+
+        result3 = self.dofit(3, bounds=bounds, guess_params=guess, biasparams_dict=biasparams_dict,
+                             lgc_ssp_light = True)
+
+        return result3
 
     @staticmethod
     def _fitresult(poles, params, cov, falltimes, cost, rsh, rp, r0,
-                   lgcfix=None):
+                   offset, offset_err, 
+                   biasparams_dict=None, lgcfix=None,
+                   ssp_light_cov=None, ssp_light_sigmas=None):
         """
         Function for converting data from different fit results to a
         results dictionary.
 
         """
 
         result = dict()
         result['lgcfix'] = lgcfix
 
-        # errores
+        # errors
         errors = np.diag(cov)**0.5
         if lgcfix is not None:
             errors = np.zeros_like(lgcfix, dtype=float)
             np.place(errors, lgcfix, 0.0)
             np.place(errors, ~lgcfix,  np.diag(cov)**0.5)
         
         if poles == 1:
@@ -864,13 +969,35 @@
                 'l': smallsignalparams[4],
                 'L': smallsignalparams[5],
                 'tau0': smallsignalparams[6],
                 'gratio': smallsignalparams[7],
                 'tau3': smallsignalparams[8],
                 'dt': smallsignalparams[9],
             }
+            
+            #we only calculate the smallsignalparameters covaraiance matrix for
+            #these parameters, so this is just a container for them
+            if (ssp_light_cov is not None) and (ssp_light_sigmas is not None):
+                ssp_light_vals = {
+                    'beta': smallsignalparams[3],
+                    'l': smallsignalparams[4],
+                    'L': smallsignalparams[5],
+                    'tau0': smallsignalparams[6],
+                    'gratio': smallsignalparams[7],
+                }
+                result['ssp_light'] = {
+                    'vals': ssp_light_vals,
+                    'cov': ssp_light_cov,
+                    'sigmas': ssp_light_sigmas,
+                }
 
+        result['offset'] = offset
+        result['offset_err'] = offset_err
+        
+        if biasparams_dict is not None:
+            result['biasparams'] = biasparams_dict
+        
         result['falltimes'] = falltimes
         result['cost'] = cost
         result['didv0'] = complexadmittance(0, **result['smallsignalparams']).real
 
         return result
```

### Comparing `QETpy-1.6.2/qetpy/core/didv/_didv_priors.py` & `QETpy-1.6.3/qetpy/core/didv/_didv_priors.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/core/didv/_plot_didv.py` & `QETpy-1.6.3/qetpy/core/didv/_plot_didv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 import matplotlib.pyplot as plt
+from scipy.fftpack import fft, ifft, fftfreq
+
 
 from ._base_didv import squarewaveresponse, complexadmittance
 from qetpy.utils import lowpassfilter
 
 
 class _PlotDIDV(object):
     """Class that contains all plotting functions for DIDV."""
@@ -36,16 +38,32 @@
                     cost_vals
                 ) if val is not None
             )[1]
             best_time_offset = dt_vals[min_cost_idx]
 
         return best_time_offset
 
+    def _get_didv_filtered_trace(self):
+        """Helper function for making a filtered version of the time domain trace with
+           only dIdV frequencies shown"""
+        st = fft(self._tmean)
+        sf = np.zeros_like(self._freq)*0.0j
+        tracelength = len(self._tmean)
+
+        oddinds = ((np.abs(np.mod(np.absolute(self._freq/self._sgfreq), 2)-1))<1e-8)
+        sf[oddinds] = 1.0
+
+        sf[tracelength//2] = 0.0j
+
+        filtered_trace = sf * st
+
+        return ifft(filtered_trace)
+
 
-    def _plot_time_domain(self, poles, lp_cutoff=None):
+    def _plot_time_domain(self, poles, lp_cutoff=None, didv_freq_filt=False):
         """Helper function for plotting the fits in time domain."""
 
         if poles == "all":
             poleslist = np.array([1, 2, 3])
         else:
             poleslist = np.array(poles)
 
@@ -66,14 +84,45 @@
             ax.plot(
                 self._time * 1e6,
                 lp_meantrace,
                 color='red',
                 label='Mean, ' + str(lp_cutoff*1e-3) + ' kHz Low Pass',
             )
 
+            if didv_freq_filt:
+                didv_filt_trace = self._get_didv_filtered_trace()
+                lp_didv_filt_trace = lowpassfilter(didv_filt_trace * 1e6,
+                                                   lp_cutoff, fs=self._fs, order=2)
+
+                ax.plot(
+                    self._time * 1e6,
+                    didv_filt_trace * 1e6,
+                    color='purple',
+                    label='Mean, dIdV Frequencies Only',
+                )
+
+                
+                ax.plot(
+                    self._time * 1e6,
+                    lp_didv_filt_trace,
+                    color='lime',
+                    label='Mean, dIdV Frequencies Only +  ' + str(lp_cutoff*1e-3) + ' kHz Low Pass',
+                )
+        elif didv_freq_filt:
+            didv_filt_trace = self._get_didv_filtered_trace()
+            
+            ax.plot(
+                self._time * 1e6,
+                didv_filt_trace,
+                color='purple',
+                label='Mean, dIdV Frequencies Only',
+            )
+
+                
+
         if (self._1poleresult is not None) and (1 in poleslist):
             if 'smallsignalparams' in self._1poleresult:
                 key = 'smallsignalparams'
             else:
                 key = 'params'
             didvfit1_timedomain = squarewaveresponse(
                 self._time,
@@ -138,15 +187,15 @@
 
         return fig, ax
 
 
     def plot_full_trace(self, poles="all",
                         saveplot=False, savepath="",
                         savename="",
-                        lp_cutoff=None):
+                        lp_cutoff=None, didv_freq_filt=False):
         """
         Function to plot the entire trace in time domain
 
         Parameters
         ----------
         poles : int, string, array_like, optional
             The pole fits that we want to plot. If set to "all", then
@@ -159,32 +208,36 @@
             directory by default.
         savename : string, optional
             A string to append to the end of the file name if saving.
             Empty string by default.
         lp_cutoff : float, optional
             cutoff frequency in Hz for display filtered trace
             Default: None (filtered trace not displayed)
+        didv_freq_filt : bool, optional
+            If true, plots an additional trace with only frequencies in 
+            the dIdV square wave passed.
 
         """
 
-        fig, ax = self._plot_time_domain(poles, lp_cutoff = lp_cutoff)
+        fig, ax = self._plot_time_domain(poles, lp_cutoff = lp_cutoff,
+                                         didv_freq_filt = didv_freq_filt)
 
         ax.set_xlim([self._time[0] * 1e6, self._time[-1] * 1e6])
         ax.set_title("Full Trace of dIdV")
 
         if saveplot:
             fig.savefig(savepath + f"full_trace_{savename}.png")
             plt.close(fig)
         else:
             plt.show()
 
 
     def plot_single_period_of_trace(self, poles="all", saveplot=False,
                                     savepath="", savename="",
-                                    lp_cutoff=None):
+                                    lp_cutoff=None, didv_freq_filt=False):
         """
         Function to plot a single period of the trace in time domain
 
         Parameters
         ----------
         poles : int, string, array_like, optional
             The pole fits that we want to plot. If set to "all", then
@@ -197,18 +250,21 @@
             directory by default.
         savename : string, optional
             A string to append to the end of the file name if saving.
             Empty string by default.
         lp_cutoff : float, optional
             cutoff frequency in Hz for display filtered trace
             Default: None (filtered trace not displayed)
+        didv_freq_filt : bool, optional
+            If true, plots an additional trace with only frequencies in 
+            the dIdV square wave passed.
 
         """
 
-        fig, ax = self._plot_time_domain(poles, lp_cutoff)
+        fig, ax = self._plot_time_domain(poles, lp_cutoff, didv_freq_filt)
 
         period = 1.0/self._sgfreq
 
         ax.set_xlim([self._time[0] * 1e6, self._time[0] * 1e6 + period * 1e6])
         ax.set_title("Single Period of Trace")
 
         if saveplot:
@@ -216,15 +272,15 @@
             plt.close(fig)
         else:
             plt.show()
 
 
     def plot_zoomed_in_trace(self, poles="all", zoomfactor=0.1,
                              saveplot=False, savepath="", savename="",
-                             lp_cutoff=None):
+                             lp_cutoff=None, didv_freq_filt=False):
         """
         Function to plot a zoomed in portion of the trace in time
         domain. This plot zooms in on the overshoot of the DIDV.
 
         Parameters
         ----------
         poles : int, string, array_like, optional
@@ -241,22 +297,26 @@
             directory by default.
         savename : string, optional
             A string to append to the end of the file name if saving.
             Empty string by default.
         lp_cutoff : float, optional
             cutoff frequency in Hz for display filtered trace
             Default: None (filtered trace not displayed)
+        didv_freq_filt : bool, optional
+            If true, plots an additional trace with only frequencies in 
+            the dIdV square wave passed.
 
         """
 
         period = 1.0 / self._sgfreq
 
         best_time_offset = self._get_best_time_offset()
 
-        fig, ax = self._plot_time_domain(poles, lp_cutoff)
+        fig, ax = self._plot_time_domain(poles, lp_cutoff,
+                                         didv_freq_filt = didv_freq_filt)
 
         ax.set_xlim(
             (best_time_offset + self._time[0] + (
                 0.5 - zoomfactor / 2
             ) * period) * 1e6,
             (best_time_offset + self._time[0] + (
                 0.5 + zoomfactor / 2) * period
```

### Comparing `QETpy-1.6.2/qetpy/cut/_cut.py` & `QETpy-1.6.3/qetpy/utils/_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1063 +1,1124 @@
 import numpy as np
-import random
-from qetpy import ofamp
-from qetpy.utils import make_template
-from astropy.stats import sigma_clip
-from scipy import stats, optimize
-from scipy.stats import skew
-import warnings
-import matplotlib.pyplot as plt
+from scipy import interpolate, signal, constants
+from scipy import ndimage
+from sympy.ntheory import factorrat
+from sympy.core.symbol import S
 
 
 __all__ = [
-    "removeoutliers",
-    "iterstat",
-    "itercov",
-    "IterCut",
-    "autocuts",
-    "get_muon_cut",
+    "make_decreasing",
+    "calc_offset",
+    "lowpassfilter",
+    "align_traces",
+    "get_offset_from_muon",
+    "powertrace_simple",
+    "energy_absorbed",
+    "slope",
+    "fill_negatives",
+    "shift",
+    "make_template",
+    "make_template_twopole",
+    "make_template_threepole",
+    "make_template_fourpole",
+    "estimate_g",
+    "resample_factors",
+    "resample_data",
+    "interpolate_parabola",
+    "interpolate_of",
+    "argmin_chisq",
 ]
 
 
-def removeoutliers(x, maxiter=20, skewtarget=0.05):
+def shift(arr, num, fill_value=0):
     """
-    Function to return indices of inlying points, removing points
-    by minimizing the skewness.
+    Function for shifting the values in an array by a certain number of
+    indices, filling the values of the bins at the head or tail of the
+    array with fill_value.
 
     Parameters
     ----------
-    x : ndarray
-        Array of real-valued variables from which to remove outliers.
-    maxiter : float, optional
-        Maximum number of iterations to continue to minimize skewness.
-        Default is 20.
-    skewtarget : float, optional
-        Desired residual skewness of distribution. Default is 0.05.
+    arr : array_like
+        Array to shift values in.
+    num : float
+        The number of values to shift by. If positive, values shift to
+        the right. If negative, values shift to the left. If num is a
+        non-whole number of bins, arr is linearly interpolated
+    fill_value : scalar, optional
+        The value to fill the bins at the head or tail of the array with.
 
     Returns
     -------
-    inds : ndarray
-        Boolean indices indicating which values to select/reject, same
-        length as `x`.
+    result : ndarray
+        The resulting array that has been shifted and filled in.
 
     """
 
-    i=1
-    inds=(x != np.inf)
-    sk=skew(x[inds])
-    while(sk > skewtarget):
-        dmed=x-np.median(x[inds])
-        dist=np.min([abs(min(dmed)),abs(max(dmed))])
-        inds=inds & (abs(dmed) < dist)
-        sk=skew(x[inds])
-        if(i > maxiter):
-            break
-        i+=1
+    result = np.empty_like(arr)
+
+    if float(num).is_integer():
+        num = int(num) # force num to int type for slicing
+
+        if num > 0:
+            result[:num] = fill_value
+            result[num:] = arr[:-num]
+        elif num < 0:
+            result[num:] = fill_value
+            result[:num] = arr[-num:]
+        else:
+            result[:] = arr
+    else:
+        result = ndimage.shift(
+            arr, num, order=1, mode='constant', cval=fill_value,
+        )
+
+    return result
 
-    return inds
 
-class _UnbiasedEstimators(object):
+def resample_factors(fs, sgfreq):
     """
-    Helper class for calculating the unbiased estimators of a 1D normal
-    distribution that has been truncated at specified bounds.
+    Function for determining the upsampling and downsampling factors
+    needed to ensure that `fs`/`sgfreq` is an integer. These factor are
+    to be used with `scipy.signal.resample_poly`. Note that these
+    factors are not a unique solution, but a simple one.
 
-    Attributes
+    Parameters
     ----------
-    mu0 : float
-        The biased estimator of the mean of the inputted and truncated
-        data.
-    std0 : float
-        The biased estimator of the standard deviation of the inputted
-        and truncated data.
-    mu : float
-        The unbiased estimator of the mean of the inputted and
-        truncated data.
-    std : float
-        The unbiased estimator of the standard deviation of the
-        inputted and truncated data.
+    fs : int
+        The digitization rate of the data in Hz.
+    sgfreq : int
+        The frequency of the square wave from the signal generator in
+        Hz.
+
+    Returns
+    -------
+    up : int
+        The upsampling factor.
+    down : int
+        The downsampling factor.
+
+    Notes
+    -----
+    See the documentation for `scipy.signal.resample_poly` for more
+    information on these factors.
 
     """
-    
-    def __init__(self, x, lwrbnd, uprbnd):
-        """
-        Initialization of the `_UnbiasedEstimators` helper class
-
-        Parameters
-        ----------
-        x : ndarray
-            A 1D array of data that has been truncated, for which the
-            unbiased estimators will be calculated.
-        lwrbnd : float
-            The lower bound of the truncation of the distribution.
-        uprbnd : float
-            The upper bound of the truncation of the distribution.
-
-        """
-
-        inds = (np.asarray(x) >= lwrbnd) & (np.asarray(x) <=uprbnd)
-
-        self._lwrbnd = lwrbnd
-        self._uprbnd = uprbnd
-
-        self._x = x[inds] # make sure data is between the specified bounds
-        self._sumx = np.sum(self._x)
-        self._sumx2 = np.sum(self._x**2)
-        self._lenx = len(self._x)
-
-        self.mu0 = np.mean(self._x)
-        self.std0 = np.std(self._x)
-
-        self._calc_unbiased_estimators()
-
-    def _equations(self, p):
-        """
-        Helper method for calculating the system of equations that will
-        be numerically solved for find the unbiased estimators.
-
-        Parameters
-        ----------
-        p : tuple
-            A tuple of length 2 containing the current estimated values
-            of the unbiased estimators: (mu, std).
-
-        Returns
-        -------
-        (mu_eqn, std_eqn) : tuple
-            A tuple containing the two equations that will be solved to
-            give the unbiased estimators of the mean and standard
-            deviation of the data.
-
-        """
-
-        mu, std = p
-
-        pdf_lwr = stats.norm.pdf(self._lwrbnd, loc=mu, scale=std)
-        pdf_upr = stats.norm.pdf(self._uprbnd, loc=mu, scale=std)
-
-        cdf_lwr = stats.norm.cdf(self._lwrbnd, loc=mu, scale=std)
-        cdf_upr = stats.norm.cdf(self._uprbnd, loc=mu, scale=std)
-
-        mu_eqn = self._sumx - self._lenx * mu
-        # term due to truncation
-        mu_eqn += self._lenx / (cdf_upr - cdf_lwr) * (pdf_upr - pdf_lwr)
-
-        std_eqn = (
-            self._sumx2 - 2 * mu * self._sumx
-        ) + (
-            self._lenx * mu**2 - self._lenx * std**2
-        )
-        # term due to truncation
-        std_eqn += self._lenx * std**2 / (cdf_upr - cdf_lwr) * (
-            (self._uprbnd - mu) * pdf_upr - (self._lwrbnd - mu) * pdf_lwr
-        )
 
-        return (mu_eqn, std_eqn)
+    if int(fs) != fs:
+        raise ValueError('`fs` must be an integer to use this function')
+    if int(sgfreq) != sgfreq:
+        raise ValueError('`sgfreq` must be an integer to use this function')
 
-    def _calc_unbiased_estimators(self):
-        """
-        Method for calculating the unbiased estimators of the truncated
-        distribution.
-
-        """
-
-        self.mu, self.std = optimize.fsolve(
-            self._equations,
-            (self.mu0, self.std0),
-        )
+    rfacs = factorrat(S(int(fs)) / int(sgfreq))
+    numer = [key for key in rfacs if rfacs[key] > 0]
+    denom = [key for key in rfacs if rfacs[key] < 0]
+
+    if len(denom)==0:
+        return 1, 1
+
+    down = np.multiply.reduce(numer)
+    up = round(down / min(denom)) * min(denom)
+
+    # round up if `sgfreq` is prime (otherwise would return 0)
+    if up==0:
+        up = np.ceil(down / min(denom)).astype(int) * min(denom)
 
+    return int(up), int(down)
 
-def iterstat(data, cut=3, precision=1000.0,
-             return_unbiased_estimates=False):
+
+def resample_data(x, fs, sgfreq, **kwargs):
     """
-    Function to iteratively remove outliers based on how many standard
-    deviations they are from the mean, where the mean and standard
-    deviation are recalculated after each cut.
+    Function that uses `resample_factors` and
+    `scipy.signal.resample_poly` to automatically resample the data to
+    ensure that `fs`/`sgfreq` is an integer.
 
     Parameters
     ----------
-    data : ndarray
-        Array of data that we want to remove outliers from.
-    cut : float, optional
-        Number of standard deviations from the mean to be used for
-        outlier rejection
-    precision : float, optional
-        Threshold for change in mean or standard deviation such that we
-        stop iterating. The threshold is determined by
-        np.std(data)/precision. This means that a higher number for
-        precision means a lower threshold (i.e. more iterations).
-    return_unbiased_estimates : bool, optional
-        Boolean flag for whether or not to return the biased or
-        unbiased estimates of the mean and standard deviation of the
-        data. Default is False.
+    x : array_like
+        The data to be resampled.
+    fs : int
+        The digitization rate of the data in Hz.
+    sgfreq : int
+        The frequency of the square wave from the signal generator in
+        Hz.
+    axis : int, optional
+        The axis of `x` that is resampled. Default is -1.
+    window : string, tuple, or array_like, optional
+        Desired window to use to design the low-pass filter, or the FIR
+        filter coefficients to employ.
+    padtype : string, optional
+        `constant`, `line`, `mean`, `median`, `maximum`, `minimum` or
+        any of the other signal extension modes supported by
+        `scipy.signal.upfirdn`. Changes assumptions on values beyond
+        the boundary. If `constant`, assumed to be `cval` (default
+        zero). If `line` assumed to continue a linear trend defined by
+        the first and last points. `mean`, `median`, `maximum` and
+        `minimum` work as in `np.pad` and assume that the values beyond
+        the boundary are the mean, median, maximum or minimum
+        respectively of the array along the axis. Default is
+        `constant`.
+    cval : float, optional
+        Value to use if `padtype='constant'`. Default is zero.
 
     Returns
     -------
-    datamean : float
-        Mean of the data after outliers have been removed.
-    datastd : float
-        Standard deviation of the data after outliers have been
-        removed.
-    datamask : ndarray
-        Boolean array indicating which values to keep or reject in
-        data, same length as data.
+    resampled_x : ndarray
+        The resampled data.
+    resampled_fs : float
+        The digitization rate of `resampled_x` in Hz.
+
+    Notes
+    -----
+    The `kwargs` are each passed to the `scipy.signal.resample_poly`
+    function, from which we took the text for this dosctring for those
+    parameters.
 
     """
 
-    stdcutoff = np.std(data)/precision
-
-    meanlast = np.mean(data)
-    stdlast = np.std(data)
-
-    nstable = 0
-    keepgoing = True
-
-    while keepgoing:
-        mask = abs(data - meanlast) < cut*stdlast
-        if sum(mask) <=1:
-            warnings.warn(
-                "The number of events passing iterative cut via iterstat is <= 1. "
-                "Iteration not converging properly. Returning simple mean and std. "
-                "No data will be cut."
-            )
-            meanthis = np.mean(data)
-            stdthis = np.std(data)
-            mask = np.ones(len(data),dtype=bool)
-            return meanthis, stdthis, mask
-
-        meanthis = np.mean(data[mask])
-        stdthis = np.std(data[mask])
-
-        if (
-            abs(meanthis - meanlast) > stdcutoff
-        ) or (
-            abs(stdthis - stdlast) > stdcutoff
-        ):
-            nstable = 0
-        else:
-            nstable = nstable + 1
-        if nstable >= 3:
-            keepgoing = False
-
-        meanlast = meanthis
-        stdlast = stdthis
-
-    if return_unbiased_estimates:
-        unb = _UnbiasedEstimators(
-            data[mask],
-            meanthis - cut * stdthis,
-            meanthis + cut * stdthis,
-        )
-        return unb.mu, unb.std, mask
+    if 'axis' not in kwargs:
+        kwargs['axis'] = -1
+
+    up, down = resample_factors(fs, sgfreq)
+    resampled_x = signal.resample_poly(x, up, down, **kwargs)
+    resampled_fs =  fs * up / down
+
+    return resampled_x, resampled_fs
 
-    return meanthis, stdthis, mask
 
-def itercov(*args, nsigma=2.75, threshold=None, maxiter=15,
-            frac_err=1e-3):
+def make_template(t, tau_r=None, tau_f=None,  offset=0,
+                  params=None, fs=None,
+                  normalize=True):
     """
-    Function for iteratively determining the estimated covariance
-    matrix of a multidimensional normal distribution.
+    Function to make an ideal pulse template in time domain with single
+    pole exponential rise and fall times, and a given time offset. The
+    template will be returned with the maximum pulse height normalized
+    to one. The pulse, by default, begins at the center of the trace,
+    which can be left or right shifted via the `offset` optional
+    argument.
 
     Parameters
     ----------
-    args : array_like
-        The data to be iteratively cut on. Can be inputted as a single
-        N-by-M array or as M arguments that are 1D vectors of length N,
-        where N is the number of data points and M is the number of
-        dimensions.
-    nsigma : float, optional
-        The number of sigma that defines that maximum chi-squared each
-        data point must be below. Default is 2.75.
-    threshold : float, NoneType, optional
-        The threshold to cut data. If left as None, this is set to the
-        larger of 3 sigma or the number of sigma such that 95% of the
-        data is kept if the data is normal.
-    maxiter : int, optional
-        The maximum number of iterations to perform when cutting.
-        Default is 15.
-    frac_err : float, optional
-        The fractional error allowed before stopping the iterations.
-        Default is 1e-3.
+    t : ndarray
+        Array of time values to make the pulse with
+    tau_r : float, optional (for back-compatibility, use params instead)
+        The time constant for the exponential rise of the pulse
+    tau_f : float, optional (for back-compatibility, use params instead)
+        The time constant for the exponential fall of the pulse
+    offset : int, optional (for back-compatibility, use params instead)
+        The number of bins the pulse template should be shifted
+        from 1/2 trace point
+    params : list, optional
+         2-pole: [A, tau_r, tau_f, (optional) t0]
+         3-pole: [A, B, tau_r, tau_f1, tau_f2, (optional) t0] 
+         4-pole: [A, B, C, tau_r, tau_f1, tau_f2, tau_f3, (optional) t0] 
+         (t0 in sec, default 1/2 trace, if t0->fs arguement required)
+    fs :  float,  optional (required if t0 in params argument)
+        sample rate
+    normalize : boolean, optional
+        if True, normalize pulse with maximum pulse
 
     Returns
     -------
-    datamean : ndarray
-        The estimated mean of the data points, after iteratively
-        cutting outliers.
-    datacov : ndarray
-        The estimated covariance of the data points, after iteratively
-        cutting outliers.
-    datamask : ndarray
-        The boolean mask of the original data that specifies which data
-        points were kept.
-
-    Raises
-    ------
-    ValueError
-        If the shape of the data does not match the two options
-            specified by `args`.
-        If the data inputted is 1-dimensional.
+    template : array
+        the pulse template in time domain
 
     """
 
-    datashape = np.shape(args)
-
-    if len(datashape) > 2:
-        ndim = datashape[-1]
-        nevts = datashape[1]
-        data = args[0].T
-    elif len(datashape) == 2:
-        ndim = datashape[0]
-        nevts = datashape[-1]
-        data = np.stack(args, axis=1).T
+    template = None
+
+    # back compatibility
+    if (tau_r is not None and
+        tau_f is not None):
+    
+        pulse = np.exp(-t/tau_f)-np.exp(-t/tau_r)
+        pulse_shifted = shift(pulse, len(t)//2 + offset)
+        if normalize:
+            template = pulse_shifted/pulse_shifted.max()
+
+    elif params is not None:
+        
+        tlen = len(params)
+
+        # 2-pole fit
+        if tlen==3 or  tlen==4:
+            t0 = None
+            if  tlen==4:
+                t0 = params[-1]
+            template = make_template_twopole(
+                t,
+                A=params[0],
+                tau_r=params[1],
+                tau_f=params[2],
+                t0=t0,
+                fs=fs
+            )
+            
+        elif tlen==5 or tlen==6:
+            t0 = None
+            if  tlen==6:
+                t0 = params[-1]
+            template = make_template_threepole(
+                t,
+                A=params[0],
+                B=params[1],
+                tau_r=params[2],
+                tau_f1=params[3],
+                tau_f2=params[4],
+                t0=t0,
+                fs=fs
+            )    
+        elif tlen==7 or tlen==8:
+            t0 = None
+            if  tlen==8:
+                t0 = params[-1]
+            template = make_template_fourpole(
+                t,
+                A=params[0],
+                B=params[1],
+                C=params[2],
+                tau_r=params[3],
+                tau_f1=params[4],
+                tau_f2=params[5],
+                tau_f3=params[6],
+                t0=t0,
+                fs=fs
+            )
+            
     else:
-        raise ValueError("Shape of data is inconsistent.")
+        raise ValueError('ERROR: unrecognized make_template parameters!')
+            
+            
+    return template
 
-    if data.shape[0] == 1:
-        raise ValueError(
-            "The inputted data is 1-dimensional, use qetpy.cut.iterstat instead."
-        )
 
-    if threshold is None:
-        sigma2 = stats.chi2.ppf(0.95**(1 / ndim), 1)**0.5
-        threshold = np.max([3, sigma2])
+def make_template_twopole(t, A=None, tau_r=None, tau_f=None,
+                          t0=None, fs=None,
+                          normalize=True):
+    """
+    Functional form of pulse in time domain with the amplitude,
+    rise time, fall time, and time offset. The
+    functional form is:
+     
+            A*(exp(-t/\tau_fall)) - A*(exp(-t/\tau_rise))
 
-    mean_last = np.mean(data, axis=1)
-    cov_last = np.atleast_1d(np.cov(data))
+    Note that there are 2 ways to interpret the 'A' parameter input
+    to this function (see below).
 
-    std_last = np.sqrt(np.diag(cov_last))
+    Parameters
+    ----------
+    t : ndarray
+        Array of time values to make the pulse with
+    A : float
+        Amplitude parameter.
+    tau_r : float
+        Rise time of two-pole pulse
+    tau_f : float
+        Fall time of two-pole pulse
+    t0 : float, optional
+        Time offset of two pole pulse
+            default: 1/2 trace
+    fs :  float, required if t0 not None
+        sample rate
+    normalize : boolean, optional
+        if True, normalize pulse with maximum pulse
 
-    err_mean = frac_err * std_last
-    err_cov = frac_err * np.sum(std_last**2)
+    Returns
+    -------
+    pulse : ndarray
+        Array of amplitude values as a function of time
 
-    mean_chi2 = ndim
-    sig_chi2 = np.sqrt(2 * ndim)
+    """
 
-    max_chi2 = mean_chi2 + nsigma * sig_chi2
+    pulse = (
+        A * (np.exp(-t/tau_f))
+    ) - (
+        A * (np.exp(-t/tau_r))
+    )
+    
+    # offset -> default 1/2 traces
+    offset = len(t)//2
+    if t0 is not None:
+        if fs is None:
+            raise ValueError(
+                'ERROR: sample rate (fs) '
+                + ' required!'
+            )
+        offset = int(t0 * fs)
+            
+    pulse = shift(pulse, offset)
+    
+    # normalize
+    if normalize:
+        pulse = pulse/pulse.max()
 
-    nstable = 0
-    keepgoing = True
-    jj = 0
+    return pulse
+        
 
-    while keepgoing:
-        delta = data - mean_last[:, np.newaxis]
+def make_template_threepole(t, A, B, tau_r, tau_f1, tau_f2,
+                            t0=None, fs=None,
+                            normalize=True):
+    """
+    Functional form of pulse in time domain with 1 rise time and
+    two fall times. The  fall times have independent amplitudes
+    (A,B) and the condition f(0)=0 constrains the rise time to have
+    amplitude (A+B). The functional form (time domain) is:
 
-        chi2 = np.sum(delta * np.dot(np.linalg.inv(cov_last), delta), axis=0)
-        mask = chi2 < max_chi2
+            A*(exp(-t/\tau_fall1)) + B*(exp(-t/\tau_fall2)) - 
+            (A+B)*(exp(-t/\tau_rise))
 
-        mask = mask & np.all(
-            np.abs(delta) < std_last[:, np.newaxis] * threshold,
-            axis=0,
-        )
-        nmask = np.sum(mask)
+    and therefore the "amplitudes" take on different meanings than
+    in the other n-pole functions
+
+    3 rise/fall times, 2 amplitudes, and time offset allowed to
+    float.
+    
+    Parameters
+    ----------
+    t : ndarray
+        Array of time values to make the pulse with
+    A : float
+        Amplitude for first fall time
+    B : float
+        Amplitude for second fall time
+    tau_r : float
+        Rise time of pulse
+    tau_f1 : float
+        First fall time of pulse
+    tau_f2 : float
+        Second fall time of pulse
+    t0 : float, optional
+        Time offset of three pole pulse
+        Default: 1/2 trace
+    fs :  float, required if t0 not None
+        sample rate
+    normalize : boolean, optional
+        if True, normalize pulse with maximum pulse
+
+
+    Returns
+    -------
+    pulse : ndarray
+        Array of amplitude values as a function of time
+    """
 
-        if nmask <= 1:
-            warnings.warn(
-                "The number of events passing iterative cut via itercov is <= 1. "
-                "Iteration not converging properly. Returning simple mean and cov. "
-                "No data will be cut."
+    pulse = (
+        A * (np.exp(-t / tau_f1))
+    ) + (
+        B * (np.exp(-t / tau_f2))
+    ) - (
+        (A + B) * (np.exp(-t / tau_r))
+    )
+
+    # offset -> default 1/2 traces
+    offset = len(t)//2
+    if t0 is not None:
+        if fs is None:
+            raise ValueError(
+                'ERROR: sample rate (fs) '
+                + ' required!'
             )
-            mean_this = np.mean(data, axis=1)
-            cov_this = np.atleast_1d(np.cov(data))
-            mask = np.ones(nevts, dtype=bool)
-
-            return mean_this, cov_this, mask
-
-        mean_this = np.mean(data[:, mask], axis=1)
-        cov_this = np.atleast_1d(np.cov(data[:, mask]))
-
-        if np.any(
-            np.abs(mean_this - mean_last) > err_mean
-        ) or np.any(
-            np.abs(cov_this - cov_last) > err_cov
-        ):
-            nstable = 0
-        else:
-            nstable += 1
+        offset = int(t0 * fs)
+            
+    pulse = shift(pulse, offset)
+    
+    # normalize
+    if normalize:
+        pulse = pulse/pulse.max()
+
+    return pulse
+
+
+def make_template_fourpole(t, A, B, C, tau_r,
+                           tau_f1, tau_f2, tau_f3,
+                           t0=None, fs=None,
+                           normalize=True):
+    """
+    Functional form of pulse in time domain with 1 rise time and
+    three fall times The fall times have independent amplitudes
+    (A,B,C). The condition f(0)=0 requires the rise time to have
+    amplitude (A+B+C). Therefore, the "amplitudes" take on
+    different meanings than in other n-pole functions. The
+    functional form (time-domain) is:
 
-        if nstable >= 2 or jj > maxiter:
-            keepgoing = False
+            A*(exp(-t/tau_fall1)) + B*(exp(-t/tau_fall2)) +
+            C*(exp(-t/tau_fall3)) - (A+B+C)*(exp(-t/tau_rise))
 
-        mean_last = mean_this
-        cov_last = cov_this
-        std_last = np.sqrt(np.diag(cov_last))
-        jj += 1
-
-    return mean_this, cov_this, mask
-
-def symmetrizedist(vals):
-    """
-    Function to symmetrize a distribution about zero. Useful for if the
-    distribution of some value centers around a nonzero value, but
-    should center around zero. An example of this would be when most of
-    the measured slopes are nonzero, but we want the slopes with zero
-    values (e.g. lots of muon tails, which we want to cut out). To do
-    this, the algorithm randomly chooses points in a histogram to cut
-    out until the histogram is symmetric about zero.
+    4 rise/fall times, 3 amplitudes, and time offset allowed to
+    float.
 
     Parameters
     ----------
-    vals : ndarray
-        A 1-d array of the values that will be symmetrized.
+    t : ndarray
+        Array of time values to make the pulse with
+    A : float
+        Amplitude for first fall time
+    B : float
+        Amplitude for second fall time
+    C : float
+        Amplitude for third fall time
+    tau_r : float
+        Rise time of pulse
+    tau_f1 : float
+        First fall time of pulse
+    tau_f2 : float
+        Second fall time of pulse
+    tau_f3 : float
+        Third fall time of pulse
+    t0 : float, optional
+        Time offset of three pole pulse
+        Default: 1/2 trace
+    fs :  float, required if t0 not None
+        sample rate
+    normalize : boolean, optional
+        if True, normalize pulse with maximum pulse
 
     Returns
     -------
-    czeromeanslope : ndarray
-        A boolean mask of the values that should be kept.
+    pulse : ndarray
+        Array of amplitude values as a function of time
 
     """
 
-    nvals = len(vals)
-    # figure out which direction the slopes are usually
-    valsmean, valsstd = iterstat(vals, cut=2, precision=10000.0)[:-1]
-
-    # if most vals are positive, flip the sign of them so we can use
-    # the same code for both negative and positive vals
-    if valsmean>0.0:
-        vals= vals
-
-    # choose symmetric upper and lower bounds for histogram to make
-    # the middle bin centered on zero (since we want zero mean)
-    histupr=max(vals)
-    histlwr=-histupr
-
-    # specify number of bins in histogram (should be an odd number
-    # so that we have the middle bin centered on zero)
-    histbins=int(np.sqrt(nvals))
-    if np.mod(histbins,2)==0:
-        histbins+=1
-
-    if histupr>0:
-        # create histogram, get number of events in each bin and
-        # where the bin edges are
-        hist_num, bin_edges = np.histogram(
-            vals,
-            bins=histbins,
-            range=(histlwr, histupr),
-        )
+    pulse = (
+        A * (np.exp(-t / tau_f1))
+    ) + (
+        B * (np.exp(-t / tau_f2))
+    ) + (
+        C * (np.exp(-t / tau_f3))
+    ) - (
+        (A + B + C) * (np.exp(-t / tau_r))
+    )
 
-        if len(hist_num)>2: # otherwise we cannot symmetrize the distribution
-            # inititalize the cut that symmetrizes the slopes
-            czeromeanvals = np.zeros(nvals, dtype=bool)
-            czeromeanvals[vals>bin_edges[histbins//2]] = True
-
-            # go through each bin and remove events until the bin number
-            # is symmetric
-            for ibin in range(histbins//2, histbins-1):
-                cvalsinbin = np.logical_and(
-                    vals<bin_edges[histbins-ibin-1],
-                    vals>=bin_edges[histbins-ibin-2],
-                )
-                ntracesinthisbin = hist_num[histbins-ibin-2]
-                ntracesinoppobin = hist_num[ibin+1]
-                ntracestoremove = ntracesinthisbin-ntracesinoppobin
-                if ntracestoremove>0.0:
-                    cvalsinbininds = np.where(cvalsinbin)[0]
-                    crandcut = np.random.choice(
-                        cvalsinbininds, ntracestoremove, replace=False,
-                    )
-                    cvalsinbin[crandcut] = False
-                # update cut to include these events
-                czeromeanvals += cvalsinbin
-        else:
-            # don't do anything about the shape of the distrbution
-            czeromeanvals = np.ones(nvals, dtype=bool)
-    else:
-        # don't do anything about the shape of the distrbution
-        czeromeanvals = np.ones(nvals, dtype=bool)
 
-    return czeromeanvals
+    # offset -> default 1/2 traces
+    offset = len(t)//2
+    if t0 is not None:
+        if fs is None:
+            raise ValueError(
+                'ERROR: sample rate (fs) '
+                + ' required!'
+            )
+        offset = int(t0 * fs)
+            
+    pulse = shift(pulse, offset)
+    
+    # normalize
+    if normalize:
+        pulse = pulse/pulse.max()
+        
+    return pulse
 
 
-class _PlotCut(object):
+def make_decreasing(y, x=None):
     """
-    Helper class for storing plotting functions for use in IterCut.
+    Function to take an array of values and make it monotonically
+    decreasing. This is done by simply tossing out any values that are
+    larger than the last value, moving from the first index to the
+    last, and interpolating between values.
+
+    Parameters
+    ----------
+    y : ndarray
+        Array of values to make monotonically decreasing.
+    x : ndarray, optional
+        The x-values corresponding to `y`, can be useful if the
+        x-values are not evenly spaced.
+
+    Returns
+    -------
+    out : ndarray
+        A monotonically decreasing version of `y`.
 
     """
 
-    def _get_plot_inds(self, cout):
-        """
-        Hidden function for accessing the indices that specify passing
-        events and failing events given some cut on the data.
+    if x is None:
+        x = np.arange(len(y))
 
-        """
+    y_dec = np.zeros(len(y))
+    y_dec[0] = y[0]
+    last_val = y[0]
 
-        cinds_pre = self._cutinds
+    for ii, val in enumerate(y):
+        if (last_val > val):
+            last_val = y[ii]
+            y_dec[ii] = y[ii]
 
-        cpass = self._cutinds[cout]
-        npass = len(cpass)
-        cfail = np.setdiff1d(cinds_pre, cpass)
-        nfail = len(cfail)
+    interp_inds = y_dec!=0
 
-        fail_plot = np.random.choice(
-            cfail,
-            size=self._nplot if nfail > self._nplot else nfail,
-            replace=False,
-        )
+    f = interpolate.interp1d(
+        x[interp_inds], y[interp_inds], fill_value="extrapolate",
+    )
 
-        pass_plot = np.random.choice(
-            cpass,
-            size=self._nplot if npass > self._nplot else npass,
-            replace=False,
-        )
+    out = f(x)
 
-        return np.sort(fail_plot), np.sort(pass_plot)
+    return out
 
-    def _plot_events(self, cout):
-        """
-        Hidden function for plotting passing events and failing events
-        given some cut on the data.
 
-        """
+def calc_offset(x, fs=1.0, sgfreq=100.0, is_didv=False):
+    """
+    Calculates the DC offset of time series trace.
 
-        fail_inds, pass_inds = self._get_plot_inds(cout)
+    Parameters
+    ----------
+    x : ndarray
+        Array to calculate offsets of.
+    fs : float, optional
+        Sample rate of the data being taken, assumed to be in units
+        of Hz.
+    sgfreq : float, optional
+        The frequency of signal generator (if is_didv is True. If False,
+        then this is ignored).
+    is_didv : bool, optional
+        If False, average of full trace is returned. If True, then the
+        average of n periods is returned (where n is the max number of
+        full periods present in a trace).
 
-        fig, axes = plt.subplots(ncols=2, sharex=True)
-        time = np.arange(self._nbin) / self.fs
+    Returns
+    -------
+    offset : ndarray
+        Array of offsets with same shape as input x minus the last
+        dimension.
+    std : ndarray
+        Array of std with same shape as offset.
 
-        for temp_trace in self.traces[fail_inds]:
-            axes[0].plot(time * 1e3, temp_trace, alpha=0.5)
+    """
 
-        for temp_trace in self.traces[pass_inds]:
-            axes[1].plot(time * 1e3, temp_trace, alpha=0.5)
+    if is_didv:
+        period =  1.0 / sgfreq
+        period_bins = period * fs
+        n_periods = int(x.shape[-1] / period_bins)
+        x = x[..., :int(n_periods * period_bins)]
 
-        axes[0].set_title('Failed Cut')
-        axes[0].set_xlim(time[0] * 1e3, time[-1] * 1e3)
+    offset = np.mean(np.mean(x, axis=-1), axis=0)
+    std = np.std(np.mean(x, axis=-1), axis=0) / np.sqrt(x.shape[0])
 
-        axes[1].set_title('Passed Cut')
-        axes[1].yaxis.set_label_position("right")
-        axes[1].yaxis.tick_right()
+    return offset, std
 
-        for ax in axes:
-            ax.tick_params(
-                which='both',
-                direction='in',
-                right=True,
-                top=True,
-                left=True,
-            )
+def slope(x, y, removemeans=True):
+    """
+    Computes the maximum likelihood slope of a set of x and y points.
 
-        fig.add_subplot(111, frameon=False)
-        plt.tick_params(
-            labelcolor='none',
-            which='both',
-            top=False,
-            bottom=False,
-            left=False,
-            right=False,
-        )
-        plt.xlabel("Time [ms]")
+    Parameters
+    ----------
+    x : array_like
+        Array of real-valued independent variables.
+    y : array_like
+        Array of real-valued dependent variables.
+    removemeans : bool
+        Boolean flag for if the mean of x should be subtracted. This
+        should be set to True if x has not already had its mean
+        subtracted. Set to False if the mean has been subtracted.
+        Default is True.
+
+    Returns
+    -------
+    slope : float
+        Maximum likelihood slope estimate, calculated as
+        sum((x-<x>)(y-<y>))/sum((x-<x>)**2)
+
+    """
+
+    x_mean = np.mean(x) if removemeans else 0
 
+    return np.sum((x - x_mean) * (y - x_mean)) / np.sum((x - x_mean) ** 2)
 
-class IterCut(_PlotCut):
+def fill_negatives(arr):
     """
-    Class for iteratively applying various cuts to data while being
-    able to track what events were cut between steps.
+    Simple helper function to remove negative and zero values from PSDs
+    and replace them with interpolated values.
 
-    Attributes
+    Parameters
     ----------
-    traces : ndarray
-        The traces that will be cut on.
-    fs : float
-        The digitization rate of the traces.
-    cmask : ndarray
-        The current data quality cut after applying the cuts before
-        this. This is a protected attribute.
-
-    """
-
-    def __init__(self, traces, fs, plotall=False, nplot=10):
-        """
-        Initialization of the IterCut class object.
-
-        Parameters
-        ----------
-        traces : ndarray
-            The traces that will be cut on.
-        fs : float
-            The digitization rate of the traces.
-        plotall : bool, optional
-            If True, the events that pass or fail each cut will be
-            plotted at each step. Default is False. To plot events that
-            pass or fail specific cuts, use the `verbose` kwarg when
-            applying those cuts to the data.
-        nplot : int, optional
-            The number of events that should be plotted from each
-            set of passing events and failing events. Default is 10.
-
-        """
-
-        self.traces = traces
-        self.fs = fs
-        self._plotall = plotall
-        self._nplot = nplot
-        self._ntraces = len(traces)
-        self._nbin = len(traces[0])
-        self._cutinds = np.arange(len(traces))
-
-    @property
-    def cmask(self):
-        _cmask = np.zeros(self._ntraces, dtype=bool)
-        _cmask[self._cutinds] = True
-        return _cmask
-
-    @cmask.setter
-    def cmask(self, value):
-        raise AttributeError("cmask is a protected attribute, can't set it")
-
-    @cmask.deleter
-    def cmask(self):
-        raise AttributeError("cmask is a protected attribute, can't delete it")
-
-    def _run_algo(self, vals, outlieralgo, verbose, **kwargs):
-        """
-        Hidden function for running the outlier algorithm on a set of
-        values.
-
-        """
-
-        if outlieralgo=="iterstat":
-            cout = iterstat(vals, **kwargs)[2]
-        elif outlieralgo=="removeoutliers": 
-            cout = removeoutliers(vals, **kwargs)
-        elif outlieralgo=="sigma_clip":
-            array = sigma_clip(vals, axis=0, masked=False, **kwargs)
-            cout = ~np.isnan(array)
-        else:
-            raise ValueError(
-                "Unrecognized outlieralgo, must be a str "
-                "of 'iterstat', 'removeoutliers', or 'sigma_clip'"
-            )
+    arr : ndarray
+        Array of values to replace neagive values on
 
-        if self._plotall or verbose:
-            self._plot_events(cout)
+    Returns
+    -------
+    arr : ndarray
+        Modified input array with the negative and zero values replace
+        by interpolated values.
+
+    """
 
-        self._cutinds = self._cutinds[cout]
+    zeros = np.array(arr <= 0)
+    inds_zero = np.where(zeros)[0]
+    inds_not_zero = np.where(~zeros)[0]
+    good_vals = arr[~zeros]
 
-    def pileupcut(self, template=None, psd=None, removemeans=False,
-                  outlieralgo="iterstat", verbose=False, **kwargs):
-        """
-        Function to automatically cut out outliers of the optimum
-        filter amplitudes of the inputted traces.
-
-        Parameters
-        ----------
-        template : ndarray, NoneType, optional
-            The pulse template to use for the optimum filter. If
-            not passed, then a 10 us rise time and 100 us fall time
-            pulse is used.
-        psd : ndarray, NoneType, optional
-            The two-sided PSD (units of A^2/Hz) to use for the
-            optimum filter. If not passed, then all frequencies are
-            weighted equally.
-        removemeans : bool, optional
-            Boolean flag for if the mean of each trace should be
-            removed before doing the optimum filter (True) or if the
-            means should not be removed (False). This is useful for
-            dIdV traces, when we want to cut out pulses that have
-            smaller amplitude than the dIdV overshoot. Default is
-            False.
-        outlieralgo : str, optional
-            Which outlier algorithm to use: iterstat, removeoutliers,
-            or astropy's sigma_clip. Default is "iterstat".
-        verbose : bool, optional
-            If True, the events that pass or fail each cut will be
-            plotted at each step. Default is False. If `plotall` is
-            True when initializing this class, then this will be
-            ignored in favor of `plotall`.
-        **kwargs
-            Keyword arguments to pass to the outlier algorithm function
-            call.
-
-        Returns
-        -------
-        cpileup : ndarray
-            Boolean array giving which indices to keep or throw out
-            based on the outlier algorithm.
-
-        """
-
-        if template is None:
-            time = np.arange(self._nbin) / self.fs
-            template = make_template(time, 10e-6, 100e-6)
-
-        if psd is None:
-            psd = np.ones(self._nbin)
-
-        temp_traces = self.traces[self._cutinds]
-
-        if removemeans:
-            mean = np.mean(temp_traces, axis=-1, keepdims=True)
-            temp_traces -= mean
-
-        ntemptraces = len(temp_traces)
-
-        amps = np.zeros(ntemptraces)
-
-        #do optimum filter on all traces
-        for itrace in range(ntemptraces):
-            amps[itrace] = ofamp(
-                temp_traces[itrace], template, psd, self.fs,
-            )[0]
-
-        self._run_algo(np.abs(amps), outlieralgo, verbose, **kwargs)
-
-        return self.cmask
-
-    def baselinecut(self, endindex=None, outlieralgo="iterstat",
-                    verbose=False, **kwargs):
-        """
-        Function to automatically cut out outliers of the baselines
-        of the inputted traces.
-
-        Parameters
-        ----------
-        endindex : int, NoneType, optional
-            The end index of the trace to average up to for the
-            basleine calculation. If not passed, the default value
-            is half of the trace length.
-        outlieralgo : str, optional
-            Which outlier algorithm to use: iterstat, removeoutliers,
-            or astropy's sigma_clip. Default is "iterstat".
-        verbose : bool, optional
-            If True, the events that pass or fail each cut will be
-            plotted at each step. Default is False. If `plotall` is
-            True when initializing this class, then this will be
-            ignored in favor of `plotall`.
-        **kwargs
-            Keyword arguments to pass to the outlier algorithm function
-            call.
-
-        Returns
-        -------
-        cbaseline : ndarray
-            Boolean array giving which indices to keep or throw out
-            based on the outlier algorithm.
+    if len(good_vals) != 0:
+        arr[zeros] = np.interp(inds_zero, inds_not_zero, good_vals)
 
-        """
-        
-        temp_traces = self.traces[self._cutinds]
-        ntemptraces = len(temp_traces)
+    return arr
 
-        if endindex is None:
-            endindex = self._nbin // 2
 
-        baselines = np.mean(temp_traces[..., :endindex], axis=-1)
 
-        self._run_algo(baselines, outlieralgo, verbose, **kwargs)
-
-        return self.cmask
-
-    def slopecut(self, outlieralgo="iterstat", verbose=False, **kwargs):
-        """
-        Function to automatically cut out outliers of the slopes of the
-        inputted traces. Slopes are calculated via maximum likelihood
-        and use the entire trace.
-
-        Parameters
-        ----------
-        outlieralgo : str, optional
-            Which outlier algorithm to use: iterstat, removeoutliers,
-            or astropy's sigma_clip. Default is "iterstat".
-        verbose : bool, optional
-            If True, the events that pass or fail each cut will be
-            plotted at each step. Default is False. If `plotall` is
-            True when initializing this class, then this will be
-            ignored in favor of `plotall`.
-        **kwargs
-            Keyword arguments to pass to the outlier algorithm function
-            call.
-
-        Returns
-        -------
-        cslope : ndarray
-            Boolean array giving which indices to keep or throw out
-            based on the outlier algorithm.
-
-        """
-
-        temp_traces = self.traces[self._cutinds]
-        ntemptraces = len(temp_traces)
-        time = np.arange(self._nbin) / self.fs
-        ymean = np.mean(temp_traces, axis=-1, keepdims=True)
-        xmean = np.mean(time)
-
-        slopes = np.sum(
-            (time - xmean) * (temp_traces - ymean),
-            axis=-1,
-        ) / np.sum(
-            (time - xmean)**2,
-        )
+def lowpassfilter(traces, cut_off_freq=100000, fs=625e3, order=1):
+    """
+    Applies a low pass filter to the inputted time series traces.
+
+    Parameters
+    ----------
+    traces : ndarray
+        An array of shape (# traces, # bins per trace).
+    cut_off_freq : float, int, optional
+        The cut off 3dB frequency for the low pass filter, defaults to
+        100000 Hz.
+    fs : float, int, optional
+        Digitization rate of data, defaults to 625e3 Hz.
+    order : int, optional
+        The order of the low pass filter, defaults to 1.
+
+    Returns
+    -------
+    filt_traces : ndarray
+        Array of low pass filtered traces with the same shape as
+        inputted traces.
+
+    """
 
-        self._run_algo(slopes, outlieralgo, verbose, **kwargs)
+    nyq = 0.5 * fs
+    cut_off = cut_off_freq / nyq
+    b,a = signal.butter(order, cut_off)
+    filt_traces = signal.filtfilt(b, a, traces, padtype='even')
 
-        return self.cmask
+    return filt_traces
 
-    def chi2cut(self, template=None, psd=None, outlieralgo="iterstat",
-                verbose=False, **kwargs):
-        """
-        Function to automatically cut out outliers of the optimum
-        filter chi-squares of the inputted traces.
-
-        Parameters
-        ----------
-        template : ndarray, NoneType, optional
-            The pulse template to use for the optimum filter. If
-            not passed, then a 10 us rise time and 100 us fall time
-            pulse is used.
-        psd : ndarray, NoneType, optional
-            The two-sided PSD (units of A^2/Hz) to use for the
-            optimum filter. If not passed, then all frequencies are
-            weighted equally.
-        outlieralgo : str, optional
-            Which outlier algorithm to use: iterstat, removeoutliers,
-            or astropy's sigma_clip. Default is "iterstat".
-        verbose : bool, optional
-            If True, the events that pass or fail each cut will be
-            plotted at each step. Default is False. If `plotall` is
-            True when initializing this class, then this will be
-            ignored in favor of `plotall`.
-        **kwargs
-            Keyword arguments to pass to the outlier algorithm function
-            call.
-
-        Returns
-        -------
-        cchi2 : ndarray
-            Boolean array giving which indices to keep or throw out
-            based on the outlier algorithm.
-
-        """
-
-        if template is None:
-            time = np.arange(self._nbin) / self.fs
-            template = make_template(time, 10e-6, 100e-6)
-
-        if psd is None:
-            psd = np.ones(self._nbin)
-
-        temp_traces = self.traces[self._cutinds]
-        ntemptraces = len(temp_traces)
-
-        chi2s = np.zeros(ntemptraces)
-
-        #do optimum filter on all traces
-        for itrace in range(ntemptraces):
-            chi2s[itrace] = ofamp(
-                temp_traces[itrace], template, psd, self.fs,
-            )[-1]
-
-        self._run_algo(chi2s, outlieralgo, verbose, **kwargs)
-
-        return self.cmask
-
-    def arbitrarycut(self, cutfunction, *args, outlieralgo="iterstat",
-                     verbose=False, **kwargs):
-        """
-        Function to automatically cut out outliers of the optimum
-        filter amplitudes of the inputted traces.
-
-        Parameters
-        ----------
-        cutfunction : FunctionType
-            A function to set cuts on. Should be able to take
-            in the traces ndarray, and any other arguments can
-            be passed before defining the kwargs.
-        *args
-            The arguments that should be passed to `cutfunction`
-            beyond the traces.
-        outlieralgo : str, optional
-            Which outlier algorithm to use: iterstat, removeoutliers,
-            or astropy's sigma_clip. Default is "iterstat".
-        verbose : bool, optional
-            If True, the events that pass or fail each cut will be
-            plotted at each step. Default is False. If `plotall` is
-            True when initializing this class, then this will be
-            ignored in favor of `plotall`.
-        **kwargs
-            Keyword arguments to pass to the outlier algorithm function
-            call.
-
-        Returns
-        -------
-        cpileup : ndarray
-            Boolean array giving which indices to keep or throw out
-            based on the outlier algorithm.
-
-        """
-
-        temp_traces = self.traces[self._cutinds]
-        vals = cutfunction(temp_traces, *args)
-
-        self._run_algo(vals, outlieralgo, verbose, **kwargs)
-
-        return self.cmask
-
-
-def autocuts(traces, fs=625e3, template=None, psd=None, is_didv=False,
-             outlieralgo="iterstat", lgcpileup1=True, lgcslope=True,
-             lgcbaseline=True, lgcpileup2=True, lgcchi2=True, nsigpileup1=2,
-             nsigslope=2, nsigbaseline=2, nsigpileup2=2, nsigchi2=3,
-             **kwargs):
+def align_traces(traces, lgcjustshifts=False, n_cut=5000, cut_off_freq=5000.0,
+                 fs=625e3):
     """
-    Function to automatically cut out bad traces based on the optimum
-    filter amplitude, slope, baseline, and chi^2 of the traces.
+    Function to align dIdV traces if each trace does not trigger at the
+    same point. Uses a convolution of the traces to find the time
+    offset.
 
     Parameters
     ----------
     traces : ndarray
-        2-dimensional array of traces to do cuts on
-    fs : float, optional
-        Sample rate that the data was taken at
-    is_didv : bool, optional
-        Boolean flag on whether or not the trace is a dIdV curve
-    outlieralgo : string, optional
-        Which outlier algorithm to use. If set to "removeoutliers",
-        uses the removeoutliers algorithm that removes data based on
-        the skewness of the dataset. If set to "iterstat", uses the
-        iterstat algorithm to remove data based on being outside a
-        certain number of standard deviations from the mean. Can also
-        be set to astropy's "sigma_clip".
-    lgcpileup1 : boolean, optional
-        Boolean value on whether or not do the pileup1 cut (this is the
-        initial pileup cut that is always done whether or not we have
-        dIdV data). Default is True.
-    lgcslope : boolean, optional
-        Boolean value on whether or not do the slope cut. Default is
-        True.
-    lgcbaseline : boolean, optional
-        Boolean value on whether or not do the baseline cut. Default is
-        True.
-    lgcpileup2 : boolean, optional
-        Boolean value on whether or not do the pileup2 cut (this cut is
-        only done when is_didv is also True). Default is True.
-    lgcchi2 : boolean, optional
-        Boolean value on whether or not do the chi2 cut. Default is
-        True.
-    nsigpileup1 : float, optional
-        If outlieralgo is "iterstat", this can be used to tune the
-        number of standard deviations from the mean to cut outliers
-        from the data when using iterstat on the optimum filter
-        amplitudes. Default is 2.
-    nsigslope : float, optional
-        If outlieralgo is "iterstat", this can be used to tune the
-        number of standard deviations from the mean to cut outliers
-        from the data when using iterstat on the slopes. Default is 2.
-    nsigbaseline : float, optional
-        If outlieralgo is "iterstat", this can be used to tune the
-        number of standard deviations from the mean to cut outliers
-        from the data when using iterstat on the baselines. Default is
-        2.
-    nsigpileup2 : float, optional
-        If outlieralgo is "iterstat", this can be used to tune the
-        number of standard deviations from the mean to cut outliers
-        from the data when using iterstat on the optimum filter
-        amplitudes after the mean has been subtracted. (only used if
-        is_didv is True). Default is 2.
-    nsigchi2 : float, optional
-        This can be used to tune the number of standard deviations
-        from the mean to cut outliers from the data when using iterstat
-        on the chi^2 values. Default is 3.
-    **kwargs
-        Placeholder kwargs for backwards compatibility.
+        Array of shape (# traces, # bins per trace).
+    lgcjustshifts : boolean, optional
+        If False, the aligned traces and the phase shifts are returned.
+        If True, just the phase shifts are returned. Default is False.
+    n_cut : int, optional
+        The number of bins to use to do the convolution. Just need
+        enough information to see the periodic signal. Default is
+        5000.
+    cut_off_freq : float or int, optional
+        3dB cut off frequency for filter. Default is 5000 Hz.
+    fs : float or int, optional
+        Sample rate of data in Hz. Default is 625e3 Hz.
 
     Returns
     -------
-    ctot : ndarray
-        Boolean array giving which indices to keep or throw out based
-        on the autocuts algorithm.
+    shifts : ndarray
+        Array of phase shifts for each trace in units of bins.
+    masked_aligned : masked ndarray, optional
+        Array of time shift corrected traces, same shape as input
+        traces. The masked array masks the np.NaN values in the time
+        shifted traces so that normal numpy functions will ignore the
+        nan's in computations.
 
     """
 
-    if is_didv and 'sgfreq' in kwargs:
-        warnings.warn(
-            "The `sgfreq` option has been deprecated and "
-            "is now ignored when is_didv is True."
-        )
+    # Filter and truncate all traces to speed up.
+    traces_filt = lowpassfilter(
+        traces[:, :n_cut], cut_off_freq=5000, fs=625e3,
+    )
+    traces_temp = traces_filt - np.mean(traces_filt, axis=-1, keepdims=True)
+    traces_norm = traces_temp / (np.amax(traces_temp, axis=-1, keepdims=True))
+
+    # use the first trace to define the origin of alignment
+    t1 = traces_norm[0]
+    # define the origin
+    orig = np.argmax(signal.fftconvolve(t1,t1[::-1],mode = 'full'))
+
+    # initialize empty array to store the aligned traces
+    traces_aligned = np.zeros_like(traces)
+    shifts = np.zeros(traces.shape[0])
+
+    for ii in range(traces.shape[0]):
+        t2 = traces_norm[ii]
+        # Convolve each trace against the origin trace, find the index of the
+        # max value, then subtract of the index of the origin trace
+        t2_shift = np.argmax(
+            signal.fftconvolve(t1, t2[::-1], mode='full'),
+        ) - orig
+        shifts[ii] = t2_shift
+        if not lgcjustshifts:
+            traces_aligned[ii] = ndimage.shift(
+                traces[ii], t2_shift, cval=np.nan,
+            )
 
-    Cut = IterCut(traces, fs)
+    if lgcjustshifts:
+        return shifts
+    else:
+        flat_aligned = traces_aligned.flatten()
+        masked_aligned = np.ma.array(
+            flat_aligned,
+            mask=np.isnan(flat_aligned),
+        ).reshape(traces_aligned.shape)
 
-    if lgcpileup1:
-        kwargs = {'cut': nsigpileup1} if outlieralgo=="iterstat" else {}
-        Cut.pileupcut(
-            template=template,
-            psd=psd,
-            outlieralgo=outlieralgo,
-            **kwargs,
-        )
+        return shifts, masked_aligned
 
-    if lgcslope:
-        kwargs = {'cut': nsigslope} if outlieralgo=="iterstat" else {}
-        Cut.slopecut(outlieralgo=outlieralgo, **kwargs)
-
-    if lgcbaseline:
-        kwargs = {'cut': nsigbaseline} if outlieralgo=="iterstat" else {}
-        Cut.baselinecut(outlieralgo=outlieralgo, **kwargs)
-
-    # do a pileup cut on the mean subtracted data if this is a dIdV,
-    # so that we remove pulses that are smaller than the dIdV peaks
-    if lgcpileup2 and is_didv:
-        kwargs = {'cut': nsigpileup2} if outlieralgo=="iterstat" else {}
-        Cut.pileupcut(
-            template=template,
-            psd=psd,
-            removemeans=True,
-            outlieralgo=outlieralgo,
-            **kwargs,
-        )
+def get_offset_from_muon(avemuon, qetbias, rn, rload, rsh=5e-3,
+                         nbaseline=6000, lgcfullrtn=True):
+    """
+    Function to calculate the offset in the measured TES current using
+    an average muon.
 
-    if lgcchi2:
-        kwargs = {'cut': nsigchi2} if outlieralgo=="iterstat" else {}
-        Cut.chi2cut(
-            template=template,
-            psd=psd,
-            outlieralgo=outlieralgo,
-            **kwargs,
-        )
+    Parameters
+    ----------
+    avemuon : ndarray
+        An average of 'good' muons in time domain, referenced to TES
+        current.
+    qetbias : float
+        Applied QET bias current
+    rn : float
+        Normal resistance of the TES
+    rload : float
+        Load resistance of TES circuit (rp + rsh)
+    rsh : float, optional
+        Value of the shunt resistor for the TES circuit
+    nbaseline : int, optional
+        The number of bins to use to calculate the baseline,
+        i.e. [0:nbaseline].
+    lgcfullrtn : bool, optional
+        If True, the offset, r0, i0, and bias power is returned. If
+        False, just the offset is returned.
+
+    Returns
+    -------
+    ioffset : float
+        The offset in the measured TES current.
+    r0 : float, optional
+        The resistance of the TES.
+    i0 : float, optional
+        The quiescent current through the TES.
+    p0 : float, optional
+        The quiescent bias power of the TES.
+
+    """
+
+    muon_max = np.max(avemuon)
+    baseline = np.mean(avemuon[:int(nbaseline)])
+    peak_loc = np.argmax(avemuon)
 
-    return Cut.cmask
+    muon_saturation = np.mean(avemuon[peak_loc:peak_loc+200])
+    muon_deltaI =  muon_saturation - baseline
 
+    vbias = qetbias * rsh
+    inormal = vbias / (rload + rn)
 
-def get_muon_cut(traces, thresh_pct=0.95, nsatbins=600):
+    i0 = inormal - muon_deltaI
+    ioffset = baseline - i0
+
+    r0 = inormal * (rn + rload)/i0 - rload
+    p0 = i0 * rsh * qetbias - rload * i0**2
+
+    if lgcfullrtn:
+        return ioffset, r0, i0, p0
+    else:
+        return ioffset
+
+def powertrace_simple(trace, ioffset, qetbias, rload, rsh):
     """
-    Function to help identify saturated muons from array of time series
+    Function to convert time series trace from units of TES current to
+    units of power. This can be done for either a single trace, or an
+    array of traces, as long as the first dimension is the number of
     traces.
 
-    ***Traces must have POSITIVE going pulses***
+    The function takes into account the second order dependence on
+    current, but assumes the infinite Irwin loop gain approximation.
+
+    Parameters
+    ----------
+    trace : ndarray
+        Time series traces, where the last dimension is the trace
+        length, referenced to TES current.
+    ioffset : float
+        The offset in the measured TES current.
+    qetbias : float
+        Applied QET bias current.
+    rload : float
+        Load resistance of TES circuit (rp + rsh).
+    rsh : float
+        Value of the shunt resistor for the TES circuit.
+
+    Returns
+    -------
+    trace_p : ndarray
+        Time series trace, in units of power referenced to the TES.
+
+    """
+
+    vbias = qetbias * rsh
+    trace_i0 = trace - ioffset
+    trace_p = trace_i0*vbias - (rload) * trace_i0**2
+
+    return trace_p
 
-    Note, for best results, only large amplitude traces should based to
-    this function. The user may need to play around with the thresh_pct
-    and nsatbins parameters to achive the desired result. 
+
+def energy_absorbed(trace, ioffset, qetbias, rload, rsh, fs=None,
+                    baseline=None, time=None, indbasepre=None,
+                    indbasepost=None):
+    """
+    Function to calculate the energy collected by the TESs by
+    integrating the power in the TES as a function of time. This can be
+    done for either a single trace, or an array of traces, as long as
+    the first dimension is the number of traces.
 
     Parameters
     ----------
-    traces: array
-        Array of time series traces of shape (#number of traces, #bins
-        per trace).
-    thresh_pct: float, optional
-        The percentage of the maximum amplitude that the pulse must
-        remain above for nsatbins in order to be considered
-        `saturated'.
-    nsatbins: int, optional
-        The minimum number of bins that a muon should be saturated for.
+    trace : ndarray
+        Time series traces, where the last dimension is the trace
+        length, referenced to TES current.
+    ioffset : float
+        The offset in the measured TES current.
+    qetbias : float
+        Applied QET bias current.
+    rload : float
+        Load resistance of TES circuit (rp + rsh).
+    rsh : float
+        Value of the shunt resistor for the TES circuit.
+    fs : float, optional
+        The sample rate of the DAQ
+    baseline : ndarray, optional
+        The baseline value of each trace, must be same dimension as
+        trace.
+    time : ndarray, optional
+        Array of time values corresponding to the trace array.
+    indbasepre : int, optional
+        The bin number corresponding to the pre-pulse baseline,
+        i.e. [:indbasepre]
+    indbasepost : int, optional
+        The bin number corresponding to the post-pulse baseline,
+        i.e. [indbasepost:]
 
     Returns
     -------
-    muon_cut: array
-        Boolean array corresponding to saturated muon events
+    integrated_energy : float, ndarray
+        The energy absorbed by the TES in units of eV.
 
     """
 
-    muon_cut = np.zeros(shape = len(traces), dtype = bool)
-    for ii, trace in enumerate(traces):
-        trace_max = np.max(trace)
-        # check that the maximum value of the trace is above the threshold and
-        # that the maximum is decently larger than the minimum
-        peak_loc = np.argmax(trace)
+    if baseline is None:
+        if indbasepre is not None:
+            base_traces = trace[..., :indbasepre]
+        else:
+            raise ValueError('Must provide indbasepre or baseline')
+        if indbasepost is not None:
+            base_traces = np.hstack((base_traces, trace[..., indbasepost:]))
+        baseline = np.mean(base_traces, axis=-1, keepdims=True)
+
+    baseline_p0 = powertrace_simple(baseline, ioffset, qetbias, rload, rsh)
+    trace_power = powertrace_simple(trace, ioffset, qetbias, rload, rsh)
+
+    if fs is not None:
+        integrated_energy = np.trapz(
+            baseline_p0 - trace_power, axis=-1,
+        ) / (fs * constants.e)
+    elif time is not None:
+        integrated_energy = np.trapz(
+            baseline_p0 - trace_power, x=time, axis=-1,
+        ) / constants.e
+    else:
+        raise ValueError('Must provide either fs or time')
+
+    return integrated_energy
 
-        # check that the peak is saturated (this should be true for muons
-        # that saturate the detector or muon that rail the amplifier) 
-        if ((peak_loc + int(nsatbins)) < traces.shape[-1]):
-            if (trace[peak_loc+int(nsatbins)] >= trace_max*thresh_pct):
-                muon_cut[ii] = True
+def estimate_g(p0, tc, tbath, p0_err=0, cov=None, n=5):
+    """
+    Function to estimate G given the measured bias power and know Tc
+    and bath temperature.
+
+    Parameters
+    ----------
+    p0 : float
+        The applied bias power.
+    tc : float
+        The SC transition temperature of the TES.
+    tbath : float
+        The bath temperature.
+    p0_err : float, optional
+        The error in the bias power.
+    cov : ndarray, NoneType, optional
+        The covariance matrix for the parameters in order: p0, tc,
+        tbath. If None, the error is just calculated from p0_err.
+    n : int, optional
+        The exponent of the power law expression. Defaults to 5.
+
+    Returns
+    -------
+    g : float
+        The estimated thermal conductance.
+    g_err : float
+        The error in the estimated thermal conductance.
+
+    """
+
+    g = n * p0 * tc**(n - 1) / (tc**n - tbath**n)
+
+    if cov is not None:
+        dgdp = g / p0
+        dgdtc = (n - 1) * g / tc - g * n * (tc**(n - 1)) / (tc**n - tbath**n)
+        dgdtbath = n * g * tbath**(n - 1) / (tc**n - tbath**n)
+
+        jac = np.zeros((3,3))
+        jac[0,0] = dgdp
+        jac[1,1] = dgdtc
+        jac[2,2] = dgdtbath
+        covout = jac.dot(cov.dot(jac.transpose()))
+        g_err = np.sqrt(np.sum(covout))
+    else:
+        g_err = np.abs(p0_err * g / p0)
+
+    return g, g_err
+
+
+
+
+def interpolate_parabola(vals, bestind, delta, t_interp=None):
+    """
+    Precomputed equation of a parabola given 3 equally spaced
+    points. Returns the coordinates of the extremum of the
+    parabola.
+    """
+
+    sf = 1 / (2 * delta**2)
+    
+    a = sf * (vals[bestind + 1] - 2 * vals[bestind] + vals[bestind - 1])
+    b = sf * delta * (vals[bestind + 1] - vals[bestind - 1])
+    c = sf * 2 * delta**2 * vals[bestind]
+    
+    if t_interp is None:
+        t_interp = - b / (2 * a)
+    vals_interp = a * t_interp**2 + b * t_interp + c
+        
+    return t_interp, vals_interp
+
+
+    
+   
+def interpolate_of(amps, chi2, bestind, delta):
+    """
+    Helper function for running `_interpolate_parabola` twice,
+    in the correct order.
+    """
+    
+    t_interp, chi2_interp = interpolate_parabola(
+        chi2, bestind, delta,
+    )
+    _, amps_interp = interpolate_parabola(
+        amps, bestind, delta, t_interp=t_interp,
+    )
+    
+    return amps_interp, t_interp, chi2_interp
+
+
+
+
+def argmin_chisq(chisq,
+                 window_min=None,
+                 window_max=None,
+                 lgc_outside_window=False,
+                 constraint_mask=None):
+    """
+    Helper function for finding the index for the minimum of a chi^2.
+    Includes options for constraining the values of chi^2.
+        
+    Parameters
+    ----------
+    chi2 : ndarray
+             An array containing the chi^2 to minimize. If `chi2` has
+             dimension greater than 1, then it is minimized along the last
+             axis. 
+
+    window_min : NoneType, int, optional
+         This is the window minimum length  (in bins) to
+          constrain the possible values to in the chi^2 minimization,
+          Default is None, `chi2` is uncontrained is both 
+          window min/max = None
+    
+    window_max : NoneType, int, optional
+          This is the window maximum length  (in bins) to
+          constrain the possible values to in the chi^2 minimization,
+          Default is None, `chi2` is uncontrained is both 
+          window min/max = None
+    
+
+    
+    lgcoutsidewindow : bool, optional
+        If False, then the function will minimize the chi^2 in the bins
+        inside the constrained window specified by window_min/max.
+        If True, the function will minimize the chi^2 in the bins outside 
+        window
+        
+    constraint_mask : NoneType, boolean ndarray, optional
+        An additional constraint on the chi^2 to apply, which should be
+        in the form of a boolean mask. If left as None, no additional
+        constraint is applied.
+    
+    Returns
+    -------
+    bestind : int, ndarray, float
+        The index of the minimum of `chi2` given the constraints
+        specified by `nconstrain` and `lgcoutsidewindow`. If the
+        dimension of `chi2` is greater than 1, then this will be an
+        ndarray of ints.
+    
+    """
+
+    # intitialize
+    bestind = np.nan
+    
+    # number samples
+    nbins = len(chisq)
+
+    # case constraints
+    if (window_min is not None
+        or window_max is not None):
+        
+        # check window min
+        if  window_min is None or window_min<0:
+            window_min = 0
+                    
+        # check window max
+        if  window_max is None or window_max>nbins:
+            window_max = nbins
+          
+
+        if window_min>window_max:
+            raise ValueError('ERROR: OF window min bin bigger than window max bin!')
+
+
+        inds=[]
+        if lgc_outside_window:
+            inds = np.concatenate(
+                (np.arange(0, window_min),
+                 np.arange(window_max, nbins))
+            )
+        else:
+            inds = np.arange(window_min, window_max)
+
+        if len(inds)==0:
+            raise ValueError('ERROR: OF window is empty. Check arguments')
+        
+        inds = inds[(inds>=0) & (inds<nbins)]
+            
+        if constraint_mask is not None:
+            inds = inds[constraint_mask[inds]]
+            
+        if len(inds)!=0:
+            bestind = np.argmin(chisq[..., inds], axis=-1)
+            bestind = inds[bestind]
+
+    else:
+
+        if constraint_mask is None:
+            bestind = np.argmin(chisq, axis=-1)
+        else:
+            inds = np.flatnonzero(constraint_mask)
+            if len(inds)!=0:
+                bestind = np.argmin(chisq[..., constraint_mask],
+                                    axis=-1)
+                bestind = inds[bestind]
+               
 
-    return muon_cut
+    return bestind
```

### Comparing `QETpy-1.6.2/qetpy/plotting/_fitting_plotting.py` & `QETpy-1.6.3/qetpy/plotting/_fitting_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/plotting/_ibis_plotting.py` & `QETpy-1.6.3/qetpy/plotting/_ibis_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/plotting/_iv_plotting.py` & `QETpy-1.6.3/qetpy/plotting/_iv_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/plotting/_noise_plotting.py` & `QETpy-1.6.3/qetpy/plotting/_noise_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/plotting/_of_nsmb_plotting.py` & `QETpy-1.6.3/qetpy/plotting/_of_nsmb_plotting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/qetpy/sim/_sim.py` & `QETpy-1.6.3/qetpy/sim/_sim.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/setup.py` & `QETpy-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,9 +68,10 @@
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'iminuit>=2',
         'sympy',
         'astropy',
+        'pandas',
     ],
 )
```

### Comparing `QETpy-1.6.2/test/test_cut.py` & `QETpy-1.6.3/test/test_cut.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,25 +64,25 @@
 
 def test_iterstat():
     """Testing function for `qetpy.cut.iterstat`."""
 
     nsig = 3
     x = stats.norm.rvs(size=100, random_state=1)
     x[0] += 100
-    res = qp.cut.iterstat(x, cut=nsig)
+    res = qp.cut.iterstat(x, sigma=nsig)
 
     expected_mask = np.ones(len(x), dtype=bool)
     expected_mask[0] = False
     expected_mu0 = x[expected_mask].mean()
     expected_std0 = x[expected_mask].std()
     expected_res = (expected_mu0, expected_std0, expected_mask)
 
     assert np.all([np.all(expected_res[ii] == res[ii]) for ii in range(3)])
 
-    res_unb = qp.cut.iterstat(x, cut=nsig, return_unbiased_estimates=True)
+    res_unb = qp.cut.iterstat(x, sigma=nsig, return_unbiased_estimates=True)
     unb = _UnbiasedEstimators(x, expected_mu0 - nsig * expected_std0, expected_mu0 + nsig * expected_std0)
     expected_res_unb = (unb.mu, unb.std, expected_mask)
 
     assert np.all([np.all(expected_res_unb[ii] == res_unb[ii]) for ii in range(3)])
 
     expected_res_warn = (0, 0, np.array([True]))
     res_warn = qp.cut.iterstat(np.array([0]))
```

### Comparing `QETpy-1.6.2/test/test_detcal.py` & `QETpy-1.6.3/test/test_detcal.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/test/test_didv.py` & `QETpy-1.6.3/test/test_didv.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/test/test_fitting.py` & `QETpy-1.6.3/test/test_fitting.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/test/test_ibis.py` & `QETpy-1.6.3/test/test_ibis.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/test/test_ofnsmb.py` & `QETpy-1.6.3/test/test_ofnsmb.py`

 * *Files identical despite different names*

### Comparing `QETpy-1.6.2/test/test_utils.py` & `QETpy-1.6.3/test/test_utils.py`

 * *Files identical despite different names*

