# Comparing `tmp/LasBuildSeg-0.1.10.tar.gz` & `tmp/LasBuildSeg-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.1.10.tar", last modified: Mon May 15 11:59:33 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.1.11.tar", last modified: Wed May 17 09:30:20 2023, max compression
```

## Comparing `LasBuildSeg-0.1.10.tar` & `LasBuildSeg-0.1.11.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:59:33.214181 LasBuildSeg-0.1.10/
--rw-rw-rw-   0        0        0      108 2023-05-15 11:57:46.000000 LasBuildSeg-0.1.10/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.10/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 11:59:33.095560 LasBuildSeg-0.1.10/LasBuildSeg/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:59:33.208182 LasBuildSeg-0.1.10/LasBuildSeg/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.10/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
--rw-rw-rw-   0        0        0    14494 2023-05-14 18:22:59.000000 LasBuildSeg-0.1.10/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      472 2023-05-14 18:36:38.000000 LasBuildSeg-0.1.10/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:59:33.176297 LasBuildSeg-0.1.10/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     2271 2023-05-15 11:59:31.000000 LasBuildSeg-0.1.10/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-15 11:59:32.000000 LasBuildSeg-0.1.10/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:59:31.000000 LasBuildSeg-0.1.10/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-15 11:59:31.000000 LasBuildSeg-0.1.10/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 11:59:31.000000 LasBuildSeg-0.1.10/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2271 2023-05-15 11:59:33.212170 LasBuildSeg-0.1.10/PKG-INFO
--rw-rw-rw-   0        0        0     1339 2023-05-15 11:57:53.000000 LasBuildSeg-0.1.10/README.md
--rw-rw-rw-   0        0        0     1496 2023-05-15 11:58:01.000000 LasBuildSeg-0.1.10/Setup.py
--rw-rw-rw-   0        0        0      123 2023-05-14 18:30:49.000000 LasBuildSeg-0.1.10/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 11:59:33.214181 LasBuildSeg-0.1.10/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.765962 LasBuildSeg-0.1.11/
+-rw-rw-rw-   0        0        0      107 2023-05-17 08:50:52.000000 LasBuildSeg-0.1.11/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.1.11/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.636387 LasBuildSeg-0.1.11/LasBuildSeg/
+drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.758031 LasBuildSeg-0.1.11/LasBuildSeg/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.1.11/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py
+-rw-rw-rw-   0        0        0    14470 2023-05-17 08:52:14.000000 LasBuildSeg-0.1.11/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      518 2023-05-17 08:50:32.000000 LasBuildSeg-0.1.11/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:30:20.726094 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     2271 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-17 09:30:19.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 09:30:17.000000 LasBuildSeg-0.1.11/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.1.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2271 2023-05-17 09:30:20.763006 LasBuildSeg-0.1.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1339 2023-05-15 11:57:53.000000 LasBuildSeg-0.1.11/README.md
+-rw-rw-rw-   0        0        0     1496 2023-05-17 08:50:44.000000 LasBuildSeg-0.1.11/Setup.py
+-rw-rw-rw-   0        0        0      123 2023-05-14 18:30:49.000000 LasBuildSeg-0.1.11/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 09:30:20.766955 LasBuildSeg-0.1.11/setup.cfg
```

### Comparing `LasBuildSeg-0.1.10/LICENSE.txt` & `LasBuildSeg-0.1.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.10/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py` & `LasBuildSeg-0.1.11/LasBuildSeg/.ipynb_checkpoints/LasBuildSeg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.10/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.1.11/LasBuildSeg/LasBuildSeg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sun May 7 10:46:30 2023
 
 
 @author: Mertcan
 """
-#This of example of an how you can run your code
-# import LasBuildSeg as Lasb
-# import numpy as np
-
-# Lasb.generate_dsm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
-# Lasb.generate_dtm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
-# Lasb.generate_ndhm('dtm.tif', 'dsm.tif')
-# img, profile = Lasb.read_geotiff('ndhm.tif')
-# img_8bit = Lasb.to_8bit(img)
-# constant = 4.6
-# block_size = 51
-# img_thresh = Lasb.threshold(img_8bit, block_size, constant)
-# kernel_size = 3
-# img_open = Lasb.morphopen(img_thresh, kernel_size)
-# min_size=35
-# max_size=5000
-# building_mask = Lasb.filter_contours(img_open, profile, min_size, max_size)
-# kernel_size = 3
-# CloseKernel_size=15
-# building_mask_closed = Lasb.close(building_mask, CloseKernel_size)
-# # Invert the building mask to make buildings appear as white ground pixels
-# inverted_building_mask = np.ones_like(building_mask, dtype=np.uint8) - building_mask_closed
-# Las.write_geotiff('buildings.tif', inverted_building_mask, profile)
-# print('All of our steps are done.')
 
 import laspy
 import numpy as np
 from scipy.interpolate import griddata
 import rasterio
 import pyproj
 import cv2
@@ -43,15 +19,15 @@
 from rasterio.mask import mask
 import rasterio.features
 from shapely.geometry import shape, mapping
 import json
 from shapely.geometry import Polygon, MultiPolygon
 
 
-def generate_dsm(las_file_name: str, input_epsg: int, resolution):
+def generate_dsm(las_file_name: str, input_epsg: int, resolution, intermethod: str):
     # Read the LAS file
     las_file = laspy.read(las_file_name)
 
     # Set the CRS information to projection
     las_file.header.scale[0] = 0.01
     las_file.header.scale[1] = 0.01
     las_file.header.scale[2] = 0.01
@@ -76,27 +52,27 @@
     y_min = np.floor(min(y))
     y_max = np.ceil(max(y))
 
     # Generate the grid of points for the DSM
     grid_x, grid_y = np.meshgrid(np.arange(x_min, x_max , resolution), np.arange(y_min, y_max , resolution))
 
     # Generate the DSM using Nearest Neighbor interpolation of the point cloud
-    dsm = griddata((x, y), z, (grid_x, grid_y), method='nearest')
+    dsm = griddata((x, y), z, (grid_x, grid_y), method=intermethod)
 
     # Save the DSM to a GeoTIFF file using rasterio
     with rasterio.open("dsm.tif", 'w', driver='GTiff', height=dsm.shape[0], width=dsm.shape[1], count=1, 
                        dtype=dsm.dtype, crs=input_crs, transform=rasterio.transform.Affine(resolution, 0, x_min, 0, resolution, y_min)) as dst:
         dst.write(dsm, 1)
     
     print('Success in Creating DSM')
 #generate_dsm('Yourdata.laz', 8734, 1)
 
 
 
-def generate_dtm(las_file_path, input_epsg, resolution):
+def generate_dtm(las_file_path, input_epsg, resolution, intermethod):
     # Load LiDAR data
     las_file_dtm = laspy.read(las_file_path)
      # Set the CRS information to projection
     las_file_dtm.header.scale[0] = 0.01
     las_file_dtm.header.scale[1] = 0.01
     las_file_dtm.header.scale[2] = 0.01
 
@@ -152,15 +128,15 @@
     dsm_file = laspy.read('updated_file.las')
     dsm_points = np.vstack((dsm_file.x, dsm_file.y, dsm_file.z)).T
 
     # Classify points as aboveground features (non-ground points)
     non_ground_points = dsm_points[dsm_file.classification != 2]
 
     # Interpolate the non-ground points onto the mesh grid
-    non_ground_z = griddata(non_ground_points[:, :2], non_ground_points[:, 2], (mesh_x, mesh_y), method='nearest')
+    non_ground_z = griddata(non_ground_points[:, :2], non_ground_points[:, 2], (mesh_x, mesh_y), method=intermethod)
 
     # Subtract the interpolated non-ground values from the interpolated ground values
     dtm = 10*mesh_z - non_ground_z
 
     # Write the output raster to a file
     with rasterio.open('dtm.tif', 'w', **profile) as dst:
         dst.write(dtm, 1)
@@ -296,14 +272,44 @@
 # kernel_size: the size of the kernel used for the morphological operation
 # Returns the image data with small objects removed.
 def morphopen(img_thresh, kernel_size=3):
     kernel = np.ones((kernel_size, kernel_size), np.uint8)
     img_open = cv2.morphologyEx(img_thresh, cv2.MORPH_OPEN, kernel)
     return img_open
 
+
+
+
+#No tri only for testing purposes
+def filter_contoursntri(img_open, profile, min_size=35, max_size=5000, squareness_threshold=0.3, width_threshold=3, height_threshold=3):
+    
+    contours, _ = cv2.findContours(img_open.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+    pixel_size = abs(profile['transform'][0])
+    building_mask = np.zeros_like(img_open, dtype=np.uint8)
+
+
+    for contour in contours:
+        rect = cv2.minAreaRect(contour)
+        w, h = rect[1]
+        if w < h:
+            w, h = h, w
+        squareness = w / h if h != 0 else 0
+        size = w * h * pixel_size ** 2
+
+        # Compute the average TRI within the building contour
+        mask = np.zeros_like(img_open, dtype=np.uint8)
+        cv2.drawContours(mask, [contour], -1, 1, -1)
+
+        if squareness >= squareness_threshold and min_size <= size <= max_size and w >= width_threshold and h >= height_threshold:
+            cv2.drawContours(building_mask, [contour], -1, 255, -1)
+
+    return building_mask
+
+
+
 # This function filters out contours that do not meet certain criteria (size, shape, etc.) and creates a binary mask of the remaining objects.
 # img_open: the image data with small objects removed
 # profile: a dictionary with metadata about the image
 # min_size: the minimum size of objects to keep
 # max_size: the maximum size of objects to keep
 # squareness_threshold: the minimum squareness of objects to keep (ratio of width to height)
 # width_threshold: the minimum width of objects to keep
```

### Comparing `LasBuildSeg-0.1.10/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.1.11/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.10
+Version: 0.1.11
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.10/PKG-INFO` & `LasBuildSeg-0.1.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.1.10
+Version: 0.1.11
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.1.10/README.md` & `LasBuildSeg-0.1.11/README.md`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.1.10/Setup.py` & `LasBuildSeg-0.1.11/Setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.1.10',
+  version='0.1.11',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

