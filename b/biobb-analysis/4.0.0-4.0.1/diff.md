# Comparing `tmp/biobb_analysis-4.0.0.tar.gz` & `tmp/biobb_analysis-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_analysis-4.0.0.tar", last modified: Tue Apr  4 15:47:39 2023, max compression
+gzip compressed data, was "dist/biobb_analysis-4.0.1.tar", last modified: Wed May 17 13:49:29 2023, max compression
```

## Comparing `biobb_analysis-4.0.0.tar` & `biobb_analysis-4.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:52:36.000000 biobb_analysis-4.0.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6256 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5212 2023-04-04 15:40:57.000000 biobb_analysis-4.0.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis/
--rw-r--r--   0 pau        (501) staff       (20)       82 2023-04-04 15:39:56.000000 biobb_analysis-4.0.0/biobb_analysis/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/
--rwxr-xr-x   0 pau        (501) staff       (20)      236 2021-06-11 09:52:36.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    15620 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13150 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_average.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12952 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_bfactor.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13114 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_convert.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13185 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_dry.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13193 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_image.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5691 2023-01-09 12:47:34.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_input.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13189 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_mask.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11296 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_rgyr.py
--rwxr-xr-x   0 pau        (501) staff       (20)    14805 2023-04-04 10:47:18.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_rms.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12899 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_rmsf.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12975 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_slice.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12759 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_snapshot.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13240 2023-03-02 13:40:59.000000 biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_strip.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/
--rwxr-xr-x   0 pau        (501) staff       (20)      153 2021-06-11 09:52:36.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    18989 2023-04-04 14:34:55.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)    15174 2023-03-28 09:23:12.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_cluster.py
--rwxr-xr-x   0 pau        (501) staff       (20)     8919 2023-01-09 12:47:34.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_energy.py
--rwxr-xr-x   0 pau        (501) staff       (20)    19177 2023-03-28 09:23:53.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_image.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11133 2023-03-28 09:24:12.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_rgyr.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11005 2023-03-28 09:24:40.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_rms.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12662 2023-03-28 09:25:34.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_trjconv_str.py
--rwxr-xr-x   0 pau        (501) staff       (20)    14030 2023-03-28 09:24:58.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_trjconv_str_ens.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13379 2023-04-04 10:57:24.000000 biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_trjconv_trj.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:52:36.000000 biobb_analysis-4.0.0/biobb_analysis/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6256 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     1328 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)     1199 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       20 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       15 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/biobb_analysis.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-04-04 15:47:39.000000 biobb_analysis-4.0.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2861 2023-04-04 15:39:04.000000 biobb_analysis-4.0.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:52:36.000000 biobb_analysis-4.0.1/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6372 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5380 2023-05-17 13:38:28.000000 biobb_analysis-4.0.1/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis/
+-rw-r--r--   0 pau        (501) staff       (20)       82 2023-05-17 13:37:33.000000 biobb_analysis-4.0.1/biobb_analysis/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/
+-rwxr-xr-x   0 pau        (501) staff       (20)      237 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    18276 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13377 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_average.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13184 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_bfactor.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13291 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_convert.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13387 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_dry.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13403 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_image.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5718 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_input.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13387 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_mask.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    11475 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rgyr.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    15009 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rms.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13109 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rmsf.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13179 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_slice.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12946 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_snapshot.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13411 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_strip.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/
+-rwxr-xr-x   0 pau        (501) staff       (20)      154 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    19167 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    17757 2023-05-11 08:49:51.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_cluster.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     9092 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_energy.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    19456 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_image.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    11312 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rgyr.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    11164 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rms.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12853 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    14280 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str_ens.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13379 2023-04-04 10:57:24.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_trj.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/biobb_analysis/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:52:36.000000 biobb_analysis-4.0.1/biobb_analysis/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6372 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     1328 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)     1199 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       20 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       15 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     2810 2023-05-17 13:35:32.000000 biobb_analysis-4.0.1/setup.py
```

### Comparing `biobb_analysis-4.0.0/LICENSE` & `biobb_analysis-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.0/PKG-INFO` & `biobb_analysis-4.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: biobb_analysis
-Version: 4.0.0
+Version: 4.0.1
 Summary: Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_analysis
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
 License: UNKNOWN
 Project-URL: Documentation, http://biobb_analysis.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
+[![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
-[![](https://img.shields.io/website?down_message=Offline&label=Biobb%20Website&up_message=Online&url=https%3A%2F%2Fmmb.irbbarcelona.org%2Fbiobb%2F)]()
+[![](https://img.shields.io/website?down_message=Offline&label=Biobb%20Website&up_message=Online&url=https%3A%2F%2Fmmb.irbbarcelona.org%2Fbiobb%2F)](https://mmb.irbbarcelona.org/biobb/)
 [![](https://img.shields.io/badge/Youtube-tutorial-blue?logo=youtube&logoColor=red)](https://www.youtube.com/watch?v=ou1DOGNs0xM)
 [![](https://zenodo.org/badge/DOI/10.1038/s41597-019-0177-4.svg)](https://doi.org/10.1038/s41597-019-0177-4)
 [![](https://img.shields.io/endpoint?color=brightgreen&url=https%3A%2F%2Fapi.juleskreuer.eu%2Fcitation-badge.php%3Fshield%26doi%3D10.1038%2Fs41597-019-0177-4)](https://www.nature.com/articles/s41597-019-0177-4#citeas)
 
 [![](https://docs.bioexcel.eu/biobb_analysis/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_analysis/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_analysis/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_analysis/coverage/)
 [![](https://docs.bioexcel.eu/biobb_analysis/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_analysis/flake8/)
@@ -54,76 +54,76 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.0.0"
+        pip install "biobb_analysis>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.0.0"
+        conda install -c bioconda "biobb_analysis>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.0.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.0--pyhdfd78af_0
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2022 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_analysis-4.0.0/README.md` & `biobb_analysis-4.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
+[![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
-[![](https://img.shields.io/website?down_message=Offline&label=Biobb%20Website&up_message=Online&url=https%3A%2F%2Fmmb.irbbarcelona.org%2Fbiobb%2F)]()
+[![](https://img.shields.io/website?down_message=Offline&label=Biobb%20Website&up_message=Online&url=https%3A%2F%2Fmmb.irbbarcelona.org%2Fbiobb%2F)](https://mmb.irbbarcelona.org/biobb/)
 [![](https://img.shields.io/badge/Youtube-tutorial-blue?logo=youtube&logoColor=red)](https://www.youtube.com/watch?v=ou1DOGNs0xM)
 [![](https://zenodo.org/badge/DOI/10.1038/s41597-019-0177-4.svg)](https://doi.org/10.1038/s41597-019-0177-4)
 [![](https://img.shields.io/endpoint?color=brightgreen&url=https%3A%2F%2Fapi.juleskreuer.eu%2Fcitation-badge.php%3Fshield%26doi%3D10.1038%2Fs41597-019-0177-4)](https://www.nature.com/articles/s41597-019-0177-4#citeas)
 
 [![](https://docs.bioexcel.eu/biobb_analysis/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_analysis/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_analysis/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_analysis/coverage/)
 [![](https://docs.bioexcel.eu/biobb_analysis/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_analysis/flake8/)
@@ -29,74 +30,74 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.0.0"
+        pip install "biobb_analysis>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.0.0"
+        conda install -c bioconda "biobb_analysis>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.0.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.0--pyhdfd78af_0
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2022 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_average.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_average.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Average class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, setup_structure, get_negative_mask, get_out_parameters, copy_instructions_file_to_container
 
 
 class CpptrajAverage(BiobbObject):
     """
     | biobb_analysis CpptrajAverage
     | Wrapper of the Ambertools Cpptraj module for calculating a structure average of a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -35,72 +36,72 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_average import cpptraj_average
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'format': 'pdb' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'format': 'pdb'
             }
-            cpptraj_average(input_top_path='/path/to/myTopology.top', 
-                            input_traj_path='/path/to/myTrajectory.dcd', 
-                            output_cpptraj_path='/path/to/newStructure.pdb', 
+            cpptraj_average(input_top_path='/path/to/myTopology.top',
+                            input_traj_path='/path/to/myTrajectory.dcd',
+                            output_cpptraj_path='/path/to/newStructure.pdb',
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -139,19 +140,20 @@
     def launch(self) -> int:
         """Execute the :class:`CpptrajAverage <ambertools.cpptraj_average.CpptrajAverage>` ambertools.cpptraj_average.CpptrajAverage object."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -169,22 +171,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_average(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajAverage <ambertools.cpptraj_average.CpptrajAverage>` class and
     execute the :meth:`launch() <ambertools.cpptraj_average.CpptrajAverage.launch>` method."""
 
-    return CpptrajAverage(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajAverage(input_top_path=input_top_path,
+                          input_traj_path=input_traj_path,
+                          output_cpptraj_path=output_cpptraj_path,
+                          properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Calculates a structure average of a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -194,15 +198,15 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed structure. Accepted formats: crd, netcdf, rst7, ncrst, dcd, pdb, mol2, binpos, trr, xtc, sqm.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_average(input_top_path=args.input_top_path, 
-                    input_traj_path=args.input_traj_path, 
-                    output_cpptraj_path=args.output_cpptraj_path, 
+    cpptraj_average(input_top_path=args.input_top_path,
+                    input_traj_path=args.input_traj_path,
+                    output_cpptraj_path=args.output_cpptraj_path,
                     properties=properties)
 
+
 if __name__ == '__main__':
     main()
-
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_bfactor.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_bfactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Bfactor class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, setup_structure, get_negative_mask, copy_instructions_file_to_container, get_mask, get_reference
 
 
 class CpptrajBfactor(BiobbObject):
     """
     | biobb_analysis CpptrajBfactor
     | Wrapper of the Ambertools Cpptraj module for calculating the Bfactor fluctuations of a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -36,23 +37,23 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_bfactor import cpptraj_bfactor
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'reference': 'first' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'reference': 'first'
             }
-            cpptraj_bfactor(input_top_path='/path/to/myTopology.top', 
-                            input_traj_path='/path/to/myTrajectory.dcd', 
+            cpptraj_bfactor(input_top_path='/path/to/myTopology.top',
+                            input_traj_path='/path/to/myTrajectory.dcd',
                             output_cpptraj_path='/path/to/newAnalysis.dat',
                             input_exp_path= '/path/to/myExpStructure.pdb',
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
@@ -60,48 +61,48 @@
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                input_exp_path = None, properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 input_exp_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path, "input_exp_path": input_exp_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path, "input_exp_path": input_exp_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.reference = properties.get('reference', 'first')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask, 'reference': self.reference }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask, 'reference': self.reference}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -141,24 +142,25 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajBfactor <ambertools.cpptraj_bfactor.CpptrajBfactor>` ambertools.cpptraj_bfactor.CpptrajBfactor object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -176,23 +178,25 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_bfactor(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, input_exp_path: str = None, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajBfactor <ambertools.cpptraj_bfactor.CpptrajBfactor>` class and
     execute the :meth:`launch() <ambertools.cpptraj_bfactor.CpptrajBfactor.launch>` method."""
 
-    return CpptrajBfactor(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    input_exp_path=input_exp_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajBfactor(input_top_path=input_top_path,
+                          input_traj_path=input_traj_path,
+                          output_cpptraj_path=output_cpptraj_path,
+                          input_exp_path=input_exp_path,
+                          properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Calculates the Bfactor fluctuations of a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -203,15 +207,16 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed analysis.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_bfactor(input_top_path=args.input_top_path, 
-                    input_traj_path=args.input_traj_path, 
-                    output_cpptraj_path=args.output_cpptraj_path, 
-                    input_exp_path=args.input_exp_path, 
+    cpptraj_bfactor(input_top_path=args.input_top_path,
+                    input_traj_path=args.input_traj_path,
+                    output_cpptraj_path=args.output_cpptraj_path,
+                    input_exp_path=args.input_exp_path,
                     properties=properties)
 
+
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_convert.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Convert class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_negative_mask, copy_instructions_file_to_container, get_out_parameters
 
 
 class CpptrajConvert(BiobbObject):
     """
     | biobb_analysis CpptrajConvert
     | Wrapper of the Ambertools Cpptraj module for converting between cpptraj compatible trajectory file formats and/or extracting a selection of atoms or frames.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -35,72 +36,72 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_convert import cpptraj_convert
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'format': 'netcdf' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'format': 'netcdf'
             }
-            cpptraj_convert(input_top_path='/path/to/myTopology.top', 
-                            input_traj_path='/path/to/myTrajectory.dcd', 
-                            output_cpptraj_path='/path/to/newTrajectory.netcdf', 
+            cpptraj_convert(input_top_path='/path/to/myTopology.top',
+                            input_traj_path='/path/to/myTrajectory.dcd',
+                            output_cpptraj_path='/path/to/newTrajectory.netcdf',
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
-            
+
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -131,57 +132,60 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajConvert <ambertools.cpptraj_convert.CpptrajConvert>` ambertools.cpptraj_convert.CpptrajConvert object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        # remove temporary folder(s)    
+        # remove temporary folder(s)
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             PurePath(self.instructions_file).parent
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_convert(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajConvert <ambertools.cpptraj_convert.CpptrajConvert>` class and
     execute the :meth:`launch() <ambertools.cpptraj_convert.CpptrajConvert.launch>` method."""
 
-    return CpptrajConvert(input_top_path=input_top_path, 
-                        input_traj_path=input_traj_path, 
-                        output_cpptraj_path=output_cpptraj_path,
-                        properties=properties, **kwargs).launch()
+    return CpptrajConvert(input_top_path=input_top_path,
+                          input_traj_path=input_traj_path,
+                          output_cpptraj_path=output_cpptraj_path,
+                          properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Converts between cpptraj compatible trajectory file formats and/or extracts a selection of atoms or frames.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -191,14 +195,15 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed structure.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_convert(input_top_path=args.input_top_path, 
-                    input_traj_path=args.input_traj_path, 
-                    output_cpptraj_path=args.output_cpptraj_path, 
+    cpptraj_convert(input_top_path=args.input_top_path,
+                    input_traj_path=args.input_traj_path,
+                    output_cpptraj_path=args.output_cpptraj_path,
                     properties=properties)
 
+
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_dry.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_strip.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python3
 
-"""Module containing the Cpptraj Dry class and the command line interface."""
+"""Module containing the Cpptraj Strip class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_out_parameters, copy_instructions_file_to_container, get_mask
 
 
-class CpptrajDry(BiobbObject):
+class CpptrajStrip(BiobbObject):
     """
-    | biobb_analysis CpptrajDry
-    | Wrapper of the Ambertools Cpptraj module for dehydrating a given cpptraj compatible trajectory stripping out solvent molecules and ions.
+    | biobb_analysis CpptrajStrip
+    | Wrapper of the Ambertools Cpptraj module for stripping a defined set of atoms (mask) from a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
 
     Args:
         input_top_path (str): Path to the input structure or topology file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/ambertools/cpptraj.parm.top>`_. Accepted formats: top (edam:format_3881), pdb (edam:format_1476), prmtop (edam:format_3881), parmtop (edam:format_3881), zip (edam:format_3987).
         input_traj_path (str): Path to the input trajectory to be processed.  File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/ambertools/cpptraj.traj.dcd>`_. Accepted formats: mdcrd (edam:format_3878), crd (edam:format_3878), cdf (edam:format_3650), netcdf (edam:format_3650), nc (edam:format_3650), restart (edam:format_3886), ncrestart (edam:format_3886), restartnc (edam:format_3886), dcd (edam:format_3878), charmm (edam:format_3887), cor (edam:format_2033), pdb (edam:format_1476), mol2 (edam:format_3816), trr (edam:format_3910), gro (edam:format_2033), binpos (edam:format_3885), xtc (edam:format_3875), cif (edam:format_1477), arc (edam:format_2333), sqm (edam:format_2033), sdf (edam:format_3814), conflib (edam:format_2033).
-        output_cpptraj_path (str): Path to the output processed trajectory. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/ambertools/ref_cpptraj.dry.netcdf>`_. Accepted formats: mdcrd (edam:format_3878), crd (edam:format_3878), netcdf (edam:format_3650), nc (edam:format_3650), rst7 (edam:format_3886), ncrst (edam:format_2033), dcd (edam:format_3878), pdb (edam:format_1476), mol2 (edam:format_3816), binpos (edam:format_3885), trr (edam:format_3910), xtc (edam:format_3875), sqm (edam:format_2033).
+        output_cpptraj_path (str): Path to the output processed trajectory. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/ambertools/ref_cpptraj.strip.netcdf>`_. Accepted formats: mdcrd (edam:format_3878), crd (edam:format_3878), netcdf (edam:format_3650), nc (edam:format_3650), rst7 (edam:format_3886), ncrst (edam:format_2033), dcd (edam:format_3878), pdb (edam:format_1476), mol2 (edam:format_3816), binpos (edam:format_3885), trr (edam:format_3910), xtc (edam:format_3875), sqm (edam:format_2033).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **start** (*int*) - (1) [1~100000|1] Starting frame for slicing.
             * **end** (*int*) - (-1) [-1~100000|1] Ending frame for slicing.
             * **steps** (*int*) - (1) [1~100000|1] Step for slicing.
             * **mask** (*str*) - ("all-atoms") Mask definition. Values: c-alpha (All c-alpha atoms; protein only), backbone (Backbone atoms), all-atoms (All system atoms), heavy-atoms (System heavy atoms; not hydrogen), side-chain (All not backbone atoms), solute (All system atoms except solvent atoms), ions (All ion molecules), solvent (All solvent atoms), AnyAmberFromatMask (Amber atom selection syntax like `@*`).
             * **format** (*str*) - ("netcdf") Output trajectory format. Values: crd (AMBER trajectory format), cdf (Format used by netCDF software library for writing and reading chromatography-MS data files), netcdf (Format used by netCDF software library for writing and reading chromatography-MS data files), nc (Format used by netCDF software library for writing and reading chromatography-MS data files), restart (AMBER coordinate/restart file with 6 coordinates per line), ncrestart (AMBER coordinate/restart file with 6 coordinates per line), restartnc (AMBER coordinate/restart file with 6 coordinates per line), dcd (AMBER trajectory format), charmm (Format of CHARMM Residue Topology Files (RTF)), cor (Charmm COR), pdb (Protein Data Bank format), mol2 (Complete and portable representation of a SYBYL molecule), trr (Trajectory of a simulation experiment used by GROMACS), gro (GROMACS structure), binpos (Translation of the ASCII atom coordinate format to binary code), xtc (Portable binary format for trajectories produced by GROMACS package), cif (Entry format of PDB database in mmCIF format), arc (Tinker ARC), sqm (SQM Input), sdf (One of a family of chemical-data file formats developed by MDL Information Systems), conflib (LMOD Conflib).
             * **binary_path** (*str*) - ("cpptraj") Path to the cpptraj executable binary.
@@ -34,73 +35,73 @@
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_analysis.ambertools.cpptraj_dry import cpptraj_dry
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'format': 'netcdf' 
+            from biobb_analysis.ambertools.cpptraj_strip import cpptraj_strip
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'format': 'netcdf'
             }
-            cpptraj_dry(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
-                        output_cpptraj_path='/path/to/newTrajectory.netcdf', 
+            cpptraj_strip(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
+                        output_cpptraj_path='/path/to/newTrajectory.netcdf',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
-         # Call parent class constructor
+        # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -108,53 +109,53 @@
             self.instructions_file = str(PurePath(fu.create_unique_dir()).joinpath(self.instructions_file))
         fu.create_name(prefix=self.prefix, step=self.step, name=self.instructions_file)
 
         # parm
         instructions_list.append('parm ' + container_io_dict["in"]["input_top_path"])
 
         # trajin
-        in_params = get_in_parameters(self.in_parameters, out_log)
+        in_parameters = self.in_parameters
+        in_params = ''
+        if in_parameters:
+            in_params = get_in_parameters(self.in_parameters, out_log, 'strip')
         instructions_list.append('trajin ' + container_io_dict["in"]["input_traj_path"] + ' ' + in_params)
 
-        # dry
-        mask_dry1 = get_negative_mask('solute', out_log)
-        instructions_list.append('strip ' + mask_dry1)
-        mask_dry2 = get_mask('heavy-atoms', out_log)
-        instructions_list.append('strip ' + mask_dry2)
-
         # mask
         mask = self.in_parameters.get('mask', '')
-        if mask:
-            strip_mask = get_negative_mask(mask, out_log)
-            instructions_list.append('strip ' + strip_mask)
+        if not mask or mask == 'None':
+            fu.log('No mask provided, exiting', out_log, self.global_log)
+            raise SystemExit('Mask parameter is mandatory')
+        strip_mask = get_mask(mask, out_log)
+        instructions_list.append('strip ' + strip_mask)
 
         # trajout
         out_params = get_out_parameters(self.out_parameters, out_log)
         instructions_list.append('trajout ' + container_io_dict["out"]["output_cpptraj_path"] + ' ' + out_params)
 
         # create .in file
         with open(self.instructions_file, 'w') as mdp:
             for line in instructions_list:
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
-        """Execute the :class:`CpptrajDry <ambertools.cpptraj_dry.CpptrajDry>` ambertools.cpptraj_dry.CpptrajDry object."""
-        
+        """Execute the :class:`CpptrajStrip <ambertools.cpptraj_strip.CpptrajStrip>` ambertools.cpptraj_strip.CpptrajStrip object."""
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -172,39 +173,42 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def cpptraj_dry(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
-    """Execute the :class:`CpptrajDry <ambertools.cpptraj_dry.CpptrajDry>` class and
-    execute the :meth:`launch() <ambertools.cpptraj_dry.CpptrajDry.launch>` method."""
-
-    return CpptrajDry(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    properties=properties, **kwargs).launch()
+
+def cpptraj_strip(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
+    """Execute the :class:`CpptrajStrip <ambertools.cpptraj_strip.CpptrajStrip>` class and
+    execute the :meth:`launch() <ambertools.cpptraj_strip.CpptrajStrip.launch>` method."""
+
+    return CpptrajStrip(input_top_path=input_top_path,
+                        input_traj_path=input_traj_path,
+                        output_cpptraj_path=output_cpptraj_path,
+                        properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
-    parser = argparse.ArgumentParser(description="Dehydrates a given cpptraj compatible trajectory stripping out solvent molecules and ions.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description="Strips a defined set of atoms (mask) from a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_top_path', required=True, help='Path to the input structure or topology file. Accepted formats: top, pdb, prmtop, parmtop, zip.')
     required_args.add_argument('--input_traj_path', required=True, help='Path to the input trajectory to be processed. Accepted formats: crd, cdf, netcdf, restart, ncrestart, restartnc, dcd, charmm, cor, pdb, mol2, trr, gro, binpos, xtc, cif, arc, sqm, sdf, conflib.')
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed trajectory.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_dry(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
-                properties=properties)
+    cpptraj_strip(input_top_path=args.input_top_path,
+                  input_traj_path=args.input_traj_path,
+                  output_cpptraj_path=args.output_cpptraj_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_image.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Image class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_mask, get_negative_mask, copy_instructions_file_to_container, get_out_parameters
 
 
 class CpptrajImage(BiobbObject):
     """
     | biobb_analysis CpptrajImage
     | Wrapper of the Ambertools Cpptraj module for correcting periodicity (image) from a given cpptraj trajectory file.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -35,72 +36,72 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_image import cpptraj_image
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'format': 'netcdf' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'format': 'netcdf'
             }
-            cpptraj_image(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
-                        output_cpptraj_path='/path/to/newTrajectory.netcdf', 
+            cpptraj_image(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
+                        output_cpptraj_path='/path/to/newTrajectory.netcdf',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
-    
+
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -137,24 +138,25 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajImage <ambertools.cpptraj_image.CpptrajImage>` ambertools.cpptraj_image.CpptrajImage object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -172,22 +174,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_image(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajImage <ambertools.cpptraj_image.CpptrajImage>` class and
     execute the :meth:`launch() <ambertools.cpptraj_image.CpptrajImage.launch>` method."""
 
-    return CpptrajImage(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajImage(input_top_path=input_top_path,
+                        input_traj_path=input_traj_path,
+                        output_cpptraj_path=output_cpptraj_path,
+                        properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Corrects periodicity (image) from a given cpptraj trajectory file.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -197,14 +201,15 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed trajectory.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_image(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
-                properties=properties)
+    cpptraj_image(input_top_path=args.input_top_path,
+                  input_traj_path=args.input_traj_path,
+                  output_cpptraj_path=args.output_cpptraj_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_input.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Input class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_in_path
 
 
 class CpptrajInput(BiobbObject):
     """
     | biobb_analysis CpptrajInput
     | Wrapper of the Ambertools Cpptraj module for performing multiple analysis and trajectory operations of a given trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -23,26 +23,26 @@
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_input import cpptraj_input
             prop = { }
-            cpptraj_input(input_instructions_path='/path/to/myInstructions.in', 
+            cpptraj_input(input_instructions_path='/path/to/myInstructions.in',
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
-            
+
     """
 
     def __init__(self, input_instructions_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
@@ -73,19 +73,20 @@
                 mdp.write(line.strip() + '\n')
 
         return output_instructions_path
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajInput <ambertools.cpptraj_input.CpptrajInput>` ambertools.cpptraj_input.CpptrajInput object."""
-        
+
         # Get local loggers from launchlogger decorator
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         output_instructions_path = self.create_instrucions_file() if not self.input_instructions_path else self.input_instructions_path
         check_in_path(output_instructions_path, self.out_log, self.__class__.__name__)
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', output_instructions_path]
@@ -94,32 +95,35 @@
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         return self.return_code
 
+
 def cpptraj_input(input_instructions_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajInput <ambertools.cpptraj_input.CpptrajInput>` class and
     execute the :meth:`launch() <ambertools.cpptraj_input.CpptrajInput.launch>` method."""
 
     return CpptrajInput(input_instructions_path=input_instructions_path,
                         properties=properties, **kwargs).launch()
 
+
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Performs multiple analysis and trajectory operations of a given trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_instructions_path', required=True, help='Path of the instructions file.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
-    #Specific call of each building block
-    cpptraj_input(input_instructions_path=args.input_instructions_path, 
-                properties=properties)
+    # Specific call of each building block
+    cpptraj_input(input_instructions_path=args.input_instructions_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_mask.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Mask class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_negative_mask, copy_instructions_file_to_container, get_out_parameters
 
 
 class CpptrajMask(BiobbObject):
     """
     | biobb_analysis CpptrajMask
     | Wrapper of the Ambertools Cpptraj module for extracting a selection of atoms from a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -35,72 +36,72 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_mask import cpptraj_mask
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'format': 'netcdf' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'format': 'netcdf'
             }
-            cpptraj_mask(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
-                        output_cpptraj_path='/path/to/newTrajectory.netcdf', 
+            cpptraj_mask(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
+                        output_cpptraj_path='/path/to/newTrajectory.netcdf',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -136,24 +137,25 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajMask <ambertools.cpptraj_mask.CpptrajMask>` ambertools.cpptraj_mask.CpptrajMask object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -171,22 +173,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_mask(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajMask <ambertools.cpptraj_mask.CpptrajMask>` class and
     execute the :meth:`launch() <ambertools.cpptraj_mask.CpptrajMask.launch>` method."""
 
-    return CpptrajMask(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajMask(input_top_path=input_top_path,
+                       input_traj_path=input_traj_path,
+                       output_cpptraj_path=output_cpptraj_path,
+                       properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Extracts a selection of atoms from a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -196,14 +200,15 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed trajectory.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_mask(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
-                properties=properties)
+    cpptraj_mask(input_top_path=args.input_top_path,
+                 input_traj_path=args.input_traj_path,
+                 output_cpptraj_path=args.output_cpptraj_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_rgyr.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rgyr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Rgyr class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_negative_mask, copy_instructions_file_to_container, setup_structure
 
 
 class CpptrajRgyr(BiobbObject):
     """
     | biobb_analysis CpptrajRgyr
     | Wrapper of the Ambertools Cpptraj module for computing the radius of gyration (Rgyr) from a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -34,70 +35,70 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_rgyr import cpptraj_rgyr
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha'
             }
-            cpptraj_rgyr(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
+            cpptraj_rgyr(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
                         output_cpptraj_path='/path/to/newAnalysis.dat',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
-            
+
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
         else:
@@ -129,24 +130,25 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajRgyr <ambertools.cpptraj_rgyr.CpptrajRgyr>` ambertools.cpptraj_rgyr.CpptrajRgyr object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -164,22 +166,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_rgyr(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajRgyr <ambertools.cpptraj_rgyr.CpptrajRgyr>` class and
     execute the :meth:`launch() <ambertools.cpptraj_rgyr.CpptrajRgyr.launch>` method."""
 
-    return CpptrajRgyr(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajRgyr(input_top_path=input_top_path,
+                       input_traj_path=input_traj_path,
+                       output_cpptraj_path=output_cpptraj_path,
+                       properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Computes the radius of gyration (Rgyr) from a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -189,14 +193,15 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output analysis.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_rgyr(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
-                properties=properties)
+    cpptraj_rgyr(input_top_path=args.input_top_path,
+                 input_traj_path=args.input_traj_path,
+                 output_cpptraj_path=args.output_cpptraj_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_rms.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Rms class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_negative_mask, copy_instructions_file_to_container, setup_structure, get_mask, get_reference_rms
 
 
 class CpptrajRms(BiobbObject):
     """
     | biobb_analysis CpptrajRms
     | Wrapper of the Ambertools Cpptraj module for calculating the Root Mean Square deviation (RMSd) of a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -40,58 +41,58 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_rms import cpptraj_rms
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'reference': 'first' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'reference': 'first'
             }
-            cpptraj_rms(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
-                        output_cpptraj_path='/path/to/newAnalysis.dat', 
+            cpptraj_rms(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
+                        output_cpptraj_path='/path/to/newAnalysis.dat',
                         input_exp_path= '/path/to/myExpStructure.pdb',
-                        output_traj_path='/path/to/newTrajectory.netcdf', 
+                        output_traj_path='/path/to/newTrajectory.netcdf',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                input_exp_path = None, output_traj_path = None, properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 input_exp_path=None, output_traj_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path, "input_exp_path": input_exp_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path, "output_traj_path": output_traj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path, "input_exp_path": input_exp_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path, "output_traj_path": output_traj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.reference = properties.get('reference', 'first')
         self.nofit = properties.get('nofit', False)
         self.norotate = properties.get('norotate', False)
         self.nomod = properties.get('nomod', False)
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
@@ -103,15 +104,15 @@
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
         if self.io_dict["out"]["output_traj_path"]:
             self.io_dict["out"]["output_traj_path"] = check_out_path(self.io_dict["out"]["output_traj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask, 'reference': self.reference }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask, 'reference': self.reference}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -139,15 +140,15 @@
 
         # reference
         reference = self.in_parameters.get('reference', '')
         inp_exp_pth = None
         if "input_exp_path" in container_io_dict["in"]:
             inp_exp_pth = container_io_dict["in"]["input_exp_path"]
         instructions_list += get_reference_rms(reference, container_io_dict["out"]["output_cpptraj_path"], inp_exp_pth, ref_mask, True,
-                                               self.__class__.__name__, out_log,  self.nofit, self.norotate, self.nomod)            
+                                               self.__class__.__name__, out_log, self.nofit, self.norotate, self.nomod)
 
         # trajout
         if ("output_traj_path" in container_io_dict["out"]):
             instructions_list.append('trajout ' + container_io_dict["out"]["output_traj_path"])
 
         # create .in file
         with open(self.instructions_file, 'w') as mdp:
@@ -155,24 +156,25 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajRms <ambertools.cpptraj_rms.CpptrajRms>` ambertools.cpptraj_rms.CpptrajRms object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -190,24 +192,26 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_rms(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, input_exp_path: str = None, output_traj_path: str = None, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajRms <ambertools.cpptraj_rms.CpptrajRms>` class and
     execute the :meth:`launch() <ambertools.cpptraj_rms.CpptrajRms.launch>` method."""
 
-    return CpptrajRms(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    input_exp_path=input_exp_path,
-                    output_traj_path=output_traj_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajRms(input_top_path=input_top_path,
+                      input_traj_path=input_traj_path,
+                      output_cpptraj_path=output_cpptraj_path,
+                      input_exp_path=input_exp_path,
+                      output_traj_path=output_traj_path,
+                      properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Calculates the Root Mean Square deviation (RMSd) of a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -219,16 +223,17 @@
     parser.add_argument('--output_traj_path', required=False, help='Path to the output processed trajectory.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_rms(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
-                input_exp_path=args.input_exp_path, 
-                output_traj_path=args.output_traj_path, 
+    cpptraj_rms(input_top_path=args.input_top_path,
+                input_traj_path=args.input_traj_path,
+                output_cpptraj_path=args.output_cpptraj_path,
+                input_exp_path=args.input_exp_path,
+                output_traj_path=args.output_traj_path,
                 properties=properties)
 
+
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_rmsf.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rmsf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Rmsf class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_negative_mask, copy_instructions_file_to_container, setup_structure, get_mask, get_reference
 
 
 class CpptrajRmsf(BiobbObject):
     """
     | biobb_analysis CpptrajRmsf
     | Wrapper of the Ambertools Cpptraj module for calculating the Root Mean Square fluctuations (RMSf) of a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -36,72 +37,72 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_rmsf import cpptraj_rmsf
-            prop = { 
+            prop = {
                 'start': 1,
                 'end': -1,
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'reference': 'first' 
+                'steps': 1,
+                'mask': 'c-alpha',
+                'reference': 'first'
             }
-            cpptraj_rmsf(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
-                        output_cpptraj_path='/path/to/newAnalysis.dat', 
+            cpptraj_rmsf(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
+                        output_cpptraj_path='/path/to/newAnalysis.dat',
                         input_exp_path= '/path/to/myExpStructure.pdb',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
-            
+
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                input_exp_path = None, properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 input_exp_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path, "input_exp_path": input_exp_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path, "input_exp_path": input_exp_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.reference = properties.get('reference', 'first')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask, 'reference': self.reference }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask, 'reference': self.reference}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -141,58 +142,61 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajRmsf <ambertools.cpptraj_rmsf.CpptrajRmsf>` ambertools.cpptraj_rmsf.CpptrajRmsf object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        # remove temporary folder(s)   
+        # remove temporary folder(s)
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             PurePath(self.instructions_file).parent
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_rmsf(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, input_exp_path: str = None, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajRmsf <ambertools.cpptraj_rmsf.CpptrajRmsf>` class and
     execute the :meth:`launch() <ambertools.cpptraj_rmsf.CpptrajRmsf.launch>` method."""
 
-    return CpptrajRmsf(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    input_exp_path=input_exp_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajRmsf(input_top_path=input_top_path,
+                       input_traj_path=input_traj_path,
+                       output_cpptraj_path=output_cpptraj_path,
+                       input_exp_path=input_exp_path,
+                       properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Calculates the Root Mean Square fluctuations (RMSf) of a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -203,15 +207,16 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed analysis.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_rmsf(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
-                input_exp_path=args.input_exp_path, 
-                properties=properties)
+    cpptraj_rmsf(input_top_path=args.input_top_path,
+                 input_traj_path=args.input_traj_path,
+                 output_cpptraj_path=args.output_cpptraj_path,
+                 input_exp_path=args.input_exp_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_slice.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Slice class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_out_parameters, get_negative_mask, copy_instructions_file_to_container
 
 
 class CpptrajSlice(BiobbObject):
     """
     | biobb_analysis CpptrajSlice
     | Wrapper of the Ambertools Cpptraj module for extracting a particular trajectory slice from a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -35,72 +36,72 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_slice import cpptraj_slice
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'format': 'netcdf' 
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'format': 'netcdf'
             }
-            cpptraj_slice(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
-                        output_cpptraj_path='/path/to/newTrajectory.netcdf', 
+            cpptraj_slice(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
+                        output_cpptraj_path='/path/to/newTrajectory.netcdf',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -131,24 +132,25 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajSlice <ambertools.cpptraj_slice.CpptrajSlice>` ambertools.cpptraj_slice.CpptrajSlice object."""
-        
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -166,22 +168,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_slice(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajSlice <ambertools.cpptraj_slice.CpptrajSlice>` class and
     execute the :meth:`launch() <ambertools.cpptraj_slice.CpptrajSlice.launch>` method."""
 
-    return CpptrajSlice(input_top_path=input_top_path, 
-                    input_traj_path=input_traj_path, 
-                    output_cpptraj_path=output_cpptraj_path,
-                    properties=properties, **kwargs).launch()
+    return CpptrajSlice(input_top_path=input_top_path,
+                        input_traj_path=input_traj_path,
+                        output_cpptraj_path=output_cpptraj_path,
+                        properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Extracts a particular trajectory slice from a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
@@ -191,14 +195,15 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed trajectory.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_slice(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
-                properties=properties)
+    cpptraj_slice(input_top_path=args.input_top_path,
+                  input_traj_path=args.input_traj_path,
+                  output_cpptraj_path=args.output_cpptraj_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_snapshot.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Cpptraj Snapshot class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_out_parameters, get_negative_mask, copy_instructions_file_to_container
 
 
 class CpptrajSnapshot(BiobbObject):
     """
     | biobb_analysis CpptrajSnapshot
     | Wrapper of the Ambertools Cpptraj module for extracting a particular snapshot from a given cpptraj compatible trajectory.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
@@ -33,68 +34,68 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.ambertools.cpptraj_snapshot import cpptraj_snapshot
-            prop = { 
-                'snapshot': 12, 
-                'mask': 'c-alpha', 
-                'format': 'pdb' 
+            prop = {
+                'snapshot': 12,
+                'mask': 'c-alpha',
+                'format': 'pdb'
             }
-            cpptraj_snapshot(input_top_path='/path/to/myTopology.top', 
-                            input_traj_path='/path/to/myTrajectory.dcd', 
-                            output_cpptraj_path='/path/to/newStructure.pdb', 
+            cpptraj_snapshot(input_top_path='/path/to/myTopology.top',
+                            input_traj_path='/path/to/myTrajectory.dcd',
+                            output_cpptraj_path='/path/to/newStructure.pdb',
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
-        self.snapshot =  properties.get('snapshot', 1)
+        self.snapshot = properties.get('snapshot', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'snapshot': self.snapshot, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'snapshot': self.snapshot, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -125,24 +126,25 @@
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`CpptrajSnapshot <ambertools.cpptraj_snapshot.CpptrajSnapshot>` ambertools.cpptraj_snapshot.CpptrajSnapshot object."""
-        
-         # check input/output paths and parameters
+
+        # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -160,22 +162,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_snapshot(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`CpptrajSnapshot <ambertools.cpptraj_snapshot.CpptrajSnapshot>` class and
     execute the :meth:`launch() <ambertools.cpptraj_snapshot.CpptrajSnapshot.launch>` method."""
 
-    return CpptrajSnapshot(input_top_path=input_top_path, 
-                            input_traj_path=input_traj_path, 
-                            output_cpptraj_path=output_cpptraj_path,
-                            properties=properties, **kwargs).launch()
+    return CpptrajSnapshot(input_top_path=input_top_path,
+                           input_traj_path=input_traj_path,
+                           output_cpptraj_path=output_cpptraj_path,
+                           properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Extracts a particular snapshot from a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=True, help='Configuration file')
 
     # Specific args of each building block
@@ -185,14 +189,15 @@
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed structure.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_snapshot(input_top_path=args.input_top_path, 
-                    input_traj_path=args.input_traj_path, 
-                    output_cpptraj_path=args.output_cpptraj_path, 
-                    properties=properties)
+    cpptraj_snapshot(input_top_path=args.input_top_path,
+                     input_traj_path=args.input_traj_path,
+                     output_cpptraj_path=args.output_cpptraj_path,
+                     properties=properties)
+
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/ambertools/cpptraj_strip.py` & `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_dry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python3
 
-"""Module containing the Cpptraj Strip class and the command line interface."""
+"""Module containing the Cpptraj Dry class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.ambertools.common import *
+from biobb_analysis.ambertools.common import get_default_value, check_top_path, check_traj_path, check_out_path, get_binary_path, get_in_parameters, get_mask, get_negative_mask, copy_instructions_file_to_container, get_out_parameters
 
 
-class CpptrajStrip(BiobbObject):
+class CpptrajDry(BiobbObject):
     """
-    | biobb_analysis CpptrajStrip
-    | Wrapper of the Ambertools Cpptraj module for stripping a defined set of atoms (mask) from a given cpptraj compatible trajectory.
+    | biobb_analysis CpptrajDry
+    | Wrapper of the Ambertools Cpptraj module for dehydrating a given cpptraj compatible trajectory stripping out solvent molecules and ions.
     | Cpptraj (the successor to ptraj) is the main program in Ambertools for processing coordinate trajectories and data files. The parameter names and defaults are the same as the ones in the official `Cpptraj manual <https://amber-md.github.io/cpptraj/CPPTRAJ.xhtml>`_.
 
     Args:
         input_top_path (str): Path to the input structure or topology file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/ambertools/cpptraj.parm.top>`_. Accepted formats: top (edam:format_3881), pdb (edam:format_1476), prmtop (edam:format_3881), parmtop (edam:format_3881), zip (edam:format_3987).
         input_traj_path (str): Path to the input trajectory to be processed.  File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/ambertools/cpptraj.traj.dcd>`_. Accepted formats: mdcrd (edam:format_3878), crd (edam:format_3878), cdf (edam:format_3650), netcdf (edam:format_3650), nc (edam:format_3650), restart (edam:format_3886), ncrestart (edam:format_3886), restartnc (edam:format_3886), dcd (edam:format_3878), charmm (edam:format_3887), cor (edam:format_2033), pdb (edam:format_1476), mol2 (edam:format_3816), trr (edam:format_3910), gro (edam:format_2033), binpos (edam:format_3885), xtc (edam:format_3875), cif (edam:format_1477), arc (edam:format_2333), sqm (edam:format_2033), sdf (edam:format_3814), conflib (edam:format_2033).
-        output_cpptraj_path (str): Path to the output processed trajectory. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/ambertools/ref_cpptraj.strip.netcdf>`_. Accepted formats: mdcrd (edam:format_3878), crd (edam:format_3878), netcdf (edam:format_3650), nc (edam:format_3650), rst7 (edam:format_3886), ncrst (edam:format_2033), dcd (edam:format_3878), pdb (edam:format_1476), mol2 (edam:format_3816), binpos (edam:format_3885), trr (edam:format_3910), xtc (edam:format_3875), sqm (edam:format_2033).
+        output_cpptraj_path (str): Path to the output processed trajectory. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/ambertools/ref_cpptraj.dry.netcdf>`_. Accepted formats: mdcrd (edam:format_3878), crd (edam:format_3878), netcdf (edam:format_3650), nc (edam:format_3650), rst7 (edam:format_3886), ncrst (edam:format_2033), dcd (edam:format_3878), pdb (edam:format_1476), mol2 (edam:format_3816), binpos (edam:format_3885), trr (edam:format_3910), xtc (edam:format_3875), sqm (edam:format_2033).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **start** (*int*) - (1) [1~100000|1] Starting frame for slicing.
             * **end** (*int*) - (-1) [-1~100000|1] Ending frame for slicing.
             * **steps** (*int*) - (1) [1~100000|1] Step for slicing.
             * **mask** (*str*) - ("all-atoms") Mask definition. Values: c-alpha (All c-alpha atoms; protein only), backbone (Backbone atoms), all-atoms (All system atoms), heavy-atoms (System heavy atoms; not hydrogen), side-chain (All not backbone atoms), solute (All system atoms except solvent atoms), ions (All ion molecules), solvent (All solvent atoms), AnyAmberFromatMask (Amber atom selection syntax like `@*`).
             * **format** (*str*) - ("netcdf") Output trajectory format. Values: crd (AMBER trajectory format), cdf (Format used by netCDF software library for writing and reading chromatography-MS data files), netcdf (Format used by netCDF software library for writing and reading chromatography-MS data files), nc (Format used by netCDF software library for writing and reading chromatography-MS data files), restart (AMBER coordinate/restart file with 6 coordinates per line), ncrestart (AMBER coordinate/restart file with 6 coordinates per line), restartnc (AMBER coordinate/restart file with 6 coordinates per line), dcd (AMBER trajectory format), charmm (Format of CHARMM Residue Topology Files (RTF)), cor (Charmm COR), pdb (Protein Data Bank format), mol2 (Complete and portable representation of a SYBYL molecule), trr (Trajectory of a simulation experiment used by GROMACS), gro (GROMACS structure), binpos (Translation of the ASCII atom coordinate format to binary code), xtc (Portable binary format for trajectories produced by GROMACS package), cif (Entry format of PDB database in mmCIF format), arc (Tinker ARC), sqm (SQM Input), sdf (One of a family of chemical-data file formats developed by MDL Information Systems), conflib (LMOD Conflib).
             * **binary_path** (*str*) - ("cpptraj") Path to the cpptraj executable binary.
@@ -34,73 +35,73 @@
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_analysis.ambertools.cpptraj_strip import cpptraj_strip
-            prop = { 
-                'start': 1, 
-                'end': -1, 
-                'steps': 1, 
-                'mask': 'c-alpha', 
-                'format': 'netcdf' 
+            from biobb_analysis.ambertools.cpptraj_dry import cpptraj_dry
+            prop = {
+                'start': 1,
+                'end': -1,
+                'steps': 1,
+                'mask': 'c-alpha',
+                'format': 'netcdf'
             }
-            cpptraj_strip(input_top_path='/path/to/myTopology.top', 
-                        input_traj_path='/path/to/myTrajectory.dcd', 
-                        output_cpptraj_path='/path/to/newTrajectory.netcdf', 
+            cpptraj_dry(input_top_path='/path/to/myTopology.top',
+                        input_traj_path='/path/to/myTrajectory.dcd',
+                        output_cpptraj_path='/path/to/newTrajectory.netcdf',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: Ambertools Cpptraj
             * version: >=20.0
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path, 
-                properties=None, **kwargs) -> None:
+    def __init__(self, input_top_path, input_traj_path, output_cpptraj_path,
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_top_path": input_top_path, "input_traj_path": input_traj_path }, 
-            "out": { "output_cpptraj_path": output_cpptraj_path } 
+        self.io_dict = {
+            "in": {"input_top_path": input_top_path, "input_traj_path": input_traj_path},
+            "out": {"output_cpptraj_path": output_cpptraj_path}
         }
 
         # Properties specific for BB
         self.instructions_file = get_default_value('instructions_file')
         self.start = properties.get('start', 1)
         self.end = properties.get('end', -1)
-        self.steps =  properties.get('steps', 1)
+        self.steps = properties.get('steps', 1)
         self.mask = properties.get('mask', 'all-atoms')
         self.format = properties.get('format', 'netcdf')
         self.properties = properties
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_top_path"], self.input_top_path_orig = check_top_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_cpptraj_path"] = check_out_path(self.io_dict["out"]["output_cpptraj_path"], out_log, self.__class__.__name__)
-        self.in_parameters = { 'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask }
-        self.out_parameters = { 'format': self.format }
+        self.in_parameters = {'start': self.start, 'end': self.end, 'step': self.steps, 'mask': self.mask}
+        self.out_parameters = {'format': self.format}
 
     def create_instructions_file(self, container_io_dict, out_log, err_log):
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
@@ -108,52 +109,54 @@
             self.instructions_file = str(PurePath(fu.create_unique_dir()).joinpath(self.instructions_file))
         fu.create_name(prefix=self.prefix, step=self.step, name=self.instructions_file)
 
         # parm
         instructions_list.append('parm ' + container_io_dict["in"]["input_top_path"])
 
         # trajin
-        in_parameters = self.in_parameters
-        in_params = ''
-        if in_parameters:
-            in_params = get_in_parameters(self.in_parameters, out_log, 'strip')
+        in_params = get_in_parameters(self.in_parameters, out_log)
         instructions_list.append('trajin ' + container_io_dict["in"]["input_traj_path"] + ' ' + in_params)
 
+        # dry
+        mask_dry1 = get_negative_mask('solute', out_log)
+        instructions_list.append('strip ' + mask_dry1)
+        mask_dry2 = get_mask('heavy-atoms', out_log)
+        instructions_list.append('strip ' + mask_dry2)
+
         # mask
         mask = self.in_parameters.get('mask', '')
-        if not mask or mask == 'None':
-            fu.log('No mask provided, exiting', out_log, self.global_log)
-            raise SystemExit('Mask parameter is mandatory')
-        strip_mask = get_mask(mask, out_log)
-        instructions_list.append('strip ' + strip_mask)
+        if mask:
+            strip_mask = get_negative_mask(mask, out_log)
+            instructions_list.append('strip ' + strip_mask)
 
         # trajout
         out_params = get_out_parameters(self.out_parameters, out_log)
         instructions_list.append('trajout ' + container_io_dict["out"]["output_cpptraj_path"] + ' ' + out_params)
 
         # create .in file
         with open(self.instructions_file, 'w') as mdp:
             for line in instructions_list:
                 mdp.write(line.strip() + '\n')
 
         return self.instructions_file
 
     @launchlogger
     def launch(self) -> int:
-        """Execute the :class:`CpptrajStrip <ambertools.cpptraj_strip.CpptrajStrip>` ambertools.cpptraj_strip.CpptrajStrip object."""
-        
+        """Execute the :class:`CpptrajDry <ambertools.cpptraj_dry.CpptrajDry>` ambertools.cpptraj_dry.CpptrajDry object."""
+
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
-        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log) 
+        self.create_instructions_file(self.stage_io_dict, self.out_log, self.err_log)
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict['unique_dir'])
 
         # create cmd and launch execution
         self.cmd = [self.binary_path, '-i', self.instructions_file]
@@ -171,39 +174,42 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def cpptraj_strip(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
-    """Execute the :class:`CpptrajStrip <ambertools.cpptraj_strip.CpptrajStrip>` class and
-    execute the :meth:`launch() <ambertools.cpptraj_strip.CpptrajStrip.launch>` method."""
-
-    return CpptrajStrip(input_top_path=input_top_path, 
-                            input_traj_path=input_traj_path, 
-                            output_cpptraj_path=output_cpptraj_path,
-                            properties=properties, **kwargs).launch()
+
+def cpptraj_dry(input_top_path: str, input_traj_path: str, output_cpptraj_path: str, properties: dict = None, **kwargs) -> int:
+    """Execute the :class:`CpptrajDry <ambertools.cpptraj_dry.CpptrajDry>` class and
+    execute the :meth:`launch() <ambertools.cpptraj_dry.CpptrajDry.launch>` method."""
+
+    return CpptrajDry(input_top_path=input_top_path,
+                      input_traj_path=input_traj_path,
+                      output_cpptraj_path=output_cpptraj_path,
+                      properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
-    parser = argparse.ArgumentParser(description="Strips a defined set of atoms (mask) from a given cpptraj compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description="Dehydrates a given cpptraj compatible trajectory stripping out solvent molecules and ions.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_top_path', required=True, help='Path to the input structure or topology file. Accepted formats: top, pdb, prmtop, parmtop, zip.')
     required_args.add_argument('--input_traj_path', required=True, help='Path to the input trajectory to be processed. Accepted formats: crd, cdf, netcdf, restart, ncrestart, restartnc, dcd, charmm, cor, pdb, mol2, trr, gro, binpos, xtc, cif, arc, sqm, sdf, conflib.')
     required_args.add_argument('--output_cpptraj_path', required=True, help='Path to the output processed trajectory.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    cpptraj_strip(input_top_path=args.input_top_path, 
-                input_traj_path=args.input_traj_path, 
-                output_cpptraj_path=args.output_cpptraj_path, 
+    cpptraj_dry(input_top_path=args.input_top_path,
+                input_traj_path=args.input_traj_path,
+                output_cpptraj_path=args.output_cpptraj_path,
                 properties=properties)
 
+
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/common.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,37 +143,35 @@
         raise SystemExit(classname + ': Format %s in output file is not compatible' % file_extension[1:])
     return path
 
 
 def get_default_value(key):
     """ Gives default values according to the given key """
 
-    default_values = {
-            "instructions_file": "instructions.in",
-            "binary_path": "gmx",
-            "terms": ["Potential"],
-            "selection": "System",
-            "xvg": "none",
-            "dista": False,
-            "method": "linkage",
-            "cutoff": 0.1,
-            "cluster_selection": "System",
-            "fit_selection": "System",
-            "center_selection": "System",
-            "output_selection": "System",
-            "pbc": "mol",
-            "center": True,
-            "fit": "none",
-            "ur": "compact",
-            "skip": 1,
-            "start": 0,
-            "end": 0,
-            "dt": 0,
-            "ot_str_ens": "pdb"
-        }
+    default_values = {"instructions_file": "instructions.in",
+                      "binary_path": "gmx",
+                      "terms": ["Potential"],
+                      "selection": "System",
+                      "xvg": "none",
+                      "dista": False,
+                      "method": "linkage",
+                      "cutoff": 0.1,
+                      "cluster_selection": "System",
+                      "fit_selection": "System",
+                      "center_selection": "System",
+                      "output_selection": "System",
+                      "pbc": "mol",
+                      "center": True,
+                      "fit": "none",
+                      "ur": "compact",
+                      "skip": 1,
+                      "start": 0,
+                      "end": 0,
+                      "dt": 0,
+                      "ot_str_ens": "pdb"}
 
     return default_values[key]
 
 
 def get_binary_path(properties, type):
     """ Gets binary path """
     return properties.get(type, get_default_value(type))
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_cluster.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,209 +1,194 @@
 #!/usr/bin/env python3
 
-"""Module containing the GMX Cluster class and the command line interface."""
+# AFEGIR PARÀMETRES DE GMX_IMAGE: PBC, CENTER, UR, FIT (NOMÉS APPEND SI L'USUARI ELS AFEGEIX)
+
+"""Module containing the GMX TrjConvStr class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.gromacs.common import *
+from biobb_analysis.gromacs.common import get_binary_path, check_input_path, check_traj_path, check_index_path, get_selection_index_file, get_selection, check_out_traj_path
 
 
-class GMXCluster(BiobbObject):
+class GMXTrjConvStr(BiobbObject):
     """
-    | biobb_analysis GMXCluster
-    | Wrapper of the GROMACS cluster module for clustering structures from a given GROMACS compatible trajectory.
-    | `GROMACS cluster <http://manual.gromacs.org/current/onlinehelp/gmx-cluster.html>`_ can cluster structures using several different methods. Distances between structures can be determined from a trajectory. RMS deviation after fitting or RMS deviation of atom-pair distances can be used to define the distance between structures.
+    | biobb_analysis GMXTrjConvStr
+    | Wrapper of the GROMACS trjconv module for converting between GROMACS compatible structure file formats and/or extracting a selection of atoms.
+    | GROMACS trjconv module can convert trajectory files in many ways. See the `GROMACS trjconv <http://manual.gromacs.org/documentation/2018/onlinehelp/gmx-trjconv.html>`_ official documentation for further information.
 
     Args:
-        input_structure_path (str): Path to the input structure file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/topology.tpr>`_. Accepted formats: tpr (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), brk (edam:format_2033), ent (edam:format_1476).
-        input_traj_path (str): Path to the GROMACS trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/trajectory.trr>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
+        input_structure_path (str): Path to the input structure file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/trajectory.trr>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
+        input_top_path (str): Path to the GROMACS input topology file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/topology.tpr>`_. Accepted formats: tpr (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), brk (edam:format_2033), ent (edam:format_1476).
         input_index_path (str) (Optional): Path to the GROMACS index file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/index.ndx>`_. Accepted formats: ndx (edam:format_2033).
-        output_pdb_path (str): Path to the output cluster file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_cluster.pdb>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
+        output_str_path (str): Path to the output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_trjconv.str.pdb>`_. Accepted formats: pdb (edam:format_1476), xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), tng (edam:format_3876).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
-            * **fit_selection** (*str*) - ("System") Group where the fitting will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups).
-            * **output_selection** (*str*) - ("System") Group that is going to be written in the output trajectory. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups).
-            * **dista** (*bool*) - (False) Use RMSD of distances instead of RMS deviation.
-            * **method** (*str*) - ("linkage") Method for cluster determination. Values: linkage (Add a structure to a cluster when its distance to any element of the cluster is less than cutoff), jarvis-patrick (Add a structure to a cluster when this structure and a structure in the cluster have each other as neighbors and they have a least P neighbors in common), monte-carlo (Reorder the RMSD matrix using Monte Carlo such that the order of the frames is using the smallest possible increments), diagonalization (Diagonalize the RMSD matrix), gromos (Count number of neighbors using cut-off and take structure with largest number of neighbors with all its neighbors as cluster and eliminate it from the pool of clusters).
-            * **cutoff** (*float*) - (0.1) [0~10|0.1] RMSD cut-off (nm) for two structures to be neighbor.
+            * **selection** (*str*) - ("System") Group where the trjconv will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups), DNA (all DNA atoms), RNA (all RNA atoms), Protein_DNA (all Protein-DNA complex atoms), Protein_RNA (all Protein-RNA complex atoms), Protein_DNA_RNA (all Protein-DNA-RNA complex atoms), DNA_RNA (all DNA-RNA complex atoms).
+            * **pbc** (*str*) - ("mol") PBC treatment (see help text for full description). Values: none (No PBC treatment), mol (Puts the center of mass of molecules in the box), res (Puts the center of mass of residues in the box), atom (Puts all the atoms in the box), nojump (Checks if atoms jump across the box and then puts them back), cluster (Clusters all the atoms in the selected index such that they are all closest to the center of mass of the cluster which is iteratively updated), whole (Only makes broken molecules whole).
+            * **center** (*bool*) - (True) Center atoms in box.
+            * **ur** (*str*) - ("compact") Unit-cell representation. Values: rect (It's the ordinary brick shape), tric (It's the triclinic unit cell), compact (Puts all atoms at the closest distance from the center of the box).
+            * **fit** (*str*) - ("none") Fit molecule to ref structure in the structure file. Values: none, rot+trans, rotxy+transxy, translation, transxy, progressive.
             * **binary_path** (*str*) - ("gmx") Path to the GROMACS executable binary.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('gromacs/gromacs:2022.2') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_analysis.gromacs.gmx_cluster import gmx_cluster
-            prop = { 
-                'fit_selection': 'System', 
-                'output_selection': 'System', 
-                'method': 'linkage' 
+            from biobb_analysis.gromacs.gmx_trjconv_str import gmx_trjconv_str
+            prop = {
+                'selection': 'System'
             }
-            gmx_cluster(input_structure_path='/path/to/myStructure.tpr', 
-                        input_traj_path='/path/to/myTrajectory.trr', 
-                        input_index_path='/path/to/myIndex.ndx', 
-                        output_pdb_path='/path/to/newStructure.pdb', 
-                        properties=prop)
+            gmx_trjconv_str(input_structure_path='/path/to/myStructure.trr',
+                            input_top_path='/path/to/myTopology.tpr',
+                            output_str_path='/path/to/newStructure.pdb',
+                            input_index_path='/path/to/myIndex.ndx',
+                            properties=prop)
 
     Info:
         * wrapped_software:
-            * name: GROMACS cluster
+            * name: GROMACS trjconv
             * version: >=2019.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_structure_path, input_traj_path, output_pdb_path, 
-                input_index_path=None, properties=None, **kwargs) -> None:
+    def __init__(self, input_structure_path, input_top_path, output_str_path,
+                 input_index_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_structure_path": input_structure_path, "input_traj_path": input_traj_path, "input_index_path": input_index_path }, 
-            "out": { "output_pdb_path": output_pdb_path } 
+        self.io_dict = {
+            "in": {"input_structure_path": input_structure_path, "input_top_path": input_top_path, "input_index_path": input_index_path},
+            "out": {"output_str_path": output_str_path}
         }
 
         # Properties specific for BB
-        self.fit_selection = properties.get('fit_selection', "System")
-        self.output_selection = properties.get('output_selection', "System")
-        self.method = properties.get('method', "linkage")
-        self.dista = properties.get('dista', False)
-        self.cutoff = properties.get('cutoff', 0.1)
+        self.selection = properties.get('selection', "System")
+        self.pbc = properties.get('pbc', None)
+        self.center = properties.get('dista', None)
+        self.ur = properties.get('ur', None)
+        self.fit = properties.get('fit', None)
         self.properties = properties
 
         # Properties common in all GROMACS BB
         self.binary_path = get_binary_path(properties, 'binary_path')
-        
+
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
-        # Internal parameters
-        self.xvg_path = fu.create_name(prefix=self.prefix, step=self.step, name=properties.get('xvg_path', 'rmsd-dist.xvg'))
-        self.xpm_path = fu.create_name(prefix=self.prefix, step=self.step, name=properties.get('xpm_path', 'rmsd-clust.xpm'))
-        self.log_path = fu.create_name(prefix=self.prefix, step=self.step, name=properties.get('log_path', 'cluster.log'))
-
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
-        self.io_dict["in"]["input_structure_path"] = check_input_path(self.io_dict["in"]["input_structure_path"], out_log, self.__class__.__name__)
-        self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
+        self.io_dict["in"]["input_structure_path"] = check_traj_path(self.io_dict["in"]["input_structure_path"], out_log, self.__class__.__name__)
+        self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_index_path"] = check_index_path(self.io_dict["in"]["input_index_path"], out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_pdb_path"] = check_out_pdb_path(self.io_dict["out"]["output_pdb_path"], out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_str_path"] = check_out_traj_path(self.io_dict["out"]["output_str_path"], out_log, self.__class__.__name__)
         if not self.io_dict["in"]["input_index_path"]:
-            self.fit_selection = get_image_selection(self.properties, 'fit_selection', out_log, self.__class__.__name__)
-            self.output_selection = get_image_selection(self.properties, 'output_selection', out_log, self.__class__.__name__)
+            self.selection = get_selection(self.properties, out_log, self.__class__.__name__)
         else:
-            self.fit_selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'fit_selection', out_log, self.__class__.__name__)
-            self.output_selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'output_selection', out_log, self.__class__.__name__)
-        self.dista = get_dista(self.properties, out_log, self.__class__.__name__)
-        self.method = get_method(self.properties, out_log, self.__class__.__name__)
-        self.cutoff = get_cutoff(self.properties, out_log, self.__class__.__name__)
+            self.selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'selection', out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self) -> int:
-        """Execute the :class:`GMXCluster <gromacs.gmx_cluster.GMXCluster>` gromacs.gmx_cluster.GMXCluster object."""
+        """Execute the :class:`GMXTrjConvStr <gromacs.gmx_trjconv_str.GMXTrjConvStr>` gromacs.gmx_trjconv_str.GMXTrjConvStr object."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
         if self.check_restart():
             return 0
 
         # standard input
-        self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.fit_selection} {self.output_selection}')
+        self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.selection}')
         self.stage_files()
 
-        # if container execution, add container_volume_path to log, xvg & xpm (because docker doesn't allow to write teses files out of the /tmp folder)
-        if self.container_path:
-            self.log_path = str(PurePath(self.container_volume_path).joinpath(self.log_path))
-            self.xvg_path = str(PurePath(self.container_volume_path).joinpath(self.xvg_path))
-            self.xpm_path = str(PurePath(self.container_volume_path).joinpath(self.xpm_path))
-
-        self.cmd = [self.binary_path, 'cluster',
-               '-g', self.log_path,
-               '-dist', self.xvg_path,
-               '-o', self.xpm_path,
-               '-s', self.stage_io_dict["in"]["input_structure_path"],
-               '-f', self.stage_io_dict["in"]["input_traj_path"],
-               '-cl', self.stage_io_dict["out"]["output_pdb_path"],
-               '-cutoff', str(self.cutoff),
-               '-method', self.method]
+        self.cmd = [self.binary_path, 'trjconv',
+                    '-f', self.stage_io_dict["in"]["input_structure_path"],
+                    '-s', self.stage_io_dict["in"]["input_top_path"],
+                    '-o', self.stage_io_dict["out"]["output_str_path"]]
+
+        if self.pbc:
+            self.cmd.append('-pbc')
+            self.cmd.append(self.pbc)
+        self.cmd.append('-center' if self.center else '-nocenter')
+        if self.ur:
+            self.cmd.append('-ur')
+            self.cmd.append(self.ur)
+        if self.fit:
+            self.cmd.append('-fit')
+            self.cmd.append(self.fit)
 
         if self.stage_io_dict["in"].get("input_index_path"):
             self.cmd.extend(['-n', self.stage_io_dict["in"]["input_index_path"]])
 
-        if self.dista:
-            self.cmd.append('-dista')
-
         # Add stdin input file
         self.cmd.append('<')
         self.cmd.append(self.stage_io_dict["in"]["stdin_file_path"])
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
-            self.io_dict['in'].get("stdin_file_path"),
-            'rmsd-clust.xpm', 
-            'rmsd-dist.xvg', 
-            'cluster.log'
+            self.io_dict['in'].get("stdin_file_path")
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
-        return self.return_code
 
-def gmx_cluster(input_structure_path: str, input_traj_path: str, output_pdb_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
-    """Execute the :class:`GMXCluster <gromacs.gmx_cluster.GMXCluster>` class and
-    execute the :meth:`launch() <gromacs.gmx_cluster.GMXCluster.launch>` method."""
-
-    return GMXCluster(input_structure_path=input_structure_path, 
-                    input_traj_path=input_traj_path, 
-                    output_pdb_path=output_pdb_path,
-                    input_index_path=input_index_path,
-                    properties=properties, **kwargs).launch()
+def gmx_trjconv_str(input_structure_path: str, input_top_path: str, output_str_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
+    """Execute the :class:`GMXTrjConvStr <gromacs.gmx_trjconv_str.GMXTrjConvStr>` class and
+    execute the :meth:`launch() <gromacs.gmx_trjconv_str.GMXTrjConvStr.launch>` method."""
+
+    return GMXTrjConvStr(input_structure_path=input_structure_path,
+                         input_top_path=input_top_path,
+                         output_str_path=output_str_path,
+                         input_index_path=input_index_path,
+                         properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
-    parser = argparse.ArgumentParser(description="Creates cluster structures from a given GROMACS compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description="Converts between GROMACS compatible structure file formats and/or extracts a selection of atoms.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
-    #Specific args of each building block
+    # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
-    required_args.add_argument('--input_structure_path', required=True, help='Path to the input structure file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
-    required_args.add_argument('--input_traj_path', required=True, help='Path to the GROMACS trajectory file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
+    required_args.add_argument('--input_structure_path', required=True, help='Path to the input structure file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
+    required_args.add_argument('--input_top_path', required=True, help='Path to the GROMACS input topology file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
     parser.add_argument('--input_index_path', required=False, help="Path to the GROMACS index file. Accepted formats: ndx.")
-    required_args.add_argument('--output_pdb_path', required=True, help='Path to the output cluster file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
+    required_args.add_argument('--output_str_path', required=True, help='Path to the output file. Accepted formats: xtc, trr, gro, g96, pdb, tng.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
-    #Specific call of each building block
-    gmx_cluster(input_structure_path=args.input_structure_path, 
-                input_traj_path=args.input_traj_path, 
-                output_pdb_path=args.output_pdb_path, 
-                input_index_path=args.input_index_path, 
-                properties=properties)
+    # Specific call of each building block
+    gmx_trjconv_str(input_structure_path=args.input_structure_path,
+                    input_top_path=args.input_top_path,
+                    output_str_path=args.output_str_path,
+                    input_index_path=args.input_index_path,
+                    properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_energy.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_energy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 
 """Module containing the GMX Energy class and the command line interface."""
 import argparse
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.gromacs.common import *
+from biobb_analysis.gromacs.common import get_binary_path, get_default_value, check_energy_path, check_out_xvg_path, get_xvg, get_terms, copy_instructions_file_to_container
 
 
 class GMXEnergy(BiobbObject):
     """
     | biobb_analysis GMXEnergy
     | Wrapper of the GROMACS energy module for extracting energy components from a given GROMACS energy file.
-    | `GROMACS energy <http://manual.gromacs.org/current/onlinehelp/gmx-energy.html>`_ extracts energy components from an energy file. The user is prompted to interactively select the desired energy terms.    
+    | `GROMACS energy <http://manual.gromacs.org/current/onlinehelp/gmx-energy.html>`_ extracts energy components from an energy file. The user is prompted to interactively select the desired energy terms.
 
     Args:
         input_energy_path (str): Path to the input EDR file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/energy.edr>`_. Accepted formats: edr (edam:format_2330).
         output_xvg_path (str): Path to the XVG output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_energy.xvg>`_. Accepted formats: xvg (edam:format_2030).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **xvg** (*str*) - ("none") XVG plot formatting. Values: xmgrace, xmgr, none.
             * **terms** (*list*) - (["Potential"]) Energy terms. Values: Angle, Proper-Dih., Improper-Dih., LJ-14, Coulomb-14, LJ-\(SR\), Coulomb-\(SR\), Coul.-recip., Position-Rest., Potential, Kinetic-En., Total-Energy, Temperature, Pressure,  Constr.-rmsd, Box-X, Box-Y,  Box-Z, Volume, Density, pV, Enthalpy, Vir-XX, Vir-XY, Vir-XZ, Vir-YX, Vir-YY, Vir-YZ, Vir-ZX, Vir-ZY, Vir-ZZ, Pres-XX, Pres-XY, Pres-XZ, Pres-YX, Pres-YY,  Pres-YZ, Pres-ZX, Pres-ZY, Pres-ZZ, #Surf*SurfTen, Box-Vel-XX, Box-Vel-YY, Box-Vel-ZZ, Mu-X, Mu-Y, Mu-Z, T-Protein, T-non-Protein, Lamb-Protein, Lamb-non-Protein.
@@ -26,50 +27,50 @@
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('gromacs/gromacs:2022.2') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
-    
+
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.gromacs.gmx_energy import gmx_energy
-            prop = { 
-                'xvg': 'xmgr', 
-                'terms': ['Potential', 'Pressure'] 
+            prop = {
+                'xvg': 'xmgr',
+                'terms': ['Potential', 'Pressure']
             }
-            gmx_energy(input_energy_path='/path/to/myEnergyFile.edr', 
-                        output_xvg_path='/path/to/newXVG.xvg', 
+            gmx_energy(input_energy_path='/path/to/myEnergyFile.edr',
+                        output_xvg_path='/path/to/newXVG.xvg',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: GROMACS energy
             * version: >=2019.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_energy_path, output_xvg_path,
-                properties=None, **kwargs) -> None:
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_energy_path": input_energy_path }, 
-            "out": { "output_xvg_path": output_xvg_path } 
+        self.io_dict = {
+            "in": {"input_energy_path": input_energy_path},
+            "out": {"output_xvg_path": output_xvg_path}
         }
 
         # Properties specific for BB
         self.xvg = properties.get('xvg', "none")
         self.terms = properties.get('terms', ["Potential"])
         self.instructions_file = get_default_value('instructions_file')
         self.properties = properties
@@ -92,15 +93,15 @@
         """Creates an input file using the properties file settings"""
         instructions_list = []
         # different path if container execution or not
         if self.container_path:
             self.instructions_file = str(PurePath(self.container_volume_path).joinpath(self.instructions_file))
         else:
             self.instructions_file = str(PurePath(fu.create_unique_dir()).joinpath(self.instructions_file))
-        #self.instructions_file = str(PurePath(fu.create_unique_dir()).joinpath(self.instructions_file))
+        # self.instructions_file = str(PurePath(fu.create_unique_dir()).joinpath(self.instructions_file))
         fu.create_name(prefix=self.prefix, step=self.step, name=self.instructions_file)
 
         for t in self.terms:
             instructions_list.append(t)
 
         # create instructions file
         with open(self.instructions_file, 'w') as mdp:
@@ -113,29 +114,30 @@
     def launch(self) -> int:
         """Execute the :class:`GMXEnergy <gromacs.gmx_energy.GMXEnergy>` gromacs.gmx_energy.GMXEnergy object."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create instructions file
         self.create_instructions_file()
 
         # if container execution, copy intructions file to container
         if self.container_path:
             copy_instructions_file_to_container(self.instructions_file, self.stage_io_dict.get("unique_dir"))
 
         self.cmd = [self.binary_path, 'energy',
-               '-f', self.stage_io_dict["in"]["input_energy_path"],
-               '-o', self.stage_io_dict["out"]["output_xvg_path"],
-               '-xvg', self.xvg,
-               '<', self.instructions_file]
+                    '-f', self.stage_io_dict["in"]["input_energy_path"],
+                    '-o', self.stage_io_dict["out"]["output_xvg_path"],
+                    '-xvg', self.xvg,
+                    '<', self.instructions_file]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -145,36 +147,39 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def gmx_energy(input_energy_path: str, output_xvg_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`GMXEnergy <gromacs.gmx_energy.GMXEnergy>` class and
     execute the :meth:`launch() <gromacs.gmx_energy.GMXEnergy.launch>` method."""
 
-    return GMXEnergy(input_energy_path=input_energy_path, 
-                    output_xvg_path=output_xvg_path,
-                    properties=properties, **kwargs).launch()
+    return GMXEnergy(input_energy_path=input_energy_path,
+                     output_xvg_path=output_xvg_path,
+                     properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Extracts energy components from a given GROMACS energy file.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
-    #Specific args of each building block
+    # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_energy_path', required=True, help='Path to the input EDR file. Accepted formats: edr.')
     required_args.add_argument('--output_xvg_path', required=True, help='Path to the XVG output file. Accepted formats: xvg.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
-    #Specific call of each building block
-    gmx_energy(input_energy_path=args.input_energy_path, 
-                output_xvg_path=args.output_xvg_path, 
-                properties=properties)
+    # Specific call of each building block
+    gmx_energy(input_energy_path=args.input_energy_path,
+               output_xvg_path=args.output_xvg_path,
+               properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_image.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 """Module containing the GMX TrjConvStr class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
+from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.gromacs.common import *
+from biobb_analysis.gromacs.common import get_binary_path, check_input_path, check_traj_path, check_index_path, get_image_selection, get_selection_index_file, check_out_traj_path, get_pbc, get_center, get_ur, get_fit
 
 
 class GMXImage(BiobbObject):
     """
     | biobb_analysis GMXImage
     | Wrapper of the GROMACS trjconv module for correcting periodicity (image) from a given GROMACS compatible trajectory file.
     | GROMACS trjconv module can convert trajectory files in many ways. See the `GROMACS trjconv <http://manual.gromacs.org/documentation/2018/onlinehelp/gmx-trjconv.html>`_ official documentation for further information.
@@ -38,49 +39,49 @@
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_analysis.gromacs.gmx_image import gmx_image
-            prop = { 
-                'fit_selection': 'System', 
-                'center_selection': 'Water_and_ions', 
-                'output_selection': 'System', 
-                'pbc': 'mol' 
+            prop = {
+                'fit_selection': 'System',
+                'center_selection': 'Water_and_ions',
+                'output_selection': 'System',
+                'pbc': 'mol'
             }
-            gmx_image(input_traj_path='/path/to/myTrajectory.trr', 
-                        input_top_path='/path/to/myTopology.tpr', 
-                        output_traj_path='/path/to/newTrajectory.xtc', 
-                        input_index_path='/path/to/myIndex.ndx', 
+            gmx_image(input_traj_path='/path/to/myTrajectory.trr',
+                        input_top_path='/path/to/myTopology.tpr',
+                        output_traj_path='/path/to/newTrajectory.xtc',
+                        input_index_path='/path/to/myIndex.ndx',
                         properties=prop)
 
     Info:
         * wrapped_software:
             * name: GROMACS trjconv
             * version: >=2019.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_traj_path, input_top_path,  output_traj_path, 
-                input_index_path=None, properties=None, **kwargs) -> None:
+    def __init__(self, input_traj_path, input_top_path, output_traj_path,
+                 input_index_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_traj_path": input_traj_path, "input_top_path": input_top_path, "input_index_path": input_index_path }, 
-            "out": { "output_traj_path": output_traj_path } 
+        self.io_dict = {
+            "in": {"input_traj_path": input_traj_path, "input_top_path": input_top_path, "input_index_path": input_index_path},
+            "out": {"output_traj_path": output_traj_path}
         }
 
         # Properties specific for BB
         self.fit_selection = properties.get('fit_selection', "System")
         self.center_selection = properties.get('center_selection', "System")
         self.cluster_selection = properties.get('cluster_selection', "System")
         self.output_selection = properties.get('output_selection', "System")
@@ -100,22 +101,26 @@
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_index_path"] = check_index_path(self.io_dict["in"]["input_index_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_traj_path"] = check_out_traj_path(self.io_dict["out"]["output_traj_path"], out_log, self.__class__.__name__)
         if not self.io_dict["in"]["input_index_path"]:
-            if self.fit != 'none': self.fit_selection = get_image_selection(self.properties, 'fit_selection', out_log, self.__class__.__name__)
-            if self.fit != 'none' or not self.center: self.center_selection = get_image_selection(self.properties, 'center_selection', out_log, self.__class__.__name__)
-            if self.pbc == 'cluster': self.cluster_selection = get_image_selection(self.properties, 'cluster_selection', out_log, self.__class__.__name__)
+            if self.fit != 'none':
+                self.fit_selection = get_image_selection(self.properties, 'fit_selection', out_log, self.__class__.__name__)
+            if self.fit != 'none' or not self.center:
+                self.center_selection = get_image_selection(self.properties, 'center_selection', out_log, self.__class__.__name__)
+            if self.pbc == 'cluster':
+                self.cluster_selection = get_image_selection(self.properties, 'cluster_selection', out_log, self.__class__.__name__)
             self.output_selection = get_image_selection(self.properties, 'output_selection', out_log, self.__class__.__name__)
         else:
             self.fit_selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'fit_selection', out_log, self.__class__.__name__)
             self.center_selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'center_selection', out_log, self.__class__.__name__)
-            if self.pbc == 'cluster': self.cluster_selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'cluster_selection', out_log, self.__class__.__name__)
+            if self.pbc == 'cluster':
+                self.cluster_selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'cluster_selection', out_log, self.__class__.__name__)
             self.output_selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'output_selection', out_log, self.__class__.__name__)
         self.pbc = get_pbc(self.properties, out_log, self.__class__.__name__)
         self.center = get_center(self.properties, out_log, self.__class__.__name__)
         self.ur = get_ur(self.properties, out_log, self.__class__.__name__)
         self.fit = get_fit(self.properties, out_log, self.__class__.__name__)
 
     @launchlogger
@@ -130,36 +135,36 @@
                 selections = self.cluster_selection + ' ' + self.output_selection
             else:
                 selections = self.output_selection
         else:
             if self.center:
                 selections = self.fit_selection + ' ' + self.center_selection + ' ' + self.output_selection
             else:
-                selections = self.fit_selection + ' ' + self.output_selection 
+                selections = self.fit_selection + ' ' + self.output_selection
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): 
+        if self.check_restart():
             return 0
 
         # standard input
         self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{selections}')
         self.stage_files()
 
         self.cmd = [self.binary_path, 'trjconv',
-               '-f', self.stage_io_dict["in"]["input_traj_path"],
-               '-s', self.stage_io_dict["in"]["input_top_path"],
-               '-fit', self.fit,
-               '-o', self.stage_io_dict["out"]["output_traj_path"]]
+                    '-f', self.stage_io_dict["in"]["input_traj_path"],
+                    '-s', self.stage_io_dict["in"]["input_top_path"],
+                    '-fit', self.fit,
+                    '-o', self.stage_io_dict["out"]["output_traj_path"]]
 
         if self.stage_io_dict["in"].get("input_index_path"):
             self.cmd.extend(['-n', self.stage_io_dict["in"]["input_index_path"]])
-            
+
         self.cmd.append('-center' if self.center else '-nocenter')
 
         # Unit-cell representation, PBC treatment is incompatible with fitting
         if self.fit == 'none':
             self.cmd.append('-pbc')
             self.cmd.append(self.pbc)
             self.cmd.append('-ur')
@@ -181,42 +186,45 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def gmx_image(input_traj_path: str, input_top_path: str, output_traj_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`GMXImage <gromacs.gmx_image.GMXImage>` class and
     execute the :meth:`launch() <gromacs.gmx_image.GMXImage.launch>` method."""
 
-    return GMXImage(input_traj_path=input_traj_path, 
-                    input_top_path = input_top_path,
+    return GMXImage(input_traj_path=input_traj_path,
+                    input_top_path=input_top_path,
                     output_traj_path=output_traj_path,
                     input_index_path=input_index_path,
                     properties=properties, **kwargs).launch()
 
+
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Corrects periodicity (image) from a given GROMACS compatible trajectory file.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
-    #Specific args of each building block
+    # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_traj_path', required=True, help='Path to the GROMACS trajectory file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
     required_args.add_argument('--input_top_path', required=True, help='Path to the GROMACS input topology file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
     parser.add_argument('--input_index_path', required=False, help="Path to the GROMACS index file. Accepted formats: ndx.")
     required_args.add_argument('--output_traj_path', required=True, help='Path to the output file. Accepted formats: xtc, trr, gro, g96, pdb, tng.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
-    #Specific call of each building block
-    gmx_image(input_traj_path=args.input_traj_path, 
-            input_top_path=args.input_top_path, 
-            output_traj_path=args.output_traj_path, 
-            input_index_path=args.input_index_path, 
-            properties=properties)
+    # Specific call of each building block
+    gmx_image(input_traj_path=args.input_traj_path,
+              input_top_path=args.input_top_path,
+              output_traj_path=args.output_traj_path,
+              input_index_path=args.input_index_path,
+              properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_rgyr.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 #!/usr/bin/env python3
 
-"""Module containing the GMX Rgyr class and the command line interface."""
+"""Module containing the GMX Rms class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
+from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.gromacs.common import *
+from biobb_analysis.gromacs.common import get_binary_path, check_input_path, check_traj_path, check_index_path, get_selection_index_file, check_out_xvg_path, get_xvg, get_selection
 
 
-class GMXRgyr(BiobbObject):
+class GMXRms(BiobbObject):
     """
-    | biobb_analysis GMXRgyr
-    | Wrapper of the GROMACS gyrate module for computing the radius of gyration (Rgyr) of a molecule about the x-, y- and z-axes, as a function of time, from a given GROMACS compatible trajectory.
-    | `GROMACS gyrate <http://manual.gromacs.org/documentation/2018/onlinehelp/gmx-gyrate.html>`_ computes the radius of gyration of a molecule and the radii of gyration about the x-, y- and z-axes, as a function of time. The atoms are explicitly mass weighted.
+    | biobb_analysis GMXRms
+    | Wrapper of the GROMACS rms module for performing a Root Mean Square deviation (RMSd) analysis from a given GROMACS compatible trajectory.
+    | `GROMACS rms <http://manual.gromacs.org/current/onlinehelp/gmx-rms.html>`_ compares two structures by computing the root mean square deviation (RMSD), the size-independent rho similarity parameter (rho) or the scaled rho (rhosc).
 
     Args:
         input_structure_path (str): Path to the input structure file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/topology.tpr>`_. Accepted formats: tpr (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), brk (edam:format_2033), ent (edam:format_1476).
         input_traj_path (str): Path to the GROMACS trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/trajectory.trr>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
         input_index_path (str) (Optional): Path to the GROMACS index file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/index.ndx>`_. Accepted formats: ndx (edam:format_2033).
-        output_xvg_path (str): Path to the XVG output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_rgyr.xvg>`_. Accepted formats: xvg (edam:format_2030).
+        output_xvg_path (str): Path to the XVG output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_rms.xvg>`_. Accepted formats: xvg (edam:format_2030).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **xvg** (*str*) - ("none") XVG plot formatting. Values: xmgrace, xmgr, none.
-            * **selection** (*str*) - ("System") Group where the rgyr will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups), DNA (all DNA atoms), RNA (all RNA atoms), Protein_DNA (all Protein-DNA complex atoms), Protein_RNA (all Protein-RNA complex atoms), Protein_DNA_RNA (all Protein-DNA-RNA complex atoms), DNA_RNA (all DNA-RNA complex atoms).
+            * **selection** (*str*) - ("System") Group where the rms will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups), DNA (all DNA atoms), RNA (all RNA atoms), Protein_DNA (all Protein-DNA complex atoms), Protein_RNA (all Protein-RNA complex atoms), Protein_DNA_RNA (all Protein-DNA-RNA complex atoms), DNA_RNA (all DNA-RNA complex atoms).
             * **binary_path** (*str*) - ("gmx") Path to the GROMACS executable binary.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('gromacs/gromacs:2022.2') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_analysis.gromacs.gmx_rgyr import gmx_rgyr
-            prop = { 
-                'xvg': 'xmgr', 
-                'selection': 'Water_and_ions' 
+            from biobb_analysis.gromacs.gmx_rms import gmx_rms
+            prop = {
+                'xvg': 'xmgr',
+                'selection': 'Water_and_ions'
             }
-            gmx_rgyr(input_structure_path='/path/to/myStructure.tpr', 
-                    input_traj_path='/path/to/myTrajectory.trr', 
-                    output_xvg_path='/path/to/newXVG.xvg', 
-                    input_index_path='/path/to/myIndex.ndx', 
+            gmx_rms(input_structure_path='/path/to/myStructure.tpr',
+                    input_traj_path='/path/to/myTrajectory.trr',
+                    output_xvg_path='/path/to/newXVG.xvg',
+                    input_index_path='/path/to/myIndex.ndx',
                     properties=prop)
 
     Info:
         * wrapped_software:
-            * name: GROMACS gyrate
+            * name: GROMACS rms
             * version: >=2019.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_structure_path, input_traj_path, output_xvg_path, 
-                input_index_path=None, properties=None, **kwargs) -> None:
+    def __init__(self, input_structure_path, input_traj_path, output_xvg_path,
+                 input_index_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_structure_path": input_structure_path, "input_traj_path": input_traj_path, "input_index_path": input_index_path }, 
-            "out": { "output_xvg_path": output_xvg_path } 
+        self.io_dict = {
+            "in": {"input_structure_path": input_structure_path, "input_traj_path": input_traj_path, "input_index_path": input_index_path},
+            "out": {"output_xvg_path": output_xvg_path}
         }
 
         # Properties specific for BB
         self.xvg = properties.get('xvg', "none")
         self.selection = properties.get('selection', "System")
         self.properties = properties
 
@@ -93,32 +94,32 @@
         if not self.io_dict["in"]["input_index_path"]:
             self.selection = get_selection(self.properties, out_log, self.__class__.__name__)
         else:
             self.selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'selection', out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self) -> int:
-        """Execute the :class:`GMXRgyr <gromacs.gmx_rgyr.GMXRgyr>` gromacs.gmx_rgyr.GMXRgyr object."""
+        """Execute the :class:`GMXRms <gromacs.gmx_rms.GMXRms>` gromacs.gmx_rms.GMXRms object."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): 
+        if self.check_restart():
             return 0
-        
+
         # standard input
-        self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.selection}')
+        self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.selection} {self.selection}')
         self.stage_files()
 
-        self.cmd = [self.binary_path, 'gyrate',
-               '-s', self.stage_io_dict["in"]["input_structure_path"],
-               '-f', self.stage_io_dict["in"]["input_traj_path"],
-               '-o', self.stage_io_dict["out"]["output_xvg_path"],
-               '-xvg', self.xvg]
+        self.cmd = [self.binary_path, 'rms',
+                    '-s', self.stage_io_dict["in"]["input_structure_path"],
+                    '-f', self.stage_io_dict["in"]["input_traj_path"],
+                    '-o', self.stage_io_dict["out"]["output_xvg_path"],
+                    '-xvg', self.xvg]
 
         if self.stage_io_dict["in"].get("input_index_path"):
             self.cmd.extend(['-n', self.stage_io_dict["in"]["input_index_path"]])
 
         # Add stdin input file
         self.cmd.append('<')
         self.cmd.append(self.stage_io_dict["in"]["stdin_file_path"])
@@ -135,42 +136,45 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def gmx_rgyr(input_structure_path: str, input_traj_path: str, output_xvg_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
-    """Execute the :class:`GMXRgyr <gromacs.gmx_rgyr.GMXRgyr>` class and
-    execute the :meth:`launch() <gromacs.gmx_rgyr.GMXRgyr.launch>` method."""
-
-    return GMXRgyr(input_structure_path=input_structure_path, 
-                    input_traj_path = input_traj_path,
-                    output_xvg_path=output_xvg_path,
-                    input_index_path=input_index_path,
-                    properties=properties, **kwargs).launch()
+
+def gmx_rms(input_structure_path: str, input_traj_path: str, output_xvg_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
+    """Execute the :class:`GMXRms <gromacs.gmx_rms.GMXRms>` class and
+    execute the :meth:`launch() <gromacs.gmx_rms.GMXRms.launch>` method."""
+
+    return GMXRms(input_structure_path=input_structure_path,
+                  input_traj_path=input_traj_path,
+                  output_xvg_path=output_xvg_path,
+                  input_index_path=input_index_path,
+                  properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
-    parser = argparse.ArgumentParser(description="Computes the radius of gyration (Rgyr) of a molecule about the x-, y- and z-axes, as a function of time, from a given GROMACS compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description="Performs a Root Mean Square deviation (RMSd) analysis from a given GROMACS compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
-    #Specific args of each building block
+    # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_structure_path', required=True, help='Path to the input structure file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
     required_args.add_argument('--input_traj_path', required=True, help='Path to the GROMACS trajectory file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
     parser.add_argument('--input_index_path', required=False, help="Path to the GROMACS index file. Accepted formats: ndx.")
     required_args.add_argument('--output_xvg_path', required=True, help='Path to the XVG output file. Accepted formats: xvg.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
-    #Specific call of each building block
-    gmx_rgyr(input_structure_path=args.input_structure_path, 
-            input_traj_path=args.input_traj_path, 
-            output_xvg_path=args.output_xvg_path, 
-            input_index_path=args.input_index_path, 
+    # Specific call of each building block
+    gmx_rms(input_structure_path=args.input_structure_path,
+            input_traj_path=args.input_traj_path,
+            output_xvg_path=args.output_xvg_path,
+            input_index_path=args.input_index_path,
             properties=properties)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_rms.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rgyr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 #!/usr/bin/env python3
 
-"""Module containing the GMX Rms class and the command line interface."""
+"""Module containing the GMX Rgyr class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
+from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.gromacs.common import *
+from biobb_analysis.gromacs.common import get_binary_path, check_input_path, check_traj_path, check_index_path, get_selection_index_file, check_out_xvg_path, get_xvg, get_selection
 
 
-class GMXRms(BiobbObject):
+class GMXRgyr(BiobbObject):
     """
-    | biobb_analysis GMXRms
-    | Wrapper of the GROMACS rms module for performing a Root Mean Square deviation (RMSd) analysis from a given GROMACS compatible trajectory.
-    | `GROMACS rms <http://manual.gromacs.org/current/onlinehelp/gmx-rms.html>`_ compares two structures by computing the root mean square deviation (RMSD), the size-independent rho similarity parameter (rho) or the scaled rho (rhosc).
+    | biobb_analysis GMXRgyr
+    | Wrapper of the GROMACS gyrate module for computing the radius of gyration (Rgyr) of a molecule about the x-, y- and z-axes, as a function of time, from a given GROMACS compatible trajectory.
+    | `GROMACS gyrate <http://manual.gromacs.org/documentation/2018/onlinehelp/gmx-gyrate.html>`_ computes the radius of gyration of a molecule and the radii of gyration about the x-, y- and z-axes, as a function of time. The atoms are explicitly mass weighted.
 
     Args:
         input_structure_path (str): Path to the input structure file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/topology.tpr>`_. Accepted formats: tpr (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), brk (edam:format_2033), ent (edam:format_1476).
         input_traj_path (str): Path to the GROMACS trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/trajectory.trr>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
         input_index_path (str) (Optional): Path to the GROMACS index file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/index.ndx>`_. Accepted formats: ndx (edam:format_2033).
-        output_xvg_path (str): Path to the XVG output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_rms.xvg>`_. Accepted formats: xvg (edam:format_2030).
+        output_xvg_path (str): Path to the XVG output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_rgyr.xvg>`_. Accepted formats: xvg (edam:format_2030).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **xvg** (*str*) - ("none") XVG plot formatting. Values: xmgrace, xmgr, none.
-            * **selection** (*str*) - ("System") Group where the rms will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups), DNA (all DNA atoms), RNA (all RNA atoms), Protein_DNA (all Protein-DNA complex atoms), Protein_RNA (all Protein-RNA complex atoms), Protein_DNA_RNA (all Protein-DNA-RNA complex atoms), DNA_RNA (all DNA-RNA complex atoms).
+            * **selection** (*str*) - ("System") Group where the rgyr will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups), DNA (all DNA atoms), RNA (all RNA atoms), Protein_DNA (all Protein-DNA complex atoms), Protein_RNA (all Protein-RNA complex atoms), Protein_DNA_RNA (all Protein-DNA-RNA complex atoms), DNA_RNA (all DNA-RNA complex atoms).
             * **binary_path** (*str*) - ("gmx") Path to the GROMACS executable binary.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('gromacs/gromacs:2022.2') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_analysis.gromacs.gmx_rms import gmx_rms
-            prop = { 
-                'xvg': 'xmgr', 
-                'selection': 'Water_and_ions' 
+            from biobb_analysis.gromacs.gmx_rgyr import gmx_rgyr
+            prop = {
+                'xvg': 'xmgr',
+                'selection': 'Water_and_ions'
             }
-            gmx_rms(input_structure_path='/path/to/myStructure.tpr', 
-                    input_traj_path='/path/to/myTrajectory.trr', 
-                    output_xvg_path='/path/to/newXVG.xvg', 
-                    input_index_path='/path/to/myIndex.ndx', 
+            gmx_rgyr(input_structure_path='/path/to/myStructure.tpr',
+                    input_traj_path='/path/to/myTrajectory.trr',
+                    output_xvg_path='/path/to/newXVG.xvg',
+                    input_index_path='/path/to/myIndex.ndx',
                     properties=prop)
 
     Info:
         * wrapped_software:
-            * name: GROMACS rms
+            * name: GROMACS gyrate
             * version: >=2019.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
-            
+
     """
 
-    def __init__(self, input_structure_path, input_traj_path,  output_xvg_path, 
-                input_index_path=None, properties=None, **kwargs) -> None:
+    def __init__(self, input_structure_path, input_traj_path, output_xvg_path,
+                 input_index_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_structure_path": input_structure_path, "input_traj_path": input_traj_path, "input_index_path": input_index_path }, 
-            "out": { "output_xvg_path": output_xvg_path } 
+        self.io_dict = {
+            "in": {"input_structure_path": input_structure_path, "input_traj_path": input_traj_path, "input_index_path": input_index_path},
+            "out": {"output_xvg_path": output_xvg_path}
         }
 
         # Properties specific for BB
         self.xvg = properties.get('xvg', "none")
         self.selection = properties.get('selection', "System")
         self.properties = properties
 
@@ -93,85 +94,87 @@
         if not self.io_dict["in"]["input_index_path"]:
             self.selection = get_selection(self.properties, out_log, self.__class__.__name__)
         else:
             self.selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'selection', out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self) -> int:
-        """Execute the :class:`GMXRms <gromacs.gmx_rms.GMXRms>` gromacs.gmx_rms.GMXRms object."""
+        """Execute the :class:`GMXRgyr <gromacs.gmx_rgyr.GMXRgyr>` gromacs.gmx_rgyr.GMXRgyr object."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
         if self.check_restart():
             return 0
 
         # standard input
-        self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.selection} {self.selection}')
+        self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.selection}')
         self.stage_files()
 
-        self.cmd = [self.binary_path, 'rms',
-               '-s', self.stage_io_dict["in"]["input_structure_path"],
-               '-f', self.stage_io_dict["in"]["input_traj_path"],
-               '-o', self.stage_io_dict["out"]["output_xvg_path"],
-               '-xvg', self.xvg]
+        self.cmd = [self.binary_path, 'gyrate',
+                    '-s', self.stage_io_dict["in"]["input_structure_path"],
+                    '-f', self.stage_io_dict["in"]["input_traj_path"],
+                    '-o', self.stage_io_dict["out"]["output_xvg_path"],
+                    '-xvg', self.xvg]
 
         if self.stage_io_dict["in"].get("input_index_path"):
             self.cmd.extend(['-n', self.stage_io_dict["in"]["input_index_path"]])
 
         # Add stdin input file
         self.cmd.append('<')
         self.cmd.append(self.stage_io_dict["in"]["stdin_file_path"])
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
-       
+
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             self.io_dict['in'].get("stdin_file_path")
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def gmx_rms(input_structure_path: str, input_traj_path: str, output_xvg_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
-    """Execute the :class:`GMXRms <gromacs.gmx_rms.GMXRms>` class and
-    execute the :meth:`launch() <gromacs.gmx_rms.GMXRms.launch>` method."""
-
-    return GMXRms(input_structure_path=input_structure_path, 
-                    input_traj_path = input_traj_path,
-                    output_xvg_path=output_xvg_path,
-                    input_index_path=input_index_path,
-                    properties=properties, **kwargs).launch()
+
+def gmx_rgyr(input_structure_path: str, input_traj_path: str, output_xvg_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
+    """Execute the :class:`GMXRgyr <gromacs.gmx_rgyr.GMXRgyr>` class and
+    execute the :meth:`launch() <gromacs.gmx_rgyr.GMXRgyr.launch>` method."""
+
+    return GMXRgyr(input_structure_path=input_structure_path,
+                   input_traj_path=input_traj_path,
+                   output_xvg_path=output_xvg_path,
+                   input_index_path=input_index_path,
+                   properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
-    parser = argparse.ArgumentParser(description="Performs a Root Mean Square deviation (RMSd) analysis from a given GROMACS compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description="Computes the radius of gyration (Rgyr) of a molecule about the x-, y- and z-axes, as a function of time, from a given GROMACS compatible trajectory.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
-    #Specific args of each building block
+    # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_structure_path', required=True, help='Path to the input structure file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
     required_args.add_argument('--input_traj_path', required=True, help='Path to the GROMACS trajectory file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
     parser.add_argument('--input_index_path', required=False, help="Path to the GROMACS index file. Accepted formats: ndx.")
     required_args.add_argument('--output_xvg_path', required=True, help='Path to the XVG output file. Accepted formats: xvg.')
 
-
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
-    #Specific call of each building block
-    gmx_rms(input_structure_path=args.input_structure_path, 
-            input_traj_path=args.input_traj_path, 
-            output_xvg_path=args.output_xvg_path, 
-            input_index_path=args.input_index_path, 
-            properties=properties)
+    # Specific call of each building block
+    gmx_rgyr(input_structure_path=args.input_structure_path,
+             input_traj_path=args.input_traj_path,
+             output_xvg_path=args.output_xvg_path,
+             input_index_path=args.input_index_path,
+             properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_trjconv_str.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str_ens.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,190 +1,222 @@
 #!/usr/bin/env python3
 
-# AFEGIR PARÀMETRES DE GMX_IMAGE: PBC, CENTER, UR, FIT (NOMÉS APPEND SI L'USUARI ELS AFEGEIX)
-
 """Module containing the GMX TrjConvStr class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
+from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.gromacs.common import *
+from biobb_analysis.gromacs.common import get_binary_path, check_input_path, check_traj_path, check_index_path, get_selection_index_file, get_selection, check_out_str_ens_path, get_skip, get_start, get_end, get_dt, get_ot_str_ens, process_output_trjconv_str_ens
 
 
-class GMXTrjConvStr(BiobbObject):
+class GMXTrjConvStrEns(BiobbObject):
     """
-    | biobb_analysis GMXTrjConvStr
-    | Wrapper of the GROMACS trjconv module for converting between GROMACS compatible structure file formats and/or extracting a selection of atoms.
+    | biobb_analysis GMXTrjConvStrEns
+    | Wrapper of the GROMACS trjconv module for extracting an ensemble of frames containing a selection of atoms from GROMACS compatible trajectory files.
     | GROMACS trjconv module can convert trajectory files in many ways. See the `GROMACS trjconv <http://manual.gromacs.org/documentation/2018/onlinehelp/gmx-trjconv.html>`_ official documentation for further information.
 
     Args:
-        input_structure_path (str): Path to the input structure file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/trajectory.trr>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
+        input_traj_path (str): Path to the GROMACS trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/trajectory.trr>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
         input_top_path (str): Path to the GROMACS input topology file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/topology.tpr>`_. Accepted formats: tpr (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), brk (edam:format_2033), ent (edam:format_1476).
         input_index_path (str) (Optional): Path to the GROMACS index file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/index.ndx>`_. Accepted formats: ndx (edam:format_2033).
-        output_str_path (str): Path to the output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_trjconv.str.pdb>`_. Accepted formats: pdb (edam:format_1476), xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), tng (edam:format_3876).
+        output_str_ens_path (str): Path to the output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_trjconv.str.ens.zip>`_. Accepted formats: zip (edam:format_3987).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **selection** (*str*) - ("System") Group where the trjconv will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups), DNA (all DNA atoms), RNA (all RNA atoms), Protein_DNA (all Protein-DNA complex atoms), Protein_RNA (all Protein-RNA complex atoms), Protein_DNA_RNA (all Protein-DNA-RNA complex atoms), DNA_RNA (all DNA-RNA complex atoms).
-            * **pbc** (*str*) - ("mol") PBC treatment (see help text for full description). Values: none (No PBC treatment), mol (Puts the center of mass of molecules in the box), res (Puts the center of mass of residues in the box), atom (Puts all the atoms in the box), nojump (Checks if atoms jump across the box and then puts them back), cluster (Clusters all the atoms in the selected index such that they are all closest to the center of mass of the cluster which is iteratively updated), whole (Only makes broken molecules whole).
-            * **center** (*bool*) - (True) Center atoms in box.
-            * **ur** (*str*) - ("compact") Unit-cell representation. Values: rect (It's the ordinary brick shape), tric (It's the triclinic unit cell), compact (Puts all atoms at the closest distance from the center of the box).
-            * **fit** (*str*) - ("none") Fit molecule to ref structure in the structure file. Values: none, rot+trans, rotxy+transxy, translation, transxy, progressive.
+            * **skip** (*int*) - (1) [0~10000|1] Only write every nr-th frame.
+            * **start** (*int*) - (0) [0~10000|1] Time of first frame to read from trajectory (default unit ps).
+            * **end** (*int*) - (0) [0~10000|1] Time of last frame to read from trajectory (default unit ps).
+            * **dt** (*int*) - (0) [0~10000|1] Only write frame when t MOD dt = first time (ps).
+            * **output_name** (*str*) - ("output") File name for ensemble of output files.
+            * **output_type** (*str*) - ("pdb") File type for ensemble of output files. Values: gro (Contains a molecular structure in Gromos87 format), g96 (Can be a GROMOS-96 initial/final configuration file or a coordinate trajectory file or a combination of both), pdb (Molecular structure files in the protein databank file format).
             * **binary_path** (*str*) - ("gmx") Path to the GROMACS executable binary.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('gromacs/gromacs:2022.2') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_analysis.gromacs.gmx_trjconv_str import gmx_trjconv_str
-            prop = { 
-                'selection': 'System' 
+            from biobb_analysis.gromacs.gmx_trjconv_str_ens import gmx_trjconv_str_ens
+            prop = {
+                'selection': 'System',
+                'start': 0,
+                'end': 10,
+                'dt': 1
             }
-            gmx_trjconv_str(input_structure_path='/path/to/myStructure.trr', 
-                            input_top_path='/path/to/myTopology.tpr', 
-                            output_str_path='/path/to/newStructure.pdb', 
-                            input_index_path='/path/to/myIndex.ndx', 
-                            properties=prop)
+            gmx_trjconv_str_ens(input_traj_path='/path/to/myStructure.trr',
+                                input_top_path='/path/to/myTopology.tpr',
+                                output_str_ens_path='/path/to/newStructureEnsemble.zip',
+                                input_index_path='/path/to/myIndex.ndx',
+                                properties=prop)
 
     Info:
         * wrapped_software:
             * name: GROMACS trjconv
             * version: >=2019.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_structure_path, input_top_path, output_str_path, 
-                input_index_path=None, properties=None, **kwargs) -> None:
+    def __init__(self, input_traj_path, input_top_path, output_str_ens_path,
+                 input_index_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_structure_path": input_structure_path, "input_top_path": input_top_path, "input_index_path": input_index_path }, 
-            "out": { "output_str_path": output_str_path } 
+        self.io_dict = {
+            "in": {"input_traj_path": input_traj_path, "input_top_path": input_top_path, "input_index_path": input_index_path},
+            "out": {"output_str_ens_path": output_str_ens_path}
         }
 
         # Properties specific for BB
         self.selection = properties.get('selection', "System")
-        self.pbc = properties.get('pbc', None)
-        self.center = properties.get('dista', None)
-        self.ur = properties.get('ur', None)
-        self.fit = properties.get('fit', None)
+        self.skip = properties.get('skip', 1)
+        self.start = properties.get('start', 0)
+        self.end = properties.get('end', 0)
+        self.dt = properties.get('dt', 0)
+        self.output_name = properties.get('output_name', "output")
+        self.output_type = properties.get('output_type', "pdb")
         self.properties = properties
 
         # Properties common in all GROMACS BB
         self.binary_path = get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
-        self.io_dict["in"]["input_structure_path"] = check_traj_path(self.io_dict["in"]["input_structure_path"], out_log, self.__class__.__name__)
+        self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
         self.io_dict["in"]["input_index_path"] = check_index_path(self.io_dict["in"]["input_index_path"], out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_str_path"] = check_out_traj_path(self.io_dict["out"]["output_str_path"], out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_str_ens_path"] = check_out_str_ens_path(self.io_dict["out"]["output_str_ens_path"], out_log, self.__class__.__name__)
         if not self.io_dict["in"]["input_index_path"]:
             self.selection = get_selection(self.properties, out_log, self.__class__.__name__)
         else:
             self.selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'selection', out_log, self.__class__.__name__)
+        self.skip = get_skip(self.properties, out_log, self.__class__.__name__)
+        self.start = get_start(self.properties, out_log, self.__class__.__name__)
+        self.end = get_end(self.properties, out_log, self.__class__.__name__)
+        self.dt = get_dt(self.properties, out_log, self.__class__.__name__)
+        self.output_name = self.properties.get('output_name', 'output')
+        self.output_type = get_ot_str_ens(self.properties, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self) -> int:
-        """Execute the :class:`GMXTrjConvStr <gromacs.gmx_trjconv_str.GMXTrjConvStr>` gromacs.gmx_trjconv_str.GMXTrjConvStr object."""
+        """Execute the :class:`GMXTrjConvStrEns <gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns>` gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns object."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
         if self.check_restart():
             return 0
 
         # standard input
         self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.selection}')
         self.stage_files()
 
+        # if container execution, output to container_volume_path, else to unique_dir
+        if self.container_path:
+            output = self.container_volume_path + '/' + self.output_name + '.' + self.output_type
+        else:
+            output = self.stage_io_dict.get("unique_dir") + '/' + self.output_name + '.' + self.output_type
+
         self.cmd = [self.binary_path, 'trjconv',
-               '-f', self.stage_io_dict["in"]["input_structure_path"],
-               '-s', self.stage_io_dict["in"]["input_top_path"],
-               '-o', self.stage_io_dict["out"]["output_str_path"]]
-
-        if self.pbc:  
-            self.cmd.append('-pbc')
-            self.cmd.append(self.pbc)
-        self.cmd.append('-center' if self.center else '-nocenter')
-        if self.ur:  
-            self.cmd.append('-ur')
-            self.cmd.append(self.ur)
-        if self.fit: 
-            self.cmd.append('-fit')
-            self.cmd.append(self.fit)
+                    '-f', self.stage_io_dict["in"]["input_traj_path"],
+                    '-s', self.stage_io_dict["in"]["input_top_path"],
+                    '-skip', self.skip,
+                    '-b', self.start,
+                    '-dt', self.dt,
+                    '-sep',
+                    '-o', output]
+
+        # checking 'end' gromacs 'bug'
+        if not str(self.end) == "0":
+            self.cmd.append('-e')
+            self.cmd.append(self.end)
 
         if self.stage_io_dict["in"].get("input_index_path"):
             self.cmd.extend(['-n', self.stage_io_dict["in"]["input_index_path"]])
 
         # Add stdin input file
         self.cmd.append('<')
         self.cmd.append(self.stage_io_dict["in"]["stdin_file_path"])
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
+        if self.container_path:
+            process_output_trjconv_str_ens(self.stage_io_dict['unique_dir'],
+                                           self.io_dict["out"]["output_str_ens_path"],
+                                           self.stage_io_dict.get("unique_dir"),
+                                           self.output_name + '*', self.out_log)
+        else:
+            process_output_trjconv_str_ens(self.stage_io_dict.get("unique_dir"),
+                                           self.stage_io_dict["out"]["output_str_ens_path"],
+                                           self.io_dict["out"]["output_str_ens_path"],
+                                           'output*.pdb', self.out_log)
+
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             self.io_dict['in'].get("stdin_file_path")
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
-def gmx_trjconv_str(input_structure_path: str, input_top_path: str, output_str_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
-    """Execute the :class:`GMXTrjConvStr <gromacs.gmx_trjconv_str.GMXTrjConvStr>` class and
-    execute the :meth:`launch() <gromacs.gmx_trjconv_str.GMXTrjConvStr.launch>` method."""
-
-    return GMXTrjConvStr(input_structure_path=input_structure_path, 
-                    input_top_path = input_top_path,
-                    output_str_path=output_str_path,
-                    input_index_path=input_index_path,
-                    properties=properties, **kwargs).launch()
+        return self.return_code
+
+
+def gmx_trjconv_str_ens(input_traj_path: str, input_top_path: str, output_str_ens_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
+    """Execute the :class:`GMXTrjConvStrEns <gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns>` class and
+    execute the :meth:`launch() <gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns.launch>` method."""
+
+    return GMXTrjConvStrEns(input_traj_path=input_traj_path,
+                            input_top_path=input_top_path,
+                            output_str_ens_path=output_str_ens_path,
+                            input_index_path=input_index_path,
+                            properties=properties).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
-    parser = argparse.ArgumentParser(description="Converts between GROMACS compatible structure file formats and/or extracts a selection of atoms.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description="Extracts an ensemble of frames containing a selection of atoms from GROMACS compatible trajectory files.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
-    #Specific args of each building block
+    # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
-    required_args.add_argument('--input_structure_path', required=True, help='Path to the input structure file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
+    required_args.add_argument('--input_traj_path', required=True, help='Path to the GROMACS trajectory file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
     required_args.add_argument('--input_top_path', required=True, help='Path to the GROMACS input topology file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
     parser.add_argument('--input_index_path', required=False, help="Path to the GROMACS index file. Accepted formats: ndx.")
-    required_args.add_argument('--output_str_path', required=True, help='Path to the output file. Accepted formats: xtc, trr, gro, g96, pdb, tng.')
+    required_args.add_argument('--output_str_ens_path', required=True, help='Path to the output file. Accepted formats: zip.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
-    #Specific call of each building block
-    gmx_trjconv_str(input_structure_path=args.input_structure_path, 
-                    input_top_path=args.input_top_path, 
-                    output_str_path=args.output_str_path, 
-                    input_index_path=args.input_index_path, 
-                    properties=properties)
+    # Specific call of each building block
+    gmx_trjconv_str_ens(input_traj_path=args.input_traj_path,
+                        input_top_path=args.input_top_path,
+                        output_str_ens_path=args.output_str_ens_path,
+                        input_index_path=args.input_index_path,
+                        properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis/gromacs/gmx_trjconv_str_ens.py` & `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_trj.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,220 +1,207 @@
 #!/usr/bin/env python3
 
 """Module containing the GMX TrjConvStr class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
-from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_analysis.gromacs.common import *
+import biobb_common.tools.file_utils as fu
+import biobb_analysis.gromacs.common as gro_common
 
 
-class GMXTrjConvStrEns(BiobbObject):
+class GMXTrjConvTrj(BiobbObject):
     """
-    | biobb_analysis GMXTrjConvStrEns
-    | Wrapper of the GROMACS trjconv module for extracting an ensemble of frames containing a selection of atoms from GROMACS compatible trajectory files.
+    | biobb_analysis GMXTrjConvTrj
+    | Wrapper of the GROMACS trjconv module for converting between GROMACS compatible trajectory file formats and/or extracts a selection of atoms.
     | GROMACS trjconv module can convert trajectory files in many ways. See the `GROMACS trjconv <http://manual.gromacs.org/documentation/2018/onlinehelp/gmx-trjconv.html>`_ official documentation for further information.
 
     Args:
         input_traj_path (str): Path to the GROMACS trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/trajectory.trr>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
-        input_top_path (str): Path to the GROMACS input topology file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/topology.tpr>`_. Accepted formats: tpr (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), brk (edam:format_2033), ent (edam:format_1476).
+        input_top_path (str) (Optional): Path to the GROMACS input topology file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/topology.tpr>`_. Accepted formats: tpr (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), brk (edam:format_2033), ent (edam:format_1476).
         input_index_path (str) (Optional): Path to the GROMACS index file. File type: input. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/data/gromacs/index.ndx>`_. Accepted formats: ndx (edam:format_2033).
-        output_str_ens_path (str): Path to the output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_trjconv.str.ens.zip>`_. Accepted formats: zip (edam:format_3987).
+        output_traj_path (str): Path to the output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_analysis/raw/master/biobb_analysis/test/reference/gromacs/ref_trjconv.trj.xtc>`_. Accepted formats: xtc (edam:format_3875), trr (edam:format_3910), cpt (edam:format_2333), gro (edam:format_2033), g96 (edam:format_2033), pdb (edam:format_1476), tng (edam:format_3876).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **selection** (*str*) - ("System") Group where the trjconv will be performed. If **input_index_path** provided, check the file for the accepted values. Values: System (all atoms in the system), Protein (all protein atoms), Protein-H (protein atoms excluding hydrogens), C-alpha (C-alpha atoms), Backbone (protein backbone atoms: N; C-alpha and C), MainChain (protein main chain atoms: N; C-alpha; C and O; including oxygens in C-terminus), MainChain+Cb (protein main chain atoms including C-beta), MainChain+H (protein main chain atoms including backbone amide hydrogens and hydrogens on the N-terminus), SideChain (protein side chain atoms: that is all atoms except N; C-alpha; C; O; backbone amide hydrogens and oxygens in C-terminus and hydrogens on the N-terminus), SideChain-H (protein side chain atoms excluding all hydrogens), Prot-Masses (protein atoms excluding dummy masses), non-Protein (all non-protein atoms), Water (water molecules), SOL (water molecules), non-Water (anything not covered by the Water group), Ion (any name matching an Ion entry in residuetypes.dat), NA (all NA atoms), CL (all CL atoms), Water_and_ions (combination of the Water and Ions groups), DNA (all DNA atoms), RNA (all RNA atoms), Protein_DNA (all Protein-DNA complex atoms), Protein_RNA (all Protein-RNA complex atoms), Protein_DNA_RNA (all Protein-DNA-RNA complex atoms), DNA_RNA (all DNA-RNA complex atoms).
-            * **skip** (*int*) - (1) [0~10000|1] Only write every nr-th frame.
             * **start** (*int*) - (0) [0~10000|1] Time of first frame to read from trajectory (default unit ps).
             * **end** (*int*) - (0) [0~10000|1] Time of last frame to read from trajectory (default unit ps).
             * **dt** (*int*) - (0) [0~10000|1] Only write frame when t MOD dt = first time (ps).
-            * **output_name** (*str*) - ("output") File name for ensemble of output files.
-            * **output_type** (*str*) - ("pdb") File type for ensemble of output files. Values: gro (Contains a molecular structure in Gromos87 format), g96 (Can be a GROMOS-96 initial/final configuration file or a coordinate trajectory file or a combination of both), pdb (Molecular structure files in the protein databank file format).
             * **binary_path** (*str*) - ("gmx") Path to the GROMACS executable binary.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('gromacs/gromacs:2022.2') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_analysis.gromacs.gmx_trjconv_str_ens import gmx_trjconv_str_ens
-            prop = { 
-                'selection': 'System', 
-                'start': 0, 
-                'end': 10, 
-                'dt': 1 
+            from biobb_analysis.gromacs.gmx_trjconv_trj import gmx_trjconv_trj
+            prop = {
+                'selection': 'System',
+                'start': 0,
+                'end': 0
             }
-            gmx_trjconv_str_ens(input_traj_path='/path/to/myStructure.trr', 
-                                input_top_path='/path/to/myTopology.tpr', 
-                                output_str_ens_path='/path/to/newStructureEnsemble.zip', 
-                                input_index_path='/path/to/myIndex.ndx', 
-                                properties=prop)
+            gmx_trjconv_trj(input_traj_path='/path/to/myStructure.trr',
+                            output_traj_path='/path/to/newTrajectory.xtc',
+                            input_index_path='/path/to/myIndex.ndx',
+                            properties=prop)
 
     Info:
         * wrapped_software:
             * name: GROMACS trjconv
             * version: >=2019.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
-            
+
     """
 
-    def __init__(self, input_traj_path, input_top_path, output_str_ens_path, 
-                input_index_path=None, properties=None, **kwargs) -> None:
+    def __init__(self, input_traj_path,
+                 output_traj_path, input_index_path=None, input_top_path=None, properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
-        self.io_dict = { 
-            "in": { "input_traj_path": input_traj_path, "input_top_path": input_top_path, "input_index_path": input_index_path }, 
-            "out": { "output_str_ens_path": output_str_ens_path } 
+        self.io_dict = {
+            "in": {"input_traj_path": input_traj_path, "input_index_path": input_index_path, "input_top_path": input_top_path},
+            "out": {"output_traj_path": output_traj_path}
         }
 
         # Properties specific for BB
-        self.selection = properties.get('selection', "System")
-        self.skip = properties.get('skip', 1)
+        if not self.io_dict["in"]["input_index_path"] and not self.io_dict["in"]["input_top_path"]:
+            self.selection = properties.get('selection', "")
+        else:
+            self.selection = properties.get('selection', "System")
         self.start = properties.get('start', 0)
         self.end = properties.get('end', 0)
         self.dt = properties.get('dt', 0)
-        self.output_name = properties.get('output_name', "output")
-        self.output_type = properties.get('output_type', "pdb")
         self.properties = properties
 
         # Properties common in all GROMACS BB
-        self.binary_path = get_binary_path(properties, 'binary_path')
+        self.binary_path = gro_common.get_binary_path(properties, 'binary_path')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
-        self.io_dict["in"]["input_traj_path"] = check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
-        self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
-        self.io_dict["in"]["input_index_path"] = check_index_path(self.io_dict["in"]["input_index_path"], out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_str_ens_path"] = check_out_str_ens_path(self.io_dict["out"]["output_str_ens_path"], out_log, self.__class__.__name__)
-        if not self.io_dict["in"]["input_index_path"]:
+        self.io_dict["in"]["input_traj_path"] = gro_common.check_traj_path(self.io_dict["in"]["input_traj_path"], out_log, self.__class__.__name__)
+        self.io_dict["in"]["input_index_path"] = gro_common.check_index_path(self.io_dict["in"]["input_index_path"], out_log, self.__class__.__name__)
+        if self.io_dict["in"]["input_top_path"]:
+            self.io_dict["in"]["input_top_path"] = gro_common.check_input_path(self.io_dict["in"]["input_top_path"], out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_traj_path"] = gro_common.check_out_traj_path(self.io_dict["out"]["output_traj_path"], out_log, self.__class__.__name__)
+        '''if not self.io_dict["in"]["input_index_path"]:
             self.selection = get_selection(self.properties, out_log, self.__class__.__name__)
         else:
-            self.selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'selection', out_log, self.__class__.__name__)
-        self.skip = get_skip(self.properties, out_log, self.__class__.__name__)
-        self.start = get_start(self.properties, out_log, self.__class__.__name__)
-        self.end = get_end(self.properties, out_log, self.__class__.__name__)
-        self.dt = get_dt(self.properties, out_log, self.__class__.__name__)
-        self.output_name = self.properties.get('output_name', 'output')
-        self.output_type = get_ot_str_ens(self.properties, out_log, self.__class__.__name__)
+            self.selection = get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'selection', out_log, self.__class__.__name__)'''
+        if self.io_dict["in"]["input_top_path"] and not self.io_dict["in"]["input_index_path"]:
+            self.selection = gro_common.get_selection(self.properties, out_log, self.__class__.__name__)
+        elif self.io_dict["in"]["input_index_path"]:
+            self.selection = gro_common.get_selection_index_file(self.properties, self.io_dict["in"]["input_index_path"], 'selection', out_log, self.__class__.__name__)
+        elif not self.io_dict["in"]["input_top_path"] and not self.io_dict["in"]["input_index_path"]:
+            self.selection = ""
+        else:
+            return True
+        self.start = gro_common.get_start(self.properties, out_log, self.__class__.__name__)
+        self.end = gro_common.get_end(self.properties, out_log, self.__class__.__name__)
+        self.dt = gro_common.get_dt(self.properties, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self) -> int:
-        """Execute the :class:`GMXTrjConvStrEns <gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns>` gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns object."""
+        """Execute the :class:`GMXTrjConvTrj <gromacs.gmx_trjconv_trj.GMXTrjConvTrj>` gromacs.gmx_trjconv_trj.GMXTrjConvTrj object."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
+        # if not input_index_path and not input_top_path provided, selection must be empty, otherwise exit
+        if not self.io_dict["in"]["input_index_path"] and not self.io_dict["in"]["input_top_path"] and self.selection != '':
+            fu.log(self.__class__.__name__ + ': If not input_index_path and not input_top_path provided, selection must be empty', self.out_log)
+            raise SystemExit(self.__class__.__name__ + ': If not input_index_path and not input_top_path provided, selection must be empty')
+
         # Setup Biobb
         if self.check_restart():
             return 0
 
         # standard input
         self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.selection}')
         self.stage_files()
 
-        # if container execution, output to container_volume_path, else to unique_dir
-        if self.container_path:
-            output = self.container_volume_path + '/' + self.output_name + '.' + self.output_type
-        else:
-            output = self.stage_io_dict.get("unique_dir") + '/' + self.output_name + '.' + self.output_type
-
         self.cmd = [self.binary_path, 'trjconv',
-               '-f', self.stage_io_dict["in"]["input_traj_path"],
-               '-s', self.stage_io_dict["in"]["input_top_path"],
-               '-skip', self.skip,
-               '-b', self.start,
-               '-dt', self.dt,
-               '-sep',
-               '-o', output]
-
-        # checking 'end' gromacs 'bug'
-        if not str(self.end) =="0":
-            self.cmd.append('-e')
-            self.cmd.append(self.end)
+                    '-f', self.stage_io_dict["in"]["input_traj_path"],
+                    '-b', self.start,
+                    '-e', self.end,
+                    '-dt', self.dt,
+                    '-o', self.stage_io_dict["out"]["output_traj_path"]]
 
-        if self.stage_io_dict["in"].get("input_index_path"):
+        if "input_index_path" in self.stage_io_dict["in"]:
             self.cmd.extend(['-n', self.stage_io_dict["in"]["input_index_path"]])
 
+        if "input_top_path" in self.stage_io_dict["in"]:
+            self.cmd.extend(['-s', self.stage_io_dict["in"]["input_top_path"]])
+
         # Add stdin input file
         self.cmd.append('<')
         self.cmd.append(self.stage_io_dict["in"]["stdin_file_path"])
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
-        if self.container_path:
-            process_output_trjconv_str_ens(self.stage_io_dict['unique_dir'], 
-                                           self.io_dict["out"]["output_str_ens_path"],
-                                           self.stage_io_dict.get("unique_dir"), 
-                                           self.output_name + '*', self.out_log)
-        else:
-            process_output_trjconv_str_ens(self.stage_io_dict.get("unique_dir"), 
-                                           self.stage_io_dict["out"]["output_str_ens_path"],
-                                           self.io_dict["out"]["output_str_ens_path"], 
-                                           'output*.pdb', self.out_log)
-
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             self.io_dict['in'].get("stdin_file_path")
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def gmx_trjconv_str_ens(input_traj_path: str, input_top_path: str, output_str_ens_path: str, input_index_path: str = None, properties: dict = None, **kwargs) -> int:
-    """Execute the :class:`GMXTrjConvStrEns <gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns>` class and
-    execute the :meth:`launch() <gromacs.gmx_trjconv_str_ens.GMXTrjConvStrEns.launch>` method."""
-
-    return GMXTrjConvStrEns(input_traj_path=input_traj_path, 
-                    input_top_path = input_top_path,
-                    output_str_ens_path=output_str_ens_path,
-                    input_index_path=input_index_path,
-                    properties=properties).launch()
+
+def gmx_trjconv_trj(input_traj_path: str, output_traj_path: str, input_index_path: str = None, input_top_path: str = None, properties: dict = None, **kwargs) -> int:
+    """Execute the :class:`GMXTrjConvTrj <gromacs.gmx_trjconv_trj.GMXTrjConvTrj>` class and
+    execute the :meth:`launch() <gromacs.gmx_trjconv_trj.GMXTrjConvTrj.launch>` method."""
+
+    return GMXTrjConvTrj(input_traj_path=input_traj_path,
+                         output_traj_path=output_traj_path,
+                         input_index_path=input_index_path,
+                         input_top_path=input_top_path,
+                         properties=properties, **kwargs).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
-    parser = argparse.ArgumentParser(description="Extracts an ensemble of frames containing a selection of atoms from GROMACS compatible trajectory files.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description="Converts between GROMACS compatible trajectory file formats and/or extracts a selection of atoms.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_traj_path', required=True, help='Path to the GROMACS trajectory file. Accepted formats: xtc, trr, cpt, gro, g96, pdb, tng.')
-    required_args.add_argument('--input_top_path', required=True, help='Path to the GROMACS input topology file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
     parser.add_argument('--input_index_path', required=False, help="Path to the GROMACS index file. Accepted formats: ndx.")
-    required_args.add_argument('--output_str_ens_path', required=True, help='Path to the output file. Accepted formats: zip.')
+    parser.add_argument('--input_top_path', required=False, help='Path to the GROMACS input topology file. Accepted formats: tpr, gro, g96, pdb, brk, ent.')
+    required_args.add_argument('--output_traj_path', required=True, help='Path to the output file. Accepted formats: xtc, trr, gro, g96, pdb, tng.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
-    gmx_trjconv_str_ens(input_traj_path=args.input_traj_path, 
-                        input_top_path=args.input_top_path, 
-                        output_str_ens_path=args.output_str_ens_path,
-                        input_index_path=args.input_index_path, 
-                        properties=properties)
+    gmx_trjconv_trj(input_traj_path=args.input_traj_path,
+                    output_traj_path=args.output_traj_path,
+                    input_index_path=args.input_index_path,
+                    input_top_path=args.input_top_path,
+                    properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis.egg-info/PKG-INFO` & `biobb_analysis-4.0.1/biobb_analysis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: biobb-analysis
-Version: 4.0.0
+Version: 4.0.1
 Summary: Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_analysis
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
 License: UNKNOWN
 Project-URL: Documentation, http://biobb_analysis.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
+[![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
-[![](https://img.shields.io/website?down_message=Offline&label=Biobb%20Website&up_message=Online&url=https%3A%2F%2Fmmb.irbbarcelona.org%2Fbiobb%2F)]()
+[![](https://img.shields.io/website?down_message=Offline&label=Biobb%20Website&up_message=Online&url=https%3A%2F%2Fmmb.irbbarcelona.org%2Fbiobb%2F)](https://mmb.irbbarcelona.org/biobb/)
 [![](https://img.shields.io/badge/Youtube-tutorial-blue?logo=youtube&logoColor=red)](https://www.youtube.com/watch?v=ou1DOGNs0xM)
 [![](https://zenodo.org/badge/DOI/10.1038/s41597-019-0177-4.svg)](https://doi.org/10.1038/s41597-019-0177-4)
 [![](https://img.shields.io/endpoint?color=brightgreen&url=https%3A%2F%2Fapi.juleskreuer.eu%2Fcitation-badge.php%3Fshield%26doi%3D10.1038%2Fs41597-019-0177-4)](https://www.nature.com/articles/s41597-019-0177-4#citeas)
 
 [![](https://docs.bioexcel.eu/biobb_analysis/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_analysis/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_analysis/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_analysis/coverage/)
 [![](https://docs.bioexcel.eu/biobb_analysis/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_analysis/flake8/)
@@ -54,76 +54,76 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.0.0"
+        pip install "biobb_analysis>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.0.0"
+        conda install -c bioconda "biobb_analysis>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.0.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.0--pyhdfd78af_0
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2022 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_analysis-4.0.0/biobb_analysis.egg-info/SOURCES.txt` & `biobb_analysis-4.0.1/biobb_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.0/biobb_analysis.egg-info/entry_points.txt` & `biobb_analysis-4.0.1/biobb_analysis.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.0/setup.py` & `biobb_analysis-4.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_analysis",
-    version="4.0.0",
+    version="4.0.1",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_analysis",
     project_urls={
         "Documentation": "http://biobb_analysis.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     install_requires=['biobb_common==4.0.0'],
-    python_requires='>=3.7,<=3.10',
+    python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "cpptraj_average = biobb_analysis.ambertools.cpptraj_average:main",
             "cpptraj_bfactor = biobb_analysis.ambertools.cpptraj_bfactor:main",
             "cpptraj_convert = biobb_analysis.ambertools.cpptraj_convert:main",
             "cpptraj_dry = biobb_analysis.ambertools.cpptraj_dry:main",
             "cpptraj_image = biobb_analysis.ambertools.cpptraj_image:main",
@@ -45,14 +45,13 @@
         ]
     },
     classifiers=(
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Operating System :: Unix"
     ),
 )
```

