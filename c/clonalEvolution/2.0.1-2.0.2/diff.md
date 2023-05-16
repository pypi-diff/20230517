# Comparing `tmp/clonalEvolution-2.0.1.tar.gz` & `tmp/clonalEvolution-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-2.0.1.tar", last modified: Tue May 16 23:26:35 2023, max compression
+gzip compressed data, was "clonalEvolution-2.0.2.tar", last modified: Tue May 16 23:36:31 2023, max compression
```

## Comparing `clonalEvolution-2.0.1.tar` & `clonalEvolution-2.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.374363 clonalEvolution-2.0.1/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:26:35.374363 clonalEvolution-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.1/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       81 2023-05-16 23:26:35.376341 clonalEvolution-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3866 2023-05-16 23:26:16.000000 clonalEvolution-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.319492 clonalEvolution-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.353403 clonalEvolution-2.0.1/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.1/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    20958 2023-05-16 23:26:07.000000 clonalEvolution-2.0.1/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    24831 2023-05-16 23:16:47.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.1/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    45629 2023-05-16 23:16:28.000000 clonalEvolution-2.0.1/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.1/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.369361 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 23:26:35.000000 clonalEvolution-2.0.1/src/clonalEvolution.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 23:26:35.372351 clonalEvolution-2.0.1/tests/
--rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.1/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.051244 clonalEvolution-2.0.2/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:36:31.052240 clonalEvolution-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.2/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-05-16 23:36:31.053237 clonalEvolution-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-05-16 23:34:18.000000 clonalEvolution-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.004369 clonalEvolution-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.032295 clonalEvolution-2.0.2/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.2/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    21300 2023-05-16 23:35:57.000000 clonalEvolution-2.0.2/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    24831 2023-05-16 23:36:02.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.2/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-16 23:36:11.000000 clonalEvolution-2.0.2/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.2/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.047253 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 23:36:30.000000 clonalEvolution-2.0.2/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 23:36:31.049248 clonalEvolution-2.0.2/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.2/tests/test_simple.py
```

### Comparing `clonalEvolution-2.0.1/LICENSE` & `clonalEvolution-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/PKG-INFO` & `clonalEvolution-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.1
+Version: 2.0.2
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.1/README.md` & `clonalEvolution-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/setup.py` & `clonalEvolution-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="2.0.1",
+    version="2.0.2",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution/__main__.py` & `clonalEvolution-2.0.2/src/clonalEvolution/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,89 +392,94 @@
     pf = np.arange(0,pfx[1],pfx[2])  
     pf[0] = pfx[0]
     if(pfx[0] != pfx[1]):
         pf = np.append(pf,pfx[1])   
     
     if len(pf) == len(ps) and len(ps) == len(f) and len(f) == len(s):
         effects = np.array([s,f,ps,pf])
-        tau,step,ct,pop,cap,kind,path,save,save_p = [0.005,10000,50,1000,1000,0,'',0,0]
+        tau,step,ct,multiply,kind,path,save,save_p = [0.005,10000,50,10,0,'',0,0]
 
         try:
             tau = float(p[int(np.where(p == '-t')[0][0]) + 1])
         except:
             WrongParameter()
         try:
             step = float(p[int(np.where(p == '-s')[0][0]) + 1])
         except:
             WrongParameter()
         try:
             ct = float(p[int(np.where(p == '-ct')[0][0]) + 1])  
         except:
             WrongParameter() 
+        try:
+            multiply = int(p[int(np.where(p == '-x')[0][0]) + 1])  
+        except:
+            WrongParameter() 
         
         kind = 0 + 1*bool(len(p[p=='-binned'])) + 2*bool(len(p[p=='-matrix']))
         path = ''
         save = 16*bool(len(p[p=='-save']))
         save_p = bool(len(p[p=='-save_params']))
         if save or save_p:
             try:
                 path = p[int(np.where(p == '-path')[0][0]) + 1]
             except:
                 print('path is obligatory when saving!')
                 return
         
         percent_max = len(N) * len(s)
         percent = 0
-        for i in N:
-            processes = []
-            pop = i
-            cap = i
-            for sx,fx,psx,pfx in effects.T:
-                percent = percent + 1
-                name = 'single' * (kind == 0) + 'binned' * (kind == 1) + 'matrix' * (kind == 2)
-                pathout = path + '/' + name + '_' + str(i) + '/probability_' + str(psx) + '_' + str(pfx) + '/effect_'  + str(sx) + '_' + str(fx) + '/'
-                params = copy.deepcopy([pop, cap, step, tau, ct, [psx, pfx], [sx, fx], 8])   
-                
-                if save_p:
-                    dfp = pd.DataFrame({
-                            'pop': pop,
-                            'cap': cap,
-                            'steps': step,
-                            'tau': tau,
-                            'skip': ct,
-                            'mut_prob': [[sx, fx]],
-                            'mut_effect': [[psx, pfx]],
-                            'threads': 8
-                        }, index=[0])
-                    
-                    filepath = Path(pathout + '/params'  + ".csv")  
-                    filepath.parent.mkdir(parents=True, exist_ok=True)  
-                    dfp.to_csv(filepath)  
-                pr = 0
-                if kind == 1:
-                    iPop = [[0, pop, 1, 0, [], [], 0]]
-                    pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
-                elif kind == 2:
-                    iPop = [[0, pop, [], [0], sc.sparse.csr_matrix(np.array([[0] for x in range(pop)])), np.ones(pop), 0]]                    
-                    pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
-                else:
-                    iMuts = np.zeros(pop, dtype=np.int64).tolist()
-                    iProp = np.ones(pop).tolist()
-                    iClones = np.zeros(pop, dtype=np.int64).tolist()
-                    iMutations = [[] for x in range(len(iMuts))]
-                    iEffect =[[] for x in range(len(iMuts))]  
+        processes = []
+        for mul in range(multiply):
+            for i in N:                
+                pop = i
+                cap = i
+                for sx,fx,psx,pfx in effects.T:
+                    percent = percent + 1
+                    name = 'single' * (kind == 0) + 'binned' * (kind == 1) + 'matrix' * (kind == 2)
+                    pathout = path + '/' + name + '_' + str(i) + '/probability_' + str(psx) + '_' + str(pfx) + '/effect_'  + str(sx) + '_' + str(fx) + '/'
+                    params = copy.deepcopy([pop, cap, step, tau, ct, [psx, pfx], [sx, fx], 8])   
                     
-                    iPop = np.array([copy.deepcopy(iMuts), copy.deepcopy(iProp), copy.deepcopy(iClones), copy.deepcopy(iMutations), copy.deepcopy(iEffect), copy.deepcopy(iClones)]).T.tolist()
-                    pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
-                    # CEML.clonalEvolutionMainLoop(iPop, params, name, "", pathout, save, -1, None, percent, kind)
-                pr.start()
-                print(str(round(percent/percent_max,3)*100) + '%')
-                processes.append(pr)
-            for pr in processes:
-                pr.join()
+                    if save_p:
+                        dfp = pd.DataFrame({
+                                'pop': pop,
+                                'cap': cap,
+                                'steps': step,
+                                'tau': tau,
+                                'skip': ct,
+                                'mut_prob': [[sx, fx]],
+                                'mut_effect': [[psx, pfx]],
+                                'threads': 8
+                            }, index=[0])
+                        
+                        filepath = Path(pathout + '/params'  + ".csv")  
+                        filepath.parent.mkdir(parents=True, exist_ok=True)  
+                        dfp.to_csv(filepath)  
+                    pr = 0
+                    if kind == 1:
+                        iPop = [[0, pop, 1, 0, [], [], 0]]
+                        pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
+                    elif kind == 2:
+                        iPop = [[0, pop, [], [0], sc.sparse.csr_matrix(np.array([[0] for x in range(pop)])), np.ones(pop), 0]]                    
+                        pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
+                    else:
+                        iMuts = np.zeros(pop, dtype=np.int64).tolist()
+                        iProp = np.ones(pop).tolist()
+                        iClones = np.zeros(pop, dtype=np.int64).tolist()
+                        iMutations = [[] for x in range(len(iMuts))]
+                        iEffect =[[] for x in range(len(iMuts))]  
+                        
+                        iPop = np.array([copy.deepcopy(iMuts), copy.deepcopy(iProp), copy.deepcopy(iClones), copy.deepcopy(iMutations), copy.deepcopy(iEffect), copy.deepcopy(iClones)]).T.tolist()
+                        pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
+                        # CEML.clonalEvolutionMainLoop(iPop, params, name, "", pathout, save, -1, None, percent, kind)
+                    pr.start()
+                    print(str(round(percent/percent_max,3)*100) + '%')
+                    processes.append(pr)
+        for pr in processes:
+            pr.join()
     else:
         print('s, f, ps and pf vectors should be same size')
         
 if __name__ == "__main__":
     p = np.array(sys.argv)
     print(p)
     if(p[p=='--admin']):
```

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_init.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.0.2/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.0.2/src/clonalEvolution/external_plots.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution/mainView.py` & `clonalEvolution-2.0.2/src/clonalEvolution/mainView.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.0.2/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.1
+Version: 2.0.2
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.1/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.0.2/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

