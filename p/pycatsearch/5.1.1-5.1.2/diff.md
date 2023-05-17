# Comparing `tmp/pycatsearch-5.1.1.tar.gz` & `tmp/pycatsearch-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.1.tar", last modified: Wed May 17 09:29:51 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.2.tar", last modified: Wed May 17 10:44:01 2023, max compression
```

## Comparing `pycatsearch-5.1.1.tar` & `pycatsearch-5.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.830012 pycatsearch-5.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.834012 pycatsearch-5.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.830012 pycatsearch-5.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.834012 pycatsearch-5.1.1/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.838013 pycatsearch-5.1.1/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:51.834012 pycatsearch-5.1.1/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 09:29:51.000000 pycatsearch-5.1.1/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-17 09:29:38.000000 pycatsearch-5.1.1/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.948428 pycatsearch-5.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.952427 pycatsearch-5.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.948428 pycatsearch-5.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.952427 pycatsearch-5.1.2/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.956427 pycatsearch-5.1.2/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/updater.py
```

### Comparing `pycatsearch-5.1.1/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/LICENSE.md` & `pycatsearch-5.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/PKG-INFO` & `pycatsearch-5.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.1
+Version: 5.1.2
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -41,15 +41,19 @@
 ### `catalog`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
+pycatsearch-cli --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
+```
+or
+```commandline
+python3 -m pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch.catalog import Catalog
```

### Comparing `pycatsearch-5.1.1/README.md` & `pycatsearch-5.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 ### `catalog`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
+pycatsearch-cli --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
+```
+or
+```commandline
+python3 -m pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch.catalog import Catalog
```

### Comparing `pycatsearch-5.1.1/main.py` & `pycatsearch-5.1.2/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/pyproject.toml` & `pycatsearch-5.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -35,19 +35,22 @@
     'Typing :: Typed',
 ]
 dynamic = [
     'version',
     'dependencies',
 ]
 
-[project.gui-scripts]
-pycatsearch = 'pycatsearch:main'
+[project.scripts]
+pycatsearch-cli = 'pycatsearch:main'
 pycatsearch-downloader = 'pycatsearch:download'
 pycatsearch-async-downloader = 'pycatsearch:async_download'
 
+[project.gui-scripts]
+pycatsearch = 'pycatsearch:main_gui'
+
 [project.urls]
 'Source Code' = 'https://github.com/StSav012/pycatsearch'
 'Bug Tracker' = 'https://github.com/StSav012/pycatsearch/issues'
 
 [tool.setuptools_scm]
 local_scheme = 'no-local-version'
 write_to = 'src/pycatsearch/_version.py'
```

### Comparing `pycatsearch-5.1.1/setup.py` & `pycatsearch-5.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/__init__.py` & `pycatsearch-5.1.2/src/pycatsearch/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,25 @@
                             'inchi', 'trivial_name', 'structural_formula', 'name', 'stoichiometric_formula',
                             'isotopolog', 'state', 'degrees_of_freedom', 'timeout']
     search_args: dict[str, str | float | int] = dict((arg, getattr(args, arg)) for arg in arg_names
                                                      if getattr(args, arg) is not None)
     if search_args:
         c: Catalog = Catalog(*args.catalog)
         c.print(**search_args)
-        exit(0)
+        return
+
+    main_gui()
+
+
+def main_gui() -> None:
+    ap: argparse.ArgumentParser = argparse.ArgumentParser(
+        description='Yet another implementation of JPL and CDMS spectroscopy catalogs offline search.\n'
+                    f'Find more at https://github.com/{__author__}/{__original_name__}.')
+    ap.add_argument('catalog', type=str, help='the catalog location to load',
+                    nargs=argparse.ZERO_OR_MORE)
 
     try:
         _make_old_qt_compatible_again()
 
         from . import gui
     except Exception as ex:
         import traceback
```

### Comparing `pycatsearch-5.1.1/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.2/src/pycatsearch/async_downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/catalog.py` & `pycatsearch-5.1.2/src/pycatsearch/catalog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.2/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/downloader.py` & `pycatsearch-5.1.2/src/pycatsearch/downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/download_dialog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/frequency_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/settings.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/substances_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/ui.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.2/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch/utils.py` & `pycatsearch-5.1.2/src/pycatsearch/utils.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.2/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.1
+Version: 5.1.2
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -41,15 +41,19 @@
 ### `catalog`
 
 ###### Sample usage:
 
 In a command line:
 
 ```commandline
-pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
+pycatsearch-cli --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
+```
+or
+```commandline
+python3 -m pycatsearch --min-frequency 118749 --max-frequency 118751 catalog.json.gz -n oxygen
 ```
 
 In a code:
 
 ```python
 # coding=utf-8
 from pycatsearch.catalog import Catalog
```

### Comparing `pycatsearch-5.1.1/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.2/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.1/updater.py` & `pycatsearch-5.1.2/updater.py`

 * *Files identical despite different names*

