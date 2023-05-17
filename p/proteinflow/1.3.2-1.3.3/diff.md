# Comparing `tmp/proteinflow-1.3.2.tar.gz` & `tmp/proteinflow-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.3.2.tar", last modified: Wed May 17 10:47:32 2023, max compression
+gzip compressed data, was "proteinflow-1.3.3.tar", last modified: Wed May 17 13:00:24 2023, max compression
```

## Comparing `proteinflow-1.3.2.tar` & `proteinflow-1.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.801216 proteinflow-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 10:47:21.000000 proteinflow-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 10:47:32.801216 proteinflow-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-17 10:47:21.000000 proteinflow-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.793216 proteinflow-1.3.2/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)   100515 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.797216 proteinflow-1.3.2/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.797216 proteinflow-1.3.2/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.797216 proteinflow-1.3.2/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 10:47:21.000000 proteinflow-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:47:32.801216 proteinflow-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.801216 proteinflow-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-17 10:47:21.000000 proteinflow-1.3.2/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 10:47:21.000000 proteinflow-1.3.2/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 10:47:21.000000 proteinflow-1.3.2/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 13:00:09.000000 proteinflow-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 13:00:24.077890 proteinflow-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-17 13:00:09.000000 proteinflow-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.073890 proteinflow-1.3.3/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   100557 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 13:00:09.000000 proteinflow-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:00:24.077890 proteinflow-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-17 13:00:10.000000 proteinflow-1.3.3/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 13:00:10.000000 proteinflow-1.3.3/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 13:00:10.000000 proteinflow-1.3.3/tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.2/LICENSE` & `proteinflow-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/PKG-INFO` & `proteinflow-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.2
+Version: 1.3.3
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.2 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.3 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.2/README.md` & `proteinflow-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/__init__.py` & `proteinflow-1.3.3/proteinflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1763,15 +1763,15 @@
         if clustering_dict_path is not None and use_fraction < 1:
             with open(clustering_dict_path, "rb") as f:
                 clusters = pickle.load(f)
             keys = sorted(clusters.keys())[: int(len(clusters) * use_fraction)]
             to_process = set()
             for key in keys:
                 to_process.update([x[0] for x in clusters[key]])
-            to_process = list(to_process)
+            to_process = [x for x in to_process if x in os.listdir(dataset_folder)]
         if debug:
             to_process = to_process[:1000]
         if self.entry_type == "pair":
             print(
                 "Please note that the pair entry type takes longer to process than the other two. The progress bar is not linear because of the varying number of chains per file."
             )
         output_tuples_list = p_map(
```

### Comparing `proteinflow-1.3.2/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.3.3/proteinflow/scripts/proteinflow_cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/async_download.py` & `proteinflow-1.3.3/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/biotite_sse.py` & `proteinflow-1.3.3/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/build_pdb.py` & `proteinflow-1.3.3/proteinflow/utils/build_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.3.3/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/filter_database.py` & `proteinflow-1.3.3/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.3.3/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/process_pdb.py` & `proteinflow-1.3.3/proteinflow/utils/process_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow/utils/split_dataset.py` & `proteinflow-1.3.3/proteinflow/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.3.3/proteinflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.2
+Version: 1.3.3
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.2 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.3 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.2/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.3.3/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/pyproject.toml` & `proteinflow-1.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.3.2"
+version = "1.3.3"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-1.3.2/tests/test_download.py` & `proteinflow-1.3.3/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/tests/test_generate.py` & `proteinflow-1.3.3/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.2/tests/test_sabdab.py` & `proteinflow-1.3.3/tests/test_sabdab.py`

 * *Files identical despite different names*

