# Comparing `tmp/frat_brain-1.5.0.tar.gz` & `tmp/frat_brain-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frat_brain-1.5.0.tar", max compression
+gzip compressed data, was "frat_brain-1.5.1.tar", max compression
```

## Comparing `frat_brain-1.5.0.tar` & `frat_brain-1.5.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.5.0/LICENSE
--rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.5.0/README.md
--rw-r--r--   0        0        0     8196 2023-05-04 14:03:22.213584 frat_brain-1.5.0/fRAT/.DS_Store
--rw-r--r--   0        0        0      228 2023-05-10 16:07:10.854878 frat_brain-1.5.0/fRAT/HOUSE/__init__.py
--rw-r--r--   0        0        0      539 2023-05-05 16:06:02.329184 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6154 2023-05-10 13:02:37.995811 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc
--rw-r--r--   0        0        0     1732 2023-05-09 12:00:42.782332 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc
--rw-r--r--   0        0        0     3402 2023-05-10 13:15:37.908106 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc
--rw-r--r--   0        0        0     2339 2023-05-10 14:23:49.376966 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc
--rw-r--r--   0        0        0     6580 2023-05-10 16:07:10.855691 frat_brain-1.5.0/fRAT/HOUSE/add_motion.py
--rw-r--r--   0        0        0     1836 2023-05-10 16:07:10.856488 frat_brain-1.5.0/fRAT/HOUSE/add_noise.py
--rw-r--r--   0        0        0     4510 2023-05-10 16:07:10.857305 frat_brain-1.5.0/fRAT/HOUSE/handler.py
--rw-r--r--   0        0        0     2047 2023-05-10 16:07:10.858140 frat_brain-1.5.0/fRAT/HOUSE/separate_noise_volumes.py
--rw-r--r--   0        0        0    53981 2023-05-10 16:07:10.859431 frat_brain-1.5.0/fRAT/__main__.py
--rw-r--r--   0        0        0       22 2023-05-10 16:14:39.878750 frat_brain-1.5.0/fRAT/_version.py
--rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.5.0/fRAT/configuration_profiles/latest_settings.toml
--rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.860695 frat_brain-1.5.0/fRAT/configuration_profiles/maps/default_config.toml
--rw-r--r--   0        0        0     4338 2023-05-10 16:07:10.861735 frat_brain-1.5.0/fRAT/configuration_profiles/maps/statmap_config.toml
--rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.862965 frat_brain-1.5.0/fRAT/configuration_profiles/maps/test_config.toml
--rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.864159 frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/default_config.toml
--rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.865669 frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
--rw-r--r--   0        0        0    17405 2023-05-10 16:07:10.866968 frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/test_config.toml
--rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.5.0/fRAT/images/fRAT.gif
--rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.5.0/fRAT/nogui.py
--rw-r--r--   0        0        0     6148 2023-05-04 14:03:22.211954 frat_brain-1.5.0/fRAT/utils/.DS_Store
--rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.5.0/fRAT/utils/__init__.py
--rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.5.0/fRAT/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.5.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.5.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.5.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
--rw-r--r--   0        0        0    17651 2023-05-10 14:13:55.023764 frat_brain-1.5.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.5.0/fRAT/utils/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.5.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc
--rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.5.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc
--rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.5.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0        0        0     9295 2023-05-10 15:56:17.112312 frat_brain-1.5.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-05-09 15:27:08.538396 frat_brain-1.5.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    15234 2023-05-04 16:27:06.681168 frat_brain-1.5.0/fRAT/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.5.0/fRAT/utils/analysis.py
--rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.5.0/fRAT/utils/bootstrap.css
--rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.5.0/fRAT/utils/dash_report.py
--rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.5.0/fRAT/utils/directory_comparison.py
--rw-r--r--   0        0        0    34597 2023-05-10 16:07:10.868291 frat_brain-1.5.0/fRAT/utils/fRAT_config_setup.py
--rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.5.0/fRAT/utils/figures.py
--rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.5.0/fRAT/utils/html_report.py
--rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.5.0/fRAT/utils/printResults.py
--rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.5.0/fRAT/utils/script.js
--rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.5.0/fRAT/utils/statistics.py
--rw-r--r--   0        0        0    13101 2023-05-10 16:07:10.869916 frat_brain-1.5.0/fRAT/utils/statmap.py
--rw-r--r--   0        0        0     9345 2023-05-10 16:07:10.871233 frat_brain-1.5.0/fRAT/utils/statmap_config_setup.py
--rw-r--r--   0        0        0    19156 2023-05-10 16:07:10.917697 frat_brain-1.5.0/fRAT/utils/utils.py
--rw-r--r--   0        0        0     2390 2023-05-10 16:14:56.329049 frat_brain-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 frat_brain-1.5.0/setup.py
--rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3354 2023-05-16 15:38:37.400002 frat_brain-1.5.1/README.md
+-rw-r--r--   0        0        0     8196 2023-05-04 14:03:22.213584 frat_brain-1.5.1/fRAT/.DS_Store
+-rw-r--r--   0        0        0      228 2023-05-10 16:07:10.854878 frat_brain-1.5.1/fRAT/HOUSE/__init__.py
+-rw-r--r--   0        0        0      539 2023-05-17 16:08:32.624385 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6154 2023-05-10 13:02:37.995811 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc
+-rw-r--r--   0        0        0     1732 2023-05-09 12:00:42.782332 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc
+-rw-r--r--   0        0        0     3402 2023-05-17 16:08:32.709491 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc
+-rw-r--r--   0        0        0     2339 2023-05-10 14:23:49.376966 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc
+-rw-r--r--   0        0        0     6580 2023-05-10 16:07:10.855691 frat_brain-1.5.1/fRAT/HOUSE/add_motion.py
+-rw-r--r--   0        0        0     1836 2023-05-10 16:07:10.856488 frat_brain-1.5.1/fRAT/HOUSE/add_noise.py
+-rw-r--r--   0        0        0     4510 2023-05-10 16:07:10.857305 frat_brain-1.5.1/fRAT/HOUSE/handler.py
+-rw-r--r--   0        0        0     2047 2023-05-10 16:07:10.858140 frat_brain-1.5.1/fRAT/HOUSE/separate_noise_volumes.py
+-rw-r--r--   0        0        0    53981 2023-05-10 16:07:10.859431 frat_brain-1.5.1/fRAT/__main__.py
+-rw-r--r--   0        0        0      211 2023-05-17 16:36:50.786298 frat_brain-1.5.1/fRAT/_version.py
+-rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.5.1/fRAT/configuration_profiles/latest_settings.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.860695 frat_brain-1.5.1/fRAT/configuration_profiles/maps/default_config.toml
+-rw-r--r--   0        0        0     4473 2023-05-17 16:16:24.744843 frat_brain-1.5.1/fRAT/configuration_profiles/maps/statmap_config.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.862965 frat_brain-1.5.1/fRAT/configuration_profiles/maps/test_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.864159 frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/default_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-17 16:21:31.060646 frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
+-rw-r--r--   0        0        0    17405 2023-05-10 16:07:10.866968 frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/test_config.toml
+-rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.5.1/fRAT/images/fRAT.gif
+-rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.5.1/fRAT/nogui.py
+-rw-r--r--   0        0        0     6148 2023-05-04 14:03:22.211954 frat_brain-1.5.1/fRAT/utils/.DS_Store
+-rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.5.1/fRAT/utils/__init__.py
+-rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.5.1/fRAT/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.5.1/fRAT/utils/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.5.1/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.5.1/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0    17651 2023-05-17 16:08:16.861001 frat_brain-1.5.1/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.5.1/fRAT/utils/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.5.1/fRAT/utils/__pycache__/html_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.5.1/fRAT/utils/__pycache__/printResults.cpython-310.pyc
+-rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.5.1/fRAT/utils/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0        0        0     9315 2023-05-17 16:16:18.839737 frat_brain-1.5.1/fRAT/utils/__pycache__/statmap.cpython-310.pyc
+-rw-r--r--   0        0        0     5726 2023-05-17 16:08:29.826539 frat_brain-1.5.1/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    15234 2023-05-17 16:08:16.669826 frat_brain-1.5.1/fRAT/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.5.1/fRAT/utils/analysis.py
+-rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.5.1/fRAT/utils/bootstrap.css
+-rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.5.1/fRAT/utils/dash_report.py
+-rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.5.1/fRAT/utils/directory_comparison.py
+-rw-r--r--   0        0        0    34597 2023-05-10 16:07:10.868291 frat_brain-1.5.1/fRAT/utils/fRAT_config_setup.py
+-rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.5.1/fRAT/utils/figures.py
+-rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.5.1/fRAT/utils/html_report.py
+-rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.5.1/fRAT/utils/printResults.py
+-rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.5.1/fRAT/utils/script.js
+-rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.5.1/fRAT/utils/statistics.py
+-rw-r--r--   0        0        0    13137 2023-05-17 16:16:14.911516 frat_brain-1.5.1/fRAT/utils/statmap.py
+-rw-r--r--   0        0        0     9345 2023-05-10 16:07:10.871233 frat_brain-1.5.1/fRAT/utils/statmap_config_setup.py
+-rw-r--r--   0        0        0    19156 2023-05-10 16:07:10.917697 frat_brain-1.5.1/fRAT/utils/utils.py
+-rw-r--r--   0        0        0     2390 2023-05-17 17:03:36.479842 frat_brain-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6306 1970-01-01 00:00:00.000000 frat_brain-1.5.1/setup.py
+-rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 frat_brain-1.5.1/PKG-INFO
```

### Comparing `frat_brain-1.5.0/LICENSE` & `frat_brain-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/README.md` & `frat_brain-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 [Home page](https://fmri-roi-analysis-tool.readthedocs.io)
 
 [Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)
 
 [ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)
 
+## Citation
+
+**When using fRAT, please include the following citation:**
+
+Howley, E., Francis, S., & Schluppeck, D. (2023). fRAT: an interactive, Python-based tool for region-of-interest summaries of functional imaging data. Journal of Open Source Software, 8(85), 5200. https://doi.org/10.21105/joss.05200
+
 ## Reporting bugs
 
 To report a bug or suggest a new feature, please go to [fRAT's Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).
 
 For other questions, issues or discussion please go to [fRAT's Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).
 
 ## Contributing to the project
```

### Comparing `frat_brain-1.5.0/fRAT/.DS_Store` & `frat_brain-1.5.1/fRAT/.DS_Store`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May  5 16:05:56 2023 UTC, .py size: 228 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6429 5564 e400 0000  o.......d)Ud....
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 e400 0000  o.........[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 5a05 6505  m.Z...d.d.l.Z.e.
 00000050: a005 6504 6501 6506 8301 6403 8302 a101  ..e.e.e...d.....
 00000060: 5a07 6404 6405 8400 6507 4400 8301 5a08  Z.d.d...e.D...Z.
 00000070: 6402 5300 2906 e900 0000 0029 04da 0764  d.S.)......)...d
```

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 13:15:34 2023 UTC, .py size: 4510 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f698 5b64 9e11 0000  o.........[d....
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 9e11 0000  o.........[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6404 6c05 6d06 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6107 6401 6108 6405 6406 8400 5a09 6407  a.d.a.d.d...Z.d.
 00000070: 6408 8400 5a0a 6409 640a 8400 5a0b 640b  d...Z.d.d...Z.d.
```

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/add_motion.py` & `frat_brain-1.5.1/fRAT/HOUSE/add_motion.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/add_noise.py` & `frat_brain-1.5.1/fRAT/HOUSE/add_noise.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/handler.py` & `frat_brain-1.5.1/fRAT/HOUSE/handler.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/HOUSE/separate_noise_volumes.py` & `frat_brain-1.5.1/fRAT/HOUSE/separate_noise_volumes.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/__main__.py` & `frat_brain-1.5.1/fRAT/__main__.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/configuration_profiles/maps/default_config.toml` & `frat_brain-1.5.1/fRAT/configuration_profiles/maps/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/configuration_profiles/maps/statmap_config.toml` & `frat_brain-1.5.1/fRAT/configuration_profiles/maps/statmap_config.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 output_folder_name = 'DEFAULT'                                                    # Directory to save output. If set to DEFAULT, the default name for the statistical map created will be used. Recommended: DEFAULT
 
 ## High pass filtering
 temporal_filter = true                                                            # true or false. Use a high pass filter to remove low frequency drift. Recommended: true
 highpass_filter_cutoff = 0.01                                                     # Highpass filter cutoff frequency converted into sigma in seconds using the formula 1/(2*f*TR). Recommended: 0.01
 
 ## Motion correction
-remove_motion_outliers = true                                                     # true or false. Use fsl_motion_outliers to remove motion outliers(uses default fsl_motion_outliers settings). Recommended: true
+remove_motion_outliers = false                                                    # true or false. Use fsl_motion_outliers to remove motion outliers(uses default fsl_motion_outliers settings). Recommended: true
 motion_correction = true                                                          # true or false. Use MCFLIRT to motion correct volumes (uses default MCFLIRT settings). Recommended: true
 
 ## Spatial smoothing
 spatial_smoothing = false                                                         # true or false. Uses SUSAN to spatial smooth. Recommended: true
 smoothing_fwhm = 8.0                                                              # fwhm of smoothing, in mm, gets converted using sqrt(8*log(2)). Recommended: 8.0
 smoothing_brightness_threshold = 2000.0                                           # Should be greater than noise level and less than contrast of edges to be preserved. Recommended: 2000.0
 
 ## Image SNR calculation
 magnitude_correction = true                                                       # true or false. Correction factor of 0.7 applied when running iSNR calculations, to correct for Rayleigh distributed noise when using magnitude vs complex images.  Reference: Constantinides, C. D., Atalar, E., & McVeigh, E. R. (1997). Signal-to-Noise Measurements in Magnitude Images from NMR Phased Arrays.
-noise_volume = true                                                               # true or false. Select true if a noise volume has been collected as part of the fMRI time series. NOTE: If true, the noise volume in the time series will be separated from the functional volumes and will be placed into the folder "func_noiseVolumeRemoved". If "noise volume" is true and "noise value" is not none, the noise volume will be used in image SNR calculation rather than the user defined noise value.
+noise_volume = true                                                               # true or false. Select true if a noise volume has been collected as part of the fMRI time series. If true, the noise volume in the time series will be separated from the functional volumes and will be placed into the folder "noise_volume", and the functional volumes will be placed into the "func_volumes" folder. If "noise volume" is true and "noise value" is not none, the noise volume will be used in image SNR calculation rather than the user defined noise value. NOTE: Use the "separate noise volume" utility before creating image SNR maps.
 iSNR_std_use_only_nonzero_voxels = true                                           # true or false.
 
 ## Add Gaussian noise
 noise_multipliers = [1, 2, 5]                                                     # Provide a comma-separated list of multipliers, e.g. '1, 5'. A separate file will be produced for each multiplier. NOTE: Added has a gaussian distribution, with a mean of 0 and a standard deviation of the noise level of each participant * multiplier.
 motion_multipliers = [1, 2, 5]                                                    # Provide a comma-separated list of multipliers, e.g. '1, 5'. A separate file will be produced for each multiplier. NOTE: Added motion has a gaussian distribution, with a mean of 0 and a standard deviation of the average rotation/translation of each participant * multiplier.
```

### Comparing `frat_brain-1.5.0/fRAT/configuration_profiles/maps/test_config.toml` & `frat_brain-1.5.1/fRAT/configuration_profiles/maps/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/default_config.toml` & `frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml` & `frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/test_config.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,114 +9,114 @@
 brain_file_loc = ''                                                               # Either the absolute location of brain files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 report_output_folder = ''                                                         # Either the absolute location of json files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 averaging_type = 'Participant averaged'                                           # Participant averaged or Session averaged. This setting is used to determine which statistics to use for plotting, and when accessing results (for example through the interactive report).  Note: Histograms will always use the raw results. The linear mixed model from the statistics will always use session averaged data Options: ['Session averaged', 'Participant averaged'].
 parameter_file = 'paramValues.csv'                                                # Recommended: paramValues.csv Name of the file to parse for critical params. Option added to allow quick swapping between different parameter files.
 file_cleanup = 'move'                                                             # Move or delete intermediate files. Options: ['move', 'delete'].
 
 ## Installation testing
-delete_test_folder = 'If completed without error'                                 # Option to choose whether the folder generated while running tests is deleted upon completion. This only applies when running the full comparison. Options: ['Always', 'If completed without error', 'Never'].
-verbose_errors = true                                                             # true or false. Print all missing files and differences found during testing to the terminal.
+delete_test_folder = 'Always'                                                     # Option to choose whether the folder generated while running tests is deleted upon completion. Options: ['Always', 'If completed without error', 'Never'].
+verbose_errors = false                                                            # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
 input_folder_name = 'func_preprocessed'                                                # Folder found in each subjects directory containing the files to be analysed. func_preprocessed is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
 output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
-run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found". These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
+run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found".  These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
 stat_map_suffix = '_tSNR.nii.gz'                                                  # File name suffix of the statistical map files. Include the file extension. Example: _tSNR.img
 conf_level_number = '95%, 1.96'                                                   # Set the confidence level for confidence interval calculations. Numbers represent the confidence level and the corresponding critical z value. Recommended: 95%, 1.96. Options: ['80%, 1.28', '85%, 1.44', '90%, 1.64', '95%, 1.96', '98%, 2.33', '99%, 2.58'].
 binary_params = ['']                                                              # Add parameters here which will either be on or off.
 
 ## Outlier detection
-noise_cutoff = true                                                               # true or false. Calculate a minimum cutoff value to be included in an ROI,based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff.  Useful for statistical maps where extracranial voxels are likely to have much lower values than those inside the brain such as tSNR maps. Recommended: true.
+noise_cutoff = true                                                               # true or false. Calculate a noise cutoff based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff, Recommended: true.
 gaussian_outlier_detection = true                                                 # true or false. Fit a gaussian to the data to determine outliers using Elliptic Envelope. Recommended: true.
 gaussian_outlier_contamination = 0.1                                              # Percent of expected outliers in dataset Recommended: 0.1
 gaussian_outlier_location = 'below gaussian'                                      # Data to remove (if gaussian outlier detection is true). For example: if set to below gaussian, data below the gaussian will be removed. Recommended: below gaussian. Options: ['below gaussian', 'above gaussian', 'both'].
 
 # Statistics
 automatically_create_statistics_options_file = true                               # true or false. Usually statisticsOptions.csv is automatically created when creating paramValues.csv. Deselect this option if you won't be running the statistics step. The create statisticsOptions.csv button above can also be used to manually create this file.
 statistics_subfolder_name = 'stats'                                               # Directory name for statistics folder.
 print_result = true                                                               # true or false. Prints results to terminal if true in addition to saving results to file.
 minimum_voxels = 400                                                              # For bootstrapped change versus baseline, for each ROI, the average number of voxels per session for an ROI must be above this value to be included in the analysis.For running the linear mixed model, for each ROI, any sessions with a voxel count below this value will be removed. Highly recommended to set a value here, as ROIs with a small number of voxels may suggest poor fitting. Recommended value 400
 bootstrap_samples = 1000                                                          # Recommended value 1000.  Note: Bootstrapping is only used to calculate percentage change versus baseline.
 bootstrap_confidence_interval = 95                                                # Recommended value: 95  Note: Bootstrapping is only used to calculate percentage change versus baseline.
-regional_stats_rois = ['all']                                                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
-include_as_variable = ['INCLUDE ALL VARIABLES']                                   # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take into account when balancing data for the main effect t test data.
-brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map. 
+regional_stats_rois = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+include_as_variable = ['Multiband', 'SENSE']                                      # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take to average across when running main effect t-tests.
+brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map.
 
 ## T-tests
-run_t_tests = true                                                                # true or false. 
-IV_type = ['FILL IV TYPE AS BETWEEN-SUBJECTS']                                    # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
+run_t_tests = true                                                                # true or false.
+IV_type = ['Within-subjects', 'Within-subjects']                                  # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
 
 ## Linear mixed models
-run_linear_mixed_models = true                                                    # true or false. 
+run_linear_mixed_models = true                                                    # true or false.
 categorical_variables = ['']                                                      # Select which variables (if any) are categorical. Used for the LMM.
 main_effects = true                                                               # true or false. Note: This option is independent from the other effect calculations.
-main_and_interaction_effects = true                                               # true or false. Note: This option is independent from the other effect calculations.
+main_and_interaction_effects = false                                              # true or false. Note: This option is independent from the other effect calculations.
 interaction_effects = false                                                       # true or false. Note: This option is independent from the other effect calculations.
 
 ## R2 vs voxel count LMM
 max_below_thresh = 0                                                              # Recommended value 0.  For a given ROI, this value sets the maximum percent of sessions that can be excluded (due to having insufficient voxel count) before the ROI is not included in r2 vs voxel count statistics. With the default value of 100(%) an ROI will not be included in this calculation if any sessions have been excluded.
 
 # Parsing
-parameter_dict1 = ['MB', 'SENSE']                                                 # Comma-separated list of independent variables. The critical parameter settings are used to supply the names and file name abbreviations of the independent variables, therefore `fRAT` supports the use of any parameters (and any number of them). As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: Leave blank if you do not want to compare between different conditions, for example, if you wish to see the overall tSNR for each region across the entire dataset.
+parameter_dict1 = ['Multiband', 'SENSE']                                          # Comma-separated list of independent variables.   As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: This field can also be blank.
 parameter_dict2 = ['mb', 's']                                                     # Comma-separated list of terms to parse the file name for. Each entry corresponds to a critical parameter above.  Optional if using table parameter verification, however if the file name contains this information it can use this information to auto-detect the critical parameters used for each fMRI volume. Note: This field can be blank.
-make_folder_structure = true                                                      # true or false. Make folder structure when creating paramValues.csv
+make_folder_structure = false                                                     # true or false. Make folder structure when creating paramValues.csv
 parsing_folder = 'func'                                                           # Folder to find files to add to paramValues.csv. If using "Make folder structure" option, this will be the directory the files in the participant folder will be moved to.
 
 # Plotting
 
 ## General plot settings
-plot_dpi = 600                                                                    # Recommended value 600
+plot_dpi = 200                                                                    # Recommended value 600
 plot_font_size = 40                                                               # Recommended value 30
 plot_scale = 10                                                                   # Recommended value 10
 make_violin_plot = true                                                           # true or false.
 make_brain_table = true                                                           # true or false.
 make_one_region_fig = true                                                        # true or false.
 make_histogram = true                                                             # true or false.
 colorblind_friendly_plot_colours = ['#ffeda0', '#feb24c', '#fc4e2a', '#bd0026']   # Hex values of colourblind friendly colour scale.
-regional_fig_rois = ['all']                                                       # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+regional_fig_rois = [18, 20]                                                      # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
 
 ## Brain table
 brain_tight_layout = false                                                        # true or false. Use a tight layout when laying out the figure. Recommended: false
 brain_fig_value_min = 0                                                           # Provides the minimum value of the colourbar when creating mean and median images. For example, set minimum to 50 to make areas with values below 50 appear black. Recommended value: 0
 brain_fig_value_max = 'None'                                                      # Provides the maximum value of the colourbar when creating mean and median images. For example, set maximum to 50 to make areas with values above 50 appear as the brighest colour on the colourbar. Recommended value: None. Note: will default to 100 for scaled maps.
 brain_x_coord = -1                                                                # Voxel location to slice the images at in the x axis. Recommended settings for both variables: 91 or 58
 brain_z_coord = 19                                                                # Voxel location to slice the images at in the z axis. Recommended settings for both variables: 91 or 58
-brain_table_col_labels = 'CHANGE TO DESIRED LABEL'                                # Label for columns.
-brain_table_row_labels = 'CHANGE TO DESIRED LABEL'                                # Label for rows.
-brain_table_cols = 'DEFAULT'                                                      # 
-brain_table_rows = 'DEFAULT'                                                      # 
+brain_table_col_labels = 'MB'                                                     # Label for columns.
+brain_table_row_labels = 'SENSE'                                                  # Label for rows.
+brain_table_cols = 'Multiband'                                                    #
+brain_table_rows = 'SENSE'                                                        #
 
 ## Violin plot
-table_x_label = 'tSNR mean'                                                       # 
-table_y_label = 'ROI'                                                             # 
+table_x_label = 'tSNR mean'                                                       #
+table_y_label = 'ROI'                                                             #
 violin_show_data = true                                                           # true or false.
 violin_jitter = true                                                              # true or false.
 violin_colour = '#fc4e2a'                                                         # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
 boxplot_colour = '#feb24c'                                                        # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
-table_cols = 'DEFAULT'                                                            # 
-table_rows = 'DEFAULT'                                                            # 
+table_cols = 'Multiband'                                                          #
+table_rows = 'SENSE'                                                              #
 
 ## Regional bar chart
-single_roi_fig_label_x = 'Multiband factor'                                       # 
-single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         # 
-single_roi_fig_label_fill = 'SENSE factor'                                        # 
-single_roi_fig_x_axis = 'DEFAULT'                                                 # 
-single_roi_fig_colour = 'DEFAULT'                                                 # 
+single_roi_fig_label_x = 'Multiband factor'                                       #
+single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         #
+single_roi_fig_label_fill = 'SENSE factor'                                        #
+single_roi_fig_x_axis = 'Multiband'                                               #
+single_roi_fig_colour = 'SENSE'                                                   #
 
 ## Regional histogram
-histogram_binwidth = 2                                                            # 
-histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          # 
-histogram_fig_label_y = 'Frequency'                                               # 
-histogram_stat_line_size = 1.5                                                    # 
+histogram_binwidth = 2                                                            #
+histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          #
+histogram_fig_label_y = 'Frequency'                                               #
+histogram_stat_line_size = 1.5                                                    #
 histogram_show_mean = true                                                        # true or false.
 histogram_show_median = true                                                      # true or false.
 histogram_show_legend = true                                                      # true or false.
-histogram_fig_x_facet = 'DEFAULT'                                                 # 
-histogram_fig_y_facet = 'DEFAULT'                                                 # 
+histogram_fig_x_facet = 'Multiband'                                               #
+histogram_fig_y_facet = 'SENSE'                                                   #
 histogram_fig_colour = '#fc4e2a'                                                  # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
```

### Comparing `frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/test_config.toml` & `frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,122 +1,122 @@
 # General
 run_analysis = true                                                               # true or false. Can skip this step if json files have already been created.
-run_statistics = true                                                             # true or false.
-run_plotting = true                                                               # true or false.
+run_statistics = false                                                            # true or false.
+run_plotting = false                                                              # true or false.
 verbose = true                                                                    # true or false.
 verbose_cmd_line_args = false                                                     # true or false.
 multicore_processing = true                                                       # true or false. Use multicore processing during analysis? Multicore processing currently works within participants not between them. Recommended: true
 max_core_usage = 'max'                                                            # 'max' to select number of cores available on the system, alternatively an int to manually select number of cores to use. Recommended: 'max' Options: ['max', 6, 5, 4, 3, 2, 1].
 brain_file_loc = ''                                                               # Either the absolute location of brain files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 report_output_folder = ''                                                         # Either the absolute location of json files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 averaging_type = 'Participant averaged'                                           # Participant averaged or Session averaged. This setting is used to determine which statistics to use for plotting, and when accessing results (for example through the interactive report).  Note: Histograms will always use the raw results. The linear mixed model from the statistics will always use session averaged data Options: ['Session averaged', 'Participant averaged'].
 parameter_file = 'paramValues.csv'                                                # Recommended: paramValues.csv Name of the file to parse for critical params. Option added to allow quick swapping between different parameter files.
 file_cleanup = 'move'                                                             # Move or delete intermediate files. Options: ['move', 'delete'].
 
 ## Installation testing
-delete_test_folder = 'Always'                                                     # Option to choose whether the folder generated while running tests is deleted upon completion. Options: ['Always', 'If completed without error', 'Never'].
-verbose_errors = false                                                            # true or false. Print all missing files and differences found during testing to the terminal.
+delete_test_folder = 'If completed without error'                                 # Option to choose whether the folder generated while running tests is deleted upon completion. This only applies when running the full comparison. Options: ['Always', 'If completed without error', 'Never'].
+verbose_errors = true                                                             # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
-input_folder_name = 'func_preprocessed'                                                # Folder found in each subjects directory containing the files to be analysed. func_preprocessed is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
+input_folder_name = 'func_preprocessed'                                           # Folder found in each subjects directory containing the files to be analysed. func_preprocessed is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain preprocessed versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
 output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
-run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found".  These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
+run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found". These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
-stat_map_suffix = '_tSNR.nii.gz'                                                  # File name suffix of the statistical map files. Include the file extension. Example: _tSNR.img
+stat_map_suffix = '_tStd.nii.gz'                                                  # File name suffix of the statistical map files. Include the file extension. Example: _tSNR.img
 conf_level_number = '95%, 1.96'                                                   # Set the confidence level for confidence interval calculations. Numbers represent the confidence level and the corresponding critical z value. Recommended: 95%, 1.96. Options: ['80%, 1.28', '85%, 1.44', '90%, 1.64', '95%, 1.96', '98%, 2.33', '99%, 2.58'].
 binary_params = ['']                                                              # Add parameters here which will either be on or off.
 
 ## Outlier detection
-noise_cutoff = true                                                               # true or false. Calculate a noise cutoff based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff, Recommended: true.
-gaussian_outlier_detection = true                                                 # true or false. Fit a gaussian to the data to determine outliers using Elliptic Envelope. Recommended: true.
+noise_cutoff = false                                                              # true or false. Calculate a minimum cutoff value to be included in an ROI,based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff.  Useful for statistical maps where extracranial voxels are likely to have much lower values than those inside the brain such as tSNR maps. Recommended: true.
+gaussian_outlier_detection = false                                                # true or false. Fit a gaussian to the data to determine outliers using Elliptic Envelope. Recommended: true.
 gaussian_outlier_contamination = 0.1                                              # Percent of expected outliers in dataset Recommended: 0.1
 gaussian_outlier_location = 'below gaussian'                                      # Data to remove (if gaussian outlier detection is true). For example: if set to below gaussian, data below the gaussian will be removed. Recommended: below gaussian. Options: ['below gaussian', 'above gaussian', 'both'].
 
 # Statistics
 automatically_create_statistics_options_file = true                               # true or false. Usually statisticsOptions.csv is automatically created when creating paramValues.csv. Deselect this option if you won't be running the statistics step. The create statisticsOptions.csv button above can also be used to manually create this file.
 statistics_subfolder_name = 'stats'                                               # Directory name for statistics folder.
 print_result = true                                                               # true or false. Prints results to terminal if true in addition to saving results to file.
 minimum_voxels = 400                                                              # For bootstrapped change versus baseline, for each ROI, the average number of voxels per session for an ROI must be above this value to be included in the analysis.For running the linear mixed model, for each ROI, any sessions with a voxel count below this value will be removed. Highly recommended to set a value here, as ROIs with a small number of voxels may suggest poor fitting. Recommended value 400
 bootstrap_samples = 1000                                                          # Recommended value 1000.  Note: Bootstrapping is only used to calculate percentage change versus baseline.
 bootstrap_confidence_interval = 95                                                # Recommended value: 95  Note: Bootstrapping is only used to calculate percentage change versus baseline.
-regional_stats_rois = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
-include_as_variable = ['Multiband', 'SENSE']                                      # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take to average across when running main effect t-tests.
-brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map.
+regional_stats_rois = ['all']                                                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+include_as_variable = ['']                                                        # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take into account when balancing data for the main effect t test data.
+brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map. 
 
 ## T-tests
-run_t_tests = true                                                                # true or false.
-IV_type = ['Within-subjects', 'Within-subjects']                                  # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
+run_t_tests = true                                                                # true or false. 
+IV_type = ['Between-subjects']                                                    # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
 
 ## Linear mixed models
-run_linear_mixed_models = true                                                    # true or false.
+run_linear_mixed_models = true                                                    # true or false. 
 categorical_variables = ['']                                                      # Select which variables (if any) are categorical. Used for the LMM.
 main_effects = true                                                               # true or false. Note: This option is independent from the other effect calculations.
-main_and_interaction_effects = false                                              # true or false. Note: This option is independent from the other effect calculations.
+main_and_interaction_effects = true                                               # true or false. Note: This option is independent from the other effect calculations.
 interaction_effects = false                                                       # true or false. Note: This option is independent from the other effect calculations.
 
 ## R2 vs voxel count LMM
 max_below_thresh = 0                                                              # Recommended value 0.  For a given ROI, this value sets the maximum percent of sessions that can be excluded (due to having insufficient voxel count) before the ROI is not included in r2 vs voxel count statistics. With the default value of 100(%) an ROI will not be included in this calculation if any sessions have been excluded.
 
 # Parsing
-parameter_dict1 = ['Multiband', 'SENSE']                                          # Comma-separated list of independent variables.   As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: This field can also be blank.
-parameter_dict2 = ['mb', 's']                                                     # Comma-separated list of terms to parse the file name for. Each entry corresponds to a critical parameter above.  Optional if using table parameter verification, however if the file name contains this information it can use this information to auto-detect the critical parameters used for each fMRI volume. Note: This field can be blank.
+parameter_dict1 = ['']                                                            # Comma-separated list of independent variables. The critical parameter settings are used to supply the names and file name abbreviations of the independent variables, therefore `fRAT` supports the use of any parameters (and any number of them). As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: Leave blank if you do not want to compare between different conditions, for example, if you wish to see the overall tSNR for each region across the entire dataset.
+parameter_dict2 = ['']                                                            # Comma-separated list of terms to parse the file name for. Each entry corresponds to a critical parameter above.  Optional if using table parameter verification, however if the file name contains this information it can use this information to auto-detect the critical parameters used for each fMRI volume. Note: This field can be blank.
 make_folder_structure = false                                                     # true or false. Make folder structure when creating paramValues.csv
 parsing_folder = 'func'                                                           # Folder to find files to add to paramValues.csv. If using "Make folder structure" option, this will be the directory the files in the participant folder will be moved to.
 
 # Plotting
 
 ## General plot settings
-plot_dpi = 200                                                                    # Recommended value 600
+plot_dpi = 600                                                                    # Recommended value 600
 plot_font_size = 40                                                               # Recommended value 30
 plot_scale = 10                                                                   # Recommended value 10
 make_violin_plot = true                                                           # true or false.
 make_brain_table = true                                                           # true or false.
 make_one_region_fig = true                                                        # true or false.
 make_histogram = true                                                             # true or false.
 colorblind_friendly_plot_colours = ['#ffeda0', '#feb24c', '#fc4e2a', '#bd0026']   # Hex values of colourblind friendly colour scale.
-regional_fig_rois = [18, 20]                                                      # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+regional_fig_rois = ['all']                                                       # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
 
 ## Brain table
 brain_tight_layout = false                                                        # true or false. Use a tight layout when laying out the figure. Recommended: false
 brain_fig_value_min = 0                                                           # Provides the minimum value of the colourbar when creating mean and median images. For example, set minimum to 50 to make areas with values below 50 appear black. Recommended value: 0
 brain_fig_value_max = 'None'                                                      # Provides the maximum value of the colourbar when creating mean and median images. For example, set maximum to 50 to make areas with values above 50 appear as the brighest colour on the colourbar. Recommended value: None. Note: will default to 100 for scaled maps.
 brain_x_coord = -1                                                                # Voxel location to slice the images at in the x axis. Recommended settings for both variables: 91 or 58
 brain_z_coord = 19                                                                # Voxel location to slice the images at in the z axis. Recommended settings for both variables: 91 or 58
-brain_table_col_labels = 'MB'                                                     # Label for columns.
-brain_table_row_labels = 'SENSE'                                                  # Label for rows.
-brain_table_cols = 'Multiband'                                                    #
-brain_table_rows = 'SENSE'                                                        #
+brain_table_col_labels = ''                                                       # Label for columns.
+brain_table_row_labels = ''                                                       # Label for rows.
+brain_table_cols = ''                                                             # 
+brain_table_rows = ''                                                             # 
 
 ## Violin plot
-table_x_label = 'tSNR mean'                                                       #
-table_y_label = 'ROI'                                                             #
+table_x_label = 'tSNR mean'                                                       # 
+table_y_label = 'ROI'                                                             # 
 violin_show_data = true                                                           # true or false.
 violin_jitter = true                                                              # true or false.
 violin_colour = '#fc4e2a'                                                         # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
 boxplot_colour = '#feb24c'                                                        # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
-table_cols = 'Multiband'                                                          #
-table_rows = 'SENSE'                                                              #
+table_cols = ''                                                                   # 
+table_rows = ''                                                                   # 
 
 ## Regional bar chart
-single_roi_fig_label_x = 'Multiband factor'                                       #
-single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         #
-single_roi_fig_label_fill = 'SENSE factor'                                        #
-single_roi_fig_x_axis = 'Multiband'                                               #
-single_roi_fig_colour = 'SENSE'                                                   #
+single_roi_fig_label_x = 'Multiband factor'                                       # 
+single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         # 
+single_roi_fig_label_fill = 'SENSE factor'                                        # 
+single_roi_fig_x_axis = ''                                                        # 
+single_roi_fig_colour = ''                                                        # 
 
 ## Regional histogram
-histogram_binwidth = 2                                                            #
-histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          #
-histogram_fig_label_y = 'Frequency'                                               #
-histogram_stat_line_size = 1.5                                                    #
+histogram_binwidth = 2                                                            # 
+histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          # 
+histogram_fig_label_y = 'Frequency'                                               # 
+histogram_stat_line_size = 1.5                                                    # 
 histogram_show_mean = true                                                        # true or false.
 histogram_show_median = true                                                      # true or false.
 histogram_show_legend = true                                                      # true or false.
-histogram_fig_x_facet = 'Multiband'                                               #
-histogram_fig_y_facet = 'SENSE'                                                   #
+histogram_fig_x_facet = ''                                                        # 
+histogram_fig_y_facet = ''                                                        # 
 histogram_fig_colour = '#fc4e2a'                                                  # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
```

### Comparing `frat_brain-1.5.0/fRAT/images/fRAT.gif` & `frat_brain-1.5.1/fRAT/images/fRAT.gif`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/nogui.py` & `frat_brain-1.5.1/fRAT/nogui.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/.DS_Store` & `frat_brain-1.5.1/fRAT/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/dash_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 14:13:52 2023 UTC, .py size: 34597 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a0a6 5b64 2587 0000  o.........[d%...
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 2587 0000  o.........[d%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0014 0000 0040 0000 0073 8e07 0000 6400  .....@...s....d.
 00000030: 5a00 6700 6401 a201 5a01 0900 6900 6402  Z.g.d...Z...i.d.
 00000040: 6403 6404 6405 6406 6407 6408 9c05 9301  d.d.d.d.d.d.....
 00000050: 6409 6403 6404 6405 640a 640b 6408 9c05  d.d.d.d.d.d.d...
 00000060: 9301 640c 6403 6404 6405 640a 640d 6408  ..d.d.d.d.d.d.d.
 00000070: 9c05 9301 640e 6403 6404 640a 640f 6410  ....d.d.d.d.d.d.
```

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/figures.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/html_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/printResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/statistics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/statmap.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 15:56:13 2023 UTC, .py size: 13101 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9dbe 5b64 2d33 0000  o.........[d-3..
+00000000: 6f0d 0d0a 0000 0000 cefd 6464 5133 0000  o.........ddQ3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6401 6c06 5a06 6403 6404 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6405 6406 6c09 5400 6401  m.Z...d.d.l.T.d.
 00000070: 610a 6407 610b 6407 610c 6408 6409 8400  a.d.a.d.a.d.d...
@@ -271,311 +271,313 @@
 000010e0: 6400 5300 6400 5300 2903 4e72 0900 0000  d.S.d.S.).Nr....
 000010f0: 720a 0000 0029 0272 6000 0000 724d 0000  r....).r`...rM..
 00001100: 0029 0672 2800 0000 724b 0000 0072 4c00  .).r(...rK...rL.
 00001110: 0000 725e 0000 0072 2a00 0000 7210 0000  ..r^...r*...r...
 00001120: 0072 0e00 0000 720e 0000 0072 1100 0000  .r....r....r....
 00001130: da0f 6372 6561 7465 5f73 7461 746d 6170  ..create_statmap
 00001140: 738c 0000 0073 0a00 0000 0801 1401 0801  s....s..........
-00001150: 1001 04ff 7274 0000 0063 0400 0000 0000  ....rt...c......
-00001160: 0000 0000 0000 0d00 0000 0900 0000 4300  ..............C.
-00001170: 0000 7364 0100 0064 007d 0467 007d 0567  ..sd...d.}.g.}.g
-00001180: 007d 0674 00a0 017c 00a1 015c 027d 077d  .}.t...|...\.}.}
-00001190: 0874 00a0 027c 0764 017c 017c 039b 0064  .t...|.d.|.|...d
-000011a0: 0274 036a 049b 0064 039d 047c 08a1 0501  .t.j...d...|....
-000011b0: 0074 036a 0572 407c 039b 0064 047c 019b  .t.j.r@|...d.|..
-000011c0: 0064 059d 047d 007c 039b 0064 067c 019b  .d...}.|...d.|..
-000011d0: 0064 079d 047d 0474 066a 07a0 087c 00a1  .d...}.t.j...|..
-000011e0: 0172 3c74 066a 07a0 087c 04a1 0173 4074  .r<t.j...|...s@t
-000011f0: 0964 0883 0182 0174 036a 0a72 5774 0a7c  .d.....t.j.rWt.|
-00001200: 007c 017c 027c 0383 045c 037d 007d 097d  .|.|.|...\.}.}.}
-00001210: 0a7c 05a0 0b7c 0aa1 0101 007c 06a0 0b7c  .|...|.....|...|
-00001220: 09a1 0101 0074 036a 0c72 7c7c 029b 0064  .....t.j.r||...d
-00001230: 027c 019b 0064 099d 047d 0b74 0d6a 0e7c  .|...d...}.t.j.|
-00001240: 007c 0b64 0a8d 02a0 0fa1 0001 007c 0b7d  .|.d.........|.}
-00001250: 0074 00a0 017c 00a1 015c 027d 077d 0874  .t...|...\.}.}.t
-00001260: 107c 077c 087c 017c 0364 0b83 057d 0074  .|.|.|.|.d...}.t
-00001270: 036a 1172 9a74 0d6a 127c 0074 036a 1374  .j.r.t.j.|.t.j.t
-00001280: 036a 147c 029b 0064 027c 019b 0064 0c9d  .j.|...d.|...d..
-00001290: 0464 0d8d 04a0 0fa1 0001 007c 029b 0064  .d.........|...d
-000012a0: 027c 019b 0064 0c9d 047d 0074 036a 1572  .|...d...}.t.j.r
-000012b0: ac74 167c 007c 027c 0183 035c 027d 007d  .t.|.|.|...\.}.}
-000012c0: 0c7c 05a0 0b7c 007c 0c67 02a1 0101 007c  .|...|.|.g.....|
-000012d0: 007c 047c 057c 0666 0453 0029 0e4e 7207  .|.|.|.f.S.).Nr.
-000012e0: 0000 0072 1300 0000 7265 0000 007a 0e2f  ...r....re...z./
-000012f0: 6675 6e63 5f76 6f6c 756d 6573 2f7a 072e  func_volumes/z..
-00001300: 6e69 692e 677a 7a0e 2f6e 6f69 7365 5f76  nii.gzz./noise_v
-00001310: 6f6c 756d 652f 7a14 5f6e 6f69 7365 5f76  olume/z._noise_v
-00001320: 6f6c 756d 652e 6e69 692e 677a 7a75 436f  olume.nii.gzzuCo
-00001330: 756c 6420 6e6f 7420 6669 6e64 2073 6570  uld not find sep
-00001340: 6172 6174 6520 6e6f 6973 6520 616e 6420  arate noise and 
-00001350: 6675 6e63 7469 6f6e 616c 2076 6f6c 756d  functional volum
-00001360: 6573 2e20 5275 6e20 7468 6520 2273 6570  es. Run the "sep
-00001370: 6172 6174 6520 6e6f 6973 6520 766f 6c75  arate noise volu
-00001380: 6d65 7322 2075 7469 6c69 7479 2074 6f20  mes" utility to 
-00001390: 6372 6561 7465 2074 6865 7365 2066 696c  create these fil
-000013a0: 6573 2e7a 185f 6d6f 7469 6f6e 5f63 6f72  es.z._motion_cor
-000013b0: 7265 6374 6564 2e6e 6969 2e67 7a72 3b00  rected.nii.gzr;.
-000013c0: 0000 7a15 4d6f 7469 6f6e 2063 6f72 7265  ..z.Motion corre
-000013d0: 6374 6564 2064 6174 617a 105f 736d 6f6f  cted dataz._smoo
-000013e0: 7468 6564 2e6e 6969 2e67 7a29 0472 3c00  thed.nii.gz).r<.
-000013f0: 0000 da04 6677 686d da14 6272 6967 6874  ....fwhm..bright
-00001400: 6e65 7373 5f74 6872 6573 686f 6c64 723d  ness_thresholdr=
-00001410: 0000 0029 1772 2000 0000 7251 0000 0072  ...).r ...rQ...r
-00001420: 6900 0000 721b 0000 0072 1c00 0000 7250  i...r....r....rP
-00001430: 0000 0072 5600 0000 7257 0000 00da 0665  ...rV...rW.....e
-00001440: 7869 7374 73da 1146 696c 654e 6f74 466f  xists..FileNotFo
-00001450: 756e 6445 7272 6f72 da16 7265 6d6f 7665  undError..remove
-00001460: 5f6d 6f74 696f 6e5f 6f75 746c 6965 7273  _motion_outliers
-00001470: da06 6578 7465 6e64 da11 6d6f 7469 6f6e  ..extend..motion
-00001480: 5f63 6f72 7265 6374 696f 6e72 0200 0000  _correctionr....
-00001490: da07 4d43 464c 4952 5472 4700 0000 726c  ..MCFLIRTrG...rl
-000014a0: 0000 00da 1173 7061 7469 616c 5f73 6d6f  .....spatial_smo
-000014b0: 6f74 6869 6e67 da05 5355 5341 4eda 0e73  othing..SUSAN..s
-000014c0: 6d6f 6f74 6869 6e67 5f66 7768 6dda 1e73  moothing_fwhm..s
-000014d0: 6d6f 6f74 6869 6e67 5f62 7269 6768 746e  moothing_brightn
-000014e0: 6573 735f 7468 7265 7368 6f6c 64da 0f74  ess_threshold..t
-000014f0: 656d 706f 7261 6c5f 6669 6c74 6572 7270  emporal_filterrp
-00001500: 0000 0029 0d72 4b00 0000 724c 0000 0072  ...).rK...rL...r
-00001510: 2a00 0000 7210 0000 0072 5e00 0000 7272  *...r....r^...rr
-00001520: 0000 00da 086f 7574 6c69 6572 7372 3700  .....outliersr7.
-00001530: 0000 7234 0000 00da 126f 7574 6c69 6572  ..r4.....outlier
-00001540: 5f74 696d 6570 6f69 6e74 735a 0d6f 7574  _timepointsZ.out
-00001550: 6c69 6572 5f66 696c 6573 da06 6f75 7470  lier_files..outp
-00001560: 7574 5a0e 7265 6475 6e64 616e 745f 6669  utZ.redundant_fi
-00001570: 6c65 720e 0000 0072 0e00 0000 7211 0000  ler....r....r...
-00001580: 00da 1570 7265 7061 7265 5f73 7461 746d  ...prepare_statm
-00001590: 6170 5f66 696c 6573 9300 0000 733c 0000  ap_files....s<..
-000015a0: 0004 0104 0204 010e 0320 0106 0210 0110  ......... ......
-000015b0: 0118 0208 0106 0314 010a 010a 0106 0210  ................
-000015c0: 0112 0204 010e 0210 0106 020e 010e 0104  ................
-000015d0: ff06 0110 0106 0210 010e 010c 0272 8500  .............r..
-000015e0: 0000 6304 0000 0000 0000 0000 0000 000f  ..c.............
-000015f0: 0000 0008 0000 0043 0000 0073 0201 0000  .......C...s....
-00001600: 7c02 9b00 6401 7c01 9b00 6402 9d04 7d04  |...d.|...d...}.
-00001610: 7c02 9b00 6401 7c01 9b00 6403 9d04 7d05  |...d.|...d...}.
-00001620: 7c02 9b00 6401 7c01 9b00 6404 9d04 7d06  |...d.|...d...}.
-00001630: 7400 6a01 7c00 7c04 7c05 7c06 6405 8d04  t.j.|.|.|.|.d...
-00001640: a002 a100 0100 7403 7c02 9b00 6401 7c01  ......t.|...d.|.
-00001650: 9b00 6402 9d04 8301 8f0c 7d07 7c07 a004  ..d.......}.|...
-00001660: a100 7d08 5700 6400 0400 0400 8303 0100  ..}.W.d.........
-00001670: 6e08 3100 733c 7701 0100 0100 0100 5900  n.1.s<w.......Y.
-00001680: 0100 6700 7d09 7405 7c08 8301 4400 5d16  ..g.}.t.|...D.].
-00001690: 5c02 7d0a 7d0b 7c0b a006 6406 6407 a102  \.}.}.|...d.d...
-000016a0: a007 6408 a101 7d0c 7c0c 6409 6b03 725d  ..d...}.|.d.k.r]
-000016b0: 7c09 a008 7c0a a101 0100 7147 7409 a00a  |...|.....qGt...
-000016c0: 7c00 a101 5c02 7d0d 7d0e 740b 6a0c 7c0d  |...\.}.}.t.j.|.
-000016d0: 7c09 640a 640b 8d03 7d0d 740d 7c0d 7c0e  |.d.d...}.t.|.|.
-000016e0: 7c01 7c03 640c 8305 7d00 7c00 7c01 740e  |.|.d...}.|.|.t.
-000016f0: 7c09 8301 6702 7c04 7c05 7c06 6703 6603  |...g.|.|.|.g.f.
-00001700: 5300 290d 4e72 1300 0000 7a0d 5f6f 7574  S.).Nr....z._out
-00001710: 6c69 6572 732e 7478 747a 0c5f 6d65 7472  liers.txtz._metr
-00001720: 6963 732e 706e 677a 0c5f 6d65 7472 6963  ics.pngz._metric
-00001730: 732e 7478 7429 0472 3c00 0000 723d 0000  s.txt).r<...r=..
-00001740: 00da 0f6f 7574 5f6d 6574 7269 635f 706c  ...out_metric_pl
-00001750: 6f74 da11 6f75 745f 6d65 7472 6963 5f76  ot..out_metric_v
-00001760: 616c 7565 7372 0b00 0000 7207 0000 00da  aluesr....r.....
-00001770: 0131 e9ff ffff ffe9 0300 0000 2901 da04  .1..........)...
-00001780: 6178 6973 7a21 5265 6d6f 7665 6420 6d6f  axisz!Removed mo
-00001790: 7469 6f6e 206f 7574 6c69 6572 2074 696d  tion outlier tim
-000017a0: 6570 6f69 6e74 7329 0f72 0200 0000 da0e  epoints).r......
-000017b0: 4d6f 7469 6f6e 4f75 746c 6965 7273 7247  MotionOutliersrG
-000017c0: 0000 0072 6600 0000 da09 7265 6164 6c69  ...rf.....readli
-000017d0: 6e65 73da 0965 6e75 6d65 7261 7465 da07  nes..enumerate..
-000017e0: 7265 706c 6163 65da 0466 696e 64da 0661  replace..find..a
-000017f0: 7070 656e 6472 2000 0000 7251 0000 00da  ppendr ...rQ....
-00001800: 026e 70da 0664 656c 6574 6572 6c00 0000  .np..deleterl...
-00001810: da03 6c65 6e29 0f72 4b00 0000 724c 0000  ..len).rK...rL..
-00001820: 0072 2a00 0000 7210 0000 005a 0c6f 7574  .r*...r....Z.out
-00001830: 6c69 6572 5f66 696c 655a 0c6f 7574 6c69  lier_fileZ.outli
-00001840: 6572 5f70 6c6f 745a 0e6f 7574 6c69 6572  er_plotZ.outlier
-00001850: 5f76 616c 7565 7372 6b00 0000 da05 6c69  _valuesrk.....li
-00001860: 6e65 7372 8300 0000 5a0a 7469 6d65 5f70  nesr....Z.time_p
-00001870: 6f69 6e74 da04 6c69 6e65 5a0d 6f75 746c  oint..lineZ.outl
-00001880: 6965 725f 6368 6563 6b72 3700 0000 7234  ier_checkr7...r4
-00001890: 0000 0072 0e00 0000 720e 0000 0072 1100  ...r....r....r..
-000018a0: 0000 7279 0000 00bf 0000 0073 2a00 0000  ..ry.......s*...
-000018b0: 1001 1001 1001 0802 0201 0201 04fe 0602  ................
-000018c0: 1602 0a01 1cff 0403 1001 1201 0801 0a01  ................
-000018d0: 0280 0e02 1001 1003 1802 7279 0000 0063  ..........ry...c
-000018e0: 0600 0000 0000 0000 0000 0000 0a00 0000  ................
-000018f0: 0700 0000 4300 0000 7378 0000 007c 0561  ....C...sx...|.a
-00001900: 0074 01a0 027c 00a1 017d 067c 019b 0064  .t...|...}.|...d
-00001910: 017c 039b 0064 017c 009b 009d 057d 007c  .|...d.|.....}.|
-00001920: 019b 0064 017c 029b 009d 037d 0274 006a  ...d.|.....}.t.j
-00001930: 0372 2274 0464 027c 069b 009d 0283 0101  .r"t.d.|........
-00001940: 0074 057c 007c 067c 027c 0183 045c 047d  .t.|.|.|.|...\.}
-00001950: 007d 077d 087d 0974 067c 047c 007c 067c  .}.}.}.t.|.|.|.|
-00001960: 077c 027c 0183 0601 0074 077c 0883 0101  .|.|.....t.|....
-00001970: 007c 0953 0029 034e 7213 0000 007a 1820  .|.S.).Nr....z. 
-00001980: 2020 2020 2020 2041 6e61 6c79 7369 6e67         Analysing
-00001990: 2066 696c 653a 2029 0872 1b00 0000 7220   file: ).r....r 
-000019a0: 0000 00da 0973 7472 6970 5f65 7874 da07  .....strip_ext..
-000019b0: 7665 7262 6f73 6572 1f00 0000 7285 0000  verboser....r...
-000019c0: 0072 7400 0000 7273 0000 0029 0a72 4b00  .rt...rs...).rK.
-000019d0: 0000 7210 0000 0072 2a00 0000 7229 0000  ..r....r*...r)..
-000019e0: 0072 2800 0000 da03 6366 6772 4c00 0000  .r(.....cfgrL...
-000019f0: 725e 0000 0072 7200 0000 7282 0000 0072  r^...rr...r....r
-00001a00: 0e00 0000 720e 0000 0072 1100 0000 da1a  ....r....r......
-00001a10: 7072 6f63 6573 735f 6669 6c65 735f 666f  process_files_fo
-00001a20: 725f 7374 6174 6d61 7073 da00 0000 7314  r_statmaps....s.
-00001a30: 0000 0004 020a 0214 010e 0106 020e 0116  ................
-00001a40: 0212 0108 0204 0272 9a00 0000 6304 0000  .......r....c...
-00001a50: 0000 0000 0000 0000 000a 0000 000a 0000  ................
-00001a60: 0043 0000 0073 a401 0000 7400 6a01 7208  .C...s....t.j.r.
-00001a70: 7402 a003 a100 7d04 6e02 6400 7d04 7400  t.....}.n.d.}.t.
-00001a80: 6a04 7218 7405 6401 7400 6a06 9b00 6402  j.r.t.d.t.j...d.
-00001a90: 7c01 9b00 9d04 8301 0100 7c00 a007 a100  |.........|.....
-00001aa0: 4400 5da7 5c02 7d05 7d06 7400 6a04 7235  D.].\.}.}.t.j.r5
-00001ab0: 7405 6403 7c05 a008 6404 a101 6405 1900  t.d.|...d...d...
-00001ac0: 9b00 6406 7409 7c06 8301 9b00 6407 9d05  ..d.t.|.....d...
-00001ad0: 8301 0100 7402 6a0a 7c05 9b00 6404 7400  ....t.j.|...d.t.
-00001ae0: 6a06 9b00 6408 9d04 6409 640a 8d02 0100  j...d...d.d.....
-00001af0: 740b 7c05 9b00 6404 7400 6a06 9b00 640b  t.|...d.t.j...d.
-00001b00: 9d04 640c 8302 8f0d 7d07 7c07 a00c 640d  ..d.....}.|...d.
-00001b10: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00001b20: 6e08 3100 735f 7701 0100 0100 0100 5900  n.1.s_w.......Y.
-00001b30: 0100 740d 7c06 740e a00f 7c05 a101 740e  ..t.|.t...|...t.
-00001b40: a00f 7c01 a101 740e a00f 7c02 a101 740e  ..|...t...|...t.
-00001b50: a00f 7c03 a101 740e a00f 7400 a101 8306  ..|...t...t.....
-00001b60: 7d08 7400 6a01 7288 7410 7c04 a011 7412  }.t.j.r.t.|...t.
-00001b70: 7c08 a102 8301 7d09 6e08 7410 740e a011  |.....}.n.t.t...
-00001b80: 7412 7c08 a102 8301 7d09 7400 6a13 72c3  t.|.....}.t.j.r.
-00001b90: 7414 6a15 640e 640f 6702 7c09 6410 8d02  t.j.d.d.g.|.d...
-00001ba0: a016 640f a101 7d09 740b 7c05 9b00 6404  ..d...}.t.|...d.
-00001bb0: 7c01 9b00 6411 9d04 640c 8302 8f11 7d07  |...d...d.....}.
-00001bc0: 7c07 a00c 7c09 6a17 6412 6413 8d01 a101  |...|.j.d.d.....
-00001bd0: 0100 5700 6400 0400 0400 8303 0100 711c  ..W.d.........q.
-00001be0: 3100 73be 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
-00001bf0: 711c 7400 6a01 72d0 7402 6a18 7c04 6412  q.t.j.r.t.j.|.d.
-00001c00: 6414 8d02 0100 6400 5300 6400 5300 2915  d.....d.S.d.S.).
-00001c10: 4e7a 160a 5365 6172 6368 696e 6720 696e  Nz..Searching in
-00001c20: 2066 6f6c 6465 723a 207a 1d0a 5361 7669   folder: z..Savi
-00001c30: 6e67 206f 7574 7075 7420 696e 2064 6972  ng output in dir
-00001c40: 6563 746f 7279 3a20 7a2c 0a43 7265 6174  ectory: z,.Creat
-00001c50: 696e 6720 7374 6174 6973 7469 6361 6c20  ing statistical 
-00001c60: 6d61 7073 2066 6f72 2070 6172 7469 6369  maps for partici
-00001c70: 7061 6e74 3a20 7213 0000 0072 8900 0000  pant: r....r....
-00001c80: 7a1d 0a20 2020 2020 2043 7265 6174 696e  z..      Creatin
-00001c90: 6720 7374 6174 6d61 7073 2066 6f72 207a  g statmaps for z
-00001ca0: 0620 6669 6c65 7372 6500 0000 5472 1600  . filesre...Tr..
-00001cb0: 0000 7263 0000 00da 0177 7207 0000 00da  ..rc.....wr.....
-00001cc0: 0446 696c 657a 104f 7574 6c69 6572 7320  .Filez.Outliers 
-00001cd0: 7265 6d6f 7665 6429 02da 0763 6f6c 756d  removed)...colum
-00001ce0: 6e73 7237 0000 007a 1f2f 6e75 6d62 6572  nsr7...z./number
-00001cf0: 5f6f 665f 6f75 746c 6965 7273 5f72 656d  _of_outliers_rem
-00001d00: 6f76 6564 2e63 7376 4629 01da 0569 6e64  oved.csvF)...ind
-00001d10: 6578 2901 da07 7265 7374 6172 7429 1972  ex)...restart).r
-00001d20: 1b00 0000 da14 6d75 6c74 6963 6f72 655f  ......multicore_
-00001d30: 7072 6f63 6573 7369 6e67 7220 0000 00da  processingr ....
-00001d40: 1573 7461 7274 5f70 726f 6365 7373 696e  .start_processin
-00001d50: 675f 706f 6f6c 7298 0000 0072 1f00 0000  g_poolr....r....
-00001d60: 721c 0000 00da 0569 7465 6d73 7258 0000  r......itemsrX..
-00001d70: 0072 9400 0000 7224 0000 0072 6600 0000  .r....r$...rf...
-00001d80: 7268 0000 00da 037a 6970 da09 6974 6572  rh.....zip..iter
-00001d90: 746f 6f6c 73da 0672 6570 6561 74da 046c  tools..repeat..l
-00001da0: 6973 74da 0773 7461 726d 6170 729a 0000  ist..starmapr...
-00001db0: 0072 7900 0000 7259 0000 00da 0944 6174  .ry...rY.....Dat
-00001dc0: 6146 7261 6d65 da0b 736f 7274 5f76 616c  aFrame..sort_val
-00001dd0: 7565 73da 0674 6f5f 6373 76da 146a 6f69  ues..to_csv..joi
-00001de0: 6e5f 7072 6f63 6573 7369 6e67 5f70 6f6f  n_processing_poo
-00001df0: 6c29 0a72 2e00 0000 722a 0000 0072 2900  l).r....r*...r).
-00001e00: 0000 7228 0000 00da 0470 6f6f 6c72 2c00  ..r(.....poolr,.
-00001e10: 0000 da05 6669 6c65 7372 6b00 0000 da08  ....filesrk.....
-00001e20: 6974 6572 6162 6c65 7282 0000 0072 0e00  iterabler....r..
-00001e30: 0000 720e 0000 0072 1100 0000 da1a 6361  ..r....r......ca
-00001e40: 6c63 756c 6174 655f 7374 6174 6973 7469  lculate_statisti
-00001e50: 6361 6c5f 6d61 7073 ed00 0000 7346 0000  cal_maps....sF..
-00001e60: 0006 010a 0104 0206 020c 0102 0108 ff10  ................
-00001e70: 0306 0114 0106 010a ff1c 031a 030c 011c  ................
-00001e80: ff04 0308 0108 0108 0108 0108 0104 fb06  ................
-00001e90: 0712 0110 0206 0218 0118 0214 011c ff02  ................
-00001ea0: 8006 0312 0104 ff72 af00 0000 6304 0000  .......r....c...
-00001eb0: 0000 0000 0000 0000 0008 0000 0005 0000  ................
-00001ec0: 0043 0000 0073 f000 0000 7400 a000 a100  .C...s....t.....
-00001ed0: 7d04 7401 a002 7c01 a101 0100 7403 7404  }.t...|.....t.t.
-00001ee0: 6a05 a006 7407 a101 8301 6a08 6401 1900  j...t.....j.d...
-00001ef0: 9b00 6402 9d02 6109 7c02 610a 7401 6a0b  ..d...a.|.a.t.j.
-00001f00: 7409 7c02 7c03 6403 8d03 610c 740d a00e  t.|.|.d...a.t...
-00001f10: 6404 a101 a00f 6405 a101 0100 7c00 6406  d.....d.....|.d.
-00001f20: 6b02 7237 740c 6a10 7337 740c 6a11 7237  k.r7t.j.s7t.j.r7
-00001f30: 7412 6407 8301 0100 7c00 6408 7600 7249  t.d.....|.d.v.rI
-00001f40: 7412 6409 7c00 9b00 640a 9d03 8301 0100  t.d.|...d.......
-00001f50: 7413 740c 7c00 8302 0100 6e19 740c 6a11  t.t.|.....n.t.j.
-00001f60: 7254 7412 640b 7c00 9b00 640c 9d03 8301  rTt.d.|...d.....
-00001f70: 0100 7414 7c00 8301 5c03 7d05 7d06 7d07  ..t.|...\.}.}.}.
-00001f80: 7415 7c05 7c06 7c07 7c00 8304 0100 740c  t.|.|.|.|.....t.
-00001f90: 6a11 7276 7412 640d 7416 7400 a000 a100  j.rvt.d.t.t.....
-00001fa0: 7c04 1800 640e 8302 9b00 640f 9d03 8301  |...d.....d.....
-00001fb0: 0100 6400 5300 6400 5300 2910 4e72 0500  ..d.S.d.S.).Nr..
-00001fc0: 0000 7a1d 2f63 6f6e 6669 6775 7261 7469  ..z./configurati
-00001fd0: 6f6e 5f70 726f 6669 6c65 732f 6d61 7073  on_profiles/maps
-00001fe0: 2f29 0172 5700 0000 7a0f 6e69 7079 7065  /).rW...z.nipype
-00001ff0: 2e77 6f72 6b66 6c6f 7772 0100 0000 7209  .workflowr....r.
-00002000: 0000 007a c422 4e6f 6973 6520 766f 6c75  ...z."Noise volu
-00002010: 6d65 2069 6e63 6c75 6465 6420 696e 2074  me included in t
-00002020: 696d 6520 7365 7269 6573 2220 6973 2066  ime series" is f
-00002030: 616c 7365 2e20 5472 7969 6e67 2074 6f20  alse. Trying to 
-00002040: 6669 6e64 2076 616c 7565 7320 666f 7220  find values for 
-00002050: 6561 6368 2070 6172 7469 6369 7061 6e74  each participant
-00002060: 2069 6e20 6e6f 6973 6556 616c 7565 732e   in noiseValues.
-00002070: 6373 7620 696e 7374 6561 642e 2049 6620  csv instead. If 
-00002080: 7468 6973 2069 7320 6e6f 7420 636f 7272  this is not corr
-00002090: 6563 742c 2073 6574 2022 4e6f 6973 6520  ect, set "Noise 
-000020a0: 766f 6c75 6d65 2069 6e63 6c75 6465 6420  volume included 
-000020b0: 696e 2074 696d 6520 7365 7269 6573 2220  in time series" 
-000020c0: 746f 2074 7275 652e 0a29 037a 1241 6464  to true..).z.Add
-000020d0: 2047 6175 7373 6961 6e20 6e6f 6973 657a   Gaussian noisez
-000020e0: 0a41 6464 206d 6f74 696f 6e7a 1653 6570  .Add motionz.Sep
-000020f0: 6172 6174 6520 6e6f 6973 6520 766f 6c75  arate noise volu
-00002100: 6d65 737a 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d  meszn.----------
-00002110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002120: 2d2d 2d2d 2d2d 0a2d 2d2d 2d2d 2d2d 2d20  ------.-------- 
-00002130: 5275 6e6e 696e 6720 7574 696c 6974 7920  Running utility 
-00002140: 2d2d 2d2d 2d2d 2d2d 0a2d 2d2d 2d2d 2d2d  --------.-------
-00002150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002160: 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 756e 6e69  ---------..Runni
-00002170: 6e67 207a 0a20 7574 696c 6974 792e 0a7a  ng z. utility..z
-00002180: 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  n.--------------
-00002190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021a0: 2d2d 0a2d 2d2d 2053 7461 7469 7374 6963  --.--- Statistic
-000021b0: 616c 206d 6170 2063 7265 6174 696f 6e20  al map creation 
-000021c0: 2d2d 2d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---.------------
-000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021e0: 2d2d 2d2d 0a0a 4372 6561 7469 6e67 207a  ----..Creating z
-000021f0: 0720 6d61 7073 2e0a 7a12 0a2d 2d2d 2043  . maps..z..--- C
-00002200: 6f6d 706c 6574 6564 2069 6e20 7203 0000  ompleted in r...
-00002210: 007a 0e20 7365 636f 6e64 7320 2d2d 2d0a  .z. seconds ---.
-00002220: 0a29 17da 0474 696d 6572 2000 0000 da0c  .)...timer .....
-00002230: 6368 6563 6b76 6572 7369 6f6e 7254 0000  checkversionrT..
-00002240: 0072 5600 0000 7257 0000 00da 0761 6273  .rV...rW.....abs
-00002250: 7061 7468 da08 5f5f 6669 6c65 5f5f 7255  path..__file__rU
-00002260: 0000 0072 2600 0000 7227 0000 00da 0b6c  ...r&...r'.....l
-00002270: 6f61 645f 636f 6e66 6967 721b 0000 00da  oad_configr.....
-00002280: 076c 6f67 6769 6e67 da09 6765 744c 6f67  .logging..getLog
-00002290: 6765 72da 0873 6574 4c65 7665 6c72 5000  ger..setLevelrP.
-000022a0: 0000 7298 0000 0072 1f00 0000 7204 0000  ..r....r....r...
-000022b0: 0072 2f00 0000 72af 0000 00da 0572 6f75  .r/...r......rou
-000022c0: 6e64 2908 7228 0000 00da 0776 6572 7369  nd).r(.....versi
-000022d0: 6f6e da0b 636f 6e66 6967 5f66 696c 6572  on..config_filer
-000022e0: 5700 0000 da0a 7374 6172 745f 7469 6d65  W.....start_time
-000022f0: 722e 0000 0072 2a00 0000 7229 0000 0072  r....r*...r)...r
-00002300: 0e00 0000 720e 0000 0072 1100 0000 da04  ....r....r......
-00002310: 6d61 696e 1801 0000 732c 0000 0008 030a  main....s,......
-00002320: 011c 0304 0110 0310 0214 0208 0108 0304  ................
-00002330: 0102 030a fd0c 0506 0304 0102 030a fd0e  ................
-00002340: 050e 0106 0222 0104 ff72 bc00 0000 720d  ....."...r....r.
-00002350: 0000 0029 1b72 a400 0000 da05 6e75 6d70  ...).r......nump
-00002360: 7972 9200 0000 5a11 6e69 7079 7065 2e69  yr....Z.nipype.i
-00002370: 6e74 6572 6661 6365 7372 0200 0000 72b5  nterfacesr....r.
-00002380: 0000 0072 b000 0000 5a0d 484f 5553 452e  ...r....Z.HOUSE.
-00002390: 6861 6e64 6c65 7272 0400 0000 da05 7574  handlerr......ut
-000023a0: 696c 7372 1b00 0000 7226 0000 0072 2700  ilsr....r&...r'.
-000023b0: 0000 722f 0000 0072 3900 0000 724d 0000  ..r/...r9...rM..
-000023c0: 0072 6000 0000 725c 0000 0072 6c00 0000  .r`...r\...rl...
-000023d0: 7270 0000 0072 7300 0000 7274 0000 0072  rp...rs...rt...r
-000023e0: 8500 0000 7279 0000 0072 9a00 0000 72af  ....ry...r....r.
-000023f0: 0000 0072 bc00 0000 720e 0000 0072 0e00  ...r....r....r..
-00002400: 0000 720e 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
-00002410: 6f64 756c 653e 0100 0000 7330 0000 0008  odule>....s0....
-00002420: 0008 020c 0108 0108 010c 0208 0104 0204  ................
-00002430: 0104 0108 0308 2208 0808 1008 1e08 0408  ......".........
-00002440: 0a08 1108 0508 0708 2c08 1b08 130e 2b    ........,.....+
+00001150: 1001 04ff 7274 0000 0063 0500 0000 0000  ....rt...c......
+00001160: 0000 0000 0000 0e00 0000 0900 0000 4300  ..............C.
+00001170: 0000 736c 0100 0064 007d 0567 007d 0667  ..sl...d.}.g.}.g
+00001180: 007d 0774 00a0 017c 01a1 015c 027d 087d  .}.t...|...\.}.}
+00001190: 0974 00a0 027c 0864 017c 027c 049b 0064  .t...|.d.|.|...d
+000011a0: 0274 036a 049b 0064 039d 047c 09a1 0501  .t.j...d...|....
+000011b0: 007c 0064 046b 0272 4474 036a 0572 447c  .|.d.k.rDt.j.rD|
+000011c0: 049b 0064 057c 029b 0064 069d 047d 017c  ...d.|...d...}.|
+000011d0: 049b 0064 077c 029b 0064 089d 047d 0574  ...d.|...d...}.t
+000011e0: 066a 07a0 087c 01a1 0172 4074 066a 07a0  .j...|...r@t.j..
+000011f0: 087c 05a1 0173 4474 0964 0983 0182 0174  .|...sDt.d.....t
+00001200: 036a 0a72 5b74 0a7c 017c 027c 037c 0483  .j.r[t.|.|.|.|..
+00001210: 045c 037d 017d 0a7d 0b7c 06a0 0b7c 0ba1  .\.}.}.}.|...|..
+00001220: 0101 007c 07a0 0b7c 0aa1 0101 0074 036a  ...|...|.....t.j
+00001230: 0c72 807c 039b 0064 027c 029b 0064 0a9d  .r.|...d.|...d..
+00001240: 047d 0c74 0d6a 0e7c 017c 0c64 0b8d 02a0  .}.t.j.|.|.d....
+00001250: 0fa1 0001 007c 0c7d 0174 00a0 017c 01a1  .....|.}.t...|..
+00001260: 015c 027d 087d 0974 107c 087c 097c 027c  .\.}.}.t.|.|.|.|
+00001270: 0464 0c83 057d 0174 036a 1172 9e74 0d6a  .d...}.t.j.r.t.j
+00001280: 127c 0174 036a 1374 036a 147c 039b 0064  .|.t.j.t.j.|...d
+00001290: 027c 029b 0064 0d9d 0464 0e8d 04a0 0fa1  .|...d...d......
+000012a0: 0001 007c 039b 0064 027c 029b 0064 0d9d  ...|...d.|...d..
+000012b0: 047d 0174 036a 1572 b074 167c 017c 037c  .}.t.j.r.t.|.|.|
+000012c0: 0283 035c 027d 017d 0d7c 06a0 0b7c 017c  ...\.}.}.|...|.|
+000012d0: 0d67 02a1 0101 007c 017c 057c 067c 0766  .g.....|.|.|.|.f
+000012e0: 0453 0029 0f4e 7207 0000 0072 1300 0000  .S.).Nr....r....
+000012f0: 7265 0000 0072 0900 0000 7a0e 2f66 756e  re...r....z./fun
+00001300: 635f 766f 6c75 6d65 732f 7a07 2e6e 6969  c_volumes/z..nii
+00001310: 2e67 7a7a 0e2f 6e6f 6973 655f 766f 6c75  .gzz./noise_volu
+00001320: 6d65 2f7a 145f 6e6f 6973 655f 766f 6c75  me/z._noise_volu
+00001330: 6d65 2e6e 6969 2e67 7a7a 7543 6f75 6c64  me.nii.gzzuCould
+00001340: 206e 6f74 2066 696e 6420 7365 7061 7261   not find separa
+00001350: 7465 206e 6f69 7365 2061 6e64 2066 756e  te noise and fun
+00001360: 6374 696f 6e61 6c20 766f 6c75 6d65 732e  ctional volumes.
+00001370: 2052 756e 2074 6865 2022 7365 7061 7261   Run the "separa
+00001380: 7465 206e 6f69 7365 2076 6f6c 756d 6573  te noise volumes
+00001390: 2220 7574 696c 6974 7920 746f 2063 7265  " utility to cre
+000013a0: 6174 6520 7468 6573 6520 6669 6c65 732e  ate these files.
+000013b0: 7a18 5f6d 6f74 696f 6e5f 636f 7272 6563  z._motion_correc
+000013c0: 7465 642e 6e69 692e 677a 723b 0000 007a  ted.nii.gzr;...z
+000013d0: 154d 6f74 696f 6e20 636f 7272 6563 7465  .Motion correcte
+000013e0: 6420 6461 7461 7a10 5f73 6d6f 6f74 6865  d dataz._smoothe
+000013f0: 642e 6e69 692e 677a 2904 723c 0000 00da  d.nii.gz).r<....
+00001400: 0466 7768 6dda 1462 7269 6768 746e 6573  .fwhm..brightnes
+00001410: 735f 7468 7265 7368 6f6c 6472 3d00 0000  s_thresholdr=...
+00001420: 2917 7220 0000 0072 5100 0000 7269 0000  ).r ...rQ...ri..
+00001430: 0072 1b00 0000 721c 0000 0072 5000 0000  .r....r....rP...
+00001440: 7256 0000 0072 5700 0000 da06 6578 6973  rV...rW.....exis
+00001450: 7473 da11 4669 6c65 4e6f 7446 6f75 6e64  ts..FileNotFound
+00001460: 4572 726f 72da 1672 656d 6f76 655f 6d6f  Error..remove_mo
+00001470: 7469 6f6e 5f6f 7574 6c69 6572 73da 0665  tion_outliers..e
+00001480: 7874 656e 64da 116d 6f74 696f 6e5f 636f  xtend..motion_co
+00001490: 7272 6563 7469 6f6e 7202 0000 00da 074d  rrectionr......M
+000014a0: 4346 4c49 5254 7247 0000 0072 6c00 0000  CFLIRTrG...rl...
+000014b0: da11 7370 6174 6961 6c5f 736d 6f6f 7468  ..spatial_smooth
+000014c0: 696e 67da 0553 5553 414e da0e 736d 6f6f  ing..SUSAN..smoo
+000014d0: 7468 696e 675f 6677 686d da1e 736d 6f6f  thing_fwhm..smoo
+000014e0: 7468 696e 675f 6272 6967 6874 6e65 7373  thing_brightness
+000014f0: 5f74 6872 6573 686f 6c64 da0f 7465 6d70  _threshold..temp
+00001500: 6f72 616c 5f66 696c 7465 7272 7000 0000  oral_filterrp...
+00001510: 290e 7228 0000 0072 4b00 0000 724c 0000  ).r(...rK...rL..
+00001520: 0072 2a00 0000 7210 0000 0072 5e00 0000  .r*...r....r^...
+00001530: 7272 0000 00da 086f 7574 6c69 6572 7372  rr.....outliersr
+00001540: 3700 0000 7234 0000 00da 126f 7574 6c69  7...r4.....outli
+00001550: 6572 5f74 696d 6570 6f69 6e74 735a 0d6f  er_timepointsZ.o
+00001560: 7574 6c69 6572 5f66 696c 6573 da06 6f75  utlier_files..ou
+00001570: 7470 7574 5a0e 7265 6475 6e64 616e 745f  tputZ.redundant_
+00001580: 6669 6c65 720e 0000 0072 0e00 0000 7211  filer....r....r.
+00001590: 0000 00da 1570 7265 7061 7265 5f73 7461  .....prepare_sta
+000015a0: 746d 6170 5f66 696c 6573 9300 0000 733c  tmap_files....s<
+000015b0: 0000 0004 0104 0204 010e 0320 010e 0210  ........... ....
+000015c0: 0110 0118 0208 0106 0314 010a 010a 0106  ................
+000015d0: 0210 0112 0204 010e 0210 0106 020e 010e  ................
+000015e0: 0104 ff06 0110 0106 0210 010e 010c 0272  ...............r
+000015f0: 8500 0000 6304 0000 0000 0000 0000 0000  ....c...........
+00001600: 000f 0000 0008 0000 0043 0000 0073 0201  .........C...s..
+00001610: 0000 7c02 9b00 6401 7c01 9b00 6402 9d04  ..|...d.|...d...
+00001620: 7d04 7c02 9b00 6401 7c01 9b00 6403 9d04  }.|...d.|...d...
+00001630: 7d05 7c02 9b00 6401 7c01 9b00 6404 9d04  }.|...d.|...d...
+00001640: 7d06 7400 6a01 7c00 7c04 7c05 7c06 6405  }.t.j.|.|.|.|.d.
+00001650: 8d04 a002 a100 0100 7403 7c02 9b00 6401  ........t.|...d.
+00001660: 7c01 9b00 6402 9d04 8301 8f0c 7d07 7c07  |...d.......}.|.
+00001670: a004 a100 7d08 5700 6400 0400 0400 8303  ....}.W.d.......
+00001680: 0100 6e08 3100 733c 7701 0100 0100 0100  ..n.1.s<w.......
+00001690: 5900 0100 6700 7d09 7405 7c08 8301 4400  Y...g.}.t.|...D.
+000016a0: 5d16 5c02 7d0a 7d0b 7c0b a006 6406 6407  ].\.}.}.|...d.d.
+000016b0: a102 a007 6408 a101 7d0c 7c0c 6409 6b03  ....d...}.|.d.k.
+000016c0: 725d 7c09 a008 7c0a a101 0100 7147 7409  r]|...|.....qGt.
+000016d0: a00a 7c00 a101 5c02 7d0d 7d0e 740b 6a0c  ..|...\.}.}.t.j.
+000016e0: 7c0d 7c09 640a 640b 8d03 7d0d 740d 7c0d  |.|.d.d...}.t.|.
+000016f0: 7c0e 7c01 7c03 640c 8305 7d00 7c00 7c01  |.|.|.d...}.|.|.
+00001700: 740e 7c09 8301 6702 7c04 7c05 7c06 6703  t.|...g.|.|.|.g.
+00001710: 6603 5300 290d 4e72 1300 0000 7a0d 5f6f  f.S.).Nr....z._o
+00001720: 7574 6c69 6572 732e 7478 747a 0c5f 6d65  utliers.txtz._me
+00001730: 7472 6963 732e 706e 677a 0c5f 6d65 7472  trics.pngz._metr
+00001740: 6963 732e 7478 7429 0472 3c00 0000 723d  ics.txt).r<...r=
+00001750: 0000 00da 0f6f 7574 5f6d 6574 7269 635f  .....out_metric_
+00001760: 706c 6f74 da11 6f75 745f 6d65 7472 6963  plot..out_metric
+00001770: 5f76 616c 7565 7372 0b00 0000 7207 0000  _valuesr....r...
+00001780: 00da 0131 e9ff ffff ffe9 0300 0000 2901  ...1..........).
+00001790: da04 6178 6973 7a21 5265 6d6f 7665 6420  ..axisz!Removed 
+000017a0: 6d6f 7469 6f6e 206f 7574 6c69 6572 2074  motion outlier t
+000017b0: 696d 6570 6f69 6e74 7329 0f72 0200 0000  imepoints).r....
+000017c0: da0e 4d6f 7469 6f6e 4f75 746c 6965 7273  ..MotionOutliers
+000017d0: 7247 0000 0072 6600 0000 da09 7265 6164  rG...rf.....read
+000017e0: 6c69 6e65 73da 0965 6e75 6d65 7261 7465  lines..enumerate
+000017f0: da07 7265 706c 6163 65da 0466 696e 64da  ..replace..find.
+00001800: 0661 7070 656e 6472 2000 0000 7251 0000  .appendr ...rQ..
+00001810: 00da 026e 70da 0664 656c 6574 6572 6c00  ...np..deleterl.
+00001820: 0000 da03 6c65 6e29 0f72 4b00 0000 724c  ....len).rK...rL
+00001830: 0000 0072 2a00 0000 7210 0000 005a 0c6f  ...r*...r....Z.o
+00001840: 7574 6c69 6572 5f66 696c 655a 0c6f 7574  utlier_fileZ.out
+00001850: 6c69 6572 5f70 6c6f 745a 0e6f 7574 6c69  lier_plotZ.outli
+00001860: 6572 5f76 616c 7565 7372 6b00 0000 da05  er_valuesrk.....
+00001870: 6c69 6e65 7372 8300 0000 5a0a 7469 6d65  linesr....Z.time
+00001880: 5f70 6f69 6e74 da04 6c69 6e65 5a0d 6f75  _point..lineZ.ou
+00001890: 746c 6965 725f 6368 6563 6b72 3700 0000  tlier_checkr7...
+000018a0: 7234 0000 0072 0e00 0000 720e 0000 0072  r4...r....r....r
+000018b0: 1100 0000 7279 0000 00bf 0000 0073 2a00  ....ry.......s*.
+000018c0: 0000 1001 1001 1001 0802 0201 0201 04fe  ................
+000018d0: 0602 1602 0a01 1cff 0403 1001 1201 0801  ................
+000018e0: 0a01 0280 0e02 1001 1003 1802 7279 0000  ............ry..
+000018f0: 0063 0600 0000 0000 0000 0000 0000 0a00  .c..............
+00001900: 0000 0700 0000 4300 0000 737a 0000 007c  ......C...sz...|
+00001910: 0561 0074 01a0 027c 00a1 017d 067c 019b  .a.t...|...}.|..
+00001920: 0064 017c 039b 0064 017c 009b 009d 057d  .d.|...d.|.....}
+00001930: 007c 019b 0064 017c 029b 009d 037d 0274  .|...d.|.....}.t
+00001940: 006a 0372 2274 0464 027c 069b 009d 0283  .j.r"t.d.|......
+00001950: 0101 0074 057c 047c 007c 067c 027c 0183  ...t.|.|.|.|.|..
+00001960: 055c 047d 007d 077d 087d 0974 067c 047c  .\.}.}.}.}.t.|.|
+00001970: 007c 067c 077c 027c 0183 0601 0074 077c  .|.|.|.|.....t.|
+00001980: 0883 0101 007c 0953 0029 034e 7213 0000  .....|.S.).Nr...
+00001990: 007a 1820 2020 2020 2020 2041 6e61 6c79  .z.        Analy
+000019a0: 7369 6e67 2066 696c 653a 2029 0872 1b00  sing file: ).r..
+000019b0: 0000 7220 0000 00da 0973 7472 6970 5f65  ..r .....strip_e
+000019c0: 7874 da07 7665 7262 6f73 6572 1f00 0000  xt..verboser....
+000019d0: 7285 0000 0072 7400 0000 7273 0000 0029  r....rt...rs...)
+000019e0: 0a72 4b00 0000 7210 0000 0072 2a00 0000  .rK...r....r*...
+000019f0: 7229 0000 0072 2800 0000 da03 6366 6772  r)...r(.....cfgr
+00001a00: 4c00 0000 725e 0000 0072 7200 0000 7282  L...r^...rr...r.
+00001a10: 0000 0072 0e00 0000 720e 0000 0072 1100  ...r....r....r..
+00001a20: 0000 da1a 7072 6f63 6573 735f 6669 6c65  ....process_file
+00001a30: 735f 666f 725f 7374 6174 6d61 7073 da00  s_for_statmaps..
+00001a40: 0000 7314 0000 0004 020a 0214 010e 0106  ..s.............
+00001a50: 020e 0118 0212 0108 0204 0272 9a00 0000  ...........r....
+00001a60: 6304 0000 0000 0000 0000 0000 000a 0000  c...............
+00001a70: 000a 0000 0043 0000 0073 a401 0000 7400  .....C...s....t.
+00001a80: 6a01 7208 7402 a003 a100 7d04 6e02 6400  j.r.t.....}.n.d.
+00001a90: 7d04 7400 6a04 7218 7405 6401 7400 6a06  }.t.j.r.t.d.t.j.
+00001aa0: 9b00 6402 7c01 9b00 9d04 8301 0100 7c00  ..d.|.........|.
+00001ab0: a007 a100 4400 5da7 5c02 7d05 7d06 7400  ....D.].\.}.}.t.
+00001ac0: 6a04 7235 7405 6403 7c05 a008 6404 a101  j.r5t.d.|...d...
+00001ad0: 6405 1900 9b00 6406 7409 7c06 8301 9b00  d.....d.t.|.....
+00001ae0: 6407 9d05 8301 0100 7402 6a0a 7c05 9b00  d.......t.j.|...
+00001af0: 6404 7400 6a06 9b00 6408 9d04 6409 640a  d.t.j...d...d.d.
+00001b00: 8d02 0100 740b 7c05 9b00 6404 7400 6a06  ....t.|...d.t.j.
+00001b10: 9b00 640b 9d04 640c 8302 8f0d 7d07 7c07  ..d...d.....}.|.
+00001b20: a00c 640d a101 0100 5700 6400 0400 0400  ..d.....W.d.....
+00001b30: 8303 0100 6e08 3100 735f 7701 0100 0100  ....n.1.s_w.....
+00001b40: 0100 5900 0100 740d 7c06 740e a00f 7c05  ..Y...t.|.t...|.
+00001b50: a101 740e a00f 7c01 a101 740e a00f 7c02  ..t...|...t...|.
+00001b60: a101 740e a00f 7c03 a101 740e a00f 7400  ..t...|...t...t.
+00001b70: a101 8306 7d08 7400 6a01 7288 7410 7c04  ....}.t.j.r.t.|.
+00001b80: a011 7412 7c08 a102 8301 7d09 6e08 7410  ..t.|.....}.n.t.
+00001b90: 740e a011 7412 7c08 a102 8301 7d09 7400  t...t.|.....}.t.
+00001ba0: 6a13 72c3 7414 6a15 640e 640f 6702 7c09  j.r.t.j.d.d.g.|.
+00001bb0: 6410 8d02 a016 640f a101 7d09 740b 7c05  d.....d...}.t.|.
+00001bc0: 9b00 6404 7c01 9b00 6411 9d04 640c 8302  ..d.|...d...d...
+00001bd0: 8f11 7d07 7c07 a00c 7c09 6a17 6412 6413  ..}.|...|.j.d.d.
+00001be0: 8d01 a101 0100 5700 6400 0400 0400 8303  ......W.d.......
+00001bf0: 0100 711c 3100 73be 7701 0100 0100 0100  ..q.1.s.w.......
+00001c00: 5900 0100 711c 7400 6a01 72d0 7402 6a18  Y...q.t.j.r.t.j.
+00001c10: 7c04 6412 6414 8d02 0100 6400 5300 6400  |.d.d.....d.S.d.
+00001c20: 5300 2915 4e7a 160a 5365 6172 6368 696e  S.).Nz..Searchin
+00001c30: 6720 696e 2066 6f6c 6465 723a 207a 1d0a  g in folder: z..
+00001c40: 5361 7669 6e67 206f 7574 7075 7420 696e  Saving output in
+00001c50: 2064 6972 6563 746f 7279 3a20 7a2c 0a43   directory: z,.C
+00001c60: 7265 6174 696e 6720 7374 6174 6973 7469  reating statisti
+00001c70: 6361 6c20 6d61 7073 2066 6f72 2070 6172  cal maps for par
+00001c80: 7469 6369 7061 6e74 3a20 7213 0000 0072  ticipant: r....r
+00001c90: 8900 0000 7a1d 0a20 2020 2020 2043 7265  ....z..      Cre
+00001ca0: 6174 696e 6720 7374 6174 6d61 7073 2066  ating statmaps f
+00001cb0: 6f72 207a 0620 6669 6c65 7372 6500 0000  or z. filesre...
+00001cc0: 5472 1600 0000 7263 0000 00da 0177 7207  Tr....rc.....wr.
+00001cd0: 0000 00da 0446 696c 657a 104f 7574 6c69  .....Filez.Outli
+00001ce0: 6572 7320 7265 6d6f 7665 6429 02da 0763  ers removed)...c
+00001cf0: 6f6c 756d 6e73 7237 0000 007a 1f2f 6e75  olumnsr7...z./nu
+00001d00: 6d62 6572 5f6f 665f 6f75 746c 6965 7273  mber_of_outliers
+00001d10: 5f72 656d 6f76 6564 2e63 7376 4629 01da  _removed.csvF)..
+00001d20: 0569 6e64 6578 2901 da07 7265 7374 6172  .index)...restar
+00001d30: 7429 1972 1b00 0000 da14 6d75 6c74 6963  t).r......multic
+00001d40: 6f72 655f 7072 6f63 6573 7369 6e67 7220  ore_processingr 
+00001d50: 0000 00da 1573 7461 7274 5f70 726f 6365  .....start_proce
+00001d60: 7373 696e 675f 706f 6f6c 7298 0000 0072  ssing_poolr....r
+00001d70: 1f00 0000 721c 0000 00da 0569 7465 6d73  ....r......items
+00001d80: 7258 0000 0072 9400 0000 7224 0000 0072  rX...r....r$...r
+00001d90: 6600 0000 7268 0000 00da 037a 6970 da09  f...rh.....zip..
+00001da0: 6974 6572 746f 6f6c 73da 0672 6570 6561  itertools..repea
+00001db0: 74da 046c 6973 74da 0773 7461 726d 6170  t..list..starmap
+00001dc0: 729a 0000 0072 7900 0000 7259 0000 00da  r....ry...rY....
+00001dd0: 0944 6174 6146 7261 6d65 da0b 736f 7274  .DataFrame..sort
+00001de0: 5f76 616c 7565 73da 0674 6f5f 6373 76da  _values..to_csv.
+00001df0: 146a 6f69 6e5f 7072 6f63 6573 7369 6e67  .join_processing
+00001e00: 5f70 6f6f 6c29 0a72 2e00 0000 722a 0000  _pool).r....r*..
+00001e10: 0072 2900 0000 7228 0000 00da 0470 6f6f  .r)...r(.....poo
+00001e20: 6c72 2c00 0000 da05 6669 6c65 7372 6b00  lr,.....filesrk.
+00001e30: 0000 da08 6974 6572 6162 6c65 7282 0000  ....iterabler...
+00001e40: 0072 0e00 0000 720e 0000 0072 1100 0000  .r....r....r....
+00001e50: da1a 6361 6c63 756c 6174 655f 7374 6174  ..calculate_stat
+00001e60: 6973 7469 6361 6c5f 6d61 7073 ed00 0000  istical_maps....
+00001e70: 7346 0000 0006 010a 0104 0206 020c 0102  sF..............
+00001e80: 0108 ff10 0306 0114 0106 010a ff1c 031a  ................
+00001e90: 030c 011c ff04 0308 0108 0108 0108 0108  ................
+00001ea0: 0104 fb06 0712 0110 0206 0218 0118 0214  ................
+00001eb0: 011c ff02 8006 0312 0104 ff72 af00 0000  ...........r....
+00001ec0: 6304 0000 0000 0000 0000 0000 0008 0000  c...............
+00001ed0: 0005 0000 0043 0000 0073 f000 0000 7400  .....C...s....t.
+00001ee0: a000 a100 7d04 7401 a002 7c01 a101 0100  ....}.t...|.....
+00001ef0: 7403 7404 6a05 a006 7407 a101 8301 6a08  t.t.j...t.....j.
+00001f00: 6401 1900 9b00 6402 9d02 6109 7c02 610a  d.....d...a.|.a.
+00001f10: 7401 6a0b 7409 7c02 7c03 6403 8d03 610c  t.j.t.|.|.d...a.
+00001f20: 740d a00e 6404 a101 a00f 6405 a101 0100  t...d.....d.....
+00001f30: 7c00 6406 6b02 7237 740c 6a10 7337 740c  |.d.k.r7t.j.s7t.
+00001f40: 6a11 7237 7412 6407 8301 0100 7c00 6408  j.r7t.d.....|.d.
+00001f50: 7600 7249 7412 6409 7c00 9b00 640a 9d03  v.rIt.d.|...d...
+00001f60: 8301 0100 7413 740c 7c00 8302 0100 6e19  ....t.t.|.....n.
+00001f70: 740c 6a11 7254 7412 640b 7c00 9b00 640c  t.j.rTt.d.|...d.
+00001f80: 9d03 8301 0100 7414 7c00 8301 5c03 7d05  ......t.|...\.}.
+00001f90: 7d06 7d07 7415 7c05 7c06 7c07 7c00 8304  }.}.t.|.|.|.|...
+00001fa0: 0100 740c 6a11 7276 7412 640d 7416 7400  ..t.j.rvt.d.t.t.
+00001fb0: a000 a100 7c04 1800 640e 8302 9b00 640f  ....|...d.....d.
+00001fc0: 9d03 8301 0100 6400 5300 6400 5300 2910  ......d.S.d.S.).
+00001fd0: 4e72 0500 0000 7a1d 2f63 6f6e 6669 6775  Nr....z./configu
+00001fe0: 7261 7469 6f6e 5f70 726f 6669 6c65 732f  ration_profiles/
+00001ff0: 6d61 7073 2f29 0172 5700 0000 7a0f 6e69  maps/).rW...z.ni
+00002000: 7079 7065 2e77 6f72 6b66 6c6f 7772 0100  pype.workflowr..
+00002010: 0000 7209 0000 007a c422 4e6f 6973 6520  ..r....z."Noise 
+00002020: 766f 6c75 6d65 2069 6e63 6c75 6465 6420  volume included 
+00002030: 696e 2074 696d 6520 7365 7269 6573 2220  in time series" 
+00002040: 6973 2066 616c 7365 2e20 5472 7969 6e67  is false. Trying
+00002050: 2074 6f20 6669 6e64 2076 616c 7565 7320   to find values 
+00002060: 666f 7220 6561 6368 2070 6172 7469 6369  for each partici
+00002070: 7061 6e74 2069 6e20 6e6f 6973 6556 616c  pant in noiseVal
+00002080: 7565 732e 6373 7620 696e 7374 6561 642e  ues.csv instead.
+00002090: 2049 6620 7468 6973 2069 7320 6e6f 7420   If this is not 
+000020a0: 636f 7272 6563 742c 2073 6574 2022 4e6f  correct, set "No
+000020b0: 6973 6520 766f 6c75 6d65 2069 6e63 6c75  ise volume inclu
+000020c0: 6465 6420 696e 2074 696d 6520 7365 7269  ded in time seri
+000020d0: 6573 2220 746f 2074 7275 652e 0a29 037a  es" to true..).z
+000020e0: 1241 6464 2047 6175 7373 6961 6e20 6e6f  .Add Gaussian no
+000020f0: 6973 657a 0a41 6464 206d 6f74 696f 6e7a  isez.Add motionz
+00002100: 1653 6570 6172 6174 6520 6e6f 6973 6520  .Separate noise 
+00002110: 766f 6c75 6d65 737a 6e0a 2d2d 2d2d 2d2d  volumeszn.------
+00002120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002130: 2d2d 2d2d 2d2d 2d2d 2d2d 0a2d 2d2d 2d2d  ----------.-----
+00002140: 2d2d 2d20 5275 6e6e 696e 6720 7574 696c  --- Running util
+00002150: 6974 7920 2d2d 2d2d 2d2d 2d2d 0a2d 2d2d  ity --------.---
+00002160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a52  -------------..R
+00002180: 756e 6e69 6e67 207a 0a20 7574 696c 6974  unning z. utilit
+00002190: 792e 0a7a 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d  y..zn.----------
+000021a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021b0: 2d2d 2d2d 2d2d 0a2d 2d2d 2053 7461 7469  ------.--- Stati
+000021c0: 7374 6963 616c 206d 6170 2063 7265 6174  stical map creat
+000021d0: 696f 6e20 2d2d 2d0a 2d2d 2d2d 2d2d 2d2d  ion ---.--------
+000021e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021f0: 2d2d 2d2d 2d2d 2d2d 0a0a 4372 6561 7469  --------..Creati
+00002200: 6e67 207a 0720 6d61 7073 2e0a 7a12 0a2d  ng z. maps..z..-
+00002210: 2d2d 2043 6f6d 706c 6574 6564 2069 6e20  -- Completed in 
+00002220: 7203 0000 007a 0e20 7365 636f 6e64 7320  r....z. seconds 
+00002230: 2d2d 2d0a 0a29 17da 0474 696d 6572 2000  ---..)...timer .
+00002240: 0000 da0c 6368 6563 6b76 6572 7369 6f6e  ....checkversion
+00002250: 7254 0000 0072 5600 0000 7257 0000 00da  rT...rV...rW....
+00002260: 0761 6273 7061 7468 da08 5f5f 6669 6c65  .abspath..__file
+00002270: 5f5f 7255 0000 0072 2600 0000 7227 0000  __rU...r&...r'..
+00002280: 00da 0b6c 6f61 645f 636f 6e66 6967 721b  ...load_configr.
+00002290: 0000 00da 076c 6f67 6769 6e67 da09 6765  .....logging..ge
+000022a0: 744c 6f67 6765 72da 0873 6574 4c65 7665  tLogger..setLeve
+000022b0: 6c72 5000 0000 7298 0000 0072 1f00 0000  lrP...r....r....
+000022c0: 7204 0000 0072 2f00 0000 72af 0000 00da  r....r/...r.....
+000022d0: 0572 6f75 6e64 2908 7228 0000 00da 0776  .round).r(.....v
+000022e0: 6572 7369 6f6e da0b 636f 6e66 6967 5f66  ersion..config_f
+000022f0: 696c 6572 5700 0000 da0a 7374 6172 745f  ilerW.....start_
+00002300: 7469 6d65 722e 0000 0072 2a00 0000 7229  timer....r*...r)
+00002310: 0000 0072 0e00 0000 720e 0000 0072 1100  ...r....r....r..
+00002320: 0000 da04 6d61 696e 1801 0000 732c 0000  ....main....s,..
+00002330: 0008 030a 011c 0304 0110 0310 0214 0208  ................
+00002340: 0108 0304 0102 030a fd0c 0506 0304 0102  ................
+00002350: 030a fd0e 050e 0106 0222 0104 ff72 bc00  ........."...r..
+00002360: 0000 720d 0000 0029 1b72 a400 0000 da05  ..r....).r......
+00002370: 6e75 6d70 7972 9200 0000 5a11 6e69 7079  numpyr....Z.nipy
+00002380: 7065 2e69 6e74 6572 6661 6365 7372 0200  pe.interfacesr..
+00002390: 0000 72b5 0000 0072 b000 0000 5a0d 484f  ..r....r....Z.HO
+000023a0: 5553 452e 6861 6e64 6c65 7272 0400 0000  USE.handlerr....
+000023b0: da05 7574 696c 7372 1b00 0000 7226 0000  ..utilsr....r&..
+000023c0: 0072 2700 0000 722f 0000 0072 3900 0000  .r'...r/...r9...
+000023d0: 724d 0000 0072 6000 0000 725c 0000 0072  rM...r`...r\...r
+000023e0: 6c00 0000 7270 0000 0072 7300 0000 7274  l...rp...rs...rt
+000023f0: 0000 0072 8500 0000 7279 0000 0072 9a00  ...r....ry...r..
+00002400: 0000 72af 0000 0072 bc00 0000 720e 0000  ..r....r....r...
+00002410: 0072 0e00 0000 720e 0000 0072 1100 0000  .r....r....r....
+00002420: da08 3c6d 6f64 756c 653e 0100 0000 7330  ..<module>....s0
+00002430: 0000 0008 0008 020c 0108 0108 010c 0208  ................
+00002440: 0104 0204 0104 0108 0308 2208 0808 1008  ..........".....
+00002450: 1e08 0408 0a08 1108 0508 0708 2c08 1b08  ............,...
+00002460: 130e 2b                                  ..+
```

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 15:25:50 2023 UTC, .py size: 9528 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 fe65 5a64 3825 0000  o........eZd8%..
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 8124 0000  o.........[d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000f 0000 0040 0000 0073 6e01 0000 6900  .....@...sn...i.
+00000020: 000e 0000 0040 0000 0073 5c01 0000 6900  .....@...s\...i.
 00000030: 6400 6401 6402 6901 9301 6403 6404 6405  d.d.d.i...d.d.d.
 00000040: 6406 6407 6408 9c04 9301 6409 6404 6405  d.d.d.....d.d.d.
 00000050: 640a 640b 9c03 9301 640c 640d 640e 6700  d.d.....d.d.d.g.
 00000060: 640f a201 6410 6411 6412 9c05 9301 6413  d...d.d.d.....d.
 00000070: 6414 6415 6410 6416 6417 6418 9c05 9301  d.d.d.d.d.d.....
 00000080: 6419 6414 641a 6410 641b 641c 9c04 9301  d.d.d.d.d.d.....
 00000090: 641d 6414 641e 6410 641f 641c 9c04 9301  d.d.d.d.d.d.....
@@ -14,341 +14,345 @@
 000000d0: 9301 6428 6404 6405 6429 640b 9c03 9301  ..d(d.d.d)d.....
 000000e0: 642a 6404 6405 642b 640b 9c03 9301 642c  d*d.d.d+d.....d,
 000000f0: 6401 6402 6901 9301 642d 6404 642e 642f  d.d.i...d-d.d.d/
 00000100: 640b 9c03 9301 6430 6414 6431 6432 6433  d.....d0d.d1d2d3
 00000110: 6408 9c04 9301 6434 6414 6435 6436 6437  d.....d4d.d5d6d7
 00000120: 6408 9c04 9301 6401 6402 6901 6404 6405  d.....d.d.i.d.d.
 00000130: 6438 640b 9c03 6404 642e 6439 643a 6408  d8d...d.d.d9d:d.
-00000140: 9c04 640d 643b 643c 643b 6702 6410 6411  ..d.d;d<d;g.d.d.
-00000150: 6412 9c05 6404 6405 643d 643e 6408 9c04  d...d.d.d=d>d...
-00000160: 6401 6402 6901 643f 6440 6441 6442 6443  d.d.i.d?d@dAdBdC
-00000170: 6444 9c05 6414 6445 6446 6447 6448 6418  dD..d.dEdFdGdHd.
-00000180: 9c05 6414 6445 6446 6449 644a 6418 9c05  ..d.dEdFdIdJd...
-00000190: 644b 9c09 a501 5a00 644c 5300 294d 7a10  dK....Z.dLS.)Mz.
-000001a0: 4765 6e65 7261 6c20 7365 7474 696e 6773  General settings
-000001b0: da04 7479 7065 da0a 7375 6268 6561 6469  ..type..subheadi
-000001c0: 6e67 da07 7665 7262 6f73 65da 0b43 6865  ng..verbose..Che
-000001d0: 636b 4275 7474 6f6e da04 7472 7565 7a1e  ckButton..truez.
-000001e0: 5665 7262 6f73 6520 7374 6174 6973 7469  Verbose statisti
-000001f0: 6361 6c20 6d61 7020 7374 6167 6573 7a2a  cal map stagesz*
-00000200: 7472 7565 206f 7220 6661 6c73 652e 2050  true or false. P
-00000210: 7269 6e74 2070 726f 6772 6573 7320 746f  rint progress to
-00000220: 2074 6572 6d69 6e61 6c2e 2904 7201 0000   terminal.).r...
-00000230: 00da 0b52 6563 6f6d 6d65 6e64 6564 da05  ...Recommended..
-00000240: 6c61 6265 6cda 0b44 6573 6372 6970 7469  label..Descripti
-00000250: 6f6e da14 6d75 6c74 6963 6f72 655f 7072  on..multicore_pr
-00000260: 6f63 6573 7369 6e67 7a95 7472 7565 206f  ocessingz.true o
-00000270: 7220 6661 6c73 652e 2055 7365 206d 756c  r false. Use mul
-00000280: 7469 636f 7265 2070 726f 6365 7373 696e  ticore processin
-00000290: 6720 6475 7269 6e67 2061 6e61 6c79 7369  g during analysi
-000002a0: 733f 204d 756c 7469 636f 7265 2070 726f  s? Multicore pro
-000002b0: 6365 7373 696e 6720 6375 7272 656e 746c  cessing currentl
-000002c0: 7920 776f 726b 7320 7769 7468 696e 2070  y works within p
-000002d0: 6172 7469 6369 7061 6e74 7320 6e6f 7420  articipants not 
-000002e0: 6265 7477 6565 6e20 7468 656d 2e20 5265  between them. Re
-000002f0: 636f 6d6d 656e 6465 643a 2074 7275 6529  commended: true)
-00000300: 0372 0100 0000 7206 0000 0072 0800 0000  .r....r....r....
-00000310: da0e 6d61 785f 636f 7265 5f75 7361 6765  ..max_core_usage
-00000320: da0a 4f70 7469 6f6e 4d65 6e75 da03 6d61  ..OptionMenu..ma
-00000330: 7829 0772 0c00 0000 e906 0000 00e9 0500  x).r............
-00000340: 0000 e904 0000 00e9 0300 0000 e902 0000  ................
-00000350: 00e9 0100 0000 da06 7374 7269 6e67 7a8b  ........stringz.
-00000360: 276d 6178 2720 746f 2073 656c 6563 7420  'max' to select 
-00000370: 6e75 6d62 6572 206f 6620 636f 7265 7320  number of cores 
-00000380: 6176 6169 6c61 626c 6520 6f6e 2074 6865  available on the
-00000390: 2073 7973 7465 6d2c 2061 6c74 6572 6e61   system, alterna
-000003a0: 7469 7665 6c79 2061 6e20 696e 7420 746f  tively an int to
-000003b0: 206d 616e 7561 6c6c 7920 7365 6c65 6374   manually select
-000003c0: 206e 756d 6265 7220 6f66 2063 6f72 6573   number of cores
-000003d0: 2074 6f20 7573 652e 2052 6563 6f6d 6d65   to use. Recomme
-000003e0: 6e64 6564 3a20 276d 6178 2729 0572 0100  nded: 'max').r..
-000003f0: 0000 7206 0000 00da 074f 7074 696f 6e73  ..r......Options
-00000400: da07 7361 7665 5f61 7372 0800 0000 da0b  ..save_asr......
-00000410: 6261 7365 5f66 6f6c 6465 72da 0545 6e74  base_folder..Ent
-00000420: 7279 da00 7a14 4261 7365 2066 6f6c 6465  ry..z.Base folde
-00000430: 7220 6c6f 6361 7469 6f6e 7a9e 4569 7468  r locationz.Eith
-00000440: 6572 2074 6865 2061 6273 6f6c 7574 6520  er the absolute 
-00000450: 6c6f 6361 7469 6f6e 206f 6620 7468 6520  location of the 
-00000460: 666f 6c64 6572 2063 6f6e 7461 696e 696e  folder containin
-00000470: 6720 7468 6520 7375 626a 6563 7473 206f  g the subjects o
-00000480: 7220 626c 616e 6b2c 2069 6620 626c 616e  r blank, if blan
-00000490: 6b20 7468 656e 2061 2062 726f 7773 6572  k then a browser
-000004a0: 2077 696e 646f 7720 7769 6c6c 2061 6c6c   window will all
-000004b0: 6f77 2079 6f75 2074 6f20 7365 6172 6368  ow you to search
-000004c0: 2066 6f72 2074 6865 2066 696c 6573 2061   for the files a
-000004d0: 7420 7275 6e74 696d 652e 2905 7201 0000  t runtime.).r...
-000004e0: 0072 0600 0000 7215 0000 0072 0700 0000  .r....r....r....
-000004f0: 7208 0000 00da 1169 6e70 7574 5f66 6f6c  r......input_fol
-00000500: 6465 725f 6e61 6d65 da04 6675 6e63 7a4c  der_name..funczL
-00000510: 466f 6c64 6572 2066 6f75 6e64 2069 6e20  Folder found in 
-00000520: 6561 6368 2073 7562 6a65 6374 7320 6469  each subjects di
-00000530: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
-00000540: 6e67 2074 6865 2066 696c 6573 2074 6f20  ng the files to 
-00000550: 6265 2061 6e61 6c79 7365 642e 2904 7201  be analysed.).r.
-00000560: 0000 0072 0600 0000 7215 0000 0072 0800  ...r....r....r..
-00000570: 0000 da12 6f75 7470 7574 5f66 6f6c 6465  ....output_folde
-00000580: 725f 6e61 6d65 da07 4445 4641 554c 547a  r_name..DEFAULTz
-00000590: 8044 6972 6563 746f 7279 2074 6f20 7361  .Directory to sa
-000005a0: 7665 206f 7574 7075 742e 2049 6620 7365  ve output. If se
-000005b0: 7420 746f 2044 4546 4155 4c54 2c20 7468  t to DEFAULT, th
-000005c0: 6520 6465 6661 756c 7420 6e61 6d65 2066  e default name f
-000005d0: 6f72 2074 6865 2073 7461 7469 7374 6963  or the statistic
-000005e0: 616c 206d 6170 2063 7265 6174 6564 2077  al map created w
-000005f0: 696c 6c20 6265 2075 7365 642e 2052 6563  ill be used. Rec
-00000600: 6f6d 6d65 6e64 6564 3a20 4445 4641 554c  ommended: DEFAUL
-00000610: 547a 1348 6967 6820 7061 7373 2066 696c  Tz.High pass fil
-00000620: 7465 7269 6e67 5a0f 7465 6d70 6f72 616c  teringZ.temporal
-00000630: 5f66 696c 7465 727a 5674 7275 6520 6f72  _filterzVtrue or
-00000640: 2066 616c 7365 2e20 5573 6520 6120 6869   false. Use a hi
-00000650: 6768 2070 6173 7320 6669 6c74 6572 2074  gh pass filter t
-00000660: 6f20 7265 6d6f 7665 206c 6f77 2066 7265  o remove low fre
-00000670: 7175 656e 6379 2064 7269 6674 2e20 5265  quency drift. Re
-00000680: 636f 6d6d 656e 6465 643a 2074 7275 655a  commended: trueZ
-00000690: 1668 6967 6870 6173 735f 6669 6c74 6572  .highpass_filter
-000006a0: 5f63 7574 6f66 6667 7b14 ae47 e17a 843f  _cutoffg{..G.z.?
-000006b0: 7a25 4869 6768 7061 7373 2066 696c 7465  z%Highpass filte
-000006c0: 7220 6375 746f 6666 2066 7265 7175 656e  r cutoff frequen
-000006d0: 6379 2028 487a 297a 7048 6967 6870 6173  cy (Hz)zpHighpas
-000006e0: 7320 6669 6c74 6572 2063 7574 6f66 6620  s filter cutoff 
-000006f0: 6672 6571 7565 6e63 7920 636f 6e76 6572  frequency conver
-00000700: 7465 6420 696e 746f 2073 6967 6d61 2069  ted into sigma i
-00000710: 6e20 7365 636f 6e64 7320 7573 696e 6720  n seconds using 
-00000720: 7468 6520 666f 726d 756c 6120 312f 2832  the formula 1/(2
-00000730: 2a66 2a54 5229 2e20 5265 636f 6d6d 656e  *f*TR). Recommen
-00000740: 6465 643a 2030 2e30 317a 114d 6f74 696f  ded: 0.01z.Motio
-00000750: 6e20 636f 7272 6563 7469 6f6e 5a16 7265  n correctionZ.re
-00000760: 6d6f 7665 5f6d 6f74 696f 6e5f 6f75 746c  move_motion_outl
-00000770: 6965 7273 7a7e 7472 7565 206f 7220 6661  iersz~true or fa
-00000780: 6c73 652e 2055 7365 2066 736c 5f6d 6f74  lse. Use fsl_mot
-00000790: 696f 6e5f 6f75 746c 6965 7273 2074 6f20  ion_outliers to 
-000007a0: 7265 6d6f 7665 206d 6f74 696f 6e20 6f75  remove motion ou
-000007b0: 746c 6965 7273 2875 7365 7320 6465 6661  tliers(uses defa
-000007c0: 756c 7420 6673 6c5f 6d6f 7469 6f6e 5f6f  ult fsl_motion_o
-000007d0: 7574 6c69 6572 7320 7365 7474 696e 6773  utliers settings
-000007e0: 292e 2052 6563 6f6d 6d65 6e64 6564 3a20  ). Recommended: 
-000007f0: 7472 7565 5a11 6d6f 7469 6f6e 5f63 6f72  trueZ.motion_cor
-00000800: 7265 6374 696f 6e7a 6774 7275 6520 6f72  rectionzgtrue or
-00000810: 2066 616c 7365 2e20 5573 6520 4d43 464c   false. Use MCFL
-00000820: 4952 5420 746f 206d 6f74 696f 6e20 636f  IRT to motion co
-00000830: 7272 6563 7420 766f 6c75 6d65 7320 2875  rrect volumes (u
-00000840: 7365 7320 6465 6661 756c 7420 4d43 464c  ses default MCFL
-00000850: 4952 5420 7365 7474 696e 6773 292e 2052  IRT settings). R
-00000860: 6563 6f6d 6d65 6e64 6564 3a20 7472 7565  ecommended: true
-00000870: 7a11 5370 6174 6961 6c20 736d 6f6f 7468  z.Spatial smooth
-00000880: 696e 675a 1173 7061 7469 616c 5f73 6d6f  ingZ.spatial_smo
-00000890: 6f74 6869 6e67 da05 6661 6c73 657a 3e74  othing..falsez>t
-000008a0: 7275 6520 6f72 2066 616c 7365 2e20 5573  rue or false. Us
-000008b0: 6573 2053 5553 414e 2074 6f20 7370 6174  es SUSAN to spat
-000008c0: 6961 6c20 736d 6f6f 7468 2e20 5265 636f  ial smooth. Reco
-000008d0: 6d6d 656e 6465 643a 2074 7275 65da 0e73  mmended: true..s
-000008e0: 6d6f 6f74 6869 6e67 5f66 7768 6d67 0000  moothing_fwhmg..
-000008f0: 0000 0000 2040 7a1b 5370 6174 6961 6c20  .... @z.Spatial 
-00000900: 736d 6f6f 7468 696e 6720 6677 686d 2028  smoothing fwhm (
-00000910: 6d6d 297a 4f66 7768 6d20 6f66 2073 6d6f  mm)zOfwhm of smo
-00000920: 6f74 6869 6e67 2c20 696e 206d 6d2c 2067  othing, in mm, g
-00000930: 6574 7320 636f 6e76 6572 7465 6420 7573  ets converted us
-00000940: 696e 6720 7371 7274 2838 2a6c 6f67 2832  ing sqrt(8*log(2
-00000950: 2929 2e20 5265 636f 6d6d 656e 6465 643a  )). Recommended:
-00000960: 2038 2e30 5a1e 736d 6f6f 7468 696e 675f   8.0Z.smoothing_
-00000970: 6272 6967 6874 6e65 7373 5f74 6872 6573  brightness_thres
-00000980: 686f 6c64 6700 0000 0000 409f 407a 2653  holdg.....@.@z&S
-00000990: 7061 7469 616c 2073 6d6f 6f74 6869 6e67  patial smoothing
-000009a0: 2062 7269 6768 746e 6573 7320 7468 7265   brightness thre
-000009b0: 7368 6f6c 647a 6753 686f 756c 6420 6265  sholdzgShould be
-000009c0: 2067 7265 6174 6572 2074 6861 6e20 6e6f   greater than no
-000009d0: 6973 6520 6c65 7665 6c20 616e 6420 6c65  ise level and le
-000009e0: 7373 2074 6861 6e20 636f 6e74 7261 7374  ss than contrast
-000009f0: 206f 6620 6564 6765 7320 746f 2062 6520   of edges to be 
-00000a00: 7072 6573 6572 7665 642e 2052 6563 6f6d  preserved. Recom
-00000a10: 6d65 6e64 6564 3a20 3230 3030 2e30 6132  mended: 2000.0a2
-00000a20: 0100 0074 7275 6520 6f72 2066 616c 7365  ...true or false
-00000a30: 2e20 436f 7272 6563 7469 6f6e 2066 6163  . Correction fac
-00000a40: 746f 7220 6f66 2030 2e37 2061 7070 6c69  tor of 0.7 appli
-00000a50: 6564 2077 6865 6e20 7275 6e6e 696e 6720  ed when running 
-00000a60: 6953 4e52 2063 616c 6375 6c61 7469 6f6e  iSNR calculation
-00000a70: 732c 2074 6f20 636f 7272 6563 7420 666f  s, to correct fo
-00000a80: 7220 5261 796c 6569 6768 2064 6973 7472  r Rayleigh distr
-00000a90: 6962 7574 6564 206e 6f69 7365 2077 6865  ibuted noise whe
-00000aa0: 6e20 7573 696e 6720 6d61 676e 6974 7564  n using magnitud
-00000ab0: 6520 7673 2063 6f6d 706c 6578 2069 6d61  e vs complex ima
-00000ac0: 6765 732e 200a 5265 6665 7265 6e63 653a  ges. .Reference:
-00000ad0: 2043 6f6e 7374 616e 7469 6e69 6465 732c   Constantinides,
-00000ae0: 2043 2e20 442e 2c20 4174 616c 6172 2c20   C. D., Atalar, 
-00000af0: 452e 2c20 2620 4d63 5665 6967 682c 2045  E., & McVeigh, E
-00000b00: 2e20 522e 2028 3139 3937 292e 2053 6967  . R. (1997). Sig
-00000b10: 6e61 6c2d 746f 2d4e 6f69 7365 204d 6561  nal-to-Noise Mea
-00000b20: 7375 7265 6d65 6e74 7320 696e 204d 6167  surements in Mag
-00000b30: 6e69 7475 6465 2049 6d61 6765 7320 6672  nitude Images fr
-00000b40: 6f6d 204e 4d52 2050 6861 7365 6420 4172  om NMR Phased Ar
-00000b50: 7261 7973 2e7a 244e 6f69 7365 2076 6f6c  rays.z$Noise vol
-00000b60: 756d 6520 696e 636c 7564 6564 2069 6e20  ume included in 
-00000b70: 7469 6d65 2073 6572 6965 7361 9901 0000  time seriesa....
-00000b80: 7472 7565 206f 7220 6661 6c73 652e 2053  true or false. S
-00000b90: 656c 6563 7420 7472 7565 2069 6620 6120  elect true if a 
-00000ba0: 6e6f 6973 6520 766f 6c75 6d65 2068 6173  noise volume has
-00000bb0: 2062 6565 6e20 636f 6c6c 6563 7465 6420   been collected 
-00000bc0: 6173 2070 6172 7420 6f66 2074 6865 2066  as part of the f
-00000bd0: 4d52 4920 7469 6d65 2073 6572 6965 732e  MRI time series.
-00000be0: 0a4e 4f54 453a 2049 6620 7472 7565 2c20  .NOTE: If true, 
-00000bf0: 7468 6520 6e6f 6973 6520 766f 6c75 6d65  the noise volume
-00000c00: 2069 6e20 7468 6520 7469 6d65 2073 6572   in the time ser
-00000c10: 6965 7320 7769 6c6c 2062 6520 7365 7061  ies will be sepa
-00000c20: 7261 7465 6420 6672 6f6d 2074 6865 2066  rated from the f
-00000c30: 756e 6374 696f 6e61 6c20 766f 6c75 6d65  unctional volume
-00000c40: 7320 616e 6420 7769 6c6c 2062 6520 706c  s and will be pl
-00000c50: 6163 6564 2069 6e74 6f20 7468 6520 666f  aced into the fo
-00000c60: 6c64 6572 2022 6675 6e63 5f6e 6f69 7365  lder "func_noise
-00000c70: 566f 6c75 6d65 5265 6d6f 7665 6422 2e0a  VolumeRemoved"..
-00000c80: 4966 2022 6e6f 6973 6520 766f 6c75 6d65  If "noise volume
-00000c90: 2220 6973 2074 7275 6520 616e 6420 226e  " is true and "n
-00000ca0: 6f69 7365 2076 616c 7565 2220 6973 206e  oise value" is n
-00000cb0: 6f74 206e 6f6e 652c 2074 6865 206e 6f69  ot none, the noi
-00000cc0: 7365 2076 6f6c 756d 6520 7769 6c6c 2062  se volume will b
-00000cd0: 6520 7573 6564 2069 6e20 696d 6167 6520  e used in image 
-00000ce0: 534e 5220 6361 6c63 756c 6174 696f 6e20  SNR calculation 
-00000cf0: 7261 7468 6572 2074 6861 6e20 7468 6520  rather than the 
-00000d00: 7573 6572 2064 6566 696e 6564 206e 6f69  user defined noi
-00000d10: 7365 2076 616c 7565 2eda 0345 6e64 5a09  se value...EndZ.
-00000d20: 4265 6769 6e6e 696e 677a 2555 7365 206f  Beginningz%Use o
-00000d30: 6e6c 7920 6e6f 6e7a 6572 6f20 766f 7865  nly nonzero voxe
-00000d40: 6c73 2066 6f72 2069 534e 5220 6361 6c63  ls for iSNR calc
-00000d50: 7a0e 7472 7565 206f 7220 6661 6c73 652e  z.true or false.
-00000d60: da06 4275 7474 6f6e da11 6372 6561 7465  ..Button..create
-00000d70: 5f6e 6f69 7365 5f66 696c 657a 1643 7265  _noise_filez.Cre
-00000d80: 6174 6520 6e6f 6973 6556 616c 7565 732e  ate noiseValues.
-00000d90: 6373 7646 61f9 0300 0043 7265 6174 6520  csvFa....Create 
-00000da0: 6120 6e6f 6973 6556 616c 7565 732e 6373  a noiseValues.cs
-00000db0: 7620 6669 6c65 2074 6f20 6465 7465 726d  v file to determ
-00000dc0: 696e 6520 7768 6174 2074 6865 2073 7461  ine what the sta
-00000dd0: 6e64 6172 6420 6465 7669 6174 696f 6e6f  ndard deviationo
-00000de0: 6620 7468 6520 4761 7573 7369 616e 2073  f the Gaussian s
-00000df0: 686f 756c 6420 6265 2077 6865 6e20 6164  hould be when ad
-00000e00: 6469 6e67 206e 6f69 7365 2074 6f20 6561  ding noise to ea
-00000e10: 6368 2070 6172 7469 6369 7061 6e74 2773  ch participant's
-00000e20: 2064 6174 6120 2874 6865 2064 6973 7472   data (the distr
-00000e30: 6962 7574 696f 6e20 7769 6c6c 2068 6176  ibution will hav
-00000e40: 6520 6120 6d65 616e 206f 6620 3029 2e54  e a mean of 0).T
-00000e50: 6869 7320 7769 6c6c 206e 6f74 206f 7665  his will not ove
-00000e60: 7277 7269 7465 2074 6865 206f 7269 6769  rwrite the origi
-00000e70: 6e61 6c20 6669 6c65 732e 2052 6563 6f6d  nal files. Recom
-00000e80: 6d65 6e64 6564 3a20 5468 6520 7374 616e  mended: The stan
-00000e90: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
-00000ea0: 7665 7220 7469 6d65 2066 6f75 6e64 2069  ver time found i
-00000eb0: 6e20 7468 6520 6461 7461 7365 742e 0a4e  n the dataset..N
-00000ec0: 4f54 453a 2043 616e 2062 6520 7573 6564  OTE: Can be used
-00000ed0: 2074 6f20 7365 6520 686f 7720 6164 6469   to see how addi
-00000ee0: 7469 6f6e 616c 206e 6f69 7365 2061 6666  tional noise aff
-00000ef0: 6563 7473 2061 6e61 6c79 7369 732e 2054  ects analysis. T
-00000f00: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-00000f10: 6e6f 6973 6520 6c65 7665 6c20 666f 7220  noise level for 
-00000f20: 6561 6368 2070 6172 7469 6369 7061 6e74  each participant
-00000f30: 2c20 6372 6561 7465 2074 534e 5220 6d61  , create tSNR ma
-00000f40: 7073 2077 6974 6820 7468 6520 6652 4154  ps with the fRAT
-00000f50: 2061 6e64 2072 756e 2074 6865 2066 756c   and run the ful
-00000f60: 6c20 616e 616c 7973 6973 2075 7369 6e67  l analysis using
-00000f70: 2074 6865 2074 5374 6420 6669 6c65 732e   the tStd files.
-00000f80: 2054 6865 206d 6561 6e20 7661 6c75 6573   The mean values
-00000f90: 206f 6620 7468 6973 2061 6e61 6c79 7369   of this analysi
-00000fa0: 7320 696e 2065 6163 6820 7061 7274 6963  s in each partic
-00000fb0: 6970 616e 7473 2073 7562 666f 6c64 6572  ipants subfolder
-00000fc0: 2c20 7769 6c6c 2074 6865 6e20 7368 6f77  , will then show
-00000fd0: 2079 6f75 2074 6865 2061 7665 7261 6765   you the average
-00000fe0: 206e 6f69 7365 2066 6f72 2065 6163 6820   noise for each 
-00000ff0: 7265 6769 6f6e 2066 6f72 2065 6163 6820  region for each 
-00001000: 7061 7274 6963 6970 616e 742e 0a0a 5468  participant...Th
-00001010: 6973 2066 696c 6520 6361 6e20 616c 736f  is file can also
-00001020: 2062 6520 7573 6564 2074 6f20 6d61 6e75   be used to manu
-00001030: 616c 6c79 2073 6574 2061 206e 6f69 7365  ally set a noise
-00001040: 2076 616c 7565 2066 6f72 2065 6163 6820   value for each 
-00001050: 7061 7274 6963 6970 616e 7420 666f 7220  participant for 
-00001060: 7573 6520 696e 2069 534e 5220 6361 6c63  use in iSNR calc
-00001070: 756c 6174 696f 6e2e 2054 6869 7320 6e6f  ulation. This no
-00001080: 6973 6520 7661 6c75 6520 6361 6e20 6265  ise value can be
-00001090: 2063 616c 6375 6c61 7465 6420 6173 2074   calculated as t
-000010a0: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
-000010b0: 6174 696f 6e20 6f66 2076 6f78 656c 2076  ation of voxel v
-000010c0: 616c 7565 7320 6f75 7473 6964 6520 6f66  alues outside of
-000010d0: 2074 6865 2062 7261 696e 2e20 4966 2022   the brain. If "
-000010e0: 4e6f 6973 6520 766f 6c75 6d65 2069 6e63  Noise volume inc
-000010f0: 6c75 6465 6420 696e 2074 696d 6520 7365  luded in time se
-00001100: 7269 6573 2220 6973 2073 6574 2074 6f20  ries" is set to 
-00001110: 7472 7565 2c20 7374 616e 6461 7264 2064  true, standard d
-00001120: 6576 6961 7469 6f6e 206f 6620 6e6f 6973  eviation of nois
-00001130: 6520 7769 6c6c 2062 6520 6361 6c63 756c  e will be calcul
-00001140: 6174 6564 2075 7369 6e67 2074 6865 206e  ated using the n
-00001150: 6f69 7365 2076 6f6c 756d 652c 2065 7665  oise volume, eve
-00001160: 6e20 6966 2061 206e 6f69 7365 2076 616c  n if a noise val
-00001170: 7565 2068 6173 2062 6565 6e20 7072 6f76  ue has been prov
-00001180: 6964 6564 2069 6e20 7468 6973 2066 696c  ided in this fil
-00001190: 652e 2905 7201 0000 00da 0743 6f6d 6d61  e.).r......Comma
-000011a0: 6e64 da04 5465 7874 7a09 5061 7373 2073  nd..Textz.Pass s
-000011b0: 656c 6672 0800 0000 7212 0000 00da 046c  elfr....r......l
-000011c0: 6973 747a 134e 6f69 7365 206d 756c 7469  istz.Noise multi
-000011d0: 706c 6965 7228 7329 7af9 5072 6f76 6964  plier(s)z.Provid
-000011e0: 6520 6120 636f 6d6d 612d 7365 7061 7261  e a comma-separa
-000011f0: 7465 6420 6c69 7374 206f 6620 6d75 6c74  ted list of mult
-00001200: 6970 6c69 6572 732c 2065 2e67 2e20 2731  ipliers, e.g. '1
-00001210: 2c20 3527 2e20 4120 7365 7061 7261 7465  , 5'. A separate
-00001220: 2066 696c 6520 7769 6c6c 2062 6520 7072   file will be pr
-00001230: 6f64 7563 6564 2066 6f72 2065 6163 6820  oduced for each 
-00001240: 6d75 6c74 6970 6c69 6572 2e0a 4e4f 5445  multiplier..NOTE
-00001250: 3a20 4164 6465 6420 6861 7320 6120 6761  : Added has a ga
-00001260: 7573 7369 616e 2064 6973 7472 6962 7574  ussian distribut
-00001270: 696f 6e2c 2077 6974 6820 6120 6d65 616e  ion, with a mean
-00001280: 206f 6620 3020 616e 6420 6120 7374 616e   of 0 and a stan
-00001290: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
-000012a0: 6620 7468 6520 6e6f 6973 6520 6c65 7665  f the noise leve
-000012b0: 6c20 6f66 2065 6163 6820 7061 7274 6963  l of each partic
-000012c0: 6970 616e 7420 2a20 6d75 6c74 6970 6c69  ipant * multipli
-000012d0: 6572 2e7a 144d 6f74 696f 6e20 6d75 6c74  er.z.Motion mult
-000012e0: 6970 6c69 6572 2873 2961 1101 0000 5072  iplier(s)a....Pr
-000012f0: 6f76 6964 6520 6120 636f 6d6d 612d 7365  ovide a comma-se
-00001300: 7061 7261 7465 6420 6c69 7374 206f 6620  parated list of 
-00001310: 6d75 6c74 6970 6c69 6572 732c 2065 2e67  multipliers, e.g
-00001320: 2e20 2731 2c20 3527 2e20 4120 7365 7061  . '1, 5'. A sepa
-00001330: 7261 7465 2066 696c 6520 7769 6c6c 2062  rate file will b
-00001340: 6520 7072 6f64 7563 6564 2066 6f72 2065  e produced for e
-00001350: 6163 6820 6d75 6c74 6970 6c69 6572 2e0a  ach multiplier..
-00001360: 4e4f 5445 3a20 4164 6465 6420 6d6f 7469  NOTE: Added moti
-00001370: 6f6e 2068 6173 2061 2067 6175 7373 6961  on has a gaussia
-00001380: 6e20 6469 7374 7269 6275 7469 6f6e 2c20  n distribution, 
-00001390: 7769 7468 2061 206d 6561 6e20 6f66 2030  with a mean of 0
-000013a0: 2061 6e64 2061 2073 7461 6e64 6172 6420   and a standard 
-000013b0: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
-000013c0: 2061 7665 7261 6765 2072 6f74 6174 696f   average rotatio
-000013d0: 6e2f 7472 616e 736c 6174 696f 6e20 6f66  n/translation of
-000013e0: 2065 6163 6820 7061 7274 6963 6970 616e   each participan
-000013f0: 7420 2a20 6d75 6c74 6970 6c69 6572 2e29  t * multiplier.)
-00001400: 097a 1549 6d61 6765 2053 4e52 2063 616c  .z.Image SNR cal
-00001410: 6375 6c61 7469 6f6e 5a14 6d61 676e 6974  culationZ.magnit
-00001420: 7564 655f 636f 7272 6563 7469 6f6e 5a0c  ude_correctionZ.
-00001430: 6e6f 6973 655f 766f 6c75 6d65 5a15 6e6f  noise_volumeZ.no
-00001440: 6973 655f 766f 6c75 6d65 5f6c 6f63 6174  ise_volume_locat
-00001450: 696f 6e5a 2069 534e 525f 7374 645f 7573  ionZ iSNR_std_us
-00001460: 655f 6f6e 6c79 5f6e 6f6e 7a65 726f 5f76  e_only_nonzero_v
-00001470: 6f78 656c 737a 1241 6464 2047 6175 7373  oxelsz.Add Gauss
-00001480: 6961 6e20 6e6f 6973 655a 1763 7265 6174  ian noiseZ.creat
-00001490: 655f 6e6f 6973 655f 6c65 7665 6c5f 6669  e_noise_level_fi
-000014a0: 6c65 5a11 6e6f 6973 655f 6d75 6c74 6970  leZ.noise_multip
-000014b0: 6c69 6572 735a 126d 6f74 696f 6e5f 6d75  liersZ.motion_mu
-000014c0: 6c74 6970 6c69 6572 734e 2901 da10 5374  ltipliersN)...St
-000014d0: 6174 6973 7469 6361 6c5f 6d61 7073 a900  atistical_maps..
-000014e0: 7226 0000 0072 2600 0000 fa5f 2f55 7365  r&...r&...._/Use
-000014f0: 7273 2f6c 7078 6568 3130 2f44 6f63 756d  rs/lpxeh10/Docum
-00001500: 656e 7473 2f52 6570 6f73 6974 6f72 6965  ents/Repositorie
-00001510: 732f 664d 5249 5f52 4f49 5f61 6e61 6c79  s/fMRI_ROI_analy
-00001520: 7369 735f 746f 6f6c 2f66 5241 542f 7574  sis_tool/fRAT/ut
-00001530: 696c 732f 7374 6174 6d61 705f 636f 6e66  ils/statmap_conf
-00001540: 6967 5f73 6574 7570 2e70 79da 083c 6d6f  ig_setup.py..<mo
-00001550: 6475 6c65 3e01 0000 0073 ba00 0000 0200  dule>....s......
-00001560: 0801 02ff 0803 0201 04ff 02fd 0606 0201  ................
-00001570: 04ff 02fa 0c0b 0201 0201 04fe 02f5 0810  ................
-00001580: 0201 0201 04fe 02f0 0816 0201 04ff 02ea  ................
-00001590: 081a 0201 04ff 02e6 081f 02e1 0621 0201  .............!..
-000015a0: 04ff 02df 0625 0201 0201 04fe 02db 082a  .....%.........*
-000015b0: 02d6 062c 0201 04ff 02d4 0630 0201 04ff  ...,.......0....
-000015c0: 02d0 0834 02cc 0636 0201 04ff 02ca 0639  ...4...6.......9
-000015d0: 0201 0201 04fe 02c7 063d 0201 0201 04fe  .........=......
-000015e0: 02c3 0642 0402 0201 04ff 0607 0201 04ff  ...B............
-000015f0: 0a08 0201 0201 04fe 0405 0201 0201 04fe  ................
-00001600: 0604 0602 0201 0201 04fe 0815 0201 04ff  ................
-00001610: 0806 0201 04ff 0c87                      ........
+00000140: 9c04 6404 6405 643b 643c 6408 9c04 6401  ..d.d.d;d<d...d.
+00000150: 6402 6901 643d 643e 643f 6440 6441 6442  d.i.d=d>d?d@dAdB
+00000160: 9c05 6414 6443 6444 6445 6446 6418 9c05  ..d.dCdDdEdFd...
+00000170: 6414 6443 6444 6447 6448 6418 9c05 6449  d.dCdDdGdHd...dI
+00000180: 9c08 a501 5a00 644a 5300 294b 7a10 4765  ....Z.dJS.)Kz.Ge
+00000190: 6e65 7261 6c20 7365 7474 696e 6773 da04  neral settings..
+000001a0: 7479 7065 da0a 7375 6268 6561 6469 6e67  type..subheading
+000001b0: da07 7665 7262 6f73 65da 0b43 6865 636b  ..verbose..Check
+000001c0: 4275 7474 6f6e da04 7472 7565 7a1e 5665  Button..truez.Ve
+000001d0: 7262 6f73 6520 7374 6174 6973 7469 6361  rbose statistica
+000001e0: 6c20 6d61 7020 7374 6167 6573 7a2a 7472  l map stagesz*tr
+000001f0: 7565 206f 7220 6661 6c73 652e 2050 7269  ue or false. Pri
+00000200: 6e74 2070 726f 6772 6573 7320 746f 2074  nt progress to t
+00000210: 6572 6d69 6e61 6c2e 2904 7201 0000 00da  erminal.).r.....
+00000220: 0b52 6563 6f6d 6d65 6e64 6564 da05 6c61  .Recommended..la
+00000230: 6265 6cda 0b44 6573 6372 6970 7469 6f6e  bel..Description
+00000240: da14 6d75 6c74 6963 6f72 655f 7072 6f63  ..multicore_proc
+00000250: 6573 7369 6e67 7a95 7472 7565 206f 7220  essingz.true or 
+00000260: 6661 6c73 652e 2055 7365 206d 756c 7469  false. Use multi
+00000270: 636f 7265 2070 726f 6365 7373 696e 6720  core processing 
+00000280: 6475 7269 6e67 2061 6e61 6c79 7369 733f  during analysis?
+00000290: 204d 756c 7469 636f 7265 2070 726f 6365   Multicore proce
+000002a0: 7373 696e 6720 6375 7272 656e 746c 7920  ssing currently 
+000002b0: 776f 726b 7320 7769 7468 696e 2070 6172  works within par
+000002c0: 7469 6369 7061 6e74 7320 6e6f 7420 6265  ticipants not be
+000002d0: 7477 6565 6e20 7468 656d 2e20 5265 636f  tween them. Reco
+000002e0: 6d6d 656e 6465 643a 2074 7275 6529 0372  mmended: true).r
+000002f0: 0100 0000 7206 0000 0072 0800 0000 da0e  ....r....r......
+00000300: 6d61 785f 636f 7265 5f75 7361 6765 da0a  max_core_usage..
+00000310: 4f70 7469 6f6e 4d65 6e75 da03 6d61 7829  OptionMenu..max)
+00000320: 0772 0c00 0000 e906 0000 00e9 0500 0000  .r..............
+00000330: e904 0000 00e9 0300 0000 e902 0000 00e9  ................
+00000340: 0100 0000 da06 7374 7269 6e67 7a8b 276d  ......stringz.'m
+00000350: 6178 2720 746f 2073 656c 6563 7420 6e75  ax' to select nu
+00000360: 6d62 6572 206f 6620 636f 7265 7320 6176  mber of cores av
+00000370: 6169 6c61 626c 6520 6f6e 2074 6865 2073  ailable on the s
+00000380: 7973 7465 6d2c 2061 6c74 6572 6e61 7469  ystem, alternati
+00000390: 7665 6c79 2061 6e20 696e 7420 746f 206d  vely an int to m
+000003a0: 616e 7561 6c6c 7920 7365 6c65 6374 206e  anually select n
+000003b0: 756d 6265 7220 6f66 2063 6f72 6573 2074  umber of cores t
+000003c0: 6f20 7573 652e 2052 6563 6f6d 6d65 6e64  o use. Recommend
+000003d0: 6564 3a20 276d 6178 2729 0572 0100 0000  ed: 'max').r....
+000003e0: 7206 0000 00da 074f 7074 696f 6e73 da07  r......Options..
+000003f0: 7361 7665 5f61 7372 0800 0000 da0b 6261  save_asr......ba
+00000400: 7365 5f66 6f6c 6465 72da 0545 6e74 7279  se_folder..Entry
+00000410: da00 7a14 4261 7365 2066 6f6c 6465 7220  ..z.Base folder 
+00000420: 6c6f 6361 7469 6f6e 7a9e 4569 7468 6572  locationz.Either
+00000430: 2074 6865 2061 6273 6f6c 7574 6520 6c6f   the absolute lo
+00000440: 6361 7469 6f6e 206f 6620 7468 6520 666f  cation of the fo
+00000450: 6c64 6572 2063 6f6e 7461 696e 696e 6720  lder containing 
+00000460: 7468 6520 7375 626a 6563 7473 206f 7220  the subjects or 
+00000470: 626c 616e 6b2c 2069 6620 626c 616e 6b20  blank, if blank 
+00000480: 7468 656e 2061 2062 726f 7773 6572 2077  then a browser w
+00000490: 696e 646f 7720 7769 6c6c 2061 6c6c 6f77  indow will allow
+000004a0: 2079 6f75 2074 6f20 7365 6172 6368 2066   you to search f
+000004b0: 6f72 2074 6865 2066 696c 6573 2061 7420  or the files at 
+000004c0: 7275 6e74 696d 652e 2905 7201 0000 0072  runtime.).r....r
+000004d0: 0600 0000 7215 0000 0072 0700 0000 7208  ....r....r....r.
+000004e0: 0000 00da 1169 6e70 7574 5f66 6f6c 6465  .....input_folde
+000004f0: 725f 6e61 6d65 da04 6675 6e63 7a4c 466f  r_name..funczLFo
+00000500: 6c64 6572 2066 6f75 6e64 2069 6e20 6561  lder found in ea
+00000510: 6368 2073 7562 6a65 6374 7320 6469 7265  ch subjects dire
+00000520: 6374 6f72 7920 636f 6e74 6169 6e69 6e67  ctory containing
+00000530: 2074 6865 2066 696c 6573 2074 6f20 6265   the files to be
+00000540: 2061 6e61 6c79 7365 642e 2904 7201 0000   analysed.).r...
+00000550: 0072 0600 0000 7215 0000 0072 0800 0000  .r....r....r....
+00000560: da12 6f75 7470 7574 5f66 6f6c 6465 725f  ..output_folder_
+00000570: 6e61 6d65 da07 4445 4641 554c 547a 8044  name..DEFAULTz.D
+00000580: 6972 6563 746f 7279 2074 6f20 7361 7665  irectory to save
+00000590: 206f 7574 7075 742e 2049 6620 7365 7420   output. If set 
+000005a0: 746f 2044 4546 4155 4c54 2c20 7468 6520  to DEFAULT, the 
+000005b0: 6465 6661 756c 7420 6e61 6d65 2066 6f72  default name for
+000005c0: 2074 6865 2073 7461 7469 7374 6963 616c   the statistical
+000005d0: 206d 6170 2063 7265 6174 6564 2077 696c   map created wil
+000005e0: 6c20 6265 2075 7365 642e 2052 6563 6f6d  l be used. Recom
+000005f0: 6d65 6e64 6564 3a20 4445 4641 554c 547a  mended: DEFAULTz
+00000600: 1348 6967 6820 7061 7373 2066 696c 7465  .High pass filte
+00000610: 7269 6e67 5a0f 7465 6d70 6f72 616c 5f66  ringZ.temporal_f
+00000620: 696c 7465 727a 5674 7275 6520 6f72 2066  ilterzVtrue or f
+00000630: 616c 7365 2e20 5573 6520 6120 6869 6768  alse. Use a high
+00000640: 2070 6173 7320 6669 6c74 6572 2074 6f20   pass filter to 
+00000650: 7265 6d6f 7665 206c 6f77 2066 7265 7175  remove low frequ
+00000660: 656e 6379 2064 7269 6674 2e20 5265 636f  ency drift. Reco
+00000670: 6d6d 656e 6465 643a 2074 7275 655a 1668  mmended: trueZ.h
+00000680: 6967 6870 6173 735f 6669 6c74 6572 5f63  ighpass_filter_c
+00000690: 7574 6f66 6667 7b14 ae47 e17a 843f 7a25  utoffg{..G.z.?z%
+000006a0: 4869 6768 7061 7373 2066 696c 7465 7220  Highpass filter 
+000006b0: 6375 746f 6666 2066 7265 7175 656e 6379  cutoff frequency
+000006c0: 2028 487a 297a 7048 6967 6870 6173 7320   (Hz)zpHighpass 
+000006d0: 6669 6c74 6572 2063 7574 6f66 6620 6672  filter cutoff fr
+000006e0: 6571 7565 6e63 7920 636f 6e76 6572 7465  equency converte
+000006f0: 6420 696e 746f 2073 6967 6d61 2069 6e20  d into sigma in 
+00000700: 7365 636f 6e64 7320 7573 696e 6720 7468  seconds using th
+00000710: 6520 666f 726d 756c 6120 312f 2832 2a66  e formula 1/(2*f
+00000720: 2a54 5229 2e20 5265 636f 6d6d 656e 6465  *TR). Recommende
+00000730: 643a 2030 2e30 317a 114d 6f74 696f 6e20  d: 0.01z.Motion 
+00000740: 636f 7272 6563 7469 6f6e 5a16 7265 6d6f  correctionZ.remo
+00000750: 7665 5f6d 6f74 696f 6e5f 6f75 746c 6965  ve_motion_outlie
+00000760: 7273 7a7e 7472 7565 206f 7220 6661 6c73  rsz~true or fals
+00000770: 652e 2055 7365 2066 736c 5f6d 6f74 696f  e. Use fsl_motio
+00000780: 6e5f 6f75 746c 6965 7273 2074 6f20 7265  n_outliers to re
+00000790: 6d6f 7665 206d 6f74 696f 6e20 6f75 746c  move motion outl
+000007a0: 6965 7273 2875 7365 7320 6465 6661 756c  iers(uses defaul
+000007b0: 7420 6673 6c5f 6d6f 7469 6f6e 5f6f 7574  t fsl_motion_out
+000007c0: 6c69 6572 7320 7365 7474 696e 6773 292e  liers settings).
+000007d0: 2052 6563 6f6d 6d65 6e64 6564 3a20 7472   Recommended: tr
+000007e0: 7565 5a11 6d6f 7469 6f6e 5f63 6f72 7265  ueZ.motion_corre
+000007f0: 6374 696f 6e7a 6774 7275 6520 6f72 2066  ctionzgtrue or f
+00000800: 616c 7365 2e20 5573 6520 4d43 464c 4952  alse. Use MCFLIR
+00000810: 5420 746f 206d 6f74 696f 6e20 636f 7272  T to motion corr
+00000820: 6563 7420 766f 6c75 6d65 7320 2875 7365  ect volumes (use
+00000830: 7320 6465 6661 756c 7420 4d43 464c 4952  s default MCFLIR
+00000840: 5420 7365 7474 696e 6773 292e 2052 6563  T settings). Rec
+00000850: 6f6d 6d65 6e64 6564 3a20 7472 7565 7a11  ommended: truez.
+00000860: 5370 6174 6961 6c20 736d 6f6f 7468 696e  Spatial smoothin
+00000870: 675a 1173 7061 7469 616c 5f73 6d6f 6f74  gZ.spatial_smoot
+00000880: 6869 6e67 da05 6661 6c73 657a 3e74 7275  hing..falsez>tru
+00000890: 6520 6f72 2066 616c 7365 2e20 5573 6573  e or false. Uses
+000008a0: 2053 5553 414e 2074 6f20 7370 6174 6961   SUSAN to spatia
+000008b0: 6c20 736d 6f6f 7468 2e20 5265 636f 6d6d  l smooth. Recomm
+000008c0: 656e 6465 643a 2074 7275 65da 0e73 6d6f  ended: true..smo
+000008d0: 6f74 6869 6e67 5f66 7768 6d67 0000 0000  othing_fwhmg....
+000008e0: 0000 2040 7a1b 5370 6174 6961 6c20 736d  .. @z.Spatial sm
+000008f0: 6f6f 7468 696e 6720 6677 686d 2028 6d6d  oothing fwhm (mm
+00000900: 297a 4f66 7768 6d20 6f66 2073 6d6f 6f74  )zOfwhm of smoot
+00000910: 6869 6e67 2c20 696e 206d 6d2c 2067 6574  hing, in mm, get
+00000920: 7320 636f 6e76 6572 7465 6420 7573 696e  s converted usin
+00000930: 6720 7371 7274 2838 2a6c 6f67 2832 2929  g sqrt(8*log(2))
+00000940: 2e20 5265 636f 6d6d 656e 6465 643a 2038  . Recommended: 8
+00000950: 2e30 5a1e 736d 6f6f 7468 696e 675f 6272  .0Z.smoothing_br
+00000960: 6967 6874 6e65 7373 5f74 6872 6573 686f  ightness_thresho
+00000970: 6c64 6700 0000 0000 409f 407a 2653 7061  ldg.....@.@z&Spa
+00000980: 7469 616c 2073 6d6f 6f74 6869 6e67 2062  tial smoothing b
+00000990: 7269 6768 746e 6573 7320 7468 7265 7368  rightness thresh
+000009a0: 6f6c 647a 6753 686f 756c 6420 6265 2067  oldzgShould be g
+000009b0: 7265 6174 6572 2074 6861 6e20 6e6f 6973  reater than nois
+000009c0: 6520 6c65 7665 6c20 616e 6420 6c65 7373  e level and less
+000009d0: 2074 6861 6e20 636f 6e74 7261 7374 206f   than contrast o
+000009e0: 6620 6564 6765 7320 746f 2062 6520 7072  f edges to be pr
+000009f0: 6573 6572 7665 642e 2052 6563 6f6d 6d65  eserved. Recomme
+00000a00: 6e64 6564 3a20 3230 3030 2e30 6132 0100  nded: 2000.0a2..
+00000a10: 0074 7275 6520 6f72 2066 616c 7365 2e20  .true or false. 
+00000a20: 436f 7272 6563 7469 6f6e 2066 6163 746f  Correction facto
+00000a30: 7220 6f66 2030 2e37 2061 7070 6c69 6564  r of 0.7 applied
+00000a40: 2077 6865 6e20 7275 6e6e 696e 6720 6953   when running iS
+00000a50: 4e52 2063 616c 6375 6c61 7469 6f6e 732c  NR calculations,
+00000a60: 2074 6f20 636f 7272 6563 7420 666f 7220   to correct for 
+00000a70: 5261 796c 6569 6768 2064 6973 7472 6962  Rayleigh distrib
+00000a80: 7574 6564 206e 6f69 7365 2077 6865 6e20  uted noise when 
+00000a90: 7573 696e 6720 6d61 676e 6974 7564 6520  using magnitude 
+00000aa0: 7673 2063 6f6d 706c 6578 2069 6d61 6765  vs complex image
+00000ab0: 732e 200a 5265 6665 7265 6e63 653a 2043  s. .Reference: C
+00000ac0: 6f6e 7374 616e 7469 6e69 6465 732c 2043  onstantinides, C
+00000ad0: 2e20 442e 2c20 4174 616c 6172 2c20 452e  . D., Atalar, E.
+00000ae0: 2c20 2620 4d63 5665 6967 682c 2045 2e20  , & McVeigh, E. 
+00000af0: 522e 2028 3139 3937 292e 2053 6967 6e61  R. (1997). Signa
+00000b00: 6c2d 746f 2d4e 6f69 7365 204d 6561 7375  l-to-Noise Measu
+00000b10: 7265 6d65 6e74 7320 696e 204d 6167 6e69  rements in Magni
+00000b20: 7475 6465 2049 6d61 6765 7320 6672 6f6d  tude Images from
+00000b30: 204e 4d52 2050 6861 7365 6420 4172 7261   NMR Phased Arra
+00000b40: 7973 2e7a 244e 6f69 7365 2076 6f6c 756d  ys.z$Noise volum
+00000b50: 6520 696e 636c 7564 6564 2069 6e20 7469  e included in ti
+00000b60: 6d65 2073 6572 6965 7361 2002 0000 7472  me seriesa ...tr
+00000b70: 7565 206f 7220 6661 6c73 652e 2053 656c  ue or false. Sel
+00000b80: 6563 7420 7472 7565 2069 6620 6120 6e6f  ect true if a no
+00000b90: 6973 6520 766f 6c75 6d65 2068 6173 2062  ise volume has b
+00000ba0: 6565 6e20 636f 6c6c 6563 7465 6420 6173  een collected as
+00000bb0: 2070 6172 7420 6f66 2074 6865 2066 4d52   part of the fMR
+00000bc0: 4920 7469 6d65 2073 6572 6965 732e 0a49  I time series..I
+00000bd0: 6620 7472 7565 2c20 7468 6520 6e6f 6973  f true, the nois
+00000be0: 6520 766f 6c75 6d65 2069 6e20 7468 6520  e volume in the 
+00000bf0: 7469 6d65 2073 6572 6965 7320 7769 6c6c  time series will
+00000c00: 2062 6520 7365 7061 7261 7465 6420 6672   be separated fr
+00000c10: 6f6d 2074 6865 2066 756e 6374 696f 6e61  om the functiona
+00000c20: 6c20 766f 6c75 6d65 7320 616e 6420 7769  l volumes and wi
+00000c30: 6c6c 2062 6520 706c 6163 6564 2069 6e74  ll be placed int
+00000c40: 6f20 7468 6520 666f 6c64 6572 2022 6e6f  o the folder "no
+00000c50: 6973 655f 766f 6c75 6d65 222c 2061 6e64  ise_volume", and
+00000c60: 2074 6865 2066 756e 6374 696f 6e61 6c20   the functional 
+00000c70: 766f 6c75 6d65 7320 7769 6c6c 2062 6520  volumes will be 
+00000c80: 706c 6163 6564 2069 6e74 6f20 7468 6520  placed into the 
+00000c90: 2266 756e 635f 766f 6c75 6d65 7322 2066  "func_volumes" f
+00000ca0: 6f6c 6465 722e 2049 6620 226e 6f69 7365  older. If "noise
+00000cb0: 2076 6f6c 756d 6522 2069 7320 7472 7565   volume" is true
+00000cc0: 2061 6e64 2022 6e6f 6973 6520 7661 6c75   and "noise valu
+00000cd0: 6522 2069 7320 6e6f 7420 6e6f 6e65 2c20  e" is not none, 
+00000ce0: 7468 6520 6e6f 6973 6520 766f 6c75 6d65  the noise volume
+00000cf0: 2077 696c 6c20 6265 2075 7365 6420 696e   will be used in
+00000d00: 2069 6d61 6765 2053 4e52 2063 616c 6375   image SNR calcu
+00000d10: 6c61 7469 6f6e 2072 6174 6865 7220 7468  lation rather th
+00000d20: 616e 2074 6865 2075 7365 7220 6465 6669  an the user defi
+00000d30: 6e65 6420 6e6f 6973 6520 7661 6c75 652e  ned noise value.
+00000d40: 0a4e 4f54 453a 2055 7365 2074 6865 2022  .NOTE: Use the "
+00000d50: 7365 7061 7261 7465 206e 6f69 7365 2076  separate noise v
+00000d60: 6f6c 756d 6522 2075 7469 6c69 7479 2062  olume" utility b
+00000d70: 6566 6f72 6520 6372 6561 7469 6e67 2069  efore creating i
+00000d80: 6d61 6765 2053 4e52 206d 6170 732e 7a25  mage SNR maps.z%
+00000d90: 5573 6520 6f6e 6c79 206e 6f6e 7a65 726f  Use only nonzero
+00000da0: 2076 6f78 656c 7320 666f 7220 6953 4e52   voxels for iSNR
+00000db0: 2063 616c 637a 0e74 7275 6520 6f72 2066   calcz.true or f
+00000dc0: 616c 7365 2eda 0642 7574 746f 6eda 1163  alse...Button..c
+00000dd0: 7265 6174 655f 6e6f 6973 655f 6669 6c65  reate_noise_file
+00000de0: 7a16 4372 6561 7465 206e 6f69 7365 5661  z.Create noiseVa
+00000df0: 6c75 6573 2e63 7376 4661 f903 0000 4372  lues.csvFa....Cr
+00000e00: 6561 7465 2061 206e 6f69 7365 5661 6c75  eate a noiseValu
+00000e10: 6573 2e63 7376 2066 696c 6520 746f 2064  es.csv file to d
+00000e20: 6574 6572 6d69 6e65 2077 6861 7420 7468  etermine what th
+00000e30: 6520 7374 616e 6461 7264 2064 6576 6961  e standard devia
+00000e40: 7469 6f6e 6f66 2074 6865 2047 6175 7373  tionof the Gauss
+00000e50: 6961 6e20 7368 6f75 6c64 2062 6520 7768  ian should be wh
+00000e60: 656e 2061 6464 696e 6720 6e6f 6973 6520  en adding noise 
+00000e70: 746f 2065 6163 6820 7061 7274 6963 6970  to each particip
+00000e80: 616e 7427 7320 6461 7461 2028 7468 6520  ant's data (the 
+00000e90: 6469 7374 7269 6275 7469 6f6e 2077 696c  distribution wil
+00000ea0: 6c20 6861 7665 2061 206d 6561 6e20 6f66  l have a mean of
+00000eb0: 2030 292e 5468 6973 2077 696c 6c20 6e6f   0).This will no
+00000ec0: 7420 6f76 6572 7772 6974 6520 7468 6520  t overwrite the 
+00000ed0: 6f72 6967 696e 616c 2066 696c 6573 2e20  original files. 
+00000ee0: 5265 636f 6d6d 656e 6465 643a 2054 6865  Recommended: The
+00000ef0: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00000f00: 696f 6e20 6f76 6572 2074 696d 6520 666f  ion over time fo
+00000f10: 756e 6420 696e 2074 6865 2064 6174 6173  und in the datas
+00000f20: 6574 2e0a 4e4f 5445 3a20 4361 6e20 6265  et..NOTE: Can be
+00000f30: 2075 7365 6420 746f 2073 6565 2068 6f77   used to see how
+00000f40: 2061 6464 6974 696f 6e61 6c20 6e6f 6973   additional nois
+00000f50: 6520 6166 6665 6374 7320 616e 616c 7973  e affects analys
+00000f60: 6973 2e20 546f 2063 616c 6375 6c61 7465  is. To calculate
+00000f70: 2074 6865 206e 6f69 7365 206c 6576 656c   the noise level
+00000f80: 2066 6f72 2065 6163 6820 7061 7274 6963   for each partic
+00000f90: 6970 616e 742c 2063 7265 6174 6520 7453  ipant, create tS
+00000fa0: 4e52 206d 6170 7320 7769 7468 2074 6865  NR maps with the
+00000fb0: 2066 5241 5420 616e 6420 7275 6e20 7468   fRAT and run th
+00000fc0: 6520 6675 6c6c 2061 6e61 6c79 7369 7320  e full analysis 
+00000fd0: 7573 696e 6720 7468 6520 7453 7464 2066  using the tStd f
+00000fe0: 696c 6573 2e20 5468 6520 6d65 616e 2076  iles. The mean v
+00000ff0: 616c 7565 7320 6f66 2074 6869 7320 616e  alues of this an
+00001000: 616c 7973 6973 2069 6e20 6561 6368 2070  alysis in each p
+00001010: 6172 7469 6369 7061 6e74 7320 7375 6266  articipants subf
+00001020: 6f6c 6465 722c 2077 696c 6c20 7468 656e  older, will then
+00001030: 2073 686f 7720 796f 7520 7468 6520 6176   show you the av
+00001040: 6572 6167 6520 6e6f 6973 6520 666f 7220  erage noise for 
+00001050: 6561 6368 2072 6567 696f 6e20 666f 7220  each region for 
+00001060: 6561 6368 2070 6172 7469 6369 7061 6e74  each participant
+00001070: 2e0a 0a54 6869 7320 6669 6c65 2063 616e  ...This file can
+00001080: 2061 6c73 6f20 6265 2075 7365 6420 746f   also be used to
+00001090: 206d 616e 7561 6c6c 7920 7365 7420 6120   manually set a 
+000010a0: 6e6f 6973 6520 7661 6c75 6520 666f 7220  noise value for 
+000010b0: 6561 6368 2070 6172 7469 6369 7061 6e74  each participant
+000010c0: 2066 6f72 2075 7365 2069 6e20 6953 4e52   for use in iSNR
+000010d0: 2063 616c 6375 6c61 7469 6f6e 2e20 5468   calculation. Th
+000010e0: 6973 206e 6f69 7365 2076 616c 7565 2063  is noise value c
+000010f0: 616e 2062 6520 6361 6c63 756c 6174 6564  an be calculated
+00001100: 2061 7320 7468 6520 7374 616e 6461 7264   as the standard
+00001110: 2064 6576 6961 7469 6f6e 206f 6620 766f   deviation of vo
+00001120: 7865 6c20 7661 6c75 6573 206f 7574 7369  xel values outsi
+00001130: 6465 206f 6620 7468 6520 6272 6169 6e2e  de of the brain.
+00001140: 2049 6620 224e 6f69 7365 2076 6f6c 756d   If "Noise volum
+00001150: 6520 696e 636c 7564 6564 2069 6e20 7469  e included in ti
+00001160: 6d65 2073 6572 6965 7322 2069 7320 7365  me series" is se
+00001170: 7420 746f 2074 7275 652c 2073 7461 6e64  t to true, stand
+00001180: 6172 6420 6465 7669 6174 696f 6e20 6f66  ard deviation of
+00001190: 206e 6f69 7365 2077 696c 6c20 6265 2063   noise will be c
+000011a0: 616c 6375 6c61 7465 6420 7573 696e 6720  alculated using 
+000011b0: 7468 6520 6e6f 6973 6520 766f 6c75 6d65  the noise volume
+000011c0: 2c20 6576 656e 2069 6620 6120 6e6f 6973  , even if a nois
+000011d0: 6520 7661 6c75 6520 6861 7320 6265 656e  e value has been
+000011e0: 2070 726f 7669 6465 6420 696e 2074 6869   provided in thi
+000011f0: 7320 6669 6c65 2e29 0572 0100 0000 da07  s file.).r......
+00001200: 436f 6d6d 616e 64da 0454 6578 747a 0950  Command..Textz.P
+00001210: 6173 7320 7365 6c66 7208 0000 0072 1200  ass selfr....r..
+00001220: 0000 da04 6c69 7374 7a13 4e6f 6973 6520  ....listz.Noise 
+00001230: 6d75 6c74 6970 6c69 6572 2873 297a f950  multiplier(s)z.P
+00001240: 726f 7669 6465 2061 2063 6f6d 6d61 2d73  rovide a comma-s
+00001250: 6570 6172 6174 6564 206c 6973 7420 6f66  eparated list of
+00001260: 206d 756c 7469 706c 6965 7273 2c20 652e   multipliers, e.
+00001270: 672e 2027 312c 2035 272e 2041 2073 6570  g. '1, 5'. A sep
+00001280: 6172 6174 6520 6669 6c65 2077 696c 6c20  arate file will 
+00001290: 6265 2070 726f 6475 6365 6420 666f 7220  be produced for 
+000012a0: 6561 6368 206d 756c 7469 706c 6965 722e  each multiplier.
+000012b0: 0a4e 4f54 453a 2041 6464 6564 2068 6173  .NOTE: Added has
+000012c0: 2061 2067 6175 7373 6961 6e20 6469 7374   a gaussian dist
+000012d0: 7269 6275 7469 6f6e 2c20 7769 7468 2061  ribution, with a
+000012e0: 206d 6561 6e20 6f66 2030 2061 6e64 2061   mean of 0 and a
+000012f0: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00001300: 696f 6e20 6f66 2074 6865 206e 6f69 7365  ion of the noise
+00001310: 206c 6576 656c 206f 6620 6561 6368 2070   level of each p
+00001320: 6172 7469 6369 7061 6e74 202a 206d 756c  articipant * mul
+00001330: 7469 706c 6965 722e 7a14 4d6f 7469 6f6e  tiplier.z.Motion
+00001340: 206d 756c 7469 706c 6965 7228 7329 6111   multiplier(s)a.
+00001350: 0100 0050 726f 7669 6465 2061 2063 6f6d  ...Provide a com
+00001360: 6d61 2d73 6570 6172 6174 6564 206c 6973  ma-separated lis
+00001370: 7420 6f66 206d 756c 7469 706c 6965 7273  t of multipliers
+00001380: 2c20 652e 672e 2027 312c 2035 272e 2041  , e.g. '1, 5'. A
+00001390: 2073 6570 6172 6174 6520 6669 6c65 2077   separate file w
+000013a0: 696c 6c20 6265 2070 726f 6475 6365 6420  ill be produced 
+000013b0: 666f 7220 6561 6368 206d 756c 7469 706c  for each multipl
+000013c0: 6965 722e 0a4e 4f54 453a 2041 6464 6564  ier..NOTE: Added
+000013d0: 206d 6f74 696f 6e20 6861 7320 6120 6761   motion has a ga
+000013e0: 7573 7369 616e 2064 6973 7472 6962 7574  ussian distribut
+000013f0: 696f 6e2c 2077 6974 6820 6120 6d65 616e  ion, with a mean
+00001400: 206f 6620 3020 616e 6420 6120 7374 616e   of 0 and a stan
+00001410: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
+00001420: 6620 7468 6520 6176 6572 6167 6520 726f  f the average ro
+00001430: 7461 7469 6f6e 2f74 7261 6e73 6c61 7469  tation/translati
+00001440: 6f6e 206f 6620 6561 6368 2070 6172 7469  on of each parti
+00001450: 6369 7061 6e74 202a 206d 756c 7469 706c  cipant * multipl
+00001460: 6965 722e 2908 7a15 496d 6167 6520 534e  ier.).z.Image SN
+00001470: 5220 6361 6c63 756c 6174 696f 6e5a 146d  R calculationZ.m
+00001480: 6167 6e69 7475 6465 5f63 6f72 7265 6374  agnitude_correct
+00001490: 696f 6e5a 0c6e 6f69 7365 5f76 6f6c 756d  ionZ.noise_volum
+000014a0: 655a 2069 534e 525f 7374 645f 7573 655f  eZ iSNR_std_use_
+000014b0: 6f6e 6c79 5f6e 6f6e 7a65 726f 5f76 6f78  only_nonzero_vox
+000014c0: 656c 737a 1241 6464 2047 6175 7373 6961  elsz.Add Gaussia
+000014d0: 6e20 6e6f 6973 655a 1763 7265 6174 655f  n noiseZ.create_
+000014e0: 6e6f 6973 655f 6c65 7665 6c5f 6669 6c65  noise_level_file
+000014f0: 5a11 6e6f 6973 655f 6d75 6c74 6970 6c69  Z.noise_multipli
+00001500: 6572 735a 126d 6f74 696f 6e5f 6d75 6c74  ersZ.motion_mult
+00001510: 6970 6c69 6572 734e 2901 da10 5374 6174  ipliersN)...Stat
+00001520: 6973 7469 6361 6c5f 6d61 7073 a900 7225  istical_maps..r%
+00001530: 0000 0072 2500 0000 fa5f 2f55 7365 7273  ...r%...._/Users
+00001540: 2f6c 7078 6568 3130 2f44 6f63 756d 656e  /lpxeh10/Documen
+00001550: 7473 2f52 6570 6f73 6974 6f72 6965 732f  ts/Repositories/
+00001560: 664d 5249 5f52 4f49 5f61 6e61 6c79 7369  fMRI_ROI_analysi
+00001570: 735f 746f 6f6c 2f66 5241 542f 7574 696c  s_tool/fRAT/util
+00001580: 732f 7374 6174 6d61 705f 636f 6e66 6967  s/statmap_config
+00001590: 5f73 6574 7570 2e70 79da 083c 6d6f 6475  _setup.py..<modu
+000015a0: 6c65 3e01 0000 0073 b200 0000 0200 0801  le>....s........
+000015b0: 02ff 0803 0201 04ff 02fd 0606 0201 04ff  ................
+000015c0: 02fa 0c0b 0201 0201 04fe 02f5 0810 0201  ................
+000015d0: 0201 04fe 02f0 0816 0201 04ff 02ea 081a  ................
+000015e0: 0201 04ff 02e6 081f 02e1 0621 0201 04ff  ...........!....
+000015f0: 02df 0625 0201 0201 04fe 02db 082a 02d6  ...%.........*..
+00001600: 062c 0201 04ff 02d4 0630 0201 04ff 02d0  .,.......0......
+00001610: 0834 02cc 0636 0201 04ff 02ca 0639 0201  .4...6.......9..
+00001620: 0201 04fe 02c7 063d 0201 0201 04fe 02c3  .......=........
+00001630: 0642 0402 0201 04ff 0607 0201 04ff 040a  .B..............
+00001640: 0201 0201 04fe 0604 0602 0201 0201 04fe  ................
+00001650: 0815 0201 04ff 0806 0201 04ff 0c8a       ..............
```

### Comparing `frat_brain-1.5.0/fRAT/utils/__pycache__/utils.cpython-310.pyc` & `frat_brain-1.5.1/fRAT/utils/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May  4 16:20:25 2023 UTC, .py size: 19156 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 49db 5364 d44a 0000  o.......I.Sd.J..
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 d44a 0000  o.........[d.J..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
```

### Comparing `frat_brain-1.5.0/fRAT/utils/analysis.py` & `frat_brain-1.5.1/fRAT/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/bootstrap.css` & `frat_brain-1.5.1/fRAT/utils/bootstrap.css`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/dash_report.py` & `frat_brain-1.5.1/fRAT/utils/dash_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/directory_comparison.py` & `frat_brain-1.5.1/fRAT/utils/directory_comparison.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/fRAT_config_setup.py` & `frat_brain-1.5.1/fRAT/utils/fRAT_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/figures.py` & `frat_brain-1.5.1/fRAT/utils/figures.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/html_report.py` & `frat_brain-1.5.1/fRAT/utils/html_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/printResults.py` & `frat_brain-1.5.1/fRAT/utils/printResults.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/statistics.py` & `frat_brain-1.5.1/fRAT/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/statmap.py` & `frat_brain-1.5.1/fRAT/utils/statmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,25 +140,25 @@
 def create_statmaps(func, file, no_ext_file, noise_file, output_folder, participant):
     if func == 'Image SNR':
         imageSNR_calc(file, noise_file, no_ext_file, output_folder, participant)
     elif func == 'Temporal SNR':
         temporalSNR_calc(file, no_ext_file, output_folder)
 
 
-def prepare_statmap_files(file, no_ext_file, output_folder, participant):
+def prepare_statmap_files(func, file, no_ext_file, output_folder, participant):
     noise_file = None
 
     redundant_files = []
     outliers = []
 
     # Save original copy of file which may be overwritten later, however allows this folder to always be used
     data, header = Utils.load_brain(file)
     Utils.save_brain(data, '', no_ext_file, f'{participant}/{config.input_folder_name}_preprocessed', header)
 
-    if config.noise_volume:
+    if func == 'Image SNR' and config.noise_volume:
         file = f'{participant}/func_volumes/{no_ext_file}.nii.gz'
         noise_file = f'{participant}/noise_volume/{no_ext_file}_noise_volume.nii.gz'
 
         if not os.path.exists(file) or not os.path.exists(noise_file):
             raise FileNotFoundError('Could not find separate noise and functional volumes. '
                                     'Run the "separate noise volumes" utility to create these files.')
 
@@ -222,15 +222,15 @@
     no_ext_file = Utils.strip_ext(file)
     file = f"{participant}/{file_location}/{file}"
     output_folder = f'{participant}/{output_folder}'
 
     if config.verbose:
         print(f'        Analysing file: {no_ext_file}')
 
-    file, noise_file, redundant_files, outliers = prepare_statmap_files(file, no_ext_file, output_folder, participant)
+    file, noise_file, redundant_files, outliers = prepare_statmap_files(func, file, no_ext_file, output_folder, participant)
     create_statmaps(func, file, no_ext_file, noise_file, output_folder, participant)
 
     delete_files(redundant_files)
 
     return outliers
```

### Comparing `frat_brain-1.5.0/fRAT/utils/statmap_config_setup.py` & `frat_brain-1.5.1/fRAT/utils/statmap_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/fRAT/utils/utils.py` & `frat_brain-1.5.1/fRAT/utils/utils.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.0/pyproject.toml` & `frat_brain-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frat-brain"
-version = "1.5.0"
+version = "1.5.1"
 description = "Application for ROI fMRI data analysis."
 authors = ["Elliot Howley <elliohow@hotmail.com>"]
 readme = "README.md"
 homepage = "https://fmri-roi-analysis-tool.readthedocs.io/en/latest/"
 repository = "https://github.com/elliohow/fMRI_ROI_Analysis_Tool"
 packages = [{include = "fRAT"}]
```

### Comparing `frat_brain-1.5.0/setup.py` & `frat_brain-1.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,17 +108,17 @@
  'zope-interface==5.2.0']
 
 entry_points = \
 {'console_scripts': ['fRAT = fRAT.__main__:start_gui']}
 
 setup_kwargs = {
     'name': 'frat-brain',
-    'version': '1.5.0',
+    'version': '1.5.1',
     'description': 'Application for ROI fMRI data analysis.',
-    'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
+    'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Citation\n\n**When using fRAT, please include the following citation:**\n\nHowley, E., Francis, S., & Schluppeck, D. (2023). fRAT: an interactive, Python-based tool for region-of-interest summaries of functional imaging data. Journal of Open Source Software, 8(85), 5200. https://doi.org/10.21105/joss.05200\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
     'author': 'Elliot Howley',
     'author_email': 'elliohow@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fmri-roi-analysis-tool.readthedocs.io/en/latest/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `frat_brain-1.5.0/PKG-INFO` & `frat_brain-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frat-brain
-Version: 1.5.0
+Version: 1.5.1
 Summary: Application for ROI fMRI data analysis.
 Home-page: https://fmri-roi-analysis-tool.readthedocs.io/en/latest/
 Author: Elliot Howley
 Author-email: elliohow@hotmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -124,14 +124,20 @@
 
 [Home page](https://fmri-roi-analysis-tool.readthedocs.io)
 
 [Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)
 
 [ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)
 
+## Citation
+
+**When using fRAT, please include the following citation:**
+
+Howley, E., Francis, S., & Schluppeck, D. (2023). fRAT: an interactive, Python-based tool for region-of-interest summaries of functional imaging data. Journal of Open Source Software, 8(85), 5200. https://doi.org/10.21105/joss.05200
+
 ## Reporting bugs
 
 To report a bug or suggest a new feature, please go to [fRAT's Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).
 
 For other questions, issues or discussion please go to [fRAT's Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).
 
 ## Contributing to the project
```

