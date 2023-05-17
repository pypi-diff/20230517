# Comparing `tmp/fpcmci-4.1.2.tar.gz` & `tmp/fpcmci-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpcmci-4.1.2.tar", last modified: Fri Feb  3 14:45:44 2023, max compression
+gzip compressed data, was "fpcmci-4.2.0.tar", last modified: Wed May 17 10:40:17 2023, max compression
```

## Comparing `fpcmci-4.1.2.tar` & `fpcmci-4.2.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-02-03 14:45:44.987017 fpcmci-4.1.2/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)    35142 2022-11-24 12:07:21.000000 fpcmci-4.1.2/LICENCE.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     6311 2023-02-03 14:45:44.987017 fpcmci-4.1.2/PKG-INFO
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     5702 2023-02-03 14:43:01.000000 fpcmci-4.1.2/README.md
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-02-03 14:45:44.983017 fpcmci-4.1.2/fpcmci/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1066 2022-11-24 12:07:21.000000 fpcmci-4.1.2/fpcmci/CPrinter.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)    15780 2023-01-09 12:03:44.000000 fpcmci-4.1.2/fpcmci/FPCMCI.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)    10295 2022-12-29 14:46:23.000000 fpcmci-4.1.2/fpcmci/PCMCI.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      240 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/__init__.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-02-03 14:45:44.983017 fpcmci-4.1.2/fpcmci/basics/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)       72 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/basics/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      401 2022-11-29 14:56:46.000000 fpcmci-4.1.2/fpcmci/basics/constants.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      506 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/basics/logger.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1235 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/basics/utils.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     8598 2022-12-29 14:46:23.000000 fpcmci-4.1.2/fpcmci/causal_graph.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-02-03 14:45:44.983017 fpcmci-4.1.2/fpcmci/preprocessing/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2304 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/Subsampler.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)        0 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     4568 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/data.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-02-03 14:45:44.983017 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3649 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      639 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/Static.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      781 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1798 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2600 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1765 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/WSStatic.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      267 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2493 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/moving_window.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-02-03 14:45:44.987017 fpcmci-4.1.2/fpcmci/selection_methods/
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1402 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/selection_methods/Corr.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2222 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/selection_methods/MI.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     2700 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/selection_methods/ParCorr.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3791 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/selection_methods/SelectionMethod.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     3805 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/selection_methods/TE.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)      134 2022-11-24 17:04:58.000000 fpcmci-4.1.2/fpcmci/selection_methods/__init__.py
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)       17 2023-02-03 14:45:37.000000 fpcmci-4.1.2/fpcmci/version.py
-drwxrwxr-x   0 lcastri   (1000) lcastri   (1000)        0 2023-02-03 14:45:44.983017 fpcmci-4.1.2/fpcmci.egg-info/
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     6311 2023-02-03 14:45:44.000000 fpcmci-4.1.2/fpcmci.egg-info/PKG-INFO
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)     1150 2023-02-03 14:45:44.000000 fpcmci-4.1.2/fpcmci.egg-info/SOURCES.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        1 2023-02-03 14:45:44.000000 fpcmci-4.1.2/fpcmci.egg-info/dependency_links.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)      154 2023-02-03 14:45:44.000000 fpcmci-4.1.2/fpcmci.egg-info/requires.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)        7 2023-02-03 14:45:44.000000 fpcmci-4.1.2/fpcmci.egg-info/top_level.txt
--rw-rw-r--   0 lcastri   (1000) lcastri   (1000)       38 2023-02-03 14:45:44.987017 fpcmci-4.1.2/setup.cfg
--rw-r--r--   0 lcastri   (1000) lcastri   (1000)     1415 2022-12-29 14:46:23.000000 fpcmci-4.1.2/setup.py
+drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 10:40:17.332130 fpcmci-4.2.0/
+-rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)     8316 2023-05-17 10:40:17.332130 fpcmci-4.2.0/PKG-INFO
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     6610 2023-05-17 10:36:55.000000 fpcmci-4.2.0/README.md
+drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 10:40:17.328130 fpcmci-4.2.0/fpcmci/
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1066 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/CPrinter.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)    16932 2023-05-17 09:58:42.000000 fpcmci-4.2.0/fpcmci/FPCMCI.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)    10260 2023-05-17 09:34:09.000000 fpcmci-4.2.0/fpcmci/PCMCI.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      240 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/__init__.py
+drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 10:40:17.328130 fpcmci-4.2.0/fpcmci/basics/
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)       72 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/basics/__init__.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      401 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/basics/constants.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      506 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/basics/logger.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1235 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/basics/utils.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     8598 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/causal_graph.py
+drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 10:40:17.328130 fpcmci-4.2.0/fpcmci/preprocessing/
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2304 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/Subsampler.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)        0 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/__init__.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     4568 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/data.py
+drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 10:40:17.332130 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     3649 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      639 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/Static.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      781 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1798 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/WSDynamic.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2600 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1765 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/WSStatic.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      267 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/__init__.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2493 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/moving_window.py
+drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 10:40:17.332130 fpcmci-4.2.0/fpcmci/selection_methods/
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1402 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/selection_methods/Corr.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2222 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/selection_methods/MI.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     2700 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/selection_methods/ParCorr.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     3791 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/selection_methods/SelectionMethod.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     3805 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/selection_methods/TE.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)      134 2023-03-03 16:48:10.000000 fpcmci-4.2.0/fpcmci/selection_methods/__init__.py
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)       17 2023-05-17 10:20:12.000000 fpcmci-4.2.0/fpcmci/version.py
+drwxrwxr-x   0 lucacastri  (1000) lucacastri  (1000)        0 2023-05-17 10:40:17.328130 fpcmci-4.2.0/fpcmci.egg-info/
+-rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)     8316 2023-05-17 10:40:17.000000 fpcmci-4.2.0/fpcmci.egg-info/PKG-INFO
+-rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)     1138 2023-05-17 10:40:17.000000 fpcmci-4.2.0/fpcmci.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)        1 2023-05-17 10:40:17.000000 fpcmci-4.2.0/fpcmci.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)      154 2023-05-17 10:40:17.000000 fpcmci-4.2.0/fpcmci.egg-info/requires.txt
+-rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)        7 2023-05-17 10:40:17.000000 fpcmci-4.2.0/fpcmci.egg-info/top_level.txt
+-rw-rw-r--   0 lucacastri  (1000) lucacastri  (1000)       38 2023-05-17 10:40:17.332130 fpcmci-4.2.0/setup.cfg
+-rw-r--r--   0 lucacastri  (1000) lucacastri  (1000)     1415 2023-05-17 10:20:14.000000 fpcmci-4.2.0/setup.py
```

### Comparing `fpcmci-4.1.2/PKG-INFO` & `fpcmci-4.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: fpcmci
-Version: 4.1.2
-Summary: A causal discovery Python package
-Home-page: https://github.com/lcastri/fpcmci
-Author: Luca Castri
-Author-email: lucacastri94@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
 # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
 
 Extension of the state-of-the-art causal discovery method [PCMCI](https://github.com/jakobrunge/tigramite) augmented with a feature-selection method based on Transfer Entropy. The algorithm, starting from a prefixed set of variables, identifies the correct subset of features and possible links between them which describe the observed process. Then, from the selected features and links, a causal model is built.
 
 
 ## Useful links
 
@@ -79,55 +61,80 @@
     year={2023},
 }
 ```
 
 
 ## Requirements
 
-* tigramite==5.1.0.3
-* pandas==1.5.2
+* tigramite>=5.1.0.3
+* pandas>=1.5.2
 * netgraph>=4.10.2
 * networkx>=2.8.6
-* ruptures==1.1.7
-* scikit_learn==1.1.3
+* ruptures>=1.1.7
+* scikit_learn>=1.1.3
 * torch>=1.11.0
-* gpytorch>=1.4       
+* gpytorch>=1.4
 * dcor>=0.5.3
-* h5py==3.7.0   
+* h5py>=3.7.0   
 
 
 ## Installation
 
-Before installing the FPCMCI package, you need to install the [IDTxl package](https://github.com/pwollstadt/IDTxl) used for the feature-selection process, following the guide described [here](https://github.com/pwollstadt/IDTxl/wiki/Installation-and-Requirements). Once complete, you can install the current release of `FPCMCI` with:
+Before installing the FPCMCI package, you need to install Java and the [IDTxl package](https://github.com/pwollstadt/IDTxl) used for the feature-selection process, following the guide described [here](https://github.com/pwollstadt/IDTxl/wiki/Installation-and-Requirements). Once complete, you can install the current release of `FPCMCI` with:
 ``` shell
 pip install fpcmci
 ```
 
-For a complete installation (IDTxl and FPCMCI) you can run the following commands:
+For a complete installation Java - IDTxl - FPCMCI, follow the following procedure.
+
+### 1 - Java installation
+Verify that you have not already installed Java:
+```shell
+java -version
+```
+if the latter returns `Command 'java' not found, ...`, you can install Java by the following commands, otherwise you can jump to IDTxl installation.
+```shell
+# Java
+sudo apt-get update
+sudo apt install default-jdk
+```
+
+Then, you need to add JAVA_HOME to the environment
+```shell
+sudo nano /etc/environment
+JAVA_HOME="/lib/jvm/java-11-openjdk-amd64/bin/java" # Paste the JAVA_HOME assignment at the bottom of the file
+source /etc/environment
+```
+
+### 2 - IDTxl installation
 ```shell
 # IDTxl
 git clone https://github.com/pwollstadt/IDTxl.git
-conda create --name fpcmci python=3 pip matplotlib h5py scipy networkx
+conda create --name fpcmci python=3.8 pip matplotlib h5py scipy networkx
 conda activate fpcmci
 conda install -c conda-forge jpype1    # required by CPU JIDT estimators
 conda install -c conda-forge pyopencl  # required by GPU OpenCL estimators
 conda install -c anaconda ecos         # required by Tartu PID estimator
 conda install numba                    # required by NumbaCuda estimators
 conda install cudatoolkit              # required by NumbaCuda estimators
 conda install mpmath
 
 cd IDTxl
 pip install -e .
+```
 
-# FPCMCI
+### 3 - FPCMCI installation
+```shell
 pip install fpcmci
 ```
 
 
 ## Recent changes
 
-* 4.1.2 tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI
-* 4.1.1 PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model
-* 4.1.0 FSelector and FValidator turned into FPCMCI and PCMCI, show_edge_label removed and dag optimized, new package included in the setup.py, added tutorials, and new example in README.md. 
-* 4.0.1 online documentation and paths fixes.
-* 4.0.0 package published.
-
+| Version | Changes |
+| :---: | ----------- |
+| 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
+| 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
+| 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
+| 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
+| 4.0.1 | online documentation and paths fixes |
+| 4.0.0 | package published |
```

### Comparing `fpcmci-4.1.2/README.md` & `fpcmci-4.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,156 @@
-# <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
-
-Extension of the state-of-the-art causal discovery method [PCMCI](https://github.com/jakobrunge/tigramite) augmented with a feature-selection method based on Transfer Entropy. The algorithm, starting from a prefixed set of variables, identifies the correct subset of features and possible links between them which describe the observed process. Then, from the selected features and links, a causal model is built.
-
-
-## Useful links
-
-* [Documentation](https://lcastri.github.io/fpcmci/)
-* [Tutorials](https://github.com/lcastri/fpcmci/tree/main/tutorials)
-
-
-## Why FPCMCI?
-
-Current state-of-the-art causal discovery approaches suffer in terms of speed and accuracy of the causal analysis when the process to be analysed is composed by a large number of features. FPCMCI is able to select the most meaningful features from a set of variables and build a causal model from such selection. To this end, the causal analysis results **faster** and **more accurate**.
-
-In the following it is presented an example showing a comparison between causal models obtained by PCMCI and FPCMCI causal discovery algorithms on the same data. The latter have been created by defining a 6-variables system defined as follows:
-
-``` python
-min_lag = 1
-max_lag = 1
-np.random.seed(1)
-nsample = 1500
-nfeature = 6
-
-d = np.random.random(size = (nsample, feature))
-for t in range(max_lag, nsample):
-  d[t, 0] += 2 * d[t-1, 1] + 3 * d[t-1, 3]
-  d[t, 2] += 1.1 * d[t-1, 1]**2
-  d[t, 3] += d[t-1, 3] * d[t-1, 2]
-  d[t, 4] += d[t-1, 4] + d[t-1, 5] * d[t-1, 0]
-```
-
-Causal Model by PCMCI       |  Causal Model by FPCMCI 
-:-------------------------:|:-------------------------:
-![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_1.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_1.png "Causal model by FPCMCI")
-Execution time ~ 6min 50sec | Execution time ~ 2min 45sec
-
-The causal analysis performed by the **FPCMCI** results not only faster but also more accurate. Indeed, the causal model derived by the FPCMCI agrees with the structure of the system of equations, instead the one derived by the PCMCI presents spurious links:
-* $X_2$ &rarr; $X_4$
-* $X_2$ &rarr; $X_5$
-
-Note that, since all the 6 variables were involved in the evolution of the system, the FPCMCI did not remove any of them. In the following example instead, we added a new variable in the system which is defined just by the noise component (as $X_1$ and $X_5$) and does not appear in any other equation, defined as follows: $X_6(t) = \eta_6(t)$. In the following the comparison between PCMCI and FPCMCI with this new system configuration:
-
-Causal Model by PCMCI       |  Causal Model by FPCMCI 
-:-------------------------:|:-------------------------:
-![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_2.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_2.png "Causal model by FPCMCI")
-Execution time ~ 8min 40sec | Execution time ~ 3min 00sec
-
-In this case the FPCMCI removes the $X_6$ variable from the causal graph leading to generate exactly the same causal model as in the previous example, with comparable executional time. Instead, the PCMCI suffers the presence of $X_6$ in terms of time and accuracy of the causal structure.
-Indeed, a spurious link $X_6$ &rarr; $X_5$ appears in the causal graph derived by the PCMCI.
-
-
-## Citation
-
-If you found this useful for your work, please cite this papers:
-```
-@inproceedings{castri2023fpcmci,
-    title={Enhancing Causal Discovery from Robot Sensor Data in Dynamic Scenarios},
-    author={Castri, Luca and Mghames, Sariah and Hanheide, Marc and Bellotto, Nicola},
-    booktitle={Conference on Causal Learning and Reasoning (CLeaR)},
-    year={2023},
-}
-```
-
-
-## Requirements
-
-* tigramite==5.1.0.3
-* pandas==1.5.2
-* netgraph>=4.10.2
-* networkx>=2.8.6
-* ruptures==1.1.7
-* scikit_learn==1.1.3
-* torch>=1.11.0
-* gpytorch>=1.4       
-* dcor>=0.5.3
-* h5py==3.7.0   
-
-
-## Installation
-
-Before installing the FPCMCI package, you need to install the [IDTxl package](https://github.com/pwollstadt/IDTxl) used for the feature-selection process, following the guide described [here](https://github.com/pwollstadt/IDTxl/wiki/Installation-and-Requirements). Once complete, you can install the current release of `FPCMCI` with:
-``` shell
-pip install fpcmci
-```
-
-For a complete installation (IDTxl and FPCMCI) you can run the following commands:
-```shell
-# IDTxl
-git clone https://github.com/pwollstadt/IDTxl.git
-conda create --name fpcmci python=3 pip matplotlib h5py scipy networkx
-conda activate fpcmci
-conda install -c conda-forge jpype1    # required by CPU JIDT estimators
-conda install -c conda-forge pyopencl  # required by GPU OpenCL estimators
-conda install -c anaconda ecos         # required by Tartu PID estimator
-conda install numba                    # required by NumbaCuda estimators
-conda install cudatoolkit              # required by NumbaCuda estimators
-conda install mpmath
-
-cd IDTxl
-pip install -e .
-
-# FPCMCI
-pip install fpcmci
-```
-
-
-## Recent changes
-
-* 4.1.2 tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI
-* 4.1.1 PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model
-* 4.1.0 FSelector and FValidator turned into FPCMCI and PCMCI, show_edge_label removed and dag optimized, new package included in the setup.py, added tutorials, and new example in README.md. 
-* 4.0.1 online documentation and paths fixes.
-* 4.0.0 package published.
+Metadata-Version: 2.1
+Name: fpcmci
+Version: 4.2.0
+Summary: A causal discovery Python package
+Home-page: https://github.com/lcastri/fpcmci
+Author: Luca Castri
+Author-email: lucacastri94@gmail.com
+License: UNKNOWN
+Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
+        
+        Extension of the state-of-the-art causal discovery method [PCMCI](https://github.com/jakobrunge/tigramite) augmented with a feature-selection method based on Transfer Entropy. The algorithm, starting from a prefixed set of variables, identifies the correct subset of features and possible links between them which describe the observed process. Then, from the selected features and links, a causal model is built.
+        
+        
+        ## Useful links
+        
+        * [Documentation](https://lcastri.github.io/fpcmci/)
+        * [Tutorials](https://github.com/lcastri/fpcmci/tree/main/tutorials)
+        
+        
+        ## Why FPCMCI?
+        
+        Current state-of-the-art causal discovery approaches suffer in terms of speed and accuracy of the causal analysis when the process to be analysed is composed by a large number of features. FPCMCI is able to select the most meaningful features from a set of variables and build a causal model from such selection. To this end, the causal analysis results **faster** and **more accurate**.
+        
+        In the following it is presented an example showing a comparison between causal models obtained by PCMCI and FPCMCI causal discovery algorithms on the same data. The latter have been created by defining a 6-variables system defined as follows:
+        
+        ``` python
+        min_lag = 1
+        max_lag = 1
+        np.random.seed(1)
+        nsample = 1500
+        nfeature = 6
+        
+        d = np.random.random(size = (nsample, feature))
+        for t in range(max_lag, nsample):
+          d[t, 0] += 2 * d[t-1, 1] + 3 * d[t-1, 3]
+          d[t, 2] += 1.1 * d[t-1, 1]**2
+          d[t, 3] += d[t-1, 3] * d[t-1, 2]
+          d[t, 4] += d[t-1, 4] + d[t-1, 5] * d[t-1, 0]
+        ```
+        
+        Causal Model by PCMCI       |  Causal Model by FPCMCI 
+        :-------------------------:|:-------------------------:
+        ![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_1.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_1.png "Causal model by FPCMCI")
+        Execution time ~ 6min 50sec | Execution time ~ 2min 45sec
+        
+        The causal analysis performed by the **FPCMCI** results not only faster but also more accurate. Indeed, the causal model derived by the FPCMCI agrees with the structure of the system of equations, instead the one derived by the PCMCI presents spurious links:
+        * $X_2$ &rarr; $X_4$
+        * $X_2$ &rarr; $X_5$
+        
+        Note that, since all the 6 variables were involved in the evolution of the system, the FPCMCI did not remove any of them. In the following example instead, we added a new variable in the system which is defined just by the noise component (as $X_1$ and $X_5$) and does not appear in any other equation, defined as follows: $X_6(t) = \eta_6(t)$. In the following the comparison between PCMCI and FPCMCI with this new system configuration:
+        
+        Causal Model by PCMCI       |  Causal Model by FPCMCI 
+        :-------------------------:|:-------------------------:
+        ![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_2.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_2.png "Causal model by FPCMCI")
+        Execution time ~ 8min 40sec | Execution time ~ 3min 00sec
+        
+        In this case the FPCMCI removes the $X_6$ variable from the causal graph leading to generate exactly the same causal model as in the previous example, with comparable executional time. Instead, the PCMCI suffers the presence of $X_6$ in terms of time and accuracy of the causal structure.
+        Indeed, a spurious link $X_6$ &rarr; $X_5$ appears in the causal graph derived by the PCMCI.
+        
+        
+        ## Citation
+        
+        If you found this useful for your work, please cite this papers:
+        ```
+        @inproceedings{castri2023fpcmci,
+            title={Enhancing Causal Discovery from Robot Sensor Data in Dynamic Scenarios},
+            author={Castri, Luca and Mghames, Sariah and Hanheide, Marc and Bellotto, Nicola},
+            booktitle={Conference on Causal Learning and Reasoning (CLeaR)},
+            year={2023},
+        }
+        ```
+        
+        
+        ## Requirements
+        
+        * tigramite>=5.1.0.3
+        * pandas>=1.5.2
+        * netgraph>=4.10.2
+        * networkx>=2.8.6
+        * ruptures>=1.1.7
+        * scikit_learn>=1.1.3
+        * torch>=1.11.0
+        * gpytorch>=1.4
+        * dcor>=0.5.3
+        * h5py>=3.7.0   
+        
+        
+        ## Installation
+        
+        Before installing the FPCMCI package, you need to install Java and the [IDTxl package](https://github.com/pwollstadt/IDTxl) used for the feature-selection process, following the guide described [here](https://github.com/pwollstadt/IDTxl/wiki/Installation-and-Requirements). Once complete, you can install the current release of `FPCMCI` with:
+        ``` shell
+        pip install fpcmci
+        ```
+        
+        For a complete installation Java - IDTxl - FPCMCI, follow the following procedure.
+        
+        ### 1 - Java installation
+        Verify that you have not already installed Java:
+        ```shell
+        java -version
+        ```
+        if the latter returns `Command 'java' not found, ...`, you can install Java by the following commands, otherwise you can jump to IDTxl installation.
+        ```shell
+        # Java
+        sudo apt-get update
+        sudo apt install default-jdk
+        ```
+        
+        Then, you need to add JAVA_HOME to the environment
+        ```shell
+        sudo nano /etc/environment
+        JAVA_HOME="/lib/jvm/java-11-openjdk-amd64/bin/java" # Paste the JAVA_HOME assignment at the bottom of the file
+        source /etc/environment
+        ```
+        
+        ### 2 - IDTxl installation
+        ```shell
+        # IDTxl
+        git clone https://github.com/pwollstadt/IDTxl.git
+        conda create --name fpcmci python=3.8 pip matplotlib h5py scipy networkx
+        conda activate fpcmci
+        conda install -c conda-forge jpype1    # required by CPU JIDT estimators
+        conda install -c conda-forge pyopencl  # required by GPU OpenCL estimators
+        conda install -c anaconda ecos         # required by Tartu PID estimator
+        conda install numba                    # required by NumbaCuda estimators
+        conda install cudatoolkit              # required by NumbaCuda estimators
+        conda install mpmath
+        
+        cd IDTxl
+        pip install -e .
+        ```
+        
+        ### 3 - FPCMCI installation
+        ```shell
+        pip install fpcmci
+        ```
+        
+        
+        ## Recent changes
+        
+        | Version | Changes |
+        | :---: | ----------- |
+        | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
+        | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
+        | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
+        | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
+        | 4.0.1 | online documentation and paths fixes |
+        | 4.0.0 | package published |
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3
+Description-Content-Type: text/markdown
```

### Comparing `fpcmci-4.1.2/fpcmci/CPrinter.py` & `fpcmci-4.2.0/fpcmci/CPrinter.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/FPCMCI.py` & `fpcmci-4.2.0/fpcmci/FPCMCI.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import pickle
 import matplotlib.pyplot as plt
 import numpy as np
-from tigramite.independence_tests import CondIndTest
+from tigramite.independence_tests.independence_tests_base import CondIndTest
 import sys
 from fpcmci.selection_methods.SelectionMethod import SelectionMethod
 from fpcmci.CPrinter import CPLevel, CP
 from fpcmci.basics.constants import *
 from fpcmci.basics.logger import Logger
 import fpcmci.basics.utils as utils
 from fpcmci.PCMCI import PCMCI
@@ -24,34 +24,37 @@
     """
 
     def __init__(self, 
                  data: Data, 
                  min_lag, max_lag, 
                  sel_method: SelectionMethod, val_condtest: CondIndTest, 
                  verbosity: CPLevel, 
-                 alpha = 0.05, 
+                 f_alpha = 0.05, 
+                 pcmci_alpha = 0.05, 
                  resfolder = None,
                  neglect_only_autodep = False):
         """
         FPCMCI class contructor
 
         Args:
             data (Data): data to analyse
             min_lag (int): minimum time lag
             max_lag (int): maximum time lag
             sel_method (SelectionMethod): selection method
             val_condtest (CondIndTest): validation method
             verbosity (CPLevel): verbosity level
-            alpha (float, optional): significance level. Defaults to 0.05.
+            f_alpha (float, optional): filter significance level. Defaults to 0.05.
+            pcmci_alpha (float, optional): PCMCI significance level. Defaults to 0.05.
             resfolder (string, optional): result folder to create. Defaults to None.
             neglect_only_autodep (bool, optional): Bit for neglecting variables with only autodependency. Defaults to False.
         """
         
         self.data = data
-        self.alpha = alpha
+        self.f_alpha = f_alpha
+        self.pcmci_alpha = pcmci_alpha
         self.min_lag = min_lag
         self.max_lag = max_lag
         self.sel_method = sel_method
         self.filter_dependencies = None
         self.o_filter_dependencies = None
         self.causal_model = None
         self.result = None
@@ -59,45 +62,45 @@
 
         self.dependency_path = None
         if resfolder is not None:
             utils.create_results_folder()
             logpath, self.dependency_path = utils.get_selectorpath(resfolder)
             sys.stdout = Logger(logpath)
         
-        self.validator = PCMCI(data, alpha, min_lag, max_lag, val_condtest, resfolder, verbosity)       
+        self.validator = PCMCI(data, self.pcmci_alpha, min_lag, max_lag, val_condtest, resfolder, verbosity)       
         CP.set_verbosity(verbosity)
 
 
     def run_filter(self):
         """
         Run filter method
         """
         CP.info("\n")
         CP.info(DASH)
         CP.info("Selecting relevant features among: " + str(self.data.features))
         CP.info("Selection method: " + self.sel_method.name)
-        CP.info("Significance level: " + str(self.alpha))
+        CP.info("Significance level: " + str(self.f_alpha))
         CP.info("Max lag time: " + str(self.max_lag))
         CP.info("Min lag time: " + str(self.min_lag))
         CP.info("Data length: " + str(self.data.T))
 
-        self.sel_method.initialise(self.data, self.alpha, self.min_lag, self.max_lag)
+        self.sel_method.initialise(self.data, self.f_alpha, self.min_lag, self.max_lag)
         self.filter_dependencies = self.sel_method.compute_dependencies()
         self.o_filter_dependecies = copy.deepcopy(self.filter_dependencies)
 
 
     def run_pcmci(self):
         """
         Run PCMCI
         
         Returns:
             list(str): list of selected variable names
             dict(str:list(tuple)): causal model
         """
-        CP.info("Significance level: " + str(self.alpha))
+        CP.info("Significance level: " + str(self.pcmci_alpha))
         CP.info("Max lag time: " + str(self.max_lag))
         CP.info("Min lag time: " + str(self.min_lag))
         CP.info("Data length: " + str(self.data.T))
 
         # causal model
         self.validator.data = self.data
         self.validator.run()
@@ -126,35 +129,52 @@
         if not tmp_sel_features:
             return self.result
 
         # shrink dataframe d and dependencies by the selector result
         self.shrink(tmp_sel_features)
         
         # selected links to check by the validator
-        selected_links = self.__get_selected_links()
+        link_assumptions = self.__get_link_assumptions()
             
         # causal model on selected links
         self.validator.data = self.data
-        pcmci_result = self.validator.run(selected_links)
+        pcmci_result = self.validator.run(link_assumptions)
         
         # application of the validator result to the filter_dependencies field
         self.__apply_validator_result(pcmci_result)
-        # final causal model
-        self.causal_model = self.validator.dependencies
         
         self.result = self.get_selected_features()
         # shrink dataframe d and dependencies by the validator result
         self.shrink(self.result)
         
+        # final causal model
+        self.causal_model = self.validator.dependencies
         self.save_validator_res()
         
         CP.info("\nFeature selected: " + str(self.result))
         return self.result, self.causal_model
     
     
+    def get_causal_matrix(self):
+        """
+        Returns a dictionary with keys the lags and values the causal matrix containing the causal weights between targets (rows) and sources (columns)
+
+        Returns:
+            dict/np.ndarray: causal matrix per 
+        """
+        cm_per_lag = {lag : np.zeros((len(self.result), len(self.result))) for lag in range(self.min_lag, self.max_lag + 1)}
+        vars = ['$' + var +'$' for var in self.result]
+        for lag in cm_per_lag:
+            for var in vars:
+                for source in self.causal_model[var]:
+                    if source[LAG] == lag: cm_per_lag[lag][vars.index(var)][vars.index(source[SOURCE])] = source[SCORE]
+        if len(cm_per_lag) == 1: return list(cm_per_lag.values())[0]
+        return cm_per_lag
+    
+    
     def get_SCM(self):
         """
         Return Structural Causal Model
 
         Raises:
             ValueError: "Causal Model not estimated yet" if self.causal_model is None
 
@@ -333,16 +353,18 @@
 
 
     def __shrink_dependencies(self):
         """
         Shrinks dependencies based on the selected features
         """
         difference_set = self.filter_dependencies.keys() - self.data.features
-        for d in difference_set: del self.filter_dependencies[d]
-        
+        for d in difference_set: 
+            del self.filter_dependencies[d]
+            if self.validator.dependencies is not None: del self.validator.dependencies['$' + d + '$']
+ 
 
     def __get_dependencies_for_target(self, t):
         """
         Returns list of sources for a specified target
 
         Args:
             t (str): target variable name
@@ -390,28 +412,28 @@
 
         dep_mat[inf_mask] = max_dep_mat
         dep_mat[neginf_mask] = min_dep_mat
         dep_mat = (dep_mat - min_dep_mat) / (max_dep_mat - min_dep_mat)
         return dep_mat
 
 
-    def __get_selected_links(self):
+    def __get_link_assumptions(self):
         """
         Return selected links found by the selector
-        in this form: {0: [(0,-1), (2,-1)]}
+        in this form: {0: {(0,-1) : "-?>", (2,-1) : "-?>"}}
 
         Returns:
             (dict): selected links
         """
-        sel_links = {self.data.features.index(f):list() for f in self.data.features}
+        sel_links = {self.data.features.index(f):dict() for f in self.data.features}
         for t in self.filter_dependencies:
             
             # add links
             for s in self.filter_dependencies[t]:
-                sel_links[self.data.features.index(t)].append((self.data.features.index(s[SOURCE]), -s[LAG]))
+                sel_links[self.data.features.index(t)][(self.data.features.index(s[SOURCE]), -s[LAG])] = '-?>'
 
         return sel_links
     
     
     def __apply_validator_result(self, causal_model):
         """
         Exclude dependencies based on validator result
```

### Comparing `fpcmci-4.1.2/fpcmci/PCMCI.py` & `fpcmci-4.2.0/fpcmci/PCMCI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import pickle
 from tigramite.pcmci import PCMCI as VAL
-from tigramite.independence_tests import CondIndTest
+from tigramite.independence_tests.independence_tests_base import CondIndTest
 import tigramite.data_processing as pp
 import numpy as np
 from fpcmci.CPrinter import CPLevel, CP
 from fpcmci.preprocessing.data import Data
 import fpcmci.basics.utils as utils
 from fpcmci.causal_graph import *
 from fpcmci.basics.constants import *
@@ -44,15 +44,15 @@
         self.respath = None
         self.dag_path = None
         self.ts_dag_path = None
         if resfolder is not None:
             self.respath, self.dag_path, self.ts_dag_path = utils.get_validatorpaths(resfolder)  
         
 
-    def run(self, selected_links = None):
+    def run(self, link_assumptions = None):
         """
         Run causal discovery algorithm
 
         Returns:
             (dict): estimated causal model
         """
         CP.info('\n')
@@ -66,18 +66,17 @@
                                  var_names = self.data.pretty_features)
         
         # init and run pcmci
         self.val_method = VAL(dataframe = dataframe,
                                 cond_ind_test = self.val_condtest,
                                 verbosity = self.verbosity)
 
-        self.result = self.val_method.run_pcmci(selected_links = selected_links,
+        self.result = self.val_method.run_pcmci(link_assumptions = link_assumptions,
                                                 tau_max = self.max_lag,
-                                                tau_min = self.min_lag,
-                                                pc_alpha = 0.05)
+                                                tau_min = self.min_lag)
         
         self.result['var_names'] = self.data.pretty_features
         # apply significance level
         self.result['graph'] = self.__apply_alpha()
         self.dependencies = self.__PCMCIres_converter()
         return self.__return_parents_dict()
```

### Comparing `fpcmci-4.1.2/fpcmci/basics/utils.py` & `fpcmci-4.2.0/fpcmci/basics/utils.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/causal_graph.py` & `fpcmci-4.2.0/fpcmci/causal_graph.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/Subsampler.py` & `fpcmci-4.2.0/fpcmci/preprocessing/Subsampler.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/data.py` & `fpcmci-4.2.0/fpcmci/preprocessing/data.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py` & `fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/EntropyBasedMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/Static.py` & `fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/Static.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py` & `fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/SubsamplingMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/WSDynamic.py` & `fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/WSDynamic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py` & `fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/WSFFTStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/WSStatic.py` & `fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/WSStatic.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/preprocessing/subsampling_methods/moving_window.py` & `fpcmci-4.2.0/fpcmci/preprocessing/subsampling_methods/moving_window.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/selection_methods/Corr.py` & `fpcmci-4.2.0/fpcmci/selection_methods/Corr.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/selection_methods/MI.py` & `fpcmci-4.2.0/fpcmci/selection_methods/MI.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/selection_methods/ParCorr.py` & `fpcmci-4.2.0/fpcmci/selection_methods/ParCorr.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/selection_methods/SelectionMethod.py` & `fpcmci-4.2.0/fpcmci/selection_methods/SelectionMethod.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci/selection_methods/TE.py` & `fpcmci-4.2.0/fpcmci/selection_methods/TE.py`

 * *Files identical despite different names*

### Comparing `fpcmci-4.1.2/fpcmci.egg-info/PKG-INFO` & `fpcmci-4.2.0/fpcmci.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,156 @@
 Metadata-Version: 2.1
 Name: fpcmci
-Version: 4.1.2
+Version: 4.2.0
 Summary: A causal discovery Python package
 Home-page: https://github.com/lcastri/fpcmci
 Author: Luca Castri
 Author-email: lucacastri94@gmail.com
 License: UNKNOWN
+Description: # <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
+        
+        Extension of the state-of-the-art causal discovery method [PCMCI](https://github.com/jakobrunge/tigramite) augmented with a feature-selection method based on Transfer Entropy. The algorithm, starting from a prefixed set of variables, identifies the correct subset of features and possible links between them which describe the observed process. Then, from the selected features and links, a causal model is built.
+        
+        
+        ## Useful links
+        
+        * [Documentation](https://lcastri.github.io/fpcmci/)
+        * [Tutorials](https://github.com/lcastri/fpcmci/tree/main/tutorials)
+        
+        
+        ## Why FPCMCI?
+        
+        Current state-of-the-art causal discovery approaches suffer in terms of speed and accuracy of the causal analysis when the process to be analysed is composed by a large number of features. FPCMCI is able to select the most meaningful features from a set of variables and build a causal model from such selection. To this end, the causal analysis results **faster** and **more accurate**.
+        
+        In the following it is presented an example showing a comparison between causal models obtained by PCMCI and FPCMCI causal discovery algorithms on the same data. The latter have been created by defining a 6-variables system defined as follows:
+        
+        ``` python
+        min_lag = 1
+        max_lag = 1
+        np.random.seed(1)
+        nsample = 1500
+        nfeature = 6
+        
+        d = np.random.random(size = (nsample, feature))
+        for t in range(max_lag, nsample):
+          d[t, 0] += 2 * d[t-1, 1] + 3 * d[t-1, 3]
+          d[t, 2] += 1.1 * d[t-1, 1]**2
+          d[t, 3] += d[t-1, 3] * d[t-1, 2]
+          d[t, 4] += d[t-1, 4] + d[t-1, 5] * d[t-1, 0]
+        ```
+        
+        Causal Model by PCMCI       |  Causal Model by FPCMCI 
+        :-------------------------:|:-------------------------:
+        ![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_1.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_1.png "Causal model by FPCMCI")
+        Execution time ~ 6min 50sec | Execution time ~ 2min 45sec
+        
+        The causal analysis performed by the **FPCMCI** results not only faster but also more accurate. Indeed, the causal model derived by the FPCMCI agrees with the structure of the system of equations, instead the one derived by the PCMCI presents spurious links:
+        * $X_2$ &rarr; $X_4$
+        * $X_2$ &rarr; $X_5$
+        
+        Note that, since all the 6 variables were involved in the evolution of the system, the FPCMCI did not remove any of them. In the following example instead, we added a new variable in the system which is defined just by the noise component (as $X_1$ and $X_5$) and does not appear in any other equation, defined as follows: $X_6(t) = \eta_6(t)$. In the following the comparison between PCMCI and FPCMCI with this new system configuration:
+        
+        Causal Model by PCMCI       |  Causal Model by FPCMCI 
+        :-------------------------:|:-------------------------:
+        ![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_2.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_2.png "Causal model by FPCMCI")
+        Execution time ~ 8min 40sec | Execution time ~ 3min 00sec
+        
+        In this case the FPCMCI removes the $X_6$ variable from the causal graph leading to generate exactly the same causal model as in the previous example, with comparable executional time. Instead, the PCMCI suffers the presence of $X_6$ in terms of time and accuracy of the causal structure.
+        Indeed, a spurious link $X_6$ &rarr; $X_5$ appears in the causal graph derived by the PCMCI.
+        
+        
+        ## Citation
+        
+        If you found this useful for your work, please cite this papers:
+        ```
+        @inproceedings{castri2023fpcmci,
+            title={Enhancing Causal Discovery from Robot Sensor Data in Dynamic Scenarios},
+            author={Castri, Luca and Mghames, Sariah and Hanheide, Marc and Bellotto, Nicola},
+            booktitle={Conference on Causal Learning and Reasoning (CLeaR)},
+            year={2023},
+        }
+        ```
+        
+        
+        ## Requirements
+        
+        * tigramite>=5.1.0.3
+        * pandas>=1.5.2
+        * netgraph>=4.10.2
+        * networkx>=2.8.6
+        * ruptures>=1.1.7
+        * scikit_learn>=1.1.3
+        * torch>=1.11.0
+        * gpytorch>=1.4
+        * dcor>=0.5.3
+        * h5py>=3.7.0   
+        
+        
+        ## Installation
+        
+        Before installing the FPCMCI package, you need to install Java and the [IDTxl package](https://github.com/pwollstadt/IDTxl) used for the feature-selection process, following the guide described [here](https://github.com/pwollstadt/IDTxl/wiki/Installation-and-Requirements). Once complete, you can install the current release of `FPCMCI` with:
+        ``` shell
+        pip install fpcmci
+        ```
+        
+        For a complete installation Java - IDTxl - FPCMCI, follow the following procedure.
+        
+        ### 1 - Java installation
+        Verify that you have not already installed Java:
+        ```shell
+        java -version
+        ```
+        if the latter returns `Command 'java' not found, ...`, you can install Java by the following commands, otherwise you can jump to IDTxl installation.
+        ```shell
+        # Java
+        sudo apt-get update
+        sudo apt install default-jdk
+        ```
+        
+        Then, you need to add JAVA_HOME to the environment
+        ```shell
+        sudo nano /etc/environment
+        JAVA_HOME="/lib/jvm/java-11-openjdk-amd64/bin/java" # Paste the JAVA_HOME assignment at the bottom of the file
+        source /etc/environment
+        ```
+        
+        ### 2 - IDTxl installation
+        ```shell
+        # IDTxl
+        git clone https://github.com/pwollstadt/IDTxl.git
+        conda create --name fpcmci python=3.8 pip matplotlib h5py scipy networkx
+        conda activate fpcmci
+        conda install -c conda-forge jpype1    # required by CPU JIDT estimators
+        conda install -c conda-forge pyopencl  # required by GPU OpenCL estimators
+        conda install -c anaconda ecos         # required by Tartu PID estimator
+        conda install numba                    # required by NumbaCuda estimators
+        conda install cudatoolkit              # required by NumbaCuda estimators
+        conda install mpmath
+        
+        cd IDTxl
+        pip install -e .
+        ```
+        
+        ### 3 - FPCMCI installation
+        ```shell
+        pip install fpcmci
+        ```
+        
+        
+        ## Recent changes
+        
+        | Version | Changes |
+        | :---: | ----------- |
+        | 4.2.0 | causal model with only selected features fix<br>adapted to tigramite 5.2<br>get_causal_matrix FPCMCI method added<br>f_alpha and pcmci_alpha instead of alpha<br>requirements changed<br>tutorials adapted to new version |
+        | 4.1.2 | tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI |
+        | 4.1.1 | PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model |
+        | 4.1.0 | FSelector and FValidator turned into FPCMCI and PCMCI<br>show_edge_label removed and dag optimized<br>new package included in the setup.py<br>added tutorials<br>new example in README.md |
+        | 4.0.1 | online documentation and paths fixes |
+        | 4.0.0 | package published |
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# <img src="https://github.com/lcastri/fpcmci/raw/developer/docs/assets/icon.png" width="25"> FPCMCI - Filtered PCMCI
-
-Extension of the state-of-the-art causal discovery method [PCMCI](https://github.com/jakobrunge/tigramite) augmented with a feature-selection method based on Transfer Entropy. The algorithm, starting from a prefixed set of variables, identifies the correct subset of features and possible links between them which describe the observed process. Then, from the selected features and links, a causal model is built.
-
-
-## Useful links
-
-* [Documentation](https://lcastri.github.io/fpcmci/)
-* [Tutorials](https://github.com/lcastri/fpcmci/tree/main/tutorials)
-
-
-## Why FPCMCI?
-
-Current state-of-the-art causal discovery approaches suffer in terms of speed and accuracy of the causal analysis when the process to be analysed is composed by a large number of features. FPCMCI is able to select the most meaningful features from a set of variables and build a causal model from such selection. To this end, the causal analysis results **faster** and **more accurate**.
-
-In the following it is presented an example showing a comparison between causal models obtained by PCMCI and FPCMCI causal discovery algorithms on the same data. The latter have been created by defining a 6-variables system defined as follows:
-
-``` python
-min_lag = 1
-max_lag = 1
-np.random.seed(1)
-nsample = 1500
-nfeature = 6
-
-d = np.random.random(size = (nsample, feature))
-for t in range(max_lag, nsample):
-  d[t, 0] += 2 * d[t-1, 1] + 3 * d[t-1, 3]
-  d[t, 2] += 1.1 * d[t-1, 1]**2
-  d[t, 3] += d[t-1, 3] * d[t-1, 2]
-  d[t, 4] += d[t-1, 4] + d[t-1, 5] * d[t-1, 0]
-```
-
-Causal Model by PCMCI       |  Causal Model by FPCMCI 
-:-------------------------:|:-------------------------:
-![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_1.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_1.png "Causal model by FPCMCI")
-Execution time ~ 6min 50sec | Execution time ~ 2min 45sec
-
-The causal analysis performed by the **FPCMCI** results not only faster but also more accurate. Indeed, the causal model derived by the FPCMCI agrees with the structure of the system of equations, instead the one derived by the PCMCI presents spurious links:
-* $X_2$ &rarr; $X_4$
-* $X_2$ &rarr; $X_5$
-
-Note that, since all the 6 variables were involved in the evolution of the system, the FPCMCI did not remove any of them. In the following example instead, we added a new variable in the system which is defined just by the noise component (as $X_1$ and $X_5$) and does not appear in any other equation, defined as follows: $X_6(t) = \eta_6(t)$. In the following the comparison between PCMCI and FPCMCI with this new system configuration:
-
-Causal Model by PCMCI       |  Causal Model by FPCMCI 
-:-------------------------:|:-------------------------:
-![](https://github.com/lcastri/fpcmci/raw/main/images/PCMCI_example_2.png "Causal model by PCMCI")  |  ![](https://github.com/lcastri/fpcmci/raw/main/images/FPCMCI_example_2.png "Causal model by FPCMCI")
-Execution time ~ 8min 40sec | Execution time ~ 3min 00sec
-
-In this case the FPCMCI removes the $X_6$ variable from the causal graph leading to generate exactly the same causal model as in the previous example, with comparable executional time. Instead, the PCMCI suffers the presence of $X_6$ in terms of time and accuracy of the causal structure.
-Indeed, a spurious link $X_6$ &rarr; $X_5$ appears in the causal graph derived by the PCMCI.
-
-
-## Citation
-
-If you found this useful for your work, please cite this papers:
-```
-@inproceedings{castri2023fpcmci,
-    title={Enhancing Causal Discovery from Robot Sensor Data in Dynamic Scenarios},
-    author={Castri, Luca and Mghames, Sariah and Hanheide, Marc and Bellotto, Nicola},
-    booktitle={Conference on Causal Learning and Reasoning (CLeaR)},
-    year={2023},
-}
-```
-
-
-## Requirements
-
-* tigramite==5.1.0.3
-* pandas==1.5.2
-* netgraph>=4.10.2
-* networkx>=2.8.6
-* ruptures==1.1.7
-* scikit_learn==1.1.3
-* torch>=1.11.0
-* gpytorch>=1.4       
-* dcor>=0.5.3
-* h5py==3.7.0   
-
-
-## Installation
-
-Before installing the FPCMCI package, you need to install the [IDTxl package](https://github.com/pwollstadt/IDTxl) used for the feature-selection process, following the guide described [here](https://github.com/pwollstadt/IDTxl/wiki/Installation-and-Requirements). Once complete, you can install the current release of `FPCMCI` with:
-``` shell
-pip install fpcmci
-```
-
-For a complete installation (IDTxl and FPCMCI) you can run the following commands:
-```shell
-# IDTxl
-git clone https://github.com/pwollstadt/IDTxl.git
-conda create --name fpcmci python=3 pip matplotlib h5py scipy networkx
-conda activate fpcmci
-conda install -c conda-forge jpype1    # required by CPU JIDT estimators
-conda install -c conda-forge pyopencl  # required by GPU OpenCL estimators
-conda install -c anaconda ecos         # required by Tartu PID estimator
-conda install numba                    # required by NumbaCuda estimators
-conda install cudatoolkit              # required by NumbaCuda estimators
-conda install mpmath
-
-cd IDTxl
-pip install -e .
-
-# FPCMCI
-pip install fpcmci
-```
-
-
-## Recent changes
-
-* 4.1.2 tutorials adapted to 4.1.1 and get_SCM method added in FPCMCI
-* 4.1.1 PCMCI dependencies fix: FPCMCI causal model field added, FPCMCI.run() and .run_pcmci() outputs the selected variables and the corresponding causal model
-* 4.1.0 FSelector and FValidator turned into FPCMCI and PCMCI, show_edge_label removed and dag optimized, new package included in the setup.py, added tutorials, and new example in README.md. 
-* 4.0.1 online documentation and paths fixes.
-* 4.0.0 package published.
-
```

### Comparing `fpcmci-4.1.2/fpcmci.egg-info/SOURCES.txt` & `fpcmci-4.2.0/fpcmci.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENCE.txt
 README.md
 setup.py
 fpcmci/CPrinter.py
 fpcmci/FPCMCI.py
 fpcmci/PCMCI.py
 fpcmci/__init__.py
 fpcmci/causal_graph.py
```

### Comparing `fpcmci-4.1.2/setup.py` & `fpcmci-4.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup
 from fpcmci.version import VERSION
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
-INSTALL_REQUIRES = ["tigramite==5.1.0.3",
-                    "pandas==1.5.2",
+INSTALL_REQUIRES = ["tigramite>=5.1.0.3",
+                    "pandas>=1.5.2",
                     "netgraph>=4.10.2",
                     "networkx>=2.8.6",
-                    "ruptures==1.1.7",
+                    "ruptures>=1.1.7",
                     "scikit_learn==1.1.3",
                     "torch>=1.11.0", 
                     "gpytorch>=1.4",       
                     "dcor>=0.5.3",
-                    "h5py==3.7.0"   
+                    "h5py>=3.7.0"   
                     ]
 
 setup(
     name = 'fpcmci',
     version = VERSION,    
     description = 'A causal discovery Python package',
     long_description = long_description,
```

