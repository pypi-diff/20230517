# Comparing `tmp/prose-2.3.0.tar.gz` & `tmp/prose-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prose-2.3.0.tar", last modified: Fri Nov 18 08:12:29 2022, max compression
+gzip compressed data, was "prose-3.0.0.tar", max compression
```

## Comparing `prose-2.3.0.tar` & `prose-3.0.0.tar`

### file list

```diff
@@ -1,72 +1,37 @@
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.327376 prose-2.3.0/
--rw-r--r--   0 lgrcia     (501) staff       (20)     1097 2022-02-22 12:25:15.000000 prose-2.3.0/LICENSE
--rw-r--r--   0 lgrcia     (501) staff       (20)       62 2022-11-18 08:09:31.000000 prose-2.3.0/MANIFEST.in
--rw-r--r--   0 lgrcia     (501) staff       (20)     3878 2022-11-18 08:12:29.327149 prose-2.3.0/PKG-INFO
--rw-r--r--   0 lgrcia     (501) staff       (20)     3435 2022-11-18 08:09:31.000000 prose-2.3.0/README.md
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.302702 prose-2.3.0/latex/
--rw-r--r--   0 lgrcia     (501) staff       (20)     2753 2022-02-22 12:25:15.000000 prose-2.3.0/latex/prose-report.cls
--rw-r--r--   0 lgrcia     (501) staff       (20)      618 2022-02-22 12:25:15.000000 prose-2.3.0/latex/report.tex
--rw-r--r--   0 lgrcia     (501) staff       (20)     1688 2022-04-12 12:36:40.000000 prose-2.3.0/latex/summary.tex
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.307031 prose-2.3.0/prose/
--rw-r--r--   0 lgrcia     (501) staff       (20)      759 2022-11-18 08:11:26.000000 prose-2.3.0/prose/__init__.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.318635 prose-2.3.0/prose/archive/
--rw-r--r--   0 lgrcia     (501) staff       (20)       57 2022-07-28 14:48:00.000000 prose-2.3.0/prose/archive/__init__.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     2870 2022-07-28 14:48:00.000000 prose-2.3.0/prose/archive/pos1.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     2475 2022-07-28 14:48:00.000000 prose-2.3.0/prose/archive/sdss.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.322645 prose-2.3.0/prose/blocks/
--rw-r--r--   0 lgrcia     (501) staff       (20)     1497 2022-07-28 14:54:29.000000 prose-2.3.0/prose/blocks/__init__.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     4528 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/alignment.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     2978 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/background.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     5242 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/catalogs.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     7426 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/centroids.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     9718 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/detection.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    11217 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/photometry.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    19818 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/psf.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    14608 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/registration.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     3491 2022-07-28 14:48:00.000000 prose-2.3.0/prose/blocks/shepard.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    28619 2022-11-18 08:11:26.000000 prose-2.3.0/prose/blocks/utils.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     3780 2022-11-18 08:09:31.000000 prose-2.3.0/prose/blocks/vizualisation.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     7891 2022-07-28 14:54:29.000000 prose-2.3.0/prose/builtins.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     9570 2022-11-18 08:09:31.000000 prose-2.3.0/prose/citations.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     4978 2022-08-24 13:02:07.000000 prose-2.3.0/prose/config.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     3688 2022-07-28 14:48:00.000000 prose-2.3.0/prose/console_utils.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.323820 prose-2.3.0/prose/core/
--rw-r--r--   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:11:26.000000 prose-2.3.0/prose/core/__init__.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     3108 2022-11-18 08:11:26.000000 prose-2.3.0/prose/core/block.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    21329 2022-11-18 08:11:26.000000 prose-2.3.0/prose/core/image.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    10107 2022-11-18 08:11:26.000000 prose-2.3.0/prose/core/sequence.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    16022 2022-11-18 08:11:26.000000 prose-2.3.0/prose/core/source.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     4116 2022-11-18 08:11:26.000000 prose-2.3.0/prose/cutouts.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    25669 2022-11-18 08:11:26.000000 prose-2.3.0/prose/fluxes.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.325035 prose-2.3.0/prose/io/
--rw-r--r--   0 lgrcia     (501) staff       (20)      138 2022-02-22 12:25:15.000000 prose-2.3.0/prose/io/__init__.py
--rw-r--r--   0 lgrcia     (501) staff       (20)      686 2022-07-28 14:48:00.000000 prose-2.3.0/prose/io/create_fm_db.sql
--rw-r--r--   0 lgrcia     (501) staff       (20)    15537 2022-11-18 08:11:26.000000 prose-2.3.0/prose/io/fitsmanager.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     5759 2022-08-24 13:02:07.000000 prose-2.3.0/prose/io/io.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     1451 2022-03-30 14:26:57.000000 prose-2.3.0/prose/models.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    39155 2022-11-18 08:11:26.000000 prose-2.3.0/prose/observation.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    10378 2022-11-18 08:11:26.000000 prose-2.3.0/prose/observations.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.325761 prose-2.3.0/prose/pipeline/
--rw-r--r--   0 lgrcia     (501) staff       (20)       80 2022-02-22 12:25:15.000000 prose-2.3.0/prose/pipeline/__init__.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     8338 2022-11-18 08:11:26.000000 prose-2.3.0/prose/pipeline/calibration.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    12655 2022-07-28 14:48:00.000000 prose-2.3.0/prose/pipeline/photometry.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.326499 prose-2.3.0/prose/reports/
--rw-r--r--   0 lgrcia     (501) staff       (20)      200 2022-04-12 12:36:40.000000 prose-2.3.0/prose/reports/__init__.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     3882 2022-11-18 08:11:26.000000 prose-2.3.0/prose/reports/core.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     6738 2022-07-28 14:54:29.000000 prose-2.3.0/prose/reports/summary.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    11016 2022-11-18 08:11:26.000000 prose-2.3.0/prose/simulations.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     6459 2022-11-18 08:11:26.000000 prose-2.3.0/prose/telescope.py
--rw-r--r--   0 lgrcia     (501) staff       (20)     3843 2022-11-18 08:11:26.000000 prose-2.3.0/prose/tutorials.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    15467 2022-11-18 08:11:26.000000 prose-2.3.0/prose/utils.py
--rw-r--r--   0 lgrcia     (501) staff       (20)    28288 2022-08-24 13:02:07.000000 prose-2.3.0/prose/visualization.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.308399 prose-2.3.0/prose.egg-info/
--rw-r--r--   0 lgrcia     (501) staff       (20)     3878 2022-11-18 08:12:28.000000 prose-2.3.0/prose.egg-info/PKG-INFO
--rw-r--r--   0 lgrcia     (501) staff       (20)     1289 2022-11-18 08:12:29.000000 prose-2.3.0/prose.egg-info/SOURCES.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)        1 2022-11-18 08:12:28.000000 prose-2.3.0/prose.egg-info/dependency_links.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)      290 2022-11-18 08:12:29.000000 prose-2.3.0/prose.egg-info/requires.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)        6 2022-11-18 08:12:29.000000 prose-2.3.0/prose.egg-info/top_level.txt
--rw-r--r--   0 lgrcia     (501) staff       (20)        1 2022-02-23 10:02:48.000000 prose-2.3.0/prose.egg-info/zip-safe
--rw-r--r--   0 lgrcia     (501) staff       (20)       38 2022-11-18 08:12:29.327481 prose-2.3.0/setup.cfg
--rw-r--r--   0 lgrcia     (501) staff       (20)     1568 2022-11-18 08:11:26.000000 prose-2.3.0/setup.py
-drwxr-xr-x   0 lgrcia     (501) staff       (20)        0 2022-11-18 08:12:29.326769 prose-2.3.0/test/
--rw-r--r--   0 lgrcia     (501) staff       (20)    13363 2022-11-18 08:11:26.000000 prose-2.3.0/test/test.py
+-rw-r--r--   0        0        0     1097 2023-05-17 11:58:22.053360 prose-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2574 2023-05-17 11:58:22.053360 prose-3.0.0/README.md
+-rw-r--r--   0        0        0      651 2023-05-17 11:58:22.177361 prose-3.0.0/prose/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-17 11:58:22.177361 prose-3.0.0/prose/archive/__init__.py
+-rw-r--r--   0        0        0     2397 2023-05-17 11:58:22.177361 prose-3.0.0/prose/archive/pos1.py
+-rw-r--r--   0        0        0     2071 2023-05-17 11:58:22.177361 prose-3.0.0/prose/archive/sdss.py
+-rw-r--r--   0        0        0      254 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/__init__.py
+-rw-r--r--   0        0        0     3553 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/alignment.py
+-rw-r--r--   0        0        0     3028 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/background.py
+-rw-r--r--   0        0        0     8569 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/catalogs.py
+-rw-r--r--   0        0        0     8706 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/centroids.py
+-rw-r--r--   0        0        0    13532 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/detection.py
+-rw-r--r--   0        0        0     6597 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/geometry.py
+-rw-r--r--   0        0        0     3743 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/photometry.py
+-rw-r--r--   0        0        0    13913 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/psf.py
+-rw-r--r--   0        0        0     3703 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/shepard.py
+-rw-r--r--   0        0        0    20531 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/utils.py
+-rw-r--r--   0        0        0     4012 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/visualization.py
+-rw-r--r--   0        0        0     4069 2023-05-17 11:58:22.181361 prose-3.0.0/prose/builtins.py
+-rw-r--r--   0        0        0     5113 2023-05-17 11:58:22.181361 prose-3.0.0/prose/config.py
+-rw-r--r--   0        0        0     3733 2023-05-17 11:58:22.181361 prose-3.0.0/prose/console_utils.py
+-rw-r--r--   0        0        0      120 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/__init__.py
+-rw-r--r--   0        0        0     3356 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/block.py
+-rw-r--r--   0        0        0    22974 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/image.py
+-rw-r--r--   0        0        0    10521 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/sequence.py
+-rw-r--r--   0        0        0    16375 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/source.py
+-rw-r--r--   0        0        0    17092 2023-05-17 11:58:22.181361 prose-3.0.0/prose/fluxes.py
+-rw-r--r--   0        0        0      137 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/__init__.py
+-rw-r--r--   0        0        0      686 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/create_fm_db.sql
+-rw-r--r--   0        0        0    20099 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/fitsmanager.py
+-rw-r--r--   0        0        0     6386 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/io.py
+-rw-r--r--   0        0        0    15085 2023-05-17 11:58:22.181361 prose-3.0.0/prose/simulations.py
+-rw-r--r--   0        0        0     7901 2023-05-17 11:58:22.181361 prose-3.0.0/prose/telescope.py
+-rw-r--r--   0        0        0    14620 2023-05-17 11:58:22.181361 prose-3.0.0/prose/utils.py
+-rw-r--r--   0        0        0    29851 2023-05-17 11:58:22.181361 prose-3.0.0/prose/visualization.py
+-rw-r--r--   0        0        0      996 2023-05-17 11:58:22.181361 prose-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 prose-3.0.0/PKG-INFO
```

### Comparing `prose-2.3.0/LICENSE` & `prose-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prose-2.3.0/README.md` & `prose-3.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,84 @@
 # prose
 
-<p align="center">
-    <img src="https://github.com/lgrcia/prose/blob/master/docs/source/prose_illustration.png" width="350">
+<p align="center" style="margin-bottom:-50px">
+    <img src="docs/_static/prose3.png" width="450">
 </p>
 
 <p align="center">
-  A python package to build FITS images pipelines.
+  Modular image processing pipelines for Astronomy
   <br>
   <p align="center">
     <a href="https://github.com/lgrcia/prose">
-      <img src="https://img.shields.io/badge/github-lgrcia/prose-blue.svg?style=flat" alt="github"/>
+      <img src="https://img.shields.io/badge/github-lgrcia/prose-03A487.svg?style=flat" alt="github"/>
     </a>
-    <a href="">
+    <a href="LICENCE">
       <img src="https://img.shields.io/badge/license-MIT-lightgray.svg?style=flat" alt="license"/>
     </a>
     <a href="https://arxiv.org/abs/2111.02814">
-      <img src="https://img.shields.io/badge/paper-yellow.svg?style=flat" alt="paper"/>
+      <img src="https://img.shields.io/badge/paper-B166A9.svg?style=flat" alt="paper"/>
     </a>
-    <a href="https://lgrcia.github.io/prose-docs">
+    <a href="https://prose.readthedocs.io/en/3.0.0">
       <img src="https://img.shields.io/badge/documentation-black.svg?style=flat" alt="documentation"/>
     </a>
   </p>
 </p>
 
- *prose* is a Python package to build pipelines dedicated to astronomical image processing, all based on pipy packages 📦. Beyond providing the blocks to do so, it features default pipelines to perform common tasks such as automated calibration, reduction and photometry.
+ *prose* is a Python package to build image processing pipelines for Astronomy. Beyond featuring the blocks to build pipelines from scratch, it provides pre-implemented ones to perform common tasks such as automated calibration, reduction and photometry.
+
+*powered by [astropy](https://www.astropy.org/) and [photutils](https://photutils.readthedocs.io)*!
 
 ## Example
 
 Here is a quick example pipeline to characterize the point-spread-function (PSF) of an example image
 
 
 ```python
-from prose import Sequence, blocks
-from prose.tutorials import example_image
 import matplotlib.pyplot as plt
+from prose import Sequence, blocks
+from prose.simulations import example_image
 
 # getting the example image
 image = example_image()
 
-sequence = Sequence([
-    blocks.SegmentedPeaks(),  # stars detection
-    blocks.Cutouts(size=21),  # cutouts extraction
-    blocks.MedianPSF(),       # PSF building
-    blocks.psf.Moffat2D(),    # PSF modeling
-])
+sequence = Sequence(
+    [
+        blocks.PointSourceDetection(),  # stars detection
+        blocks.Cutouts(shape=21),  # cutouts extraction
+        blocks.MedianEPSF(),  # PSF building
+        blocks.Moffat2D(),  # PSF modeling
+    ]
+)
 
 sequence.run(image)
 
 # plotting
-image.show()           # detected stars
-image.plot_psf_model() # PSF model
-```
-
-While being run on a single image, a Sequence is designed to be run on list of images (paths) and provides the architecture to build powerful pipelines. For more details check [Quickstart](https://lgrcia.github.io/prose-docs/html/notebooks/quickstart.html) and [What is a pipeline?](https://lgrcia.github.io/prose-docs/html/rst/core.html)
-
-## Default pipelines
- *prose* features default pipelines to perform common tasks like:
-
-```python
-
-from prose.pipeline import Calibration, AperturePhotometry
-
-destination = "reduced_folder"
-
-reduction = Calibration(darks=[...], flats=[...])
-reduction.run(images, destination)
-
-photometry = AperturePhotometry(calib.images, calib.stack)
-photometry.run(calib.phot)
+image.show()  # detected stars
 
+# effective PSF parameters
+image.epsf.params
 ```
 
-However, the package is designed to avoid pre-implemented black-boxes, in favor of transparent pipelines. For a practical illustration of that, check our [Photometry tutorial](https://lgrcia.github.io/prose-docs/html/notebooks/photometry.html).
+While being run on a single image, a Sequence is designed to be run on list of images (paths) and provides the architecture to build powerful pipelines. For more details check [Quickstart](https://prose.readthedocs.io/en/latest/ipynb/quickstart.html) and [What is a pipeline?](https://prose.readthedocs.io/en/latest/ipynb/core.html)
 
 ## Installation
 
 ### latest
 
 *prose* is written for python 3 and can be installed from [pypi](https://pypi.org/project/prose/) with:
 
 ```shell
 pip install prose
 ```
 
-To install it through conda (recommended, within a fresh environment):
+For the latest version 
 
 ```shell
-conda install numpy scipy tensorflow netcdf4 numba
-
-# then 
-
-pip install prose
-```
-
-### dev
-
-clone the repo
-
-```shell
-git clone https://github.com/lgrcia/prose.git
+pip install 'prose @ git+https://github.com/lgrcia/prose'
 ```
 
-install locally (if within conda, same environment setup as above)
-
-```
-pip install -e {path_to_repo}
-```
-
-
-## Helping us
-
-We are interested in seeing how you use prose, as well as helping creating blocks you need. Do not hesitate to reach us out! ☎️
+## Contributions
+See our [contributions guidelines](docs/CONTRIBUTING.md)
 
 <p align="center">
-    <img src="docs/source/lookatit.png" width="150">
+    <img src="docs/_static/lookatit.png" width="150">
 </p>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,39 +1,26 @@
 # prose
-           [https://github.com/lgrcia/prose/blob/master/docs/source/
-                            prose_illustration.png]
-               A python package to build FITS images pipelines.
+                           [docs/_static/prose3.png]
+               Modular image processing pipelines for Astronomy
                   [github] [license] [paper] [documentation]
-*prose* is a Python package to build pipelines dedicated to astronomical image
-processing, all based on pipy packages ð¦. Beyond providing the blocks to do
-so, it features default pipelines to perform common tasks such as automated
-calibration, reduction and photometry. ## Example Here is a quick example
-pipeline to characterize the point-spread-function (PSF) of an example image
-```python from prose import Sequence, blocks from prose.tutorials import
-example_image import matplotlib.pyplot as plt # getting the example image image
-= example_image() sequence = Sequence([ blocks.SegmentedPeaks(), # stars
-detection blocks.Cutouts(size=21), # cutouts extraction blocks.MedianPSF(), #
-PSF building blocks.psf.Moffat2D(), # PSF modeling ]) sequence.run(image) #
-plotting image.show() # detected stars image.plot_psf_model() # PSF model ```
-While being run on a single image, a Sequence is designed to be run on list of
-images (paths) and provides the architecture to build powerful pipelines. For
-more details check [Quickstart](https://lgrcia.github.io/prose-docs/html/
-notebooks/quickstart.html) and [What is a pipeline?](https://lgrcia.github.io/
-prose-docs/html/rst/core.html) ## Default pipelines *prose* features default
-pipelines to perform common tasks like: ```python from prose.pipeline import
-Calibration, AperturePhotometry destination = "reduced_folder" reduction =
-Calibration(darks=[...], flats=[...]) reduction.run(images, destination)
-photometry = AperturePhotometry(calib.images, calib.stack) photometry.run
-(calib.phot) ``` However, the package is designed to avoid pre-implemented
-black-boxes, in favor of transparent pipelines. For a practical illustration of
-that, check our [Photometry tutorial](https://lgrcia.github.io/prose-docs/html/
-notebooks/photometry.html). ## Installation ### latest *prose* is written for
-python 3 and can be installed from [pypi](https://pypi.org/project/prose/
-) with: ```shell pip install prose ``` To install it through conda
-(recommended, within a fresh environment): ```shell conda install numpy scipy
-tensorflow netcdf4 numba # then pip install prose ``` ### dev clone the repo
-```shell git clone https://github.com/lgrcia/prose.git ``` install locally (if
-within conda, same environment setup as above) ``` pip install -e
-{path_to_repo} ``` ## Helping us We are interested in seeing how you use prose,
-as well as helping creating blocks you need. Do not hesitate to reach us out!
-âï¸
-                          [docs/source/lookatit.png]
+*prose* is a Python package to build image processing pipelines for Astronomy.
+Beyond featuring the blocks to build pipelines from scratch, it provides pre-
+implemented ones to perform common tasks such as automated calibration,
+reduction and photometry. *powered by [astropy](https://www.astropy.org/) and
+[photutils](https://photutils.readthedocs.io)*! ## Example Here is a quick
+example pipeline to characterize the point-spread-function (PSF) of an example
+image ```python import matplotlib.pyplot as plt from prose import Sequence,
+blocks from prose.simulations import example_image # getting the example image
+image = example_image() sequence = Sequence( [ blocks.PointSourceDetection(), #
+stars detection blocks.Cutouts(shape=21), # cutouts extraction
+blocks.MedianEPSF(), # PSF building blocks.Moffat2D(), # PSF modeling ] )
+sequence.run(image) # plotting image.show() # detected stars # effective PSF
+parameters image.epsf.params ``` While being run on a single image, a Sequence
+is designed to be run on list of images (paths) and provides the architecture
+to build powerful pipelines. For more details check [Quickstart](https://
+prose.readthedocs.io/en/latest/ipynb/quickstart.html) and [What is a pipeline?]
+(https://prose.readthedocs.io/en/latest/ipynb/core.html) ## Installation ###
+latest *prose* is written for python 3 and can be installed from [pypi](https:/
+/pypi.org/project/prose/) with: ```shell pip install prose ``` For the latest
+version ```shell pip install 'prose @ git+https://github.com/lgrcia/prose' ```
+## Contributions See our [contributions guidelines](docs/CONTRIBUTING.md)
+                          [docs/_static/lookatit.png]
```

### Comparing `prose-2.3.0/prose/archive/pos1.py` & `prose-3.0.0/prose/archive/pos1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,19 @@
+from io import StringIO
+
+import astropy.units as u
 import numpy as np
-from astropy.table import Table
 import requests
-from io import StringIO
-from .. import Image, blocks, utils
-from prose.console_utils import info
 from astropy.io import fits
-import astropy.units as u
-from astropy.time import Time
-
-ps1_pixel_scale = 0.258
+from astropy.table import Table
 
-class PS1Image(Image):
+from prose import FITSImage, blocks, utils
+from prose.console_utils import info
+from prose.telescope import Telescope
 
-    ra = None
-    dec = None
-    filter = None
-    
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args,**kwargs)
-        
-    @property
-    def pixel_scale(self):
-        return ps1_pixel_scale * u.arcsec
-    
-    @property
-    def jd_utc(self):
-        return self.header["MJD-OBS"] + 2400000.5
-        
-    @property
-    def date(self):
-        """datetime of the observation
-
-        Returns
-        -------
-        datetime.datetime
-        """
-        return Time(self.jd_utc, format="jd", scale="utc").to_datetime()
- 
 
 def pos1_image(skycoord, fov, filter="z"):
     """
     A function to retrieve an PS1 ``Image`` object
 
     Parameters
     ----------
@@ -49,49 +22,54 @@
             - a list of int (interpreted as deg)
             - a str (interpreted as houranlgle, deg)
             - a SkyCoord object
     fov : list, tuple or Quantity array
         field of view of the image in the two axes. If list or tuple, interpreted as arcmin
     filter : str
         one of ["g", "r", "i", "z", "y"]
-    
+
     helped by https://outerspace.stsci.edu/display/PANSTARRS/PS1+Image+Cutout+Service
     """
 
     skycoord = utils.check_skycoord(skycoord)
+    telescope = Telescope(pixel_scale=0.258, keyword_observation_date="DATE")
 
     if isinstance(fov, (tuple, list)):
-        fov = np.array(fov)*u.arcmin
-    
-    w = (fov[0]/(ps1_pixel_scale * u.arcsec)).decompose().value
-    h = (fov[1]/(ps1_pixel_scale * u.arcsec)).decompose().value
+        fov = np.array(fov) * u.arcmin
+
+    w = (fov[0] / (telescope.pixel_scale * u.arcsec)).decompose().value
+    h = (fov[1] / (telescope.pixel_scale * u.arcsec)).decompose().value
     ra = skycoord.ra.to(u.deg).value
     dec = skycoord.dec.to(u.deg).value
-    
+
     size = int(np.max([w, h]))
-        
+
     cbuf = StringIO()
     cbuf.write(f"{ra} {dec}")
     cbuf.seek(0)
 
     info("Querying https://ps1images.stsci.edu/cgi-bin/ps1filenames.py")
     r = requests.post(
-        "https://ps1images.stsci.edu/cgi-bin/ps1filenames.py", 
+        "https://ps1images.stsci.edu/cgi-bin/ps1filenames.py",
         data=dict(filters=filter, type="stack"),
-        files=dict(file=cbuf)
+        files=dict(file=cbuf),
     )
     r.raise_for_status()
     tab = Table.read(r.text, format="ascii")
- 
-    urlbase = "{}?size={}&format={}".format("https://ps1images.stsci.edu/cgi-bin/fitscut.cgi", size, "fits")
-    tab["url"] = ["{}&ra={}&dec={}&red={}".format(urlbase,ra,dec,filename)
-            for (filename,ra,dec) in zip(tab["filename"],tab["ra"],tab["dec"])]
-    
+
+    urlbase = "{}?size={}&format={}".format(
+        "https://ps1images.stsci.edu/cgi-bin/fitscut.cgi", size, "fits"
+    )
+    tab["url"] = [
+        "{}&ra={}&dec={}&red={}".format(urlbase, ra, dec, filename)
+        for (filename, ra, dec) in zip(tab["filename"], tab["ra"], tab["dec"])
+    ]
+
     url = tab[0]["url"]
     query = requests.get(url)
     hdu = fits.HDUList.fromstring(query.content)
-    image = PS1Image(data=hdu[0].data, header=hdu[0].header, verbose=False)
-    image = blocks.Trim(trim=[int((size-w)/2), int((size-h)/2)])(image)
-    image.ra = skycoord.ra
-    image.dec = skycoord.dec
-    image.filter = filter
-    return image
+    image = FITSImage(hdu[0], telescope=telescope)
+    image = blocks.Trim(trim=[int((size - w) / 2), int((size - h) / 2)])(image)
+    image.metadata["ra"] = ra
+    image.metadata["dec"] = dec
+    image.metadata["filter"] = filter
+    return image
```

### Comparing `prose-2.3.0/prose/archive/sdss.py` & `prose-3.0.0/prose/archive/sdss.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,16 @@
+import astropy.units as u
 import numpy as np
-from astropy.coordinates import SkyCoord
-from prose.console_utils import info
 import requests
 from astropy.io import fits
-from .. import Image, utils
-import astropy.units as u
-from dateutil import parser as dparser
 
-class PhotographicPlate(Image):
+from prose import FITSImage, utils
+from prose.console_utils import info
+from prose.telescope import Telescope
 
-    ra = None
-    dec = None
-    filter = None
-    
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-    
-    @property
-    def pixel_scale(self):
-        return self.header["PLTSCALE"]*(u.arcsec/u.mm) * (self.header["XPIXELSZ"]*u.um).to(u.mm)
-    
-    @property
-    def skycoord(self):
-        return SkyCoord(*self.wcs.pixel_to_world_values([np.array(self.shape)/2])[0] * u.deg)
-
-    @property
-    def date(self):
-        date_str = self.header[self.telescope.keyword_observation_date][0:10]
-        return dparser.parse(date_str)
-    
 
 def sdss_image(skycoord, fov, filter="poss1_blue", return_hdu=False):
     """A function to retrieve an SDSS ``Image`` object
 
     Parameters
     ----------
     skycoord : list, tuple or SkyCoord
@@ -54,29 +32,34 @@
     Returns
     -------
     Image
         ``Image`` object of the SDSS field
     """
 
     skycoord = utils.check_skycoord(skycoord)
-        
+
     if isinstance(fov, (tuple, list)):
-        fov = np.array(fov)*u.arcmin
+        fov = np.array(fov) * u.arcmin
 
-    ra, dec = skycoord.to_string().split(' ')
+    ra, dec = skycoord.to_string().split(" ")
     h, w = fov.to(u.arcmin).value
     url = f"https://archive.stsci.edu/cgi-bin/dss_search?v={filter}&r={ra}&d={dec}&e=J2000&h={h}&w={w}&f=fits&c=none&s=on&fov=NONE&v3="
     info("Querying https://archive.stsci.edu/cgi-bin/dss_form")
     query = requests.get(url)
     hdu = fits.HDUList.fromstring(query.content)
-    
+
     if return_hdu:
         return hdu
-    
     else:
-        image = PhotographicPlate(data=np.array(hdu[0].data).astype(float), header=hdu[0].header, verbose=False)
-        image.ra = skycoord.ra
-        image.dec = skycoord.dec
-        image.filter = filter
-
+        pixel_scale = (
+            hdu[0].header["PLTSCALE"]
+            * (u.arcsec / u.mm)
+            * (hdu[0].header["XPIXELSZ"] * u.um).to(u.mm)
+        ).value
+        telescope = Telescope(pixel_scale=pixel_scale)
+
+        hdu[0].header["DATE-OBS"] = hdu[0].header["DATE-OBS"][0:10]
+        image = FITSImage(hdu[0], telescope=telescope)
+        image.metadata["ra"] = ra
+        image.metadata["dec"] = dec
+        image.metadata["filter"] = filter
         return image
-
```

### Comparing `prose-2.3.0/prose/blocks/background.py` & `prose-3.0.0/prose/blocks/background.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-from prose import  Block
-from prose.blocks.psf import *
+import numpy as np
 from astropy.stats import SigmaClip
 from photutils.background import Background2D, MedianBackground
-import numpy as np
-from ..utils import binn2D
 
+from prose import Block
+from prose.blocks.psf import *
+from prose.utils import binn2D
+
+# TODO
 
-class PhotutilsBackground2D(Block):
 
+class PhotutilsBackground2D(Block):
     def __init__(self, subtract=True, box_size=(50, 50), filter_size=(3, 3), **kwargs):
         super().__init__(**kwargs)
-        self.sigma_clip = SigmaClip(sigma=3.)
+        self.sigma_clip = SigmaClip(sigma=3.0)
         self.bkg_estimator = MedianBackground()
         self.subtract = subtract
         self.box_size = box_size
         self.filter_size = filter_size
 
     def run(self, image):
-        sigma_clip = SigmaClip(sigma=3.)
+        sigma_clip = SigmaClip(sigma=3.0)
         self.bkg = Background2D(
-            image.data, box_size=self.box_size,
+            image.data,
+            box_size=self.box_size,
             filter_size=self.filter_size,
-            sigma_clip=sigma_clip, 
-            bkg_estimator=self.bkg_estimator
+            sigma_clip=sigma_clip,
+            bkg_estimator=self.bkg_estimator,
         ).background
         if self.subtract:
             image.bkg = self.bkg
             image.data = image.data - self.bkg
 
     @property
     def citations(self):
@@ -47,43 +50,48 @@
         if ref is not None:
             self.X = self.design_matrix(ref.shape)
         else:
             self.X = None
         self.iterations = iterations
         self.sigclip = sigclip
         self.binning = binning
-        
+
     def design_matrix(self, shape):
         x, y = np.indices(shape)
         X = np.polynomial.polynomial.polyvander2d(
-                x.flatten(), y.flatten(), (self.order, self.order)
-            )
+            x.flatten(), y.flatten(), (self.order, self.order)
+        )
         X[:, 1:] -= X.mean(0)[1:]
         X[:, 1:] -= X.std(0)[1:]
         return X
-    
+
     def run(self, image):
         # First sigma clipping and binning
         data = image.data.copy()
-        mask = (data - np.mean(data)) < self.sigclip*np.std(data)
+        mask = (data - np.mean(data)) < self.sigclip * np.std(data)
         data[~mask] = np.median(data[mask])
         bin_data = binn2D(data, self.binning)
         mask = np.ones_like(bin_data).astype(bool).flatten()
-        
+
         if self.X is None:
             self.X = self.design_matrix(image.shape)
         elif self.X.shape[0] != np.product(image.shape):
             self.X = self.design_matrix(image.shape)
-            
-        bin_X = np.array([binn2D(np.reshape(x, image.shape), self.binning).flatten() for x in self.X.T]).T
-    
+
+        bin_X = np.array(
+            [
+                binn2D(np.reshape(x, image.shape), self.binning).flatten()
+                for x in self.X.T
+            ]
+        ).T
+
         for _ in range(self.iterations):
             masked_data = bin_data.flatten()[mask]
             w = np.linalg.lstsq(bin_X[mask, :], masked_data, rcond=False)[0]
-            res = bin_data.flatten() - bin_X@w
-            mask *= res < self.sigclip*np.std(res[mask])
-        
-        image.bkg = np.reshape(self.X@w, image.shape)
+            res = bin_data.flatten() - bin_X @ w
+            mask *= res < self.sigclip * np.std(res[mask])
+
+        image.bkg = np.reshape(self.X @ w, image.shape)
 
     @property
     def citations(self):
-        return "numpy"
+        return "numpy"
```

### Comparing `prose-2.3.0/prose/blocks/shepard.py` & `prose-3.0.0/prose/blocks/shepard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-from .. import Block
-from .psf import good_cutouts, cutouts
-from astropy.stats import gaussian_sigma_to_fwhm
-from prose.blocks.psf import Gaussian2D
 from itertools import product
+
 import numpy as np
+from astropy.stats import gaussian_sigma_to_fwhm
 from scipy.special import hermite
 
+from prose import Block
+from prose.blocks.psf import Gaussian2D
+
+from .psf import cutouts, good_cutouts
+
+
 def shapelet1d(x, n, b=1):
     _x = x / b
-    s = (1 / np.sqrt((2 ** n) * np.sqrt(np.pi) * np.math.factorial(n))) * hermite(n)(_x) * np.exp(-(_x ** 2) / 2)
+    s = (
+        (1 / np.sqrt((2**n) * np.sqrt(np.pi) * np.math.factorial(n)))
+        * hermite(n)(_x)
+        * np.exp(-(_x**2) / 2)
+    )
     return (1 / np.sqrt(b)) * s
 
 
 def shapelet2d(x, y, n1, n2, b=1):
     X, Y = np.meshgrid(x, y)
     return shapelet1d(X, n1, b) * shapelet1d(Y, n2, b)
 
 
 class Shepard(Block):
-
-    
     def __init__(self, order=4, size=31, **kwargs):
         super().__init__(**kwargs)
         self.order = order
         self.size = size
 
         # --------------
 
@@ -44,22 +50,26 @@
         x = np.arange(self.size)
 
         def basis(x0, y0):
             if self.size == 0:
                 ns = [(0, 0)]
             else:
                 ns = product(range(self.order), repeat=2)
-            return [*[shapelet2d(x - x0, x - y0, n1, n2, fwhm).flatten() for n1, n2 in ns]]
+            return [
+                *[shapelet2d(x - x0, x - y0, n1, n2, fwhm).flatten() for n1, n2 in ns]
+            ]
 
         stars_groups = []
         _xy_dict = dict(zip(np.arange(len(stars)), stars))
 
         for i, _xy in _xy_dict.copy().items():
             if i in _xy_dict:
-                close = np.nonzero(np.linalg.norm(_xy - stars, axis=1) < self.size / 2)[0]
+                close = np.nonzero(np.linalg.norm(_xy - stars, axis=1) < self.size / 2)[
+                    0
+                ]
                 if len(close) >= 1:
                     stars_groups.append(close)
                     for c in close:
                         if c in _xy_dict:
                             del _xy_dict[c]
 
         stars_coords_groups = np.array([stars[s] for s in stars_groups])
@@ -70,24 +80,32 @@
         self.group_centers = group_centers[idxs]
         self.stars_coords_groups = stars_coords_groups[idxs]
 
         self.Xs = []
         for i, c in enumerate(groups_cutouts):
             c = groups_cutouts[i]
             scg = self.stars_coords_groups[i] - (c.bbox.ixmin, c.bbox.iymin)
-            X = np.vstack([np.ones((self.size, self.size)).flatten(), *[basis(*s) for s in scg]])
+            X = np.vstack(
+                [np.ones((self.size, self.size)).flatten(), *[basis(*s) for s in scg]]
+            )
             self.Xs.append(X)
 
     def run(self, image, **kwargs):
         if self.Xs is None:
             self.prepare(image.data, image.stars_coords, image.fwhm)
 
         fluxes = {}
         idxs, groups_cutouts = cutouts(image.data, self.group_centers, self.size)
         for i, c in enumerate(groups_cutouts):
             w = np.linalg.lstsq(self.Xs[i].T, c.data.flatten())[0]
             scg = self.stars_coords_groups[i]
-            for j, _X, _w in zip(self.stars_groups[i], np.split(self.Xs[i][1::], len(scg)), np.split(w[1::], len(scg))):
+            for j, _X, _w in zip(
+                self.stars_groups[i],
+                np.split(self.Xs[i][1::], len(scg)),
+                np.split(w[1::], len(scg)),
+            ):
                 fluxes[j] = (_w @ _X).sum()
 
-        image.fluxes = np.array([np.array([fluxes.get(i, np.nan) for i in range(len(image.stars_coords))])])
+        image.fluxes = np.array(
+            [np.array([fluxes.get(i, np.nan) for i in range(len(image.stars_coords))])]
+        )
         image.fluxes_errors = np.sqrt(image.fluxes)
```

### Comparing `prose-2.3.0/prose/blocks/vizualisation.py` & `prose-3.0.0/prose/blocks/visualization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,139 @@
-import numpy as np
-from .. import Block, viz
-import matplotlib.pyplot as plt
+import io
+import shutil
+import tempfile
+import time
+
 import imageio
-from prose.visualization import corner_text
-from skimage.transform import resize
+import matplotlib.pyplot as plt
+import numpy as np
 from matplotlib.backends.backend_agg import FigureCanvasAgg
-import time
+from skimage.transform import resize
+
+from prose import Block, viz
+from prose.visualization import corner_text
+
+__all__ = ["VideoPlot"]
+
 
 def im_to_255(image, factor=0.25):
-    if factor !=1:
+    if factor != 1:
         return (
             resize(
                 image.astype(float),
                 (np.array(np.shape(image)) * factor).astype(int),
                 anti_aliasing=False,
-            ) * 255).astype("uint8")
+            )
+            * 255
+        ).astype("uint8")
     else:
         data = image.copy().astype(float)
-        data = data/np.max(data)
+        data = data / np.max(data)
         data = data * 255
         return data.astype("uint8")
 
 
 class _Video(Block):
-    """Base block to build a video
-    """
+    """Base block to build a video"""
 
     def __init__(self, destination, fps=10, **kwargs):
-
         super().__init__(**kwargs)
         self.destination = destination
         self.images = []
         self.fps = fps
         self.checked_writer = False
-        
+
     def run(self, image):
         if not self.checked_writer:
             _ = imageio.get_writer(self.destination, mode="I")
             self.checked_writer = True
-            
+
     def terminate(self):
         imageio.mimsave(self.destination, self.images, fps=self.fps)
 
     @property
     def citations(self):
         return "imageio"
 
 
 class RawVideo(_Video):
-    
-    def __init__(self, destination, attribute="data", fps=10, function=None, scale=1, **kwargs):
+    def __init__(
+        self, destination, attribute="data", fps=10, function=None, scale=1, **kwargs
+    ):
         super().__init__(destination, fps=fps, **kwargs)
         if function is None:
-            def _donothing(data): return data
+
+            def _donothing(data):
+                return data
+
             function = _donothing
-        
+
         self.function = function
         self.scale = scale
         self.attribute = attribute
-    
+
     def run(self, image):
         super().run(image)
         data = self.function(image.__dict__[self.attribute])
         self.images.append(im_to_255(data, factor=self.scale))
-        
-        
-class PlotVideo(_Video):
 
-    def __init__(self, plot_function, destination, fps=10, antialias=False, **kwargs):
-        super().__init__(destination, fps=fps, **kwargs)
-        self.plot_function = plot_function
-        self._init_alias = plt.rcParams['text.antialiased']
-        plt.rcParams['text.antialiased'] = antialias
 
-    def to_rbg(self):
-        fig = plt.gcf()
-        canvas = FigureCanvasAgg(fig)
-        canvas.draw()
-        width, height = fig.canvas.get_width_height()
-        returned = np.frombuffer(canvas.tostring_rgb(), dtype='uint8').reshape(height, width, 3)
-        plt.imshow(returned)
-        plt.close()
-        return returned
+class VideoPlot(_Video):
+    def __init__(self, plot_function, destination, fps=10, name=None):
+        """Make a video out of a plotting function
+
+        Parameters
+        ----------
+        plot_function : function
+            a plotting function taking an :py:class:`prose.Image` as input
+        destination : str or Path
+            destination of the video, including extension
+        fps : int, optional
+            frame per seconds, by default 10
+        antialias : bool, optional
+            whether pyplot antialias should be used, by default False
+        """
+        super().__init__(destination, fps=fps, name=name)
+        self.plot_function = plot_function
+        self.destination = destination
+        self._temp = tempfile.mkdtemp()
+        self._images = []
 
     def run(self, image):
-        super().run(image)
         self.plot_function(image)
-        self.images.append(self.to_rbg())
+        buf = io.BytesIO()
+        plt.savefig(buf)
+        self.images.append(imageio.imread(buf))
+        plt.close()
 
     def terminate(self):
         super().terminate()
-        plt.rcParams['text.antialiased'] = self._init_alias
+        shutil.rmtree(self._temp)
 
 
 class LivePlot(Block):
-
-    def __init__(self, plot_function=None, sleep=0., size=None, **kwargs):
+    def __init__(self, plot_function=None, sleep=0.0, size=None, **kwargs):
         super().__init__(**kwargs)
         if plot_function is None:
             plot_function = lambda im: viz.show_stars(
-                im.data, im.stars_coords if hasattr(im, "stars_coords") else None,
-                size=size
-                )
+                im.data,
+                im.stars_coords if hasattr(im, "stars_coords") else None,
+                size=size,
+            )
 
         self.plot_function = plot_function
         self.sleep = sleep
         self.display = None
         self.size = size
         self.figure_added = False
 
     def run(self, image):
         if not self.figure_added:
             from IPython import display as disp
+
             self.display = disp
             if isinstance(self.size, tuple):
                 plt.figure(figsize=self.size)
             self.figure_added = True
 
         self.plot_function(image)
         self.display.clear_output(wait=True)
```

### Comparing `prose-2.3.0/prose/config.py` & `prose-3.0.0/prose/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import shutil
 from os import path
 from pathlib import Path
-import yaml
-from yaml import Loader
+
 import numpy as np
-import shutil
-from .builtins import built_in_telescopes
-import glob
 import requests
+import yaml
+from yaml import Loader
+
+from prose.builtins import built_in_telescopes
 
 info = print
 package_name = "prose"
 
+
 class ConfigManager:
     def __init__(self):
-
         self.config = None
 
         self.folder_path = Path.home() / f".{package_name}"
         self.folder_path.mkdir(exist_ok=True)
 
         self.config_file = self.folder_path / "config"
 
@@ -25,15 +26,14 @@
         self.create_builtins_telescopes_files()
         self.check_config_file(load=True)
         self.telescopes_dict = self.build_telescopes_dict()
         self.check_ballet()
         self.logs = []
 
     def check_config_file(self, load=False):
-
         if self.config_file.exists():
             with self.config_file.open(mode="r") as file:
                 if load:
                     self.config = yaml.load(file.read(), Loader=Loader)
         else:
             info(f"A config file as been created in {self.folder_path}")
             self.config = {"color": "blue"}
@@ -49,30 +49,31 @@
         return self.config.get(key)
 
     def set(self, key, value):
         self.config[key] = value
         self.save()
 
     def rename_id_files_to_telescopes(self):
-        """For backward compat with 0.9.6 downward
-        """
+        """For backward compat with 0.9.6 downward"""
         id_files = list(self.folder_path.glob("*.id"))
         if len(id_files) > 0:
             info("Renaming some old .id telescope files")
             for fpath in id_files:
                 shutil.move(fpath, str(fpath).replace(".id", ".telescope"))
 
     def check_builtins_changes(self):
         for name, telescope in built_in_telescopes.items():
             telescope_file_name = path.join(self.folder_path, f"{name}.telescope")
             if path.exists(telescope_file_name):
                 with open(telescope_file_name, mode="r") as f:
                     existing_telescope = yaml.load(f, Loader=yaml.FullLoader)
                     if existing_telescope != telescope:
-                        info(f"{Path(telescope_file_name).name} differs from builtins (use prose.CONFIG.update_builtins() to update)")
+                        info(
+                            f"{Path(telescope_file_name).name} differs from builtins (use prose.CONFIG.update_builtins() to update)"
+                        )
 
     def update_builtins(self):
         self.create_builtins_telescopes_files(force=True)
 
     def build_telescopes_dict(self):
         telescope_files = self.folder_path.glob("*.telescope")
 
@@ -99,32 +100,39 @@
     def save_telescope_file(self, file):
         if isinstance(file, str):
             name = Path(file).stem.lower()
             shutil.copyfile(file, self.folder_path / f"{name}.telescope")
             info("Telescope '{}' saved".format(name))
         elif isinstance(file, dict):
             name = file["name"].lower()
-            telescope_file_path =  self.folder_path / f"{name}.telescope"
+            telescope_file_path = self.folder_path / f"{name}.telescope"
             yaml.dump(file, telescope_file_path.open(mode="w"))
             info("Telescope '{}' saved".format(name))
         else:
             raise AssertionError("input type not understood")
         self.telescopes_dict = self.build_telescopes_dict()
 
     def match_telescope_name(self, name):
-        if not isinstance(name, str):
-            return None
         available_telescopes_names = list(self.telescopes_dict.keys())
-        has_telescope = np.where(
+        has_telescope = np.flatnonzero(
             [t.lower() == name.lower() for t in available_telescopes_names]
-        )[0]
+        )
         if len(has_telescope) > 0:
-            i = np.argmax([len(name) for name in np.array(available_telescopes_names)[has_telescope]])
+            i = np.argmax(
+                [
+                    len(name)
+                    for name in np.array(available_telescopes_names)[has_telescope]
+                ]
+            )
             return self.telescopes_dict[available_telescopes_names[has_telescope[i]]]
+        else:
+            return None
 
     def check_ballet(self):
         model_path = self.folder_path / "centroid.h5"
 
         if not model_path.exists():
             print("downloading ballet model (~30Mb)")
-            model = requests.get("https://github.com/lgrcia/ballet/raw/master/models/centroid.h5").content
+            model = requests.get(
+                "https://github.com/lgrcia/ballet/raw/master/models/centroid.h5"
+            ).content
             model_path.open(mode="wb").write(model)
```

### Comparing `prose-2.3.0/prose/console_utils.py` & `prose-3.0.0/prose/console_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import os
+import platform
 import shlex
 import struct
-import platform
 import subprocess
-from . import CONFIG
+import warnings
 from datetime import datetime
-from tqdm import tqdm as _tqdm
+
+from tqdm import TqdmExperimentalWarning
+
+from prose import CONFIG
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore", category=TqdmExperimentalWarning)
+    from tqdm.autonotebook import tqdm
+
 
 def color(s, i):
     return f"\u001b[38;5;{i}m{s}\x1b[0m"
 
+
 TQDM_BAR_FORMAT = "%s {l_bar}%s{bar}%s{r_bar}" % (
-    color("RUN", 12), "\u001b[38;5;12m", "\x1b[0m"
+    color("RUN", 12),
+    "\u001b[38;5;12m",
+    "\x1b[0m",
 )
 
-def tqdm(x, desc="run", unit="images", **kwargs):
-    return _tqdm(x, desc=desc, unit=unit, ncols=80, bar_format=TQDM_BAR_FORMAT, **kwargs)
 
 def progress(show, **kwargs):
     if show:
         return lambda x: tqdm(x, **kwargs)
     else:
         return lambda x: x
 
+
 def get_terminal_size():
-    """ getTerminalSize()
-     - get width and height of console
-     - works on linux,os x,windows,cygwin(windows)
-     originally retrieved from:
-     http://stackoverflow.com/questions/566746/how-to-get-console-window-width-in-python
+    """getTerminalSize()
+    - get width and height of console
+    - works on linux,os x,windows,cygwin(windows)
+    originally retrieved from:
+    http://stackoverflow.com/questions/566746/how-to-get-console-window-width-in-python
     """
     current_os = platform.system()
     tuple_xy = None
     if current_os == "Windows":
         tuple_xy = _get_terminal_size_windows()
         if tuple_xy is None:
             tuple_xy = _get_terminal_size_tput()
@@ -45,15 +55,15 @@
         tuple_xy = (80, 25)  # default value
 
     return tuple_xy
 
 
 def _get_terminal_size_windows():
     try:
-        from ctypes import windll, create_string_buffer
+        from ctypes import create_string_buffer, windll
 
         # stdin handle is -10
         # stdout handle is -11
         # stderr handle is -12
         h = windll.kernel32.GetStdHandle(-12)
         csbi = create_string_buffer(22)
         res = windll.kernel32.GetConsoleScreenBufferInfo(h, csbi)
@@ -113,29 +123,32 @@
             cr = (os.environ["LINES"], os.environ["COLUMNS"])
         except:
             return None
 
     return int(cr[1]), int(cr[0])
 
 
-
 def _log(type, s):
     date = datetime.now().strftime("[%Y-%m-%d %H:%M:%S]")
     for file in CONFIG.logs:
         open(file, "a").write(f"{date} {type} {s}\n")
 
+
 def log(s):
     print(s)
     for file in CONFIG.logs:
         open(file, "a").write(f"{s}\n")
 
+
 def info(s):
     print(f"{color('INFO', 12)} {s}")
-    _log('INFO', s)
+    _log("INFO", s)
+
 
 def warning(s):
     print(f"{color('WARNING', 3)} {s}")
-    _log('WARNING', s)
+    _log("WARNING", s)
+
 
 def error(s):
     print(f"{color('ERROR', 1)} {s}")
-    _log('ERROR', s)
+    _log("ERROR", s)
```

### Comparing `prose-2.3.0/prose/core/image.py` & `prose-3.0.0/prose/core/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,351 +1,135 @@
-from astropy.time import Time
+import pickle
+from copy import deepcopy
+from dataclasses import asdict, dataclass
+from datetime import timedelta
+from pathlib import Path
+from typing import Union
+
+import astropy.units as u
 import matplotlib.pyplot as plt
 import numpy as np
-from astropy.coordinates import SkyCoord
-import astropy.units as u
-from astropy.coordinates import Angle
-from dateutil import parser as dparser
+from astropy.coordinates import Angle, SkyCoord
+from astropy.io import fits
+from astropy.io.fits.hdu.base import _BaseHDU
+from astropy.io.fits.header import Header
+from astropy.nddata import Cutout2D as astopy_Cutout2D
+from astropy.nddata import overlap_slices
+from astropy.time import Time
 from astropy.wcs import WCS
-from .. import viz, utils, Telescope
-from ..utils import gaia_query
-from functools import partial
+from astropy.wcs.wcs import WCS
+from dateutil import parser as dparser
 from matplotlib import gridspec
-from astropy.io import fits
-from datetime import timedelta
-from pathlib import Path
-from .source import PointSource
-
-class Image:
-    def __init__(self, fitspath=None, data=None, header=None, verbose=True, telescope=None, **kwargs):
-        r"""Object containing image data and metadata
+from PIL import Image
 
-        When a FITS path (or header) is provided, keyword values are used to identify and instantiate a :py:class:`~prose.Telescope` object. Image attributes then use this object to retrieve specific image information such as ra, dec, untis... etc
+from prose import utils, viz
+from prose.core.source import Sources
+from prose.telescope import Telescope
 
-        Parameters
-        ----------
-        fitspath : str or Path, optional
-            file path , by default None
-        data : numpy.ndarray, optional
-            image data, by default None
-        header : dict-like, optional
-            image metadata, by default None 
-
-        Example
-        -------
 
-        .. jupyter-execute::
-
-            from prose.tutorials import image_sample
-
-            # loading and showing an example image
-            image = image_sample("05 38 44.851", "+04 32 47.68")
-            image.show()
-
-        .. jupyter-execute::
-            
-            image.header[0:10] # the 10 first lines
-
-        Once this object is instantiated, its parameters are mapped to the ones of the telescope, detected from the header information. This exposes conveniant attributres, for example:
-
-        .. jupyter-execute::
-
-            print(f"pixel scale : {image.pixel_scale:.2f}\nFOV: {image.fov}\nnight: {image.night_date}\n")
-
-        some of them being directly translated into astropy Quantity or datetime object.
-
-        """
-        self.verbose = verbose
+@dataclass
+class Image:
+    """
+    Image object containing image data and metadata
 
-        if fitspath is not None:
-            self._get_data_header(fitspath)
+    This is a Python Data Class, so that most attributes described below can be used as
+    keyword-arguments when instantiated
+    """
+
+    data: np.ndarray = None
+    """Image data"""
+
+    metadata: dict = None
+    """Image metadata"""
+
+    catalogs: dict = None
+    """Catalogs associated with the image contained in a dictionary of 
+    pandas dataframes"""
+
+    _sources: Union[Sources, dict] = None
+
+    origin: tuple = (0, 0)
+    """Image origin"""
+
+    discard: bool = False
+    """Whether image as been discarded by a block"""
+
+    computed: dict = None
+    """A dictionary containing any user and block-defined attributes"""
+
+    header: Header = None
+    """FITS header associated with the image (optional)"""
+
+    _wcs = None
+
+    def __post_init__(self):
+        assert (
+            isinstance(self.data, np.ndarray) or self.data is None
+        ), f"data must be a np.ndarray, not {type(self.data)}"
+        if self.metadata is None:
+            self.metadata = {}
+        if self.catalogs is None:
+            self.catalogs = {}
+        if self.computed is None:
+            self.computed = {}
+        if self.header is None:
+            self.header = Header()
+        if isinstance(self._sources, dict):
+            self._sources = Sources(**self._sources)
+        if self._sources is None:
+            self._sources = Sources([])
+
+    def __setattr__(self, name, value):
+        if hasattr(self, name):
+            super().__setattr__(name, value)
         else:
-            self.data = data
-            self.header = header if header is not None else {}
-            self.path = None
-        
-        self.sources = []
-        self.telescope = None
-        self.discard = False
-        self.__dict__.update(kwargs)
-        if telescope is None:
-            self._check_telescope()
-        else:
-            self.telescope = Telescope.from_name(telescope, verbose=verbose)
-        self.catalogs = {}
-
-    def _get_data_header(self, fitspath):
-        """Retrieve data and metadata from an image
-        """
-        if isinstance(fitspath, (str, Path)):
-            self.path = fitspath
-            self.data = fits.getdata(self.path).astype(float)
-            self.header = fits.getheader(self.path)
+            if "computed" in self.__dict__:
+                self.computed[name] = value
+            else:
+                super().__setattr__(name, value)
 
+    def __getattr__(self, name):
+        if "computed" not in self.__dict__:
+            super.__getattr__(self, name)
         else:
-            raise ValueError("fitspath must be str or None")
+            if name in self.computed:
+                return self.computed[name]
+            else:
+                raise AttributeError(f"{name} cannot be interpreted as Image attribute")
 
     def copy(self, data=True):
         """Copy of image object
 
         Parameters
         ----------
         data : bool, optional
             whether to copy data, by default True
 
         Returns
         -------
         Image
             copied object
         """
-        d = self.__dict__.copy()
-        d["telescope"] = self.telescope.name
-        new_self = self.__class__(**d)
-        new_self.data = new_self.data.copy()
-        new_self.header = new_self.header.copy()
-        new_self.catalogs = self.catalogs.copy()
-        new_self.sources = self.sources.copy()
-        if not data:
-            del new_self.__dict__["data"]
-
+        new_self = deepcopy(self)
         return new_self
 
-    def _check_telescope(self):
-        """Instantiate ``self.telescope`` from ``INSTRUME`` and or ``TELESCOP`` keywords
-        """
-        if self.header:
-           self.telescope = Telescope.from_names(
-               self.header.get("INSTRUME", ""), 
-               self.header.get("TELESCOP", ""), 
-               verbose=self.verbose
-            )
-
-    def get(self, key, default=None):
-        """Return corresponding value from header, similar to ``dict.get``
-
-        Parameters
-        ----------
-        key : str
-        default : any, optional
-            value to return if key not in ``Image.header``, by default None
-        """
-        return self.header.get(key, default)
-
-    @property
-    def wcs(self):
-        """astropy.wcs.WCS object associated with the FITS ``Image.header``
-        """
-        return WCS(self.header)
-
-    @wcs.setter
-    def wcs(self, new_wcs):
-        self.header.update(new_wcs.to_header())
-
-    # backward compatibility
-    # ----------------------
-    # TODO: handle SkyCoords input
-
-    @property
-    def stars_coords(self):
-        """Image sources pixel coordinates
-
-        Returns
-        -------
-        np.ndarray
-            coords 
-        """
-        return np.array([s.coords for s in self.sources])
-
-    @stars_coords.setter
-    def  stars_coords(self, coords):
-        """Set Image sources pixel coordinates
-        """
-        self.sources = np.array([PointSource(coords=s) for s in coords])
-
-    @property 
-    def peaks(self):
-        return np.array([s.peak for s in self.sources])
-
-    @peaks.setter
-    def peaks(self, peaks):
-        """Image sources peak values in ADUs
-
-        Returns
-        -------
-        np.array
-        """
-        for i, p in enumerate(peaks):
-            self.sources[i].peak = p
-    # ----------------------
-
-    @property
-    def exposure(self):
-        """Image exposure time in seconds
-
-        Returns
-        -------
-        astropy.units.quantity.Quantity
-        """
-        return self.get(self.telescope.keyword_exposure_time, None) * u.s
-
-    @property
-    def jd_utc(self):
-        """JD UTC time of the observation
-
-        Returns
-        -------
-        astropy.time.Time
-        """
-        # if jd keyword not in header compute jd from date
-        if self.telescope.keyword_jd in self.header:
-            jd = self.get(self.telescope.keyword_jd, None) + self.telescope.mjd
-        else:
-            jd = Time(self.date, scale="utc").to_value('jd') + self.telescope.mjd
-
-        return Time(
-            jd,
-            format="jd",
-            scale=self.telescope.jd_scale,
-            location=self.telescope.earth_location).utc.value
-
-    @property
-    def bjd_tdb(self):
-        """BJD TDB time of the observation
-
-        Returns
-        -------
-        astropy.time.Time
-        """
-        jd_bjd = self.get(self.telescope.keyword_bjd, None)
-        if jd_bjd is not None:
-            jd_bjd += self.telescope.mjd
-
-            if self.telescope.keyword_jd in self.header:
-                time_format = "bjd"
-            else:
-                time_format = "jd"
-
-            return Time(jd_bjd,
-                        format=time_format,
-                        scale=self.telescope.jd_scale,
-                        location=self.telescope.earth_location).tdb.value
-
-        else:
-            return None
-
-    @property
-    def seeing(self):
-        """Seeing of the image as written is header
-        """
-        return self.get(self.telescope.keyword_seeing, None)
-
-    @property
-    def ra(self):
-        """RA of the image as written in header
-
-        Returns
-        -------
-        astropy.coordinates.angles.Angle
-        """
-        _ra = self.get(self.telescope.keyword_ra, None)
-        if _ra is not None:
-            _ra = Angle(_ra, self.telescope.ra_unit).to(u.deg)
-        return _ra
-
-    @property
-    def dec(self):
-        """DEC of the image as written in header
-
-        Returns
-        -------
-        astropy.coordinates.angles.Angle
-        """
-        _dec = self.get(self.telescope.keyword_dec, None)
-        if _dec is not None:
-            _dec = Angle(_dec, self.telescope.dec_unit).to(u.deg)
-        return _dec
-
-    @property
-    def flip(self):
-        """Telescope flip as written in image header
-        """
-        return self.get(self.telescope.keyword_flip, None)
-
-    @property
-    def airmass(self):
-        """Observation airmass as written in image header
-        """
-        return self.get(self.telescope.keyword_airmass, None)
-
-    @property
-    def shape(self):
-        """Shape of the image data np.ndarray
-
-        Returns
-        -------
-        2D tuple
-        """
-        return np.array(self.data.shape)
-
-    @property
-    def date(self):
-        """datetime of the observation
-
-        Returns
-        -------
-        datetime.datetime
-        """
-        return dparser.parse(self.header[self.telescope.keyword_observation_date])
-
-    @property
-    def night_date(self):
-        """date of the night when night started.
-
-        Returns
-        -------
-        datetime.date
-        """
-        # TODO: do according to last astronomical twilight?
-        return (dparser.parse(self.header[self.telescope.keyword_observation_date]) - timedelta(hours=15)).date()
-
-    @property
-    def label(self):
-        """A conveniant {Telescope}_{Date}_{Object}_{Filter} string
-
-        Returns
-        -------
-        str
-        """
-        return "_".join([
-            self.telescope.name,
-            self.night_date.strftime("%Y%m%d"),
-            self.object,
-            self.filter
-        ])
-
-    @property
-    def object(self):
-        return self.header.get(self.telescope.keyword_object, "?")
+    def __copy__(self):
+        return self.copy()
 
-    @property
-    def filter(self):
-        """Observation filter as written in image header
-        """
-        return self.header.get(self.telescope.keyword_filter, None)
-    
-    def show(self, 
-        cmap="Greys_r", 
-        ax=None, 
-        figsize=(10,10), 
-        stars=True, 
+    def show(
+        self,
+        cmap="Greys_r",
+        ax=None,
+        figsize=8,
         zscale=True,
         frame=False,
         contrast=0.1,
-        **kwargs
-        ):
+        sources=True,
+        **kwargs,
+    ):
         """Show image data
 
         Parameters
         ----------
         cmap : str, optional
             matplotlib colormap, by default "Greys_r"
         ax : subplot, optional
@@ -370,15 +154,15 @@
         See also
         --------
         show_cutout :
             Show a specific star cutout
         plot_catalog :
             Plot catalog stars on an image
         plot_circle :
-            Plot circle with radius in astronomical units  
+            Plot circle with radius in astronomical units
         """
         if ax is None:
             if not isinstance(figsize, (list, tuple)):
                 if isinstance(figsize, (float, int)):
                     figsize = (figsize, figsize)
                 else:
                     raise TypeError("figsize must be tuple or list or float or int")
@@ -386,291 +170,604 @@
             if frame:
                 ax = fig.add_subplot(111, projection=self.wcs)
             else:
                 ax = fig.add_subplot(111)
 
         if zscale is False:
             vmin = np.nanmedian(self.data)
-            vmax = vmax = vmin*(1+contrast)/(1-contrast)
-            _ = ax.imshow(self.data, cmap=cmap, origin="lower",vmin=vmin,vmax=vmax, **kwargs)
+            vmax = vmax = vmin * (1 + contrast) / (1 - contrast)
+            _ = ax.imshow(
+                self.data, cmap=cmap, origin="lower", vmin=vmin, vmax=vmax, **kwargs
+            )
         else:
-            _ = ax.imshow(utils.z_scale(self.data, contrast), cmap=cmap, origin="lower", **kwargs)
-        
-        if stars:
-            self.plot_sources()
+            _ = ax.imshow(
+                utils.z_scale(self.data, contrast), cmap=cmap, origin="lower", **kwargs
+            )
 
         if frame:
             overlay = ax.get_coords_overlay(self.wcs)
-            overlay.grid(color='white', ls='dotted')
-            overlay[0].set_axislabel('Right Ascension (J2000)')
-            overlay[1].set_axislabel('Declination (J2000)')
-
-        return ax
-
-    def plot_sources(self, ax=None, **kwargs):
-        if len(self.sources) > 0:
-            if ax is None:
-                ax = plt.gca()
-            xlim, ylim = np.array(ax.get_xlim()), np.array(ax.get_ylim())
-            xlim.sort()
-            ylim.sort()
-            x, y = self.stars_coords.T
-            within = np.argwhere(np.logical_and.reduce([xlim[0] < x,  x < xlim[1],  ylim[0] < y,  y < ylim[1]])).flatten()
-            
-            for i in within:
-                self.sources[i].plot(**kwargs)
-
-            ax.set_xlim(xlim)
-            ax.set_ylim(ylim)
-
-    def show_cutout(self, star=None, size=200, **kwargs):
-        """Show a zoomed cutout around a detected star or coordinates
+            overlay.grid(color="white", ls="dotted")
+            overlay[0].set_axislabel("Right Ascension (J2000)")
+            overlay[1].set_axislabel("Declination (J2000)")
+
+        if sources:
+            if self.sources is not None:
+                self.sources.plot()
+
+        ax.set_xlim(0, self.shape[1] - 1)
+        ax.set_ylim(0, self.shape[0] - 1)
+        self._wcs = None
+
+    def _from_metadata_with_unit(self, name):
+        unit_name = f"{name}_unit"
+        value = self.metadata[name]
+        unit = str_to_astropy_unit(self.metadata[unit_name])
+        if name in ["ra", "dec"]:
+            return Angle(value, unit).to(u.deg)
+        if value is not None:
+            return value * unit
+        else:
+            return None
 
-        Parameters
-        ----------
-        star : [type], optional
-            detected star id or (x, y) coordinate, by default None
-        size : int, optional
-            side size of square cutout in pixel, by default 200
-        **kwargs passed to self.show
-        """
-
-        if star is None:
-            x, y = self.stars_coords[self.target]
-        elif isinstance(star, int):
-            x, y = self.stars_coords[star]
-        elif isinstance(star, (tuple, list, np.ndarray)):
-            x, y = star
+    @property
+    def shape(self):
+        return np.array(self.data.shape)
+
+    @property
+    def ra(self):
+        """Right-Ascension as an astropy Quantity"""
+        return self._from_metadata_with_unit("ra")
+
+    @property
+    def dec(self):
+        """Declination as an astropy Quantity"""
+        return self._from_metadata_with_unit("dec")
+
+    @property
+    def exposure(self):
+        """Exposure time as an astropy Quantity"""
+        if "exposure" in self.metadata:
+            return self._from_metadata_with_unit("exposure")
         else:
-            raise ValueError("star type not understood")
+            return None
 
-        self.show(stars=False, **kwargs)
-        plt.xlim(np.array([-size / 2, size / 2]) + x)
-        plt.ylim(np.array([-size / 2, size / 2]) + y)
-        self.plot_sources()
+    @property
+    def jd(self):
+        return self.metadata["jd"]
 
     @property
-    def skycoord(self):
-        """astropy SkyCoord object based on header RAn, DEC
-        """
-        return SkyCoord(self.ra, self.dec, frame='icrs')
+    def pixel_scale(self):
+        """Pixel scale (or plate scale) as an astropy Quantity"""
+        return self._from_metadata_with_unit("pixel_scale")
 
+    @property
+    def filter(self):
+        """Filter name"""
+        return self.metadata["filter"]
 
     @property
     def fov(self):
         """RA-DEC field of view of the image in degrees
 
         Returns
         -------
         astropy.units Quantity
         """
         return np.array(self.shape)[::-1] * self.pixel_scale.to(u.deg)
 
     @property
-    def pixel_scale(self):
-        """Pixel scale (or plate scale) in arcseconds
+    def date(self):
+        """datetime of the observation
 
         Returns
         -------
-        astropy.units Quantity
+        datetime.datetime
         """
-        return self.telescope.pixel_scale.to(u.arcsec)
+        return dparser.parse(self.metadata["date"])
 
-    def plot_aperture(self, center, arcmin=2.5):
-        """Plot an aperture with radius defined in arcmin
+    @property
+    def night_date(self):
+        """date of the night when night started.
 
-        must be over :py:class:`Image.show` or :py:class:`Image.show_cutout` plot)
+        Returns
+        -------
+        datetime.date
+        """
+        # TODO: do according to last astronomical twilight?
+        return (self.date - timedelta(hours=15)).date()
+
+    def set(self, name: str, value):
+        """Set a computed value
 
         Parameters
         ----------
-        center : int or tuple-like
-            center of the aperture
-            - if int: index of ``Image.stars_coords`` serving as center
-        arcmin : float, optional
-            radius of the aperture in arcminutes, by default 2.5
+        name : str
+            name of the computed value
+        value : any
+            value to set
         """
-        if isinstance(center, int):
-            x, y = self.stars[center]
-        elif isinstance(center, (tuple, list, np.ndarray)):
-            x, y = center
+        self.computed[name] = value
+
+    def get(self, name):
+        return self.computed[name]
+
+    @property
+    def sources(self):
+        """Image sources.
+
+        Returns
+        -------
+        prose.core.source.Sources
+        """
+        return self._sources
+
+    @sources.setter
+    def sources(self, new_sources):
+        if isinstance(new_sources, Sources):
+            self._sources = new_sources
         else:
-            raise ValueError("center type not understood")
+            self._sources = Sources(np.array(new_sources))
+
+    def cutout(
+        self,
+        coords: Union[list, tuple, np.ndarray],
+        shape: Union[int, tuple],
+        wcs: bool = True,
+        sources: bool = True,
+        reset_index: bool = True,
+    ) -> Image:
+        """Return a cutout Image instance.
+
+        Parameters
+        ----------
+        coords : list, tuple, np.ndarray
+            cutout center coordinates
+        shape : tuple or int
+            The shape of the cutouts to extract. If int, shape is (shape, shape)
+        wcs : bool, optional
+            whether to compute and include cutouts WCS (takes more time), by default True
+        sources : bool, optional
+            whether to compute and include cutouts sources, by default True
+        reset_index: bool,
+            whether to reset the sources indexes, by default True
+        Returns
+        -------
+        Image
+            Image instance with data and catalogs containing cutout data and sources
+        """
+        if isinstance(shape, (int, float)):
+            shape = (shape, shape)
+
+        if isinstance(coords, int):
+            coords = self.sources.coords[coords]
+
+        new_image = astopy_Cutout2D(
+            self.data,
+            coords,
+            shape,
+            wcs=self.wcs if wcs else None,
+            fill_value=np.nan,
+            mode="partial",
+        )
+
+        # get sources
+        new_sources = []
+        if sources:
+            if len(self._sources) > 0:
+                sources_in = np.all(
+                    np.abs(self.sources.coords - coords) < np.array(shape)[::-1] / 2, 1
+                )
+                _sources = self._sources[sources_in]
+
+                for s in _sources:
+                    _s = s.copy()
+                    _s.coords = _s.coords - coords + np.array(shape)[::-1] / 2
+                    new_sources.append(_s)
+
+        image = Image(new_image.data, deepcopy(self.metadata), deepcopy(self.computed))
+        image._sources = Sources(new_sources)
+        image.wcs = new_image.wcs
+        image.origin = tuple(np.array(new_image.bbox_original).T[0][::-1])
+        image.catalogs = deepcopy(self.catalogs)
+        for name, catalog in image.catalogs.items():
+            image.catalogs[name][["x", "y"]] -= coords - np.array(shape) / 2
+            # xy = catalog[["x", "y"]].values
+            # idxs = np.all((xy - coords / 2) < np.array(shape) / 2, 1)
+            # image.catalogs[name] = catalog[idxs]
+
+        if reset_index:
+            for i, s in enumerate(image.sources):
+                s.i = i
+
+        return image
 
-        search_radius = (60 * arcmin * u.arcmin / self.pixel_scale).decompose().value
-        circle = plt.Circle((x, y), search_radius, fill=None, ec="white", alpha=0.6)
+    @property
+    def wcs(self):
+        """astropy.wcs.WCS object associated with the FITS ``Image.header``."""
+        if self._wcs is None:
+            self._wcs = WCS(self.metadata.get("wcs", None))
+        return self._wcs
+
+    @wcs.setter
+    def wcs(self, new_wcs):
+        if new_wcs is not None:
+            if isinstance(new_wcs, WCS):
+                self.metadata["wcs"] = new_wcs.to_header().tostring()
+                self._wcs = new_wcs
 
-        ax = plt.gca()
-        ax.add_artist(circle)
-        plt.annotate(f"radius {arcmin}'", xy=[x, y + search_radius + 15], color="white",
-                     ha='center', fontsize=12, va='bottom', alpha=0.6)
+    @property
+    def plate_solved(self):
+        """Return whether the image is plate solved."""
+        return self.wcs.has_celestial
+
+    def writeto(self, destination: Union[str, Path]):
+        """Write image to FITS file
+
+        Parameters
+        ----------
+        destination : Union[str, Path]
+            destination path
+        """
+        hdu = fits.PrimaryHDU(
+            data=self.data, header=fits.Header(utils.clean_header(self.header))
+        )
+        hdu.writeto(destination, overwrite=True)
+
+    @property
+    def skycoord(self):
+        """Astropy SkyCoord object based on header RAn, DEC."""
+        return SkyCoord(self.ra, self.dec, frame="icrs")
 
     def plot_catalog(self, name, color="y", label=False, n=100000):
-        """Plot catalog stars 
-        
+        """Plot catalog stars
+
         must be over :py:class:`Image.show` or :py:class:`Image.show_cutout` plot
 
         Parameters
         ----------
         name : str
             catalog name as stored in :py:class:Image.catalog`
         color : str, optional
             color of stars markers, by default "y"
         label : bool, optional
             whether to show stars catalogs ids, by default False
         n : int, optional
             number of brightest catalog stars to show, by default 100000
         """
-        assert name in self.catalogs, f"Catalog '{name}' not present, consider using ..."
-        x, y = self.catalogs[name][["x", "y"]].values[0:n].T
+        assert (
+            name in self.catalogs
+        ), f"Catalog '{name}' not present, consider using ..."
+        x, y = self.catalogs[name][["x", "y"]].values.T
         labels = self.catalogs[name]["id"].values if label else None
         viz.plot_marks(x, y, labels, color=color)
 
-    @property
-    def plate_solved(self):
-        """Return whether the image is plate solved
-        """
-        return self.wcs.has_celestial
+    def plot_model(self, data, figsize=(5, 5), cmap=None, c="C0", contour=False):
+        plt.figure(figsize=figsize)
+        axes = gridspec.GridSpec(2, 2, width_ratios=[9, 2], height_ratios=[2, 9])
+        axes.update(wspace=0, hspace=0)
 
-    def writeto(self, destination):
-        hdu = fits.PrimaryHDU(data=self.data, header=fits.Header(utils.clean_header(self.header)))
-        hdu.writeto(destination, overwrite=True)
+        # axtt = plt.subplot(gs[1, 1])
+        ax = plt.subplot(axes[1, 0])
+        axr = plt.subplot(axes[1, 1], sharey=ax)
+        axt = plt.subplot(axes[0, 0], sharex=ax)
+
+        ax.imshow(self.data, alpha=1, cmap=cmap, origin="lower")
+        if contour:
+            ax.contour(data, colors="w", alpha=0.7)
+
+        x, y = np.indices(data.shape)
+
+        axt.plot(y[0], np.mean(self.data, axis=0), c=c, label="data")
+        axt.plot(y[0], np.mean(data, axis=0), "--", c="k", label="model")
+        axt.axis("off")
+        axt.legend()
+
+        axr.plot(np.mean(self.data, axis=1), y[0], c=c)
+        axr.plot(np.mean(data, axis=1), y[0], "--", c="k")
+        axr.axis("off")
+
+    def asdict(self, image_dtype="int16", low_data=True):
+        im_dict = asdict(self.copy())
+        if low_data:
+            im_dict["data"] = utils.z_scale(im_dict["data"]) * (2**7 - 1)
+            image_dtype = "int8"
+        im_dict["data"] = im_dict["data"].astype(image_dtype)
+        return im_dict
+
+    def save(self, filepath, image_dtype="int16", low_data=True):
+        with open(filepath, "wb") as f:
+            pickle.dump(self.asdict(image_dtype=image_dtype, low_data=low_data), f)
 
-    def gaia_stars(self, world=False, inplace=True):
-        """Query gaia stars in the image  (only in >= 2.0.3)
+    @classmethod
+    def load(cls, filepath):
+        return cls(**pickle.load(open(filepath, "rb")))
+
+    def symetric_profile(self, source, binn=1.0):
+        x, y = source.coords
+        Y, X = np.indices(self.shape)
+        radii = (np.sqrt((X - x) ** 2 + (Y - y) ** 2)).flatten()
+        d, values = self.profile(radii)
+        idxs = utils.index_binning(d, binn)
+        mean = lambda x: np.array([np.mean(x[i]) for i in idxs])
+        return mean(d), mean(values)
+
+    def profile(self, d):
+        idxs = np.argsort(d)
+        _d = d[idxs]
+        pixels = self.data.flatten()
+        pixels = pixels[idxs]
+
+        return _d, pixels
+
+    def data_cutouts(
+        self, sources: Union[np.ndarray, Sources], shape: Union[int, tuple]
+    ) -> np.ndarray:
+        """Extract cutouts from image.
 
         Parameters
         ----------
-        world : bool, optional
-            wether to return coordinates as SkyCoord if inplace is False, by default False which return the pixel location of stars in image
-        inplace : bool, optional
-            wether to set set Image.stars_coords to pixel coordinates of stars instead of returning them, by default True
-        """
-        fovmax = np.max(self.fov)
-        fov = u.Quantity([fovmax, fovmax])
-        stars_radec = gaia_query(self.skycoord, fov, "ra", "dec", circular=False).to_pandas().values
-        stars_worlds = SkyCoord(*stars_radec.T, unit=("deg", "deg"))
-        stars_coords = np.array(self.wcs.world_to_pixel(stars_worlds)).T
-        
-        if not inplace:
-            if world:
-                return stars_worlds
-            else:
-                return stars_coords
-        else:
-            self.stars_coords = stars_coords
-            
-    def plot_marks(self, coordinates, label=None, ax=None, **kwargs):
-        """Plot circular marks given world coordinates (only in >= 2.0.3)
+        sources : Union[np.ndarray, Sources]
+            Coordinates (or Sources) of the cutouts centers
+        shape : Union[int, tuple]
+            Shape of the cutouts
+
+        Returns
+        -------
+        np.ndarray
+            cutouts
+        """
+        if isinstance(sources, Sources):
+            sources = sources.coords
+
+        if isinstance(shape, int):
+            shape = (shape, shape)
+
+        cutouts = []
+        for x, y in sources:
+            c = np.zeros(shape)
+            large, small = overlap_slices(self.shape, shape, (y, x))
+            c[small] = self.data[large]
+            cutouts.append(c)
+
+        return np.array(cutouts)
+
+    def major_profile(self, source, binn=1.0, debug=False):
+        p1 = source.coords[:, None, None]
+        p2 = (source.vertexes[0])[:, None, None]
+        Y, X = np.indices(self.data.shape)
+        p3 = np.array([X, Y])
+
+        # projection
+        # https://stackoverflow.com/questions/61341712/calculate-projected-point-location-x-y-on-given-line-startx-y-endx-y
+        l2 = np.sum((p1 - p2) ** 2)
+        assert l2 != 0, "p1 and p2 are the same points"
+        distances = np.sum((p3 - p1) * (p2 - p1), 0) / np.sqrt(l2)
+        flat_distance = distances.flatten()
+        idxs = utils.index_binning(flat_distance, binn)
+        distance = np.array([flat_distance[i].mean() for i in idxs])
+        values = np.array([np.nanmax(self.data.flatten()[i]) for i in idxs])
+
+        if debug:
+            D = np.zeros(self.data.flatten().shape)
+            for i, j in enumerate(idxs):
+                D[j] = i
+            plt.figure()
+            plt.imshow(np.reshape(D, self.shape), origin="lower")
+
+        return distance, values
+
+    @property
+    def label(self):
+        """A conveniant {Telescope}_{Date}_{Object}_{Filter} string
+
+        Returns
+        -------
+        str
+        """
+        return "_".join(
+            [
+                self.metadata["telescope"],
+                self.night_date.strftime("%Y%m%d"),
+                self.metadata["object"],
+                self.filter,
+            ]
+        )
+
+
+def str_to_astropy_unit(unit_string):
+    return u.__dict__[unit_string]
+
+
+def FITSImage(
+    filepath_or_hdu: Union[str, Path, _BaseHDU],
+    verbose: bool = False,
+    load_units: bool = True,
+    load_data: bool = True,
+    telescope: Telescope = None,
+) -> Image:
+    """Create an image from a FITS file
+
+    Parameters
+    ----------
+    filepath_or_hdu : str
+        path of fits file of HDU object
+    verbose : bool, optional
+        whether to be verbose, by default False
+    load_units : bool, optional
+        whether to load metadata units, by default True
+    load_data : bool, optional
+        whether to load image data, by default True
+
+    Returns
+    -------
+    :py:class:`~prose.Image`
+    """
+    if isinstance(filepath_or_hdu, (str, Path)):
+        values = fits.getdata(filepath_or_hdu).astype(float) if load_data else None
+        header = fits.getheader(filepath_or_hdu)
+        path = filepath_or_hdu
+    elif issubclass(type(filepath_or_hdu), _BaseHDU):
+        values = filepath_or_hdu.data
+        header = filepath_or_hdu.header
+        path = None
+    else:
+        raise ValueError("filepath must be a str")
+
+    if telescope is None:
+        telescope = Telescope.from_names(
+            header.get("INSTRUME", ""), header.get("TELESCOP", ""), verbose=verbose
+        )
+
+    metadata = {
+        "telescope": telescope.name,
+        "exposure": header.get(telescope.keyword_exposure_time, None),
+        "ra": header.get(telescope.keyword_ra, None),
+        "dec": header.get(telescope.keyword_dec, None),
+        "filter": header.get(telescope.keyword_filter, None),
+        "date": telescope.date(header).isoformat(),
+        "jd": header.get(telescope.keyword_jd, None),
+        "object": header.get(telescope.keyword_object, None),
+        "pixel_scale": telescope.pixel_scale,
+        "overscan": telescope.trimming[::-1],
+        "path": path,
+        "dimensions": (header.get("NAXIS1", 1), header.get("NAXIS2", 1)),
+        "type": telescope.image_type(header),
+    }
+
+    if load_units:
+        metadata.update(
+            {
+                "exposure_unit": "s",
+                "ra_unit": telescope.ra_unit,
+                "dec_unit": telescope.dec_unit,
+                "jd_scale": telescope.jd_scale,
+                "pixel_scale_unit": "arcsec",
+            }
+        )
+
+    image = Image(values, metadata, {})
+    if image.metadata["jd"] is None:
+        image.metadata["jd"] = Time(image.date).jd
+    image.fits_header = header
+    image.wcs = WCS(header)
+    image.telescope = telescope
+
+    return image
+
+
+class Buffer:
+    def __init__(self, size: int, loader: callable = None):
+        """Object to load and access adjacent items in a list
 
         Parameters
         ----------
-        coordinates : _type_
-            _description_
-        label : _type_, optional
-            _description_, by default None
-        ax : _type_, optional
-            _description_, by default None
+        size : int
+            number of items accessible
+        loader : callable, optional
+            a function that load an item in the buffer, by default None corresponding
+            to lambda x: x
 
         Example
         -------
+        .. code-block:: python
 
-        .. jupyter-execute::
+            from prose.core.image import Buffer
+            import numpy as np
 
-            from prose import archive
-            import matplotlib.pyplot as plt
+            # items to be loaded in the buffer
+            init = np.arange(0, 10)
 
-            # star coordinates
-            coord = "04 27 01.36232", "-28 12 48.21681"
+            # create and initialize
+            buffer = Buffer(size=3)
+            buffer.init(init)
+
+            for buffer in buffer:
+                print(buffer.previous, buffer.current, buffer.next)
+
+        .. code-block:: text
+
+            None 0 1
+            0 1 2
+            1 2 3
+            2 3 4
+            3 4 5
+            4 5 6
+            5 6 7
+            6 7 8
+            7 8 9
+            8 9 None
+
+        """
+        assert size % 2 == 1, "size must be odd"
+        self.mid_index = int((size - 1) // 2)
+        self.items = [None] * max(size, 1)
+        if loader is None:
+            loader = lambda item: item
+        self.loader = loader
+        self.queue = None  # items to be loaded
 
-            # getting an archival image for example
-            field_of_view = [3, 1.5] 
-            image = archive.pos1_image(coord, field_of_view)
-
-            # overplotting coord on image
-            image.show()
-            plt.title(image.date.date())
-            image.plot_marks(coord, color="k", ms=15)
-
-        """
-        
-        if len(np.shape(coordinates)) == 1:
-            coordinates = utils.check_skycoord(coordinates)
-        
-        if isinstance(coordinates, SkyCoord):
-            stars_coords = np.array(self.wcs.world_to_pixel(coordinates)).T
-        else:
-            stars_coords = coordinates
-        
-        label = np.arange(len(stars_coords)) if label is True else None
-        
-        if ax is None:
-            ax = plt.gca()
-            
-        viz.plot_marks(*stars_coords.T, label=label, ax=ax, **kwargs)
+    def __len__(self):
+        return len(self.items)
 
-    @classmethod
-    def from_telescope(cls, telescope):
-        return partial(cls, telescope=telescope)
+    def __getitem__(self, i: int):
+        """Get item by index relative to current
 
-    def plot_psf_model(self, cmap="inferno", c="blueviolet", figsize=(5, 5), axes=None):
-        
-        # Plotting
-        # --------
-        assert hasattr(self, "psf"), "PSF not present in image"
-        data = self.psf
-        model = self.psf_model
-
-        if axes is None:
-            plt.figure(figsize=figsize)
-            axes = gridspec.GridSpec(2, 2, width_ratios=[9, 2], height_ratios=[2, 9])
-            axes.update(wspace=0, hspace=0)
-            
-        #axtt = plt.subplot(gs[1, 1])
-        ax = plt.subplot(axes[1, 0])
-        axr = plt.subplot(axes[1, 1], sharey=ax)
-        axt = plt.subplot(axes[0, 0], sharex=ax)
+        Parameters
+        ----------
+        i : int
+            index
 
-        ax.imshow(self.psf, alpha=1, cmap=cmap, origin="lower")
-        ax.contour(self.psf_model, colors="w", alpha=0.7)
+        Returns
+        -------
+        Image or None
+            images[current + i]
+        """
+        return self.items[self.mid_index + i]
 
-        x, y = np.indices(data.shape)
+    def __setitem__(self, i: int, item: Image):
+        self.items[self.mid_index + i] = item
 
-        axt.plot(y[0], np.mean(data, axis=0), c=c, label="data")
-        axt.plot(y[0], np.mean(model, axis=0), "--", c="k", label="model")
-        axt.axis("off")
-        axt.legend()
+    def append(self, item):
+        """Add an item to the buffer (and delete last)
 
-        axr.plot(np.mean(data, axis=1), y[0], c=c)
-        axr.plot(np.mean(model, axis=1), y[0], "--", c="k")
-        axr.axis("off")
-        ax.text(1, 1, f"FWHM x: {self.fwhmx:.2f} pix\n"
-                    f"FWHM y: {self.fwhmy:.2f} pix\n"
-                    f"angle: {self.theta/np.pi*180:.2f}°", c="w")
-
-    def has_stars(self, error=False):
-        if not hasattr(self, "stars_coords"):
-            if error:
-                raise ValueError(f"`stars_coords` not found in Image (did you use a detection block?)")
-            return False
-        elif self.stars_coords is None:
-            if error:
-                raise ValueError(f"`stars_coords` is empty (no stars detected)")
-            return False
-        else:
-            return True
+        Parameters
+        ----------
+        item : any
+            item to be loaded
+        """
+        last_item = self.items.pop(0)
+        del last_item
+        self.items.append(item)
 
-    def enough_stars(self, n=0, error=False):
-        has = self.has_stars(error=error)
-        if has:
-            if len(self.stars_coords) == 0:
-                if error:
-                    raise ValueError(f"`stars_coords` is empty (no stars detected)")
-                return False
-
-            elif len(self.stars_coords) < n:
-                if error:
-                    raise ValueError(f"only {len(self.stars_coords)} stars detected (at least {n} needed)")
-                return False
-            else:
-                return True
-        else:
-            return False
+    def init(self, items):
+        """Prepare items to be loaded in the buffer.
+
+        The first items are loaded with the :code:`Buffer.loader` function
+
+        Parameters
+        ----------
+        items : list
+            items to be loaded in the buffer
+        """
+        for item in items[: self.mid_index]:
+            self.append(self.loader(item))
+        self.queue = [*items[self.mid_index :], *[None] * self.mid_index]
+
+    def __iter__(self):
+        for item in self.queue:
+            self.append(self.loader(item))
+            yield self
+
+    def sub(self, size, offset):
+        pass
+
+    @property
+    def previous(self):
+        return self[-1]
+
+    @property
+    def current(self):
+        return self[0]
+
+    @property
+    def next(self):
+        return self[1]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prose-2.3.0/prose/core/sequence.py` & `prose-3.0.0/prose/core/sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-from tqdm import tqdm
-from ..console_utils import TQDM_BAR_FORMAT, warning, error
+import sys
 from collections import OrderedDict
-from tabulate import tabulate
-import numpy as np
-from time import time
-from .image import Image
-from pathlib import Path
 from functools import partial
-import multiprocessing as mp
-from ..blocks.utils import DataBlock
-import sys
+from pathlib import Path
+from time import time
+
+import multiprocess as mp
+import numpy as np
 import yaml
-from ..utils import full_class_name
-from ..citations import _all_citations
+from tabulate import tabulate
+from tqdm.autonotebook import tqdm
+
+from prose.console_utils import TQDM_BAR_FORMAT, error, warning
+from prose.core.image import Buffer, FITSImage, Image
+from prose.utils import full_class_name
+
 
 def progress(name, x, **kwargs):
-    return tqdm(
-        x,
-        desc=name,
-        unit="images",
-        ncols=80,
-        bar_format=TQDM_BAR_FORMAT,
-        **kwargs
-    )
+    return tqdm(x, desc=name, unit="images", **kwargs)
+
 
 class Sequence:
     def __init__(self, blocks, name=None):
         """A sequence of :py:class:`Block` objects to sequentially process images
 
         Parameters
         ----------
         blocks : list
             list of :py:class:`Block` objects
         name : str, optional
             name of the sequence, by default None
         """
         self.name = name
         self.images = []
+        self.blocks_dict = None
         self.blocks = blocks
 
         self.data = {}
         self.n_processed_images = None
+        self.last_image = None
+
+        # initially the buffer must have a size of max(front_size) + max(back_size) in
+        # order to hold all images necessary to all blocks
+        buffer_size = np.max([block.size for block in self.blocks])
+        self.buffer = Buffer(buffer_size)
 
     def __getattr__(self, item):
         return self.blocks_dict[item]
 
     @property
     def blocks(self):
         """list of :py:class:`Block` objects
@@ -54,24 +56,26 @@
         _type_
             _description_
         """
         return list(self.blocks_dict.values())
 
     @blocks.setter
     def blocks(self, blocks):
-        self.blocks_dict = OrderedDict({
-            block.name if block.name is not None else "block{}".format(i): block
-            for i, block in enumerate(blocks)
-        })
+        self.blocks_dict = OrderedDict(
+            {
+                block.name if block.name is not None else "block{}".format(i): block
+                for i, block in enumerate(blocks)
+            }
+        )
 
     def _set_blocks_in_sequence(self, in_sequence):
         for b in self.blocks:
             b.in_sequence = in_sequence
 
-    def run(self, images, terminate=True, show_progress=True, loader=Image):
+    def run(self, images, terminate=True, show_progress=True, loader=FITSImage):
         """Run the sequence
 
         Parameters
         ----------
         images : list, str, :py:class:`Image`
             :py:class:`Image` object or path (single or as a list) to be processed by the sequence
         terminate : bool, optional
@@ -82,15 +86,18 @@
             An Image sub-class to load images path(s) of provided as inputs, by default py:class:`Image`
         """
         self._set_blocks_in_sequence(True)
         self.images = images if not isinstance(images, (str, Path, Image)) else [images]
         assert len(self.images) != 0, "Empty array or no images provided"
 
         if not show_progress:
-            def _p(x, **kwargs): return x
+
+            def _p(x, **kwargs):
+                return x
+
             self.progress = _p
         else:
             self.progress = partial(progress, self.name)
 
         if isinstance(self.images, list):
             if len(self.images) == 0:
                 raise ValueError("No images to process")
@@ -100,94 +107,100 @@
         # run
         self.n_processed_images = 0
         self.discards = {}
         self._run(loader=loader)
 
         if terminate:
             self.terminate()
-        
-        for block_name, discarded in self.discards.items():
-            warning(f"{block_name} discarded image{'s' if len(discarded)>1 else ''} {', '.join(discarded)}")
-
-    def _run(self, loader=Image):
-        for i, image in enumerate(self.progress(self.images)):
-            if isinstance(image, (str, Path)):
-                image = loader(image)
 
-            image.i = i
+        for block_name, discarded in self.discards.items():
+            warning(
+                f"{block_name} discarded image{'s' if len(discarded)>1 else ''} {', '.join(discarded)}"
+            )
+
+    def _load(self, image, loader=FITSImage):
+        _image = loader(image) if isinstance(image, (str, Path)) else image
+        return _image
+
+    def _run(self, loader=FITSImage):
+        self.buffer.loader = partial(self._load, loader=loader)
+        self.buffer.init(self.images)
+
+        for i, buffer in enumerate(self.progress(self.buffer, total=len(self.images))):
+            buffer.current.i = i
+            self.last_image = buffer.current
 
             for block in self.blocks:
-                block._run(image)
+                block._run(buffer)
                 # This allows to discard image in any Block
-                if image.discard:
-                    self._add_discard(type(block).__name__, i)
-                    break
+                if buffer.current is not None:
+                    if buffer.current.discard:
+                        self._add_discard(type(block).__name__, buffer.current.i)
+                        break
 
-            del image
             self.n_processed_images += 1
 
     def terminate(self):
-        """Run the :py:class:`Block.terminate` method of all blocks
-        """
+        """Run the :py:class:`Block.terminate` method of all blocks"""
         for block in self.blocks:
             block.terminate()
         self._set_blocks_in_sequence(False)
 
     def __str__(self):
-        rows = [[
-            i, block.name, block.__class__.__name__, f"{block.processing_time:.3f} s ({(block.processing_time/self.processing_time)*100:.0f}%)"] 
-            for i, block in enumerate(self.blocks)
+        rows = [
+            [
+                i,
+                block.name,
+                block.__class__.__name__,
+                f"{block.processing_time:.3f} s ({(block.processing_time/self.processing_time)*100:.0f}%)",
             ]
+            for i, block in enumerate(self.blocks)
+        ]
         headers = ["index", "name", "type", "processing"]
 
         return tabulate(rows, headers, tablefmt="fancy_grid")
 
     def __repr__(self) -> str:
         return self.__str__()
 
     @property
     def processing_time(self):
-        """Total processing time of the sequence last run
-        """
+        """Total processing time of the sequence last run"""
         return np.sum([block.processing_time for block in self.blocks])
 
     def __getitem__(self, item):
         return self.blocks[item]
 
     # io
     # --
 
     def _add_discard(self, discard_block, i):
         if discard_block not in self.discards:
             self.discards[discard_block] = []
         self.discards[discard_block].append(str(i))
 
-
     @property
     def args(self):
         blocks = []
-        for block in self.blocks:        
-            blocks.append({
-                'block': full_class_name(block),
-                **block.args
-            })
+        for block in self.blocks:
+            blocks.append({"block": full_class_name(block), **block.args})
 
         return blocks
 
     @classmethod
     def from_args(cls, args):
         import prose
-        
+
         blocks = []
         for block_dict in args:
             block_class = block_dict["block"]
             del block_dict["block"]
             block = eval(block_class).from_args(block_dict)
             blocks.append(block)
-            
+
         return cls(blocks)
 
     @property
     def params_str(self):
         return yaml.safe_dump(self.args, sort_keys=False)
 
     def citations(self):
@@ -202,30 +215,22 @@
 
         Example
         -------
         .. jupyter-execute::
 
             from prose import Sequence, blocks
 
-            sequence = Sequence([              
+            sequence = Sequence([
                 blocks.psf.Moffat2D(),
                 blocks.detection.LimitStars(min=3),
                 blocks.Set(stars_coords=None),
                 blocks.AffineTransform(data=False, inverse=True),
-                blocks.BalletCentroid(),                           
+                blocks.BalletCentroid(),
                 blocks.PhotutilsAperturePhotometry(scale=1.),
                 blocks.Peaks(),
-                blocks.XArray(
-                    ("time", "jd_utc"),
-                    ("time", "bjd_tdb"),
-                    ("time", "flip"),
-                    ("time", "fwhm"),
-                    ("time", "fwhmx"),
-                    name="xarray"
-                ),
             ])
 
             tex, bib = sequence.citations()
 
             print(tex)
             print(bib[0:500], "...")
         """
@@ -238,90 +243,103 @@
                 if c.strip("\n").strip(" ")[0] == "@":
                     name = c.split("{")[1].split(",")[0]
                     cites[name] = c
                 else:
                     if c in _all_citations:
                         cites[c] = _all_citations[c]
                     else:
-                        raise KeyError(f"{c} not in defautls citations, please provide it as a dict")
+                        raise KeyError(
+                            f"{c} not in defautls citations, please provide it as a dict"
+                        )
 
             elif isinstance(c, dict):
                 cites.update(c)
 
         for c in citations:
             if isinstance(c, (list, tuple)):
                 for cc in c:
                     add_citation(cc)
             else:
                 add_citation(c)
-                
-        tex_citep = ", ".join([f"{name} \citep{{{name}}}" for name in cites.keys() if name not in ["prose", "astropy"]])
+
+        tex_citep = ", ".join(
+            [
+                f"{name} \citep{{{name}}}"
+                for name in cites.keys()
+                if name not in ["prose", "astropy"]
+            ]
+        )
         tex_citep += " and astropy \citep{astropy}"
-        tex = f"This research made use of \\textsf{{prose}} \citep{{prose}} and its dependencies ({tex_citep})."""
+        tex = (
+            f"This research made use of \\textsf{{prose}} \citep{{prose}} and its dependencies ({tex_citep})."
+            ""
+        )
 
         return tex, "\n\n".join(cites.values())
 
 
-class MPSequence(Sequence):
-
-    def __init__(self, blocks, data_blocks=None, name="", loader=Image):
-        super().__init__(blocks, name=name, loader=loader)
+class SequenceParallel(Sequence):
+    def __init__(self, blocks, data_blocks=None, name=""):
+        super().__init__(blocks, name=name)
         if data_blocks is None:
             self.data = None
             self._has_data = False
         else:
             self.data = Sequence(data_blocks)
             self._has_data = True
 
     def check_data_blocks(self):
         bad_blocks = []
-        for b in self.blocks: 
-            if isinstance(b, DataBlock):
+        for b in self.blocks:
+            if b._data_block:
                 bad_blocks.append(f"{b.__class__.__name__}")
         if len(bad_blocks) > 0:
-            bad_blocks = ', '.join(list(np.unique(bad_blocks)))
-            error(f"Data blocks [{bad_blocks}] cannot be used in MPSequence\n\nConsider using the data_blocks kwargs")
+            bad_blocks = ", ".join(list(np.unique(bad_blocks)))
+            error(
+                f"Data blocks [{bad_blocks}] cannot be used in MPSequence\n\nConsider using the data_blocks kwargs"
+            )
             sys.exit()
-    
-    def _run(self, telescope=None):
+
+    def _run(self, loader=FITSImage):
         self.check_data_blocks()
 
         self.n_processed_images = 0
         n = len(self.images)
         processed_blocks = mp.Manager().list(self.blocks)
         images_i = list(enumerate(self.images))
 
         with mp.Pool() as pool:
-            for image in self.progress(pool.imap(partial(
-                _run_all,
-                blocks=processed_blocks,
-                loader=self.loader
-            ), images_i), total=n):
+            for image in self.progress(
+                pool.imap(
+                    partial(_run_all, blocks=processed_blocks, loader=loader), images_i
+                ),
+                total=n,
+            ):
                 if not image.discard:
                     if self._has_data:
                         self.data.run(image, terminate=False, show_progress=False)
                 else:
                     self._add_discard(image.discard_block, image.i)
 
     def terminate(self):
         if self._has_data:
             self.data.terminate()
 
-def _run_all(image_i, blocks=None, loader=None):
 
+def _run_all(image_i, blocks=None, loader=None):
     i, image = image_i
 
     if isinstance(image, (str, Path)):
         image = loader(image)
-    
+
     image.i = i
 
     for block in blocks:
         # This allows to discard image in any Block
         if image.discard:
             return image
         else:
             block._run(image)
             if image.discard:
                 image.discard_block = type(block).__name__
 
-    return image
+    return image
```

### Comparing `prose-2.3.0/prose/core/source.py` & `prose-3.0.0/prose/fluxes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,459 +1,568 @@
-from matplotlib.patches import Ellipse, Circle
-from photutils.aperture import *
-from photutils.isophote import EllipseGeometry
-from photutils.isophote import Ellipse as IsoEllipse
-import numpy as np
+import pickle
+import warnings
+from copy import deepcopy
+from dataclasses import asdict, dataclass
+from pathlib import Path
+from typing import Union
+
 import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
 
-color = [0.51, 0.86, 1.]
+from prose import utils
 
-def distance(p1, p2):
-    return np.sqrt(np.power(p1[0] - p2[0], 2) + np.power(p1[1] - p2[1], 2))
 
-def clean_stars_positions(positions, tolerance=50):
-    keep = []
+def binned_white_function(x, bins: int = 12):
+    # set binning idxs for white noise evaluation
+    bins = np.min([x.shape[-1], bins])
+    n = x.shape[-1] // bins
+    idxs = np.arange(n * bins)
 
-    distance_to_others = np.array(
-        [[distance(v, w) for w in positions] for v in positions]
-    )
-    for i, _distances in enumerate(distance_to_others):
-        _distances[i] = np.inf
-        close_stars = np.flatnonzero(_distances < tolerance)
-        if len(close_stars) == 0:
-            keep.append(i)
-
-    return np.unique(keep)
-    
-class Source:
-    def __init__(self, region=None, coords=None, peak=0, i=None):
-        """Representation of a source in an image
+    def compute(f):
+        return np.nanmean(
+            np.nanstd(np.array(np.split(f.take(idxs, axis=-1), n, axis=-1)), axis=-1),
+            axis=0,
+        )
 
-        Parameters
-        ----------
-        region : skimage.measure.RegionProperties, optional
-            An skimage RegionProperties containing the source, by default None. Only one of 'coords' or 'region' must be provided
-        coords : array, optional
-            Pixel coordinates of the source, by default None. Only one of 'coords' or 'region' must be provided
-        peak : float, optional
-            maximum pixel value of the source, by default 0
-        i : int, optional
-            index identifier of the source, by default None
-        """
-        # assert (region is not None) or (coords is not None), "One of 'coords' or 'region' must be provided"
-        # if (region is not None) and (coords is not None):
-        #     AssertionError("Only one of 'coords' or 'region' must be provided")
-        # if (region is not None) and (peak != 0):
-        #     AssertionError("Providing 'peak' has no effect when 'region' is provided")
-
-        if region is not None:
-            self.a = region.axis_major_length
-            self.b = region.axis_minor_length
-            self.orientation = region.orientation
-            self.coords = np.array(region.centroid_weighted[::-1])
-            self.peak = region.intensity_max
+    return compute
+
+
+def weights(
+    fluxes: np.ndarray, tolerance: float = 1e-3, max_iteration: int = 200, bins: int = 5
+):
+    """Returns the weights computed using Broeg 2005
+
+    Parameters
+    ----------
+    fluxes : np.ndarray
+        fluxes matrix with dimensions (star, flux) or (aperture, star, flux)
+    tolerance : float, optional
+        the minimum standard deviation of weights difference to attain (meaning weights are stable), by default 1e-3
+    max_iteration : int, optional
+        maximum number of iterations to compute weights, by default 200
+    bins : int, optional
+        binning size (in number of points) to compute the white noise, by default 5
+
+    Returns
+    -------
+    np.ndarray
+        Broeg weights
+    """
+
+    # normalize
+    dfluxes = fluxes / np.expand_dims(np.nanmean(fluxes, -1), -1)
+    binned_white = binned_white_function(fluxes, bins=bins)
+
+    i = 0
+    evolution = 1e25
+    lcs = None
+    weights = None
+    last_weights = np.zeros(dfluxes.shape[0 : len(dfluxes.shape) - 1])
+
+    # Broeg 2004 algorithm to find weights of comp stars
+    # --------------------------------------------------
+    while evolution > tolerance and i < max_iteration:
+        if i == 0:
+            weights = 1 / binned_white(dfluxes)
         else:
-            self.a = 1.
-            self.b = 1.
-            self.orientation = 0.
-            self.coords = coords
-            self.peak = peak
-
-        self.i = i
-        self.discarded = False
-        self._region = region
+            # This metric is preferred from std to optimize over white noise and not red noise
+            std = binned_white(lcs)
+            weights = 1 / std
+
+        weights[~np.isfinite(weights)] = 0
+
+        # Keep track of weights
+        evolution = np.nanstd(
+            np.abs(np.nanmean(weights, axis=-1) - np.nanmean(last_weights, axis=-1))
+        )
 
-    @property
-    def vertexes(self):
-        """Coordinates of the Ellipse vertexes, endpoints of the major axis
+        last_weights = weights
+        lcs = diff(dfluxes, weights=weights)
+        i += 1
+
+    return weights
+
+
+def diff(fluxes: np.ndarray, weights: np.ndarray = None):
+    """Returns differential fluxes.
+
+    If weights are specified, they are used to produce an artificial light curve by which all flux are differentiated (see Broeg 2005)
+
+    Parameters
+    ----------
+    fluxes : np.ndarray
+        fluxes matrix with dimensions (star, flux) or (aperture, star, flux)
+    weights :np.ndarray, optional
+        weights matrix with dimensions (star) or (aperture, star), by default None which simply returns normalized fluxes
+
+    Returns
+    -------
+    np.ndarray
+        Differential fluxes if weights is provided, else normalized fluxes
+    """
+    diff_fluxes = fluxes / np.expand_dims(np.nanmean(fluxes, -1), -1)
+    if weights is not None:
+        # not to divide flux by itself
+        sub = np.expand_dims((~np.eye(fluxes.shape[-2]).astype(bool)).astype(int), 0)
+        weighted_fluxes = diff_fluxes * np.expand_dims(weights, -1)
+        # see broeg 2005
+        artificial_light_curve = (sub @ weighted_fluxes) / np.expand_dims(
+            weights @ sub[0], -1
+        )
+        diff_fluxes = diff_fluxes / artificial_light_curve
+    return diff_fluxes
 
-        Returns
-        -------
-        np.array
-            vertexes coordinates
-        """
-        x0, y0 = self.coords
-        theta = self.orientation
-        x1 = x0 - np.sin(np.pi+theta) * 0.5 * self.a
-        y1 = y0 - np.cos(np.pi+theta) * 0.5 * self.a
-        x2 = x0 - np.sin(theta) * 0.5 * self.a
-        y2 = y0 - np.cos(theta) * 0.5 * self.a
 
-        return np.array([x1, y1]), np.array([x2, y2])
+def auto_diff_1d(fluxes, i=None):
+    dfluxes = fluxes / np.expand_dims(np.nanmean(fluxes, -1), -1)
+    w = weights(dfluxes)
+    if i is not None:
+        idxs = np.argsort(w)[::-1]
+        white_noise = binned_white_function(dfluxes)
+        last_white_noise = 1e10
+
+        def best_weights(j):
+            _w = w.copy()
+            _w[idxs[j::]] = 0.0
+            _w[i] = 0.0
+            return _w
+
+        for j in range(w.shape[-1]):
+            _w = best_weights(j)
+            _df = diff(dfluxes, _w)
+            _white_noise = np.take(white_noise(_df), i, axis=-1)[0]
+            if not np.isfinite(_white_noise):
+                continue
+            if _white_noise < last_white_noise:
+                last_white_noise = _white_noise
+            else:
+                break
+
+        w = best_weights(j - 1)
+
+    df = diff(dfluxes, w)
+
+    return df.reshape(fluxes.shape), w
+
+
+def auto_diff(fluxes: np.array, i: int = None):
+    if fluxes.ndim == 3:
+        auto_diffs = [auto_diff_1d(f, i) for f in fluxes]
+        w = [a[1] for a in auto_diffs]
+        fluxes = np.array([a[0] for a in auto_diffs])
+        return fluxes, np.array(w)
+    else:
+        return auto_diff_1d(fluxes, i)
+
+
+def optimal_flux(diff_fluxes, method="stddiff", sigma=4):
+    fluxes = diff_fluxes.copy()
+    fluxes = fluxes[
+        ...,
+        np.all(
+            (fluxes - np.median(fluxes, 1)[..., None])
+            < sigma * np.std(fluxes, 1)[..., None],
+            0,
+        ),
+    ]
+    if method == "binned":
+        white_noise = binned_white_function(fluxes)
+        criterion = white_noise(fluxes)
+    elif method == "stddiff":
+        criterion = utils.std_diff_metric(fluxes)
+    elif method == "stability":
+        criterion = utils.stability_aperture(fluxes)
+    else:
+        raise ValueError("{} is not a valid method".format(method))
+
+    i = np.argmin(criterion)
+    return i
+
+
+@dataclass
+class Fluxes:
+    """Photometric fluxes, from single to multiple stars and apertures.
+
+    Also hold contemporary time-series, errors and apertures properties.
+    """
+
+    fluxes: np.ndarray
+    """Fluxes either as 1, 2, or 3 dimensional arrays, with following dimensions
+        - 1: (time)
+        - 2: (star, time)
+        - 3: (aperture, star, time)
+    """
+    time: np.ndarray = None
+    """Array of observed time"""
+    errors: np.ndarray = None
+    """Errors with same shape as :code:`fluxes`"""
+    data: dict = None
+    """A dict of data time-series, each with the same shape as :code:`time`"""
+    apertures: np.ndarray = None
+    """Apertures radii"""
+    weights: np.ndarray = None
+    """Fluxes weights (from differential photometry)"""
+    target: int = None
+    """Index of selected target"""
+    aperture: int = None
+    """Index of selected aperture"""
+    metadata: dict = None
 
     @property
-    def co_vertexes(self):
-        """Coordinates of the Ellipse co-vertexes, endpoints of the minor axis
+    def _is_target_aperture_set(self):
+        """Check if target and aperture are set depending on `fluxes` dimensions.
 
         Returns
         -------
-        np.array
-            co-vertexes coordinates
+        bool
+            whether target and aperture are set
         """
-        x0, y0 = self.coords
-        theta = self.orientation + np.pi/2
-        x1 = x0 - np.sin(np.pi+theta) * 0.5 * self.b
-        y1 = y0 - np.cos(np.pi+theta) * 0.5 * self.b
-        x2 = x0 - np.sin(theta) * 0.5 * self.b
-        y2 = y0 - np.cos(theta) * 0.5 * self.b
+        if self.ndim == 1:
+            return True
+        if self.ndim == 2:
+            return self.target is not None
+        else:
+            return self.target is not None and self.aperture is not None
 
-        return np.array([x1, y1]), np.array([x2, y2])
+    def __post_init__(self):
+        assert self.fluxes.ndim in [1, 2, 3], "fluxes must be 1, 2 or 3 dimensional"
+        if self.data is None:
+            self.data = {}
+        if self.ndim == 1:
+            self.target = 0
+            self.aperture = 0
+            self.fluxes = self.fluxes.copy()[None, None, :]
+            if self.errors is not None:
+                self.errors = self.errors.copy()[None, None, :]
+        elif self.ndim == 2:
+            self.aperture = 0
+            self.fluxes = self.fluxes.copy()[None, :]
+            if self.errors is not None:
+                self.errors = self.errors.copy()[None, :]
+        if self.metadata is None:
+            self.metadata = {}
+
+    def _target_attr(self, name, full=False):
+        assert self.__dict__[name] is not None, f"{name} not provided"
+        assert self.target is not None, "target must be set"
+        if full:
+            return self.__dict__[name][:, self.target]
+        else:
+            assert self.aperture is not None, "aperture must be set"
+            return self.__dict__[name][self.aperture, self.target]
 
-    def copy(self):
-        """Return a copy of the Source
+    @property
+    def flux(self) -> np.array:
+        """Main flux
 
         Returns
         -------
-        Source
-            copy
+        np.array
+            Main flux
         """
-        copy = self.__class__()
-        copy.a = self.a
-        copy.b = self.b
-        copy.peak = self.peak
-        copy.orientation = self.orientation
-        copy.i = self.i
-        copy.coords = self.coords
-        return copy
+        return self._target_attr("fluxes")
 
-    
-    def plot_circle(self, radius, c=color, ax=None, label=True, fontsize=12, **kwargs):
-        """Plot a circle centered on source
+    @property
+    def error(self) -> np.array:
+        return self._target_attr("errors")
 
-        Parameters
-        ----------
-        radius : float
-            radii of the circle in pixels
-        c : str, optional
-            color of the circle, by default color
-        ax : Axe, optional
-            pyplot axe in which to plot the circle, by default None
-        label : bool, optional
-            whether to display the Source.i index, by default True
-        fontsize : int, optional
-            Font size for the source index, by default 12
-        """
-        if ax is None:
-            ax = plt.gca()
-        circle = Circle(self.coords, radius, fill=None, ec=c, **kwargs)
-        ax.add_artist(circle)
-        if label and self.i is not None:
-            plt.text(*(np.array(self.coords) - [0, 1.5*radius]), self.i, c=c, ha="center", va="top", fontsize=fontsize)
-        
-    def plot_ellipse(self, n=10, c=color, ax=None, label=True, fontsize=12, **kwargs):
-        """Plot an ellipse centered on source, with semi-major/minor length defined by the source itself 
+    @property
+    def shape(self):
+        return self.fluxes.shape
 
-        Parameters
-        ----------
-        n : float
-            offset added to the major and minor axis (major axis of the plotted ellipse will be `Source.a + n`)
-        c : str, optional
-            color of the circle, by default color
-        ax : Axe, optional
-            pyplot axe in which to plot the circle, by default None
-        label : bool, optional
-            whether to display the Source.i index, by default True
-        fontsize : int, optional
-            Font size for the source index, by default 12
-        """
-        if ax is None:
-            ax = plt.gca()
+    @property
+    def ndim(self):
+        return self.fluxes.ndim
 
-        ax = plt.gca()
-        e = Ellipse(
-            xy=self.coords,
-            width=n + self.b,
-            height=n + self.a,
-            angle=-self.orientation * 180. / np.pi,
-            **kwargs
-        )
-        e.set_facecolor('none')
-        e.set_edgecolor(c)
-        ax.add_artist(e) 
-    
-        if label and self.i is not None:
-            rad = np.pi/2 + self.orientation
-            label_coord = self.coords + [0, -(np.abs(self.a*rad/2) + self.b/2)]
-            plt.text(*label_coord, self.i, c=c, ha="center", va="top", fontsize=fontsize)
-
-    def circular_aperture(self, r, scale=True):
-        """`photutils.aperture.CircularAperture` centered on the source
+    def vander(consant=True, **kwargs):
+        pass
+
+    def diff(self, comps: np.ndarray = None):
+        """Differential photometry
 
         Parameters
         ----------
-        r : float
-            radius
-        scale : bool, optional
-            whether to scale r to Source.a, by default True
+        comps : np.ndarray, optional
+            index of comparison stars, by default None
 
         Returns
         -------
-        photutils.aperture.CircularAperture
+        differential :code:`Fluxes`
         """
-        if scale:
-            radius = r*self.a
+        if comps is not None:
+            weights = np.zeros(self.fluxes[0:2])
+            weights[:, comps] = 1
         else:
-            radius = r
-        return CircularAperture(self.coords, radius)
+            weights = None
 
-    def elliptical_aperture(self, r, scale=True):
-        """`photutils.aperture.EllipticalAperture` centered on the source
+        diff_fluxes = diff(self.fluxes, weights)
+        _new = deepcopy(self)
+        _new.fluxes = diff_fluxes
+        _new.weights = weights
+        return _new
 
-        Parameters
-        ----------
-        r : float
-            semi-major axis of the aperture. Semi minor will be `r*Source.b/Source.a`
-        scale : bool, optional
-            whether to scale r to Source.a, by default True
+    def autodiff(self):
+        """Automatic differential photometry with Broeg et al. 2005
 
         Returns
         -------
-        photutils.aperture.CircularAperture
+        differential :code:`Fluxes`
         """
-        if scale:
-            _a, _b = r*self.a, r*self.b
-        else:
-            _a, _b = r, r*self.b/self.a
-        return EllipticalAperture(self.coords, _a, _b, np.pi/2-self.orientation)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", RuntimeWarning)
+            diff_fluxes, weights = auto_diff(self.fluxes, self.target)
 
-    def rectangular_aperture(self, r, scale=True):
-        if scale:
-            _a, _b = r*self.a, r*self.b
-        else:
-            _a, _b = r, r*self.b/self.a
-        return RectangularAperture(self.coords, _a, _b, np.pi/2-self.orientation)
+        _new = deepcopy(self)
+        _new.fluxes = diff_fluxes
+        _new.weights = weights
+        _new.aperture = _new.best_aperture_index()
 
-    def circular_annulus(self, r0, r1, scale=False):
-        if scale:
-            _r0 = r0*self.a
-            _r1 = r1*self.a
-        else:
-            _r0 = r0
-            _r1 = r1
-        return CircularAnnulus(self.coords, _r0, _r1)
-
-    def elliptical_annulus(self, r0, r1, scale=False):
-        if scale:
-            _a0, _b0 = r0*self.a, r0*self.b
-            _a1, _b1 = r1*self.a, r1*self.b
-        else:
-            _a0, _b0 = r0, r0*self.b/self.a
-            _a1, _b1 = r1, r1*self.b/self.a
-        return EllipticalAnnulus(self.coords, _a0, _a1, _b1, theta=np.pi/2-self.orientation)
-
-    def rectangular_annulus(self, r0, r1, scale=False):
-        if scale:
-            _a0, _b0 = r0*self.a, r0*self.b
-            _a1, _b1 = r1*self.a, r1*self.b
-        else:
-            _a0, _b0 = r0, r0*self.b/self.a
-            _a1, _b1 = r1, r1*self.b/self.a
-        return RectangularAnnulus(self.coords, _a0, _a1, _b1, theta=np.pi/2-self.orientation)
+        return _new
 
-    def fit_isophotes(self, debug=False):
-        """Fit a photutils.isophote.Ellipse to the source. Requires the source to be instantiated from a skimage RegionProperties
+    def best_aperture_index(self, method="stddiff", sigma=4):
+        """Find index of best aperture
 
         Parameters
         ----------
-        debug : bool, optional
-            whether to plot the result for debugging, by default False
+        method : str, optional
+            Method to find best aperture, by default "stddiff"
 
         Returns
         -------
-        output of photutils.isophote.Ellipse.fit_image
+        int
+            index of best aperture
         """
-        data = self._region.image_intensity
-        y0, x0 = np.unravel_index(np.argmax(data), data.shape)
-        e = self.b / self.a
-        geometry = EllipseGeometry(x0, y0, sma=self.a/4, eps=e, pa=np.pi/2 - self.orientation)
-        ellipse = IsoEllipse(data - np.median(data), geometry)
-        isolist = ellipse.fit_image()
-        
-        if debug:
-            plt.imshow(data)
-            smas = np.linspace(3, 20, 15)
-            for sma in smas:
-                iso = isolist.get_closest(sma)
-                x, y, = iso.sampled_coordinates()
-                plt.plot(x, y, color='white')
-                
-        return isolist
+        i = optimal_flux(self._target_attr("fluxes", full=True), method, sigma=sigma)
+        return i
 
-    @property
-    def _symbol(self):
-        return "?"
+    def estimate_best_aperture(
+        self, target: int = None, method: str = "stddiff", sigma=4
+    ):
+        """Inplace setting of best aperture.
 
-    @property
-    def _desc(self):
-        return f"{self._symbol} {self.__class__.__name__}" + f" {self.i}" if self.i is not None else ""
+        Parameters
+        ----------
+        target : int, optional
+            Index of target, by default None
+        method : str, optional
+            Method to find best aperture, by default "stddiff"
+        """
+        if target is None:
+            target = self.target
+        self.aperture = self.best_aperture_index(method=method, sigma=sigma)
 
-    def _repr_dict(self, n=8):
-        return {
-            "coords": f"{self.coords[0]:.2f}".rjust(n) + f"{self.coords[1]:.2f}".rjust(n),
-            "a, b": f"{self.a:.2f}".rjust(n) + f"{self.b:.2f}".rjust(n),
-            "e": f"{self.b/self.a:.2f}".rjust(n),
-            "region": str(self._region is not None).rjust(n)
-            }
-
-    def __str__(self):
-        table = "\n".join([f"  {n}".ljust(8) + f"{v}" for n, v in self._repr_dict().items()])
-        return f"{self._desc}\n  {'-'*(len(self._desc)-2)}\n{table}"
-    
-def auto_source(region, i=None, trace=0.3, extended=0.9, discard=False):
-    if region is None:
-        return DiscardedSource(region, i=i)
-    a = region.axis_major_length
-    b = region.axis_minor_length
-    if a == 0.:
-        if discard:
-            return DiscardedSource(region, i=i)
-        else:
-            return PointSource(region, i=i)
-    ratio = b/a
-    if ratio <= extended:
-        if ratio <= trace:
-            return TraceSource(region, i=i)
-        else:
-            return ExtendedSource(region, i=i)
-    else:
-        return PointSource(region, i=i)
+    def estimate_error(self):
+        pass
+
+    def plot(self, marker=".", color="0.8", ls="", ax=None, **kwargs):
+        """Plot light curve
 
-class DiscardedSource(Source):
-    def __init__(self, region, i=None):
-        super().__init__(region, i=i)
-        self.discarded = True
-        
-    def plot(self, ms=15, c="C0", ax=None, **kwargs):
+        Parameters
+        ----------
+        marker : str, optional
+            Marker style, by default "."
+        color : str, optional
+            Marker color, by default "0.8"
+        ls : str, optional
+            Line style, by default ""
+        ax : _type_, optional
+            Matplotlib axis, by default None which takes :code:`plt.gca()`
+        """
         if ax is None:
             ax = plt.gca()
-        ax.plot(*self.coords, "x", c=c, ms=ms, **kwargs)
-    
-class PointSource(Source):
-    def __init__(self, region=None, coords=None, peak=0, i=None):
-        """Point source (star)
+        kwargs.update(dict(marker=marker, color=color, ls=ls))
+        if self.time is None:
+            ax.plot(self.flux, **kwargs)
+        else:
+            ax.plot(self.time, self.flux, **kwargs)
+
+    def errorbar(self, color="k", fmt=".", **kwargs):
+        """Error bar plot of the light curve
 
         Parameters
         ----------
-        region : skimage.measure.RegionProperties, optional
-            An skimage RegionProperties containing the source, by default None. Only one of 'coords' or 'region' must be provided
-        coords : array, optional
-            Pixel coordinates of the source, by default None. Only one of 'coords' or 'region' must be provided
-        peak : float, optional
-            maximum pixel value of the source, by default 0
-        i : int, optional
-            index identifier of the source, by default None
+        color : str, optional
+            Marker color, by default "k"
+        fmt : str, optional
+            Error bar plot style, by default "."
         """
-        super().__init__(region=region, coords=coords, peak=peak, i=i)
-
-    @property
-    def _symbol(self):
-        return chr(8226)
+        kwargs.update(dict(color=color, fmt=fmt))
+        plt.errorbar(self.time, self.flux, self.error, **kwargs)
 
-    def plot(self, radius=15, **kwargs):
-        """Plot circle centered on source
+    def bin(self, size: float, estimate_error: bool = False) -> "Fluxes":
+        """Returns a :code:`Fluxes` instance with binned time series
 
         Parameters
         ----------
-        radius : int, optional
-            radius, by default 15
+        size : float
+            bin size in same unit as :code:`self.time`
+        estimate_error : bool, optional
+            whether to estimate error as the standard deviation of flux in each bin,
+            by default False
+
+        Returns
+        -------
+        _type_
+            _description_
         """
-        self.plot_circle(radius, **kwargs)
+        if isinstance(size, float):
+            assert (
+                self.time is not None
+            ), "using a float bin size requires time to be set"
 
-    def aperture(self, r=1, scale=True):
-        return self.circular_aperture(r, scale=scale)
+        time = self.time if self.time is not None else np.arange(self.fluxes.shape[-1])
+        idxs = utils.index_binning(time, size)
+        _new = deepcopy(self)
 
-    def annulus(self, r0=1.05, r1=1.4, scale=True):
-        return self.circular_annulus(r0, r1, scale=scale)
+        _new.fluxes = np.array([np.mean(self.fluxes.T[i], 0) for i in idxs]).T
 
-    
-class ExtendedSource(Source):
-    def __init__(self, region=None, coords=None, peak=0, i=None):
-        """Extended source (comet, galaxy or lensed source)
+        if self.time is not None:
+            _new.time = np.array([np.mean(self.time[i], 0) for i in idxs])
+        if self.errors is not None:
+            _new.errors = np.array(
+                [np.mean(self.errors.T[i], 0) / np.sqrt(len(i)) for i in idxs]
+            ).T
+
+        if estimate_error:
+            _new.errors = np.array(
+                [np.std(self.fluxes.T[i], 0) / np.sqrt(len(i)) for i in idxs]
+            ).T
+        elif self.errors is not None:
+            _new.errors = np.array(
+                [np.sqrt(np.sum(np.power(self.errors[i], 2))) / len(i) for i in idxs]
+            ).T
+
+        return _new
+
+    def save(self, path: Union[str, Path]):
+        """Save fluxes to file
 
         Parameters
         ----------
-        region : skimage.measure.RegionProperties, optional
-            An skimage RegionProperties containing the source, by default None. Only one of 'coords' or 'region' must be provided
-        coords : array, optional
-            Pixel coordinates of the source, by default None. Only one of 'coords' or 'region' must be provided
-        peak : float, optional
-            maximum pixel value of the source, by default 0
-        i : int, optional
-            index identifier of the source, by default None
+        path : Union[str, Path]
+            path of the file
         """
-        super().__init__(region=region, coords=coords, peak=peak, i=i)
+        with open(path, "wb") as f:
+            pickle.dump(asdict(self), f)
+
+    def load(path: Union[str, Path]):
+        with open(path, "rb") as f:
+            return Fluxes(**pickle.load(f))
+
+    def copy(self):
+        return deepcopy(self)
 
     @property
-    def _symbol(self):
-        return chr(11053)
+    def dataframe(self):
+        df_dict = self.data.copy()
+        df_dict.update({"time": self.time})
+        if self._is_target_aperture_set:
+            df_dict.update({"flux": self.flux})
 
-    def plot(self, radius=6, **kwargs):
-        """Plot Ellipse on source
+        return pd.DataFrame(df_dict)
+
+    @property
+    def df(self):
+        return self.dataframe
+
+    def mask(self, array):
+        """Mask time-dependant fluxes attributes (time, fluxes, errors, data)
 
         Parameters
         ----------
-        radius : int, optional
-            extension to minor/major axis, by default 6
-        """
-        self.plot_ellipse(radius, **kwargs)
+        m : np.array of bool
+            mask
 
-    def compute_centroid(self, method="max"):
-        """Recompute source centroid (inplace). To use this method, source must be obtained from a region 
+        Returns
+        -------
+        Fluxes
+            masked Fluxes
         """
-        if method == "max":
-            y0, x0 = np.unravel_index(np.argmax(self._region.image_intensity), self._region.image.shape)
-            dy, dx, _, _ = self._region.bbox
-            self.coords = np.array([x0+dx, y0+dy])
-        elif method == "isophote":
-            isolist = self.fit_isophotes()
-            origin = np.array(self._region.bbox)[0:2][::-1]
-            self.coords = np.array([isolist[0].x0, isolist[0].y0]) + origin
-
-    def aperture(self, r=1, scale=True):
-        return self.elliptical_aperture(r, scale=scale)
-    
-    def annulus(self, r0=1.05, r1=1.4, scale=True):
-        return self.elliptical_annulus(r0, r1, scale=scale)
+        _new = self.copy()
+        _new.data = {key: value[array] for key, value in self.data.items()}
+        if self.fluxes is not None:
+            _new.fluxes = self.fluxes[..., array]
+        if self.errors is not None:
+            _new.errors = self.errors[..., array]
+        if self.time is not None:
+            _new.time = self.time[array]
+
+        return _new
+
+    def sigma_clipping_data(self, iterations: int = 5, **kwargs):
+        """Return a Fluxes instance masked using iteratively sigma clipped data.
 
+        Parameters
+        ----------
+        it : int, optional
+            iterations, by default 5
+        **kwargs: dict
+            dict where keys are the names of the data to sigma clip and value are the
+            sigma
 
-class TraceSource(Source):
-    def __init__(self, region=None, coords=None, peak=0, i=None):
-        """Trace source (diffracted spectrum, satellite streak or cosmic ray)
+        Returns
+        -------
+        Fluxes
+            sigma clipped Fluxes
+        """
+        mask = np.ones_like(self.time).astype(bool)
+        for _ in range(iterations):
+            for name, sigma in kwargs.items():
+                value = self.data[name].copy()
+                value[~mask] = np.nan
+                m = np.abs(value - np.nanmean(value)) < np.nanstd(value) * sigma
+                mask = mask & m
+        return self.mask(mask)
+
+    def sigma_clip_flux(self, iterations: int = 5, sigma: float = 4.0):
+        """Return a Fluxes instance masked using iteratively sigma clipping.
 
         Parameters
         ----------
-        region : skimage.measure.RegionProperties, optional
-            An skimage RegionProperties containing the source, by default None. Only one of 'coords' or 'region' must be provided
-        coords : array, optional
-            Coordinates of the source, by default None. Only one of 'coords' or 'region' must be provided
-        peak : float, optional
-            maximum pixel value of the source, by default 0
-        i : int, optional
-            index identifier of the source, by default None
+        it : int, optional
+            iterations, by default 5
+        sigma: float
+            sigma, by default 4.0
+
+        Returns
+        -------
+        Fluxes
+            sigma clipped Fluxes
         """
-        super().__init__(region=region, coords=coords, peak=peak, i=i)
-        self.discarded = True
-        
-    def plot(self, offset=10, ax=None, c=color, label=True, fontsize=12):
-        if ax is None:
-            ax = plt.gca()
-        x0, y0 = self.coords
-        theta = self.orientation
-        x1 = x0 - np.sin(np.pi+theta) * 0.5 * self.a
-        y1 = y0 - np.cos(np.pi+theta) * 0.5 * self.a
-        x2 = x0 - np.sin(theta) * 0.5 * self.a
-        y2 = y0 - np.cos(theta) * 0.5 * self.a
-
-        ax.plot((x1, x2), (y1, y2), c=c)
-
-        if label and self.i is not None:
-            label_coords = self.coords + [0, -offset]
-            plt.text(*label_coords, self.i, c=c, ha="center", va="top", fontsize=fontsize)
-    
-    def aperture(self, r=1, scale=True):
-        return self.rectangular_aperture(r, scale=scale)
+        flux = self.flux.copy()
+        mask = np.ones_like(self.time).astype(bool)
+        for _ in range(iterations):
+            mask &= np.abs(flux - np.nanmean(flux)) < np.nanstd(flux[mask]) * sigma
+        return self.mask(mask)
+
+    def mask_stars(self, mask: np.array, keep_indexing: bool = True):
+        """Mask stars fluxes.
 
-    def annulus(self, r0=1.05, r1=1.4, scale=True):
-        return self.rectangular_annulus(r0, r1, scale=scale)
+        In order to keep indexing, the fluxes are set to -1.
 
+        Parameters
+        ----------
+        mask : np.array
+            A boolean array of the same length as the number of stars, indicating which fluxes should be masked
+        remove : bool, optional
+            whether to keep indexing (recommended) and only set pixels to 1, by default False
 
-    
+        Returns
+        -------
+        Fluxes
+            A new Fluxes instance with masked stars
+        """
+        copy = self.copy()
+        if not keep_indexing:
+            copy.fluxes = self.fluxes[..., mask, :]
+            if copy.errors is not None:
+                copy.errors = self.errors[..., mask, :]
+            if copy.weights is not None:
+                copy.weights = self.weights[..., mask, :]
+        else:
+            copy.fluxes[:, ~mask] = -1
+            if copy.errors is not None:
+                copy.errors[:, ~mask] = -1
+            if copy.weights is not None:
+                copy.errors[:, ~mask] = 0
+        return copy
```

### Comparing `prose-2.3.0/prose/io/create_fm_db.sql` & `prose-3.0.0/prose/io/create_fm_db.sql`

 * *Files identical despite different names*

### Comparing `prose-2.3.0/prose/io/fitsmanager.py` & `prose-3.0.0/prose/io/fitsmanager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import sqlite3
+from functools import partial
+from pathlib import Path
+
 import numpy as np
 import pandas as pd
-from pathlib import Path
-from .io import get_files, fits_to_df
 from IPython.display import display
-from ..console_utils import progress, info
+
+from prose.console_utils import info, progress
+
+from .io import fits_to_df, get_files
 
 # Convenience
 # -----------
 SQL_DAYS_BETWEEN = "date >= date('{date}', '-{past:.0f} days') AND date <= date('{date}', '+{future:.0f} days')"
 
-UNIQUE_FIELDS_LIST = ["date", "telescope", "filter", "target", "type", "width", "height", "exposure"]
+UNIQUE_FIELDS_LIST = [
+    "date",
+    "telescope",
+    "filter",
+    "target",
+    "type",
+    "width",
+    "height",
+    "exposure",
+]
 UNIQUE_FIELDS = ",".join(UNIQUE_FIELDS_LIST)
-QMARKS_UNIQUE = ",".join(['?']*len(UNIQUE_FIELDS.split(",")))
+QMARKS_UNIQUE = ",".join(["?"] * len(UNIQUE_FIELDS.split(",")))
 
 PWD = Path(__file__).parent
 
 
 def in_value(value):
     return f"'{value}'" if isinstance(value, str) else value
 
+
 def exposure_constraint(exposure=0, tolerance=1000000):
     return f"exposure between {exposure-tolerance} and {exposure+tolerance}"
+
+
 # ------------
 
 
 class FitsManager:
     """Object to parse and retrieve FITS files from folder and sub-folders
 
     This object scans files in a folder and stores the data in a mysql database for conveniance (but all products can be accessed without knowledge of the SQL language)
@@ -43,91 +59,180 @@
     file : _type_, optional
         _description_, by default None
     batch_size : bool or int, optional
         - if False: update database after all FITS files are parsed
         - if int: update database every time ``batch_size`` FITS files are parsed
 
         by default False
+    telescope: :py:class:`~prose.Telescope``
+        telescope to use while parsing files, by default None
     """
-    
-    def __init__(self, folders=None, files=None, depth=0, hdu=0, extension=".f*t*", file=None, batch_size=False, scan=None, verbose=True, to_df=None):
+
+    def __init__(
+        self,
+        folders=None,
+        files=None,
+        depth=0,
+        hdu=0,
+        extension=".f*t*",
+        file=None,
+        batch_size=False,
+        scan=None,
+        verbose=True,
+        to_df=None,
+        telescope=None,
+    ):
         if file is None:
             file = ":memory:"
 
         self.con = sqlite3.connect(file)
         self.cur = self.con.cursor()
 
         # check if file Table exists
-        tables = list(self.cur.execute("SELECT name FROM sqlite_master WHERE type='table';"))
+        tables = list(
+            self.cur.execute("SELECT name FROM sqlite_master WHERE type='table';")
+        )
         if len(tables) == 0:
             db_creation = open(PWD / "create_fm_db.sql", "r").read()
             self.cur.executescript(db_creation)
-        
+
         if folders is not None:
             assert files is None, "Only 'folders' or 'files' must be provided, not both"
             files = self.get_files(folders, extension, depth=depth, scan=scan)
-        
+
         if to_df is None:
-            self.fits_to_df = fits_to_df
+            if telescope is None:
+                self.fits_to_df = fits_to_df
+            else:
+                self.fits_to_df = partial(fits_to_df, telescope=telescope)
         else:
             self.fits_to_df = to_df
 
         if files is not None:
             if len(files) > 0:
-                self.scan_files(files, batch_size=batch_size, hdu=hdu, verbose=verbose)
-
-    def _insert(self, path, date, telescope, type, target, filter, dimensions, _, jd, exposure, id=None, update_obs=True):
-        """Insert FITS data to object database
-        """
+                self.scan_files(
+                    files,
+                    batch_size=batch_size,
+                    hdu=hdu,
+                    verbose=verbose,
+                    telescope=telescope,
+                )
+
+    def _insert(
+        self,
+        path,
+        date,
+        telescope,
+        type,
+        target,
+        filter,
+        dimensions,
+        _,
+        jd,
+        exposure,
+        id=None,
+        update_obs=True,
+    ):
+        """Insert FITS data to object database"""
         if isinstance(filter, float):
             filter = ""
         else:
             filter = filter or ""
         telescope = telescope or ""
         target = target or ""
         id = id or "NULL"
         width, height = dimensions
         filter = filter.replace("'", "p")
 
         # update observation
         if update_obs:
             obs = (date, telescope, filter, target, type, width, height, exposure)
-            self.con.execute(f"INSERT or IGNORE INTO observations({UNIQUE_FIELDS}, files) VALUES ({QMARKS_UNIQUE}, 0)", obs)
-            query = " AND ".join([f"{str(key)} = {in_value(value)}" for key, value in zip(UNIQUE_FIELDS_LIST, obs)])
-            id = self.con.execute(f"SELECT id FROM observations where {query}").fetchall()[0][0]
-            self.con.execute(f"UPDATE observations SET files = files + 1 WHERE id = {id}")
-            
+            self.con.execute(
+                f"INSERT or IGNORE INTO observations({UNIQUE_FIELDS}, files) VALUES ({QMARKS_UNIQUE}, 0)",
+                obs,
+            )
+            query = " AND ".join(
+                [
+                    f"{str(key)} = {in_value(value)}"
+                    for key, value in zip(UNIQUE_FIELDS_LIST, obs)
+                ]
+            )
+            id = self.con.execute(
+                f"SELECT id FROM observations where {query}"
+            ).fetchall()[0][0]
+            self.con.execute(
+                f"UPDATE observations SET files = files + 1 WHERE id = {id}"
+            )
+
         # or IGNORE to handle the unique constraint
         self.cur.execute(
             f"INSERT or IGNORE INTO files VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
-            (date, path, telescope, filter, type, target, width, height, jd, id, exposure))
-            
+            (
+                date,
+                path,
+                telescope,
+                filter,
+                type,
+                target,
+                width,
+                height,
+                jd,
+                id,
+                exposure,
+            ),
+        )
 
     def get_files(self, folders, extension, scan=None, depth=0):
+        """Return path of files with specific extension in the specified folder(s)
+
+        Parameters
+        ----------
+        folders : str or list of str
+            path or list of paths of folders to look into
+        extension : str
+            wildcard pattern for file extension
+        scan : function, optional
+            function to use, called on each folder path, by default None
+        depth : int, optional
+            number of sub-folders to look into, by default 0
+        """
+
         def _get_files(folder):
             if scan is None:
                 return get_files(extension, folder, depth=depth)
             else:
                 return scan(folder)
 
         if isinstance(folders, (list, tuple)):
-            files = [] 
+            files = []
             for folder in folders:
                 assert Path(folder).exists(), f"Folder {folder} does not exists"
                 files += _get_files(folder)
         else:
             assert Path(folders).exists(), f"Folder {folders} does not exists"
             files = _get_files(folders)
 
         return files
 
     def _path_in(self, path):
-        return self.con.execute(f"SELECT * FROM files WHERE path='{path}'").fetchone() is not None
-
-    def scan_files(self, files, batch_size=False, verbose=True, hdu=0, telescope=None, verbose_new=False, verbose_os=False):
+        return (
+            self.con.execute(f"SELECT * FROM files WHERE path='{path}'").fetchone()
+            is not None
+        )
+
+    def scan_files(
+        self,
+        files,
+        batch_size=False,
+        verbose=True,
+        hdu=0,
+        telescope=None,
+        verbose_new=False,
+        verbose_os=False,
+    ):
         """Scan files and add data to database
 
         Parameters
         ----------
         files : list of str or Path
             paths of files
         batch_size : bool or int, optional
@@ -135,14 +240,16 @@
             - if int: update database every time ``batch_size`` FITS files are parse
 
             by default False
         verbose : bool, optional
             whether to show progress bar during parsing, by default True
         hdu: int
             FITS data unit extension where header will be parsed
+        telescope: prose.Telescope
+            telescope to be imposed for these files, by default None
         """
 
         if len(files) > 0:
             files_to_scan = [path for path in files if not self._path_in(path)]
             if verbose_new:
                 info(f"{len(files_to_scan)} new files to scan")
 
@@ -155,134 +262,231 @@
                     batches = [files_to_scan]
                 else:
                     assert isinstance(batch_size, int), "batch_size must be an int"
 
                     if len(files_to_scan) < batch_size:
                         batches = [files_to_scan]
                     else:
-                        batches = np.array_split(files_to_scan, len(files_to_scan)//batch_size)
-                
+                        batches = np.array_split(
+                            files_to_scan, len(files_to_scan) // batch_size
+                        )
+
                 _verbose = verbose and batch_size is not False
                 _progress = progress(_verbose, desc="Reading fits", unit="files")
 
                 if batch_size is not False:
                     for batch in _progress(batches):
-                        df = self.fits_to_df(batch, verbose=False, hdu=hdu, verbose_os=verbose_os)
-                        for row in df.values:
-                            if telescope is not None:
-                                row[2] = telescope
-                            self._insert(*row)
-                        self.con.commit()
+                        try:
+                            df = self.fits_to_df(
+                                batch, verbose=False, hdu=hdu, verbose_os=verbose_os
+                            )
+                            for row in df.values:
+                                if telescope is not None:
+                                    row[2] = telescope.name
+                                self._insert(*row)
+                            self.con.commit()
+                        except:
+                            "ERROR, batch ignored"
                 else:
-                    df = self.fits_to_df(files_to_scan, verbose=True, hdu=hdu, verbose_os=verbose_os)
+                    df = self.fits_to_df(
+                        files_to_scan, verbose=verbose, hdu=hdu, verbose_os=verbose_os
+                    )
                     for row in df.values:
                         if telescope is not None:
-                            row[2] = telescope
+                            row[2] = telescope.name
                         self._insert(*row)
                     self.con.commit()
             else:
                 if not verbose_new:
                     f"{len(files_to_scan)} new files to scan"
         else:
             raise AssertionError(f"No files provided")
 
     def observations(self, hide_exposure=True, **kwargs):
-        columns = {c[1]: "%" for c in self.con.execute("PRAGMA table_info(observations)").fetchall()[1:-3]}
+        """return a pandas DataFrame of observations given some metadata constraints in the form of wildcards
+
+        Parameters
+        ----------
+        hide_exposure : bool, optional
+            whether to include exposure in the pandas.DataFrame header, by default True
+        **kwargs:
+            wildcards value for telescope, target, filter, type or id, default is '*'
+
+        Returns
+        -------
+        pd.DataFrame
+            pandas DataFrame filtered with kwargs wildcards
+        """
+        columns = {
+            c[1]: "%"
+            for c in self.con.execute("PRAGMA table_info(observations)").fetchall()[
+                1:-3
+            ]
+        }
         inputs = kwargs.copy()
-            
+
         for key, value in inputs.items():
             inputs[key] = "%" if value is None else str(value).replace("*", "%")
-            
+
         columns.update(inputs)
-        
-        where = " AND ".join([f"{key} LIKE {in_value(value)}" for key, value in columns.items()])
+
+        where = " AND ".join(
+            [f"{key} LIKE {in_value(value)}" for key, value in columns.items()]
+        )
         query = f"select * from observations where {where}"
-        
+
         if hide_exposure:
             query = f"select *, SUM(files) from observations where {where} GROUP BY date, telescope, target, filter, type"
             df = self.to_pandas(query)
             df["files"]
-            df = df.drop(columns=["files", "exposure"]).rename(columns={"SUM(files)": "files"})
+            df = df.drop(columns=["files", "exposure"]).rename(
+                columns={"SUM(files)": "files"}
+            )
         else:
             query = f"select * from observations where {where}"
             df = self.to_pandas(query)
-            
+
         return df.set_index(["id"])
 
     def calibrations(self, **kwargs):
+        """return a pandas DataFrame of calibrations observations given some metadata constraints in the form of wildcards
+
+        Parameters
+        ----------
+        **kwargs:
+            wildcards value for telescope, target, filter or id, default is '*'
+        """
         darks = self.observations(type="dark", **kwargs)
         flats = self.observations(type="flat", **kwargs)
         bias = self.observations(type="bias", **kwargs)
-        
+
         return pd.concat([darks, flats, bias], axis=0)
-        
+
     def files(self, id=None, path=False, exposure=0, tolerance=1000, **kwargs):
-        columns = {c[1]: "%" for c in self.con.execute("PRAGMA table_info(files)").fetchall()}
+        """Return a pandas DataFrame of files given some metadata constraints in the form of wildcards
+
+        Parameters
+        ----------
+        id : int, optional
+            id of the observation for which files are retrieved, by default None, i.e. all files
+        path : bool, optional
+            whether to include files paths in the pandas.DataFrame header, by default False
+        exposure : int, optional
+            exposure constraint on the files to retrieve, by default 0
+        tolerance : int, optional
+            tolerance on the exposure constraint, by default 1000. For example: if exposure is set to 10 and tolerance to 2, all
+            files with exposure = 10 +- 2 will be retrieved
+        """
+        columns = {
+            c[1]: "%" for c in self.con.execute("PRAGMA table_info(files)").fetchall()
+        }
         if not path:
             del columns["path"]
         columns["id"] = id or "%"
         inputs = kwargs.copy()
 
         for key, value in inputs.items():
             inputs[key] = "%" if value is None else str(value).replace("*", "%")
 
         columns.update(inputs)
 
-        where = " AND ".join([f"{key} LIKE {in_value(value)}" for key, value in columns.items()])
+        where = " AND ".join(
+            [f"{key} LIKE {in_value(value)}" for key, value in columns.items()]
+        )
         where += f" AND {exposure_constraint(exposure, tolerance)}"
 
         del columns["id"]
-        df = self.to_pandas(f"select {','.join(columns.keys())} from files where {where} order by jd")
+        df = self.to_pandas(
+            f"select {','.join(columns.keys())} from files where {where} order by jd"
+        )
         return df
-    
-    def observation_files(self, i, past=1e3, future=0, tolerance=1e15, same_telescope=True, lights="images", show=True):
+
+    def paths(self, **kwargs):
+        """Get the paths of all files matching the kwargs query (see prose.FitsImage.files)
+
+        Returns
+        -------
+        list
+            list of files paths
+        """
+        return self.files(**kwargs, path=True).path.values
+
+    def observation_files(
+        self,
+        i,
+        past=1e3,
+        future=0,
+        tolerance=1e15,
+        same_telescope=True,
+        lights="images",
+        show=True,
+    ):
         files = {}
 
         obs_dict = self.observations(id=i, hide_exposure=False).to_dict("records")[0]
-        sql_days = SQL_DAYS_BETWEEN.format(date=obs_dict["date"], future=future, past=past)
-        sql_exposure = exposure_constraint(exposure=obs_dict["exposure"], tolerance=tolerance)
-
-        files[lights] = self.to_pandas(f"SELECT path from files where id = {i} order by jd").values.flatten()
+        sql_days = SQL_DAYS_BETWEEN.format(
+            date=obs_dict["date"], future=future, past=past
+        )
+        sql_exposure = exposure_constraint(
+            exposure=obs_dict["exposure"], tolerance=tolerance
+        )
+
+        files[lights] = self.to_pandas(
+            f"SELECT path from files where id = {i} order by jd"
+        ).values.flatten()
         dfs = []
 
         if show:
             dfs.append(self.to_pandas(f"SELECT * from observations where id = {i}"))
 
         for type in ("dark", "bias", "flat"):
             fields = ["width", "height"]
             if same_telescope:
                 fields.append("telescope")
             if type == "flat":
                 fields.append("filter")
 
-            query = " AND ".join([f"{key} = {in_value(obs_dict[key])}" for key in fields])
+            query = " AND ".join(
+                [f"{key} = {in_value(obs_dict[key])}" for key in fields]
+            )
             query += f" AND type = '{type}'"
             query = query.format(**obs_dict)
 
-            obs_ids = self.to_pandas(f"""SELECT id FROM observations WHERE {sql_exposure} AND {query}
+            obs_ids = self.to_pandas(
+                f"""SELECT id FROM observations WHERE {sql_exposure} AND {query}
                 AND date = (SELECT MAX(date) FROM files WHERE {sql_days} AND {query})
-            """).values.flatten()
-            
+            """
+            ).values.flatten()
+
             if show:
-                dfs.append(self.to_pandas(f"""SELECT * FROM observations WHERE {sql_exposure} 
+                dfs.append(
+                    self.to_pandas(
+                        f"""SELECT * FROM observations WHERE {sql_exposure} 
                     AND {query} AND type = '{type}'
                     AND date = (SELECT MAX(date) FROM files 
                     WHERE {sql_days} AND {query})
-                """))
-
-            _files = [self.to_pandas(f"select path from files where id={j} order by jd").values.flatten() for j in obs_ids]
+                """
+                    )
+                )
+
+            _files = [
+                self.to_pandas(
+                    f"select path from files where id={j} order by jd"
+                ).values.flatten()
+                for j in obs_ids
+            ]
             if len(_files) > 0:
                 _files = np.hstack(_files)
 
             files[type + ("s" if type[-1] != "s" else "")] = _files
-            
+
         if show:
             df = pd.concat(dfs, axis=0).set_index(["id"])
             display(df)
-        
+
         return files
 
     @property
     def unique_obs(self):
         """Return whether the object contains a unique observation (observation is defined as a unique combinaison of date, telescope, target and filter).
 
         Returns
@@ -295,58 +499,57 @@
     def all_images(self):
         """fits paths of the observation science images
 
         Returns
         -------
         list of str
         """
-        return self.files(type='light', path=True).path.values
+        return self.files(type="light", path=True).path.values
 
     def images(self, i, show=False, **kwargs):
-        return self.observation_files(i, show=show, **kwargs)['images']
+        return self.observation_files(i, show=show, **kwargs)["images"]
 
     @property
     def all_darks(self):
         """fits paths of the observation dark images
 
         Returns
         -------
         list of str
         """
-        return self.files(type='dark', path=True).path.values
+        return self.files(type="dark", path=True).path.values
 
     def bias(self, i, show=False, **kwargs):
-        return self.observation_files(i, show=show, **kwargs)['bias']
-
+        return self.observation_files(i, show=show, **kwargs)["bias"]
 
     @property
     def all_bias(self):
         """fits paths of the observation bias images
 
         Returns
         -------
         list of str
         """
-        return self.files(type='bias', path=True).path.values
+        return self.files(type="bias", path=True).path.values
 
     def darks(self, i, show=False, **kwargs):
-        return self.observation_files(i, show=show, **kwargs)['darks']
+        return self.observation_files(i, show=show, **kwargs)["darks"]
 
     @property
     def all_flats(self):
         """fits paths of the observation flats images
 
         Returns
         -------
         list of str
         """
-        return self.files(type='flat', path=True).path.values
+        return self.files(type="flat", path=True).path.values
 
     def flats(self, i, show=False, **kwargs):
-        return self.observation_files(i, show=show, **kwargs)['flats']
+        return self.observation_files(i, show=show, **kwargs)["flats"]
 
     @property
     def stack(self):
         """fits paths of the observation stack image if present
 
         Returns
         -------
@@ -366,44 +569,62 @@
 
     def label(self, i):
         date, telescope, filter, _, target, *_ = self.observations(id=i).values[0]
         return f"{telescope}_{date.replace('-', '')}_{target}_{filter}"
 
     @property
     def obs_name(self):
-        """Observation name ({telescope}_{date}_{target}_{filter}) if a single observation is present
-        """
+        """Observation name ({telescope}_{date}_{target}_{filter}) if a single observation is present"""
         if self.unique_obs:
             return self.label()
         else:
-            raise AssertionError("obs_name property is only available for FitsManager containing a unique observation")
+            raise AssertionError(
+                "obs_name property is only available for FitsManager containing a unique observation"
+            )
 
     def __repr__(self):
         return str(self.observations())
 
     def _repr_html_(self):
         return self.observations()._repr_html_()
 
     def to_pandas(self, query):
         return pd.read_sql_query(query, self.con)
 
     def _update_observations(self, verbose=False):
         """
         Slow! This should never be used (use update_obs=True in _insert)
         """
-        observations = self.to_pandas(f"select {UNIQUE_FIELDS} from files WHERE id is NULL GROUP BY {UNIQUE_FIELDS}").values
+        observations = self.to_pandas(
+            f"select {UNIQUE_FIELDS} from files WHERE id is NULL GROUP BY {UNIQUE_FIELDS}"
+        ).values
 
         _progress = progress(verbose, desc="observations scan", unit=" obs")
 
         for obs in _progress(observations):
             # insert obs
-            self.con.execute(f"INSERT or IGNORE INTO observations({UNIQUE_FIELDS}, files) VALUES ({QMARKS_UNIQUE}, 0)", obs)
+            self.con.execute(
+                f"INSERT or IGNORE INTO observations({UNIQUE_FIELDS}, files) VALUES ({QMARKS_UNIQUE}, 0)",
+                obs,
+            )
             self.con.commit()
 
             # get its id
-            query = " AND ".join([f"{str(key)} = {in_value(value)}" for key, value in zip(UNIQUE_FIELDS_LIST, obs)])
-            obs_id = self.con.execute(f"SELECT id FROM observations where {query}").fetchall()[0][0]
+            query = " AND ".join(
+                [
+                    f"{str(key)} = {in_value(value)}"
+                    for key, value in zip(UNIQUE_FIELDS_LIST, obs)
+                ]
+            )
+            obs_id = self.con.execute(
+                f"SELECT id FROM observations where {query}"
+            ).fetchall()[0][0]
 
             # and fill files id values
-            self.con.execute(f"UPDATE files SET id = ? WHERE id is NULL AND {query}", [obs_id])
+            self.con.execute(
+                f"UPDATE files SET id = ? WHERE id is NULL AND {query}", [obs_id]
+            )
             files_updated = self.con.execute("select changes()").fetchall()[0][0]
-            self.con.execute("UPDATE observations SET files = files + ? WHERE id = ?", [files_updated, obs_id])
+            self.con.execute(
+                "UPDATE observations SET files = files + ? WHERE id = ?",
+                [files_updated, obs_id],
+            )
```

### Comparing `prose-2.3.0/prose/io/io.py` & `prose-3.0.0/prose/io/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import glob
+import os
+import zipfile
+from datetime import timedelta
 from os import path
-import pandas as pd
+
 import numpy as np
-from ..telescope import Telescope
-from datetime import timedelta
+import pandas as pd
 from astropy.io import fits
-from ..console_utils import tqdm, warning
 from astropy.time import Time
-import os
-import zipfile
+
+from prose.console_utils import progress, warning
+from prose.telescope import Telescope
 
 
 def phot2dict(filename):
     hdu = fits.open(filename)
     dictionary = {h.name.lower(): h.data for h in hdu}
     dictionary["header"] = hdu[0].header
 
     return dictionary
 
 
 def get_files(
-        ext,
-        folder,
-        depth=0,
-        return_folders=False,
-        single_list_removal=False,
-        none_for_empty=False,
+    ext,
+    folder,
+    depth=0,
+    return_folders=False,
+    single_list_removal=False,
+    none_for_empty=False,
 ):
     """
 
     Return files of specific extension in the specified folder and sub-folders
 
     Parameters
     ----------
+    extension: str
+        wildcard pattern for file extension
     folder : str
         Folder to be analyzed
     depth : int
         Number how sub-folder layer to look into.
         0 (default) will look into current folder
         1 will look into current folder and its sub-folders
         2 will look into current folder, its sub-folders and their sub-folders
@@ -75,112 +79,148 @@
     if key in hdu_list:
         hdu_list[key] = value
     else:
         hdu_list.append(value)
 
 
 def fits_to_df(
-    files, 
-    telescope_kw="TELESCOP", 
-    instrument_kw="INSTRUME", 
-    verbose=True, 
-    hdu=0, 
-    raise_oserror=False, 
-    verbose_os=False
-    ):
-    
+    files,
+    telescope_kw="TELESCOP",
+    instrument_kw="INSTRUME",
+    telescope=None,
+    verbose=True,
+    hdu=0,
+    raise_oserror=False,
+    verbose_os=False,
+):
     assert len(files) > 0, "Files not provided"
 
     last_telescope = "_"
     telescopes_seen = []
-    telescope = None
+    _telescope = None
     df_list = []
 
-    def progress(x):
-        return tqdm(x, "Parsing FITS") if verbose else x
-
-    for i in progress(files):
+    for i in progress(verbose, desc="Parsing FITS")(files):
         try:
             header = fits.getheader(i, hdu)
         except OSError as err:
             if verbose_os:
                 warning(f"OS error for file {i}")
             if raise_oserror:
                 print(f"OS error: {err}")
                 raise
             else:
                 continue
-            
-        telescope_name = header.get(telescope_kw, "")
-        instrument_name = header.get(instrument_kw, "")
-
-        telescope_id = f"{telescope_name}_{instrument_name}"
-        if telescope_id not in telescopes_seen:
-            telescopes_seen.append(telescope_id)
-            verbose = True
+
+        if telescope is None:
+            telescope_name = header.get(telescope_kw, "")
+            instrument_name = header.get(instrument_kw, "")
+
+            telescope_id = f"{telescope_name}_{instrument_name}"
+            if telescope_id not in telescopes_seen:
+                telescopes_seen.append(telescope_id)
+                verbose = True
+            else:
+                verbose = False
+
+            if telescope_id != last_telescope or _telescope is None:
+                _telescope = Telescope.from_names(
+                    header.get(instrument_kw, ""), header.get(telescope_kw, "")
+                )
+                last_telescope = telescope_id
         else:
-            verbose = False
+            _telescope = telescope
+
+        df_list.append(
+            dict(
+                path=i,
+                date=_telescope.date(header).isoformat(),
+                telescope=_telescope.name,
+                type=_telescope.image_type(header),
+                target=header.get(_telescope.keyword_object, ""),
+                filter=header.get(_telescope.keyword_filter, ""),
+                dimensions=(header.get("NAXIS1", 1), header.get("NAXIS2", 1)),
+                flip=header.get(_telescope.keyword_flip, ""),
+                jd=header.get(_telescope.keyword_jd, ""),
+                exposure=float(header.get(_telescope.keyword_exposure_time, -1)),
+            )
+        )
 
-        if telescope_id != last_telescope:
-            telescope = Telescope.from_names(header.get(instrument_kw, ""), header.get(telescope_kw, ""))
-            last_telescope = telescope_id
-
-        df_list.append(dict(
-            path=i,
-            date=telescope.date(header).isoformat(),
-            telescope=telescope.name,
-            type=telescope.image_type(header),
-            target=header.get(telescope.keyword_object, ""),
-            filter=header.get(telescope.keyword_filter, ""),
-            dimensions=(header.get("NAXIS1", 1), header.get("NAXIS2", 1)),
-            flip=header.get(telescope.keyword_flip, ""),
-            jd=header.get(telescope.keyword_jd, ""),
-            exposure=float(header.get(telescope.keyword_exposure_time, None))
-        ))
-
-    df = pd.DataFrame(df_list, columns=(
-        "path",
-        "date",
-        "telescope",
-        "type",
-        "target",
-        "filter",
-        "dimensions",
-        "flip",
-        "jd",
-        "exposure"
-    ))
-
-    if len(df) > 0 and telescope is not None:
-        df.type.loc[df.type.str.lower().str.contains(telescope.keyword_light_images.lower())] = "light"
-        df.type.loc[df.type.str.lower().str.contains(telescope.keyword_dark_images.lower())] = "dark"
-        df.type.loc[df.type.str.lower().str.contains(telescope.keyword_bias_images.lower())] = "bias"
-        df.type.loc[df.type.str.lower().str.contains(telescope.keyword_flat_images.lower())] = "flat"
+    df = pd.DataFrame(
+        df_list,
+        columns=(
+            "path",
+            "date",
+            "telescope",
+            "type",
+            "target",
+            "filter",
+            "dimensions",
+            "flip",
+            "jd",
+            "exposure",
+        ),
+    )
+
+    if len(df) > 0 and _telescope is not None:
+        df.type.loc[
+            df.type.str.lower().str.contains(_telescope.keyword_light_images.lower())
+        ] = "light"
+        df.type.loc[
+            df.type.str.lower().str.contains(_telescope.keyword_dark_images.lower())
+        ] = "dark"
+        df.type.loc[
+            df.type.str.lower().str.contains(_telescope.keyword_bias_images.lower())
+        ] = "bias"
+        df.type.loc[
+            df.type.str.lower().str.contains(_telescope.keyword_flat_images.lower())
+        ] = "flat"
         df.telescope.loc[df.telescope.str.lower().str.contains("unknown")] = ""
         df.date = pd.to_datetime(df.date)
         df["filter"] = df["filter"].str.replace("'", "p")
 
         if (df.jd == "").all():  # jd empty then convert from date
-            df.jd = Time(df.date, scale="utc").to_value('jd') + telescope.mjd
+            df.jd = Time(df.date, scale="utc").to_value("jd") + _telescope.mjd
 
         # We want dates that correspond to same observations but night might be over 2 days (before and after midnight)
         # So we remove 15 hours to be sure the date year-month-day are consistent with single observations
-        df.date = (df.date - timedelta(hours=15)).apply(lambda x: x.strftime('%Y-%m-%d'))
+        df.date = (df.date - timedelta(hours=15)).apply(
+            lambda x: x.strftime("%Y-%m-%d")
+        )
 
     return df
 
 
 def get_new_fits(current_df, folder, depth=3):
     dirs = np.array(os.listdir(folder))
     new_dirs = dirs[
-        np.argwhere(pd.to_datetime(dirs, errors='coerce') > pd.to_datetime(current_df.date).max()).flatten()]
-    return np.hstack([get_files("*.f*ts", path.join(folder, f), depth=depth) for f in new_dirs])
+        np.argwhere(
+            pd.to_datetime(dirs, errors="coerce")
+            > pd.to_datetime(current_df.date).max()
+        ).flatten()
+    ]
+    return np.hstack(
+        [get_files("*.f*ts", path.join(folder, f), depth=depth) for f in new_dirs]
+    )
+
 
 def convert_old_index(df):
-    new_df = df[["date", "path", "telescope", "type", "target", "filter", "dimensions", "flip", "jd"]]
+    new_df = df[
+        [
+            "date",
+            "path",
+            "telescope",
+            "type",
+            "target",
+            "filter",
+            "dimensions",
+            "flip",
+            "jd",
+        ]
+    ]
     new_df.dimensions = new_df.dimensions.apply(
         lambda x: tuple(np.array(x.split("x")).astype(int) if x != np.nan else x)
     )
     return new_df
 
 
 def is_zip(filename):
```

### Comparing `prose-2.3.0/prose/utils.py` & `prose-3.0.0/prose/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-from datetime import timedelta
-import numpy as np
-from astropy.visualization import ZScaleInterval
-from astropy.io import fits
-import numba
-import astropy.constants as c
+import inspect
 import urllib
-from astropy.time import Time
-from astropy.table import Table
-from astropy.coordinates import SkyCoord
+from datetime import datetime, timedelta
+from functools import wraps
+
+import astropy.constants as c
 import astropy.units as u
-from datetime import datetime
-import inspect
+import numpy as np
+from astropy.coordinates import SkyCoord
+from astropy.stats import gaussian_sigma_to_fwhm
+from astropy.time import Time
+from astropy.visualization import ZScaleInterval
 from scipy import ndimage
-from functools import wraps
-from collections import OrderedDict
 
 earth2sun = (c.R_earth / c.R_sun).value
 
-def remove_sip(dict_like):
 
+def remove_sip(dict_like):
     for kw in [
-        'A_ORDER',
-        'A_0_2',
-        'A_1_1',
-        'A_2_0',
-        'B_ORDER',
-        'B_0_2',
-        'B_1_1',
-        'B_2_0',
-        'AP_ORDER',
-        'AP_0_0',
-        'AP_0_1',
-        'AP_0_2',
-        'AP_1_0',
-        'AP_1_1',
-        'AP_2_0',
-        'BP_ORDER',
-        'BP_0_0',
-        'BP_0_1',
-        'BP_0_2',
-        'BP_1_0',
-        'BP_1_1',
-        'BP_2_0'
+        "A_ORDER",
+        "A_0_2",
+        "A_1_1",
+        "A_2_0",
+        "B_ORDER",
+        "B_0_2",
+        "B_1_1",
+        "B_2_0",
+        "AP_ORDER",
+        "AP_0_0",
+        "AP_0_1",
+        "AP_0_2",
+        "AP_1_0",
+        "AP_1_1",
+        "AP_2_0",
+        "BP_ORDER",
+        "BP_0_0",
+        "BP_0_1",
+        "BP_0_2",
+        "BP_1_0",
+        "BP_1_1",
+        "BP_2_0",
     ]:
         if kw in dict_like:
             del dict_like[kw]
 
 
 def format_iso_date(date, night_date=True):
     """
@@ -68,159 +65,59 @@
     """
     if isinstance(date, str):
         date = Time(date, format="fits").datetime
     elif isinstance(date, datetime):
         date = Time(date, format="datetime").datetime
 
     if night_date:
-        return (date - timedelta(hours=15)).date()  # If obs goes up to 15pm it still belongs to day before
+        return (
+            date - timedelta(hours=15)
+        ).date()  # If obs goes up to 15pm it still belongs to day before
     else:
         return date
 
 
 def std_diff_metric(fluxes):
     k = len(list(np.shape(fluxes)))
     return np.std(np.diff(fluxes, axis=k - 1), axis=k - 1)
 
 
 def stability_aperture(fluxes):
     lc_c = np.abs(np.diff(fluxes, axis=0))
     return np.mean(lc_c, axis=1)
 
 
-def binning(x, y, bins, error=None, std=False, mean_method=np.mean,
-            mean_error_method=lambda x: np.sqrt(np.sum(np.power(x, 2))) / len(x)):
-
-    bins = np.arange(np.min(x), np.max(x), bins)
-    d = np.digitize(x, bins)
-
-    final_bins = []
-    binned_flux = []
-    binned_error = []
-    _std = []
-
-    for i in range(1, np.max(d) + 1):
-        s = np.where(d == i)
-        if len(s[0]) > 0:
-            binned_flux.append(mean_method(y[s[0]]))
-            final_bins.append(np.mean(x[s[0]]))
-            _std.append(np.std(y[s[0]]) / np.sqrt(len(s[0])))
-            if error is not None:
-                binned_error.append(mean_error_method(error[s[0]]))
-
-    if std:
-        return np.array(final_bins), np.array(binned_flux), np.array(_std)
-    elif error is not None and isinstance(error, (np.ndarray, list)):
-        return np.array(final_bins), np.array(binned_flux), np.array(binned_error)
+def index_binning(x, size):
+    if isinstance(size, float):
+        bins = np.arange(np.min(x), np.max(x), size)
     else:
-        return np.array(final_bins), np.array(binned_flux)
-
+        x = np.arange(0, len(x))
+        bins = np.arange(0.0, len(x), size)
 
-# @numba.jit(fastmath=True, parallel=False, nopython=True)
-# def fast_binning(x, y, bins, error=None, std=False):
-#     bins = np.arange(np.min(x), np.max(x), bins)
-#     d = np.digitize(x, bins)
-#
-#     binned_x = []
-#     binned_y = []
-#     binned_error = []
-#
-#     for i in range(1, np.max(d) + 1):
-#         s = np.where(d == i)
-#         if len(s[0]) > 0:
-#             s = s[0]
-#             binned_y.append(np.mean(y[s]))
-#             binned_x.append(np.mean(x[s]))
-#             binned_error.append(np.std(y[s]) / np.sqrt(len(s)))
-#
-#             if error is not None:
-#                 err = error[s]
-#                 binned_error.append(np.sqrt(np.sum(np.power(err, 2))) / len(err))
-#             else:
-#                 binned_error.append(np.std(y[s]) / np.sqrt(len(s)))
-#
-#     return np.array(binned_x), np.array(binned_y), np.array(binned_error)
-
-
-@numba.jit(fastmath=True, parallel=False, nopython=True)
-def fast_binning(x, y, bins, error=None, std=False):
-    bins = np.arange(np.min(x), np.max(x), bins)
-    d = np.digitize(x, bins)
-
-    n = np.max(d) + 2
-
-    binned_x = np.empty(n)
-    binned_y = np.empty(n)
-    binned_error = np.empty(n)
-
-    binned_x[:] = -np.pi
-    binned_y[:] = -np.pi
-    binned_error[:] = -np.pi
-
-    for i in range(0, n):
-        s = np.where(d == i)
-        if len(s[0]) > 0:
-            s = s[0]
-            binned_y[i] = np.mean(y[s])
-            binned_x[i] = np.mean(x[s])
-            binned_error[i] = np.std(y[s]) / np.sqrt(len(s))
-
-            if error is not None:
-                err = error[s]
-                binned_error[i] = np.sqrt(np.sum(np.power(err, 2))) / len(err)
-            else:
-                binned_error[i] = np.std(y[s]) / np.sqrt(len(s))
-
-    nans = binned_x == -np.pi
-
-    return binned_x[~nans], binned_y[~nans], binned_error[~nans]
-
-
-@numba.jit(fastmath=True, parallel=False, nopython=True)
-def index_binning(x, bins):
-    bins = np.arange(np.min(x), np.max(x), bins)
     d = np.digitize(x, bins)
     n = np.max(d) + 2
     indexes = []
 
     for i in range(0, n):
         s = np.where(d == i)
         if len(s[0]) > 0:
             s = s[0]
             indexes.append(s)
 
     return indexes
 
 
-@numba.jit(fastmath=True, parallel=False, nopython=True)
-def fast_points_binning(x, y, n):
-    n = int(len(x) / n)
-    bins = np.linspace(x.min(), x.max(), n)
-    digitized = np.digitize(x, bins)
-    binned_mean = np.zeros(n)
-    binned_std = np.zeros(n)
-    binned_time = np.zeros(n)
-    for i in range(1, len(bins)):
-        binned_mean[i] = y[digitized == i].mean()
-        binned_std[i] = y[digitized == i].std()
-        binned_time[i] = x[digitized == i].mean()
-
-    return binned_time, binned_mean, binned_std
-
-
 def z_scale(data, c=0.05):
-    if type(data) == str:
-        data = fits.getdata(data)
     interval = ZScaleInterval(contrast=c)
     return interval(data.copy())
 
 
 def rescale(y):
     ry = y - np.mean(y)
-    return ry/np.std(ry)
+    return ry / np.std(ry)
 
 
 def check_class(_class, base, default):
     if _class is None:
         return default
     elif isinstance(_class, base):
         return _class
@@ -239,15 +136,14 @@
 
 
 def fold(t, t0, p):
     return (t - t0 + 0.5 * p) % p - 0.5 * p
 
 
 def header_to_cdf4_dict(header):
-
     header_dict = {}
 
     for key, value in header.items():
         if isinstance(value, str):
             if len(key) > 0 and len(value) > 0:
                 header_dict[key] = value
         elif isinstance(value, (float, np.ndarray, np.number)):
@@ -305,28 +201,30 @@
         return [np.hstack(fx) for fx in filled_xs]
 
 
 def jd_to_bjd(jd, ra, dec):
     """
     Convert JD to BJD using http://astroutils.astronomy.ohio-state.edu (Eastman et al. 2010)
     """
-    bjd = urllib.request.urlopen(f"http://astroutils.astronomy.ohio-state.edu/time/convert.php?JDS={','.join(jd.astype(str))}&RA={ra}&DEC={dec}&FUNCTION=utc2bjd").read()
+    bjd = urllib.request.urlopen(
+        f"http://astroutils.astronomy.ohio-state.edu/time/convert.php?JDS={','.join(jd.astype(str))}&RA={ra}&DEC={dec}&FUNCTION=utc2bjd"
+    ).read()
     bjd = bjd.decode("utf-8")
     return np.array(bjd.split("\n"))[0:-1].astype(float)
 
 
 def remove_arrays(d):
     copy = d.copy()
     for name, value in d.items():
         if isinstance(value, (list, np.ndarray)):
             del copy[name]
     return copy
 
 
-def sigma_clip(y, sigma=5., return_mask=False, x=None):
+def sigma_clip(y, sigma=5.0, return_mask=False, x=None):
     mask = np.abs(y - np.nanmedian(y)) < sigma * np.nanstd(y)
 
     if return_mask:
         return mask
 
     else:
         if x is None:
@@ -342,94 +240,106 @@
     for p in s.parameters.values():
         if p.default != inspect._empty:
             kwargs[p.name] = p.default
         else:
             args.append(p.name)
     return args, kwargs
 
+
 # todo: adapt to work with positional parameters like register
 def register_args(f):
     """
     When used within a class, saves args and kwargs passed to a function
     (mostly used to record __init__ inputs)
     """
+
     @wraps(f)
     def inner(*_args, **_kwargs):
         self = _args[0]
         args, kwargs = args_kwargs(f)
         args = dict(zip(args[1::], _args[1::]))
         kwargs.update(_kwargs)
         self.args = args
         self.kwargs = kwargs
         return f(self, *args.values(), **kwargs)
+
     return inner
-    
 
-def nan_gaussian_filter(data, sigma=1., truncate=4.):
+
+def nan_gaussian_filter(data, sigma=1.0, truncate=4.0):
     """https://stackoverflow.com/questions/18697532/gaussian-filtering-a-image-with-nan-in-python
 
     Parameters
     ----------
     U : _type_
         _description_
     sigma : _type_, optional
         _description_, by default 1.
     truncate : _type_, optional
         _description_, by default 4.
     """
 
-    V=data.copy()
-    V[np.isnan(data)]=0
-    VV=ndimage.gaussian_filter(V,sigma=sigma,truncate=truncate)
-
-    W=0*data.copy()+1
-    W[np.isnan(data)]=0
-    WW=ndimage.gaussian_filter(W,sigma=sigma,truncate=truncate)
+    V = data.copy()
+    V[np.isnan(data)] = 0
+    VV = ndimage.gaussian_filter(V, sigma=sigma, truncate=truncate)
+
+    W = 0 * data.copy() + 1
+    W[np.isnan(data)] = 0
+    WW = ndimage.gaussian_filter(W, sigma=sigma, truncate=truncate)
+
+    return VV / WW
 
-    return VV/WW
 
 def clean_header(header_dict):
-    return {key: value for key, value in header_dict.items() if not isinstance(value, (list, tuple)) and key.isupper()}
+    return {
+        key: value
+        for key, value in header_dict.items()
+        if not isinstance(value, (list, tuple)) and key.isupper()
+    }
 
 
 def easy_median(images):
     # To avoid memory errors, we split the median computation in 50
     images = np.array(images)
     shape_divisors = divisors(images.shape[1])
     n = shape_divisors[np.argmin(np.abs(50 - shape_divisors))]
-    return np.concatenate([np.nanmedian(im, axis=0) for im in np.split(images, n, axis=1)])
+    return np.concatenate(
+        [np.nanmedian(im, axis=0) for im in np.split(images, n, axis=1)]
+    )
 
 
 def image_in_xarray(image, xarr, name="stack", stars=False):
     xarr.attrs.update(header_to_cdf4_dict(image.header))
-    xarr.attrs.update(dict(
-        telescope=image.telescope.name,
-        filter=image.header.get(image.telescope.keyword_filter, ""),
-        exptime=image.header.get(image.telescope.keyword_exposure_time, ""),
-        name=image.header.get(image.telescope.keyword_object, ""),
-    ))
+    xarr.attrs.update(
+        dict(
+            telescope=image.telescope.name,
+            filter=image.header.get(image.telescope.keyword_filter, ""),
+            exptime=image.header.get(image.telescope.keyword_exposure_time, ""),
+            name=image.header.get(image.telescope.keyword_object, ""),
+        )
+    )
 
     if image.telescope.keyword_observation_date in image.header:
         date = image.header[image.telescope.keyword_observation_date]
     else:
         date = Time(image.header[image.telescope.keyword_jd], format="jd").datetime
 
     xarr.attrs.update(dict(date=format_iso_date(date).isoformat()))
-    xarr.coords[name] = (('w', 'h'), image.data)
+    xarr.coords[name] = (("w", "h"), image.data)
 
     xarr = xarr.assign_coords(time=xarr.jd_utc)
     xarr = xarr.sortby("time")
     xarr.attrs["time_format"] = "jd_utc"
-    
+
     if stars:
         xarr = xarr.assign_coords(stars=(("star", "n"), image.stars_coords))
 
-    
     return xarr
 
+
 def check_skycoord(skycoord):
     """
     Check that skycoord is either:
     - a list of int (interpreted as deg)
     - a str (interpreted as houranlgle, deg)
     - a SkyCoord object
 
@@ -457,69 +367,171 @@
     return skycoord
 
 
 def gaia_query(center, fov, *args, limit=10000, circular=True):
     """
     https://gea.esac.esa.int/archive/documentation/GEDR3/Gaia_archive/chap_datamodel/sec_dm_main_tables/ssec_dm_gaia_source.html
     """
-    
+
     from astroquery.gaia import Gaia
-    
+
     if isinstance(center, SkyCoord):
         ra = center.ra.to(u.deg).value
         dec = center.dec.to(u.deg).value
-    
+
     if not isinstance(fov, u.Quantity):
         fov = fov * u.deg
-    
+
     if fov.ndim == 1:
         ra_fov, dec_fov = fov.to(u.deg).value
     else:
         ra_fov = dec_fov = fov.to(u.deg).value
 
-    radius = np.min([ra_fov, dec_fov])/2
+    radius = np.min([ra_fov, dec_fov]) / 2
 
-    fields = ','.join(args) if isinstance(args, (tuple, list)) else args
+    fields = ",".join(args) if isinstance(args, (tuple, list)) else args
 
     if circular:
-        job = Gaia.launch_job(f"select top {limit} {fields} from gaiadr2.gaia_source where "
-                            "1=CONTAINS("
-                            f"POINT('ICRS', {ra}, {dec}), "
-                            f"CIRCLE('ICRS',ra, dec, {radius}))"
-                            "order by phot_g_mean_mag")
+        job = Gaia.launch_job(
+            f"select top {limit} {fields} from gaiadr2.gaia_source where "
+            "1=CONTAINS("
+            f"POINT('ICRS', {ra}, {dec}), "
+            f"CIRCLE('ICRS',ra, dec, {radius}))"
+            "order by phot_g_mean_mag"
+        )
     else:
-        job = Gaia.launch_job(f"select top {limit} {fields} from gaiadr2.gaia_source where "
-                    f"ra BETWEEN {ra-ra_fov/2} AND {ra+ra_fov/2} AND "
-                    f"dec BETWEEN {dec-dec_fov/2} AND {dec+dec_fov/2} "
-                    "order by phot_g_mean_mag") 
+        job = Gaia.launch_job(
+            f"select top {limit} {fields} from gaiadr2.gaia_source where "
+            f"ra BETWEEN {ra-ra_fov/2} AND {ra+ra_fov/2} AND "
+            f"dec BETWEEN {dec-dec_fov/2} AND {dec+dec_fov/2} "
+            "order by phot_g_mean_mag"
+        )
 
     return job.get_results()
 
-def sparsify(stars, radius):
 
+def sparsify(stars, radius):
     _stars = stars.copy()
     deleted_stars = np.zeros([], dtype=int)
     sparse_stars = []
-    
+
     for i, s in enumerate(_stars):
         if not i in deleted_stars:
-            distances = np.linalg.norm(_stars-s, axis=1)
-            idxs = np.flatnonzero(distances<radius)
+            distances = np.linalg.norm(_stars - s, axis=1)
+            idxs = np.flatnonzero(distances < radius)
             sparse_stars.append(s)
             deleted_stars = np.hstack([deleted_stars, idxs])
-    
+
     return np.array(sparse_stars)
 
+
 def full_class_name(o):
     # https://stackoverflow.com/questions/2020014/get-fully-qualified-class-name-of-an-object-in-python
     klass = o.__class__
     module = klass.__module__
-    if module == 'builtins':
-        return klass.__qualname__ # avoid outputs like 'builtins.str'
-    return module + '.' + klass.__qualname__
+    if module == "builtins":
+        return klass.__qualname__  # avoid outputs like 'builtins.str'
+    return module + "." + klass.__qualname__
 
 
 def binn2D(arr, factor):
     new_shape = np.array(arr.shape) // factor
-    shape = (new_shape[0], factor,
-             new_shape[1], factor)
-    return np.mean(arr.reshape(shape).mean(-1), 1)
+    shape = (new_shape[0], factor, new_shape[1], factor)
+    return np.mean(arr.reshape(shape).mean(-1), 1)
+
+
+from functools import partial
+
+import numpy as np
+from scipy.spatial import KDTree
+from skimage.transform import AffineTransform as skAT
+from twirl import utils as tutils
+
+
+def distance(p1, p2):
+    return np.sqrt(np.power(p1[0] - p2[0], 2) + np.power(p1[1] - p2[1], 2))
+
+
+def distances(coords, coord):
+    return [
+        np.sqrt(((coord[0] - x) ** 2 + (coord[1] - y) ** 2))
+        for x, y in zip(coords[0].flatten(), coords[1].flatten())
+    ]
+
+
+def cross_match(S1, S2, tolerance=10, return_idxs=False, none=True):
+    # cleaning
+    s1 = S1.copy()
+    s2 = S2.copy()
+
+    s1[np.any(np.isnan(s1), 1)] = (1e15, 1e15)
+    s2[np.any(np.isnan(s2), 1)] = (1e15, 1e15)
+
+    # matching
+    matches = []
+
+    for i, s in enumerate(s1):
+        distances = np.linalg.norm(s - s2, axis=1)
+        closest = np.argmin(distances)
+        if distances[closest] < tolerance:
+            matches.append([i, closest])
+        else:
+            if none:
+                matches.append([i, np.nan])
+
+    matches = np.array(matches)
+
+    if return_idxs:
+        return matches
+    else:
+        if len(matches) > 0:
+            return s1[matches[:, 0]], s2[matches[:, 1]]
+        else:
+            return np.array([]), np.array([])
+
+
+def moments(data):
+    """Returns (height, x, y, width_x, width_y)
+    the gaussian parameters of a 2D distribution by calculating its
+    moments"""
+    height = data.max()
+    background = data.min()
+    data = data - np.min(data)
+    total = data.sum()
+    x, y = np.indices(data.shape)
+    x = (x * data).sum() / total
+    y = (y * data).sum() / total
+    col = data[:, int(y)]
+    width_x = np.sqrt(abs((np.arange(col.size) - y) ** 2 * col).sum() / col.sum())
+    row = data[int(x), :]
+    width_y = np.sqrt(abs((np.arange(row.size) - x) ** 2 * row).sum() / row.sum())
+    width_x /= gaussian_sigma_to_fwhm
+    width_y /= gaussian_sigma_to_fwhm
+    return {
+        "amplitude": height,
+        "x": x,
+        "y": y,
+        "sigma_x": width_x,
+        "sigma_y": width_y,
+        "background": background,
+        "theta": 0.0,
+    }
+
+
+def get_all_blocks():
+    """Returns a list of all block names from prose (exposed in blocks.__init__.py)
+
+    Returns
+    -------
+    list
+        List of all block names
+    """
+    from prose import blocks
+
+    blocks = [
+        getattr(blocks, b)
+        for b in dir(blocks)
+        if isinstance(getattr(blocks, b), type)
+        and issubclass(getattr(blocks, b), blocks.Block)
+    ]
+
+    return blocks
```

### Comparing `prose-2.3.0/prose/visualization.py` & `prose-3.0.0/prose/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import matplotlib
-from .utils import binning
-import numpy as np
-from . import utils
 import matplotlib.offsetbox
-from matplotlib.lines import Line2D
-from matplotlib import patches
-from astropy.io import fits
-from mpl_toolkits import axes_grid1
-from mpl_toolkits.axes_grid1.inset_locator import zoomed_inset_axes,  inset_axes
+import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
-from skimage.transform import resize
+import numpy as np
+from astropy.io import fits
+from matplotlib import patches
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
-from matplotlib.ticker import AutoMinorLocator
 from matplotlib.legend_handler import HandlerPatch
-import matplotlib.patches as mpatches
-from .models import transit
+from matplotlib.lines import Line2D
+from matplotlib.ticker import AutoMinorLocator
+from mpl_toolkits import axes_grid1
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes, zoomed_inset_axes
+from skimage.transform import resize
+
+from prose import utils
 
 
 def plot(
     time,
     flux,
     error=None,
     bins=0.005,
@@ -30,15 +29,17 @@
     label=None,
     binlabel=None,
 ):
     plt.plot(time, flux, ".", color=color, alpha=alpha, zorder=0, label=label)
 
     if bins is not None:
         blc = binning(time, flux, bins=bins, error=error, std=std)
-        plt.errorbar(*blc, fmt=".", zorder=1, color=bincolor, alpha=binalpha, label=binlabel)
+        plt.errorbar(
+            *blc, fmt=".", zorder=1, color=bincolor, alpha=binalpha, label=binlabel
+        )
 
 
 def plot_marginal_model(data, model, cmap="inferno", c="blueviolet"):
     x, y = np.indices(data.shape)
 
     plt.subplot(131)
     plt.imshow(utils.z_scale(data), alpha=1, cmap=cmap)
@@ -90,58 +91,79 @@
                 color="w",
             )
 
             if stars is not None:
                 for j, s in enumerate(stars_in[i][0]):
                     ax.plot(*stars_in[i][1][j], "x", c="C0")
         else:
-            ax.axis('off')
+            ax.axis("off")
 
 
 class AnchoredHScaleBar(matplotlib.offsetbox.AnchoredOffsetbox):
-
-    def __init__(self, size=1, extent=0.03, label="", loc=2, ax=None,
-                 pad=0.4, borderpad=0.5, ppad=0, sep=2, prop=None,
-                 frameon=True, linekw={}, **kwargs):
-
+    def __init__(
+        self,
+        size=1,
+        extent=0.03,
+        label="",
+        loc=2,
+        ax=None,
+        pad=0.4,
+        borderpad=0.5,
+        ppad=0,
+        sep=2,
+        prop=None,
+        frameon=True,
+        linekw={},
+        **kwargs,
+    ):
         if not ax:
             ax = plt.gca()
 
         trans = ax.get_xaxis_transform()
         size_bar = matplotlib.offsetbox.AuxTransformBox(trans)
         line = Line2D([0, size], [0, 0], **linekw)
-        vline1 = Line2D([0, 0], [-extent / 2., extent / 2.], **linekw)
-        vline2 = Line2D([size, size], [-extent / 2., extent / 2.], **linekw)
+        vline1 = Line2D([0, 0], [-extent / 2.0, extent / 2.0], **linekw)
+        vline2 = Line2D([size, size], [-extent / 2.0, extent / 2.0], **linekw)
         size_bar.add_artist(line)
         size_bar.add_artist(vline1)
         size_bar.add_artist(vline2)
-        txt = matplotlib.offsetbox.TextArea(label, minimumdescent=False, textprops=dict(color=linekw.get("color", "k")))
-        self.vpac = matplotlib.offsetbox.VPacker(children=[size_bar, txt],
-                                                 align="center", pad=ppad, sep=sep)
-        matplotlib.offsetbox.AnchoredOffsetbox.__init__(self, loc, pad=pad,
-                                                        borderpad=borderpad, child=self.vpac, prop=prop,
-                                                        frameon=frameon,
-                                                        **kwargs)
+        txt = matplotlib.offsetbox.TextArea(
+            label, minimumdescent=False, textprops=dict(color=linekw.get("color", "k"))
+        )
+        self.vpac = matplotlib.offsetbox.VPacker(
+            children=[size_bar, txt], align="center", pad=ppad, sep=sep
+        )
+        matplotlib.offsetbox.AnchoredOffsetbox.__init__(
+            self,
+            loc,
+            pad=pad,
+            borderpad=borderpad,
+            child=self.vpac,
+            prop=prop,
+            frameon=frameon,
+            **kwargs,
+        )
 
 
 def multiplot(
-        data,
-        bins=0.005,
-        std=True,
-        color="gainsboro",
-        bincolor="k",
-        alpha=0.6,
-        binalpha=0.8,
-        w=4,
-        show=None,
-        hide=None,
-        ylim=None,
-        size=None,
-        labels=None,
-        force_width=True):
+    data,
+    bins=0.005,
+    std=True,
+    color="gainsboro",
+    bincolor="k",
+    alpha=0.6,
+    binalpha=0.8,
+    w=4,
+    show=None,
+    hide=None,
+    ylim=None,
+    size=None,
+    labels=None,
+    force_width=True,
+):
     """Plot multiple x, y with some shared axis
 
     Parameters
     ----------
     data : list
         a list of (x, y)
     w : int, optional
@@ -160,99 +182,107 @@
         bin size, by default 0.005
     force_width : bool, optional
         whether to occupy all width, by default True
     """
 
     if size is None:
         size = (4, 3)
-    
+
     if isinstance(data[0], dict):
         data = [[d["time"], d["lc"]] for d in data]
-    
+
     if show is None:
         show = np.arange(0, len(data))
     if hide is None:
         hide = []
-    
+
     indexes = np.setdiff1d(show, hide)
 
     H = np.ceil(len(indexes) / w).astype(int)
     if not force_width:
         w = np.min([len(indexes), w])
     fig, axes = plt.subplots(H, w, figsize=(w * size[0], H * size[1]))
-    fig.patch.set_facecolor('white')
+    fig.patch.set_facecolor("white")
     max_duration = np.max([jd.max() - jd.min() for jd, _ in [data[i] for i in indexes]])
-    
+
     for _i, ax in enumerate(axes.flat if len(indexes) > 1 else [axes]):
         if _i < len(indexes):
             i = indexes[_i]
             plt.sca(ax)
             jd, lc = data[i]
-            center = jd.min() + (jd.max() - jd.min())/2
+            center = jd.min() + (jd.max() - jd.min()) / 2
 
-            plot(jd, lc, bins=bins, std=std, bincolor=bincolor, color=color, alpha=alpha, binalpha=binalpha)
+            plot(
+                jd,
+                lc,
+                bins=bins,
+                std=std,
+                bincolor=bincolor,
+                color=color,
+                alpha=alpha,
+                binalpha=binalpha,
+            )
             if ylim is not None:
                 plt.ylim(ylim)
 
-            plt.xlim(center - (max_duration/2), center + (max_duration/2))
+            plt.xlim(center - (max_duration / 2), center + (max_duration / 2))
             # ax.get_legend().remove()
-            if i%w != 0 and ylim is not None:
+            if i % w != 0 and ylim is not None:
                 ax.tick_params(labelleft=False)
             ax.set_title(None)
             if labels is not None:
                 text = str(labels[i])
             else:
                 text = str(i)
             ax.annotate(
-                    text,
-                    xy=(0.05, 0.05),
-                    xycoords="axes fraction",
-                    textcoords="axes fraction",
-                    ha="left",
-                    va="bottom",
-                    fontsize=12,
-                    color="k",
-                )
+                text,
+                xy=(0.05, 0.05),
+                xycoords="axes fraction",
+                textcoords="axes fraction",
+                ha="left",
+                va="bottom",
+                fontsize=12,
+                color="k",
+            )
         else:
-            ax.axis('off')
+            ax.axis("off")
 
     plt.tight_layout()
 
 
 def bokeh_style(xminor=True, yminor=True, axes=None):
-    
     if axes is None:
         axes = plt.gcf().axes
     elif not isinstance(axes, list):
         axes = [axes]
-    
+
     for axe in axes:
         axe.set_axisbelow(True)
         axe.set_titleweight = 500
         axe.tick_params(gridOn=True, grid_color="whitesmoke")
         if xminor:
             axe.xaxis.set_minor_locator(AutoMinorLocator())
         if yminor:
             axe.yaxis.set_minor_locator(AutoMinorLocator())
         axe.tick_params(direction="inout", which="both")
-        if hasattr(axe, 'spines'):
-            axe.spines['bottom'].set_color('#545454')
-            axe.spines['left'].set_color('#545454')
-            axe.spines['top'].set_color('#DBDBDB')
-            axe.spines['right'].set_color('#DBDBDB')
-            axe.spines['top'].set_linewidth(1)
-            axe.spines['right'].set_linewidth(1)
+        if hasattr(axe, "spines"):
+            axe.spines["bottom"].set_color("#545454")
+            axe.spines["left"].set_color("#545454")
+            axe.spines["top"].set_color("#DBDBDB")
+            axe.spines["right"].set_color("#DBDBDB")
+            axe.spines["top"].set_linewidth(1)
+            axe.spines["right"].set_linewidth(1)
 
 
 def paper_style(axes=None):
     if axes is None:
         axes = plt.gcf().axes
     elif not isinstance(axes, list):
         axes = [axes]
-    
+
     for axe in axes:
         axe.set_axisbelow(True)
         axe.set_titleweight = 500
         axe.tick_params(gridOn=True, grid_color="whitesmoke")
         axe.xaxis.set_minor_locator(AutoMinorLocator())
         axe.yaxis.set_minor_locator(AutoMinorLocator())
         axe.xaxis.set_ticks_position("both")
@@ -267,23 +297,28 @@
     pad = axes_grid1.axes_size.Fraction(pad_fraction, width)
     current_ax = plt.gca()
     cax = divider.append_axes("right", size=width, pad=pad)
     plt.sca(current_ax)
     return im.axes.figure.colorbar(im, cax=cax, **kwargs)
 
 
-def show_stars(image, stars=None, highlight=None, size=15, options={}, flip=None, color=None, contrast=0.05):
-
+def show_stars(
+    image,
+    stars=None,
+    highlight=None,
+    size=15,
+    options={},
+    flip=None,
+    color=None,
+    contrast=0.05,
+):
     if color is None:
         color = np.array([131, 220, 255]) / 255
 
-    _options = {
-        "aperture_color": "seagreen",
-        "aperture_ls": "--"
-    }
+    _options = {"aperture_color": "seagreen", "aperture_ls": "--"}
     _options.update(options)
 
     if isinstance(image, str):
         image = fits.getdata(image)
 
     image_size = np.array(np.shape(image))[::-1]
 
@@ -296,56 +331,72 @@
     else:
         image = utils.z_scale(image, c=contrast)
 
     ax = fig.add_subplot(111)
     ax.imshow(image, cmap="Greys_r")
     plt.title("Stack image", loc="left")
 
-    size_factor = size/7
-    fontsize = min(size_factor, 1)*15
-    label_yoffset = min(size_factor, 1)*15
+    size_factor = size / 7
+    fontsize = min(size_factor, 1) * 15
+    label_yoffset = min(size_factor, 1) * 15
 
     if stars is not None:
         if highlight is not None:
-
             plt.plot(
                 stars[highlight, 0],
                 stars[highlight, 1],
                 "o",
-                markersize=14*size_factor,
+                markersize=14 * size_factor,
                 markeredgecolor=color,
                 markerfacecolor="none",
                 label="target",
             )
             plt.annotate(
-                highlight, xy=[stars[highlight][0], stars[highlight][1] + label_yoffset],
-                color=color, fontsize=fontsize, ha='center', va='top'
+                highlight,
+                xy=[stars[highlight][0], stars[highlight][1] + label_yoffset],
+                color=color,
+                fontsize=fontsize,
+                ha="center",
+                va="top",
             )
 
         else:
             highlight = -1
 
         other_stars = np.arange(len(stars))
 
         other_stars = np.setdiff1d(other_stars, highlight)
 
         plt.plot(
             stars[other_stars, 0],
             stars[other_stars, 1],
             "o",
-            markersize=14*size_factor,
+            markersize=14 * size_factor,
             markeredgecolor=color,
             markerfacecolor="none",
-            alpha=0.4 if highlight >= 0 else 1
+            alpha=0.4 if highlight >= 0 else 1,
         )
 
         plt.tight_layout()
 
 
-def plot_marks(x, y, label=None, position="bottom", offset=7, fontsize=12, color=[0.51, 0.86, 1.], ms=12, n=None, inside=True, alpha=1, ax=None):
+def plot_marks(
+    x,
+    y,
+    label=None,
+    position="bottom",
+    offset=7,
+    fontsize=12,
+    color=[0.51, 0.86, 1.0],
+    ms=12,
+    n=None,
+    inside=True,
+    alpha=1,
+    ax=None,
+):
     y_offset = ms + offset
 
     if position == "top":
         y_offset *= -1
 
     if not isinstance(x, (list, np.ndarray, tuple)):
         x = np.array([x])
@@ -356,24 +407,25 @@
             label = np.array([label])
     else:
         if label is True:
             label = np.arange(len(x))
         elif label is not None:
             label = np.array(label)
 
-
     if ax is None:
         ax = plt.gcf().axes[0]
 
     if inside:
         ax = ax
         xlim, ylim = np.array(ax.get_xlim()), np.array(ax.get_ylim())
         xlim.sort()
         ylim.sort()
-        within = np.argwhere(np.logical_and.reduce([xlim[0] < x,  x < xlim[1],  ylim[0] < y,  y < ylim[1]])).flatten()
+        within = np.argwhere(
+            np.logical_and.reduce([xlim[0] < x, x < xlim[1], ylim[0] < y, y < ylim[1]])
+        ).flatten()
         x = x[within]
         y = y[within]
         if label is not None:
             print
             label = label[within]
 
     if n is not None:
@@ -387,40 +439,43 @@
 
     for _x, _y, _label in zip(x, y, label):
         circle = mpatches.Circle((_x, _y), ms, fill=None, ec=color, alpha=alpha)
         ax = plt.gca()
         ax.add_artist(circle)
         f = 5
         if _label is not None:
-            plt.annotate(_label, xy=[_x, _y - y_offset], color=color, ha='center', fontsize=fontsize, alpha=alpha,
-                         va="top" if position == "bottom" else "bottom")
+            plt.annotate(
+                _label,
+                xy=[_x, _y - y_offset],
+                color=color,
+                ha="center",
+                fontsize=fontsize,
+                alpha=alpha,
+                va="top" if position == "bottom" else "bottom",
+            )
 
 
 def fancy_show_stars(
-        image,
-        stars,
-        ref_stars=None,
-        target=None,
-        size=15,
-        pixel_scale=None,
-        contrast=0.05,
-        aperture=None,
-        marker_color=np.array([131, 220, 255]) / 255,
-        proper_motion=False,
-        n_stars=None,
-        flip=False,
-        view="all",
-        zoom=True,
-        options={},
+    image,
+    stars,
+    ref_stars=None,
+    target=None,
+    size=15,
+    pixel_scale=None,
+    contrast=0.05,
+    aperture=None,
+    marker_color=np.array([131, 220, 255]) / 255,
+    proper_motion=False,
+    n_stars=None,
+    flip=False,
+    view="all",
+    zoom=True,
+    options={},
 ):
-
-    _options = {
-        "aperture_color": "seagreen",
-        "aperture_ls": "--"
-    }
+    _options = {"aperture_color": "seagreen", "aperture_ls": "--"}
     _options.update(options)
 
     marker_size = 9
 
     if isinstance(image, str):
         image = fits.getdata(image)
 
@@ -439,175 +494,258 @@
     plt.title("Stack image", loc="left")
 
     size_factor = size / 15
     fontsize = min(size_factor, 1) * 15
     label_yoffset = min(size_factor, 1) * 30
 
     if view == "all":
-
         for i, coord in enumerate(stars):
-            circle = mpatches.Circle(coord, marker_size, fill=None, ec=marker_color, )
+            circle = mpatches.Circle(
+                coord,
+                marker_size,
+                fill=None,
+                ec=marker_color,
+            )
             ax = plt.gca()
             ax.add_artist(circle)
-            plt.annotate(str(i),
-                         xy=[coord[0], coord[1] + marker_size + 8],
-                         color=marker_color,
-                         ha='center', fontsize=12, va='top')
+            plt.annotate(
+                str(i),
+                xy=[coord[0], coord[1] + marker_size + 8],
+                color=marker_color,
+                ha="center",
+                fontsize=12,
+                va="top",
+            )
 
     if ref_stars is not None:
-        circle = mpatches.Circle(stars[target, :], marker_size, fill=None, ec=marker_color, label="target")
+        circle = mpatches.Circle(
+            stars[target, :], marker_size, fill=None, ec=marker_color, label="target"
+        )
         ax = plt.gca()
         ax.add_artist(circle)
-        plt.annotate(target, xy=[stars[target][0], stars[target][1] + marker_size + 8],
-                     color=marker_color, ha='center', fontsize=12, va='top')
+        plt.annotate(
+            target,
+            xy=[stars[target][0], stars[target][1] + marker_size + 8],
+            color=marker_color,
+            ha="center",
+            fontsize=12,
+            va="top",
+        )
 
         plt.imshow(image, cmap="Greys_r")
 
         for i in ref_stars:
-            circle = mpatches.Circle(stars[i, :], marker_size, fill=None, ec="yellow", label="comparison")
+            circle = mpatches.Circle(
+                stars[i, :], marker_size, fill=None, ec="yellow", label="comparison"
+            )
             ax.add_artist(circle)
-            plt.annotate(str(i), xy=[stars[i][0], stars[i][1] + marker_size+8], color="yellow",
-                         fontsize=12,
-                         ha='center',
-                         va='top')
+            plt.annotate(
+                str(i),
+                xy=[stars[i][0], stars[i][1] + marker_size + 8],
+                color="yellow",
+                fontsize=12,
+                ha="center",
+                va="top",
+            )
 
         other_stars = np.arange(len(stars))
 
         other_stars = np.setdiff1d(other_stars, target)
         other_stars = np.setdiff1d(other_stars, ref_stars)
 
         for i in other_stars:
-            circle = mpatches.Circle(stars[i, :], marker_size, fill=None, ec=marker_color, label="comparison",
-                                     alpha=0.4)
+            circle = mpatches.Circle(
+                stars[i, :],
+                marker_size,
+                fill=None,
+                ec=marker_color,
+                label="comparison",
+                alpha=0.4,
+            )
             ax.add_artist(circle)
 
     plt.tight_layout()
 
     if pixel_scale is not None:
-        ob = AnchoredHScaleBar(size=60 / pixel_scale, label="1'", loc=4, frameon=False, extent=0,
-                               pad=0.6, sep=4, linekw=dict(color="white", linewidth=0.8))
+        ob = AnchoredHScaleBar(
+            size=60 / pixel_scale,
+            label="1'",
+            loc=4,
+            frameon=False,
+            extent=0,
+            pad=0.6,
+            sep=4,
+            linekw=dict(color="white", linewidth=0.8),
+        )
         ax.add_artist(ob)
 
     if target is not None and zoom:
-        with plt.rc_context({
-            'axes.edgecolor': "white",
-            'xtick.color': "white",
-            'ytick.color': "white"
-        }):
+        with plt.rc_context(
+            {"axes.edgecolor": "white", "xtick.color": "white", "ytick.color": "white"}
+        ):
             x, y = stars[target]
             rect = patches.Rectangle(
                 (x - 80, y - 80),
-                160, 160, linewidth=1,
-                edgecolor='white',
-                facecolor='none',
-                alpha=0.3)
+                160,
+                160,
+                linewidth=1,
+                edgecolor="white",
+                facecolor="none",
+                alpha=0.3,
+            )
 
             ax.add_patch(rect)
             axins = zoomed_inset_axes(ax, 2.5, loc=1)
             axins.imshow(image, cmap="Greys_r", origin="upper")
             if aperture is not None:
                 ap = aperture / 2
                 aperture = patches.Circle(
                     (x, y),
-                    ap, linewidth=1,
+                    ap,
+                    linewidth=1,
                     ls=_options["aperture_ls"],
                     edgecolor=_options["aperture_color"],
-                    facecolor='none',
-                    alpha=1)
+                    facecolor="none",
+                    alpha=1,
+                )
                 axins.add_patch(aperture)
             axins.set_xlim([x - 80, x + 80])
             axins.set_ylim([y + 80, y - 80])
 
             if pixel_scale is not None:
-                obin = AnchoredHScaleBar(size=15 / pixel_scale, label="15\"", loc=4,
-                                         frameon=False, extent=0, pad=0.6, sep=4,
-                                         linekw=dict(color="white", linewidth=0.8))
+                obin = AnchoredHScaleBar(
+                    size=15 / pixel_scale,
+                    label='15"',
+                    loc=4,
+                    frameon=False,
+                    extent=0,
+                    pad=0.6,
+                    sep=4,
+                    linekw=dict(color="white", linewidth=0.8),
+                )
                 axins.add_artist(obin)
 
     return fig
 
 
 def plot_rms(fluxes_lcs, diff_lcs, target=None, highlights=None, bins=0.005):
     fluxes_lcs.set_best_aperture_id(diff_lcs.best_aperture_id)
     lcs = diff_lcs.fluxes
     errors = diff_lcs.errors
     fluxes = fluxes_lcs.fluxes
 
     time = diff_lcs[0].time.copy()
 
     fluxes_median = np.median(fluxes, axis=1)
-    stds_median = np.array([np.median(utils.binning(time, lc, bins, error=error, std=True)[2]) for lc, error in zip(lcs, errors)])
+    stds_median = np.array(
+        [
+            np.median(utils.binning(time, lc, bins, error=error, std=True)[2])
+            for lc, error in zip(lcs, errors)
+        ]
+    )
     stds_median /= fluxes_median
-    errors_median = np.array([np.median(utils.binning(time, lc, bins, error=error, std=False)[2]) for lc, error in zip(lcs, errors)])
+    errors_median = np.array(
+        [
+            np.median(utils.binning(time, lc, bins, error=error, std=False)[2])
+            for lc, error in zip(lcs, errors)
+        ]
+    )
     errors_median /= fluxes_median
 
     plt.grid(color="whitesmoke", zorder=0)
 
     if highlights is not None:
         for c in highlights:
             comp_flux_median = fluxes_median[c]
             comp_std_median = stds_median[c]
             plt.plot(comp_flux_median, comp_std_median, ".", c="gold", zorder=5)
-        plt.plot(comp_flux_median, comp_std_median, ".", c="gold", label="comparison stars", zorder=5)
+        plt.plot(
+            comp_flux_median,
+            comp_std_median,
+            ".",
+            c="gold",
+            label="comparison stars",
+            zorder=5,
+        )
 
     if target is not None:
         target_flux_median = fluxes_median[target]
         target_std_median = stds_median[target]
-        plt.plot(target_flux_median, target_std_median, ".", c="C0", label="target",zorder=6, ms=10)
+        plt.plot(
+            target_flux_median,
+            target_std_median,
+            ".",
+            c="C0",
+            label="target",
+            zorder=6,
+            ms=10,
+        )
 
     idxs = np.argsort(fluxes_median)
 
     stds_median = stds_median[idxs]
     errors_median = errors_median[idxs]
     fluxes_median = fluxes_median[idxs]
 
     plt.title("Light curves binned rms", loc="left")
     plt.plot(fluxes_median, stds_median, ".", c="darkgrey", zorder=4, label="others")
-    plt.plot(fluxes_median, errors_median, c="k", lw=1, zorder=7, label="CCD equation", alpha=0.8)
+    plt.plot(
+        fluxes_median,
+        errors_median,
+        c="k",
+        lw=1,
+        zorder=7,
+        label="CCD equation",
+        alpha=0.8,
+    )
     plt.legend()
-    plt.yscale('log')
-    plt.xscale('log')
+    plt.yscale("log")
+    plt.xscale("log")
     plt.xlabel("ADUs")
     plt.ylabel("diff. flux rms ({} JD bin)".format(bins))
 
-    fluxes_median = fluxes_median[fluxes_median>0]
+    fluxes_median = fluxes_median[fluxes_median > 0]
     plt.xlim(fluxes_median.min(), fluxes_median.max())
 
 
 def gif_image_array(image, factor=0.25):
-    return (utils.z_scale(
-        resize(
-            image.astype(float),
-            (np.array(np.shape(image)) * factor).astype(int),
-            anti_aliasing=False,
-        )) * 255).astype("uint8")
+    return (
+        utils.z_scale(
+            resize(
+                image.astype(float),
+                (np.array(np.shape(image)) * factor).astype(int),
+                anti_aliasing=False,
+            )
+        )
+        * 255
+    ).astype("uint8")
 
 
 def fancy_gif_image_array(image, median_psf, factor=0.25):
-
     fig = plt.figure(frameon=False)
     canvas = FigureCanvas(fig)
     ax = fig.add_axes([0, 0, 1, 1])
-    ax.axis('off')
+    ax.axis("off")
     gif_im = utils.z_scale(
         resize(
             image,
             np.array(np.shape(image)).astype(int) * factor,
             anti_aliasing=True,
-        ))
+        )
+    )
     ax.imshow(gif_im, cmap="Greys_r")
     axins = inset_axes(ax, width=1, height=1, loc=3)
-    axins.axis('off')
+    axins.axis("off")
     axins.imshow(median_psf)
     canvas.draw()
     width, height = (fig.get_size_inches() * fig.get_dpi()).astype(int)
-    return np.fromstring(canvas.tostring_rgb(), dtype='uint8').reshape(height, width, 3)
+    return np.fromstring(canvas.tostring_rgb(), dtype="uint8").reshape(height, width, 3)
 
 
-def array_to_tex(a, fmt='{: 0.3f}', dim=True):
+def array_to_tex(a, fmt="{: 0.3f}", dim=True):
     """Display a LaTeX matrix in notebook
 
     Parameters
     ----------
     a : np.ndarray
         matric to display
     fmt : str, optional
@@ -616,42 +754,44 @@
         show matrix dim, by default True
 
     Raises
     ------
     ValueError
         [description]
     """
-    from IPython.display import display, Math
+    from IPython.display import Math, display
+
     if isinstance(a, tuple):
         a = np.array(a)
-        
+
     shape = a.shape
     if len(shape) > 2:
-        raise ValueError('bmatrix can at most display two dimensions')
-        
-    with np.printoptions(formatter={'float': fmt.format}):
-        lines = str(a).replace('[', '').replace(']', '').splitlines()
-        rv = [r'\begin{bmatrix}']
-        rv += ['  ' + ' & '.join(l.split()) + r'\\' for l in lines]
-        rv +=  [r'\end{bmatrix}']
+        raise ValueError("bmatrix can at most display two dimensions")
+
+    with np.printoptions(formatter={"float": fmt.format}):
+        lines = str(a).replace("[", "").replace("]", "").splitlines()
+        rv = [r"\begin{bmatrix}"]
+        rv += ["  " + " & ".join(l.split()) + r"\\" for l in lines]
+        rv += [r"\end{bmatrix}"]
     if dim:
         if len(shape) == 2:
-            teX_math = "M_{" + str(shape[0]) + " \\times "+ str(shape[1]) + "}="
+            teX_math = "M_{" + str(shape[0]) + " \\times " + str(shape[1]) + "}="
         elif len(shape) == 1:
             teX_math = "a_{" + str(shape[0]) + "}="
     else:
         teX_math = ""
-        
-    teX_math += '\n'.join(rv)
-    
+
+    teX_math += "\n".join(rv)
+
     display(Math(r"{}".format(teX_math)))
 
 
 def print_tex(tex):
-    from IPython.display import display, Math
+    from IPython.display import Math, display
+
     display(Math(r"{}".format(tex)))
 
 
 def plot_expected_transit(time, epoch, period, duration, depth=None, color="gainsboro"):
     tmax = time.max()
     t_epoch = tmax - epoch
     t0 = t_epoch % period
@@ -660,66 +800,79 @@
 
     plt.axvspan(ingress, egress, color=color, alpha=0.02, zorder=-1)
     plt.axvline(ingress, color=color, alpha=0.3, zorder=-1, label="expected transit")
     plt.axvline(egress, color=color, alpha=0.3, zorder=-1)
 
     if depth is not None:
         model = transit(time, epoch, duration, depth, period=period).flatten()
-        plt.plot(time, model + 1., c="grey")
+        plt.plot(time, model + 1.0, c="grey")
 
 
 def rename_tab(name):
     """Rename a notebook tab
 
     Parameters
     ----------
     name : str
         name to be used
     """
-    from IPython.display import display, Javascript
+    from IPython.display import Javascript, display
+
     return Javascript('document.title="{}"'.format(name))
 
 
 def plot_section(y, s, t0, duration, c="C0", y0=1, offset=0.002):
-    plt.hlines(y , t0 - duration/2, t0+duration/2, clip_on=False, zorder=100, lw=2, alpha=0.5, color=c)
+    plt.hlines(
+        y,
+        t0 - duration / 2,
+        t0 + duration / 2,
+        clip_on=False,
+        zorder=100,
+        lw=2,
+        alpha=0.5,
+        color=c,
+    )
     plt.text(t0, y + offset, s, ha="center", color=c, fontsize=11, alpha=0.8)
-    plt.vlines(t0 - duration/2, y, y0, alpha=0.15, color=c)
-    plt.vlines(t0 + duration/2, y, y0, alpha=0.15, color=c)
+    plt.vlines(t0 - duration / 2, y, y0, alpha=0.15, color=c)
+    plt.vlines(t0 + duration / 2, y, y0, alpha=0.15, color=c)
     ymin = plt.ylim()[0]
     plt.vlines(t0 - duration / 2, ymin, ymin + 0.002, color=c, alpha=0.6)
     plt.vlines(t0 + duration / 2, ymin, ymin + 0.002, color=c, alpha=0.6)
     plt.tight_layout()
 
+
 # Debugging helpers
 
-from astroquery.mast import Catalogs
 import astropy.units as u
 import numpy as np
-from astropy.wcs import WCS, utils as wcsutils
-from prose.telescope import Telescope
 from astropy.coordinates import SkyCoord
+from astropy.wcs import WCS
+from astropy.wcs import utils as wcsutils
+from astroquery.mast import Catalogs
 
+from prose.telescope import Telescope
 
-def _show_tics(data, header= None, telescope_kw="TELESCOP", r=12*u.arcminute):
+
+def _show_tics(data, header=None, telescope_kw="TELESCOP", r=12 * u.arcminute):
     if header is None:
         header = fits.getheader(data)
         data = fits.getdata(data)
 
     telescope = Telescope.from_name(header[telescope_kw])
     ra = header["RA"]
     dec = header["DEC"]
-    skycoord = SkyCoord(ra, dec, frame='icrs', unit=(telescope.ra_unit, telescope.dec_unit))
+    skycoord = SkyCoord(
+        ra, dec, frame="icrs", unit=(telescope.ra_unit, telescope.dec_unit)
+    )
 
     coord = skycoord
     tic_data = Catalogs.query_region(coord, r, "TIC", verbose=False)
     tic_data.sort("Jmag")
 
-    skycoords = SkyCoord(
-        ra=tic_data['ra'],
-        dec=tic_data['dec'], unit="deg")
+    skycoords = SkyCoord(ra=tic_data["ra"], dec=tic_data["dec"], unit="deg")
 
     x, y = np.array(wcsutils.skycoord_to_pixel(skycoords, WCS(header)))
     _ = show_stars(data, contrast=0.5)
     plot_marks(x, y)
 
 
 def plot_transit_window(epoch, period, duration, color="C0"):
@@ -738,34 +891,48 @@
     """
     axes = plt.gcf().axes
 
     for ax in axes:
         if ax.has_data():
             xmin, xmax = ax.get_xlim()
             n_p = np.round((xmax - epoch) / period)
-            if (xmin - epoch - duration / 2) / period < n_p < (xmax - epoch + duration / 2) / period:
+            if (
+                (xmin - epoch - duration / 2) / period
+                < n_p
+                < (xmax - epoch + duration / 2) / period
+            ):
                 ax.axvline(n_p * period + epoch - duration / 2, color=color, alpha=0.4)
                 ax.axvline(n_p * period + epoch + duration / 2, color=color, alpha=0.4)
-                ax.axvspan(n_p * period + epoch - duration / 2, n_p * period + epoch + duration / 2, facecolor=color,
-                           alpha=0.05)
+                ax.axvspan(
+                    n_p * period + epoch - duration / 2,
+                    n_p * period + epoch + duration / 2,
+                    facecolor=color,
+                    alpha=0.05,
+                )
 
 
 def polynomial_trend_latex(**kwargs):
-    """LateX math for a polynomial trend 
+    """LateX math for a polynomial trend
 
     Returns
     -------
     kwargs:
         dict of variable name and order (example: dict(x=2, y=4))
     """
-    monomials = [f"{name}" + (f"^{order}" if order>1 else "") for name, order in kwargs.items() if order>0]
+    monomials = [
+        f"{name}" + (f"^{order}" if order > 1 else "")
+        for name, order in kwargs.items()
+        if order > 0
+    ]
     return rf"${' + '.join(monomials)}$"
 
 
-def corner_text(text, loc=(0.05, 0.05), va="bottom", ha='left', fontsize=12, c="k", ax=None):
+def corner_text(
+    text, loc=(0.05, 0.05), va="bottom", ha="left", fontsize=12, c="k", ax=None
+):
     """Plot a text on the corner of axe
 
     Parameters
     ----------
     text : str
         text in plt.txt
     loc : tuple, optional
@@ -775,18 +942,29 @@
     ha : str, optional
         as in plt.txt, by default 'left'
     fontsize : int, optional
          as in plt.txt, by default 12
     """
     if ax is None:
         ax = plt.gca()
-    ax.text(*loc, text, fontsize=fontsize, ha=ha, va=va, transform=ax.transAxes, color=c)
+    ax.text(
+        *loc, text, fontsize=fontsize, ha=ha, va=va, transform=ax.transAxes, color=c
+    )
 
 
-def plot_systematics_signal(x, y, systematics, signal=None, ylim=None, offset=None, figsize=(6, 7), signal_label=None):
+def plot_systematics_signal(
+    x,
+    y,
+    systematics,
+    signal=None,
+    ylim=None,
+    offset=None,
+    figsize=(6, 7),
+    signal_label=None,
+):
     """Plot a systematics and signal model over data. systematics + signal is plotted on top, signal alone on detrended
     data on bottom
 
     Parameters
     ----------
     x : np.ndarray
     y : np.ndarray
@@ -814,45 +992,62 @@
     if signal is None:
         signal = np.zeros_like(x)
         has_signal = False
     else:
         has_signal = True
 
     fig = plt.figure(figsize=figsize)
-    fig.patch.set_facecolor('white')
-    plot(x, y, label='data', binlabel='binned data (7.2 min)')
-    plt.plot(x, systematics + signal, c="C0",
-             label=f"systematics {'+ signal' if has_signal else ''} model")
+    fig.patch.set_facecolor("white")
+    plot(x, y, label="data", binlabel="binned data (7.2 min)")
+    plt.plot(
+        x,
+        systematics + signal,
+        c="C0",
+        label=f"systematics {'+ signal' if has_signal else ''} model",
+    )
     if has_signal:
-        plt.plot(x, signal + 1. - offset, label=signal_label, c="k")
+        plt.plot(x, signal + 1.0 - offset, label=signal_label, c="k")
     plt.text(plt.xlim()[1] + 0.005, 1, "RAW", rotation=270, va="center")
-    plot(x, y - systematics + 1. - offset)
+    plot(x, y - systematics + 1.0 - offset)
     plt.text(plt.xlim()[1] + 0.005, 1 - offset, "DETRENDED", rotation=270, va="center")
     plt.ylim(ylim)
 
 
 class HandlerEllipse(HandlerPatch):
-    def create_artists(self, legend, orig_handle,
-                       xdescent, ydescent, width, height, fontsize, trans):
+    def create_artists(
+        self, legend, orig_handle, xdescent, ydescent, width, height, fontsize, trans
+    ):
         center = 0.5 * width - 0.5 * xdescent, 0.5 * height - 0.5 * ydescent
-        p = mpatches.Ellipse(xy=center, width=height + xdescent,
-                             height=height + ydescent)
+        p = mpatches.Ellipse(
+            xy=center, width=height + xdescent, height=height + ydescent
+        )
         self.update_prop(p, orig_handle, legend)
         p.set_transform(trans)
         return [p]
 
 
 def circles_legend(colors, texts, ax=None):
     if ax is None:
         ax = plt.gca()
-    c = [mpatches.Circle((0.5, 0.5), radius = 0.25, fill=None, ec=colors[i]) for i in range(len(texts))]
-    ax.legend(c, texts , bbox_to_anchor=(1, 1.05), loc='upper right', ncol=3, handler_map={mpatches.Circle: HandlerEllipse()}, frameon=False)
+    c = [
+        mpatches.Circle((0.5, 0.5), radius=0.25, fill=None, ec=colors[i])
+        for i in range(len(texts))
+    ]
+    ax.legend(
+        c,
+        texts,
+        bbox_to_anchor=(1, 1.05),
+        loc="upper right",
+        ncol=3,
+        handler_map={mpatches.Circle: HandlerEllipse()},
+        frameon=False,
+    )
 
 
 def plot_signal(x, y, label=None, **kwargs):
     axes = plt.gcf().axes
     for i, ax in enumerate(axes):
         xmin, xmax = ax.get_xlim()
         idxs = (xmin <= x) & (x <= xmax)
         ax.plot(x[idxs], y[idxs], label=label if i == 0 else None, **kwargs)
         if label is not None and i == 0:
-            ax.legend()
+            ax.legend()
```

