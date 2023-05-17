# Comparing `tmp/nemophoto-0.4.0.tar.gz` & `tmp/nemophoto-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nemophoto-0.4.0.tar", last modified: Wed Nov 23 14:39:50 2022, max compression
+gzip compressed data, was "dist/nemophoto-0.5.0.tar", last modified: Wed May 17 06:50:04 2023, max compression
```

## Comparing `nemophoto-0.4.0.tar` & `nemophoto-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2022-11-23 14:39:50.881081 nemophoto-0.4.0/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       51 2022-11-23 13:19:51.000000 nemophoto-0.4.0/.gitignore
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     1071 2021-10-01 13:50:37.000000 nemophoto-0.4.0/LICENSE
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       25 2021-10-30 15:21:47.000000 nemophoto-0.4.0/MANIFEST.in
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7703 2022-11-23 14:39:50.880081 nemophoto-0.4.0/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     6450 2022-11-23 13:19:51.000000 nemophoto-0.4.0/README.md
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2022-11-23 14:39:50.865081 nemophoto-0.4.0/batch_examples/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      315 2021-10-06 19:56:05.000000 nemophoto-0.4.0/batch_examples/qc.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      245 2021-10-06 19:56:05.000000 nemophoto-0.4.0/batch_examples/slurm.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      205 2022-11-23 13:19:52.000000 nemophoto-0.4.0/batch_examples/td.in
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      118 2022-11-23 13:19:53.000000 nemophoto-0.4.0/batch_examples/ts.sh
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2022-11-23 14:39:50.872081 nemophoto-0.4.0/nemo/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        0 2021-10-07 12:24:10.000000 nemophoto-0.4.0/nemo/__init__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8533 2022-11-23 13:19:53.000000 nemophoto-0.4.0/nemo/__main__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2022-11-23 14:23:13.000000 nemophoto-0.4.0/nemo/__version__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    35885 2022-11-23 13:19:53.000000 nemophoto-0.4.0/nemo/analysis.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     2417 2022-11-23 13:19:53.000000 nemophoto-0.4.0/nemo/batch_lx.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    18042 2022-11-23 13:19:53.000000 nemophoto-0.4.0/nemo/tools.py
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2022-11-23 14:39:50.879081 nemophoto-0.4.0/nemophoto.egg-info/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7703 2022-11-23 14:39:50.000000 nemophoto-0.4.0/nemophoto.egg-info/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      438 2022-11-23 14:39:50.000000 nemophoto-0.4.0/nemophoto.egg-info/SOURCES.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        1 2022-11-23 14:39:50.000000 nemophoto-0.4.0/nemophoto.egg-info/dependency_links.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       45 2022-11-23 14:39:50.000000 nemophoto-0.4.0/nemophoto.egg-info/entry_points.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       24 2022-11-23 14:39:50.000000 nemophoto-0.4.0/nemophoto.egg-info/requires.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        5 2022-11-23 14:39:50.000000 nemophoto-0.4.0/nemophoto.egg-info/top_level.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       38 2022-11-23 14:39:50.881081 nemophoto-0.4.0/setup.cfg
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     3644 2022-11-23 14:23:13.000000 nemophoto-0.4.0/setup.py
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.453790 nemophoto-0.5.0/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       51 2022-11-23 13:19:51.000000 nemophoto-0.5.0/.gitignore
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     1071 2021-10-01 13:50:37.000000 nemophoto-0.5.0/LICENSE
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       25 2021-10-30 15:21:47.000000 nemophoto-0.5.0/MANIFEST.in
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-05-17 06:50:04.451790 nemophoto-0.5.0/PKG-INFO
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     6722 2023-05-17 06:49:22.000000 nemophoto-0.5.0/README.md
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.372789 nemophoto-0.5.0/Tutorial/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    20260 2023-05-17 06:49:22.000000 nemophoto-0.5.0/Tutorial/Tutorial.md
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.392790 nemophoto-0.5.0/batch_examples/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      315 2021-10-06 19:56:05.000000 nemophoto-0.5.0/batch_examples/qc.sh
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      245 2021-10-06 19:56:05.000000 nemophoto-0.5.0/batch_examples/slurm.sh
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      205 2022-11-23 13:19:52.000000 nemophoto-0.5.0/batch_examples/td.in
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      118 2022-11-23 13:19:53.000000 nemophoto-0.5.0/batch_examples/ts.sh
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.438790 nemophoto-0.5.0/nemo/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        0 2021-10-07 12:24:10.000000 nemophoto-0.5.0/nemo/__init__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8440 2023-05-17 06:49:22.000000 nemophoto-0.5.0/nemo/__main__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2023-05-17 06:49:22.000000 nemophoto-0.5.0/nemo/__version__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    41306 2023-05-17 06:49:22.000000 nemophoto-0.5.0/nemo/analysis.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     2417 2022-11-23 13:19:53.000000 nemophoto-0.5.0/nemo/batch_lx.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    18042 2022-11-23 13:19:53.000000 nemophoto-0.5.0/nemo/tools.py
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.449790 nemophoto-0.5.0/nemophoto.egg-info/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/PKG-INFO
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      459 2023-05-17 06:50:04.000000 nemophoto-0.5.0/nemophoto.egg-info/SOURCES.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        1 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/dependency_links.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       45 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/entry_points.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       24 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/requires.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        5 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/top_level.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       38 2023-05-17 06:50:04.453790 nemophoto-0.5.0/setup.cfg
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     3644 2023-05-17 06:49:22.000000 nemophoto-0.5.0/setup.py
```

### Comparing `nemophoto-0.4.0/LICENSE` & `nemophoto-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nemophoto-0.4.0/PKG-INFO` & `nemophoto-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nemophoto
-Version: 0.4.0
+Version: 0.5.0
 Summary: Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.
 Home-page: https://github.com/LeonardoESousa/NEMO
 Author: Leonardo Evaristo de Sousa
 Author-email: ledso@dtu.dk
 License: MIT
 Description: 
         # NEMO - Photophysics with the Nuclear Ensemble Method
         
         [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
         [![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
         [![down](https://img.shields.io/pypi/dm/nemophoto)]()
-        [![maint](https://img.shields.io/maintenance/yes/2021)]()
+        [![maint](https://img.shields.io/maintenance/yes/2023)]()
         [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
         
         
          Fluorescence, phosphorescence and intersystem crossing (ISC) rate calculations. Absorption, fluorescence and phosphorescence spectrum simulations. Förster radius and singlet exciton diffusion length estimates. Interfaces with the QChem package. 
         
         Table of Contents
         =================
@@ -62,26 +62,28 @@
         
         ## How to install it?
         
         Run:
         
         `pip install nemophoto`
         
-        To get the latest commit run:
+        To get the latest commit, run:
         
         `pip install git+https://github.com/LeonardoESousa/NEMO`
         
         Alternatively, clone the repository to your computer. Inside the NEMO folder, run:
         
         `pip install .`
         
         Once installed, you should be able to run the program from any folder by just using the `nemo` command.
         
         ## How to use it?
         
+        Here is a quick guide on how to use the software. For a detailed tutorial, click [here](https://github.com/LeonardoESousa/NEMO/blob/main/Tutorial/Tutorial.md).
+        
         1. Initial steps:
             - Create a folder for your project. Add the log file for the frequency calculation to your folder. If the frequency calculation was run with Gaussian, you must also provide a QChem input file containing some settings you wish to apply in the ensemble calculations (e.g. functional, basis set, omega value, charge and multiplicity etc). An example of such file (td.in) is provided [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples).
             - A frequency calculation in the S0 state is suitable for computing an absorption spectrum. For fluorescence spectra and/or ISC rates calculations from Sn states to triplet states, a Sn frequency calculation is expected. Finally, for phosphorescence spectra and/or rISC rates calculations from Tn states to singlet states, a Tn frequency calculation is expected.  
             - Run the `nemo` command. Choose option 1 and follow the instructions to select the parameters of the calculation. This includes the dielectric constant and refractive index of the medium. This information will be used to obtain state-specific solvent corrections to the TD(A)-DFT energies.  
             - Add a bash script file to the folder. This file depends on which batch system you use. Examples of this file for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples)).
             - Run the `nemo` command again, choose option 2 and follow the instructions. Alternatively, just run all calculations created in the Geometries folder. Once the calculations are running, you may use option 3 to check the progress or option 4 to abort.
         
@@ -94,14 +96,15 @@
         4. IMPORTANT:
             - You may choose to calculate spectra and rates with different solvent dielectric constant and refractive index than the ones selected as input in Option 1. To do so, NEMO will resort to the extrapolation procedure described in ADD PAPER to adjust the results to the new solvent. 
         
         5. For exciton properties:
             - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. Copy both spectra to a folder and inside this folder run the `nemo` command. Choose option 7. Follow the instructions to set the calculation parameters. A file will be generated with all the information. Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. These estimations follow from the procedures described in: "de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071." 
         
         
+        For better visualization of results, consider using  [Nemoview](https://github.com/LeonardoESousa/nemoview). 
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `nemophoto-0.4.0/README.md` & `nemophoto-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # NEMO - Photophysics with the Nuclear Ensemble Method
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
 [![down](https://img.shields.io/pypi/dm/nemophoto)]()
-[![maint](https://img.shields.io/maintenance/yes/2021)]()
+[![maint](https://img.shields.io/maintenance/yes/2023)]()
 [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
 
 
  Fluorescence, phosphorescence and intersystem crossing (ISC) rate calculations. Absorption, fluorescence and phosphorescence spectrum simulations. Förster radius and singlet exciton diffusion length estimates. Interfaces with the QChem package. 
 
 Table of Contents
 =================
@@ -53,26 +53,28 @@
 
 ## How to install it?
 
 Run:
 
 `pip install nemophoto`
 
-To get the latest commit run:
+To get the latest commit, run:
 
 `pip install git+https://github.com/LeonardoESousa/NEMO`
 
 Alternatively, clone the repository to your computer. Inside the NEMO folder, run:
 
 `pip install .`
 
 Once installed, you should be able to run the program from any folder by just using the `nemo` command.
 
 ## How to use it?
 
+Here is a quick guide on how to use the software. For a detailed tutorial, click [here](https://github.com/LeonardoESousa/NEMO/blob/main/Tutorial/Tutorial.md).
+
 1. Initial steps:
     - Create a folder for your project. Add the log file for the frequency calculation to your folder. If the frequency calculation was run with Gaussian, you must also provide a QChem input file containing some settings you wish to apply in the ensemble calculations (e.g. functional, basis set, omega value, charge and multiplicity etc). An example of such file (td.in) is provided [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples).
     - A frequency calculation in the S0 state is suitable for computing an absorption spectrum. For fluorescence spectra and/or ISC rates calculations from Sn states to triplet states, a Sn frequency calculation is expected. Finally, for phosphorescence spectra and/or rISC rates calculations from Tn states to singlet states, a Tn frequency calculation is expected.  
     - Run the `nemo` command. Choose option 1 and follow the instructions to select the parameters of the calculation. This includes the dielectric constant and refractive index of the medium. This information will be used to obtain state-specific solvent corrections to the TD(A)-DFT energies.  
     - Add a bash script file to the folder. This file depends on which batch system you use. Examples of this file for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples)).
     - Run the `nemo` command again, choose option 2 and follow the instructions. Alternatively, just run all calculations created in the Geometries folder. Once the calculations are running, you may use option 3 to check the progress or option 4 to abort.
 
@@ -85,7 +87,8 @@
 4. IMPORTANT:
     - You may choose to calculate spectra and rates with different solvent dielectric constant and refractive index than the ones selected as input in Option 1. To do so, NEMO will resort to the extrapolation procedure described in ADD PAPER to adjust the results to the new solvent. 
 
 5. For exciton properties:
     - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. Copy both spectra to a folder and inside this folder run the `nemo` command. Choose option 7. Follow the instructions to set the calculation parameters. A file will be generated with all the information. Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. These estimations follow from the procedures described in: "de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071." 
 
 
+For better visualization of results, consider using  [Nemoview](https://github.com/LeonardoESousa/nemoview).
```

### Comparing `nemophoto-0.4.0/nemo/__main__.py` & `nemophoto-0.5.0/nemo/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,25 +43,29 @@
             rem, cm, _ = nemo.tools.busca_input(template)
         else:    
             rem, cm, spec = nemo.tools.busca_input(freqlog)        
         print('\nThe suggested configurations for you are:\n')
         print(rem)
         change = input('Are you satisfied with these parameters? y or n?\n')
         if change.lower() == 'n':     
-            rem2 = ''
+            rem2 = '$rem\n'
             for elem in rem.split('\n'):
                 if len(elem.split()) > 1:
                     if '$' not in elem:
                         base = nemo.tools.default(elem, f'{elem.split()[0]} is set to: {elem.split()[-1]}. If ok, Enter. Otherwise, type the correct value. Type del to delete line.\n')
                         if base.lower() == 'del':
-                            base = ''
+                            rem2 += ''
+                        else:
+                            if len(base.split()) > 1:
+                                rem2 += base+'\n'
+                            else:    
+                                rem2 += f'{elem.split()[0]}    {base}\n'    
                     else:    
-                        base = elem
-                    rem2 += base+'\n'
-            rem = rem2
+                        rem2 += elem+'\n'
+            rem = rem2+'$end\n'
         rem   += "\n$pcm\ntheory                  IEFPCM\nChargeSeparation        Marcus\nStateSpecific           Perturb\n$end\n"
         static = input("Solvent's static dielectric constant?\n")
         refrac = input("Solvent's refractive index?\n")
         try:
             static = float(static)
             refrac = float(refrac)
         except:
@@ -90,16 +94,15 @@
             nemo.tools.fatal_error("Have you heard about absolute zero? Goodbye!")
         if gauss:
             import lx.tools
             lx.tools.make_ensemble(freqlog, num_geoms, T, header,'$end\n')
             G, atomos = lx.tools.pega_geom(freqlog)
         else:    
             nemo.tools.make_ensemble(freqlog, num_geoms, T, header,'$end\n')  
-            G, atomos = nemo.tools.pega_geom(freqlog)  
-        nemo.tools.write_input(atomos,G,rem.replace(f'$rem',"$comment\n{spec}\n$end\n\n$rem\ncis_n_roots             {num_ex}\ncis_singlets            true\ncis_triplets            true\ncalc_soc                false\nSTS_MOM                 false\nCIS_RELAXED_DENSITY     TRUE\n$molecule\n{cm}\n"),'$end\n',"Opt_Lambda.com")    
+            G, atomos = nemo.tools.pega_geom(freqlog)      
     elif op == '2':
         nemo.tools.batch() 
     elif op == '3':
         nemo.tools.andamento()
     elif op == '4':
         nemo.tools.abort_batch()
     elif op == '5':
```

### Comparing `nemophoto-0.4.0/nemo/analysis.py` & `nemophoto-0.5.0/nemo/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -519,38 +519,50 @@
     eps_i, nr_i = nemo.tools.get_nr()
     kbT         = nemo.tools.detect_sigma()
     if 's' in initial.lower():
         Numbers, Singlets, Triplets, Oscs, Ss_s, Ss_t, GP, IND_S, IND_T   = analysis(files) 
         if 's0' == initial.lower():
             label_oscs = [f'osc_s{i+1}' for i in range(Oscs.shape[1])]
         else:
-            Oscs       = Oscs[:,n_state][:,np.newaxis]
-            label_oscs = ['osc']
+            #Oscs       = Oscs[:,n_state][:,np.newaxis]
+            label_oscs = [f'osce_s{n_state+1+i}' for i in range(Oscs.shape[1])]
             noscs      = pega_oscs(files, IND_S,initial)
             label_oscs.extend([f'osc_s{n_state+2+i}' for i in range(noscs.shape[1])])
             Oscs       = np.hstack((Oscs,noscs))     
         try:
-            socs_complete  = avg_socs(files,'singlet',n_state)
-            header7 = ['soc_t'+str(i) for i in range(1,1+socs_complete.shape[1])]
+            header7 = []
+            for i in range(Singlets.shape[1]):
+                socs_partial  = avg_socs(files,'singlet',i)
+                header7.extend([f'soc_s{i+1}_t{j}' for j in range(1,1+socs_partial.shape[1])])
+                try:
+                    socs_complete = np.hstack((socs_complete,socs_partial))
+                except:
+                    socs_complete = socs_partial
         except:
             pass
     else:
         Numbers, Singlets, Triplets, _, Ss_s, Ss_t, GP, IND_S, IND_T = analysis(files)
         Oscs       = get_osc_phosph(files,Singlets, Triplets, Ss_s, Ss_t, IND_S, IND_T)
-        Oscs       = Oscs[:,n_state][:,np.newaxis]
-        label_oscs = ['osc']
+        #Oscs       = Oscs[:,n_state][:,np.newaxis]
+        label_oscs = [f'osce_t{n_state+1+i}' for i in range(Oscs.shape[1])]
         noscs      = pega_oscs(files, IND_T,initial)
         Oscs       = np.hstack((Oscs,noscs)) 
         label_oscs.extend([f'osc_t{n_state+2+i}' for i in range(noscs.shape[1])])
         try:
-            socs_complete = np.hstack((avg_socs(files,'ground',n_state),avg_socs(files,'triplet',n_state),avg_socs(files,'tts',n_state)))
-            indices  = [i+1 for i in range(Triplets.shape[1]) if i != n_state] #Removed Tn to Tn transfers
-            header7  = ['soc_s0']
-            header7.extend(['soc_s'+str(i) for i in range(1,1+Singlets.shape[1])])
-            header7.extend(['soc_t'+str(i) for i in indices])   
+            header7 = []
+            for i in range(Triplets.shape[1]):
+                socs_partial = np.hstack((avg_socs(files,'ground',i),avg_socs(files,'triplet',i),avg_socs(files,'tts',i)))
+                indices  = [j+1 for j in range(Triplets.shape[1]) if j != i] #Removed Tn to Tn transfers
+                header7.extend([f'soc_t{i+1}_s0'])
+                header7.extend([f'soc_t{i+1}_s{j}' for j in range(1,1+Singlets.shape[1])])
+                header7.extend([f'soc_t{i+1}_t{j}' for j in indices]) 
+                try:
+                    socs_complete = np.hstack((socs_complete,socs_partial))
+                except:
+                    socs_complete = socs_partial    
         except:
             pass
     header = ['geometry']
     header.extend(['e_s'+str(i) for i in range(1,1+Singlets.shape[1])])
     header.extend(['e_t'+str(i) for i in range(1,1+Triplets.shape[1])])
     header.extend(['d_s'+str(i) for i in range(1,1+Ss_s.shape[1])])
     header.extend(['d_t'+str(i) for i in range(1,1+Ss_t.shape[1])])
@@ -559,18 +571,24 @@
     try:
         header.extend(header7)
         data = np.hstack((Numbers,Singlets,Triplets,Ss_s,Ss_t,GP[:,np.newaxis],Oscs,socs_complete))
     except:
         data = np.hstack((Numbers,Singlets,Triplets,Ss_s,Ss_t,GP[:,np.newaxis],Oscs))
     arquivo = f'Ensemble_{initial.upper()}_.lx'
     data = pd.DataFrame(data,columns=header)
-    data.insert(0,'ensemble',initial.upper())
-    data.insert(0,'kbT',kbT)
-    data.insert(0,'nr',nr_i)
-    data.insert(0,'eps',eps_i)
+    #add 'ensemble', 'kbT', 'nr', 'eps' columns with constant values
+    # values are initial.upper(), kbT, nr_i, eps_i
+    data['ensemble'] = initial.upper()
+    data['kbT']      = kbT
+    data['nr']       = nr_i
+    data['eps']      = eps_i
+    # make these the first columns
+    cols = data.columns.tolist()
+    cols = cols[-4:] + cols[:-4]
+    data = data[cols]
     if save:
         data.to_csv(arquivo,index=False)
     return data
 #######################################################################################
 
 ###PRINTS RATES AND EMISSION SPECTRUM##################################################
 def export_results(data,emission,dielec):
@@ -591,16 +609,45 @@
     arquivo = nemo.tools.naming(f'rates_{initial}_.lx')  
     solvent = f'#Epsilon: {dielec[0]:.3f} nr: {dielec[1]:.3f}\n'
     with open(arquivo, 'w') as f:
         f.write(solvent+data.to_string(header=True, index=False))
     print(f'Rates are written in the {arquivo} file')  
 #######################################################################################
 
+def reorder(initial_state, final_state, Ss_i, Ss_f, socs):
+    argsort = np.argsort(initial_state, axis=1)
+    initial_state = np.take_along_axis(initial_state, argsort, axis=1)
+    Ss_i = np.take_along_axis(Ss_i, argsort, axis=1)
+    corredor = int(np.sqrt(socs.shape[1]))
+    socs_complete = socs.reshape((socs.shape[0], corredor,corredor))
+    for j in range(socs_complete.shape[1]):
+        socs_complete[:,j,:] = np.take_along_axis(socs_complete[:,j,:], argsort, axis=1)
+    argsort = np.argsort(final_state, axis=1)
+    final_state = np.take_along_axis(final_state, argsort, axis=1)
+    Ss_f = np.take_along_axis(Ss_f, argsort, axis=1)
+    for j in range(socs_complete.shape[1]):
+        socs_complete[:,:,j] = np.take_along_axis(socs_complete[:,:,j], argsort, axis=1)
+    return initial_state, final_state, Ss_i, Ss_f, socs_complete
+
+
+def fix_absent_soc(data):
+    columns = data.columns.values
+    #check if at least one column contains soc_
+    if any('soc_' in i for i in columns):
+        return data
+    else:
+        singlets = [i.split('_')[1] for i in columns if 'e_s' in i]
+        triplets = [i.split('_')[1] for i in columns if 'e_t' in i]        
+        for ss in singlets:
+            for tt in triplets:
+                data[f'soc_{ss}_{tt}'] = 0
+    return data            
+
 ###CALCULATES ISC AND EMISSION RATES & SPECTRA#########################################
-def rates(initial,dielec,data=None,ensemble_average=False):
+def rates(initial,dielec,data=None,ensemble_average=False, detailed=False):
     if data is None:
         data        = gather_data(initial,save=True) 
         eps_i, nr_i = nemo.tools.get_nr()
         kbT         = nemo.tools.detect_sigma()
     else:
         eps_i  = data['eps'][0]
         nr_i   = data['nr'][0]
@@ -609,32 +656,41 @@
     alphast1   = nemo.tools.get_alpha(eps_i)
     alphast2   = nemo.tools.get_alpha(eps)  
     alphaopt1  = nemo.tools.get_alpha(nr_i**2)
     alphaopt2  = nemo.tools.get_alpha(nr**2)
     n_state    = int(initial[1:]) -1
     initial    = initial.lower()       
 
+    data = fix_absent_soc(data)    
+
+
     #Emission Calculations
-    lambda_be  = (alphast2/alphast1 - alphaopt2/alphast1)*data['gp']
+    lambda_be  = (alphast2/alphast1 - alphaopt2/alphast1)*data['gp'].to_numpy()
     Ltotal     = np.sqrt(2*lambda_be*kbT + kbT**2)
-    delta_emi  = data['e_'+initial] - (alphast2/alphaopt1)*data['d_'+initial]
-    if 's' in initial:
-        constante = ((nr**2)*(e**2)/(2*np.pi*hbar*mass*(c**3)*epsilon0))
-    elif 't' in initial:
-        constante = (1/3)*((nr**2)*(e**2)/(2*np.pi*hbar*mass*(c**3)*epsilon0))
-
-    espectro  = (constante*((delta_emi-lambda_be)**2)*data['osc'])
-    tdm       = nemo.tools.calc_tdm(data['osc'],data['e_'+initial],espectro)    
-    left      = max(min(delta_emi-2*Ltotal),0.01)
-    right     = max(delta_emi+2*Ltotal)    
-    x         = np.linspace(left,right, int((right-left)/0.01))
-    y         = espectro.to_numpy()[:,np.newaxis]*nemo.tools.gauss(x,delta_emi.to_numpy()[:,np.newaxis],Ltotal.to_numpy()[:,np.newaxis])
-    N         = y.shape[0]
-    mean_y    = np.sum(y,axis=0)/N 
-    error     = np.sqrt(np.sum((y-mean_y)**2,axis=0)/(N*(N-1))) 
+    energies   = data.filter(regex=f'^e_{initial[0]}').to_numpy()
+    delta_emi  = energies - (alphast2/alphaopt1)*data.filter(regex=f'^d_{initial[0]}').to_numpy()
+    constante  = ((nr**2)*(e**2)/(2*np.pi*hbar*mass*(c**3)*epsilon0))
+    if 't' in initial:
+        constante *= (1/3)
+    oscs        = data.filter(regex='^osce_').to_numpy()
+    argsort_emi = np.argsort(delta_emi, axis=1)
+    delta_emi   = np.take_along_axis(delta_emi, argsort_emi, axis=1)
+    oscs        = np.take_along_axis(oscs, argsort_emi, axis=1)
+    delta_emi   = delta_emi[:,n_state]
+    oscs        = oscs[:,n_state]
+    energies    = np.take_along_axis(energies, argsort_emi, axis=1)[:,n_state]
+    espectro    = (constante*((delta_emi-lambda_be)**2)*oscs)
+    tdm         = nemo.tools.calc_tdm(oscs,energies,espectro)    
+    left        = max(min(delta_emi-2*Ltotal),0.01)
+    right       = max(delta_emi+2*Ltotal)    
+    x           = np.linspace(left,right, int((right-left)/0.01))
+    y           = espectro[:,np.newaxis]*nemo.tools.gauss(x,delta_emi[:,np.newaxis],Ltotal[:,np.newaxis])
+    N           = y.shape[0]
+    mean_y      = np.sum(y,axis=0)/N 
+    error       = np.sqrt(np.sum((y-mean_y)**2,axis=0)/(N*(N-1))) 
     emi_rate, emi_error = nemo.tools.calc_emi_rate(x, mean_y,error)     
     gap_emi        = means(delta_emi,espectro,ensemble_average)    
     mean_sigma_emi = means(Ltotal,espectro,ensemble_average) 
     mean_part_emi  = (100/N)/means(espectro/np.sum(espectro),espectro,ensemble_average) 
     emi            = np.hstack((x[:,np.newaxis],mean_y[:,np.newaxis],error[:,np.newaxis]))
     emi            = pd.DataFrame(emi,columns=['Energy','Diffrate','Error'])
     emi.insert(0,'TDM',tdm)
@@ -643,50 +699,68 @@
     if data is None:
         N    = data.shape[0]
         coms = nemo.tools.start_counter()
         if N != coms:
             print(f"There are {coms} inputs and just {N} log files. Something is not right! Computing the rates anyway...")
     
     #Intersystem Crossing Rates
-    Singlets    =  data[[i for i in data.columns.values if 'e_s' in i]].to_numpy()
-    Triplets    =  data[[i for i in data.columns.values if 'e_t' in i]].to_numpy()
+    Singlets    =  data[[i for i in data.columns.values if 'e_s' in i and 'osc' not in i]].to_numpy()
+    Triplets    =  data[[i for i in data.columns.values if 'e_t' in i and 'osc' not in i]].to_numpy()
     Ss_s        =  data[[i for i in data.columns.values if 'd_s' in i]].to_numpy()
     Ss_t        =  data[[i for i in data.columns.values if 'd_t' in i]].to_numpy()
     if 's' in initial:
-        socs_complete =  data[[i for i in data.columns.values if 'soc_t' in i]].to_numpy()
-        delta    = Triplets + np.repeat((alphast2/alphaopt1)*Ss_s[:,n_state][:,np.newaxis] - Singlets[:,n_state][:,np.newaxis],Triplets.shape[1],axis=1) - (alphaopt2/alphaopt1)*Ss_t   #Tn (final) - Sm (initial) + lambda_b
+        initial_state = Singlets - (alphast2/alphaopt1)*Ss_s
+        final_state   = Triplets - (alphaopt2/alphaopt1)*Ss_t
+        socs_complete = data[[i for i in data.columns.values if f'soc_s' in i]].to_numpy()
+        initial_state, final_state, Ss_s, Ss_t, socs_complete = reorder(initial_state, final_state, Ss_s, Ss_t, socs_complete)
+        initial_state = initial_state[:,n_state]
+        socs_complete = socs_complete[:,n_state,:]
+        delta = final_state - np.repeat(initial_state[:,np.newaxis],final_state.shape[1],axis=1)
         lambda_b = (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_t
-        final    = [i.upper()[4:] for i in data.columns.values if 'soc_t' in i]
+        final    = [i.split('_')[2].upper() for i in data.columns.values if 'soc_s1' in i]
         ##FOR WHEN IC IS AVAILABLE
         #socs_complete = np.hstack((socs_complete,0.0001*np.ones((Singlets.shape[0],Singlets.shape[1]-1))))
         #delta_ss = Singlets + np.repeat((alphast2/alphaopt1)*Ss_s[:,n_state][:,np.newaxis] - Singlets[:,n_state][:,np.newaxis],Singlets.shape[1],axis=1) - (alphaopt2/alphaopt1)*Ss_s    #Sm (final) - Sn (initial) + lambda_b
         #indices  = [i for i in range(Singlets.shape[1]) if i != n_state] #Removed Sn to Sn transfers
         #delta    = np.hstack((delta,delta_ss[:,indices]))
         #lambda_bt= (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_s
         #lambda_b = np.hstack((lambda_b,lambda_bt[:,indices]))
     elif 't' in initial: 
         #Tn to Sm ISC
-        socs_complete =  data[[i for i in data.columns.values if 'soc_s' in i and 'soc_s0' not in i]].to_numpy()
-        delta         = Singlets + np.repeat((alphast2/alphaopt1)*Ss_t[:,n_state][:,np.newaxis] - Triplets[:,n_state][:,np.newaxis],Singlets.shape[1],axis=1) - (alphaopt2/alphaopt1)*Ss_s    #Sm (final) - Tn (initial) + lambda_b
-        lambda_b      = (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_s
-        socs_s0       = data['soc_s0'].to_numpy()[:,np.newaxis]
-        socs_complete = np.hstack((socs_s0,socs_complete))
-        delta         = np.hstack((delta_emi.to_numpy()[:,np.newaxis],delta))
-        lambda_b      = np.hstack((lambda_be.to_numpy()[:,np.newaxis],lambda_b))
-        final         = [i.upper()[4:] for i in data.columns.values if 'soc_s' in i]
+        initial_state = Triplets - (alphast2/alphaopt1)*Ss_t
+        final_state = Singlets - (alphaopt2/alphaopt1)*Ss_s
+        socs_complete =  data[[i for i in data.columns.values if 'soc_t' in i and 's0' not in i and i.count('t') == 1]].to_numpy()
+        initial_state, final_state, Ss_t, Ss_s, socs_complete = reorder(initial_state, final_state, Ss_t, Ss_s, socs_complete)
+        initial_state = initial_state[:,n_state]
+        socs_complete = socs_complete[:,n_state,:]
+        delta = final_state - np.repeat(initial_state[:,np.newaxis],final_state.shape[1],axis=1)
+        lambda_b = (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_s
+        final    = [i.split('_')[2].upper() for i in data.columns.values if 'soc_t1' in i and i.count('t') == 1]
+        #Tn to S0 ISC
+        socs_s0 = data[[i for i in data.columns.values if f'soc_t' in i and 's0' in i]].to_numpy()
+        socs_s0 = np.take_along_axis(socs_s0, argsort_emi, axis=1)
+        socs_s0 = socs_s0[:,n_state]
+        socs_complete = np.hstack((socs_s0[:,np.newaxis],socs_complete))
+        delta = np.hstack((delta_emi[:,np.newaxis],delta))
+        lambda_b = np.hstack((lambda_be[:,np.newaxis],lambda_b))
         #Tn to Tm ISC
         #delta_tt = Triplets + np.repeat((alphast2/alphaopt1)*Ss_t[:,n_state][:,np.newaxis] - Triplets[:,n_state][:,np.newaxis],Triplets.shape[1],axis=1) - (alphaopt2/alphaopt1)*Ss_t    #Tm (final) - Tn (initial) + lambda_b
         #indices  = [i for i in range(Triplets.shape[1]) if i != n_state] #Removed Tn to Tn transfers
         #delta    = np.hstack((delta,delta_tt[:,indices]))
         #lambda_bt= (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_t
         #lambda_b = np.hstack((lambda_b,lambda_bt[:,indices]))
         #final.extend([i.upper()[4:] for i in data.columns.values if 'soc_t' in i])
 
+
+
     sigma = np.sqrt(2*lambda_b*kbT + kbT**2)
     y     = (2*np.pi/hbar)*(socs_complete**2)*nemo.tools.gauss(delta,0,sigma)
+    # hstack y and espectro
+    individual = np.hstack((espectro[:,np.newaxis],y))
+    individual /= individual.shape[0]
     N     = y.shape[0]
     rate  = np.sum(y,axis=0)/N
     total = emi_rate + np.sum(rate)
     #Error estimate
     error = np.sqrt(np.sum((y-rate)**2,axis=0)/(N*(N-1)))  
     
     results    = np.array([[emi_rate,emi_error,100*emi_rate/total,gap_emi,np.nan,mean_sigma_emi,mean_part_emi]])
@@ -695,24 +769,37 @@
     mean_sigma = means(sigma,y,ensemble_average)[:,np.newaxis]
     with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             mean_part  = np.nan_to_num(100*rate/means(y,y,ensemble_average))
     rate       = rate[:,np.newaxis]
     error      = error[:,np.newaxis]
     labels = [f'{initial.upper()}->S0'] + [f'{initial.upper()}~>{j}' for j in final]
+
+
+    # make a dataframe with Ss_s and Ss_t
+    breakdown = pd.DataFrame(np.hstack((Ss_s/alphaopt1,Ss_t/alphaopt1)),columns=[f'chi_s{i+1}' for i in range(Ss_s.shape[1])] + [f'chi_t{i+1}' for i in range(Ss_t.shape[1])])
+    # append a columns with energies named eng
+    breakdown['eng'] = delta_emi
+    breakdown['sigma'] = Ltotal
+    # append individual to df, use labels as columns
+    breakdown = pd.concat([breakdown,pd.DataFrame(individual,columns=labels)],axis=1)
+    
     labels = np.array(labels)
     results_isc = np.hstack((rate,error,100*rate/total,mean_gap,mean_soc,mean_sigma,mean_part[:,np.newaxis])) 
     results = np.vstack((results,results_isc))
     results = pd.DataFrame(results,columns=['Rate(s^-1)','Error(s^-1)','Prob(%)','AvgDE+L(eV)','AvgSOC(meV)','AvgSigma(eV)','AvgConc(%)'])
     results.insert(0,'Transition',labels)
-    return results, emi       
+    if detailed:
+        return results, emi, breakdown
+    else:
+        return results, emi    
 #########################################################################################    
 
 ###COMPUTES ABSORPTION SPECTRA########################################################### 
-def absorption(initial,dielec,data=None, save=False):
+def absorption(initial,dielec,data=None, save=False, detailed=False):
     if data is None:
         data        = gather_data(initial,save=True) 
         eps_i, nr_i = nemo.tools.get_nr()
         kbT         = nemo.tools.detect_sigma()
     else:
         eps_i  = data['eps'][0]
         nr_i   = data['nr'][0]
@@ -720,55 +807,86 @@
     eps, nr    = dielec[0], dielec[1]
     alphast1   = nemo.tools.get_alpha(eps_i)
     alphast2   = nemo.tools.get_alpha(eps)  
     alphaopt1  = nemo.tools.get_alpha(nr_i**2)
     alphaopt2  = nemo.tools.get_alpha(nr**2)
     initial    = initial.lower()
     constante  = (np.pi*(e**2)*hbar)/(2*nr*mass*c*epsilon0)*1e20
+    spin = initial[0]
     if initial == 's0':
-        engs = [i for i in data.columns if 'e_s' in i]
+        engs = [i for i in data.columns if 'e_s' in i and 'osc' not in i]
         ds   = [i for i in data.columns if 'd_s' in i]
         oscs = [i for i in data.columns if 'osc_s' in i]
         oscs = data[oscs].values
         engs = data[engs].values
         ds   = data[ds].values
         lambda_b = (alphast2/alphaopt1 - alphaopt2/alphaopt1)*ds
         DE   = engs - (alphaopt2/alphaopt1)*ds
     else:
-        spin = initial[0]
         num  = int(initial[1:])
-        engs = [i for i in data.columns if f'e_{spin}' in i]
+        engs = [i for i in data.columns if f'e_{spin}' in i and 'osc' not in i]
         engs = [i for i in engs if int(i.split('_')[1][1:]) > num]
         ds   = [i for i in data.columns if f'd_{spin}' in i]
         ds   = [i for i in ds if int(i.split('_')[1][1:]) > num]
         oscs = [i for i in data.columns if 'osc_' in i]
         oscs = [i for i in oscs if int(i.split('_')[1][1:]) > num]
         base = data[f'e_{initial}'].values[:,np.newaxis]
         bs   = data[f'd_{initial}'].values[:,np.newaxis]
         engs = data[engs].values
         ds   = data[ds].values
         oscs = data[oscs].values
         lambda_b = (alphast2/alphaopt1 - alphaopt2/alphaopt1)*ds
         DE   = engs - (alphaopt2/alphaopt1)*ds - np.repeat(base -(alphast2/alphaopt1)*bs,engs.shape[1],axis=1)  
-    lambda_b = lambda_b.flatten()
-    DE       = DE.flatten()
-    oscs     = oscs.flatten()
+    # Sorting states by energy
+    argsort = np.argsort(DE,axis=1)
+    DE      = np.take_along_axis(DE,argsort,axis=1)
+    oscs    = np.take_along_axis(oscs,argsort,axis=1)
+    lambda_b= np.take_along_axis(lambda_b,argsort,axis=1)
+    ds      = np.take_along_axis(ds,argsort,axis=1)	
     Ltotal = np.sqrt(2*lambda_b*kbT + kbT**2)
-    left   = max(min(DE-2*Ltotal),0.01)
-    right  = max(DE+2*Ltotal)    
+    left   = max(np.min(DE-2*Ltotal),0.01)
+    right  = np.max(DE+2*Ltotal)    
     x      = np.linspace(left,right,int((right-left)/0.01))
-    y      = constante*oscs[:,np.newaxis]*nemo.tools.gauss(x,(DE+lambda_b)[:,np.newaxis],Ltotal[:,np.newaxis])
+    # Add extra dimension to DE and Ltotal to match x shape
+    DE      = DE[:,:,np.newaxis]
+    Ltotal  = Ltotal[:,:,np.newaxis]
+    oscs  = oscs[:,:,np.newaxis]
+    lambda_b = lambda_b[:,:,np.newaxis]
+    y      = constante*oscs*nemo.tools.gauss(x,(DE+lambda_b),Ltotal)
     N      = oscs.shape[0]
     mean_y = np.sum(y,axis=0)/N 
     #Error estimate
     sigma    = np.sqrt(np.sum((y-mean_y)**2,axis=0)/(N*(N-1))) 
+    mean_y = mean_y.T
+    sigma  = sigma.T
+    total = np.sum(mean_y,axis=1)
+    sigma = np.sum(sigma,axis=1)
+    #append total to mean_y
+    mean_y = np.append(mean_y,total[:,np.newaxis],axis=1)
+
+    # make dataframe
+    labels = [initial[0].upper()+str(int(initial[1:])+i+1) for i in range(0,mean_y.shape[1]-1)]
+    labels += ['Total','Error']
+    labels = ['Energy'] + labels
+    abs_spec = pd.DataFrame(np.hstack((x[:,np.newaxis],mean_y,sigma[:,np.newaxis])),columns=labels)
+    
     if save:
         arquivo  = nemo.tools.naming(f'cross_section_{initial.upper()}_.lx')
-        primeira = f"{'#Energy(ev)':8s} {'cross_section(A^2)':8s} {'error(A^2)':8s}\n# Absorption from State: {initial.upper()}\n#Epsilon: {eps:.3f} nr: {nr:.3f}\n"
-        with open(arquivo, 'w') as f:
-            f.write(primeira)
-            for i in range(0,len(x)):
-                text = f"{x[i]:.6f} {mean_y[i]:.6e} {sigma[i]:.6e}\n"
-                f.write(text)
+        primeira = f"{'Energy(ev)':8s} {'cross_section(A^2)':8s} {'error(A^2)':8s}\nAbsorption from State: {initial.upper()}\nEpsilon: {eps:.3f} nr: {nr:.3f}\n"
+        labels = ['{:14s}'.format(i) for i in labels]
+        primeira += ' '.join(labels)
+        fmt = ['%14.6e' for i in range(0,mean_y.shape[1])]
+        fmt = ' '.join(fmt)
+        np.savetxt(arquivo, np.hstack((x[:,np.newaxis],mean_y,sigma[:,np.newaxis])), fmt='%14.6f '+ fmt +' %14.6e', header=primeira)
         print(f'Spectrum printed in the {arquivo} file')
-    return np.hstack((x[:,np.newaxis],mean_y[:,np.newaxis],sigma[:,np.newaxis]))                 
+
+    # concatenate oscs[:,:,0] with DE[:,:,0] and ds
+    colunas = [f'{initial.upper()}->{spin.upper()}{i}' for i in range(int(initial[1:])+1,int(initial[1:])+oscs.shape[1]+1)]
+    colunas += [f'eng_{spin}{i}' for i in range(int(initial[1:])+1,int(initial[1:])+DE.shape[1]+1)]
+    colunas += [f'chi_{spin}{i}' for i in range(int(initial[1:])+1,int(initial[1:])+ds.shape[1]+1)]
+    # concatenate oscs[:,:,0] with DE[:,:,0] and ds
+    breakdown = pd.DataFrame(np.hstack((oscs[:,:,0],(DE+lambda_b)[:,:,0],ds/alphaopt1)),columns=colunas)
+    if detailed:
+        return abs_spec, breakdown
+    else:
+        return abs_spec          
 #########################################################################################
```

### Comparing `nemophoto-0.4.0/nemo/batch_lx.py` & `nemophoto-0.5.0/nemo/batch_lx.py`

 * *Files identical despite different names*

### Comparing `nemophoto-0.4.0/nemo/tools.py` & `nemophoto-0.5.0/nemo/tools.py`

 * *Files identical despite different names*

### Comparing `nemophoto-0.4.0/nemophoto.egg-info/PKG-INFO` & `nemophoto-0.5.0/nemophoto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nemophoto
-Version: 0.4.0
+Version: 0.5.0
 Summary: Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.
 Home-page: https://github.com/LeonardoESousa/NEMO
 Author: Leonardo Evaristo de Sousa
 Author-email: ledso@dtu.dk
 License: MIT
 Description: 
         # NEMO - Photophysics with the Nuclear Ensemble Method
         
         [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
         [![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
         [![down](https://img.shields.io/pypi/dm/nemophoto)]()
-        [![maint](https://img.shields.io/maintenance/yes/2021)]()
+        [![maint](https://img.shields.io/maintenance/yes/2023)]()
         [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
         
         
          Fluorescence, phosphorescence and intersystem crossing (ISC) rate calculations. Absorption, fluorescence and phosphorescence spectrum simulations. Förster radius and singlet exciton diffusion length estimates. Interfaces with the QChem package. 
         
         Table of Contents
         =================
@@ -62,26 +62,28 @@
         
         ## How to install it?
         
         Run:
         
         `pip install nemophoto`
         
-        To get the latest commit run:
+        To get the latest commit, run:
         
         `pip install git+https://github.com/LeonardoESousa/NEMO`
         
         Alternatively, clone the repository to your computer. Inside the NEMO folder, run:
         
         `pip install .`
         
         Once installed, you should be able to run the program from any folder by just using the `nemo` command.
         
         ## How to use it?
         
+        Here is a quick guide on how to use the software. For a detailed tutorial, click [here](https://github.com/LeonardoESousa/NEMO/blob/main/Tutorial/Tutorial.md).
+        
         1. Initial steps:
             - Create a folder for your project. Add the log file for the frequency calculation to your folder. If the frequency calculation was run with Gaussian, you must also provide a QChem input file containing some settings you wish to apply in the ensemble calculations (e.g. functional, basis set, omega value, charge and multiplicity etc). An example of such file (td.in) is provided [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples).
             - A frequency calculation in the S0 state is suitable for computing an absorption spectrum. For fluorescence spectra and/or ISC rates calculations from Sn states to triplet states, a Sn frequency calculation is expected. Finally, for phosphorescence spectra and/or rISC rates calculations from Tn states to singlet states, a Tn frequency calculation is expected.  
             - Run the `nemo` command. Choose option 1 and follow the instructions to select the parameters of the calculation. This includes the dielectric constant and refractive index of the medium. This information will be used to obtain state-specific solvent corrections to the TD(A)-DFT energies.  
             - Add a bash script file to the folder. This file depends on which batch system you use. Examples of this file for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples)).
             - Run the `nemo` command again, choose option 2 and follow the instructions. Alternatively, just run all calculations created in the Geometries folder. Once the calculations are running, you may use option 3 to check the progress or option 4 to abort.
         
@@ -94,14 +96,15 @@
         4. IMPORTANT:
             - You may choose to calculate spectra and rates with different solvent dielectric constant and refractive index than the ones selected as input in Option 1. To do so, NEMO will resort to the extrapolation procedure described in ADD PAPER to adjust the results to the new solvent. 
         
         5. For exciton properties:
             - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. Copy both spectra to a folder and inside this folder run the `nemo` command. Choose option 7. Follow the instructions to set the calculation parameters. A file will be generated with all the information. Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. These estimations follow from the procedures described in: "de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071." 
         
         
+        For better visualization of results, consider using  [Nemoview](https://github.com/LeonardoESousa/nemoview). 
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `nemophoto-0.4.0/setup.py` & `nemophoto-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nemophoto'
 DESCRIPTION = 'Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.'
 URL = 'https://github.com/LeonardoESousa/NEMO'
 EMAIL = 'ledso@dtu.dk'
 AUTHOR = 'Leonardo Evaristo de Sousa'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.4.0'
+VERSION = '0.5.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['numpy', 'scipy', 'pandas', 'LeoX']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

