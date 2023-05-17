# Comparing `tmp/pvbm-2.0.0.tar.gz` & `tmp/pvbm-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-2.0.0.tar", last modified: Wed May 17 14:53:31 2023, max compression
+gzip compressed data, was "pvbm-2.1.0.tar", last modified: Wed May 17 15:16:12 2023, max compression
```

## Comparing `pvbm-2.0.0.tar` & `pvbm-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.515562 pvbm-2.0.0/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 14:53:31.515427 pvbm-2.0.0/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.513067 pvbm-2.0.0/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    11131 2023-05-17 14:49:51.000000 pvbm-2.0.0/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4602 2023-05-17 14:44:47.000000 pvbm-2.0.0/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.0.0/PVBM/__init__.py
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.514278 pvbm-2.0.0/PVBM/helpers/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.0.0/PVBM/helpers/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.0.0/PVBM/helpers/branching2.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     8674 2023-04-30 12:24:25.000000 pvbm-2.0.0/PVBM/helpers/branching_angle.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.0.0/PVBM/helpers/tortuosity.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     3799 2023-05-17 14:52:46.000000 pvbm-2.0.0/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.515233 pvbm-2.0.0/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      337 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-17 14:53:31.515609 pvbm-2.0.0/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-17 14:53:23.000000 pvbm-2.0.0/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:16:12.978945 pvbm-2.1.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 15:16:12.978827 pvbm-2.1.0/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:16:12.976911 pvbm-2.1.0/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    11131 2023-05-17 15:14:40.000000 pvbm-2.1.0/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4909 2023-05-17 15:12:06.000000 pvbm-2.1.0/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.0/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:16:12.977857 pvbm-2.1.0/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.0/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.1.0/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     8674 2023-04-30 12:24:25.000000 pvbm-2.1.0/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.1.0/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     3799 2023-05-17 14:52:46.000000 pvbm-2.1.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:16:12.978654 pvbm-2.1.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 15:16:12.000000 pvbm-2.1.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      337 2023-05-17 15:16:12.000000 pvbm-2.1.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-17 15:16:12.000000 pvbm-2.1.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-17 15:16:12.000000 pvbm-2.1.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-17 15:16:12.000000 pvbm-2.1.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-17 15:16:12.978983 pvbm-2.1.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-17 15:15:08.000000 pvbm-2.1.0/setup.py
```

### Comparing `pvbm-2.0.0/PKG-INFO` & `pvbm-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.0.0/PVBM/FractalAnalysis.py` & `pvbm-2.1.0/PVBM/FractalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.0.0/PVBM/GeometricalAnalysis.py` & `pvbm-2.1.0/PVBM/GeometricalAnalysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,20 @@
     def compute_particular_points(self,segmentation_skeleton):
         """
     The particular point is the union between the endpoints and the intersection points.
     This function computes the number of endpoints and intersection points of the fundus image vasculature segmentation.
 
     :param segmentation_skeleton: The skeleton of the segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
     :type segmentation_skeleton: np.ndarray
-    :return: The number of endpoints, the number of intersection points, an array with endpoint pixel positions, and an array with intersection point pixel positions.
+    :return:
+        - The number of endpoints
+        - The number of intersection points,
+        - An array with endpoint pixel positions
+        - An array with intersection point pixel positions.
+    
     :rtype: (int, int, np.ndarray, np.ndarray)
     """
         filter_ = np.array([[1, 1, 1], [1, 10, 1], [1, 1, 1]])
         neighbours = convolve2d(segmentation_skeleton, filter_, mode="same")
 
         end_points = neighbours == 11
         inter_points = neighbours >= 13
@@ -42,29 +47,39 @@
         inter_points_count = np.sum(inter_points)
 
         return end_points_count, inter_points_count, end_points, inter_points
     
     def compute_tortuosity_length(self,segmentation_skeleton):
         """
     This function computes the median tortuosity and the length of the fundus image vasculature segmentation.
+    
     :param segmentation_skeleton: The skeleton of the segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
     :type segmentation_skeleton: np.ndarray
-    :return: The median tortuosity, overall length (in pixel), a list of chord distance of each blood vessel (in pixel), a list of lengths distance (arc) of each blood vessel (in pixel), and a dictionary with connection information.
+    :return:
+        - The median tortuosity
+        - The overall length (in pixel)
+        - A list of chord distance of each blood vessel (in pixel)
+        - A list of lengths distance (arc) of each blood vessel (in pixel)
+        - A dictionary with connection information.
+    
     :rtype: (float, float, list, list, dict)
     """
         median_tor,length,tor,l,connection_dico = compute_tortuosity(segmentation_skeleton)
         return median_tor,length ,tor,l,connection_dico
 
     def compute_perimeter(self,segmentation):
         """
     This function computes the perimeter and the border of the fundus image vasculature segmentation.
 
     :param segmentation: The segmentation is a two-dimensional array (HxW) with binary value (0 or 1).
     :type segmentation: np.ndarray
-    :return: The perimeter (in pixel) and a matrix containing the edges of the segmentation.
+    :return:
+        - The perimeter (in pixel)
+        - A matrix containing the edges of the segmentation.
+    
     :rtype: (float, np.ndarray)
     """
         filter_ = np.array([[-1, -1, -1], [-1, 8, -1], [-1, -1, -1]])
         derivative = convolve2d(segmentation,filter_, mode="same")
         border = derivative>0
         segmentation_skeleton = skeletonize(np.ascontiguousarray(border.T)).T
         _,perim,_,_,_ = compute_tortuosity(segmentation_skeleton)
@@ -72,15 +87,21 @@
     
     def compute_branching_angles(self,segmentation_skeleton):
         """
     This function computes the mean, standard deviation, and median branching angle of the fundus image vasculature segmentation.
 
     :param segmentation_skeleton: The skeleton of the segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
     :type segmentation_skeleton: np.ndarray
-    :return: The mean branching angles (°), the standard deviation of branching angles (°), the median branching angles (°), a dictionary containing all the branching angles, and a numpy array with a visualization of the computed centroid.
+    :return:
+        - The mean of the branching angles (in degrees)
+        - The standard deviation of the branching angles (in degrees)
+        - The median of the branching angles (in degrees)
+        - A dictionary containing all the branching angles with their respective indices in the array as keys
+        - A two-dimensional numpy array representing the visualization of the computed centroid of the segmentation skeleton.
+
     :rtype: (float, float, float, dict, np.ndarray)
     """
         img= segmentation_skeleton
         #return compute_angles_dictionary(img)
         angle_dico,centroid = compute_angles_dictionary(img)
         mean_ba = np.mean(list(angle_dico.values()))
         std_ba = np.std(list(angle_dico.values()))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pvbm-2.0.0/PVBM/helpers/branching2.py` & `pvbm-2.1.0/PVBM/helpers/branching2.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.0.0/PVBM/helpers/branching_angle.py` & `pvbm-2.1.0/PVBM/helpers/branching_angle.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.0.0/PVBM/helpers/tortuosity.py` & `pvbm-2.1.0/PVBM/helpers/tortuosity.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.0.0/README.md` & `pvbm-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-2.0.0/pvbm.egg-info/PKG-INFO` & `pvbm-2.1.0/pvbm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.0.0/setup.py` & `pvbm-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='2.0.0',
+    version='2.1.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

