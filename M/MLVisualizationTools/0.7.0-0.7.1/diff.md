# Comparing `tmp/MLVisualizationTools-0.7.0.tar.gz` & `tmp/MLVisualizationTools-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLVisualizationTools-0.7.0.tar", last modified: Sun May  7 03:37:03 2023, max compression
+gzip compressed data, was "MLVisualizationTools-0.7.1.tar", last modified: Wed May 17 19:46:42 2023, max compression
```

## Comparing `MLVisualizationTools-0.7.0.tar` & `MLVisualizationTools-0.7.1.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.690009 MLVisualizationTools-0.7.0/MLVisualizationTools/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/colorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/dashbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/datainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/AnimationDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashKaggleDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashNotebookDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DataOverlayDemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.682010 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train.csv
--rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/MatplotlibDemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.682010 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb
--rw-r--r--   0 runner    (1001) docker     (123)    93696 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb
--rw-r--r--   0 runner    (1001) docker     (123)    89084 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/SklearnDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/TrainTitanicModel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/express/
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/express/DashModelVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/express/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/graphinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/modelanalytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/modelinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.682010 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/dark_assets/
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/dark_assets/darktheme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/light_assets/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/light_assets/lighttheme.css
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.690009 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/tests/testconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.874645 MLVisualizationTools-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.866645 MLVisualizationTools-0.7.1/MLVisualizationTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/colorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/dashbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/datainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.870645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/AnimationDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DashDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DashKaggleDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DashNotebookDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DataOverlayDemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.866645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.870645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/Titanic/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/Titanic/train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/MatplotlibDemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.866645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.870645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb
+-rw-r--r--   0 runner    (1001) docker     (123)    93696 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.870645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.870645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb
+-rw-r--r--   0 runner    (1001) docker     (123)    89084 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.870645 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/RemoveFeatureDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/SklearnDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/examples/TrainTitanicModel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.874645 MLVisualizationTools-0.7.1/MLVisualizationTools/express/
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/express/DashModelVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/express/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/graphinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/modelanalytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/modelinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/removefeature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.866645 MLVisualizationTools-0.7.1/MLVisualizationTools/theme_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.874645 MLVisualizationTools-0.7.1/MLVisualizationTools/theme_assets/dark_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/theme_assets/dark_assets/darktheme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.874645 MLVisualizationTools-0.7.1/MLVisualizationTools/theme_assets/light_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/theme_assets/light_assets/lighttheme.css
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/MLVisualizationTools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.870645 MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-17 19:46:42.000000 MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-17 19:46:42.000000 MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:46:42.000000 MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 19:46:42.000000 MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 19:46:42.000000 MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-17 19:46:42.874645 MLVisualizationTools-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 19:46:42.874645 MLVisualizationTools-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:46:42.874645 MLVisualizationTools-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 19:46:31.000000 MLVisualizationTools-0.7.1/tests/testconf.py
```

### Comparing `MLVisualizationTools-0.7.0/LICENSE` & `MLVisualizationTools-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/backend.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/backend.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/colorizers.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/colorizers.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/dashbackend.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/dashbackend.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/datainterface.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/datainterface.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/AnimationDemo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/AnimationDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashDemo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DashDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashKaggleDemo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DashKaggleDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashNotebookDemo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DashNotebookDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DataOverlayDemo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/DataOverlayDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train.csv` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/Titanic/train.csv`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Demo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Demo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/MatplotlibDemo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/MatplotlibDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/SklearnDemo.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/SklearnDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/TrainTitanicModel.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/examples/TrainTitanicModel.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/express/DashModelVisualizer.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/express/DashModelVisualizer.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/graphinterface.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/graphinterface.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/modelanalytics.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/modelanalytics.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/modelinterface.py` & `MLVisualizationTools-0.7.1/MLVisualizationTools/modelinterface.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/dark_assets/darktheme.css` & `MLVisualizationTools-0.7.1/MLVisualizationTools/theme_assets/dark_assets/darktheme.css`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/PKG-INFO` & `MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLVisualizationTools
-Version: 0.7.0
+Version: 0.7.1
 Summary: A set of functions and demos to make machine learning projects easier to understand through effective visualizations.
 Home-page: https://github.com/RobertJN64/MLVisualizationTools
 Author: Robert Nies
 Author-email: robertjnies@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -72,23 +72,23 @@
 ```
 
 ## Functions
 
 MLVisualizationTools connects a variety of smaller functions.
 
 Steps:
-1. Keras Model and Dataframe with features
+1. Start with a ML Model and Dataframe with features
 2. Analyzer
 3. Interface / Interface Raw (if you don't have a dataframe)
 4. Colorizers (optional)
 5. Apply Training Data Points (Optional)
 6. Colorize data points (Optional)
 7. Graphs
 
-Analyzers take a keras model and return information about the inputs
+Analyzers take a ml model and return information about the inputs
 such as which ones have high variance.
 
 Interfaces take parameters and construct a multidimensional grid
 of values based on plugging these numbers into the model.
 
 (Raw interfaces allow you to use interfaces by specifying column
 data instead of a pandas dataframe. Column data is a list with a dict with name, min,
@@ -133,14 +133,33 @@
 - DashKaggleDemo: Notebook version of an dash demo that works in kaggle
 notebooks
 - DataOverlayDemo: Demonstrates data overlay features
 
 See [MLVisualizationTools/Examples](/MLVisualizationTools/examples) for more examples.
 Use example.main() to run the examples and set parameters such as themes.
 
+## Tensorflow Compatibility
+
+MLVisualizationTools is distributed with a pretrained tensorflow model
+to make running examples quick and easy. It is not needed for main library functions.
+
+For version 2.0 through 2.4, we load a v2.0 model.
+For version 2.5+ we load a v2.5 model.
+
+If this causes compatibility issues you can still use the main library on your models. 
+If you need an example model, retrain it with 
+[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
+
+## scikit-learn Compatibility
+
+See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+
+Sklearn can be used exactly like TF because it has the same `.predict(X) -> Y` interface.
+
+
 ## Support for more ML Libraries
 
 We support any ML library that has a `predict()` call that takes
 a pd Dataframe with features. If this doesn't work, use a wrapper class like 
 in this example:
 
 ```python
@@ -150,24 +169,13 @@
     def __init(self, model):
         self.model = model
 
     def predict(self, dataframe: pd.DataFrame):
         ... #Do whatever code you need here
 ```
 
-## Tensorflow Compatibility
-
-MLVisualizationTools is distributed with a pretrained tensorflow model
-to make running examples quick and easy. It is not needed for main library functions.
-
-For version 2.0 through 2.4, we load a v2.0 model.
-For version 2.5+ we load a v2.5 model.
-
-If this causes compatibility issues you can still use the main library on your models. 
-If you need an example model, retrain it with 
-[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
-
-## scikit-learn Compatibility
+## Remove Feature Testing
 
-See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+See [RemoveFeatureDemo.py](/MLVisualizationTools/examples/RemoveFeatureDemo.py)
 
-Sklearn can be used exactly like TF because it has the same `.predict(X, Y)` interface.
+Tests if features can be removed from dataset without significantly affecting accuracy.
+Replaces each dataset column with mean and compares to baseline accuracy.
```

### Comparing `MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/SOURCES.txt` & `MLVisualizationTools-0.7.1/MLVisualizationTools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 MLVisualizationTools/backend.py
 MLVisualizationTools/colorizers.py
 MLVisualizationTools/dashbackend.py
 MLVisualizationTools/datainterface.py
 MLVisualizationTools/graphinterface.py
 MLVisualizationTools/modelanalytics.py
 MLVisualizationTools/modelinterface.py
+MLVisualizationTools/removefeature.py
 MLVisualizationTools/types.py
 MLVisualizationTools.egg-info/PKG-INFO
 MLVisualizationTools.egg-info/SOURCES.txt
 MLVisualizationTools.egg-info/dependency_links.txt
 MLVisualizationTools.egg-info/requires.txt
 MLVisualizationTools.egg-info/top_level.txt
 MLVisualizationTools/examples/AnimationDemo.py
 MLVisualizationTools/examples/DashDemo.py
 MLVisualizationTools/examples/DashKaggleDemo.py
 MLVisualizationTools/examples/DashNotebookDemo.py
 MLVisualizationTools/examples/DataOverlayDemo.py
 MLVisualizationTools/examples/Demo.py
 MLVisualizationTools/examples/MatplotlibDemo.py
+MLVisualizationTools/examples/RemoveFeatureDemo.py
 MLVisualizationTools/examples/SklearnDemo.py
 MLVisualizationTools/examples/TrainTitanicModel.py
 MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py
 MLVisualizationTools/examples/Datasets/Titanic/train.csv
 MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv
 MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb
 MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb
```

### Comparing `MLVisualizationTools-0.7.0/PKG-INFO` & `MLVisualizationTools-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLVisualizationTools
-Version: 0.7.0
+Version: 0.7.1
 Summary: A set of functions and demos to make machine learning projects easier to understand through effective visualizations.
 Home-page: https://github.com/RobertJN64/MLVisualizationTools
 Author: Robert Nies
 Author-email: robertjnies@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -72,23 +72,23 @@
 ```
 
 ## Functions
 
 MLVisualizationTools connects a variety of smaller functions.
 
 Steps:
-1. Keras Model and Dataframe with features
+1. Start with a ML Model and Dataframe with features
 2. Analyzer
 3. Interface / Interface Raw (if you don't have a dataframe)
 4. Colorizers (optional)
 5. Apply Training Data Points (Optional)
 6. Colorize data points (Optional)
 7. Graphs
 
-Analyzers take a keras model and return information about the inputs
+Analyzers take a ml model and return information about the inputs
 such as which ones have high variance.
 
 Interfaces take parameters and construct a multidimensional grid
 of values based on plugging these numbers into the model.
 
 (Raw interfaces allow you to use interfaces by specifying column
 data instead of a pandas dataframe. Column data is a list with a dict with name, min,
@@ -133,14 +133,33 @@
 - DashKaggleDemo: Notebook version of an dash demo that works in kaggle
 notebooks
 - DataOverlayDemo: Demonstrates data overlay features
 
 See [MLVisualizationTools/Examples](/MLVisualizationTools/examples) for more examples.
 Use example.main() to run the examples and set parameters such as themes.
 
+## Tensorflow Compatibility
+
+MLVisualizationTools is distributed with a pretrained tensorflow model
+to make running examples quick and easy. It is not needed for main library functions.
+
+For version 2.0 through 2.4, we load a v2.0 model.
+For version 2.5+ we load a v2.5 model.
+
+If this causes compatibility issues you can still use the main library on your models. 
+If you need an example model, retrain it with 
+[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
+
+## scikit-learn Compatibility
+
+See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+
+Sklearn can be used exactly like TF because it has the same `.predict(X) -> Y` interface.
+
+
 ## Support for more ML Libraries
 
 We support any ML library that has a `predict()` call that takes
 a pd Dataframe with features. If this doesn't work, use a wrapper class like 
 in this example:
 
 ```python
@@ -150,24 +169,13 @@
     def __init(self, model):
         self.model = model
 
     def predict(self, dataframe: pd.DataFrame):
         ... #Do whatever code you need here
 ```
 
-## Tensorflow Compatibility
-
-MLVisualizationTools is distributed with a pretrained tensorflow model
-to make running examples quick and easy. It is not needed for main library functions.
-
-For version 2.0 through 2.4, we load a v2.0 model.
-For version 2.5+ we load a v2.5 model.
-
-If this causes compatibility issues you can still use the main library on your models. 
-If you need an example model, retrain it with 
-[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
-
-## scikit-learn Compatibility
+## Remove Feature Testing
 
-See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+See [RemoveFeatureDemo.py](/MLVisualizationTools/examples/RemoveFeatureDemo.py)
 
-Sklearn can be used exactly like TF because it has the same `.predict(X, Y)` interface.
+Tests if features can be removed from dataset without significantly affecting accuracy.
+Replaces each dataset column with mean and compares to baseline accuracy.
```

### Comparing `MLVisualizationTools-0.7.0/README.md` & `MLVisualizationTools-0.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,23 +49,23 @@
 ```
 
 ## Functions
 
 MLVisualizationTools connects a variety of smaller functions.
 
 Steps:
-1. Keras Model and Dataframe with features
+1. Start with a ML Model and Dataframe with features
 2. Analyzer
 3. Interface / Interface Raw (if you don't have a dataframe)
 4. Colorizers (optional)
 5. Apply Training Data Points (Optional)
 6. Colorize data points (Optional)
 7. Graphs
 
-Analyzers take a keras model and return information about the inputs
+Analyzers take a ml model and return information about the inputs
 such as which ones have high variance.
 
 Interfaces take parameters and construct a multidimensional grid
 of values based on plugging these numbers into the model.
 
 (Raw interfaces allow you to use interfaces by specifying column
 data instead of a pandas dataframe. Column data is a list with a dict with name, min,
@@ -110,14 +110,33 @@
 - DashKaggleDemo: Notebook version of an dash demo that works in kaggle
 notebooks
 - DataOverlayDemo: Demonstrates data overlay features
 
 See [MLVisualizationTools/Examples](/MLVisualizationTools/examples) for more examples.
 Use example.main() to run the examples and set parameters such as themes.
 
+## Tensorflow Compatibility
+
+MLVisualizationTools is distributed with a pretrained tensorflow model
+to make running examples quick and easy. It is not needed for main library functions.
+
+For version 2.0 through 2.4, we load a v2.0 model.
+For version 2.5+ we load a v2.5 model.
+
+If this causes compatibility issues you can still use the main library on your models. 
+If you need an example model, retrain it with 
+[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
+
+## scikit-learn Compatibility
+
+See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+
+Sklearn can be used exactly like TF because it has the same `.predict(X) -> Y` interface.
+
+
 ## Support for more ML Libraries
 
 We support any ML library that has a `predict()` call that takes
 a pd Dataframe with features. If this doesn't work, use a wrapper class like 
 in this example:
 
 ```python
@@ -127,24 +146,13 @@
     def __init(self, model):
         self.model = model
 
     def predict(self, dataframe: pd.DataFrame):
         ... #Do whatever code you need here
 ```
 
-## Tensorflow Compatibility
-
-MLVisualizationTools is distributed with a pretrained tensorflow model
-to make running examples quick and easy. It is not needed for main library functions.
-
-For version 2.0 through 2.4, we load a v2.0 model.
-For version 2.5+ we load a v2.5 model.
-
-If this causes compatibility issues you can still use the main library on your models. 
-If you need an example model, retrain it with 
-[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
-
-## scikit-learn Compatibility
+## Remove Feature Testing
 
-See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+See [RemoveFeatureDemo.py](/MLVisualizationTools/examples/RemoveFeatureDemo.py)
 
-Sklearn can be used exactly like TF because it has the same `.predict(X, Y)` interface.
+Tests if features can be removed from dataset without significantly affecting accuracy.
+Replaces each dataset column with mean and compares to baseline accuracy.
```

### Comparing `MLVisualizationTools-0.7.0/setup.cfg` & `MLVisualizationTools-0.7.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = MLVisualizationTools
 description = A set of functions and demos to make machine learning projects easier to understand through effective visualizations.
 author = Robert Nies
 license = MIT
 license_file = LICENSE
 url = https://github.com/RobertJN64/MLVisualizationTools
 author_email = robertjnies@gmail.com
-version = 0.7.0
+version = 0.7.1
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
```

### Comparing `MLVisualizationTools-0.7.0/tests/test_basic.py` & `MLVisualizationTools-0.7.1/tests/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,7 +208,12 @@
     project.DataInterfaces.addClumpedData(anim, df, outputkey='Survived')
 
     grid = project.Colorizers.simple(grid, 'white', apply_to_data=True)
 
     project.Graphs.plotlyGraph(anim)
     project.Graphs.plotlyGraph(panim)
     project.Graphs.matplotlibGraph(grid)
+
+def test_rm_feature():
+    from MLVisualizationTools.examples import RemoveFeatureDemo
+    RemoveFeatureDemo.main() #verbose true
+    RemoveFeatureDemo.main(False) #verbose false
```

