# Comparing `tmp/pycatsearch-5.1.0.tar.gz` & `tmp/pycatsearch-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.0.tar", last modified: Wed May 17 08:40:03 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.1.tar", last modified: Wed May 17 09:29:51 2023, max compression
```

## Comparing `pycatsearch-5.1.0.tar` & `pycatsearch-5.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:40:03.910597 pycatsearch-5.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:40:03.902597 pycatsearch-5.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:40:03.906597 pycatsearch-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-05-17 08:40:03.910597 pycatsearch-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 08:40:03.910597 pycatsearch-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:40:03.902597 pycatsearch-5.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:40:03.906597 pycatsearch-5.1.0/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 08:40:03.000000 pycatsearch-5.1.0/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:40:03.910597 pycatsearch-5.1.0/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:40:03.906597 pycatsearch-5.1.0/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-05-17 08:40:03.000000 pycatsearch-5.1.0/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 08:40:03.000000 pycatsearch-5.1.0/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:40:03.000000 pycatsearch-5.1.0/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 08:40:03.000000 pycatsearch-5.1.0/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 08:40:03.000000 pycatsearch-5.1.0/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 08:40:03.000000 pycatsearch-5.1.0/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-17 08:39:51.000000 pycatsearch-5.1.0/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.830012 pycatsearch-5.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.834012 pycatsearch-5.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.830012 pycatsearch-5.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.834012 pycatsearch-5.1.1/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.834012 pycatsearch-5.1.1/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/updater.py
```

### Comparing `pycatsearch-5.1.0/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/LICENSE.md` & `pycatsearch-5.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/PKG-INFO` & `pycatsearch-5.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.0
+Version: 5.1.1
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -27,29 +27,29 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# pycatsearch
+# PyCatSearch
 
 Yet another implementation of [JPL](https://spec.jpl.nasa.gov/) and [CDMS](https://astro.uni-koeln.de/)
 spectroscopy catalogs offline search.
 
 It consists of three parts:
 
 ### `catalog`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-python3 catalog.py --min-frequency 118749 --max-frequency 118751 catalog_115-178.json.gz -n oxygen
+pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch.catalog import Catalog
@@ -120,15 +120,15 @@
 ### `downloader`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-python3 downloader.py --min-frequency 115000 --max-frequency 178000 catalog_115-178.json.gz
+pycatsearch-downloader --min-frequency 115000 --max-frequency 178000 catalog.json.gz
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch import downloader
@@ -159,14 +159,31 @@
 
 This is just like `downloader`, but much, much faster.
 The download speed is limited by the remote servers.
 Most of the time, it takes no more than 90 seconds to load all the data.
 
 Requires `aiohttp`.
 
+###### Sample usage:
+
+In a command line:
+
+```commandline
+pycatsearch-async-downloader --min-frequency 115000 --max-frequency 178000 catalog.json.gz
+```
+
+In a code:
+
+```python
+# coding=utf-8
+from pycatsearch import async_downloader
+
+async_downloader.save_catalog('catalog.json.gz', (115000, 178000))
+```
+
 ###### Functions:
 
 - `get_catalog(frequency_limits: Tuple[float, float] = (0.0, math.inf)) ->
   List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
 - `save_catalog(filename: str, frequency_limits: Tuple[float, float] = (0.0, math.inf)) -> bool`
 
 The functions behave _almost_ exactly like their namesakes from `downloader`.
@@ -191,15 +208,15 @@
 and contains spectral lines within the specified frequency range.
 The second one is the number of species yet to be downloaded and processed.
 The numbers are the same as what `get_catalog` function types.
 
 ### `gui`
 
 This is the graphical interface built with Python bindings for Qt (`PyQt5`, `PySide6`, `PyQt6`, or `PySide2`).
-Just run `main.py` and see for yourself.
+Just run `pycatsearch` and see for yourself.
 
 ### Requirements
 
 The code is developed under `python 3.11`. It should work under `python 3.8` but merely tested.
 
 The non-GUI parts require absolute minimum of non-standard modules.
 If you want to download the catalog data faster, consider `async_downloader` module;
```

### Comparing `pycatsearch-5.1.0/README.md` & `pycatsearch-5.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# pycatsearch
+# PyCatSearch
 
 Yet another implementation of [JPL](https://spec.jpl.nasa.gov/) and [CDMS](https://astro.uni-koeln.de/)
 spectroscopy catalogs offline search.
 
 It consists of three parts:
 
 ### `catalog`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-python3 catalog.py --min-frequency 118749 --max-frequency 118751 catalog_115-178.json.gz -n oxygen
+pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch.catalog import Catalog
@@ -87,15 +87,15 @@
 ### `downloader`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-python3 downloader.py --min-frequency 115000 --max-frequency 178000 catalog_115-178.json.gz
+pycatsearch-downloader --min-frequency 115000 --max-frequency 178000 catalog.json.gz
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch import downloader
@@ -126,14 +126,31 @@
 
 This is just like `downloader`, but much, much faster.
 The download speed is limited by the remote servers.
 Most of the time, it takes no more than 90 seconds to load all the data.
 
 Requires `aiohttp`.
 
+###### Sample usage:
+
+In a command line:
+
+```commandline
+pycatsearch-async-downloader --min-frequency 115000 --max-frequency 178000 catalog.json.gz
+```
+
+In a code:
+
+```python
+# coding=utf-8
+from pycatsearch import async_downloader
+
+async_downloader.save_catalog('catalog.json.gz', (115000, 178000))
+```
+
 ###### Functions:
 
 - `get_catalog(frequency_limits: Tuple[float, float] = (0.0, math.inf)) ->
   List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
 - `save_catalog(filename: str, frequency_limits: Tuple[float, float] = (0.0, math.inf)) -> bool`
 
 The functions behave _almost_ exactly like their namesakes from `downloader`.
@@ -158,15 +175,15 @@
 and contains spectral lines within the specified frequency range.
 The second one is the number of species yet to be downloaded and processed.
 The numbers are the same as what `get_catalog` function types.
 
 ### `gui`
 
 This is the graphical interface built with Python bindings for Qt (`PyQt5`, `PySide6`, `PyQt6`, or `PySide2`).
-Just run `main.py` and see for yourself.
+Just run `pycatsearch` and see for yourself.
 
 ### Requirements
 
 The code is developed under `python 3.11`. It should work under `python 3.8` but merely tested.
 
 The non-GUI parts require absolute minimum of non-standard modules.
 If you want to download the catalog data faster, consider `async_downloader` module;
```

### Comparing `pycatsearch-5.1.0/main.py` & `pycatsearch-5.1.1/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/pyproject.toml` & `pycatsearch-5.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 dynamic = [
     'version',
     'dependencies',
 ]
 
 [project.gui-scripts]
 pycatsearch = 'pycatsearch:main'
+pycatsearch-downloader = 'pycatsearch:download'
+pycatsearch-async-downloader = 'pycatsearch:async_download'
 
 [project.urls]
 'Source Code' = 'https://github.com/StSav012/pycatsearch'
 'Bug Tracker' = 'https://github.com/StSav012/pycatsearch/issues'
 
 [tool.setuptools_scm]
 local_scheme = 'no-local-version'
```

### Comparing `pycatsearch-5.1.0/setup.py` & `pycatsearch-5.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/__init__.py` & `pycatsearch-5.1.1/src/pycatsearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,7 +165,19 @@
             elif isinstance(ex, ImportError):
                 tkinter.messagebox.showerror(title='Package Missing', message=error_message)
             else:
                 tkinter.messagebox.showerror(title='Error', message=error_message)
             root.destroy()
     else:
         gui.run()
+
+
+def download() -> None:
+    from . import downloader
+
+    downloader.download()
+
+
+def async_download() -> None:
+    from . import async_downloader
+
+    async_downloader.download()
```

### Comparing `pycatsearch-5.1.0/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.1/src/pycatsearch/async_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import asyncio
-import gzip
 import json
 import logging
 import random
 from contextlib import suppress
 from math import inf
 from queue import Empty, Queue
 from threading import Thread
-from typing import Any, BinaryIO, Final, Mapping, cast
+from typing import Any, Final, Mapping, cast
 from urllib.error import HTTPError
 from urllib.parse import urlencode
 
 import aiohttp
 import aiohttp.client_exceptions
 
 from .catalog_entry import CatalogEntry
 from .utils import *
 
-__all__ = ['Downloader', 'get_catalog', 'save_catalog']
+__all__ = ['Downloader', 'get_catalog', 'save_catalog', 'download']
 
 logger: logging.Logger = logging.getLogger('async_downloader')
 
 
 class Downloader(Thread):
     def __init__(self,
                  frequency_limits: tuple[float, float] = (-inf, inf),
@@ -207,15 +206,15 @@
     """
 
     return save_catalog_to_file(filename=filename,
                                 catalog=get_catalog(frequency_limits),
                                 frequency_limits=frequency_limits)
 
 
-if __name__ == '__main__':
+def download() -> None:
     import argparse
     from datetime import datetime
 
     ap: argparse.ArgumentParser = argparse.ArgumentParser(
         allow_abbrev=True,
         description='Download JPL and CDMS spectroscopy catalogs for offline search.\n'
                     'Find more at https://github.com/StSav012/pycatsearch.')
@@ -224,7 +223,11 @@
     ap.add_argument('-f''max', '--max-frequency', type=float, help='the upper frequency [MHz] to take', default=+inf)
     args: argparse.Namespace = ap.parse_intermixed_args()
 
     logging.basicConfig(level=logging.DEBUG)
     logger.info(f'started at {datetime.now()}')
     save_catalog(args.catalog, (args.min_frequency, args.max_frequency))
     logger.info(f'finished at {datetime.now()}')
+
+
+if __name__ == '__main__':
+    download()
```

### Comparing `pycatsearch-5.1.0/src/pycatsearch/catalog.py` & `pycatsearch-5.1.1/src/pycatsearch/catalog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.1/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/downloader.py` & `pycatsearch-5.1.1/src/pycatsearch/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Any, Final, Mapping, cast
 from urllib.error import HTTPError
 from urllib.parse import ParseResult, urlencode, urlparse
 
 from .catalog_entry import CatalogEntry
 from .utils import *
 
-__all__ = ['Downloader', 'get_catalog', 'save_catalog']
+__all__ = ['Downloader', 'get_catalog', 'save_catalog', 'download']
 
 logger: logging.Logger = logging.getLogger('downloader')
 
 
 class Downloader(Thread):
     def __init__(self,
                  frequency_limits: tuple[float, float] = (-inf, inf),
@@ -216,15 +216,15 @@
     """
 
     return save_catalog_to_file(filename=filename,
                                 catalog=get_catalog(frequency_limits),
                                 frequency_limits=frequency_limits)
 
 
-if __name__ == '__main__':
+def download() -> None:
     import argparse
     from datetime import datetime
 
     ap: argparse.ArgumentParser = argparse.ArgumentParser(
         allow_abbrev=True,
         description='Download JPL and CDMS spectroscopy catalogs for offline search.\n'
                     'Find more at https://github.com/StSav012/pycatsearch.')
@@ -233,7 +233,11 @@
     ap.add_argument('-f''max', '--max-frequency', type=float, help='the upper frequency [MHz] to take', default=+inf)
     args: argparse.Namespace = ap.parse_intermixed_args()
 
     logging.basicConfig(level=logging.DEBUG)
     logger.info(f'started at {datetime.now()}')
     save_catalog(args.catalog, (args.min_frequency, args.max_frequency))
     logger.info(f'finished at {datetime.now()}')
+
+
+if __name__ == '__main__':
+    download()
```

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/download_dialog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/frequency_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/settings.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/substances_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/ui.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.1/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch/utils.py` & `pycatsearch-5.1.1/src/pycatsearch/utils.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.1/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.0
+Version: 5.1.1
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -27,29 +27,29 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# pycatsearch
+# PyCatSearch
 
 Yet another implementation of [JPL](https://spec.jpl.nasa.gov/) and [CDMS](https://astro.uni-koeln.de/)
 spectroscopy catalogs offline search.
 
 It consists of three parts:
 
 ### `catalog`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-python3 catalog.py --min-frequency 118749 --max-frequency 118751 catalog_115-178.json.gz -n oxygen
+pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch.catalog import Catalog
@@ -120,15 +120,15 @@
 ### `downloader`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-python3 downloader.py --min-frequency 115000 --max-frequency 178000 catalog_115-178.json.gz
+pycatsearch-downloader --min-frequency 115000 --max-frequency 178000 catalog.json.gz
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch import downloader
@@ -159,14 +159,31 @@
 
 This is just like `downloader`, but much, much faster.
 The download speed is limited by the remote servers.
 Most of the time, it takes no more than 90 seconds to load all the data.
 
 Requires `aiohttp`.
 
+###### Sample usage:
+
+In a command line:
+
+```commandline
+pycatsearch-async-downloader --min-frequency 115000 --max-frequency 178000 catalog.json.gz
+```
+
+In a code:
+
+```python
+# coding=utf-8
+from pycatsearch import async_downloader
+
+async_downloader.save_catalog('catalog.json.gz', (115000, 178000))
+```
+
 ###### Functions:
 
 - `get_catalog(frequency_limits: Tuple[float, float] = (0.0, math.inf)) ->
   List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
 - `save_catalog(filename: str, frequency_limits: Tuple[float, float] = (0.0, math.inf)) -> bool`
 
 The functions behave _almost_ exactly like their namesakes from `downloader`.
@@ -191,15 +208,15 @@
 and contains spectral lines within the specified frequency range.
 The second one is the number of species yet to be downloaded and processed.
 The numbers are the same as what `get_catalog` function types.
 
 ### `gui`
 
 This is the graphical interface built with Python bindings for Qt (`PyQt5`, `PySide6`, `PyQt6`, or `PySide2`).
-Just run `main.py` and see for yourself.
+Just run `pycatsearch` and see for yourself.
 
 ### Requirements
 
 The code is developed under `python 3.11`. It should work under `python 3.8` but merely tested.
 
 The non-GUI parts require absolute minimum of non-standard modules.
 If you want to download the catalog data faster, consider `async_downloader` module;
```

### Comparing `pycatsearch-5.1.0/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.1/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.0/updater.py` & `pycatsearch-5.1.1/updater.py`

 * *Files identical despite different names*

