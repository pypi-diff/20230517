# Comparing `tmp/clonalEvolution-2.0.0.tar.gz` & `tmp/clonalEvolution-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-2.0.0.tar", last modified: Tue May 16 23:18:12 2023, max compression
+gzip compressed data, was "clonalEvolution-2.0.1.tar", last modified: Tue May 16 23:26:35 2023, max compression
```

## Comparing `clonalEvolution-2.0.0.tar` & `clonalEvolution-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.170106 clonalEvolution-2.0.0/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:18:12.170106 clonalEvolution-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.0/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       81 2023-05-16 23:18:12.172101 clonalEvolution-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3866 2023-05-16 23:17:51.000000 clonalEvolution-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.109270 clonalEvolution-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.144177 clonalEvolution-2.0.0/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.0/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    21156 2023-05-16 23:16:36.000000 clonalEvolution-2.0.0/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    24831 2023-05-16 23:16:47.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.0/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    45629 2023-05-16 23:16:28.000000 clonalEvolution-2.0.0/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.0/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.164124 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.167116 clonalEvolution-2.0.0/tests/
--rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.0/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.374363 clonalEvolution-2.0.1/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:26:35.374363 clonalEvolution-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.1/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-05-16 23:26:35.376341 clonalEvolution-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-05-16 23:26:16.000000 clonalEvolution-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.319492 clonalEvolution-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.353403 clonalEvolution-2.0.1/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.1/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    20958 2023-05-16 23:26:07.000000 clonalEvolution-2.0.1/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    24831 2023-05-16 23:16:47.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.1/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-16 23:16:28.000000 clonalEvolution-2.0.1/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.1/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.369361 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.372351 clonalEvolution-2.0.1/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.1/tests/test_simple.py
```

### Comparing `clonalEvolution-2.0.0/LICENSE` & `clonalEvolution-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/PKG-INFO` & `clonalEvolution-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.0
+Version: 2.0.1
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.0/README.md` & `clonalEvolution-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/setup.py` & `clonalEvolution-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="2.0.0",
+    version="2.0.1",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution/__main__.py` & `clonalEvolution-2.0.1/src/clonalEvolution/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,22 +406,15 @@
             step = float(p[int(np.where(p == '-s')[0][0]) + 1])
         except:
             WrongParameter()
         try:
             ct = float(p[int(np.where(p == '-ct')[0][0]) + 1])  
         except:
             WrongParameter() 
-        try:
-            pop = int(p[int(np.where(p == '-pop')[0][0]) + 1])
-        except:
-            WrongParameter()
-        try:
-            cap = int(p[int(np.where(p == '-cap')[0][0]) + 1])
-        except:
-            WrongParameter()
+        
         kind = 0 + 1*bool(len(p[p=='-binned'])) + 2*bool(len(p[p=='-matrix']))
         path = ''
         save = 16*bool(len(p[p=='-save']))
         save_p = bool(len(p[p=='-save_params']))
         if save or save_p:
             try:
                 path = p[int(np.where(p == '-path')[0][0]) + 1]
@@ -429,14 +422,16 @@
                 print('path is obligatory when saving!')
                 return
         
         percent_max = len(N) * len(s)
         percent = 0
         for i in N:
             processes = []
+            pop = i
+            cap = i
             for sx,fx,psx,pfx in effects.T:
                 percent = percent + 1
                 name = 'single' * (kind == 0) + 'binned' * (kind == 1) + 'matrix' * (kind == 2)
                 pathout = path + '/' + name + '_' + str(i) + '/probability_' + str(psx) + '_' + str(pfx) + '/effect_'  + str(sx) + '_' + str(fx) + '/'
                 params = copy.deepcopy([pop, cap, step, tau, ct, [psx, pfx], [sx, fx], 8])   
                 
                 if save_p:
```

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_init.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.0.1/src/clonalEvolution/external_plots.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution/mainView.py` & `clonalEvolution-2.0.1/src/clonalEvolution/mainView.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.0.1/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.0
+Version: 2.0.1
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.0/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.0.1/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

