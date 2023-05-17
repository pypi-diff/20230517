# Comparing `tmp/brainextractor-0.2.1.tar.gz` & `tmp/brainextractor-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainextractor-0.2.1.tar", last modified: Fri Sep 16 15:46:53 2022, max compression
+gzip compressed data, was "brainextractor-0.2.2.tar", last modified: Wed May 17 05:49:45 2023, max compression
```

## Comparing `brainextractor-0.2.1.tar` & `brainextractor-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:46:53.983689 brainextractor-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-09-16 15:46:44.000000 brainextractor-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-09-16 15:46:53.983689 brainextractor-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-09-16 15:46:44.000000 brainextractor-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:46:53.983689 brainextractor-0.2.1/brainextractor/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-16 15:46:44.000000 brainextractor-0.2.1/brainextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4138 2022-09-16 15:46:44.000000 brainextractor-0.2.1/brainextractor/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    17916 2022-09-16 15:46:44.000000 brainextractor-0.2.1/brainextractor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:46:53.983689 brainextractor-0.2.1/brainextractor/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 15:46:44.000000 brainextractor-0.2.1/brainextractor/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2900 2022-09-16 15:46:44.000000 brainextractor-0.2.1/brainextractor/scripts/brainextractor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3942 2022-09-16 15:46:44.000000 brainextractor-0.2.1/brainextractor/scripts/brainextractor_render.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 15:46:53.983689 brainextractor-0.2.1/brainextractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-09-16 15:46:53.000000 brainextractor-0.2.1/brainextractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-09-16 15:46:53.000000 brainextractor-0.2.1/brainextractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 15:46:53.000000 brainextractor-0.2.1/brainextractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-16 15:46:53.000000 brainextractor-0.2.1/brainextractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-16 15:46:53.000000 brainextractor-0.2.1/brainextractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-16 15:46:53.000000 brainextractor-0.2.1/brainextractor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 15:46:53.000000 brainextractor-0.2.1/brainextractor.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-16 15:46:44.000000 brainextractor-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-09-16 15:46:53.983689 brainextractor-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-16 15:46:44.000000 brainextractor-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:49:45.615438 brainextractor-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 05:49:30.000000 brainextractor-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-17 05:49:45.615438 brainextractor-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-17 05:49:30.000000 brainextractor-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:49:45.615438 brainextractor-0.2.2/brainextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 05:49:30.000000 brainextractor-0.2.2/brainextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-17 05:49:30.000000 brainextractor-0.2.2/brainextractor/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-05-17 05:49:30.000000 brainextractor-0.2.2/brainextractor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:49:45.615438 brainextractor-0.2.2/brainextractor/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:49:30.000000 brainextractor-0.2.2/brainextractor/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2023-05-17 05:49:30.000000 brainextractor-0.2.2/brainextractor/scripts/brainextractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3942 2023-05-17 05:49:30.000000 brainextractor-0.2.2/brainextractor/scripts/brainextractor_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:49:45.615438 brainextractor-0.2.2/brainextractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-17 05:49:45.000000 brainextractor-0.2.2/brainextractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 05:49:45.000000 brainextractor-0.2.2/brainextractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:49:45.000000 brainextractor-0.2.2/brainextractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 05:49:45.000000 brainextractor-0.2.2/brainextractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 05:49:45.000000 brainextractor-0.2.2/brainextractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 05:49:45.000000 brainextractor-0.2.2/brainextractor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:49:45.000000 brainextractor-0.2.2/brainextractor.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-17 05:49:30.000000 brainextractor-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 05:49:45.619438 brainextractor-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-17 05:49:30.000000 brainextractor-0.2.2/setup.py
```

### Comparing `brainextractor-0.2.1/LICENSE` & `brainextractor-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brainextractor-0.2.1/PKG-INFO` & `brainextractor-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,41 @@
-Metadata-Version: 2.1
-Name: brainextractor
-Version: 0.2.1
-Summary: brain extraction in python
-Author-email: Andrew Van <vanandrew@wustl.edu>
-License: MIT License
-Project-URL: github, https://github.com/vanandrew/brainextractor
-Keywords: python,image-processing,neuroscience,neuroimaging,segmentation,fsl,brain-extraction,skull-stripping
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: C++
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # brainextractor
-A reimplementation of FSL's Brain Extraction Tool in Python.
+A re-implementation of FSL's Brain Extraction Tool in Python.
 
 Follows the algorithm as described in:
 
 ```
 Smith SM. Fast robust automated brain extraction. Hum Brain Mapp.
 2002 Nov;17(3):143-55. doi: 10.1002/hbm.10062. PMID: 12391568; PMCID: PMC6871816.
 ```
 
+This code was originally made for a [course project](https://www.cse.wustl.edu/~taoju/cse554/).
+
 https://user-images.githubusercontent.com/3641187/190677589-be019bc6-60e4-4e96-8c71-266285ab0755.mp4
 
 ## Install
 
-To install, simply use `pip` to install this repo:
+To install, use `pip` to install this repo:
 
 ```
 # install from pypi
 pip install brainextractor
 
 # install repo with pip
 pip install git+https://github.com/vanandrew/brainextractor@main
 
 # install from local copy
 pip install /path/to/local/repo
 ```
 
-Note that it is recommended to use `brainextractor` on python 3.7+
+> **__NOTE:__** It is recommended to use `brainextractor` on **Python 3.7** and above.
 
 ## Usage
 
-To extract a brain mask from a image, you can call:
+To extract a brain mask from an image, you can call:
 
 ```
 # basic usage
 brainextractor [input_image] [output_image]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz
@@ -62,31 +47,31 @@
 # with custom set threshold
 brainextractor [input_image] [output_image] -f [threshold]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz -f 0.4
 ```
 
-To view the deformation process, you can use the `-w` flag to write the
-surfaces to a file. Then use `brainextractor_render` to view them:
+To view the deformation process (as in the video above), you can use the `-w` flag to
+write the surfaces to a file. Then use `brainextractor_render` to view them:
 
 ```
 # writes surfaces to file
 brainextractor [input_image] [output_image] -w [surfaces_file]
 
 # load surfaces and render
 brainextractor_render [surfaces_file]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz -w /path/to/surface_file.surfaces
 
 brainextractor_render /path/to/surface_file.surfaces
 ```
 
-If you need an explanation of the options at any time, simply run the help:
+If you need an explanation of the options at any time, simply run the `--help` flag:
 
 ```
 brainextractor --help
 ```
 
 If you need to call Brainextractor directly from python:
 ```python
```

### Comparing `brainextractor-0.2.1/README.md` & `brainextractor-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,58 @@
+Metadata-Version: 2.1
+Name: brainextractor
+Version: 0.2.2
+Summary: brain extraction in python
+Author-email: Andrew Van <vanandrew@wustl.edu>
+License: MIT License
+Project-URL: github, https://github.com/vanandrew/brainextractor
+Keywords: python,image-processing,neuroscience,neuroimaging,segmentation,fsl,brain-extraction,skull-stripping
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: C++
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # brainextractor
-A reimplementation of FSL's Brain Extraction Tool in Python.
+A re-implementation of FSL's Brain Extraction Tool in Python.
 
 Follows the algorithm as described in:
 
 ```
 Smith SM. Fast robust automated brain extraction. Hum Brain Mapp.
 2002 Nov;17(3):143-55. doi: 10.1002/hbm.10062. PMID: 12391568; PMCID: PMC6871816.
 ```
 
+This code was originally made for a [course project](https://www.cse.wustl.edu/~taoju/cse554/).
+
 https://user-images.githubusercontent.com/3641187/190677589-be019bc6-60e4-4e96-8c71-266285ab0755.mp4
 
 ## Install
 
-To install, simply use `pip` to install this repo:
+To install, use `pip` to install this repo:
 
 ```
 # install from pypi
 pip install brainextractor
 
 # install repo with pip
 pip install git+https://github.com/vanandrew/brainextractor@main
 
 # install from local copy
 pip install /path/to/local/repo
 ```
 
-Note that it is recommended to use `brainextractor` on python 3.7+
+> **__NOTE:__** It is recommended to use `brainextractor` on **Python 3.7** and above.
 
 ## Usage
 
-To extract a brain mask from a image, you can call:
+To extract a brain mask from an image, you can call:
 
 ```
 # basic usage
 brainextractor [input_image] [output_image]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz
@@ -45,31 +64,31 @@
 # with custom set threshold
 brainextractor [input_image] [output_image] -f [threshold]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz -f 0.4
 ```
 
-To view the deformation process, you can use the `-w` flag to write the
-surfaces to a file. Then use `brainextractor_render` to view them:
+To view the deformation process (as in the video above), you can use the `-w` flag to
+write the surfaces to a file. Then use `brainextractor_render` to view them:
 
 ```
 # writes surfaces to file
 brainextractor [input_image] [output_image] -w [surfaces_file]
 
 # load surfaces and render
 brainextractor_render [surfaces_file]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz -w /path/to/surface_file.surfaces
 
 brainextractor_render /path/to/surface_file.surfaces
 ```
 
-If you need an explanation of the options at any time, simply run the help:
+If you need an explanation of the options at any time, simply run the `--help` flag:
 
 ```
 brainextractor --help
 ```
 
 If you need to call Brainextractor directly from python:
 ```python
```

### Comparing `brainextractor-0.2.1/brainextractor/helpers.py` & `brainextractor-0.2.2/brainextractor/helpers.py`

 * *Files identical despite different names*

### Comparing `brainextractor-0.2.1/brainextractor/main.py` & `brainextractor-0.2.2/brainextractor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     Main BrainExtractor class
 """
 import os
 import warnings
 import numpy as np
 import nibabel as nib
 import trimesh
-from numba import jit, prange
+from numba import jit
 from numba.typed import List
 from .helpers import sphere, closest_integer_point, bresenham3d, l2norm, l2normarray, diagonal_dot
 
 
 class BrainExtractor:
     """
     Implemenation of the FSL Brain Extraction Tool
@@ -103,15 +103,15 @@
         # update the surface attributes
         self.num_vertices = self.surface.vertices.shape[0]
         self.num_faces = self.surface.faces.shape[0]
         self.vertices = np.array(self.surface.vertices)
         self.faces = np.array(self.surface.faces)
         self.vertex_neighbors_idx = List([np.array(i) for i in self.surface.vertex_neighbors])
         # compute location of vertices in face array
-        self.face_vertex_idxs = np.zeros((self.num_vertices, 6, 2), dtype=np.int)
+        self.face_vertex_idxs = np.zeros((self.num_vertices, 6, 2), dtype=np.int64)
         for v in range(self.num_vertices):
             f, i = np.asarray(self.faces == v).nonzero()
             self.face_vertex_idxs[v, : i.shape[0], 0] = f
             self.face_vertex_idxs[v, : i.shape[0], 1] = i
             if i.shape[0] == 5:
                 self.face_vertex_idxs[v, 5, 0] = -1
                 self.face_vertex_idxs[v, 5, 1] = -1
```

### Comparing `brainextractor-0.2.1/brainextractor/scripts/brainextractor.py` & `brainextractor-0.2.2/brainextractor/scripts/brainextractor.py`

 * *Files identical despite different names*

### Comparing `brainextractor-0.2.1/brainextractor/scripts/brainextractor_render.py` & `brainextractor-0.2.2/brainextractor/scripts/brainextractor_render.py`

 * *Files identical despite different names*

### Comparing `brainextractor-0.2.1/brainextractor.egg-info/PKG-INFO` & `brainextractor-0.2.2/brainextractor.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
 Name: brainextractor
-Version: 0.2.1
+Version: 0.2.2
 Summary: brain extraction in python
 Author-email: Andrew Van <vanandrew@wustl.edu>
 License: MIT License
 Project-URL: github, https://github.com/vanandrew/brainextractor
 Keywords: python,image-processing,neuroscience,neuroimaging,segmentation,fsl,brain-extraction,skull-stripping
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # brainextractor
-A reimplementation of FSL's Brain Extraction Tool in Python.
+A re-implementation of FSL's Brain Extraction Tool in Python.
 
 Follows the algorithm as described in:
 
 ```
 Smith SM. Fast robust automated brain extraction. Hum Brain Mapp.
 2002 Nov;17(3):143-55. doi: 10.1002/hbm.10062. PMID: 12391568; PMCID: PMC6871816.
 ```
 
+This code was originally made for a [course project](https://www.cse.wustl.edu/~taoju/cse554/).
+
 https://user-images.githubusercontent.com/3641187/190677589-be019bc6-60e4-4e96-8c71-266285ab0755.mp4
 
 ## Install
 
-To install, simply use `pip` to install this repo:
+To install, use `pip` to install this repo:
 
 ```
 # install from pypi
 pip install brainextractor
 
 # install repo with pip
 pip install git+https://github.com/vanandrew/brainextractor@main
 
 # install from local copy
 pip install /path/to/local/repo
 ```
 
-Note that it is recommended to use `brainextractor` on python 3.7+
+> **__NOTE:__** It is recommended to use `brainextractor` on **Python 3.7** and above.
 
 ## Usage
 
-To extract a brain mask from a image, you can call:
+To extract a brain mask from an image, you can call:
 
 ```
 # basic usage
 brainextractor [input_image] [output_image]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz
@@ -62,31 +64,31 @@
 # with custom set threshold
 brainextractor [input_image] [output_image] -f [threshold]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz -f 0.4
 ```
 
-To view the deformation process, you can use the `-w` flag to write the
-surfaces to a file. Then use `brainextractor_render` to view them:
+To view the deformation process (as in the video above), you can use the `-w` flag to
+write the surfaces to a file. Then use `brainextractor_render` to view them:
 
 ```
 # writes surfaces to file
 brainextractor [input_image] [output_image] -w [surfaces_file]
 
 # load surfaces and render
 brainextractor_render [surfaces_file]
 
 # example
 brainextractor /path/to/test_image.nii.gz /path/to/some_output_image.nii.gz -w /path/to/surface_file.surfaces
 
 brainextractor_render /path/to/surface_file.surfaces
 ```
 
-If you need an explanation of the options at any time, simply run the help:
+If you need an explanation of the options at any time, simply run the `--help` flag:
 
 ```
 brainextractor --help
 ```
 
 If you need to call Brainextractor directly from python:
 ```python
```

### Comparing `brainextractor-0.2.1/brainextractor.egg-info/SOURCES.txt` & `brainextractor-0.2.2/brainextractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainextractor-0.2.1/pyproject.toml` & `brainextractor-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     "neuroimaging",
     "segmentation",
     "fsl",
     "brain-extraction",
     "skull-stripping",
 ]
 classifiers = [
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: C++",
     "Topic :: Scientific/Engineering :: Image Processing",
 ]
 urls = { github = "https://github.com/vanandrew/brainextractor" }
-version = "0.2.1"
+version = "0.2.2"
 dynamic = ["entry-points"]
 dependencies = [
     "numba >= 0.51.2",
     "nibabel >= 3.2.1",
     "trimesh >= 3.8.15",
     "numpy >= 1.19.4",
     "scipy >= 1.5.4",
```

### Comparing `brainextractor-0.2.1/setup.py` & `brainextractor-0.2.2/setup.py`

 * *Files identical despite different names*

