# Comparing `tmp/archaea-1.1.8.tar.gz` & `tmp/archaea-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archaea-1.1.8.tar", last modified: Tue Jan 24 07:29:27 2023, max compression
+gzip compressed data, was "archaea-1.1.9.tar", last modified: Fri Feb 10 12:14:54 2023, max compression
```

## Comparing `archaea-1.1.8.tar` & `archaea-1.1.9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.098638 archaea-1.1.8/
--rw-rw-rw-   0        0        0    11558 2022-10-28 15:01:40.000000 archaea-1.1.8/LICENSE
--rw-rw-rw-   0        0        0    11558 2022-10-28 15:01:40.000000 archaea-1.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2504 2023-01-24 07:29:27.098638 archaea-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2023-01-23 17:17:26.000000 archaea-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.063819 archaea-1.1.8/archaea/
--rw-rw-rw-   0        0        0      731 2023-01-23 19:46:14.000000 archaea-1.1.8/archaea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.079083 archaea-1.1.8/archaea/earcut/
--rw-rw-rw-   0        0        0        0 2022-12-28 06:58:18.000000 archaea-1.1.8/archaea/earcut/__init__.py
--rw-rw-rw-   0        0        0    19263 2022-12-29 04:07:44.000000 archaea-1.1.8/archaea/earcut/earcut.py
--rw-rw-rw-   0        0        0    20722 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/earcut/earcut3d.py
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.089118 archaea-1.1.8/archaea/geometry/
--rw-rw-rw-   0        0        0        0 2022-11-10 05:00:25.000000 archaea-1.1.8/archaea/geometry/__init__.py
--rw-rw-rw-   0        0        0     1676 2022-12-27 11:03:38.000000 archaea-1.1.8/archaea/geometry/coordinate_array.py
--rw-rw-rw-   0        0        0     3258 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/face.py
--rw-rw-rw-   0        0        0     5716 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/line_segment.py
--rw-rw-rw-   0        0        0     6336 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/loop.py
--rw-rw-rw-   0        0        0     1380 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/mesh.py
--rw-rw-rw-   0        0        0      119 2022-12-29 08:09:46.000000 archaea-1.1.8/archaea/geometry/orientation.py
--rw-rw-rw-   0        0        0     1741 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/plane.py
--rw-rw-rw-   0        0        0      955 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/point2d.py
--rw-rw-rw-   0        0        0     1242 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/point3d.py
--rw-rw-rw-   0        0        0     1092 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/polyline.py
--rw-rw-rw-   0        0        0     1727 2022-12-29 09:45:27.000000 archaea-1.1.8/archaea/geometry/utils.py
--rw-rw-rw-   0        0        0     1458 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/vector.py
--rw-rw-rw-   0        0        0      626 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/vector2d.py
--rw-rw-rw-   0        0        0     1381 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/geometry/vector3d.py
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.090115 archaea-1.1.8/archaea/writer/
--rw-rw-rw-   0        0        0        0 2022-10-28 15:01:40.000000 archaea-1.1.8/archaea/writer/__init__.py
--rw-rw-rw-   0        0        0     2287 2023-01-22 11:58:31.000000 archaea-1.1.8/archaea/writer/to_manual_stl.py
--rw-rw-rw-   0        0        0      766 2022-12-27 06:40:05.000000 archaea-1.1.8/archaea/writer/to_stl.py
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.077086 archaea-1.1.8/archaea.egg-info/
--rw-rw-rw-   0        0        0     2504 2023-01-24 07:29:26.000000 archaea-1.1.8/archaea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1221 2023-01-24 07:29:27.000000 archaea-1.1.8/archaea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 07:29:26.000000 archaea-1.1.8/archaea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-01-24 07:29:26.000000 archaea-1.1.8/archaea.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-24 07:29:27.000000 archaea-1.1.8/archaea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-24 07:29:27.100638 archaea-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1489 2023-01-24 07:28:55.000000 archaea-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.091117 archaea-1.1.8/test/
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.096118 archaea-1.1.8/test/geometry/
--rw-rw-rw-   0        0        0        0 2022-11-10 04:44:56.000000 archaea-1.1.8/test/geometry/__init__.py
--rw-rw-rw-   0        0        0     2026 2023-01-22 11:58:31.000000 archaea-1.1.8/test/geometry/test_coordinate_array.py
--rw-rw-rw-   0        0        0     4588 2023-01-22 11:58:31.000000 archaea-1.1.8/test/geometry/test_line_segment.py
--rw-rw-rw-   0        0        0     3935 2023-01-22 11:58:31.000000 archaea-1.1.8/test/geometry/test_loop.py
--rw-rw-rw-   0        0        0     5517 2023-01-22 11:58:31.000000 archaea-1.1.8/test/geometry/test_mesh.py
--rw-rw-rw-   0        0        0     1250 2023-01-22 11:58:31.000000 archaea-1.1.8/test/geometry/test_vector.py
--rw-rw-rw-   0        0        0     1229 2023-01-22 11:58:31.000000 archaea-1.1.8/test/geometry/test_vector3d.py
--rw-rw-rw-   0        0        0     1833 2023-01-22 11:58:31.000000 archaea-1.1.8/test/geometry/test_wall.py
-drwxrwxrwx   0        0        0        0 2023-01-24 07:29:27.098638 archaea-1.1.8/test/simulation_objects/
--rw-rw-rw-   0        0        0        0 2022-11-14 06:19:28.000000 archaea-1.1.8/test/simulation_objects/__init__.py
--rw-rw-rw-   0        0        0     2167 2023-01-22 11:58:31.000000 archaea-1.1.8/test/simulation_objects/test_domain.py
--rw-rw-rw-   0        0        0     1441 2023-01-22 11:58:31.000000 archaea-1.1.8/test/simulation_objects/test_wall.py
--rw-rw-rw-   0        0        0     2303 2023-01-22 11:58:31.000000 archaea-1.1.8/test/simulation_objects/test_zone.py
--rw-rw-rw-   0        0        0      794 2023-01-22 11:58:31.000000 archaea-1.1.8/test/test_area.py
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.361144 archaea-1.1.9/
+-rw-rw-rw-   0        0        0    11558 2022-10-20 10:22:44.000000 archaea-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0    11558 2023-02-10 11:49:26.000000 archaea-1.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2504 2023-02-10 12:14:54.361144 archaea-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2023-02-10 11:49:26.000000 archaea-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.323223 archaea-1.1.9/archaea/
+-rw-rw-rw-   0        0        0      731 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.335190 archaea-1.1.9/archaea/earcut/
+-rw-rw-rw-   0        0        0        0 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/earcut/__init__.py
+-rw-rw-rw-   0        0        0    19263 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/earcut/earcut.py
+-rw-rw-rw-   0        0        0    20722 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/earcut/earcut3d.py
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.347158 archaea-1.1.9/archaea/geometry/
+-rw-rw-rw-   0        0        0        0 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/__init__.py
+-rw-rw-rw-   0        0        0     1676 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/coordinate_array.py
+-rw-rw-rw-   0        0        0     3258 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/face.py
+-rw-rw-rw-   0        0        0     5716 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/line_segment.py
+-rw-rw-rw-   0        0        0     6336 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/loop.py
+-rw-rw-rw-   0        0        0     1380 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/mesh.py
+-rw-rw-rw-   0        0        0      119 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/orientation.py
+-rw-rw-rw-   0        0        0     1741 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/plane.py
+-rw-rw-rw-   0        0        0      955 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/point2d.py
+-rw-rw-rw-   0        0        0     1249 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/point3d.py
+-rw-rw-rw-   0        0        0     1092 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/polyline.py
+-rw-rw-rw-   0        0        0     1727 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/utils.py
+-rw-rw-rw-   0        0        0     1458 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/vector.py
+-rw-rw-rw-   0        0        0      626 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/vector2d.py
+-rw-rw-rw-   0        0        0     1381 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/geometry/vector3d.py
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.349152 archaea-1.1.9/archaea/writer/
+-rw-rw-rw-   0        0        0        0 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/writer/__init__.py
+-rw-rw-rw-   0        0        0     2287 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/writer/to_manual_stl.py
+-rw-rw-rw-   0        0        0      766 2023-02-10 11:49:26.000000 archaea-1.1.9/archaea/writer/to_stl.py
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.333194 archaea-1.1.9/archaea.egg-info/
+-rw-rw-rw-   0        0        0     2504 2023-02-10 12:14:54.000000 archaea-1.1.9/archaea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1251 2023-02-10 12:14:54.000000 archaea-1.1.9/archaea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-10 12:14:54.000000 archaea-1.1.9/archaea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-02-10 12:14:54.000000 archaea-1.1.9/archaea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-02-10 12:14:54.000000 archaea-1.1.9/archaea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-02-10 12:14:54.362117 archaea-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1489 2023-02-10 12:13:22.000000 archaea-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.350150 archaea-1.1.9/test/
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.357131 archaea-1.1.9/test/geometry/
+-rw-rw-rw-   0        0        0        0 2022-10-20 10:22:44.000000 archaea-1.1.9/test/geometry/__init__.py
+-rw-rw-rw-   0        0        0     2026 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_coordinate_array.py
+-rw-rw-rw-   0        0        0     4588 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_line_segment.py
+-rw-rw-rw-   0        0        0     3935 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_loop.py
+-rw-rw-rw-   0        0        0     5517 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_mesh.py
+-rw-rw-rw-   0        0        0      632 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_point3d.py
+-rw-rw-rw-   0        0        0     1250 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_vector.py
+-rw-rw-rw-   0        0        0     1229 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_vector3d.py
+-rw-rw-rw-   0        0        0     1833 2023-02-10 11:49:26.000000 archaea-1.1.9/test/geometry/test_wall.py
+drwxrwxrwx   0        0        0        0 2023-02-10 12:14:54.360148 archaea-1.1.9/test/simulation_objects/
+-rw-rw-rw-   0        0        0        0 2022-11-14 04:45:13.000000 archaea-1.1.9/test/simulation_objects/__init__.py
+-rw-rw-rw-   0        0        0     2167 2023-02-10 11:49:26.000000 archaea-1.1.9/test/simulation_objects/test_domain.py
+-rw-rw-rw-   0        0        0     1441 2023-02-10 11:49:26.000000 archaea-1.1.9/test/simulation_objects/test_wall.py
+-rw-rw-rw-   0        0        0     2303 2023-02-10 11:49:26.000000 archaea-1.1.9/test/simulation_objects/test_zone.py
+-rw-rw-rw-   0        0        0      794 2023-02-10 11:49:26.000000 archaea-1.1.9/test/test_area.py
```

### Comparing `archaea-1.1.8/LICENSE` & `archaea-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/LICENSE.txt` & `archaea-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/PKG-INFO` & `archaea-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: archaea
-Version: 1.1.8
+Version: 1.1.9
 Summary: Playground for geometry.
 Home-page: https://github.com/archaeans/archaea
-Download-URL: https://github.com/archaeans/archaea/archive/refs/tags/1.1.8.tar.gz
+Download-URL: https://github.com/archaeans/archaea/archive/refs/tags/1.1.9.tar.gz
 Author: Oğuzhan Koral
 Author-email: oguzhankoral@gmail.com
 License: Apache 2.0
 Keywords: geometry,mesh,stl,triangulation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `archaea-1.1.8/README.md` & `archaea-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/__init__.py` & `archaea-1.1.9/archaea/__init__.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/earcut/earcut.py` & `archaea-1.1.9/archaea/earcut/earcut.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/earcut/earcut3d.py` & `archaea-1.1.9/archaea/earcut/earcut3d.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/coordinate_array.py` & `archaea-1.1.9/archaea/geometry/coordinate_array.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/face.py` & `archaea-1.1.9/archaea/geometry/face.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/line_segment.py` & `archaea-1.1.9/archaea/geometry/line_segment.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/loop.py` & `archaea-1.1.9/archaea/geometry/loop.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/mesh.py` & `archaea-1.1.9/archaea/geometry/mesh.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/plane.py` & `archaea-1.1.9/archaea/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/point2d.py` & `archaea-1.1.9/archaea/geometry/point2d.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/point3d.py` & `archaea-1.1.9/archaea/geometry/point3d.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,8 +35,8 @@
         return Vector3d(other.x - self.x, other.y - self.y, other.z - self.z)
 
     def distance_to(self, other):
         return (((self.x - other.x) ** 2) + ((self.y - other.y) ** 2) + ((self.z - other.z) ** 2)) ** 0.5
 
     @classmethod
     def origin(cls):
-        cls(0, 0, 0)
+        return cls(0, 0, 0)
```

### Comparing `archaea-1.1.8/archaea/geometry/polyline.py` & `archaea-1.1.9/archaea/geometry/polyline.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/utils.py` & `archaea-1.1.9/archaea/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/vector.py` & `archaea-1.1.9/archaea/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/vector2d.py` & `archaea-1.1.9/archaea/geometry/vector2d.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/geometry/vector3d.py` & `archaea-1.1.9/archaea/geometry/vector3d.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/writer/to_manual_stl.py` & `archaea-1.1.9/archaea/writer/to_manual_stl.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea/writer/to_stl.py` & `archaea-1.1.9/archaea/writer/to_stl.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/archaea.egg-info/PKG-INFO` & `archaea-1.1.9/archaea.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: archaea
-Version: 1.1.8
+Version: 1.1.9
 Summary: Playground for geometry.
 Home-page: https://github.com/archaeans/archaea
-Download-URL: https://github.com/archaeans/archaea/archive/refs/tags/1.1.8.tar.gz
+Download-URL: https://github.com/archaeans/archaea/archive/refs/tags/1.1.9.tar.gz
 Author: Oğuzhan Koral
 Author-email: oguzhankoral@gmail.com
 License: Apache 2.0
 Keywords: geometry,mesh,stl,triangulation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `archaea-1.1.8/archaea.egg-info/SOURCES.txt` & `archaea-1.1.9/archaea.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 archaea/writer/to_stl.py
 test/test_area.py
 test/geometry/__init__.py
 test/geometry/test_coordinate_array.py
 test/geometry/test_line_segment.py
 test/geometry/test_loop.py
 test/geometry/test_mesh.py
+test/geometry/test_point3d.py
 test/geometry/test_vector.py
 test/geometry/test_vector3d.py
 test/geometry/test_wall.py
 test/simulation_objects/__init__.py
 test/simulation_objects/test_domain.py
 test/simulation_objects/test_wall.py
 test/simulation_objects/test_zone.py
```

### Comparing `archaea-1.1.8/setup.py` & `archaea-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='archaea',
     packages=setuptools.find_packages(exclude=['archaea.extensions', 'archaea.format', 'test']),
-    version='1.1.8',
+    version='1.1.9',
     license='Apache 2.0',
     description='Playground for geometry.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme='README.md',
     author='Oğuzhan Koral',
     author_email='oguzhankoral@gmail.com',
     url='https://github.com/archaeans/archaea',
-    download_url='https://github.com/archaeans/archaea/archive/refs/tags/1.1.8.tar.gz',
+    download_url='https://github.com/archaeans/archaea/archive/refs/tags/1.1.9.tar.gz',
     keywords=['geometry', 'mesh', 'stl', 'triangulation'],
     install_requires=[
         'numpy',
         'numpy-stl'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `archaea-1.1.8/test/geometry/test_coordinate_array.py` & `archaea-1.1.9/test/geometry/test_coordinate_array.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/geometry/test_line_segment.py` & `archaea-1.1.9/test/geometry/test_line_segment.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/geometry/test_loop.py` & `archaea-1.1.9/test/geometry/test_loop.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/geometry/test_mesh.py` & `archaea-1.1.9/test/geometry/test_mesh.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/geometry/test_vector.py` & `archaea-1.1.9/test/geometry/test_vector.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/geometry/test_vector3d.py` & `archaea-1.1.9/test/geometry/test_vector3d.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/geometry/test_wall.py` & `archaea-1.1.9/test/geometry/test_wall.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/simulation_objects/test_domain.py` & `archaea-1.1.9/test/simulation_objects/test_domain.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/simulation_objects/test_wall.py` & `archaea-1.1.9/test/simulation_objects/test_wall.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/simulation_objects/test_zone.py` & `archaea-1.1.9/test/simulation_objects/test_zone.py`

 * *Files identical despite different names*

### Comparing `archaea-1.1.8/test/test_area.py` & `archaea-1.1.9/test/test_area.py`

 * *Files identical despite different names*

