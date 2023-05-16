# Comparing `tmp/clonalEvolution-2.0.3.tar.gz` & `tmp/clonalEvolution-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-2.0.3.tar", last modified: Tue May 16 23:39:42 2023, max compression
+gzip compressed data, was "clonalEvolution-2.0.4.tar", last modified: Tue May 16 23:46:28 2023, max compression
```

## Comparing `clonalEvolution-2.0.3.tar` & `clonalEvolution-2.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.188634 clonalEvolution-2.0.3/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:39:42.188634 clonalEvolution-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.3/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       81 2023-05-16 23:39:42.190630 clonalEvolution-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3866 2023-05-16 23:38:47.000000 clonalEvolution-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.140764 clonalEvolution-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.169686 clonalEvolution-2.0.3/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.3/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    21317 2023-05-16 23:39:20.000000 clonalEvolution-2.0.3/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    24831 2023-05-16 23:36:02.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.3/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    45629 2023-05-16 23:36:11.000000 clonalEvolution-2.0.3/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.3/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.183648 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.186640 clonalEvolution-2.0.3/tests/
--rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.3/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:46:28.245554 clonalEvolution-2.0.4/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:46:28.245554 clonalEvolution-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.4/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-05-16 23:46:28.247073 clonalEvolution-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-05-16 23:46:07.000000 clonalEvolution-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:46:28.196686 clonalEvolution-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 23:46:28.225607 clonalEvolution-2.0.4/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.4/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    21317 2023-05-16 23:39:20.000000 clonalEvolution-2.0.4/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    25157 2023-05-16 23:45:49.000000 clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.4/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-16 23:36:11.000000 clonalEvolution-2.0.4/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.4/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:46:28.240567 clonalEvolution-2.0.4/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:46:28.000000 clonalEvolution-2.0.4/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-16 23:46:28.000000 clonalEvolution-2.0.4/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 23:46:28.000000 clonalEvolution-2.0.4/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-16 23:46:28.000000 clonalEvolution-2.0.4/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-16 23:46:28.000000 clonalEvolution-2.0.4/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 23:46:28.000000 clonalEvolution-2.0.4/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 23:46:28.243561 clonalEvolution-2.0.4/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.4/tests/test_simple.py
```

### Comparing `clonalEvolution-2.0.3/LICENSE` & `clonalEvolution-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/PKG-INFO` & `clonalEvolution-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.3
+Version: 2.0.4
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.3/README.md` & `clonalEvolution-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/setup.py` & `clonalEvolution-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="2.0.3",
+    version="2.0.4",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution/__main__.py` & `clonalEvolution-2.0.4/src/clonalEvolution/__main__.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,14 +398,15 @@
             16 - ack to save data
         t_iter - value of starting iteration (for resume t_iter != 0)
         q - queue to comunicate with simulation in thread
         ID - simulation ID
         select - 0 normal, 1 binned
     """
     global end
+    pop = params[0]
     cap = params[1]
     steps = params[2]
     tau = params[3]
     skip = params[4]
     mut_effect = params[6]
     mut_prob = params[5]   
     threads = params[7]
@@ -509,17 +510,26 @@
             else:
                 FILE = open(file_localization + '/' + "report/"  + file_name + "_report_" + str(ID) + ".txt", 'a')
                 FILE.write(str(ID) + ',' + str(tx) + ',' + str(CPU) + ',' + str(mem))
                 FILE.write('\n')
                 FILE.close()
             tx = time.time()
                 
-        if iter_outer % steps == 0 and iter_outer > 0:
+        if (iter_outer % steps == 0 and iter_outer > 0):
             print('simulation ended, ID: %i' % ID)
             break
+        if select == 0: 
+            if(len(iPop)) >= 10*pop:
+                break
+        elif select == 1:
+            if(sum([row[1] for row in iPop])) >= 10*pop:
+                break
+        elif select == 2:
+            if(sum([row[1] for row in iPop])) >= 10*pop:
+                break
         
         if select == 0:            
             iPop = CEL.clonalEvolutionLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads)
         elif select == 1:
             iPop = CEBL.clonalEvolutionBinnedLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads, print_time)
         elif select == 2:
             iPop = CECML.clonalEvolutionCloneMatrixLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads, print_time)
```

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.0.4/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.0.4/src/clonalEvolution/external_plots.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution/mainView.py` & `clonalEvolution-2.0.4/src/clonalEvolution/mainView.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.0.4/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.3
+Version: 2.0.4
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.3/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.0.4/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

