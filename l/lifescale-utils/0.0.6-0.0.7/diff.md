# Comparing `tmp/lifescale-utils-0.0.6.tar.gz` & `tmp/lifescale-utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifescale-utils-0.0.6.tar", last modified: Wed Apr 26 20:35:30 2023, max compression
+gzip compressed data, was "lifescale-utils-0.0.7.tar", last modified: Wed May 17 16:45:45 2023, max compression
```

## Comparing `lifescale-utils-0.0.6.tar` & `lifescale-utils-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2020-07-16 17:28:33.000000 lifescale-utils-0.0.6/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/MANIFEST.in
--rw-rw-r--   0 heller    (1000) heller    (1000)     2792 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2331 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1002 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/__init__.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/command_line/
--rw-rw-r--   0 heller    (1000) heller    (1000)      723 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/command_line/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4451 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/command_line/command_line.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    18823 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      718 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    43282 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    24410 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5898 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/masses_model.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4958 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/panel_metadata_model.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    30974 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/resources.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6323 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/gui/sample_summary_model.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    28693 2023-04-26 20:29:04.000000 lifescale-utils-0.0.6/lifescale/models/ls_data.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.265561 lifescale-utils-0.0.6/lifescale/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1170 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/scripts/ls2csv.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      264 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/lifescale/scripts/run_gui.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/lifescale_utils.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     2792 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)      807 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)      120 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       38 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       10 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-26 20:35:30.000000 lifescale-utils-0.0.6/lifescale_utils.egg-info/zip-safe
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-12-30 08:49:47.000000 lifescale-utils-0.0.6/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)      836 2023-04-26 20:35:30.269561 lifescale-utils-0.0.6/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-05-17 16:45:45.578512 lifescale-utils-0.0.7/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2020-07-16 17:28:33.000000 lifescale-utils-0.0.7/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2023-04-26 20:29:04.000000 lifescale-utils-0.0.7/MANIFEST.in
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3687 2023-05-17 16:45:45.578512 lifescale-utils-0.0.7/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3226 2023-05-17 16:45:22.000000 lifescale-utils-0.0.7/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-05-17 16:45:45.574512 lifescale-utils-0.0.7/lifescale/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1002 2023-05-17 16:42:17.000000 lifescale-utils-0.0.7/lifescale/__init__.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-05-17 16:45:45.574512 lifescale-utils-0.0.7/lifescale/command_line/
+-rw-rw-r--   0 heller    (1000) heller    (1000)      723 2022-12-30 08:49:47.000000 lifescale-utils-0.0.7/lifescale/command_line/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4451 2023-05-16 13:18:16.000000 lifescale-utils-0.0.7/lifescale/command_line/command_line.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-05-17 16:45:45.574512 lifescale-utils-0.0.7/lifescale/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18823 2023-04-26 20:29:04.000000 lifescale-utils-0.0.7/lifescale/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      718 2023-04-26 20:29:04.000000 lifescale-utils-0.0.7/lifescale/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    43282 2023-04-26 20:29:04.000000 lifescale-utils-0.0.7/lifescale/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    25129 2023-05-16 13:18:16.000000 lifescale-utils-0.0.7/lifescale/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5898 2023-05-16 13:18:16.000000 lifescale-utils-0.0.7/lifescale/gui/masses_model.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4958 2023-05-16 13:18:16.000000 lifescale-utils-0.0.7/lifescale/gui/panel_metadata_model.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    30974 2023-04-26 20:29:04.000000 lifescale-utils-0.0.7/lifescale/gui/resources.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6323 2023-05-16 13:18:16.000000 lifescale-utils-0.0.7/lifescale/gui/sample_summary_model.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-05-17 16:45:45.574512 lifescale-utils-0.0.7/lifescale/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.7/lifescale/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    28693 2023-05-16 13:18:16.000000 lifescale-utils-0.0.7/lifescale/models/ls_data.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-05-17 16:45:45.574512 lifescale-utils-0.0.7/lifescale/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)      708 2022-12-30 08:49:47.000000 lifescale-utils-0.0.7/lifescale/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1170 2022-12-30 08:49:47.000000 lifescale-utils-0.0.7/lifescale/scripts/ls2csv.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      264 2022-12-30 08:49:47.000000 lifescale-utils-0.0.7/lifescale/scripts/run_gui.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-05-17 16:45:45.578512 lifescale-utils-0.0.7/lifescale_utils.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3687 2023-05-17 16:45:45.000000 lifescale-utils-0.0.7/lifescale_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)      807 2023-05-17 16:45:45.000000 lifescale-utils-0.0.7/lifescale_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-05-17 16:45:45.000000 lifescale-utils-0.0.7/lifescale_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)      120 2023-05-17 16:45:45.000000 lifescale-utils-0.0.7/lifescale_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       38 2023-05-17 16:45:45.000000 lifescale-utils-0.0.7/lifescale_utils.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       10 2023-05-17 16:45:45.000000 lifescale-utils-0.0.7/lifescale_utils.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-05-17 16:45:45.000000 lifescale-utils-0.0.7/lifescale_utils.egg-info/zip-safe
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-12-30 08:49:47.000000 lifescale-utils-0.0.7/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)      836 2023-05-17 16:45:45.578512 lifescale-utils-0.0.7/setup.cfg
```

### Comparing `lifescale-utils-0.0.6/LICENSE` & `lifescale-utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/PKG-INFO` & `lifescale-utils-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-Metadata-Version: 2.1
-Name: lifescale-utils
-Version: 0.0.6
-Summary: Lifescale utility software.
-Home-page: https://gitlab.com/hellerdev/lifescale_utils
-Author: Andreas Hellerschmied
-Author-email: heller182@gmx.at
-License: GNU GPLv3
-Keywords: Lifescale
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: <4,>=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # lifescale_utils
-Data analysis utility tools for lifescale.
+Data analysis utilities for lifescale.
+
+# Programs:
+
+## lsgui
+*lsgui* starts the graphical user interface (gui) of lifescale-utils. It provides toe following main features:
+  * Read lifescale xlsm files
+  * Visualize the data from the xlsm file and calculate various statistics
+  * Assess the mass distribution of samples by histograms and flag invalid data
+  * Write the cleand data to csv files (see *ls2csv*)
+
+### Usage:
+```
+usage: lsgui [-h]
 
-# Command line programs:
+Starts lifescale utils gui.
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
 
 ## ls2csv
-*ls2csv* is a command line program that reads the content of the xlsm files written by lifescale units, parses the data and writes them to three csv 
-files (where `[run-name]` is the name from the settings sheet):
-  * `Masses_Vibrio_[run-name].csv`: Data series from the sheet AcquisitionIntervals.
-  * `Metadata_[run-name].csv`: Data from the sheet PanelData.
-  * `SampleSummary_[run-name].csv`: Data from the sheet IntervalAnalysis plus sample related data from AcquisitionIntervals.
+*ls2csv* is a command line program that converts xlsm files written by lifescale units to csv files. The following files  
+are created:
+  * `Masses_<run-name>_<guid>.csv`: Data series from the sheet AcquisitionIntervals.
+  * `Metadata_<run-name>_<guid>.csv`: Data from the sheet PanelData.
+  * `SampleSummary_<run-name>_<guid>.csv`: Data from the sheet IntervalAnalysis plus sample related data from AcquisitionIntervals.
+`<run-name>` and `<guid>` are the taken from the fields `Name` and `Guid` (if available) from the settings sheet of the xml file.
 
 ### Usage:
 ```
 usage: ls2csv [-h] -i INPUT_XLSM -o OUT_DIR [-nv] [-s] [-t]
 
 Conversion from lifescale xlsm output to csv files
 
@@ -43,28 +46,36 @@
                         deviation, quartiles, interquartile range) and add
                         them to the SampleSummary output CSV file (columns:
                         Mass_median, Mass_std, Mass_q25, Mass_q75,Mass_iqr).
                         (default: False)
   -t, --sort-masses-by-time
                         Sort data in the Masses CSV file by acquisition time.
                         (default: False)
-
+                        
 ```
 
+# Python package and installation
+
+Lifescale_utils is available at https://pypi.org/project/lifescale-utils/
+
+Installation: ```pip install lifescale_utils```
 
 # License and copyright
 
-Copyright (C) 2022  Andreas Hellerschmied (<heller182@gmx.at>)
+Copyright (C) 2023  Andreas Hellerschmied (<heller182@gmx.at>)
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# Funding
+lifescale_utils was funded by the Centre for Microbiology and Environmental Systems Science (CMES) of the University of 
+Vienna (https://cmess.univie.ac.at/).
```

### Comparing `lifescale-utils-0.0.6/lifescale/__init__.py` & `lifescale-utils-0.0.7/lifescale/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (heller182@gmx.at)
 """
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://gitlab.com/hellerdev/lifescale_utils'
 __email__ = 'heller182@gmx.at'
 __copyright__ = '(c) 2023 Andreas Hellerschmied'
 __pypi_repo__ = 'https://pypi.org/project/lifescale-utils/'
```

### Comparing `lifescale-utils-0.0.6/lifescale/command_line/__init__.py` & `lifescale-utils-0.0.7/lifescale/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale/command_line/command_line.py` & `lifescale-utils-0.0.7/lifescale/command_line/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Command line interface of lifescale utils.
 
-Copyright (C) 2022  Andreas Hellerschmied <heller182@gmx.at>
+Copyright (C) 2023  Andreas Hellerschmied <heller182@gmx.at>
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `lifescale-utils-0.0.6/lifescale/gui/MainWindow.py` & `lifescale-utils-0.0.7/lifescale/gui/MainWindow.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale/gui/__init__.py` & `lifescale-utils-0.0.7/lifescale/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale/gui/dialog_about.py` & `lifescale-utils-0.0.7/lifescale/gui/dialog_about.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale/gui/gui_main.py` & `lifescale-utils-0.0.7/lifescale/gui/gui_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+"""Main GUI model for lifescale_uitls.
+
+Copyright (C) 2023  Andreas Hellerschmied <heller182@gmx.at>
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import sys
 import os
 from PyQt6.QtWidgets import QApplication, QMainWindow, QMessageBox, QFileDialog, QDialog
 from PyQt6.QtCore import pyqtSlot, QDir, Qt
 import numpy as np
 import pyqtgraph as pg
```

### Comparing `lifescale-utils-0.0.6/lifescale/gui/masses_model.py` & `lifescale-utils-0.0.7/lifescale/gui/masses_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Masses model class for PyQt's model view architectrue.
 
-Copyright (C) 2022  Andreas Hellerschmied <heller182@gmx.at>
+Copyright (C) 2023  Andreas Hellerschmied <heller182@gmx.at>
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `lifescale-utils-0.0.6/lifescale/gui/panel_metadata_model.py` & `lifescale-utils-0.0.7/lifescale/gui/panel_metadata_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Panel data model class for PyQt's model view architectrue.
 
-Copyright (C) 2022  Andreas Hellerschmied <heller182@gmx.at>
+Copyright (C) 2023  Andreas Hellerschmied <heller182@gmx.at>
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `lifescale-utils-0.0.6/lifescale/gui/resources.py` & `lifescale-utils-0.0.7/lifescale/gui/resources.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale/gui/sample_summary_model.py` & `lifescale-utils-0.0.7/lifescale/gui/sample_summary_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Sample model class for PyQt's model view architectrue.
 
-Copyright (C) 2022  Andreas Hellerschmied <heller182@gmx.at>
+Copyright (C) 2023  Andreas Hellerschmied <heller182@gmx.at>
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `lifescale-utils-0.0.6/lifescale/models/__init__.py` & `lifescale-utils-0.0.7/lifescale/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale/models/ls_data.py` & `lifescale-utils-0.0.7/lifescale/models/ls_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Modelling the data output of a LifeScale run.
 
-Copyright (C) 2022  Andreas Hellerschmied <heller182@gmx.at>
+Copyright (C) 2023  Andreas Hellerschmied <heller182@gmx.at>
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `lifescale-utils-0.0.6/lifescale/scripts/__init__.py` & `lifescale-utils-0.0.7/lifescale/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale/scripts/ls2csv.py` & `lifescale-utils-0.0.7/lifescale/scripts/ls2csv.py`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/lifescale_utils.egg-info/PKG-INFO` & `lifescale-utils-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 Metadata-Version: 2.1
 Name: lifescale-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Lifescale utility software.
 Home-page: https://gitlab.com/hellerdev/lifescale_utils
 Author: Andreas Hellerschmied
 Author-email: heller182@gmx.at
 License: GNU GPLv3
 Keywords: Lifescale
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <4,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lifescale_utils
-Data analysis utility tools for lifescale.
+Data analysis utilities for lifescale.
 
-# Command line programs:
+# Programs:
+
+## lsgui
+*lsgui* starts the graphical user interface (gui) of lifescale-utils. It provides toe following main features:
+  * Read lifescale xlsm files
+  * Visualize the data from the xlsm file and calculate various statistics
+  * Assess the mass distribution of samples by histograms and flag invalid data
+  * Write the cleand data to csv files (see *ls2csv*)
+
+### Usage:
+```
+usage: lsgui [-h]
+
+Starts lifescale utils gui.
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
 
 ## ls2csv
-*ls2csv* is a command line program that reads the content of the xlsm files written by lifescale units, parses the data and writes them to three csv 
-files (where `[run-name]` is the name from the settings sheet):
-  * `Masses_Vibrio_[run-name].csv`: Data series from the sheet AcquisitionIntervals.
-  * `Metadata_[run-name].csv`: Data from the sheet PanelData.
-  * `SampleSummary_[run-name].csv`: Data from the sheet IntervalAnalysis plus sample related data from AcquisitionIntervals.
+*ls2csv* is a command line program that converts xlsm files written by lifescale units to csv files. The following files  
+are created:
+  * `Masses_<run-name>_<guid>.csv`: Data series from the sheet AcquisitionIntervals.
+  * `Metadata_<run-name>_<guid>.csv`: Data from the sheet PanelData.
+  * `SampleSummary_<run-name>_<guid>.csv`: Data from the sheet IntervalAnalysis plus sample related data from AcquisitionIntervals.
+`<run-name>` and `<guid>` are the taken from the fields `Name` and `Guid` (if available) from the settings sheet of the xml file.
 
 ### Usage:
 ```
 usage: ls2csv [-h] -i INPUT_XLSM -o OUT_DIR [-nv] [-s] [-t]
 
 Conversion from lifescale xlsm output to csv files
 
@@ -43,28 +61,36 @@
                         deviation, quartiles, interquartile range) and add
                         them to the SampleSummary output CSV file (columns:
                         Mass_median, Mass_std, Mass_q25, Mass_q75,Mass_iqr).
                         (default: False)
   -t, --sort-masses-by-time
                         Sort data in the Masses CSV file by acquisition time.
                         (default: False)
-
+                        
 ```
 
+# Python package and installation
+
+Lifescale_utils is available at https://pypi.org/project/lifescale-utils/
+
+Installation: ```pip install lifescale_utils```
 
 # License and copyright
 
-Copyright (C) 2022  Andreas Hellerschmied (<heller182@gmx.at>)
+Copyright (C) 2023  Andreas Hellerschmied (<heller182@gmx.at>)
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# Funding
+lifescale_utils was funded by the Centre for Microbiology and Environmental Systems Science (CMES) of the University of 
+Vienna (https://cmess.univie.ac.at/).
```

### Comparing `lifescale-utils-0.0.6/lifescale_utils.egg-info/SOURCES.txt` & `lifescale-utils-0.0.7/lifescale_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifescale-utils-0.0.6/setup.cfg` & `lifescale-utils-0.0.7/setup.cfg`

 * *Files identical despite different names*

