# Comparing `tmp/metagentools-0.0.7.tar.gz` & `tmp/metagentools-0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metagentools-0.0.7.tar", last modified: Wed May 17 07:31:45 2023, max compression
+gzip compressed data, was "metagentools-0.0.dev2.tar", last modified: Fri Jan 27 14:02:02 2023, max compression
```

## Comparing `metagentools-0.0.7.tar` & `metagentools-0.0.dev2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:31:45.084060 metagentools-0.0.7/
--rw-rw-r--   0 vtec      (1000) vtec      (1000)    11337 2022-09-05 16:31:43.000000 metagentools-0.0.7/LICENSE
--rw-r--r--   0 vtec      (1000) vtec      (1000)      146 2023-04-24 08:32:11.000000 metagentools-0.0.7/MANIFEST.in
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2269 2023-05-17 07:31:45.084060 metagentools-0.0.7/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1517 2023-04-22 08:19:48.000000 metagentools-0.0.7/README.md
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1825 2023-04-24 08:32:11.000000 metagentools-0.0.7/default_parsing_rules.json
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:31:45.074060 metagentools-0.0.7/legacy/
--rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      897 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/analyze_final_report.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     5981 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/analyze_using_bayes_autocpt.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1980 2022-10-29 06:12:30.000000 metagentools-0.0.7/legacy/architecture.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2491 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/datasets.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2311 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/evaluation_on_simulated_150mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1566 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/evaluation_on_simulated_50mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1654 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/evaluation_on_simulated_HIV.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      805 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/generate_report.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1565 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/predict_100mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      858 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/predict_50mers.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1629 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/predict_on_realdata.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     8649 2023-04-24 09:48:25.000000 metagentools-0.0.7/legacy/preprocessing.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1999 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/training_model.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     6489 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)      851 2022-10-07 01:34:07.000000 metagentools-0.0.7/legacy/voting.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    12176 2022-10-29 06:12:30.000000 metagentools-0.0.7/legacy/wandb.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:31:45.074060 metagentools-0.0.7/metagentools/
--rw-r--r--   0 vtec      (1000) vtec      (1000)      203 2023-05-17 07:23:38.000000 metagentools-0.0.7/metagentools/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    21762 2023-05-17 07:27:19.000000 metagentools-0.0.7/metagentools/_modidx.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     7767 2023-05-17 07:23:38.000000 metagentools-0.0.7/metagentools/art.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     3372 2023-05-17 07:23:38.000000 metagentools-0.0.7/metagentools/bio.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:31:45.084060 metagentools-0.0.7/metagentools/cnn_virus/
--rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:23:38.000000 metagentools-0.0.7/metagentools/cnn_virus/__init__.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2538 2023-05-17 07:27:19.000000 metagentools-0.0.7/metagentools/cnn_virus/architecture.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    24035 2023-05-17 07:27:19.000000 metagentools-0.0.7/metagentools/cnn_virus/data.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1712 2023-05-17 07:23:38.000000 metagentools-0.0.7/metagentools/cnn_virus/utils.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    13854 2023-05-17 07:27:19.000000 metagentools-0.0.7/metagentools/core.py
--rw-r--r--   0 vtec      (1000) vtec      (1000)    10884 2023-05-17 07:23:38.000000 metagentools-0.0.7/metagentools/wandb.py
-drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-05-17 07:31:45.084060 metagentools-0.0.7/metagentools.egg-info/
--rw-r--r--   0 vtec      (1000) vtec      (1000)     2269 2023-05-17 07:31:44.000000 metagentools-0.0.7/metagentools.egg-info/PKG-INFO
--rw-r--r--   0 vtec      (1000) vtec      (1000)     1056 2023-05-17 07:31:44.000000 metagentools-0.0.7/metagentools.egg-info/SOURCES.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-05-17 07:31:44.000000 metagentools-0.0.7/metagentools.egg-info/dependency_links.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       46 2023-05-17 07:31:44.000000 metagentools-0.0.7/metagentools.egg-info/entry_points.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2022-10-29 12:01:44.000000 metagentools-0.0.7/metagentools.egg-info/not-zip-safe
--rw-r--r--   0 vtec      (1000) vtec      (1000)       64 2023-05-17 07:31:44.000000 metagentools-0.0.7/metagentools.egg-info/requires.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)       20 2023-05-17 07:31:44.000000 metagentools-0.0.7/metagentools.egg-info/top_level.txt
--rw-r--r--   0 vtec      (1000) vtec      (1000)      926 2023-04-24 08:36:18.000000 metagentools-0.0.7/settings.ini
--rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-05-17 07:31:45.084060 metagentools-0.0.7/setup.cfg
--rw-rw-r--   0 vtec      (1000) vtec      (1000)     2541 2022-09-05 16:31:43.000000 metagentools-0.0.7/setup.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/
+-rw-rw-r--   0 vtec      (1000) vtec      (1000)    11337 2022-09-05 16:31:43.000000 metagentools-0.0.dev2/LICENSE
+-rw-rw-r--   0 vtec      (1000) vtec      (1000)      111 2022-09-05 16:31:43.000000 metagentools-0.0.dev2/MANIFEST.in
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1391 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      735 2023-01-17 09:05:10.000000 metagentools-0.0.dev2/README.md
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/legacy/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      897 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/analyze_final_report.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5981 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/analyze_using_bayes_autocpt.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1980 2022-10-29 06:12:30.000000 metagentools-0.0.dev2/legacy/architecture.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2491 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/datasets.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2311 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/evaluation_on_simulated_150mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1566 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/evaluation_on_simulated_50mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1654 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/evaluation_on_simulated_HIV.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      805 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/generate_report.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1565 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/predict_100mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      858 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/predict_50mers.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1629 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/predict_on_realdata.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     8642 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/preprocessing.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1999 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/training_model.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     6489 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      851 2022-10-07 01:34:07.000000 metagentools-0.0.dev2/legacy/voting.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    12176 2022-10-29 06:12:30.000000 metagentools-0.0.dev2/legacy/wandb.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/metagentools/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     5845 2023-01-27 13:32:29.000000 metagentools-0.0.dev2/metagentools/_modidx.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     7429 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/art.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2750 2023-01-27 13:07:20.000000 metagentools-0.0.dev2/metagentools/bio.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/metagentools/cnn_virus/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        0 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/__init__.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2284 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/architecture.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     2802 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/data.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1712 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/cnn_virus/utils.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)      201 2023-01-27 13:07:20.000000 metagentools-0.0.dev2/metagentools/core.py
+-rw-r--r--   0 vtec      (1000) vtec      (1000)    10884 2023-01-27 13:05:49.000000 metagentools-0.0.dev2/metagentools/wandb.py
+drwxr-xr-x   0 vtec      (1000) vtec      (1000)        0 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/metagentools.egg-info/
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1391 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/PKG-INFO
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1029 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/SOURCES.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/dependency_links.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       46 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/entry_points.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)        1 2022-10-29 12:01:44.000000 metagentools-0.0.dev2/metagentools.egg-info/not-zip-safe
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       64 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/requires.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       20 2023-01-27 14:02:02.000000 metagentools-0.0.dev2/metagentools.egg-info/top_level.txt
+-rw-r--r--   0 vtec      (1000) vtec      (1000)     1005 2023-01-27 14:01:46.000000 metagentools-0.0.dev2/settings.ini
+-rw-r--r--   0 vtec      (1000) vtec      (1000)       38 2023-01-27 14:02:02.607491 metagentools-0.0.dev2/setup.cfg
+-rw-rw-r--   0 vtec      (1000) vtec      (1000)     2541 2022-09-05 16:31:43.000000 metagentools-0.0.dev2/setup.py
```

### Comparing `metagentools-0.0.7/LICENSE` & `metagentools-0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/analyze_final_report.py` & `metagentools-0.0.dev2/legacy/analyze_final_report.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/analyze_using_bayes_autocpt.py` & `metagentools-0.0.dev2/legacy/analyze_using_bayes_autocpt.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/architecture.py` & `metagentools-0.0.dev2/legacy/architecture.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/datasets.py` & `metagentools-0.0.dev2/legacy/datasets.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/evaluation_on_simulated_150mers.py` & `metagentools-0.0.dev2/legacy/evaluation_on_simulated_150mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/evaluation_on_simulated_50mers.py` & `metagentools-0.0.dev2/legacy/evaluation_on_simulated_50mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/evaluation_on_simulated_HIV.py` & `metagentools-0.0.dev2/legacy/evaluation_on_simulated_HIV.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/generate_report.py` & `metagentools-0.0.dev2/legacy/generate_report.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/predict_100mers.py` & `metagentools-0.0.dev2/legacy/predict_100mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/predict_50mers.py` & `metagentools-0.0.dev2/legacy/predict_50mers.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/predict_on_realdata.py` & `metagentools-0.0.dev2/legacy/predict_on_realdata.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/preprocessing.py` & `metagentools-0.0.dev2/legacy/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from tensorflow.keras.utils import Sequence, to_categorical
 
-# dictionary for one-hot encoding
-d_nucl = {"A": 0,"C": 1,"G": 2,"T": 3,"N":4}
+#dictionary for one-hot encoding
+d_nucl={"A":0,"C":1,"G":2,"T":3,"N":4}
 
 #get different learning weights for different classes
 def get_learning_weights(filepath):
     f=open(filepath,"r").readlines()
     d_weights={}
     for i in f:
         i = i.strip().split("\t")
```

### Comparing `metagentools-0.0.7/legacy/training_model.py` & `metagentools-0.0.dev2/legacy/training_model.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/utils.py` & `metagentools-0.0.dev2/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/voting.py` & `metagentools-0.0.dev2/legacy/voting.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/legacy/wandb.py` & `metagentools-0.0.dev2/legacy/wandb.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/metagentools/art.py` & `metagentools-0.0.dev2/metagentools/art.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 from fastcore.utils import run, join_path_file
 from pathlib import Path
 from typing import Tuple, List, Optional
 
 # %% ../nbs-dev/02_art.ipynb 6
 # Private Utility functions to export ==============================================
 
-def _run(args:List[str], shell:bool=False, print_output=True):
+def _run(args: List[str], shell: bool=False):
     """Wrapper subprocess.run and prints the output"""
     p = subprocess.run(args=args, stdout=subprocess.PIPE, shell=shell)
-    if print_output:
-        print('return code: ',p.returncode, '\n')
-        print(str(p.stdout, 'utf-8'))
+    print('return code: ',p.returncode, '\n')
+    print(str(p.stdout, 'utf-8'))
 
 def _validate_path(p:str|Path) -> Path:
     """checks that path is a string or a Path, and returns a Path"""
     if isinstance(p, str): 
         p = Path(p)
     elif not isinstance(p, Path): 
         raise TypeError(f"a path must be a string or a Path, not a {type(p)}")
@@ -42,27 +41,24 @@
         'HS25': 'HiSeq 2500 (125bp, 150bp)', 'HSXn': 'HiSeqX PCR free (150bp)', 'HSXt': 'HiSeqX TruSeq (150bp)',
         'MinS': 'MiniSeq TruSeq (50bp)', 'MSv1': 'MiSeq v1 (250bp)', 'MSv3': 'MiSeq v3 (250bp)',
         'NS50': 'NextSeq500 v2 (75bp)'
         }
 
     def __init__(
         self, 
-        path2app: str|Path,            # full path to art_illumina application on the system
-        input_dir: str|Path,           # full path to dir where input files are
-        output_dir: str|Path=None,     # full path to dir where to save output files, if different from input_dir
-        app_in_system_path:bool=False, # whether `art_illumina` is in the system path or not
+        path2app: str|Path,           # path to the art_illumina application on the system
+        input_dir: str|Path,          # path to dir where input files are
+        output_dir: str|Path=None     # path to dir where to save output files, if different from input_dir
         ):
         """Initialize the art_illumina instance"""
 
         # Validate and save paths
-        path2app = _validate_path(path2app)
-        if app_in_system_path:
-            self.app_cmd = 'art_illumina'
-        elif path2app.is_file():
-            self.app_cmd = str(path2app.absolute())
+        path2app = _validate_path(path2app)        
+        if path2app.is_file():
+            self.app = path2app
         else:
             raise ValueError(f"{path2app.name} is not a file, please check the path to the application")
 
         input_dir = _validate_path(input_dir)
         if input_dir.is_dir():
             self.input_dir = input_dir
         else:
@@ -73,41 +69,39 @@
         else:
             output_dir = _validate_path(output_dir)
             if output_dir.is_dir():
                 self.output_dir = output_dir
             else:
                 raise ValueError(f"{input_dir.name} is not a directory, please check the path")
 
-        print(f"Ready to operate with art: {self.app_cmd}")
+        print(f"Ready to operate with art: {self.app.absolute()}")
         print(f"Input files from : {self.input_dir.absolute()}")
         print(f"Output files to :  {self.output_dir.absolute()}")
 
     def sim_reads(
         self,
         input_file: str,          # name of the fasta file to use as input
         output_seed: str,         # seed to use for the output files
         sim_type: str='single',   # type of read simmulation: 'single' or 'paired'
         read_length: int=150,     # length of the read in bp
         fold: int=10,             # fold
         mean_read: int=None,      # mean length of the read for paired reads
         std_read: int=None,       # std of the read length, for paired reads
         ss: str='HS25',           # quality profile to use for simulation,
-        overwrite: bool=False,    # overwrite existing output files if true, raise error if false 
-        print_output:bool=True    # if True, prints art ilumina's CLI output
+        overwrite: bool=False     # overwrite existing output files if true, raise error if false 
         ):
         """Simulates reads with art_illumina. Output files saved in a separate directory"""
 
         # validate input file and save in instance
         path2inputfile = self.input_dir / input_file
         if path2inputfile.is_file(): 
             self.last_input_file = path2inputfile
         else:
             raise ValueError(f"{input_file} is not a file in {self.input_dir}")
 
-        
         # validate output seed and save in instance
         if not overwrite and len(list(self.output_dir.glob(f"{output_seed}*"))) > 0: 
             raise ValueError(f"Existing output directory starting with {output_seed}")
         else:
             self.last_output_seed = output_seed
             self.last_read_output_dir = self.output_dir/self.last_output_seed
             os.makedirs(self.last_read_output_dir, exist_ok=True)
@@ -126,16 +120,17 @@
                 params = f"-ss {ss} -p -l {read_length} -f {fold} -m {mean_read} -s {std_read}"
         else:
             raise RuntimeError(f"{sim_type} in not a type or is not implemented yet")
 
         p2in = self.last_input_file.absolute()
         p2out = (self.output_dir / self.last_output_seed / self.last_output_seed).absolute()
 
-        cmd = f"{self.app_cmd} -i {p2in} {params} -o {p2out}"
-        _run(args=shlex.split(cmd), print_output=print_output)
+        cmd = f"{self.app.absolute()} -i {p2in} {params} -o {p2out}"
+
+        _run(args=shlex.split(cmd))
 
     def get_last_output_files(self):
         """Returns the path to all output files from last simulation"""
         return [f for f in self.last_read_output_dir.iterdir()]
 
     def list_last_output_files(self):
         """Prints a list of the last simulation's output files"""
```

### Comparing `metagentools-0.0.7/metagentools/cnn_virus/architecture.py` & `metagentools-0.0.dev2/metagentools/cnn_virus/architecture.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs-dev/03_cnn_virus_architecture.ipynb.
 
 # %% auto 0
 __all__ = ['create_model_original']
 
-# %% ../../nbs-dev/03_cnn_virus_architecture.ipynb 3
+# %% ../../nbs-dev/03_cnn_virus_architecture.ipynb 2
 # Imports all dependencies
 import tensorflow as tf
 import tensorflow.keras
 
 from pathlib import Path
 from typing import Callable, Tuple
 
 from tensorflow.keras.layers import Convolution1D, Dense, Flatten, Dropout, Activation, BatchNormalization, Input
 from tensorflow.keras.layers import MaxPooling1D, Concatenate
 from tensorflow.keras.models import Sequential, Model, load_model
 
-# %% ../../nbs-dev/03_cnn_virus_architecture.ipynb 8
+# %% ../../nbs-dev/03_cnn_virus_architecture.ipynb 6
 def create_model_original() -> tf.keras.Model: # new instance of an original paper architecture
     """Build a CNN model as per CNN Virus paper"""
 
     print("Creating CNN Model (Original)")
 
     #build cnn model
-    input_seq=Input(shape=(50,5), name='input-seq')
-    layer1=Convolution1D(512, 5, padding="same",activation="relu",kernel_initializer="he_uniform", name="conv-1")(input_seq)
-    layer2=BatchNormalization(momentum=0.6, name='bn-1')(layer1)
-    layer3=MaxPooling1D(pool_size=2,padding='same', name='maxpool-1')(layer2)
-    layer4=Convolution1D(512, 5, padding="same",activation="relu",kernel_initializer="he_uniform", name="conv-2")(layer3)
-    layer5=BatchNormalization(momentum=0.6, name='bn-2')(layer4)
-    layer6=MaxPooling1D(pool_size=2,padding='same',name='maxpool-2')(layer5)
-    layer7=Convolution1D(1024, 7, padding="same", activation="relu",kernel_initializer="he_uniform", name="conv-3")(layer6)
-    layer8=Convolution1D(1024, 7, padding="same", activation="relu",kernel_initializer="he_uniform", name="conv-4")(layer7)
-    layer9=BatchNormalization(momentum=0.6, name='bn-3')(layer8)
-    layer10=MaxPooling1D(pool_size=2,padding='same', name='maxpool-3')(layer9)
-    layer11=Flatten(name='flatten')(layer10)
-    layer12=Dense(1024,kernel_initializer="he_uniform", name='dense-1')(layer11)
-    layer13=BatchNormalization(momentum=0.6, name='bn-4')(layer12)
-    layer14=Dropout(0.2, name='do-1')(layer13)
-    labels=Dense(187, activation='softmax',kernel_initializer="he_uniform",name="labels")(layer14)
-    output_con=Concatenate(name='concat')([layer14,labels])
-    layer15=Dense(1024, kernel_initializer="he_uniform", name='dense-2')(output_con)
-    layer16=BatchNormalization(momentum=0.6, name='bn-5')(layer15)
-    pos=Dense(10, activation='softmax',kernel_initializer="he_uniform",name="pos")(layer16)
-    model = Model(inputs=input_seq, outputs=[labels,pos])
+    input_seq=Input(shape=(50,5))
+    layer1=Convolution1D(512, 5, padding="same",activation="relu",kernel_initializer="he_uniform")(input_seq)
+    layer2=BatchNormalization(momentum=0.6)(layer1)
+    layer3=MaxPooling1D(pool_size=2,padding='same')(layer2)
+    layer4=Convolution1D(512, 5, padding="same",activation="relu",kernel_initializer="he_uniform")(layer3)
+    layer5=BatchNormalization(momentum=0.6)(layer4)
+    layer6=MaxPooling1D(pool_size=2,padding='same')(layer5)
+    layer7=Convolution1D(1024, 7, padding="same",activation="relu",kernel_initializer="he_uniform")(layer6)
+    layer8=Convolution1D(1024, 7, padding="same",activation="relu",kernel_initializer="he_uniform")(layer7)
+    layer9=BatchNormalization(momentum=0.6)(layer8)
+    layer10=MaxPooling1D(pool_size=2,padding='same')(layer9)
+    layer11=Flatten()(layer10)
+    layer12=Dense(1024,kernel_initializer="he_uniform")(layer11)
+    layer13=BatchNormalization(momentum=0.6)(layer12)
+    layer14=Dropout(0.2)(layer13)
+    output1=Dense(187, activation='softmax',kernel_initializer="he_uniform",name="output1")(layer14)
+    output_con=Concatenate()([layer14,output1])
+    layer15=Dense(1024, kernel_initializer="he_uniform")(output_con)
+    layer16=BatchNormalization(momentum=0.6)(layer15)
+    output2=Dense(10, activation='softmax',kernel_initializer="he_uniform",name="output2")(layer16)
+    model = Model(inputs=input_seq, outputs=[output1,output2])
     return model
```

### Comparing `metagentools-0.0.7/metagentools/cnn_virus/utils.py` & `metagentools-0.0.dev2/metagentools/cnn_virus/utils.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/metagentools/wandb.py` & `metagentools-0.0.dev2/metagentools/wandb.py`

 * *Files identical despite different names*

### Comparing `metagentools-0.0.7/metagentools.egg-info/SOURCES.txt` & `metagentools-0.0.dev2/metagentools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-default_parsing_rules.json
 settings.ini
 setup.py
 legacy/__init__.py
 legacy/analyze_final_report.py
 legacy/analyze_using_bayes_autocpt.py
 legacy/architecture.py
 legacy/datasets.py
```

### Comparing `metagentools-0.0.7/setup.py` & `metagentools-0.0.dev2/setup.py`

 * *Files identical despite different names*

