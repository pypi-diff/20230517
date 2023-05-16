# Comparing `tmp/clonalEvolution-2.0.2.tar.gz` & `tmp/clonalEvolution-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-2.0.2.tar", last modified: Tue May 16 23:36:31 2023, max compression
+gzip compressed data, was "clonalEvolution-2.0.3.tar", last modified: Tue May 16 23:39:42 2023, max compression
```

## Comparing `clonalEvolution-2.0.2.tar` & `clonalEvolution-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.051244 clonalEvolution-2.0.2/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:36:31.052240 clonalEvolution-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.2/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       81 2023-05-16 23:36:31.053237 clonalEvolution-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3866 2023-05-16 23:34:18.000000 clonalEvolution-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.004369 clonalEvolution-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.032295 clonalEvolution-2.0.2/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.2/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    21300 2023-05-16 23:35:57.000000 clonalEvolution-2.0.2/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    24831 2023-05-16 23:36:02.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.2/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    45629 2023-05-16 23:36:11.000000 clonalEvolution-2.0.2/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.2/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.047253 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.049248 clonalEvolution-2.0.2/tests/
--rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.2/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.188634 clonalEvolution-2.0.3/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:39:42.188634 clonalEvolution-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.3/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-05-16 23:39:42.190630 clonalEvolution-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-05-16 23:38:47.000000 clonalEvolution-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.140764 clonalEvolution-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.169686 clonalEvolution-2.0.3/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.3/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    21317 2023-05-16 23:39:20.000000 clonalEvolution-2.0.3/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    24831 2023-05-16 23:36:02.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.3/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-16 23:36:11.000000 clonalEvolution-2.0.3/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.3/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.183648 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 23:39:42.000000 clonalEvolution-2.0.3/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 23:39:42.186640 clonalEvolution-2.0.3/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.3/tests/test_simple.py
```

### Comparing `clonalEvolution-2.0.2/LICENSE` & `clonalEvolution-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/PKG-INFO` & `clonalEvolution-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.2
+Version: 2.0.3
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.2/README.md` & `clonalEvolution-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/setup.py` & `clonalEvolution-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="2.0.2",
+    version="2.0.3",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution/__main__.py` & `clonalEvolution-2.0.3/src/clonalEvolution/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,15 @@
         for mul in range(multiply):
             for i in N:                
                 pop = i
                 cap = i
                 for sx,fx,psx,pfx in effects.T:
                     percent = percent + 1
                     name = 'single' * (kind == 0) + 'binned' * (kind == 1) + 'matrix' * (kind == 2)
-                    pathout = path + '/' + name + '_' + str(i) + '/probability_' + str(psx) + '_' + str(pfx) + '/effect_'  + str(sx) + '_' + str(fx) + '/'
+                    pathout = path + '/' + str(mul) + '_' + name + '_' + str(i) + '/probability_' + str(psx) + '_' + str(pfx) + '/effect_'  + str(sx) + '_' + str(fx) + '/'
                     params = copy.deepcopy([pop, cap, step, tau, ct, [psx, pfx], [sx, fx], 8])   
                     
                     if save_p:
                         dfp = pd.DataFrame({
                                 'pop': pop,
                                 'cap': cap,
                                 'steps': step,
```

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_init.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.0.3/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.0.3/src/clonalEvolution/external_plots.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution/mainView.py` & `clonalEvolution-2.0.3/src/clonalEvolution/mainView.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.0.3/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.2
+Version: 2.0.3
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.2/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.0.3/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

