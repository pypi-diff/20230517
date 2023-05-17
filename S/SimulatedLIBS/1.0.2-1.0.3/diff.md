# Comparing `tmp/SimulatedLIBS-1.0.2.tar.gz` & `tmp/SimulatedLIBS-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimulatedLIBS-1.0.2.tar", last modified: Sat Feb 25 19:56:12 2023, max compression
+gzip compressed data, was "SimulatedLIBS-1.0.3.tar", last modified: Wed May 17 18:41:46 2023, max compression
```

## Comparing `SimulatedLIBS-1.0.2.tar` & `SimulatedLIBS-1.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.937240 SimulatedLIBS-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.909239 SimulatedLIBS-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.913240 SimulatedLIBS-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-02-25 19:56:12.937240 SimulatedLIBS-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.913240 SimulatedLIBS-1.0.2/SimulatedLIBS/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/animation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.909239 SimulatedLIBS-1.0.2/SimulatedLIBS/animations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.917240 SimulatedLIBS-1.0.2/SimulatedLIBS/animations/saved-gifs/
--rw-r--r--   0 runner    (1001) docker     (123)   203642 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/animations/saved-gifs/animated_density.gif
--rw-r--r--   0 runner    (1001) docker     (123)   805303 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/animations/saved-gifs/animated_resolution.gif
--rw-r--r--   0 runner    (1001) docker     (123)   271781 2023-02-25 19:56:00.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/animations/saved-gifs/animated_temperature.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.917240 SimulatedLIBS-1.0.2/SimulatedLIBS/drivers/
--rw-r--r--   0 runner    (1001) docker     (123) 11775488 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/drivers/chromedriver.exe
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/SimulatedLIBS/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.913240 SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-02-25 19:56:12.000000 SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-25 19:56:12.000000 SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 19:56:12.000000 SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-25 19:56:12.000000 SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-25 19:56:12.000000 SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.933240 SimulatedLIBS-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/docs/libs-dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3253118 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/docs/output.csv
--rw-r--r--   0 runner    (1001) docker     (123)    98115 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/docs/single-spectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   141185 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/docs/single_simulation.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.933240 SimulatedLIBS-1.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.933240 SimulatedLIBS-1.0.2/examples/output_data/
--rw-r--r--   0 runner    (1001) docker     (123)    22285 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/examples/output_data/plot_dynamic.png
--rw-r--r--   0 runner    (1001) docker     (123)    34158 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/examples/output_data/plot_ion_spectra.png
--rw-r--r--   0 runner    (1001) docker     (123)    24165 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/examples/output_data/plot_static.png
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/examples/plot_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.937240 SimulatedLIBS-1.0.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)    22285 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/images/plot_dynamic.png
--rw-r--r--   0 runner    (1001) docker     (123)    34158 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/images/plot_ion_spectra.png
--rw-r--r--   0 runner    (1001) docker     (123)    24165 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/images/plot_static.png
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-25 19:56:12.937240 SimulatedLIBS-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:12.937240 SimulatedLIBS-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/tests/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/tests/test_SimulatedLIBS.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-25 19:56:01.000000 SimulatedLIBS-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.752655 SimulatedLIBS-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.728655 SimulatedLIBS-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.728655 SimulatedLIBS-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-17 18:41:46.752655 SimulatedLIBS-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.728655 SimulatedLIBS-1.0.3/SimulatedLIBS/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/animation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.728655 SimulatedLIBS-1.0.3/SimulatedLIBS/animations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.732655 SimulatedLIBS-1.0.3/SimulatedLIBS/animations/saved-gifs/
+-rw-r--r--   0 runner    (1001) docker     (123)   203642 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/animations/saved-gifs/animated_density.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   805303 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/animations/saved-gifs/animated_resolution.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   271781 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/animations/saved-gifs/animated_temperature.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.732655 SimulatedLIBS-1.0.3/SimulatedLIBS/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123) 11775488 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/drivers/chromedriver.exe
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/SimulatedLIBS/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.732655 SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-17 18:41:46.000000 SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-17 18:41:46.000000 SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:41:46.000000 SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 18:41:46.000000 SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 18:41:46.000000 SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.748655 SimulatedLIBS-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/docs/libs-dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3253118 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/docs/output.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    98115 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/docs/single-spectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   141185 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/docs/single_simulation.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.748655 SimulatedLIBS-1.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.748655 SimulatedLIBS-1.0.3/examples/output_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    22285 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/examples/output_data/plot_dynamic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34158 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/examples/output_data/plot_ion_spectra.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24165 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/examples/output_data/plot_static.png
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/examples/plot_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.752655 SimulatedLIBS-1.0.3/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    22285 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/images/plot_dynamic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34158 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/images/plot_ion_spectra.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24165 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/images/plot_static.png
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-17 18:41:46.752655 SimulatedLIBS-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:46.752655 SimulatedLIBS-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/tests/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/tests/test_SimulatedLIBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-17 18:41:34.000000 SimulatedLIBS-1.0.3/tox.ini
```

### Comparing `SimulatedLIBS-1.0.2/.github/workflows/python-publish.yml` & `SimulatedLIBS-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/.github/workflows/test.yml` & `SimulatedLIBS-1.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/.gitignore` & `SimulatedLIBS-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/LICENSE.md` & `SimulatedLIBS-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/PKG-INFO` & `SimulatedLIBS-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimulatedLIBS
-Version: 1.0.2
+Version: 1.0.3
 Summary: SimulatedLIBS provides simple Python class to simulate LIBS spectra with NIST LIBS Database interface
 Home-page: https://github.com/MKastek/SimulatedLIBS
 Author: Marcin Kastek
 Author-email: marcin.kastek@ifpilm.pl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SimulatedLIBS-1.0.2/README.md` & `SimulatedLIBS-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS/animation.py` & `SimulatedLIBS-1.0.3/SimulatedLIBS/animation.py`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS/animations/saved-gifs/animated_density.gif` & `SimulatedLIBS-1.0.3/SimulatedLIBS/animations/saved-gifs/animated_density.gif`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS/animations/saved-gifs/animated_resolution.gif` & `SimulatedLIBS-1.0.3/SimulatedLIBS/animations/saved-gifs/animated_resolution.gif`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS/animations/saved-gifs/animated_temperature.gif` & `SimulatedLIBS-1.0.3/SimulatedLIBS/animations/saved-gifs/animated_temperature.gif`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS/drivers/chromedriver.exe` & `SimulatedLIBS-1.0.3/SimulatedLIBS/drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS/simulation.py` & `SimulatedLIBS-1.0.3/SimulatedLIBS/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
         output_df = pd.DataFrame(columns=columns)
 
         for spectra in spectra_pool:
             intensity = spectra.result()["spectrum"]["intensity"].values.tolist()
 
             percentages = spectra.result()["composition"]["percentages"].values.tolist()
             intensity.extend(percentages)
-            intensity.extend(spectra.result()["name"])
+            intensity.append(spectra.result()["name"])
             intensity.append(spectra.result()["Te[eV]"])
             intensity.append(spectra.result()["Ne[cm^-3]".format(Ne_min=Ne_min)])
             output_df = pd.concat(
                 [output_df, pd.DataFrame(data=[intensity], columns=columns)],
                 ignore_index=True,
             )
```

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/PKG-INFO` & `SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimulatedLIBS
-Version: 1.0.2
+Version: 1.0.3
 Summary: SimulatedLIBS provides simple Python class to simulate LIBS spectra with NIST LIBS Database interface
 Home-page: https://github.com/MKastek/SimulatedLIBS
 Author: Marcin Kastek
 Author-email: marcin.kastek@ifpilm.pl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SimulatedLIBS-1.0.2/SimulatedLIBS.egg-info/SOURCES.txt` & `SimulatedLIBS-1.0.3/SimulatedLIBS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/docs/libs-dataset.ipynb` & `SimulatedLIBS-1.0.3/docs/libs-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/docs/output.csv` & `SimulatedLIBS-1.0.3/docs/output.csv`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/docs/single-spectra.ipynb` & `SimulatedLIBS-1.0.3/docs/single-spectra.ipynb`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/docs/single_simulation.csv` & `SimulatedLIBS-1.0.3/docs/single_simulation.csv`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/examples/output_data/plot_dynamic.png` & `SimulatedLIBS-1.0.3/examples/output_data/plot_dynamic.png`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/examples/output_data/plot_ion_spectra.png` & `SimulatedLIBS-1.0.3/examples/output_data/plot_ion_spectra.png`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/examples/output_data/plot_static.png` & `SimulatedLIBS-1.0.3/examples/output_data/plot_static.png`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/examples/plot_example.py` & `SimulatedLIBS-1.0.3/examples/plot_example.py`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/images/plot_dynamic.png` & `SimulatedLIBS-1.0.3/images/plot_dynamic.png`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/images/plot_ion_spectra.png` & `SimulatedLIBS-1.0.3/images/plot_ion_spectra.png`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/images/plot_static.png` & `SimulatedLIBS-1.0.3/images/plot_static.png`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/pyproject.toml` & `SimulatedLIBS-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/setup.cfg` & `SimulatedLIBS-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `SimulatedLIBS-1.0.2/tests/test_SimulatedLIBS.py` & `SimulatedLIBS-1.0.3/tests/test_SimulatedLIBS.py`

 * *Files identical despite different names*

