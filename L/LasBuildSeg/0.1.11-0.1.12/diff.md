# Comparing `tmp/LasBuildSeg-0.1.11.tar.gz` & `tmp/LasBuildSeg-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.11.tar", last modified: Wed May 17 09:30:20 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.12.tar", last modified: Wed May 17 19:19:37 2023, max compression
```

## Comparing `LasBuildSeg-0.1.11.tar` & `LasBuildSeg-0.1.12.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.765962 LasBuildSeg-0.1.11/
--rw-rw-rw-   0        0        0      107 2023-05-17 08:50:52.000000 LasBuildSeg-0.1.11/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.11/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.636387 LasBuildSeg-0.1.11/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.758031 LasBuildSeg-0.1.11/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.11/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    14470 2023-05-17 08:52:14.000000 LasBuildSeg-0.1.11/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.11/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.726094 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     2271 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-17 09:30:19.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.11/MANIFEST.in
--rw-rw-rw-   0        0        0     2271 2023-05-17 09:30:20.763006 LasBuildSeg-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     1339 2023-05-15 11:57:53.000000 LasBuildSeg-0.1.11/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-17 08:50:44.000000 LasBuildSeg-0.1.11/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-14 18:30:49.000000 LasBuildSeg-0.1.11/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 09:30:20.766955 LasBuildSeg-0.1.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 19:19:37.063806 LasBuildSeg-0.1.12/
+-rw-rw-rw-   0        0        0      107 2023-05-17 19:14:54.000000 LasBuildSeg-0.1.12/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.12/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 19:19:36.913309 LasBuildSeg-0.1.12/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-17 19:19:37.056830 LasBuildSeg-0.1.12/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.12/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    14489 2023-05-17 19:17:14.000000 LasBuildSeg-0.1.12/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.12/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 19:19:37.001016 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     2372 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-17 19:19:36.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 19:19:35.000000 LasBuildSeg-0.1.12/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     2372 2023-05-17 19:19:37.060816 LasBuildSeg-0.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2023-05-17 09:56:57.000000 LasBuildSeg-0.1.12/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-17 19:14:58.000000 LasBuildSeg-0.1.12/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-17 11:16:46.000000 LasBuildSeg-0.1.12/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 19:19:37.063806 LasBuildSeg-0.1.12/setup.cfg
```

### Comparing `LasBuildSeg-0.1.11/LICENSE.txt` & `LasBuildSeg-0.1.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.11/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.12/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.11/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.12/LasBuildSeg/LasBuildSeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 from rasterio.mask import mask
 import rasterio.features
 from shapely.geometry import shape, mapping
 import json
 from shapely.geometry import Polygon, MultiPolygon
 
 
-def generate_dsm(las_file_name: str, input_epsg: int, resolution, intermethod: str):
+def generate_dsm(las_file_name: str, input_epsg: int, resolution, intermethod: str, scale):
     # Read the LAS file
     las_file = laspy.read(las_file_name)
 
     # Set the CRS information to projection
-    las_file.header.scale[0] = 0.01
-    las_file.header.scale[1] = 0.01
-    las_file.header.scale[2] = 0.01
+    las_file.header.scale[0] = scale
+    las_file.header.scale[1] = scale
+    las_file.header.scale[2] = scale
 
     # Write the updated LAS file
     las_file.write("updated_file.las")
 
     # Read the updated LAS file
     las_file = laspy.read('updated_file.las')
 
@@ -64,21 +64,21 @@
         dst.write(dsm, 1)
     
     print('Success in Creating DSM')
 #generate_dsm('Yourdata.laz', 8734, 1)
 
 
 
-def generate_dtm(las_file_path, input_epsg, resolution, intermethod):
+def generate_dtm(las_file_path, input_epsg, resolution, intermethod,scale):
     # Load LiDAR data
     las_file_dtm = laspy.read(las_file_path)
      # Set the CRS information to projection
-    las_file_dtm.header.scale[0] = 0.01
-    las_file_dtm.header.scale[1] = 0.01
-    las_file_dtm.header.scale[2] = 0.01
+    las_file_dtm.header.scale[0] = scale
+    las_file_dtm.header.scale[1] = scale
+    las_file_dtm.header.scale[2] = scale
 
     # Write the updated LAS file
     las_file_dtm.write("updated_file.las")
 
     # Read the updated LAS file
     las_file_dtm = laspy.read('updated_file.las')
```

### Comparing `LasBuildSeg-0.1.11/LasBuildSeg/__init__.py` & `LasBuildSeg-0.1.12/LasBuildSeg/__init__.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.11/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.12/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.11
+Version: 0.1.12
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,18 +42,22 @@
 dem, _ = lasb.read_geotiff('dsm3857.tif')
 img_8bit = lasb.to_8bit(img)
 constant = 3.6
 block_size = 51
 img_thresh = lasb.threshold(img_8bit, block_size, constant)
 kernel_size = 3
 img_open = lasb.morphopen(img_thresh, kernel_size)
-min_size=35
-max_size=5000
+
+min_size = 35
+max_size = 5000
+squareness_threshold=0.3 
+width_threshold=3 
+height_threshold=3 
 tri_threshold=3
-building_mask = lasb.filter_contours(img_open, dem, profile, min_size, max_size, tri_threshold=tri_threshold)
+building_mask = Lasb.filter_contoursntri(img_open, profile, min_size, max_size, squareness_threshold, width_threshold, height_threshold)
 kernel_size = 3
 CloseKernel_size=15
 building_mask_closed = lasb.close(building_mask, CloseKernel_size)
 # Invert the building mask to make buildings appear as white ground pixels
 inverted_building_mask = np.ones_like(building_mask, dtype=np.uint8) - building_mask_closed
 lasb.write_geotiff('buildings.tif', building_mask_closed, profile)
 lasb.building_footprints_to_geojson('buildings.tif', 'building.geojson')
```

### Comparing `LasBuildSeg-0.1.11/PKG-INFO` & `LasBuildSeg-0.1.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.11
+Version: 0.1.12
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,18 +42,22 @@
 dem, _ = lasb.read_geotiff('dsm3857.tif')
 img_8bit = lasb.to_8bit(img)
 constant = 3.6
 block_size = 51
 img_thresh = lasb.threshold(img_8bit, block_size, constant)
 kernel_size = 3
 img_open = lasb.morphopen(img_thresh, kernel_size)
-min_size=35
-max_size=5000
+
+min_size = 35
+max_size = 5000
+squareness_threshold=0.3 
+width_threshold=3 
+height_threshold=3 
 tri_threshold=3
-building_mask = lasb.filter_contours(img_open, dem, profile, min_size, max_size, tri_threshold=tri_threshold)
+building_mask = Lasb.filter_contoursntri(img_open, profile, min_size, max_size, squareness_threshold, width_threshold, height_threshold)
 kernel_size = 3
 CloseKernel_size=15
 building_mask_closed = lasb.close(building_mask, CloseKernel_size)
 # Invert the building mask to make buildings appear as white ground pixels
 inverted_building_mask = np.ones_like(building_mask, dtype=np.uint8) - building_mask_closed
 lasb.write_geotiff('buildings.tif', building_mask_closed, profile)
 lasb.building_footprints_to_geojson('buildings.tif', 'building.geojson')
```

### Comparing `LasBuildSeg-0.1.11/Setup.py` & `LasBuildSeg-0.1.12/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.11',
+  version='0.1.12',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

