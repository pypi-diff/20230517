# Comparing `tmp/napari-feature-classifier-0.1.0.tar.gz` & `tmp/napari-feature-classifier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-feature-classifier-0.1.0.tar", last modified: Tue May  9 18:05:29 2023, max compression
+gzip compressed data, was "napari-feature-classifier-0.1.1.tar", last modified: Wed May 17 18:52:38 2023, max compression
```

## Comparing `napari-feature-classifier-0.1.0.tar` & `napari-feature-classifier-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.249215 napari-feature-classifier-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.249215 napari-feature-classifier-0.1.0/src/napari_feature_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_annotator_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_classifier_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/annotator_init_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/annotator_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/classifier_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/dev_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/feature_loader_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-09 18:05:11.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:05:29.253214 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 18:05:29.000000 napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:52:38.381378 napari-feature-classifier-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-17 18:52:38.381378 napari-feature-classifier-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-17 18:52:38.385378 napari-feature-classifier-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:52:38.381378 napari-feature-classifier-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:52:38.381378 napari-feature-classifier-0.1.1/src/napari_feature_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:52:38.381378 napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/test_annotator_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/test_classifier_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/annotator_init_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/annotator_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24268 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/classifier_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/dev_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/feature_loader_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-17 18:52:17.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:52:38.381378 napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-17 18:52:38.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-17 18:52:38.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:52:38.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 18:52:38.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-17 18:52:38.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 18:52:38.000000 napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/top_level.txt
```

### Comparing `napari-feature-classifier-0.1.0/LICENSE` & `napari-feature-classifier-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/PKG-INFO` & `napari-feature-classifier-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-feature-classifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: An interactive classifier plugin to use with label images and feature measurements
 Home-page: https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
 Author: Joel Luethi and Max Hess
 Author-email: joel.luethi@uzh.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/issues
 Project-URL: Documentation, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier#napari-feature-classifier
```

### Comparing `napari-feature-classifier-0.1.0/README.md` & `napari-feature-classifier-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/setup.cfg` & `napari-feature-classifier-0.1.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-feature-classifier
-version = 0.1.0
+version = 0.1.1
 author = Joel Luethi and Max Hess
 author_email = joel.luethi@uzh.ch
 url = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
 project_urls = 
 	Bug Tracker = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/issues
 	Documentation = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier#napari-feature-classifier
 	Source Code = https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
@@ -35,15 +35,15 @@
 	=src
 install_requires = 
 	numpy
 	napari
 	matplotlib
 	magicgui
 	pandas
-	scikit-learn
+	scikit-learn >= 1.2.2
 	pandera
 	xxhash
 	hypothesis
 
 [options.packages.find]
 where = src
```

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_annotator_widgets.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/test_annotator_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_classifier.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/_tests/test_classifier_widget.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/_tests/test_classifier_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """ Tests for classifier widget initialization"""
 import numpy as np
 import pandas as pd
+import pytest
+import os
 
 import imageio
 from pathlib import Path
 from napari_feature_classifier.feature_loader_widget import make_features
 from napari_feature_classifier.classifier_widget import (
     ClassifierWidget,
 )
@@ -27,25 +29,27 @@
     classifier_widget.initialize_run_widget()
 
     # TODO: Catch that it doesn't actually initialize, but instead shows a 
     # message to the user that now features were selected
     assert classifier_widget._run_container is None
 
 
+
+features = make_features(np.unique(lbl_img_np)[1:], roi_id="ROI1", n_features=6)
+features_no_roi_id = features.drop(columns=["roi_id"])
 # make_napari_viewer is a pytest fixture that returns a napari viewer object
-# TODO: Verify the actual results of the classification
-def test_running_classification_through_widget(make_napari_viewer):
+@pytest.mark.parametrize("features", [features, features_no_roi_id])
+def test_running_classification_through_widget(features, make_napari_viewer):
     """
     Tests if the main widget launches
     """
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
     label_layer = viewer.add_labels(lbl_img_np)
-    labels = np.unique(lbl_img_np)[1:]
-    label_layer.features = make_features(labels, roi_id="ROI1", n_features=6)
+    label_layer.features = features
 
     # Start init widget
     classifier_widget = ClassifierWidget(viewer)
 
     # Select relevant features
     classifier_widget._init_container._feature_combobox.value = [
         "feature_1",
@@ -62,11 +66,20 @@
     label_layer.features.loc[0, "annotations"] = 1.0
     label_layer.features.loc[1, "annotations"] = 1.0
     label_layer.features.loc[3, "annotations"] = 3.0
 
     # Run the classifier
     classifier_widget._run_container.run()
 
-    # TODO: Assert something
+    # Assert something that the layer is visible, predictions exist and are not NaN
     assert classifier_widget._run_container._prediction_layer.visible
     assert "prediction" in label_layer.features.columns
     assert pd.notna(label_layer.features["prediction"]).all().all()
+
+    # Check that the classifier file was saved
+    assert Path("lbl_img_np_classifier.clf").exists()
+
+    # Delete the classifier file (cleanup to avoid overwriting confirmation)
+    os.remove("lbl_img_np_classifier.clf")
+
+# TODO: Add a test to check the overwrite confirmations working correctly
+# For classifier files, for annotations and for exported predictions
```

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/annotator_init_widget.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/annotator_init_widget.py`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/annotator_widget.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/annotator_widget.py`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/classifier.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,17 +194,16 @@
         ----------
         dict_of_features : dict
             Dictionary with roi as key and dataframe with feature measurements 
             and annotations as value
         """
         for roi in dict_of_features:
             if "roi_id" not in dict_of_features[roi]:
-                df = dict_of_features[roi]["roid_id"] = roi
-            else:
-                df = df = dict_of_features[roi]
+                dict_of_features[roi]["roi_id"] = roi
+            df = dict_of_features[roi]
             napari_info(f"Adding features for {roi=}...")
             self.add_features(df)
 
     def get_class_names(self):
         return self._class_names
 
     def get_feature_names(self):
```

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/classifier_widget.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/classifier_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,16 +294,20 @@
         Run method that adds features to the classifier, trains it, triggers
         predictions & saves the classifier
         """
 
         self.add_features_to_classifier()
         try:
             self._classifier.train()
-        except ValueError:
-            napari_info("Not enough annotations made. Please make more annotations.")
+        except ValueError as e:
+            napari_info(
+                "Training failed. A typical reason are not having "
+                "enough annotations. \nThe error message was: "
+                f"{e}"
+            )
         else:
             self.make_predictions()
             self._prediction_layer.visible = True
             self.save()
 
     def add_features_to_classifier(self):
         """
@@ -498,15 +502,17 @@
     def _update_export_destination(self, label_layer: napari.layers.Labels):
         """
         Update the default export destination to the name of the label layer.
         If a base_path was already set, keep it on that base path.
 
         """
         base_path = Path(self._export_destination.value).parent
-        self._export_destination.value = base_path / f"annotation_{label_layer.name}.csv"
+        self._export_destination.value = (
+            base_path / f"{label_layer.name}_predictions.csv"
+        )
 
     def export_results(self):
         """
         Export classifier results for the current layer if available
         """
         if not overwrite_check_passed(
             file_path=self._export_destination.value, output_type="predictions"
```

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/dev_main.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/dev_main.py`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/feature_loader_widget.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/feature_loader_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,8 +66,9 @@
         warn_str = "Label image labels do not match with feature table.\n"
         "Label objects with no features: "
         f"{sorted(set(image_labels).difference(feature_labels))}\n"
         "Features with no label objects: "
         f"{sorted(set(feature_labels).difference(image_labels))}"
         napari_info(warn_str)
         warnings.warn(warn_str)
+    napari_info(f"Loaded features and attached them to \"{layer}\" layer")
     return (layer.data, {"name": layer.name, "features": df}, "labels")
```

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/napari.yaml` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier/utils.py` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier/utils.py`

 * *Files identical despite different names*

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/PKG-INFO` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-feature-classifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: An interactive classifier plugin to use with label images and feature measurements
 Home-page: https://github.com/fractal-napari-plugins-collection/napari-feature-classifier
 Author: Joel Luethi and Max Hess
 Author-email: joel.luethi@uzh.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier/issues
 Project-URL: Documentation, https://github.com/fractal-napari-plugins-collection/napari-feature-classifier#napari-feature-classifier
```

### Comparing `napari-feature-classifier-0.1.0/src/napari_feature_classifier.egg-info/SOURCES.txt` & `napari-feature-classifier-0.1.1/src/napari_feature_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

