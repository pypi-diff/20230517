# Comparing `tmp/aafitrans-0.1.1.tar.gz` & `tmp/aafitrans-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aafitrans-0.1.1.tar", last modified: Tue Apr 25 19:35:29 2023, max compression
+gzip compressed data, was "aafitrans-0.1.2.tar", last modified: Wed May 17 11:10:49 2023, max compression
```

## Comparing `aafitrans-0.1.1.tar` & `aafitrans-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.725807 aafitrans-0.1.1/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1103 2023-04-02 07:47:45.000000 aafitrans-0.1.1/LICENSE.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-04-25 19:35:29.724807 aafitrans-0.1.1/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     4581 2023-04-25 05:53:18.000000 aafitrans-0.1.1/README.md
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      741 2023-04-03 06:04:32.000000 aafitrans-0.1.1/pyproject.toml
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-25 19:35:29.725807 aafitrans-0.1.1/setup.cfg
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.721807 aafitrans-0.1.1/src/
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.722807 aafitrans-0.1.1/src/aafitrans/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       65 2023-04-25 19:16:05.000000 aafitrans-0.1.1/src/aafitrans/__init__.py
--rwxrwx---   0 prajwel   (1000) prajwel   (1000)    15597 2023-04-25 19:32:41.000000 aafitrans-0.1.1/src/aafitrans/aafitrans.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.724807 aafitrans-0.1.1/src/aafitrans.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      273 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       25 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       10 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/top_level.txt
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-17 11:10:49.832341 aafitrans-0.1.2/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1103 2023-04-02 07:47:45.000000 aafitrans-0.1.2/LICENSE.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-05-17 11:10:49.831341 aafitrans-0.1.2/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     4581 2023-04-25 05:53:18.000000 aafitrans-0.1.2/README.md
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      813 2023-04-27 08:59:38.000000 aafitrans-0.1.2/pyproject.toml
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-05-17 11:10:49.832341 aafitrans-0.1.2/setup.cfg
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-17 11:10:49.823341 aafitrans-0.1.2/src/
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-17 11:10:49.829341 aafitrans-0.1.2/src/aafitrans/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       65 2023-04-25 19:16:05.000000 aafitrans-0.1.2/src/aafitrans/__init__.py
+-rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    15346 2023-05-17 10:31:45.000000 aafitrans-0.1.2/src/aafitrans/aafitrans.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-17 11:10:49.831341 aafitrans-0.1.2/src/aafitrans.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-05-17 11:10:49.000000 aafitrans-0.1.2/src/aafitrans.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      292 2023-05-17 11:10:49.000000 aafitrans-0.1.2/src/aafitrans.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-05-17 11:10:49.000000 aafitrans-0.1.2/src/aafitrans.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       25 2023-05-17 11:10:49.000000 aafitrans-0.1.2/src/aafitrans.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       10 2023-05-17 11:10:49.000000 aafitrans-0.1.2/src/aafitrans.egg-info/top_level.txt
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-17 11:10:49.831341 aafitrans-0.1.2/tests/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     2286 2023-05-17 11:08:29.000000 aafitrans-0.1.2/tests/test_aafi.py
```

### Comparing `aafitrans-0.1.1/LICENSE.txt` & `aafitrans-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aafitrans-0.1.1/PKG-INFO` & `aafitrans-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aafitrans
-Version: 0.1.1
+Version: 0.1.2
 Summary: match coordinate lists
 Author-email: Prajwel Joseph <prajwel.pj@gmail.com>
 Project-URL: Homepage, https://github.com/prajwel/aafitrans
 Project-URL: Bug Tracker, https://github.com/prajwel/aafitrans/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aafitrans-0.1.1/README.md` & `aafitrans-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aafitrans-0.1.1/pyproject.toml` & `aafitrans-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -22,7 +22,12 @@
 
 [project.urls]
 "Homepage" = "https://github.com/prajwel/aafitrans"
 "Bug Tracker" = "https://github.com/prajwel/aafitrans/issues"
 
 [tool.setuptools.dynamic]
 version = {attr = "aafitrans.aafitrans.__version__"}
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
```

### Comparing `aafitrans-0.1.1/src/aafitrans/aafitrans.py` & `aafitrans-0.1.2/src/aafitrans/aafitrans.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 MIT License
 
 Copyright (c) 2016-2019 Martin Beroiz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -18,35 +18,39 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 Modified by Prajwel Joseph
-'''
+"""
 
-'''
+"""
 The following paper should be cited if you use the script in a scientific
 publication
 
 Astroalign: A Python module for astronomical image registration.
 Beroiz, M., Cabral, J. B., & Sanchez, B.
 Astronomy & Computing, Volume 32, July 2020, 100384.
-'''
-
+"""
 
 import numpy as np
 from scipy.spatial import KDTree
 from itertools import combinations
 from functools import partial
 from collections import Counter
 from skimage import transform
 
+__version__ = "0.1.2"
+
+
+def get_unique_array(array):
+    _, idx = np.unique(array, return_index=True, axis=0)
+    return array[np.sort(idx)]
 
-__version__ = '0.1.1'
 
 class _MatchTransform:
     def __init__(self, source, target, ttype):
         self.source = source
         self.target = target
         self.ttype = ttype
 
@@ -65,38 +69,36 @@
             self.ttype, self.source[s], self.target[d]
         )
         return approx_t
 
     def get_error(self, data, approx_t):
         d1, d2, d3 = data.shape
         s, d = data.reshape(d1 * d2, d3).T
-        resid = approx_t.residuals(self.source[s], self.target[d]).reshape(
-            d1, d2
-        )
+        resid = approx_t.residuals(self.source[s], self.target[d]).reshape(d1, d2)
         error = resid.max(axis=1)
         return error
-    
+
     def get_total_error(self, data, approx_t):
         d1, d2, d3 = data.shape
         s, d = data.reshape(d1 * d2, d3).T
         resid = approx_t.residuals(self.source[s], self.target[d])
-        total_error = np.sqrt(np.sum(np.square(resid)) / (len(resid) * 3))    
-        return total_error       
-    
-    
+        total_error = np.sqrt(np.sum(np.square(resid)) / (len(resid) * 3))
+        return total_error
+
+
 def _invariantfeatures(x1, x2, x3):
     """Given 3 points x1, x2, x3, return the invariant features for the set."""
     sides = np.sort(
         [
             np.linalg.norm(x1 - x2),
             np.linalg.norm(x2 - x3),
             np.linalg.norm(x1 - x3),
         ]
     )
-    return [sides[2] / sides[1], sides[1] / sides[0]]    
+    return [sides[2] / sides[1], sides[1] / sides[0]]
 
 
 def _arrangetriplet(sources, vertex_indices):
     """Order vertex_indices according to length side.
 
     Order in (a, b, c) form Where:
       a is the vertex defined by L1 & L2
@@ -128,15 +130,14 @@
 def _generate_invariants(sources, num_nearest_neighbors):
     """Return an array of (unique) invariants derived from the array `sources`.
 
     Return an array of the indices of `sources` that correspond to each
     invariant, arranged as described in _arrangetriplet.
     """
 
-
     arrange = partial(_arrangetriplet, sources=sources)
 
     inv = []
     triang_vrtx = []
     coordtree = KDTree(sources)
     # The number of nearest neighbors to request (to work with few sources)
     knn = min(len(sources), num_nearest_neighbors)
@@ -147,40 +148,38 @@
         # them with the order (a, b, c) defined in _arrangetriplet
         all_asterism_triang = [
             arrange(vertex_indices=list(cmb)) for cmb in combinations(indx, 3)
         ]
         triang_vrtx.extend(all_asterism_triang)
 
         inv.extend(
-            [
-                _invariantfeatures(*sources[triplet])
-                for triplet in all_asterism_triang
-            ]
+            [_invariantfeatures(*sources[triplet]) for triplet in all_asterism_triang]
         )
 
     # Remove here all possible duplicate triangles
-    uniq_ind = [
-        pos for (pos, elem) in enumerate(inv) if elem not in inv[pos + 1 :]
-    ]
+    uniq_ind = [pos for (pos, elem) in enumerate(inv) if elem not in inv[pos + 1 :]]
     inv_uniq = np.array(inv)[uniq_ind]
     triang_vrtx_uniq = np.array(triang_vrtx)[uniq_ind]
 
     return inv_uniq, triang_vrtx_uniq
 
 
-def find_transform(source, target, 
-                   max_control_points=50, 
-                   ttype='similarity', 
-                   pixel_tolerance=2, 
-                   min_matches=4, 
-                   num_nearest_neighbors=8,
-                   kdtree_search_radius = 0.02,
-                   n_samples = 1,
-                   get_best_fit = True,
-                   seed = None):
+def find_transform(
+    source,
+    target,
+    max_control_points=50,
+    ttype="similarity",
+    pixel_tolerance=2,
+    min_matches=4,
+    num_nearest_neighbors=8,
+    kdtree_search_radius=0.02,
+    n_samples=1,
+    get_best_fit=True,
+    seed=None,
+):
     """Estimate the transform between ``source`` and ``target``.
 
     Return a GeometricTransform object ``T`` that maps pixel x, y indices from
     the source image s = (x, y) into the target (destination) image t = (x, y).
     T contains parameters of the tranformation.
 
     Parameters
@@ -190,31 +189,31 @@
         target
             An iterable of (x, y) coordinates of the target control points.
         max_control_points
             The maximum number of control point-sources to find the transformation.
         ttype
             The type of Transform to be estimated.
         pixel_tolerance
-            The maximum residual error for the estimated tranform.            
+            The maximum residual error for the estimated tranform.
         min_matches
             The minimum number of matches to be found.
         num_nearest_neighbors
-            The number of nearest neighbors of a given star (including itself) 
-            to construct the triangle invariants.                      
+            The number of nearest neighbors of a given star (including itself)
+            to construct the triangle invariants.
         kdtree_search_radius
             The default is 0.02. This radius is used to find nearest neighbours
-            while conducting a KD tree search of invariant features. 
+            while conducting a KD tree search of invariant features.
         n_samples
             The minimum number of data points to fit the model to. A value of 1
-            refers to 1 triangle, corresponding to 3 pairs of coordinates. 
+            refers to 1 triangle, corresponding to 3 pairs of coordinates.
         get_best_fit
-            Whether to minimise the total error.                          
+            Whether to minimise the total error.
         seed
-            Seed value for Numpy Random Generator.       
-            
+            Seed value for Numpy Random Generator.
+
     Returns
     -------
         T, (source_pos_array, target_pos_array)
             The transformation object and a tuple of corresponding star positions
             in source and target.
 
     Raises
@@ -222,37 +221,45 @@
         TypeError
             If input type of ``source`` or ``target`` is not supported.
         ValueError
             If it cannot find more than 3 stars on any input.
         MaxIterError
             If no transformation is found.
     """
-    
+
+    try:
+        source = get_unique_array(source)
+        target = get_unique_array(target)
+    except Exception:
+        raise TypeError("Input type for source not supported.")
+
     try:
         source_controlp = np.array(source)[:max_control_points]
         target_controlp = np.array(target)[:max_control_points]
     except Exception:
         raise TypeError("Input type for source not supported.")
 
     # Check for low number of reference points
     if len(source_controlp) < 3:
         raise ValueError(
-            "Reference stars in source image are less than the "
-            "minimum value (3)."
+            "Reference stars in source image are less than the " "minimum value (3)."
         )
     if len(target_controlp) < 3:
         raise ValueError(
-            "Reference stars in target image are less than the "
-            "minimum value (3)."
+            "Reference stars in target image are less than the " "minimum value (3)."
         )
 
-    source_invariants, source_asterisms = _generate_invariants(source_controlp, num_nearest_neighbors)
+    source_invariants, source_asterisms = _generate_invariants(
+        source_controlp, num_nearest_neighbors
+    )
     source_invariant_tree = KDTree(source_invariants)
 
-    target_invariants, target_asterisms = _generate_invariants(target_controlp, num_nearest_neighbors)
+    target_invariants, target_asterisms = _generate_invariants(
+        target_controlp, num_nearest_neighbors
+    )
     target_invariant_tree = KDTree(target_invariants)
 
     # r = 0.1 is the maximum search distance, 0.1 is an empirical value that
     # returns about the same number of matches than inputs
     # matches_list is a list of lists such that for each element
     # source_invariant_tree.data[i], matches_list[i] is a list of the indices
     # of its neighbors in target_invariant_tree.data
@@ -272,38 +279,37 @@
             matches.append(list(zip(t1, t2)))
     matches = np.array(matches)
 
     inv_model = _MatchTransform(source_controlp, target_controlp, ttype)
     # Set the minimum matches to be between 1 and 10 asterisms
     # min_matches = max(1, min(10, int(min_matches)))
 
-    if (len(source_controlp) == 3 or len(target_controlp) == 3) and len(
-        matches
-    ) == 1:
+    if (len(source_controlp) == 3 or len(target_controlp) == 3) and len(matches) == 1:
         best_t = inv_model.fit(matches)
         inlier_ind = np.arange(len(matches))  # All of the indices
     else:
-        best_t, inlier_ind = _ransac(matches, 
-                                     inv_model, 
-                                     pixel_tolerance, 
-                                     min_matches, 
-                                     n_samples, 
-                                     get_best_fit,
-                                     seed)
-        
+        best_t, inlier_ind = _ransac(
+            matches,
+            inv_model,
+            pixel_tolerance,
+            min_matches,
+            n_samples,
+            get_best_fit,
+            seed,
+        )
+
     triangle_inliers = matches[inlier_ind]
     d1, d2, d3 = triangle_inliers.shape
     inl_arr = triangle_inliers.reshape(d1 * d2, d3)
     inl_arr_unique = np.unique(inl_arr, axis=0)
     s, t = inl_arr_unique.T
 
     return best_t, (source_controlp[s], target_controlp[t])
 
 
-
 # Copyright (c) 2004-2007, Andrew D. Straw. All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
 
 #     * Redistributions of source code must retain the above copyright
@@ -333,18 +339,21 @@
 #
 # Modified by Martin Beroiz
 # Modified by Prajwel Joseph
 
 
 class MaxIterError(RuntimeError):
     """Raise if maximum iterations reached."""
+
     pass
 
 
-def _ransac(data, model, thresh, min_matches, n_samples = 1, get_best_fit = True, seed = None):
+def _ransac(
+    data, model, thresh, min_matches, n_samples=1, get_best_fit=True, seed=None
+):
     """Fit model parameters to data using the RANSAC algorithm.
 
     Parameters
     ----------
         data
             A set of data points
         model
@@ -353,49 +362,48 @@
             A threshold value to determine when a data point fits a model
         min_matches
             The min number of matches required to assert that a model
             fits well to data
         n_samples
             The minimum number of data points to fit the model to.
         get_best_fit
-            Whether to minimise the total error.            
+            Whether to minimise the total error.
         seed
-            Seed value for Numpy Random Generator.     
+            Seed value for Numpy Random Generator.
     Returns
     -------
         bestfit: model parameters which best fit the data (or nil if no good
                   model is found)
     """
     good_fit = None
     n_data = data.shape[0]
     all_idxs = np.arange(n_data)
     rng = np.random.default_rng(seed)
     rng.shuffle(all_idxs)
     best_error = np.inf
     improve_error_counter = 0
-    
+
     for iter_i in range(n_data):
         # Partition indices into two random subsets
         maybe_idxs = all_idxs[iter_i : iter_i + n_samples]
-        test_idxs = np.concatenate([all_idxs[:iter_i], 
-                                    all_idxs[iter_i + n_samples:]])        
+        test_idxs = np.concatenate([all_idxs[:iter_i], all_idxs[iter_i + n_samples :]])
         maybeinliers = data[maybe_idxs, :]
         test_points = data[test_idxs, :]
         maybemodel = model.fit(maybeinliers)
         test_err = model.get_error(test_points, maybemodel)
         # select indices of rows with accepted points
         also_idxs = test_idxs[test_err < thresh]
         alsoinliers = data[also_idxs, :]
         if len(alsoinliers) >= min_matches:
             good_data = np.concatenate((maybeinliers, alsoinliers))
             good_fit = model.fit(good_data)
             total_error = model.get_total_error(good_data, good_fit)
             if get_best_fit and total_error < best_error:
                 best_error = total_error
-                best_fit = good_fit 
+                best_fit = good_fit
                 improve_error_counter += 1
                 if improve_error_counter == 100:
                     break
             else:
                 best_fit = good_fit
 
     if good_fit is None:
```

### Comparing `aafitrans-0.1.1/src/aafitrans.egg-info/PKG-INFO` & `aafitrans-0.1.2/src/aafitrans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aafitrans
-Version: 0.1.1
+Version: 0.1.2
 Summary: match coordinate lists
 Author-email: Prajwel Joseph <prajwel.pj@gmail.com>
 Project-URL: Homepage, https://github.com/prajwel/aafitrans
 Project-URL: Bug Tracker, https://github.com/prajwel/aafitrans/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

