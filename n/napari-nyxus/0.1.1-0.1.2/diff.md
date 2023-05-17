# Comparing `tmp/napari_nyxus-0.1.1-py3-none-any.whl.zip` & `tmp/napari_nyxus-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 9015 bytes, number of entries: 10
--rw-r--r--  2.0 unx      144 b- defN 23-May-05 15:39 napari_nyxus/__init__.py
--rw-r--r--  2.0 unx      497 b- defN 23-May-05 15:39 napari_nyxus/_version.py
--rw-r--r--  2.0 unx     1433 b- defN 23-May-05 15:39 napari_nyxus/nyx.py
--rw-r--r--  2.0 unx    15412 b- defN 23-May-05 15:39 napari_nyxus/nyx_napari.py
--rw-r--r--  2.0 unx      983 b- defN 23-May-05 15:39 napari_nyxus/util.py
--rw-r--r--  2.0 unx     5194 b- defN 23-May-05 15:39 napari_nyxus-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 15:39 napari_nyxus-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       58 b- defN 23-May-05 15:39 napari_nyxus-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-05 15:39 napari_nyxus-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      814 b- defN 23-May-05 15:39 napari_nyxus-0.1.1.dist-info/RECORD
-10 files, 24640 bytes uncompressed, 7621 bytes compressed:  69.1%
+Zip file size: 9393 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      144 b- defN 23-May-17 14:10 napari_nyxus/__init__.py
+-rw-r--r--  2.0 unx      497 b- defN 23-May-17 14:10 napari_nyxus/_version.py
+-rw-r--r--  2.0 unx      251 b- defN 23-May-17 14:10 napari_nyxus/napari.yaml
+-rw-r--r--  2.0 unx     1387 b- defN 23-May-17 14:10 napari_nyxus/nyx.py
+-rw-r--r--  2.0 unx    14495 b- defN 23-May-17 14:10 napari_nyxus/nyx_napari.py
+-rw-r--r--  2.0 unx      983 b- defN 23-May-17 14:10 napari_nyxus/util.py
+-rw-r--r--  2.0 unx     5644 b- defN 23-May-17 14:10 napari_nyxus-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 14:10 napari_nyxus-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       58 b- defN 23-May-17 14:10 napari_nyxus-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-May-17 14:10 napari_nyxus-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 23-May-17 14:10 napari_nyxus-0.1.2.dist-info/RECORD
+11 files, 24458 bytes uncompressed, 7875 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: napari_nyxus/__init__.py
 Comment: 
 
 Filename: napari_nyxus/_version.py
 Comment: 
 
+Filename: napari_nyxus/napari.yaml
+Comment: 
+
 Filename: napari_nyxus/nyx.py
 Comment: 
 
 Filename: napari_nyxus/nyx_napari.py
 Comment: 
 
 Filename: napari_nyxus/util.py
 Comment: 
 
-Filename: napari_nyxus-0.1.1.dist-info/METADATA
+Filename: napari_nyxus-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: napari_nyxus-0.1.1.dist-info/WHEEL
+Filename: napari_nyxus-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: napari_nyxus-0.1.1.dist-info/entry_points.txt
+Filename: napari_nyxus-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: napari_nyxus-0.1.1.dist-info/top_level.txt
+Filename: napari_nyxus-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: napari_nyxus-0.1.1.dist-info/RECORD
+Filename: napari_nyxus-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## napari_nyxus/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-05-05T11:31:42-0400",
+ "date": "2023-05-17T10:09:10-0400",
  "dirty": false,
  "error": null,
- "full-revisionid": "7b4a6ff7289f5c01eaf6d8b78a7c60460116f117",
- "version": "0.1.1"
+ "full-revisionid": "3fb5a1c87e321ba641a79b78c8f566e4a9db5467",
+ "version": "0.1.2"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## napari_nyxus/nyx.py

```diff
@@ -1,9 +1,9 @@
 import napari
-from napari.layers import Image
+from napari.layers import Image, Labels
 from magicgui import magic_factory
 
 from napari_nyxus.nyx_napari import Features
 
 
 logo = "docs/source/img/polus.png"
 
@@ -16,19 +16,18 @@
         widget_type="Label", label=f"For information on the provided features see the <a href='https://nyxus.readthedocs.io/en/latest/featurelist.html'>documentation</a>"
     )
 )
 def widget_factory(
     label_head,
     viewer: napari.Viewer,
     Intensity: Image, 
-    Segmentation: Image,
+    Segmentation: Labels,
     Features: Features,
-    Save_to_csv: bool = True,
     Output_path: "str" = "",
-    Neighbor_distance: float = 5.0,
+    Neighbor_distance: int = 5,
     Pixels_per_micron: float = 1.0,
     Coarse_gray_depth: int = 256, 
     Use_CUDA_Enabled_GPU: bool = False,
     GPU_id: int = 0,
     documentation = ""
     ):
     
@@ -39,15 +38,14 @@
     import os
     
     nyx = nyx_napari.NyxusNapari(
         viewer,
         Intensity, 
         Segmentation,
         Features,
-        Save_to_csv,
         Output_path,
         Neighbor_distance,
         Pixels_per_micron,
         Coarse_gray_depth, 
         Use_CUDA_Enabled_GPU,
         GPU_id)
```

### html2text {}

```diff
@@ -1,17 +1,17 @@
-import napari from napari.layers import Image from magicgui import
+import napari from napari.layers import Image, Labels from magicgui import
 magic_factory from napari_nyxus.nyx_napari import Features logo = "docs/source/
 img/polus.png" @magic_factory( label_head=dict( #widget_type="Label", label=f'
 ****** [{logo}] Nyxus ******
 ' widget_type="Label", label=f'
 ****** Nyxus ******
 ' ), documentation=dict( widget_type="Label", label=f"For information on the
 provided features see the documentation" ) ) def widget_factory( label_head,
-viewer: napari.Viewer, Intensity: Image, Segmentation: Image, Features:
-Features, Save_to_csv: bool = True, Output_path: "str" = "", Neighbor_distance:
-float = 5.0, Pixels_per_micron: float = 1.0, Coarse_gray_depth: int = 256,
+viewer: napari.Viewer, Intensity: Image, Segmentation: Labels, Features:
+Features, Output_path: "str" = "", Neighbor_distance: int = 5,
+Pixels_per_micron: float = 1.0, Coarse_gray_depth: int = 256,
 Use_CUDA_Enabled_GPU: bool = False, GPU_id: int = 0, documentation = "" ):
 #wait for function call to load large modules from napari_nyxus import
 nyx_napari import pandas as pd import numpy as np import os nyx =
-nyx_napari.NyxusNapari( viewer, Intensity, Segmentation, Features, Save_to_csv,
-Output_path, Neighbor_distance, Pixels_per_micron, Coarse_gray_depth,
-Use_CUDA_Enabled_GPU, GPU_id) nyx.run()
+nyx_napari.NyxusNapari( viewer, Intensity, Segmentation, Features, Output_path,
+Neighbor_distance, Pixels_per_micron, Coarse_gray_depth, Use_CUDA_Enabled_GPU,
+GPU_id) nyx.run()
```

## napari_nyxus/nyx_napari.py

```diff
@@ -1,23 +1,27 @@
-from qtpy.QtWidgets import QWidget, QScrollArea, QTableWidget, QVBoxLayout,QTableWidgetItem, QLineEdit, QLabel, QHBoxLayout
-from qtpy.QtCore import Qt
+from qtpy.QtWidgets import QWidget, QScrollArea, QTableWidget, QVBoxLayout,QTableWidgetItem, QLineEdit, QLabel, QHBoxLayout, QAbstractItemView
+from qtpy.QtCore import Qt, QTimer
 from qtpy import QtCore, QtGui, QtWidgets
 from superqt import QLabeledDoubleRangeSlider
 import napari
-from napari.layers import Image
+from napari.layers import Image, Labels
 from napari.qt.threading import thread_worker
 from napari.utils.notifications import show_info
 from magicgui import magic_factory
 from enum import Enum
 import numpy as np
 import pandas as pd
 import dask
 
 from napari_nyxus import util
 
+#from napari_nyxus.table import TableWidget, add_table, get_table
+from napari_skimage_regionprops import TableWidget, add_table, get_table
+from napari_workflows._workflow import _get_layer_from_data
+
 import nyxus
 
 class Features(Enum):
     All = "*ALL*"
     Intensity = "*ALL_INTENSITY*"
     All_Morphology = "*ALL_MORPHOLOGY*"
     Basic_Morphology = "*BASIC_MORPHOLOGY*"
@@ -48,29 +52,27 @@
     
     """
     
     def __init__(
         self,
         viewer: napari.Viewer,
         intensity: Image, 
-        segmentation: Image,
+        segmentation: Labels,
         features: Features,
-        save_to_csv: bool = True,
         output_path: "str" = "",
-        neighbor_distance: float = 5.0,
+        neighbor_distance: int = 5,
         pixels_per_micron: float = 1.0,
         coarse_gray_depth: int = 256, 
         use_CUDA_Enabled_GPU: bool = False,
         gpu_id: int = 0):
 
         # Set class data
         self.viewer = viewer
         self.intensity = intensity
         self.segmentation = segmentation
-        self.save_to_csv = save_to_csv
         self.output_path = output_path
     
         self.nyxus_object = None
         self.result = None
 
         self.current_label = 0
         self.seg = self.segmentation.data
@@ -106,37 +108,55 @@
             self.nyxus_object = nyxus.Nyxus([features.value], 
                                     neighbor_distance=neighbor_distance, 
                                     pixels_per_micron=pixels_per_micron, 
                                     coarse_gray_depth=coarse_gray_depth,
                                     using_gpu = -1)
         
         # Add event handler for ROI clicking feature
+        
         @segmentation.mouse_drag_callbacks.append
-        def clicked_roi(layer, event):
+        def _after_labels_clicked(layer, event):
             """ Adds click event to segmentation image so when ROIs are clicked in the viewer,
             the correct ROI is highlighted in the results table
             """
             coords = np.round(event.position).astype(int)
-            value = layer.data[coords[0]][coords[1]]
+            
+            try:
+                value = layer.data[coords[0]][coords[1]]
+            except:
+                return
+            
             if (value == 0):
                 return
+
             self.table.selectRow(value-1)
             
+            self.after_click(value)
+            
         @intensity.mouse_drag_callbacks.append
-        def clicked_roi(layer, event):
+        def clicked_roi(layer, event, event1):
             """ Adds click event to intensity image so when ROIs are clicked in the viewer,
             the correct ROI is highlighted in the results table
             """
             coords = np.round(event.position).astype(int)
-            value = segmentation.data[coords[0]][coords[1]]
+            
+            try:
+                value = segmentation.data[coords[0]][coords[1]]
+            except:
+                return
+            
             if (value == 0):
                 return
+
             self.table.selectRow(value-1)
+
     
-    
+    def after_click(self, value):
+        self.table.selectRow(value-1)
+
   
     def run(self):  
         """ Run Nyxus on data from napari viewer
         """
         show_info("Calculating features...")
         self._run_calculate()
         self.add_features_table()
@@ -173,57 +193,67 @@
         for idx in np.ndindex(self.intensity.data.numblocks):
             results.append(self.nyxus_object.featurize(
                                 self.intensity.data.blocks[idx].compute(), 
                                 self.segmentation.data.blocks[idx].compute()))
             
         self.result = pd.concat(results)
     
-
-    def save_csv(self):
-        """ Saves feature calculations to a csv
-        """
-        if (self.save_to_csv):
-            show_info("Saving results to " + self.output_path + "out.csv")
-            self.result.to_csv(self.output_path + 'out.csv', sep='\t', encoding='utf-8')
     
     def add_features_table(self):
         """ Appends table consisting of results dataframe from the feature calculations to the
         Napari viewer
         """
-        #show_info("Creating features table")
-        self.save_csv()
+        show_info("Creating features table")
+
         self._add_features_table()
 
     
     def _add_features_table(self):   
         """ Adds table to Napari viewer
         """ 
-        # Create window for the DataFrame viewer
-        self.win = FeaturesWidget()
-        scroll = QScrollArea()
-        layout = QVBoxLayout()
-        self.table = QTableWidget()
-        scroll.setWidget(self.table)
-        layout.addWidget(self.table)
-        self.win.setLayout(layout)    
-        self.win.setWindowTitle("Feature Results")
-
-        # Add DataFrame to widget window
-        self.table.setColumnCount(len(self.result.columns))
-        self.table.setRowCount(len(self.result.index))
-        self.table.setHorizontalHeaderLabels(self.result.columns)
-        for i in range(len(self.result.index)):
-            for j in range(len(self.result.columns)):
-                self.table.setItem(i,j,QTableWidgetItem(str(self.result.iloc[i, j])))
-                
-        self.table.cellClicked.connect(self.cell_was_clicked)
-        self.table.horizontalHeader().sectionClicked.connect(self.onHeaderClicked)
 
-        # add DataFrame to Viewer
-        self.viewer.window.add_dock_widget(self.win)
+        labels_layer = _get_layer_from_data(self.viewer, self.seg)
+        new_table = self.result.to_dict()
+        
+        flipped_dict = {}
+        for key, value in new_table.items():
+            values_list = list(value.values())
+            flipped_dict[key] = values_list
+            
+        
+        labels_layer.properties = flipped_dict
+        
+        add_table(labels_layer, self.viewer)
+        
+        widget_table = get_table(labels_layer, self.viewer)
+        
+        self.table = widget_table._view
+        
+        self.table.cellDoubleClicked.connect(self.cell_was_clicked)
+
+        # remove label clicking event to use our own
+        widget_table._layer.mouse_drag_callbacks.remove(widget_table._clicked_labels)
+        
+        # add new label clicking event
+        self.table.horizontalHeader().sectionDoubleClicked.connect(self.onHeaderClicked)
+
+            
+    def cell_was_clicked(self, event):
+        
+        if (self.batched):
+            show_info('Feature not enabled for batched processing')
+            return
+        
+        current_column = self.table.currentColumn()
+        
+        if(current_column == 2):
+            current_row = self.table.currentRow()
+            cell_value = self.table.item(current_row, current_column).text()
+            
+            self.highlight_value(cell_value)
     
     def highlight_value(self, value):
         """ 
         """
         
         if (self.batched):
             show_info('Feature not enabled for batched processing')
@@ -244,84 +274,43 @@
             self.current_label += 1
             
         if (not self.labels_added):
             self.viewer.add_labels(np.array(self.labels).astype('int8'), name="Selected ROI")
             self.labels_added = True
         else:
             self.viewer.layers["Selected ROI"].data = np.array(self.labels).astype('int8')
-
-            
-    def cell_was_clicked(self, event):
-        
-        if (self.batched):
-            show_info('Feature not enabled for batched processing')
-            return
-        
-        current_column = self.table.currentColumn()
-        
-        if(current_column == 2):
-            current_row = self.table.currentRow()
-            cell_value = self.table.item(current_row, current_column).text()
-            
-            self.highlight_value(cell_value)
-    
+ 
     def onHeaderClicked(self, logicalIndex):
         
         if (self.batched):
             show_info('Feature not enabled for batched processing')
             return
+
+        column = self.result.columns[logicalIndex]
         
-        self.create_feature_color_map(logicalIndex)
+        self.slider_feature_name = column
         
-    def create_feature_color_map(self, logicalIndex):
+        max = self.result[column].max()
+        min = self.result[column].min()
         
-        if (self.batched):
-            show_info('Feature not enabled for batched processing')
-            return
-        
-        self.colormap = np.zeros_like(self.seg)
+        self.slider_layer_name = column + " in " + self.segmentation.name
         
         labels = self.result.iloc[:,2]
         values = self.result.iloc[:,logicalIndex]
         self.label_values = pd.Series(values, index=labels).to_dict()
         
-        min_value = float('inf')
-        max_value = float('-inf')
-
-        self.slider_feature_name = self.result.columns[logicalIndex]
-        
-        for ix, iy in np.ndindex(self.seg.shape):
-            
-            if (self.seg[ix, iy] != 0):
-                if(np.isnan(self.label_values[int(self.seg[ix, iy])])):
-                    continue
-                
-                value = self.label_values[int(self.seg[ix, iy])]
+        self.colormap = None
+        for layer in self.viewer.layers:
+            if layer.name == self.slider_layer_name:
+                self.colormap = layer.data 
                 
-                min_value = min(min_value, value)
-                max_value = max(max_value, value)
+        if (self.colormap is None):
+            raise RuntimeError(f"Colormap layer {self.slider_layer_name} not found.")
                 
-                self.colormap[ix, iy] = value
-                
-            else:
-                self.colormap[ix, iy] = 0
-        
-        if (not self.colormap_added):
-            self.viewer.add_image(np.array(self.colormap), name="Colormap")
-            self.colormap_added = True
-            
-        else:
-            self.viewer.layers["Colormap"].data = np.array(self.colormap)
-        
-        #if (self.slider_added):
-        #    self._update_slider([min_value, max_value])
-            
-        #else:
-        self._add_range_slider(min_value, max_value)
-        
+        self._add_range_slider(min, max)
     
     
     def _get_label_from_range(self, min_bound, max_bound):
 
         for ix, iy in np.ndindex(self.colormap.shape):
             
             if (self.seg[ix, iy] != 0):
@@ -334,36 +323,33 @@
                 if (value <= max_bound and value >= min_bound):
                     self.labels[ix, iy] = self.seg[ix, iy]
                     self.colormap[ix, iy] = value
                 else:
                     self.labels[ix, iy] = 0
                     self.colormap[ix, iy] = 0
                 
-        if (not self.colormap_added):
-            self.viewer.add_image(np.array(self.colormap), name="Colormap")
-            self.colormap_added = True
-            
-        else:
-            self.viewer.layers["Colormap"].data = np.array(self.colormap)
+       
+        self.viewer.layers[self.slider_layer_name].data = np.array(self.colormap)
             
              
         if (not self.labels_added):
             self.viewer.add_labels(np.array(self.labels).astype('int8'), name="Selected ROI")
             self.labels_added = True
             
         else:
             self.viewer.layers["Selected ROI"].data = np.array(self.labels).astype('int8')
             
     
     def _add_range_slider(self, min_value, max_value):
+
         min_value = util.round_down_to_5_sig_figs(min_value)
         max_value = util.round_up_to_5_sig_figs(max_value)
         
         if (self.slider_added):
-            print("in slider added code")
+
             self.slider.setRange(min_value, max_value)
             self.range = [min_value, max_value]
             self.slider.setValue([min_value, max_value])
             self.name_label.setText(self.slider_feature_name)
             self.min_box.setText(str(min_value))
             self.max_box.setText(str(max_value))
             
@@ -406,18 +392,21 @@
             self.label.setAlignment(Qt.AlignCenter)
             self.dock_widget.setTitleBarWidget(self.label)
 
             self.slider_added = True
 
         
     def _update_slider(self, event):
+        
         min_value = util.round_down_to_5_sig_figs(event[0])
         max_value = util.round_up_to_5_sig_figs(event[1])
+        
         self.min_box.setText(str(min_value))
         self.max_box.setText(str(max_value))
+        
         self._get_label_from_range(min_value, max_value)
 
     def _get_minimum_text(self):
         user_input = self.min_box.text()
 
         try :
             value = float(user_input)
@@ -427,12 +416,14 @@
             return
         
     def _get_maximum_text(self):
         user_input = self.max_box.text()
 
         try: 
             value = float(user_input)
-            if (value >= self.range[0] and value <= self.range[1]):
+            if (value >= self.range[0] and value <= self.range[1]): 
                 self.slider.setValue([float(self.min_box.text()), value])
         
         except:
-            return
+            return
+            
+
```

## Comparing `napari_nyxus-0.1.1.dist-info/METADATA` & `napari_nyxus-0.1.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: napari-nyxus
-Version: 0.1.1
+Version: 0.1.2
 Summary: A napari plugin for calculating features from intensity-label image data
 Home-page: https://github.com/PolusAI/napari-nyxus
 Author: Jesse McKinzie
 Author-email: Jesse.McKinzie@axleinfo.com
 Classifier: Framework :: napari
 Description-Content-Type: text/markdown
 Requires-Dist: napari
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: nyxus (>=0.5.0)
 Requires-Dist: imagecodecs
+Requires-Dist: napari-skimage-regionprops
 
 # Nyxus Napari
 
 Nyxus Napari is a Napari plugin for running feature calculations on image-segmentation image pairs, using the
 Nyxus application to compute features. Nyxus is a feature-rich, highly optimized, Python/C++ application capable 
 of analyzing images of arbitrary size and assembling complex regions of interest (ROIs) split across multiple image tiles and files. 
 
@@ -78,34 +79,45 @@
 ![](docs/source/img/nyxus_loaded.png)
 
 As shown by the example above, Nyxus will take in Intensity and Segmentation images. These parameters can either be a stack
 of images or a single image pair. To load an image pair, use File -> Open File(s)... and select the images to load.
 
 ![](docs/source/img/open_image.png)
 
+
 Note that this method can also be used to open a stack of image, by using File -> Open Folder... instead of images. 
+
+If the segmentation is loaded as an Image type in the napari viewer, it must first be converted to the Labels type. The image can converted as shown below.
+
+![](docs/source/img/convert_to_labels.png)
+
 The loaded files can then be selected with the Intensity and Segmentation drop down menus. Other parameters can also be changed,
 such as which features to calculate. For more information on the available features, see https://nyxus.readthedocs.io/en/latest/featurelist.html.
 
 ![](docs/source/img/setup_calculation.png)
 
-There is an option to save the feature calculations to a csv file using the Save to csv option. If no path is prodivded in Output path,
-the csv will be saved to the current working directory. After running Nyxus, the feature calculations will also appear in the Napari viewer.
+After running Nyxus, the feature calculations will also appear in the Napari viewer.
 
 ![](docs/source/img/feature_results.png)
 
-The Nyxus Napari plugin provides functionality to interact with the table containing the feature calculatins. For example, if a value
-is clicked in the `label` column of the table, the respective ROI will be highlighted in the segmentation image in the viewer.
+The Nyxus Napari plugin provides functionality to interact with the table containing the feature calculations. First, click on the segmentation image and then select `show selected` in the layer controls. 
+
+
+Then, if a value is clicked in the `label` column of the table, the respective ROI will be highlighted in the segmentation image in the viewer.
 
 ![](docs/source/img/click_label.png)
 
+To select the ROI and have it added to a separate Labels image, the label in the table can be double clicked. Each double clicked label will be added to the same Labels image as show below. To unselect, the ROI, double click its respective label again.
+
+![](docs/source/img/double_click_label.png)
+
 This feature can also be used in the opposite way, i.e. if an ROI is clicked in the segmentation image, the respective row in the 
 feature table will be highlighted.
 
-If one of the column headers are clicked, a colormap will be generated in the Napari viewer showing the values of the features in the clicked
+If one of the column headers are double clicked, a colormap will be generated in the Napari viewer showing the values of the features in the clicked
 column. For example, if `Intensity` features are calculated, the `INTEGRATED_INTENSITY` column can be clicked and the colormap will appear.
 
 ![](docs/source/img/feature_colormap.png)
 
 Once the colormap is loaded, a slider will appear in the window with the minimum value being the minimum value of the feature colormap and the 
 maximum value of the slider is the maximum value of the colormap. By adjusting the ranges in the slider, a new label image will appear in the viewer
 that contains the ROIs who's features values fall within the slider values.
```

