# Comparing `tmp/lapy-0.4.1.tar.gz` & `tmp/lapy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapy-0.4.1.tar", last modified: Thu Feb 23 16:46:30 2023, max compression
+gzip compressed data, was "lapy-0.6.0.tar", last modified: Wed May 17 15:43:27 2023, max compression
```

## Comparing `lapy-0.4.1.tar` & `lapy-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:30.176495 lapy-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-23 16:45:51.000000 lapy-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-02-23 16:46:30.176495 lapy-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-02-23 16:45:51.000000 lapy-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:30.172495 lapy-0.4.1/lapy/
--rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/Conformal.py
--rw-r--r--   0 runner    (1001) docker     (123)    22109 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/DiffGeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/FuncIO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/Heat.py
--rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/ShapeDNA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30443 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/Solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/TetIO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/TetMesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/TriaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    37475 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/TriaMesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:30.176495 lapy-0.4.1/lapy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/commands/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/read_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:30.176495 lapy-0.4.1/lapy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/utils/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-23 16:45:51.000000 lapy-0.4.1/lapy/utils/_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:46:30.172495 lapy-0.4.1/lapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-02-23 16:46:30.000000 lapy-0.4.1/lapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-23 16:46:30.000000 lapy-0.4.1/lapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:46:30.000000 lapy-0.4.1/lapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 16:46:30.000000 lapy-0.4.1/lapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-23 16:46:30.000000 lapy-0.4.1/lapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-23 16:46:30.000000 lapy-0.4.1/lapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-02-23 16:45:51.000000 lapy-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:46:30.176495 lapy-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:45:51.000000 lapy-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.714751 lapy-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-17 15:42:50.000000 lapy-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-17 15:43:27.714751 lapy-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-17 15:42:50.000000 lapy-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.710751 lapy-0.6.0/lapy/
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Conformal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/DiffGeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/FuncIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Heat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/ShapeDNA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30698 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/Solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TetIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TetMesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TriaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42560 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/TriaMesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.710751 lapy-0.6.0/lapy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/commands/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/read_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.714751 lapy-0.6.0/lapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/utils/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-17 15:42:50.000000 lapy-0.6.0/lapy/utils/_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:27.710751 lapy-0.6.0/lapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 15:43:27.000000 lapy-0.6.0/lapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-17 15:42:50.000000 lapy-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:43:27.714751 lapy-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:42:50.000000 lapy-0.6.0/setup.py
```

### Comparing `lapy-0.4.1/LICENSE` & `lapy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lapy-0.4.1/PKG-INFO` & `lapy-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapy
-Version: 0.4.1
+Version: 0.6.0
 Summary: A package for differential geometry on meshes (Laplace, FEM)
 Author-email: Martin Reuter <martin.reuter@dzne.de>
 Maintainer-email: Martin Reuter <martin.reuter@dzne.de>
 License: MIT License
         
         Copyright (c) 2020 Deep Medical Imaging Lab (PI Reuter)
         
@@ -71,19 +71,14 @@
 - Solver: a class for linear FEM computation (Laplace stiffness and mass
   matrix, fast and sparse eigenvalue solver, anisotropic Laplace, Poisson)
 - DiffGeo: compute gradients, divergence, mean curvature flow, etc.
 - Heat: for heat kernel and diffusion
 - ShapeDNA: compute the ShapeDNA descriptor of surfaces and solids
 - Plot: functions for interactive visualization (wrapping plotly)
 
-## ToDo:
-
-- Add unit tests and automated testing (e.g. travis)
-- Add command line scripts for various functions
-
 ## Usage:
 
 The LaPy package is a comprehensive collection of scripts, so we refer to the
 'help' function and docstring of each module / function / class for usage info.
 For example:
 
 ```
@@ -103,29 +98,33 @@
 `python3 -m pip install lapy`
 
 Use the following code to install the dev package in editable mode to a location of
 your choice:
 
 `python3 -m pip install --user --src /my/preferred/location --editable git+https://github.com/Deep-MI/Lapy.git#egg=lapy`
 
-Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package and will fall back to LU if the import fails. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
+Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. The default is to use the LU decomposition. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
 
 ## References:
 
 If you use this software for a publication please cite both these papers:
 
-[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
+[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
 
-[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
+[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
 
 [1] introduces the FEM methods and the Laplace spectra for shape analysis, while [2] focusses on medical applications.
 
 For Geodesics please cite:
 
 [3] Crane K, Weischedel C, Wardetzky M. Geodesics in heat: A new approach to computing distance based on heat flow. ACM Transactions on Graphics. https://doi.org/10.1145/2516971.2516977
 
 For non-singular mean curvature flow please cite:
 
 [4] Kazhdan M, Solomon J, Ben-Chen M. 2012. Can Mean-Curvature Flow be Modified to be Non-singular? Comput. Graph. Forum 31, 5, 1745–1754.
 https://doi.org/10.1111/j.1467-8659.2012.03179.x
 
+For conformal mapping please cite:
+
+[5] Choi PT, Lam KC, Lui LM. FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces. SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015. https://doi.org/10.1137/130950008
+
 We also invite you to check out our lab webpage at https://deep-mi.org
```

### Comparing `lapy-0.4.1/README.md` & `lapy-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 - Solver: a class for linear FEM computation (Laplace stiffness and mass
   matrix, fast and sparse eigenvalue solver, anisotropic Laplace, Poisson)
 - DiffGeo: compute gradients, divergence, mean curvature flow, etc.
 - Heat: for heat kernel and diffusion
 - ShapeDNA: compute the ShapeDNA descriptor of surfaces and solids
 - Plot: functions for interactive visualization (wrapping plotly)
 
-## ToDo:
-
-- Add unit tests and automated testing (e.g. travis)
-- Add command line scripts for various functions
-
 ## Usage:
 
 The LaPy package is a comprehensive collection of scripts, so we refer to the
 'help' function and docstring of each module / function / class for usage info.
 For example:
 
 ```
@@ -49,29 +44,33 @@
 `python3 -m pip install lapy`
 
 Use the following code to install the dev package in editable mode to a location of
 your choice:
 
 `python3 -m pip install --user --src /my/preferred/location --editable git+https://github.com/Deep-MI/Lapy.git#egg=lapy`
 
-Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package and will fall back to LU if the import fails. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
+Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. The default is to use the LU decomposition. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
 
 ## References:
 
 If you use this software for a publication please cite both these papers:
 
-[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
+[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
 
-[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
+[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
 
 [1] introduces the FEM methods and the Laplace spectra for shape analysis, while [2] focusses on medical applications.
 
 For Geodesics please cite:
 
 [3] Crane K, Weischedel C, Wardetzky M. Geodesics in heat: A new approach to computing distance based on heat flow. ACM Transactions on Graphics. https://doi.org/10.1145/2516971.2516977
 
 For non-singular mean curvature flow please cite:
 
 [4] Kazhdan M, Solomon J, Ben-Chen M. 2012. Can Mean-Curvature Flow be Modified to be Non-singular? Comput. Graph. Forum 31, 5, 1745–1754.
 https://doi.org/10.1111/j.1467-8659.2012.03179.x
 
+For conformal mapping please cite:
+
+[5] Choi PT, Lam KC, Lui LM. FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces. SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015. https://doi.org/10.1137/130950008
+
 We also invite you to check out our lab webpage at https://deep-mi.org
```

### Comparing `lapy-0.4.1/lapy/Conformal.py` & `lapy-0.6.0/lapy/Conformal.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,56 +8,73 @@
 # If you use this code in your own work, please cite the following paper:
 # [1] P. T. Choi, K. C. Lam, and L. M. Lui,
 # "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0
 #  Closed Brain Surfaces."
 # SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
 
 
+import importlib
+
 import numpy as np
 from scipy import sparse
 from scipy.optimize import minimize
 
 from .Solver import Solver
 from .TriaMesh import TriaMesh
 from .utils._imports import import_optional_dependency
 
 
-def spherical_conformal_map(tria):
+def spherical_conformal_map(tria, use_cholmod=False):
     """
     A linear method for computing spherical conformal map of a genus-0 closed surface
 
-    Input:   TriaMesh (vertices and faces)
-    Output:
-    mapped_vertices: nv x 3 vertex coordinates of the spherical conformal parameterization
+    Parameters
+    ----------
+    tria : TriaMesh
+        vertices and faces
+    use_cholmod : bool, default=False
+        Which solver to use:
+            * True : Use Cholesky decomposition from scikit-sparse cholmod
+            * False: Use spsolve (LU decomposition)        
+
+    Returns
+    -------
+    mapping: np.ndarray of shape (n,3)
+        vertex coordinates of the spherical conformal parameterization
 
+    Notes
+    -------
     If you use this code in your own work, please cite the following paper:
     [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-       "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces."
+       "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
+       for Genus-0 Closed Brain Surfaces."
        SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
 
     Adopted from Matlab code at
     https://github.com/garyptchoi/spherical-conformal-map
     with this
     Copyright (c) 2013-2020, Gary Pui-Tung Choi
     https://math.mit.edu/~ptchoi
     and has been distributed with the Apache 2 License
     """
+
     # Check whether the input mesh is spherical topology (genus-0)
     if tria.euler() != 2:
         print("ERROR: The mesh is not a genus-0 closed surface ..")
         raise ValueError("not genus-0")
 
     # Find the most regular triangle as the "big triangle"
     tquals = tria.tria_qualities()
     bigtri = np.argmax(tquals)
     # print(bigtri, tquals[bigtri])
     # If it turns out that the spherical parameterization result is homogeneous
     # you can try to change bigtri to the id of some other triangles with good quality
 
-    # North pole step: Compute spherical map by solving laplace equation on a big triangle
+    # North pole step: Compute spherical map
+    #   by solving laplace equation on a big triangle
     nv = tria.v.shape[0]
     S = Solver(tria)
     M = S.stiffness.astype(complex)
 
     p0 = tria.t[bigtri, 0]
     p1 = tria.t[bigtri, 1]
     p2 = tria.t[bigtri, 2]
@@ -89,15 +106,15 @@
     c[p0], c[p1], c[p2] = x0, x1, x2
     d = np.zeros((nv, 1))
     d[p0], d[p1], d[p2] = y0, y1, y2
     rhs = np.empty(c.shape[:-1], dtype=complex)
     rhs.real = c.flatten()
     rhs.imag = d.flatten()
 
-    z = sparse_symmetric_solve(M, rhs)
+    z = sparse_symmetric_solve(M, rhs, use_cholmod=use_cholmod)
     z = np.squeeze(np.array(z))
     z = z - np.mean(z, axis=0)
 
     # inverse stereographic projection (not scaled well)
     S = inverse_stereographic(z)
 
     # Find optimal big triangle size
@@ -152,50 +169,59 @@
     )
 
     # compute the Beltrami coefficient (value per triangle)
     triasouth = TriaMesh(P, tria.t)
     mu = beltrami_coefficient(triasouth, tria.v)
 
     # compose the map with another quasi-conformal map to cancel the distortion
-    mapping = linear_beltrami_solver(triasouth, mu, fixed, P[fixed, :])
+    mapping = linear_beltrami_solver(triasouth, mu, fixed, P[fixed, :], use_cholmod=use_cholmod)
 
     if np.isnan(np.sum(mapping)):
         # if the result has NaN entries, then most probably the number of
         # boundary constraints is not large enough
         # increase the number of boundary constrains and run again
         print("South pole compsed map has nan value(s)!")
         fixnum = fixnum * 5  # again, this number can be changed
         fixed = idx[0 : np.minimum(nv, fixnum)]
-        mapping = linear_beltrami_solver(triasouth, mu, fixed, P[fixed, :])
+        mapping = linear_beltrami_solver(triasouth, mu, fixed, P[fixed, :], use_cholmod=use_cholmod)
         if np.isnan(np.sum(mapping)):
             mapping = P  # use the old result
 
     # inverse south pole stereographic projection
     mapping = inverse_stereographic(mapping)
     return mapping
 
 
 def mobius_area_correction_spherical(tria, mapping):
     """
-    Find an optimal Mobius transformation for reducing the area distortion of a spherical conformal parameterization
-    using the method in [1].
+    Find an optimal Mobius transformation for reducing the area distortion
+    of a spherical conformal parameterization using the method in [1].
 
-    Input:
-    tria : TriaMesh (vertices, triangle) of genus-0 closed triangle mesh
-    mapping: nv x 3 vertex coordinates of the spherical conformal parameterization
-
-    Output:
-    map_mobius: nv x 3 vertex coordinates of the updated spherical conformal parameterization
-    x: the optimal parameters for the Mobius transformation, where
-       f(z) = \frac{az+b}{cz+d}
-            = ((x(1)+x(2)*1j)*z+(x(3)+x(4)*1j))/((x(5)+x(6)*1j)*z+(x(7)+x(8)*1j))
+    Parameters
+    -------
+    tria : TriaMesh
+        (vertices, triangle) of genus-0 closed triangle mesh
+    mapping : np.ndarray of shape (n,3)
+        vertex coordinates of the spherical conformal parameterization
+
+    Returns
+    -------
+    map_mobius: np.ndarray of shape (n,3)
+        vertex coordinates of the updated spherical conformal parameterization
+    result: OptimizeResult
+        the optimal parameters (x) for the Mobius transformation, where
+            f(z) = \frac{az+b}{cz+d}
+                = ((x(1)+x(2)*1j)*z+(x(3)+x(4)*1j))/((x(5)+x(6)*1j)*z+(x(7)+x(8)*1j))
 
+    Notes
+    -------
     If you use this code in your own work, please cite the following paper:
     [1] G. P. T. Choi, Y. Leung-Liu, X. Gu, and L. M. Lui,
-        "Parallelizable global conformal parameterization of simply-connected surfaces via partial welding."
+        "Parallelizable global conformal parameterization
+        of simply-connected surfaces via partial welding."
         SIAM Journal on Imaging Sciences, 2020.
 
     Adopted by Martin Reuter from Matlab code at
     https://github.com/garyptchoi/spherical-conformal-map
     with this
     Copyright (c) 2019-2020, Gary Pui-Tung Choi
     https://scholar.harvard.edu/choi
@@ -247,26 +273,43 @@
     map_mobius = inverse_stereographic(fz)
     return map_mobius, result
 
 
 def beltrami_coefficient(tria, mapping):
     """
     Compute the Beltrami coefficient of a mapping.
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        (vertices, triangle) of genus-0 closed triangle mesh
+        TriaMesh should be planar mapping on complex plane
+    mapping : np.ndarray of shape (n,3)
+        coordinates of the spherical conformal parameterization
+
+    Returns
+    -------
+    mu: np.ndarray of complex beltrami coefficient per triangle
+
+    Notes
+    -------
     If you use this code in your own work, please cite the following paper:
     [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces."
+    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
+    for Genus-0 Closed Brain Surfaces."
     SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
 
     Adopted by Martin Reuter from Matlab code at
     https://github.com/garyptchoi/spherical-conformal-map
     with this
     Copyright (c) 2013-2020, Gary Pui-Tung Choi
     https://math.mit.edu/~ptchoi
     and has been distributed with the Apache 2 License
     """
+
     # here we should be in the plane
     if np.amax(tria.v[:, 2]) - np.amin(tria.v[:, 2]) > 0.001:
         print("ERROR: mesh should be on complex plane ..")
         raise ValueError("not planar")
 
     # get 2d vetrices, edges and area
     v0 = (tria.v[tria.t[:, 0], :])[:, :-1]
@@ -304,20 +347,43 @@
     G = dXdv**2 + dYdv**2 + dZdv**2
     F = dXdu * dXdv + dYdu * dYdv + dZdu * dZdv
     mu = (E - G + 2j * F) / (E + G + 2.0 * np.sqrt(E * G - F**2))
 
     return mu
 
 
-def linear_beltrami_solver(tria, mu, landmark, target):
+def linear_beltrami_solver(tria, mu, landmark, target, use_cholmod=False):
     """
     Linear Beltrami solver
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        (vertices, triangle) of genus-0 closed triangle mesh
+        TriaMesh should be planar mapping on complex plane
+    mu : np.array of complex beltrami coefficients
+    landmark : np.ndarray of fixed vertex indices
+    target : np.ndarray of shape (n,3)
+        2D landmark target coordinates (third coordinate is zero)
+    use_cholmod : bool, default=False
+        Which solver to use:
+            * True : Use Cholesky decomposition from scikit-sparse cholmod
+            * False: Use spsolve (LU decomposition)             
+
+    Returns
+    -------
+    mapping : np.ndarray of shape (n,3)
+        vertex coordinates of new mapping
+
+    Notes
+    ------
     If you use this code in your own work, please cite the following paper:
     [1] P. T. Choi, K. C. Lam, and L. M. Lui,
-    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces."
+    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
+    for Genus-0 Closed Brain Surfaces."
     SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
 
     Adopted by Martin Reuter from Matlab code at
     https://github.com/garyptchoi/spherical-conformal-map
     with this
     Copyright (c) 2013-2020, Gary Pui-Tung Choi
     https://math.mit.edu/~ptchoi
@@ -387,53 +453,127 @@
     Azero = sparse.csc_matrix((mval, (mrow, landmark[mcol])), shape=(nv, nv))
     Aones = sparse.csr_matrix(
         (np.ones(landmark.shape[0]), (landmark, landmark)), shape=(nv, nv)
     )
     A = A - Azero + Aones
     A.eliminate_zeros()
 
-    x = sparse_symmetric_solve(A, b)
+    x = sparse_symmetric_solve(A, b, use_cholmod=use_cholmod)
 
     mapping = np.squeeze(np.array(x))
     mapping = np.column_stack((np.real(mapping), np.imag(mapping)))
     return mapping
 
 
-def sparse_symmetric_solve(A, b, use_cholmod=True):
-    sksparse = import_optional_dependency("sksparse", raise_error=use_cholmod)
-    if sksparse is not None:
+def sparse_symmetric_solve(A, b, use_cholmod=False):
+    """
+    A sparse symmetric solver for ``A x = b``
+
+    Parameters
+    ----------
+    A : sparse matrix of shape (n, n)
+    b : np.ndarray vector of length n
+    use_cholmod : bool, default=False
+        Which solver to use:
+            * True : Use Cholesky decomposition from scikit-sparse cholmod
+            * False: Use spsolve (LU decomposition)
+
+    Returns
+    -------
+    x: np.ndarray of length n, solution to  ``A x = b``
+    """
+
+    if use_cholmod:
+        sksparse = import_optional_dependency("sksparse", raise_error=True)
+        importlib.import_module(".cholmod", sksparse.__name__)
+    else:
+        sksparse = None
+    if use_cholmod:
         print("Solver: Cholesky decomposition from scikit-sparse cholmod ...")
         chol = sksparse.cholmod.cholesky(A)
         x = chol(b)
     else:
         from scipy.sparse.linalg import splu
 
         print("Solver: spsolve (LU decomposition) ...")
         lu = splu(A)
         x = lu.solve(b)
     return x
 
 
 def stereographic(u):
-    # Map sphere to complex plane
-    # u has three columns (x,y,z)
-    # return z as array of complex numbers
+    """
+    Map sphere to complex plane via stereographic projection
+
+    Parameters
+    ----------
+    u : np.ndarray of shape (n,3)
+        u represents the three vertex coordinates
+
+    Returns
+    -------
+    v: np.ndarray of n complex numbers
+       stereographic map of u in complex plane
+
+    Notes
+    -------
+    If you use this code in your own work, please cite the following paper:
+    [1] P. T. Choi, K. C. Lam, and L. M. Lui,
+    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
+     for Genus-0 Closed Brain Surfaces."
+    SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
+
+    Adopted by Martin Reuter from Matlab code at
+    https://github.com/garyptchoi/spherical-conformal-map
+    with this
+    Copyright (c) 2013-2020, Gary Pui-Tung Choi
+    https://math.mit.edu/~ptchoi
+    and has been distributed with the Apache 2 License
+    """
+
     x = u[:, 0]
     y = u[:, 1]
     z = u[:, 2]
     v = np.empty(u.shape[:-1], dtype=complex)
     v.real = (x / (1 - z)).flatten()
     v.imag = (y / (1 - z)).flatten()
     return v
 
 
 def inverse_stereographic(u):
-    # Computes mapping from complex plane to sphere
-    # u can be complex array, or two columns (real,img)
-    # returns v as (nv x 3) coordinates on sphere
+    """
+    Map from complex plane to sphere via inverse stereographic projection
+
+    Parameters
+    ----------
+    u : np.ndarray
+        can be complex array, or two columns (real,img)
+        for coordinates on complex plane
+
+    Returns
+    -------
+    v: np.ndarray of shape (n,3)
+        coordinates on sphere in 3D
+
+    Notes
+    -------
+    If you use this code in your own work, please cite the following paper:
+    [1] P. T. Choi, K. C. Lam, and L. M. Lui,
+    "FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization
+     for Genus-0 Closed Brain Surfaces."
+    SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015.
+
+    Adopted by Martin Reuter from Matlab code at
+    https://github.com/garyptchoi/spherical-conformal-map
+    with this
+    Copyright (c) 2013-2020, Gary Pui-Tung Choi
+    https://math.mit.edu/~ptchoi
+    and has been distributed with the Apache 2 License
+    """
+
     if np.iscomplexobj(u):
         x = u.real
         y = u.imag
     else:
         x = u[:, 0]
         y = u[:, 1]
     z = 1 + x**2 + y**2
```

### Comparing `lapy-0.4.1/lapy/DiffGeo.py` & `lapy-0.6.0/lapy/DiffGeo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,200 @@
 import numpy as np
+import importlib
 from scipy import sparse
 
 from .Solver import Solver
 from .TriaMesh import TriaMesh
 from .utils._imports import import_optional_dependency
 
 
 def compute_gradient(geom, vfunc):
+    """
+    Computes gradient of a vertex function f
+
+    Parameters
+    -------
+    geom : TriaMesh or TetMesh
+        geometry vertices
+    vfunc : function
+        scalar function at vertices
+
+    Returns
+    -------
+    tfunc : function
+        3d vector function of gradient
+
+    Raises
+    -------
+    ValueError: Unknown geometry type
+    """
+
     if type(geom).__name__ == "TriaMesh":
         return tria_compute_gradient(geom, vfunc)
     elif type(geom).__name__ == "TetMesh":
         return tet_compute_gradient(geom, vfunc)
     else:
         raise ValueError('Geometry type "' + type(geom).__name__ + '" unknown')
 
 
 def compute_divergence(geom, vfunc):
+    """
+    Computes divergence of a vertex function f
+
+    Parameters
+    ----------
+    geom : TriaMesh or TetMesh
+        geometry vertices
+    vfunc : function
+        scalar function at vertices
+
+    Returns
+    -------
+    vfunc : function
+        scalar function of divergence
+
+    Raises
+    -------
+    ValueError: unknown geometry type
+    """
     if type(geom).__name__ == "TriaMesh":
         return tria_compute_divergence(geom, vfunc)
     elif type(geom).__name__ == "TetMesh":
         return tet_compute_divergence(geom, vfunc)
     else:
         raise ValueError('Geometry type "' + type(geom).__name__ + '" unknown')
 
 
 def compute_rotated_f(geom, vfunc):
+    """
+    Compute function whose level sets are orthgonal to the ones of vfunc
+
+    Parameters
+    ----------
+    geom : TriaMesh
+        geometry vertices
+    vfunc : function
+        scalar function at vertices
+
+    Returns
+    -------
+    vfunc : function
+        rotated function
+
+    Raises
+    -------
+    Value Error: Unknown geometry type
+    """
+
     if type(geom).__name__ == "TriaMesh":
         return tria_compute_rotated_f(geom, vfunc)
     else:
         raise ValueError('Geometry type "' + type(geom).__name__ + '" not implemented')
 
 
 def compute_geodesic_f(geom, vfunc):
     """
     Computes function with normalized gradient (geodesic distance)
 
-    Inputs:     geom        geometry either TriaMesh, TetMesh
-                vfunc       scalar function at vertices
-
-    :return:    vfunc       scalar geodesic function at vertices
-
     Computes gradient, normalizes it and computes function with this normalized
     gradient by solving the Poisson equation with the divergence of grad.
     This idea is also described in the paper "Geodesics in Heat" for triangles.
+
+    Parameters
+    ----------
+    geom : TriaMesh, TetMesh
+        geometry vertices
+    vfunc : function
+        scalar function at vertices
+
+    Returns
+    -------
+    vfunc : function
+        scalar geodesic function at vertices
     """
+
     gradf = compute_gradient(geom, vfunc)
     # normalize gradient
     gradnorm = gradf / np.sqrt((gradf**2).sum(1))[:, np.newaxis]
     gradnorm = np.nan_to_num(gradnorm)
     divf = compute_divergence(geom, gradnorm)
     fem = Solver(geom, lump=True)
-    # as long as div does not care about weighing with a Bi, we can pass identity instead of B here:
+    # as long as div does not care about weighing with a Bi,
+    #   we can pass identity instead of B here:
     fem.mass = sparse.eye(fem.stiffness.shape[0], dtype=fem.stiffness.dtype)
     vf = fem.poisson(divf)
     vf -= min(vf)
     return vf
 
 
 def tria_compute_geodesic_f(tria, vfunc):
     """
     Computes function with normalized gradient (geodesic distance)
 
-    Inputs:    v           vertices
-               t           triangles
-               vfunc       scalar function at vertices
-
-    Outputs:   vfunc       scalar geodesic function at vertices
-
     Computes gradient, normalizes it and computes function with this normalized
     gradient by solving the Poisson equation with the divergence of grad.
     This idea is also described in the paper "Geodesics in Heat".
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        geometry vertices
+            v           vertices
+            t           triangles
+    vfunc : function
+        scalar function at vertices
+
+    Returns
+    -------
+    vfunc: function
+        scalar geodesic function at vertices
     """
     gradf = tria_compute_gradient(tria, vfunc)
     # normalize gradient
     gradnorm = gradf / np.sqrt((gradf**2).sum(1))[:, np.newaxis]
     gradnorm = np.nan_to_num(gradnorm)
     divf = tria_compute_divergence(tria, gradnorm)
     fem = Solver(tria)
-    # as long as div does not care about weighing with a Bi, we can pass identity instead of B here:
+    # as long as div does not care about weighing with a Bi,
+    #   we can pass identity instead of B here:
     # div is the integrated divergence (so it is already B*div)
     fem.mass = sparse.eye(fem.stiffness.shape[0])
     vf = fem.poisson(divf)
     vf -= min(vf)
     return vf
 
 
 # note , numexpr could speed up the following functions if necessary
 def tria_compute_gradient(tria, vfunc):
     """
     Computes gradient of a vertex function f (for each triangle)
 
-    Inputs:    v           vertices
-               t           triangles
-               vfunc       scalar function at vertices
-
-    Outputs:   tfunc       3d vector function of gradient at triangles
-
     grad(f) = [ (f_j - f_i) (vi-vk)' + (f_k - f_i) (vj-vi)' ] / (2 A)
             = [ f_i (vk-vj)' + f_j (vi-vk)' +  f_k (vj-vi)' ] / (2 A)
     for triangle (vi,vj,vk) with area A, where (.)' is 90 degrees rotated
     edge, which is equal to cross(n,vec).
 
+    Parameters
+    ----------
+    tria : TriaMesh
+        geometry vertices
+            v           vertices
+            t           triangles
+    vfunc : function
+        scalar function at vertices
+
+    Returns
+    -------
+    vfunc: function
+        3d vector function of gradient at triangles where
+
+    Notes
+    -------
+    numexpr could speed up this functions if necessary
+
     Good background to read:
     http://dgd.service.tu-berlin.de/wordpress/vismathws10/2012/10/17/gradient-of-scalar-functions/
     Mancinelli, Livesu, Puppo, Gradient Field Estimation on Triangle Meshes
       http://pers.ge.imati.cnr.it/livesu/papers/MLP18/MLP18.pdf
     Desbrun ...
     """
     import sys
@@ -130,25 +220,38 @@
     return tfunc
 
 
 def tria_compute_divergence(tria, tfunc):
     """
     Computes integrated divergence of a 3d triangle function f (for each vertex)
 
-    Inputs:    v           vertices
-               t           triangles
-               tfunc       3d vector field on triangles
-
-    Outputs:   vfunc       scalar function of divergence at vertices
-
     Divergence is the flux density leaving or entering a point.
 
     Note: this is the integrated divergence, you may want to multiply
     with B^-1 to get back the function in some applications
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        geometry vertices
+            v           vertices
+            t           triangles
+    tfunc : function
+        3d vector field on triangles
+
+    Returns
+    -------
+    vfunc: function
+        scalar function of divergence at vertices
+
+    Notes
+    -------
+    numexpr could speed up this functions if necessary
     """
+
     import sys
 
     v0 = tria.v[tria.t[:, 0], :]
     v1 = tria.v[tria.t[:, 1], :]
     v2 = tria.v[tria.t[:, 2], :]
     e2 = v1 - v0
     e0 = v2 - v1
@@ -177,32 +280,43 @@
     # convert back to nparray 1D
     vfunc = np.squeeze(
         np.asarray(0.5 * sparse.csc_matrix((dat, (i, j))).todense(), dtype=tfunc.dtype)
     )
     return vfunc
 
 
-# another way to compute divergence using cross products
 def tria_compute_divergence2(tria, tfunc):
     """
     Computes integrated divergence of a 3d triangle function f (for each vertex)
 
-    Inputs:    v           vertices
-               t           triangles
-               tfunc       3d vector field on triangles
-
-    Outputs:   vfunc       scalar function of divergence at vertices
-
     Divergence is the flux density leaving or entering a point.
     It can be measured by summing the dot product of the vector
     field with the normals to the outer edges of the 1-ring triangles
     around a vertex. Summing < tfunc , e_ij cross n >
 
     Note: this is the integrated divergence, you may want to multiply
     with B^-1 to get back the function in some applications
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        geometry vertices
+            v           vertices
+            t           triangles
+    tfunc : function
+        3d vector field on triangles
+
+    Returns
+    -------
+    vfunc: function
+        scalar function of divergence at vertices
+
+    Notes
+    -------
+    numexpr could speed up this functions if necessary
     """
     import sys
 
     v0 = tria.v[tria.t[:, 0], :]
     v1 = tria.v[tria.t[:, 1], :]
     v2 = tria.v[tria.t[:, 2], :]
     e2 = v1 - v0
@@ -227,74 +341,110 @@
     return vfunc
 
 
 def tria_compute_rotated_f(tria, vfunc):
     """
     Compute function whose level sets are orthgonal to the ones of vfunc.
 
-    Inputs:    v           vertices
-               t           triangles
-               vfunc       scalar function at triangles
-
-    Outputs:   vfunc       rotated function
-
     This is done by rotating the gradient around the normal by 90 degrees,
     then solving the Poisson equations with the divergence of rotated grad.
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        geometry vertices
+            v           vertices
+            t           triangles
+    vfunc : function
+        scalar function at triangles
+
+    Returns
+    -------
+    vfunc: function
+        rotated function
+
+    Notes
+    -------
+    numexpr could speed up this functions if necessary
     """
+
     gradf = tria_compute_gradient(tria, vfunc)
     tn = tria.tria_normals()
     # lg = np.sqrt(np.sum(gradf * gradf, axis=1))
     # lgi = np.divide(1.0,lg)[:,np.newaxis]
     # gradf *= lgi
     gradf = np.cross(tn, gradf)
     divf = tria_compute_divergence(tria, gradf)
     fem = Solver(tria)
-    # as long as div does not care about weighing with a Bi, we can pass identity instead of B here:
+    # as long as div does not care about weighing with a Bi,
+    #   we can pass identity instead of B here:
     # div is the integrated divergence (so it is already B*div)
     fem.mass = sparse.eye(fem.stiffness.shape[0], dtype=vfunc.dtype)
     vf = fem.poisson(divf)
     return vf
 
 
 def tria_mean_curvature_flow(
-    tria, max_iter=30, stop_eps=1e-13, step=1.0, use_cholmod=True
+    tria, max_iter=30, stop_eps=1e-13, step=1.0, use_cholmod=False
 ):
     """
     mean_curvature_flow iteratively flows a triangle mesh along mean curvature
     normal (non-singular, see Kazhdan 2012)
 
-    Inputs:   tria        TriaMesh object (vertices and triangles)
-              max_iter    maximal number of steps
-              stops_eps   stopping threshold
-              step        Euler step size
-
-    Outputs:  TriaMesh - TriaMesh object (vertices and triangles)
-
     This uses the algorithm described in Kazhdan 2012 "Can mean curvature flow be
     made non-singular" which uses the Laplace-Beltrami operator but keeps the
     stiffness matrix (A) fixed and only adjusts the mass matrix (B) during the
     steps. It will normalize surface area of the mesh and translate the barycenter
     to the origin. Closed meshes will map to the unit sphere.
-    """
-    sksparse = import_optional_dependency("sksparse", raise_error=use_cholmod)
+
+    Parameters
+    ----------
+    tria : TriaMesh
+         object of vertices and triangles
+    max_iter : int, default=30
+        maximal number of steps
+    stop_eps : float, default=1e-13
+        stopping threshold
+    step : float, default=1.0
+        Euler step size
+    use_cholmod : bool, default=False
+        Which solver to use:
+            * True : Use Cholesky decomposition from scikit-sparse cholmod
+            * False: Use spsolve (LU decomposition)
+
+    Returns
+    -------
+    tria : TriaMesh
+        vertices and triangles
+
+    Notes
+    -------
+    numexpr could speed up this functions if necessary
+    """
+
+    if use_cholmod:
+        sksparse = import_optional_dependency("sksparse", raise_error=True)
+        importlib.import_module(".cholmod", sksparse.__name__)
+    else:
+        sksparse = None
     # pre-normalize
     trianorm = TriaMesh(tria.v, tria.t)
     trianorm.normalize_()
     # compute fixed A
     lump = True  # for computation here and inside loop
     fem = Solver(trianorm, lump)
     a_mat = fem.stiffness
     for x in range(max_iter):
         # store last position (for delta computation below)
         vlast = trianorm.v
         # get current mass matrix and Mv
         mass = Solver.fem_tria_mass(trianorm, lump)
         mass_v = mass.dot(trianorm.v)
         # solve (M + step*A) * v = Mv and update vertices
-        if sksparse is not None:
+        if use_cholmod:
             print("Solver: Cholesky decomposition from scikit-sparse cholmod ...")
             factor = sksparse.cholmod.cholesky(mass + step * a_mat)
             trianorm.v = factor(mass_v)
         else:
             # Note, it would be better to do sparse Cholesky (CHOLMOD)
             # as it can be 5-6 times faster
             from scipy.sparse.linalg import spsolve
@@ -319,19 +469,33 @@
            and then projects the spectral embedding onto a sphere. This works
            when the first functions have a single closed zero level set,
            splitting the mesh into two domains each. Depending on the original
            shape triangles could get inverted. We also flip the functions
            according to the axes that they are aligned with for the special
            case of brain surfaces in FreeSurfer coordinates.
 
-    Inputs:   tria      : TriaMesh
-              flow_iter : mean curv flow iterations (3 should be enough)
-
-    Outputs:  tria      : TriaMesh
+    Parameters
+    ----------
+    tria : TriaMesh
+        object of vertices and triangles
+    flow_iter : int, default=3
+        mean curv flow iterations (3 should be enough)
+    debug : bool, default=False
+        prints debug values if true
+
+    Returns
+    -------
+    tria: TriaMesh
+        object of vertices and triangles
+
+    Notes
+    -----
+    numexpr could speed up this functions if necessary
     """
+
     import math
 
     if not tria.is_closed():
         raise ValueError("Error: Can only project closed meshes!")
 
     # sub-function to compute flipped area of trias where normal
     # points towards origin, meaningful for the sphere, centered at zero
@@ -508,27 +672,38 @@
     return trianew
 
 
 def tet_compute_gradient(tet, vfunc):
     """
     Computes gradient of a vertex function f (for each tetra)
 
-    Inputs:    vfunc       scalar function at vertices
-
-    :return:   tfunc       3d vector function of gradient at tetras
-
     grad(f) = [  (f_j - f_i) (vi-vk) x (vh-vk)
                + (f_k - f_i) (vi-vh) x (vj-vh)
                + (f_h - f_i) (vk-vi) x (vj-vi) ] / (2 V)
             = [  f_i (?-?) x ( ? -?)
                + f_j (vi-vk) x (vh-vk)
                + f_k (vi-vh) x (vj-vh)
                + f_h (vk-vi) x (vj-vi) ] / (2 V)
     for tetrahedron (vi,vj,vk,vh) with volume V.
 
+    Parameters
+    ----------
+    tet : TetMesh
+    vfunc : function
+        scalar function at vertices
+
+    Returns
+    -------
+    tfunc : function
+        3d vector function of gradient at tetras
+
+    Notes
+    -----
+    numexpr could speed up this functions if necessary
+
     Good background to read:
     Mancinelli, Livesu, Puppo, Gradient Field Estimation on Triangle Meshes
     http://pers.ge.imati.cnr.it/livesu/papers/MLP18/MLP18.pdf
     http://dgd.service.tu-berlin.de/wordpress/vismathws10/2012/10/17/gradient-of-scalar-functions/
     Desbrun ...
     """
     import sys
@@ -564,26 +739,36 @@
     return tfunc
 
 
 def tet_compute_divergence(tet, tfunc):
     """
     Computes integrated divergence of a 3d tetra function f (for each vertex)
 
-    Inputs:    tfunc       3d vector field on tets
-
-    :return:   vfunc       scalar function of divergence at vertices
-
     Divergence is the flux density leaving or entering a point.
     It can be measured by summing the dot product of the vector
     field with the normals to the outer faces of the 1-ring tetras
     around a vertex. Summing < tfunc , n_tria_oposite_v >
 
-    Note: this is the integrated divergence, you may want to multiply
+    Parameters
+    ----------
+    tet : TetMesh
+    tfunc : function
+        3d vector field on tets
+
+    Returns
+    -------
+    vfunc: function
+        scalar function of divergence at vertices
+
+    Notes
+    -----
+    this is the integrated divergence, you may want to multiply
     with B^-1 to get back the function in some applications
     """
+
     v0 = tet.v[tet.t[:, 0], :]
     v1 = tet.v[tet.t[:, 1], :]
     v2 = tet.v[tet.t[:, 2], :]
     v3 = tet.v[tet.t[:, 3], :]
     e0 = v1 - v0
     e1 = v2 - v1
     e2 = v2 - v0
```

### Comparing `lapy-0.4.1/lapy/FuncIO.py` & `lapy-0.6.0/lapy/FuncIO.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,30 @@
 
 
 def import_vfunc_deprecated(infile):
     """
     Imports vertex function from txt file. Values can be separated by ; or ,
     and surrounded by {} or () brackets. Also first line can have the
     keyword "Solution:", i.e. the PSOL format from ShapeDNA
+
+    Parameters
+    ----------
+    infile : str
+        filename of input
+
+    Returns
+    -------
+    vals : list
+        list of vfunc parameters
+
+    Notes
+    ------
+    deprecated, use import_vfunc() instead
     """
+
     import re
 
     try:
         f = open(infile, "r")
     except IOError:
         print("[File " + infile + " not found or not readable]")
         return
@@ -34,25 +49,35 @@
 
 
 def import_vfunc(filename):
     """
     Imports vertex function from txt file. Values can be separated by ; or ,
     and surrounded by {} or () brackets. Also first line can have the
     keyword "Solution:", i.e. the PSOL format from ShapeDNA
+
+    Parameters
+    ----------
+    filename : str
+        filename of input
+
+    Returns
+    -------
+    vals : np.ndarray
+        list of vfunc parameters
     """
 
     import re
 
     import numpy as np
 
     try:
         with open(filename) as f:
             txt = f.readlines()
     except IOError:
-        print("[File " + infile + " not found or not readable]")
+        print("[File " + filename + " not found or not readable]")
         return
 
     txt = [x.strip() for x in txt]
 
     txt.remove("Solution:")
 
     txt = [re.sub("[{()}]", "", x) for x in txt]
@@ -66,15 +91,27 @@
 
     return txt
 
 
 def import_ev(infile):
     """
     Load EV file
+
+    Parameters
+    ----------
+    infile : str
+        filename of input
+
+    Returns
+    -------
+    d: dict
+        dictionary of eigenvalues, eigenvectors (optional), and associated
+        information
     """
+
     # open file
     try:
         f = open(infile, "r")
     except IOError:
         print("[File " + infile + " not found or not readable]")
         return
     # read file (and get rid of all \n)
@@ -192,15 +229,24 @@
     return d
 
 
 def export_ev(outfile, d):
     """
     Save EV data structures as txt file (format from ShapeDNA)
     usage: exportEV(data,outfile)
+
+    Parameters
+    ----------
+    outfile : str
+        filename to save to
+    d : dict
+        dictionary of eigenvalues, eigenvectors (optional), and associated
+        information
     """
+
     # open file
     try:
         f = open(outfile, "w")
     except IOError:
         print("[File " + outfile + " not writable]")
         return
     # check data structure
@@ -280,15 +326,23 @@
     f.close()
 
 
 def export_vfunc(outfile, vfunc):
     """
     Exports vertex function in PSOL txt file:
     First line "Solution:", "," separated values inside ()
+
+    Parameters
+    ----------
+    outfile : str
+        filename to save to
+    vfunc : array_like
+        list of vfunc parameters
     """
+
     try:
         f = open(outfile, "w")
     except IOError:
         print("[File " + outfile + " not writable]")
         return
     f.write("Solution:\n")
     f.write("(" + ",".join(vfunc.astype(str)) + ")")
```

### Comparing `lapy-0.4.1/lapy/Plot.py` & `lapy-0.6.0/lapy/Plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 """
-
 Dependency:
     plotly 3.6
 
 In jupyter notebook do this:
     import plotly
     plotly.offline.init_notebook_mode(connected=True)
-
 """
 import re
 from bisect import bisect
 
 import numpy as np
 import plotly
 import plotly.graph_objs as go
 
 # import matplotlib.cm as cm
 from .TetMesh import TetMesh
 
 
 def _get_color_levels():
+    """returns a pre-set colorscale
+
+    Returns
+    -------
+    colorscale: array_like of shape (38, 2)
+        vector color for different levels
+    """
+
     color1 = "rgb(55, 155, 255)"
     color2 = "rgb(255, 255, 0)"
     colorscale = [
         [0, color1],
         [0.09999, color1],
         [0.1, color2],
         [0.105, color2],
@@ -62,15 +68,30 @@
         [0.9050001, color1],
         [1, color1],
     ]
     return colorscale
 
 
 def _get_colorscale(vmin, vmax):
-    # put together a colorscale map depending on the range of v-values
+    """
+    put together a colorscale map depending on the range of v-values
+    Parameters
+
+    ----------
+    vmin : float
+        minimum value
+    vmax : float
+        maximum value
+
+    Returns
+    -------
+    colorscale: array_like of shape (2,2)
+        colorscale map
+    """
+
     if vmin > vmax:
         raise ValueError("incorrect relation between vmin and vmax")
     # color definitions
     posstart = "rgb(255, 0, 0)"
     posstop = "rgb(255, 255, 51)"
     negstart = "rgb(51, 255, 255)"
     negstop = "rgb(0, 0, 255)"
@@ -112,18 +133,29 @@
                 [zz + zero + eps, posstart],
                 [1, posstop],
             ]
     return colorscale
 
 
 def _get_colorval(t, colormap):
-    # t must be 0...1 and
-    # colormap is a list of values and color code strings
-    #     (should have entries at least for 0 and 1)
-    # we return the interpolated color for this value of t
+    """turn a scalar value into a color value
+
+    Parameters
+    ----------
+    t : float
+        must be 0...1
+    colormap : array_like
+        list of values and color code strings (should have entries at least for 0 and 1)
+
+    Returns
+    -------
+    cstr/*: str
+        interpolated color for this value of t
+    """
+
     if t == 0:
         return colormap[0][1]
     if t == 1:
         return colormap[-1][1]
     # ok here we need to interpolate
     # first find two colors before and after
     columns = list(zip(*colormap))
@@ -142,15 +174,34 @@
     cval = np.rint(rv1 + tt * (rv2 - rv1)).astype(int)
     # format as string again
     cstr = "rgb(%d, %d, %d)" % (cval[0], cval[1], cval[2])
     return cstr
 
 
 def _map_z2color(zval, colormap, zmin, zmax):
-    # map the normalized value zval to a corresponding color in the colormap
+    """
+    map the normalized value zval to a corresponding color in the colormap
+
+    Parameters
+    ----------
+    zval : float
+        value to be mapped
+    colormap : matplotlib.colors.LinearSegmentedColormap or np.ndarray
+        list of values and color code strings
+    zmin : float
+        minimum
+    zmax : float
+        minimum
+
+    Returns
+    -------
+    rgb : str
+        corresponding color of the zval
+    """
+
     if zmin > zmax:
         raise ValueError("incorrect relation between zmin and zmax")
 
     t = (zval - zmin) / float((zmax - zmin))  # normalize val
     if type(colormap) == "matplotlib.colors.LinearSegmentedColormap":
         r, g, b, alpha = colormap(t)
         rgb = (
@@ -167,15 +218,15 @@
 
     return rgb
 
 
 def plot_tet_mesh(
     tetra,
     vfunc=None,
-    plot_edges=None,
+    plot_edges=False,
     plot_levels=False,
     tfunc=None,
     cutting=None,
     edge_color="rgb(50,50,50)",
     html_output=False,
     width=800,
     height=800,
@@ -183,33 +234,64 @@
     xrange=None,
     yrange=None,
     zrange=None,
     showcaxis=False,
     caxis=None,
 ):
     """
-    this is a function to plot tetra meshes
+    plot tetra meshes
 
-    it is essentially a wrapper around the plotTriaMesh function,
-    as the tetra mesh will be converted to its tria boundary mesh,
+    the tetra mesh will be converted to its tria boundary mesh,
     and only this will be plotted.
 
-    to view the 'interior' of the tetra mesh, one or more cutting
-    criteria can be defined as input arguments to this function:
-
-    e.g. cutting=('x<-10') or cutting=('z>=5') or cutting=('f>4')
-
-    where x,y,z represent dimensions 0,1,2 of the vertex array,
-    and f represents the vfunc (which cannot be None if f is used
-    to define a cutting criterion)
-
-    only tetras whose vertices fulfill all criteria will be considered
-    for plotting
-
+    Parameters
+    ----------
+    tetra : lapy.TetMesh.TetMesh
+        tetraheral mesh to plot
+    vfunc : function, Default=None
+        scalar function at vertices
+    plot_edges : bool, Default=False
+        whether to plot edges or not
+    plot_levels : bool, Default=False
+        whether to plot levels or not
+    tfunc : function, Default=None
+        3d vector function of gradient
+    cutting : str, Default=None
+        to view the 'interior' of the tetra mesh, one or more cutting
+        criteria can be defined as input arguments to this function:
+
+        e.g. cutting=('x<-10') or cutting=('z>=5') or cutting=('f>4')
+
+        where x,y,z represent dimensions 0,1,2 of the vertex array,
+        and f represents the vfunc (which cannot be None if f is used
+        to define a cutting criterion)
+    edge_color : str, Default="rgb(50,50,50)"
+        color of the edge
+    html_output : bool, Default=False
+        weather or not to give out as html output
+    width : int, Default=800
+        width of the plot (in px)
+    height : int, Default=800
+        height  of the plot (in px)
+    flatshading : bool, Default=False
+        whether normal smoothing is applied to the meshes or not
+    xrange : list or tuple of shape (2, 1)
+        Sets the range of the x-axis
+    yrange : list or tuple of shape (2, 1)
+        Sets the range of the y-axis
+    zrange :  list or tuple of shape (2, 1)
+        Sets the range of the z-axis
+    showcaxis : bool, Default=False
+        whether a colorbar is displayed or not
+    caxis : list or tuple of shape (2, 1):
+        Sets the bound of the color domain.
+        caxis[0] is lower bound caxis[1] upper bound.
+        Elements are int or float
     """
+
     if type(tetra).__name__ != "TetMesh":
         raise ValueError("plot_tet_mesh works only on TetMesh class")
 
     # from plotTriaMesh import plotTriaMesh
     # from tria import is_oriented
     # from tetra import tetra_get_boundary_tria, tetra_fix_orientation
 
@@ -218,15 +300,16 @@
         # check inputs
         if type(cutting) is not list:
             cutting = [cutting]
 
         # check if vfunc is defined when functional thresholds are used, otherwise exit
         if any(["f" in x for x in cutting]) and vfunc is None:
             raise ValueError(
-                "Need to specify vfunc if 'f' is used within the 'cutting' argument, exiting."
+                "Need to specify vfunc if 'f' is used"
+                " within the 'cutting' argument, exiting."
             )
 
         # create criteria from cutting info
         criteria = (
             "("
             + ")&(".join(
                 [
@@ -299,45 +382,100 @@
     vcolor=None,
     tcolor=None,
     showcaxis=False,
     caxis=None,
     xrange=None,
     yrange=None,
     zrange=None,
-    plot_edges=None,
+    plot_edges=False,
     plot_levels=False,
     edge_color="rgb(50,50,50)",
     tic_color="rgb(50,200,10)",
     background_color=None,
     flatshading=False,
-    view=None,
     width=800,
     height=800,
     camera=None,
     html_output=False,
     export_png=None,
     scale_png=1.0,
     no_display=False,
 ):
+    """
+    plot tria mesh
+
+    Parameters
+    ----------
+    tria : lapy.TriaMesh.Triamesh
+        triangle mesh to plot
+    vfunc : function, Default=None
+        scalar function at vertices
+    tfunc : function, Default=None
+        3d vector function of gradient
+    vcolor : list of str, Default=None
+        Sets the color of each vertex
+    tcolor : list of str, Default=None
+         Sets the color of each face
+    showcaxis : bool, Default=False
+        whether a colorbar is displayed or not
+    caxis : list or tuple of shape (2, 1):
+        Sets the bound of the color domain.
+        caxis[0] is lower bound caxis[1] upper bound.
+        Elements are int or float
+    xrange : list or tuple of shape (2, 1)
+        Sets the range of the x-axis
+    yrange : list or tuple of shape (2, 1)
+        Sets the range of the y-axis
+    zrange :  list or tuple of shape (2, 1)
+        Sets the range of the z-axis
+    plot_edges : bool, Default=False
+        whether to plot edges or not
+    plot_levels : bool, Default=False
+        whether to plot levels or not
+    edge_color : str, Default="rgb(50,50,50)"
+        color of the edge
+    tic_color : str, Default="rgb(50,200,10)"
+        color of the ticks
+    background_color : str, Default=None
+        color of background
+    flatshading : bool, Default=False
+        whether normal smoothing is applied to the meshes or not
+    width : int, Default=800
+        width of the plot (in px)
+    height : int, Default=800
+        height  of the plot (in px)
+    camera :
+    html_output : bool, Default=False
+        weather or not to give out as html output
+    export_png : str or writeable, Default=None
+        local file path or a writeable object to write the image on
+    scale_png : int or float
+        scale factor of image. >1.0 increase resolution; <1.0 decrease resolution
+    no_display : bool, Default=False
+        whether to plot on display or not
+    """
+
     # interesting example codes:
     # https://plot.ly/~empet/14749/mesh3d-with-intensities-and-flatshading/#/
-    #
+
     if type(tria).__name__ != "TriaMesh":
         raise ValueError("plot_tria_mesh works only on TriaMesh class")
 
     if (vfunc is not None or tfunc is not None) and (
         vcolor is not None or tcolor is not None
     ):
         raise ValueError(
-            "plot_tria_mesh can only use either vfunc/tfunc or vcolor/tcolor, but not both at the same time"
+            "plot_tria_mesh can only use either vfunc/tfunc or vcolor/tcolor,"
+            " but not both at the same time"
         )
 
     if vcolor is not None and tcolor is not None:
         raise ValueError(
-            "plot_tria_mesh can only use either vcolor or tcolor, but not both at the same time"
+            "plot_tria_mesh can only use either vcolor or tcolor,"
+            " but not both at the same time"
         )
 
     x, y, z = zip(*tria.v)
     i, j, k = zip(*tria.t)
 
     vlines = []
     if vfunc is None:
```

### Comparing `lapy-0.4.1/lapy/Solver.py` & `lapy-0.6.0/lapy/Solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import importlib
 from typing import Optional, Tuple, Union
 
 import numpy as np
 from scipy import sparse
 
 from .TetMesh import TetMesh
 from .TriaMesh import TriaMesh
@@ -29,34 +30,39 @@
         If a tuple ``(a_min, a_max), differentially affects the minimum and maximum
         curvature directions. e.g. ``(0, 50)`` will set scaling to 1 into the minimum
         curvature direction, even if the maximum curvature is large in those regions (
         i.e. isotropic in regions with large maximum curvature and minimum curvature
         close to 0, i.e. a concave cylinder).
     aniso_smooth : int
         Number of smoothing iterations for curvature computation on vertices.
-    use_cholmod : bool
+    use_cholmod : bool, default: False
         If True, attempts to use the Cholesky decomposition for improved execution
-        speed. Requires the ``scikit-sparse`` library. If it can not be found, fallback
-        to LU decomposition.
+        speed. Requires the ``scikit-sparse`` library. If it can not be found, an error 
+        will be thrown.
+        If False, will use slower LU decomposition.
 
     Notes
     -----
     The class has a static member to create the mass matrix of `~lapy.TriaMesh` for
     external function that do not need stiffness.
     """
 
     def __init__(
         self,
         geometry: Union[TriaMesh, TetMesh],
         lump: bool = False,
         aniso: Optional[Union[float, Tuple[float, float]]] = None,
         aniso_smooth: int = 10,
-        use_cholmod: bool = True,
+        use_cholmod: bool = False,
     ) -> None:
-        self.sksparse = import_optional_dependency("sksparse", raise_error=use_cholmod)
+        if use_cholmod:
+            self.sksparse = import_optional_dependency("sksparse", raise_error=True)
+            importlib.import_module(".cholmod", self.sksparse.__name__)
+        else:
+            self.sksparse = None
         if type(geometry).__name__ == "TriaMesh":
             if aniso is not None:
                 # anisotropic Laplace
                 print("TriaMesh with anisotropic Laplace-Beltrami")
                 u1, u2, c1, c2 = geometry.curvature_tria(smoothit=aniso_smooth)
                 # Diag mat to specify anisotropy strength
                 if isinstance(aniso, (list, tuple, set, np.ndarray)):
@@ -80,14 +86,15 @@
             print("TetMesh with regular Laplace")
             a, b = self._fem_tetra(geometry, lump)
         else:
             raise ValueError('Geometry type "' + type(geometry).__name__ + '" unknown')
         self.stiffness = a
         self.mass = b
         self.geotype = type(geometry)
+        self.use_cholmod = use_cholmod
 
     @staticmethod
     def _fem_tria(tria: TriaMesh, lump: bool = False):  # computeABtria(v,t)
         r"""Compute the 2 sparse symmetric matices of the Laplace-Beltrami operator for a triangle mesh.
 
         The 2 sparse symmetric matrices are computed for a given triangle mesh using the
         linear finite element method (assuming a closed mesh or Neumann boundary
@@ -621,27 +628,27 @@
         eigenvalues : array of shape (k)
             Array of k eigenvalues. For closed meshes or Neumann boundary condition,
             ``0`` will be the first eigenvalue (with constant eigenvector).
         eigenvectors : array of shape (N, k)
             Array representing the k eigenvectors. The column ``eigenvectors[:, i]`` is
             the eigenvector corresponding to ``eigenvalues[i]``.
         """
-        from scipy.sparse.linalg import LinearOperator
+        from scipy.sparse.linalg import LinearOperator, eigsh
 
         sigma = -0.01
-        if self.sksparse is not None:
+        if self.use_cholmod:
             print("Solver: Cholesky decomposition from scikit-sparse cholmod ...")
             chol = self.sksparse.cholmod.cholesky(self.stiffness - sigma * self.mass)
             op_inv = LinearOperator(
                 matvec=chol,
                 shape=self.stiffness.shape,
                 dtype=self.stiffness.dtype,
             )
         else:
-            from scipy.sparse.linalg import eigsh, splu
+            from scipy.sparse.linalg import splu
 
             print("Solver: spsolve (LU decomposition) ...")
             # turns out it is much faster to use cholesky and pass operator
             lu = splu(self.stiffness - sigma * self.mass)
             op_inv = LinearOperator(
                 matvec=lu.solve,
                 shape=self.stiffness.shape,
@@ -752,17 +759,17 @@
                 a = a[:, mask]
             else:
                 raise ValueError("A matrix needs to be sparse CSC or CSR")
         else:
             a = self.stiffness
         # solve A x = b
         print("Matrix Format now: " + a.getformat())
-        if self.sparse is not None:
+        if self.use_cholmod:
             print("Solver: Cholesky decomposition from scikit-sparse cholmod ...")
-            chol = self.sparse.cholesky(a)
+            chol = self.sksparse.cholmod.cholesky(a)
             x = chol(b)
         else:
             from scipy.sparse.linalg import splu
 
             print("Solver: spsolve (LU decomposition) ...")
             lu = splu(a)
             x = lu.solve(b.astype(np.float32))
```

### Comparing `lapy-0.4.1/lapy/TetIO.py` & `lapy-0.6.0/lapy/TetIO.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,26 @@
 
 from .TetMesh import TetMesh
 
 
 def import_gmsh(infile):
     """
     Load GMSH tetrahedron mesh
+
+    Parameters
+    ----------
+    infile : str
+        filename to load
+
+    Returns
+    -------
+    tet : TetMesh
+        Object of loaded  GMSH tetrahedron mesh
     """
+
     extension = os.path.splitext(infile)[1]
     verbose = 1
     if verbose > 0:
         print("--> GMSH format         ... ")
     if extension != ".msh":
         print("[no .msh file] --> FAILED\n")
         return
@@ -101,15 +112,26 @@
     print(" --> DONE ( V: " + str(v.shape[0]) + " , T: " + str(t.shape[0]) + " )\n")
     return TetMesh(v, t)
 
 
 def import_vtk(infile):
     """
     Load VTK tetrahedron mesh
+
+    Parameters
+    ----------
+    infile : str
+        filename to load
+
+    Returns
+    -------
+    tet : TetMesh
+        Object of loaded  VTK tetrahedron mesh
     """
+
     verbose = 1
     if verbose > 0:
         print("--> VTK format         ... ")
     try:
         f = open(infile, "r")
     except IOError:
         print("[file not found or not readable]\n")
@@ -177,16 +199,23 @@
     print(" --> DONE ( V: " + str(v.shape[0]) + " , T: " + str(t.shape[0]) + " )\n")
     return TetMesh(v, t)
 
 
 def export_vtk(tet, outfile):
     """
     Save VTK file
-    usage: exportVTK(TetMesh,outfile)
+
+    Parameters
+    ----------
+    tet : TetMesh
+        tetrahedron mesh to save
+    outfile : str
+        filename to save to
     """
+
     # open file
     try:
         f = open(outfile, "w")
     except IOError:
         print("[File " + outfile + " not writable]")
         return
     # check data structure
```

### Comparing `lapy-0.4.1/lapy/TetMesh.py` & `lapy-0.6.0/lapy/TetMesh.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,41 +11,86 @@
 """
 
 import numpy as np
 from scipy import sparse
 
 
 class TetMesh:
-    """A class representing a tetraheral mesh"""
+    """
+    A class representing a tetraheral mesh
+
+    Attributes
+    -------
+    v : array_like
+        List of lists of 3 float coordinates
+    t : array_like
+        List of lists of 4 int of indices (>=0) into v array
+    adj_sym : scipy.sparse.csc_matrix
+        symmetric adjacency matrix as csc sparse matrix
+
+    Methods
+    -------
+    construct_adj_sym()
+        Creates adjacency symmetric matrix
+    has_free_vertices()
+        Checks if the vertex list has more vertices than what is used in tetra
+    is_oriented()
+        Check if tet mesh is oriented
+    avg_edge_length()
+        Get average edge lengths in tet mesh
+    boundary_tria(tetfunc)
+        Get boundary triangle mesh of tetrahedra
+    rm_free_vertices_()
+        Remove unused (free) vertices from v and t
+    orient_()
+        Ensure that tet mesh is oriented
+    """
 
     def __init__(self, v, t):
+        """Constructor
+
+        Parameters
+        ----------
+        v : array_like
+            List of lists of 3 float coordinates
+        t : array_like
+            List of lists of 4 int of indices (>=0) into v array
+            Ordering is important: so that t0,t1,t2 are oriented
+            counterclockwise when looking from above, and t3 is
+            on top of that triangle.
+
+        Raises
+        -------
+        ValueError
+            Max index exceeds number of vertices
         """
-        Inputs:   v - vertices   List of lists of 3 float coordinates
-                  t - tetra      List of lists of 4 int of indices (>=0) into v array
-                                 Ordering is important: so that t0,t1,t2 are oriented
-                                 counterclockwise when looking from above, and t3 is
-                                 on top of that triangle.
-        """
+
         self.v = np.array(v)
         self.t = np.array(t)
         vnum = np.max(self.v.shape)
         if np.max(self.t) >= vnum:
             raise ValueError("Max index exceeds number of vertices")
         # put more checks here (e.g. the dim 3 conditions on columns)
         # self.orient_()
         self.adj_sym = self.construct_adj_sym()
 
     def construct_adj_sym(self):
-        """
+        """Creates adjacency symmetric matrix
+
         The adjacency matrix will be symmetric. Each inner
         edge will get the number of tetrahedra that contain this edge.
         Inner edges are usually 3 or larger, boundary, 2 or 1.
         Works on tetras only.
-        :return:    symmetric adjacency matrix as csc sparse matrix
+
+        Returns
+        -------
+        adj : scipy.sparse.csc_matrix
+            symmetric adjacency matrix as csc sparse matrix
         """
+
         t1 = self.t[:, 0]
         t2 = self.t[:, 1]
         t3 = self.t[:, 2]
         t4 = self.t[:, 3]
         i = np.column_stack((t1, t2, t2, t3, t3, t1, t1, t2, t3, t4, t4, t4)).reshape(
             -1
         )
@@ -55,28 +100,37 @@
         adj = sparse.csc_matrix((np.ones(i.shape), (i, j)))
         return adj
 
     def has_free_vertices(self):
         """
         Checks if the vertex list has more vertices than what is used in tetra
         (same implementation as in TriaMesh)
-        :return:    bool
+
+        Returns
+        -------
+        bool
+            whether vertex list has more vertices than tetra or not
         """
+
         vnum = np.max(self.v.shape)
         vnumt = len(np.unique(self.t.reshape(-1)))
         return vnum != vnumt
 
     def is_oriented(self):
         """
         Check if tet mesh is oriented. True if all tetrahedra are oriented
         so that v0,v1,v2 are oriented counterclockwise when looking from above,
         and v3 is on top of that triangle.
 
-        :return:   oriented       bool True if max(adj_directed)=1
+        Returns
+        -------
+        oriented: bool
+            True if max(adj_directed)=1
         """
+
         # Compute vertex coordinates and a difference vector for each triangle:
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         t3 = self.t[:, 3]
         v0 = self.v[t0, :]
         v1 = self.v[t1, :]
@@ -100,39 +154,52 @@
         else:
             print("Orientations are not uniform")
             return False
 
     def avg_edge_length(self):
         """
         Get average edge lengths in tet mesh
-        :return:    double  average edge length
+
+        Returns
+        -------
+        double
+            average edge length
         """
+
         # get only upper off-diag elements from symmetric adj matrix
         triadj = sparse.triu(self.adj_sym, 1, format="coo")
         edgelens = np.sqrt(
             ((self.v[triadj.row, :] - self.v[triadj.col, :]) ** 2).sum(1)
         )
         return edgelens.mean()
 
     def boundary_tria(self, tetfunc=None):
         """
-        Get boundary triangle mesh of tetrahedra (can have multiple connected components).
-        Tria will have same vertices (including free vertices), so that the tria indices
-        agree with the tet-mesh, in case we want to transfer information back, e.g.
-        a FEM boundary condition, or to access a TetMesh vertex function with
-        TriaMesh.t indices.
+        Get boundary triangle mesh of tetrahedra (can have multiple connected
+        components). Tria will have same vertices (including free vertices),
+        so that the tria indices agree with the tet-mesh, in case we want to
+        transfer information back, e.g. a FEM boundary condition, or to access
+        a TetMesh vertex function with TriaMesh.t indices.
 
         !! Note, that it seems to be returning non-oriented triangle meshes,
         may need some debugging, until then use tria.orient_() after this. !!
 
-        Inputs:   tetfunc        List of tetra function values (optional)
-
-        :return:  TriaMesh       TriaMesh of boundary (potentially >1 components)
-                  triafunc       List of tria function values (if tetfunc passed)
+        Parameters
+        ----------
+        tetfunc : array_like, Default=None
+            List of tetra function values (optional)
+
+        Returns
+        -------
+        TriaMesh
+            TriaMesh of boundary (potentially >1 components)
+        triafunc array_like
+            List of tria function values (if tetfunc passed)
         """
+
         from .TriaMesh import TriaMesh
 
         # get all triangles
         allt = np.vstack(
             (
                 self.t[:, np.array([3, 1, 2])],
                 self.t[:, np.array([2, 0, 3])],
@@ -161,17 +228,27 @@
         Remove unused (free) vertices from v and t. These are vertices that are not
         used in any triangle. They can produce problems when constructing, e.g.,
         Laplace matrices.
 
         Will update v and t in mesh.
         Same implementation as in TriaMesh
 
-        :return:    vkeep          Indices (from original list) of kept vertices
-                    vdel           Indices of deleted (unused) vertices
+        Returns
+        -------
+        vkeep: np.ndarray
+            Indices (from original list) of kept vertices
+        vdel: np.ndarray
+            Indices of deleted (unused) vertices
+
+        Raises
+        -------
+        ValueError
+            Max index exceeds number of vertices
         """
+
         tflat = self.t.reshape(-1)
         vnum = np.max(self.v.shape)
         if np.max(tflat) >= vnum:
             raise ValueError("Max index exceeds number of vertices")
         # determine which vertices to keep
         vkeep = np.full(vnum, False, dtype=bool)
         vkeep[tflat] = True
@@ -194,16 +271,20 @@
 
     def orient_(self):
         """
         Ensure that tet mesh is oriented. Re-orient tetras so that
         v0,v1,v2 are oriented counterclockwise when looking from above,
         and v3 is on top of that triangle.
 
-        :return:    int     number of re-oriented tetras
+        Returns
+        -------
+        onum : int
+            number of re-oriented tetras
         """
+
         # Compute vertex coordinates and a difference vector for each tetra:
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         t3 = self.t[:, 3]
         v0 = self.v[t0, :]
         v1 = self.v[t1, :]
```

### Comparing `lapy-0.4.1/lapy/TriaIO.py` & `lapy-0.6.0/lapy/TriaIO.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,26 @@
 
 from .TriaMesh import TriaMesh
 
 
 def import_fssurf(infile):
     """
     Load triangle mesh from FreeSurfer surface geometry file
-    :return:    TriaMesh
+
+    Parameters
+    ----------
+    infile : str
+        filename to load
+
+    Returns
+    -------
+    TriaMesh
+        loaded triangle mesh
     """
+
     verbose = 1
     if verbose > 0:
         print("--> FS Surf format     ... ")
     try:
         # here we use our copy to also support surfaces from dev (and maybe v7*?)
         # these have an empty line and mess up Nibabel
         # once this is fixed in nibabel we can switch back
@@ -28,16 +38,26 @@
 
     return TriaMesh(surf[0], surf[1], fsinfo=surf[2])
 
 
 def import_off(infile):
     """
     Load triangle mesh from OFF txt file
-    :return:    TriaMesh
+
+    Parameters
+    ----------
+    infile : str
+        filename to load
+
+    Returns
+    -------
+    TriaMesh
+        loaded triangle mesh
     """
+
     verbose = 1
     if verbose > 0:
         print("--> OFF format         ... ")
     try:
         f = open(infile, "r")
     except IOError:
         print("[file not found or not readable]\n")
@@ -75,15 +95,26 @@
     return TriaMesh(v, t)
 
 
 def import_vtk(infile):
     """
     Load triangle mesh from VTK txt file
     :return:    TriaMesh
+
+    Parameters
+    ----------
+    infile : str
+        filename to load
+
+    Returns
+    -------
+    TriaMesh
+        loaded triangle mesh
     """
+
     verbose = 1
     if verbose > 0:
         print("--> VTK format         ... ")
     try:
         f = open(infile, "r")
     except IOError:
         print("[file not found or not readable]\n")
@@ -175,14 +206,35 @@
     print(" --> DONE ( V: " + str(v.shape[0]) + " , T: " + str(t.shape[0]) + " )\n")
     return TriaMesh(v, t)
 
 
 def import_gmsh(infile):
     """
     Load GMSH tetra mesh ASCII Format
+
+    Parameters
+    ----------
+    infile : str
+        filename to load
+
+    Returns
+    -------
+    points : np.ndarray
+        List of points
+    cells : array_like
+        List of cells
+    point_data : array_like
+        data of points
+    cell_data : aray_like
+        data of cells
+    field_data : array_like
+        data of fields
+
+    Notes
+    -------
     http://geuz.org/gmsh/doc/texinfo/gmsh.html#MSH-ASCII-file-format
     .. moduleauthor:: Nico Schloemer <nico.schloemer@gmail.com>
     LICENSE MIT
     https://github.com/nschloe/meshio
     """
 
     import logging
@@ -228,15 +280,15 @@
         11: "tetra10",
         12: "hexahedron27",
         13: "prism18",
         14: "pyramid14",
         26: "line4",
         36: "quad16",
     }
-    _meshio_to_gmsh_type = {v: k for k, v in _gmsh_to_meshio_type.items()}
+    _meshio_to_gmsh_type = {v: k for k, v in _gmsh_to_meshio_type.items()}  # noqa: F841
 
     verbose = 1
     if verbose > 0:
         print("--> GMSH format         ... ")
 
     try:
         f = open(infile, "r")
@@ -421,15 +473,23 @@
     return points, cells, point_data, cell_data, field_data
 
 
 def export_vtk(tria, outfile):
     """
     Save VTK file
     usage: exportVTK(TriaMesh,outfile)
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        Triangle mesh to save
+    outfile : str
+        filename to save to
     """
+
     # open file
     try:
         f = open(outfile, "w")
     except IOError:
         print("[File " + outfile + " not writable]")
         return
     # check data structure
@@ -455,14 +515,25 @@
         f.write("\n")
     f.close()
 
 
 def export_fssurf(tria, outfile):
     """
     Save Freesurfer Surface Geometry file (wrap Nibabel)
+
+    Parameters
+    ----------
+    tria : TriaMesh
+        Triangle mesh to save
+    outfile : str
+        filename to save to
+
+    Returns
+    -------
+    None
     """
     # open file
     try:
         from nibabel.freesurfer.io import write_geometry
 
         write_geometry(outfile, tria.v, tria.t, volume_info=tria.fsinfo)
     except IOError:
```

### Comparing `lapy-0.4.1/lapy/TriaMesh.py` & `lapy-0.6.0/lapy/TriaMesh.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,122 @@
 
 Original Author: Martin Reuter
 Date: Feb-01-2019
 """
 
 
 class TriaMesh:
-    """A class representing a triangle mesh"""
+    """
+    A class representing a triangle mesh
+
+    Attributes
+    -------
+    v : array_like
+        List of lists of 3 float coordinates
+    t : array_like
+        List of lists of 4 int of indices (>=0) into v array
+    adj_sym : scipy.sparse.csc_matrix
+        symmetric adjacency matrix as csc sparse matrix
+    adj_dir :
+        directed adjacency matrix as csc sparse matrix
+    fsinfo :
+        FreeSurfer Surface Header Info
+
+    Methods
+    -------
+    _construct_adj_sym()
+        Constructs symmetric adjacency matrix
+    _construct_adj_dir()
+        Constructs directed adjacency matrix of triangle mesh t
+    construct_adj_dir_tidx()
+        Constructs directed adjacency matrix of triangle mesh t
+        containing the triangle indices
+    is_closed()
+        Check if triangle mesh is closed
+    is_manifold()
+        Check if triangle mesh is manifold
+    is_oriented()
+        Check if triangle mesh is oriented
+    euler()
+        Computes the Euler Characteristic
+    tria_areas()
+        Computes the area of triangles
+    area()
+        Computes the total surface area of triangle mesh
+    volume()
+        Computes the volume of closed triangle mesh
+    vertex_degrees()
+        Computes the vertex degrees
+    vertex_areas()
+        Computes the area associated to each vertex
+    avg_edge_length()
+        Computes the average edge length of the mesh
+    tria_normals()
+        Computes triangle normals
+    vertex_normals()
+        computes vertex normals
+    has_free_vertices()
+        Checks if the vertex list has more vertices
+    tria_qualities()
+        Computes triangle quality for each triangle in mesh
+    boundary_loops()
+        Computes a tuple of boundary loops
+    centroid()
+        Computes centroid of triangle mesh as a weighted average of triangle centers
+    edges(with_boundary=False)
+        Compute vertices and adjacent triangle ids for each edge
+    curvature(smoothit=3)
+        Compute various curvature values at vertices.
+    curvature_tria(smoothit=3)
+        Compute min and max curvature and directions
+    normalize_()
+        Normalizes TriaMesh to unit surface area
+    rm_free_vertices_()
+        Remove unused (free) vertices from v and t
+    refine_(it=1)
+        Refines the triangle mesh
+    normal_offset_(d)
+        moves vertices along normal by distance d
+    orient_()
+        re-orients triangles of manifold mesh to be consistent
+    map_tfunc_to_vfunc(tfunc, weighted=False)
+        Maps function for each tria to each vertex
+    map_vfunc_to_tfunc(vfunc)
+        Maps function for each vertex to each triangle
+    smooth_vfunc(vfunc, n=1):
+        Smoothes vector float function on the mesh iteratively
+    smooth_(n=1)
+        Smoothes mesh in place for a number of iterations
+    """
 
     def __init__(self, v, t, fsinfo=None):
+        """Constructor
+
+        Parameters
+        ----------
+        v : array_like
+            List of lists of 3 float coordinates
+        t : array_like
+            List of lists of 3 int of indices (>=0) into v array
+            Ordering is important: All triangles should be
+            oriented the same way (counter-clockwise, when
+            looking from above)
+        fsinfo : dict, Default=None
+            FreeSurfer Surface Header Info
+
+        Raises
+        -------
+        ValueError
+            Max index exceeds number of vertices
+        ValurError
+            Triangles should have 3 vertices
+        ValueError
+            Vertices should have 3 coordinates
         """
-        :param    v - vertices   List of lists of 3 float coordinates
-                  t - triangles  List of lists of 3 int of indices (>=0) into v array
-                                 Ordering is important: All triangles should be
-                                 oriented the same way (counter-clockwise, when
-                                 looking from above)
-                  fsinfo         optional, FreeSurfer Surface Header Info
-        """
+
         self.v = np.array(v)
         self.t = np.array(t)
         # transpose if necessary
         if self.v.shape[0] < self.v.shape[1]:
             self.v = self.v.T
         if self.t.shape[0] < self.t.shape[1]:
             self.t = self.t.T
@@ -44,63 +141,83 @@
         self.adj_dir = self._construct_adj_dir()
         self.fsinfo = fsinfo  # place for Freesurfer Header info
 
     def _construct_adj_sym(self):
         """
         Constructs symmetric adjacency matrix (edge graph) of triangle mesh t
         Operates only on triangles.
-        :return:    Sparse symmetric CSC matrix
-                    The non-directed adjacency matrix
-                    will be symmetric. Each inner edge (i,j) will have
-                    the number of triangles that contain this edge.
-                    Inner edges usually 2, boundary edges 1. Higher
-                    numbers can occur when there are non-manifold triangles.
-                    The sparse matrix can be binarized via:
-                    adj.data = np.ones(adj.data.shape)
+
+        Returns
+        -------
+        scipy.sparse.csc_matrix
+            Sparse symmetric CSC matrix
+            The non-directed adjacency matrix
+            will be symmetric. Each inner edge (i,j) will have
+            the number of triangles that contain this edge.
+            Inner edges usually 2, boundary edges 1. Higher
+            numbers can occur when there are non-manifold triangles.
+            The sparse matrix can be binarized via:
+            adj.data = np.ones(adj.data.shape)
         """
+
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         i = np.column_stack((t0, t1, t1, t2, t2, t0)).reshape(-1)
         j = np.column_stack((t1, t0, t2, t1, t0, t2)).reshape(-1)
         dat = np.ones(i.shape)
         n = self.v.shape[0]
         return sparse.csc_matrix((dat, (i, j)), shape=(n, n))
 
     def _construct_adj_dir(self):
         """
         Constructs directed adjacency matrix (edge graph) of triangle mesh t
         Operates only on triangles.
-        :return:    Sparse CSC matrix
-                    The directed adjacency matrix is not symmetric if
-                    boundaries exist or if mesh is non-manifold.
-                    For manifold meshes, there are only entries with
-                    value 1. Symmetric entries are inner edges. Non-symmetric
-                    are boundary edges. The direction prescribes a direction
-                    on the boundary loops. Adding the matrix to its transpose
-                    creates the non-directed version.
+
+        Returns
+        -------
+        scipy.sparse.csc_matrix
+            Sparse CSC matrix
+            The directed adjacency matrix is not symmetric if
+            boundaries exist or if mesh is non-manifold.
+            For manifold meshes, there are only entries with
+            value 1. Symmetric entries are inner edges. Non-symmetric
+            are boundary edges. The direction prescribes a direction
+            on the boundary loops. Adding the matrix to its transpose
+            creates the non-directed version.
         """
+
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
         i = np.column_stack((t0, t1, t2)).reshape(-1)
         j = np.column_stack((t1, t2, t0)).reshape(-1)
         dat = np.ones(i.shape)
         n = self.v.shape[0]
         return sparse.csc_matrix((dat, (i, j)), shape=(n, n))
 
     def construct_adj_dir_tidx(self):
         """
         Constructs directed adjacency matrix (edge graph) of triangle mesh t
         containing the triangle indices (only for non-manifold meshes)
         Operates only on triangles.
-        :return:    Sparse CSC matrix
-                    Similar to adj_dir, but stores the tria idx+1 instead
-                    of one in the matrix (allows lookup of vertex to tria).
+
+        Returns
+        -------
+        scipy.sparse.csc_matrix
+            Sparse CSC matrix
+            Similar to adj_dir, but stores the tria idx+1 instead
+            of one in the matrix (allows lookup of vertex to tria).
+
+        Raises
+        -------
+        ValueError
+            Can only tidx matrix for oriented triangle meshes!
         """
+
         if not self.is_oriented():
             raise ValueError(
                 "Error: Can only tidx matrix for oriented triangle meshes!"
             )
         t0 = self.t[:, 0]
         t1 = self.t[:, 1]
         t2 = self.t[:, 2]
@@ -111,52 +228,77 @@
         n = self.v.shape[0]
         return sparse.csc_matrix((dat, (i, j)), shape=(n, n))
 
     def is_closed(self):
         """
         Check if triangle mesh is closed (no boundary edges)
         Operates only on triangles
-        :return:   closed         bool True if no boundary edges in adj matrix
+
+        Returns
+        -------
+        bool
+            True if no boundary edges in adj matrix
         """
+
         return 1 not in self.adj_sym.data
 
     def is_manifold(self):
         """
         Check if triangle mesh is manifold (no edges with >2 triangles)
         Operates only on triangles
-        :return:   manifold       bool True if no edges with > 2 triangles
+
+        Returns
+        -------
+        bool:
+            True if no edges with > 2 triangles
         """
+
         return np.max(self.adj_sym.data) <= 2
 
     def is_oriented(self):
         """
         Check if triangle mesh is oriented. True if all triangles are oriented
         counter-clockwise, when looking from above.
         Operates only on triangles
-        :return:   oriented       bool True if max(adj_directed)=1
+
+        Returns
+        -------
+        bool
+            True if max(adj_directed)=1
         """
+
         return np.max(self.adj_dir.data) == 1
 
     def euler(self):
         """
         Computes the Euler Characteristic (=#V-#E+#T)
         Operates only on triangles
-        :return:   euler          Euler Characteristic (2=sphere,0=torus)
+
+        Returns
+        -------
+        int
+            Euler Characteristic (2=sphere,0=torus)
         """
+
         # v can contain unused vertices so we get vnum from trias
         vnum = len(np.unique(self.t.reshape(-1)))
         tnum = np.max(self.t.shape)
         enum = int(self.adj_sym.nnz / 2)
         return vnum - enum + tnum
 
     def tria_areas(self):
         """
         Computes the area of triangles using Heron's formula
-        :return:   areas          ndarray with areas of each triangle
+
+        Returns
+        -------
+        areas : np.ndarray
+            array with areas of each triangle
         """
+
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv1 = v2 - v1
         v0mv2 = v0 - v2
         a = np.sqrt(np.sum(v1mv0 * v1mv0, axis=1))
@@ -165,24 +307,39 @@
         ph = 0.5 * (a + b + c)
         areas = np.sqrt(ph * (ph - a) * (ph - b) * (ph - c))
         return areas
 
     def area(self):
         """
         Computes the total surface area of triangle mesh
-        :return:   area           Total surface area
+
+        Returns
+        -------
+        float
+            Total surface area
         """
+
         areas = self.tria_areas()
         return np.sum(areas)
 
     def volume(self):
         """
         Computes the volume of closed triangle mesh, summing tetrahedra at origin
-        :return:   volume         Total enclosed volume
+
+        Returns
+        -------
+        vol : float
+            Total enclosed volume
+
+        Raises
+        -------
+        ValueError
+            can only compute volume for oriented triangle meshes
         """
+
         if not self.is_closed():
             return 0.0
         if not self.is_oriented():
             raise ValueError(
                 "Error: Can only compute volume for oriented triangle meshes!"
             )
         v0 = self.v[self.t[:, 0], :]
@@ -194,24 +351,34 @@
         spatvol = np.sum(v0 * cr, axis=1)
         vol = np.sum(spatvol) / 6.0
         return vol
 
     def vertex_degrees(self):
         """
         Computes the vertex degrees (number of edges at each vertex)
-        :return:   vdeg           Array of vertex degrees
+
+        Returns
+        -------
+        vdeg : np.ndarray
+            Array of vertex degrees
         """
+
         vdeg = np.bincount(self.t.reshape(-1))
         return vdeg
 
     def vertex_areas(self):
         """
         Computes the area associated to each vertex (1/3 of one-ring trias)
-        :return:   vareas         Array of vertex areas
+
+        Returns
+        -------
+        vareas : np.ndarray
+            Array of vertex areas
         """
+
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv0 = v2 - v0
         cr = np.cross(v1mv0, v2mv0)
         area = 0.5 * np.sqrt(np.sum(cr * cr, axis=1))
@@ -219,29 +386,39 @@
         # varea = accumarray(t(:),area3(:))./3;
         vareas = np.bincount(self.t.reshape(-1), area3.reshape(-1)) / 3.0
         return vareas
 
     def avg_edge_length(self):
         """
         Computes the average edge length of the mesh
-        :return:   edgelength     Avg. edge length
+
+        Returns
+        -------
+        float
+            Avg. edge length
         """
+
         # get only upper off-diag elements from symmetric adj matrix
         triadj = sparse.triu(self.adj_sym, 1, format="coo")
         edgelens = np.sqrt(
             ((self.v[triadj.row, :] - self.v[triadj.col, :]) ** 2).sum(1)
         )
         return edgelens.mean()
 
     def tria_normals(self):
         """
         Computes triangle normals
         Ordering of trias is important: counterclockwise when looking
-        :return:  n - normals (num triangles X 3 )
+
+        Returns
+        -------
+        n : np.ndarray
+            normals (num triangles X 3 )
         """
+
         import sys
 
         # Compute vertex coordinates and a difference vectors for each triangle:
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
@@ -260,31 +437,42 @@
     def vertex_normals(self):
         """
         get_vertex_normals(v,t) computes vertex normals
             Triangle normals around each vertex are averaged, weighted
             by the angle that they contribute.
             Ordering is important: counterclockwise when looking
             at the triangle from above.
-        :return:  n - normals (num vertices X 3 )
+
+        Returns
+        -------
+        n : np.ndarray
+            normals (num triangles X 3 )
+
+        Raises
+        -------
+        ValueError
+            Vertex normals are meaningless for un-oriented triangle meshes!
         """
+
         if not self.is_oriented():
             raise ValueError(
                 "Error: Vertex normals are meaningless for un-oriented triangle meshes!"
             )
         import sys
 
         # Compute vertex coordinates and a difference vector for each triangle:
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv1 = v2 - v1
         v0mv2 = v0 - v2
         # Compute cross product at every vertex
-        # will all point in the same direction but have different lengths depending on spanned area
+        # will all point in the same direction but have
+        #   different lengths depending on spanned area
         cr0 = np.cross(v1mv0, -v0mv2)
         cr1 = np.cross(v2mv1, -v1mv0)
         cr2 = np.cross(v0mv2, -v2mv1)
         # Add normals at each vertex (there can be duplicate indices in t at vertex i)
         n = np.zeros(self.v.shape)
         np.add.at(n, self.t[:, 0], cr0)
         np.add.at(n, self.t[:, 1], cr1)
@@ -298,30 +486,40 @@
         # n[:, 1] *= lni
         # n[:, 2] *= lni
         return n
 
     def has_free_vertices(self):
         """
         Checks if the vertex list has more vertices than what is used in tria
-        :return:    bool
+
+        Returns
+        -------
+        bool
+            whether vertex list has more vertices or not
         """
+
         vnum = np.max(self.v.shape)
         vnumt = len(np.unique(self.t.reshape(-1)))
         return vnum != vnumt
 
     def tria_qualities(self):
         """
         Computes triangle quality for each triangle in mesh where
         q = 4 sqrt(3) A / (e1^2 + e2^2 + e3^2 )
         where A is the triangle area and ei the edge length of the three edges.
         This measure is used by FEMLAB and can also be found in:
             R.E. Bank, PLTMG ..., Frontiers in Appl. Math. (7), 1990.
         Constants are chosen so that q=1 for the equilateral triangle.
-        :return:    ndarray with triangle qualities
+
+        Returns
+        -------
+        np.ndarray
+            Array with triangle qualities
         """
+
         # Compute vertex coordinates and a difference vectors for each triangle:
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v1mv0 = v1 - v0
         v2mv1 = v2 - v1
         v0mv2 = v0 - v2
@@ -336,16 +534,26 @@
     def boundary_loops(self):
         """
         Computes a tuple of boundary loops. Meshes can have 0 or more boundary
         loops, which are cycles in the directed adjacency graph of the boundary
         edges.
         Works on trias only. Could fail if loops are connected via a single
         vertex (like a figure 8). That case needs debugging.
-        :return:   loops          List of lists with boundary loops
+
+        Returns
+        -------
+        loops : np.ndarray
+            List of lists with boundary loops
+
+        Raises
+        -------
+        ValueError
+            tria not manifold (edges with more than 2 triangles)!
         """
+
         if not self.is_manifold():
             raise ValueError(
                 "Error: tria not manifold (edges with more than 2 triangles)!"
             )
         if self.is_closed():
             return []
         # get directed matrix of only boundary edges
@@ -386,18 +594,22 @@
         """
         Computes centroid of triangle mesh as a weighted average of triangle
         centers. The weight is determined by the triangle area.
         (This could be done much faster if a FEM lumped mass matrix M is
         already available where this would be M*v, because it is equivalent
         with averaging vertices weighted by vertex area)
 
-        :return:    centroid    The centroid of the mesh
-                    totalarea   The total area of the mesh
-
+        Returns
+        -------
+        centroid : float
+            The centroid of the mesh
+        totalarea : float
+            he total area of the mesh
         """
+
         v0 = self.v[self.t[:, 0], :]
         v1 = self.v[self.t[:, 1], :]
         v2 = self.v[self.t[:, 2], :]
         v2mv1 = v2 - v1
         v0mv2 = v0 - v2
         # Compute cross product and area for each triangle:
         cr = np.cross(v2mv1, v0mv2)
@@ -408,26 +620,40 @@
         c = centers * areas[:, np.newaxis]
         return np.sum(c, axis=0), totalarea
 
     def edges(self, with_boundary=False):
         """
         Compute vertices and adjacent triangle ids for each edge
 
-        :param      with_boundary   also work on boundary half edges, default ignore
-
-        :return:    vids            2 column array with starting and end vertex for each
-                                    unique inner edge
-                    tids            2 column array with triangle containing the half edge
-                                    from vids[0,:] to vids [1,:] in first column and the
-                                    neighboring triangle in the second column
-                    bdrvids         if with_boundary is true: 2 column array with each
-                                    boundary half-edge
-                    bdrtids         if with_boundary is true: 1 column array with the
-                                    associated triangle to each boundary edge
+        Parameters
+        ----------
+        with_boundary : bool, Default=False
+            also work on boundary half edges, default ignore
+
+        Returns
+        -------
+        vids : np.ndarray
+            column array with starting and end vertex for each unique inner edge
+        tids : np.ndarray
+            2 column array with triangle containing the half edge
+            from vids[0,:] to vids [1,:] in first column and the
+            neighboring triangle in the second column
+        bdrvids : np.ndarray
+            if with_boundary is true: 2 column array with each
+            boundary half-edge
+        bdrtids : np.ndarray
+            if with_boundary is true: 1 column array with the
+            associated triangle to each boundary edge
+
+        Raises
+        -------
+        ValueError
+            Error: Can only compute edge information for oriented meshes!
         """
+
         if not self.is_oriented():
             raise ValueError(
                 "Error: Can only compute edge information for oriented meshes!"
             )
         adjtria = self.construct_adj_dir_tidx().tolil()
         # for boundary edges, we can just remove those edges (implicitly a zero angle)
         bdredges = []
@@ -453,27 +679,42 @@
         return vids, tids, bdrv, bdrtrias
 
     def curvature(self, smoothit=3):
         """
         Compute various curvature values at vertices.
 
         For the algorithm see e.g.
-        Pierre Alliez, David Cohen-Steiner, Olivier Devillers, Bruno Levy, and Mathieu Desbrun.
+        Pierre Alliez, David Cohen-Steiner, Olivier Devillers,
+        Bruno Levy, and Mathieu Desbrun.
         Anisotropic Polygonal Remeshing.
         ACM Transactions on Graphics, 2003.
 
-        :param      smoothit  smoothing iterations on vertex functions
-        :return:    u_min     minimal curvature directions (vnum x 3)
-                    u_max     maximal curvature directions (vnum x 3)
-                    c_min     minimal curvature
-                    c_max     maximal curvature
-                    c_mean    mean curvature: (c_min + c_max) / 2.0
-                    c_gauss   Gauss curvature: c_min * c_max
-                    normals   normals (vnum x 3)
+        Parameters
+        ----------
+        smoothit : int, Default=3
+            smoothing iterations on vertex functions
+
+        Returns
+        -------
+        u_min : np.ndarray
+            minimal curvature directions (vnum x 3)
+        u_max : np.ndarray
+             maximal curvature directions (vnum x 3)
+        c_min : np.ndarray
+             minimal curvature
+        c_max : np.ndarray
+             maximal curvature
+        c_mean : np.ndarray
+            mean curvature: (c_min + c_max) / 2.0
+        c_gauss : np.ndarray
+           Gauss curvature: c_min * c_max
+        normals : np.ndarray
+           normals (vnum x 3)
         """
+
         # import warnings
         # warnings.filterwarnings('error')
         import sys
 
         # get edge information for inner edges (vertex ids and tria ids):
         vids, tids = self.edges()
         # compute normals for each tria
@@ -570,20 +811,32 @@
 
     def curvature_tria(self, smoothit=3):
         """
         Compute min and max curvature and directions (orthogonal and in tria plane)
         for each triangle. First we compute these values on vertices and then smooth
         there. Finally they get mapped to the trias (averaging) and projected onto
         the triangle plane, and orthogonalized.
-        :param smoothit: number of smoothing iterations for curvature computation on vertices
-        :return: u_min : min curvature direction on triangles
-                 u_max : max curvature direction on triangles
-                 c_min : min curvature on triangles
-                 c_max : max curvature on triangles
+
+        Parameters
+        ----------
+        smoothit : int, Default=3
+            number of smoothing iterations for curvature computation on vertices
+
+        Returns
+        -------
+        u_min : np.ndarray
+            min curvature direction on triangles
+        u_max : np.ndarray
+            max curvature direction on triangles
+        c_min : np.ndarray
+            min curvature on triangles
+        c_max : np.ndarray
+            max curvature on triangles
         """
+
         u_min, u_max, c_min, c_max, c_mean, c_gauss, normals = self.curvature(smoothit)
 
         # pool vertex functions (u_min and u_max) to triangles:
         tumin = self.map_vfunc_to_tfunc(u_min)
         # tumax = self.map_vfunc_to_tfunc(u_max)
         tcmin = self.map_vfunc_to_tfunc(c_min)
         tcmax = self.map_vfunc_to_tfunc(c_max)
@@ -597,26 +850,29 @@
         tn = np.cross(e0, e1)
         tnl = np.sqrt(np.sum(tn * tn, axis=1)).reshape(-1, 1)
         tn = tn / np.maximum(tnl, 1e-8)
         # project tumin back to tria plane and normalize
         tumin2 = tumin - tn * (np.sum(tn * tumin, axis=1)).reshape(-1, 1)
         tuminl = np.sqrt(np.sum(tumin2 * tumin2, axis=1)).reshape(-1, 1)
         tumin2 = tumin2 / np.maximum(tuminl, 1e-8)
-        # project tumax back to tria plane and normalize (will not be orthogonal to tumin)
+        # project tumax back to tria plane and normalize
+        #   (will not be orthogonal to tumin)
         # tumax1 = tumax - tn * (np.sum(tn * tumax, axis=1)).reshape(-1, 1)
         # in a second step orthorgonalize to tumin
         # tumax1 = tumax1 - tumin * (np.sum(tumin * tumax1, axis=1)).reshape(-1, 1)
         # normalize
         # tumax1l = np.sqrt(np.sum(tumax1 * tumax1, axis=1)).reshape(-1, 1)
         # tumax1 = tumax1 / np.maximum(tumax1l, 1e-8)
         # or simply create vector that is orthogonal to both normal and tumin
         tumax2 = np.cross(tn, tumin2)
         # if really necessary flip direction if that is true for inputs
-        # tumax3 = np.sign(np.sum(np.cross(tumin, tumax) * tn, axis=1)).reshape(-1, 1) * tumax2
-        # I wonder how much changes, if we first map umax to tria and then find orhtogonal umin next?
+        # tumax3 = np.sign(np.sum(np.cross(tumin, tumax) * tn, axis=1)).reshape(-1, 1)
+        #           * tumax2
+        # I wonder how much changes, if we first map umax to tria and then
+        #   find orthogonal umin next?
         return tumin2, tumax2, tcmin, tcmax
 
     def normalize_(self):
         """
         Normalizes TriaMesh to unit surface area with a centroid at the origin.
         Modifies the vertices.
         """
@@ -627,17 +883,27 @@
         """
         Remove unused (free) vertices from v and t. These are vertices that are not
         used in any triangle. They can produce problems when constructing, e.g.,
         Laplace matrices.
 
         Will update v and t in mesh.
 
-        :return:    vkeep          Indices (from original list) of kept vertices
-                    vdel           Indices of deleted (unused) vertices
+        Returns
+        -------
+        vkeep : np.ndarray
+            Indices (from original list) of kept vertices
+        vdel : np.ndarray
+            Indices of deleted (unused) vertices
+
+        Raises
+        ------
+        Value Error
+            Max index exceeds number of vertices
         """
+
         tflat = self.t.reshape(-1)
         vnum = np.max(self.v.shape)
         if np.max(tflat) >= vnum:
             raise ValueError("Max index exceeds number of vertices")
         # determine which vertices to keep
         vkeep = np.full(vnum, False, dtype=bool)
         vkeep[tflat] = True
@@ -658,17 +924,22 @@
         self.__init__(vnew, tnew)
         return vkeep, vdel
 
     def refine_(self, it=1):
         """
         Refines the triangle mesh by placing new vertex on each edge midpoint
         and thus creating 4 similar triangles from one parent triangle.
-        :param    it      : iterations (default 1)
-        :return:  none, modifies mesh in place
+        Modifies mesh in place
+
+        Parameters
+        ----------
+        it : int, default=1
+            number of iterations
         """
+
         for x in range(it):
             # make symmetric adj matrix to upper triangle
             adjtriu = sparse.triu(self.adj_sym, 0, format="csr")
             # create new vertex index for each edge
             edgeno = adjtriu.data.shape[0]
             vno = self.v.shape[0]
             adjtriu.data = np.arange(vno, vno + edgeno)
@@ -689,38 +960,52 @@
             tnew = np.reshape(np.concatenate((t1, t2, t3, t4), axis=1), (-1, 3))
             # set new vertices and tria and re-init adj matrices
             self.__init__(vnew, tnew)
 
     def normal_offset_(self, d):
         """
         normal_offset(d) moves vertices along normal by distance d
-        :param    d    move distance, can be a number or array of vertex length
-        :return:  none, modifies vertices in place
+
+        Parameters
+        ----------
+        d : int or np.ndarray
+            move distance
         """
+
         n = self.vertex_normals()
         vn = self.v + d * n
         self.v = vn
         # no need to re-init, only changed vertices
 
     def orient_(self):
         """
         orient_ re-orients triangles of manifold mesh to be consistent, so that vertices
         are listed counter-clockwise, when looking from above (outside).
 
-        :return:    none, modifies triangles in place and re-inits adj matrices
-
         Algorithm:
         1. Construct list for each half-edge with its triangle and edge direction
         2. Drop boundary half-edges and find half-edge pairs
-        3. Construct sparse matrix with triangle neighbors, with entry 1 for opposite half edges
-           and -1 for parallel half-edges (normal flip across this edge)
-        4. Flood mesh from first tria using triangle neighbor matrix - keeping track of sign
+        3. Construct sparse matrix with triangle neighbors, with entry 1 for opposite
+            half edges and -1 for parallel half-edges (normal flip across this edge)
+        4. Flood mesh from first tria using triangle neighbor matrix
+            - keeping track of sign
         5. When flooded, negative sign for a triangle indicates it needs to be flipped
         6. If global volume is negative, flip everything (first tria was wrong)
+
+        Returns
+        -------
+        flipped : int
+            number of trias flipped
+
+        Raises
+        ------
+        ValueError
+            Without boundary edges, all should have two triangles!
         """
+
         tnew = self.t
         flipped = 0
         if not self.is_oriented():
             # get half edges
             t0 = self.t[:, 0]
             t1 = self.t[:, 1]
             t2 = self.t[:, 2]
@@ -759,15 +1044,16 @@
             tdir = ijks.reshape((-1, 8))[:, [2, 6, 3, 7]]
             # compute sign vector (1 if edge points from small to large, else -1)
             tsgn = 2 * np.logical_xor(tdir[:, 2], tdir[:, 3]) - 1
             # append to itself for symmetry
             tsgn = np.append(tsgn, tsgn)
             i = np.append(tdir[:, 0], tdir[:, 1])
             j = np.append(tdir[:, 1], tdir[:, 0])
-            # construct sparse tria neighbor matrix where weights indicate normal flips across edge
+            # construct sparse tria neighbor matrix where
+            #   weights indicate normal flips across edge
             tmat = sparse.csc_matrix((tsgn, (i, j)))
             tdim = max(i) + 1
             tmat = tmat + sparse.eye(tdim)
             # flood by starting with neighbors of tria 0 to fill all trias
             # sadly we still need a loop for this, matrix power would be too slow
             # as we don't really need to compute full matrix, only need first column
             v = tmat[:, 0]
@@ -800,25 +1086,37 @@
         return flipped
 
     def map_tfunc_to_vfunc(self, tfunc, weighted=False):
         """
         Maps function for each tria to each vertex by attributing 1/3 to each
         Uses vertices and trias.
 
-        :param    tfunc :        Float vector or matrix (#t x N) of values at
-                                 vertices
-        :param    weighted :     False, weigh only by 1/3, e.g. to compute
-                                 vertex areas from tria areas
-                                 True, weigh by triangle area / 3, e.g. to
-                                 integrate a function defined on the trias,
-                                 for example integrating the "one" function
-                                 will also yield the vertex areas.
-
-        :return:   vfunc          Function on vertices vector or matrix (#v x N)
+        Parameters
+        ----------
+        tfunc : np.ndarray
+            Float vector or matrix (#t x N) of values at vertices
+        weighted : bool, default=False
+            False, weigh only by 1/3, e.g. to compute
+            vertex areas from tria areas
+            True, weigh by triangle area / 3, e.g. to
+            integrate a function defined on the trias,
+            for example integrating the "one" function
+            will also yield the vertex areas.
+
+        Returns
+        -------
+        vfunc : np.ndarray
+            Function on vertices vector or matrix (#v x N)
+
+        Raises
+        -------
+        ValueError
+            length of tfunc needs to match number of triangles
         """
+
         if self.t.shape[0] != tfunc.shape[0]:
             raise ValueError(
                 "Error: length of tfunc needs to match number of triangles"
             )
         tfunca = np.array(tfunc)
         # make sure tfunc is 2D (even with only 1-dim input)
         if tfunca.ndim == 1:
@@ -833,35 +1131,53 @@
         return np.squeeze(vfunc / 3.0)
 
     def map_vfunc_to_tfunc(self, vfunc):
         """
         Maps function for each vertex to each triangle by attributing 1/3 to each
         Uses number of vertices and trias
 
-        :param    vfunc          Float vector or matrix (#t x N) of values at
-                                 vertices
-
-        :return:  tfunc          Function on trias vector or matrix (#t x N)
+        Parameters
+        ----------
+        vfunc : np.ndarray
+            Float vector or matrix (#t x N) of values at vertices
+
+        Returns
+        -------
+        tfunc
+            Function on trias vector or matrix (#t x N)
+
+        Raises
+        -------
+        ValueError
+            length of vfunc needs to match number of vertices
         """
+
         if self.v.shape[0] != vfunc.shape[0]:
             raise ValueError("Error: length of vfunc needs to match number of vertices")
         vfunc = np.array(vfunc) / 3.0
         tfunc = np.sum(vfunc[self.t], axis=1)
         return tfunc
 
     def smooth_vfunc(self, vfunc, n=1):
         """
         Smoothes vector float function on the mesh iteratively
 
-        :param    vfunc :            Float vector of values at vertices,
-                                     if empty, use vertex coordinates
-        :param    n :                Number of iterations for smoothing
-
-        :return:  vfunc              Smoothed surface vertex function
+        Parameters
+        ----------
+        vfunc : no.ndarray
+            Float vector of values at vertices, if empty, use vertex coordinates
+        n : int, default=1
+            Number of iterations for smoothing
+
+        Returns
+        -------
+        vfunc : Function
+            Smoothed surface vertex function
         """
+
         if vfunc is None:
             vfunc = self.v
         vfunc = np.array(vfunc)
         if self.v.shape[0] != vfunc.shape[0]:
             raise ValueError("Error: length of vfunc needs to match number of vertices")
         areas = self.vertex_areas()[:, np.newaxis]
         adj = self.adj_sym.copy()
@@ -878,13 +1194,17 @@
         for i in range(n - 1):
             vout = adj2.dot(vout)
         return vout
 
     def smooth_(self, n=1):
         """
         Smoothes mesh in place for a number of iterations
-        :param n:   smoothing iterations
-        :return:    none, smoothes mesh in place
+
+        Parameters
+        ----------
+        n : int, default=1
+            smoothing iterations
         """
+
         vfunc = self.smooth_vfunc(self.v, n)
         self.v = vfunc
         return
```

### Comparing `lapy-0.4.1/lapy/read_geometry.py` & `lapy-0.6.0/lapy/read_geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # IMPORTS
 import warnings
 from collections import OrderedDict
 
 import numpy as np
 
 """
-Read FreeSurfer geometry (fix for dev, ll 126-128); 
+Read FreeSurfer geometry (fix for dev, ll 126-128);
 
-Code was taken from nibabel.freesurfer package (https://github.com/nipy/nibabel/blob/master/nibabel/freesurfer/io.py).
+Code was taken from nibabel.freesurfer package
+(https://github.com/nipy/nibabel/blob/master/nibabel/freesurfer/io.py).
 This software is licensed under the following license:
 
 The MIT License
 
 Copyright (c) 2009-2019 Matthew Brett <matthew.brett@gmail.com>
 Copyright (c) 2010-2013 Stephan Gerhard <git@unidesign.ch>
 Copyright (c) 2006-2014 Michael Hanke <michael.hanke@gmail.com>
@@ -47,20 +48,33 @@
     fobj : file
         File descriptor
     Returns
     -------
     n : int
         A 3 byte int
     """
+
     b1, b2, b3 = np.fromfile(fobj, ">u1", 3)
     return (b1 << 16) + (b2 << 8) + b3
 
 
 def _read_volume_info(fobj):
-    """Helper for reading the footer from a surface file."""
+    """Helper for reading the footer from a surface file.
+
+    Parameters
+    ----------
+    fobj : file
+        File descriptor
+
+    Returns
+    -------
+    volume_info: np.ndarray
+        Key-value pairs found in the file.
+    """
+
     volume_info = OrderedDict()
     head = np.fromfile(fobj, ">i4", 1)
     if not np.array_equal(head, [20]):  # Read two bytes more
         head = np.concatenate([head, np.fromfile(fobj, ">i4", 2)])
         if not np.array_equal(head, [2, 0, 20]) and not np.array_equal(
             head, [2, 1, 20]
         ):
@@ -90,14 +104,15 @@
             volume_info[key] = np.array(pair[1].split()).astype(float)
     # Ignore the rest
     return volume_info
 
 
 def read_geometry(filepath, read_metadata=False, read_stamp=False):
     """Read a triangular format Freesurfer surface mesh.
+
     Parameters
     ----------
     filepath : str
         Path to surface file.
     read_metadata : bool, optional
         If True, read and return metadata as key-value pairs.
         Valid keys:
@@ -108,27 +123,29 @@
         * 'voxelsize' : array of float, shape (3,)
         * 'xras' : array of float, shape (3,)
         * 'yras' : array of float, shape (3,)
         * 'zras' : array of float, shape (3,)
         * 'cras' : array of float, shape (3,)
     read_stamp : bool, optional
         Return the comment from the file
+
     Returns
     -------
     coords : numpy array
         nvtx x 3 array of vertex (x, y, z) coordinates.
     faces : numpy array
         nfaces x 3 array of defining mesh triangles.
     volume_info : OrderedDict
         Returned only if `read_metadata` is True.  Key-value pairs found in the
         geometry file.
     create_stamp : str
         Returned only if `read_stamp` is True.  The comment added by the
         program that saved the file.
     """
+
     volume_info = OrderedDict()
 
     TRIANGLE_MAGIC = 16777214
 
     with open(filepath, "rb") as fobj:
         magic = _fread3(fobj)
```

### Comparing `lapy-0.4.1/lapy/utils/_config.py` & `lapy-0.6.0/lapy/utils/_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 
 def sys_info(fid: Optional[IO] = None, developer: bool = False):
     """Print the system information for debugging.
 
     Parameters
     ----------
-    fid : file-like | None
+    fid : file-like, default=None
         The file to write to, passed to :func:`print`.
         Can be None to use :data:`sys.stdout`.
-    developer : bool
+    developer : bool, default=False
         If True, display information about optional dependencies.
     """
+
     ljust = 26
     out = partial(print, end="", file=fid)
     package = __package__.split(".")[0]
 
     # OS information - requires python 3.8 or above
     out("Platform:".ljust(ljust) + platform.platform() + "\n")
     # Python information
@@ -63,15 +64,27 @@
             if len(dependencies) == 0:
                 continue
             out(f"\nOptional '{key}' info\n")
             _list_dependencies_info(out, ljust, dependencies)
 
 
 def _list_dependencies_info(out: Callable, ljust: int, dependencies: List[str]):
-    """List dependencies names and versions."""
+    """List dependencies names and versions.
+
+    Parameters
+    ----------
+    out : Callable
+        output function
+    ljust : int
+         length of returned string
+    dependencies : List[str]
+        list of dependencies
+
+    """
+
     for dep in dependencies:
         # handle dependencies with version specifiers
         specifiers_pattern = r"(~=|==|!=|<=|>=|<|>|===)"
         specifiers = re.findall(specifiers_pattern, dep)
         if len(specifiers) != 0:
             dep, _ = dep.split(specifiers[0])
             while not dep[-1].isalpha():
```

### Comparing `lapy-0.4.1/lapy/utils/_imports.py` & `lapy-0.6.0/lapy/utils/_imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,28 +22,34 @@
     By default, if a dependency is missing an ImportError with a nice message
     will be raised.
 
     Parameters
     ----------
     name : str
         The module name.
-    extra : str
+    extra : str, default=""
         Additional text to include in the ImportError message.
-    raise_error : bool
+    raise_error : bool, default=True
         What to do when a dependency is not found.
         * True : Raise an ImportError.
         * False: Return None.
 
     Returns
     -------
     module : Optional[ModuleType]
         The imported module when found.
         None is returned when the package is not found and raise_error is
         False.
+
+    Raises
+    -------
+    ImportError
+        dependency not found; see raise_error
     """
+
     package_name = INSTALL_MAPPING.get(name)
     install_name = package_name if package_name is not None else name
 
     try:
         module = importlib.import_module(name)
     except ImportError:
         if raise_error:
```

### Comparing `lapy-0.4.1/lapy.egg-info/PKG-INFO` & `lapy-0.6.0/lapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapy
-Version: 0.4.1
+Version: 0.6.0
 Summary: A package for differential geometry on meshes (Laplace, FEM)
 Author-email: Martin Reuter <martin.reuter@dzne.de>
 Maintainer-email: Martin Reuter <martin.reuter@dzne.de>
 License: MIT License
         
         Copyright (c) 2020 Deep Medical Imaging Lab (PI Reuter)
         
@@ -71,19 +71,14 @@
 - Solver: a class for linear FEM computation (Laplace stiffness and mass
   matrix, fast and sparse eigenvalue solver, anisotropic Laplace, Poisson)
 - DiffGeo: compute gradients, divergence, mean curvature flow, etc.
 - Heat: for heat kernel and diffusion
 - ShapeDNA: compute the ShapeDNA descriptor of surfaces and solids
 - Plot: functions for interactive visualization (wrapping plotly)
 
-## ToDo:
-
-- Add unit tests and automated testing (e.g. travis)
-- Add command line scripts for various functions
-
 ## Usage:
 
 The LaPy package is a comprehensive collection of scripts, so we refer to the
 'help' function and docstring of each module / function / class for usage info.
 For example:
 
 ```
@@ -103,29 +98,33 @@
 `python3 -m pip install lapy`
 
 Use the following code to install the dev package in editable mode to a location of
 your choice:
 
 `python3 -m pip install --user --src /my/preferred/location --editable git+https://github.com/Deep-MI/Lapy.git#egg=lapy`
 
-Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package and will fall back to LU if the import fails. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
+Several functions, e.g. the Solver, require a sparse matrix decomposition, for which either the LU decomposition (from scipy sparse) or the faster Cholesky decomposition (from scikit-sparse cholmod) can be used. The default is to use the LU decomposition. If the parameter flag use_cholmod is True, the code will try to import cholmod from the scikit-sparse package. If this fails, an error will be thrown. If you would like to use cholmod, you need to install scikit-sparse separately. It cannot be listed among LaPy's dependencies as that causes errors with pip. scikit-sparse requires numpy and scipy to be installed separately beforehand.
 
 ## References:
 
 If you use this software for a publication please cite both these papers:
 
-[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
+[1] Laplace-Beltrami spectra as 'Shape-DNA' of surfaces and solids. Reuter M, Wolter F-E, Peinecke N. Computer-Aided Design. 2006;38(4):342-366. http://dx.doi.org/10.1016/j.cad.2005.10.011
 
-[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
+[2] BrainPrint: a discriminative characterization of brain morphology. Wachinger C, Golland P, Kremen W, Fischl B, Reuter M. Neuroimage. 2015;109:232-48. http://dx.doi.org/10.1016/j.neuroimage.2015.01.032 http://www.ncbi.nlm.nih.gov/pubmed/25613439
 
 [1] introduces the FEM methods and the Laplace spectra for shape analysis, while [2] focusses on medical applications.
 
 For Geodesics please cite:
 
 [3] Crane K, Weischedel C, Wardetzky M. Geodesics in heat: A new approach to computing distance based on heat flow. ACM Transactions on Graphics. https://doi.org/10.1145/2516971.2516977
 
 For non-singular mean curvature flow please cite:
 
 [4] Kazhdan M, Solomon J, Ben-Chen M. 2012. Can Mean-Curvature Flow be Modified to be Non-singular? Comput. Graph. Forum 31, 5, 1745–1754.
 https://doi.org/10.1111/j.1467-8659.2012.03179.x
 
+For conformal mapping please cite:
+
+[5] Choi PT, Lam KC, Lui LM. FLASH: Fast Landmark Aligned Spherical Harmonic Parameterization for Genus-0 Closed Brain Surfaces. SIAM Journal on Imaging Sciences, vol. 8, no. 1, pp. 67-94, 2015. https://doi.org/10.1137/130950008
+
 We also invite you to check out our lab webpage at https://deep-mi.org
```

### Comparing `lapy-0.4.1/lapy.egg-info/SOURCES.txt` & `lapy-0.6.0/lapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lapy-0.4.1/pyproject.toml` & `lapy-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 61.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'lapy'
-version = '0.4.1'
+version = '0.6.0'
 description = 'A package for differential geometry on meshes (Laplace, FEM)'
 readme = 'README.md'
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
 authors = [
     {name = 'Martin Reuter', email = 'martin.reuter@dzne.de'},
 ]
```

