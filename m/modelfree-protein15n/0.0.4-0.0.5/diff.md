# Comparing `tmp/modelfree-protein15n-0.0.4.tar.gz` & `tmp/modelfree-protein15n-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelfree-protein15n-0.0.4.tar", last modified: Wed May 17 13:42:20 2023, max compression
+gzip compressed data, was "modelfree-protein15n-0.0.5.tar", last modified: Wed May 17 21:12:43 2023, max compression
```

## Comparing `modelfree-protein15n-0.0.4.tar` & `modelfree-protein15n-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:42:20.483753 modelfree-protein15n-0.0.4/
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/LICENSE
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/MANIFEST.in
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3604 2023-05-17 13:42:20.482330 modelfree-protein15n-0.0.4/PKG-INFO
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2703 2023-05-17 13:26:36.000000 modelfree-protein15n-0.0.4/README.md
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:42:20.450263 modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3604 2023-05-17 13:42:20.000000 modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/PKG-INFO
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      573 2023-05-17 13:42:20.000000 modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/SOURCES.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-17 13:42:20.000000 modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/dependency_links.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-17 13:42:20.000000 modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/entry_points.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       48 2023-05-17 13:42:20.000000 modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/requires.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-17 13:42:20.000000 modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/top_level.txt
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:42:20.475717 modelfree-protein15n-0.0.4/modfree/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/__init__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/__main__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1736 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/analysis.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      719 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/constants_functions.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/data_format.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6476 2023-05-17 13:41:43.000000 modelfree-protein15n-0.0.4/modfree/generator.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2327 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/inputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14130 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/mf_standard.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5840 2023-05-17 13:42:02.000000 modelfree-protein15n-0.0.4/modfree/modfree.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3667 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/outputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2481 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/parser.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5079 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/modfree/ploter.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3346 2023-05-17 13:14:17.000000 modelfree-protein15n-0.0.4/modfree/run_fit.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-17 13:42:20.483753 modelfree-protein15n-0.0.4/setup.cfg
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1094 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.4/setup.py
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 21:12:43.497717 modelfree-protein15n-0.0.5/
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/LICENSE
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/MANIFEST.in
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-17 21:12:43.494481 modelfree-protein15n-0.0.5/PKG-INFO
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2698 2023-05-17 21:05:22.000000 modelfree-protein15n-0.0.5/README.md
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 21:12:43.460197 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/PKG-INFO
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      573 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/SOURCES.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/dependency_links.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/entry_points.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       48 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/requires.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/top_level.txt
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 21:12:43.489258 modelfree-protein15n-0.0.5/modfree/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/__init__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/__main__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1736 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/analysis.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      719 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/constants_functions.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/data_format.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6555 2023-05-17 20:50:18.000000 modelfree-protein15n-0.0.5/modfree/generator.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2327 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/inputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14130 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/mf_standard.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5837 2023-05-17 21:04:33.000000 modelfree-protein15n-0.0.5/modfree/modfree.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3675 2023-05-17 19:59:19.000000 modelfree-protein15n-0.0.5/modfree/outputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2481 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/parser.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     4488 2023-05-17 20:40:18.000000 modelfree-protein15n-0.0.5/modfree/ploter.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3389 2023-05-17 21:03:40.000000 modelfree-protein15n-0.0.5/modfree/run_fit.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-17 21:12:43.497717 modelfree-protein15n-0.0.5/setup.cfg
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1094 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/setup.py
```

### Comparing `modelfree-protein15n-0.0.4/LICENSE` & `modelfree-protein15n-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/PKG-INFO` & `modelfree-protein15n-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.4
+Version: 0.0.5
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Model-Free analysis framework for protein backbone amide 15N NMR spin relaxation rates.
@@ -52,15 +52,15 @@
         
         To fit relaxation data, you will need your data in a specific format akin to the generated data. Generate some data to see how it's done. You will also need a directory file and a parameter file. type the following command to fit the data generated in the previous section:
         
             $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml
             
         You can also fit only part of the data with the flag -r:
         
-            $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r [10, 11, 12, 13, 14, 15, 16]
+            $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r 10 11 12 13 14 15 16 17
             
         Or
         
             $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r 15
         
         ## Data plotting
```

### Comparing `modelfree-protein15n-0.0.4/README.md` & `modelfree-protein15n-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 To fit relaxation data, you will need your data in a specific format akin to the generated data. Generate some data to see how it's done. You will also need a directory file and a parameter file. type the following command to fit the data generated in the previous section:
 
     $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml
     
 You can also fit only part of the data with the flag -r:
 
-    $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r [10, 11, 12, 13, 14, 15, 16]
+    $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r 10 11 12 13 14 15 16 17
     
 Or
 
     $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r 15
 
 ## Data plotting
```

### Comparing `modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/PKG-INFO` & `modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.4
+Version: 0.0.5
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Model-Free analysis framework for protein backbone amide 15N NMR spin relaxation rates.
@@ -52,15 +52,15 @@
         
         To fit relaxation data, you will need your data in a specific format akin to the generated data. Generate some data to see how it's done. You will also need a directory file and a parameter file. type the following command to fit the data generated in the previous section:
         
             $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml
             
         You can also fit only part of the data with the flag -r:
         
-            $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r [10, 11, 12, 13, 14, 15, 16]
+            $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r 10 11 12 13 14 15 16 17
             
         Or
         
             $ modfree fit -o Generated_fit -d Generated/directories.toml -p Generated/parameters.toml -r 15
         
         ## Data plotting
```

### Comparing `modelfree-protein15n-0.0.4/modelfree_protein15n.egg-info/SOURCES.txt` & `modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/modfree/analysis.py` & `modelfree-protein15n-0.0.5/modfree/analysis.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/modfree/constants_functions.py` & `modelfree-protein15n-0.0.5/modfree/constants_functions.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/modfree/data_format.py` & `modelfree-protein15n-0.0.5/modfree/data_format.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/modfree/generator.py` & `modelfree-protein15n-0.0.5/modfree/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     return None
 
 
 def generate(N, output_dir, fields=(400, 600, 800, 1000, 1200), rates=('R1', 'R2', 'nOe', 'etaXY'), modes=2, noise_proportion=0.01):
     if type(modes) is not int:
         print("the number of dynamic modes must be an int")
         modes = int(modes)
+    if type(fields) is int or type(fields) is float:
+        fields = [fields]
     RES = np.arange(1, N+1)
     print("Parameter generation...")
     if modes == 1:
         amps = [1]
         taus = [random_tau_100ps(N)]
     elif modes == 2:
         a1 = random_amp1(N)
```

### Comparing `modelfree-protein15n-0.0.4/modfree/inputs.py` & `modelfree-protein15n-0.0.5/modfree/inputs.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/modfree/mf_standard.py` & `modelfree-protein15n-0.0.5/modfree/mf_standard.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/modfree/modfree.py` & `modelfree-protein15n-0.0.5/modfree/modfree.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import modfree.inputs as inputs
 import modfree.outputs as outputs
 import modfree.run_fit as run_fit
 import modfree.ploter as ploter
 import modfree.generator as generator
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 console = Console()
 
 
 header = "\n".join(
 [
@@ -77,15 +77,15 @@
     subparsers = parser.add_subparsers(dest="commands")
 
     fit_parser = subparsers.add_parser("fit", help="Fit the data")
     fit_parser.set_defaults(func=fit)
     fit_parser.add_argument('-o', type=str, help="output directory", default="Outputs")
     fit_parser.add_argument('-d', type=str, help="directory file. toml file. contains the directories and the corresponding conditions", default="directories.toml")
     fit_parser.add_argument('-p', type=str, help="parameter file. toml file", default="params.toml")
-    fit_parser.add_argument('-r', type=str, help="residue to analyse. can be 'all' or a number corresponding to the residue number.", default="None")
+    fit_parser.add_argument('-r', type=int, nargs="+", help="Residue(s) to analyse. By default, the program reads the parameter file.", default=0)
     fit_parser.add_argument('-m', type=str, help="fitting model: standard (std), arrhenius (arrh), viscosity (visc), arrhenius-viscosity (arvi).", default="std")
     fit_parser.add_argument('-plot', type=bool, help="plot the output", default=False)
     
     plot_parser = subparsers.add_parser("plot", help="Plot the data")
     plot_parser.set_defaults(func=plot)
     plot_parser.add_argument('-o', type=str, help="output directory", default="Outputs")
     plot_parser.add_argument('-p', type=str, help="what to plot: all, relaxation, parameters, statistics, correlation", default="all")
```

### Comparing `modelfree-protein15n-0.0.4/modfree/outputs.py` & `modelfree-protein15n-0.0.5/modfree/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         os.mkdir(directory)
     if directory[-1] != "/":
         directory = directory + "/"
     values = df.swap(result_dic, 1, 2)['values']
     #values = df.swap(values, 2, 3) # values[res][amps/taus][0,1,2,...]
     errors = df.swap(result_dic, 1, 2)['error']
     #errors = df.swap(errors, 2, 3)
-    X = [res for res in values.keys()]
+    X = sorted([res for res in values.keys()])
     # residue specific monte carlo results
     if not os.path.isdir(directory+"Monte_Carlo"):
         os.mkdir(directory+"Monte_Carlo")
     for res in X:
         if not os.path.isdir(directory+"Monte_Carlo/"+str(res)):
             os.mkdir(directory+"Monte_Carlo/"+str(res))
         save_param(result_dic[res]['mc_red_chi2_distrib'], outputname=directory+"Monte_Carlo/"+str(res)+"/mc_redchi2.out")
```

### Comparing `modelfree-protein15n-0.0.4/modfree/parser.py` & `modelfree-protein15n-0.0.5/modfree/parser.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.4/modfree/ploter.py` & `modelfree-protein15n-0.0.5/modfree/ploter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import glob
 import os
+import re
 from modfree.inputs import read_relaxation_data_file
 
 
 plt.rcParams['font.family'] = 'FreeSans'
 plt.rcParams['legend.numpoints'] = 1
 plt.rc('text', usetex=False)
 plt.rcParams['mathtext.default'] = 'regular'
@@ -19,15 +20,15 @@
 
 
 def check_output_dir(output_dir):
     if not os.path.isdir(output_dir+"/Plots"):
         os.mkdir(output_dir+"/Plots")
 
 
-def plot_param(filename, plotname=None, color="darkblue", ax=None, log=False, file_format="pdf", dpi=600):
+def plot_param(filename, color="darkblue", ax=None, log=False):
     with open(filename, "r") as f:
         dat = [el.rstrip("\n").split() for el in f.readlines()]
     x = [int(el[0]) for el in dat]
     if ax == None:
         fig, ax = plt.subplots(1, 1, figsize=(8, 5))
     if len(dat[0]) == 1:
         ax.plot(x, color=color)
@@ -39,37 +40,33 @@
         dy = [float(el[2]) for el in dat]
         ax.errorbar(x, y, yerr=dy, color=color)
     if log:
         ax.set_yscale("log")
     ax.set_xlabel("Sequence")
     ax.set_ylabel(filename.split("/")[-1].replace(".out", ""))
     ax.set_ylim(0.8*np.min(y), 1.2*np.max(y))
-    #if plotname is not None:
-    #    plt.savefig(output_dir+"/"+plotname, format=file_format, dpi=dpi)
 
 
-def plot_params_std(output_dir, plotname, file_format="pdf", dpi=600):
+def plot_params_std(output_dir, file_format="pdf", dpi=600):
     check_output_dir(output_dir)
-    fig, ax = plt.subplots(3, 2, figsize=(16, 10))
-    plot_param(output_dir+"/amp1.out", None, "darkblue", ax[0][0])
-    plot_param(output_dir+"/amp2.out", None, "darkblue", ax[1][0])
-    plot_param(output_dir+"/amp3.out", None, "darkblue", ax[2][0])
-    plot_param(output_dir+"/tau1.out", None, "darkblue", ax[0][1], log=True)
-    plot_param(output_dir+"/tau2.out", None, "darkblue", ax[1][1], log=True)
-    plot_param(output_dir+"/tau3.out", None, "darkblue", ax[2][1], log=True)
-    plt.savefig(output_dir+"/Plots/"+plotname, format=file_format, dpi=dpi)
-    plt.close()
+    param_files = glob.glob(output_dir+"/*.out")
+    for el in param_files:
+        log = True if re.search("tau", el) else False
+        fig, ax = plt.subplots(1, 1, figsize=(8, 5))
+        plot_param(el, ax=ax, log=log, color="darkblue")
+        plt.savefig(output_dir+"/Plots/"+el.split("/")[-1].replace(".out", "."+file_format), format=file_format, dpi=dpi)
+        plt.close()
     
 
 def plot_statistics_std(output_dir, plotname, file_format="pdf", dpi=600):
     check_output_dir(output_dir)
     fig, ax = plt.subplots(3, 1, figsize=(8, 10))
-    plot_param(output_dir+"/redchi2.out", None, "darkblue", ax[0], log=True)
-    plot_param(output_dir+"/aic.out", None, "darkblue", ax[1])
-    plot_param(output_dir+"/bic.out", None, "darkblue", ax[2])
+    plot_param(output_dir+"/redchi2.out", color="darkblue", ax=ax[0], log=True)
+    plot_param(output_dir+"/aic.out", color="darkblue", ax=ax[1])
+    plot_param(output_dir+"/bic.out", color="darkblue", ax=ax[2])
     plt.savefig(output_dir+"/Plots/"+plotname, format=file_format, dpi=dpi)
     plt.close()
     
     
 def plot_rates_corr_std(output_dir, plotname, file_format="pdf", dpi=600):
     check_output_dir(output_dir)
     rates_fit_dirs = sorted(glob.glob(output_dir+"/Relaxation_Rates/*.fit"))
@@ -98,17 +95,8 @@
         ax.fill_between(x1, np.array(y1)-np.array(dy1), np.array(y1)+np.array(dy1), color="darkblue", alpha=0.5)
         ax.plot(x2, y2, color="darkorange", label="Fit")
         ax.fill_between(x2, np.array(y2)-np.array(dy2), np.array(y2)+np.array(dy2), color="darkorange", alpha=0.5)
         ax.set_xlabel("Sequence")
         ax.set_ylabel(rdir.split("/")[-1].replace(".exp", ""))
         ax.legend(frameon=False)
         plt.savefig(output_dir+"/Plots/"+rdir.split("/")[-1].replace("exp", str(file_format)), format=file_format, dpi=dpi)
-        plt.close()
-    
-    
-def plot_monte_carlo(output_dir, plotname, file_format="pdf", dpi=600):
-    # Chi2 distributions, parameter correlations (maybe its own plot function)
-    print("to be implemented")
-
-
-if __name__ == "__main__":
-    print("this is the plot module")
+        plt.close()
```

### Comparing `modelfree-protein15n-0.0.4/modfree/run_fit.py` & `modelfree-protein15n-0.0.5/modfree/run_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     else:
         print("model not implemented in run_fit.run_fit")
         return None
 
 
 def launch_fits(input_parameters_dic, residue, directories, model="std"):
     data_dic, error_dic = format_data(input_parameters_dic, directories, model=model)
-    if residue == "None":
+    if residue == 0:
         residue = input_parameters_dic["residues"]
     if residue == "all":
         results = dict()
-        for res in data_dic.keys():
+        for res in sorted(list(data_dic.keys())):
             print("\nresidue", res)
             try:
                 results[res] = run_fit(data_dic[res], error_dic[res], input_parameters_dic, model=model)
             except TypeError:
                 print("TypeError exception, there is probably not enough data for this residue.")
-    elif type(residue) == list:
+    elif type(residue) == list or type(residue) == tuple:
         results = dict()
-        for res in residue:
+        for res in sorted(residue):
             if res not in data_dic.keys():
                 print("\nresidue", res, "not in data")
                 continue
             print("\nresidue", res)
             try:
                 results[res] = run_fit(data_dic[res], error_dic[res], input_parameters_dic, model=model)
             except TypeError:
```

### Comparing `modelfree-protein15n-0.0.4/setup.py` & `modelfree-protein15n-0.0.5/setup.py`

 * *Files identical despite different names*

