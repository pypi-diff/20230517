# Comparing `tmp/segment-geospatial-0.6.0.tar.gz` & `tmp/segment-geospatial-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.6.0.tar", last modified: Wed May 17 02:18:45 2023, max compression
+gzip compressed data, was "segment-geospatial-0.6.1.tar", last modified: Wed May 17 03:52:57 2023, max compression
```

## Comparing `segment-geospatial-0.6.0.tar` & `segment-geospatial-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68522 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    26605 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:52:57.767978 segment-geospatial-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-17 03:52:57.767978 segment-geospatial-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:52:57.767978 segment-geospatial-0.6.1/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68522 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26605 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:52:57.767978 segment-geospatial-0.6.1/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-17 03:52:57.000000 segment-geospatial-0.6.1/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-17 03:52:57.000000 segment-geospatial-0.6.1/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 03:52:57.000000 segment-geospatial-0.6.1/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:52:57.000000 segment-geospatial-0.6.1/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 03:52:57.000000 segment-geospatial-0.6.1/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 03:52:57.000000 segment-geospatial-0.6.1/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-17 03:52:57.767978 segment-geospatial-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-17 03:52:41.000000 segment-geospatial-0.6.1/setup.py
```

### Comparing `segment-geospatial-0.6.0/LICENSE` & `segment-geospatial-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.6.0/PKG-INFO` & `segment-geospatial-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.6.0
+Version: 0.6.1
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,15 @@
 # segment-geospatial
 
 [![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
+[![Docker Pulls](https://badgen.net/docker/pulls/giswqs/segment-geospatial?icon=docker&label=pulls)](https://hub.docker.com/r/giswqs/segment-geospatial/)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
```

### Comparing `segment-geospatial-0.6.0/README.md` & `segment-geospatial-0.6.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # segment-geospatial
 
 [![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
+[![Docker Pulls](https://badgen.net/docker/pulls/giswqs/segment-geospatial?icon=docker&label=pulls)](https://hub.docker.com/r/giswqs/segment-geospatial/)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
```

### Comparing `segment-geospatial-0.6.0/samgeo/common.py` & `segment-geospatial-0.6.1/samgeo/common.py`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.6.0/samgeo/samgeo.py` & `segment-geospatial-0.6.1/samgeo/samgeo.py`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.6.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.6.1/segment_geospatial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.6.0
+Version: 0.6.1
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,15 @@
 # segment-geospatial
 
 [![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
+[![Docker Pulls](https://badgen.net/docker/pulls/giswqs/segment-geospatial?icon=docker&label=pulls)](https://hub.docker.com/r/giswqs/segment-geospatial/)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
```

### Comparing `segment-geospatial-0.6.0/setup.py` & `segment-geospatial-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.6.0',
+    version='0.6.1',
     zip_safe=False,
 )
```

