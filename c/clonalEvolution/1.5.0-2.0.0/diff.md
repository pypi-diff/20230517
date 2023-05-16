# Comparing `tmp/clonalEvolution-1.5.0.tar.gz` & `tmp/clonalEvolution-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-1.5.0.tar", last modified: Mon Nov 14 12:48:24 2022, max compression
+gzip compressed data, was "clonalEvolution-2.0.0.tar", last modified: Tue May 16 23:18:12 2023, max compression
```

## Comparing `clonalEvolution-1.5.0.tar` & `clonalEvolution-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 12:48:23.830000 clonalEvolution-1.5.0/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     5378 2022-11-14 12:48:26.000000 clonalEvolution-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-1.5.0/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       81 2022-11-14 12:48:26.000000 clonalEvolution-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3865 2022-11-14 12:36:34.000000 clonalEvolution-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-14 12:48:23.870000 clonalEvolution-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-14 12:48:23.920000 clonalEvolution-1.5.0/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-1.5.0/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    15503 2022-11-12 23:28:20.000000 clonalEvolution-1.5.0/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-11-13 09:30:36.000000 clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    24416 2022-11-14 12:30:22.000000 clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32298 2022-11-14 12:47:46.000000 clonalEvolution-1.5.0/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    46062 2022-11-14 12:35:58.000000 clonalEvolution-1.5.0/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-1.5.0/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2022-11-14 12:48:23.960000 clonalEvolution-1.5.0/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2022-11-14 12:48:24.000000 clonalEvolution-1.5.0/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2022-11-14 12:48:24.000000 clonalEvolution-1.5.0/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 12:48:24.000000 clonalEvolution-1.5.0/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-11-14 12:48:24.000000 clonalEvolution-1.5.0/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2022-11-14 12:48:24.000000 clonalEvolution-1.5.0/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-11-14 12:48:24.000000 clonalEvolution-1.5.0/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.170106 clonalEvolution-2.0.0/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:18:12.170106 clonalEvolution-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.0/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-05-16 23:18:12.172101 clonalEvolution-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-05-16 23:17:51.000000 clonalEvolution-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.109270 clonalEvolution-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.144177 clonalEvolution-2.0.0/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.0/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    21156 2023-05-16 23:16:36.000000 clonalEvolution-2.0.0/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    24831 2023-05-16 23:16:47.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32529 2023-05-16 08:25:54.000000 clonalEvolution-2.0.0/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-16 23:16:28.000000 clonalEvolution-2.0.0/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.0/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.164124 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 23:18:12.000000 clonalEvolution-2.0.0/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 23:18:12.167116 clonalEvolution-2.0.0/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.0/tests/test_simple.py
```

### Comparing `clonalEvolution-1.5.0/LICENSE` & `clonalEvolution-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-1.5.0/PKG-INFO` & `clonalEvolution-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 1.5.0
+Version: 2.0.0
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-1.5.0/README.md` & `clonalEvolution-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-1.5.0/setup.py` & `clonalEvolution-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="1.5.0",
+    version="2.0.0",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
@@ -68,15 +68,15 @@
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
     entry_points={ 
         "console_scripts": [
-            "clonaEvolution=__main__:main",
+            "clonalEvolution=__main__:main",
         ],
     },
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
```

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution/__main__.py` & `clonalEvolution-2.0.0/src/clonalEvolution/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import sys
 import os
 import copy
 from pathlib import Path
 import numpy as np
 import pandas as pd
 import scipy as sc
+from multiprocessing import Process
 
 import clonalEvolution.clonal_evolution_init as CEML
 import clonalEvolution.external_plots as external_plots
 from clonalEvolution.mainView import run
 
+# import clonal_evolution_init as CEML
+# import external_plots as external_plots
+# from mainView import run
+
 disclaimer = '''Cellular/Microbial Clonal Evolution simulations basing on Gillespie algorithm. Copyright (C) 2022 by Jarosław Gil. 
     This program comes with ABSOLUTELY NO WARRANTY.
     This is free software, and you are welcome to redistribute it
     under certain conditions.'''
 
+class WrongParameter(Exception):
+    pass
+
 def loadPaths(fname):        
     # self.showDialog("Select file same as resume simulation", "Info")
     xname = fname.split('/')
     
     ##TODO interpret only last number!!!
     
     path = ""
@@ -347,11 +355,134 @@
                                                        copy.deepcopy(iProp), 
                                                        copy.deepcopy(iClones), 
                                                        copy.deepcopy(iMutations), 
                                                        copy.deepcopy(iEffect),
                                                        copy.deepcopy(iClones)]).T.tolist(), 
                                              copy.deepcopy([dfp['pop'][0], dfp['cap'][0], dfp['steps'][0], dfp['tau'][0], dfp['skip'][0], dfp['mut_prob'][0], dfp['mut_effect'][0], dfp['threads'][0]]), 
                                              name, "", output, plots, select=0)              
-                                         
-            
+
+def adminMode():
+    p = np.array(sys.argv)
+    N = p[int(np.where(p == '-N')[0][0]) + 1]        
+    N = np.array(list(map(lambda x: int(x), N.split(','))))   
+    N = 10**np.array(range(N[0],N[1]+1,N[2]))     
+
+    s = p[int(np.where(p == '-S')[0][0]) + 1]        
+    sx = np.array(list(map(lambda x: float(x), s.split(','))))   
+    s = np.arange(0,sx[1],sx[2])  
+    s[0] = sx[0]
+    if(sx[0] != sx[1]):
+        s = np.append(s,sx[1])                 
+        
+    f = p[int(np.where(p == '-F')[0][0]) + 1]        
+    fx = np.array(list(map(lambda x: float(x), f.split(','))))   
+    f = np.arange(0,fx[1],fx[2])  
+    f[0] = fx[0]
+    if(fx[0] != fx[1]):
+        f = np.append(f,fx[1])          
+
+    ps = p[int(np.where(p == '-PS')[0][0]) + 1]        
+    psx = np.array(list(map(lambda x: float(x), ps.split(','))))   
+    ps = np.arange(0,psx[1],psx[2])  
+    ps[0] = psx[0]
+    if(psx[0] != psx[1]):
+        ps = np.append(ps,psx[1])                 
+        
+    pf = p[int(np.where(p == '-PF')[0][0]) + 1]        
+    pfx = np.array(list(map(lambda x: float(x), pf.split(','))))   
+    pf = np.arange(0,pfx[1],pfx[2])  
+    pf[0] = pfx[0]
+    if(pfx[0] != pfx[1]):
+        pf = np.append(pf,pfx[1])   
+    
+    if len(pf) == len(ps) and len(ps) == len(f) and len(f) == len(s):
+        effects = np.array([s,f,ps,pf])
+        tau,step,ct,pop,cap,kind,path,save,save_p = [0.005,10000,50,1000,1000,0,'',0,0]
+
+        try:
+            tau = float(p[int(np.where(p == '-t')[0][0]) + 1])
+        except:
+            WrongParameter()
+        try:
+            step = float(p[int(np.where(p == '-s')[0][0]) + 1])
+        except:
+            WrongParameter()
+        try:
+            ct = float(p[int(np.where(p == '-ct')[0][0]) + 1])  
+        except:
+            WrongParameter() 
+        try:
+            pop = int(p[int(np.where(p == '-pop')[0][0]) + 1])
+        except:
+            WrongParameter()
+        try:
+            cap = int(p[int(np.where(p == '-cap')[0][0]) + 1])
+        except:
+            WrongParameter()
+        kind = 0 + 1*bool(len(p[p=='-binned'])) + 2*bool(len(p[p=='-matrix']))
+        path = ''
+        save = 16*bool(len(p[p=='-save']))
+        save_p = bool(len(p[p=='-save_params']))
+        if save or save_p:
+            try:
+                path = p[int(np.where(p == '-path')[0][0]) + 1]
+            except:
+                print('path is obligatory when saving!')
+                return
+        
+        percent_max = len(N) * len(s)
+        percent = 0
+        for i in N:
+            processes = []
+            for sx,fx,psx,pfx in effects.T:
+                percent = percent + 1
+                name = 'single' * (kind == 0) + 'binned' * (kind == 1) + 'matrix' * (kind == 2)
+                pathout = path + '/' + name + '_' + str(i) + '/probability_' + str(psx) + '_' + str(pfx) + '/effect_'  + str(sx) + '_' + str(fx) + '/'
+                params = copy.deepcopy([pop, cap, step, tau, ct, [psx, pfx], [sx, fx], 8])   
+                
+                if save_p:
+                    dfp = pd.DataFrame({
+                            'pop': pop,
+                            'cap': cap,
+                            'steps': step,
+                            'tau': tau,
+                            'skip': ct,
+                            'mut_prob': [[sx, fx]],
+                            'mut_effect': [[psx, pfx]],
+                            'threads': 8
+                        }, index=[0])
+                    
+                    filepath = Path(pathout + '/params'  + ".csv")  
+                    filepath.parent.mkdir(parents=True, exist_ok=True)  
+                    dfp.to_csv(filepath)  
+                pr = 0
+                if kind == 1:
+                    iPop = [[0, pop, 1, 0, [], [], 0]]
+                    pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
+                elif kind == 2:
+                    iPop = [[0, pop, [], [0], sc.sparse.csr_matrix(np.array([[0] for x in range(pop)])), np.ones(pop), 0]]                    
+                    pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
+                else:
+                    iMuts = np.zeros(pop, dtype=np.int64).tolist()
+                    iProp = np.ones(pop).tolist()
+                    iClones = np.zeros(pop, dtype=np.int64).tolist()
+                    iMutations = [[] for x in range(len(iMuts))]
+                    iEffect =[[] for x in range(len(iMuts))]  
+                    
+                    iPop = np.array([copy.deepcopy(iMuts), copy.deepcopy(iProp), copy.deepcopy(iClones), copy.deepcopy(iMutations), copy.deepcopy(iEffect), copy.deepcopy(iClones)]).T.tolist()
+                    pr = (Process(target=CEML.clonalEvolutionMainLoop, args=(iPop, params, name, "", pathout, save, -1, None, percent, kind)))
+                    # CEML.clonalEvolutionMainLoop(iPop, params, name, "", pathout, save, -1, None, percent, kind)
+                pr.start()
+                print(str(round(percent/percent_max,3)*100) + '%')
+                processes.append(pr)
+            for pr in processes:
+                pr.join()
+    else:
+        print('s, f, ps and pf vectors should be same size')
+        
 if __name__ == "__main__":
-    main()
+    p = np.array(sys.argv)
+    print(p)
+    if(p[p=='--admin']):
+        adminMode()
+    else:
+        main()
```

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,32 @@
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 '''
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy as sc
+import psutil
 import time
 import os
 import copy
 import pandas as pd
 from pathlib import Path  
 from threading import Thread
 
 import clonalEvolution.clonal_evolution_binned_loop as CEBL
 import clonalEvolution.clonal_evolution_clone_matrix_loop as CECML
 import clonalEvolution.clonal_evolution_loop as CEL
 import clonalEvolution.wmean as wm
 
+# import clonal_evolution_binned_loop as CEBL
+# import clonal_evolution_clone_matrix_loop as CECML
+# import clonal_evolution_loop as CEL
+# import wmean as wm
+
 end = False
     
 def waveMut_ar(iMuts, iClones, cln):
     muts = iMuts
     clones = iClones
     m_u = []
     c_u = []
@@ -485,25 +491,28 @@
 
         if end:
             break
 
         print_time = not iter_inner % round(cycle/skip)   
         if print_time and plots & 16:
             tx = time.time() - tx
+            p = psutil.Process()
+            mem = p.memory_percent()
+            CPU = p.cpu_percent()
             if not os.path.exists(file_localization + '/' + "report/"  + file_name + "_report_" + str(ID) + ".txt"):
                 os.makedirs(file_localization + '/' + "report/", exist_ok=True)
                 FILE = open(file_localization + '/' + "report/"  + file_name + "_report_" + str(ID) + ".txt", 'w')
                 FILE.write("threads: %i" % threads)
                 FILE.write('\n')
-                FILE.write(str(ID) + ',' + str(tx))
+                FILE.write(str(ID) + ',' + str(tx) + ',' + str(CPU) + ',' + str(mem))
                 FILE.write('\n')
                 FILE.close()
             else:
                 FILE = open(file_localization + '/' + "report/"  + file_name + "_report_" + str(ID) + ".txt", 'a')
-                FILE.write(str(ID) + ',' + str(tx))
+                FILE.write(str(ID) + ',' + str(tx) + ',' + str(CPU) + ',' + str(mem))
                 FILE.write('\n')
                 FILE.close()
             tx = time.time()
                 
         if iter_outer % steps == 0 and iter_outer > 0:
             print('simulation ended, ID: %i' % ID)
             break
@@ -513,9 +522,11 @@
         elif select == 1:
             iPop = CEBL.clonalEvolutionBinnedLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads, print_time)
         elif select == 2:
             iPop = CECML.clonalEvolutionCloneMatrixLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads, print_time)
             
         resume = 0
         iter_inner = iter_inner + 1
-            
-    q.put(['ended', ID])
+    if q!= None:        
+        q.put(['ended', ID])
+    else:
+        print('ended: ' + str(ID))
```

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.0.0/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.0.0/src/clonalEvolution/external_plots.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 import numpy as np
 import os
 from pathlib import Path
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import scipy as sc
 
-def clonePlot(paths_in, paths_out, ids):
+def clonePlot(paths_in, ids):
     prop = np.transpose([paths_in, ids])
     for path_in, _id in prop:     
         
-        os.chdir(paths_out)
-        path_out = paths_out + '/Figures/' + _id + '/'
+        path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/' + _id +'/'
             
         df = []
         if path_in.endswith('.csv'):
             df = pd.read_csv(path_in)
         elif path_in.endswith('.txt'):
             df = loadFile(path_in)
         elif path_in.endswith('.mtx'):
@@ -87,16 +86,15 @@
         
 def mutWavePlot(paths_in, paths_out, ids):
     prop = np.transpose([paths_in, ids])
     print("mutation")
     print(prop)
     for path_in, _id in prop:
         
-        os.chdir(paths_out)
-        path_out = paths_out + '/Figures/' + _id + '/'
+        path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/' + _id +'/'
             
         df = []
         if path_in.endswith('.csv'):
             df = pd.read_csv(path_in)
         elif path_in.endswith('.txt'):
             df = loadFile(path_in)
         elif path_in.endswith('.mtx'):
@@ -140,22 +138,21 @@
                     os.remove(path_out + "%s_mutation_wave.jpg" % _id)
                 fig.savefig(path_out + "%s_mutation_wave.jpg" % _id)
                 plt.close(fig)            
         else:
             print("Wrong file: %s" % path_in)
             continue        
 
-def fitWavePlot(paths_in, paths_out, ids):
+def fitWavePlot(paths_in, ids):
     prop = np.transpose([paths_in, ids])
     print("fitness")
     print(prop)
     for path_in, _id in prop:
         
-        os.chdir(paths_out)
-        path_out = paths_out + '/Figures/' + _id + '/'
+        path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/' + _id +'/'
             
         df = []
         if path_in.endswith('.csv'):
             df = pd.read_csv(path_in)
         elif path_in.endswith('.txt'):
             df = loadFile(path_in)
         elif path_in.endswith('.mtx'):
@@ -198,26 +195,25 @@
                     os.remove(path_out + "%s_fitness_wave.jpg" % _id)
                 fig.savefig(path_out + "%s_fitness_wave.jpg" % _id)
                 plt.close(fig)            
         else:
             print("Wrong file: %s" % path_in)
             continue  
 
-def mullerPlot(path_in, path_out):   
+def mullerPlot(path_in):   
     '''
     path_in - absolute path to file with .txt extension (simulation data is saved into txt file)
     path_out - absolute path to figures save localization
     '''
     
     if not path_in.endswith('.txt'):
         print("Wrong file")
-        return
+        return   
     
-    if not path_out.endswith('/'):
-        path_out = path_out + '/'
+    path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/'
     
     _F = open(path_in, 'r')
     _L = _F.readlines()
     
     clones = []
     ret = []
     first = True
@@ -249,14 +245,19 @@
     
     ## Generation number, clone number, cells count
     Population = pd.DataFrame(Population)
     temp = ["Generation"]
     temp.extend([str(x) for x in clones])
     Population.columns = temp
     ax = Population.plot.bar(x="Generation", stacked=True, legend=False, width=1, figsize=(40,20))
+    ax.set_xticks(list(range(0,len(Population['Generation']),200)))
+    ax.set_xlabel('Generation', fontsize=50)
+    ax.set_ylabel('Cells number', fontsize=50)
+    plt.xticks(fontsize=40)
+    plt.yticks(fontsize=40)
     
     fig = ax.get_figure()
     try:
         os.makedirs(path_out, exist_ok=True) 
     except OSError as error:
         print(error)
     finally:
@@ -331,28 +332,26 @@
                 df.pop()
                 break
     df = pd.DataFrame(df)
     df.columns = columns
     _f.close()
     return df
 
-def binnedHist(paths_in, paths_out, ids):
+def binnedHist(paths_in, ids):
     '''
     path_in - absolute path to file with .txt extension (binned simulation data is saved into txt file)
     path_out - absolute path to figures save localization
     '''
     prop = np.transpose([paths_in, ids])
     for path_in, _id in prop:
         if not path_in.endswith('.txt'):
             print("Wrong file")
             return
         
-        path_out = paths_out + '/Figures/' + _id
-        if not paths_out.endswith('/'):
-            path_out = path_out + '/'
+        path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/' + _id +'/'
         
         df = loadFile(path_in)
         
         pass_m_l = []
         driv_m_l = []
         
         for row in df.iterrows():
@@ -489,28 +488,26 @@
                     if os.path.exists(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(int(row[1]['Clone number'])) +".jpg"):
                         os.remove(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(int(row[1]['Clone number'])) +".jpg")
                     fig.savefig(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(int(row[1]['Clone number'])) +".jpg")
                     plt.close(fig)
             else:
                 continue
 
-def matrixHist(paths_in, paths_out, ids):
+def matrixHist(paths_in, ids):
     '''
     path_in - absolute path to file with .txt extension (binned simulation data is saved into txt file)
     path_out - absolute path to figures save localization
     '''
     prop = np.transpose([paths_in, ids])
     for path_in, _id in prop:    
         if not path_in.endswith('.mtx'):
             print("Wrong file")
             return
         os.chdir(paths_out)
-        path_out = paths_out + '/Figures/' + _id
-        if not path_out.endswith('/'):
-            path_out = path_out + '/'
+        path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/' + _id +'/'
     
         df = pd.read_csv(path_in)
         
         mm = []
         for row in df.iterrows():
             try:
                 mm.append(sc.sparse.load_npz(row[1]['Mutation matrix']))
@@ -678,28 +675,26 @@
                 print(error)
             finally:
                 if os.path.exists(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(int(clone[1]['Clone number'])) +".jpg"):
                     os.remove(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(int(clone[1]['Clone number'])) +".jpg")
                 fig.savefig(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(int(clone[1]['Clone number'])) +".jpg")
                 plt.close(fig)           
 
-def singleHist(paths_in, paths_out, ids):
+def singleHist(paths_in, ids):
     '''
     path_in - absolute path to file with .txt extension (binned simulation data is saved into txt file)
     path_out - absolute path to figures save localization
     '''
     prop = np.transpose([paths_in, ids])
     for path_in, _id in prop:    
         if not path_in.endswith('.csv'):
             print("Wrong file")
             return
         
-        path_out = paths_out + '/Figures/' + _id
-        if not path_out.endswith('/'):
-            path_out = path_out + '/'
+        path_out = '/'.join(np.array(path_in.split('/'))[0:len(path_in.split('/'))-1]) + '/Figures/' + _id +'/'
         
         filepath = Path(path_in)  
         filepath.parent.mkdir(parents=True, exist_ok=True)
         
         df = pd.read_csv(filepath)
         
         b = 0
@@ -812,9 +807,9 @@
                 if os.path.exists(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(clones[i]) +".jpg"):
                     os.remove(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(clones[i]) +".jpg")
                 fig.savefig(path_out + "%s_clone_mutations_VAF_ID_" % _id + str(clones[i]) +".jpg")
                 plt.close(fig)
                 print("saving files %.1f %%" % (i/len(clones) * 100))
             
 if __name__ == "__main__":
-    fitWavePlot(["E:\\Simulations\\Publication\\Normal Test S B M\\m3\\m3_matrix_3500.mtx"], 
-                "E:\\Simulations\\Publication\\Normal Test S B M\\m3", [3500])
+    mullerPlot("E:\\Simulations\\Publication\\Normal Test S B M\\m8\\m8_muller_plot_matrix_data.txt", 
+                "E:\\Simulations\\Publication\\Normal Test S B M\\m8\\Figures")
```

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution/mainView.py` & `clonalEvolution-2.0.0/src/clonalEvolution/mainView.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 import copy
 
 import clonalEvolution.external_plots as external_plots
 from clonalEvolution.clonal_evolution_init import clonalEvolutionMainLoop 
 
+# import external_plots as external_plots
+# from clonal_evolution_init import clonalEvolutionMainLoop 
+
 class mainFormat(qtWidget.QWidget):
     def __init__(self, parent=None):
         super().__init__(parent)
         self.ID = 1
         self.idx_s = 0
         self.idx_r = 0
         self.th_r = []
@@ -145,35 +148,35 @@
                         self.status.setText("Ended")
                     if not self.th_r and not self.th_s:
                         self.status.setStyleSheet("background-color: red")
                 else:
                     q.put(data)
             if self._th_muller.is_alive():
                 self._th_muller.join(1) 
-                if self._th_muller.is_alive():                   
+                if not self._th_muller.is_alive():                   
                     self.status.setText("muller plot done")
                     # self._th_muller = None
             if self._th_hist.is_alive():
                 self._th_hist.join(1)     
-                if self._th_hist.is_alive():               
+                if not self._th_hist.is_alive():               
                     self.status.setText("histograms done")
                     # self._th_hist = None
             if self._th_mw.is_alive():
                 self._th_mw.join(1)   
-                if self._th_mw.is_alive():                 
+                if not self._th_mw.is_alive():                 
                     self.status.setText("mutation wave done")
                     # self._th_mw = None
             if self._th_fw.is_alive():
                 self._th_fw.join(1) 
-                if self._th_fw.is_alive():                   
+                if not self._th_fw.is_alive():                   
                     self.status.setText("fitness wave done")
                     # self._th_fw = None
             if self._th_cp.is_alive():
                 self._th_cp.join(1)   
-                if self._th_cp.is_alive():                 
+                if not self._th_cp.is_alive():                 
                     self.status.setText("clone plot done")
                     # self._th_cp = None
                 
     def closeEvent(self, event):
         
         for i in self.s_ID:
             self.q.put(['1', str(i).split(',')[0], "exit"])
@@ -280,64 +283,55 @@
         _about.clicked.connect(self.about)
         layout.addWidget(_about)
         
         self.setLayout(layout)
         
     def mullerPlotAction(self):
         try:
-            if self._file_path.text() == "":
-                raise Exception()
             if self._th_muller.is_alive():
                 raise NameError()
         except NameError:
             self.showDialog("Plotting already", "Alert")
             return
-        except:
-            self.showDialog("Enter save path", "Alert")
-            return
+
         fname = qtWidget.QFileDialog.getOpenFileName(self, 'Open file', "Z://","CSV files (*.txt)")[0]  
         if fname == "":
             self.showDialog("No file selected!", "Alert")
             return
-        self._th_muller = (Thread(target=external_plots.mullerPlot, args=(fname, self._file_path.text() + "/Figures")))
-        # external_plots.mullerPlot(fname, self._file_path.text() + "/Figures")
+        self._th_muller = (Thread(target=external_plots.mullerPlot, args=([fname])))
+        # external_plots.mullerPlot(fname)
         self._th_muller.start()
         self.status.setText("muller plot ongoing")
         
     def cloneHistAction(self):
         try:
-            if self._file_path.text() == "":
-                raise Exception()
             if self._th_hist.is_alive():
                 raise NameError()
         except NameError:
             self.showDialog("Plotting already", "Alert")
             return
-        except:
-            self.showDialog("Enter save path", "Alert")
-            return
         fname = qtWidget.QFileDialog.getOpenFileNames(None, 'Open file', "Z://","Single data files (*.csv);; Binned data files (*.txt);; Matrix data files (*.mtx)")[0] 
         if len(fname) == 0:
             self.showDialog("No file selected!", "Alert")
             return
         name_id = []
         for i in fname:
             name_id.append(re.findall('\d+', i)[-1])
         if all(map(lambda x: x.endswith('.txt'), fname)):
-            self._th_hist = (Thread(target=external_plots.binnedHist, args=(fname, self._file_path.text(), name_id)))
+            self._th_hist = (Thread(target=external_plots.binnedHist, args=(fname, name_id)))
             # external_plots.binnedHist(fname, self._file_path.text(), name_id)
             self._th_hist.start()
             self.status.setText("mutations histograms ongoing")
         elif all(map(lambda x: x.endswith('.csv'), fname)):
-            self._th_hist = (Thread(target=external_plots.singleHist, args=(fname, self._file_path.text(), name_id)))
+            self._th_hist = (Thread(target=external_plots.singleHist, args=(fname, name_id)))
             # external_plots.singleHist(fname, self._file_path.text(), name_id)
             self._th_hist.start()
             self.status.setText("mutations histograms ongoing")
         elif all(map(lambda x: x.endswith('.mtx'), fname)):
-            self._th_hist = (Thread(target=external_plots.matrixHist, args=(fname, self._file_path.text(), name_id)))
+            self._th_hist = (Thread(target=external_plots.matrixHist, args=(fname, name_id)))
             # external_plots.matrixHist(fname, self._file_path.text(), name_id)
             self._th_hist.start()
             self.status.setText("mutations histograms ongoing")
         else:
             self.showDialog("Wrong file/files extension. Use only one kind at time", "Alert")
             
     def mutWaveAction(self):
@@ -357,15 +351,15 @@
         if len(fname) == 0:
             self.showDialog("No file selected!", "Alert")
             return
         name_id = []
         for i in fname:
             name_id.append(re.findall('\d+', i)[-1])
             
-        self._th_mw = (Thread(target=external_plots.mutWavePlot, args=(fname, self._file_path.text(), name_id)))
+        self._th_mw = (Thread(target=external_plots.mutWavePlot, args=(fname, name_id)))
         # external_plots.mutWavePlot(fname, self._file_path.text(), name_id)
         self._th_mw.start()
         self.status.setText("mutation wave ongoing")
     
     def fitWaveAction(self):
         try:
             if self._file_path.text() == "":
@@ -383,23 +377,23 @@
         if len(fname) == 0:
             self.showDialog("No file selected!", "Alert")
             return
         name_id = []
         for i in fname:
             name_id.append(re.findall('\d+', i)[-1])
             
-        self._th_fw = (Thread(target=external_plots.fitWavePlot, args=(fname, self._file_path.text(), name_id)))
+        self._th_fw = (Thread(target=external_plots.fitWavePlot, args=(fname, name_id)))
         # external_plots.fitWavePlot(fname, self._file_path.text(), name_id)
         self._th_fw.start()
         self.status.setText("fitness wave ongoing")
         
     def clonePlotAction(self):
         try:
-            if self._file_path.text() == "":
-                raise Exception()
+            # if self._file_path.text() == "":
+                # raise Exception()
             if self._th_cp.is_alive():
                 raise NameError()
         except NameError:
             self.showDialog("Plotting already", "Alert")
             return
         except:
             self.showDialog("Enter save path", "Alert")
@@ -409,15 +403,15 @@
         if len(fname) == 0:
             self.showDialog("No file selected!", "Alert")
             return
         name_id = []
         for i in fname:
             name_id.append(re.findall('\d+', i)[-1])
         
-        self._th_cp = (Thread(target=external_plots.clonePlot, args=(fname, self._file_path.text(), name_id)))
+        self._th_cp = (Thread(target=external_plots.clonePlot, args=(fname, name_id)))
         # external_plots.clonePlot(fname, self._file_path.text(), name_id)
         self._th_cp.start()
         self.status.setText("clone plot ongoing")
     
     def threadTabUI(self):
         self.threadTab = qtWidget.QWidget()
         _threadTab = qtWidget.QFormLayout()
```

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.0.0/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 1.5.0
+Version: 2.0.0
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-1.5.0/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.0.0/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 src/clonalEvolution/mainView.py
 src/clonalEvolution/wmean.py
 src/clonalEvolution.egg-info/PKG-INFO
 src/clonalEvolution.egg-info/SOURCES.txt
 src/clonalEvolution.egg-info/dependency_links.txt
 src/clonalEvolution.egg-info/entry_points.txt
 src/clonalEvolution.egg-info/requires.txt
-src/clonalEvolution.egg-info/top_level.txt
+src/clonalEvolution.egg-info/top_level.txt
+tests/test_simple.py
```

