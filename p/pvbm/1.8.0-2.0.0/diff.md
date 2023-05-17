# Comparing `tmp/pvbm-1.8.0.tar.gz` & `tmp/pvbm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-1.8.0.tar", last modified: Thu May  4 16:47:14 2023, max compression
+gzip compressed data, was "pvbm-2.0.0.tar", last modified: Wed May 17 14:53:31 2023, max compression
```

## Comparing `pvbm-1.8.0.tar` & `pvbm-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.058326 pvbm-1.8.0/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-05-04 16:47:14.058161 pvbm-1.8.0/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.055688 pvbm-1.8.0/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    10404 2023-04-13 10:09:55.000000 pvbm-1.8.0/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5257 2023-04-30 12:10:25.000000 pvbm-1.8.0/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-1.8.0/PVBM/__init__.py
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.056993 pvbm-1.8.0/PVBM/helpers/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-1.8.0/PVBM/helpers/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-1.8.0/PVBM/helpers/branching2.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     8674 2023-04-30 12:24:25.000000 pvbm-1.8.0/PVBM/helpers/branching_angle.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-1.8.0/PVBM/helpers/tortuosity.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1007 2023-04-30 13:59:40.000000 pvbm-1.8.0/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.057934 pvbm-1.8.0/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      337 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-04 16:47:14.058365 pvbm-1.8.0/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-04 16:47:00.000000 pvbm-1.8.0/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.515562 pvbm-2.0.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 14:53:31.515427 pvbm-2.0.0/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.513067 pvbm-2.0.0/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    11131 2023-05-17 14:49:51.000000 pvbm-2.0.0/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4602 2023-05-17 14:44:47.000000 pvbm-2.0.0/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.0.0/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.514278 pvbm-2.0.0/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.0.0/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.0.0/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     8674 2023-04-30 12:24:25.000000 pvbm-2.0.0/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.0.0/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     3799 2023-05-17 14:52:46.000000 pvbm-2.0.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 14:53:31.515233 pvbm-2.0.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      337 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-17 14:53:31.000000 pvbm-2.0.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-17 14:53:31.515609 pvbm-2.0.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-17 14:53:23.000000 pvbm-2.0.0/setup.py
```

### Comparing `pvbm-1.8.0/PVBM/GeometricalAnalysis.py` & `pvbm-2.0.0/PVBM/GeometricalAnalysis.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,95 +3,86 @@
 from scipy.signal import convolve2d
 from PVBM.helpers.tortuosity import compute_tortuosity
 #from PVBM.helpers.perimeter import compute_perimeter
 from PVBM.helpers.branching_angle import compute_angles_dictionary
 #from PVBM.helpers.far import far
 
 class GeometricalVBMs:
-    """A class which holds all required methods to perform
-        geometrical biomarker computation.
+    """A class that can perform geometrical biomarker computation for a fundus image.
     """
 
     def area(self,segmentation):
-        """This function compute the overall area of the segmentation.
-
-        :param array segmentation: The segmentation is an two-dimensional array (HxW) with binary value (0 or 1).
-        :returns: The area of the segmentation
-
-        :rtype: float
         """
+    This function computes the area of the blood vessels calculated as the total number of pixels in the segmentation, 
+    and is expressed in pixels^2 (squared pixels).
+
+    :param segmentation: The segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
+    :type segmentation: array
+    :return: The area of the segmentation.
+    :rtype: float
+    """
         return np.sum(segmentation)
     
     def compute_particular_points(self,segmentation_skeleton):
         """
-        This function compute the number of endpoints and intersection points of the segmentation.
+    The particular point is the union between the endpoints and the intersection points.
+    This function computes the number of endpoints and intersection points of the fundus image vasculature segmentation.
 
-        :param np.ndarray segmentation_skeleton: The skeleton of the segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
-        :returns int end_points_count: The number of endpoints 
-        :returns int inter_points_count: The number of intersection points 
-        :returns np.ndarray end_points: An array where the value at the position (i,j) is True if the pixel is an endpoint, False otherwise
-        :returns np.ndarray inter_points: An array where the value at the position (i,j) is True if the pixel is an intersection point, False otherwise
-        :rtype: (int, int, np.ndarray, np.ndarray)
-        """
+    :param segmentation_skeleton: The skeleton of the segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
+    :type segmentation_skeleton: np.ndarray
+    :return: The number of endpoints, the number of intersection points, an array with endpoint pixel positions, and an array with intersection point pixel positions.
+    :rtype: (int, int, np.ndarray, np.ndarray)
+    """
         filter_ = np.array([[1, 1, 1], [1, 10, 1], [1, 1, 1]])
         neighbours = convolve2d(segmentation_skeleton, filter_, mode="same")
 
         end_points = neighbours == 11
         inter_points = neighbours >= 13
 
         end_points_count = np.sum(end_points)
         inter_points_count = np.sum(inter_points)
 
         return end_points_count, inter_points_count, end_points, inter_points
     
     def compute_tortuosity_length(self,segmentation_skeleton):
-        """This function compute the median tortuosity and the lengh of the segmentation.
-
-        :param array segmentation_skeleton: The skeleton of the segmentation is an two-dimensional array (HxW) with binary value (0 or 1).
-        :returns float median_tor: The median tortuosity
-        :returns float length: The overall normalized length 
-        :returns list tor: A list containing the arc-chord ratio of every blood vessels (between two particular points).
-        :returns list l: A list containing the non normalized length of every blood vessels (between two particular points).
-        :returns dictionary connection_dico: A dictionnary containing in key some particular points and in value the list of the particular points connected to him, with their length. This dictionnary was build by navigating through the skeleton. 
-
-        :rtype: (float,float,List,List,Dictionary)
         """
+    This function computes the median tortuosity and the length of the fundus image vasculature segmentation.
+    :param segmentation_skeleton: The skeleton of the segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
+    :type segmentation_skeleton: np.ndarray
+    :return: The median tortuosity, overall length (in pixel), a list of chord distance of each blood vessel (in pixel), a list of lengths distance (arc) of each blood vessel (in pixel), and a dictionary with connection information.
+    :rtype: (float, float, list, list, dict)
+    """
         median_tor,length,tor,l,connection_dico = compute_tortuosity(segmentation_skeleton)
         return median_tor,length ,tor,l,connection_dico
 
     def compute_perimeter(self,segmentation):
-        """This function compute the perimeter and the border of the segmentation.
-
-            :param array segmentation: The segmentation is an two-dimensional array (HxW) with binary value (0 or 1).
-            :returns float perim: The perimeter
-            :returns NumpyArray border: The matrix containing the edges of the segmentation.
-            :rtype: (float,NumpyArray)
         """
+    This function computes the perimeter and the border of the fundus image vasculature segmentation.
+
+    :param segmentation: The segmentation is a two-dimensional array (HxW) with binary value (0 or 1).
+    :type segmentation: np.ndarray
+    :return: The perimeter (in pixel) and a matrix containing the edges of the segmentation.
+    :rtype: (float, np.ndarray)
+    """
         filter_ = np.array([[-1, -1, -1], [-1, 8, -1], [-1, -1, -1]])
         derivative = convolve2d(segmentation,filter_, mode="same")
         border = derivative>0
         segmentation_skeleton = skeletonize(np.ascontiguousarray(border.T)).T
         _,perim,_,_,_ = compute_tortuosity(segmentation_skeleton)
         return perim,segmentation_skeleton.T
     
     def compute_branching_angles(self,segmentation_skeleton):
-        """This function compute the mean, std and median branching angle of the segmentation.
-
-            :param array segmentation_skeleton: The skeleton of the segmentation is an two-dimensional array (HxW) with binary value (0 or 1).
-            :returns float mean_ba: The mean branching angles
-            :returns float std_ba: The std branching angles
-            :returns float median_ba: The median branching angles
-            :returns dictionary angle_dico: A dictionnary containing all the branching angles
-            :returns NumpyArray centroid: A numpy array containing a visualisation of the computed centroid
-
-            :rtype: (int,int)
         """
-        #img_tmp = np.zeros((segmentation_skeleton.shape[0]+20,segmentation_skeleton.shape[0]+20)) #np.zeros((segmentation_skeleton.shape[0]+20,segmentation_skeleton.shape[0]+20)) 
-        #img_tmp[10:-10,10:-10] = segmentation_skeleton
+    This function computes the mean, standard deviation, and median branching angle of the fundus image vasculature segmentation.
 
+    :param segmentation_skeleton: The skeleton of the segmentation is a two-dimensional array (HxW) with binary values (0 or 1).
+    :type segmentation_skeleton: np.ndarray
+    :return: The mean branching angles (°), the standard deviation of branching angles (°), the median branching angles (°), a dictionary containing all the branching angles, and a numpy array with a visualization of the computed centroid.
+    :rtype: (float, float, float, dict, np.ndarray)
+    """
         img= segmentation_skeleton
         #return compute_angles_dictionary(img)
         angle_dico,centroid = compute_angles_dictionary(img)
         mean_ba = np.mean(list(angle_dico.values()))
         std_ba = np.std(list(angle_dico.values()))
         median_ba = np.median(list(angle_dico.values()))
         return mean_ba, std_ba, median_ba,angle_dico,centroid
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pvbm-1.8.0/PVBM/helpers/branching2.py` & `pvbm-2.0.0/PVBM/helpers/branching2.py`

 * *Files identical despite different names*

### Comparing `pvbm-1.8.0/PVBM/helpers/branching_angle.py` & `pvbm-2.0.0/PVBM/helpers/branching_angle.py`

 * *Files identical despite different names*

### Comparing `pvbm-1.8.0/PVBM/helpers/tortuosity.py` & `pvbm-2.0.0/PVBM/helpers/tortuosity.py`

 * *Files identical despite different names*

### Comparing `pvbm-1.8.0/setup.py` & `pvbm-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='1.8.0',
+    version='2.0.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

