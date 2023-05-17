# Comparing `tmp/superscreen-0.9.0.tar.gz` & `tmp/superscreen-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superscreen-0.9.0.tar", last modified: Wed May 17 00:21:47 2023, max compression
+gzip compressed data, was "superscreen-0.9.1.tar", last modified: Wed May 17 19:27:44 2023, max compression
```

## Comparing `superscreen-0.9.0.tar` & `superscreen-0.9.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.462604 superscreen-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 00:21:36.000000 superscreen-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 00:21:47.462604 superscreen-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-17 00:21:36.000000 superscreen-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:21:47.466604 superscreen-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-17 00:21:36.000000 superscreen-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.454604 superscreen-0.9.0/superscreen/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.458603 superscreen-0.9.0/superscreen/device/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42839 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/edge_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/device/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/fem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/fluxoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46337 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.458603 superscreen-0.9.0/superscreen/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19003 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/solve.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/solve_film.py
--rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/solver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.458603 superscreen-0.9.0/superscreen/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/dipole.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/sources/vortex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.462604 superscreen-0.9.0/superscreen/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/test/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    39839 2023-05-17 00:21:36.000000 superscreen-0.9.0/superscreen/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:21:47.454604 superscreen-0.9.0/superscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 00:21:47.000000 superscreen-0.9.0/superscreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.590081 superscreen-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 19:27:34.000000 superscreen-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 19:27:44.586080 superscreen-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-17 19:27:34.000000 superscreen-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:27:44.590081 superscreen-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-17 19:27:34.000000 superscreen-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42839 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/edge_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/device/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/fem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/fluxoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46337 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19003 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/solve_film.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/solver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/dipole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/sources/vortex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/test/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39839 2023-05-17 19:27:34.000000 superscreen-0.9.1/superscreen/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:27:44.586080 superscreen-0.9.1/superscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 19:27:44.000000 superscreen-0.9.1/superscreen.egg-info/top_level.txt
```

### Comparing `superscreen-0.9.0/LICENSE` & `superscreen-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/PKG-INFO` & `superscreen-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.9.0
+Version: 0.9.1
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
```

### Comparing `superscreen-0.9.0/README.md` & `superscreen-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/setup.py` & `superscreen-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/__init__.py` & `superscreen-0.9.1/superscreen/__init__.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/about.py` & `superscreen-0.9.1/superscreen/about.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/device/device.py` & `superscreen-0.9.1/superscreen/device/device.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/device/edge_mesh.py` & `superscreen-0.9.1/superscreen/device/edge_mesh.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/device/layer.py` & `superscreen-0.9.1/superscreen/device/layer.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/device/mesh.py` & `superscreen-0.9.1/superscreen/device/mesh.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,52 +26,41 @@
             form a triangle. [[0, 1, 2], [0, 1, 3]] corresponds to a triangle
             connecting vertices 0, 1, and 2 and another triangle connecting vertices
             0, 1, and 3.
         boundary_indices: Indices corresponding to the boundary.
         vertex_areas: The areas corresponding to the sites or vertices.
         triangle_areas: The areas of the triangular mesh elements.
         edge_mesh: The edge mesh.
+        build_operators: Whether to build the :class:`superscreen.device.MeshOperators`
+            for the mesh.
     """
 
     def __init__(
         self,
         sites: Sequence[Tuple[float, float]],
         elements: Sequence[Tuple[int, int, int]],
         boundary_indices: Sequence[int],
-        vertex_areas: Optional[Sequence[float]] = None,
-        triangle_areas: Optional[Sequence[float]] = None,
-        edge_mesh: Optional[EdgeMesh] = None,
+        vertex_areas: Sequence[float],
+        triangle_areas: Sequence[float],
+        edge_mesh: EdgeMesh,
+        build_operators: bool = True,
     ):
         self.sites = np.asarray(sites).squeeze()
-        # Setting dtype to int64 is important when running on Windows.
-        # Using default dtype uint64 does not work as Scipy indices in some
-        # instances.
         self.elements = np.asarray(elements, dtype=np.int64)
         self.boundary_indices = np.asarray(boundary_indices, dtype=np.int64)
-        if vertex_areas is not None:
-            vertex_areas = np.asarray(vertex_areas)
-        self.vertex_areas = vertex_areas
-        if triangle_areas is not None:
-            triangle_areas = np.asarray(triangle_areas)
-        self.triangle_areas = triangle_areas
+        self.vertex_areas = np.asarray(vertex_areas)
+        self.triangle_areas = np.asarray(triangle_areas)
         self.edge_mesh = edge_mesh
-        if (
-            self.edge_mesh is None
-            or self.vertex_areas is None
-            or self.triangle_areas is None
-        ):
-            self.operators = None
-        else:
+        self.operators: Optional[MeshOperators] = None
+        if build_operators:
             self.operators = MeshOperators.from_mesh(self)
 
     def stats(self) -> Dict[str, Union[int, float]]:
         """Returns a dictionary of information about the mesh."""
-        edge_lengths = None
-        if self.edge_mesh is not None:
-            edge_lengths = self.edge_mesh.edge_lengths
+        edge_lengths = self.edge_mesh.edge_lengths
         vertex_areas = self.vertex_areas
 
         def _min(arr):
             if arr is not None:
                 return arr.min()
 
         def _max(arr):
@@ -115,14 +104,16 @@
 
         Args:
             sites: The (x, y) coordinates of the mesh sites.
             elements: A list of triplets that correspond to the indices of the vertices
                 that form a triangle.   E.g. [[0, 1, 2], [0, 1, 3]] corresponds to a
                 triangle connecting vertices 0, 1, and 2 and another triangle
                 connecting vertices 0, 1, and 3.
+            build_operators: Whether to build the :class:`superscreen.device.MeshOperators`
+                for the mesh.
 
         Returns:
             A new :class:`tdgl.finite_volume.Mesh` instance
         """
         sites = np.asarray(sites).squeeze()
         elements = np.asarray(elements).squeeze()
         if sites.ndim != 2 or sites.shape[1] != 2:
@@ -130,26 +121,25 @@
                 f"The site coordinates must have shape (n, 2), got {sites.shape!r}"
             )
         if elements.ndim != 2 or elements.shape[1] != 3:
             raise ValueError(
                 f"The elements must have shape (m, 3), got {elements.shape!r}."
             )
         boundary_indices = Mesh.find_boundary_indices(elements)
-        edge_mesh = triangle_areas = vertex_areas = None
-        if build_operators:
-            edge_mesh = EdgeMesh.from_mesh(sites, elements)
-            triangle_areas = utils.triangle_areas(sites, elements)
-            vertex_areas = utils.vertex_areas(sites, elements, tri_areas=triangle_areas)
+        edge_mesh = EdgeMesh.from_mesh(sites, elements)
+        triangle_areas = utils.triangle_areas(sites, elements)
+        vertex_areas = utils.vertex_areas(sites, elements, tri_areas=triangle_areas)
         return Mesh(
             sites=sites,
             elements=elements,
             boundary_indices=boundary_indices,
             edge_mesh=edge_mesh,
             vertex_areas=vertex_areas,
             triangle_areas=triangle_areas,
+            build_operators=build_operators,
         )
 
     @staticmethod
     def find_boundary_indices(elements: np.ndarray) -> np.ndarray:
         """Find the boundary vertices.
 
         Args:
@@ -159,20 +149,22 @@
             An array of site indices corresponding to the boundary.
         """
         edges, is_boundary = utils.get_edges(elements)
         # Get the boundary edges and all boundary points
         boundary_edges = edges[is_boundary]
         return np.unique(boundary_edges.ravel())
 
-    def smooth(self, iterations: int) -> "Mesh":
+    def smooth(self, iterations: int, build_operators: bool = True) -> "Mesh":
         """Perform Laplacian smoothing of the mesh, i.e., moving each interior vertex
         to the arithmetic average of its neighboring points.
 
         Args:
             iterations: The number of smoothing iterations to perform.
+            build_operators: Whether to build the :class:`superscreen.device.MeshOperators`
+                for the mesh.
 
         Returns:
             A new Mesh with relaxed vertex positions.
         """
         mesh = self
         elements = mesh.elements
         edges, _ = utils.get_edges(elements)
@@ -192,15 +184,17 @@
             new_sites += np.array(
                 [np.bincount(edges[:, 1], val, minlength=n) for val in vals]
             ).T
             new_sites /= num_neighbors[:, np.newaxis]
             # reset boundary points
             new_sites[boundary] = sites[boundary]
             mesh = Mesh.from_triangulation(
-                new_sites, elements, build_operators=(i == (iterations - 1))
+                new_sites,
+                elements,
+                build_operators=(build_operators and (i == (iterations - 1))),
             )
         return mesh
 
     def plot(
         self,
         ax: Union[plt.Axes, None] = None,
         show_sites: bool = False,
@@ -311,31 +305,50 @@
         )
         if self.operators is not None:
             mesh.operators = self.operators.copy()
         return mesh
 
 
 class MeshOperators:
+    """A container for the finite element operators for a :class:`superscreen.Mesh`.
+
+    Args:
+        weights: The mesh weights or effective vertex areas, shape ``(n, )``
+        Q: The kernel matrix ``Q``, shape ``(n, n)``
+        gradient_x: The x-gradient matrix, shape ``(n, n)``
+        gradient_y: The y-gradient matrix, shape ``(n, n)``
+        laplacian: The mesh Laplacian, shape ``(n, n)``
+    """
+
     def __init__(
         self,
         *,
         weights: np.ndarray,
         Q: np.ndarray,
-        gradient_x: Union[np.ndarray, sp.spmatrix],
-        gradient_y: Union[np.ndarray, sp.spmatrix],
-        laplacian: Union[np.ndarray, sp.spmatrix],
+        gradient_x: sp.spmatrix,
+        gradient_y: sp.spmatrix,
+        laplacian: sp.spmatrix,
     ):
         self.weights = weights
         self.Q = Q
         self.gradient_x = gradient_x
         self.gradient_y = gradient_y
         self.laplacian = laplacian
 
     @staticmethod
     def from_mesh(mesh: Mesh) -> "MeshOperators":
+        """Construct a :class:`superscreen.device.MeshOperators` instance
+        from a :class:`superscreen.Mesh`.
+
+        Args:
+            mesh: The :class:`superscreen.Mesh`
+
+        Returns:
+            A new :class:`superscreen.device.MeshOperators` instance
+        """
         sites = mesh.sites
         elements = mesh.elements
         weights = mesh.vertex_areas
         Q = MeshOperators.Q_matrix(sites, weights)
         gradient_x, gradient_y = gradient_vertices(
             sites, elements, areas=mesh.triangle_areas
         )
@@ -348,14 +361,15 @@
             Q=Q,
             gradient_x=gradient_x,
             gradient_y=gradient_y,
             laplacian=laplacian,
         )
 
     def copy(self) -> "MeshOperators":
+        """Returns a deep copy."""
         return deepcopy(self)
 
     @staticmethod
     def C_vector(points: np.ndarray) -> np.ndarray:
         """Computes the edge vector, C:
 
         .. math::
```

### Comparing `superscreen-0.9.0/superscreen/device/polygon.py` & `superscreen-0.9.1/superscreen/device/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,36 +192,41 @@
 
     def make_mesh(
         self,
         min_points: Optional[int] = None,
         max_edge_length: Optional[float] = None,
         convex_hull: bool = False,
         smooth: int = 0,
+        build_operators: bool = False,
         **meshpy_kwargs,
     ) -> Mesh:
         """Creates a :class:`Mesh` for the polygon.
 
         Args:
             min_points: Minimum number of vertices in the mesh. If None, then
                 the number of vertices will be determined by meshpy_kwargs and the
                 number of vertices in the underlying polygons.
             max_edge_length: The maximum distance between vertices in the resulting mesh.
             convex_hull: If True, then the entire convex hull of the polygon (minus holes)
                 will be meshed. Otherwise, only the polygon interior is meshed.
             smooth: Number of Laplacian smoothing steps to perform.
+            build_operators: Whether to build the :class:`superscreen.device.MeshOperators`
+                for the mesh.
             **meshpy_kwargs: Passed to meshpy.triangle.build().
         """
         points, triangles = generate_mesh(
             self.points,
             min_points=min_points,
             max_edge_length=max_edge_length,
             convex_hull=convex_hull,
             **meshpy_kwargs,
         )
-        return Mesh.from_triangulation(points, triangles).smooth(smooth)
+        return Mesh.from_triangulation(
+            points, triangles, build_operators=build_operators
+        ).smooth(smooth, build_operators=build_operators)
 
     def rotate(
         self,
         degrees: float,
         origin: Union[str, Tuple[float, float]] = (0.0, 0.0),
         inplace: bool = False,
     ) -> "Polygon":
```

### Comparing `superscreen-0.9.0/superscreen/device/utils.py` & `superscreen-0.9.1/superscreen/device/utils.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/distance.py` & `superscreen-0.9.1/superscreen/distance.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/fem.py` & `superscreen-0.9.1/superscreen/fem.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,29 +236,27 @@
 def laplace_operator(
     points: np.ndarray,
     triangles: np.ndarray,
     masses: Optional[np.ndarray] = None,
     weight_method: Literal[
         "uniform", "half_cotangent", "inv_euclidean"
     ] = "half_cotangent",
-    sparse: bool = True,
-) -> Union[np.ndarray, sp.csr_array]:
+) -> sp.csr_array:
     """Laplacian operator for the mesh (sometimes called
     Laplace-Beltrami operator).
 
     The Laplacian operator is defined as ``inv(M) @ L``,
     where M is the mass matrix and L is the Laplacian matrix.
 
     Args:
         points: Shape (n, 2) array of x, y coordinates of vertices.
         triangles: Shape (m, 3) array of triangle indices.
         masses: Pre-computed mass matrix, i.e., the vertex areas.
         weight_method: Method for calculating the weights. One of: "uniform",
             "inv_euclidean", or "half_cotangent".
-        sparse: Whether to return a sparse matrix or numpy ndarray.
 
     Returns:
         Shape (n, n) Laplacian operator
     """
     # See: http://rodolphe-vaillant.fr/?e=20
     # See: http://ddg.cs.columbia.edu/SGP2014/LaplaceBeltrami.pdf
     if masses is None:
@@ -268,17 +266,15 @@
     L = calculate_weights(points, triangles, weight_method, sparse=True)
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", message="Changing the sparsity structure")
         L.setdiag(0)
         L.setdiag(-L.sum(axis=1))
         L = L.tocsr()
     laplacian = sp.diags(1 / masses, format="csr") @ L
-    if sparse:
-        return laplacian
-    return laplacian.toarray()
+    return laplacian
 
 
 def gradient_triangles(
     points: np.ndarray,
     triangles: np.ndarray,
     areas: Optional[np.ndarray] = None,
 ) -> Tuple[sp.csr_array, sp.csr_array]:
```

### Comparing `superscreen-0.9.0/superscreen/fluxoid.py` & `superscreen-0.9.1/superscreen/fluxoid.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/geometry.py` & `superscreen-0.9.1/superscreen/geometry.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/io.py` & `superscreen-0.9.1/superscreen/io.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/parameter.py` & `superscreen-0.9.1/superscreen/parameter.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/solution.py` & `superscreen-0.9.1/superscreen/solution.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/solver/solve.py` & `superscreen-0.9.1/superscreen/solver/solve.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/solver/solve_film.py` & `superscreen-0.9.1/superscreen/solver/solve_film.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/solver/utils.py` & `superscreen-0.9.1/superscreen/solver/utils.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/sources/constant.py` & `superscreen-0.9.1/superscreen/sources/constant.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/sources/current.py` & `superscreen-0.9.1/superscreen/sources/current.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/sources/dipole.py` & `superscreen-0.9.1/superscreen/sources/dipole.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/sources/vortex.py` & `superscreen-0.9.1/superscreen/sources/vortex.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/test/test_device.py` & `superscreen-0.9.1/superscreen/test/test_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         holes=holes,
         abstract_regions=abstract_regions,
     )
     assert device.meshes is None
     device.make_mesh(min_points=3000)
     assert isinstance(device.meshes, dict)
     assert set(device.meshes) == set(device.films)
-    assert all(isinstance(mesh, sc.device.Mesh) for mesh in device.meshes.values())
+    assert all(isinstance(mesh, sc.Mesh) for mesh in device.meshes.values())
     for mesh in device.meshes.values():
         centroids = sc.fem.centroids(mesh.sites, mesh.elements)
         assert centroids.shape[0] == mesh.elements.shape[0]
 
     print(device)
     assert device == device
     assert all(film == film for film in films)
```

### Comparing `superscreen-0.9.0/superscreen/test/test_distance.py` & `superscreen-0.9.1/superscreen/test/test_distance.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/test/test_parameter.py` & `superscreen-0.9.1/superscreen/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/test/test_polygon.py` & `superscreen-0.9.1/superscreen/test/test_polygon.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,26 +99,30 @@
         _ = sc.Polygon(name="bowtie", layer="layer", points=bowtie)
 
 
 @pytest.mark.parametrize("min_points", [None, 1000])
 @pytest.mark.parametrize("max_edge_length", [None, 0.25])
 @pytest.mark.parametrize("convex_hull", [False, True])
 @pytest.mark.parametrize("smooth", [0, 100])
-def test_polygon_make_mesh(min_points, max_edge_length, convex_hull, smooth):
+@pytest.mark.parametrize("build_operators", [False, True])
+def test_polygon_make_mesh(
+    min_points, max_edge_length, convex_hull, smooth, build_operators
+):
     poly = sc.Polygon(points=sc.geometry.box(2))
     poly = (
         poly.difference(poly.translate(dx=-1, dy=-1))
         .set_name("name")
         .set_layer("layer")
     )
     mesh = poly.make_mesh(
         min_points=min_points,
         max_edge_length=max_edge_length,
         convex_hull=convex_hull,
         smooth=smooth,
+        build_operators=build_operators,
     )
     assert isinstance(mesh, sc.Mesh)
 
 
 def test_plot_polygon():
     with non_gui_backend():
         ax = sc.Polygon(points=sc.geometry.box(1)).plot()
```

### Comparing `superscreen-0.9.0/superscreen/test/test_solution.py` & `superscreen-0.9.1/superscreen/test/test_solution.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/test/test_solve.py` & `superscreen-0.9.1/superscreen/test/test_solve.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/test/test_sources.py` & `superscreen-0.9.1/superscreen/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/test/test_transport.py` & `superscreen-0.9.1/superscreen/test/test_transport.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/test/test_visualization.py` & `superscreen-0.9.1/superscreen/test/test_visualization.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen/visualization.py` & `superscreen-0.9.1/superscreen/visualization.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.9.0/superscreen.egg-info/PKG-INFO` & `superscreen-0.9.1/superscreen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.9.0
+Version: 0.9.1
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
```

### Comparing `superscreen-0.9.0/superscreen.egg-info/SOURCES.txt` & `superscreen-0.9.1/superscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

