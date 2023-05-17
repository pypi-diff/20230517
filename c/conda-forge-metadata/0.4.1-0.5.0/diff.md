# Comparing `tmp/conda-forge-metadata-0.4.1.tar.gz` & `tmp/conda-forge-metadata-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-forge-metadata-0.4.1.tar", last modified: Fri Apr 21 21:32:13 2023, max compression
+gzip compressed data, was "conda-forge-metadata-0.5.0.tar", last modified: Wed May 17 18:41:28 2023, max compression
```

## Comparing `conda-forge-metadata-0.4.1.tar` & `conda-forge-metadata-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.247955 conda-forge-metadata-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.251955 conda-forge-metadata-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.251955 conda-forge-metadata-0.4.1/conda_forge_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/info_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/import_to_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/feedstock_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/libcfgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/oci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_feedstock_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_info_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_libcfgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_map_import_to_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_map_pypi_to_conda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.760373 conda-forge-metadata-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.768374 conda-forge-metadata-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.768374 conda-forge-metadata-0.5.0/conda_forge_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/info_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/import_to_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/pypi_to_conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/oci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.768374 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_info_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_map_import_to_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_map_pypi_to_conda.py
```

### Comparing `conda-forge-metadata-0.4.1/.github/workflows/pypi.yml` & `conda-forge-metadata-0.5.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/.github/workflows/tests.yml` & `conda-forge-metadata-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/.gitignore` & `conda-forge-metadata-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/.pre-commit-config.yaml` & `conda-forge-metadata-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/LICENSE` & `conda-forge-metadata-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/PKG-INFO` & `conda-forge-metadata-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.4.1
+Version: 0.5.0
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/info_json.py` & `conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/info_json.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/import_to_pkg.py` & `conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/import_to_pkg.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py` & `conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/pypi_to_conda.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "master/mappings/pypi/name_mapping.yaml"
     )
     req.raise_for_status()
     return yaml.YAML(typ="safe").load(req.text)
 
 
 @lru_cache(maxsize=1)
-def _grayskull_pypi_mapping():
+def get_grayskull_pypi_mapping():
     req = requests.get(
         "https://raw.githubusercontent.com/regro/cf-graph-countyfair/"
         "master/mappings/pypi/grayskull_pypi_mapping.json"
     )
     req.raise_for_status()
     return req.json()
 
@@ -33,9 +33,9 @@
         The name on PyPi. This is case-sensitive.
 
     Returns
     -------
     conda_name : str
         The most likely Conda name.
     """
-    pypi_map = _grayskull_pypi_mapping()
+    pypi_map = get_grayskull_pypi_mapping()
     return pypi_map.get(pypi_name, {}).get("conda_name", pypi_name.lower())
```

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata/feedstock_outputs.py` & `conda-forge-metadata-0.5.0/conda_forge_metadata/feedstock_outputs.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata/libcfgraph.py` & `conda-forge-metadata-0.5.0/conda_forge_metadata/libcfgraph.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata/oci.py` & `conda-forge-metadata-0.5.0/conda_forge_metadata/oci.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/PKG-INFO` & `conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.4.1
+Version: 0.5.0
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/SOURCES.txt` & `conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/pyproject.toml` & `conda-forge-metadata-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/tests/test_info_json.py` & `conda-forge-metadata-0.5.0/tests/test_info_json.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.4.1/tests/test_libcfgraph.py` & `conda-forge-metadata-0.5.0/tests/test_libcfgraph.py`

 * *Files identical despite different names*

