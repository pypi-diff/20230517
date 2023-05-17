# Comparing `tmp/omero-cli-zarr-0.5.1.tar.gz` & `tmp/omero-cli-zarr-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-cli-zarr-0.5.1.tar", last modified: Thu Nov  3 15:25:35 2022, max compression
+gzip compressed data, was "omero-cli-zarr-0.5.2.tar", last modified: Wed May 17 21:08:21 2023, max compression
```

## Comparing `omero-cli-zarr-0.5.1.tar` & `omero-cli-zarr-0.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.461317 omero-cli-zarr-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.457316 omero-cli-zarr-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.461317 omero-cli-zarr-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/.github/workflows/precommit.yml
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    17987 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4691 2022-11-03 15:25:35.461317 omero-cli-zarr-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 15:25:35.461317 omero-cli-zarr-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.457316 omero-cli-zarr-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.457316 omero-cli-zarr-0.5.1/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.461317 omero-cli-zarr-0.5.1/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/src/omero/plugins/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.461317 omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4691 2022-11-03 15:25:35.000000 omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-11-03 15:25:35.000000 omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 15:25:35.000000 omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-03 15:25:35.000000 omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-03 15:25:35.000000 omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 15:25:35.461317 omero-cli-zarr-0.5.1/src/omero_zarr/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/src/omero_zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-03 15:25:35.000000 omero-cli-zarr-0.5.1/src/omero_zarr/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    13312 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/src/omero_zarr/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    19047 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/src/omero_zarr/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    10947 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/src/omero_zarr/raw_pixels.py
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-11-03 15:25:20.000000 omero-cli-zarr-0.5.1/src/omero_zarr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.591786 omero-cli-zarr-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.github/workflows/precommit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.591786 omero-cli-zarr-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.591786 omero-cli-zarr-0.5.2/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero/plugins/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:08:21.595786 omero-cli-zarr-0.5.2/src/omero_zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 21:08:21.000000 omero-cli-zarr-0.5.2/src/omero_zarr/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/raw_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-17 21:08:17.000000 omero-cli-zarr-0.5.2/src/omero_zarr/util.py
```

### Comparing `omero-cli-zarr-0.5.1/.github/workflows/publish_pypi.yml` & `omero-cli-zarr-0.5.2/.github/workflows/publish_pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 on: push
 
 jobs:
   build-n-publish:
     name: Publish to PyPI
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
       - name: Build a binary wheel and a source tarball
         run: |
           python -mpip install wheel
           python setup.py sdist bdist_wheel
       - name: Publish distribution to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@v1.3.0
```

### Comparing `omero-cli-zarr-0.5.1/.pre-commit-config.yaml` & `omero-cli-zarr-0.5.2/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 
   - repo: https://github.com/asottile/seed-isort-config
     rev: v2.2.0
     hooks:
       - id: seed-isort-config
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         args: ["--profile", "black"]
 
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: [--target-version=py36]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.1.0
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args:
           - --py36-plus
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
         exclude: .bumpversion.cfg
       - id: end-of-file-fixer
       - id: check-json
         files: \.(json)$
       - id: check-yaml
@@ -41,15 +41,15 @@
       - id: check-merge-conflict
       - id: check-symlinks
       - id: pretty-format-json
         args:
           - --autofix
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [
           flake8-blind-except,
           flake8-builtins,
           flake8-rst-docstrings,
           flake8-logging-format,
@@ -59,29 +59,29 @@
           "--max-line-length=88",
           # Conflicts with black: E203 whitespace before ':'
           "--ignore=E203",
           "--rst-roles=class,func,ref,module,const",
         ]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.982
+    rev: v1.3.0
     hooks:
       - id: mypy
       # This is for checking tests/* (everything else has a stricter check
       # below), but since there's no include it's run on everything
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.982
+    rev: v1.3.0
     hooks:
       - id: mypy
         args: [
           --disallow-untyped-defs,
           --ignore-missing-imports,
         ]
         exclude: tests/
 
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.28.0
+    rev: v1.31.0
     hooks:
       - id: yamllint
         # args: [--config-data=relaxed]
         #
```

### Comparing `omero-cli-zarr-0.5.1/LICENSE.txt` & `omero-cli-zarr-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.1/PKG-INFO` & `omero-cli-zarr-0.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: omero-cli-zarr
-Version: 0.5.1
+Version: 0.5.2
 Summary: Plugin for exporting images in zarr format.
 Home-page: https://github.com/ome/omero-cli-zarr/
 Author: The Open Microscopy Team
 Author-email: 
+License: UNKNOWN
 Keywords: OMERO.CLI,plugin
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Natural Language :: English
@@ -63,19 +65,21 @@
 
     # Plate will be saved in current directory as 2.zarr
     $ omero zarr export Plate:2
 
     # Specify an output directory
     $ omero zarr --output /home/user/zarr_files export Image:1
 
-    # Cache each plane as a numpy file.npy. If connection is lost, and you need
-    # to export again, we can use these instead of downloading again
-    # omero zarr --cache_numpy export Image:1
+    # By default, a tile size of 1024 is used. Specify values with
+    $ omero zarr export Image:1 --tile_width 256 --tile_height 256
 
 
+NB: If the connection to OMERO is lost and the Image is partially exported,
+re-running the command will attempt to complete the export.
+
 To export images via bioformats2raw we use the ```--bf``` flag::
 
     export MANAGED_REPO=/var/omero/data/ManagedRepository
     export BF2RAW=/opt/tools/bioformats2raw-0.2.0-SNAPSHOT
 
     $ omero zarr --output /home/user/zarr_files export 1 --bf
     Image exported to /home/user/zarr_files/2chZT.lsm
@@ -126,7 +130,20 @@
     41,Chromosomes,1369133
     42,Chromosomes,1369135
     ...
 
 This will create zarr groups of `Cell` and `Chromosomes` under `5514375.zarr/labels/`::
 
     $ omero zarr masks Image:5514375 --label-map=5514375.rois
+
+License
+-------
+
+This project, similar to many Open Microscopy Environment (OME) projects, is
+licensed under the terms of the GNU General Public License (GPL) v2 or later.
+
+Copyright
+---------
+
+2020-2023, The Open Microscopy Environment
+
+
```

### Comparing `omero-cli-zarr-0.5.1/README.rst` & `omero-cli-zarr-0.5.2/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -42,19 +42,21 @@
 
     # Plate will be saved in current directory as 2.zarr
     $ omero zarr export Plate:2
 
     # Specify an output directory
     $ omero zarr --output /home/user/zarr_files export Image:1
 
-    # Cache each plane as a numpy file.npy. If connection is lost, and you need
-    # to export again, we can use these instead of downloading again
-    # omero zarr --cache_numpy export Image:1
+    # By default, a tile size of 1024 is used. Specify values with
+    $ omero zarr export Image:1 --tile_width 256 --tile_height 256
 
 
+NB: If the connection to OMERO is lost and the Image is partially exported,
+re-running the command will attempt to complete the export.
+
 To export images via bioformats2raw we use the ```--bf``` flag::
 
     export MANAGED_REPO=/var/omero/data/ManagedRepository
     export BF2RAW=/opt/tools/bioformats2raw-0.2.0-SNAPSHOT
 
     $ omero zarr --output /home/user/zarr_files export 1 --bf
     Image exported to /home/user/zarr_files/2chZT.lsm
@@ -105,7 +107,18 @@
     41,Chromosomes,1369133
     42,Chromosomes,1369135
     ...
 
 This will create zarr groups of `Cell` and `Chromosomes` under `5514375.zarr/labels/`::
 
     $ omero zarr masks Image:5514375 --label-map=5514375.rois
+
+License
+-------
+
+This project, similar to many Open Microscopy Environment (OME) projects, is
+licensed under the terms of the GNU General Public License (GPL) v2 or later.
+
+Copyright
+---------
+
+2020-2023, The Open Microscopy Environment
```

### Comparing `omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/PKG-INFO` & `omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: omero-cli-zarr
-Version: 0.5.1
+Version: 0.5.2
 Summary: Plugin for exporting images in zarr format.
 Home-page: https://github.com/ome/omero-cli-zarr/
 Author: The Open Microscopy Team
 Author-email: 
+License: UNKNOWN
 Keywords: OMERO.CLI,plugin
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Natural Language :: English
@@ -63,19 +65,21 @@
 
     # Plate will be saved in current directory as 2.zarr
     $ omero zarr export Plate:2
 
     # Specify an output directory
     $ omero zarr --output /home/user/zarr_files export Image:1
 
-    # Cache each plane as a numpy file.npy. If connection is lost, and you need
-    # to export again, we can use these instead of downloading again
-    # omero zarr --cache_numpy export Image:1
+    # By default, a tile size of 1024 is used. Specify values with
+    $ omero zarr export Image:1 --tile_width 256 --tile_height 256
 
 
+NB: If the connection to OMERO is lost and the Image is partially exported,
+re-running the command will attempt to complete the export.
+
 To export images via bioformats2raw we use the ```--bf``` flag::
 
     export MANAGED_REPO=/var/omero/data/ManagedRepository
     export BF2RAW=/opt/tools/bioformats2raw-0.2.0-SNAPSHOT
 
     $ omero zarr --output /home/user/zarr_files export 1 --bf
     Image exported to /home/user/zarr_files/2chZT.lsm
@@ -126,7 +130,20 @@
     41,Chromosomes,1369133
     42,Chromosomes,1369135
     ...
 
 This will create zarr groups of `Cell` and `Chromosomes` under `5514375.zarr/labels/`::
 
     $ omero zarr masks Image:5514375 --label-map=5514375.rois
+
+License
+-------
+
+This project, similar to many Open Microscopy Environment (OME) projects, is
+licensed under the terms of the GNU General Public License (GPL) v2 or later.
+
+Copyright
+---------
+
+2020-2023, The Open Microscopy Environment
+
+
```

### Comparing `omero-cli-zarr-0.5.1/src/omero_cli_zarr.egg-info/SOURCES.txt` & `omero-cli-zarr-0.5.2/src/omero_cli_zarr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-cli-zarr-0.5.1/src/omero_zarr/cli.py` & `omero-cli-zarr-0.5.2/src/omero_zarr/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+#!/usr/bin/env python
+
+# Copyright (C) 2023 University of Dundee & Open Microscopy Environment.
+# All rights reserved.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import argparse
 import subprocess
 import sys
 from functools import wraps
 from pathlib import Path
 from typing import Any, Callable, List
 
@@ -64,15 +82,15 @@
 
   --max_workers
 
      Maximum number of workers to use for parallel generation of pyramids
 
   --tile_width / --tile_height
 
-     Maximum tile width or height to read (only for use with bioformats2raw)
+     Maximum tile width or height to read
 
   --resolutions
 
      Number of pyramid resolutions to generate
 
 """
 
@@ -111,31 +129,24 @@
                 self.gateway = None
                 self.client = None  # type: ignore
 
     return _wrapper
 
 
 class ZarrControl(BaseControl):
-
     gateway = None
     client = None
 
     def _configure(self, parser: Parser) -> None:
         parser.add_login_arguments()
 
         parser.add_argument(
             "--output", type=str, default="", help="The output directory"
         )
 
-        parser.add_argument(
-            "--cache_numpy",
-            action="store_true",
-            help="Save planes as .npy files in case of connection loss",
-        )
-
         # Subcommands
         sub = parser.sub()
         polygons = parser.add(sub, self.polygons, POLYGONS_HELP)
         polygons.add_argument(
             "object",
             type=ProxyStringType("Image"),
             help="The Image from which to export Polygons.",
@@ -245,20 +256,20 @@
             "--bfpath",
             help="Use bioformats2raw on a local copy of a file. Requires"
             " bioformats2raw 0.4.0 or higher.",
         )
         export.add_argument(
             "--tile_width",
             default=None,
-            help="Maximum tile width to read (only for use with bioformats2raw)",
+            help="Maximum tile width",
         )
         export.add_argument(
             "--tile_height",
             default=None,
-            help="Maximum tile height to read (only for use with bioformats2raw)",
+            help="Maximum tile height",
         )
         export.add_argument(
             "--resolutions",
             default=None,
             help="Number of pyramid resolutions to generate"
             " (only for use with bioformats2raw)",
         )
```

### Comparing `omero-cli-zarr-0.5.1/src/omero_zarr/masks.py` & `omero-cli-zarr-0.5.2/src/omero_zarr/masks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+#!/usr/bin/env python
+
+# Copyright (C) 2023 University of Dundee & Open Microscopy Environment.
+# All rights reserved.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import argparse
 import logging
 import re
 import time
 from collections import defaultdict
 from fileinput import input
 from typing import Dict, List, Optional, Set, Tuple
@@ -29,15 +47,15 @@
     "C": 1,
     "Z": 2,
     "Y": 3,
     "X": 4,
 }
 
 MASK_DTYPE_SIZE: Dict[int, np.dtype] = {
-    1: np.bool,
+    1: bool,
     8: np.int8,
     16: np.int16,
     32: np.int32,
     64: np.int64,
 }
 
 OME_MODEL_POINT_LIST_RE = re.compile(r"([\d.]+),([\d.]+)")
@@ -95,15 +113,15 @@
                         saver.save(list(masks.values()), args.label_name)
                 print_status(int(t0), int(time.time()), count, total)
 
 
 def get_label_map(masks: Dict, label_map_arg: str) -> Dict:
     label_map = defaultdict(list)
     roi_map = {}
-    for (roi_id, roi) in masks.items():
+    for roi_id, roi in masks.items():
         roi_map[roi_id] = roi
 
     try:
         for line in input(label_map_arg):
             line = line.strip()
             sid, name, roi = line.split(",")
             label_map[name].append(roi_map[int(roi)])
@@ -111,15 +129,14 @@
         # KeyError: if a roi is missing from the roi_map
         # ValueError: if there aren't enough separators
         print(f"Error parsing {label_map_arg}: {e}")
     return label_map
 
 
 def get_shapes(image: omero.gateway.ImageWrapper, shape_types: List[str]) -> Dict:
-
     shape_classes = []
     for klass in shape_types:
         if klass in SHAPE_TYPES:
             shape_classes.append(SHAPE_TYPES[klass])
 
     conn = image._conn
     roi_service = conn.getRoiService()
@@ -166,15 +183,15 @@
             args.label_path,
             args.style,
             args.source_image,
             args.overlaps,
         )
 
         if args.style == "split":
-            for (roi_id, roi) in masks.items():
+            for roi_id, roi in masks.items():
                 saver.save([roi], str(roi_id))
         else:
             if args.label_map:
                 label_map = get_label_map(masks, args.label_map)
                 for name, values in label_map.items():
                     print(f"Label map: {name} (count: {len(values)})")
                     saver.save(values, name)
@@ -399,15 +416,14 @@
         binarray = np.reshape(binarray[: (w * h)], (h, w))
 
         return binarray, (t, c, z, y, x, h, w)
 
     def _polygon_to_binim_yx(
         self, polygon: omero.model.Shape
     ) -> Tuple[np.ndarray, Tuple[int, ...]]:
-
         t = unwrap(polygon.theT)
         c = unwrap(polygon.theC)
         z = unwrap(polygon.theZ)
 
         # "10,20, 50,150, 200,200, 250,75"
         points = unwrap(polygon.points).strip()
         coords = OME_MODEL_POINT_LIST_RE.findall(points)
@@ -443,16 +459,16 @@
             return [d_value]
         return range(d_size)
 
     def masks_to_labels(
         self,
         masks: List[omero.model.Mask],
         mask_shape: Tuple[int, ...],
-        ignored_dimensions: Set[str] = None,
-        check_overlaps: bool = None,
+        ignored_dimensions: Optional[Set[str]] = None,
+        check_overlaps: Optional[bool] = None,
     ) -> Tuple[np.ndarray, Dict[int, str], Dict[int, Dict]]:
         """
         :param masks [MaskI]: Iterable container of OMERO masks
         :param mask_shape 5-tuple: the image dimensions (T, C, Z, Y, X), taking
             into account `ignored_dimensions`
 
         :param ignored_dimensions set(char): Ignore these dimensions and set
@@ -530,15 +546,15 @@
                 for i_t in self._get_indices(ignored_dimensions, "T", t, size_t):
                     for i_c in self._get_indices(ignored_dimensions, "C", c, size_c):
                         for i_z in self._get_indices(
                             ignored_dimensions, "Z", z, size_z
                         ):
                             overlap = np.logical_and(
                                 labels[i_t, i_c, i_z, y : (y + h), x : (x + w)].astype(
-                                    np.bool
+                                    bool
                                 ),
                                 binim_yx,
                             )
                             # ADD to the array, so zeros in our binarray don't
                             # wipe out previous shapes
                             labels[i_t, i_c, i_z, y : (y + h), x : (x + w)] += (
                                 binim_yx * shape_value
```

