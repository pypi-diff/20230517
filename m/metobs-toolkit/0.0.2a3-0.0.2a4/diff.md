# Comparing `tmp/metobs_toolkit-0.0.2a3.tar.gz` & `tmp/metobs_toolkit-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metobs_toolkit-0.0.2a3.tar", max compression
+gzip compressed data, was "metobs_toolkit-0.0.2a4.tar", max compression
```

## Comparing `metobs_toolkit-0.0.2a3.tar` & `metobs_toolkit-0.0.2a4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a3/LICENSE
--rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.0.2a3/README.md
--rw-r--r--   0        0        0      222 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/custom_template.csv
--rw-r--r--   0        0        0      485 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/custom_template_Ian.csv
--rw-r--r--   0        0        0      295 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/vlindersmall_template.csv
--rw-r--r--   0        0        0      160 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/wow_template.csv
--rw-r--r--   0        0        0     1426 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/data_func.py
--rw-r--r--   0        0        0      825 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/errors.py
--rw-r--r--   0        0        0     4857 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/extra_windows.py
--rw-r--r--   0        0        0     3369 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/fig_window.ui
--rw-r--r--   0        0        0     2320 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/figuremodel.py
--rw-r--r--   0        0        0     2029 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/json_save_func.py
--rw-r--r--   0        0        0    10955 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/main.py
--rw-r--r--   0        0        0     1435 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/merge_overview.ui
--rw-r--r--   0        0        0     2367 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/pandasmodel.py
--rw-r--r--   0        0        0     2288 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/path_handler.py
--rw-r--r--   0        0        0      283 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/save_gui_vals.json
--rw-r--r--   0        0        0    46735 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/templ_build.ui
--rw-r--r--   0        0        0    11554 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/template_func.py
--rw-r--r--   0        0        0     7330 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/tlk_scripts.py
--rw-r--r--   0        0        0     2503 2023-05-12 10:11:37.762628 metobs_toolkit-0.0.2a3/metobs_toolkit/__init__.py
--rw-r--r--   0        0        0    19751 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a3/metobs_toolkit/analysis.py
--rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a3/metobs_toolkit/convertors.py
--rw-r--r--   0        0        0    12056 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a3/metobs_toolkit/data_import.py
--rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/db_templates.py
--rw-r--r--   0        0        0     1701 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/import_templates.py
--rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/template_defaults/default_template.csv
--rwxr-xr-x   0        0        0  9062298 2023-05-12 09:54:16.849478 metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_datafile.csv
--rw-r--r--   0        0        0     2306 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_metadatafile.csv
--rw-r--r--   0        0        0      931 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_templatefile.csv
--rw-r--r--   0        0        0    68582 2023-05-12 09:54:16.881478 metobs_toolkit-0.0.2a3/metobs_toolkit/dataset.py
--rw-r--r--   0        0        0    17115 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/dataset_settings_updater.py
--rw-r--r--   0        0        0    11623 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/df_helpers.py
--rw-r--r--   0        0        0    22073 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/gap.py
--rw-r--r--   0        0        0    15267 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/gap_filling.py
--rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/geometry_functions.py
--rw-r--r--   0        0        0      222 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/gui_launcher.py
--rw-r--r--   0        0        0    18129 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/landcover_functions.py
--rw-r--r--   0        0        0     7973 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/missingobs.py
--rw-r--r--   0        0        0     4723 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/modeldata.py
--rw-r--r--   0        0        0    20497 2023-05-12 09:54:16.877478 metobs_toolkit-0.0.2a3/metobs_toolkit/plotting_functions.py
--rw-r--r--   0        0        0     1847 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/printing.py
--rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/qc_checks.py
--rw-r--r--   0        0        0     4159 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/qc_statistics.py
--rw-r--r--   0        0        0    14146 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings.py
--rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/app_print_settings.json
--rw-r--r--   0        0        0      237 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/dataset_resolution_settings.json
--rw-r--r--   0        0        0     4509 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/default_formats_settings.py
--rw-r--r--   0        0        0     1831 2023-05-12 09:54:16.873478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gaps_and_missing_settings.py
--rw-r--r--   0        0        0     3880 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gee_settings.py
--rw-r--r--   0        0        0     2851 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/qc_settings.py
--rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/server_login.json
--rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
--rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
--rw-r--r--   0        0        0      916 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/station.py
--rw-r--r--   0        0        0     2441 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a3/metobs_toolkit/writing_files.py
--rw-r--r--   0        0        0      853 2023-05-12 10:11:37.682628 metobs_toolkit-0.0.2a3/pyproject.toml
--rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a4/LICENSE
+-rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.0.2a4/README.md
+-rw-r--r--   0        0        0      222 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/custom_template.csv
+-rw-r--r--   0        0        0      485 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/custom_template_Ian.csv
+-rw-r--r--   0        0        0      295 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/vlindersmall_template.csv
+-rw-r--r--   0        0        0      160 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/wow_template.csv
+-rw-r--r--   0        0        0     1426 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/data_func.py
+-rw-r--r--   0        0        0      825 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/errors.py
+-rw-r--r--   0        0        0     4857 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/extra_windows.py
+-rw-r--r--   0        0        0     3369 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/fig_window.ui
+-rw-r--r--   0        0        0     2323 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/figuremodel.py
+-rw-r--r--   0        0        0     2029 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/json_save_func.py
+-rw-r--r--   0        0        0    11180 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/main.py
+-rw-r--r--   0        0        0     1435 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/merge_overview.ui
+-rw-r--r--   0        0        0     2367 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/pandasmodel.py
+-rw-r--r--   0        0        0     2288 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/path_handler.py
+-rw-r--r--   0        0        0      283 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/save_gui_vals.json
+-rw-r--r--   0        0        0    46804 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/templ_build.ui
+-rw-r--r--   0        0        0    11554 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/template_func.py
+-rw-r--r--   0        0        0     7330 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/tlk_scripts.py
+-rw-r--r--   0        0        0     2503 2023-05-17 14:40:31.641025 metobs_toolkit-0.0.2a4/metobs_toolkit/__init__.py
+-rw-r--r--   0        0        0    19751 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a4/metobs_toolkit/analysis.py
+-rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a4/metobs_toolkit/convertors.py
+-rw-r--r--   0        0        0    12056 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a4/metobs_toolkit/data_import.py
+-rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/db_templates.py
+-rw-r--r--   0        0        0     1701 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/import_templates.py
+-rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/template_defaults/default_template.csv
+-rwxr-xr-x   0        0        0  9062298 2023-05-12 09:54:16.849478 metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_datafile.csv
+-rw-r--r--   0        0        0     2306 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_metadatafile.csv
+-rw-r--r--   0        0        0      931 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_templatefile.csv
+-rw-r--r--   0        0        0    83222 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/dataset.py
+-rw-r--r--   0        0        0    18352 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/dataset_settings_updater.py
+-rw-r--r--   0        0        0    13810 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/df_helpers.py
+-rw-r--r--   0        0        0    24294 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/gap.py
+-rw-r--r--   0        0        0    17104 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/gap_filling.py
+-rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/geometry_functions.py
+-rw-r--r--   0        0        0      222 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/gui_launcher.py
+-rw-r--r--   0        0        0    18380 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/landcover_functions.py
+-rw-r--r--   0        0        0     9081 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/missingobs.py
+-rw-r--r--   0        0        0     5078 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/modeldata.py
+-rw-r--r--   0        0        0    20732 2023-05-17 14:40:15.908854 metobs_toolkit-0.0.2a4/metobs_toolkit/plotting_functions.py
+-rw-r--r--   0        0        0     1847 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/printing.py
+-rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/qc_checks.py
+-rw-r--r--   0        0        0     3978 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/qc_statistics.py
+-rw-r--r--   0        0        0    14130 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/settings.py
+-rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/app_print_settings.json
+-rw-r--r--   0        0        0      225 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/dataset_resolution_settings.json
+-rw-r--r--   0        0        0     4505 2023-05-17 14:40:15.908854 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/default_formats_settings.py
+-rw-r--r--   0        0        0     1888 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gaps_and_missing_settings.py
+-rw-r--r--   0        0        0     3880 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gee_settings.py
+-rw-r--r--   0        0        0     2851 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/qc_settings.py
+-rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/server_login.json
+-rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
+-rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
+-rw-r--r--   0        0        0      916 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/station.py
+-rw-r--r--   0        0        0     2269 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a4/metobs_toolkit/writing_files.py
+-rw-r--r--   0        0        0      933 2023-05-17 14:40:31.537024 metobs_toolkit-0.0.2a4/pyproject.toml
+-rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a4/PKG-INFO
```

### Comparing `metobs_toolkit-0.0.2a3/LICENSE` & `metobs_toolkit-0.0.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/data_func.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/data_func.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/errors.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/errors.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/extra_windows.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/extra_windows.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/fig_window.ui` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/fig_window.ui`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/figuremodel.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/figuremodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on Thu Apr 27 12:41:38 2023
 
 @author: thoverga
 """
 
 import sys, os
 import matplotlib
-matplotlib.use('Qt5Agg')
+# matplotlib.use('Qt5Agg')
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib.figure import Figure
 
@@ -61,15 +61,15 @@
 
 
         self.axes = self.dataset.make_plot(stationnames=stationnames,
                                            obstype=obstype,
                                            colorby=colorby,
                                            starttime=None,
                                            endtime=None,
-                                           ax=self.axes,
+                                           _ax=self.axes,
                                            title=None,
                                            legend=False,
                                            show_outliers=show_outliers)
         print('figure is made')
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/json_save_func.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/json_save_func.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/main.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 # command: designer in terminal to open the desinger tool
 
 # DEBUG
 import sys
 sys.path.insert(0, '/home/thoverga/Documents/VLINDER_github/MetObs_toolkit/metobs_toolkit')
 import metobs_toolkit
-# END DEBUG
+
 
 import os, sys
 from pathlib import Path
+import matplotlib
 from PyQt5 import QtWidgets
 from PyQt5.QtWidgets import QDialog, QApplication, QFileDialog, QMainWindow
 from PyQt5.uic import loadUi
 
 import pandas as pd
 import pytz
 
@@ -288,16 +289,18 @@
 # =============================================================================
 # Testing
 # =============================================================================
 
 
     def make_figure(self):
         self.tswindow.set_dataset(self.dataset)
-
+        print(self.dataset)
+        print('tswindow set')
         self.tswindow.make_plot()
+        print('plot made')
         self.tswindow.show()
 
 
 #%%
 
 # =============================================================================
 # Main and protector
@@ -321,14 +324,15 @@
         pass
     sys.exit(app.exec_())
 
     return succesfull
 
 
 if __name__ == '__main__':
+    matplotlib.use('Qt5Agg') #in protector because server runners do not support this, when this module is imported from the __init__
     app=QApplication(sys.argv)
 
     widget = main()
     widget.show()
     sys.exit(app.exec_())
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/merge_overview.ui` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/merge_overview.ui`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/pandasmodel.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/path_handler.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/path_handler.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/templ_build.ui` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/templ_build.ui`

 * *Files 0% similar despite different names*

#### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/templ_build.ui` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/templ_build.ui`

```diff
@@ -19,15 +19,15 @@
           <x>-10</x>
           <y>0</y>
           <width>1281</width>
           <height>981</height>
         </rect>
       </property>
       <property name="currentIndex">
-        <number>0</number>
+        <number>1</number>
       </property>
       <widget class="QWidget" name="tab">
         <attribute name="title">
           <string>Mapping</string>
         </attribute>
         <widget class="QLabel" name="label_2">
           <property name="geometry">
@@ -1288,23 +1288,23 @@
           <property name="text">
             <string>Save</string>
           </property>
         </widget>
       </widget>
       <widget class="QWidget" name="tab_2">
         <attribute name="title">
-          <string>name of tab2</string>
+          <string>Import data</string>
         </attribute>
         <widget class="QComboBox" name="select_temp">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="geometry">
             <rect>
-              <x>10</x>
+              <x>20</x>
               <y>40</y>
               <width>111</width>
               <height>25</height>
             </rect>
           </property>
         </widget>
         <widget class="QLabel" name="label_29">
@@ -1418,15 +1418,15 @@
             <string>Toolkit status</string>
           </property>
         </widget>
         <widget class="QPushButton" name="make_dataset">
           <property name="geometry">
             <rect>
               <x>10</x>
-              <y>600</y>
+              <y>660</y>
               <width>171</width>
               <height>25</height>
             </rect>
           </property>
           <property name="text">
             <string>Make dataset</string>
           </property>
@@ -1552,18 +1552,18 @@
           <property name="checked">
             <bool>true</bool>
           </property>
         </widget>
         <widget class="QTextEdit" name="prompt">
           <property name="geometry">
             <rect>
-              <x>90</x>
+              <x>20</x>
               <y>460</y>
-              <width>911</width>
-              <height>121</height>
+              <width>981</width>
+              <height>191</height>
             </rect>
           </property>
         </widget>
         <widget class="Line" name="line_3">
           <property name="geometry">
             <rect>
               <x>10</x>
@@ -1900,15 +1900,15 @@
             <string>Max. decr. per hour</string>
           </property>
         </widget>
         <widget class="QPushButton" name="apply_qc">
           <property name="geometry">
             <rect>
               <x>210</x>
-              <y>600</y>
+              <y>660</y>
               <width>171</width>
               <height>25</height>
             </rect>
           </property>
           <property name="text">
             <string>Apply Qualty control</string>
           </property>
@@ -1952,38 +1952,41 @@
             <double>-50.000000000000000</double>
           </property>
         </widget>
         <widget class="QPushButton" name="show_dataset">
           <property name="geometry">
             <rect>
               <x>800</x>
-              <y>600</y>
+              <y>660</y>
               <width>161</width>
               <height>25</height>
             </rect>
           </property>
           <property name="text">
             <string>Show dataset</string>
           </property>
         </widget>
         <widget class="QPushButton" name="plot_dataset">
           <property name="geometry">
             <rect>
               <x>800</x>
-              <y>640</y>
+              <y>700</y>
               <width>161</width>
               <height>25</height>
             </rect>
           </property>
           <property name="text">
             <string>Plot dataset</string>
           </property>
         </widget>
       </widget>
       <widget class="QWidget" name="tab_3">
+        <property name="enabled">
+          <bool>false</bool>
+        </property>
         <attribute name="title">
           <string>Page</string>
         </attribute>
       </widget>
     </widget>
   </widget>
   <resources/>
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/template_func.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/template_func.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/tlk_scripts.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/tlk_scripts.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/__init__.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,9 +76,9 @@
 from metobs_toolkit.dataset_settings_updater import Dataset
 
 # =============================================================================
 # Version
 # =============================================================================
 
 # DO not change this manually!
-__version__ = "0.0.2a3"
+__version__ = "0.0.2a4"
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/analysis.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/analysis.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/convertors.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/convertors.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/data_import.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/data_import.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/db_templates.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/db_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/import_templates.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/import_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/template_defaults/default_template.csv` & `metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/template_defaults/default_template.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_datafile.csv` & `metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_datafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_metadatafile.csv` & `metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_metadatafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_templatefile.csv` & `metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_templatefile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/dataset.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 The class object for a Vlinder/mocca station
 @author: thoverga
 """
 
 import os
 import copy
 from datetime import datetime
-from pytz import all_timezones, common_timezones
+import pytz
 import logging
 import pandas as pd
 import numpy as np
 
 
 from metobs_toolkit.settings import Settings
 from metobs_toolkit.data_import import (
@@ -49,27 +49,36 @@
 
 from metobs_toolkit.qc_statistics import get_freq_statistics
 from metobs_toolkit.writing_files import write_dataset_to_csv
 
 from metobs_toolkit.missingobs import Missingob_collection
 
 from metobs_toolkit.gap import (
-    Gap_collection,
+    Gap,
+    remove_gaps_from_obs,
     missing_timestamp_and_gap_check,
+    get_gaps_indx_in_obs_space,
+    get_station_gaps,
+    apply_interpolate_gaps,
+    make_gapfill_df,
+    apply_debias_era5_gapfill,
+    gaps_to_df,
 )
 
 
 from metobs_toolkit.df_helpers import (
     multiindexdf_datetime_subsetting,
     remove_outliers_from_obs,
+    init_multiindex,
     init_multiindexdf,
     init_triple_multiindexdf,
     metadf_to_gdf,
     conv_applied_qc_to_df,
     get_freqency_series,
+    value_labeled_doubleidxdf_to_triple_idxdf,
 )
 
 from metobs_toolkit.analysis import Analysis
 from metobs_toolkit.modeldata import Modeldata
 
 from metobs_toolkit import observation_types
 
@@ -93,15 +102,15 @@
         # Dataset with 'good' observations
         self.df = pd.DataFrame()
 
         # Dataset with outlier observations
         self.outliersdf = init_triple_multiindexdf()
 
         self.missing_obs = None  # becomes a Missingob_collection after import
-        self.gaps = None  # becomes a gap_collection after import
+        self.gaps = None  # becomes a list of gaps
 
         self.gapfilldf = init_multiindexdf()
         self.missing_fill_df = init_multiindexdf()
 
         # Dataset with metadata (static)
         self.metadf = pd.DataFrame()
         # dataframe containing all information on the description and mapping
@@ -113,14 +122,36 @@
         self._applied_qc = pd.DataFrame(columns=["obstype", "checkname"])
         self._qc_checked_obstypes = []  # list with qc-checked obstypes
 
         self.settings = copy.deepcopy(Settings())
 
 
 
+    def __str__(self):
+        if self.df.empty:
+            return f"Empty instance of a Dataset."
+        add_info = ''
+        n_stations = self.df.index.get_level_values('name').unique().shape[0]
+        n_obs_tot = self.df.shape[0]
+        n_outl = self.outliersdf.shape[0]
+
+        if ((not self.metadf['lat'].isnull().all()) &
+            (not self.metadf['lon'].isnull().all())):
+            add_info += '     *Coordinates are available for all stations. \n'
+
+
+        return (f"Dataset instance containing: \n \
+    *{n_stations} stations \n \
+    *{n_obs_tot} observation records \n \
+    *{n_outl} records labeled as outliers \n \
+    *{len(self.gaps)} gaps \n \
+    *{self.missing_obs.series.shape[0]} missing observations \n" + add_info)
+
+    def __repr__(self):
+        return self.__str__()
 
 
     def show_settings(self):
         """
         A function that prints out all the settings, structured per thematic.
 
         Returns
@@ -164,15 +195,15 @@
         try:
             sta_outliers = self.outliersdf.xs(
                 stationname, level="name", drop_level=False
             )
         except KeyError:
             sta_outliers = init_multiindexdf()
 
-        sta_gaps = self.gaps.get_station_gaps(stationname)
+        sta_gaps = get_station_gaps(self.gaps, stationname)
         sta_missingobs = self.missing_obs.get_station_missingobs(stationname)
 
         try:
             sta_gapfill = self.gapfilldf.xs(stationname, level="name", drop_level=False)
         except KeyError:
             sta_gapfill = init_multiindexdf()
 
@@ -232,65 +263,83 @@
         obstype="temp",
         colorby="name",
         starttime=None,
         endtime=None,
         title=None,
         legend=True,
         show_outliers=True,
-        ax=None
+        show_filled = True,
+        _ax=None, #needed for GUI, not recommended use
     ):
         """
         This function creates a timeseries plot for the dataset. The variable observation type
         is plotted for all stationnames from a starttime to an endtime.
 
+        All styling attributes are extracted from the Settings.
 
-         All styling attributes are extracted from the Settings.
+        Parameters
+        ----------
 
-         Parameters
-         ----------
-         stationnames : list, optional
-             A list with stationnames to include in the timeseries. If None is given, all the stations are used, defaults to None.
-         obstype : string, optional
+        stationnames : list, optional
+            A list with stationnames to include in the timeseries. If None is given, all the stations are used, defaults to None.
+        obstype : string, optional
              Fieldname to visualise. This can be an observation or station
              attribute. The default is 'temp'.
-         colorby : 'label' or 'name', optional
+        colorby : 'label' or 'name', optional
              Indicate how colors should be assigned to the lines. 'label' will color the lines by their quality control label. 'name' will color by each station, defaults to 'name'.
-         starttime : datetime.datetime, optional
+        starttime : datetime.datetime, optional
              Specifiy the start datetime for the plot. If None is given it will use the start datetime of the dataset, defaults to None.
-         endtime : datetime.datetime, optional
+        endtime : datetime.datetime, optional
              Specifiy the end datetime for the plot. If None is given it will use the end datetime of the dataset, defaults to None.
-         title : string, optional
+        title : string, optional
              Title of the figure, if None a default title is generated. The default is None.
-         legend : bool, optional
+        legend : bool, optional
              I True, a legend is added to the plot. The default is True.
-         show_outliers : bool, optional
+        show_outliers : bool, optional
              If true the observations labeld as outliers will be included in the plot, defaults to True
+        show_filled : bool, optional
+             If true the filled values for gaps and missing observations will
+             be included in the plot, defaults to True
 
 
-         Returns
-         -------
-         axis : matplotlib.pyplot.axes
+        Returns
+        -------
+        axis : matplotlib.pyplot.axes
              The timeseries axes of the plot is returned.
 
         """
 
         logger.info(f"Make {obstype}-timeseries plot for {stationnames}")
 
         # combine all dataframes
         mergedf = self.combine_all_to_obsspace()
 
+        # subset to obstype
+        mergedf = mergedf.xs(obstype, level='obstype')
+
         # Subset on stationnames
         if not stationnames is None:
-            mergedf = mergedf.loc[
-                mergedf.index.get_level_values("name").isin(stationnames)
-            ]
+            mergedf = mergedf.reset_index()
+            mergedf = mergedf.loc[mergedf['name'].isin(stationnames)]
+            mergedf = mergedf.set_index(['name', 'datetime'])
+
 
         # Subset on start and endtime
         mergedf = multiindexdf_datetime_subsetting(mergedf, starttime, endtime)
 
+        # remove outliers if required
+        if not show_outliers:
+            outlier_labels = [var['outlier_flag'] for var in self.settings.qc['qc_checks_info'].values()]
+            mergedf = mergedf[~mergedf['label'].isin(outlier_labels)]
+
+        # remove filled values if required
+        if not show_filled:
+            fill_labels = ['gap fill', 'missing observation fill'] #toolkit representation labels
+            mergedf = mergedf[~mergedf['toolkit_representation'].isin(fill_labels)]
+
         # Get plot styling attributes
         if title is None:
             if stationnames is None:
                 if self._istype == "Dataset":
                     title = (
                         self.settings.app["display_name_mapper"][obstype]
                         + " for all stations. "
@@ -305,43 +354,26 @@
             else:
                 title = (
                     self.settings.app["display_name_mapper"][obstype]
                     + " for stations: "
                     + str(stationnames)
                 )
 
-        if (obstype + "_final_label" not in mergedf.columns) & (
-            (colorby == "label") | (show_outliers)
-        ):
-            # user whant outier information but no QC is applied on this obstype
-            print(
-                f" No quality control is applied on {obstype}! \
-                  No outlier information is available."
-            )
-            print(
-                'Colorby is set to "name" and show_outliers \
-                  is set to False.'
-            )
-            colorby = "name"
-            show_outliers = False
 
         # Make plot
         ax = timeseries_plot(
             mergedf=mergedf,
-            obstype=obstype,
             title=title,
             xlabel="Timestamp",
             ylabel=self.data_template[obstype]["orig_name"],
             colorby=colorby,
             show_legend=legend,
             show_outliers=show_outliers,
-            plot_settings=self.settings.app["plot_settings"],
-            gap_settings=self.settings.gap,
-            qc_info_settings=self.settings.qc["qc_checks_info"],
-            ax=ax,
+            settings = self.settings,
+            _ax = _ax
         )
 
         return ax
 
     def make_geo_plot(
         self,
         obstype="temp",
@@ -442,14 +474,18 @@
             End datetime of the model timeseries. If None, the last datetime of the dataset is used. The default is None.
 
         Returns
         -------
         Modl : metobs_toolkit.Modeldata
             The extracted modeldata for period and a set of stations.
 
+        NOTE
+        ------
+        Only 2mT extraction of ERA5 is implemented at the moment.
+
         """
 
         Modl = Modeldata(modelname)
 
         # Filters
         if startdt is None:
             startdt = self.df.index.get_level_values("datetime").min()
@@ -459,28 +495,347 @@
             if isinstance(stations, str):
                 metadf = self.metadf.loc[[stations]]
             if isinstance(stations, list):
                 metadf = self.metadf.iloc[self.metadf.index.isin(stations)]
         else:
             metadf = self.metadf
 
+        # Convert to UTC
+        startdt_utc = startdt.astimezone(pytz.utc)
+        enddt_utc = enddt.astimezone(pytz.utc)
+
         # fill modell with data
         if modelname == "ERA5_hourly":
-            Modl.get_ERA5_data(metadf, startdt, enddt)
+            Modl.get_ERA5_data(metadf, startdt_utc, enddt_utc)
 
             return Modl
         else:
             print(f"{modelname} for set_modeldata is not implemented yet")
             return None
 
+    def update_gaps_and_missing_from_outliers(self, obstype='temp', n_gapsize=None):
+        """
+        Interpret the outliers as missing observations. If there is a sequence
+        of these outliers for a station, larger than n_gapsize than this will
+        be interpreted as a gap.
+
+        The outliers are not removed.
+
+        Parameters
+        ----------
+        obstype : str, optional
+            Use the outliers on this observation type to update the gaps and
+            missing timestamps.The obstype should be an element of
+            metobs_toolkit.observation_types. The default is 'temp'.
+        n_gapsize : int, optional
+            The minimum number of consecutive missing observations to define
+            as a gap. If None, n_gapsize is taken from the settings defenition
+            of gaps. The default is None.
+
+        Returns
+        -------
+        None.
+
+        Note
+        -------
+        Gaps and missing observations resulting from an outlier on a specific
+        obstype, are assumed to be gaps/missing observation for all obstypes.
+
+        Note
+        ------
+        Be aware that n_gapsize is used for the current resolution of the Dataset,
+        this is different from the gap check applied on the inported data, if
+        the dataset is coarsend.
+
+        """
+        if n_gapsize is None:
+            n_gapsize = self.settings.gap['gaps_settings']['gaps_finder']['gapsize_n']
+            if not self.metadf["assumed_import_frequency"].eq(self.metadf['dataset_resolution']).all():
+                print(f'The defenition of the gapsize (n_gapsize = {n_gapsize}) \
+                               will have another effect on the update of the gaps and missing \
+                                   timestamps because coarsening is applied and the defenition \
+                                   of the gapsize is not changed.')
+
+
+
+        # combine to one dataframe
+        mergedf = self.combine_all_to_obsspace()
+        mergedf = mergedf.xs(obstype, level='obstype')
+
+
+        # ignore labels
+        possible_outlier_labels = [vals['outlier_flag'] for vals in self.settings.qc['qc_checks_info'].values()]
+
+
+        # create groups when the final label changes
+        persistance_filter = ((mergedf['label'].shift() != mergedf['label'])).cumsum()
+        grouped = mergedf.groupby(['name', persistance_filter])
+
+        #locate new gaps by size of consecutive the same final label per station
+        group_sizes = grouped.size()
+        outlier_groups = group_sizes[
+            group_sizes > n_gapsize
+        ]
+
+        # find only groups with final label as an outlier
+        gaps = []
+        # new_gapsdf = pd.DataFrame()
+        new_gaps_idx = init_multiindex()
+        for group_idx in outlier_groups.index:
+            groupdf = grouped.get_group(group_idx)
+            group_final_label = groupdf['label'].iloc[0]
+            if not group_final_label in possible_outlier_labels:
+                #no gap candidates
+                continue
+            else:
+                gap =Gap(name=groupdf.index.get_level_values('name')[0],
+                         startdt=groupdf.index.get_level_values('datetime').min(),
+                         enddt=groupdf.index.get_level_values('datetime').max())
+
+                gaps.append(gap)
+                # new_gapsdf = pd.concat([new_gapsdf,
+                #                         pd.DataFrame(data={'start_gap': [groupdf.index.get_level_values('datetime').min()],
+                #                                            'end_gap': [groupdf.index.get_level_values('datetime').max()]},
+                #                                      index=[groupdf.index.get_level_values('name')[0]])])
+
+                new_gaps_idx = new_gaps_idx.union(groupdf.index, sort=False)
+
+
+
+        # add all the outliers, that are not in the new gaps to the new missing obs
+        new_missing_obs = mergedf[mergedf['label'].isin(possible_outlier_labels)].index
+        new_missing_obs = new_missing_obs.drop(new_gaps_idx.to_numpy(), errors='ignore')
+
+
+        # to series
+        missing_obs_series = new_missing_obs.to_frame().reset_index(drop=True).set_index('name')['datetime']
+        # Create missing obs
+        new_missing_collection = Missingob_collection(missing_obs_series)
+
+
+
+        # update self
+        self.gaps.extend(gaps)
+        self.missing_obs = self.missing_obs + new_missing_collection
+
+
+
     # =============================================================================
     #   Gap Filling
     # =============================================================================
 
-    def fill_gaps_linear(self, obstype="temp"):
+    # def fill_gaps_automatic(self, modeldata, obstype='temp',
+    #                         max_interpolate_duration_str=None,
+    #                         overwrite=True):
+    #     """
+    #     Fill gaps using an automatic decision on which method to use to fill.
+    #     For small gaps (gap_duration <= max_interpolate_duration_str) interpolation
+    #     is applied, for larger gaps the model debias method is used.
+
+    #     Parameters
+    #     ----------
+    #     modeldata : metobs_toolkit.Modeldata
+    #         The ERA5 Modeldata instance containing observations for the periods
+    #         gaps and the leading/trailing periods..
+    #     obstype : str, optional
+    #         Observation type to fill the gaps for. The default is 'temp'.
+    #     max_interpolate_duration_str : timedelta or timedeltastring, optional
+    #         A time indication (like '5H') to indicate the maximum gapsize to use
+    #         interpolation for. If None, the default settings will be used. The default is None.
+    #     overwrite : bool, optional
+    #         If True, present gapfill values will be overwritten. The default is True.
+
+    #     Returns
+    #     -------
+    #     comb_df : TYPE
+    #         DESCRIPTION.
+
+    #     """
+
+    #     # Validate input
+    #     # check if modeldata is available
+    #     if modeldata is None:
+    #         print(
+    #             "The dataset has no modeldate. Use the set_modeldata() function to add modeldata."
+    #         )
+    #         return None
+
+    #     # check if obstype is present in eramodel
+    #     assert (
+    #         obstype in modeldata.df.columns
+    #     ), f"{obstype} is not present in the modeldate: {modeldata}"
+
+    #     # check if all station are present in eramodeldata
+    #     stations = self.gaps.to_df().index.unique().to_list()
+    #     assert all(
+    #         [sta in modeldata.df.index.get_level_values("name") for sta in stations]
+    #     ), f"Not all stations with gaps are in the modeldata!"
+
+    #     if not self.gapfilldf.empty:
+    #         if overwrite:
+    #             print("Gapfilldf will be overwritten!")
+    #             self.gapfilldf = init_multiindexdf()
+    #         else:
+    #             print('Gapfilldf is not empty, set "overwrite=True" to overwrite it!')
+    #             print("CANCEL gap fill with ERA5")
+    #             return
+
+    #     if max_interpolate_duration_str is None:
+    #         max_interpolate_duration_str = self.settings.gap["gaps_fill_settings"]["automatic"]["max_interpolation_duration_str"]
+
+    #     fill_info = self.settings.gap["gaps_fill_info"]
+
+    #     # select the method to apply gapfill per gap
+    #     interpolate_gaps = []
+    #     debias_gaps = []
+
+    #     for gap in self.gaps.list:
+    #         if gap.duration <= pd.to_timedelta(max_interpolate_duration_str):
+    #             interpolate_gaps.append(gap)
+    #         else:
+    #             debias_gaps.append(gap)
+
+
+    #     # convert to Gap_collection
+    #     interpolate_gap_collection = _gap_collection_from_list_of_gaps(interpolate_gaps)
+    #     debias_gap_collection =_gap_collection_from_list_of_gaps(debias_gaps)
+
+
+    #     #1  Fill by interpolation
+
+    #     filldf_interp = init_multiindexdf()
+
+    #     fill_settings_interp = self.settings.gap["gaps_fill_settings"]["linear"]
+
+
+    #     filldf_interp[obstype] = interpolate_gap_collection.apply_interpolate_gaps(
+    #                         obsdf=self.df,
+    #                         outliersdf=self.outliersdf,
+    #                         dataset_res=self.metadf["dataset_resolution"],
+    #                         obstype=obstype,
+    #                         method=fill_settings_interp["method"],
+    #                         max_consec_fill=fill_settings_interp["max_consec_fill"],
+    #                         )
+
+    #     # add label column
+    #     filldf_interp[obstype + "_" + fill_info["label_columnname"]] = fill_info["label"]["linear"]
+
+
+    #     #2 Fill by debias
+    #     filldf_debias = init_multiindexdf()
+
+    #     fill_settings_debias = self.settings.gap["gaps_fill_settings"]["model_debias"]
+
+
+    #     apply_debias_era5_gapfill(gapslist = self.gaps
+    #                               dataset=self,
+    #                               eraModelData=modeldata,
+    #                               obstype=obstype,
+    #                               debias_settings=fill_settings_debias)
+
+    #     # add label column
+    #     filldf_debias[obstype + "_" + fill_info["label_columnname"]] = fill_info["label"]["model_debias"]
+
+
+    #     # combine both fill df's
+    #     comb_df = pd.concat([filldf_interp, filldf_debias])
+    #     if overwrite:
+    #         self.gapfilldf = comb_df
+    #     return comb_df
+
+
+    def fill_gaps_automatic(self, modeldata, obstype='temp',
+                            max_interpolate_duration_str=None,
+                            overwrite=True):
+
+        # Validate input
+        # check if modeldata is available
+        if modeldata is None:
+            print(
+                "The dataset has no modeldate. Use the set_modeldata() function to add modeldata."
+            )
+            return None
+
+        # check if obstype is present in eramodel
+        assert (
+            obstype in modeldata.df.columns
+        ), f"{obstype} is not present in the modeldate: {modeldata}"
+
+        # check if all station are present in eramodeldata
+        # stations = self.gaps.to_df().index.unique().to_list()
+        stations = list(set([gap.name for gap in self.gaps]))
+        assert all(
+            [sta in modeldata.df.index.get_level_values("name") for sta in stations]
+        ), f"Not all stations with gaps are in the modeldata!"
+
+        if not self.gapfilldf.empty:
+            if overwrite:
+                print("Gapfilldf will be overwritten!")
+                self.gapfilldf = init_multiindexdf()
+            else:
+                print('Gapfilldf is not empty, set "overwrite=True" to overwrite it!')
+                print("CANCEL gap fill with ERA5")
+                return
+
+        if max_interpolate_duration_str is None:
+            max_interpolate_duration_str = self.settings.gap["gaps_fill_settings"]["automatic"]["max_interpolation_duration_str"]
+
+        fill_info = self.settings.gap["gaps_fill_info"]
+
+        # select the method to apply gapfill per gap
+        interpolate_gaps = []
+        debias_gaps = []
+
+        for gap in self.gaps:
+            if gap.duration <= pd.to_timedelta(max_interpolate_duration_str):
+                interpolate_gaps.append(gap)
+            else:
+                debias_gaps.append(gap)
+
+        #1  Fill by interpolation
+
+        fill_settings_interp = self.settings.gap["gaps_fill_settings"]["linear"]
+
+
+        apply_interpolate_gaps(
+                            gapslist=interpolate_gaps,
+                            obsdf=self.df,
+                            outliersdf=self.outliersdf,
+                            dataset_res=self.metadf["dataset_resolution"],
+                            gapfill_settings=self.settings.gap['gaps_fill_info'],
+                            obstype=obstype,
+                            method=fill_settings_interp["method"],
+                            max_consec_fill=fill_settings_interp["max_consec_fill"],
+                            )
+
+        filldf_interp = make_gapfill_df(interpolate_gaps)
+
+        #2 Fill by debias
+
+        fill_settings_debias = self.settings.gap["gaps_fill_settings"]["model_debias"]
+
+
+        apply_debias_era5_gapfill(gapslist=debias_gaps,
+                                        dataset=self,
+                                        eraModelData=modeldata,
+                                        obstype=obstype,
+                                        debias_settings=fill_settings_debias)
+
+        # add label column
+        filldf_debias = make_gapfill_df(debias_gaps)
+
+
+        # combine both fill df's
+        comb_df = pd.concat([filldf_interp, filldf_debias])
+        if overwrite:
+            self.gapfilldf = comb_df
+        return comb_df
+
+
+    def fill_gaps_linear(self, obstype="temp", overwrite=True):
         """
         Fill the gaps using linear interpolation.
 
         Parameters
         ----------
         obstype : string, optional
             Fieldname to visualise. This can be an observation or station
@@ -492,27 +847,33 @@
 
         """
         # TODO logging
         fill_settings = self.settings.gap["gaps_fill_settings"]["linear"]
         fill_info = self.settings.gap["gaps_fill_info"]
 
         # fill gaps
-        self.gapfilldf[obstype] = self.gaps.apply_interpolate_gaps(
+        apply_interpolate_gaps(
+            gapslist=self.gaps,
             obsdf=self.df,
             outliersdf=self.outliersdf,
             dataset_res=self.metadf["dataset_resolution"],
+            gapfill_settings=self.settings.gap['gaps_fill_info'],
             obstype=obstype,
             method=fill_settings["method"],
             max_consec_fill=fill_settings["max_consec_fill"],
         )
 
-        # add label column
-        self.gapfilldf[obstype + "_" + fill_info["label_columnname"]] = fill_info[
-            "label"
-        ]["linear"]
+        # get gapfilldf
+        gapfilldf = make_gapfill_df(self.gaps)
+
+        if overwrite:
+            self.gapfilldf = gapfilldf
+
+        return gapfilldf
+
 
     def fill_missing_obs_linear(self, obstype='temp'):
         # TODO logging
         fill_settings = self.settings.missing_obs['missing_obs_fill_settings']['linear']
         fill_info = self.settings.missing_obs['missing_obs_fill_info']
 
 
@@ -527,14 +888,27 @@
         missing_fill_df = self.missing_obs.fill_df
         missing_fill_df[obstype+'_' + fill_info["label_columnname"]] = fill_info["label"]["linear"]
 
         # Update attribute
 
         self.missing_fill_df = missing_fill_df
 
+    def get_gaps_df(self):
+        """
+        List all gaps into an overview dataframe.
+
+        Returns
+        -------
+        pandas.DataFrame
+            A DataFrame with stationnames as index, and the start, end and duretion
+            of the gaps as columns.
+
+        """
+        return gaps_to_df(self.gaps)
+
 
 
     def get_analysis(self):
         """
         Create a MetObs_toolkit.Analysis instance from the Dataframe
 
         Returns
@@ -568,15 +942,16 @@
             Fieldname to visualise. This can be an observation or station
             attribute. The default is 'temp'.
         overwrite : bool, optional
             If True, the Dataset.Gapfilldf will be overwritten. The default is True.
 
         Returns
         -------
-        None.
+        Gapfilldf : pandas.DataFrame
+            A dataframe containing all gap filled values and the use method.
 
         """
 
         fill_info = self.settings.gap["gaps_fill_info"]
 
         # check if modeldata is available
         if modeldata is None:
@@ -585,77 +960,88 @@
             )
             return None
         # check if obstype is present in eramodel
         assert (
             obstype in modeldata.df.columns
         ), f"{obstype} is not present in the modeldate: {modeldata}"
         # check if all station are present in eramodeldata
-        stations = self.gaps.to_df().index.unique().to_list()
+        # stations = self.gaps.to_df().index.unique().to_list()
+        stations = list(set([gap.name for gap in self.gaps]))
         assert all(
             [sta in modeldata.df.index.get_level_values("name") for sta in stations]
         ), f"Not all stations with gaps are in the modeldata!"
 
-        if not self.gapfilldf.empty:
-            if overwrite:
-                print("Gapfilldf will be overwritten!")
-                self.gapfilldf = init_multiindexdf()
-            else:
-                print('Gapfilldf is not empty, set "overwrite=True" to overwrite it!')
-                print("CANCEL gap fill with ERA5")
-                return
 
         if method == "debias":
-            test = self.gaps.apply_debias_era5_gapfill(
-                dataset=self,
-                eraModelData=modeldata,
-                obstype=obstype,
-                debias_settings=self.settings.gap["gaps_fill_settings"]["model_debias"],
-            )
 
-            self.gapfilldf[obstype] = test
-            # add label column
-            self.gapfilldf[obstype + "_" + fill_info["label_columnname"]] = fill_info[
-                "label"
-            ]["model_debias"]
+            fill_settings_debias = self.settings.gap["gaps_fill_settings"]["model_debias"]
+
+
+            apply_debias_era5_gapfill(gapslist=self.gaps,
+                                            dataset=self,
+                                            eraModelData=modeldata,
+                                            obstype=obstype,
+                                            debias_settings=fill_settings_debias)
+
+            # get fill df
+            filldf = make_gapfill_df(self.gaps)
         else:
             print("not implemented yet")
 
+        if overwrite:
+            self.gapfilldf = filldf
+        return filldf
+
     def write_to_csv(
         self,
+        obstype=None,
         filename=None,
         include_outliers=True,
-        include_gapfill=True,
+        include_fill_values=True,
         add_final_labels=True,
         use_tlk_obsnames=True,
+        overwrite_outliers_by_gaps_and_missing=True,
+        seperate_metadata_file = True
     ):
         """
         Write the dataset to a file where the observations, metadata and
         (if available) the quality labels per observation type are merged
         together.
 
         A final qualty control label for each
         quality-controlled-observation type can be added in the outputfile.
 
         The file will be writen to the outputfolder specified in the settings.
 
         Parameters
         ----------
+        obstype : string, optional
+            Specify an observation type to subset all observations to. If None,
+            all available observation types are writen to file. The default is
+            None.
         filename : string, optional
             The name of the output csv file. If none, a standard-filename
             is generated based on the period of data. The default is None.
         include_outliers : bool, optional
             If True, the outliers will be present in the csv file. The default is True.
-        include_gapfill : bool, optional
-            If True, the filled gap values will be present in the csv file. The default is True.
+        include_fill_values : bool, optional
+            If True, the filled gap and missing observation values will be
+            present in the csv file. The default is True.
         add_final_labels : bool, optional
             If True, a column is added containing the final label of an observation. The default is True.
         use_tlk_obsnames : bool, optional
             If True, the standard naming of the metobs_toolkit is used, else
             the original names for obstypes is used. The default is True.
-
+        overwrite_outliers_by_gaps_and_missing : bool, optional
+            If the gaps and missing observations are updated using outliers,
+            interpret these records as gaps/missing outliers if True. Else these
+            will be interpreted as outliers. The default is True.
+        seperate_metadata_file : bool, optional
+            If true, the metadat is writen to a seperate file, else the metadata
+            is merged to the observation in one file. The default is True.
         Returns
         -------
         None.
 
         """
 
         logger.info("Writing the dataset to a csv file")
@@ -666,89 +1052,64 @@
 
         assert os.path.isdir(
             self.settings.IO["output_folder"]
         ), f'The outputfolder: \
             {self.settings.IO["output_folder"]} is not found. '
 
         # combine all dataframes
-        mergedf = self.combine_all_to_obsspace()  # with outliers
+        mergedf = self.combine_all_to_obsspace(
+            overwrite_outliers_by_gaps_and_missing=overwrite_outliers_by_gaps_and_missing)  # with outliers
+        # Unstack mergedf
+        # remove duplicates
+        mergedf = mergedf[~mergedf.index.duplicated(keep='first')]
+
+        # drop outliers if required
+        if not include_outliers:
+            outlier_labels = [var['outlier_flag'] for var in self.settings.qc['qc_checks_info']]
+            mergedf = mergedf[~mergedf['label'].isin(outlier_labels)]
+
+
+        # drop fill values if required
+        if not include_fill_values:
+            fill_labels = ['gap fill', 'missing observation fill'] #toolkit representation labels
+            mergedf = mergedf[~mergedf['toolkit_representation'].isin(fill_labels)]
 
-        # select which columns to keep
-        if include_outliers:
-            if not add_final_labels:
-                _fin_cols = [
-                    col for col in mergedf.columns if col.endswith("_final_label")
-                ]
-                mergedf = mergedf.drop(columns=_fin_cols)
-
-        else:  # exclude outliers
-            if add_final_labels:
-                cols_to_keep = [
-                    col for col in mergedf.columns if col in observation_types
-                ]
-                cols_to_keep.extend(
-                    [col for col in mergedf.columns if col.endswith("_final_label")]
-                )
-                mergedf = mergedf[cols_to_keep]
-
-        if not include_gapfill:
-            # locate all filled values
-            filled_df = init_multiindexdf()
-            final_columns = [
-                col for col in mergedf.columns if col.endswith("_final_label")
-            ]
-            for final_column in final_columns:
-                filled_df = pd.concat(
-                    [
-                        filled_df,
-                        mergedf.loc[
-                            mergedf[final_column]
-                            == self.settings.gaps["gaps_fill_info"]["label"]
-                        ],
-                    ]
-                )
-
-            # drop filled values from mergedf
-            mergedf = mergedf.drop(filled_df.index, errors="ignore")
+        if not obstype is None:
+            mergedf = mergedf.xs(obstype, level='obstype', drop_level=False)
 
-            # fill with numpy nan
-            nan_columns = {
-                col: np.nan for col in mergedf.columns if col in observation_types
-            }
-            filled_df = filled_df.assign(**nan_columns)
-            # rename label
-            filled_df = filled_df.replace(
-                {
-                    self.settings.gaps["gaps_fill_info"]["label"]: self.settings.gaps[
-                        "gaps_info"
-                    ]["gap"]["outlier_flag"]
-                }
-            )
-            # add to mergedf
-            mergedf = pd.concat([mergedf, filled_df]).sort_index()
 
-        present_obstypes = [col for col in observation_types if col in mergedf.columns]
 
         # Map obstypes columns
         if not use_tlk_obsnames:
-            # TODO
-            print("not implemented yet")
+            mapper = self.data_template.transpose()['orig_name'].to_dict()
+            mergedf = mergedf.reset_index()
+            mergedf['new_names'] = mergedf['obstype'].map(mapper)
+            mergedf = mergedf.drop(columns=['obstype'])
+            mergedf = mergedf.rename(columns={'new_names': 'obstype'})
+            mergedf = mergedf.set_index(['name', 'datetime', 'obstype'])
+
+
+        mergedf = mergedf.unstack('obstype')
+
+        # to one level for the columns
+        mergedf.columns = [' : '.join(col).strip() for col in mergedf.columns.values]
+
 
-        # TODO Convert units if needed.
 
         # columns to write
         write_dataset_to_csv(
             df=mergedf,
             metadf=self.metadf,
             filename=filename,
             outputfolder=self.settings.IO["output_folder"],
             location_info=self.settings.app["location_info"],
-            observation_types=present_obstypes,
+            seperate_metadata_file=seperate_metadata_file,
         )
 
+
     # =============================================================================
     #     Quality control
     # =============================================================================
 
     def apply_quality_control(
         self,
         obstype="temp",
@@ -780,24 +1141,25 @@
              If True the gross_value check is applied if False not. The default
              is True.
          persistance : Bool, optional
             If True the persistance check is applied if False not. The default
             is True.. The default is True.
          step : Bool, optional
             If True the step check is applied if False not. The default is True.
-        internal_consistency : Bool, optional
+         internal_consistency : Bool, optional
             If True the internal consistency check is applied if False not. The
             default is True.
-        qc_info: Bool, optional
+         qc_info: Bool, optional
             If True info about the quality control is printed if False not. The
             default is True.
          ignore_val : numeric, optional
              Values to ignore in the quality checks. The default is np.nan.
 
          Returns
+         ---------
 
          None.
 
         """
 
         if repetitions:
             print("Applying the repetitions-check on all stations.")
@@ -934,168 +1296,128 @@
                 ignore_index=True,
             )
 
         self._qc_checked_obstypes.append(obstype)
         self._qc_checked_obstypes = list(set(self._qc_checked_obstypes))
         self.outliersdf = self.outliersdf.sort_index()
 
-    def combine_all_to_obsspace(self, repr_outl_as_nan=False):
-        """
-        Combine observations, outliers, gaps and missing timesteps to one
-        dataframe in the resolution of the dataset. Final quality labels are
-        calculated for all checked obstypes.
-
-        If an observation value exist for an outlier, it will be used in the
-        corresponding obstype column.
 
-        Returns
 
-        comb_df : pandas.DataFrame()
-            Multi index dataframe with observations and labels.
+    def combine_all_to_obsspace(self, repr_outl_as_nan=False,
+                                overwrite_outliers_by_gaps_and_missing=True):
 
-        """
+        # TODO: docstring
+        # TODO: what to do with repr_outl_as_nan
+        # TODO: label values from settings not hardcoding
 
         # =============================================================================
-        # Unstack outliers to regular multiindex
+        # Stack outliers
         # =============================================================================
-        outliersdf = self.outliersdf
-
-        # remove duplicate indixes (needed for update)
-        outliersdf = outliersdf[~outliersdf.index.duplicated(keep="first")]
 
-        if not outliersdf.empty:
-            outliersdf_values = outliersdf["value"].unstack()  # for later use
-            # convert to wide df with labels
-            outliersdf = outliersdf["label"].unstack()
-
-            # convert to final label names for columns
-            outliersdf = outliersdf.rename(
-                columns={col: col + "_final_label" for col in outliersdf.columns}
-            )
-
-        else:
-            outliersdf = init_multiindexdf()
-            outliersdf_values = init_multiindexdf()  # for later use
-            outliercolumns = [
-                col + "_final_label" for col in self.df if col in observation_types
-            ]
-            for column in outliercolumns:
-                outliersdf[column] = "not checked"
+        outliersdf = self.outliersdf
+        outliersdf['toolkit_representation'] = 'outlier'
 
         # =============================================================================
-        # Combine observations and outliers
+        # Stack observations
         # =============================================================================
-        # get observations
         df = self.df
+        # better save than sorry
+        present_obstypes = [col for col in df if col in observation_types]
+        df = df[present_obstypes]
 
-        # 0. make shure there is a final column for each obstype in the df,
-        # if qc did not found any outliers, then there is apriori no final label column
-        present_obstypes = [col for col in observation_types if col in df.columns]
-        for presen_obstype in present_obstypes:
-            final_label = presen_obstype + "_final_label"
-            if not final_label in outliersdf.columns:
-                outliersdf[final_label] = np.nan
-
-        # 1. Merge the label columns
-        df_and_outl = df.merge(
-            outliersdf, how="outer", left_index=True, right_index=True
-        )
-
-        # 2. fill the missing labels
-
-        # split between obstype that are checked by qc and obstypes that are not checked
-        checked_cols = [
-            col + "_final_label" for col in list(set(self._qc_checked_obstypes))
-        ]
-        not_checked_cols = [
-            col
-            for col in df_and_outl.columns
-            if ((col.endswith("_final_label")) and (not col in checked_cols))
-        ]
+        # to tripple index
+        df = df.stack(dropna=False).reset_index().rename(columns={'level_2': 'obstype', 0: 'value'}).set_index(['name', 'datetime', 'obstype'])
 
-        # if obstype checked, and value is nan --> label ok
-        df_and_outl[checked_cols] = df_and_outl[checked_cols].fillna("ok")
-        # if obstype is not checked and label is missing --> label 'not checked'
-        df_and_outl[not_checked_cols] = df_and_outl[not_checked_cols].fillna(
-            "not checked"
-        )
+        df['label'] = 'ok'
+        df['toolkit_representation'] = 'observation'
+
+        # remove outliers from the observations
+        df = df[~ df.index.isin(outliersdf.index)]
 
-        # 3. Update the values if needed
-        if not repr_outl_as_nan:
-            # Merge obs and outliers, where obs values will be updated by outliers
-            df_and_outl.update(
-                other=outliersdf_values, join="left", overwrite=True, errors="ignore"
-            )
 
         # =============================================================================
-        # Make gaps, gapsfill and missing dataframes
+        # Stack gaps
         # =============================================================================
 
-        # add gaps observations and fill with default values
-        gapsidx = self.gaps.get_gaps_indx_in_obs_space(
-            self.df, self.outliersdf, self.metadf["dataset_resolution"]
-        )
-        gapsdf = gapsidx.to_frame()
 
         # add gapfill and remove the filled records from gaps
         gapsfilldf = self.gapfilldf.copy()
-        gapsdf = gapsdf.drop(gapsfilldf.index, errors="ignore")
+
+        # to triple index
+        gapsfilldf = value_labeled_doubleidxdf_to_triple_idxdf(gapsfilldf)
+        gapsfilldf['toolkit_representation'] = 'gap fill'
+
+        gapsidx = get_gaps_indx_in_obs_space(gapslist=self.gaps,
+                                             obsdf = self.df,
+                                             outliersdf = self.outliersdf,
+                                             resolutionseries=self.metadf["dataset_resolution"])
+
+        gapsdf = pd.DataFrame(index=gapsidx, columns=present_obstypes)
+        gapsdf = gapsdf.stack(dropna=False).reset_index().rename(columns={'level_2': 'obstype', 0: 'value'}).set_index(['name', 'datetime', 'obstype'])
+
+        gapsdf['label'] = self.settings.gap['gaps_info']['gap']['outlier_flag']
+        gapsdf['toolkit_representation'] = 'gap'
+
+
+        # Remove gaps from df
+        df = df[~ df.index.isin(gapsdf.index)]
+
+        if overwrite_outliers_by_gaps_and_missing:
+            outliersdf = outliersdf.drop(index=gapsdf.index, errors='ignore')
+
+
+        # Remove gapfill values records from the gaps
+        gapsdf = gapsdf.drop(index=gapsfilldf.index)
+
+
+
+        # =============================================================================
+        # Stack missing
+        # =============================================================================
+
+        missingfilldf = self.missing_fill_df.copy()
+        missingfilldf = value_labeled_doubleidxdf_to_triple_idxdf(missingfilldf)
+        missingfilldf['toolkit_representation'] = 'missing observation fill'
 
 
         # add missing observations if they occure in observation space
         missingidx = self.missing_obs.get_missing_indx_in_obs_space(
             self.df, self.metadf["dataset_resolution"]
         )
-        missingdf = missingidx.to_frame()
-        missingfilldf = self.missing_fill_df.copy()
-        missingdf = missingdf.drop(missingfilldf.index, errors="ignore")
 
+        missingdf = pd.DataFrame(index=missingidx, columns=present_obstypes)
 
 
-        # initiate default values for gaps and missing that are not filled
-        for col in df_and_outl.columns:
-            if col in observation_types:
-                default_value_gap = np.nan  # nan for observations
-                default_value_missing = np.nan
-
-            elif col.endswith("_final_label"):
-                # 'gap' for final label
-                default_value_gap = self.settings.gap["gaps_info"]["gap"][
-                    "outlier_flag"
-                ]
-
-                # 'is_missing_timestamp' for final label
-                default_value_missing = self.settings.gap["gaps_info"][
-                    "missing_timestamp"
-                ]["outlier_flag"]
+        missingdf = missingdf.stack(dropna=False).reset_index().rename(columns={'level_2': 'obstype', 0: 'value'}).set_index(['name', 'datetime', 'obstype'])
 
-            else:
-                default_value_gap = "not checked"
-                default_value_missing = "not checked"
+        missingdf['label'] = self.settings.gap['gaps_info']['missing_timestamp']['outlier_flag']
+        missingdf['toolkit_representation'] = 'missing observation'
+
+        # Remove missing from df
+        df = df[~ df.index.isin(missingdf.index)]
+
+        if overwrite_outliers_by_gaps_and_missing:
+            outliersdf = outliersdf.drop(index=missingdf.index, errors='ignore')
+
+        # Remove missingfill values records from the missing
+        missingdf = missingdf.drop(index=missingfilldf.index)
+
+
+        # =============================================================================
+        # combine all
+        # =============================================================================
+
+        combdf = pd.concat([df, outliersdf, gapsdf, gapsfilldf, missingdf, missingfilldf]).sort_index()
+
+        # To be shure?
+        combdf = combdf[~combdf.index.duplicated(keep='first')]
+        return combdf
 
 
-            gapsdf[col] = default_value_gap
-            missingdf[col] = default_value_missing
-            if not col in gapsfilldf.columns:
-                gapsfilldf[col] = default_value_gap
-            if not col in missingfilldf.columns:
-                missingfilldf[col] = default_value_missing
-
-        # sort columns
-        column_order = df_and_outl.columns.to_list()
-        gapsdf = gapsdf[column_order]
-        gapsfilldf=gapsfilldf[column_order]
-        missingdf = missingdf[column_order]
-        missingfilldf = missingfilldf[column_order]
-
-        # Merge all together
-        comb_df = pd.concat([df_and_outl, gapsdf, missingdf,
-                             gapsfilldf, missingfilldf]).sort_index()
 
-        return comb_df
 
     def get_qc_stats(self, obstype="temp", stationnames=None, make_plot=True):
         """
         Compute frequency statistics on the qc labels for an observationtype.
         The output is a dataframe containing the frequency statistics presented
         as percentages.
 
@@ -1123,16 +1445,16 @@
 
         """
 
         # cobmine all and get final label
         comb_df = self.combine_all_to_obsspace()
 
         # subset to relevant columnt
-        relev_columns = [obstype, obstype + "_final_label"]
-        comb_df = comb_df[relev_columns]
+        comb_df = comb_df.xs(obstype, level='obstype')[['label']]
+
 
         # compute freq statistics
         final_freq, outl_freq, specific_freq = get_freq_statistics(
             comb_df=comb_df,
             obstype=obstype,
             checks_info=self.settings.qc["qc_checks_info"],
             gaps_info=self.settings.gap["gaps_info"],
@@ -1258,15 +1580,15 @@
         self.metadf["dataset_resolution"] = pd.to_timedelta(freq)
         # update df
         self.df = df
 
         # Remove gaps and missing from the observatios
         # most gaps and missing are already removed but when increasing timeres,
         # some records should be removed as well.
-        self.df = self.gaps.remove_gaps_from_obs(obsdf=self.df)
+        self.df = remove_gaps_from_obs(gaplist = self.gaps, obsdf=self.df)
         self.df = self.missing_obs.remove_missing_from_obs(obsdf=self.df)
 
 
     def sync_observations(self, tollerance, verbose=True):
         """
         Simplify and syncronize the observation timestamps along different stations.
 
@@ -1753,15 +2075,15 @@
 
         # add import frequencies to metadf (after import qc!)
         self.metadf["assumed_import_frequency"] = freq_series_import
 
         self.metadf["dataset_resolution"] = freq_series
 
         # Remove gaps and missing from the observations AFTER timecoarsening
-        self.df = self.gaps.remove_gaps_from_obs(obsdf=self.df)
+        self.df = remove_gaps_from_obs(gaplist = self.gaps, obsdf=self.df)
         self.df = self.missing_obs.remove_missing_from_obs(obsdf=self.df)
 
 
     def _initiate_df_attribute(self, dataframe, update_metadf=True):
         logger.info(
             f"Updating dataset by dataframe with shape:\
                     {dataframe.shape}."
@@ -1780,22 +2102,22 @@
             metadf = metadf[~metadf.index.duplicated(keep="first")]
 
             self.metadf = metadf_to_gdf(metadf)
 
 
     def _apply_qc_on_import(self):
         # find missing obs and gaps, and remove them from the df
-        self.df, missing_obs, gaps_df = missing_timestamp_and_gap_check(
+        self.missing_obs, self.gaps = missing_timestamp_and_gap_check(
             df=self.df,
             gapsize_n=self.settings.gap["gaps_settings"]["gaps_finder"]["gapsize_n"],
         )
 
         # Create gaps and missing obs objects
-        self.gaps = Gap_collection(gaps_df)
-        self.missing_obs = Missingob_collection(missing_obs)
+        # self.gaps = gaps_list
+        # self.missing_obs = Missingob_collection(missing_obs)
 
         # Perform QC checks on original observation frequencies
         self.df, dup_outl_df = duplicate_timestamp_check(
             df=self.df,
             checks_info=self.settings.qc["qc_checks_info"],
             checks_settings=self.settings.qc["qc_check_settings"],
         )
@@ -1864,30 +2186,81 @@
 
         # update metadata
         self.metadf = self.metadf.merge(
             altitude_series.to_frame(), how="left", left_index=True, right_index=True
         )
         return altitude_series
 
-    def get_landcover(self, buffer=100, aggregate=True):
+    def get_landcover(self, buffers=[100], aggregate=True, overwrite=True, gee_map='worldcover'):
+        """
+        Extract the landcover fractions in a buffer with a specific radius for
+        all stations. If an aggregation scheme is define, one can choose to
+        aggregate the landcoverclasses.
+
+        The landcover fractions will be added to the Dataset.metadf if overwrite
+        is True. Presented as seperate columns where each column represent the
+        landcovertype and corresponding buffer.
+
+
+
+
+        Parameters
+        ----------
+        buffers : num, optional
+            The list of buffer radia in dataset units (meters for ESA worldcover) . The default is 100.
+        aggregate : bool, optional
+            If True, the classes will be aggregated with the corresponding
+            aggregation scheme. The default is True.
+        overwrite : bool, optional
+            If True, the Datset.metadf will be updated with the generated
+            landcoverfractions. The default is True.
+        gee_map : str, optional
+            The name of the dataset to use. This name should be present in the
+            settings.gee['gee_dataset_info']. If aggregat is True, an aggregation
+            scheme should included as well. The default is 'worldcover'
+
+        Returns
+        -------
+        frac_df : pandas.DataFrame
+            A Dataframe with index: name, buffer_radius and the columns are the
+            fractions.
+
+        """
         # connect to gee
         connect_to_gee()
 
-        # Extract landcover fractions for all stations
-        lc_frac_df = lc_fractions_extractor(
-            metadf=self.metadf,
-            mapinfo=self.settings.gee["gee_dataset_info"]["worldcover"],
-            buffer=buffer,
-            agg=aggregate,
-        )
+        df_list = []
+        for buffer in buffers:
 
-        # remove columns if they exists
-        self.metadf = self.metadf.drop(
-            columns=list(lc_frac_df.columns), errors="ignore"
-        )
+            print(f'Extracting landcover from {gee_map} with buffer radius = {buffer}')
+            # Extract landcover fractions for all stations
+            lc_frac_df, buffer = lc_fractions_extractor(
+                metadf=self.metadf,
+                mapinfo=self.settings.gee["gee_dataset_info"][gee_map],
+                buffer=buffer,
+                agg=aggregate,
+            )
 
-        # update metadf
-        self.metadf = self.metadf.merge(
-            lc_frac_df, how="left", left_index=True, right_index=True
-        )
+            # add buffer to the index
+            lc_frac_df['buffer_radius'] = buffer
+            lc_frac_df = lc_frac_df.reset_index().set_index(['name', 'buffer_radius'])
+            lc_frac_df = lc_frac_df.sort_index()
+
+            # add to the list
+            df_list.append(lc_frac_df)
+
+
+        # concat all df for different buffers to one
+        frac_df = pd.concat(df_list)
+        frac_df = frac_df.sort_index()
+
+
+        if overwrite:
+
+            for buf in frac_df.index.get_level_values('buffer_radius').unique():
+                buf_df = frac_df.xs(buf, level='buffer_radius')
+                buf_df.columns= [col + f'_{int(buf)}m' for col in buf_df.columns]
+
+                # overwrite the columns or add them if they did not exist
+                self.metadf[buf_df.columns] = buf_df
 
-        return lc_frac_df
+        return frac_df
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/dataset_settings_updater.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/dataset_settings_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         self.settings.app["default_name"] = str(default_name)
 
 
 
     def update_gap_and_missing_fill_settings(self, gap_interpolation_method=None, gap_interpolation_max_consec_fill=None,
                                              gap_debias_prefered_leading_period_hours=None, gap_debias_prefered_trailing_period_hours=None,
                                              gap_debias_minimum_leading_period_hours=None, gap_debias_minimum_trailing_period_hours=None,
-                                             missing_obs_interpolation_method=None):
+                                             automatic_max_interpolation_duration_str=None, missing_obs_interpolation_method=None):
         """
         Update the settings on the filling methods for missing observations and gaps.
 
         If None, the current setting is not updated.
 
         Parameters
         ----------
@@ -122,14 +122,18 @@
             biasses wrt the model. The default is None.
         gap_debias_minimum_leading_period_hours : int, optional
             The minimum size of the leading period for calculating hourly
             biasses wrt the model. The default is None.
         gap_debias_minimum_trailing_period_hours : int, optional
             The minimum size of the trailing period for calculating hourly
             biasses wrt the model. The default is None.
+        automatic_max_interpolation_duration_str : Timedelta or str, optional
+            Maximum duration to apply interpolation for gapfill when using the
+            automatic gapfill method. Gaps with longer durations will be filled
+            using debiased modeldata. The default is None.
         missing_obs_interpolation_method : str, optional
             The interpolation method to pass to numpy.interpolate. The default is None.
 
         Returns
         -------
         None.
 
@@ -164,14 +168,23 @@
             self.settings.gap["gaps_fill_settings"]["model_debias"]["debias_period"]["minimum_leading_sample_duration_hours"] = abs(int(gap_debias_minimum_leading_period_hours))
 
         if not gap_debias_minimum_trailing_period_hours is None:
             logger.info(f' The minimum size of the trailing period for debias gapfill is updated: \
         {self.settings.gap["gaps_fill_settings"]["model_debias"]["debias_period"]["minimum_trailing_sample_duration_hours"]} --> {abs(int(gap_debias_minimum_trailing_period_hours))}')
             self.settings.gap["gaps_fill_settings"]["model_debias"]["debias_period"]["minimum_trailing_sample_duration_hours"] = abs(int(gap_debias_minimum_trailing_period_hours))
 
+        # Gapfill automatic
+        if not automatic_max_interpolation_duration_str is None:
+            if is_timedelta(str(automatic_max_interpolation_duration_str)):
+                logger.info(f' The maximum interpolation duration for automatic gapfill is updated: \
+            {self.settings.gap["gaps_fill_settings"]["automatic"]["max_interpolation_duration_str"]} --> {str(automatic_max_interpolation_duration_str)}')
+                self.settings.gap["gaps_fill_settings"]["automatic"]["max_interpolation_duration_str"] = str(automatic_max_interpolation_duration_str)
+            else:
+                logger.warning(f' {str(automatic_max_interpolation_duration_str)} is not a valid timedelta string. No update on this setting.')
+
         # Missing obs interpolation
         if not missing_obs_interpolation_method is None:
             logger.info(f' The missing observations interpolation method is updated: \
         {self.settings.missing_obs["missing_obs_fill_settings"]["linear"]["method"]} --> {str(missing_obs_interpolation_method)}')
             self.settings.missing_obs['missing_obs_fill_settings']['linear']['method'] = str(missing_obs_interpolation_method)
 
 
@@ -181,22 +194,23 @@
                             win_var_max_increase_per_sec=None, win_var_max_decrease_per_sec=None, win_var_time_win_to_check=None,
                             win_var_min_num_obs=None, step_max_increase_per_sec=None, step_max_decrease_per_sec=None):
 
         """
         Update the QC settings for the specified observation type.
 
         If a argument value is None, the default settings will not be updated.
+
         Parameters
         ----------
         gapsize_in_records : int (> 0), optional
             A gap is defined as a sequence of missing observations with a length
             greater or equal to this number, on the input frequencies. The default is None.
         dupl_timestamp_keep : bool, optional
             Setting that determines to keep, or remove duplicated timestamps. The default is None.
-        persis_time_win_to_check : Timedelta or str, optional
+        persis_time_win_to_check :automatic_max_interpolation_duration_str
             Time window for persistance check. The default is None.
         persis_min_num_obs : int (> 0), optional
             Minimal window members for persistance check. The default is None.
         rep_max_valid_repetitions : int (> 0), optional
             Maximal valid repetitions for repetitions check. The default is None.
         gross_value_min_value : numeric, optional
             Minimal value for gross value check. The default is None.
@@ -219,21 +233,17 @@
         -------
         None.
 
         Note
         -------
         The gap defenition is independend of the observation type, and is thus set for
         all the observation types.
+
         """
-        def is_timedelta(timedeltastr):
-            try:
-                pd.to_timedelta(timedeltastr)
-                return True
-            except:
-                return False
+
 
         assert obstype in observation_types, f'{obstype} is not a known observation type'
 
         # Gap defenition
         if not gapsize_in_records is None:
             logger.info(f' The defenition of a gap (=gapsize) is updated: \
         {self.settings.gap["gaps_settings"]["gaps_finder"]["gapsize_n"]} --> {abs(int(gapsize_in_records))}')
@@ -305,8 +315,19 @@
             logger.info(f'Maximal increase per second for step check updated:\
                         {self.settings.qc["qc_check_settings"]["step"][obstype]["max_increase_per_second"]}--> {abs(float(step_max_increase_per_sec))}')
             self.settings.qc['qc_check_settings']["step"][obstype]['max_increase_per_second'] = abs(float(step_max_increase_per_sec))
 
         if not step_max_decrease_per_sec is None:
             logger.info(f'Maximal decrease per second for step check updated:\
                        {self.settings.qc["qc_check_settings"]["step"][obstype]["max_decrease_per_second"]} --> {-1.0 * abs(float(step_max_decrease_per_sec))}')
-            self.settings.qc['qc_check_settings']["step"][obstype]['max_decrease_per_second'] = -1.0 * abs(float(step_max_decrease_per_sec))
+            self.settings.qc['qc_check_settings']["step"][obstype]['max_decrease_per_second'] = -1.0 * abs(float(step_max_decrease_per_sec))
+
+
+# =============================================================================
+# dtype check functions
+# =============================================================================
+def is_timedelta(timedeltastr):
+    try:
+        pd.to_timedelta(timedeltastr)
+        return True
+    except:
+        return False
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/df_helpers.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/df_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import sys
 import pandas as pd
 import numpy as np
 import geopandas as gpd
 import itertools
+from metobs_toolkit import observation_types
 
 
 def init_multiindex():
     return pd.MultiIndex(
         levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
     )
 
@@ -58,14 +59,76 @@
     """
 
     if "obstype" in outliersdf.index.names:
         return outliersdf.droplevel("obstype")
     else:
         return outliersdf
 
+def value_labeled_doubleidxdf_to_triple_idxdf(df,value_col_name='value', label_col_name = 'label'):
+    """
+    This function converts a double index dataframe with an 'obstype' column,
+    and a 'obstype_final_label' column to a triple index dataframe where the
+    obstype values are added to the index.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Dataframe with ['name', 'datetime'] as index and two columns: [obstype, obstype_final_label].
+        Where obstype is an observation type.
+    value_col_name : str, optional
+        Name of the column for the values. The default is 'value'.
+    label_col_name : str, optional
+        Name of the column for the labels. The default is 'label'.
+
+    Returns
+    -------
+    values : pd.DataFrame()
+        Dataframe with a ['name', 'datetime', obstype] index and two columnd:
+            [value_col_name, label_col_name]
+
+    """
+    if df.empty:
+        return df
+
+    present_obstypes = [col for col in df.columns if col in observation_types]
+
+    # get all values in triple index form
+    values = (df[present_obstypes].stack(dropna=False)
+              .reset_index()
+              .rename(columns={'level_2': 'obstype', 0: value_col_name})
+              .set_index(['name', 'datetime', 'obstype']))
+
+
+    # make a triple label dataframe
+    labelsdf = pd.DataFrame()
+    for obstype in present_obstypes:
+        subdf = df.loc[:, [obstype+'_final_label']]
+        subdf['obstype'] = obstype
+        subdf = subdf.reset_index()
+        subdf = subdf.set_index(['name', 'datetime', 'obstype'])
+        subdf = subdf.rename(columns={obstype+'_final_label': label_col_name})
+
+        labelsdf = pd.concat([labelsdf, subdf])
+
+    values[label_col_name] = labelsdf[label_col_name]
+
+    return values
+
+def _find_closes_occuring_date(refdt, series_of_dt, where="before"):
+    if where == "before":
+        diff = refdt - (series_of_dt[series_of_dt < refdt])
+    elif where == "after":
+        diff = (series_of_dt[series_of_dt > refdt]) - refdt
+
+    if diff.empty:
+        # no occurences before of after
+
+        return np.nan
+    else:
+        return min(diff).total_seconds()
 
 def remove_outliers_from_obs(obsdf, outliersdf):
     # TODO this function can only be used with care!!!
     # because all timestamps will be removed that have an oulier in one specific obstype !!!!
     return obsdf.loc[~obsdf.index.isin(outliersdf.index)]
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/gap.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/gap.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,17 +22,20 @@
     create_leading_trailing_debias_periods,
     make_era_bias_correction,
 )
 
 from metobs_toolkit.df_helpers import (
     format_outliersdf_to_doubleidx,
     get_likely_frequency,
+    _find_closes_occuring_date
 )
 
+from metobs_toolkit.df_helpers import init_multiindex, init_multiindexdf
 
+from metobs_toolkit.missingobs import Missingob_collection
 
 logger = logging.getLogger(__name__)
 
 
 # =============================================================================
 # Gap class
 
@@ -61,71 +64,126 @@
         None
 
         """
         # init attributes
         self.name = name
         self.startgap = startdt  # in IO space
         self.endgap = enddt  # in IO space
+        self.duration = enddt - startdt
 
         # computed attributes
         self.leading_timestamp = None  # last ob_dt before gap in datset space
+        self.leading_val = {} #keys are obstypes
         self.trailing_timestamp = None  # first ob_dt after gap in dataset space
+        self.trailing_val = {} #keys are obstypes
 
         self.exp_gap_idx = None
 
         # gap fill (only for conventional saving)
-        self.gapfill_values = None
-        self.gapfill_technique = None
+        self.gapfill_df = pd.DataFrame() #index: datetime, columns: obstypes, values: fill_values
+        self.gapfill_technique = None #will become a string
+        self.gapfill_info = None #only for the user
+        self.gapfill_errormessage = {} #keys are obstypes
+
 
     def __str__(self):
-        return f"Gap instance of {self.name} for {self.startgap} --> {self.endgap}"
+        return f"Gap instance of {self.name} for {self.startgap} --> {self.endgap}, duration: {self.duration}"
     def __repr__(self):
         return self.__str__()
 
+    def get_info(self):
+        print(f'Gap for {self.name} with: \n')
+        print(f'\n ---- Gap info ----- \n')
+        print(f'  * Start gap: {self.startgap} \n')
+        print(f'  * End gap: {self.endgap} \n')
+        print(f'  * Duration gap: {self.duration} \n')
+        print(f'\n ---- Gap fill info ----- \n')
+
+        obstypes = self.gapfill_df.columns.to_list()
+        if self.gapfill_df.empty:
+            print ('(No gapfill applied)')
+        elif self.gapfill_technique == 'interpolation':
+            for obstype in obstypes:
+                print(f'  * On observation type: {obstype}')
+                print(f'  * Technique: {self.gapfill_technique} \n')
+                print(f'  * Leading timestamp: {self.leading_timestamp} with  {obstype} = {self.leading_val[obstype]}\n')
+                print(f'  * Trailing timestamp: {self.trailing_timestamp} with  {obstype} = {self.trailing_val[obstype]}\n')
+                print(f'  * Filled values: {self.gapfill_df[obstype]} \n')
+                if obstype in self.gapfill_errormessage:
+                    print(f'  * Gapfill message: {self.gapfill_errormessage[obstype]} \n')
+
+
+        elif self.gapfill_technique == "debias gapfill":
+            for obstype in obstypes:
+                print(f'  * On observation type: {obstype}')
+                print(f'  * Technique: {self.gapfill_technique} \n')
+                # print(f'  * Leading timestamp: {self.leading_timestamp} with  {obstype} = {self.leading_val[obstype]}\n')
+                # print(f'  * Trailing timestamp: {self.trailing_timestamp} with  {obstype} = {self.trailing_val[obstype]}\n')
+                print(f'  * Filled values: {self.gapfill_df[obstype]} \n')
+                if obstype in self.gapfill_errormessage:
+                    print(f'  * Gapfill message: {self.gapfill_errormessage[obstype]} \n')
+        else:
+            print('technique not implemented in yet in show')
+
+
 
     def to_df(self):
         """
         Convert a Gap object to a dataframe (with one row). The station name is
         the index and two colums ('start_gap', 'end_gap') are constructed.
 
         Returns
         -------
         pandas.DataFrame()
             Gap in dataframe format.
 
         """
         return pd.DataFrame(
-            index=[self.name], data={"start_gap": self.startgap, "end_gap": self.endgap}
+            index=[self.name],
+            data={"start_gap": self.startgap,
+                  "end_gap": self.endgap,
+                  "duration": self.duration}
         )
 
-    def update_leading_trailing_obs(self, obsdf, outliersdf):
+    def update_leading_trailing_obs(self, obsdf, outliersdf, obs_only=False):
         """
         Add the leading (last obs before gap) and trailing (first obs after gap)
         as extra columns to the self.df.
 
-        The obsdf and outliersdf are both used to scan for the leading and trailing obs.
+        One can specify to look for leading and trailing in the obsdf or in both
+        the obsdf and outliersdf.
+
+        The gap leading and trailing timestamps and value attributes are updated.
+
+        If no leading/trailing timestamp is found, it is set to the gaps startdt/enddt.
 
         Parameters
         ----------
         obsdf : pandas.DataFrame
             Dataset.df
         outliersdf : pandas.DataFrame
             Dataset.outliersdf
+        obs_only: bool, optional
+            If True, only the obsdf will be used to search for leading and trailing.
 
         Returns
         -------
         None.
 
         """
-        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
-        # combine timestamps of observations and outliers
         sta_obs = obsdf.xs(self.name, level="name").index
-        sta_outl = outliersdf.xs(self.name, level="name").index
-        sta_comb = sta_obs.append(sta_outl)
+        if obs_only:
+            sta_comb = sta_obs
+        else:
+            outliersdf = format_outliersdf_to_doubleidx(outliersdf)
+
+            # combine timestamps of observations and outliers
+            sta_outl = outliersdf.xs(self.name, level="name").index
+            sta_comb = sta_obs.append(sta_outl)
 
         # find minimium timediff before
         before_diff = _find_closes_occuring_date(
             refdt=self.startgap, series_of_dt=sta_comb, where="before"
         )
 
         # if no timestamps are before gap, assume gap at the start of the observations
@@ -140,14 +198,28 @@
         if math.isnan(after_diff):
             after_diff = 0.0
 
         # get before and after timestamps
         self.leading_timestamp = self.startgap - timedelta(seconds=before_diff)
         self.trailing_timestamp = self.endgap + timedelta(seconds=after_diff)
 
+        # get the values
+        try:
+            self.leading_val = obsdf.loc[(self.name, self.leading_timestamp)].to_dict()
+        except KeyError:
+            print('LEADING VAL NOT IN OBSDF --> THIS IS NOT WHAT YOU WHANT I THINK ; FIX THIS')
+            self.leading_val = {}
+        try:
+            self.trailing_val = obsdf.loc[(self.name, self.trailing_timestamp)].to_dict()
+        except KeyError:
+            print('LEADING VAL NOT IN OBSDF --> THIS IS NOT WHAT YOU WHANT I THINK ; FIX THIS')
+            self.trailing_val = {}
+
+
+
     def update_gaps_indx_in_obs_space(self, obsdf, outliersdf, dataset_res):
         """
 
         Explode the gap, to the dataset resolution and format to a multiindex
         with name -- datetime.
 
         In addition the last observation before the gap (leading), and first
@@ -224,335 +296,332 @@
 
         Returns
         -------
         Pandas.Series
             Multiindex Series with filled gap values in dataset space.
 
         """
-
+        print(f' interpolate on {self}')
         outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
-        gapfill_series = interpolate_gap(
+        gapfill_series= interpolate_gap(
             gap=self,
             obsdf=obsdf,
             outliersdf=outliersdf,
             dataset_res=dataset_res,
             obstype=obstype,
             method=method,
             max_consec_fill=max_consec_fill,
         )
-        gapdf = gapfill_series.to_frame().reset_index()
-        gapdf["name"] = self.name
-        gapdf.index = pd.MultiIndex.from_arrays(
-            arrays=[gapdf["name"].values, gapdf["datetime"].values],
-            names=["name", "datetime"],
-        )
-        return gapdf[obstype]
 
-    def get_leading_trailing_debias_periods(self, station, obstype, debias_periods):
-        # get debias periods
+        # update self
+        self.gapfill_technique = 'interpolation'
+        self.gapfill_df[obstype] = gapfill_series
 
-        leading_period, trailing_period = create_leading_trailing_debias_periods(
-            station=station,
-            gap=self,
-            debias_period_settings=debias_periods,
-            obstype=obstype,
-        )
 
-        return leading_period, trailing_period
 
 
-class Gap_collection:
-    def __init__(self, gapsdf):
-        self.list = [
-            Gap(sta, row["start_gap"], row["end_gap"]) for sta, row in gapsdf.iterrows()
-        ]
-
-    def __str__(self):
-        if not bool(self.list):
-            return f'Empty gap collection'
-        longstring = ''
-        for gap in self.list:
-            longstring += str(gap) + '\n'
-        return f"Gap collection for: \n {longstring}"
-    def __repr__(self):
-        return self.__str__()
 
-    def to_df(self):
-        gaps_names = []
-        gaps_startdt = []
-        gaps_enddt = []
-        for gap in self.list:
-            gaps_names.append(gap.name)
-            gaps_startdt.append(gap.startgap)
-            gaps_enddt.append(gap.endgap)
-
-        df = pd.DataFrame(
-            index=pd.Index(gaps_names),
-            data={"start_gap": gaps_startdt, "end_gap": gaps_enddt},
-        )
-        df.index.name = "name"
+# =============================================================================
+# Find gaps and missing values
+# =============================================================================
+def get_station_gaps(gapslist, name):
+       """
+       Extract a Gap_collection specific to one station. If no gaps are found
+       for the station, an empty Gap_collection is returned.
+
+       Parameters
+       ----------
+       name : String
+           Name of the station to extract a Gaps_collection from.
+
+       Returns
+       -------
+       Gap_collection
+           A Gap collection specific of the specified station.
 
-        return df
+       """
+       return [gap for gap in gapslist if gap.name == name]
 
-    def get_station_gaps(self, name):
-        """
-        Extract a Gap_collection specific to one station. If no gaps are found
-        for the station, an empty Gap_collection is returned.
 
-        Parameters
-        ----------
-        name : String
-            Name of the station to extract a Gaps_collection from.
+def get_gaps_indx_in_obs_space(gapslist, obsdf, outliersdf, resolutionseries):
+    """
 
-        Returns
-        -------
-        Gap_collection
-            A Gap collection specific of the specified station.
+    Explode the gaps, to the dataset resolution and format to a multiindex
+    with name -- datetime.
 
-        """
-        gapdf = self.to_df()
+    In addition the last observation before the gap (leading), and first
+    observation (after) the gap are computed and stored in the df attribute.
+    (the outliers are used to look for leading and trailing observations.)
 
-        if name in gapdf.index:
-            return Gap_collection(gapdf.loc[name])
-        else:
-            return Gap_collection(pd.DataFrame())
 
-    def remove_gaps_from_obs(self, obsdf):
-        """
-        Remove station - datetime records that are in the gaps from the obsdf.
+    Parameters
+    ----------
+    obsdf : TYPE
+        DESCRIPTION.
+    outliersdf : TYPE
+        DESCRIPTION.
+    resolutionseries : TYPE
+        DESCRIPTION.
 
-        (Usefull when filling timestamps to a df, and if you whant to remove the
-         gaps.)
+    Returns
+    -------
+    expanded_gabsidx_obsspace : TYPE
+        DESCRIPTION.
 
-        Parameters
-        ----------
-        obsdf : pandas.DataFrame()
-            A MultiIndex dataframe with name -- datetime as index.
+    """
+    outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
-        Returns
-        -------
-        obsdf : pandas.DataFrame()
-            The same dataframe with records inside gaps removed.
+    expanded_gabsidx_obsspace = init_multiindex()
 
-        """
 
-        # Create index for gaps records in the obsdf
-        expanded_gabsidx = pd.MultiIndex(
-            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
+    for gap in gapslist:
+        gap.update_gaps_indx_in_obs_space(
+            obsdf, outliersdf, resolutionseries.loc[gap.name]
+        )
+        expanded_gabsidx_obsspace = expanded_gabsidx_obsspace.append(
+            gap.exp_gap_idx
         )
 
-        for gap in self.list:
-            sta_records = obsdf.xs(gap.name, level="name").index  # filter by name
 
-            gaps_dt = sta_records[
-                (sta_records >= gap.startgap)
-                & (  # filter if the observations are within a gap
-                    sta_records <= gap.endgap
-                )
-            ]
+    return expanded_gabsidx_obsspace
 
-            gaps_multiidx = pd.MultiIndex.from_arrays(
-                arrays=[[gap.name] * len(gaps_dt), gaps_dt], names=["name", "datetime"]
-            )
 
-            expanded_gabsidx = expanded_gabsidx.append(gaps_multiidx)
+def gaps_to_df(gapslist):
+    """
+    Combine all gaps into a dataframe as an overview.
 
-        # remove gaps idx from the obsdf
-        obsdf = obsdf.drop(index=expanded_gabsidx)
-        return obsdf
+    Parameters
+    ----------
+    gapslist : list
+        List of gaps.
 
-    def get_gaps_indx_in_obs_space(self, obsdf, outliersdf, resolutionseries):
-        """
+    Returns
+    -------
+    pandas.DataFrame
+        A DataFrame with stationnames as index, and the start, end and duretion
+        of the gaps as columns.
 
-        Explode the gaps, to the dataset resolution and format to a multiindex
-        with name -- datetime.
+    """
 
-        In addition the last observation before the gap (leading), and first
-        observation (after) the gap are computed and stored in the df attribute.
-        (the outliers are used to look for leading and trailing observations.)
 
+    gapdflist = []
+    for gap in gapslist:
+        gapdflist.append(gap.to_df())
 
-        Parameters
-        ----------
-        obsdf : TYPE
-            DESCRIPTION.
-        outliersdf : TYPE
-            DESCRIPTION.
-        resolutionseries : TYPE
-            DESCRIPTION.
+    return pd.concat(gapdflist)
 
-        Returns
-        -------
-        expanded_gabsidx_obsspace : TYPE
-            DESCRIPTION.
+def remove_gaps_from_obs(gaplist, obsdf):
+    """
+    Remove station - datetime records that are in the gaps from the obsdf.
 
-        """
-        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
+    (Usefull when filling timestamps to a df, and if you whant to remove the
+      gaps.)
 
-        expanded_gabsidx_obsspace = pd.MultiIndex(
-            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
-        )
+    Parameters
+    ----------
+    obsdf : pandas.DataFrame()
+        A MultiIndex dataframe with name -- datetime as index.
 
-        for gap in self.list:
-            gap.update_gaps_indx_in_obs_space(
-                obsdf, outliersdf, resolutionseries.loc[gap.name]
-            )
-            expanded_gabsidx_obsspace = expanded_gabsidx_obsspace.append(
-                gap.exp_gap_idx
-            )
+    Returns
+    -------
+    obsdf : pandas.DataFrame()
+        The same dataframe with records inside gaps removed.
 
-        return expanded_gabsidx_obsspace
+    """
 
-    def apply_interpolate_gaps(
-        self,
-        obsdf,
-        outliersdf,
-        dataset_res,
-        obstype="temp",
-        method="time",
-        max_consec_fill=100,
-    ):
-        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
+    # Create index for gaps records in the obsdf
+    expanded_gabsidx = init_multiindex()
+    for gap in gaplist:
+        sta_records = obsdf.xs(gap.name, level="name").index  # filter by name
+
+        gaps_dt = sta_records[
+            (sta_records >= gap.startgap)
+            & (  # filter if the observations are within a gap
+                sta_records <= gap.endgap
+            )
+        ]
 
-        expanded_gabsidx_obsspace = pd.MultiIndex(
-            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
-        )
-        filled_gaps_series = pd.Series(
-            data=[], index=expanded_gabsidx_obsspace, dtype=object
+        gaps_multiidx = pd.MultiIndex.from_arrays(
+            arrays=[[gap.name] * len(gaps_dt), gaps_dt], names=["name", "datetime"]
         )
 
-        for gap in self.list:
-            gapfill_series = interpolate_gap(
-                gap=gap,
-                obsdf=obsdf,
-                outliersdf=outliersdf,
-                dataset_res=dataset_res.loc[gap.name],
-                obstype=obstype,
-                method=method,
-                max_consec_fill=max_consec_fill,
-            )
+        expanded_gabsidx = expanded_gabsidx.append(gaps_multiidx)
 
-            gapdf = gapfill_series.to_frame().reset_index()
-            gapdf["name"] = gap.name
-            gapdf = gapdf.set_index(['name', 'datetime'])
-            # gapdf.index = pd.MultiIndex.from_arrays(
-            #     arrays=[gapdf["name"].values, gapdf["datetime"].values],
-            #     names=["name", "datetime"],
-            # )
-
-            # Update gap
-            gap.gapfill_technique = "interpolation"
-            gap.gapfill_values = gapdf[obstype]
+    # remove gaps idx from the obsdf
+    obsdf = obsdf.drop(index=expanded_gabsidx)
+    return obsdf
 
-            filled_gaps_series = pd.concat([filled_gaps_series, gapdf[obstype]])
-        return filled_gaps_series
+# =============================================================================
+# Helpers
+# =============================================================================
 
-    def apply_debias_era5_gapfill(
-        self, dataset, eraModelData, debias_settings, obstype="temp"
+
+# def _find_closes_occuring_date(refdt, series_of_dt, where="before"):
+#     if where == "before":
+#         diff = refdt - (series_of_dt[series_of_dt < refdt])
+#     elif where == "after":
+#         diff = (series_of_dt[series_of_dt > refdt]) - refdt
+
+#     if diff.empty:
+#         # no occurences before of after
+
+#         return np.nan
+#     else:
+#         return min(diff).total_seconds()
+
+
+
+def apply_debias_era5_gapfill(
+        gapslist, dataset, eraModelData, debias_settings, obstype="temp",
     ):
-        expanded_gabsidx_obsspace = pd.MultiIndex(
-            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
-        )
+
+        gapfill_settings = dataset.settings.gap['gaps_fill_info']
+        expanded_gabsidx_obsspace = init_multiindex()
+
         filled_gaps_series = pd.Series(
             data=[], index=expanded_gabsidx_obsspace, dtype=object
         )
 
-        for gap in self.list:
+        # Convert modeldata to the same timzone as the data
+        targettz = dataset.df.index.get_level_values('datetime').tz.zone
+        eraModelData._conv_to_timezone(targettz)
+
+
+        for gap in gapslist:
+            print(f' Era5 gapfill for {gap}')
+            gap.gapfill_technique = "debias gapfill"
+
             # avoid passing full dataset around
             station = dataset.get_station(gap.name)
 
             # Update gap attributes
             gap.update_gaps_indx_in_obs_space(
                 obsdf=station.df,
                 outliersdf=station.outliersdf,
                 dataset_res=station.metadf["dataset_resolution"].squeeze(),
             )
 
             # get leading and trailing period
-            leading_obs, trailing_obs = gap.get_leading_trailing_debias_periods(
+            leading_obs, trailing_obs = create_leading_trailing_debias_periods(
+                station=station,
+                gap=gap,
+                debias_period_settings=debias_settings["debias_period"],
                 obstype=obstype,
-                station=dataset.get_station(gap.name),
-                debias_periods=debias_settings["debias_period"],
             )
+
             # check if leading/trailing is valid
             if leading_obs.empty | trailing_obs.empty:
                 print(
                     "No suitable leading or trailing period found. Gapfill not possible"
                 )
-                gap.gapfill_technique = (
-                    "debias era5 gapfill (not possible: no leading/trailing period)"
-                )
+                gap.gapfill_errormessage[obstype] = 'gapfill not possible: no leading/trailing period'
+
                 default_return = pd.Series(
                     index=gap.exp_gap_idx, name=obstype, dtype="object"
                 )
-                gap.gapfill_values = default_return
-                filled_gaps_series = pd.concat([filled_gaps_series, default_return])
+
+                default_return.name = obstype
+                gapfill_df =default_return.to_frame()
+                gapfill_df[obstype + "_" + gapfill_settings["label_columnname"]] = gapfill_settings["label"]["model_debias"]
+
+                # update the gaps attributes
+                gap.gapfill_df = gapfill_df
+
                 continue
 
             # extract model values at leading and trailing period
             leading_model = eraModelData.interpolate_modeldata(leading_obs.index)
             trailing_model = eraModelData.interpolate_modeldata(trailing_obs.index)
 
             # TODO check if there is modeldata for the leading and trailing + obs period
             if (leading_model[obstype].isnull().any()) | (
                 trailing_model[obstype].isnull().any()
             ):
                 print(
                     "No modeldata for the full leading/trailing period found. Gapfill not possible"
                 )
-                gap.gapfill_technique = (
-                    "debias era5 gapfill (not possible: not enough modeldata)"
-                )
+                gap.gapfill_errormessage[obstype] = 'gapfill not possible: not enough modeldata'
+
                 default_return = pd.Series(
                     index=gap.exp_gap_idx, name=obstype, dtype="object"
                 )
-                gap.gapfill_values = default_return
-                filled_gaps_series = pd.concat([filled_gaps_series, default_return])
+                default_return.name = obstype
+                gapfill_df =default_return.to_frame()
+                gapfill_df[obstype + "_" + gapfill_settings["label_columnname"]] = gapfill_settings["label"]["model_debias"]
+
+                # update the gaps attributes
+                gap.gapfill_df = gapfill_df
+                continue
 
             # Get model data for gap timestamps
             gap_model = eraModelData.interpolate_modeldata(gap.exp_gap_idx)
 
             # apply bias correction
-            filled_gap_series = make_era_bias_correction(
+            filled_gap_series, fill_info, err_message = make_era_bias_correction(
                 leading_model=leading_model,
                 trailing_model=trailing_model,
                 gap_model=gap_model,
                 leading_obs=leading_obs,
                 trailing_obs=trailing_obs,
                 obstype=obstype,
             )
 
-            # Update gap
-            gap.gapfill_technique = "debias era5 gapfill"
-            gap.gapfill_values = filled_gap_series
 
-            filled_gaps_series = pd.concat([filled_gaps_series, filled_gap_series])
+            filled_gap_series.name = obstype
+            gapfill_df =filled_gap_series.to_frame()
+            gapfill_df[obstype + "_" + gapfill_settings["label_columnname"]] = gapfill_settings["label"]["model_debias"]
+
+            # update the gaps attributes
+            gap.gapfill_df = gapfill_df
+            gap.gapfill_technique = gapfill_settings["label"]["model_debias"]
+            gap.gapfill_info = fill_info
+            if bool(err_message):
+                gap.gapfill_errormessage = err_message
+
 
-        filled_gaps_series.name = obstype
-        return filled_gaps_series
 
 
-# =============================================================================
-# Find gaps and missing values
-# =============================================================================
 
+def apply_interpolate_gaps(gapslist, obsdf, outliersdf, dataset_res, gapfill_settings,
+                           obstype="temp", method="time", max_consec_fill=100,
+                           ):
 
-def _find_closes_occuring_date(refdt, series_of_dt, where="before"):
-    if where == "before":
-        diff = refdt - (series_of_dt[series_of_dt < refdt])
-    elif where == "after":
-        diff = (series_of_dt[series_of_dt > refdt]) - refdt
-
-    if diff.empty:
-        # no occurences before of after
-
-        return np.nan
-    else:
-        return min(diff).total_seconds()
+    """ No return, only update the gaps instances attributes"""
+
+    for gap in gapslist:
+        gapfill_series = interpolate_gap(
+                        gap=gap,
+                        obsdf=obsdf.xs(gap.name, level='name', drop_level=False),
+                        outliersdf=outliersdf.xs(gap.name, level='name', drop_level=False),
+                        dataset_res=dataset_res.loc[gap.name],
+                        obstype=obstype,
+                        method=method,
+                        max_consec_fill=max_consec_fill,
+                        )
+
+        gapfill_series.name = obstype
+        gapfill_df = gapfill_series.to_frame()
+        gapfill_df[obstype + "_" + gapfill_settings["label_columnname"]] = gapfill_settings["label"]["linear"]
+
+        # update the gaps attributes
+        gap.gapfill_df = gapfill_df
+        gap.gapfill_technique = gapfill_settings["label"]["linear"]
+
+
+def make_gapfill_df(gapslist):
+    concatlist = []
+    for gap in gapslist:
+        subgapfill = gap.gapfill_df.reset_index()
+        subgapfill['name'] = gap.name
+        subgapfill = subgapfill.set_index(['name', 'datetime'])
+
+        concatlist.append(subgapfill)
+
+    return pd.concat(concatlist).sort_index()
 
 
 def missing_timestamp_and_gap_check(df, gapsize_n):
     # TODO update docstring
     """
 
     V3
@@ -576,16 +645,17 @@
     outlier_df : pandas.DataFrame()
         The dataframe containing the missing timestamps (not gaps) with the outlier label.
     gap_df : pandas.Dataframe()
         The dataframe containing the start and end date of a specific gap.
 
     """
 
-    gap_df = pd.DataFrame()
-    gap_indices = []
+    gap_list = []
+    # gap_df = pd.DataFrame()
+    # gap_indices = []
     missing_timestamp_series = pd.Series(dtype=object)
     station_freqs = {}
 
     # missing timestamp per station (because some stations can have other frequencies!)
 
     stationnames = df.index.get_level_values(level="name").unique()
     for station in stationnames:
@@ -614,43 +684,21 @@
         consec_missing_groups = missing_datetimeseries.groupby(gap_defenition)
         group_sizes = consec_missing_groups.size()
 
         gap_groups = group_sizes[group_sizes > gapsize_n]
 
         # iterate over the gabs and fill the gapsdf
         for gap_idx in gap_groups.index:
-            # fill the gaps df
             datetime_of_gap_records = consec_missing_groups.get_group(gap_idx).index
-            gap_df = pd.concat(
-                [
-                    gap_df,
-                    pd.DataFrame(
-                        data=[
-                            [
-                                datetime_of_gap_records.min(),
-                                datetime_of_gap_records.max(),
-                            ]
-                        ],
-                        index=[station],
-                        columns=["start_gap", "end_gap"],
-                    ),
-                ]
-            )
+            gap = Gap(name=station,
+                      startdt=datetime_of_gap_records.min(),
+                      enddt=datetime_of_gap_records.max())
+            gap_list.append(gap)
+
 
-            logger.debug(
-                f"Data gap from {datetime_of_gap_records.min()} --> {datetime_of_gap_records.max()} found for {station}."
-            )
-            gap_indices.extend(
-                list(
-                    zip(
-                        [station] * datetime_of_gap_records.shape[0],
-                        datetime_of_gap_records,
-                    )
-                )
-            )
 
         # combine the missing timestams values
         missing_timestamp_groups = group_sizes[group_sizes <= gapsize_n]
         for missing_idx in missing_timestamp_groups.index:
             datetime_of_missing_records = consec_missing_groups.get_group(
                 missing_idx
             ).index.to_list()
@@ -661,10 +709,13 @@
                     pd.Series(
                         index=[station] * len(datetime_of_missing_records),
                         data=datetime_of_missing_records,
                     ),
                 ]
             )
 
+    missing_obs_collection = Missingob_collection(missing_timestamp_series)
     df = df.sort_index()
 
-    return df, missing_timestamp_series, gap_df
+    return missing_obs_collection, gap_list
+
+
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/gap_filling.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/gap_filling.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,75 +27,98 @@
 
 def interpolate_gap(
     gap, obsdf, outliersdf, dataset_res, obstype, method, max_consec_fill
 ):
     outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
     # 1 get trailing and leading + exploded index
-    gap.update_leading_trailing_obs(obsdf, outliersdf)
     gap.update_gaps_indx_in_obs_space(obsdf, outliersdf, dataset_res)
+    gap.update_leading_trailing_obs(obsdf, outliersdf, obs_only=True)
 
     # initiate return value when no interpolation can be performed
     empty_interp = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel("name"))
     empty_interp.name = obstype
 
     # 2 check if there is a trailing and leading gap
     if gap.startgap == gap.leading_timestamp:
-        print(
-            f"No leading timestamp found for gap ({gap.name}): {gap.startgap} --> {gap.endgap}"
-        )
+        message =f"No leading timestamp found for gap {gap}"
+        print(message)
+        gap.gapfill_errormessage[obstype]=message
         return empty_interp
 
     if gap.endgap == gap.trailing_timestamp:
-        print(
-            f"No trailing timestamp found for gap ({gap.name}): {gap.startgap} --> {gap.endgap}"
-        )
+        message = f"No trailing timestamp found for gap {gap}"
+        print(message)
+        gap.gapfill_errormessage[obstype]=message
         return empty_interp
 
-    # 3 check both leading and trailing are in obs, and look for alternative leading/trailing if the original is an outlier.
-    sta_obs = obsdf.xs(gap.name, level="name")
 
-    # leading
-    if gap.leading_timestamp in sta_obs.index:
-        # leading found in obs
-        leading_dt = gap.leading_timestamp
-        leading_val = sta_obs.loc[gap.leading_timestamp, obstype]
-    else:
-        # look for last observation before leading timestamp
-        delta_dt = (
-            gap.leading_timestamp - sta_obs.index[sta_obs.index < gap.leading_timestamp]
-        )
-        if delta_dt.empty:
-            print(
-                f"No cadidate for leading {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
-            )
-            return empty_interp
+    # 3. Get leading and trailing val
+    if not bool(gap.leading_val):
+        # empty dict --> no value in the obs
+        message =f"No cadidate for leading {obstype} observation found for {gap}"
+        print(message)
+        gap.gapfill_errormessage[obstype]=message
+        return empty_interp
 
-        leading_dt = gap.leading_timestamp - delta_dt.min()
-        leading_val = sta_obs.loc[leading_dt, obstype]
+    if not bool(gap.trailing_val):
+        # empty dict --> no value in the obs
+        message =f"No cadidate for trailing {obstype} observation found for {gap}"
+        print(message)
+        gap.gapfill_errormessage[obstype]=message
+        return empty_interp
 
-    # trailing
-    if gap.trailing_timestamp in sta_obs.index:
-        # leading found in obs
-        trailing_dt = gap.trailing_timestamp
-        trailing_val = sta_obs.loc[gap.trailing_timestamp, obstype]
-    else:
-        # look for last observation before leading timestamp
-        delta_dt = (
-            sta_obs.index[sta_obs.index > gap.trailing_timestamp]
-            - gap.trailing_timestamp
-        )
-        if delta_dt.empty:
-            print(
-                f"No cadidate for trailing {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
-            )
-            return empty_interp
-        # TODO: settings restrictions on maximum delta_dt ??
-        trailing_dt = gap.trailing_timestamp + delta_dt.min()
-        trailing_val = sta_obs.loc[trailing_dt, obstype]
+
+    leading_dt = gap.leading_timestamp
+    leading_val = gap.leading_val[obstype]
+    trailing_dt = gap.trailing_timestamp
+    trailing_val = gap.trailing_val[obstype]
+
+
+    # # 3 check both leading and trailing are in obs, and look for alternative leading/trailing if the original is an outlier.
+    # sta_obs = obsdf.xs(gap.name, level="name")
+
+    # # leading
+    # if gap.leading_timestamp in sta_obs.index:
+    #     # leading found in obs
+    #     leading_dt = gap.leading_timestamp
+    #     leading_val = sta_obs.loc[gap.leading_timestamp, obstype]
+    # else:
+    #     # look for last observation before leading timestamp
+    #     delta_dt = (
+    #         gap.leading_timestamp - sta_obs.index[sta_obs.index < gap.leading_timestamp]
+    #     )
+    #     if delta_dt.empty:
+    #         print(
+    #             f"No cadidate for leading {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
+    #         )
+    #         return empty_interp
+
+    #     leading_dt = gap.leading_timestamp - delta_dt.min()
+    #     leading_val = sta_obs.loc[leading_dt, obstype]
+
+    # # trailing
+    # if gap.trailing_timestamp in sta_obs.index:
+    #     # leading found in obs
+    #     trailing_dt = gap.trailing_timestamp
+    #     trailing_val = sta_obs.loc[gap.trailing_timestamp, obstype]
+    # else:
+    #     # look for last observation before leading timestamp
+    #     delta_dt = (
+    #         sta_obs.index[sta_obs.index > gap.trailing_timestamp]
+    #         - gap.trailing_timestamp
+    #     )
+    #     if delta_dt.empty:
+    #         print(
+    #             f"No cadidate for trailing {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
+    #         )
+    #         return empty_interp
+    #     # TODO: settings restrictions on maximum delta_dt ??
+    #     trailing_dt = gap.trailing_timestamp + delta_dt.min()
+    #     trailing_val = sta_obs.loc[trailing_dt, obstype]
 
     # Make interpolation series
     gaps_series = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel("name"))
     gaps_series = pd.concat(
         [
             gaps_series,
             pd.Series(
@@ -110,18 +133,22 @@
         method=method,
         limit=max_consec_fill,  # Maximum number of consecutive NaNs to fill. Must be greater than 0.
         limit_area="inside",
         inplace=True,
     )
 
     # Subset only gap indixes
-    gaps_series = gaps_series[gap.exp_gap_idx.droplevel("name")]
-    gaps_series.name = obstype
+    gaps_fill_series = gaps_series[gap.exp_gap_idx.droplevel("name")]
+    gaps_fill_series.name = obstype
 
-    return gaps_series
+    # update gapfill info
+    gap.gapfill_info = gaps_series.to_frame()
+
+
+    return gaps_fill_series
 
 
 # =============================================================================
 # Debiasing period
 # =============================================================================
 
 
@@ -163,14 +190,15 @@
     # only datetimes are relevant
     obs = obs.reset_index()
     obs = obs[["name", "datetime", obstype]]
 
     # Select all leading and all trailing obs
     leading_period = obs[obs["datetime"] < gap.startgap]
     trailing_period = obs[obs["datetime"] > gap.endgap]
+    print(f'   {leading_period.shape[0]} leading records, {trailing_period.shape[0]} trailing records.')
 
     # some derived integers
     poss_shrinkage_leading = leading_period.shape[0] - debias_min_sample_size_leading
     poss_shrinkage_trailing = trailing_period.shape[0] - debias_min_sample_size_trailing
     poss_extention_leading = leading_period.shape[0] - debias_pref_sample_size_leading
     poss_extention_trailing = (
         trailing_period.shape[0] - debias_pref_sample_size_trailing
@@ -330,17 +358,18 @@
     biases = diff.groupby(["name", "hours", "minutes", "seconds"])[obstype].mean()
     biases.name = obstype + "_bias_" + period
 
     biases = biases.reset_index()
     return biases
 
 
-def make_era_bias_correction(
-    leading_model, trailing_model, gap_model, leading_obs, trailing_obs, obstype
-):
+def make_era_bias_correction(leading_model, trailing_model,
+                             gap_model, leading_obs, trailing_obs,
+                             obstype):
+    error_message = ''
     # 1. get lead timestamp biases
     lead_biases = get_time_specific_biases(
         model=leading_model, obs=leading_obs, obstype=obstype, period="lead"
     )
 
     # 2. get trailing timestamp biases
     trail_biases = get_time_specific_biases(
@@ -354,35 +383,50 @@
     gap_model["lead_weight"] = 1.0 - gap_model["trail_weight"]
 
     # aggregate to timestamps
     gap_model["hours"] = gap_model.index.get_level_values("datetime").hour
     gap_model["minutes"] = gap_model.index.get_level_values("datetime").minute
     gap_model["seconds"] = gap_model.index.get_level_values("datetime").second
 
-    # 4. merge biases and model values together
-    gap_debias = gap_model.merge(
+
+    # testing
+    gap_model = gap_model.reset_index()
+
+    gap_model = gap_model.merge(
         right=lead_biases[["hours", "minutes", "seconds", obstype + "_bias_lead"]],
         how="left",
         on=["hours", "minutes", "seconds"],
     )
 
-    gap_debias = gap_debias.merge(
-        right=trail_biases[["hours", "minutes", "seconds", obstype + "_bias_trail"]],
-        how="left",
-        on=["hours", "minutes", "seconds"],
-    )
+    gap_model = gap_model.merge(
+         right=trail_biases[["hours", "minutes", "seconds", obstype + "_bias_trail"]],
+         how="left",
+         on=["hours", "minutes", "seconds"],
+     )
+
+    gap_model = gap_model.set_index(['name', 'datetime'])
+
+    # Idea: if BOTH leadin and trailing (hourly) biases is available, than use
+    # use the debias corection (even if it is for a part of the gap!).
+    # If either one or both are missing, than no bias correction is applied
+    no_debias = gap_model[(gap_model[obstype + '_bias_lead'].isnull()) |
+                          (gap_model[obstype + '_bias_trail'].isnull())].index
+    error_message =f'WARNING!, No debias possible for these gap records: {no_debias},the gap will be filled by model data without bias correction. '
+    print(error_message)
+
+
+    # set weights to zero if not debias correction can be applied on that record
+    gap_model.loc[no_debias, obstype+'_bias_trail'] = 0.
+    gap_model.loc[no_debias, obstype+'_bias_lead'] = 0.
 
-    gap_debias.index = (
-        gap_model.index
-    )  # TODO: this might be dangerous, but the merge removes the index ??
 
     # 5. compute the debiased fill value
     # leave this dataframe for debugging
-    gap_debias[obstype + "_fill"] = gap_debias[obstype] - (
-        (gap_debias["lead_weight"] * gap_debias[obstype + "_bias_lead"])
-        + (gap_debias["trail_weight"] * gap_debias[obstype + "_bias_trail"])
+    gap_model[obstype + "_fill"] = gap_model[obstype] - (
+        (gap_model["lead_weight"] * gap_model[obstype + "_bias_lead"])
+        + (gap_model["trail_weight"] * gap_model[obstype + "_bias_trail"])
     )
 
     # 6. make returen
-    returnseries = gap_debias[obstype + "_fill"]
+    returnseries = gap_model[obstype + "_fill"]
     returnseries.name = obstype
-    return returnseries
+    return returnseries, gap_model, error_message
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/geometry_functions.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/landcover_functions.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/landcover_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,50 +48,45 @@
         metadf=relevant_metadf, mapinfo=mapinfo, output_column_name="lcz"
     )
     return lcz_df["lcz"]  # return series
 
 
 def lc_fractions_extractor(metadf, mapinfo, buffer, agg):
     # make return in case something went wrong
-    default_return = pd.DataFrame(index=metadf.index)
+    default_return = (pd.DataFrame(index=metadf.index), buffer)
 
     # test if metadata is suitable
     if not _validate_metadf(metadf):
         print(f"Metadf is not suitable for GEE extractiond: {metadf}")
         return default_return
 
     relevant_metadf = metadf.reset_index()[["name", "lat", "lon"]]
 
     freqs_df = extract_buffer_frequencies(
         metadf=relevant_metadf, mapinfo=mapinfo, bufferradius=buffer
     )
 
     # apply aggregation if required
     if agg:
-        print("aggregateion")
+        print(f"Using aggregation scheme: {mapinfo['aggregation']}")
         agg_df = pd.DataFrame()
         for agg_name, agg_classes in mapinfo["aggregation"].items():
             present_agg_classes = [
                 str(num) for num in agg_classes if str(num) in freqs_df.columns
             ]
-            agg_df[agg_name + "_" + str(buffer) + "m"] = freqs_df[
-                present_agg_classes
-            ].sum(axis=1)
+            agg_df[agg_name] = freqs_df[present_agg_classes].sum(axis=1)
 
-        return agg_df
+        return agg_df, buffer
 
     else:
         # map numeric classes to human
-        mapper = {
-            str(num): human + "_" + str(buffer) + "m"
-            for num, human in mapinfo["categorical_mapper"].items()
-        }
+        mapper = {str(num): human for num, human in mapinfo["categorical_mapper"].items()}
         freqs_df = freqs_df.rename(columns=mapper)
 
-        return freqs_df
+        return freqs_df, buffer
 
 
 def height_extractor(metadf, mapinfo):
     # make return in case something went wrong
     default_return = pd.Series(
         index=metadf.index, data="Location_unknown", name="altitude", dtype=object
     )
@@ -113,15 +108,18 @@
 # Object convertors
 # =============================================================================
 
 
 def _datetime_to_gee_datetime(datetime):
     # covert to UTC!
     utcdt = datetime.astimezone(pytz.utc)
-    return ee.Date(utcdt.strftime("%Y-%m-%dT%H:%M:%S"))
+    print(utcdt.replace(tzinfo=None))
+    return ee.Date(utcdt.replace(tzinfo=None))
+    # print(f'formaat:   {utcdt.strftime("%Y-%m-%dT%H:%M:%S")}')
+    # return ee.Date(utcdt.strftime("%Y-%m-%dT%H:%M:%S"))
 
 
 def get_ee_obj(mapinfo, band=None):
     if mapinfo["is_image"]:
         obj = ee.Image(mapinfo["location"])
     elif mapinfo["is_imagecollection"]:
         if isinstance(band, type(None)):
@@ -462,14 +460,16 @@
     def rasterExtraction(image):
         feature = image.sampleRegions(
             collection=ee_fc,  # feature collection here
             scale=scale,  # Cell size of raster
         )
         return feature
 
+    print(f'startdtfilter: { _datetime_to_gee_datetime(startdt).getInfo()}')
+    print(f'enddtfilter: { _datetime_to_gee_datetime(enddt).getInfo()}')
     raster = get_ee_obj(mapinfo, bandname)  # dataset
     results = (
         raster.filter(
             ee.Filter.date(
                 _datetime_to_gee_datetime(startdt), _datetime_to_gee_datetime(enddt)
             )
         )
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/missingobs.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/missingobs.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 import pandas as pd
 import numpy as np
 from datetime import datetime, timedelta
 import logging
 
-from metobs_toolkit.gap import _find_closes_occuring_date
+from metobs_toolkit.df_helpers import _find_closes_occuring_date
 
 logger = logging.getLogger(__name__)
 
 # =============================================================================
 # Missing observation
 
 # a missing observation is a missing timestamp
@@ -25,24 +25,41 @@
 
 class Missingob_collection:
     """ Class object handling a set of missing observations. """
     def __init__(self, missing_obs_series):
 
         missing_obs_series.name = 'datetime'
         missing_obs_series.index.name = 'name'
+
+        missing_obs_series = missing_obs_series.drop_duplicates()
+        missing_obs_series = missing_obs_series.sort_index()
+
         missing_idx = missing_obs_series.reset_index()
         missing_idx = missing_idx.set_index(['name', 'datetime'])
 
         self.series = missing_obs_series
         self.idx = missing_idx.index
 
         # gap fill (only for conventional saving)
         self.fill_df = pd.DataFrame()
         self.fill_technique = None
 
+    def __add__(self, other):
+        comb_series = pd.concat([self.series, other.series])
+
+        comb_series = comb_series.drop_duplicates()
+        comb_series = comb_series.sort_index()
+
+        self.series = comb_series
+        comb_idx = comb_series.reset_index()
+        comb_idx = comb_idx.set_index(['name', 'datetime'])
+        self.idx = comb_idx.index
+        return self
+
+
     def __str__(self):
         if self.series.empty:
             return f'Empty missing observations.'
         if not self.fill_df.empty:
             return f'Missing observations with filled ({self.fill_technique}) \
                 values: \n {self.fill_df} \n Original missing observations on import: \n {self.idx}'
 
@@ -133,28 +150,33 @@
         self.fill_df = pd.DataFrame(index=missing_obsspace)
 
 
         for staname, missingdt in missing_obsspace:
             staobs = obsdf.xs(staname, level='name')[obstype]
             # exclude nan values because they are no good leading/trailing
             staobs = staobs[~staobs.isnull()]
-
+            print(f'staname: {staname}, missingdt: {missingdt}')
             # find leading and trailing datetimes
-            leading_dt = missingdt - timedelta(
-                seconds=_find_closes_occuring_date(
-                    refdt = missingdt,
-                    series_of_dt = staobs.index,
-                    where='before')
-                )
-            trailing_dt = missingdt + timedelta(
-                seconds=_find_closes_occuring_date(
-                    refdt = missingdt,
-                    series_of_dt = staobs.index,
-                    where='after')
-                )
+            leading_seconds =_find_closes_occuring_date(refdt = missingdt,
+                                                        series_of_dt = staobs.index,
+                                                        where='before')
+            if np.isnan(leading_seconds):
+                logger.warn(f'missing obs: {staname}, at {missingdt} does not have a leading timestamp.')
+                continue
+
+            leading_dt = missingdt - timedelta(seconds=leading_seconds)
+
+            trailing_seconds =_find_closes_occuring_date(
+                                                    refdt = missingdt,
+                                                    series_of_dt = staobs.index,
+                                                    where='after')
+            if np.isnan(trailing_seconds):
+                logger.warn(f'missing obs: {staname}, at {missingdt} does not have a trailing timestamp.')
+                continue
+            trailing_dt = missingdt + timedelta(seconds=trailing_seconds)
 
             # extract the values and combine them in a dataframe
             leading_val = staobs.loc[leading_dt]
             trailing_val = staobs.loc[trailing_dt]
 
             stadf = pd.DataFrame(
                 index=[leading_dt, missingdt, trailing_dt],
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/modeldata.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/modeldata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Wed Mar 22 13:50:17 2023
 
 @author: thoverga
 """
+
 import pandas as pd
 
 from metobs_toolkit.df_helpers import init_multiindexdf, conv_tz_multiidxdf
 
 from metobs_toolkit.landcover_functions import connect_to_gee, gee_extract_timeseries
 
 from metobs_toolkit.convertors import convert_to_toolkit_units
@@ -27,15 +28,25 @@
 
         self._settings = Settings()
         self.mapinfo = self._settings.gee["gee_dataset_info"]
 
     def __repr__(self):
         return f"ModelData instance: {self.modelname} model data of {list(self.df.columns)}"
 
-    # def _conv_to_timezone(self, tz):
+    def _conv_to_timezone(self, tzstr):
+        # get tzstr by datetimindex.tz.zone
+
+
+        df=self.df
+        df['datetime_utc'] = df.index.get_level_values('datetime').tz_convert(tzstr)
+        df = df.reset_index()
+        df = df.drop(columns=['datetime'])
+        df = df.rename(columns={'datetime_utc': 'datetime'})
+        df = df.set_index(['name', 'datetime'])
+        self.df = df
 
     def get_ERA5_data(self, metadf, startdt, enddt, obstype="temp"):
         # startdt and enddt IN UTC FORMAT!!!!!
 
         era_mapinfo = self.mapinfo["ERA5_hourly"]
         # Connect to Gee
         connect_to_gee()
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/plotting_functions.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/plotting_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -240,157 +240,158 @@
     ax.set_title(title)
 
     return ax
 
 
 def timeseries_plot(
     mergedf,
-    obstype,
+    # obstype,
     title,
     xlabel,
     ylabel,
     colorby,
     show_legend,
     show_outliers,
-    plot_settings,
-    gap_settings,
-    qc_info_settings,
-    ax=None
+    settings,
+    _ax=None #needed for GUI, not recommended use
 ):
 
-    if isinstance(ax, type(None)):
-        # init figure
-        fig, ax = plt.subplots(figsize=plot_settings["time_series"]["figsize"])
+    plot_settings = settings.app["plot_settings"]
 
 
-    # subbset and cleanup data
+    if isinstance(_ax, type(None)):
+        # init figure
+        fig, ax = plt.subplots(figsize=plot_settings["time_series"]["figsize"])
+    else:
+        ax=_ax
 
+    # get data ready
     mergedf = mergedf[~mergedf.index.duplicated()]
     init_idx = mergedf.index
 
-    if not show_outliers:
-        if obstype + "_final_label" in mergedf.columns:
-            # remove outliers from plotting data
-            mergedf = mergedf[mergedf[obstype + "_final_label"] == "ok"]
-            mergedf = mergedf[[obstype, obstype + "_final_label"]]
-        else:
-            # no final label available, so plot all data
-            mergedf = mergedf[[obstype]]
+    # define different groups (different plotting styles)
+
+    # ok group
+    ok_group_label = 'ok'
+
+    # filled value groups
+    fill_labels= [ val for val in settings.gap['gaps_fill_info']['label'].values()]
+    missing_fill_labels = [ val for val in settings.missing_obs['missing_obs_fill_info']['label'].values()]
+    fill_labels.extend(missing_fill_labels)
+
+    # outlier groups
+    # Catching with an else
+
+
+    custom_handles = [] #add legend items to it
 
     if colorby == "label":
         # iterate over label groups
-        col_mapper = _all_possible_labels_colormapper(
-            plot_settings, qc_info_settings, gap_settings
-        )  # get color mapper
-        outl_groups = mergedf.groupby(obstype + "_final_label")
+        col_mapper = _all_possible_labels_colormapper(settings) # get color mapper
+
+        outl_groups = mergedf.groupby('label')
         legenddict = {}
         for outl_label, groupdf in outl_groups:
             outl_color = col_mapper[outl_label]
 
-            # plot data
-            if outl_label == "ok":  # ok data as lines
+            # plot data for the 'ok' group
+            if outl_label == ok_group_label:  # ok data as lines
                 # add init_idx andf fill with nans (to avoid matplotlib interpolation)
                 fill_idx = init_idx.to_frame().drop(groupdf.index)
                 groupdf = pd.concat([groupdf, fill_idx])
                 groupdf = groupdf.drop(columns=["name", "datetime"], errors="ignore")
                 groupdf.sort_index()
+
                 plotdf = groupdf.reset_index().pivot(
-                    index="datetime", columns="name", values=obstype
+                    index="datetime", columns="name", values='value'
                 )  # long to wide
 
                 ax = plotdf.plot(
                     kind="line",
                     color=outl_color,
                     ax=ax,
                     legend=False,
                     zorder=plot_settings["time_series"]["linezorder"],
                     linewidth=plot_settings["time_series"]["linewidth"],
                 )
 
-            elif outl_label in list(
-                gap_settings["gaps_fill_info"]["label"].items()
-            ):  # fill gaps as dashed lines
+                # add legend handl
+                custom_handles.append(
+                    Line2D([0], [0], color=outl_color, label="ok", lw=4))
+
+
+
+            # plot filled data
+            elif outl_label in  fill_labels:  # fill gaps as dashed lines
+
                 fill_idx = init_idx.to_frame().drop(groupdf.index)
                 groupdf = pd.concat([groupdf, fill_idx])
                 groupdf = groupdf.drop(columns=["name", "datetime"], errors="ignore")
                 groupdf.sort_index()
                 plotdf = groupdf.reset_index().pivot(
-                    index="datetime", columns="name", values=obstype
+                    index="datetime", columns="name", values='value'
                 )  # long to wide
 
                 ax = plotdf.plot(
                     kind="line",
                     style="--",
                     color=outl_color,
                     ax=ax,
                     legend=False,
-                    zorder=plot_settings["dashedzorder"],
-                    linewidth=plot_settings["linewidth"],
+                    zorder=plot_settings['time_series']["dashedzorder"],
+                    linewidth=plot_settings['time_series']["linewidth"],
                 )
 
+                # add legend handle
+                custom_handles.append(
+                    Line2D([0],[0],
+                        color=outl_color,
+                        label=f"filled value ({outl_label})",
+                        lw=1,
+                        linestyle="--",)
+                    )
+
             else:  # outliers as scatters
-                plotdf = groupdf[obstype]
+                plotdf = groupdf['value']
                 plotdf.index = plotdf.index.droplevel("name")
                 plotdf = plotdf.reset_index()
                 ax = plotdf.plot(
                     kind="scatter",
                     x="datetime",
-                    y=obstype,
+                    y='value',
                     ax=ax,
                     color=outl_color,
                     legend=False,
                     zorder=plot_settings["time_series"]["scatterzorder"],
                     s=plot_settings["time_series"]["scattersize"],
                 )
 
+                # add legend handle
+                custom_handles.append(
+                    Line2D([0],[0], marker="o", color="w",
+                        markerfacecolor=outl_color,
+                        label=outl_label,
+                        lw=1,)
+                    )
             legenddict[outl_label] = outl_color
 
         # make legend
         if show_legend:
-            custom_handles = []
-            # add ok label at the top
-            if "ok" in legenddict.keys():
-                custom_handles.append(
-                    Line2D([0], [0], color=legenddict["ok"], label="ok", lw=4)
-                )
-                del legenddict["ok"]  # remove ok key
-
-            for gapfillmethod, label in gap_settings["gaps_fill_info"]["label"].items():
-                if label in legenddict.keys():
-                    custom_handles.append(
-                        Line2D(
-                            [0],
-                            [0],
-                            color=legenddict[gap_settings["gap_fill_info"]["label"]],
-                            label=f"gap filled ({gapfillmethod})",
-                            lw=4,
-                            linestyle="--",
-                        )
-                    )
-                    del legenddict[label]  # remove key
-
-            custom_scatters = [
-                Line2D(
-                    [0],
-                    [0],
-                    marker="o",
-                    color="w",
-                    markerfacecolor=col,
-                    label=lab,
-                    lw=1,
-                )
-                for lab, col in legenddict.items()
-            ]
-
-            custom_handles.extend(custom_scatters)
+            # TODO: sort items
+            # # sort legend items
+            # sorted_handles = []
+            # # group 1, 2, 3
+            # sorted_handles.append([item[1] for item in custom_handles if item[0] == 1])
+            # sorted_handles.append([item[1] for item in custom_handles if item[0] == 2])
+            # sorted_handles.append([item[1] for item in custom_handles if item[0] == 3])
             ax.legend(handles=custom_handles)
 
     elif colorby == "name":
         plotdf = mergedf.reset_index().pivot(
-            index="datetime", columns="name", values=obstype
+            index="datetime", columns="name", values='value'
         )
         ax = plotdf.plot(kind="line", legend=show_legend, ax=ax)
 
     # Set title
     ax.set_title(title)
     # ax.legend().set_title('')
 
@@ -512,16 +513,24 @@
     outl_col_mapper = {
         outl_type: color_defenitions[outl_name_mapper[outl_type]]
         for outl_type in outl_name_mapper.keys()
     }
     return outl_col_mapper
 
 
-def _all_possible_labels_colormapper(plot_settings, qc_info_settings, gap_settings):
+def _all_possible_labels_colormapper(settings):
     """Make color mapper for all LABELVALUES to colors."""
+
+
+    plot_settings = settings.app["plot_settings"]
+    gap_settings = settings.gap
+    qc_info_settings = settings.qc["qc_checks_info"]
+    missing_obs_settings = settings.missing_obs['missing_obs_fill_info']
+
+
     color_defenitions = plot_settings["color_mapper"]
 
     mapper = dict()
 
     # get QC outlier labels
 
     outl_col_mapper = _outl_value_to_colormapper(
@@ -534,18 +543,26 @@
 
     # update gap and missing timestamp labels
     mapper[gap_settings["gaps_info"]["gap"]["outlier_flag"]] = color_defenitions["gap"]
     mapper[
         gap_settings["gaps_info"]["missing_timestamp"]["outlier_flag"]
     ] = color_defenitions["missing_timestamp"]
 
-    # add gapfill
+    # add fill for gaps
     for method, label in gap_settings["gaps_fill_info"]["label"].items():
         mapper[label] = color_defenitions[method]
 
+    # add fill for missing
+    for method, label in missing_obs_settings['label'].items():
+        mapper[label] = color_defenitions[method]
+
+
+
+
+
     return mapper
 
 
 def qc_stats_pie(
     final_stats, outlier_stats, specific_stats, plot_settings, qc_check_info
 ):
     # restore rcParams
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/printing.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/printing.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/qc_checks.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/qc_checks.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/qc_statistics.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/qc_statistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def get_freq_statistics(comb_df, obstype, checks_info, gaps_info, applied_qc_order):
     outlier_labels = [qc["outlier_flag"] for qc in checks_info.values()]
 
-    if not obstype + "_final_label" in comb_df.columns:
-        print(f"Final observation label for {obstype} is not computed!")
-        return (None, None, None)
-
-    final_counts = comb_df[obstype + "_final_label"].value_counts()
+    final_counts = comb_df['label'].value_counts()
 
     # add missing labels
     # QC labels
     non_triggered_labels_dict = {}
     # fill with zeros for non-triggered checks
     for outl_label in outlier_labels:
         if not outl_label in final_counts.index:
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/settings.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,29 +242,27 @@
         data_template_file=None,
         metadata_template_file=None,
     ):
         """
         Update some settings that are relevent before data is imported. The self
         object will be updated.
 
-
         :param output_folder: a directory to store the output to, defaults to None.
         :type output_folder: String, optional
         :param input_data_file: Path to the input data file, defaults to None.
         :type input_data_file: String, optional
         :param input_metadata_file: Path to the input metadata file, defaults to None
         :type input_metadata_file: String, optional
-        :param data_template_file: Path to the mapper-template csv file to be used on the observations.
-        If not given, the default template is used.
+        :param data_template_file: Path to the mapper-template csv file to be used on the observations. If not given, the default template is used.
         :type data_template_file: String, optional
-        :param metadata_template_file: Path to the mapper-template csv file to be used on the metadata.
-        If not given, the default template is used.
+        :param metadata_template_file: Path to the mapper-template csv file to be used on the metadata. If not given, the default template is used.
         :type metadata_template_file: String, optional
         :return: No return
         :rtype: No return
+
         """
 
         logger.info("Updating settings with input: ")
 
         if not isinstance(output_folder, type(None)):
             print(
                 "Update output_folder: ",
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/default_formats_settings.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/default_formats_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     "persistance": "#f0051c",
     "repetitions": "#056ff0",
     "step": "#05d4f0",
     "window_variation": "#05f0c9",
     # missing and gap
     "gap": "#f00592",
     "missing_timestamp": "#e86bb6",
-    # Gap filling
+    # filling
     "linear": "#d406c6",
     "model_debias": "#6e1868",
     # common
     "ok": "#07f72b",
     "not checked": "#f7cf07",
     # Aggregated
     "outlier": "#f20000",
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gaps_and_missing_settings.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gaps_and_missing_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         "debias_period": {
             "prefered_leading_sample_duration_hours": 48,
             "prefered_trailing_sample_duration_hours": 48,
             "minimum_leading_sample_duration_hours": 24,
             "minimum_trailing_sample_duration_hours": 24,
         }
     },
+    "automatic":{'max_interpolation_duration_str': '5H'}
 }
 
 
 gaps_fill_info = {
     "label_columnname": "final_label",
     "label": {"linear": "gap_interpolation", "model_debias": "gap_debiased_era5"},
     "numeric_flag": 21,
```

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gee_settings.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gee_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/qc_settings.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/qc_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp` & `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx` & `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/station.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/station.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a3/metobs_toolkit/writing_files.py` & `metobs_toolkit-0.0.2a4/metobs_toolkit/writing_files.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: thoverga
 """
 # --
 import os
 
 
 def write_dataset_to_csv(
-    df, metadf, filename, outputfolder, location_info, observation_types
+    df, metadf, filename, outputfolder, location_info, seperate_metadata_file,
 ):
     """
     Write the dataset to a file where the observations, metadata and (if available)
     the quality labels per observation type are merged together.
 
     A final qualty controll label for each quality-controlled-observation type
     can be added in the outputfile.
@@ -34,35 +34,36 @@
 
     Returns
     -------
     None
 
     """
 
-    # make column ordering 'datetime', 'name', obs, QC, Qc final metadata
-    write_cols = ["datetime", "name"]
-    write_cols.extend([col for col in df.columns if col in observation_types])
-    write_cols.extend([col for col in df.columns if col.endswith("_label")])
-    write_cols.extend(location_info)  # metadata
+
 
     df = df.reset_index()
 
-    # merge metadata
-    df = df.merge(metadf, how="left", left_on="name", right_index=True)
 
-    # subset and order columns
-    df = df[write_cols]
+    # find metadata that are not present
+    ignore_metadat = [col for col in location_info if metadf[col].isnull().all()]
+
+
+    if not seperate_metadata_file:
+        # merge metadata
+        df = df.merge(metadf, how="left", left_on="name", right_index=True)
+        df = df.drop(columns=ignore_metadat)
+    else:
+        metadf = metadf.reset_index()
+        metadf = metadf.drop(columns=ignore_metadat)
+        metadatafile = os.path.join(outputfolder, "metadata_file.csv")
+        print(f"write metadata to file: {metadatafile}")
+        metadf.to_csv(path_or_buf=metadatafile, sep=";", na_rep="NaN", index=False)
+
 
-    # find observation type that are not present
-    ignore_obstypes = [col for col in observation_types if df[col].isnull().all()]
-    df = df.drop(columns=ignore_obstypes)
 
-    # find metadata that are not present
-    ignore_metadat = [col for col in location_info if df[col].isnull().all()]
-    df = df.drop(columns=ignore_metadat)
 
     df = df.sort_values(["name", "datetime"])
 
     # make filename
     if isinstance(filename, type(None)):
         startstr = df["datetime"].min().strftime("%Y%m%d")
         endstr = df["datetime"].max().strftime("%Y%m%d")
```

### Comparing `metobs_toolkit-0.0.2a3/pyproject.toml` & `metobs_toolkit-0.0.2a4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MetObs-toolkit"
-version = "0.0.2a3"
+version = "0.0.2a4"
 description = "A Meteorological observations toolkit for scientists"
 authors = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 maintainers = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 license = "LICENSE"
 readme = "README.md"
 documentation = "https://python-poetry.org/docs/"
 packages = [{include = "metobs_toolkit"}]
@@ -14,18 +14,19 @@
 python = "^3.9"
 pandas = "^1.3.0"
 numpy = "^1.17.3"
 matplotlib = "^3.0.0"
 mysql-connector-python = "^8.0.6"
 geopandas = "^0.9.0"
 pyproj = "~3.4"
-#rasterstats = "^0.16.0"
 mapclassify = "^2.4.0"
 earthengine-api = "^0.1.340"
-PyQt5 = "^5.15.0"
+PyQt5 = "=5.12.2" #Technical: this version is the latest to build from source
+pyqt5-sip = "^12.12.1"
+pyqt5-qt5 = "^5.15.2"
 
 
 
 [tool.poetry.group.dev.dependencies]
 poetry = "^1.3.2"
 
 [build-system]
```

### Comparing `metobs_toolkit-0.0.2a3/PKG-INFO` & `metobs_toolkit-0.0.2a4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: metobs-toolkit
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: A Meteorological observations toolkit for scientists
 License: LICENSE
 Keywords: meteorology,observations,urban climate
 Author: Thomas Vergauwen
 Author-email: thomas.vergauwen@meteo.be
 Maintainer: Thomas Vergauwen
 Maintainer-email: thomas.vergauwen@meteo.be
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyQt5 (>=5.15.0,<6.0.0)
+Requires-Dist: PyQt5 (==5.12.2)
 Requires-Dist: earthengine-api (>=0.1.340,<0.2.0)
 Requires-Dist: geopandas (>=0.9.0,<0.10.0)
 Requires-Dist: mapclassify (>=2.4.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.6,<9.0.0)
 Requires-Dist: numpy (>=1.17.3,<2.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pyproj (>=3.4,<3.5)
+Requires-Dist: pyqt5-qt5 (>=5.15.2,<6.0.0)
+Requires-Dist: pyqt5-sip (>=12.12.1,<13.0.0)
 Project-URL: Documentation, https://python-poetry.org/docs/
 Description-Content-Type: text/markdown
 
 # MetObs-toolkit
 
 This repo contains all the software for the [metobs_toolkit](https://test.pypi.org/project/metobs-toolkit/).
 The MetObs-toolkit is a package for scientists who make use meteorological observations.
```

