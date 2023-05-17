# Comparing `tmp/read_rapidpe-0.5.0.tar.gz` & `tmp/read_rapidpe-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_rapidpe-0.5.0.tar", max compression
+gzip compressed data, was "read_rapidpe-0.5.1.tar", max compression
```

## Comparing `read_rapidpe-0.5.0.tar` & `read_rapidpe-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.5.0/README.md
--rw-r--r--   0        0        0      627 2023-05-16 05:05:36.967467 read_rapidpe-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      353 2023-04-16 13:12:20.078578 read_rapidpe-0.5.0/read_rapidpe/__init__.py
--rw-r--r--   0        0        0    11295 2023-05-13 16:31:51.989559 read_rapidpe-0.5.0/read_rapidpe/grid_point.py
--rw-r--r--   0        0        0     3445 2023-05-16 05:02:30.343719 read_rapidpe-0.5.0/read_rapidpe/io.py
--rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.5.0/read_rapidpe/p_astro.py
--rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.5.0/read_rapidpe/parser.py
--rw-r--r--   0        0        0     1474 2023-04-16 14:05:36.413685 read_rapidpe-0.5.0/read_rapidpe/plot.py
--rw-r--r--   0        0        0    24548 2023-05-16 04:46:04.027718 read_rapidpe-0.5.0/read_rapidpe/result.py
--rw-r--r--   0        0        0     2200 2022-11-25 08:05:18.514011 read_rapidpe-0.5.0/read_rapidpe/transform.py
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.5.1/README.md
+-rw-r--r--   0        0        0      627 2023-05-17 02:32:20.876202 read_rapidpe-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      303 2023-05-17 02:31:18.161235 read_rapidpe-0.5.1/read_rapidpe/__init__.py
+-rw-r--r--   0        0        0    11295 2023-05-13 16:31:51.989559 read_rapidpe-0.5.1/read_rapidpe/grid_point.py
+-rw-r--r--   0        0        0     3445 2023-05-16 05:02:30.343719 read_rapidpe-0.5.1/read_rapidpe/io.py
+-rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.5.1/read_rapidpe/p_astro.py
+-rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.5.1/read_rapidpe/parser.py
+-rw-r--r--   0        0        0     1802 2023-05-17 02:28:36.535926 read_rapidpe-0.5.1/read_rapidpe/plot.py
+-rw-r--r--   0        0        0    24661 2023-05-17 02:20:02.934691 read_rapidpe-0.5.1/read_rapidpe/result.py
+-rw-r--r--   0        0        0     4871 2023-05-17 02:06:29.545978 read_rapidpe-0.5.1/read_rapidpe/transform.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.5.1/PKG-INFO
```

### Comparing `read_rapidpe-0.5.0/README.md` & `read_rapidpe-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.0/pyproject.toml` & `read_rapidpe-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "read-rapidpe"
-version = "0.5.0"
+version = "0.5.1"
 description = "Read and analyse results generated by rapidpe-rift-pipe"
 authors = ["Cory Chu <cory@gwlab.page>"]
 readme = "README.md"
 packages = [{include = "read_rapidpe"}]
 homepage = "https://github.com/c0rychu/read-rapidpe"
 repository = "https://git.ligo.org/yu-kuang.chu/read-rapidpe"
```

### Comparing `read_rapidpe-0.5.0/read_rapidpe/grid_point.py` & `read_rapidpe-0.5.1/read_rapidpe/grid_point.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.0/read_rapidpe/io.py` & `read_rapidpe-0.5.1/read_rapidpe/io.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.0/read_rapidpe/p_astro.py` & `read_rapidpe-0.5.1/read_rapidpe/p_astro.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.0/read_rapidpe/parser.py` & `read_rapidpe-0.5.1/read_rapidpe/parser.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.0/read_rapidpe/plot.py` & `read_rapidpe-0.5.1/read_rapidpe/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,20 @@
         n)
     etalist = np.linspace(
         result.symmetric_mass_ratio.min()+0.00001,
         result.symmetric_mass_ratio.max()-0.00001,
         n)
     mc, eta = np.meshgrid(mclist, etalist)
     return mc, eta
+
+
+def meshgrid_mcq(result, n=100):
+    mclist = np.linspace(
+        result.chirp_mass.min()+0.00001,
+        result.chirp_mass.max()-0.00001,
+        n)
+    qlist = np.linspace(
+        result.mass_ratio.min()+0.00001,
+        result.mass_ratio.max()-0.00001,
+        n)
+    mc, q = np.meshgrid(mclist, qlist)
+    return mc, q
```

### Comparing `read_rapidpe-0.5.0/read_rapidpe/result.py` & `read_rapidpe-0.5.1/read_rapidpe/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .io import load_injection_info_txt
 from .io import dict_of_ndarray_to_recarray
 from .io import dict_from_hdf_group
 from .io import dict_to_hdf_group
 
 from .transform import transform_m1m2_to_mceta, transform_mceta_to_m1m2
 from .transform import jacobian_mceta_by_m1m2
+from .transform import Mass_Spin
 
 from matplotlib.tri import Triangulation
 from matplotlib.tri import LinearTriInterpolator, CubicTriInterpolator
 from scipy.interpolate import LinearNDInterpolator, NearestNDInterpolator
 from scipy.interpolate import CloughTocher2DInterpolator
 from scipy.stats import multinomial
 
@@ -330,19 +331,20 @@
                 result.iteration[i] = int(re_iter.search(filename).group(1))
             # t2 = time.time()
             # print("parallel reading time: ", t1-t0)
             # print("post-proccessing time: ", t2-t1)
 
         # Add chirp_mass and symmetric_mass_ratio
         if ("mass_1" in result._keys) and ("mass_2" in result._keys):
-            result.chirp_mass, result.symmetric_mass_ratio = \
-                transform_m1m2_to_mceta(result.mass_1, result.mass_2)
-            result._keys.extend(["chirp_mass", "symmetric_mass_ratio"])
-
-            # TODO: Addn mass_ratio q
+            x = Mass_Spin.from_m1m2(result.mass_1, result.mass_2)
+            result.chirp_mass = x.chirp_mass
+            result.symmetric_mass_ratio = x.symmetric_mass_ratio
+            result.mass_ratio = x.mass_ratio
+            result._keys.extend(
+                ["chirp_mass", "symmetric_mass_ratio", "mass_ratio"])
 
         return cls(result)
 
     def to_hdf(self, hdf_filename, compression=None):
         """
         Save result to hdf file
```

### Comparing `read_rapidpe-0.5.0/PKG-INFO` & `read_rapidpe-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read-rapidpe
-Version: 0.5.0
+Version: 0.5.1
 Summary: Read and analyse results generated by rapidpe-rift-pipe
 Home-page: https://github.com/c0rychu/read-rapidpe
 Author: Cory Chu
 Author-email: cory@gwlab.page
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```
