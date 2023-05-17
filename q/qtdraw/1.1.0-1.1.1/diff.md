# Comparing `tmp/qtdraw-1.1.0.tar.gz` & `tmp/qtdraw-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdraw-1.1.0.tar", last modified: Tue May 16 07:28:31 2023, max compression
+gzip compressed data, was "qtdraw-1.1.1.tar", last modified: Wed May 17 12:45:44 2023, max compression
```

## Comparing `qtdraw-1.1.0.tar` & `qtdraw-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-16 07:28:31.912933 qtdraw-1.1.0/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.0/LICENSE
--rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.0/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2092 2023-05-16 07:28:31.913027 qtdraw-1.1.0/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-05-15 22:06:02.000000 qtdraw-1.1.0/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-16 07:28:31.907215 qtdraw-1.1.0/qtdraw/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2023-05-16 07:13:18.000000 qtdraw-1.1.0/qtdraw/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-16 07:28:31.912361 qtdraw-1.1.0/qtdraw/core/
--rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/core/basic_object.py
--rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/color_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/core/color_palette.py
--rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/default_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/core/dialog_about.py
--rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/dialog_preference.py
--rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/core/editable_widget.py
--rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/group_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/group_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/group_tab.py
--rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/group_view.py
--rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/core/line_edit.py
--rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/core/pixmap_converter.py
--rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/qt_logging.py
--rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/qtdraw.png
--rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/qtdraw.ui
--rw-r--r--   0 hiro       (501) staff       (20)    17478 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/table_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/tree_item.py
--rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/tree_item_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     7499 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/core/util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/core/validator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-16 07:28:31.912794 qtdraw-1.1.0/qtdraw/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)    46964 2023-05-15 12:36:33.000000 qtdraw-1.1.0/qtdraw/multipie/dialog_group.py
--rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.0/qtdraw/multipie/dialog_group_info.py
--rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/multipie/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)    91973 2023-05-15 12:36:32.000000 qtdraw-1.1.0/qtdraw/qt_draw.py
--rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.0/qtdraw/qt_draw_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-16 07:28:31.907882 qtdraw-1.1.0/qtdraw.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2092 2023-05-16 07:28:31.000000 qtdraw-1.1.0/qtdraw.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)      944 2023-05-16 07:28:31.000000 qtdraw-1.1.0/qtdraw.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-16 07:28:31.000000 qtdraw-1.1.0/qtdraw.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       96 2023-05-16 07:28:31.000000 qtdraw-1.1.0/qtdraw.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        7 2023-05-16 07:28:31.000000 qtdraw-1.1.0/qtdraw.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      640 2023-05-16 07:28:31.913449 qtdraw-1.1.0/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.0/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.098284 qtdraw-1.1.1/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.1/LICENSE
+-rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.1/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2414 2023-05-17 12:45:44.098375 qtdraw-1.1.1/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     2034 2023-05-17 12:42:17.000000 qtdraw-1.1.1/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.091917 qtdraw-1.1.1/qtdraw/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2023-05-17 01:26:21.000000 qtdraw-1.1.1/qtdraw/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.097700 qtdraw-1.1.1/qtdraw/core/
+-rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/basic_object.py
+-rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/color_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/color_palette.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/default_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/dialog_about.py
+-rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/dialog_preference.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/editable_widget.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_tab.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_view.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/line_edit.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/pixmap_converter.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/qt_logging.py
+-rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/qtdraw.png
+-rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/qtdraw.ui
+-rw-r--r--   0 hiro       (501) staff       (20)    17478 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/table_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/tree_item.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/tree_item_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7499 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/validator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.098150 qtdraw-1.1.1/qtdraw/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)    46964 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/multipie/dialog_group.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.1/qtdraw/multipie/dialog_group_info.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/multipie/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)    91973 2023-05-15 12:36:32.000000 qtdraw-1.1.1/qtdraw/qt_draw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/qt_draw_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.092650 qtdraw-1.1.1/qtdraw.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2414 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)      944 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       96 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        7 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      640 2023-05-17 12:45:44.098810 qtdraw-1.1.1/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.1/setup.py
```

### Comparing `qtdraw-1.1.0/LICENSE` & `qtdraw-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/PKG-INFO` & `qtdraw-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.0
+Version: 1.1.1
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
@@ -19,18 +19,22 @@
 
 ## Installation
 
 QtDraw can be installed from PyPI using pip on Python >= 3.8:
 ```
 pip install qtdraw
 ```
+It is useful to associate with the following application or batch file with `.qtdw` extension.
+- [Mac](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_MacApp.zip)
+- [Windows](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_WinApp.zip)
+
 You can also visit
 [PyPI](https://pypi.org/project/qtdraw/) or [GitHub](https://github.com/CMT-MU/QtDraw) to download the source.
 
-See the Installation for more details.
+See also, [Install Guide (in Japanese)](https://github.com/CMT-MU/QtDraw/blob/main/docs/install_guide.pdf)
 
 ## Authors
 Hiroaki Kusunose
 
 ## Citing QtDraw and MultiPie
 
 If you are using QtDraw and/or MultiPie in your scientific research, please help our scientific visibility by citing our work:
```

### Comparing `qtdraw-1.1.0/README.md` & `qtdraw-1.1.1/qtdraw.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,40 @@
+Metadata-Version: 2.1
+Name: qtdraw
+Version: 1.1.1
+Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
+Home-page: https://github.com/CMT-MU/QtDraw
+Author: Hiroaki Kusunose
+Author-email: hiroaki.kusunose@gmail.com
+License: MIT
+Keywords: pyvista,qtpy5
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # QtDraw
 
 3D drawing tool for molecules and crystals based on [PyVista](https://docs.pyvista.org/) and [Qt](https://www.riverbankcomputing.com/static/Docs/PyQt5/#).
 Drawings are associated with crystallographic symmetry operations provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Installation
 
 QtDraw can be installed from PyPI using pip on Python >= 3.8:
 ```
 pip install qtdraw
 ```
+It is useful to associate with the following application or batch file with `.qtdw` extension.
+- [Mac](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_MacApp.zip)
+- [Windows](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_WinApp.zip)
+
 You can also visit
 [PyPI](https://pypi.org/project/qtdraw/) or [GitHub](https://github.com/CMT-MU/QtDraw) to download the source.
 
-See the Installation for more details.
+See also, [Install Guide (in Japanese)](https://github.com/CMT-MU/QtDraw/blob/main/docs/install_guide.pdf)
 
 ## Authors
 Hiroaki Kusunose
 
 ## Citing QtDraw and MultiPie
 
 If you are using QtDraw and/or MultiPie in your scientific research, please help our scientific visibility by citing our work:
```

### Comparing `qtdraw-1.1.0/qtdraw/core/basic_object.py` & `qtdraw-1.1.1/qtdraw/core/basic_object.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/color_dialog.py` & `qtdraw-1.1.1/qtdraw/core/color_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/color_palette.py` & `qtdraw-1.1.1/qtdraw/core/color_palette.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/default_panel.ui` & `qtdraw-1.1.1/qtdraw/core/default_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/dialog_about.py` & `qtdraw-1.1.1/qtdraw/core/dialog_about.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/dialog_preference.py` & `qtdraw-1.1.1/qtdraw/core/dialog_preference.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/editable_widget.py` & `qtdraw-1.1.1/qtdraw/core/editable_widget.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/group_model.py` & `qtdraw-1.1.1/qtdraw/core/group_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/group_panel.ui` & `qtdraw-1.1.1/qtdraw/core/group_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/group_tab.py` & `qtdraw-1.1.1/qtdraw/core/group_tab.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/group_view.py` & `qtdraw-1.1.1/qtdraw/core/group_view.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/line_edit.py` & `qtdraw-1.1.1/qtdraw/core/line_edit.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/pixmap_converter.py` & `qtdraw-1.1.1/qtdraw/core/pixmap_converter.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/qt_logging.py` & `qtdraw-1.1.1/qtdraw/core/qt_logging.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/qtdraw.png` & `qtdraw-1.1.1/qtdraw/core/qtdraw.png`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/qtdraw.ui` & `qtdraw-1.1.1/qtdraw/core/qtdraw.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/setting.py` & `qtdraw-1.1.1/qtdraw/core/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/table_dialog.py` & `qtdraw-1.1.1/qtdraw/core/table_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/tree_item.py` & `qtdraw-1.1.1/qtdraw/core/tree_item.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/tree_item_model.py` & `qtdraw-1.1.1/qtdraw/core/tree_item_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/util.py` & `qtdraw-1.1.1/qtdraw/core/util.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/core/validator.py` & `qtdraw-1.1.1/qtdraw/core/validator.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/multipie/dialog_group.py` & `qtdraw-1.1.1/qtdraw/multipie/dialog_group.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/multipie/dialog_group_info.py` & `qtdraw-1.1.1/qtdraw/multipie/dialog_group_info.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/multipie/setting.py` & `qtdraw-1.1.1/qtdraw/multipie/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/qt_draw.py` & `qtdraw-1.1.1/qtdraw/qt_draw.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw/qt_draw_base.py` & `qtdraw-1.1.1/qtdraw/qt_draw_base.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/qtdraw.egg-info/PKG-INFO` & `qtdraw-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-Metadata-Version: 2.1
-Name: qtdraw
-Version: 1.1.0
-Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
-Home-page: https://github.com/CMT-MU/QtDraw
-Author: Hiroaki Kusunose
-Author-email: hiroaki.kusunose@gmail.com
-License: MIT
-Keywords: pyvista,qtpy5
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # QtDraw
 
 3D drawing tool for molecules and crystals based on [PyVista](https://docs.pyvista.org/) and [Qt](https://www.riverbankcomputing.com/static/Docs/PyQt5/#).
 Drawings are associated with crystallographic symmetry operations provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Installation
 
 QtDraw can be installed from PyPI using pip on Python >= 3.8:
 ```
 pip install qtdraw
 ```
+It is useful to associate with the following application or batch file with `.qtdw` extension.
+- [Mac](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_MacApp.zip)
+- [Windows](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_WinApp.zip)
+
 You can also visit
 [PyPI](https://pypi.org/project/qtdraw/) or [GitHub](https://github.com/CMT-MU/QtDraw) to download the source.
 
-See the Installation for more details.
+See also, [Install Guide (in Japanese)](https://github.com/CMT-MU/QtDraw/blob/main/docs/install_guide.pdf)
 
 ## Authors
 Hiroaki Kusunose
 
 ## Citing QtDraw and MultiPie
 
 If you are using QtDraw and/or MultiPie in your scientific research, please help our scientific visibility by citing our work:
```

### Comparing `qtdraw-1.1.0/qtdraw.egg-info/SOURCES.txt` & `qtdraw-1.1.1/qtdraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.0/setup.cfg` & `qtdraw-1.1.1/setup.cfg`

 * *Files identical despite different names*

