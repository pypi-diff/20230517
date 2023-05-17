# Comparing `tmp/pvbm-2.1.1.tar.gz` & `tmp/pvbm-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-2.1.1.tar", last modified: Wed May 17 15:46:55 2023, max compression
+gzip compressed data, was "pvbm-2.1.2.tar", last modified: Wed May 17 15:49:29 2023, max compression
```

## Comparing `pvbm-2.1.1.tar` & `pvbm-2.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:46:55.332191 pvbm-2.1.1/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 15:46:55.332007 pvbm-2.1.1/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:46:55.329506 pvbm-2.1.1/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    11131 2023-05-17 15:14:40.000000 pvbm-2.1.1/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4909 2023-05-17 15:12:06.000000 pvbm-2.1.1/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.1/PVBM/__init__.py
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:46:55.330491 pvbm-2.1.1/PVBM/helpers/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.1/PVBM/helpers/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.1.1/PVBM/helpers/branching2.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     6297 2023-05-17 15:46:28.000000 pvbm-2.1.1/PVBM/helpers/branching_angle.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.1.1/PVBM/helpers/tortuosity.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     3799 2023-05-17 14:52:46.000000 pvbm-2.1.1/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:46:55.331721 pvbm-2.1.1/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 15:46:55.000000 pvbm-2.1.1/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      337 2023-05-17 15:46:55.000000 pvbm-2.1.1/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-17 15:46:55.000000 pvbm-2.1.1/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-17 15:46:55.000000 pvbm-2.1.1/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-17 15:46:55.000000 pvbm-2.1.1/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-17 15:46:55.332244 pvbm-2.1.1/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-17 15:46:47.000000 pvbm-2.1.1/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:49:29.543917 pvbm-2.1.2/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 15:49:29.543804 pvbm-2.1.2/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:49:29.542018 pvbm-2.1.2/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    11131 2023-05-17 15:14:40.000000 pvbm-2.1.2/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4909 2023-05-17 15:12:06.000000 pvbm-2.1.2/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.2/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:49:29.542847 pvbm-2.1.2/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.2/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.1.2/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:49:11.000000 pvbm-2.1.2/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.1.2/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     3799 2023-05-17 14:52:46.000000 pvbm-2.1.2/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-17 15:49:29.543638 pvbm-2.1.2/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4061 2023-05-17 15:49:29.000000 pvbm-2.1.2/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      337 2023-05-17 15:49:29.000000 pvbm-2.1.2/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-17 15:49:29.000000 pvbm-2.1.2/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-17 15:49:29.000000 pvbm-2.1.2/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-17 15:49:29.000000 pvbm-2.1.2/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-17 15:49:29.543952 pvbm-2.1.2/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-17 15:49:19.000000 pvbm-2.1.2/setup.py
```

### Comparing `pvbm-2.1.1/PKG-INFO` & `pvbm-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.1.1/PVBM/FractalAnalysis.py` & `pvbm-2.1.2/PVBM/FractalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.1/PVBM/GeometricalAnalysis.py` & `pvbm-2.1.2/PVBM/GeometricalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.1/PVBM/helpers/branching2.py` & `pvbm-2.1.2/PVBM/helpers/branching2.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.1/PVBM/helpers/branching_angle.py` & `pvbm-2.1.2/PVBM/helpers/branching_angle.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         for j in range(final_eroded.shape[1]):
             if final_eroded[i,j] == True:
                 origin_points.append((i,j))
     return origin_points
 
 def iterative(i,j,skeleton,origin_points,visited,dist,distance_dictionnary):
     pq = PriorityQueue()
-    pq.put((0, i_or, j_or, i_or, j_or,0))
+    pq.put((0, i, j, i, j,0))
     priotities = [0,1,2,3,4,5,6,7]
     while not pq.empty():
         _, i_or, j_or, i, j,dist = pq.get()
         directions = [(i-1,j),(i+1,j),(i,j-1),(i,j+1),(i-1,j-1),(i-1,j+1),(i+1,j-1),(i+1,j+1)]
         for direction,priority in zip(directions,priotities):
           x,y = direction
           if x >= 0 and x < skeleton.shape[0] and y >= 0 and y < skeleton.shape[1] and visited[direction] == 0:
```

### Comparing `pvbm-2.1.1/PVBM/helpers/tortuosity.py` & `pvbm-2.1.2/PVBM/helpers/tortuosity.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.1/README.md` & `pvbm-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.1/pvbm.egg-info/PKG-INFO` & `pvbm-2.1.2/pvbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.1.1/setup.py` & `pvbm-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='2.1.1',
+    version='2.1.2',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

