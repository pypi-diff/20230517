# Comparing `tmp/superscreen-0.8.2.tar.gz` & `tmp/superscreen-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superscreen-0.8.2.tar", last modified: Sat May  6 18:47:15 2023, max compression
+gzip compressed data, was "superscreen-0.9.0.tar", last modified: Wed May 17 00:21:47 2023, max compression
```

## Comparing `superscreen-0.8.2.tar` & `superscreen-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-06 18:47:03.000000 superscreen-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-06 18:47:15.049204 superscreen-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-06 18:47:03.000000 superscreen-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 18:47:15.049204 superscreen-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-06 18:47:03.000000 superscreen-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.045204 superscreen-0.8.2/superscreen/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/superscreen/device/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26205 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    46147 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/fem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/fluxoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21535 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/superscreen/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/dipole.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/vortex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/superscreen/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38166 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.045204 superscreen-0.8.2/superscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.462604 superscreen-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 00:21:36.000000 superscreen-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 00:21:47.462604 superscreen-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-17 00:21:36.000000 superscreen-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:21:47.466604 superscreen-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-17 00:21:36.000000 superscreen-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.454604 superscreen-0.9.0/superscreen/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.458603 superscreen-0.9.0/superscreen/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42839 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/edge_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/fem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/fluxoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46337 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.458603 superscreen-0.9.0/superscreen/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19003 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/solve_film.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.458603 superscreen-0.9.0/superscreen/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/dipole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/vortex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.462604 superscreen-0.9.0/superscreen/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39839 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.454604 superscreen-0.9.0/superscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/top_level.txt
```

### Comparing `superscreen-0.8.2/LICENSE` & `superscreen-0.9.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2022 Logan Bishop-Van Horn
+Copyright (c) 2021-2023 Logan Bishop-Van Horn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `superscreen-0.8.2/PKG-INFO` & `superscreen-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.8.2
+Version: 0.9.0
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
@@ -15,24 +15,24 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: jax
 License-File: LICENSE
 
 
 # SuperScreen
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/loganbvh/superscreen/lint-and-test.yml?branch=main) [![Documentation Status](https://readthedocs.org/projects/superscreen/badge/?version=latest)](https://superscreen.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/gh/loganbvh/superscreen/branch/main/graph/badge.svg?token=XW7LSY8WVD)](https://codecov.io/gh/loganbvh/superscreen) ![GitHub](https://img.shields.io/github/license/loganbvh/superscreen) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/376110557.svg)](https://zenodo.org/badge/latestdoi/376110557)
 
@@ -44,13 +44,13 @@
 
 ## Learn `SuperScreen`
 
 The documentation for `SuperScreen` can be found at [superscreen.readthedocs.io](https://superscreen.readthedocs.io/en/latest/).
 
 ## Try `SuperScreen`
 
-Click the badge below and navigate to `docs/notebooks/` to try `SuperScreen` interactively online via [Binder](https://mybinder.org/):
+Click the badge below to try `SuperScreen` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/superscreen/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/superscreen/blob/main/docs/notebooks/quickstart.ipynb)
```

### Comparing `superscreen-0.8.2/README.md` & `superscreen-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 ## Learn `SuperScreen`
 
 The documentation for `SuperScreen` can be found at [superscreen.readthedocs.io](https://superscreen.readthedocs.io/en/latest/).
 
 ## Try `SuperScreen`
 
-Click the badge below and navigate to `docs/notebooks/` to try `SuperScreen` interactively online via [Binder](https://mybinder.org/):
+Click the badge below to try `SuperScreen` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/superscreen/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/superscreen/blob/main/docs/notebooks/quickstart.ipynb)
 
 ## Install `SuperScreen`
 
-`SuperScreen` requires `python >=3.7, <3.11`. We recommend installing `SuperScreen` in a fresh [`conda` environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). For more details, see the [documentation](https://superscreen.readthedocs.io/en/latest/).
+`SuperScreen` requires `python >=3.8, <3.12`. We recommend installing `SuperScreen` in a fresh [`conda` environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). For more details, see the [documentation](https://superscreen.readthedocs.io/en/latest/).
 
 ### Install via `pip`
 
 From [PyPI](https://pypi.org/project/superscreen/), the Python Package Index:
 
 ```bash
 pip install superscreen
```

### Comparing `superscreen-0.8.2/setup.py` & `superscreen-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,77 +11,76 @@
 
 ## Learn `SuperScreen`
 
 The documentation for `SuperScreen` can be found at [superscreen.readthedocs.io](https://superscreen.readthedocs.io/en/latest/).
 
 ## Try `SuperScreen`
 
-Click the badge below and navigate to `docs/notebooks/` to try `SuperScreen` interactively online via [Binder](https://mybinder.org/):
+Click the badge below to try `SuperScreen` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/superscreen/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/superscreen/blob/main/docs/notebooks/quickstart.ipynb)
 
 """
 
 from setuptools import find_packages, setup
 
 DESCRIPTION = "SuperScreen: simulate Meissner screening in 2D superconducting devices."
 LONG_DESCRIPTION = __doc__
 
 NAME = "superscreen"
 AUTHOR = "Logan Bishop-Van Horn"
 AUTHOR_EMAIL = "logan.bvh@gmail.com"
 URL = "https://github.com/loganbvh/superscreen"
 LICENSE = "MIT"
-PYTHON_VERSION = ">=3.7, <3.11"
+PYTHON_VERSION = ">=3.8, <3.12"
 
 INSTALL_REQUIRES = [
     "dill",
+    "h5py",
     "ipython",
     "joblib",
     "jupyter",
     "matplotlib",
     "meshpy",
+    "numba",
     "numpy",
-    "pandas",
     "pint",
-    "pre-commit",
     "pytest",
-    "pytest-cov",
-    "ray[default]",
     "scipy",
     "shapely",
+    "tqdm",
 ]
 
 EXTRAS_REQUIRE = {
+    "dev": [
+        "pytest-cov",
+        "pre-commit",
+    ],
     "docs": [
-        "IPython",
         "sphinx",
         "sphinx_rtd_theme",
         "sphinx-autodoc-typehints",
         "nbsphinx",
         "pillow",  # required for image scaling in RTD
     ],
-    "jax": [
-        "jax[cpu]",
-    ],
 }
 
 CLASSIFIERS = """\
 Development Status :: 4 - Beta
 Intended Audience :: Science/Research
 License :: OSI Approved :: MIT License
 Operating System :: MacOS
 Operating System :: POSIX
 Operating System :: Unix
 Operating System :: Microsoft :: Windows
 Programming Language :: Python
-Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Topic :: Scientific/Engineering
 Topic :: Scientific/Engineering :: Physics
 """
 
 CLASSIFIERS = [line for line in CLASSIFIERS.splitlines() if line]
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "superconductor meissner screening"
```

### Comparing `superscreen-0.8.2/superscreen/about.py` & `superscreen-0.9.0/superscreen/about.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,19 @@
 import sys
 import time
 from typing import Dict, Optional
 
 import IPython
 import joblib
 import matplotlib
+import numba
 import numpy
-import ray
 import scipy
 from IPython.display import HTML
 
-try:
-    import jax
-
-    jax_version = jax.__version__
-except (ModuleNotFoundError, ImportError, RuntimeError):
-    jax_version = None
-
 import superscreen
 
 
 def _blas_info() -> str:
     # https://github.com/qutip/qutip/blob/3ff3f42d2cd950c99af8936b12d9221ed79de5e3/
     # qutip/utilities.py#L335-L355
     config = numpy.__config__
@@ -53,18 +46,17 @@
 
 def version_dict() -> Dict[str, str]:
     """Returns a dictionary containing the versions of important dependencies."""
     cpu_count = [joblib.cpu_count(only_physical_cores=b) for b in (True, False)]
     return {
         "SuperScreen": superscreen.__version__,
         "Numpy": numpy.__version__,
+        "Numba": numba.__version__,
         "SciPy": scipy.__version__,
         "matplotlib": matplotlib.__version__,
-        "ray": ray.__version__,
-        "jax": str(jax_version),
         "IPython": IPython.__version__,
         "Python": sys.version,
         "OS": f"{os.name} [{sys.platform}]",
         "Number of CPUs": f"Physical: {cpu_count[0]}, Logical: {cpu_count[1]}",
         "BLAS Info": _blas_info(),
     }
```

### Comparing `superscreen-0.8.2/superscreen/device/components.py` & `superscreen-0.9.0/superscreen/device/polygon.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,154 +1,57 @@
 import logging
 from copy import deepcopy
 from typing import Iterable, Optional, Tuple, Union
 
+import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import path
 from scipy import interpolate
 from shapely import affinity
 from shapely import geometry as geo
 from shapely.validation import explain_validity
 
 from ..geometry import close_curve
-from ..parameter import Parameter
-from .mesh import generate_mesh, smooth_mesh
+from .mesh import Mesh
+from .utils import generate_mesh
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("device")
 
-
-class Layer:
-    """A single layer of a superconducting device.
-
-    You can provide either an effective penetration depth Lambda,
-    or both a London penetration depth (lambda_london) and a layer
-    thickness. Lambda and london_lambda can either be real numers or
-    Parameters which compute the penetration depth as a function of
-    position.
-
-    Args:
-        name: Name of the layer.
-        Lambda: The effective magnetic penetration depth of the superconducting
-            film(s) in the layer.
-        thickness: Thickness of the superconducting film(s) located in the layer.
-        london_lambda: London penetration depth of the superconducting film(s)
-            located in the layer.
-        z0: Vertical location of the layer.
-    """
-
-    __slots__ = ("name", "thickness", "london_lambda", "z0", "_Lambda")
-
-    def __init__(
-        self,
-        name: str,
-        Lambda: Optional[Union[float, Parameter]] = None,
-        london_lambda: Optional[Union[float, Parameter]] = None,
-        thickness: Optional[float] = None,
-        z0: float = 0,
-    ):
-        self.name = name
-        self.thickness = thickness
-        self.london_lambda = london_lambda
-        self.z0 = z0
-        if Lambda is None:
-            if london_lambda is None or thickness is None:
-                raise ValueError(
-                    "You must provide either an effective penetration depth Lambda "
-                    "or both a london_lambda and a thickness."
-                )
-            self._Lambda = None
-        else:
-            if london_lambda is not None or thickness is not None:
-                raise ValueError(
-                    "You must provide either an effective penetration depth Lambda "
-                    "or both a london_lambda and a thickness (but not all three)."
-                )
-            self._Lambda = Lambda
-
-    @property
-    def Lambda(self) -> Union[float, Parameter]:
-        """Effective penetration depth of the superconductor."""
-        if self._Lambda is not None:
-            return self._Lambda
-        return self.london_lambda**2 / self.thickness
-
-    @Lambda.setter
-    def Lambda(self, value: Union[float, Parameter]) -> None:
-        """Effective penetration depth of the superconductor."""
-        if self._Lambda is None:
-            raise AttributeError(
-                "Can't set Lambda directly. Set london_lambda and/or thickness instead."
-            )
-        self._Lambda = value
-
-    def __repr__(self) -> str:
-        Lambda = self.Lambda
-        if isinstance(Lambda, (int, float)):
-            Lambda = f"{Lambda:.3f}"
-        d = self.thickness
-        if isinstance(d, (int, float)):
-            d = f"{d:.3f}"
-        london = self.london_lambda
-        if isinstance(london, (int, float)):
-            london = f"{london:.3f}"
-        return (
-            f'{self.__class__.__name__}("{self.name}", Lambda={Lambda}, '
-            f"thickness={d}, london_lambda={london}, z0={self.z0:.3f})"
-        )
-
-    def __eq__(self, other) -> bool:
-        if other is self:
-            return True
-
-        if not isinstance(other, Layer):
-            return False
-
-        return (
-            self.name == other.name
-            and self.thickness == other.thickness
-            and self.london_lambda == other.london_lambda
-            and self.Lambda == other.Lambda
-            and self.z0 == other.z0
-        )
-
-    def copy(self):
-        return deepcopy(self)
+PolygonType = Union[
+    "Polygon",
+    np.ndarray,
+    geo.linestring.LineString,
+    geo.polygon.LinearRing,
+    geo.polygon.Polygon,
+]
 
 
 class Polygon:
-    """A polygonal region located in a Layer.
+    """A simply-connected polygon located in a Layer.
 
     Args:
         name: Name of the polygon.
         layer: Name of the layer in which the polygon is located.
         points: The polygon vertices. This can be a shape ``(n, 2)`` array of x, y
-            coordinates or a shapely ``LineString``, ``LinearRing``, or ``Polygon``.
-        mesh: Whether to include this polygon when computing a mesh.
+            coordinates or a shapely ``LineString``, ``LinearRing``, or :class:`superscreen.Polygon`.
     """
 
-    __slots__ = ("name", "layer", "_points", "mesh")
+    __slots__ = ("name", "layer", "_points")
 
     def __init__(
         self,
         name: Optional[str] = None,
         *,
         layer: Optional[str] = None,
-        points: Union[
-            np.ndarray,
-            geo.linestring.LineString,
-            geo.polygon.LinearRing,
-            geo.polygon.Polygon,
-        ],
-        mesh: bool = True,
+        points: PolygonType,
     ):
         self.name = name
         self.layer = layer
         self.points = points
-        self.mesh = mesh
 
     @property
     def points(self) -> np.ndarray:
         """A shape ``(n, 2)`` array of counter-clockwise-oriented polygon vertices."""
         return self._points
 
     @points.setter
@@ -175,15 +78,15 @@
         points = close_curve(np.array(points.exterior.coords))
         if points.ndim != 2 or points.shape[-1] != 2:
             raise ValueError(f"Expected shape (n, 2), but got {points.shape}.")
         self._points = points
 
     @property
     def is_valid(self) -> bool:
-        """True if the ``Polygon`` has a ``name`` and ``layer`` its geometry is valid."""
+        """True if the :class:`superscreen.Polygon` has a ``name`` and ``layer`` its geometry is valid."""
         polygon = self.polygon
         return (
             self.name is not None
             and self.layer is not None
             and polygon.is_valid
             and not polygon.interiors
         )
@@ -197,22 +100,46 @@
     def extents(self) -> Tuple[float, float]:
         """Returns the total x, y extent of the polygon, (Delta_x, Delta_y)."""
         minx, miny, maxx, maxy = self.polygon.bounds
         return (maxx - minx), (maxy - miny)
 
     @property
     def polygon(self) -> geo.polygon.Polygon:
-        """A shapely ``Polygon`` representing the Polygon."""
+        """A shapely :class:`superscreen.Polygon` representing the :class:`superscreen.Polygon`"""
         return geo.polygon.Polygon(self.points)
 
     @property
     def path(self) -> path.Path:
         """A matplotlib.path.Path representing the polygon boundary."""
         return path.Path(self.points, closed=True)
 
+    def set_name(self, name: Union[str, None]) -> "Polygon":
+        """Sets the Polygon's name and returns ``self``.
+
+        Args:
+            name: The new name for the :class:`superscreen.Polygon`
+
+        Returns:
+            ``self``
+        """
+        self.name = name
+        return self
+
+    def set_layer(self, layer: Union[str, None]) -> "Polygon":
+        """Sets the Polygon's layer and returns ``self``.
+
+        Args:
+            layer: The new layer for the :class:`superscreen.Polygon`
+
+        Returns:
+            ``self``
+        """
+        self.layer = layer
+        return self
+
     def contains_points(
         self,
         points: np.ndarray,
         index: bool = False,
         radius: float = 0,
     ) -> Union[bool, np.ndarray]:
         """Determines whether ``points`` lie within the polygon.
@@ -262,43 +189,39 @@
         if index:
             return np.where(boundary)[0]
         return boundary
 
     def make_mesh(
         self,
         min_points: Optional[int] = None,
+        max_edge_length: Optional[float] = None,
+        convex_hull: bool = False,
         smooth: int = 0,
         **meshpy_kwargs,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """Returns the vertices and triangles of a Delaunay mesh covering the Polygon.
+    ) -> Mesh:
+        """Creates a :class:`Mesh` for the polygon.
 
         Args:
             min_points: Minimum number of vertices in the mesh. If None, then
                 the number of vertices will be determined by meshpy_kwargs and the
                 number of vertices in the underlying polygons.
+            max_edge_length: The maximum distance between vertices in the resulting mesh.
+            convex_hull: If True, then the entire convex hull of the polygon (minus holes)
+                will be meshed. Otherwise, only the polygon interior is meshed.
             smooth: Number of Laplacian smoothing steps to perform.
             **meshpy_kwargs: Passed to meshpy.triangle.build().
-
-        Returns:
-            Mesh vertex coordinates and triangle indices
         """
         points, triangles = generate_mesh(
             self.points,
             min_points=min_points,
-            convex_hull=False,
+            max_edge_length=max_edge_length,
+            convex_hull=convex_hull,
             **meshpy_kwargs,
         )
-        if smooth:
-            logger.debug(f"Optimizing mesh with {points.shape[0]} vertices.")
-            points, triangles = smooth_mesh(points, triangles, smooth)
-        logger.debug(
-            f"Finished generating mesh with {points.shape[0]} points and "
-            f"{triangles.shape[0]} triangles."
-        )
-        return points, triangles
+        return Mesh.from_triangulation(points, triangles).smooth(smooth)
 
     def rotate(
         self,
         degrees: float,
         origin: Union[str, Tuple[float, float]] = (0.0, 0.0),
         inplace: bool = False,
     ) -> "Polygon":
@@ -370,20 +293,15 @@
         polygon.points = affinity.scale(
             self.polygon, xfact=xfact, yfact=yfact, origin=origin
         )
         return polygon
 
     def _join_via(
         self,
-        other: Union[
-            np.ndarray,
-            "Polygon",
-            geo.polygon.Polygon,
-            geo.polygon.LinearRing,
-        ],
+        other: PolygonType,
         operation: str,
     ) -> geo.polygon.Polygon:
         """Joins ``self.polygon`` with another polygon-like object
         via a given operation.
         """
         valid_types = (
             np.ndarray,
@@ -432,93 +350,73 @@
                 f"The {operation} of the two polygons is not a valid polygon "
                 f"for the following reason: {reason}."
             )
         return joined
 
     def union(
         self,
-        *others: Union[
-            "Polygon",
-            np.ndarray,
-            geo.linestring.LineString,
-            geo.polygon.LinearRing,
-            geo.polygon.Polygon,
-        ],
+        *others: PolygonType,
         name: Optional[str] = None,
     ) -> "Polygon":
         """Returns the union of the polygon and zero or more other polygons.
 
         Args:
             others: One or more objects with which to join the polygon.
-            name: A name for the resulting joined Polygon (defaults to ``self.name``.)
+            name: A name for the resulting joined :class:`superscreen.Polygon` (defaults to ``self.name``.)
 
         Returns:
             A new :class:`Polygon` instance representing the union
             of ``self`` and ``others``.
         """
         if not others:
             return self.copy()
         first, *rest = others
         return Polygon(
             name=name or self.name,
             layer=self.layer,
             points=self._join_via(first, "union"),
-            mesh=self.mesh,
         ).union(*rest, name=name)
 
     def intersection(
         self,
-        *others: Union[
-            "Polygon",
-            np.ndarray,
-            geo.linestring.LineString,
-            geo.polygon.LinearRing,
-            geo.polygon.Polygon,
-        ],
+        *others: PolygonType,
         name: Optional[str] = None,
     ) -> "Polygon":
         """Returns the intersection of the polygon and zero or more other polygons.
 
         Args:
             others: One or more objects with which to join the polygon.
-            name: A name for the resulting joined Polygon (defaults to ``self.name``.)
+            name: A name for the resulting joined :class:`superscreen.Polygon` (defaults to ``self.name``.)
 
         Returns:
             A new :class:`Polygon` instance representing the intersection
             of ``self`` and ``others``.
         """
         if not others:
             return self.copy()
         first, *rest = others
         return Polygon(
             name=name or self.name,
             layer=self.layer,
             points=self._join_via(first, "intersection"),
-            mesh=self.mesh,
         ).intersection(*rest, name=name)
 
     def difference(
         self,
-        *others: Union[
-            "Polygon",
-            np.ndarray,
-            geo.linestring.LineString,
-            geo.polygon.LinearRing,
-            geo.polygon.Polygon,
-        ],
+        *others: PolygonType,
         symmetric: bool = False,
         name: Optional[str] = None,
     ) -> "Polygon":
         """Returns the difference of the polygon and zero more other polygons.
 
         Args:
             others: One or more objects with which to join the polygon.
             symmetric: Whether to join via a symmetric difference operation (aka XOR).
                 See the `shapely documentation`_.
-            name: A name for the resulting joined Polygon (defaults to ``self.name``.)
+            name: A name for the resulting joined :class:`superscreen.Polygon` (defaults to ``self.name``.)
 
         Returns:
             A new :class:`Polygon` instance representing the difference
             of ``self`` and ``others``.
 
         .. _shapely documentation: https://shapely.readthedocs.io/en/stable/manual.html
         """
@@ -526,58 +424,55 @@
         if not others:
             return self.copy()
         first, *rest = others
         return Polygon(
             name=name or self.name,
             layer=self.layer,
             points=self._join_via(first, operation),
-            mesh=self.mesh,
         ).difference(*rest, symmetric=symmetric, name=name)
 
     def buffer(
         self,
         distance: float,
         join_style: Union[str, int] = "mitre",
         mitre_limit: float = 5.0,
         single_sided: bool = True,
         as_polygon: bool = True,
     ) -> Union[np.ndarray, "Polygon"]:
-        """Returns polygon points or a new Polygon object with vertices offset from
+        """Returns polygon points or a new :class:`superscreen.Polygon` object with vertices offset from
         ``self.points`` by a given ``distance``. If ``distance > 0`` this "inflates"
         the polygon, and if ``distance < 0`` this shrinks the polygon.
 
 
         Args:
             distance: The amount by which to inflate or deflate the polygon.
             join_style: One of "round" (1), "mitre" (2), or "bevel" (3).
                 See the `shapely documentation`_.
             mitre_limit: See the `shapely documentation`_.
             single_sided: See the `shapely documentation`_.
-            as_polygon: If True, returns a new ``Polygon`` instance, otherwise
+            as_polygon: If True, returns a new :class:`superscreen.Polygon` instance, otherwise
                 returns a shape ``(n, 2)`` array of polygon vertices.
 
         Returns:
-            A new ``Polygon`` or an array of vertices offset by ``distance``.
+            A new :class:`superscreen.Polygon` or an array of vertices offset by ``distance``.
 
         .. _shapely documentation: https://shapely.readthedocs.io/en/stable/manual.html
         """
         if isinstance(join_style, str):
             join_style = getattr(geo.JOIN_STYLE, join_style)
         poly = self.polygon.buffer(
             distance,
             join_style=join_style,
             mitre_limit=mitre_limit,
             single_sided=single_sided,
         )
-
         polygon = Polygon(
-            name=f"{self.name} ({distance:+.3f})",
+            name=f"{self.name}",
             layer=self.layer,
             points=poly,
-            mesh=self.mesh,
         )
         npts = max(polygon.points.shape[0], self.points.shape[0])
         polygon = polygon.resample(npts)
         if as_polygon:
             return polygon
         return polygon.points
 
@@ -607,15 +502,14 @@
         tck, _ = interpolate.splprep(points.T, k=degree, s=smooth)
         x, y = interpolate.splev(np.linspace(0, 1, num_points - 1), tck)
         points = close_curve(np.stack([x, y], axis=1))
         return Polygon(
             name=self.name,
             layer=self.layer,
             points=points,
-            mesh=self.mesh,
         )
 
     def plot(self, ax: Optional[plt.Axes] = None, **kwargs) -> plt.Axes:
         """Plots the Polygon's vertices.
 
         Args:
             ax: The matplotlib Axes on which to plot. If None is given, a new one
@@ -632,118 +526,88 @@
         ax.plot(*self.points.T, **kwargs)
         ax.set_aspect("equal")
         return ax
 
     @classmethod
     def from_union(
         cls,
-        items: Iterable[
-            Union[
-                "Polygon",
-                np.ndarray,
-                geo.linestring.LineString,
-                geo.polygon.LinearRing,
-                geo.polygon.Polygon,
-            ],
-        ],
+        items: Iterable[PolygonType],
         *,
         name: Optional[str] = None,
         layer: Optional[str] = None,
-        mesh: bool = True,
     ) -> "Polygon":
         """Creates a new :class:`Polygon` from the union of a sequence of polygons.
 
         Args:
             items: A sequence of polygon-like objects to join.
             name: Name of the polygon.
             layer: Name of the layer in which the polygon is located.
-            mesh: Whether to include this polygon when computing a mesh.
 
         Returns:
             A new :class:`Polygon`.
         """
         first, *rest = items
-        polygon = cls(name=name, layer=layer, points=first, mesh=mesh)
+        polygon = cls(name=name, layer=layer, points=first)
         return polygon.union(*rest)
 
     @classmethod
     def from_intersection(
         cls,
-        items: Iterable[
-            Union[
-                "Polygon",
-                np.ndarray,
-                geo.linestring.LineString,
-                geo.polygon.LinearRing,
-                geo.polygon.Polygon,
-            ],
-        ],
+        items: Iterable[PolygonType],
         *,
         name: Optional[str] = None,
         layer: Optional[str] = None,
-        mesh: bool = True,
     ) -> "Polygon":
         """Creates a new :class:`Polygon` from the intersection
         of a sequence of polygons.
 
         Args:
             items: A sequence of polygon-like objects to join.
             name: Name of the polygon.
             layer: Name of the layer in which the polygon is located.
-            mesh: Whether to include this polygon when computing a mesh.
 
         Returns:
             A new :class:`Polygon`.
         """
         first, *rest = items
-        polygon = cls(name=name, layer=layer, points=first, mesh=mesh)
+        polygon = cls(name=name, layer=layer, points=first)
         return polygon.intersection(*rest)
 
     @classmethod
     def from_difference(
         cls,
-        items: Iterable[
-            Union[
-                "Polygon",
-                np.ndarray,
-                geo.linestring.LineString,
-                geo.polygon.LinearRing,
-                geo.polygon.Polygon,
-            ],
-        ],
+        items: Iterable[PolygonType],
         *,
         name: Optional[str] = None,
         layer: Optional[str] = None,
-        mesh: bool = True,
         symmetric: bool = False,
     ) -> "Polygon":
         """Creates a new :class:`Polygon` from the difference
         of a sequence of polygons.
 
         Args:
             items: A sequence of polygon-like objects to join.
             name: Name of the polygon.
             layer: Name of the layer in which the polygon is located.
-            mesh: Whether to include this polygon when computing a mesh.
             symmetric: If True, creates a new :class:`Polygon` from the
                 "symmetric difference" (aka XOR) of the inputs.
 
         Returns:
             A new :class:`Polygon`.
         """
         first, *rest = items
-        polygon = cls(name=name, layer=layer, points=first, mesh=mesh)
+        polygon = cls(name=name, layer=layer, points=first)
         return polygon.difference(*rest, symmetric=symmetric)
 
     def __repr__(self) -> str:
-        name = f'"{self.name}"' if self.name is not None else None
-        layer = f'"{self.layer}"' if self.layer is not None else None
+        name = f"{self.name!r}" if self.name is not None else None
+        layer = f"{self.layer!r}" if self.layer is not None else None
         return (
             f"{self.__class__.__name__}(name={name}, layer={layer}, "
-            f"points=<ndarray: shape={self.points.shape}>, mesh={self.mesh})"
+            f"points=<ndarray: shape={self.points.shape}>)"
         )
 
     def __eq__(self, other) -> bool:
         if other is self:
             return True
 
         if not isinstance(other, Polygon):
@@ -753,7 +617,22 @@
             self.name == other.name
             and self.layer == other.layer
             and np.allclose(self.points, other.points)
         )
 
     def copy(self) -> "Polygon":
         return deepcopy(self)
+
+    def to_hdf5(self, h5group: h5py.Group):
+        if self.name:
+            h5group.attrs["name"] = self.name
+        if self.layer:
+            h5group.attrs["layer"] = self.layer
+        h5group["points"] = self.points
+
+    @staticmethod
+    def from_hdf5(h5group: h5py.Group) -> "Polygon":
+        return Polygon(
+            name=h5group.attrs.get("name", None),
+            layer=h5group.attrs.get("layer", None),
+            points=np.asarray(h5group["points"]),
+        )
```

### Comparing `superscreen-0.8.2/superscreen/device/device.py` & `superscreen-0.9.0/superscreen/device/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,114 @@
-import json
 import logging
 import os
 from collections import defaultdict
-from contextlib import contextmanager
-from copy import deepcopy
-from typing import Any, Dict, List, Optional, Tuple, Union
+from contextlib import contextmanager, nullcontext
+from typing import Dict, List, Literal, Optional, Sequence, Tuple, Union
 
 import dill
+import h5py
 import matplotlib.pyplot as plt
 import numpy as np
-import scipy.sparse as sp
+from IPython.display import HTML
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
+from shapely import geometry as geo
 
 from .. import fem
-from ..parameter import Parameter
+from ..geometry import ensure_unique
 from ..units import ureg
-from . import mesh
-from .components import Layer, Polygon
+from . import utils
+from .layer import Layer
+from .mesh import Mesh
+from .polygon import Polygon
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("device")
 
 
 class Device:
-    """An object representing a device composed of multiple layers of
+    """An object representing a device composed of one or more layers of
     thin film superconductor.
 
     Args:
         name: Name of the device.
         layers: ``Layers`` making up the device.
         films: ``Polygons`` representing regions of superconductor.
         holes: ``Holes`` representing holes in superconducting films.
+        terminals: A dict of ``{film_name: terminals}`` representing transport
+            terminals in the device.
         abstract_regions: ``Polygons`` representing abstract regions in a device.
-            Abstract regions will be meshed, and one can calculate the flux through them.
         length_units: Distance units for the coordinate system.
         solve_dtype: The float data type to use when solving the device.
     """
 
-    ARRAY_NAMES = (
-        "points",
-        "triangles",
-        "weights",
-        "Del2",
-        "Q",
-        "gradx",
-        "grady",
-    )
-
-    POLYGONS = (
-        "films",
-        "holes",
-        "abstract_regions",
-    )
-
     ureg = ureg
 
     def __init__(
         self,
         name: str,
         *,
-        layers: Union[List[Layer], Dict[str, Layer]],
-        films: Union[List[Polygon], Dict[str, Polygon]],
-        holes: Optional[Union[List[Polygon], Dict[str, Polygon]]] = None,
-        abstract_regions: Optional[Union[List[Polygon], Dict[str, Polygon]]] = None,
+        layers: Union[Sequence[Layer], Dict[str, Layer]],
+        films: Union[Sequence[Polygon], Dict[str, Polygon]],
+        holes: Optional[Union[Sequence[Polygon], Dict[str, Polygon]]] = None,
+        terminals: Optional[Dict[str, List[Polygon]]] = None,
+        abstract_regions: Optional[Union[Sequence[Polygon], Dict[str, Polygon]]] = None,
         length_units: str = "um",
-        solve_dtype: Union[str, np.dtype] = "float64",
+        solve_dtype: Union[str, np.dtype] = "float32",
     ):
         self.name = name
 
-        self._films_list = []
-        self._holes_list = []
-        self._abstract_regions_list = []
-        self.layers_list = []
-
         if isinstance(layers, dict):
-            self.layers = layers
-        else:
-            self.layers = {layer.name: layer for layer in layers}
+            layers = list(layers.values())
+        self.layers = {layer.name: layer for layer in layers}
+
         if isinstance(films, dict):
-            self.films = films
-        else:
-            self.films = {film.name: film for film in films}
+            films = list(films.values())
+        self.films = {film.name: film for film in films}
+
         if holes is None:
             holes = []
         if isinstance(holes, dict):
-            self.holes = holes
-        else:
-            self.holes = {hole.name: hole for hole in holes}
+            holes = list(holes.values())
+        self.holes = {hole.name: hole for hole in holes}
+
+        if terminals is None:
+            terminals = {}
+        self.terminals = terminals
+        if not set(self.terminals).issubset(self.films):
+            raise ValueError(
+                f"terminals.keys() must be a subset of films.keys() ({list(self.films)!r})."
+            )
+        for film, terminals in self.terminals.items():
+            for terminal in terminals:
+                terminal.layer = self.films[film].layer
+
         if abstract_regions is None:
             abstract_regions = []
         if isinstance(abstract_regions, dict):
-            self.abstract_regions = abstract_regions
-        else:
-            self.abstract_regions = {region.name: region for region in abstract_regions}
-        for polygons, label in [(self._films_list, "film"), (self._holes_list, "hole")]:
+            abstract_regions = list(abstract_regions.values())
+        self.abstract_regions = {region.name: region for region in abstract_regions}
+
+        for polygons, label in [
+            (self.films.values(), "film"),
+            (self.holes.values(), "hole"),
+        ]:
             for polygon in polygons:
                 if not polygon.is_valid:
                     raise ValueError(f"The following {label} is not valid: {polygon}.")
                 if polygon.layer not in self.layers:
                     raise ValueError(
                         f"The following {label} is assigned to a layer that doesn not "
                         f"exist in the device: {polygon}."
                     )
 
-        if len(self.polygons) < (
-            len(self._holes_list)
-            + len(self._films_list)
-            + len(self._abstract_regions_list)
-        ):
-            raise ValueError("All Polygons in a Device must have a unique name.")
         # Make units a "read-only" attribute.
         # It should never be changed after instantiation.
         self._length_units = length_units
         self.solve_dtype = solve_dtype
-
-        self.points = None
-        self.triangles = None
-
-        self.weights = None
-        self.Del2 = None
-        self.Q = None
-        self.gradx = None
-        self.grady = None
+        self.meshes: Union[Dict[str, Mesh], None] = None
 
     @property
     def length_units(self) -> str:
         """Length units used for the device geometry."""
         return self._length_units
 
     @property
@@ -137,296 +120,143 @@
     def solve_dtype(self, dtype) -> None:
         try:
             _ = np.finfo(dtype)
         except ValueError as e:
             raise ValueError(f"Invalid float dtype: {dtype}") from e
         self._solve_dtype = np.dtype(dtype)
 
-    @property
-    def layers(self) -> Dict[str, Layer]:
-        """Dict of ``{layer_name: layer}``"""
-        return {layer.name: layer for layer in self.layers_list}
-
-    @staticmethod
-    def _validate_polygons(polygons: List[Polygon], label: str) -> List[Polygon]:
-        for polygon in polygons:
-            if not polygon.is_valid:
-                raise ValueError(f"The following {label} is not valid: {polygon}.")
-        return polygons
-
-    @layers.setter
-    def layers(self, layers_dict: Dict[str, Layer]) -> None:
-        """Dict of ``{layer_name: layer}``"""
-        if not (
-            isinstance(layers_dict, dict)
-            and all(isinstance(obj, Layer) for obj in layers_dict.values())
-        ):
-            raise TypeError("Layers must be a dict of {layer_name: Layer}.")
-        self.layers_list = list(layers_dict.values())
+    def get_polygons(self, include_terminals: bool = True) -> List[Polygon]:
+        """Returns list of all Polygons in the device.
 
-    @property
-    def films(self) -> Dict[str, Polygon]:
-        """Dict of ``{film_name: film_polygon}``"""
-        return {film.name: film for film in self._films_list}
-
-    @films.setter
-    def films(self, films_dict: Dict[str, Polygon]) -> None:
-        """Dict of ``{film_name: film_polygon}``"""
-        if not (
-            isinstance(films_dict, dict)
-            and all(isinstance(obj, Polygon) for obj in films_dict.values())
-        ):
-            raise TypeError("Films must be a dict of {film_name: Polygon}.")
-        for name, polygon in films_dict.items():
-            polygon.name = name
-        self._films_list = list(self._validate_polygons(films_dict.values(), "film"))
+        Args:
+            include_terminals: Include transport terminals in the list.
 
-    @property
-    def holes(self) -> Dict[str, Polygon]:
-        """Dict of ``{hole_name: hole_polygon}``"""
-        return {hole.name: hole for hole in self._holes_list}
-
-    @holes.setter
-    def holes(self, holes_dict: Dict[str, Polygon]) -> None:
-        """Dict of ``{hole_name: hole_polygon}``"""
-        if not (
-            isinstance(holes_dict, dict)
-            and all(isinstance(obj, Polygon) for obj in holes_dict.values())
-        ):
-            raise TypeError("Holes must be a dict of {hole_name: Polygon}.")
-        for name, polygon in holes_dict.items():
-            polygon.name = name
-        self._holes_list = list(self._validate_polygons(holes_dict.values(), "hole"))
+        Returns:
+            A list of all Polygons in the device.
+        """
+        polygons = []
+        for attr_name in ("films", "holes", "abstract_regions"):
+            polygons.extend(list(getattr(self, attr_name).values()))
+        if include_terminals:
+            for terminals in self.terminals.values():
+                polygons.extend(terminals)
+        return polygons
 
     @property
-    def abstract_regions(self) -> Dict[str, Polygon]:
-        """Dict of ``{region_name: region_polygon}``"""
-        return {region.name: region for region in self._abstract_regions_list}
-
-    @abstract_regions.setter
-    def abstract_regions(self, regions_dict: Dict[str, Polygon]) -> None:
-        """Dict of ``{region_name: region_polygon}``"""
-        if not (
-            isinstance(regions_dict, dict)
-            and all(isinstance(obj, Polygon) for obj in regions_dict.values())
-        ):
-            raise TypeError(
-                "Abstract regions must be a dict of {region_name: Polygon}."
-            )
-        for name, polygon in regions_dict.items():
-            polygon.name = name
-        self._abstract_regions_list = list(
-            self._validate_polygons(regions_dict.values(), "abstract region")
+    def poly_points(self) -> np.ndarray:
+        """Shape (n, 2) array of (x, y) coordinates of all Polygons in the Device."""
+        points = np.concatenate(
+            [poly.points for poly in self.get_polygons(include_terminals=False)]
         )
-
-    @property
-    def polygons(self) -> Dict[str, Polygon]:
-        """A dict of ``{name: polygon}`` for all Polygons in the device."""
-        polygons = {}
-        for attr_name in self.POLYGONS:
-            polygons.update(getattr(self, attr_name))
-        return polygons
+        # Remove duplicate points to avoid meshing issues.
+        # If you don't do this and there are duplicate points,
+        # meshpy.triangle will segfault.
+        return ensure_unique(points)
 
     def polygons_by_layer(
-        self, polygon_type: Optional[str] = None
+        self,
+        polygon_type: Optional[
+            Literal["film", "hole", "abstract", "terminal", "all"]
+        ] = None,
     ) -> Dict[str, List[Polygon]]:
         """Returns a dict of ``{layer_name: list of polygons in layer}``.
 
         Args:
-            polygon_type: One of 'film', 'hole', or 'all', specifying which types of
-                polygons to include.
+            polygon_type: One of 'film', 'hole', 'abstract', 'terminal', or 'all', specifying
+                which types of polygons to include.
 
         Returns:
            A dict of ``{layer_name: list of polygons in layer of the given type}``.
         """
-        valid_types = ("film", "hole", "all")
+        valid_types = ("film", "hole", "abstract", "terminal", "all")
         if polygon_type is None:
             polygon_type = "all"
         polygon_type = polygon_type.lower()
         if polygon_type not in valid_types:
             raise ValueError(
                 f"Invalid polygon type ({polygon_type}). Expected one of {valid_types!r}."
             )
         if polygon_type == "film":
             all_polygons = self.films.values()
         elif polygon_type == "hole":
             all_polygons = self.holes.values()
+        elif polygon_type == "abstract":
+            all_polygons = self.abstract_regions.values()
+        elif polygon_type == "terminal":
+            all_polygons = []
+            for terminals in self.terminals.values():
+                all_polygons.extend(terminals)
         else:
-            # Films + holes + abstract regions
-            all_polygons = self.polygons.values()
+            # Films + holes + terminals + abstract regions
+            all_polygons = self.get_polygons()
         polygons = {}
         for layer in self.layers:
             polygons[layer] = [p for p in all_polygons if p.layer == layer]
         return polygons
 
-    def contains_points_by_layer(
-        self,
-        points: np.ndarray,
-        polygon_type: Optional[str] = None,
-        index: bool = False,
-        radius: float = 0,
-    ) -> Dict[str, np.ndarray]:
-        """For each layer, determines whether ``points`` lie within a polygon
-        in that layer.
-
-        Args:
-            points: Shape ``(n, 2)`` array of x, y coordinates.
-            polygon_type: One of 'film', 'hole', or 'all', specifying which types of
-                polygons to include.
-            index: If True, then return the indices of the points in ``points``
-                that lie within the polygon. Otherwise, returns a shape ``(n, )``
-                boolean array.
-            radius: An additional margin on ``polygon.path``.
-                See :meth:`matplotlib.path.Path.contains_points`.
-
-        Returns:
-            A dict of ``{layer_name: contains_points}``. If index is True, then
-            ``contains_points`` is an array of indices of the points in ``points``
-            that lie within any polygon in the layer. Otherwise, ``contains_points``
-            is a shape ``(n, )`` boolean array indicating whether each point lies
-            within a polygon in the layer.
-        """
-        polygons_by_layer = self.polygons_by_layer(polygon_type)
-        in_polygons = {}
-        for layer, polygons in polygons_by_layer.items():
-            contains_points = np.logical_or.reduce(
-                [p.contains_points(points, radius=radius) for p in polygons]
-            )
-            if index:
-                contains_points = np.where(contains_points)[0]
-            in_polygons[layer] = contains_points
-        return in_polygons
-
-    @property
-    def poly_points(self) -> np.ndarray:
-        """Shape (n, 2) array of (x, y) coordinates of all Polygons in the Device."""
-        points = np.concatenate(
-            [poly.points for poly in self.polygons.values() if poly.mesh]
-        )
-        # Remove duplicate points to avoid meshing issues.
-        # If you don't do this and there are duplicate points,
-        # meshpy.triangle will segfault.
-        _, ix = np.unique(points, return_index=True, axis=0)
-        points = points[np.sort(ix)]
-        return points
-
-    @property
-    def vertex_distances(self) -> np.ndarray:
-        """An array of the mesh vertex-to-vertex distances."""
-        if self.points is None:
-            return None
-        inv_distances = fem.weights_inv_euclidean(
-            self.points, self.triangles, sparse=True
-        )
-        distances = (1 / inv_distances[inv_distances.nonzero()].toarray()).squeeze()
-        return distances
-
-    @property
-    def triangle_areas(self) -> np.ndarray:
-        """An array of the mesh triangle areas."""
-        if self.points is None:
-            return None
-        return fem.areas(self.points, self.triangles)
-
-    def get_arrays(
-        self,
-        copy_arrays: bool = False,
-        dense: bool = True,
-    ) -> Optional[
-        Dict[str, Union[Union[np.ndarray, sp.csr_matrix], Dict[str, np.ndarray]]]
-    ]:
-        """Returns a dict of the large arrays that belong to the device.
-
-        Args:
-            copy_arrays: Whether to copy all of the arrays or just return references
-                to the existing arrays.
-            dense: Whether to convert any sparse matrices to dense numpy arrays.
+    def holes_by_film(self) -> Dict[str, List[Polygon]]:
+        """Generates a mapping of films to holes contained in the film.
 
         Returns:
-            A dict of arrays, with keys specified by ``Device.ARRAY_NAMES``,
-            or None if the arrays don't exist.
-        """
-        arrays = {name: getattr(self, name, None) for name in self.ARRAY_NAMES}
-        if all(val is None for val in arrays.values()):
-            return None
-        if copy_arrays:
-            arrays = deepcopy(arrays)
-        for name, array in arrays.items():
-            if dense and sp.issparse(array):
-                arrays[name] = array.toarray()
-        return arrays
-
-    def set_arrays(
-        self,
-        arrays: Dict[
-            str, Union[Union[np.ndarray, sp.csr_matrix], Dict[str, np.ndarray]]
-        ],
-    ) -> None:
-        """Sets the Device's large arrays from a dict like that returned
-        by Device.get_arrays().
-
-        Args:
-            arrays: The dict containing the arrays to use.
+           A dict of ``{film_name: list of holes in the film}``.
         """
-        # Ensure that all names and types are valid before setting any attributes.
-        valid_types = {name: (np.ndarray,) for name in self.ARRAY_NAMES}
-        for name in ("Del2", "gradx", "grady"):
-            valid_types[name] = valid_types[name] + (sp.spmatrix,)
-        for name, array in arrays.items():
-            if name not in self.ARRAY_NAMES:
-                raise ValueError(f"Unexpected array name: {name}.")
-            if array is not None and not isinstance(array, valid_types[name]):
-                raise TypeError(
-                    f"Expected type in {valid_types[name]} for array '{name}', "
-                    f"but got {type(array)}."
-                )
-        # Finally actually set the attributes
-        for name, array in arrays.items():
-            setattr(self, name, array)
+        holes_by_layer = self.polygons_by_layer("hole")
+        holes_by_film = {}
+        for film in self.films.values():
+            holes_by_film[film.name] = []
+            for hole in holes_by_layer[film.layer]:
+                if film.contains_points(hole.points).all():
+                    holes_by_film[film.name].append(hole)
+        return holes_by_film
 
-    def copy(self, with_arrays: bool = True, copy_arrays: bool = False) -> "Device":
+    def copy(self, with_mesh: bool = True, copy_mesh: bool = False) -> "Device":
         """Copy this Device to create a new one.
 
         Args:
-            with_arrays: Whether to set the large arrays on the new Device.
-            copy_arrays: Whether to create copies of the large arrays, or just
-                return references to the existing arrays.
+            with_mesh: Whether to shallow copy the ``meshes`` dictionary.
+            copy_mesh: Whether to deepcopy the arrays defining the mesh.
 
         Returns:
             A new Device instance, copied from self
         """
-        layers = [layer.copy() for layer in self.layers_list]
+        layers = [layer.copy() for layer in self.layers.values()]
         films = [film.copy() for film in self.films.values()]
         holes = [hole.copy() for hole in self.holes.values()]
+        terminals = {
+            film: [term.copy() for term in film_terms]
+            for film, film_terms in self.terminals.items()
+        }
         abstract_regions = [region.copy() for region in self.abstract_regions.values()]
 
         device = Device(
             self.name,
             layers=layers,
             films=films,
             holes=holes,
+            terminals=terminals,
             abstract_regions=abstract_regions,
             length_units=self.length_units,
         )
-        if with_arrays:
-            arrays = self.get_arrays(copy_arrays=copy_arrays)
-            if arrays is not None:
-                device.set_arrays(arrays)
+        if with_mesh and self.meshes is not None:
+            meshes = self.meshes
+            if copy_mesh:
+                meshes = {name: mesh.copy() for name, mesh in meshes.items()}
+            device.meshes = meshes
         return device
 
     def __copy__(self) -> "Device":
         # Shallow copy (create new references to existing arrays).
-        return self.copy(with_arrays=True, copy_arrays=False)
+        return self.copy(with_mesh=True, copy_mesh=False)
 
     def __deepcopy__(self, memo) -> "Device":
         # Deep copy (copy all arrays and return references to copies)
-        return self.copy(with_arrays=True, copy_arrays=True)
+        return self.copy(with_mesh=True, copy_mesh=True)
 
     def _warn_if_mesh_exist(self, method: str) -> None:
-        if self.points is None and self.triangles is None:
+        if not self.meshes:
             return
         message = (
             f"Calling device.{method} on a device whose mesh already exists returns "
             f"a new device with no mesh. Call new_device.make_mesh() to generate the mesh "
             f"for the new device."
         )
         logger.warning(message)
@@ -450,16 +280,16 @@
         if not (
             isinstance(origin, tuple)
             and len(origin) == 2
             and all(isinstance(val, (int, float)) for val in origin)
         ):
             raise TypeError("Origin must be a tuple of floats (x, y).")
         self._warn_if_mesh_exist("scale()")
-        device = self.copy(with_arrays=False)
-        for polygon in device.polygons.values():
+        device = self.copy(with_mesh=False)
+        for polygon in device.get_polygons():
             polygon.scale(xfact=xfact, yfact=yfact, origin=origin, inplace=True)
         return device
 
     def rotate(self, degrees: float, origin: Tuple[float, float] = (0, 0)) -> "Device":
         """Returns a new device with polygons rotated a given amount
         counterclockwise about specified origin.
 
@@ -473,63 +303,64 @@
         if not (
             isinstance(origin, tuple)
             and len(origin) == 2
             and all(isinstance(val, (int, float)) for val in origin)
         ):
             raise TypeError("Origin must be a tuple of floats (x, y).")
         self._warn_if_mesh_exist("rotate()")
-        device = self.copy(with_arrays=False)
-        for polygon in device.polygons.values():
+        device = self.copy(with_mesh=False)
+        for polygon in device.get_polygons():
             polygon.rotate(degrees, origin=origin, inplace=True)
         return device
 
     def mirror_layers(self, about_z: float = 0.0) -> "Device":
         """Returns a new device with its layers mirrored about the plane
         ``z = about_z``.
 
         Args:
             about_z: The z-position of the plane (parallel to the x-y plane)
                 about which to mirror the layers.
 
         Returns:
             The mirrored :class:`superscreen.Device`.
         """
-        device = self.copy(with_arrays=True, copy_arrays=True)
+        self._warn_if_mesh_exist("mirror_layers()")
+        device = self.copy(with_mesh=False)
         for layer in device.layers.values():
             layer.z0 = about_z - layer.z0
         return device
 
     def translate(
         self,
         dx: float = 0,
         dy: float = 0,
         dz: float = 0,
         inplace: bool = False,
     ) -> "Device":
-        """Translates the device polygons, layers, and mesh in space by a given amount.
+        """Translates the device polygons, layers, and meshes in space by a given amount.
 
         Args:
             dx: Distance by which to translate along the x-axis.
             dy: Distance by which to translate along the y-axis.
             dz: Distance by which to translate layers along the z-axis.
             inplace: If True, modifies the device (``self``) in-place and returns None,
                 otherwise, creates a new device, translates it, and returns it.
 
         Returns:
             The translated device.
         """
         if inplace:
             device = self
         else:
-            self._warn_if_mesh_exist("translate(..., inplace=False)")
-            device = self.copy(with_arrays=True, copy_arrays=True)
-        for polygon in device.polygons.values():
+            device = self.copy(with_mesh=True, copy_mesh=True)
+        for polygon in device.get_polygons():
             polygon.translate(dx, dy, inplace=True)
-        if device.points is not None:
-            device.points += np.array([[dx, dy]])
+        if device.meshes:
+            for mesh in device.meshes.values():
+                mesh.sites += np.array([[dx, dy]])
         if dz:
             for layer in device.layers.values():
                 layer.z0 += dz
         return device
 
     @contextmanager
     def translation(self, dx: float, dy: float, dz: float = 0) -> None:
@@ -545,104 +376,164 @@
             self.translate(dx, dy, dz=dz, inplace=True)
             yield
         finally:
             self.translate(-dx, -dy, dz=-dz, inplace=True)
 
     def make_mesh(
         self,
-        bounding_polygon: Optional[str] = None,
-        compute_matrices: bool = True,
-        convex_hull: bool = True,
-        weight_method: str = "half_cotangent",
-        min_points: Optional[int] = None,
-        smooth: int = 0,
+        buffer_factor: Union[float, Dict[str, float], None] = 0.05,
+        buffer: Union[float, Dict[str, float], None] = None,
+        join_style: str = "round",
+        min_points: Union[int, Dict[str, int], None] = None,
+        max_edge_length: Union[float, Dict[str, float], None] = None,
+        preserve_boundary: bool = False,
+        smooth: Union[int, Dict[str, int]] = 0,
         **meshpy_kwargs,
     ) -> None:
-        """Generates and optimizes the triangular mesh.
+        """Generates the triangular mesh for each film and stores them in the
+        ``self.meshes`` dictionary.
+
+        The arguments ``buffer_factor``, ``buffer``, ``min_points``,
+        ``max_edge_length``, and ``smooth`` can be specified either as a
+        single value for all films or as a dict of ``{film_name: argument_value}``.
 
         Args:
-            compute_matrices: Whether to compute the field-independent matrices
-                (weights, Q, Laplace operator) needed for Brandt simulations.
-            convex_hull: If True, mesh the entire convex hull of the device's polygons.
-            weight_method: Weight methods for computing the Laplace operator:
-                one of "uniform", "half_cotangent", or "inv_euclidian".
+            buffer_factor: Buffer for the film bounding box(es), in units of the maximum
+                film dimension. This argument is ignored if ``buffer`` is not None.
+            buffer: Buffer for the film bounding box(es), in ``length_units``.
+            join_style: The join style for the buffered region (see :meth:`superscreen.Polygon.buffer`).
             min_points: Minimum number of vertices in the mesh. If None, then
                 the number of vertices will be determined by meshpy_kwargs and the
                 number of vertices in the underlying polygons.
+            max_edge_length: The maximum distance between vertices in the resulting mesh.
+            preserve_boundary: Do not add any mesh sites to the boundary.
             smooth: Number of Laplacian smoothing iterations to perform.
             **meshpy_kwargs: Passed to meshpy.triangle.build().
         """
-        logger.info("Generating mesh...")
-        poly_points = self.poly_points
-        if bounding_polygon is None:
-            boundary = None
-        else:
-            boundary = self.polygons[bounding_polygon].points
-        points, triangles = mesh.generate_mesh(
-            poly_points,
-            min_points=min_points,
-            convex_hull=convex_hull,
-            boundary=boundary,
-            **meshpy_kwargs,
-        )
-        if smooth:
-            logger.info(f"Smoothin mesh with {points.shape[0]} vertices.")
-            points, triangles = mesh.smooth_mesh(points, triangles, smooth)
-        logger.info(
-            f"Finished generating mesh with {points.shape[0]} points and "
-            f"{triangles.shape[0]} triangles."
-        )
-        self.points = points
-        self.triangles = triangles
-
-        self.weights = None
-        self.Del2 = None
-        self.Q = None
-        self.gradx = None
-        self.grady = None
-        if compute_matrices:
-            self.compute_matrices(weight_method=weight_method)
+        films = self.films
+        meshes = {}
+        if not isinstance(buffer_factor, dict):
+            buffer_factor = {name: buffer_factor for name in films}
+        if not isinstance(buffer, dict):
+            buffer = {name: buffer for name in films}
+        if not isinstance(min_points, dict):
+            min_points = {name: min_points for name in films}
+        if not isinstance(max_edge_length, dict):
+            max_edge_length = {name: max_edge_length for name in films}
+        if not isinstance(smooth, dict):
+            smooth = {name: smooth for name in films}
+        holes_by_layer = self.polygons_by_layer("hole")
+        abs_regions_by_layer = self.polygons_by_layer("abstract")
+        for name, film in films.items():
+            film_terminals = self.terminals.get(name)
+            holes = holes_by_layer[film.layer]
+            abs_regions = abs_regions_by_layer[film.layer]
+            coords = [film.points]
+            for poly in holes + abs_regions:
+                if film.contains_points(poly.points).all():
+                    coords.append(poly.points)
+            if film_terminals is not None or (
+                buffer_factor[name] is None and buffer[name] is None
+            ):
+                boundary = film.points
+            else:
+                boundary = Polygon(points=film.points)
+                if buffer[name] is None:
+                    buffer_size = buffer_factor[name] * max(boundary.extents)
+                else:
+                    buffer_size = buffer[name]
+                buffered = boundary.polygon.buffer(
+                    buffer_size,
+                    join_style=getattr(geo.JOIN_STYLE, join_style),
+                    single_sided=True,
+                    mitre_limit=5.0,
+                ).exterior.coords
+                boundary = Polygon(points=buffered).resample(len(film.points)).points
+                coords.append(boundary)
+            points, triangles = utils.generate_mesh(
+                ensure_unique(np.concatenate(coords, axis=0)),
+                min_points=min_points[name],
+                max_edge_length=max_edge_length[name],
+                boundary=boundary,
+                convex_hull=False,
+                preserve_boundary=preserve_boundary or (film_terminals is not None),
+                **meshpy_kwargs,
+            )
+            if smooth[name]:
+                meshes[name] = Mesh.from_triangulation(
+                    points, triangles, build_operators=False
+                ).smooth(smooth[name])
+            else:
+                meshes[name] = Mesh.from_triangulation(points, triangles)
+        self.meshes = meshes
 
-    def compute_matrices(self, weight_method: str = "half_cotangent") -> None:
-        """Calculcates mesh weights, Laplace oeprator, and kernel functions.
+    def boundary_vertices(self, film: str) -> np.ndarray:
+        """An array of boundary vertex indices, ordered counterclockwise.
 
         Args:
-            weight_method: Meshing scheme: either "uniform", "half_cotangent",
-                or "inv_euclidian".
+            film: The name of the film for which to find boundary indices.
+
+        Returns:
+            An array of indices for vertices that are on the film boundary,
+            ordered counterclockwise.
         """
+        if self.meshes is None:
+            return None
+        mesh = self.meshes[film]
+        points = mesh.sites
+        triangles = mesh.elements
+        indices = utils.boundary_vertices(points, triangles)
+        if film not in self.terminals:
+            return indices
+        # Ensure that the indices wrap around outside of any terminals.
+        for terminal in self.terminals[film]:
+            boundary_points = points[indices]
+            terminal_indices = terminal.contains_points(boundary_points, index=True)
+            discont = np.diff(terminal_indices) != 1
+            if np.any(discont):
+                i_discont = np.where(discont)[0][0]
+                indices = np.roll(indices, -(i_discont + 1))
+                break
+        return indices
+
+    def mesh_stats_dict(self) -> Optional[Dict[str, Dict[str, Union[int, float]]]]:
+        """Returns a dictionary of information about all meshes."""
+        if self.meshes is None:
+            return None
+        return {name: mesh.stats() for name, mesh in self.meshes.items()}
 
-        from ..solve import C_vector, Q_matrix, q_matrix
+    def mesh_stats(self, precision: int = 3) -> Optional[HTML]:
+        """When called with in Jupyter notebook, displays
+        a table of information about the mesh.
 
-        points = self.points
-        triangles = self.triangles
+        Args:
+            precision: Number of digits after the decimal for float values.
 
-        if points is None or triangles is None:
-            raise ValueError(
-                "Device mesh does not exist. Run Device.make_mesh() "
-                "to generate the mesh."
-            )
+        Returns:
+            An HTML table of mesh statistics.
+        """
+        all_stats = self.mesh_stats_dict()
+        if all_stats is None:
+            return None
 
-        logger.info("Calculating weight matrix.")
-        self.weights = fem.mass_matrix(points, triangles)
+        def make_row(*cols):
+            return "<tr>" + "".join([f"<td>{c}</td>" for c in cols]) + "</tr>"
 
-        logger.info("Calculating Laplace operator.")
-        self.Del2 = fem.laplace_operator(
-            points,
-            triangles,
-            masses=self.weights,
-            weight_method=weight_method,
-            sparse=True,
-        )
-        logger.info("Calculating kernel matrix.")
-        solve_dtype = self.solve_dtype
-        q = q_matrix(points, dtype=solve_dtype)
-        C = C_vector(points, dtype=solve_dtype)
-        self.Q = Q_matrix(q, C, self.weights, dtype=solve_dtype)
-        logger.info("Calculating gradient matrix.")
-        self.gradx, self.grady = fem.gradient_vertices(points, triangles)
+        html = ["<table>", "<tr><h2>Mesh Statistics</h2></tr>"]
+        html.append(make_row("", "<b>length_units</b>", repr(self.length_units)))
+        for name, stats in all_stats.items():
+            for i, (key, value) in enumerate(stats.items()):
+                if isinstance(value, float):
+                    value = f"{value:.{precision}e}"
+                if i == 0:
+                    html.append(make_row(f"<b>{name!r}</b>", f"<b>{key}</b>", value))
+                else:
+                    html.append(make_row("", f"<b>{key}</b>", value))
+        html.append("</table>")
+        return HTML("".join(html))
 
     def mutual_inductance_matrix(
         self,
         hole_polygon_mapping: Optional[Dict[str, np.ndarray]] = None,
         units: str = "pH",
         all_iterations: bool = False,
         **solve_kwargs,
@@ -670,15 +561,15 @@
         Returns:
             If all_iterations is False, returns a shape ``(n_holes, n_holes)`` mutual
             inductance matrix from the final iteration. Otherwise, returns a list of
             mutual inductance matrices, each with shape ``(n_holes, n_holes)``. The
             length of the list is ``1`` if the device has a single layer, or
             ``iterations + 1`` if the device has multiple layers.
         """
-        from ..solve import solve
+        from ..solver import solve
 
         holes = self.holes
         if hole_polygon_mapping is None:
             from ..fluxoid import make_fluxoid_polygons
 
             hole_polygon_mapping = make_fluxoid_polygons(self)
 
@@ -699,122 +590,190 @@
             solution_slice = slice(None)
         else:
             n_iter = 1
             solution_slice = slice(-1, None)
         mutual_inductance = np.zeros((n_iter, n_holes, n_holes))
         for j, hole_name in enumerate(hole_polygon_mapping):
             logger.info(
-                f"Evaluating '{self.name}' mutual inductance matrix "
+                f"Evaluating {self.name!r} mutual inductance matrix "
                 f"column ({j+1}/{len(hole_polygon_mapping)}), "
-                f"source = '{hole_name}'."
+                f"source = {hole_name!r}."
             )
             solutions = solve(
                 device=self,
                 circulating_currents={hole_name: str(I_circ)},
                 **solve_kwargs,
             )[solution_slice]
+            films_by_hole = {}
+            for film, holes in self.holes_by_film().items():
+                for hole in holes:
+                    films_by_hole[hole.name] = film
             for n, solution in enumerate(solutions):
                 logger.info(
                     f"Evaluating fluxoids for solution {n + 1}/{len(solutions)}."
                 )
                 for i, (name, polygon) in enumerate(hole_polygon_mapping.items()):
-                    layer = holes[name].layer
-                    fluxoid = solution.polygon_fluxoid(polygon, layer)[layer]
+                    fluxoid = solution.polygon_fluxoid(
+                        polygon, film=films_by_hole[name]
+                    )
                     mutual_inductance[n, i, j] = (
                         (sum(fluxoid) / I_circ).to(units).magnitude
                     )
         mutual_inductance = mutual_inductance * self.ureg(units)
         # Return a list to make it clear that we are returning n_iter distinct
         # matrices. You can convert back to an ndarray using
         # np.stack(result, axis=0).
         result = [m for m in mutual_inductance]
         if not all_iterations:
             assert len(result) == 1
             result = result[0]
         return result
 
-    def plot(
+    def plot_polygons(
         self,
         ax: Optional[plt.Axes] = None,
         subplots: bool = False,
-        legend: bool = True,
+        legend: bool = False,
         figsize: Optional[Tuple[float, float]] = None,
-        mesh: bool = False,
-        mesh_kwargs: Dict[str, Any] = dict(color="k", lw=0.5),
         **kwargs,
     ) -> Tuple[plt.Figure, plt.Axes]:
-        """Plot all of the device's polygons.
+        """Plot all of the Device's polygons.
 
         Args:
             ax: matplotlib axis on which to plot. If None, a new figure is created.
-            subplots: If True, plots each layer on a different subplot.
+            subplots: If True, plots each film on a different subplot.
             legend: Whether to add a legend.
             figsize: matplotlib figsize, only used if ax is None.
-            mesh: If True, plot the mesh.
-            mesh_kwargs: Keyword arguments passed to ``ax.triplot()``
-                if ``mesh`` is True.
             kwargs: Passed to ``ax.plot()`` for the polygon boundaries.
 
         Returns:
             Matplotlib Figure and Axes
         """
-        if len(self.layers_list) > 1 and subplots and ax is not None:
+        if len(self.films) > 1 and subplots and ax is not None:
             raise ValueError(
                 "Axes may not be provided if subplots is True and the device has "
-                "multiple layers."
+                "multiple films."
             )
         if ax is None:
             if subplots:
                 from ..visualization import auto_grid
 
                 fig, axes = auto_grid(
-                    len(self.layers_list),
+                    len(self.films),
                     max_cols=2,
                     figsize=figsize,
                     constrained_layout=True,
                 )
             else:
                 fig, axes = plt.subplots(figsize=figsize, constrained_layout=True)
-                axes = np.array([axes for _ in self.layers_list])
+                axes = np.array([axes for _ in self.films])
         else:
             subplots = False
             fig = ax.get_figure()
-            axes = np.array([ax for _ in self.layers_list])
-        polygons_by_layer = defaultdict(list)
-        for polygon in self.polygons.values():
-            polygons_by_layer[polygon.layer].append(polygon)
-        if mesh:
-            if self.triangles is None:
-                raise RuntimeError(
-                    "Mesh does not exist. Run device.make_mesh() to generate the mesh."
-                )
-            x = self.points[:, 0]
-            y = self.points[:, 1]
-            tri = self.triangles
-            mesh_kwargs = mesh_kwargs or {}
-            if subplots:
-                for ax in axes.flat:
-                    ax.triplot(x, y, tri, **mesh_kwargs)
-            else:
-                axes[0].triplot(x, y, tri, **mesh_kwargs)
-        for ax, (layer, polygons) in zip(axes.flat, polygons_by_layer.items()):
-            for polygon in polygons:
-                ax = polygon.plot(ax=ax, **kwargs)
+            axes = np.array([ax for _ in self.films])
+        holes_by_film = self.holes_by_film()
+        terminals = self.terminals
+        for ax, (name, film) in zip(axes.flat, self.films.items()):
+            _ = film.plot(ax=ax, **kwargs)
+            for hole in holes_by_film[name]:
+                _ = hole.plot(ax=ax, **kwargs)
+            if name in terminals:
+                for terminal in terminals[name]:
+                    _ = terminal.plot(ax=ax, **kwargs)
             if subplots:
-                ax.set_title(layer)
+                ax.set_title(name)
             if legend:
                 ax.legend(bbox_to_anchor=(1, 1), loc="upper left")
             units = self.ureg(self.length_units).units
             ax.set_xlabel(f"$x$ $[{units:~L}]$")
             ax.set_ylabel(f"$y$ $[{units:~L}]$")
             ax.set_aspect("equal")
         if not subplots:
             axes = axes[0]
         return fig, axes
 
+    def plot_mesh(
+        self,
+        ax: Optional[plt.Axes] = None,
+        subplots: bool = False,
+        figsize: Optional[Tuple[float, float]] = None,
+        show_sites: bool = False,
+        show_edges: bool = True,
+        site_color: Union[str, Sequence[float], None] = None,
+        edge_color: Union[str, Sequence[float], None] = None,
+        linewidth: float = 0.75,
+        linestyle: str = "-",
+        marker: str = ".",
+    ) -> Tuple[plt.Figure, plt.Axes]:
+        """Plot all of the Device's meshes.
+
+        Args:
+            ax: matplotlib axis on which to plot. If None, a new figure is created.
+            subplots: If True, plots each film on a different subplot.
+            figsize: matplotlib figsize, only used if ax is None.
+            show_sites: Whether to show the mesh sites.
+            show_edges: Whether to show the mesh edges.
+            site_color: The color for the sites.
+            edge_color: The color for the edges.
+            linewidth: The line width for all edges.
+            linestyle: The line style for all edges.
+            marker: The marker to use for the mesh sites.
+
+        Returns:
+            Matplotlib Figure and Axes
+        """
+        if len(self.films) > 1 and subplots and ax is not None:
+            raise ValueError(
+                "Axes may not be provided if subplots is True and the device has "
+                "multiple films."
+            )
+        if self.meshes is None:
+            raise ValueError(
+                "Mesh doesn't exist. Run Device.make_mesh() to generate one."
+            )
+        if ax is None:
+            if subplots:
+                from ..visualization import auto_grid
+
+                fig, axes = auto_grid(
+                    len(self.films),
+                    max_cols=2,
+                    figsize=figsize,
+                    constrained_layout=True,
+                )
+            else:
+                fig, axes = plt.subplots(figsize=figsize, constrained_layout=True)
+                axes = np.array([axes for _ in self.films])
+        else:
+            subplots = False
+            fig = ax.get_figure()
+            axes = np.array([ax for _ in self.films])
+        for i, (ax, (name, mesh)) in enumerate(zip(axes.flat, self.meshes.items())):
+            sc = f"C{i}" if site_color is None else site_color
+            ec = f"C{i}" if edge_color is None else edge_color
+            ax = mesh.plot(
+                ax=ax,
+                show_sites=show_sites,
+                show_edges=show_edges,
+                site_color=sc,
+                edge_color=ec,
+                linestyle=linestyle,
+                linewidth=linewidth,
+                marker=marker,
+            )
+            if subplots:
+                ax.set_title(name)
+            units = self.ureg(self.length_units).units
+            ax.set_xlabel(f"$x$ $[{units:~L}]$")
+            ax.set_ylabel(f"$y$ $[{units:~L}]$")
+            ax.set_aspect("equal")
+        if not subplots:
+            axes = axes[0]
+        return fig, axes
+
     def patches(self) -> Dict[str, Dict[str, PathPatch]]:
         """Returns a dict of ``{layer_name: {film_name: PathPatch}}``
         for visualizing the device.
         `"""
         abstract_regions = self.abstract_regions
         polygons_by_layer = self.polygons_by_layer()
         holes_by_layer = self.polygons_by_layer(polygon_type="hole")
@@ -865,15 +824,15 @@
                 from the figure.
             layer_order: If ``"increasing"`` (``"decreasing"``) draw polygons in
                 increasing (decreasing) order by layer height ``layer.z0``.
 
         Returns:
             Matplotlib Figre and Axes.
         """
-        if len(self.layers_list) > 1 and subplots and ax is not None:
+        if len(self.layers) > 1 and subplots and ax is not None:
             raise ValueError(
                 "Axes may not be provided if subplots is True and the device has "
                 "multiple layers."
             )
         layer_order = layer_order.lower()
         layer_orders = ("increasing", "decreasing")
         if layer_order not in layer_orders:
@@ -882,30 +841,32 @@
                 f"Valid layer orders are {layer_orders}."
             )
         if ax is None:
             if subplots:
                 from ..visualization import auto_grid
 
                 fig, axes = auto_grid(
-                    len(self.layers_list),
+                    len(self.layers),
                     max_cols=max_cols,
                     figsize=figsize,
                     constrained_layout=True,
                 )
             else:
                 fig, ax = plt.subplots(figsize=figsize, constrained_layout=True)
-                axes = np.array([ax for _ in self.layers_list])
+                axes = np.array([ax for _ in self.layers])
         else:
             subplots = False
             fig = ax.get_figure()
-            axes = np.array([ax for _ in self.layers_list])
+            axes = np.array([ax for _ in self.layers])
         exclude = exclude or []
         if isinstance(exclude, str):
             exclude = [exclude]
-        layers = [layer.name for layer in sorted(self.layers_list, key=lambda x: x.z0)]
+        layers = [
+            layer.name for layer in sorted(self.layers.values(), key=lambda x: x.z0)
+        ]
         if layer_order == "decreasing":
             layers = layers[::-1]
         patches = self.patches()
         used_axes = set()
         units = self.ureg(self.length_units).units
         x, y = self.poly_points.T
         margin = 0.1
@@ -949,228 +910,154 @@
                     fig.delaxes(ax)
         else:
             axes = axes[0]
             if legend:
                 axes.legend(handles, labels, bbox_to_anchor=(1, 1), loc="upper left")
         return fig, axes
 
-    def to_file(
-        self, directory: str, save_mesh: bool = True, compressed: bool = True
+    def to_hdf5(
+        self,
+        path_or_group: Union[os.PathLike, h5py.Group],
+        save_mesh: bool = True,
+        compress: bool = True,
     ) -> None:
-        """Serializes the Device to disk.
+        """Serializes the Device to and HDF5 file.
 
         Args:
-            directory: The name of the directory in which to save the Device
-                (must either be empty or not yet exist).
+            path_or_group: Path to an HDF5 file to create, or an open HD5F file.
             save_mesh: Whether to save the full mesh to file.
-            compressed: Whether to use numpy.savez_compressed rather than numpy.savez
-                when saving the mesh.
+            compress: Save the minimum amount of data needed to recreate the mesh.
         """
-        from ..io import NumpyJSONEncoder
-
-        if os.path.isdir(directory) and len(os.listdir(directory)):
-            raise IOError(f"Directory '{directory}' already exists and is not empty.")
-        os.makedirs(directory, exist_ok=True)
-
-        # Serialize films, holes, and abstract_regions to JSON
-        polygons = {"device_name": self.name, "length_units": self.length_units}
-        for poly_type in ["films", "holes", "abstract_regions"]:
-            polygons[poly_type] = {}
-            for name, poly in getattr(self, poly_type).items():
-                polygons[poly_type][name] = {
-                    "layer": poly.layer,
-                    "points": poly.points,
-                }
-        with open(os.path.join(directory, "polygons.json"), "w") as f:
-            json.dump(polygons, f, indent=4, cls=NumpyJSONEncoder)
-
-        # Serialize layers to JSON.
-        # If Lambda or london_lambda is a Parameter, then we will
-        # pickle it using dill.
-        layers = {
-            "device_name": self.name,
-            "length_units": self.length_units,
-            "solve_dtype": str(self.solve_dtype),
-        }
-        for name, layer in self.layers.items():
-            layers[name] = {"z0": layer.z0, "thickness": layer.thickness}
-            if isinstance(layer._Lambda, (int, float)):
-                layers[name]["Lambda"] = layer._Lambda
-                layers[name]["london_lambda"] = None
-            elif isinstance(layer.london_lambda, (int, float)):
-                layers[name]["Lambda"] = None
-                layers[name]["london_lambda"] = layer.london_lambda
-            else:
-                if isinstance(layer._Lambda, Parameter):
-                    # Lambda is defined as a Parameter and london_lambda is None
-                    assert layer.london_lambda is None
-                    param = layer._Lambda
-                    key = "Lambda"
-                    null_key = "london_lambda"
-                else:
-                    # london_lambda is defined as a Parameter and _Lambda is None
-                    assert layer._Lambda is None
-                    param = layer.london_lambda
-                    key = "london_lambda"
-                    null_key = "Lambda"
-                dill_fname = f"{layer.name}_{param.func.__name__}.dill"
-                layers[name][null_key] = None
-                layers[name][key] = {"path": dill_fname}
-                with open(os.path.join(directory, dill_fname), "wb") as f:
-                    dill.dump(param, f)
-
-        with open(os.path.join(directory, "layers.json"), "w") as f:
-            json.dump(layers, f, indent=4, cls=NumpyJSONEncoder)
-
-        if save_mesh:
-            # Serialize mesh, if it exists.
-            save_npz = np.savez_compressed if compressed else np.savez
-            if self.points is not None:
-                save_npz(
-                    os.path.join(directory, "mesh.npz"),
-                    points=self.points,
-                    triangles=self.triangles,
-                )
+        if isinstance(path_or_group, h5py.Group):
+            save_context = nullcontext(path_or_group)
+        else:
+            save_context = h5py.File(path_or_group, "x")
+        with save_context as h5group:
+            h5group.attrs["name"] = self.name
+            h5group.attrs["length_units"] = self.length_units
+            h5group.attrs["solve_dtype"] = str(self.solve_dtype)
+            layer_grp = h5group.create_group("layers")
+            film_grp = h5group.create_group("films")
+            hole_grp = h5group.create_group("holes")
+            terminals_grp = h5group.create_group("terminals")
+            abs_grp = h5group.create_group("abstract_regions")
+            for name, layer in self.layers.items():
+                layer.to_hdf5(layer_grp.create_group(name))
+            for name, polygon in self.films.items():
+                polygon.to_hdf5(film_grp.create_group(name))
+            for name, polygon in self.holes.items():
+                polygon.to_hdf5(hole_grp.create_group(name))
+            for name, polygon in self.abstract_regions.items():
+                polygon.to_hdf5(abs_grp.create_group(name))
+            for film_name, terminals in self.terminals.items():
+                grp = terminals_grp.create_group(film_name)
+                for i, terminal in enumerate(terminals):
+                    terminal.to_hdf5(grp.create_group(str(i)))
+            if save_mesh and self.meshes:
+                mesh_grp = h5group.create_group("mesh")
+                for name, mesh in self.meshes.items():
+                    mesh.to_hdf5(mesh_grp.create_group(name), compress=compress)
 
-    @classmethod
-    def from_file(cls, directory: str, compute_matrices: bool = False) -> "Device":
-        """Creates a new Device from one serialized to disk.
+    @staticmethod
+    def from_hdf5(path_or_group: Union[os.PathLike, h5py.Group]) -> "Device":
+        """Loads a Device from an HDF5 file.
 
         Args:
-            directory: The directory from which to load the device.
-            compute_matrices: Whether to compute the field-independent
-                matrices for the device if the mesh already exists.
+            path_or_group: Path to an HDF5 file to read, or an open HD5F file.
 
         Returns:
-            The loaded Device instance
+            The deserialized Device.
         """
-        from ..io import json_numpy_obj_hook
-
-        # Load all polygons (films, holes, abstract_regions)
-        with open(os.path.join(directory, "polygons.json"), "r") as f:
-            polygons_json = json.load(f, object_hook=json_numpy_obj_hook)
-
-        device_name = polygons_json.pop("device_name")
-        length_units = polygons_json.pop("length_units")
-        films = {
-            name: Polygon(name, **kwargs)
-            for name, kwargs in polygons_json["films"].items()
-        }
-        holes = {
-            name: Polygon(name, **kwargs)
-            for name, kwargs in polygons_json["holes"].items()
-        }
-        abstract_regions = {
-            name: Polygon(name, **kwargs)
-            for name, kwargs in polygons_json["abstract_regions"].items()
-        }
-
-        # Load all layers
-        with open(os.path.join(directory, "layers.json"), "r") as f:
-            layers_json = json.load(f, object_hook=json_numpy_obj_hook)
-
-        device_name = layers_json.pop("device_name")
-        length_units = layers_json.pop("length_units")
-        solve_dtype = layers_json.pop("solve_dtype", "float64")
-        for name, layer_dict in layers_json.items():
-            # Check whether either Lambda or london_lambda is a Parameter
-            # that was pickled.
-            if isinstance(layer_dict["Lambda"], dict):
-                assert layer_dict["london_lambda"] is None
-                path = layer_dict["Lambda"]["path"]
-                with open(os.path.join(directory, path), "rb") as f:
-                    Lambda = dill.load(f)
-                layers_json[name]["Lambda"] = Lambda
-            elif isinstance(layer_dict["london_lambda"], dict):
-                assert layer_dict["Lambda"] is None
-                path = layer_dict["london_lambda"]["path"]
-                with open(os.path.join(directory, path), "rb") as f:
-                    london_lambda = dill.load(f)
-                layers_json[name]["london_lambda"] = london_lambda
-
-        layers = {name: Layer(name, **kwargs) for name, kwargs in layers_json.items()}
-
-        device = cls(
-            device_name,
-            layers=layers,
-            films=films,
-            holes=holes,
-            abstract_regions=abstract_regions,
-            length_units=length_units,
-            solve_dtype=solve_dtype,
-        )
-
-        # Load the mesh if it exists
-        if "mesh.npz" in os.listdir(directory):
-            with np.load(os.path.join(directory, "mesh.npz")) as npz:
-                device.points = npz["points"]
-                device.triangles = npz["triangles"]
-
-        if compute_matrices and device.Del2 is None:
-            device.compute_matrices()
-
-        return device
+        if isinstance(path_or_group, h5py.Group):
+            read_context = nullcontext(path_or_group)
+        else:
+            read_context = h5py.File(path_or_group, "r")
+        with read_context as h5group:
+            terminals = {}
+            for film, grp in h5group["terminals"].items():
+                terminals[film] = []
+                for i in range(len(grp)):
+                    terminals[film].append(Polygon.from_hdf5(grp[str(i)]))
+            device = Device(
+                name=h5group.attrs["name"],
+                layers=[Layer.from_hdf5(grp) for grp in h5group["layers"].values()],
+                films=[Polygon.from_hdf5(grp) for grp in h5group["films"].values()],
+                holes=[Polygon.from_hdf5(grp) for grp in h5group["holes"].values()],
+                terminals=terminals,
+                abstract_regions=[
+                    Polygon.from_hdf5(grp)
+                    for grp in h5group["abstract_regions"].values()
+                ],
+                length_units=h5group.attrs["length_units"],
+                solve_dtype=h5group.attrs["solve_dtype"],
+            )
+            if "mesh" in h5group:
+                device.meshes = {
+                    name: Mesh.from_hdf5(grp) for name, grp in h5group["mesh"].items()
+                }
+            return device
 
     def __repr__(self) -> str:
         # Normal tab "\t" renders a bit too big in jupyter if you ask me.
         indent = 4
         t = " " * indent
         nt = "\n" + t
 
-        # def format_dict(d):
-        #     if not d:
-        #         return None
-        #     items = [f'{t}"{key}": {value}' for key, value in d.items()]
-        #     return "{" + nt + (", " + nt).join(items) + "," + nt + "}"
-
-        # args = [
-        #     f'"{self.name}"',
-        #     f"layers={format_dict(self.layers)}",
-        #     f"films={format_dict(self.films)}",
-        #     f"holes={format_dict(self.holes)}",
-        #     f"abstract_regions={format_dict(self.abstract_regions)}",
-        #     f'length_units="{self.length_units}"',
-        # ]
-
         def format_list(L):
             if not L:
                 return None
             items = [f"{t}{value}" for value in L]
             return "[" + nt + (", " + nt).join(items) + "," + nt + "]"
 
+        def format_dict(D):
+            if not D:
+                return None
+            items = [f"{t}{key!r}: {value}" for key, value in D.items()]
+            return "{" + nt + (", " + nt).join(items) + "," + nt + "}"
+
         args = [
             f'"{self.name}"',
-            f"layers={format_list(self.layers_list)}",
-            f"films={format_list(self._films_list)}",
-            f"holes={format_list(self._holes_list)}",
-            f"abstract_regions={format_list(self._abstract_regions_list)}",
+            f"layers={format_list(self.layers.values())}",
+            f"films={format_list(self.films.values())}",
+            f"holes={format_list(self.holes.values())}",
+            f"terminals={format_dict(self.terminals)}",
+            f"abstract_regions={format_list(self.abstract_regions.values())}",
             f'length_units="{self.length_units}"',
         ]
 
         return f"{self.__class__.__name__}(" + nt + (", " + nt).join(args) + ",\n)"
 
     def __eq__(self, other) -> bool:
         if other is self:
             return True
 
         if not isinstance(other, Device):
             return False
 
+        def equals_sorted(first, second):
+            def key(x):
+                return x.name
+
+            return sorted(first, key=key) == sorted(second, key=key)
+
         return (
             self.name == other.name
-            and self.layers_list == other.layers_list
-            and self.films == other.films
-            and self.holes == other.holes
-            and self.abstract_regions == other.abstract_regions
+            and equals_sorted(self.layers.values(), other.layers.values())
+            and equals_sorted(self.films.values(), other.films.values())
+            and equals_sorted(self.holes.values(), other.holes.values())
+            and self.terminals == other.terminals
+            and equals_sorted(
+                self.abstract_regions.values(), other.abstract_regions.values()
+            )
             and self.length_units == other.length_units
         )
 
     def __getstate__(self):
         state = self.__dict__.copy()
         # Use dill for Layer objects because Layer.Lambda could be a Parameter
-        state["layers_list"] = dill.dumps(self.layers_list)
+        state["layers"] = dill.dumps(self.layers)
         return state
 
     def __setstate__(self, state):
         # Use dill for Layer objects because Layer.Lambda could be a Parameter
-        state["layers_list"] = dill.loads(state["layers_list"])
+        state["layers"] = dill.loads(state["layers"])
         self.__dict__.update(state)
```

### Comparing `superscreen-0.8.2/superscreen/fem.py` & `superscreen-0.9.0/superscreen/fem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 import warnings
-from typing import Optional, Tuple, Union
+from typing import Literal, Optional, Tuple, Union
 
 import numpy as np
 import scipy.linalg as la
 import scipy.sparse as sp
 from matplotlib.path import Path
 
 
+def triangle_areas(points: np.ndarray, triangles: np.ndarray) -> np.ndarray:
+    """Calculates the area of each triangle.
+
+    Args:
+        points: Shape (n, 2) array of x, y coordinates of vertices
+        triangles: Shape (m, 3) array of triangle indices
+
+    Returns:
+        Shape (m, ) array of triangle areas
+    """
+    xy = points[triangles]
+    # s1 = xy[:, 2, :] - xy[:, 1, :]
+    # s2 = xy[:, 0, :] - xy[:, 2, :]
+    # s3 = xy[:, 1, :] - xy[:, 0, :]
+    # which can be simplified to
+    # s = xy[:, [2, 0, 1]] - xy[:, [1, 2, 0]]  # 3D
+    s = xy[:, [2, 0]] - xy[:, [1, 2]]  # 2D
+    a = np.linalg.det(s)
+    return a * 0.5
+
+
 def in_polygon(
     poly_points: np.ndarray,
     query_points: np.ndarray,
     radius: float = 0,
 ) -> Union[bool, np.ndarray]:
     """Returns a boolean array indicating which points in ``query_points``
     lie inside the polygon defined by ``poly_points``.
@@ -42,69 +63,48 @@
 
     Returns:
         Shape (m, 2) array of triangle centroid (center of mass) coordinates
     """
     return points[triangles].sum(axis=1) / 3
 
 
-def areas(points: np.ndarray, triangles: np.ndarray) -> np.ndarray:
-    """Calculates the area of each triangle.
-
-    Args:
-        points: Shape (n, 2) array of x, y coordinates of vertices
-        triangles: Shape (m, 3) array of triangle indices
-
-    Returns:
-        Shape (m, ) array of triangle areas
-    """
-    xy = points[triangles]
-    # s1 = xy[:, 2, :] - xy[:, 1, :]
-    # s2 = xy[:, 0, :] - xy[:, 2, :]
-    # s3 = xy[:, 1, :] - xy[:, 0, :]
-    # which can be simplified to
-    # s = xy[:, [2, 0, 1]] - xy[:, [1, 2, 0]]  # 3D
-    s = xy[:, [2, 0]] - xy[:, [1, 2]]  # 2D
-    a = np.linalg.det(s)
-    return a * 0.5
-
-
 def adjacency_matrix(
     triangles: np.ndarray, sparse: bool = True
-) -> Union[np.ndarray, sp.csr_matrix]:
+) -> Union[np.ndarray, sp.csr_array]:
     """Computes the adjacency matrix for a given set of triangles.
 
     Args:
         triangles: Shape (m, 3) array of triangle indices
-        sparse: Whether to return a sparse matrix or numpy ndarray.
+        sparse: Whether to return a sparse array or numpy ndarray.
 
     Returns:
         Shape (n, n) adjacency matrix, where n = triangles.max() + 1
 
     """
     # shape (m * 3, 2) array of graph edges
     edges = np.concatenate(
         [triangles[:, [0, 1]], triangles[:, [1, 2]], triangles[:, [2, 0]]]
     )
     row, col = edges[:, 0], edges[:, 1]
     nrow, ncol = row.max() + 1, col.max() + 1
     data = np.ones_like(row, dtype=int)
-    # This is the (data, (row_ind, col_ind)) format for csr_matrix,
+    # This is the (data, (row_ind, col_ind)) format for csr_array,
     # meaning that adj[row_ind[k], col_ind[k]] = data[k]
-    adj = sp.csr_matrix((data, (row, col)), shape=(nrow, ncol))
+    adj = sp.csr_array((data, (row, col)), shape=(nrow, ncol))
     # Undirected graph -> symmetric adjacency matrix
     adj = adj + adj.T
     adj = (adj > 0).astype(int)
     if sparse:
         return adj
     return adj.toarray()
 
 
 def weights_inv_euclidean(
     points: np.ndarray, triangles: np.ndarray, sparse: bool = True
-) -> Union[np.ndarray, sp.lil_matrix]:
+) -> Union[np.ndarray, sp.lil_array]:
     """Weights edges by the inverse Euclidean distance of the edge lengths.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices.
         triangles: Shape (m, 3) array of triangle indices.
         sparse: Whether to return a sparse matrix or numpy ndarray.
 
@@ -112,16 +112,16 @@
         Shape (n, n) matrix of vertex weights
     """
     # Adapted from spharaphy.TriMesh:
     # https://spharapy.readthedocs.io/en/latest/modules/trimesh.html
     # https://gitlab.com/uwegra/spharapy/-/blob/master/spharapy/trimesh.py
     N = points.shape[0]
     if sparse:
-        # Use lil_matrix for operations that change matrix sparsity
-        weights = sp.lil_matrix((N, N), dtype=float)
+        # Use lil_array for operations that change matrix sparsity
+        weights = sp.lil_array((N, N), dtype=float)
     else:
         weights = np.zeros((N, N), dtype=float)
 
     # Compute the three vectors of each triangle and their norms
     vec10 = points[triangles[:, 1]] - points[triangles[:, 0]]
     vec20 = points[triangles[:, 2]] - points[triangles[:, 0]]
     vec21 = points[triangles[:, 2]] - points[triangles[:, 1]]
@@ -137,15 +137,15 @@
     weights[triangles[:, 1], triangles[:, 2]] = 1 / n21
 
     return weights
 
 
 def weights_half_cotangent(
     points: np.ndarray, triangles: np.ndarray, sparse: bool = True
-) -> Union[np.ndarray, sp.lil_matrix]:
+) -> Union[np.ndarray, sp.lil_array]:
     """Weights edges by half of the cotangent of the two angles opposite the edge.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices.
         triangles: Shape (m, 3) array of triangle indices.
         sparse: Whether to return a sparse matrix or numpy ndarray.
 
@@ -153,16 +153,16 @@
         Shape (n, n) matrix of vertex weights
     """
     # Adapted from spharaphy.TriMesh:
     # https://spharapy.readthedocs.io/en/latest/modules/trimesh.html
     # https://gitlab.com/uwegra/spharapy/-/blob/master/spharapy/trimesh.py
     N = points.shape[0]
     if sparse:
-        # Use lil_matrix for operations that change matrix sparsity
-        weights = sp.lil_matrix((N, N), dtype=float)
+        # Use lil_array for operations that change matrix sparsity
+        weights = sp.lil_array((N, N), dtype=float)
     else:
         weights = np.zeros((N, N), dtype=float)
 
     # First vertex
     vec1 = points[triangles[:, 1]] - points[triangles[:, 0]]
     vec2 = points[triangles[:, 2]] - points[triangles[:, 0]]
     w = 0.5 / np.tan(
@@ -202,15 +202,15 @@
 
 
 def calculate_weights(
     points: np.ndarray,
     triangles: np.ndarray,
     method: str,
     sparse: bool = True,
-) -> Union[np.ndarray, sp.csr_matrix]:
+) -> Union[np.ndarray, sp.csr_array]:
     """Returns the weight matrix, calculated using the specified method.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices.
         triangles: Shape (m, 3) array of triangle indices.
         method: Method for calculating the weights. One of: "uniform",
             "inv_euclidean", or "half_cotangent".
@@ -229,190 +229,173 @@
         return weights_half_cotangent(points, triangles, sparse=sparse)
     raise ValueError(
         f"Unknown method ({method}). "
         f"Supported methods are 'uniform', 'inv_euclidean', and 'half_cotangent'."
     )
 
 
-def mass_matrix(
-    points: np.ndarray,
-    triangles: np.ndarray,
-    sparse: bool = False,
-) -> Union[np.ndarray, sp.csc_matrix]:
-    """The mass matrix defines an effective area for each vertex.
-
-    Args:
-        points: Shape (n, 2) array of x, y coordinates of vertices.
-        triangles: Shape (m, 3) array of triangle indices.
-        sparse: Whether to return a sparse matrix or numpy ndarray.
-
-    Returns:
-        Shape (n, n) sparse mass matrix or shape (n,) vector of diagonals.
-    """
-    # Adapted from spharaphy.TriMesh:
-    # https://spharapy.readthedocs.io/en/latest/modules/trimesh.html
-    # https://gitlab.com/uwegra/spharapy/-/blob/master/spharapy/trimesh.py
-    N = points.shape[0]
-    if sparse:
-        mass = sp.lil_matrix((N, N), dtype=float)
-    else:
-        mass = np.zeros((N, N), dtype=float)
-
-    tri_areas = areas(points, triangles)
-
-    for a, t in zip(tri_areas / 3, triangles):
-        mass[t[0], t[0]] += a
-        mass[t[1], t[1]] += a
-        mass[t[2], t[2]] += a
-
-    if sparse:
-        # Use csc_matrix because we will eventually invert the mass matrix,
-        # and csc is efficient for inversion.
-        return mass.tocsc()
-    return mass.diagonal()
-
-
 def laplace_operator(
     points: np.ndarray,
     triangles: np.ndarray,
-    masses: Optional[Union[np.ndarray, sp.spmatrix]] = None,
-    weight_method: str = "half_cotangent",
+    masses: Optional[np.ndarray] = None,
+    weight_method: Literal[
+        "uniform", "half_cotangent", "inv_euclidean"
+    ] = "half_cotangent",
     sparse: bool = True,
-) -> Union[np.ndarray, sp.csr_matrix]:
+) -> Union[np.ndarray, sp.csr_array]:
     """Laplacian operator for the mesh (sometimes called
     Laplace-Beltrami operator).
 
     The Laplacian operator is defined as ``inv(M) @ L``,
     where M is the mass matrix and L is the Laplacian matrix.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices.
         triangles: Shape (m, 3) array of triangle indices.
-        masses: Pre-computed mass matrix: shape (n, n) sparse diagonal matrix
-            or shape (n,) array of diagonals.
+        masses: Pre-computed mass matrix, i.e., the vertex areas.
         weight_method: Method for calculating the weights. One of: "uniform",
             "inv_euclidean", or "half_cotangent".
         sparse: Whether to return a sparse matrix or numpy ndarray.
 
     Returns:
         Shape (n, n) Laplacian operator
     """
     # See: http://rodolphe-vaillant.fr/?e=20
     # See: http://ddg.cs.columbia.edu/SGP2014/LaplaceBeltrami.pdf
     if masses is None:
-        masses = mass_matrix(points, triangles)
-    if sp.issparse(masses):
-        masses = masses.diagonal()
+        from .device.utils import vertex_areas
+
+        masses = vertex_areas(points, triangles)
     L = calculate_weights(points, triangles, weight_method, sparse=True)
     with warnings.catch_warnings():
-        # scipy.sparse throws a warning here
         warnings.filterwarnings("ignore", message="Changing the sparsity structure")
         L.setdiag(0)
-        w_sum = np.atleast_2d(L.sum(axis=1))
-        L.setdiag(-w_sum)
+        L.setdiag(-L.sum(axis=1))
         L = L.tocsr()
-    Del2 = sp.diags(1 / masses, format="csr") @ L
-    if not sparse:
-        Del2 = Del2.toarray()
-    return Del2
+    laplacian = sp.diags(1 / masses, format="csr") @ L
+    if sparse:
+        return laplacian
+    return laplacian.toarray()
 
 
 def gradient_triangles(
     points: np.ndarray,
     triangles: np.ndarray,
-    triangle_areas: Optional[np.ndarray] = None,
-) -> Tuple[sp.csr_matrix, sp.csr_matrix]:
+    areas: Optional[np.ndarray] = None,
+) -> Tuple[sp.csr_array, sp.csr_array]:
     """Returns the triangle gradient operators ``Gx`` and ``Gy``.
 
     Given a mesh with ``n`` vertices and ``m`` triangles and a scalar field ``f``
     defined at the mesh vertices, ``Gx`` and ``Gy`` are shape ``(m, n)`` matrices
     such that ``Gx @ f`` and ``Gy @ f`` compute the gradients of ``f`` along
     x and y, evaluated at the triangle centroids.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices
         triangles: Shape (m, 3) array of triangle indices
-        triangle_areas: Shape (m, ) array of triangle areas
+        _areas: Shape (m, ) array of triangle areas
 
     Returns:
         x and y gradient matrices, both of which have shape ``(m, n)``
     """
-    if triangle_areas is None:
-        triangle_areas = areas(points, triangles)
+    if areas is None:
+        areas = triangle_areas(points, triangles)
     # Shape (triangles.shape[0], 3, 2)
     xy = points[triangles]
     edges = np.roll(xy, 2, axis=1) - np.roll(xy, 1, axis=1)
     # Rotate edges clockwise by 90 degrees:
     # +x --> -y, +y --> +x
     edges_rot = np.empty_like(edges)
     edges_rot[:, :, 0] = +edges[:, :, 1]
     edges_rot[:, :, 1] = -edges[:, :, 0]
 
-    tri_data = edges_rot / (2 * triangle_areas[:, np.newaxis, np.newaxis])
+    tri_data = edges_rot / (2 * areas[:, np.newaxis, np.newaxis])
     tri_data = tri_data.reshape(-1, 2).T
     shape = (triangles.shape[0], points.shape[0])
     # Row indices: [0, 0, 0, 1, 1, 1, ...]
     row_ind = np.array([[i] * 3 for i in range(len(triangles))]).ravel()
     # Column indices: [t[0,0], t[0,1], t[0,2], t[1,0], t[1,1], t[1,2], ...]
     col_ind = triangles.ravel()
-    Gx = sp.csr_matrix(
+    Gx = sp.csr_array(
         (tri_data[0], (row_ind, col_ind)),
         shape=shape,
         dtype=float,
     )
-    Gy = sp.csr_matrix(
+    Gy = sp.csr_array(
         (tri_data[1], (row_ind, col_ind)),
         shape=shape,
         dtype=float,
     )
     return Gx, Gy
 
 
 def gradient_vertices(
     points: np.ndarray,
     triangles: np.ndarray,
-    triangle_areas: Optional[np.ndarray] = None,
-) -> Tuple[sp.csr_matrix, sp.csr_matrix]:
+    areas: Optional[np.ndarray] = None,
+) -> Tuple[sp.csr_array, sp.csr_array]:
     """Returns the vertex gradient operators ``gx`` and ``gy``.
 
     Given a mesh with ``n`` vertices and ``m`` triangles and a scalar field ``f``
     defined at the mesh vertices, ``gx`` and ``gy`` are shape ``(n, n)`` matrices
     such that ``gx @ f`` and ``gy @ f`` compute the gradients of ``f`` along
     x and y, evaluated at the vertices.
 
     The vertex gradient operators are calculated by averaging the the triangle
     gradient operators over all triangles adjacent to each vertex.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices
         triangles: Shape (m, 3) array of triangle indices
-        triangle_areas: Shape (m, ) array of triangle areas
+        areas: Shape (m, ) array of triangle areas
 
     Returns:
         x and y gradient matrices, both of which have shape ``(n, n)``
     """
-    if triangle_areas is None:
-        triangle_areas = areas(points, triangles)
+    if areas is None:
+        areas = triangle_areas(points, triangles)
     n = points.shape[0]
-    Gx, Gy = gradient_triangles(points, triangles, triangle_areas=triangle_areas)
+    Gx, Gy = gradient_triangles(points, triangles, areas=areas)
     # Use numpy arrays for fast slicing even though the operators are sparse.
     Gx = Gx.toarray()
     Gy = Gy.toarray()
-    gx = np.zeros((n, n), dtype=float)
-    gy = np.zeros((n, n), dtype=float)
+    gx = sp.lil_array((n, n), dtype=float)
+    gy = sp.lil_array((n, n), dtype=float)
     # This loop is difficult to vectorize because different vertices
     # have different numbers of adjacent triangles.
     for i in range(n):
         adjacent_triangles, _ = np.where(np.isin(triangles, i))
         t = adjacent_triangles
         # Weight each triangle adjacent to vertex i by its angle at the vertex.
         vec1 = points[triangles[t, 1]] - points[triangles[t, 0]]
         vec2 = points[triangles[t, 2]] - points[triangles[t, 0]]
         weights = np.arccos(
             np.sum(vec1 * vec2, axis=1)
             / (la.norm(vec1, axis=1) * la.norm(vec2, axis=1))
         )
         weights /= weights.sum()
-        assert (weights > 0).all()
         gx[i, :] = np.einsum("i, ij -> j", weights, Gx[t, :])
         gy[i, :] = np.einsum("i, ij -> j", weights, Gy[t, :])
-    return sp.csr_matrix(gx), sp.csr_matrix(gy)
+    return gx.asformat("csr"), gy.asformat("csr")
+
+
+# def gradient_edges(
+#     points: np.ndarray,
+#     edges: np.ndarray,
+#     edge_lengths: np.ndarray,
+# ) -> sp.csr_array:
+#     """Build the gradient for a function living on the sites onto the edges.
+
+#     Args:
+#         points: Mesh vertex positions
+#         edges: Mesh edge indices.
+#         edge_lengths: Mesh edge lengths.
+
+#     Returns:
+#         The gradient matrix.
+#     """
+#     edge_indices = np.arange(len(edges))
+#     weights = 1 / edge_lengths
+#     rows = np.concatenate([edge_indices, edge_indices])
+#     cols = np.concatenate([edges[:, 1], edges[:, 0]])
+#     values = np.concatenate([weights, -weights])
+#     return sp.csr_array((values, (rows, cols)), shape=(len(edges), len(points)))
```

### Comparing `superscreen-0.8.2/superscreen/fluxoid.py` & `superscreen-0.9.0/superscreen/fluxoid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 
 from .device import Device
 from .solution import Solution
-from .solve import solve
+from .solver import solve
 
 logger = logging.getLogger(__name__)
 
 
 def make_fluxoid_polygons(
     device: Device,
     holes: Optional[Union[List[str], str]] = None,
```

### Comparing `superscreen-0.8.2/superscreen/geometry.py` & `superscreen-0.9.0/superscreen/geometry.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 def path_vectors(path: np.ndarray) -> Tuple[float, np.ndarray]:
     """Computes the total length and the unit normals for a path.
 
     Args:
         path: Shape ``(n, 2)`` array of coordinates representing a continuous path.
 
     Returns:
-        The total path length and an array of of unit vectors normal to
+        The edge lengths and an array of of unit vectors normal to
         each edge in the path.
     """
     dr = np.diff(path, axis=0)
+    # x cross z = -y
+    # y cross z = +x
     normals = np.cross(dr, [0, 0, 1])
     unit_normals = unit_vector(normals)
-    total_length = np.sum(la.norm(dr, axis=1))
+    edge_lengths = la.norm(dr, axis=1)
     unit_normals = np.concatenate([unit_normals, unit_normals[-1:]], axis=0)
-    return total_length, unit_normals[:, :2]
+    return edge_lengths, unit_normals[:, :2]
 
 
 def rotation_matrix(angle_radians: float) -> np.ndarray:
     """Returns a 2D rotation matrix."""
     c = np.cos(angle_radians)
     s = np.sin(angle_radians)
     return np.array([[c, -s], [s, c]])
@@ -122,55 +124,60 @@
         angle=0,
     )
 
 
 def box(
     width: float,
     height: Optional[float] = None,
-    points_per_side: int = 25,
+    points: int = 101,
     center: Tuple[float, float] = (0, 0),
     angle: float = 0,
 ) -> np.ndarray:
     """Returns the coordinates for a rectangle with a given width and height,
     centered at the specified center.
 
     Args:
         width: Width of the rectangle (in the x direction).
         height: Height of the rectangle (in the y direction). If None is given,
             then height is set to width and the function returns a square.
-        points_per_side: Number of points on each side of the box.
+        points: The target number of points making up the box. The actual number of
+            points may be slightly different than this value.
         center: Coordinates of the center of the rectangle.
         angle: Angle (in degrees) by which to rotate counterclockwise about (0, 0)
-            **before** translating to the specified center.
+            **after** translating to the specified center.
 
     Returns:
-        A shape ``(4 * points_per_side, 2)`` array of (x, y) coordinates
+        A shape ``(m, 2)`` or array of (x, y) coordinates.
     """
     width = abs(width)
     if height is None:
         height = width
     height = abs(height)
     x0, y0 = center
+    perimeter = 2 * (width + height)
+    x_points = round(points * width / perimeter)
+    y_points = round(points * height / perimeter)
+
     xs = np.concatenate(
         [
-            width / 2 * np.ones(points_per_side),
-            np.linspace(width / 2, -width / 2, points_per_side),
-            -width / 2 * np.ones(points_per_side),
-            np.linspace(-width / 2, width / 2, points_per_side),
+            width / 2 * np.ones(y_points),
+            np.linspace(width / 2, -width / 2, x_points),
+            -width / 2 * np.ones(y_points),
+            np.linspace(-width / 2, width / 2, x_points),
         ]
     )
     ys = np.concatenate(
         [
-            np.linspace(-height / 2, height / 2, points_per_side),
-            height / 2 * np.ones(points_per_side),
-            np.linspace(height / 2, -height / 2, points_per_side),
-            -height / 2 * np.ones(points_per_side),
+            np.linspace(-height / 2, height / 2, y_points),
+            height / 2 * np.ones(x_points),
+            np.linspace(height / 2, -height / 2, y_points),
+            -height / 2 * np.ones(x_points),
         ]
     )
-    coords = np.stack([xs, ys], axis=1) + np.array([[x0, y0]])
+    coords = np.array([xs, ys]).T + np.array([[x0, y0]])
     if angle:
         coords = rotate(coords, angle)
     return coords
 
 
 def close_curve(points: np.ndarray) -> np.ndarray:
     """Close a curve (making the start point equal to the end point),
@@ -182,7 +189,18 @@
     Returns:
         ``points`` with the first point appended to the end if the start point
         was not already equal to the end point.
     """
     if not np.allclose(points[0], points[-1]):
         points = np.concatenate([points, points[:1]], axis=0)
     return points
+
+
+def ensure_unique(coords: np.ndarray) -> np.ndarray:
+    # Coords is a shape (n, 2) array of vertex coordinates.
+    coords = np.asarray(coords)
+    # Remove duplicate coordinates, otherwise triangle.build() will segfault.
+    # By default, np.unique() does not preserve order, so we have to remove
+    # duplicates this way:
+    _, ix = np.unique(coords, return_index=True, axis=0)
+    coords = coords[np.sort(ix)]
+    return coords
```

### Comparing `superscreen-0.8.2/superscreen/parameter.py` & `superscreen-0.9.0/superscreen/parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,44 +193,44 @@
         if self.func.__code__ != other.func.__code__:
             return False
 
         return self.kwargs == other.kwargs
 
 
 class CompositeParameter(Parameter):
-    """A callable object that behaves like a Parameter
+    """A callable object that behaves like a :class:`superscreen.Parameter`
     (i.e. it computes a scalar or vector quantity as a function of
-    position coordinates x, y, z). A CompositeParameter object is created as
-    a result of mathematical operations between Parameters, CompositeParameters,
-    and/or real numbers.
+    position coordinates x, y, z). A :class:`superscreen.parameter.CompositeParameter`
+    object is created as a result of mathematical operations between ``Parameters``,
+    ``CompositeParameters``, and/or real numbers.
 
     Addition, subtraction, multiplication, division, and exponentiation
-    between Parameters, CompositeParameters and real numbers (ints and floats)
+    between ``Parameters``, ``CompositeParameters`` and real numbers (ints and floats)
     are supported. The result of any of these operations is a new
-    CompositeParameter object.
+    :class:`superscreen.parameter.CompositeParameter` object.
 
     Args:
         left: The object on the left-hand side of the operator.
         right: The object on the right-hand side of the operator.
-        operator_: The operator acting on left and right (or its string representation).
+        op: The operator acting on left and right (or its string representation).
     """
 
     VALID_OPERATORS = {
         operator.add: "+",
         operator.sub: "-",
         operator.mul: "*",
         operator.truediv: "/",
         operator.pow: "**",
     }
 
     def __init__(
         self,
         left: Union[int, float, Parameter, "CompositeParameter"],
         right: Union[int, float, Parameter, "CompositeParameter"],
-        operator_: Union[Callable, str],
+        op: Union[Callable, str],
     ):
         valid_types = (int, float, Parameter, CompositeParameter)
         if not isinstance(left, valid_types):
             raise TypeError(
                 f"Left must be a number, Parameter, or CompositeParameter, "
                 f"not {type(left)!r}."
             )
@@ -239,25 +239,25 @@
                 f"Right must be a number, Parameter, or CompositeParameter, "
                 f"not {type(right)!r}."
             )
         if isinstance(left, (int, float)) and isinstance(right, (int, float)):
             raise TypeError(
                 "Either left or right must be a Parameter or CompositeParameter."
             )
-        if isinstance(operator_, str):
+        if isinstance(op, str):
             operators = {v: k for k, v in self.VALID_OPERATORS.items()}
-            operator_ = operators.get(operator_.strip(), None)
-        if operator_ not in self.VALID_OPERATORS:
+            op = operators.get(op.strip(), None)
+        if op not in self.VALID_OPERATORS:
             raise ValueError(
-                f"Unknown operator, {operator_!r}. "
+                f"Unknown operator, {op!r}. "
                 f"Valid operators are {list(self.VALID_OPERATORS)!r}."
             )
         self.left = left
         self.right = right
-        self.operator = operator_
+        self.operator = op
 
     def __call__(
         self,
         x: Union[int, float, np.ndarray],
         y: Union[int, float, np.ndarray],
         z: Optional[Union[int, float, np.ndarray]] = None,
     ) -> Union[int, float, np.ndarray]:
```

### Comparing `superscreen-0.8.2/superscreen/solution.py` & `superscreen-0.9.0/superscreen/solution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-import json
+import datetime as dt
 import logging
 import os
-import zipfile
-from datetime import datetime
-from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Union
+from contextlib import nullcontext
+from dataclasses import dataclass
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    NamedTuple,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
-import dill
+import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 import pint
 from scipy import interpolate
-from scipy.spatial.distance import cdist
 
 from .about import version_dict
 from .device import Device, Polygon
+from .distance import cdist
 from .fem import in_polygon
+from .geometry import path_vectors
+from .io import deserialize_obj, serialize_obj
 from .parameter import Constant
 from .sources.current import biot_savart_2d
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("solution")
 
-
-class Vortex(NamedTuple):
-    """A vortex located at position ``(x, y)`` in ``layer`` containing
-    a total flux ``nPhi0`` in units of the flux quantum :math:`\\Phi_0`.
-
-    Args:
-        x: Vortex x-position.
-        y: Vortex y-position.
-        layer: The layer in which the vortex is pinned.
-        nPhi0: The number of flux quanta contained in the vortex.
-    """
-
-    x: float
-    y: float
-    layer: str
-    nPhi0: float = 1
+InterpolatorType = Literal["nearest", "linear", "cubic"]
 
 
 class Fluxoid(NamedTuple):
     """The fluxoid for a closed region :math:`S` with boundary :math:`\\partial S`
     is defined as:
 
     .. math::
@@ -57,66 +55,196 @@
         supercurrent_part: :math:`\\oint_{\\partial S}\\mu_0\\Lambda(\\vec{r})\\vec{J}(\\vec{r})\\cdot\\mathrm{d}\\vec{r}`.
     """
 
     flux_part: Union[float, pint.Quantity]
     supercurrent_part: Union[float, pint.Quantity]
 
 
+@dataclass
+class Vortex:
+    """A vortex located at position ``(x, y)`` in ``film`` containing
+    a total flux ``nPhi0`` in units of the flux quantum :math:`\\Phi_0`.
+
+    Args:
+        x: Vortex x-position.
+        y: Vortex y-position.
+        film: The name of the film in which the vortex is pinned.
+        nPhi0: The number of flux quanta contained in the vortex.
+    """
+
+    x: float
+    y: float
+    film: str
+    nPhi0: float = 1
+
+    def to_hdf5(self, h5group: h5py.Group) -> None:
+        h5group.attrs["x"] = self.x
+        h5group.attrs["y"] = self.y
+        h5group.attrs["film"] = self.film
+        h5group.attrs["nPhi0"] = self.nPhi0
+
+    @staticmethod
+    def from_hdf5(h5group: h5py.Group) -> "Vortex":
+        return Vortex(
+            x=h5group.attrs["x"],
+            y=h5group.attrs["y"],
+            film=h5group.attrs["film"],
+            nPhi0=h5group.attrs["nPhi0"],
+        )
+
+
+class FilmSolution:
+    """Raw solution data for a single film.
+
+    Args:
+        stream: The stream function
+        current_density: The sheet current density
+        applied_field: The applied field
+        self_field: The field due to screening currents in the film
+        field_from_other_films: The field due to screening currents in other films
+    """
+
+    def __init__(
+        self,
+        stream: np.ndarray,
+        current_density: np.ndarray,
+        applied_field: np.ndarray,
+        self_field: np.ndarray,
+        field_from_other_films: Optional[np.ndarray] = None,
+    ):
+        self.stream = np.asarray(stream)
+        self.current_density = np.asarray(current_density)
+        self.applied_field = np.asarray(applied_field)
+        self.self_field = np.asarray(self_field)
+        if field_from_other_films is not None:
+            field_from_other_films = np.asarray(field_from_other_films)
+        self.field_from_other_films = field_from_other_films
+        self._total_field: Optional[np.ndarray] = None
+
+    @property
+    def total_field(self) -> np.ndarray:
+        """The total magnetic field in the film."""
+        if self._total_field is None:
+            self._total_field = self.applied_field + self.self_field
+            if self.field_from_other_films is not None:
+                self._total_field += self.field_from_other_films
+        return self._total_field
+
+    def to_hdf5(self, h5group: h5py.Group) -> None:
+        """Save the :class:`superscreen.FilmSolution` to an :class:`h5py.Group`.
+
+        Args:
+            h5group: The :class:`h5py.Group` in which to save the :class:`superscreen.FilmSolution`
+        """
+        h5group["stream"] = self.stream
+        h5group["current_density"] = self.current_density
+        h5group["applied_field"] = self.applied_field
+        h5group["self_field"] = self.self_field
+        if self.field_from_other_films is not None:
+            h5group["field_from_other_films"] = self.field_from_other_films
+
+    @staticmethod
+    def from_hdf5(h5group: h5py.Group) -> "FilmSolution":
+        """Load a :class:`superscreen.FilmSolution` from an :class:`h5py.Group`.
+
+        Args:
+            h5group: The :class:`h5py.Group` from which to load the :class:`superscreen.FilmSolution`
+
+        Returns:
+            The loaded :class:`superscreen.FilmSolution`
+        """
+        field_from_other_films = h5group.get("field_from_other_films", None)
+        if field_from_other_films is not None:
+            field_from_other_films = np.array(field_from_other_films)
+        return FilmSolution(
+            stream=np.array(h5group["stream"]),
+            current_density=np.array(h5group["current_density"]),
+            applied_field=np.array(h5group["applied_field"]),
+            self_field=np.array(h5group["self_field"]),
+            field_from_other_films=field_from_other_films,
+        )
+
+    def is_close(
+        self, other: "FilmSolution", rtol: float = 1e-4, atol: float = 1e-7
+    ) -> bool:
+        """Check whether two FilmSolutions are equal to within a tolerance.
+
+        Args:
+            other: The other FilmSolution
+            rtol: Relative tolerance (see :func:`numpy.allclose`)
+            atol: Absolute tolerance (see :func:`numpy.allclose`)
+
+        Returns:
+            True if the two FilmSolutions are equal within the given tolerances.
+        """
+        kw = dict(rtol=rtol, atol=atol)
+        return (
+            np.allclose(self.stream, other.stream, **kw)
+            and np.allclose(self.applied_field, other.applied_field, **kw)
+            and np.allclose(self.self_field, other.self_field, **kw)
+            and np.allclose(self.total_field, other.total_field, **kw)
+        )
+
+    def __eq__(self, other) -> bool:
+        if other is self:
+            return True
+        if not isinstance(other, FilmSolution):
+            return False
+        if self.field_from_other_films is None:
+            if other.field_from_other_films is not None:
+                return False
+        if other.field_from_other_films is None:
+            if self.field_from_other_films is not None:
+                return False
+        return self.is_close(other)
+
+
 class Solution:
     """A container for the calculated stream functions and fields,
     with some convenient data processing methods.
 
     Args:
         device: The ``Device`` that was solved
-        streams: A dict of ``{layer_name: stream_function}``
-        current_densities: A dict of ``{layer_name: current_density}``
-        fields: A dict of ``{layer_name: total_field}``
-        screening_fields: A dict of ``{layer_name: screening_field}``
-        applied_field: The function defining the applied field
+        film_solutions: A dict of ``{film_name: film_solution}`` containing the raw
+            simulation results in ``field_units``, ``current_units``, and ``device.length_units``.
+        applied_field_func: The function defining the applied field
         field_units: Units of the applied field
         current_units: Units used for current quantities.
         circulating_currents: A dict of ``{hole_name: circulating_current}``.
         terminal_currents: A dict of ``{terminal_name: terminal_current}``.
         vortices: A list of ``Vortex`` objects located in the ``Device``.
         solver: The solver method that generated the solution.
+
     """
 
     def __init__(
         self,
         *,
         device: Device,
-        streams: Dict[str, np.ndarray],
-        current_densities: Dict[str, np.ndarray],
-        fields: Dict[str, np.ndarray],
-        screening_fields: Dict[str, np.ndarray],
-        applied_field: Callable,
+        film_solutions: Dict[str, FilmSolution],
+        applied_field_func: Callable,
         field_units: str,
         current_units: str,
-        circulating_currents: Optional[
-            Dict[str, Union[float, str, pint.Quantity]]
-        ] = None,
-        terminal_currents: Optional[Dict[str, Union[float, str, pint.Quantity]]] = None,
+        circulating_currents: Optional[Dict[str, float]] = None,
+        terminal_currents: Optional[Dict[str, float]] = None,
         vortices: Optional[List[Vortex]] = None,
         solver: str = "superscreen.solve",
     ):
-        self.device = device.copy(with_arrays=True, copy_arrays=False)
-        self.streams = streams
-        self.current_densities = current_densities
-        self.fields = fields
-        self.applied_field = applied_field
-        self.screening_fields = screening_fields
+        self.device = device.copy(with_mesh=True, copy_mesh=False)
+        self.film_solutions = film_solutions
+        self.applied_field_func = applied_field_func
         self.circulating_currents = circulating_currents or {}
         self.terminal_currents = terminal_currents or {}
         self.vortices = vortices or []
         # Make field_units and current_units "read-only" attributes.
         # The should never be changed after instantiation.
         self._field_units = field_units
         self._current_units = current_units
         self._solver = solver
-        self._time_created = datetime.now()
+        self._time_created = dt.datetime.now()
         self._version_info = version_dict()
 
     @property
     def field_units(self) -> str:
         """The units in which magnetic fields are specified."""
         return self._field_units
 
@@ -127,354 +255,254 @@
 
     @property
     def solver(self) -> str:
         """The solver method that generated the solution."""
         return self._solver
 
     @property
-    def time_created(self) -> datetime:
+    def time_created(self) -> dt.datetime:
         """The time at which the solution was originally created."""
         return self._time_created
 
     @property
     def version_info(self) -> Dict[str, str]:
         """A dictionary of dependency versions."""
         return self._version_info
 
-    def grid_data(
-        self,
-        dataset: str,
-        *,
-        layers: Optional[Union[str, List[str]]] = None,
-        grid_shape: Union[int, Tuple[int, int]] = (200, 200),
-        method: str = "linear",
-        with_units: bool = False,
-        **kwargs,
-    ) -> Tuple[np.ndarray, np.ndarray, Dict[str, np.ndarray]]:
-        """Interpolates results from the triangular mesh to a rectangular grid.
+    @staticmethod
+    def _select_interpolator(method: InterpolatorType) -> type:
+        return {
+            "nearest": interpolate.NearestNDInterpolator,
+            "linear": interpolate.LinearNDInterpolator,
+            "cubic": interpolate.CloughTocher2DInterpolator,
+        }[method]
 
-        Keyword arguments are passed to scipy.interpolate.griddata().
-
-        Args:
-            dataset: Name of the dataset to interpolate
-                (one of "streams", "fields", or "screening_fields", "current_densities").
-            layers: Name(s) of the layer(s) for which to interpolate results.
-            grid_shape: Shape of the desired rectangular grid. If a single integer
-                N is given, then the grid will be square, shape = (N, N).
-            method: Interpolation method to use (see scipy.interpolate.griddata).
-            with_units: Whether to return arrays of pint.Quantities with units attached.
-
-        Returns:
-            x grid, y grid, dict of interpolated data for each layer
-        """
-        valid_data = ("streams", "fields", "screening_fields", "current_densities")
-        if dataset not in valid_data:
-            raise ValueError(f"Expected one of {', '.join(valid_data)}, not {dataset}.")
-        if dataset == "current_densities":
-            return self.grid_current_density(
-                layers=layers,
-                grid_shape=grid_shape,
-                method=method,
-                with_units=with_units,
-                **kwargs,
-            )
-        datasets = getattr(self, dataset)
-
-        if isinstance(layers, str):
-            layers = [layers]
-        if layers is None:
-            layers = list(self.device.layers)
-        else:
-            for layer in layers:
-                if layer not in self.device.layers:
-                    raise ValueError(f"Unknown layer, {layer}.")
-
-        if isinstance(grid_shape, int):
-            grid_shape = (grid_shape, grid_shape)
-        if not isinstance(grid_shape, (tuple, list)) or len(grid_shape) != 2:
-            raise TypeError(
-                f"Expected a tuple of length 2, but got {grid_shape} "
-                f"({type(grid_shape)})."
-            )
-
-        points = self.device.points
-        x = points[:, 0]
-        y = points[:, 1]
-        xgrid, ygrid = np.meshgrid(
-            np.linspace(x.min(), x.max(), grid_shape[1]),
-            np.linspace(y.min(), y.max(), grid_shape[0]),
-        )
-        zgrids = {}
-        for name, array in datasets.items():
-            if name in layers:
-                zgrid = interpolate.griddata(
-                    points, array, (xgrid, ygrid), method=method, **kwargs
-                )
-                zgrids[name] = zgrid
-        if with_units:
-            xgrid = xgrid * self.device.ureg(self.device.length_units)
-            ygrid = ygrid * self.device.ureg(self.device.length_units)
-            if dataset in ("fields", "screening_fields"):
-                units = self.field_units
-            else:
-                units = self.current_units
-            zgrids = {
-                layer: data * self.device.ureg(units) for layer, data in zgrids.items()
-            }
-        return xgrid, ygrid, zgrids
-
-    def grid_current_density(
+    def interp_current_density(
         self,
+        positions: np.ndarray,
         *,
-        layers: Optional[Union[str, List[str]]] = None,
-        grid_shape: Union[int, Tuple[int, int]] = (200, 200),
-        method: str = "linear",
+        film: str,
+        method: InterpolatorType = "linear",
         units: Optional[str] = None,
         with_units: bool = False,
         **kwargs,
-    ) -> Tuple[np.ndarray, np.ndarray, Dict[str, np.ndarray]]:
-        """Computes the current density ``J = [dg/dy, -dg/dx]`` on a rectangular grid.
+    ) -> np.ndarray:
+        """Interpolates the current density ``J = [dg/dy, -dg/dx]`` within a film.
 
-        Keyword arguments are passed to scipy.interpolate.griddata().
+        Additional keyword arguments are passed to the relevant interpolator:
+        :class:`scipy.interpolate.NearestNDInterpolator`,
+        :class:`scipy.interpolate.LinearNDInterpolator`, or
+        :class:`scipy.interpolate.CloughTocher2DInterpolator`.
 
         Args:
-            layers: Name(s) of the layer(s) for which to interpolate current density.
-            grid_shape: Shape of the desired rectangular grid. If a single integer
-                N is given, then the grid will be square, shape = (N, N).
-            method: Interpolation method to use (see scipy.interpolate.griddata).
+            positions: Shape ``(m, 2)`` array of x, y coordinates at which to evaluate
+                the current density.
+            film: The name of the film in which to interpolate current density.
+            method: Interpolation method to use ("nearest", "linear" or "cubic").
             units: The desired units for the current density. Defaults to
                 ``self.current_units / self.device.length_units``.
             with_units: Whether to return arrays of pint.Quantities with units attached.
 
         Returns:
-            x grid, y grid, dict of interpolated current density for each layer
+            The interpolated current density
         """
-        xgrid, ygrid, streams = self.grid_data(
-            dataset="streams",
-            layers=layers,
-            grid_shape=grid_shape,
-            method=method,
-            with_units=True,
-            **kwargs,
-        )
-        units = units or f"{self.current_units} / {self.device.length_units}"
-        Js = {}
-        for layer, g in streams.items():
-            # J = [dg/dy, -dg/dx]
-            # y is axis 0 (rows), x is axis 1 (columns)
-            dg_dy, dg_dx = np.gradient(
-                g.magnitude, ygrid[:, 0].magnitude, xgrid[0, :].magnitude
-            )
-            J = (np.array([dg_dy, -dg_dx]) * g.units / xgrid.units).to(units)
-            if not with_units:
-                J = J.magnitude
-            Js[layer] = J
-        if not with_units:
-            xgrid = xgrid.magnitude
-            ygrid = ygrid.magnitude
-        return xgrid, ygrid, Js
+        device = self.device
+        default_units = f"{self.current_units} / {device.length_units}"
+        if units is None:
+            units = default_units
+        positions = np.atleast_2d(positions)
+        interpolator = self._select_interpolator(method)
+        xy = device.meshes[film].sites
+        J = self.film_solutions[film].current_density
+        Jx_interp = interpolator(xy, J[:, 0], **kwargs)
+        Jy_interp = interpolator(xy, J[:, 1], **kwargs)
+        J = np.stack([Jx_interp(positions), Jy_interp(positions)], axis=1)
+        in_film = device.films[film].contains_points(positions)
+        J[~in_film] = 0
+        J[~np.isfinite(J).all(axis=1)] = 0
+        J = (J * self.device.ureg(default_units)).to(units)
+        if with_units:
+            return J
+        return J.magnitude
 
-    def interp_current_density(
+    def current_through_path(
         self,
-        positions: np.ndarray,
+        path_coords: np.ndarray,
         *,
-        layers: Optional[Union[str, List[str]]] = None,
-        grid_shape: Union[int, Tuple[int, int]] = (200, 200),
-        method: str = "linear",
-        units: Optional[str] = None,
-        with_units: bool = False,
-        **kwargs,
-    ):
-        """Computes the current density ``J = [dg/dy, -dg/dx]``
-        at unstructured coordinates via interpolation.
-
-        Keyword arguments are passed to scipy.interpolate.griddata().
+        film: str,
+        interp_method: str = "linear",
+        units: Union[str, None] = None,
+        with_units: bool = True,
+    ) -> Union[float, pint.Quantity]:
+        """Calculates the total current crossing a given path.
 
         Args:
-            positions: Shape ``(m, 2)`` array of x, y coordinates at which to evaluate
-                the current density.
-            layers: Name(s) of the layer(s) for which to interpolate current density.
-            grid_shape: Shape of the desired rectangular grid. If a single integer
-                N is given, then the grid will be square, shape = (N, N).
-            method: Interpolation method to use (see scipy.interpolate.griddata).
-            units: The desired units for the current density. Defaults to
-                ``self.current_units / self.device.length_units``.
-            with_units: Whether to return arrays of pint.Quantities with units attached.
+            path_coords: An ``(n, 2)`` array of ``(x, y)`` coordinates defining
+                the path.
+            film: The name of the film in which to interpolate current density.
+            interp_method: Interpolation method to use ("nearest", "linear" or "cubic").
+            units: The current units to return.
+            with_units: Whether to return a :class:`pint.Quantity` with units attached.
 
         Returns:
-            A dict of interpolated current density for each layer.
+            The total current crossing the path as either a float or a
+            :class:`pint.Quantity`.
         """
-        valid_methods = ("nearest", "linear", "cubic")
-        if method not in valid_methods:
-            raise ValueError(
-                f"Interpolation method must be one of {valid_methods} (got {method})."
-            )
-        if method == "nearest":
-            interpolator = interpolate.NearestNDInterpolator
-            interp_kwargs = dict()
-        elif method == "linear":
-            interpolator = interpolate.LinearNDInterpolator
-            interp_kwargs = dict(fill_value=0)
-        else:  # "cubic"
-            interpolator = interpolate.CloughTocher2DInterpolator
-            interp_kwargs = dict(fill_value=0)
+        device = self.device
         if units is None:
-            units = f"{self.current_units} / {self.device.length_units}"
-        positions = np.atleast_2d(positions)
-        xgrid, ygrid, Jgrids = self.grid_current_density(
-            layers=layers,
-            grid_shape=grid_shape,
-            method=method,
-            units=units,
-            with_units=False,
-            **kwargs,
+            units = self.current_units
+        # The center of each edge in the path
+        edge_positions = (path_coords[:-1] + path_coords[1:]) / 2
+        # Evaluate the supercurrent at the edge centers
+        J_edge = self.interp_current_density(
+            edge_positions,
+            film=film,
+            method=interp_method,
+            with_units=True,
         )
-        xy = np.stack([xgrid.ravel(), ygrid.ravel()], axis=1)
-        interpolated_Js = {}
-        for layer, (Jx, Jy) in Jgrids.items():
-            Jx_interp = interpolator(xy, Jx.ravel(), **interp_kwargs)
-            Jy_interp = interpolator(xy, Jy.ravel(), **interp_kwargs)
-            J = np.stack([Jx_interp(positions), Jy_interp(positions)], axis=1)
-            J[~np.isfinite(J)] = 0
-            if with_units:
-                J = J * self.device.ureg(units)
-            interpolated_Js[layer] = J
-        return interpolated_Js
+        edge_lengths, unit_normals = path_vectors(path_coords)
+        edge_lengths = edge_lengths * device.ureg(device.length_units)
+        J_dot_n = (J_edge * unit_normals[:-1]).sum(axis=1)
+        total_current = np.trapz(J_dot_n * edge_lengths).to(units)
+        if not with_units:
+            total_current = total_current.magnitude
+        return total_current
 
-    def interp_fields(
+    def interp_field(
         self,
         positions: np.ndarray,
         *,
-        layers: Optional[Union[str, List[str]]] = None,
-        method: str = "linear",
+        film: str,
+        dataset: Literal[
+            "field", "self_field", "applied_field", "field_from_other_films"
+        ] = "field",
+        method: InterpolatorType = "linear",
         units: Optional[str] = None,
         with_units: bool = False,
         **kwargs,
     ):
-        """Interpolates the fields in one or more layers.
+        """Interpolates the z-component of the field within a film.
 
         Additional keyword arguments are passed to the relevant interpolator:
-        :class``scipy.interpolate.NearestNDInterpolator`,
+        :class:`scipy.interpolate.NearestNDInterpolator`,
         :class:`scipy.interpolate.LinearNDInterpolator`, or
         :class:`scipy.interpolate.CloughTocher2DInterpolator`.
 
         Args:
             positions: Shape ``(m, 2)`` array of x, y coordinates at which to evaluate
                 the fields.
-            layers: Name(s) of the layer(s) for which to interpolate fields.
+            film: The name of the film in which to interpolate the field.
+            dataset: The dataset to interpolate. One of 'field', 'self_field',
+                'applied_field', or 'field_from_other_films'.
             method: Interpolation method to use: 'nearest', 'linear', or 'cubic'.
             units: The desired units for the current density. Defaults to
                 ``self.field_units``.
             with_units: Whether to return arrays of pint.Quantities with units attached.
 
         Returns:
-            A dict of interpolated fields for each layer.
+            The interpolated field
         """
-        from .solve import convert_field
+        from .solver import convert_field
 
-        valid_methods = ("nearest", "linear", "cubic")
-        if method not in valid_methods:
-            raise ValueError(
-                f"Interpolation method must be one of {valid_methods} (got {method})."
-            )
-        if method == "nearest":
-            interpolator = interpolate.NearestNDInterpolator
-        elif method == "linear":
-            interpolator = interpolate.LinearNDInterpolator
-        else:  # "cubic"
-            interpolator = interpolate.CloughTocher2DInterpolator
+        interpolator = self._select_interpolator(method)
         device = self.device
         if units is None:
             units = self.field_units
-        if layers is None:
-            layers = list(device.layers)
-        positions = np.atleast_2d(positions)
-        interpolated_fields = {}
-        for layer, field in self.fields.items():
-            if layer not in layers:
-                continue
-            Hz_interp = interpolator(device.points, field, **kwargs)
-            Hz = convert_field(
-                Hz_interp(positions),
-                units,
-                old_units=self.field_units,
-                ureg=device.ureg,
-                with_units=with_units,
+        valid_datasets = (
+            "field",
+            "self_field",
+            "applied_field",
+            "field_from_other_films",
+        )
+        points = self.device.meshes[film].sites
+        if dataset not in valid_datasets:
+            raise ValueError(
+                f"Invalid dataset: {dataset!r}. Expected one of {valid_datasets!r}"
             )
-            interpolated_fields[layer] = Hz
-        return interpolated_fields
+        if dataset == "field":
+            field = self.film_solutions[film].total_field
+        elif dataset == "self_field":
+            field = self.film_solutions[film].self_field
+        elif dataset == "applied_field":
+            field = self.film_solutions[film].applied_field
+        else:
+            field = self.film_solutions[film].field_from_other_films
+            if field is None:
+                field = np.zeros(len(points))
+        positions = np.atleast_2d(positions)
+        Hz_interp = interpolator(points, field, **kwargs)
+        Hz = convert_field(
+            Hz_interp(positions),
+            units,
+            old_units=self.field_units,
+            ureg=device.ureg,
+            with_units=with_units,
+        )
+        return Hz
 
     def polygon_flux(
         self,
-        *,
-        polygons: Optional[Union[str, List[str]]] = None,
+        name: str,
         units: Optional[Union[str, pint.Unit]] = None,
         with_units: bool = True,
     ) -> Dict[str, Union[float, pint.Quantity]]:
-        """Computes the flux through all polygons (films, holes, and flux regions)
-        by integrating the calculated fields.
+        """Computes the flux through a given polygon.
 
         Args:
-            polygons: Name(s) of the polygon(s) for which to compute the flux.
-                Default: All polygons.
+            name: The name of the polygon for which to compute the flux.
             units: The flux units to use.
-            with_units: Whether to a dict of pint.Quantities with units attached.
+            with_units: Whether to a return a pint.Quantity with units attached.
 
         Returns:
-            A dict of ``{polygon_name: polygon_flux}``
+            The polygon flux.
         """
-        from .solve import convert_field
+        from .solver import convert_field
 
-        films = list(self.device.films)
-        holes = list(self.device.holes)
-        abstract_regions = list(self.device.abstract_regions)
-        all_polygons = films + holes + abstract_regions
-
-        if isinstance(polygons, str):
-            polygons = [polygons]
-        if polygons is None:
-            polygons = all_polygons
-        else:
-            for poly in polygons:
-                if poly not in all_polygons:
-                    raise ValueError(f"Unknown polygon, {poly}.")
+        device = self.device
+        ureg = device.ureg
+        polygons = {p.name: p for p in device.get_polygons(include_terminals=False)}
+        if name not in polygons:
+            raise ValueError(f"Unknown polygon: {name!r}.")
 
-        ureg = self.device.ureg
-        new_units = units or f"{self.field_units} * {self.device.length_units}**2"
+        new_units = units or f"{self.field_units} * {device.length_units}**2"
         if isinstance(new_units, str):
             new_units = ureg(new_units)
-
-        points = self.device.points
-        areas = self.device.weights * ureg(f"{self.device.length_units}") ** 2
-        fluxes = {}
-        for name in polygons:
-            if name in films:
-                poly = self.device.films[name]
-            elif name in holes:
-                poly = self.device.holes[name]
-            else:
-                poly = self.device.abstract_regions[name]
-            ix = poly.contains_points(points, index=True)
-            field = self.fields[poly.layer][ix] * ureg(self.field_units)
-            area = areas[ix]
-            # Convert field to B = mu0 * H
-            field = convert_field(field, "mT", ureg=ureg)
-            flux = np.einsum("i, i -> ", field, area).to(new_units)
-            if with_units:
-                fluxes[name] = flux
-            else:
-                fluxes[name] = flux.magnitude
-        return fluxes
+        polygon = polygons[name]
+        if name in device.films:
+            mesh = device.meshes[name]
+            polygon_name = name
+        else:
+            for film in device.films.values():
+                if (
+                    film.layer == polygon.layer
+                    and film.contains_points(polygon.points).all()
+                ):
+                    break
+            mesh = device.meshes[film.name]
+            polygon_name = film.name
+        points = mesh.sites
+        areas = mesh.vertex_areas * ureg(f"{self.device.length_units}") ** 2
+        total_field = self.film_solutions[polygon_name].total_field
+
+        ix = polygon.contains_points(points, index=True)
+        field = total_field[ix] * ureg(self.field_units)
+        area = areas[ix]
+        # Convert field to B = mu0 * H
+        field = convert_field(field, "mT", ureg=ureg)
+        flux = np.einsum("i, i -> ", field, area).to(new_units)
+        if with_units:
+            return flux
+        return flux.magnitude
 
     def polygon_fluxoid(
         self,
-        polygon_points: np.ndarray,
-        layers: Optional[Union[str, List[str]]] = None,
-        grid_shape: Union[int, Tuple[int, int]] = (200, 200),
-        interp_method: str = "linear",
+        polygon_coords: Union[np.ndarray, Polygon],
+        *,
+        film: str,
+        interp_method: InterpolatorType = "linear",
         units: Optional[str] = "Phi_0",
         with_units: bool = True,
     ) -> Dict[str, Fluxoid]:
         """Computes the :class:`Fluxoid` (flux + supercurrent) for
         a given polygonal region.
 
         The fluxoid for a closed region :math:`S` with boundary :math:`\\partial S`
@@ -487,258 +515,342 @@
             }_{\\text{flux part}}
             + \\underbrace{
                 \\oint_{\\partial S}
                 \\mu_0\\Lambda(\\vec{r})\\vec{J}(\\vec{r})\\cdot\\mathrm{d}\\vec{r}
             }_{\\text{supercurrent part}}
 
         Args:
-            polygon_points: A shape ``(n, 2)`` array of ``(x, y)`` coordinates of
-                polygon vertices defining the closed region :math:`S`.
-            layers: Name(s) of the layer(s) for which to compute the fluxoid.
-            grid_shape: Shape of the desired rectangular grid to use for interpolation.
-                If a single integer N is given, then the grid will be square,
-                shape = (N, N).
+            polygon_coords: A shape ``(n, 2)`` array of ``(x, y)`` coordinates of
+                polygon vertices defining the closed region :math:`S`,
+                or a :class:`Polygon` instance.
+            film: The name of the film in which to evaluate the field and current.
             interp_method: Interpolation method to use.
             units: The desired units for the current density.
                 Defaults to :math:`\\Phi_0`.
             with_units: Whether to return values as pint.Quantities with units attached.
 
         Returns:
-            A dict of ``{layer_name: fluxoid}`` for each specified layer, where
-            ``fluxoid`` is an instance of :class:`Fluxoid`.
+            The :class:`Fluxoid` for the given polygon.
         """
         device = self.device
         ureg = device.ureg
-        if layers is None:
-            layers = list(device.layers)
-        if isinstance(layers, str):
-            layers = [layers]
         if units is None:
             units = f"{self.field_units} * {self.device.length_units} ** 2"
-        polygon = Polygon(
-            name="__polygon",
-            layer=layers[0],
-            points=polygon_points,
-        )
+        polygon = Polygon(points=polygon_coords)
         points = polygon.points
-        if not any(
-            film.contains_points(points).all() for film in device.films.values()
-        ):
+
+        if not device.films[film].contains_points(points).all():
             raise ValueError(
-                "The polygon must lie completely within a superconducting film."
+                f"The polygon is not contained within the film ({film!r})."
             )
 
+        poly_mesh = device.meshes[film]
+        ix = polygon.contains_points(poly_mesh.sites)
+        fields = self.film_solutions[film].total_field * ureg(self.field_units)
+        areas = poly_mesh.vertex_areas * ureg(f"{device.length_units} ** 2")
+        flux_part = np.einsum("i, i ->", fields[ix], areas[ix]).to(units)
+
         # Evaluate the supercurrent density at the polygon coordinates.
         J_units = f"{self.current_units} / {device.length_units}"
-        J_polys = self.interp_current_density(
+        J_poly = self.interp_current_density(
             points,
-            grid_shape=grid_shape,
-            layers=layers,
+            film=film,
             method=interp_method,
             units=J_units,
             with_units=False,
         )
-
-        old_regions = device.abstract_regions
-        temp_regions = old_regions.copy()
-        temp_regions[polygon.name] = polygon
-        fluxoids = {}
-        for layer in layers:
-            # Compute the flux part of the fluxoid:
-            # \int_{poly} \mu_0 H_z(x, y) dx dy
-            try:
-                polygon.layer = layer
-                device.abstract_regions = temp_regions
-                flux_part = self.polygon_flux(
-                    polygons=polygon.name,
-                    units=units,
-                    with_units=True,
-                )[polygon.name]
-            finally:
-                device.abstract_regions = old_regions
-
-            # Compute the supercurrent part of the fluxoid:
-            # \oint_{\\partial poly} \mu_0\Lambda \vec{J}\cdot\mathrm{d}\vec{r}
-            J_poly = J_polys[layer]
-            Lambda = device.layers[layer].Lambda
-            if not callable(Lambda):
-                Lambda = Constant(Lambda)
-            Lambda_poly = Lambda(points[:, 0], points[:, 1])
-            # \oint_{poly}\Lambda\vec{J}\cdot\mathrm{d}\vec{r}
-            dl = np.diff(points, axis=0)
-            int_J = np.trapz(Lambda_poly[:-1] * np.sum(J_poly[:-1] * dl, axis=1))
-            int_J = int_J * ureg(J_units) * ureg(device.length_units) ** 2
-            supercurrent_part = (ureg("mu_0") * int_J).to(units)
-            if not with_units:
-                flux_part = flux_part.magnitude
-                supercurrent_part = supercurrent_part.magnitude
-            fluxoids[layer] = Fluxoid(flux_part, supercurrent_part)
-        return fluxoids
+        # Compute the supercurrent part of the fluxoid:
+        # \oint_{\\partial poly} \mu_0\Lambda \vec{J}\cdot\mathrm{d}\vec{r}
+        Lambda = device.layers[device.films[film].layer].Lambda
+        if not callable(Lambda):
+            Lambda = Constant(Lambda)
+        Lambda_poly = Lambda(points[:, 0], points[:, 1])
+        # \oint_{poly}\Lambda\vec{J}\cdot\mathrm{d}\vec{r}
+        dl = np.diff(points, axis=0)
+        int_J = np.trapz(Lambda_poly[:-1] * np.sum(J_poly[:-1] * dl, axis=1))
+        int_J = int_J * ureg(J_units) * ureg(device.length_units) ** 2
+        supercurrent_part = (ureg("mu_0") * int_J).to(units)
+        if not with_units:
+            flux_part = flux_part.magnitude
+            supercurrent_part = supercurrent_part.magnitude
+        return Fluxoid(flux_part, supercurrent_part)
 
     def hole_fluxoid(
         self,
         hole_name: str,
         points: Optional[np.ndarray] = None,
-        grid_shape: Union[int, Tuple[int, int]] = (200, 200),
-        interp_method: str = "linear",
+        interp_method: InterpolatorType = "linear",
         units: Optional[str] = "Phi_0",
         with_units: bool = True,
     ) -> Fluxoid:
         """Calculcates the fluxoid for a polygon enclosing the specified hole.
 
         Args:
             hole_name: The name of the hole for which to calculate the fluxoid.
             points: The vertices of the polygon enclosing the hole. If None is given,
                 a polygon is generated using
                 :func:`supercreen.fluxoid.make_fluxoid_polygons`.
-            grid_shape: Shape of the desired rectangular grid to use for interpolation.
-                If a single integer N is given, then the grid will be square,
-                shape = (N, N).
             interp_method: Interpolation method to use.
             units: The desired units for the current density.
                 Defaults to :math:`\\Phi_0`.
             with_units: Whether to return values as pint.Quantities with units attached.
 
         Returns:
             The hole's Fluxoid.
         """
         if points is None:
             from .fluxoid import make_fluxoid_polygons
 
             points = make_fluxoid_polygons(self.device, holes=hole_name)[hole_name]
-        hole = self.device.holes[hole_name]
+
+        device = self.device
+        hole = device.holes[hole_name]
+
         if not in_polygon(points, hole.points).all():
             raise ValueError(
-                f"Hole {hole_name} is not completely enclosed by the given polygon."
+                f"Hole {hole.name} is not completely enclosed by the given polygon."
             )
-        fluxoids = self.polygon_fluxoid(
+        for film_name, holes in self.device.holes_by_film().items():
+            if hole.name in [h.name for h in holes]:
+                break
+        return self.polygon_fluxoid(
             points,
-            hole.layer,
-            grid_shape=grid_shape,
+            film=film_name,
             interp_method=interp_method,
             units=units,
             with_units=with_units,
         )
-        return fluxoids[hole.layer]
 
-    def field_at_position(
+    def screening_field_at_position(
         self,
         positions: np.ndarray,
         *,
-        zs: Optional[Union[float, np.ndarray]] = None,
+        zs: Union[float, np.ndarray, None] = None,
         vector: bool = False,
+        interp_method: InterpolatorType = "linear",
         units: Optional[str] = None,
         with_units: bool = True,
         return_sum: bool = True,
     ) -> Union[np.ndarray, Dict[str, np.ndarray]]:
-        """Calculates the field due to currents in the device at any point(s) in space.
+        """Calculates the field due to currents in the device at any point(s) in space
+        (excluding the applied field).
 
         Args:
             positions: Shape (m, 2) array of (x, y) coordinates, or (m, 3) array
                 of (x, y, z) coordinates at which to calculate the magnetic field.
                 A single sequence like [x, y] or [x, y, z] is also allowed.
             zs: z coordinates at which to calculate the field. If positions has shape
                 (m, 3), then this argument is not allowed. If zs is a scalar, then
                 the fields are calculated in a plane parallel to the x-y plane.
                 If zs is any array, then it must be same length as positions.
             vector: Whether to return the full vector magnetic field
                 or just the z component.
+            interp_method: Interpolation method to use.
             units: Units to which to convert the fields (can be either magnetic field H
                 or magnetic flux density B = mu0 * H). If not given, then the fields
                 are returned in units of ``self.field_units``.
             with_units: Whether to return the fields as ``pint.Quantity``
                 with units attached.
             return_sum: Whether to return the sum of the fields from all layers in
                 the device, or a dict of ``{layer_name: field_from_layer}``.
 
         Returns:
             An np.ndarray if return_sum is True, otherwise a dict of
-            ``{layer_name: field_from_layer}``. If with_units is True, then the
-            array(s) will contain pint.Quantities. ``field_from_layer`` will have
+            ``{film_name: field_from_film}``. If with_units is True, then the
+            array(s) will contain pint.Quantities. ``field_from_film`` will have
             shape ``(m, )`` if vector is False, or shape ``(m, 3)`` if ``vector`` is True.
         """
-        from .solve import convert_field
+        from .solver import convert_field
 
         device = self.device
         dtype = device.solve_dtype
         ureg = device.ureg
-        points = device.points.astype(dtype, copy=False)
+        layers = device.layers
+        meshes = device.meshes
         units = units or self.field_units
         # In case something like a list [x, y] or [x, y, z] is given
         positions = np.atleast_2d(positions)
         # If positions includes z coordinates, peel those off here
         if positions.shape[1] == 3:
             if zs is not None:
                 raise ValueError(
                     "If positions has shape (m, 3) then zs cannot be specified."
                 )
             zs = positions[:, 2]
             positions = positions[:, :2]
-        elif isinstance(zs, (int, float, np.generic)):
-            # constant zs
-            zs = zs * np.ones(positions.shape[0], dtype=dtype)
-        zs = zs.squeeze()
+        else:
+            zs = np.squeeze(zs)
+            if zs.ndim == 0:
+                zs = zs.item() * np.ones(positions.shape[0], dtype=dtype)
         if not isinstance(zs, np.ndarray):
             raise ValueError(f"Expected zs to be an ndarray, but got {type(zs)}.")
-        Hz_applied = self.applied_field(
-            positions[:, 0], positions[:, 1], zs[:, np.newaxis]
-        )
-        if vector:
-            zeros = np.zeros_like(Hz_applied)
-            H_applied = np.stack([zeros, zeros, Hz_applied], axis=1)
-        else:
-            H_applied = Hz_applied
-        H_applied = convert_field(
-            H_applied,
-            units,
-            old_units=self.field_units,
-            ureg=ureg,
-            with_units=with_units,
-        )
+
         fields = {}
-        # Compute the fields at the specified positions from the currents in each layer
-        for name, layer in device.layers.items():
-            if np.all((zs - layer.z0) == 0):
-                H = np.zeros_like(H_applied)
-                for film in device.films.values():
-                    if film.layer == name and film.contains_points(positions).any():
-                        raise ValueError(
-                            "Use Solution.interp_fields() to interpolate "
-                            "fields within a layer."
-                        )
-            else:
-                H = biot_savart_2d(
-                    positions[:, 0],
-                    positions[:, 1],
-                    zs,
-                    positions=points,
-                    areas=device.weights,
-                    current_densities=self.current_densities[name],
-                    z0=layer.z0,
-                    length_units=device.length_units,
-                    current_units=self.current_units,
-                    vector=vector,
+        shape = (len(positions),)
+        if vector:
+            shape = shape + (3,)
+            zeros = np.zeros(len(positions), dtype=dtype)
+        # Compute the fields at the specified positions from the currents in each film
+        for name, film in device.films.items():
+            layer = layers[film.layer]
+            field_from_film = np.zeros(len(positions), dtype=dtype)
+            in_film = np.zeros(len(positions), dtype=bool)
+            if np.all(zs == layer.z0):
+                # Evaluate the screening field within a film.
+                in_film[film.contains_points(positions)] = True
+                field_in_film = self.interp_field(
+                    positions[in_film],
+                    film=film.name,
+                    dataset="self_field",
+                    method=interp_method,
+                    units="tesla",
+                    with_units=False,
                 )
+                if vector:
+                    # Make shape (m, 3)
+                    field_in_film = np.array([zeros, zeros, field_in_film]).T
+                field_from_film[in_film] = field_in_film
+            # Evaluate the screening field outside of any films.
+            not_in_film = ~in_film
+            field_from_film[not_in_film] = biot_savart_2d(
+                positions[not_in_film, 0],
+                positions[not_in_film, 1],
+                zs[not_in_film],
+                positions=meshes[name].sites,
+                areas=meshes[name].vertex_areas,
+                current_densities=self.film_solutions[name].current_density,
+                z0=layer.z0,
+                length_units=device.length_units,
+                current_units=self.current_units,
+                vector=vector,
+            )
             fields[name] = convert_field(
-                H,
+                field_from_film,
                 units,
                 old_units="tesla",
                 ureg=ureg,
                 with_units=with_units,
             )
-        fields["applied_field"] = np.atleast_1d(H_applied).squeeze()
+        if return_sum:
+            return sum(fields.values())
+        return fields
+
+    def field_at_position(
+        self,
+        positions: np.ndarray,
+        *,
+        zs: Union[float, np.ndarray, None] = None,
+        interp_method: InterpolatorType = "linear",
+        units: Optional[str] = None,
+        with_units: bool = True,
+        return_sum: bool = True,
+    ) -> Union[np.ndarray, Dict[str, np.ndarray]]:
+        """Calculates the field due to currents in the device at any point(s) in space.
+
+        Args:
+            positions: Shape (m, 2) array of (x, y) coordinates, or (m, 3) array
+                of (x, y, z) coordinates at which to calculate the magnetic field.
+                A single sequence like [x, y] or [x, y, z] is also allowed.
+            zs: z coordinates at which to calculate the field. If positions has shape
+                (m, 3), then this argument is not allowed. If zs is a scalar, then
+                the fields are calculated in a plane parallel to the x-y plane.
+                If zs is any array, then it must be same length as positions.
+            interp_method: Interpolation method to use.
+            units: Units to which to convert the fields (can be either magnetic field H
+                or magnetic flux density B = mu0 * H). If not given, then the fields
+                are returned in units of ``self.field_units``.
+            with_units: Whether to return the fields as ``pint.Quantity``
+                with units attached.
+            return_sum: Whether to return the sum of the fields from all layers in
+                the device, or a dict of ``{layer_name: field_from_layer}``.
+
+        Returns:
+            An np.ndarray if return_sum is True, otherwise a dict of
+            ``{film_name: field_from_film}``. If with_units is True, then the
+            array(s) will contain pint.Quantities.
+        """
+        from .solver.utils import convert_field
+
+        device = self.device
+        dtype = device.solve_dtype
+        units = units or self.field_units
+        # In case something like a list [x, y] or [x, y, z] is given
+        positions = np.atleast_2d(positions)
+        # If positions includes z coordinates, peel those off here
+        if positions.shape[1] == 3:
+            if zs is not None:
+                raise ValueError(
+                    "If positions has shape (m, 3) then zs cannot be specified."
+                )
+            zs = positions[:, 2]
+            positions = positions[:, :2]
+        else:
+            zs = np.squeeze(zs)
+            if zs.ndim == 0:
+                zs = zs.item() * np.ones(positions.shape[0], dtype=dtype)
+        if not isinstance(zs, np.ndarray):
+            raise ValueError(f"Expected zs to be an ndarray, but got {type(zs)}.")
+        # Evaluate the screening fields
+        fields = self.screening_field_at_position(
+            positions,
+            zs=zs,
+            vector=False,
+            interp_method=interp_method,
+            units=self.field_units,
+            with_units=False,
+            return_sum=False,
+        )
+        # Evaluate the applied fields
+        films_by_layer = device.polygons_by_layer("film")
+        Hz_applied = np.zeros(len(positions), dtype=dtype)
+        in_film = np.zeros(len(positions), dtype=bool)
+        for name, layer in device.layers.items():
+            if np.all(zs == layer.z0):
+                for film in films_by_layer[name]:
+                    ix = film.contains_points(positions)
+                    in_film[ix] = True
+                    Hz_applied[ix] = self.interp_field(
+                        positions[ix],
+                        film=film.name,
+                        dataset="applied_field",
+                        method=interp_method,
+                        units=self.field_units,
+                        with_units=False,
+                    )
+                    Hz_applied[ix] += self.interp_field(
+                        positions[ix],
+                        film=film.name,
+                        dataset="field_from_other_films",
+                        method=interp_method,
+                        units=self.field_units,
+                        with_units=False,
+                    )
+                break
+        mask = ~in_film
+        Hz_applied[mask] = self.applied_field_func(
+            positions[mask, 0], positions[mask, 1], zs[mask, np.newaxis]
+        )
+        fields["applied_field"] = np.atleast_1d(Hz_applied).squeeze()
+        for key, field in fields.items():
+            fields[key] = convert_field(
+                field,
+                units,
+                old_units=self.field_units,
+                ureg=device.ureg,
+                with_units=with_units,
+            )
         if return_sum:
             return sum(fields.values())
         return fields
 
     def vector_potential_at_position(
         self,
         positions: np.ndarray,
         *,
-        zs: Optional[Union[float, np.ndarray]] = None,
+        zs: Union[float, np.ndarray, None] = None,
         units: Optional[str] = None,
         with_units: bool = True,
         return_sum: bool = True,
     ) -> Union[np.ndarray, Dict[str, np.ndarray]]:
         """Calculates the vector potential due to currents in the device at any
         point(s) in space. Note that this only considers the vector potential
         due to currents in the device, so only represents the total vector potential
@@ -766,207 +878,223 @@
             with_units: Whether to return the vector potential as a ``pint.Quantity``
                 with units attached.
             return_sum: Whether to return the sum of the potential from all layers in
                 the device, or a dict of ``{layer_name: potential_from_layer}``.
 
         Returns:
             An np.ndarray if return_sum is True, otherwise a dict of
-            ``{layer_name: potential_from_layer}``. If with_units is True, then the
-            array(s) will contain pint.Quantities. ``potential_from_layer`` will have
+            ``{film_name: potential_from_film}``. If with_units is True, then the
+            array(s) will contain pint.Quantities. ``potential_from_film`` will have
             shape ``(m, 3)``.
         """
         device = self.device
+        layers = device.layers
+        meshes = device.meshes
         dtype = device.solve_dtype
         ureg = device.ureg
-        points = device.points.astype(dtype, copy=False)
-        areas = device.weights
         units = units or f"{self.field_units} * {device.length_units}"
+        layers_by_film = {}
+        for name, film in device.films.items():
+            layers_by_film[name] = layers[film.layer]
 
         # In case something like a list [x, y] or [x, y, z] is given
         positions = np.atleast_2d(positions)
         # If positions includes z coordinates, peel those off here
         if positions.shape[1] == 3:
             if zs is not None:
                 raise ValueError(
                     "If positions has shape (m, 3) then zs cannot be specified."
                 )
             zs = positions[:, 2]
             positions = positions[:, :2]
-        elif isinstance(zs, (int, float, np.generic)):
-            # constant zs
-            zs = zs * np.ones(positions.shape[0], dtype=dtype)
+        else:
+            zs = np.squeeze(zs)
+            if zs.ndim == 0:
+                zs = zs.item() * np.ones(positions.shape[0], dtype=dtype)
         if not isinstance(zs, np.ndarray):
             raise ValueError(f"Expected zs to be an ndarray, but got {type(zs)}.")
         if zs.ndim == 1:
             # We need zs to be shape (m, 1)
             zs = zs[:, np.newaxis]
-        rho2 = cdist(positions, points, metric="sqeuclidean").astype(dtype, copy=False)
+
         # Compute the vector potential at the specified positions
-        # from the currents in each layer
+        # from the currents in each film
         vector_potentials = {}
-        for name, layer in device.layers.items():
-            dz = zs - layer.z0
-            if np.any(dz == 0):
+        for name, film in device.films.items():
+            dz = zs - layers_by_film[name].z0
+            if np.all(dz == 0) and film.contains_points(positions).all():
                 raise ValueError(
-                    f"Cannot calculate fields in the same plane as layer {name}."
+                    f"Cannot evaluate vector potential inside the film ({name!r})."
                 )
+            mesh = meshes[name]
+            rho2 = cdist(positions, mesh.sites, metric="sqeuclidean")
+            areas = mesh.vertex_areas
             # J has units of [current / length], shape = (device.points.shape[0], 2)
-            J = self.current_densities[name]
+            J = self.film_solutions[name].current_density
             # rho has units of [length] and
             # shape = (postitions.shape[0], device.points.shape[0], 1)
             rho = np.sqrt(rho2 + dz**2)[:, :, np.newaxis]
-            Axy = np.einsum("ijk, j -> ik", J / rho, areas, dtype=dtype)
+            Axy = np.einsum("ijk, j -> ik", J / rho, areas)
             # z-component is zero because currents are parallel to the x-y plane.
             A = np.concatenate([Axy, np.zeros_like(Axy[:, :1])], axis=1)
             A = A * ureg(self.current_units)
             A = (ureg("mu_0") / (4 * np.pi) * A).to(units)
             if not with_units:
                 A = A.magnitude
             vector_potentials[name] = A
         if return_sum:
             return sum(vector_potentials.values())
         return vector_potentials
 
-    def to_file(
+    def to_hdf5(
         self,
-        directory: str,
-        save_mesh: bool = True,
-        compressed: bool = True,
-        to_zip: bool = False,
+        path_or_group: Union[os.PathLike, h5py.Group],
+        device_path: Optional[str] = None,
+        compress: bool = True,
     ) -> None:
-        """Saves a Solution to disk.
+        """Save the Solution to an HDF5 file.
+
+        path_or_group: An HDF5 file path or an open h5py.Group in which to save
+            the Solution.
+        device_path: Path within the HDF5 file in which the Solution's Device
+            is saved. If None, the Device will be saved at ``"/device"``.
+        compress: Save the mesh in a compressed format.
+        """
+        if isinstance(path_or_group, h5py.Group):
+            save_context = nullcontext(path_or_group)
+        else:
+            save_context = h5py.File(path_or_group, "x")
+        with save_context as h5group:
+            h5group.attrs["time_created"] = self.time_created.isoformat()
+            h5group.attrs["field_units"] = self.field_units
+            h5group.attrs["current_units"] = self.current_units
+            h5group.attrs["solver"] = self.solver
+            version_grp = h5group.create_group("version_info")
+            version_grp.attrs.update(self.version_info)
+            if device_path is None:
+                self.device.to_hdf5(
+                    h5group.create_group("device"), save_mesh=True, compress=compress
+                )
+            else:
+                h5group["device"] = h5py.SoftLink(device_path)
+            grp = h5group.create_group("film_solutions")
+            for name, film_solution in self.film_solutions.items():
+                film_solution.to_hdf5(grp.create_group(name))
+            vortices_grp = h5group.create_group("vortices")
+            for i, vortex in enumerate(self.vortices):
+                vortex.to_hdf5(vortices_grp.create_group(str(i)))
+            serialize_obj(h5group, self.applied_field_func, "applied_field_func")
+            circ_grp = h5group.create_group("circulating_currents")
+            circ_grp.attrs.update(self.circulating_currents)
+            term_grp = h5group.create_group("terminal_currents")
+            term_grp.attrs.update(self.terminal_currents)
+
+    @staticmethod
+    def from_hdf5(
+        path_or_group: Union[os.PathLike, h5py.Group],
+    ) -> "Solution":
+        """Load a Solution from and HDF5 file.
 
         Args:
-            directory: The name of the directory in which to save the solution
-                (must either be empty or not yet exist).
-            save_mesh: Whether to save the device mesh.
-            compressed: Whether to use numpy.savez_compressed rather than numpy.savez.
-            to_zip: Whether to save the Solution to a zip file.
+            path_or_group: An HDF5 file path or an open h5py.Group from which to load
+                the Solution.
+
+        Returns:
+            The loaded Solution
         """
-        if to_zip:
-            from .io import zip_solution
+        if isinstance(path_or_group, h5py.Group):
+            read_context = nullcontext(path_or_group)
+        else:
+            read_context = h5py.File(path_or_group, "r")
+        with read_context as h5group:
+            device = Device.from_hdf5(h5group["device"])
+            film_solutions = {}
+            for name, grp in h5group["film_solutions"].items():
+                film_solutions[name] = FilmSolution.from_hdf5(grp)
+            applied_field_func = deserialize_obj(h5group, "applied_field_func")
+            vortices = []
+            for i in sorted(h5group["vortices"], key=int):
+                vortices.append(Vortex.from_hdf5(h5group[f"vortices/{i}"]))
+            time_created = dt.datetime.fromisoformat(h5group.attrs["time_created"])
+            version_info = dict(h5group["version_info"].attrs)
+
+            solution = Solution(
+                device=device,
+                film_solutions=film_solutions,
+                applied_field_func=applied_field_func,
+                vortices=vortices,
+                circulating_currents=dict(h5group["circulating_currents"].attrs),
+                terminal_currents=dict(h5group["terminal_currents"].attrs),
+                current_units=h5group.attrs["current_units"],
+                field_units=h5group.attrs["field_units"],
+                solver=h5group.attrs["solver"],
+            )
+            # Set "read-only" attributes
+            solution._time_created = time_created
+            solution._version_info = version_info
+
+        return solution
 
-            zip_solution(self, directory)
+    @staticmethod
+    def save_solutions(
+        solutions: Sequence["Solution"],
+        path_or_group: Union[os.PathLike, h5py.Group],
+        compress: bool = True,
+    ) -> None:
+        """Save a series of Solutions to an HDF5 file.
+
+        Args:
+            solutions: A series of Solutions to save.
+            path_or_group: An HDF5 file path or an open h5py.Group in which to save
+                the Solutions.
+            compress: Save the meshes in a compressed format.
+        """
+        if not solutions:
             return
+        device = solutions[0].device
+        if isinstance(path_or_group, h5py.Group):
+            save_context = nullcontext(path_or_group)
+        else:
+            save_context = h5py.File(path_or_group, "x")
+        with save_context as h5group:
+            device_grp = h5group.create_group("device")
+            device.to_hdf5(device_grp)
+            for i, solution in enumerate(solutions):
+                device_path = None
+                if solution.device == device:
+                    device_path = device_grp.name
+                solution.to_hdf5(
+                    h5group.create_group(str(i)),
+                    device_path=device_path,
+                    compress=compress,
+                )
 
-        if os.path.isdir(directory) and len(os.listdir(directory)):
-            raise IOError(f"Directory '{directory}' already exists and is not empty.")
-        os.makedirs(directory, exist_ok=True)
-
-        # Save device
-        device_path = "device"
-        self.device.to_file(os.path.join(directory, device_path), save_mesh=save_mesh)
-
-        # Save arrays
-        array_paths = []
-        save_npz = np.savez_compressed if compressed else np.savez
-        for layer in self.device.layers:
-            path = f"{layer}_arrays.npz"
-            save_npz(
-                os.path.join(directory, path),
-                streams=self.streams[layer],
-                current_densities=self.current_densities[layer],
-                fields=self.fields[layer],
-                screening_fields=self.screening_fields[layer],
-            )
-            array_paths.append(path)
+    @staticmethod
+    def load_solutions(
+        path_or_group: Union[os.PathLike, h5py.Group]
+    ) -> List["Solution"]:
+        """Load a series of Solutions from an HDF5 file.
 
-        # Save applied field function
-        applied_field_path = "applied_field.dill"
-        with open(os.path.join(directory, applied_field_path), "wb") as f:
-            dill.dump(self.applied_field, f)
-
-        # Handle circulating current formatting
-        circ_currents = {}
-        for name, val in self.circulating_currents.items():
-            if isinstance(val, pint.Quantity):
-                val = str(val)
-            circ_currents[name] = val
-
-        metadata = {
-            "device": device_path,
-            "arrays": array_paths,
-            "applied_field": applied_field_path,
-            "circulating_currents": circ_currents,
-            "vortices": self.vortices,
-            "field_units": self.field_units,
-            "current_units": self.current_units,
-            "solver": self.solver,
-            "time_created": self.time_created.isoformat(),
-            "version_info": self.version_info,
-        }
-
-        with open(os.path.join(directory, "metadata.json"), "w") as f:
-            json.dump(metadata, f, indent=4)
-
-    @classmethod
-    def from_file(cls, directory: str, compute_matrices: bool = False) -> "Solution":
-        """Loads a Solution from file.
-
-        Args:
-            directory: The directory from which to load the solution.
-            compute_matrices: Whether to compute the field-independent
-                matrices for the device if the mesh already exists.
-
-        Returns:
-            The loaded Solution instance
-        """
-        if directory.endswith(".zip") or zipfile.is_zipfile(directory):
-            from .io import unzip_solution
-
-            solution = unzip_solution(directory)
-            if compute_matrices:
-                solution.device.compute_matrices()
-            return solution
-
-        with open(os.path.join(directory, "metadata.json"), "r") as f:
-            info = json.load(f)
-
-        # Load device
-        device_path = os.path.join(directory, info.pop("device"))
-        device = Device.from_file(device_path, compute_matrices=compute_matrices)
-
-        # Load arrays
-        streams = {}
-        current_densities = {}
-        fields = {}
-        screening_fields = {}
-        array_paths = info.pop("arrays")
-        for path in array_paths:
-            layer = path.replace("_arrays.npz", "")
-            with np.load(os.path.join(directory, path)) as arrays:
-                streams[layer] = arrays["streams"]
-                current_densities[layer] = arrays["current_densities"]
-                fields[layer] = arrays["fields"]
-                screening_fields[layer] = arrays["screening_fields"]
-
-        # Load applied field function
-        with open(os.path.join(directory, info.pop("applied_field")), "rb") as f:
-            applied_field = dill.load(f)
-
-        time_created = datetime.fromisoformat(info.pop("time_created"))
-        version_info = info.pop("version_info", None)
-        vortices = info.pop("vortices", [])
-        vortices = [Vortex(*v) for v in vortices]
-
-        solution = cls(
-            device=device,
-            streams=streams,
-            current_densities=current_densities,
-            fields=fields,
-            screening_fields=screening_fields,
-            applied_field=applied_field,
-            vortices=vortices,
-            **info,
-        )
-        # Set "read-only" attributes
-        solution._time_created = time_created
-        solution._version_info = version_info
+        Args:
+            path_or_group: An HDF5 file path or an open h5py.Group from which to load
+                the Solutions.
 
-        return solution
+        Returns:
+            A list of loaded Solutions.
+        """
+        if isinstance(path_or_group, h5py.Group):
+            read_context = nullcontext(path_or_group)
+        else:
+            read_context = h5py.File(path_or_group, "r")
+        solutions = []
+        with read_context as h5group:
+            groups = sorted((key for key in h5group if key.isdigit()), key=int)
+            for group in groups:
+                solutions.append(Solution.from_hdf5(h5group[group]))
+        return solutions
 
     def equals(
         self,
         other: Any,
         require_same_timestamp: bool = False,
     ) -> bool:
         """Checks whether two solutions are equal.
@@ -990,31 +1118,22 @@
             and (self.field_units == other.field_units)
             and (self.current_units == other.current_units)
             and (self.circulating_currents == other.circulating_currents)
             and (
                 getattr(self, "terminal_currents", None)
                 == getattr(other, "terminal_currents", None)
             )
-            and (self.applied_field == other.applied_field)
+            and (self.applied_field_func == other.applied_field_func)
             and (self.vortices == other.vortices)
         ):
             return False
         if require_same_timestamp and (self.time_created != other.time_created):
             return False
-        # Then check the arrays, which will take longer
-        for name, array in self.streams.items():
-            if not np.allclose(array, other.streams[name]):
-                return False
-        for name, array in self.current_densities.items():
-            if not np.allclose(array, other.current_densities[name]):
-                return False
-        for name, array in self.fields.items():
-            if not np.allclose(array, other.fields[name]):
-                return False
-        return True
+        # Then check the film_solutions, which will take longer
+        return self.film_solutions == other.film_solutions
 
     def __eq__(self, other) -> bool:
         return self.equals(other, require_same_timestamp=True)
 
     def plot_streams(self, **kwargs) -> Tuple[plt.Figure, np.ndarray]:
         """Alias for :func:`superscreen.visualization.plot_streams`."""
         from .visualization import plot_streams
```

### Comparing `superscreen-0.8.2/superscreen/solve.py` & `superscreen-0.9.0/superscreen/visualization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1244 +1,1033 @@
-import contextlib
 import itertools
-import logging
-import os
-import tempfile
+import warnings
 from collections import defaultdict
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from contextlib import contextmanager
+from typing import Dict, List, Literal, Optional, Sequence, Tuple, Union
 
+import matplotlib as mpl
+import matplotlib.pyplot as plt
 import numpy as np
 import pint
-import psutil
-import scipy.linalg as la
-import scipy.sparse as sp
-from scipy.spatial import distance
-
-try:
-    import jax
-    import jax.numpy as jnp
-    import jax.scipy.linalg as jla
-
-    HAS_JAX = True
-except (ModuleNotFoundError, ImportError, RuntimeError):
-    HAS_JAX = False
-
-from .device import Device
-from .device.transport import TransportDevice, stream_from_terminal_current
-from .parameter import Constant, Parameter
-from .solution import Solution, Vortex
-from .sources import ConstantField
-
-lambda_str = "\u03bb"
-Lambda_str = "\u039b"
-
-logger = logging.getLogger(__name__)
-
-
-class LambdaInfo:
-    def __init__(
-        self,
-        *,
-        layer: str,
-        Lambda: np.ndarray,
-        london_lambda: Optional[np.ndarray] = None,
-        thickness: Optional[float] = None,
-    ):
-        self.layer = layer
-        self.Lambda = Lambda
-        self.london_lambda = london_lambda
-        self.thickness = thickness
-        self.inhomogeneous = (
-            np.ptp(self.Lambda) / max(np.min(np.abs(self.Lambda)), np.finfo(float).eps)
-            > 1e-6
-        )
-        if self.inhomogeneous:
-            logger.warning(
-                f"Inhomogeneous {Lambda_str} in layer '{self.layer}', "
-                f"which violates the assumptions of the London model. "
-                f"Results may not be reliable."
-            )
-        if self.london_lambda is not None:
-            assert self.thickness is not None
-            assert np.allclose(self.Lambda, self.london_lambda**2 / self.thickness)
-        if np.any(self.Lambda < 0):
-            raise ValueError(f"Negative Lambda in layer '{layer}'.")
-
-
-def q_matrix(
-    points: np.ndarray, dtype: Optional[Union[str, np.dtype]] = None
-) -> np.ndarray:
-    """Computes the denominator matrix, q:
+from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
+from scipy import interpolate
 
-    .. math::
+from .device.mesh import Mesh
+from .solution import InterpolatorType, Solution
+from .solver import convert_field
 
-        q_{ij} = \\frac{1}{4\\pi|\\vec{r}_i-\\vec{r}_j|^3}
 
-    See Eq. 7 in [Brandt-PRB-2005]_, Eq. 8 in [Kirtley-RSI-2016]_,
-    and Eq. 8 in [Kirtley-SST-2016]_.
+@contextmanager
+def non_gui_backend():
+    """A contextmanager that temporarily uses a non-GUI backend for matplotlib."""
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            "ignore", category=UserWarning, message="Matplotlib is currently using agg"
+        )
+        try:
+            old_backend = mpl.get_backend()
+            mpl.use("Agg")
+            yield
+        finally:
+            mpl.use(old_backend)
+
+
+def auto_range_iqr(
+    data_array: np.ndarray,
+    cutoff_percentile: Union[float, Tuple[float, float]] = 1,
+) -> Tuple[float, float]:
+    """Get the min and max range of the provided array that excludes outliers
+    following the IQR rule.
+
+    This function computes the inter-quartile-range (IQR), defined by Q3-Q1,
+    i.e. the percentiles for 75 and 25 percent of the distribution. The region
+    without outliers is defined by [Q1-1.5*IQR, Q3+1.5*IQR].
+    Taken from `qcodes <https://github.com/QCoDeS/Qcodes/blob/
+    6c8f7202f6b6fca4884bfc0f6e1e9a6564628d75/qcodes/utils/plotting.py#L28-L76>`_.
 
     Args:
-        points: Shape (n, 2) array of x,y coordinates of vertices.
-        dtype: Output dtype.
+        data_array: Array of arbitrary dimension containing the
+            statistical data.
+        cutoff_percentile: Percentile of data that may maximally be
+            clipped on both sides of the distribution. If given a
+            tuple (a, b) the percentile limits will be a and 100-b.
 
     Returns:
-        Shape (n, n) array, qij
+        vmin, vmax
     """
-    # Euclidean distance between points
-    distances = distance.cdist(points, points, metric="euclidean")
-    if dtype is not None:
-        distances = distances.astype(dtype, copy=False)
-    with np.errstate(divide="ignore"):
-        q = 1 / (4 * np.pi * distances**3)
-    np.fill_diagonal(q, np.inf)
-    return q.astype(dtype, copy=False)
-
-
-def C_vector(
-    points: np.ndarray,
-    dtype: Optional[Union[str, np.dtype]] = None,
-) -> np.ndarray:
-    """Computes the edge vector, C:
-
-    .. math::
-        C_i &= \\frac{1}{4\\pi}\\sum_{p,q=\\pm1}\\sqrt{(\\Delta x - px_i)^{-2}
-            + (\\Delta y - qy_i)^{-2}}\\\\
-        \\Delta x &= \\frac{1}{2}(\\mathrm{max}(x) - \\mathrm{min}(x))\\\\
-        \\Delta y &= \\frac{1}{2}(\\mathrm{max}(y) - \\mathrm{min}(y))
+    if isinstance(cutoff_percentile, tuple):
+        bottom, top = cutoff_percentile
+    else:
+        bottom = cutoff_percentile
+        top = 100 - bottom
+    z = data_array.flatten()
+    zmax = np.nanmax(z)
+    zmin = np.nanmin(z)
+    zrange = zmax - zmin
+    pmin, q3, q1, pmax = np.nanpercentile(z, [bottom, 75, 25, top])
+    iqr = q3 - q1
+    # handle corner case of all data zero, such that IQR is zero
+    # to counter numerical artifacts do not test IQR == 0, but IQR on its
+    # natural scale (zrange) to be smaller than some very small number.
+    # also test for zrange to be 0.0 to avoid division by 0.
+    if zrange == 0.0 or iqr / zrange < 1e-8:
+        vmin = zmin
+        vmax = zmax
+    else:
+        vmin = max(q1 - 1.5 * iqr, zmin)
+        vmax = min(q3 + 1.5 * iqr, zmax)
+        vmin = min(vmin, pmin)
+        vmax = max(vmax, pmax)
+    return vmin, vmax
+
+
+def auto_grid(
+    num_plots: int,
+    max_cols: int = 3,
+    delaxes: bool = True,
+    **kwargs,
+) -> Tuple[plt.Figure, np.ndarray]:
+    """Creates a grid of at least ``num_plots`` subplots
+    with at most ``max_cols`` columns.
 
-    See Eq. 12 in [Brandt-PRB-2005]_, Eq. 16 in [Kirtley-RSI-2016]_,
-    and Eq. 15 in [Kirtley-SST-2016]_.
+    Additional keyword arguments are passed to plt.subplots().
 
     Args:
-        points: Shape (n, 2) array of x, y coordinates of vertices.
-        dtype: Output dtype.
+        num_plots: Total number of plots that will be populated.
+        max_cols: Maximum number of columns in the grid.
+        delaxes: Whether to remove unused axes.
 
     Returns:
-        Shape (n, ) array, Ci
+        matplotlib figure and axes
     """
-    x = points[:, 0]
-    y = points[:, 1]
-    x = x - x.mean()
-    y = y - y.mean()
-    a = np.ptp(x) / 2
-    b = np.ptp(y) / 2
-    with np.errstate(divide="ignore"):
-        C = sum(
-            np.sqrt((a - p * x) ** (-2) + (b - q * y) ** (-2))
-            for p, q in itertools.product((-1, 1), repeat=2)
-        )
-    C[np.isinf(C)] = 1e30
-    C /= 4 * np.pi
-    if dtype is not None:
-        C = C.astype(dtype, copy=False)
-    return C
-
-
-def Q_matrix(
-    q: np.ndarray,
-    C: np.ndarray,
-    weights: np.ndarray,
-    dtype: Optional[Union[str, np.dtype]] = None,
-) -> np.ndarray:
-    """Computes the kernel matrix, Q:
-
-    .. math::
-
-        Q_{ij} = (\\delta_{ij}-1)q_{ij}
-        + \\delta_{ij}\\frac{1}{w_{ij}}\\left(C_i
-        + \\sum_{l\\neq i}q_{il}w_{il}\\right)
+    ncols = min(max_cols, num_plots)
+    nrows = int(np.ceil(num_plots / ncols))
+    fig, axes = plt.subplots(nrows, ncols, **kwargs)
+    if not isinstance(axes, (list, np.ndarray)):
+        axes = np.array([axes])
+    if delaxes:
+        flat_axes = list(axes.flat)
+        for ax in flat_axes[num_plots:]:
+            fig.delaxes(ax)
+    return fig, axes
+
 
-    See Eq. 10 in [Brandt-PRB-2005]_, Eq. 11 in [Kirtley-RSI-2016]_,
-    and Eq. 11 in [Kirtley-SST-2016]_.
+def grids_to_vecs(
+    xgrid: np.ndarray, ygrid: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Extracts coordinate vectors from 2D meshgrids.
 
     Args:
-        q: Shape (n, n) matrix qij.
-        C: Shape (n, ) vector Ci.
-        weights: Shape (n, ) weight vector.
-        dtype: Output dtype.
+        xgrid: meshgrid of x coordinates
+        ygrid: meshgrid of y coordinates
 
     Returns:
-        Shape (n, n) array, Qij
+        vector of x coordinates, vector of y coordinates
     """
-    if sp.issparse(weights):
-        weights = weights.diagonal()
-    # q[i, i] are np.inf, but Q[i, i] involves a sum over only the
-    # off-diagonal elements of q, so we can just set q[i, i] = 0 here.
-    q = q.copy()
-    np.fill_diagonal(q, 0)
-    Q = -q
-    np.fill_diagonal(Q, (C + np.einsum("ij, j -> i", q, weights)) / weights)
-    if dtype is not None:
-        Q = Q.astype(dtype, copy=False)
-    return Q
-
-
-def convert_field(
-    value: Union[np.ndarray, float, str, pint.Quantity],
-    new_units: Union[str, pint.Unit],
-    old_units: Optional[Union[str, pint.Unit]] = None,
-    ureg: Optional[pint.UnitRegistry] = None,
-    with_units: bool = True,
-) -> Union[pint.Quantity, np.ndarray, float]:
-    """Converts a value between different field units, either magnetic field H
-    [current] / [length] or flux density B = mu0 * H [mass] / ([curret] [time]^2)).
+    return xgrid[0, :], ygrid[:, 0]
+
+
+def setup_color_limits(
+    dict_of_arrays: Dict[str, np.ndarray],
+    vmin: Optional[float] = None,
+    vmax: Optional[float] = None,
+    share_color_scale: bool = False,
+    symmetric_color_scale: bool = False,
+    auto_range_cutoff: Optional[Union[float, Tuple[float, float]]] = None,
+) -> Dict[str, Tuple[float, float]]:
+    """Set up color limits (vmin, vmax) for a dictionary of numpy arrays.
 
     Args:
-        value: The value to convert. It can either be a numpy array (no units),
-            a float (no units), a string like "1 uA/um", or a scalar or array
-            ``pint.Quantity``. If value is not a string wiht units or a ``pint.Quantity``,
-            then old_units must specify the units of the float or array.
-        new_units: The units to convert to.
-        old_units: The old units of ``value``. This argument is required if ``value``
-            is not a string with units or a ``pint.Quantity``.
-        ureg: The ``pint.UnitRegistry`` to use for conversion. If None is given,
-            a new instance is created.
-        with_units: Whether to return a ``pint.Quantity`` with units attached.
+        dict_of_arrays: Dict of ``{name: array}`` for which to compute color limits.
+        vmin: If provided, this vmin will be used for all arrays. If vmin is not None,
+            then vmax must also not be None.
+        vmax: If provided, this vmax will be used for all arrays. If vmax is not None,
+            then vmin must also not be None.
+        share_color_scale: Whether to force all arrays to share the same color scale.
+            This option is ignored if vmin and vmax are provided.
+        symmetric_color_scale: Whether to use a symmetric color scale (vmin = -vmax).
+            This option is ignored if vmin and vmax are provided.
+        auto_range_cutoff: Cutoff percentile for ``auto_range_iqr``.
 
     Returns:
-        The converted value, either a pint.Quantity (scalar or array with units),
-        or an array or float without units, depending on the ``with_units`` argument.
+        A dict of ``{name: (vmin, vmax)}``
     """
-    if ureg is None:
-        ureg = pint.UnitRegistry()
-    if isinstance(value, str):
-        value = ureg(value)
-    if isinstance(value, pint.Quantity):
-        old_units = value.units
-    if old_units is None:
-        raise ValueError(
-            "Old units must be specified if value is not a string or pint.Quantity."
-        )
-    if isinstance(old_units, str):
-        old_units = ureg(old_units)
-    if isinstance(new_units, str):
-        new_units = ureg(new_units)
-    if not isinstance(value, pint.Quantity):
-        value = value * old_units
-    if new_units.dimensionality == old_units.dimensionality:
-        value = value.to(new_units)
-    elif "[length]" in old_units.dimensionality:
-        # value is H in units with dimensionality [current] / [length]
-        # and we want B = mu0 * H
-        value = (value * ureg("mu0")).to(new_units)
+    if (vmin is not None and vmax is None) or (vmax is not None and vmin is None):
+        raise ValueError("If either vmin or max is provided, both must be provided.")
+    if vmin is not None:
+        return {name: (vmin, vmax) for name in dict_of_arrays}
+
+    if auto_range_cutoff is None:
+        clims = {
+            name: (np.nanmin(array), np.nanmax(array))
+            for name, array in dict_of_arrays.items()
+        }
     else:
-        # value is B = mu0 * H in units with dimensionality
-        # [mass] / ([current] [time]^2) and we want H = B / mu0
-        value = (value / ureg("mu0")).to(new_units)
-    if not with_units:
-        value = value.magnitude
-    return value
+        clims = {
+            name: auto_range_iqr(array, cutoff_percentile=auto_range_cutoff)
+            for name, array in dict_of_arrays.items()
+        }
+
+    if share_color_scale:
+        # All subplots share the same color scale
+        global_vmin = np.inf
+        global_vmax = -np.inf
+        for vmin, vmax in clims.values():
+            global_vmin = min(vmin, global_vmin)
+            global_vmax = max(vmax, global_vmax)
+        clims = {name: (global_vmin, global_vmax) for name in dict_of_arrays}
+
+    if symmetric_color_scale:
+        # Set vmin = -vmax
+        new_clims = {}
+        for name, (vmin, vmax) in clims.items():
+            new_vmax = max(vmax, -vmin)
+            new_clims[name] = (-new_vmax, new_vmax)
+        clims = new_clims
 
+    return clims
 
-def field_conversion_factor(
-    field_units: str,
-    current_units: str,
-    length_units: str = "m",
-    ureg: Optional[pint.UnitRegistry] = None,
-) -> pint.Quantity:
-    """Returns a conversion factor from ``field_units`` to ``current_units / length_units``.
+
+def make_lims(vals: np.ndarray, buffer: float = 0.0) -> Tuple[float, float]:
+    """Create axis limits with a buffer.
 
     Args:
-        field_units: Magnetic field/flux unit to convert, having dimensionality
-            either of magnetic field ``H`` (e.g. A / m or Oe) or of
-            magnetic flux density ``B = mu0 * H`` (e.g. Tesla or Gauss).
-        current_units: Current unit to use for the conversion.
-        length_units: Lenght/distance unit to use for the conversion.
-        ureg: pint UnitRegistry to use for the conversion. If None is provided,
-            a new UnitRegistry is created.
+        vals: The axis coordinates
+        buffer: Axis limit buffer in units of the peak-to-peak of the coordinates.
 
     Returns:
-        Conversion factor as a ``pint.Quantity``. ``conversion_factor.magnitude``
-        gives you the numerical value of the conversion factor.
+        vmin, vmax
     """
-    if ureg is None:
-        ureg = pint.UnitRegistry()
-    field = ureg(field_units)
-    target_units = f"{current_units} / {length_units}"
-    try:
-        field = field.to(target_units)
-    except pint.DimensionalityError:
-        # field_units is flux density B = mu0 * H
-        field = (field / ureg("mu0")).to(target_units)
-    return field / ureg(field_units)
-
-
-def _make_system(Q, weights, Lambda, Del2, grad_Lambda_term, ix, inhomogeneous=False):
-    """Builds the linear system for the 'effective applied fields'."""
-    if inhomogeneous:
-        grad_Lambda = grad_Lambda_term[:, ix]
-    else:
-        grad_Lambda = 0
-    return Q[:, ix] * weights[ix, 0] - Lambda[ix, 0] * Del2[:, ix] - grad_Lambda
+    vmin = np.min(vals)
+    vmax = np.max(vals)
+    dv = vmax - vmin
+    return vmin - buffer * dv, vmax + buffer * dv
 
 
-def _make_system_2d(
-    Q, weights, Lambda, Del2, grad_Lambda_term, ix1d, inhomogeneous=False
-):
-    """Builds the linear system to solve for the stream function."""
-    ix2d = np.ix_(ix1d, ix1d)
-    if inhomogeneous:
-        grad_Lambda = grad_Lambda_term[ix2d]
-    else:
-        grad_Lambda = 0
-    return Q[ix2d] * weights[ix1d, 0] - Lambda[ix1d, 0] * Del2[ix2d] - grad_Lambda
+def cross_section(
+    dataset_coords: np.ndarray,
+    dataset_values: np.ndarray,
+    cross_section_coords: Union[np.ndarray, Sequence[np.ndarray]],
+    interp_method: InterpolatorType = "linear",
+) -> Tuple[List[np.ndarray], List[np.ndarray], List[np.ndarray]]:
+    """Takes a cross-section of the specified dataset values along
+    a path given by the given dataset coordinates.
 
+    Args:
+        dataset_coords: A shape (n, 2) array of (x, y) coordinates for the dataset.
+        dataset_values: A shape (n, ) array of dataset values of which
+            to take a cross-section.
+        cross_section_coords: A shape (m, 2) array of (x, y) coordinates specifying
+            the cross-section path (or a list of such arrays for multiple
+            cross sections).
+        interp_method: The interpolation method to use: "nearest", "linear", "cubic".
 
-def _solve_for_terminal_current_stream(
-    device: TransportDevice,
-    points: np.ndarray,
-    in_hole: np.ndarray,
-    Q: np.ndarray,
-    weights: np.ndarray,
-    Del2: np.ndarray,
-    Lambda: np.ndarray,
-    grad_Lambda_term: np.ndarray,
-    terminal_currents: Dict[str, float],
-    hole_indices: np.ndarray,
-    gpu: bool = False,
-    inhomogeneous: bool = False,
-) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    1. Solve for the stream function in the film assuming no applied field and
-    ignoring the presence of any holes.
-    2. Set the stream function in each hole to the weighted average of the stream
-    function found in step 1.
-    3. Re-solve for the stream function in the film with the new hole boundary conditions.
+    Returns:
+        A list of coordinate arrays, a list of curvilinear coordinate (path) arrays,
+        and a list of cross section values.
     """
-    device._check_current_mapping(terminal_currents)
-    terminal_currents = terminal_currents.copy()
-    # The drain terminal must sink all current
-    if device.drain_terminal is not None:
-        terminal_currents[device.drain_terminal.name] = -sum(
-            terminal_currents.get(term.name, 0) for term in device.source_terminals
+    valid_methods = ("nearest", "linear", "cubic")
+    if interp_method not in valid_methods:
+        raise ValueError(
+            f"Interpolation method must be one of {valid_methods} "
+            f"(got {interp_method})."
         )
-    boundary_indices = device.boundary_vertices()
-    on_boundary = np.zeros(points.shape[0], dtype=bool)
-    boundary_points = points[boundary_indices]
-    on_boundary[boundary_indices] = True
-
-    if gpu:
-        g = jnp.zeros(points.shape[0])
-        Ha_eff = jnp.zeros(points.shape[0])
-    else:
-        g = np.zeros(points.shape[0])
-        Ha_eff = np.zeros(points.shape[0])
+    if interp_method == "nearest":
+        interpolator = interpolate.NearestNDInterpolator
+    elif interp_method == "linear":
+        interpolator = interpolate.LinearNDInterpolator
+    else:  # "cubic"
+        interpolator = interpolate.CloughTocher2DInterpolator
+
+    if not (isinstance(cross_section_coords, Sequence)):
+        cross_section_coords = [cross_section_coords]
+    cross_section_coords = [np.asarray(c) for c in cross_section_coords]
+    for i, arr in enumerate(cross_section_coords):
+        if arr.ndim != 2 or arr.shape[1] != 2:
+            raise ValueError(
+                f"Invalid shape for coordinate array {i}: {arr.shape}. "
+                f"Coordinate arrays must have shape (n, 2)."
+            )
+    # Calculcate curvilinear cross section coordinates
+    paths = []
+    for c in cross_section_coords:
+        path = np.cumsum(np.sqrt(np.sum(np.diff(c, axis=0) ** 2, axis=1)))
+        paths.append(np.concatenate([[0], path], axis=0))
+    # Calculate cross sections.
+    cross_sections = []
+    mask = np.isfinite(dataset_values)
+    z_interp = interpolator(dataset_coords[mask], dataset_values[mask])
+    for c in cross_section_coords:
+        cross_sections.append(z_interp(c[:, 0], c[:, 1]))
+
+    return cross_section_coords, paths, cross_sections
+
+
+def plot_streams(
+    solution: Solution,
+    films: Optional[Union[List[str], str]] = None,
+    units: Optional[str] = None,
+    max_cols: int = 3,
+    cmap: str = "coolwarm",
+    colorbar: bool = True,
+    shading: Literal["flat", "gouraud"] = "flat",
+    auto_range_cutoff: Optional[Union[float, Tuple[float, float]]] = None,
+    share_color_scale: bool = False,
+    symmetric_color_scale: bool = True,
+    vmin: Optional[float] = None,
+    vmax: Optional[float] = None,
+    **kwargs,
+) -> Tuple[plt.Figure, np.ndarray]:
+    """Plots the stream function for multiple layers in a Device.
 
-    if not any(terminal_currents.values()):
-        return g, on_boundary
+    Additional keyword arguments are passed to plt.subplots().
 
-    ix_points = np.arange(points.shape[0], dtype=int)
-    Lambda = 1e10 * np.ones_like(Lambda)
+    Args:
+        solution: The Solution from which to extract stream functions.
+        films: Name(s) of films(s) for which to plot the stream function.
+            By default, the stream function is plotted for all films in the Device.
+        units: Units in which to plot the stream function. Defaults to
+            solution.current_units.
+        max_cols: Maximum number of columns in the grid of subplots.
+        cmap: Name of the matplotlib colormap to use.
+        colorbar: Whether to add a colorbar to each subplot.
+        shading: May be ``"flat"`` or ``"gouraud"``. The latter does some interpolation.
+        auto_range_cutoff: Cutoff percentile for ``auto_range_iqr``.
+        share_color_scale: Whether to force all layers to use the same color scale.
+        symmetric_color_scale: Whether to use a symmetric color scale (vmin = -vmax).
+        vmin: Color scale minimum to use for all layers
+        vmax: Color scale maximum to use for all layers
 
-    def min_index(terminal):
-        return terminal.contains_points(boundary_points, index=True).max()
-
-    terminals = sorted(device.source_terminals + [device.drain_terminal], key=min_index)
-    # Rotate terminals so that the drain is the last element
-    while terminals[-1] is not device.drain_terminal:
-        terminals.append(terminals.pop(0))
-    for terminal in terminals:
-        current = terminal_currents[terminal.name]
-        ix_boundary = sorted(
-            terminal.contains_points(boundary_points, index=True).tolist()
-        )
-        remaining_boundary = boundary_indices[(ix_boundary[-1] + 1) :]
-        ix_terminal = boundary_indices[ix_boundary]
-        stream = stream_from_terminal_current(points[ix_terminal], -current)
-        if gpu:
-            g = g.at[ix_terminal].add(stream)
-            g = g.at[remaining_boundary].add(stream[-1])
-        else:
-            g[ix_terminal] += stream
-            g[remaining_boundary] += stream[-1]
-    # The stream function on the "reference boundary" (i.e., the boundary
-    # immediately after the output terminal in a CCW direction) should be zero.
-    g_ref = g[ix_terminal.max()]
-    ix = boundary_indices
-    if gpu:
-        g = g.at[ix].add(-g_ref)
-    else:
-        g[ix] += -g_ref
-    A = _make_system(
-        Q, weights, Lambda, Del2, grad_Lambda_term, ix, inhomogeneous=inhomogeneous
-    )
-    if gpu:
-        Ha_eff = Ha_eff.at[ix_points].add(-A @ g[ix])
-    else:
-        Ha_eff += -A @ g[ix]
-    # First solve for the stream function inside the film, ignoring the
-    # presence of holes completely.
-    film = device.film
-    ix1d = np.logical_and.reduce(
-        [film.contains_points(points), np.logical_not(on_boundary)]
-    )
-    ix1d = np.where(ix1d)[0]
-    A = _make_system_2d(
-        Q, weights, Lambda, Del2, grad_Lambda_term, ix1d, inhomogeneous=inhomogeneous
+    Returns:
+        matplotlib figure and axes
+    """
+    device = solution.device
+    meshes = device.meshes
+    length_units = device.ureg(device.length_units).units
+    units = units or solution.current_units
+    if isinstance(units, str):
+        units = device.ureg(units).units
+    if films is None:
+        films = list(device.films)
+    if isinstance(films, str):
+        films = [films]
+    fig, axes = auto_grid(len(films), max_cols=max_cols, **kwargs)
+    streams = {}
+    for film in films:
+        stream = solution.film_solutions[film].stream
+        stream = stream * device.ureg(solution.current_units)
+        streams[film] = stream.to(units).magnitude
+    clim_dict = setup_color_limits(
+        streams,
+        vmin=vmin,
+        vmax=vmax,
+        share_color_scale=share_color_scale,
+        symmetric_color_scale=symmetric_color_scale,
+        auto_range_cutoff=auto_range_cutoff,
     )
-    h = -Ha_eff[ix1d]
-    if gpu:
-        lu_piv = jla.lu_factor(-A)
-        gf = jla.lu_solve(lu_piv, h)
-        g = g.at[ix1d].set(gf)
-    else:
-        lu_piv = la.lu_factor(-A)
-        gf = la.lu_solve(lu_piv, h)
-        g[ix1d] = gf
-
-    holes = {
-        name: hole for name, hole in device.holes.items() if hole.layer == film.layer
-    }
-    if len(holes) == 0:
-        return g, on_boundary
-
-    # Set the stream function in each hole to the average value
-    # obtained when ignoring holes.
-    if gpu:
-        Ha_eff = jnp.zeros(points.shape[0])
-    else:
-        Ha_eff = np.zeros(points.shape[0])
-    for name in holes:
-        ix = hole_indices[name]
-        if gpu:
-            g = g.at[ix].set(jnp.average(g[ix], weights=weights[ix, 0]))
-        else:
-            g[ix] = np.average(g[ix], weights=weights[ix, 0])
-        A = _make_system(
-            Q, weights, Lambda, Del2, grad_Lambda_term, ix, inhomogeneous=inhomogeneous
+    used_axes = []
+    for ax, film in zip(fig.axes, films):
+        stream = streams[film]
+        mesh = meshes[film]
+        film_vmin, film_vmax = clim_dict[film]
+        norm = mpl.colors.Normalize(vmin=film_vmin, vmax=film_vmax)
+        x = mesh.sites[:, 0]
+        y = mesh.sites[:, 1]
+        tri = mesh.elements
+        im = ax.tripcolor(
+            x,
+            y,
+            stream,
+            triangles=tri,
+            shading=shading,
+            cmap=cmap,
+            norm=norm,
         )
-        if gpu:
-            Ha_eff = Ha_eff.at[ix_points].add(-A @ g[ix])
-        else:
-            Ha_eff += -A @ g[ix]
+        ax.set_xlabel(f"$x$ [${length_units:~L}$]")
+        ax.set_ylabel(f"$y$ [${length_units:~L}$]")
+        ax.set_title(f"$g$ ({film!r})")
+        ax.set_aspect("equal")
+        cbar = None
+        if colorbar:
+            ax_divider = make_axes_locatable(ax)
+            cax = ax_divider.append_axes("right", size="8%", pad="4%")
+            cbar = fig.colorbar(im, cax=cax)
+            cbar.set_label(f"$g$ [${units:~L}$]")
+        ax.set_xlim(*make_lims(x, buffer=0.05))
+        ax.set_ylim(*make_lims(y, buffer=0.05))
+        used_axes.append(ax)
+        used_axes.append(ax)
+        if cbar is not None:
+            used_axes.append(cbar.ax)
+    for ax in fig.axes:
+        if ax not in used_axes:
+            fig.delaxes(ax)
+    fig.tight_layout()
+    return fig, axes
+
+
+def plot_fields(
+    solution: Solution,
+    films: Optional[Union[List[str], str]] = None,
+    dataset: Literal[
+        "field", "self_field", "applied_field", "field_from_other_films"
+    ] = "field",
+    normalize: bool = False,
+    units: Optional[str] = None,
+    shading: Literal["flat", "gouraud"] = "flat",
+    max_cols: int = 3,
+    cmap: str = "cividis",
+    colorbar: bool = True,
+    auto_range_cutoff: Optional[Union[float, Tuple[float, float]]] = None,
+    share_color_scale: bool = False,
+    symmetric_color_scale: bool = False,
+    vmin: Optional[float] = None,
+    vmax: Optional[float] = None,
+    cross_section_coords: Optional[Union[np.ndarray, Sequence[np.ndarray]]] = None,
+    **kwargs,
+) -> Tuple[plt.Figure, np.ndarray]:
+    """Plots the fields for one or more films in a Device.
 
-    ix = boundary_indices
-    A = _make_system(
-        Q, weights, Lambda, Del2, grad_Lambda_term, ix, inhomogeneous=inhomogeneous
-    )
-    if gpu:
-        Ha_eff = Ha_eff.at[ix_points].add(-A @ g[ix])
-    else:
-        Ha_eff += -A @ g[ix]
-
-    # Solve for the stream function inside the superconducting film again,
-    # now with the new boundary conditions for the holes.
-    ix1d = np.logical_and.reduce(
-        [
-            film.contains_points(points),
-            np.logical_not(in_hole),
-            np.logical_not(on_boundary),
-        ]
-    )
-    ix1d = np.where(ix1d)[0]
-    A = _make_system_2d(
-        Q, weights, Lambda, Del2, grad_Lambda_term, ix1d, inhomogeneous=inhomogeneous
-    )
-    h = -Ha_eff[ix1d]
-    if gpu:
-        lu_piv = jla.lu_factor(-A)
-        gf = jla.lu_solve(lu_piv, h)
-        g = g.at[ix1d].set(gf)
-    else:
-        lu_piv = la.lu_factor(-A)
-        gf = la.lu_solve(lu_piv, h)
-        g[ix1d] = gf
-    return g, on_boundary
-
-
-def solve_layer(
-    *,
-    device: Device,
-    layer: str,
-    applied_field: np.ndarray,
-    kernel: np.ndarray,
-    weights: np.ndarray,
-    Del2: np.ndarray,
-    grad: np.ndarray,
-    Lambda_info: LambdaInfo,
-    terminal_currents: Optional[Dict[str, Union[float, str, pint.Quantity]]] = None,
-    circulating_currents: Optional[Dict[str, Union[float, str, pint.Quantity]]] = None,
-    vortices: Optional[List[Vortex]] = None,
-    current_units: str = "uA",
-    check_inversion: bool = False,
-    gpu: bool = False,
-) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-    """Computes the stream function and magnetic field within a single layer of a ``Device``.
+    Additional keyword arguments are passed to plt.subplots().
 
     Args:
-        device: The Device to simulate.
-        layer: Name of the layer to analyze.
-        applied_field: The applied magnetic field evaluated at the mesh vertices.
-        weights: The Device's weight vector.
-        kernel: The Device's kernel matrix ``Q``.
-        Del2: The Device's Laplacian operator.
-        grad: The Device's vertex gradient matrix, shape (num_vertices, 2, num_vertices).
-        Lambda_info: A LambdaInfo instance defining Lambda(x, y).
-        terminal_currents: A dict of ``{source_name: source_current}`` for
-            each source terminal. This argument is only allowed if ``device``
-            as an instance of ``TransportDevice``.
-        circulating_currents: A dict of ``{hole_name: circulating_current}``.
-            If circulating_current is a float, then it is assumed to be in units
-            of current_units. If circulating_current is a string, then it is
-            converted to a pint.Quantity.
-        vortices: A list of Vortex objects located in films in this layer.
-        current_units: Units to use for current quantities. The applied field will be
-            converted to units of ``{current_units} / {device.length_units}``.
-        check_inversion: Whether to verify the accuracy of the matrix inversion.
-        gpu: Solve on a GPU if available (requires JAX and CUDA).
+        solution: The Solution from which to extract fields.
+        films: Name(s) of films(s) for which to plot the fields.
+            By default, the field is plotted for all films in the Device.
+        dataset: Which set of fields to plot, either "field", "self_field",
+            "applied_field", or "field_from_other_films".
+        normalize: Whether to normalize the fields by the applied field.
+        units: Units in which to plot the fields. Defaults to solution.field_units.
+            This argument is ignored if normalize is True.
+        shading: May be ``"flat"`` or ``"gouraud"``. The latter does some interpolation.
+        max_cols: Maximum number of columns in the grid of subplots.
+        cmap: Name of the matplotlib colormap to use.
+        colorbar: Whether to add a colorbar to each subplot.
+        auto_range_cutoff: Cutoff percentile for ``auto_range_iqr``.
+        share_color_scale: Whether to force all layers to use the same color scale.
+        symmetric_color_scale: Whether to use a symmetric color scale (vmin = -vmax).
+        vmin: Color scale minimum to use for all layers
+        vmax: Color scale maximum to use for all layers
+        cross_section_coords: Shape (m, 2) array of (x, y) coordinates for a
+            cross-section (or a list of such arrays).
 
     Returns:
-        stream function, current density, total field, film screening field
+        matplotlib figure and axes
     """
-
-    circulating_currents = circulating_currents or {}
-    terminal_currents = terminal_currents or {}
-    for name in circulating_currents:
-        if name not in device.holes:
-            raise ValueError(f"Circulating current specified for unknown hole: {name}.")
-    if isinstance(device, TransportDevice):
-        transport_device = True
-    else:
-        if terminal_currents:
-            raise TypeError("Terminal currents are only allowed for TransportDevices.")
-        transport_device = False
-    vortices = vortices or []
-    # Vortex flux in magnetization-like units,
-    # i.e. H * area as opposed to B * area = mu_0 * H * area.
-    # ([current] / [length]) * [length]^2 = [current] * [length]
-    vortex_flux = (
-        device.ureg("Phi_0 / mu_0")
-        .to(f"{current_units} * {device.length_units}")
-        .magnitude
+    valid_datasets = (
+        "field",
+        "self_field",
+        "applied_field",
+        "field_from_other_films",
     )
+    if dataset not in valid_datasets:
+        raise ValueError(f"Dataset must be one of {valid_datasets!r}.")
 
-    films = {name: film for name, film in device.films.items() if film.layer == layer}
-    holes = {name: hole for name, hole in device.holes.items() if hole.layer == layer}
-    Q = kernel
-    points = device.points
-
-    if gpu:
-        if not HAS_JAX:
-            raise ValueError("Running solve_layer(..., gpu=True) requires JAX.")
-        einsum_ = jnp.einsum
+    device = solution.device
+    meshes = device.meshes
+    # Length units from the Device
+    length_units = device.ureg(device.length_units).units
+    # The units the fields are currently in
+    old_units = device.ureg(solution.field_units).units
+    # The units we want to convert to
+    if units is None:
+        units = old_units
+    if isinstance(units, str):
+        units = device.ureg(units).units
+
+    if films is None:
+        films = list(device.films)
+    if isinstance(films, str):
+        films = [films]
+
+    fig, axes = auto_grid(len(films), max_cols=max_cols, **kwargs)
+    film_solutions = solution.film_solutions
+    applied_fields = {
+        name: fs.applied_field.copy() for name, fs in film_solutions.items()
+    }
+    if dataset == "field":
+        clabel = "$H_z$"
+        fields = {name: fs.total_field.copy() for name, fs in film_solutions.items()}
+    elif dataset == "self_field":
+        clabel = "$H_\\mathrm{sc}$"
+        fields = {name: fs.self_field.copy() for name, fs in film_solutions.items()}
+    elif dataset == "applied_field":
+        clabel = "$H_\\mathrm{applied}$"
+        fields = applied_fields
     else:
-        einsum_ = np.einsum
-
-    # Units: current_units / device.length_units.
-    Hz_applied = applied_field
-    inhomogeneous = Lambda_info.inhomogeneous
-    Lambda = Lambda_info.Lambda
-    if inhomogeneous:
-        grad_Lambda_term = einsum_("ijk, ijk -> jk", (grad @ Lambda), grad)
+        clabel = "$H_\\mathrm{other}$"
+        fields = {}
+        zeros = None
+        for name, fs in film_solutions.items():
+            other_field = fs.field_from_other_films
+            if other_field is None:
+                if zeros is None:
+                    zeros = np.zeros(len(applied_fields[name]))
+                other_field = zeros
+            fields[name] = other_field
+    if "[mass]" in units.dimensionality:
+        # We want flux density, B = mu0 * H
+        clabel = "$\\mu_0$" + clabel
+    if normalize:
+        for film, field in fields.items():
+            fields[film] = fields[film] / applied_fields[film]
+        clabel = clabel + " / $H_\\mathrm{applied}$"
     else:
-        grad_Lambda_term = None
-
-    # Identify holes in the superconductor
-    hole_indices = {}
-    in_hole = np.zeros(points.shape[0], dtype=bool)
-    for name, hole in holes.items():
-        ix = hole.contains_points(points)
-        hole_indices[name] = np.where(ix)[0]
-        in_hole = np.logical_or(in_hole, ix)
-
-    g = np.zeros_like(Hz_applied)
-    Ha_eff = np.zeros_like(Hz_applied)
-    if gpu:
-        g = jax.device_put(g)
-        ix_points = np.arange(Ha_eff.shape[0], dtype=int)
-        Ha_eff = jax.device_put(Ha_eff)
-
-    # Set the boundary conditions for all holes:
-    # 1. g[hole] = I_circ_hole
-    # 2. Effective field associated with I_circ_hole
-    # See Section II(a) in [Brandt], Eqs. 18-19 in [Kirtley1],
-    # and Eqs 17-18 in [Kirtley2].
-    for name in holes:
-        current = circulating_currents.get(name, 0)
-        ix = hole_indices[name]
-        if gpu:
-            g = g.at[ix].add(current)
-        else:
-            g[ix] += current  # g[hole] = I_circ
-        # Effective field associated with the circulating currents:
-        # current is in [current_units], Lambda is in [device.length_units],
-        # and Del2 is in [device.length_units ** (-2)], so
-        # Ha_eff has units of [current_unit / device.length_units]
-        A = _make_system(
-            Q, weights, Lambda, Del2, grad_Lambda_term, ix, inhomogeneous=inhomogeneous
-        )
-        if gpu:
-            Ha_eff = Ha_eff.at[ix_points].add(-A @ g[ix])
-        else:
-            Ha_eff += -A @ g[ix]
-
-    if transport_device:
-        g_transport, on_boundary = _solve_for_terminal_current_stream(
-            device,
-            points,
-            in_hole,
-            Q,
-            weights,
-            Del2,
-            Lambda,
-            grad_Lambda_term,
-            terminal_currents,
-            hole_indices,
-            gpu=gpu,
-            inhomogeneous=inhomogeneous,
-        )
-        if gpu:
-            g = g.at[ix_points].add(g_transport)
-        else:
-            g += g_transport
-
-    film_to_vortices = defaultdict(list)
-    for vortex in vortices:
-        for name, film in films.items():
-            if film.contains_points([vortex.x, vortex.y]):
-                film_to_vortices[name].append(vortex)
-                # A given vortex can only lie in a single film.
-                continue
-
-    # Now solve for the stream function inside the superconducting films
-    for name, film in films.items():
-        # We want all points that are in a film and not in a hole.
-        ix1d = np.logical_and(film.contains_points(points), np.logical_not(in_hole))
-        if transport_device:
-            ix1d = np.logical_and(ix1d, np.logical_not(on_boundary))
-        ix1d = np.where(ix1d)[0]
-        # # Form the linear system for the film:
-        # # gf = -K @ h, where K = inv(Q * w - Lambda * Del2 - grad_Lambda_term) = inv(A)
-        # # Eqs. 15-17 in [Brandt], Eqs 12-14 in [Kirtley1], Eqs. 12-14 in [Kirtley2].
-        A = _make_system_2d(
-            Q,
-            weights,
-            Lambda,
-            Del2,
-            grad_Lambda_term,
-            ix1d,
-            inhomogeneous=inhomogeneous,
+        for film in films:
+            fields[film] = convert_field(
+                fields[film],
+                units,
+                old_units=old_units,
+                ureg=device.ureg,
+                with_units=False,
+            )
+        clabel = clabel + f" [${units:~L}$]"
+    clim_dict = setup_color_limits(
+        fields,
+        vmin=vmin,
+        vmax=vmax,
+        share_color_scale=share_color_scale,
+        symmetric_color_scale=symmetric_color_scale,
+        auto_range_cutoff=auto_range_cutoff,
+    )
+    # Keep track of which axes are actually used,
+    # and delete unused axes later
+    used_axes = []
+    for ax, film in zip(fig.axes, films):
+        field = fields[film]
+        mesh = meshes[film]
+        film_vmin, film_vmax = clim_dict[film]
+        norm = mpl.colors.Normalize(vmin=film_vmin, vmax=film_vmax)
+        x = mesh.sites[:, 0]
+        y = mesh.sites[:, 1]
+        tri = mesh.elements
+        im = ax.tripcolor(
+            x,
+            y,
+            field,
+            triangles=tri,
+            shading=shading,
+            cmap=cmap,
+            norm=norm,
         )
-        h = Hz_applied[ix1d] - Ha_eff[ix1d]
-        if gpu:
-            lu_piv = jla.lu_factor(-A)
-            gf = jla.lu_solve(lu_piv, h)
-            g = g.at[ix1d].add(gf)
-        else:
-            lu_piv = la.lu_factor(-A)
-            gf = la.lu_solve(lu_piv, h)
-            g[ix1d] += gf
-
-        if check_inversion:
-            # Validate solution
-            hsim = -A @ gf
-            if not np.allclose(hsim, h):
-                logger.warning(
-                    f"Unable to solve for stream function in {layer} ({name}), "
-                    f"maximum error {np.abs(hsim - h).max():.3e}."
-                )
-        K = None  # Matrix inverse of A
-        for vortex in film_to_vortices[name]:
-            if K is None:
-                # Compute K only once if needed
-                if gpu:
-                    K = -jla.lu_solve(lu_piv, jnp.eye(A.shape[0]))
-                else:
-                    K = -la.lu_solve(lu_piv, np.eye(A.shape[0]))
-            # Index of the mesh vertex that is closest to the vortex position:
-            # in the film-specific sub-mesh
-            j_film = np.argmin(la.norm(points[ix1d] - [[vortex.x, vortex.y]], axis=1))
-            # ... and in the full device mesh.
-            j_device = np.argmin(la.norm(points - [[vortex.x, vortex.y]], axis=1))
-            # Eq. 28 in [Brandt]
-            g_vortex = vortex_flux * vortex.nPhi0 * K[:, j_film] / weights[j_device]
-            if gpu:
-                g = g.at[ix1d].add(g_vortex)
-            else:
-                g[ix1d] += g_vortex
-            del g_vortex
-    # Current density J = curl(g \hat{z}) = [dg/dy, -dg/dx]
-    Gx = grad[0]
-    Gy = grad[1]
-    Jx = np.asarray(Gy @ g)
-    Jy = np.asarray(-Gx @ g)
-    J = np.stack([Jx, Jy], axis=1)
-    # Eq. 7 in [Kirtley1], Eq. 7 in [Kirtley2]
-    screening_field = np.asarray(Q @ (weights[:, 0] * g))
-    # Above is equivalent to the following, but much faster
-    # screening_field = np.einsum("ij, ji, j -> i", Q, weights, g)
-    total_field = np.asarray(Hz_applied) + screening_field
-    return g, J, total_field, screening_field
-
-
-def solve(
-    device: Device,
-    *,
-    applied_field: Optional[Callable] = None,
-    terminal_currents: Optional[Dict[str, Union[float, str, pint.Quantity]]] = None,
-    circulating_currents: Optional[Dict[str, Union[float, str, pint.Quantity]]] = None,
-    vortices: Optional[List[Vortex]] = None,
-    field_units: str = "mT",
-    current_units: str = "uA",
-    check_inversion: bool = False,
-    iterations: int = 0,
-    return_solutions: bool = True,
-    directory: Optional[str] = None,
-    cache_memory_cutoff: float = np.inf,
-    log_level: int = logging.INFO,
-    gpu: bool = False,
-    _solver: str = "superscreen.solve",
-) -> List[Solution]:
-    """Computes the stream functions and magnetic fields for all layers in a ``Device``.
-
-    The simulation strategy is:
-
-    1. Compute the stream functions and fields for each layer given
-    only the applied field.
-
-    2. If iterations > 1 and there are multiple layers, then for each layer,
-    calculate the screening field from all other layers and recompute the
-    stream function and fields based on the sum of the applied field
-    and the screening fields from all other layers.
+        ax.set_title(f"{clabel.split('[')[0].strip()} ({film!r})")
+        ax.set_aspect("equal")
+        ax.set_xlabel(f"$x$ [${length_units:~L}$]")
+        ax.set_ylabel(f"$y$ [${length_units:~L}$]")
+        ax.set_xlim(*make_lims(x, buffer=0.05))
+        ax.set_ylim(*make_lims(y, buffer=0.05))
+        used_axes.append(ax)
+        if cross_section_coords is not None:
+            ax_divider = make_axes_locatable(ax)
+            cax = ax_divider.append_axes("bottom", size="40%", pad="30%")
+            coords, paths, cross_sections = cross_section(
+                np.stack([x, y]).T,
+                field,
+                cross_section_coords=cross_section_coords,
+            )
+            for i, (coord, path, cross) in enumerate(
+                zip(coords, paths, cross_sections)
+            ):
+                color = f"C{i % 10}"
+                ax.plot(*coord.T, "--", color=color, lw=2)
+                ax.plot(*coord[0], "o", color=color)
+                ax.plot(*coord[-1], "s", color=color)
+                cax.plot(path, cross, color=color, lw=2)
+                cax.plot(path[0], cross[0], "o", color=color)
+                cax.plot(path[-1], cross[-1], "s", color=color)
+            cax.grid(True)
+            cax.set_xlabel(f"Distance along cut [${length_units:~L}$]")
+            cax.set_ylabel(clabel)
+            used_axes.append(cax)
+        if colorbar:
+            cbar = fig.colorbar(im, ax=ax, orientation="vertical")
+            cbar.set_label(clabel)
+            used_axes.append(cbar.ax)
+    for ax in fig.axes:
+        if ax not in used_axes:
+            fig.delaxes(ax)
+    return fig, axes
+
+
+def plot_currents(
+    solution: Solution,
+    films: Optional[Union[List[str], str]] = None,
+    units: Optional[str] = None,
+    max_cols: int = 3,
+    cmap: str = "inferno",
+    colorbar: bool = True,
+    shading: Literal["flat", "gouraud"] = "flat",
+    auto_range_cutoff: Optional[Union[float, Tuple[float, float]]] = None,
+    share_color_scale: bool = False,
+    symmetric_color_scale: bool = False,
+    vmin: Optional[float] = None,
+    vmax: Optional[float] = None,
+    streamplot: bool = True,
+    grid_shape: Union[int, Tuple[int, int]] = (200, 200),
+    min_stream_amp: float = 0.025,
+    cross_section_coords: Optional[Union[np.ndarray, Sequence[np.ndarray]]] = None,
+    **kwargs,
+) -> Tuple[plt.Figure, np.ndarray]:
+    """Plots the sheet current density for one or more films in a Device.
 
-    3. Repeat step 2 (iterations - 1) times.
+    Additional keyword arguments are passed to plt.subplots().
 
     Args:
-        device: The Device to simulate.
-        applied_field: A callable that computes the applied magnetic field
-            as a function of x, y, z coordinates.
-        terminal_currents: A dict of ``{source_name: source_current}`` for
-            each source terminal. This argument is only allowed if ``device``
-            as an instance of ``TransportDevice``.
-        circulating_currents: A dict of ``{hole_name: circulating_current}``.
-            If circulating_current is a float, then it is assumed to be in units
-            of current_units. If circulating_current is a string, then it is
-            converted to a pint.Quantity.
-        vortices: A list of Vortex objects located in the Device.
-        field_units: Units of the applied field. Can either be magnetic field H
-            or magnetic flux density B = mu0 * H.
-        current_units: Units to use for current quantities. The applied field will be
-            converted to units of [current_units / device.length_units].
-        check_inversion: Whether to verify the accuracy of the matrix inversion.
-        iterations: Number of times to compute the interactions between layers.
-        return_solutions: Whether to return a list of Solution objects.
-        directory: If not None, resulting Solutions will be saved in this directory.
-        cache_memory_cutoff: If the memory needed for layer-to-layer kernel
-            matrices exceeds ``cache_memory_cutoff`` times the current available
-            system memory, then the kernel matrices will be cached to disk rather than
-            in memory. Setting this value to ``inf`` disables caching to disk. In this
-            case, the arrays will remain in memory unless they are swapped to disk
-            by the operating system.
-        log_level: Logging level to use, if any.
-        gpu: Solve on a GPU if available (requires JAX and CUDA).
-        _solver: Name of the solver method used.
+        solution: The Solution from which to extract sheet current.
+        films: Name(s) of film(s) for which to plot the sheet current.
+            By default, the sheet current is plotted for all films in the Device.
+        units: Units in which to plot the current density. Defaults to
+            solution.current_units / solution.device.length_units.
+        max_cols: Maximum number of columns in the grid of subplots.
+        cmap: Name of the matplotlib colormap to use.
+        colorbar: Whether to add a colorbar to each subplot.
+        shading: May be ``"flat"`` or ``"gouraud"``. The latter does some interpolation.
+        auto_range_cutoff: Cutoff percentile for ``auto_range_iqr``.
+        share_color_scale: Whether to force all layers to use the same color scale.
+        symmetric_color_scale: Whether to use a symmetric color scale (vmin = -vmax).
+        vmin: Color scale minimum to use for all layers
+            (ignored if share_color_scale is True).
+        vmax: Color scale maximum to use for all layers
+            (ignored if share_color_scale is True).
+        streamplot: Whether to overlay current streamlines on the plot.
+        grid_shape: Shape of the rectangular grid used to contruct streamlines.
+            If a single integer N is given, the grid will be square, shape = (N, N).
+        min_stream_amp: Streamlines will not be drawn anywhere the
+            current density is less than min_stream_amp * max(current_density).
+            This avoids streamlines being drawn where there is no current flowing.
+        cross_section_coords: Shape (m, 2) array of (x, y) coordinates for a
+            cross-section (or a list of such arrays).
 
     Returns:
-        If ``return_solutions`` is True, returns a list of Solutions of
-        length ``iterations + 1``.
+        matplotlib figure and axes
     """
+    device = solution.device
+    length_units = device.ureg(device.length_units).units
+    old_units = device.ureg(f"{solution.current_units} / {device.length_units}").units
+    units = units or old_units
+    if isinstance(units, str):
+        units = device.ureg(units).units
+    if films is None:
+        films = list(device.films)
+    if isinstance(films, str):
+        films = [films]
+    if isinstance(grid_shape, int):
+        grid_shape = (grid_shape, grid_shape)
+    fig, axes = auto_grid(len(films), max_cols=max_cols, **kwargs)
+
+    jcs = {}
+    Js = {}
+    for film_name, film_solution in solution.film_solutions.items():
+        jc = film_solution.current_density
+        jc = (jc * old_units).to(units).magnitude
+        jcs[film_name] = jc
+        Js[film_name] = np.linalg.norm(jc, axis=1)
+
+    clabel = "$|\\,\\vec{J}\\,|$" + f" [${units:~L}$]"
+    clim_dict = setup_color_limits(
+        Js,
+        vmin=vmin,
+        vmax=vmax,
+        share_color_scale=share_color_scale,
+        symmetric_color_scale=symmetric_color_scale,
+        auto_range_cutoff=auto_range_cutoff,
+    )
+    # Keep track of which axes are actually used,
+    # and delete unused axes later
+    used_axes = []
+    holes_by_film = device.holes_by_film()
+    for ax, film_name in zip(fig.axes, films):
+        film = device.films[film_name]
+        Jx, Jy = jcs[film_name].T
+        J = Js[film_name]
+        mesh = device.meshes[film_name]
+        x, y = mesh.sites.T
+        tri = mesh.elements
+        layer_vmin, layer_vmax = clim_dict[film_name]
+        norm = mpl.colors.Normalize(vmin=layer_vmin, vmax=layer_vmax)
+        im = ax.tripcolor(x, y, J, triangles=tri, shading=shading, cmap=cmap, norm=norm)
+        ax.set_title(f"{clabel.split('[')[0].strip()} ({film_name})")
+        ax.set_aspect("equal")
+        ax.set_xlabel(f"$x$ [${length_units:~L}$]")
+        ax.set_ylabel(f"$y$ [${length_units:~L}$]")
+        ax.set_xlim(*make_lims(x, buffer=0.05))
+        ax.set_ylim(*make_lims(y, buffer=0.05))
+        used_axes.append(ax)
+        if cross_section_coords is not None:
+            ax_divider = make_axes_locatable(ax)
+            cax = ax_divider.append_axes("bottom", size="40%", pad="30%")
+            coords, paths, cross_sections = cross_section(
+                np.array([x, y]).T, J, cross_section_coords
+            )
+            for i, (coord, path, cross) in enumerate(
+                zip(coords, paths, cross_sections)
+            ):
+                cross[~film.contains_points(coord)] *= 0
+                color = f"C{i % 10}"
+                ax.plot(*coord.T, "--", color=color, lw=2)
+                ax.plot(*coord[0], "o", color=color)
+                ax.plot(*coord[-1], "s", color=color)
+                cax.plot(path, cross, color=color, lw=2)
+                cax.plot(path[0], cross[0], "o", color=color)
+                cax.plot(path[-1], cross[-1], "s", color=color)
+            cax.grid(True)
+            cax.set_xlabel(f"Distance along cut [${length_units:~L}$]")
+            cax.set_ylabel(clabel)
+            used_axes.append(cax)
+        if streamplot:
+            xy = np.array([x, y]).T
+            xgrid, ygrid = np.meshgrid(
+                np.linspace(x.min(), x.max(), grid_shape[1]),
+                np.linspace(y.min(), y.max(), grid_shape[0]),
+            )
+            # Create masks to set the current density to zero in holes
+            # and outside of films.
+            coords = np.array([xgrid.ravel(), ygrid.ravel()]).T
+            film_mask = film.contains_points(coords)
+            for hole in holes_by_film[film_name]:
+                film_mask = film_mask & ~hole.contains_points(coords)
+            film_mask = film_mask.reshape(xgrid.shape)
+            Jx_grid = interpolate.griddata(xy, Jx, (xgrid, ygrid), method="linear")
+            Jy_grid = interpolate.griddata(xy, Jy, (xgrid, ygrid), method="linear")
+            Jx_grid[~film_mask] = np.nan
+            Jy_grid[~film_mask] = np.nan
+            J_grid = np.sqrt(Jx_grid**2 + Jy_grid**2)
+            if min_stream_amp is not None:
+                cutoff = np.nanmax(J_grid) * min_stream_amp
+                Jx_grid[J_grid < cutoff] = np.nan
+                Jy_grid[J_grid < cutoff] = np.nan
+            ax.streamplot(
+                xgrid, ygrid, Jx_grid, Jy_grid, color="w", density=1, linewidth=0.75
+            )
+        if colorbar:
+            cbar = fig.colorbar(im, ax=ax, orientation="vertical")
+            cbar.set_label(clabel)
+            used_axes.append(cbar.ax)
+    for ax in fig.axes:
+        if ax not in used_axes:
+            fig.delaxes(ax)
+    return fig, axes
+
+
+def plot_field_at_positions(
+    solution: Solution,
+    positions: Union[np.ndarray, Mesh],
+    zs: Optional[Union[float, np.ndarray]] = None,
+    units: Optional[str] = None,
+    shading: Literal["flat", "gouraud"] = "gouraud",
+    cmap: str = "cividis",
+    colorbar: bool = True,
+    auto_range_cutoff: Optional[Union[float, Tuple[float, float]]] = None,
+    share_color_scale: bool = False,
+    symmetric_color_scale: bool = False,
+    vmin: Optional[float] = None,
+    vmax: Optional[float] = None,
+    cross_section_coords: Optional[Union[float, List[float]]] = None,
+    **kwargs,
+) -> Tuple[plt.Figure, plt.Axes]:
+    """Plots the total field (either all three components or just the
+    z component) anywhere in space.
 
-    if log_level is not None:
-        logging.basicConfig(level=log_level)
+    Additional keyword arguments are passed to plt.subplots().
 
-    if directory is not None:
-        os.makedirs(directory, exist_ok=True)
+    Args:
+        solution: The Solution from which to extract fields.
+        positions: Shape (m, 2) array of (x, y) coordinates, or (m, 3) array of (x, y, z)
+            coordinates at which to calculate the magnetic field. A single list like [x, y]
+            or [x, y, z] is also allowed.
+        zs: z coordinates at which to calculate the field. If positions has shape (m, 3), then
+            this argument is not allowed. If zs is a scalar, then the fields are calculated in
+            a plane parallel to the x-y plane. If zs is any array, then it must be same length
+            as positions.
+        units: Units in which to plot the fields. Defaults to solution.field_units.
+            This argument is ignored if normalize is True.
+        shading: May be ``"flat"`` or ``"gouraud"``. The latter does some interpolation.
+        max_cols: Maximum number of columns in the grid of subplots.
+        cmap: Name of the matplotlib colormap to use.
+        colorbar: Whether to add a colorbar to each subplot.
+        auto_range_cutoff: Cutoff percentile for ``auto_range_iqr``.
+        share_color_scale: Whether to force all layers to use the same color scale.
+        symmetric_color_scale: Whether to use a symmetric color scale (vmin = -vmax).
+        vmin: Color scale minimum to use for all layers
+        vmax: Color scale maximum to use for all layers
+        cross_section_coords: Shape (m, 2) array of (x, y) coordinates for a
+            cross-section (or a list of such arrays).
 
-    if device.points is None:
-        raise ValueError(
-            "The device does not have a mesh. Call device.make_mesh() to generate it."
-        )
-    if device.weights is None or device.Del2 is None:
-        raise ValueError(
-            "The device does not have a Laplace operator. "
-            "Call device.compute_matrices() to calculate it."
-        )
-    if gpu:
-        if not HAS_JAX:
-            raise ValueError("Running solve(..., gpu=True) requires JAX.")
-        jax_device = jax.devices()[0]
-        logger.info(f"Using JAX with device {jax_device}.")
-        if "cpu" in jax_device.device_kind:
-            logger.warning("No GPU found. Using JAX on the CPU.")
-            _solver = _solver + ":jax:cpu"
-        else:
-            _solver = _solver + ":jax:gpu"
-        dtype = np.float32
+    Returns:
+        matplotlib figure and axes
+    """
+    device = solution.device
+    # Length units from the Device
+    length_units = device.ureg(device.length_units).units
+    # The units the fields are currently in
+    old_units = device.ureg(solution.field_units).units
+    # The units we want to convert to
+    if units is None:
+        units = old_units
+    if isinstance(units, str):
+        units = device.ureg(units).units
+
+    if isinstance(positions, Mesh):
+        if zs is None:
+            raise ValueError("zs must be given if positions is Mesh.")
+        mesh = positions
+        positions = mesh.sites
+        triangles = mesh.elements
     else:
-        dtype = device.solve_dtype
+        triangles = None
 
-    # Convert all circulating and terminal currents to floats.
-    def current_to_float(value):
-        if isinstance(value, str):
-            value = device.ureg(value)
-        if isinstance(value, pint.Quantity):
-            value = value.to(current_units).magnitude
-        return value
-
-    circulating_currents = circulating_currents or {}
-    _circ_currents = circulating_currents.copy()
-    circulating_currents = {}
-    for name, current in _circ_currents.items():
-        circulating_currents[name] = current_to_float(current)
-    terminal_currents = terminal_currents or {}
-    _term_currents = terminal_currents.copy()
-    terminal_currents = {}
-    for name, current in _term_currents.items():
-        terminal_currents[name] = current_to_float(current)
-
-    points = device.points.astype(dtype, copy=False)
-    weights = device.weights.astype(dtype, copy=False)
-    Q = device.Q.astype(dtype, copy=False)
-    if weights.ndim == 1:
-        # Shape (n, ) --> (n, 1)
-        weights = weights[:, np.newaxis]
-    Del2 = device.Del2
-    gradx = device.gradx
-    grady = device.grady
-    if sp.issparse(Del2):
-        Del2 = Del2.toarray().astype(dtype, copy=False)
-    if sp.issparse(gradx):
-        gradx = gradx.toarray().astype(dtype, copy=False)
-    if sp.issparse(grady):
-        grady = grady.toarray().astype(dtype, copy=False)
-    grad = np.stack([gradx, grady], axis=0)
-
-    if gpu:
-        weights = jax.device_put(weights)
-        Del2 = jax.device_put(Del2)
-        grad = jax.device_put(grad)
-        Q = jax.device_put(Q)
-        grad = jax.device_put(grad)
-
-    solutions = []
-    streams = {}
-    currents = {}
-    fields = {}
-    screening_fields = {}
-    applied_field = applied_field or ConstantField(0)
-    vortices = vortices or []
-
-    field_conversion = field_conversion_factor(
-        field_units,
-        current_units,
-        length_units=device.length_units,
-        ureg=device.ureg,
+    field = solution.field_at_position(
+        positions,
+        zs=zs,
+        units=units,
+        with_units=False,
     )
-    logger.debug(
-        f"Conversion factor from {device.ureg(field_units).units:~P} to "
-        f"{device.ureg(current_units) / device.ureg(device.length_units):~P}: "
-        f"{field_conversion:~P}."
+    fig, ax = plt.subplots(**kwargs)
+    x, y, *_ = positions.T
+    clabel = f"$H_z$  [${units:~L}$]"
+    if "[mass]" in units.dimensionality:
+        # We want flux density, B = mu0 * H
+        clabel = "$\\mu_0$" + clabel
+    clim = setup_color_limits(
+        {"field": field},
+        vmin=vmin,
+        vmax=vmax,
+        share_color_scale=share_color_scale,
+        symmetric_color_scale=symmetric_color_scale,
+        auto_range_cutoff=auto_range_cutoff,
+    )["field"]
+    layer_vmin, layer_vmax = clim
+    norm = mpl.colors.Normalize(vmin=layer_vmin, vmax=layer_vmax)
+    im = ax.tripcolor(
+        x, y, field, triangles=triangles, shading=shading, cmap=cmap, norm=norm
     )
-    field_conversion_magnitude = field_conversion.magnitude
-    # Only compute the applied field and Lambda once.
-    layer_fields = {}
-    layer_Lambdas = {}
-    for name, layer in device.layers.items():
-        # Units: current_units / device.length_units
-        layer_field = (
-            applied_field(device.points[:, 0], device.points[:, 1], layer.z0)
-            * field_conversion_magnitude
-        ).astype(dtype, copy=False)
-        # Check and cache penetration depth
-        london_lambda = layer.london_lambda
-        d = layer.thickness
-        Lambda = layer.Lambda
-        if isinstance(london_lambda, (int, float)) and london_lambda <= d:
-            length_units = device.ureg(device.length_units).units
-            logger.warning(
-                f"Layer '{name}': The film thickness, d = {d:.4f} {length_units:~P}"
-                f", is greater than or equal to the London penetration depth, resulting "
-                f"in an effective penetration depth {Lambda_str} = {Lambda:.4f} "
-                f"{length_units:~P} <= {lambda_str} = {london_lambda:.4f} {length_units:~P}. "
-                f"The assumption that the current density is nearly constant over the "
-                f"thickness of the film may not be valid. "
-            )
-        if isinstance(Lambda, (int, float)):
-            Lambda = Constant(Lambda)
-        Lambda = Lambda(device.points[:, 0], device.points[:, 1]).astype(
-            dtype, copy=False
-        )[:, np.newaxis]
-        if london_lambda is not None:
-            if isinstance(london_lambda, (int, float)):
-                london_lambda = Constant(london_lambda)
-            london_lambda = london_lambda(
-                device.points[:, 0], device.points[:, 1]
-            ).astype(dtype, copy=False)[:, np.newaxis]
-        if gpu:
-            layer_field = jax.device_put(layer_field)
-            Lambda = jax.device_put(Lambda)
-            if london_lambda is not None:
-                london_lambda = jax.device_put(london_lambda)
-        layer_fields[name] = layer_field
-        layer_Lambdas[name] = LambdaInfo(
-            layer=name,
-            Lambda=Lambda,
-            london_lambda=london_lambda,
-            thickness=layer.thickness,
+    ax.set_title(f"{clabel.split('[')[0].strip()}")
+    ax.set_aspect("equal")
+    ax.set_xlabel(f"$x$ [${length_units:~L}$]")
+    ax.set_ylabel(f"$y$ [${length_units:~L}$]")
+    ax.set_xlim(x.min(), x.max())
+    ax.set_ylim(y.min(), y.max())
+    if cross_section_coords is not None:
+        ax_divider = make_axes_locatable(ax)
+        cax = ax_divider.append_axes("bottom", size="40%", pad="30%")
+        coords, paths, cross_sections = cross_section(
+            np.array([x, y]).T,
+            field,
+            cross_section_coords=cross_section_coords,
         )
+        for i, (coord, path, cross) in enumerate(zip(coords, paths, cross_sections)):
+            color = f"C{i % 10}"
+            ax.plot(*coord.T, "--", color=color, lw=2)
+            ax.plot(*coord[0], "o", color=color)
+            ax.plot(*coord[-1], "s", color=color)
+            cax.plot(path, cross, color=color, lw=2)
+            cax.plot(path[0], cross[0], "o", color=color)
+            cax.plot(path[-1], cross[-1], "s", color=color)
+        cax.grid(True)
+        cax.set_xlabel(f"Distance along cut [${length_units:~L}$]")
+        cax.set_ylabel(clabel)
+    if colorbar:
+        cbar = fig.colorbar(im, ax=ax, orientation="vertical")
+        cbar.set_label(clabel)
+    return fig, ax
+
+
+def plot_mutual_inductance(
+    M: Union[np.ndarray, List[np.ndarray]],
+    diff: bool = False,
+    iteration_offset: int = 0,
+    absolute: bool = False,
+    ax: Optional[plt.Axes] = None,
+    figsize: Optional[Tuple[float, float]] = None,
+    logy: bool = False,
+    grid: bool = True,
+    legend: bool = True,
+    **kwargs,
+) -> Tuple[plt.Figure, plt.Axes]:
+    """Plot the convergence vs. iteration of a set of mutual inductance matrices,
+    given by the output of :meth:`superscreen.Device.mutual_inductance_matrix`
+    with ``all_iterations=True``.
 
-    vortices_by_layer = defaultdict(list)
-    for vortex in vortices:
-        if not isinstance(vortex, Vortex):
-            raise TypeError(f"Expected a Vortex, but got {type(vortex)}.")
-        if vortex.layer not in device.layers:
-            raise ValueError(f"Vortex located in unknown layer: {vortex}.")
-        films_in_layer = [f for f in device.films.values() if f.layer == vortex.layer]
-        holes_in_layer = [h for h in device.holes.values() if h.layer == vortex.layer]
-        if not any(
-            film.contains_points([vortex.x, vortex.y]) for film in films_in_layer
-        ):
-            raise ValueError(f"Vortex {vortex} is not located in a film.")
-        if any(hole.contains_points([vortex.x, vortex.y]) for hole in holes_in_layer):
-            raise ValueError(f"Vortex {vortex} is located in a hole.")
-        vortices_by_layer[vortex.layer].append(vortex)
-
-    # Compute the stream functions and fields for each layer
-    # given only the applied field.
-    for name, layer in device.layers.items():
-        logger.info(f"Calculating {name} response to applied field.")
-        g, J, total_field, screening_field = solve_layer(
-            device=device,
-            layer=name,
-            applied_field=layer_fields[name],
-            kernel=Q,
-            terminal_currents=terminal_currents,
-            circulating_currents=circulating_currents,
-            vortices=vortices_by_layer[name],
-            weights=weights,
-            Del2=Del2,
-            grad=grad,
-            Lambda_info=layer_Lambdas[name],
-            current_units=current_units,
-            check_inversion=check_inversion,
-            gpu=gpu,
-        )
-        # Units: current_units
-        streams[name] = g.astype(dtype)
-        # Units: currents_units / device.length_units
-        currents[name] = J.astype(dtype, copy=False)
-        # Units: current_units / device.length_units
-        fields[name] = total_field.astype(dtype, copy=False)
-        screening_fields[name] = screening_field.astype(dtype, copy=False)
-
-    solution = Solution(
-        device=device,
-        streams={
-            layer: np.asarray(stream, dtype=dtype) for layer, stream in streams.items()
-        },
-        current_densities=currents,
-        fields={
-            # Units: field_units
-            layer: (field / field_conversion_magnitude).astype(dtype, copy=False)
-            for layer, field in fields.items()
-        },
-        screening_fields={
-            # Units: field_units
-            layer: (field / field_conversion_magnitude).astype(dtype, copy=False)
-            for layer, field in screening_fields.items()
-        },
-        applied_field=applied_field,
-        field_units=field_units,
-        current_units=current_units,
-        circulating_currents=circulating_currents,
-        terminal_currents=terminal_currents,
-        vortices=vortices,
-        solver=_solver,
-    )
-    if directory is not None:
-        solution.to_file(os.path.join(directory, str(0)))
-    if return_solutions:
-        solutions.append(solution)
-    else:
-        del solution
+    Args:
+        M: A length ``m`` list of shape ``(n, n)`` mutual inductance matrices, or
+            a shape ``(m, n, n)`` array representing the same.
+        diff: If True, plots the difference in mutual inductance between subsequent
+            iterations.
+        iteration_offset: The first iteration (index in ``M``) to consider when
+            calculating convergence.
+        absolute: If True (and diff is True), plots the absolute change in mutual
+            inductance vs. iteration, otherwise plots relative change.
+        ax: Matplotlib Axes instance on which to plot.
+        figsize: Matplotlib figure size to create if ``ax`` is None.
+        logy: If True, sets the y axis scaling to logarithmic.
+        grid: If True, turns on plot grid lines.
+        legend: If True, adds a legend to the plot.
+        kwargs: Passed to ``ax.plot()``.
 
-    layer_names = list(device.layers)
-    nlayers = len(layer_names)
-    if nlayers < 2 or iterations < 1:
-        if return_solutions:
-            return solutions
-        return
-    rho2 = distance.cdist(points, points, metric="sqeuclidean").astype(
-        dtype,
-        copy=False,
-    )
-    # Cache kernel matrices.
-    kernels = {}
-    if cache_memory_cutoff is None:
-        cache_memory_cutoff = np.inf
-    if cache_memory_cutoff < 0:
-        raise ValueError(
-            f"Kernel cache memory cutoff must be greater than zero "
-            f"(got {cache_memory_cutoff})."
-        )
-    nkernels = nlayers * (nlayers - 1) // 2
-    total_bytes = nkernels * rho2.nbytes
-    available_bytes = psutil.virtual_memory().available
-    if total_bytes > cache_memory_cutoff * available_bytes:
-        # Save kernel matrices to disk to avoid filling up memory.
-        cache_kernels_to_disk = True
-        context = tempfile.TemporaryDirectory()
-    else:
-        # Cache kernels in memory (much faster than saving to/loading from disk).
-        cache_kernels_to_disk = False
-        context = contextlib.nullcontext()
-    if gpu:
-        cache_kernels_to_disk = False
-        rho2 = jax.device_put(rho2)
-    with context as tempdir:
-        for i in range(iterations):
-            # Calculate the screening fields at each layer from every other layer
-            zeros = jnp.zeros if gpu else np.zeros
-            other_screening_fields = {
-                name: zeros(points.shape[0], dtype=dtype) for name in layer_names
-            }
-            for layer, other_layer in itertools.product(device.layers_list, repeat=2):
-                if layer.name == other_layer.name:
-                    continue
-                if (
-                    i == 0
-                    and layer.name == layer_names[0]
-                    and other_layer.name == layer_names[1]
-                ):
-                    logger.info(
-                        f"Caching {nkernels} layer-to-layer kernel(s) "
-                        f"({total_bytes / 1024 ** 2:.0f} MB total) "
-                        f"{'to disk' if cache_kernels_to_disk else 'in memory'}."
-                    )
-                logger.debug(
-                    f"Calculating screening field at {layer.name} "
-                    f"from {other_layer.name} ({i+1}/{iterations})."
-                )
-                g = streams[other_layer.name]
-                dz = other_layer.z0 - layer.z0
-                key = frozenset((layer.name, other_layer.name))
-                # Get the cached kernel matrix,
-                # or calculate it if it's not yet in the cache.
-                q = kernels.get(key, None)
-                if q is None:
-                    q = (2 * dz**2 - rho2) / (4 * np.pi * (dz**2 + rho2) ** (5 / 2))
-                    if cache_kernels_to_disk:
-                        fname = os.path.join(tempdir, "_".join(key))
-                        np.save(fname, q)
-                        kernels[key] = f"{fname}.npy"
-                    else:
-                        kernels[key] = q
-                elif isinstance(q, str):
-                    # Kernel was cached to disk, so load it into memory.
-                    q = np.load(q)
-                # Calculate the dipole kernel and integrate
-                # Eqs. 1-2 in [Brandt], Eqs. 5-6 in [Kirtley1], Eqs. 5-6 in [Kirtley2].
-                screening_field = q @ (weights[:, 0] * g)
-                other_screening_fields[layer.name] += screening_field
-                del q, g
-            # Solve again with the screening fields from all layers.
-            # Calculate applied fields only once per iteration.
-            new_layer_fields = {}
-            for name, layer in device.layers.items():
-                # Units: current_units / device.length_units
-                new_layer_fields[name] = (
-                    layer_fields[name] + other_screening_fields[name]
-                )
-            streams = {}
-            fields = {}
-            screening_fields = {}
-            for name, layer in device.layers.items():
-                logger.info(
-                    f"Calculating {name} response to applied field and "
-                    f"screening field from other layers ({i+1}/{iterations})."
-                )
-                g, J, total_field, screening_field = solve_layer(
-                    device=device,
-                    layer=name,
-                    applied_field=new_layer_fields[name],
-                    kernel=Q,
-                    weights=weights,
-                    Del2=Del2,
-                    grad=grad,
-                    Lambda_info=layer_Lambdas[name],
-                    circulating_currents=circulating_currents,
-                    vortices=vortices_by_layer[name],
-                    current_units=current_units,
-                    check_inversion=check_inversion,
-                    gpu=gpu,
+    Returns:
+        Matplotlib Figure and Axes.
+    """
+    if isinstance(M, list):
+        for i, item in enumerate(M):
+            is_quantity = isinstance(item, pint.Quantity) and isinstance(
+                item.magnitude, np.ndarray
+            )
+            if not (
+                is_quantity
+                or isinstance(item, np.ndarray)
+                and item.ndim == 2
+                and item.shape[0] == item.shape[1]
+            ):
+                raise ValueError(
+                    f"Element {i} of list M is not a square array: {item!r}."
                 )
-                # Units: current_units
-                streams[name] = g
-                # Units: current_units / device.length_units
-                currents[name] = J
-                # Units: current_units / device.length_units
-                fields[name] = total_field
-                screening_fields[name] = screening_field
-
-            solution = Solution(
-                device=device,
-                streams={
-                    layer: np.asarray(g, dtype=dtype) for layer, g in streams.items()
-                },
-                current_densities=currents,
-                fields={
-                    # Units: field_units
-                    layer: (np.asarray(field) / field_conversion_magnitude).astype(
-                        dtype, copy=False
-                    )
-                    for layer, field in fields.items()
-                },
-                screening_fields={
-                    # Units: field_units
-                    layer: (np.asarray(field) / field_conversion_magnitude).astype(
-                        dtype, copy=False
-                    )
-                    for layer, field in screening_fields.items()
-                },
-                applied_field=applied_field,
-                field_units=field_units,
-                current_units=current_units,
-                circulating_currents=circulating_currents,
-                terminal_currents=terminal_currents,
-                vortices=vortices,
-                solver=_solver,
+        M = np.stack(M, axis=0)
+    if isinstance(M, pint.Quantity):
+        units = f"${M.units:~L}$"
+        M = M.magnitude
+    else:
+        units = "?"
+    if not (isinstance(M, np.ndarray) and M.ndim == 3 and M.shape[1] == M.shape[2]):
+        raise ValueError(f"Expected M to be a shape (m, n, n) array, but got {M!r}.")
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize)
+    else:
+        fig = ax.figure
+    n = M.shape[1]
+    i0 = int(iteration_offset)
+    iterations = np.arange(M.shape[0])
+    plot_kwargs = kwargs.copy()
+    for i, j in itertools.product(range(n), repeat=2):
+        plot_kwargs["label"] = f"$M_{{{i}{j}}}$"
+        if diff:
+            xs = iterations[i0 + 1 :]
+            ys = np.abs(np.diff(M[i0:, i, j]))
+            if not absolute:
+                ys = ys / np.abs(M[i0 + 1 :, i, j])
+            ax.plot(xs, ys, **plot_kwargs)
+        else:
+            xs = iterations[i0:]
+            ax.plot(xs, M[i0:, i, j], **plot_kwargs)
+    if logy:
+        ax.set_yscale("log")
+    if grid:
+        ax.grid(True)
+    if legend:
+        ax.legend(bbox_to_anchor=(1, 1), loc="upper left")
+    if diff:
+        ylabel = "$\\Delta M_{{ij, k}}$"
+        if absolute:
+            title = "$\\Delta M_{{ij, k}} = |M_{{ij, k}} - M_{{ij, k-1}}|$"
+            ylabel = ylabel + f" [{units}]"
+        else:
+            title = (
+                "$\\Delta M_{{ij, k}} = "
+                "\\frac{{|M_{{ij, k}} - M_{{ij, k-1}}|}}{{|M_{{ij, k}}|}}$"
             )
-            if directory is not None:
-                solution.to_file(os.path.join(directory, str(i + 1)))
-            if return_solutions:
-                solutions.append(solution)
-            else:
-                del solution
-    if cache_kernels_to_disk:
-        context.cleanup()
-    if return_solutions:
-        return solutions
-
-
-def solve_many(
-    device: Device,
-    *,
-    parallel_method: Optional[str] = None,
-    applied_fields: Optional[Union[Parameter, List[Parameter]]] = None,
-    circulating_currents: Optional[
-        Union[
-            Dict[str, Union[float, str, pint.Quantity]],
-            List[Dict[str, Union[float, str, pint.Quantity]]],
-        ]
-    ] = None,
-    vortices: Optional[Union[List[Vortex], List[List[Vortex]]]] = None,
-    layer_updater: Optional[Callable] = None,
-    layer_update_kwargs: Optional[List[Dict[str, Any]]] = None,
-    field_units: str = "mT",
-    current_units: str = "uA",
-    check_inversion: bool = False,
-    iterations: int = 0,
-    product: bool = False,
-    directory: Optional[str] = None,
-    return_solutions: bool = False,
-    keep_only_final_solution: bool = False,
-    cache_memory_cutoff: float = np.inf,
-    log_level: int = logging.INFO,
-    use_shared_memory: bool = True,
-    num_cpus: Optional[int] = None,
-    gpu: bool = False,
-) -> Tuple[Optional[Union[List[Solution], List[List[Solution]]]], Optional[List[str]]]:
-    """Solves many models involving the same device, optionally in parallel using
-    multiple processes.
+        ax.set_title(title)
+    else:
+        ylabel = f"$M_{{ij, k}}$ [{units}]"
+    ax.set_ylabel(ylabel)
+    ax.set_xlabel("Iteration, $k$")
+    return fig, ax
+
+
+def plot_polygon_flux(
+    solutions: List[Solution],
+    diff: bool = False,
+    iteration_offset: int = 0,
+    absolute: bool = False,
+    units: Optional[str] = None,
+    ax: Optional[plt.Axes] = None,
+    figsize: Optional[Tuple[float, float]] = None,
+    logy: bool = False,
+    grid: bool = True,
+    legend: bool = True,
+    **kwargs,
+) -> Tuple[plt.Figure, plt.Axes]:
+    """Plot the convergence vs. iteration of the flux through all polygons in a Device,
+    given by the output of :meth:`superscreen.solve()`
 
     Args:
-        device: The Device to simulate.
-        parallel_method: The method to use for multiprocessing (None, "mp", or "ray").
-        applied_fields: A callable or list of callables that compute(s) the applied
-            magnetic field as a function of x, y, z coordinates.
-        circulating_currents: A dict of ``{hole_name: circulating_current}`` or list
-            of such dicts. If circulating_current is a float, then it is assumed to
-            be in units of current_units. If circulating_current is a string, then
-            it is converted to a pint.Quantity.
-        vortices: A list (list of lists) of ``Vortex`` objects.
-        layer_updater: A callable with signature
-            ``layer_updater(layer: Layer, **kwargs) -> Layer`` that updates
-            parameter(s) of each layer in a device.
-        layer_update_kwargs: A list of dicts of keyword arguments passed to
-            ``layer_updater``.
-        field_units: Units of the applied field. Can either be magnetic field H
-            or magnetic flux density B = mu0 * H.
-        current_units: Units to use for current quantities. The applied field will be
-            converted to units of [current_units / device.length_units].
-        check_inversion: Whether to verify the accuracy of the matrix inversion.
-        iterations: Number of times to compute the interactions between layers
-        product: If True, then all combinations of applied_fields,
-            circulating_currrents, and layer_update_kwargs are simulated (the
-            behavior is given by itertools.product(), i.e. a nested for loop).
-            Otherwise, the behavior is similar to zip().
-            See superscreen.parallel.create_models for more details.
-        directory: The directory in which to save the results. If None is given, then
-            the results are not automatically saved to disk.
-        return_solutions: Whether to return the Solution objects.
-        keep_only_final_solution: Whether to keep/save only the Solution from
-            the final iteration of superscreen.solve.solve for each setup.
-        cache_memory_cutoff: If the memory needed for layer-to-layer kernel
-            matrices exceeds ``cache_memory_cutoff`` times the current available
-            system memory, then the kernel matrices will be cached to disk rather than
-            in memory. Setting this value to ``inf`` disables caching to disk. In this
-            case, the arrays will remain in memory unless they are swapped to disk
-            by the operating system.
-        log_level: Logging level to use, if any.
-        use_shared_memory: Whether to use shared memory if parallel_method is not None.
-        num_cpus: The number of processes to utilize.
-        gpu: Solve on a GPU if available (requires JAX and CUDA). gpu = True is only allowed
-            for serial execution, i.e., ``parallel_method in {None, False, "serial"}``.
+        solutions: A list of ``Solutions``, one per solve iteration.
+        diff: If True, plots the difference in flux between subsequent iterations.
+        iteration_offset: The first iteration (index in ``solutions``) to consider when
+            calculating convergence.
+        absolute: If True (and diff is True), plots the absolute change in flux vs.
+            iteration, otherwise plots relative change.
+        units: The flux units to display if ``absolute`` is True.
+        ax: Matplotlib Axes instance on which to plot.
+        figsize: Matplotlib figure size to create if ``ax`` is None.
+        logy: If True, sets the y axis scaling to logarithmic.
+        grid: If True, turns on plot grid lines.
+        legend: If True, adds a legend to the plot.
+        kwargs: Passed to ``ax.plot()``.
 
     Returns:
-        solutions, paths. If return_solutions is True, solutions is either a list of
-        lists of Solutions (if keep_only_final_solution is False), or a list
-        of Solutions (the final iteration for each setup). If directory is True,
-        paths is a list of paths to the saved solutions, otherwise paths is None.
+        Matplotlib Figure and Axes.
     """
-    from . import parallel
+    device = solutions[0].device
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize)
+    else:
+        fig = ax.figure
+    if units is None:
+        units = f"{solutions[0].field_units} * {device.length_units}**2"
+    i0 = int(iteration_offset)
+    iterations = np.arange(len(solutions))
+    plot_kwargs = kwargs.copy()
+    polygons = device.get_polygons(include_terminals=False)
+    polygon_flux = defaultdict(list)
+    for solution in solutions:
+        for polygon in polygons:
+            polygon_flux[polygon.name].append(
+                solution.polygon_flux(polygon.name, units=units, with_units=False)
+            )
+    units = device.ureg(units)
+    for name, flux_vals in polygon_flux.items():
+        plot_kwargs["label"] = name
+        if diff:
+            xs = iterations[i0 + 1 :]
+            ys = np.abs(np.diff(flux_vals[i0:]))
+            if not absolute:
+                ys = ys / np.abs(flux_vals[i0 + 1 :])
+            ax.plot(xs, ys, **plot_kwargs)
+        else:
+            xs = iterations[i0:]
+            ax.plot(xs, flux_vals[i0:], **plot_kwargs)
+    if logy:
+        ax.set_yscale("log")
+    if grid:
+        ax.grid(True)
+    if legend:
+        ax.legend(bbox_to_anchor=(1, 1), loc="upper left")
+    if diff:
+        ylabel = "$\\Delta\\Phi_i$"
+        if absolute:
+            title = "$\\Delta\\Phi_i = |\\Phi_i - \\Phi_{i-1}|$"
+            ylabel = ylabel + f" [${units:~L}$]"
+        else:
+            title = "$\\Delta\\Phi_i = " "\\frac{|\\Phi_i - \\Phi_{i-1}|}{|\\Phi_{i}|}$"
+        ax.set_title(title)
+    else:
+        ylabel = f"$\\Phi_i$ [${units:~L}$]"
+    ax.set_ylabel(ylabel)
+    ax.set_xlabel("Iteration, $i$")
+    return fig, ax
 
-    parallel_methods = {
-        None: parallel.solve_many_serial,
-        False: parallel.solve_many_serial,
-        "serial": parallel.solve_many_serial,
-        "multiprocessing": parallel.solve_many_mp,
-        "mp": parallel.solve_many_mp,
-        "ray": parallel.solve_many_ray,
-    }
 
-    if parallel_method not in parallel_methods:
-        raise ValueError(
-            f"Unknown parallel method, {parallel_method}. "
-            f"Valid methods are {list(parallel_methods)}."
-        )
-    serial_methods = {None, False, "serial"}
-    if num_cpus is not None and parallel_method in serial_methods:
-        logger.warning(
-            f"Ignoring num_cpus because parallel_method = {parallel_method!r}."
+def _patch_docstring(func):
+    other_func = getattr(Solution, func.__name__)
+    other_func.__doc__ = (
+        other_func.__doc__
+        + "\n\n"
+        + "\n".join(
+            [line for line in func.__doc__.split("\n    ") if "solution:" not in line]
         )
-
-    kwargs = dict(
-        device=device,
-        applied_fields=applied_fields,
-        circulating_currents=circulating_currents,
-        vortices=vortices,
-        layer_updater=layer_updater,
-        layer_update_kwargs=layer_update_kwargs,
-        field_units=field_units,
-        current_units=current_units,
-        check_inversion=check_inversion,
-        iterations=iterations,
-        product=product,
-        directory=directory,
-        return_solutions=return_solutions,
-        keep_only_final_solution=keep_only_final_solution,
-        cache_memory_cutoff=cache_memory_cutoff,
-        log_level=log_level,
-        use_shared_memory=use_shared_memory,
-        num_cpus=num_cpus,
     )
+    annotations = func.__annotations__.copy()
+    _ = annotations.pop("solution", None)
+    other_func.__annotations__.update(annotations)
 
-    if parallel_method in serial_methods:
-        kwargs["gpu"] = gpu
-    elif gpu:
-        raise ValueError(
-            "Running solve_many() with gpu = True requires serial execution "
-            "(i.e., parallel method in {None, False, 'serial'})."
-        )
 
-    solutions, paths = parallel_methods[parallel_method](**kwargs)
-    return solutions, paths
+for func in (plot_streams, plot_currents, plot_fields, plot_field_at_positions):
+    _patch_docstring(func)
```

### Comparing `superscreen-0.8.2/superscreen/sources/constant.py` & `superscreen-0.9.0/superscreen/sources/constant.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.2/superscreen/sources/current.py` & `superscreen-0.9.0/superscreen/sources/current.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Union
 
 import numpy as np
 from scipy.constants import mu_0
 from scipy.spatial import Delaunay
 
-from ..fem import mass_matrix
+from ..device.utils import vertex_areas
+from ..distance import pairwise_difference
 from ..parameter import Parameter
 from ..units import ureg
 
 
 def biot_savart_2d(
     x: Union[float, np.ndarray],
     y: Union[float, np.ndarray],
@@ -82,21 +83,21 @@
     positions = positions * to_meter
     z0 = z0 * to_meter
     current_densities = current_densities * to_amp_per_meter
     # Calculate the pairwise distance between the current sheet and evaluation
     # points for each axis.
     x0, y0 = positions[:, 0], positions[:, 1]
     Jx, Jy = current_densities[:, 0], current_densities[:, 1]
-    dx = np.subtract.outer(x, x0)
-    dy = np.subtract.outer(y, y0)
-    dz = np.subtract.outer(z, z0 * np.ones_like(x0))
+    dx = pairwise_difference(x, x0)
+    dy = pairwise_difference(y, y0)
+    dz = pairwise_difference(z, z0 * np.ones_like(x0))
     if areas is None:
         # Triangulate the current sheet to assign an effective area to each vertex.
         triangles = Delaunay(positions).simplices
-        areas = mass_matrix(positions, triangles)
+        areas = vertex_areas(positions, triangles)
     else:
         areas = areas * to_meter**2
     # Evaluate the Biot-Savart integral.
     pref = (mu_0 / (4 * np.pi)) * areas * (dx**2 + dy**2 + dz**2) ** (-3 / 2)
     Jx_dy = np.einsum("ij, ij, j -> i", pref, dy, Jx)
     Jy_dx = np.einsum("ij, ij, j -> i", pref, dx, Jy)
     Bz = Jx_dy - Jy_dx
```

### Comparing `superscreen-0.8.2/superscreen/sources/dipole.py` & `superscreen-0.9.0/superscreen/sources/dipole.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.2/superscreen/sources/vortex.py` & `superscreen-0.9.0/superscreen/sources/vortex.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.2/superscreen/test/test_device.py` & `superscreen-0.9.0/superscreen/test/test_device.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,23 @@
-import contextlib
 import copy
+import os
 import pickle
 import tempfile
+from typing import Optional
 
+import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
-import scipy.sparse as sp
-import shapely
+from IPython.display import HTML
 
 import superscreen as sc
 from superscreen.visualization import non_gui_backend
 
 
-def test_set_polygon_points():
-    box = shapely.geometry.box(0, 0, 1, 1).exterior.coords
-    hole = shapely.geometry.box(0.25, 0.25, 0.75, 0.75, ccw=False)
-    polygon = shapely.geometry.polygon.Polygon(box, holes=[hole.exterior.coords])
-
-    with pytest.raises(ValueError):
-        _ = sc.Polygon("bad", layer="None", points=polygon)
-
-    invalid = shapely.geometry.polygon.LinearRing(
-        [(0, 0), (0, 2), (1, 1), (2, 2), (2, 0), (1, 1), (0, 0)]
-    )
-
-    with pytest.raises(ValueError):
-        _ = sc.Polygon(points=invalid)
-
-    x, y = sc.geometry.circle(1).T
-    z = np.ones_like(x)
-    points = np.stack([x, y, z], axis=1)
-    with pytest.raises(ValueError):
-        _ = sc.Polygon(points=points)
-
-
-def test_polygon_on_boundary(radius=1):
-    points = sc.geometry.circle(radius, points=501)
-    polygon = sc.Polygon(points=points)
-    Delta_x, Delta_y = polygon.extents
-    assert np.isclose(Delta_x, 2 * radius)
-    assert np.isclose(Delta_y, 2 * radius)
-
-    smaller = sc.geometry.circle(radius - 0.01)
-    bigger = sc.geometry.circle(radius + 0.01)
-    assert polygon.on_boundary(smaller, radius=0.1).all()
-    assert polygon.on_boundary(bigger, radius=0.1).all()
-    assert not polygon.on_boundary(smaller, radius=0.001).any()
-    assert not polygon.on_boundary(bigger, radius=0.001).any()
-    assert issubclass(polygon.on_boundary(smaller, index=True).dtype.type, np.integer)
-
-
-def test_polygon_join():
-    square1 = sc.Polygon(points=sc.geometry.box(1))
-    square2 = sc.Polygon(points=sc.geometry.translate(sc.geometry.box(1), 0.5, 0.5))
-    square3 = sc.geometry.box(1, center=(-0.25, 0.25))
-    name = "name"
-    layer = "layer"
-    for items in (
-        [square1, square2, square3],
-        [square1.points, square2.points, square3],
-        [square1.polygon, square2.polygon, square3],
-    ):
-        _ = sc.Polygon.from_union(items, name=name, layer=layer)
-        _ = sc.Polygon.from_difference(items, name=name, layer=layer)
-        _ = sc.Polygon.from_intersection(items, name=name, layer=layer)
-
-    assert (
-        square1.union(square2, square3).polygon
-        == sc.Polygon.from_union(items, name=name, layer=layer).polygon
-    )
-
-    assert (
-        square1.intersection(square2, square3).polygon
-        == sc.Polygon.from_intersection(items, name=name, layer=layer).polygon
-    )
-
-    assert (
-        square1.difference(square2, square3).polygon
-        == sc.Polygon.from_difference(items, name=name, layer=layer).polygon
-    )
-
-    square1.layer = square2.layer = None
-    with pytest.raises(ValueError):
-        _ = sc.Polygon.from_difference([square1, square1], name=name, layer=layer)
-
-    with pytest.raises(ValueError):
-        _ = square1._join_via(square2, "invalid")
-
-    with pytest.raises(ValueError):
-        _ = sc.Polygon.from_difference(
-            [square1, square2],
-            name=name,
-            layer=layer,
-            symmetric=True,
-        )
-
-    assert square1.resample(False) == square1
-    assert square1.resample(None).points.shape == square1.points.shape
-    assert square1.resample(71).points.shape != square1.points.shape
-
-    with pytest.raises(ValueError):
-        bowtie = [(0, 0), (0, 2), (1, 1), (2, 2), (2, 0), (1, 1), (0, 0)]
-        _ = sc.Polygon(name="bowtie", layer="layer", points=bowtie)
-
-    with pytest.raises(ValueError):
-        square1.name = None
-        sc.Device._validate_polygons([square1], "label")
-
-    for min_points, smooth in [(0, 0), (500, 0), (500, 10)]:
-        points, triangles = square1.make_mesh(min_points=min_points, smooth=smooth)
-        if min_points:
-            assert points.shape[0] > min_points
-
-
-def test_plot_polygon():
-    with non_gui_backend():
-        ax = sc.Polygon("square1", layer="layer", points=sc.geometry.box(1)).plot()
-        assert isinstance(ax, plt.Axes)
-
-
 @pytest.fixture(scope="module")
 def device():
     layers = [
         sc.Layer("layer0", london_lambda=1, thickness=0.1, z0=0),
         sc.Layer("layer1", london_lambda=2, thickness=0.05, z0=0.5),
     ]
 
@@ -149,17 +43,17 @@
         films[0].contains_points([[0, 0], [2, 1]], index=True), np.array([0, 1])
     )
     assert np.isclose(films[0].area, np.pi * 5**2, rtol=1e-3)
     assert np.isclose(films[1].area, np.pi * 3 * 2, rtol=1e-3)
 
     abstract_regions = [
         sc.Polygon(
-            "bounding_box",
+            "abstract",
             layer="layer0",
-            points=sc.geometry.box(12, angle=90),
+            points=sc.geometry.box(5, angle=90),
         ),
     ]
 
     with pytest.raises(ValueError):
         device = sc.Device(
             "device",
             layers=layers[:1],
@@ -175,19 +69,17 @@
         holes=holes,
         abstract_regions=abstract_regions,
     )
 
     with pytest.raises(AttributeError):
         device.layers["layer0"].Lambda = 0
     with pytest.raises(ValueError):
-        device.compute_matrices()
-    with pytest.raises(ValueError):
         device.solve_dtype = "int64"
 
-    assert device.get_arrays() is None
+    assert device.meshes is None
 
     with pytest.raises(TypeError):
         device.scale(xfact=-1, origin="center")
     with pytest.raises(TypeError):
         device.rotate(90, origin="centroid")
 
     assert isinstance(device.scale(xfact=-1), sc.Device)
@@ -195,16 +87,23 @@
     assert isinstance(device.rotate(90), sc.Device)
     assert isinstance(device.mirror_layers(about_z=0), sc.Device)
     dx = 1
     dy = -1
     dz = 1
     assert isinstance(device.translate(dx, dy, dz=dz), sc.Device)
     d = device.copy()
+    assert d == device
     assert d.translate(dx, dy, dz=dz, inplace=True) is d
 
+    with d.translation(-dx, -dy, dz=-dz):
+        assert d == device
+
+    assert device.mesh_stats_dict() is None
+    assert device.mesh_stats() is None
+
     return device
 
 
 def test_layer_bad_init():
     with pytest.raises(ValueError):
         _ = sc.Layer("layer0", Lambda=10, london_lambda=1, thickness=0.1, z0=0)
 
@@ -246,101 +145,88 @@
     device = sc.Device(
         "device",
         layers=layers,
         films=films,
         holes=holes,
         abstract_regions=abstract_regions,
     )
-    assert device.vertex_distances is None
-    assert device.triangle_areas is None
+    assert device.meshes is None
     device.make_mesh(min_points=3000)
-    assert isinstance(device.vertex_distances, np.ndarray)
-    assert isinstance(device.triangle_areas, np.ndarray)
-    centroids = sc.fem.centroids(device.points, device.triangles)
-    assert centroids.shape[0] == device.triangles.shape[0]
+    assert isinstance(device.meshes, dict)
+    assert set(device.meshes) == set(device.films)
+    assert all(isinstance(mesh, sc.device.Mesh) for mesh in device.meshes.values())
+    for mesh in device.meshes.values():
+        centroids = sc.fem.centroids(mesh.sites, mesh.elements)
+        assert centroids.shape[0] == mesh.elements.shape[0]
 
     print(device)
     assert device == device
     assert all(film == film for film in films)
     assert all(layer == layer for layer in layers)
     assert films[0] != layers[0]
     assert layers[0] != films[0]
     assert layers[0] == layers[0].copy()
     assert layers[0] is not layers[0].copy()
     assert films[0] == films[0].copy()
     assert films[0] is not films[0].copy()
     assert device != layers[0]
-    with pytest.raises(TypeError):
-        device.layers = []
-    with pytest.raises(TypeError):
-        device.films = []
-    with pytest.raises(TypeError):
-        device.holes = []
-    with pytest.raises(TypeError):
-        device.abstract_regions = []
     device.layers["layer1"].Lambda = sc.Constant(3)
 
     assert (
         copy.deepcopy(device)
         == copy.copy(device)
-        == device.copy(with_arrays=True)
+        == device.copy(with_mesh=True)
         == device
     )
 
     d = device.scale(xfact=-1)
     assert isinstance(d, sc.Device)
-    assert d.points is None
+    assert d.meshes is None
     d = device.scale(yfact=-1)
     assert isinstance(d, sc.Device)
-    assert d.points is None
+    assert d.meshes is None
     d = device.rotate(90)
     assert isinstance(d, sc.Device)
-    assert d.points is None
+    assert d.meshes is None
     d = device.mirror_layers(about_z=-1)
     assert isinstance(d, sc.Device)
-    assert np.array_equal(d.points, device.points)
+    assert d.meshes is None
     dx = 1
     dy = -1
     dz = 1
     assert isinstance(device.translate(dx, dy, dz=dz), sc.Device)
-    d = device.copy(with_arrays=True, copy_arrays=True)
-    assert d.translate(dx, dy, dz=dz, inplace=True) is d
-
-    for points in ("poly_points", "points"):
-        x0, y0 = getattr(device, points).mean(axis=0)
-        z0s = {layer.name: layer.z0 for layer in layers}
-        with device.translation(dx, dy, dz=dz):
-            x, y = getattr(device, points).mean(axis=0)
-            assert np.isclose(x, x0 + dx)
-            assert np.isclose(y, y0 + dy)
-            for layer in device.layers.values():
-                assert np.isclose(layer.z0, z0s[layer.name] + dz)
-        x, y = getattr(device, points).mean(axis=0)
-        assert np.isclose(x, x0)
-        assert np.isclose(y, y0)
-        for layer in device.layers.values():
-            assert np.isclose(layer.z0, z0s[layer.name])
-
+    d = device.copy(with_mesh=True, copy_mesh=True)
+    assert isinstance(device.mesh_stats_dict(), dict)
+    assert isinstance(device.mesh_stats(), HTML)
     return device
 
 
 @pytest.mark.parametrize("subplots", [False, True])
 @pytest.mark.parametrize("legend", [False, True])
-def test_plot_device(device, device_with_mesh, legend, subplots, mesh=True):
+@pytest.mark.parametrize("show_sites", [False, True])
+@pytest.mark.parametrize("show_edges", [False, True])
+def test_plot_device(
+    device: sc.Device,
+    device_with_mesh: sc.Device,
+    legend: bool,
+    subplots: bool,
+    show_sites: bool,
+    show_edges: bool,
+):
     with non_gui_backend():
-        fig, axes = device.plot(legend=legend, subplots=subplots)
+        fig, axes = device.plot_polygons(legend=legend, subplots=subplots)
         if subplots:
             assert isinstance(axes, np.ndarray)
             assert all(isinstance(ax, plt.Axes) for ax in axes.flat)
             with pytest.raises(ValueError):
                 fig, ax = plt.subplots()
-                _ = device.plot(ax=ax, subplots=subplots)
-        with pytest.raises(RuntimeError):
-            _ = device.plot(legend=legend, subplots=subplots, mesh=mesh)
-        fig, axes = device_with_mesh.plot(legend=legend, subplots=subplots, mesh=mesh)
+                _ = device.plot_polygons(ax=ax, subplots=subplots)
+        fig, axes = device_with_mesh.plot_mesh(
+            subplots=subplots, show_sites=show_sites, show_edges=show_edges
+        )
         plt.close("all")
 
 
 @pytest.mark.parametrize("subplots", [False, True])
 @pytest.mark.parametrize("legend", [False, True])
 def test_draw_device(device, legend, subplots):
     with non_gui_backend():
@@ -367,83 +253,83 @@
             layers=[sc.Layer("layer", Lambda=0, z0=0)],
             films=[sc.Polygon("disk", layer="layer", points=sc.geometry.circle(1))],
         ).draw(ax=ax)
         plt.close("all")
 
 
 @pytest.mark.parametrize(
-    ", ".join(["min_points", "smooth"]),
-    [(None, None), (None, 20), (1200, None), (1200, 20)],
+    ", ".join(["min_points", "max_edge_length", "smooth"]),
+    [(None, None, None), (None, 0.4, 20), (1200, 0.4, None), (1200, 0.4, 20)],
 )
 @pytest.mark.parametrize(
-    "weight_method", ["uniform", "half_cotangent", "inv_euclidean", "invalid"]
+    "buffer_factor, buffer", [(None, None), (None, 0.5), (0.05, None)]
 )
-def test_make_mesh(device, min_points, smooth, weight_method):
-    if weight_method == "invalid":
-        context = pytest.raises(ValueError)
-    else:
-        context = contextlib.nullcontext()
-
-    with context:
-        device.make_mesh(
-            min_points=min_points,
-            smooth=smooth,
-            weight_method=weight_method,
-        )
-
-    if weight_method == "invalid":
-        return
+@pytest.mark.parametrize("preserve_boundary", [False, True])
+def test_make_mesh(
+    device: sc.Device,
+    min_points: Optional[int],
+    max_edge_length: Optional[float],
+    smooth: Optional[int],
+    buffer_factor: Optional[float],
+    buffer: Optional[float],
+    preserve_boundary: bool,
+):
+    device.make_mesh(
+        min_points=min_points,
+        max_edge_length=max_edge_length,
+        smooth=smooth,
+        buffer_factor=buffer_factor,
+        buffer=buffer,
+        preserve_boundary=preserve_boundary,
+    )
 
-    assert device.points is not None
-    assert device.triangles is not None
+    assert isinstance(device.meshes, dict)
+    assert set(device.meshes) == set(device.films)
     if min_points:
-        assert device.points.shape[0] >= min_points
+        for mesh in device.meshes.values():
+            assert len(mesh.sites) >= min_points
 
-    assert isinstance(device.weights, np.ndarray)
-    assert device.weights.shape == (device.points.shape[0],)
+    mesh = device.meshes["disk"]
+    for weight_method in ("uniform", "inv_euclidean", "half_cotangent"):
+        _ = sc.fem.laplace_operator(
+            mesh.sites, mesh.elements, weight_method=weight_method
+        )
 
 
 @pytest.mark.parametrize("save_mesh", [False, True])
-@pytest.mark.parametrize("compressed", [False, True])
-def test_device_to_file(device, device_with_mesh, save_mesh, compressed):
-    with tempfile.TemporaryDirectory() as directory:
-        device.to_file(directory, save_mesh=save_mesh, compressed=compressed)
-        loaded_device = sc.Device.from_file(directory)
-    assert device == loaded_device
-
-    with tempfile.TemporaryDirectory() as directory:
-        device_with_mesh.to_file(directory, save_mesh=save_mesh, compressed=compressed)
-        loaded_device = sc.Device.from_file(directory)
-    assert device_with_mesh == loaded_device
+@pytest.mark.parametrize("compress", [False, True])
+def test_device_to_hdf5(
+    device: sc.Device,
+    device_with_mesh: sc.Device,
+    save_mesh: bool,
+    compress: bool,
+):
+    for sc_device in (device, device_with_mesh):
+        with tempfile.TemporaryDirectory() as directory:
+            fname = os.path.join(directory, "test-0.h5")
+            sc_device.to_hdf5(fname, save_mesh=save_mesh, compress=compress)
+            loaded_device = sc.Device.from_hdf5(fname)
+            assert loaded_device == sc_device
+
+            with h5py.File(os.path.join(directory, "test-1.h5"), "x") as h5file:
+                sc_device.to_hdf5(h5file, save_mesh=save_mesh, compress=compress)
+                loaded_device = sc.Device.from_hdf5(h5file)
+                assert loaded_device == sc_device
 
 
 def test_pickle_device(device, device_with_mesh):
     loaded_device = pickle.loads(pickle.dumps(device))
     loaded_device_with_mesh = pickle.loads(pickle.dumps(device_with_mesh))
 
     assert loaded_device == device
     assert loaded_device_with_mesh == device_with_mesh
 
     assert loaded_device.ureg("1 m") == loaded_device.ureg("1000 mm")
 
 
-@pytest.mark.parametrize("dense", [False, True])
-def test_copy_arrays(device_with_mesh, dense):
-    arrays = device_with_mesh.get_arrays(copy_arrays=False, dense=dense)
-    copied_arrays = device_with_mesh.get_arrays(copy_arrays=True, dense=dense)
-
-    for key, val in arrays.items():
-        assert val is not copied_arrays[key]
-        if sp.issparse(val):
-            assert not dense
-            assert np.array_equal(val.toarray(), copied_arrays[key].toarray())
-        else:
-            assert np.array_equal(val, copied_arrays[key])
-
-
 def poly_derivative(coeffs):
     """Given polynomial coefficients (c0, c1, c2, ...) specifying a polynomial
     y = c0 * x**0 + c1 * x**1 + c2 * x**2 + ..., returns the coefficients of the first
     derivative of y: (c1, 2 * c2, ...)
     """
     return tuple(c * (n + 1) for n, c in enumerate(coeffs[1:])) + (0,)
 
@@ -452,17 +338,18 @@
     deg = len(coeffs) - 1
     fit_coeffs = np.polyfit(xs, ys, deg)[::-1]
     poly_coeffs = np.array(poly_derivative(coeffs))
     assert np.allclose(fit_coeffs, poly_coeffs, rtol=rtol, atol=atol)
 
 
 @pytest.mark.parametrize("poly_degree", [0, 1, 2])
-def test_gradient_triangles(device_with_mesh, poly_degree):
-    points = device_with_mesh.points
-    triangles = device_with_mesh.triangles
+def test_gradient_triangles(device_with_mesh: sc.Device, poly_degree: int):
+    mesh = device_with_mesh.meshes["disk"]
+    points = mesh.sites
+    triangles = mesh.elements
 
     x, y = points[:, 0], points[:, 1]
     centroids = sc.fem.centroids(points, triangles)
     xt, yt = centroids[:, 0], centroids[:, 1]
 
     Gx, Gy = sc.fem.gradient_triangles(points, triangles)
 
@@ -483,17 +370,18 @@
     assert_consistent_polynomial(xt, dfx_dx, poly_coeffs)
     assert_consistent_polynomial(yt, dfx_dy, 0 * poly_coeffs)
     assert_consistent_polynomial(xt, dfy_dx, 0 * poly_coeffs)
     assert_consistent_polynomial(yt, dfy_dy, poly_coeffs)
 
 
 @pytest.mark.parametrize("poly_degree", [0, 1, 2])
-def test_gradient_vertices(device_with_mesh, poly_degree):
-    points = device_with_mesh.points
-    triangles = device_with_mesh.triangles
+def test_gradient_vertices(device_with_mesh: sc.Device, poly_degree: int):
+    mesh = device_with_mesh.meshes["disk"]
+    points = mesh.sites
+    triangles = mesh.elements
 
     x, y = points[:, 0], points[:, 1]
 
     Gx, Gy = sc.fem.gradient_vertices(points, triangles)
 
     rng = np.random.default_rng(seed=poly_degree)
     poly_coeffs = 2 * (rng.random(size=poly_degree + 1) - 0.5)
```

### Comparing `superscreen-0.8.2/superscreen/test/test_parameter.py` & `superscreen-0.9.0/superscreen/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.2/superscreen/test/test_solution.py` & `superscreen-0.9.0/superscreen/test/test_solution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,203 +1,103 @@
 import contextlib
-import os
-import shutil
-import tempfile
-from datetime import datetime
+import datetime as dt
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pint
 import pytest
 
 import superscreen as sc
 
 
-@contextlib.contextmanager
-def make_tempdir(**kwargs):
-    tmp = tempfile.mkdtemp(**kwargs)
-    try:
-        yield tmp
-    finally:
-        if os.path.isdir(tmp):
-            shutil.rmtree(tmp)
-
-
 @pytest.fixture(scope="module")
-def device():
+def device() -> sc.Device:
     layers = [
         sc.Layer("layer0", london_lambda=1, thickness=0.1, z0=0),
         sc.Layer("layer1", london_lambda=2, thickness=0.05, z0=0.5),
     ]
 
     films = [
         sc.Polygon("disk", layer="layer0", points=sc.geometry.circle(5)),
         sc.Polygon("ring", layer="layer1", points=sc.geometry.circle(4)),
     ]
 
     holes = [
         sc.Polygon("ring_hole", layer="layer1", points=sc.geometry.circle(2)),
     ]
 
-    abstract_regions = [
-        sc.Polygon("bounding_box", layer="layer0", points=sc.geometry.box(12)),
-    ]
-
     device = sc.Device(
         "device",
         layers=layers,
         films=films,
         holes=holes,
-        abstract_regions=abstract_regions,
     )
-    device.make_mesh(min_points=3000)
-
+    device.make_mesh(max_edge_length=0.4, min_points=3000)
     return device
 
 
 @pytest.fixture(scope="module")
-def solution1(device):
+def solution1(device: sc.Device) -> sc.Solution:
     applied_field = sc.sources.ConstantField(1)
 
     solutions = sc.solve(
         device=device,
         applied_field=applied_field,
-        vortices=[sc.Vortex(x=0, y=0, layer="layer0")],
+        vortices=[sc.Vortex(x=0, y=0, film="disk")],
         circulating_currents=None,
         field_units="mT",
         iterations=1,
     )
 
     return solutions[-1]
 
 
 @pytest.fixture(scope="module")
-def solution2(device):
+def solution2(device: sc.Device) -> sc.Solution:
     applied_field = sc.sources.ConstantField(0)
 
-    circulating_currents = {
-        "ring_hole": "1 mA",
-    }
+    circulating_currents = {"ring_hole": "1 mA"}
 
     solutions = sc.solve(
         device=device,
         applied_field=applied_field,
         circulating_currents=circulating_currents,
         field_units="mT",
-        iterations=2,
+        iterations=5,
     )
 
     return solutions[-1]
 
 
-def test_solution_equals(solution1, solution2):
+def test_save_and_load_solutions(solution1, tmp_path):
+    h5path = tmp_path / "solution1.h5"
+    sc.Solution.save_solutions([solution1] * 5, h5path)
+
+    solutions = sc.Solution.load_solutions(h5path)
+    assert all(solution == solution1 for solution in solutions)
+
+
+def test_solution_equals(solution1: sc.Solution, solution2: sc.Solution):
     assert solution1 == solution1
     assert solution2 == solution2
     assert solution1 != solution2
     assert solution1 != 0
 
 
-@pytest.mark.parametrize(
-    "dataset", ["streams", "fields", "screening_fields", "current_densities"]
-)
-@pytest.mark.parametrize("with_units", [False, True])
-def test_grid_data(solution1, dataset, with_units):
-    with pytest.raises(ValueError):
-        _ = solution1.grid_data("invalid_dataset")
-
-    with pytest.raises(ValueError):
-        _ = solution1.grid_data("streams", layers="invalid_layer")
-
-    with pytest.raises(TypeError):
-        _ = solution1.grid_data("streams", grid_shape=(100, 100, 2))
-
-    xgrid, ygrid, zgrids = solution1.grid_data(
-        dataset,
-        grid_shape=(20, 20),
-        with_units=with_units,
-    )
-
-    if with_units:
-        assert isinstance(xgrid.magnitude, np.ndarray)
-        assert isinstance(ygrid.magnitude, np.ndarray)
-    else:
-        assert isinstance(xgrid, np.ndarray)
-        assert isinstance(ygrid, np.ndarray)
-    assert isinstance(zgrids, dict)
-
-    for layer, array in zgrids.items():
-        assert isinstance(layer, str)
-        if with_units:
-            assert isinstance(array, pint.Quantity)
-            assert isinstance(array.magnitude, np.ndarray)
-            if dataset == "streams":
-                assert array.units == solution1.device.ureg(solution1.current_units)
-            elif dataset == "current_densities":
-                device = solution1.device
-                current_units = device.ureg(solution1.current_units)
-                length_units = device.ureg(device.length_units)
-                assert array.units == current_units / length_units
-            else:
-                assert array.units == solution1.device.ureg(solution1.field_units)
-        else:
-            assert isinstance(array, np.ndarray)
-        if dataset == "current_densities":
-            assert xgrid.shape == ygrid.shape
-            assert array.shape == (2,) + xgrid.shape
-        else:
-            assert xgrid.shape == ygrid.shape == array.shape
-
-
-@pytest.mark.parametrize("units", [None, "mA / um"])
-@pytest.mark.parametrize("with_units", [False, True])
-def test_current_density(solution1, units, with_units):
-    xgrid, ygrid, current_density = solution1.grid_current_density(
-        grid_shape=(20, 20),
-        units=units,
-        with_units=with_units,
-    )
-
-    if with_units:
-        assert isinstance(xgrid.magnitude, np.ndarray)
-        assert isinstance(ygrid.magnitude, np.ndarray)
-    else:
-        assert isinstance(xgrid, np.ndarray)
-        assert isinstance(ygrid, np.ndarray)
-    assert isinstance(current_density, dict)
-
-    for layer, array in current_density.items():
-        assert isinstance(layer, str)
-        if with_units:
-            assert isinstance(array, pint.Quantity)
-            assert isinstance(array.magnitude, np.ndarray)
-            if units is None:
-                units = f"{solution1.current_units} / {solution1.device.length_units}"
-                assert array.units == solution1.device.ureg(units)
-            else:
-                assert array.units == solution1.device.ureg(units)
-        else:
-            assert isinstance(array, np.ndarray)
-        assert array.shape[0] == 2
-        assert xgrid.shape == ygrid.shape == array.shape[1:]
-
-
 @pytest.mark.parametrize("units", [None, "Phi_0", "mT * um**2"])
 @pytest.mark.parametrize("with_units", [False, True])
-def test_polygon_flux(solution2, units, with_units):
+def test_polygon_flux(solution2: sc.Solution, units, with_units):
     with pytest.raises(ValueError):
-        _ = solution2.polygon_flux(polygons="invalid_polygon")
-
-    flux_dict = solution2.polygon_flux(units=units, with_units=with_units)
+        _ = solution2.polygon_flux(name="invalid_polygon")
 
-    assert isinstance(flux_dict, dict)
-    assert len(flux_dict) == (
-        len(solution2.device.films)
-        + len(solution2.device.holes)
-        + len(solution2.device.abstract_regions)
-    )
+    flux_dict = {}
+    for polygon in solution2.device.get_polygons(include_terminals=False):
+        flux_dict[polygon.name] = solution2.polygon_flux(
+            polygon.name, units=units, with_units=with_units
+        )
 
     units = units or f"{solution2.field_units} * {solution2.device.length_units}**2"
     ureg = solution2.device.ureg
 
     for name, flux in flux_dict.items():
         assert isinstance(name, str)
         if with_units:
@@ -207,285 +107,251 @@
             assert isinstance(flux, float)
 
 
 @pytest.mark.parametrize(
     "positions, zs",
     [
         (np.array([[-1, 1, -2], [1, -1, 2]]), None),
+        (np.array([[-1, 1], [1, -1]]), 0.0),
+        (np.array([[-1, 1], [1, -1]]), 0.5),
         (np.array([[-1, 1], [1, -1]]), 2),
         (np.array([[-1, 1], [1, -1]]), np.array([2, 2])),
         (np.array([[-1, 1], [1, -1]]), np.array([[2], [2]])),
     ],
 )
 @pytest.mark.parametrize("units", [None, "mT", "mA/um"])
 @pytest.mark.parametrize("with_units", [False, True])
-@pytest.mark.parametrize("vector", [False, True])
 @pytest.mark.parametrize("return_sum", [False, True])
 def test_field_at_positions(
-    solution2, positions, zs, vector, units, with_units, return_sum
+    solution2: sc.Solution, positions, zs, units, with_units, return_sum
 ):
     H = solution2.field_at_position(
         positions,
         zs=zs,
-        vector=vector,
         units=units,
         with_units=with_units,
         return_sum=return_sum,
     )
 
     units = units or solution2.field_units
     units = solution2.device.ureg(units)
 
     if return_sum:
         if with_units:
             assert isinstance(H, pint.Quantity)
             assert isinstance(H.magnitude, np.ndarray)
             assert H.units == units
-        if vector:
-            assert H.shape == positions.shape[:1] + (3,)
-        else:
-            assert H.shape == positions.shape[:1]
+        assert H.shape == positions.shape[:1]
 
     else:
         assert isinstance(H, dict)
         assert "applied_field" in H
         for item in H.values():
             if with_units:
                 assert isinstance(item, pint.Quantity)
                 assert isinstance(item.magnitude, np.ndarray)
                 assert item.units == units
             else:
                 assert isinstance(item, np.ndarray)
-            if vector:
-                assert item.shape == positions.shape[:1] + (3,)
-            else:
-                assert item.shape == positions.shape[:1]
+            assert item.shape == positions.shape[:1]
 
 
-@pytest.mark.parametrize("to_zip", [False, True])
-@pytest.mark.parametrize("save_mesh", [False, True])
-@pytest.mark.parametrize("compressed", [False, True])
-def test_save_solution(solution1, solution2, save_mesh, compressed, to_zip):
-    with make_tempdir() as directory:
-        solution1.to_file(
-            directory, save_mesh=save_mesh, compressed=compressed, to_zip=to_zip
-        )
-        loaded_solution1 = sc.Solution.from_file(directory + (".zip" if to_zip else ""))
+@pytest.mark.parametrize("compress", [False, True])
+def test_save_solution(
+    solution1: sc.Solution,
+    solution2: sc.Solution,
+    compress,
+    tmp_path,
+):
+    solution1.to_hdf5(tmp_path / "solution1.h5", compress=compress)
+    loaded_solution1 = sc.Solution.from_hdf5(tmp_path / "solution1.h5")
     assert solution1 == loaded_solution1
 
-    with make_tempdir() as other_directory:
-        solution2.to_file(
-            other_directory, save_mesh=save_mesh, compressed=compressed, to_zip=to_zip
-        )
-        loaded_solution2 = sc.Solution.from_file(
-            other_directory + (".zip" if to_zip else "")
-        )
+    solution2.to_hdf5(tmp_path / "solution2.h5", compress=compress)
+    loaded_solution2 = sc.Solution.from_hdf5(tmp_path / "solution2.h5")
     assert solution2 == loaded_solution2
 
-    loaded_solution2._time_created = datetime.now()
+    loaded_solution2._time_created = dt.datetime.now()
     assert solution2 != loaded_solution2
 
-    with make_tempdir() as directory:
-        solution1.to_file(
-            directory, save_mesh=save_mesh, compressed=compressed, to_zip=to_zip
-        )
-        if not to_zip:
-            with pytest.raises(IOError):
-                solution1.to_file(
-                    directory, save_mesh=save_mesh, compressed=compressed, to_zip=to_zip
-                )
-
 
 @pytest.mark.parametrize("polygon_shape", ["circle", "rectangle"])
 @pytest.mark.parametrize("center", [(-4, 0), (-2, 2), (0, 0), (1, -2)])
-@pytest.mark.parametrize("layers", ["layer0", ["layer0"]])
 @pytest.mark.parametrize("with_units", [False, True])
 @pytest.mark.parametrize("units", ["Phi_0", None])
 def test_fluxoid_simply_connected(
-    solution1,
+    solution1: sc.Solution,
     units,
     with_units,
-    layers,
     center,
     polygon_shape,
 ):
     ureg = solution1.device.ureg
     if polygon_shape == "circle":
-        coords = sc.geometry.circle(1.5, points=501, center=center)
+        coords = sc.geometry.circle(1.5, points=201, center=center)
     else:
-        coords = sc.geometry.box(3, 2, points_per_side=100, center=center)[::-1]
+        coords = sc.geometry.box(3, 2, points=401, center=center)[::-1]
 
     if center == (-4, 0):
         # The polygon goes outside of the film -> raise ValueError
         context = pytest.raises(ValueError)
     else:
         context = contextlib.nullcontext()
 
     with context:
-        fluxoid_dict = solution1.polygon_fluxoid(
-            polygon_points=coords,
-            layers=layers,
+        fluxoid = solution1.polygon_fluxoid(
+            polygon_coords=coords,
+            film="disk",
             units=units,
             with_units=with_units,
         )
     if units is None:
         units = f"{solution1.field_units} * {solution1.device.length_units} ** 2"
 
     if center == (-4, 0):
         return
 
-    for name, fluxoid in fluxoid_dict.items():
-        assert name in solution1.device.layers
-        flux_part, supercurrent_part = fluxoid
-        desired_type = pint.Quantity if with_units else float
-        assert isinstance(flux_part, desired_type)
-        assert isinstance(supercurrent_part, desired_type)
-        total_fluxoid = sum(fluxoid)
-        if with_units:
-            flux_part = flux_part.m
-            total_fluxoid = total_fluxoid.m
-        # For a simply connected region, the total fluxoid should be equal to
-        # Phi0 times the number of vortices in the region.
-        total_vortex_flux = 0
-        for vortex in solution1.vortices:
-            if vortex.layer == name:
-                if sc.fem.in_polygon(coords, [vortex.x, vortex.y]):
-                    total_vortex_flux += (
-                        (vortex.nPhi0 * ureg("Phi_0")).to(units).magnitude
-                    )
-        if total_vortex_flux:
-            # There are vortices in the region.
-            assert (
-                abs(total_fluxoid - total_vortex_flux) / abs(total_vortex_flux)
-            ) < 5e-2
-        else:
-            # No vortices - fluxoid should be zero.
-            assert abs(total_fluxoid) / abs(flux_part) < 5e-2
+    flux_part, supercurrent_part = fluxoid
+    desired_type = pint.Quantity if with_units else float
+    assert isinstance(flux_part, desired_type)
+    assert isinstance(supercurrent_part, desired_type)
+    total_fluxoid = sum(fluxoid)
+    if with_units:
+        flux_part = flux_part.m
+        total_fluxoid = total_fluxoid.m
+    # For a simply connected region, the total fluxoid should be equal to
+    # Phi0 times the number of vortices in the region.
+    total_vortex_flux = 0
+    for vortex in solution1.vortices:
+        if sc.fem.in_polygon(coords, (vortex.x, vortex.y)):
+            total_vortex_flux += (vortex.nPhi0 * ureg("Phi_0")).to(units).magnitude
+    if total_vortex_flux:
+        # There are vortices in the region.
+        assert (abs(total_fluxoid - total_vortex_flux) / abs(total_vortex_flux)) < 5e-2
+    else:
+        # No vortices - fluxoid should be zero.
+        assert abs(total_fluxoid) / abs(flux_part) < 5e-2
 
 
 @pytest.mark.parametrize("units, with_units", [("uA / um", False), (None, True)])
 @pytest.mark.parametrize(
-    "layers, method, positions",
+    "film, method, positions",
     [
-        ("layer0", "nearest", [0, 0]),
-        (None, "linear", np.array([[1, 0], [0, 1]])),
-        (["layer0"], "cubic", None),
+        ("disk", "nearest", [0, 0]),
+        ("ring", "linear", np.array([[1, 0], [0, 1]])),
+        ("disk", "cubic", None),
     ],
 )
 def test_interp_current_density(
-    solution1, positions, method, layers, units, with_units
+    solution1: sc.Solution, positions, method, film, units, with_units
 ):
     if positions is None:
-        positions = solution1.device.points
+        positions = solution1.device.meshes["disk"].sites
 
-    with pytest.raises(ValueError):
+    with pytest.raises(KeyError):
         _ = solution1.interp_current_density(
             positions,
-            layers=layers,
+            film=film,
             method="invalid_method",
             units=units,
             with_units=with_units,
         )
 
     current_densities = solution1.interp_current_density(
         positions,
-        layers=layers,
+        film=film,
         method=method,
         units=units,
         with_units=with_units,
     )
-    if layers is None:
-        assert set(current_densities) == set(solution1.device.layers)
-    else:
-        assert set(current_densities) == set(["layer0"])
-    for array in current_densities.values():
-        assert array.shape == np.atleast_2d(positions).shape
-        if with_units:
-            assert isinstance(array, pint.Quantity)
+    assert current_densities.shape == np.atleast_2d(positions).shape
+    if with_units:
+        assert isinstance(current_densities, pint.Quantity)
 
 
-def test_visualization(solution1):
+def test_visualization(solution1: sc.Solution):
     with sc.visualization.non_gui_backend():
         fig, _ = solution1.plot_streams()
         plt.close(fig)
 
         fig, _ = solution1.plot_fields()
         plt.close(fig)
 
         fig, _ = solution1.plot_currents()
         plt.close(fig)
 
-        fig, _ = solution1.plot_field_at_positions(solution1.device.points, zs=0.3333)
+        fig, _ = solution1.plot_field_at_positions(
+            solution1.device.meshes["disk"].sites, zs=0.3333
+        )
         plt.close(fig)
 
 
 @pytest.mark.parametrize("use_zs", [False, True, "z0"])
 @pytest.mark.parametrize("units", [None, "uT * um"])
 @pytest.mark.parametrize("with_units", [False, True])
 @pytest.mark.parametrize("return_sum", [False, True])
-def test_bz_from_vector_potential(solution2, use_zs, units, with_units, return_sum):
+def test_bz_from_vector_potential(
+    solution2: sc.Solution, use_zs, units, with_units, return_sum
+):
     solution = solution2
-    applied_field = solution.applied_field
+    applied_field = solution.applied_field_func
     device = solution.device
     ureg = device.ureg
-    gradx = device.gradx
-    grady = device.grady
+    bz_units = None if units is None else "uT"
+    gradx = device.meshes["disk"].operators.gradient_x.toarray()
+    grady = device.meshes["disk"].operators.gradient_y.toarray()
     if with_units:
         gradx = gradx / ureg(device.length_units)
         grady = grady / ureg(device.length_units)
-    positions = device.points.copy()
+    positions = device.meshes["disk"].sites
     z0 = 1.5
     zs = z0 * np.ones_like(positions[:, :1])
     applied_field = applied_field(positions[:, 0], positions[:, 1], zs[0])
+    applied_field = applied_field * ureg(solution.field_units)
+    if bz_units:
+        applied_field.ito(bz_units)
     if not use_zs:
         positions = np.concatenate([positions, zs], axis=1)
         zs = None
     elif use_zs == "z0":
         zs = z0
-    bz_units = None if units is None else "uT"
     Bz = solution.field_at_position(
         positions, zs=zs, units=bz_units, with_units=with_units
     )
     A = solution.vector_potential_at_position(
         positions,
         zs=zs,
         units=units,
         with_units=with_units,
         return_sum=return_sum,
     )
     if not return_sum:
         assert isinstance(A, dict)
-        assert len(A) == len(device.layers)
+        assert len(A) == len(device.films)
         A = sum(A.values())
     Ax = A[:, 0]
     Ay = A[:, 1]
-    if with_units:
-        applied_field = applied_field * ureg(solution.field_units)
+    if not with_units:
+        applied_field = applied_field.magnitude
     Bz_from_A = applied_field + (gradx @ Ay - grady @ Ax)
     if with_units:
         Bz_from_A.ito(Bz.units)
-    assert np.all(np.abs(Bz_from_A - Bz) < 0.1 * np.max(np.abs(Bz)))
+    assert np.all(np.abs(Bz_from_A - Bz) < 5e-2 * np.max(np.abs(Bz)))
 
 
-@pytest.mark.parametrize("layers", [["layer1"], None])
 @pytest.mark.parametrize("units", [None, "mT", "mA/um"])
 @pytest.mark.parametrize("with_units", [False, True])
 @pytest.mark.parametrize("method", ["nearest", "linear", "cubic"])
-def test_interp_fields(solution2, layers, units, with_units, method):
+def test_interp_field(solution2: sc.Solution, units, with_units, method):
     solution = solution2
-    positions = np.random.random(size=200).reshape((100, 2))
-    fields = solution.interp_fields(
+    positions = np.random.random(size=(100, 2))
+    field = solution.interp_field(
         positions,
-        layers=layers,
+        film="disk",
         units=units,
         with_units=with_units,
         method=method,
     )
-    if layers is None:
-        assert set(fields) == set(solution.device.layers)
-    else:
-        assert set(fields) == set(layers)
-    for value in fields.values():
-        if with_units:
-            assert isinstance(value, pint.Quantity)
-            assert isinstance(value.magnitude, np.ndarray)
-        assert value.shape == positions.shape[:1]
+    if with_units:
+        assert isinstance(field, pint.Quantity)
+        assert isinstance(field.magnitude, np.ndarray)
+    assert field.shape == positions.shape[:1]
```

### Comparing `superscreen-0.8.2/superscreen/test/test_solve.py` & `superscreen-0.9.0/superscreen/test/test_solve.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-import os
-
+import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 import pint
 import pytest
 
-try:
-    import jax  # noqa: F401
-
-    HAS_JAX = True
-    os.environ["JAX_PLATFORMS"] = "cpu"
-except (ModuleNotFoundError, ImportError, RuntimeError):
-    HAS_JAX = False
-
-
 import superscreen as sc
 import superscreen.geometry as geo
 
 
 @pytest.fixture(scope="module")
 def device():
     layers = [
@@ -28,28 +18,24 @@
         sc.Polygon("ring", layer="layer1", points=geo.circle(4)),
     ]
 
     holes = [
         sc.Polygon(
             "ring_hole",
             layer="layer1",
-            points=geo.circle(3, center=(0.5, 0.5)),
+            points=geo.circle(2),
         ),
     ]
-
-    abstract_regions = [sc.Polygon("bounding_box", layer="layer1", points=geo.box(10))]
-
     device = sc.Device(
         "device",
         layers=layers,
         films=films,
         holes=holes,
-        abstract_regions=abstract_regions,
     )
-    device.make_mesh(min_points=5000, smooth=200)
+    device.make_mesh(max_edge_length=0.15)
 
     return device
 
 
 @pytest.fixture(scope="module")
 def two_rings():
     length_units = "um"
@@ -103,102 +89,127 @@
         abstract_regions=abstract_regions,
         length_units=length_units,
     )
     device.make_mesh(min_points=4000)
     return device
 
 
+@pytest.mark.parametrize("pre_factorize", [False, True])
 @pytest.mark.parametrize("return_solutions", [False, True])
 @pytest.mark.parametrize("save", [False, True])
 @pytest.mark.parametrize("inhomogeneous", [False, True])
-@pytest.mark.parametrize("gpu", [False, True])
-def test_current_value(device, return_solutions, save, tmp_path, inhomogeneous, gpu):
+def test_current_value(
+    device, pre_factorize, return_solutions, save, tmp_path, inhomogeneous
+):
     applied_field = sc.sources.ConstantField(0)
 
     circulating_currents = {
         "ring_hole": "1 mA",
     }
 
     # https://docs.pytest.org/en/stable/tmpdir.html
-    directory = str(tmp_path) if save else None
+    save_path = tmp_path / "solution.h5" if save else None
 
     old_lambda = device.layers["layer1"].london_lambda
     try:
         if inhomogeneous:
 
             def linear(x, y, offset=0):
-                return offset + (y - y.min()) + (x - x.min())
+                return offset + 0.1 * ((y - y.min()) + (x - x.min()))
 
             device.layers["layer1"].london_lambda = sc.Parameter(
                 linear, offset=old_lambda
             )
-        solutions = sc.solve(
-            device=device,
-            applied_field=applied_field,
-            circulating_currents=circulating_currents,
-            field_units="mT",
-            iterations=1,
-            return_solutions=return_solutions,
-            directory=directory,
-            gpu=(HAS_JAX and gpu),
-        )
+        if pre_factorize:
+            model = sc.factorize_model(
+                device=device,
+                circulating_currents=circulating_currents,
+                current_units="uA",
+            )
+            model_save_path = tmp_path / "model.h5"
+            with h5py.File(model_save_path, "x") as h5file:
+                model.to_hdf5(h5file)
+
+            with h5py.File(model_save_path, "r") as h5file:
+                model = sc.FactorizedModel.from_hdf5(h5file)
+
+            solutions = sc.solve(
+                model=model,
+                applied_field=applied_field,
+                field_units="mT",
+                iterations=1,
+                return_solutions=return_solutions,
+                save_path=save_path,
+            )
+        else:
+            solutions = sc.solve(
+                device=device,
+                applied_field=applied_field,
+                circulating_currents=circulating_currents,
+                field_units="mT",
+                current_units="uA",
+                iterations=1,
+                return_solutions=return_solutions,
+                save_path=save_path,
+            )
     finally:
         device.layers["layer1"].london_lambda = old_lambda
-    if directory is not None:
-        assert os.path.isdir(directory)
-        assert len(os.listdir(directory)) == 1
 
     if return_solutions:
         assert isinstance(solutions, list)
         assert len(solutions) == 1
         solution = solutions[0]
-        grid_shape = 500
-
-        xgrid, ygrid, J = solution.grid_current_density(
-            grid_shape=grid_shape, units="uA / um", with_units=False
-        )
-        jx, jy = J["layer1"]
-        x, y = sc.grids_to_vecs(xgrid, ygrid)
-
-        dx = x[1] - x[0]
-        dy = y[1] - y[0]
-
-        N = grid_shape // 2
+        xs = np.linspace(1.9, 4.1, 1001)
+        ys = np.zeros_like(xs)
+        positions = np.array([xs, ys]).T
+        rtol = 5e-2
+        for angle, axis in [(0, 1), (90, 0), (180, 1), (270, 0)]:
+            coords = sc.geometry.rotate(positions, angle)
+            current = solution.current_through_path(
+                coords,
+                film="ring",
+                units="uA",
+                with_units=False,
+            )
+            assert np.isclose(abs(current), 1000, rtol=rtol)
 
-        assert np.isclose(np.sum(-jy[N, :N]) * dx, 1000)
-        assert np.isclose(np.sum(+jy[N, N:]) * dx, 1000)
-        assert np.isclose(np.sum(-jx[N:, N]) * dy, 1000)
-        assert np.isclose(np.sum(+jx[:N, N]) * dy, 1000)
-    else:
-        assert solutions is None
+            j = solution.interp_current_density(
+                coords,
+                film="ring",
+                units="uA / um",
+                with_units=False,
+            )
+            dr = np.linalg.norm(np.diff(coords, axis=0), axis=1)
+            current = np.sum(j[1:, axis] * dr)
+            assert np.isclose(abs(current), 1000, rtol=rtol)
 
 
 def test_invalid_vortex_args(device):
     with pytest.raises(TypeError):
         _ = sc.solve(device=device, vortices=[0, 1, 2])
 
-    # Vortex in unknown layer
-    with pytest.raises(ValueError):
+    # Vortex in unknown film
+    with pytest.raises(KeyError):
         _ = sc.solve(
             device=device,
-            vortices=[sc.Vortex(x=3.5, y=0, layer="invalid")],
+            vortices=[sc.Vortex(x=3.5, y=0, film="invalid")],
         )
 
     # Vortex in hole
     with pytest.raises(ValueError):
         _ = sc.solve(
             device=device,
-            vortices=[sc.Vortex(x=0, y=0, layer="layer1")],
+            vortices=[sc.Vortex(x=0, y=0, film="ring")],
         )
 
     # Vortex outside film
     with pytest.raises(ValueError):
         _ = sc.solve(
             device=device,
-            vortices=[sc.Vortex(x=4.5, y=0, layer="layer1")],
+            vortices=[sc.Vortex(x=4.5, y=0, film="ring")],
         )
 
 
 def test_mutual_inductance_errors(two_rings):
     with pytest.raises(ValueError):
         _ = two_rings.mutual_inductance_matrix(
             hole_polygon_mapping={"invalid": None},
@@ -217,31 +228,28 @@
         all_iterations=True,
     )
     # Check that M is symmetric
     assert np.isclose(M[-1][0, 1], M[-1][1, 0], rtol=5e-2)
     return M
 
 
-@pytest.mark.parametrize("gpu", [False, True])
 def test_mutual_inductance_matrix(
     two_rings,
     mutual_inductance_matrix,
-    gpu,
     iterations=3,
 ):
     hole_polygon_mapping = {
         "big_hole": geo.circle(6),
         "little_hole": geo.circle(4),
     }
 
     M = two_rings.mutual_inductance_matrix(
         hole_polygon_mapping=hole_polygon_mapping,
         iterations=iterations,
         all_iterations=True,
-        gpu=(HAS_JAX and gpu),
     )
     assert isinstance(M, list)
     assert len(M) == iterations + 1
     assert all(isinstance(m, pint.Quantity) for m in M)
     assert all(isinstance(m.magnitude, np.ndarray) for m in M)
     M = M[-1]
     assert isinstance(M, pint.Quantity)
@@ -285,23 +293,20 @@
     with pytest.raises(ValueError):
         _ = sc.plot_mutual_inductance(M[0])
 
     with pytest.raises(ValueError):
         _ = sc.plot_mutual_inductance([M[0], 0])
 
 
-@pytest.mark.parametrize("gpu", [False, True])
-def test_fluxoid_single(device, gpu):
+def test_fluxoid_single(device):
     _ = sc.make_fluxoid_polygons(device, interp_points=None)
     _ = sc.make_fluxoid_polygons(device, interp_points=101)
 
     fluxoids = {hole: 0 for hole in device.holes}
-    solution = sc.find_fluxoid_solution(
-        device, fluxoids=fluxoids, gpu=(HAS_JAX and gpu)
-    )
+    solution = sc.find_fluxoid_solution(device, fluxoids=fluxoids)
     assert isinstance(solution, sc.Solution)
     fluxoid = solution.hole_fluxoid(list(device.holes)[0])
     assert np.isclose(sum(fluxoid).to("Phi_0").m, 0)
 
 
 def test_fluxoid_multi(two_rings):
     fluxoids = {hole: 0 for hole in two_rings.holes}
@@ -314,9 +319,9 @@
     )
     assert isinstance(solution, sc.Solution)
     for hole_name in two_rings.holes:
         fluxoid = solution.hole_fluxoid(hole_name)
         assert np.isclose(
             sum(fluxoid).to("Phi_0").m,
             fluxoids[hole_name],
-            atol=1e-6,
+            atol=3e-6,
         )
```

### Comparing `superscreen-0.8.2/superscreen/test/test_sources.py` & `superscreen-0.9.0/superscreen/test/test_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,16 @@
     else:
         assert field.shape == shape
     assert np.all(field >= 0)
 
 
 def test_sheet_current():
     wire = sc.Polygon(points=sc.geometry.box(12, 1))
-    points, _ = wire.make_mesh(min_points=2000)
+    mesh = wire.make_mesh(min_points=2000)
+    points = mesh.sites
 
     current_densities = np.array([1, 0]) * np.ones((points.shape[0], 1))
 
     field = sc.sources.SheetCurrentField(
         sheet_positions=points,
         current_densities=current_densities,
         z0=0,
```

### Comparing `superscreen-0.8.2/superscreen/test/test_transport.py` & `superscreen-0.9.0/superscreen/test/test_transport.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,60 @@
+import h5py
 import numpy as np
 import pytest
 
 import superscreen as sc
 
 
 @pytest.fixture()
 def plus_device():
     layer = sc.Layer("base", Lambda=1)
     width, height = 10, 2
     points = sc.geometry.box(width, height)
     bar = sc.Polygon("plus", points=points)
-    plus = bar.union(bar.rotate(90))
+    plus = bar.union(bar.rotate(90)).resample(501)
     plus.name = "plus"
     plus.layer = layer.name
     terminal = sc.Polygon(
         points=sc.geometry.box(height, width / 100, center=(0, -width / 2))
     )
     terminals = []
     for i, name in enumerate(["drain", "source1", "source2", "source3"]):
         term = terminal.rotate(i * 90)
         term.name = name
         terminals.append(term)
-    drain, *sources = terminals
 
-    with pytest.raises(ValueError):
-        device = sc.TransportDevice(
-            "plus",
-            film=plus,
-            layer=layer,
-            source_terminals=None,
-            drain_terminal=drain,
-            length_units="um",
-        )
-
-    with pytest.raises(ValueError):
-        device = sc.TransportDevice(
-            "plus",
-            film=plus,
-            layer=layer,
-            source_terminals=sources,
-            drain_terminal=None,
-            length_units="um",
-        )
-
-    device = sc.TransportDevice(
+    device = sc.Device(
         "plus",
-        film=plus,
-        layer=layer,
-        source_terminals=sources,
-        drain_terminal=drain,
+        films=[plus],
+        layers=[layer],
+        terminals={"plus": terminals},
         length_units="um",
     )
-    device.make_mesh(min_points=2000, smooth=20)
+    device.make_mesh(max_edge_length=0.2)
     return device
 
 
 @pytest.fixture()
 def plus_device_no_terminals():
     layer = sc.Layer("base", Lambda=1)
     width, height = 10, 2
     points = sc.geometry.box(width, height)
     bar = sc.Polygon("plus", points=points)
-    plus = bar.union(bar.rotate(90))
+    plus = bar.union(bar.rotate(90)).resample(501)
     plus.name = "plus"
     plus.layer = layer.name
-    device = sc.TransportDevice(
+    device = sc.Device(
         "plus",
-        film=plus,
-        layer=layer,
-        source_terminals=None,
-        drain_terminal=None,
+        films=[plus],
+        layers=[layer],
+        terminals=None,
         length_units="um",
     )
-    device.make_mesh(min_points=2000, smooth=20)
+    device.make_mesh(max_edge_length=0.2)
     return device
 
 
 @pytest.fixture()
 def holey_device():
     width = 1
     height = width * 2
@@ -103,95 +81,138 @@
     source_terminal = sc.Polygon(
         "source", points=sc.geometry.box(width, height / 100, center=(0, height / 2))
     )
     drain_terminal = sc.Polygon(
         "drain", points=sc.geometry.box(width, height / 100, center=(0, -height / 2))
     )
 
-    device = sc.TransportDevice(
+    device = sc.Device(
         "constriction",
-        layer=sc.Layer("base", Lambda=2),
-        film=film,
+        layers=[sc.Layer("base", Lambda=2)],
+        films=[film],
         holes=[
             sc.Polygon(
                 "hole1",
                 layer="base",
                 points=sc.geometry.circle(width / 4, center=(0, +height / 4)),
             ),
             sc.Polygon(
                 "hole2",
                 layer="base",
                 points=sc.geometry.circle(width / 4, center=(0, -height / 4)),
             ),
         ],
-        source_terminals=[source_terminal],
-        drain_terminal=drain_terminal,
+        terminals={"film": [source_terminal, drain_terminal]},
         length_units=length_units,
     ).translate(dx=dx, dy=dy)
-    device.make_mesh(min_points=2000, smooth=20)
+    device.make_mesh(max_edge_length=0.2)
+    print(device)
     return device
 
 
-@pytest.mark.parametrize("gpu", [False, True])
+def test_save_and_load_device_with_terminals(holey_device: sc.Device, tmp_path):
+    h5path = tmp_path / "holey_device.h5"
+    holey_device.to_hdf5(h5path)
+    loaded_device = sc.Device.from_hdf5(h5path)
+    assert loaded_device == holey_device
+
+
+@pytest.fixture()
+def factorized_model(holey_device) -> sc.FactorizedModel:
+    model = sc.factorize_model(
+        device=holey_device,
+        current_units="uA",
+        terminal_currents={"film": {"source": "10 uA", "drain": "-10 uA"}},
+        circulating_currents={"hole1": "5 uA"},
+        vortices=[sc.Vortex(x=0, y=0, film="film")],
+    )
+    return model
+
+
+def test_save_and_load_factorized_model(factorized_model: sc.FactorizedModel, tmp_path):
+    h5path = tmp_path / "factorized-model.h5"
+    with h5py.File(h5path, "x") as f:
+        factorized_model.to_hdf5(f)
+
+    with h5py.File(h5path, "r") as f:
+        loaded_model = sc.FactorizedModel.from_hdf5(f)
+
+    assert isinstance(loaded_model, sc.FactorizedModel)
+
+
 @pytest.mark.parametrize("applied_field", [0, -1, 2])
-def test_multi_terminal_currents(plus_device, gpu, applied_field):
+def test_multi_terminal_currents(plus_device, applied_field):
     xs = np.linspace(-2, 2, 201)
     ys = -3 * np.ones_like(xs)
     rs = np.stack([xs, ys], axis=1)
     sections = [sc.geometry.rotate(rs, i * 90) for i in range(4)]
 
+    with pytest.raises(ValueError):
+        # Current not conserved
+        terminal_currents = {
+            "plus": {
+                "drain": -5,
+                "source1": "1 uA",
+                "source2": sc.ureg("2 uA"),
+                "source3": 3,
+            }
+        }
+        solution = sc.solve(
+            plus_device,
+            terminal_currents=terminal_currents,
+            applied_field=sc.sources.ConstantField(applied_field),
+            current_units="uA",
+            field_units="uT",
+        )[-1]
+
     terminal_currents = {
-        "source1": "1 uA",
-        "source2": sc.ureg("2 uA"),
-        "source3": 3,
+        "plus": {
+            "drain": -6,
+            "source1": "1 uA",
+            "source2": sc.ureg("2 uA"),
+            "source3": 3,
+        }
     }
     solution = sc.solve(
         plus_device,
         terminal_currents=terminal_currents,
         applied_field=sc.sources.ConstantField(applied_field),
         current_units="uA",
         field_units="uT",
-        gpu=gpu,
     )[-1]
 
     currents = []
     for coords in sections:
-        J = solution.interp_current_density(coords, units="uA/um", with_units=False)[
-            "base"
-        ]
+        J = solution.interp_current_density(
+            coords, film="plus", units="uA/um", with_units=False
+        )
         _, unit_normals = sc.geometry.path_vectors(coords)
         dr = np.linalg.norm(np.diff(coords, axis=0), axis=1)[0]
         currents.append(np.sum(J * dr * unit_normals))
-    drain_current, *source_currents = currents
-    target_currents = solution.terminal_currents.values()
-    total_current = sum(target_currents)
-    assert np.isclose(drain_current, total_current, rtol=1e-3)
-    for actual, target in zip(source_currents, target_currents):
-        assert np.isclose(-actual, target, rtol=1e-3)
+    target_currents = solution.terminal_currents["plus"].values()
+    assert np.abs(np.sum(currents) / terminal_currents["plus"]["drain"]) < 5e-2
+    for actual, target in zip(currents, target_currents):
+        assert np.isclose(-actual, target, rtol=5e-2)
 
 
-@pytest.mark.parametrize("gpu", [False, True])
-def test_holey_device(holey_device, gpu):
+def test_holey_device(holey_device):
     device = holey_device
-    terminal_currents = {
-        "source": "2 uA",
-    }
+    terminal_currents = {"film": {"source": "2 uA", "drain": "-2 uA"}}
     circulating_currents = {
         "hole1": "1 uA",
         "hole2": "-1 uA",
     }
 
     solution = sc.solve(
         device,
         terminal_currents=terminal_currents,
         circulating_currents=circulating_currents,
         applied_field=sc.sources.ConstantField(0),
         field_units="uT",
         current_units="uA",
-        gpu=gpu,
     )[-1]
 
     xs_left = np.linspace(-0.5, 0, 201)
     ys_left = np.ones_like(xs_left)
     xs_right = -xs_left[::-1]
     ys_right = ys_left
     xs = np.linspace(-0.5, 0.5, 401)
@@ -204,22 +225,23 @@
         np.stack([xs_left, -0.5 * ys_left], axis=1),
     ]
     target_currents = [2, 2, 2, 0, 0]
     currents = []
     for coords in sections:
         J = solution.interp_current_density(
             coords,
+            film="film",
             units="uA/um",
             with_units=False,
-        )["base"]
+        )
         _, unit_normals = sc.geometry.path_vectors(coords)
         dr = np.linalg.norm(np.diff(coords, axis=0), axis=1)[0]
         currents.append(np.sum(J * dr * unit_normals))
     for actual, target in zip(currents, target_currents):
-        assert np.isclose(actual, target, rtol=1e-2, atol=1e-2)
+        assert np.isclose(actual, target, rtol=5e-2, atol=1e-2)
 
 
 def test_no_terminals(plus_device_no_terminals):
     device = plus_device_no_terminals
     solutions = sc.solve(
         device=device,
         applied_field=sc.sources.ConstantField(1),
```

### Comparing `superscreen-0.8.2/superscreen/test/test_visualization.py` & `superscreen-0.9.0/superscreen/test/test_visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,50 +66,48 @@
             units=units,
             logy=logy,
             grid=True,
         )
     plt.close(fig)
 
 
-@pytest.mark.parametrize("layers", [None, "layer0"])
+@pytest.mark.parametrize("films", [None, "disk", ["disk", "ring"]])
 @pytest.mark.parametrize("units", [None, "mA"])
-@pytest.mark.parametrize("filled", [False, True])
-def test_plot_streams(solution, layers, units, filled):
+def test_plot_streams(solution, films, units):
     with non_gui_backend():
         fig, ax = sc.plot_streams(
             solution,
-            layers=layers,
+            films=films,
             units=units,
-            filled=filled,
         )
         plt.close(fig)
 
 
 cross_section_coord_params = [
     None,
-    np.stack([np.linspace(-1, 1, 101), 1 * np.ones(101)], axis=1),
+    np.array([np.linspace(-1, 1, 101), 1 * np.ones(101)]).T,
     [
-        np.stack([np.linspace(-1, 1, 101), 1 * np.ones(101)], axis=1),
-        np.stack([1 * np.ones(101), np.linspace(-1, 1, 101)], axis=1),
+        np.array([np.linspace(-1, 1, 101), 1 * np.ones(101)]).T,
+        np.array([1 * np.ones(101), np.linspace(-1, 1, 101)]).T,
     ],
 ]
 thetas = np.linspace(0, 2 * np.pi, endpoint=False)
 cross_section_coord_params.append(
     [r * np.stack([np.cos(thetas), np.sin(thetas)], axis=1) for r in (0.5, 1.0, 1.5)]
 )
 
 
 @pytest.mark.parametrize("interp_method", ["nearest", "linear", "cubic"])
 @pytest.mark.parametrize("cross_section_coords", cross_section_coord_params)
 def test_cross_section(solution, cross_section_coords, interp_method):
     if cross_section_coords is None:
         return
 
-    dataset_coords = solution.device.points
-    dataset_values = solution.fields[list(solution.device.layers)[0]]
+    dataset_coords = solution.device.meshes["disk"].sites
+    dataset_values = solution.film_solutions["disk"].total_field
 
     with pytest.raises(ValueError):
         _ = sc.visualization.cross_section(
             dataset_coords,
             dataset_values,
             cross_section_coords,
             interp_method="invalid",
@@ -134,96 +132,101 @@
             == len(cross_section_coords)
         )
     else:
         assert len(coords) == len(paths) == len(cross_sections) == 1
         assert np.array_equal(coords[0], cross_section_coords)
 
 
-def test_cross_section_bad_shape(solution):
-    dataset_coords = solution.device.points
-    dataset_values = solution.fields[list(solution.device.layers)[0]]
-    cross_section_coords = np.stack([np.ones(101)] * 3, axis=1)
+def test_cross_section_bad_shape(solution: sc.Solution):
+    dataset_coords = solution.device.meshes["disk"].sites
+    dataset_values = solution.film_solutions["disk"].total_field
+    cross_section_coords = np.array([np.ones(101)] * 3).T
 
     with pytest.raises(ValueError):
         _ = sc.visualization.cross_section(
             dataset_coords,
             dataset_values,
             cross_section_coords,
             interp_method="invalid",
         )
 
 
-@pytest.mark.parametrize("layers", [None, "layer0"])
+@pytest.mark.parametrize("films", [None, "disk", ["disk", "ring"]])
 @pytest.mark.parametrize("units", [None, "mA/um"])
 @pytest.mark.parametrize("streamplot", [False, True])
 @pytest.mark.parametrize("cross_section_coords", cross_section_coord_params)
+@pytest.mark.parametrize(
+    "dataset", ["field", "self_field", "applied_field", "field_from_other_films"]
+)
 # @pytest.mark.parametrize("auto_range_cutoff", [None, 1])
 # @pytest.mark.parametrize("share_color_scale", [False, True])
 # @pytest.mark.parametrize("symmetric_color_scale", [False, True])
 def test_plot_currents_and_fields(
     solution,
-    layers,
+    films,
     units,
     streamplot,
+    dataset,
     cross_section_coords,
     share_color_scale=True,
     symmetric_color_scale=True,
     auto_range_cutoff=1,
 ):
     with non_gui_backend():
         fig, ax = sc.plot_currents(
             solution,
-            grid_shape=(100, 100),
-            layers=layers,
+            grid_shape=200,
+            films=films,
             units=units,
             cross_section_coords=cross_section_coords,
             streamplot=streamplot,
             auto_range_cutoff=auto_range_cutoff,
             share_color_scale=share_color_scale,
             symmetric_color_scale=symmetric_color_scale,
         )
         plt.close(fig)
 
         fig, ax = sc.plot_fields(
             solution,
-            layers=layers,
+            dataset=dataset,
+            films=films,
             units=units,
             cross_section_coords=cross_section_coords,
             auto_range_cutoff=auto_range_cutoff,
             share_color_scale=share_color_scale,
             symmetric_color_scale=symmetric_color_scale,
         )
         plt.close(fig)
 
 
-@pytest.mark.parametrize("vector", [False, True])
 @pytest.mark.parametrize(
     "positions, zs",
     [
         (np.random.rand(200).reshape((-1, 2)), np.random.rand(100)),
         (np.random.rand(200).reshape((-1, 2)), 1),
         (np.random.rand(300).reshape((-1, 3)), None),
+        (None, 1),
     ],
 )
 @pytest.mark.parametrize("units", [None, "mT"])
 @pytest.mark.parametrize("auto_range_cutoff", [None, 1])
 @pytest.mark.parametrize("cross_section_coords", cross_section_coord_params)
 def test_plot_field_at_positions(
-    solution,
+    solution: sc.Solution,
     positions,
     zs,
     units,
     cross_section_coords,
     auto_range_cutoff,
-    vector,
 ):
+    if positions is None:
+        positions = list(solution.device.meshes.values())[0]
     with non_gui_backend():
         fig, ax = sc.plot_field_at_positions(
             solution,
             positions,
             zs=zs,
-            vector=vector,
             units=units,
             cross_section_coords=cross_section_coords,
             auto_range_cutoff=auto_range_cutoff,
         )
         plt.close(fig)
```

### Comparing `superscreen-0.8.2/superscreen.egg-info/PKG-INFO` & `superscreen-0.9.0/superscreen.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.8.2
+Version: 0.9.0
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
@@ -15,24 +15,24 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: jax
 License-File: LICENSE
 
 
 # SuperScreen
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/loganbvh/superscreen/lint-and-test.yml?branch=main) [![Documentation Status](https://readthedocs.org/projects/superscreen/badge/?version=latest)](https://superscreen.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/gh/loganbvh/superscreen/branch/main/graph/badge.svg?token=XW7LSY8WVD)](https://codecov.io/gh/loganbvh/superscreen) ![GitHub](https://img.shields.io/github/license/loganbvh/superscreen) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/376110557.svg)](https://zenodo.org/badge/latestdoi/376110557)
 
@@ -44,13 +44,13 @@
 
 ## Learn `SuperScreen`
 
 The documentation for `SuperScreen` can be found at [superscreen.readthedocs.io](https://superscreen.readthedocs.io/en/latest/).
 
 ## Try `SuperScreen`
 
-Click the badge below and navigate to `docs/notebooks/` to try `SuperScreen` interactively online via [Binder](https://mybinder.org/):
+Click the badge below to try `SuperScreen` interactively online via [Google Colab](https://colab.research.google.com/):
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/superscreen/HEAD)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/loganbvh/superscreen/blob/main/docs/notebooks/quickstart.ipynb)
```

### Comparing `superscreen-0.8.2/superscreen.egg-info/SOURCES.txt` & `superscreen-0.9.0/superscreen.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 LICENSE
 README.md
 setup.py
 superscreen/__init__.py
 superscreen/about.py
+superscreen/distance.py
 superscreen/fem.py
 superscreen/fluxoid.py
 superscreen/geometry.py
 superscreen/io.py
-superscreen/parallel.py
 superscreen/parameter.py
 superscreen/solution.py
-superscreen/solve.py
 superscreen/testing.py
 superscreen/units.py
 superscreen/version.py
 superscreen/visualization.py
 superscreen.egg-info/PKG-INFO
 superscreen.egg-info/SOURCES.txt
 superscreen.egg-info/dependency_links.txt
 superscreen.egg-info/requires.txt
 superscreen.egg-info/top_level.txt
 superscreen/device/__init__.py
-superscreen/device/components.py
 superscreen/device/device.py
+superscreen/device/edge_mesh.py
+superscreen/device/layer.py
 superscreen/device/mesh.py
-superscreen/device/transport.py
+superscreen/device/polygon.py
+superscreen/device/utils.py
+superscreen/solver/__init__.py
+superscreen/solver/solve.py
+superscreen/solver/solve_film.py
+superscreen/solver/utils.py
 superscreen/sources/__init__.py
 superscreen/sources/constant.py
 superscreen/sources/current.py
 superscreen/sources/dipole.py
 superscreen/sources/vortex.py
 superscreen/test/__init__.py
 superscreen/test/conftest.py
 superscreen/test/test_about.py
 superscreen/test/test_device.py
-superscreen/test/test_io.py
-superscreen/test/test_parallel.py
+superscreen/test/test_distance.py
 superscreen/test/test_parameter.py
+superscreen/test/test_polygon.py
 superscreen/test/test_solution.py
 superscreen/test/test_solve.py
 superscreen/test/test_sources.py
 superscreen/test/test_transport.py
 superscreen/test/test_visualization.py
```

