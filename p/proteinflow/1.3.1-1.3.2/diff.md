# Comparing `tmp/proteinflow-1.3.1.tar.gz` & `tmp/proteinflow-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.3.1.tar", last modified: Wed May 10 11:04:36 2023, max compression
+gzip compressed data, was "proteinflow-1.3.2.tar", last modified: Wed May 17 10:47:32 2023, max compression
```

## Comparing `proteinflow-1.3.1.tar` & `proteinflow-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.732840 proteinflow-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 11:04:23.000000 proteinflow-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-10 11:04:36.732840 proteinflow-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-10 11:04:23.000000 proteinflow-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.728840 proteinflow-1.3.1/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    97798 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.728840 proteinflow-1.3.1/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.732840 proteinflow-1.3.1/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    41037 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-10 11:04:23.000000 proteinflow-1.3.1/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.728840 proteinflow-1.3.1/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 11:04:36.000000 proteinflow-1.3.1/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-10 11:04:23.000000 proteinflow-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:04:36.732840 proteinflow-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:04:36.732840 proteinflow-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-10 11:04:23.000000 proteinflow-1.3.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-10 11:04:23.000000 proteinflow-1.3.1/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-10 11:04:23.000000 proteinflow-1.3.1/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.801216 proteinflow-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 10:47:21.000000 proteinflow-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 10:47:32.801216 proteinflow-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-17 10:47:21.000000 proteinflow-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.793216 proteinflow-1.3.2/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   100515 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.797216 proteinflow-1.3.2/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.797216 proteinflow-1.3.2/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-17 10:47:21.000000 proteinflow-1.3.2/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.797216 proteinflow-1.3.2/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 10:47:32.000000 proteinflow-1.3.2/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 10:47:21.000000 proteinflow-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:47:32.801216 proteinflow-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:32.801216 proteinflow-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-17 10:47:21.000000 proteinflow-1.3.2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 10:47:21.000000 proteinflow-1.3.2/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 10:47:21.000000 proteinflow-1.3.2/tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.1/LICENSE` & `proteinflow-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/PKG-INFO` & `proteinflow-1.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.1
+Version: 1.3.2
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -74,15 +74,15 @@
 ## Usage
 ### Downloading pre-computed datasets (stable)
 Already precomputed datasets with consensus set of parameters and can be accessed and downloaded using the `proteinflow`. package. Check the output of `proteinflow check_tags` for a list of available tags.
 ```bash
 proteinflow download --tag 20230102_stable 
 ```
 
-### Running the pipeline
+### Running the pipeline (PDB)
 You can also run `proteinflow` with your own parameters. Check the output of `proteinflow check_snapshots` for a list of available PDB snapshots (naming rule: `yyyymmdd`).
 
 For instance, let's generate a dataset with the following description:
 - resolution threshold: 5 angstrom,
 - PDB snapshot: 20190101,
 - structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
 - sequence identity threshold for clustering: 40% sequence similarity,
@@ -94,15 +94,32 @@
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
 A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
-You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
+### Running the pipeline (SAbDab)
+You can also use the `--sabdab` option in `proteinflow generate` to load files from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will download the latest up-to-date version of the SabDab dataset and cluster the antibodies based on their CDR sequence.
+Alternatively, it can be used together with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or folder. This allows you to use search and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a custom dataset by downloading the archived zip file of the structures selected. (Under Downloads section of your SabDab query).
+
+SAbDab sequences clustering is done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1, L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic constructs are clustered together with other heavy chain CDRs. The resulting CDR clusters are split into training, test and validation in a way that ensures that every PDB file only appears in one subset.
+
+Individual output pickle files represent heavy chain - light chain - antigen complexes (created from SAbDab annotation, sometimes more than one per PDB entry). Each of the elements (heavy chain, light chain, antigen) can be missing in specific entries and there can be multiple antigen chains. In order to filter for at least one antigen chain, use the `--require_antigen` option.
+
+For instance, let's generate a dataset with the following description:
+- SabDab version: latest (up-to-date),
+- resolution threshold: 5 angstrom,
+- structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
+- sequence identity threshold for clustering (CDRs): 40%,
+- size of validation subset: 10%.
+
+```bash
+proteinflow generate --sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split 0.1
+```
 
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
@@ -115,18 +132,20 @@
 - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
 - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check `proteinflow.sidechain_order()` for the order of atoms),
 - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
     zeros to missing values,
 - `'seq'`: a string of length `L` with residue types.
 
 In a SAbDab datasets, an additional key is added to the dictionary:
-- `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
+- `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
     and non-CDR residues are marked with `'-'`.
+    
+Note that the sequence information in the PDB files is aligned to the FASTA sequences to identify the missing residues.
 
-Once your data is ready, you can open the files with `pickle`.
+Once your data is ready, you can open the files with `pickle` directly.
 
 ```python
 import pickle
 import os
 
 train_folder = "./data/proteinflow_new/training"
 for filename in os.listdir(train_folder):
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.1 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.2 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -43,34 +43,58 @@
 github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
 The docker image can be accessed in interactive mode with this command. ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
 ### Downloading pre-computed datasets (stable) Already precomputed datasets
 with consensus set of parameters and can be accessed and downloaded using the
 `proteinflow`. package. Check the output of `proteinflow check_tags` for a list
 of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
-Running the pipeline You can also run `proteinflow` with your own parameters.
-Check the output of `proteinflow check_snapshots` for a list of available PDB
-snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
-with the following description: - resolution threshold: 5 angstrom, - PDB
-snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
-NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
-similarity, - maximum length per sequence: 1000 residues, - minimum length per
-sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
-size of validation subset: 10%. ```bash proteinflow generate --tag new --
-resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
---max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
-See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
-generate --help`) for the full list of parameters and more information. A
-registry of all the files that are removed during the filtering as well as
-description with the reason for their removal is created automatically for each
-`generate` command. The log files are save (at `data/logs` by default) and a
-summary can be accessed running `proteinflow get_summary {log_path}`. You can
-also use the `--sabdab` option to load files from SAbDab and cluster them based
-on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip
-file. ### Splitting By default, both `proteinflow generate` and `proteinflow
+Running the pipeline (PDB) You can also run `proteinflow` with your own
+parameters. Check the output of `proteinflow check_snapshots` for a list of
+available PDB snapshots (naming rule: `yyyymmdd`). For instance, let's generate
+a dataset with the following description: - resolution threshold: 5 angstrom, -
+PDB snapshot: 20190101, - structure methods accepted: all (x-ray
+christolography, NRM, Cryo-EM), - sequence identity threshold for clustering:
+40% sequence similarity, - maximum length per sequence: 1000 residues, -
+minimum length per sequence: 5 residues, - maximum fraction of missing values
+at the ends: 10%, - size of validation subset: 10%. ```bash proteinflow
+generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --
+not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --
+missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs](https://
+adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the
+full list of parameters and more information. A registry of all the files that
+are removed during the filtering as well as description with the reason for
+their removal is created automatically for each `generate` command. The log
+files are save (at `data/logs` by default) and a summary can be accessed
+running `proteinflow get_summary {log_path}`. ### Running the pipeline (SAbDab)
+You can also use the `--sabdab` option in `proteinflow generate` to load files
+from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will
+download the latest up-to-date version of the SabDab dataset and cluster the
+antibodies based on their CDR sequence. Alternatively, it can be used together
+with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or
+folder. This allows you to use search and query tools from the [SabDab web
+interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a
+custom dataset by downloading the archived zip file of the structures selected.
+(Under Downloads section of your SabDab query). SAbDab sequences clustering is
+done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1,
+L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/
+9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic
+constructs are clustered together with other heavy chain CDRs. The resulting
+CDR clusters are split into training, test and validation in a way that ensures
+that every PDB file only appears in one subset. Individual output pickle files
+represent heavy chain - light chain - antigen complexes (created from SAbDab
+annotation, sometimes more than one per PDB entry). Each of the elements (heavy
+chain, light chain, antigen) can be missing in specific entries and there can
+be multiple antigen chains. In order to filter for at least one antigen chain,
+use the `--require_antigen` option. For instance, let's generate a dataset with
+the following description: - SabDab version: latest (up-to-date), - resolution
+threshold: 5 angstrom, - structure methods accepted: all (x-ray
+christolography, NRM, Cryo-EM), - sequence identity threshold for clustering
+(CDRs): 40%, - size of validation subset: 10%. ```bash proteinflow generate --
+sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split
+0.1 ``` ### Splitting By default, both `proteinflow generate` and `proteinflow
 download` will also split your data into training, test and validation
 according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
 However, you can skip this step with a `--skip_splitting` flag and then perform
 it separately with the `proteinflow split` command. The following command will
 perform the splitting with a 10% validation set, a 5% test set and a 50%
 threshold for sequence identity clusters. ```bash proteinflow split --tag new -
 -valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
@@ -80,31 +104,33 @@
 are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
 array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
 `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
 coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
 `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
 known coordinates and zeros to missing values, - `'seq'`: a string of length
 `L` with residue types. In a SAbDab datasets, an additional key is added to the
-dictionary: - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are
+dictionary: - `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are
 marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
-are marked with `'-'`. Once your data is ready, you can open the files with
-`pickle`. ```python import pickle import os train_folder = "./data/
-proteinflow_new/training" for filename in os.listdir(train_folder): with open
-(os.path.join(train_folder, filename), "rb") as f: data = pickle.load(f) crd_bb
-= data["crd_bb"] seq = data["seq"] ... ``` Alternatively, you can use our
-`ProteinDataset` or `ProteinLoader` classes for convenient processing. Among
-other things, they allow for feature extraction, single chain / homomer /
-heteromer filtering and randomized sampling from sequence identity clusters.
-For example, here is how we can create a data loader that: - samples a
-different cluster representative at every epoch, - extracts dihedral angles,
-sidechain orientation and secondary structure features, - only loads pairs of
-interacting proteins (larger biounits are broken up into pairs), - has batch
-size 8. ```python from proteinflow import ProteinLoader train_loader =
-ProteinLoader.from_args( "./data/proteinflow_new/training",
-clustering_dict_path="./data/proteinflow_new/splits_dict/train.pickle",
+are marked with `'-'`. Note that the sequence information in the PDB files is
+aligned to the FASTA sequences to identify the missing residues. Once your data
+is ready, you can open the files with `pickle` directly. ```python import
+pickle import os train_folder = "./data/proteinflow_new/training" for filename
+in os.listdir(train_folder): with open(os.path.join(train_folder, filename),
+"rb") as f: data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ...
+``` Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes
+for convenient processing. Among other things, they allow for feature
+extraction, single chain / homomer / heteromer filtering and randomized
+sampling from sequence identity clusters. For example, here is how we can
+create a data loader that: - samples a different cluster representative at
+every epoch, - extracts dihedral angles, sidechain orientation and secondary
+structure features, - only loads pairs of interacting proteins (larger biounits
+are broken up into pairs), - has batch size 8. ```python from proteinflow
+import ProteinLoader train_loader = ProteinLoader.from_args( "./data/
+proteinflow_new/training", clustering_dict_path="./data/proteinflow_new/
+splits_dict/train.pickle",
 node_features_type="dihedral+sidechain_orientation+secondary_structure",
 entry_type="pair", batch_size=8, ) for batch in train_loader: crd_bb = batch
 ["X"] #(B, L, 4, 3) seq = batch["S"] #(B, L) sse = batch["secondary_structure"]
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
```

### Comparing `proteinflow-1.3.1/README.md` & `proteinflow-1.3.2/proteinflow.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: proteinflow
+Version: 1.3.2
+Summary: Versatile pipeline for processing protein structure data for deep learning applications.
+Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
+License: BSD-3-Clause
+Keywords: bioinformatics,dataset,protein,PDB,deep learning
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
     <b> ProteinFlow - A data processing pipeline for all your protein design needs </b> <br />
 </p>
 
 <p align="center">
   <a href="https://adaptyvbio.github.io/ProteinFlow/" target="_blank">
       Docs
@@ -63,15 +74,15 @@
 ## Usage
 ### Downloading pre-computed datasets (stable)
 Already precomputed datasets with consensus set of parameters and can be accessed and downloaded using the `proteinflow`. package. Check the output of `proteinflow check_tags` for a list of available tags.
 ```bash
 proteinflow download --tag 20230102_stable 
 ```
 
-### Running the pipeline
+### Running the pipeline (PDB)
 You can also run `proteinflow` with your own parameters. Check the output of `proteinflow check_snapshots` for a list of available PDB snapshots (naming rule: `yyyymmdd`).
 
 For instance, let's generate a dataset with the following description:
 - resolution threshold: 5 angstrom,
 - PDB snapshot: 20190101,
 - structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
 - sequence identity threshold for clustering: 40% sequence similarity,
@@ -83,15 +94,32 @@
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
 A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
-You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
+### Running the pipeline (SAbDab)
+You can also use the `--sabdab` option in `proteinflow generate` to load files from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will download the latest up-to-date version of the SabDab dataset and cluster the antibodies based on their CDR sequence.
+Alternatively, it can be used together with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or folder. This allows you to use search and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a custom dataset by downloading the archived zip file of the structures selected. (Under Downloads section of your SabDab query).
+
+SAbDab sequences clustering is done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1, L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic constructs are clustered together with other heavy chain CDRs. The resulting CDR clusters are split into training, test and validation in a way that ensures that every PDB file only appears in one subset.
+
+Individual output pickle files represent heavy chain - light chain - antigen complexes (created from SAbDab annotation, sometimes more than one per PDB entry). Each of the elements (heavy chain, light chain, antigen) can be missing in specific entries and there can be multiple antigen chains. In order to filter for at least one antigen chain, use the `--require_antigen` option.
+
+For instance, let's generate a dataset with the following description:
+- SabDab version: latest (up-to-date),
+- resolution threshold: 5 angstrom,
+- structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
+- sequence identity threshold for clustering (CDRs): 40%,
+- size of validation subset: 10%.
+
+```bash
+proteinflow generate --sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split 0.1
+```
 
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
@@ -104,18 +132,20 @@
 - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
 - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check `proteinflow.sidechain_order()` for the order of atoms),
 - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
     zeros to missing values,
 - `'seq'`: a string of length `L` with residue types.
 
 In a SAbDab datasets, an additional key is added to the dictionary:
-- `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
+- `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
     and non-CDR residues are marked with `'-'`.
+    
+Note that the sequence information in the PDB files is aligned to the FASTA sequences to identify the missing residues.
 
-Once your data is ready, you can open the files with `pickle`.
+Once your data is ready, you can open the files with `pickle` directly.
 
 ```python
 import pickle
 import os
 
 train_folder = "./data/proteinflow_new/training"
 for filename in os.listdir(train_folder):
```

#### html2text {}

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.2 Summary: Versatile
+pipeline for processing protein structure data for deep learning applications.
+Author-email: Liza Kozlova
+adaptyvbio.com>, Arthur Valentin
+adaptyvbio.com> License: BSD-3-Clause Keywords:
+bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
                                      Docs
 --- [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)]
 (https://opensource.org/licenses/BSD-3-Clause) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/
 project/proteinflow/) [![Conda](https://img.shields.io/conda/v/adaptyvbio/
@@ -36,34 +43,58 @@
 github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
 The docker image can be accessed in interactive mode with this command. ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
 ### Downloading pre-computed datasets (stable) Already precomputed datasets
 with consensus set of parameters and can be accessed and downloaded using the
 `proteinflow`. package. Check the output of `proteinflow check_tags` for a list
 of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
-Running the pipeline You can also run `proteinflow` with your own parameters.
-Check the output of `proteinflow check_snapshots` for a list of available PDB
-snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
-with the following description: - resolution threshold: 5 angstrom, - PDB
-snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
-NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
-similarity, - maximum length per sequence: 1000 residues, - minimum length per
-sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
-size of validation subset: 10%. ```bash proteinflow generate --tag new --
-resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
---max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
-See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
-generate --help`) for the full list of parameters and more information. A
-registry of all the files that are removed during the filtering as well as
-description with the reason for their removal is created automatically for each
-`generate` command. The log files are save (at `data/logs` by default) and a
-summary can be accessed running `proteinflow get_summary {log_path}`. You can
-also use the `--sabdab` option to load files from SAbDab and cluster them based
-on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip
-file. ### Splitting By default, both `proteinflow generate` and `proteinflow
+Running the pipeline (PDB) You can also run `proteinflow` with your own
+parameters. Check the output of `proteinflow check_snapshots` for a list of
+available PDB snapshots (naming rule: `yyyymmdd`). For instance, let's generate
+a dataset with the following description: - resolution threshold: 5 angstrom, -
+PDB snapshot: 20190101, - structure methods accepted: all (x-ray
+christolography, NRM, Cryo-EM), - sequence identity threshold for clustering:
+40% sequence similarity, - maximum length per sequence: 1000 residues, -
+minimum length per sequence: 5 residues, - maximum fraction of missing values
+at the ends: 10%, - size of validation subset: 10%. ```bash proteinflow
+generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --
+not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --
+missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs](https://
+adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the
+full list of parameters and more information. A registry of all the files that
+are removed during the filtering as well as description with the reason for
+their removal is created automatically for each `generate` command. The log
+files are save (at `data/logs` by default) and a summary can be accessed
+running `proteinflow get_summary {log_path}`. ### Running the pipeline (SAbDab)
+You can also use the `--sabdab` option in `proteinflow generate` to load files
+from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will
+download the latest up-to-date version of the SabDab dataset and cluster the
+antibodies based on their CDR sequence. Alternatively, it can be used together
+with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or
+folder. This allows you to use search and query tools from the [SabDab web
+interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a
+custom dataset by downloading the archived zip file of the structures selected.
+(Under Downloads section of your SabDab query). SAbDab sequences clustering is
+done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1,
+L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/
+9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic
+constructs are clustered together with other heavy chain CDRs. The resulting
+CDR clusters are split into training, test and validation in a way that ensures
+that every PDB file only appears in one subset. Individual output pickle files
+represent heavy chain - light chain - antigen complexes (created from SAbDab
+annotation, sometimes more than one per PDB entry). Each of the elements (heavy
+chain, light chain, antigen) can be missing in specific entries and there can
+be multiple antigen chains. In order to filter for at least one antigen chain,
+use the `--require_antigen` option. For instance, let's generate a dataset with
+the following description: - SabDab version: latest (up-to-date), - resolution
+threshold: 5 angstrom, - structure methods accepted: all (x-ray
+christolography, NRM, Cryo-EM), - sequence identity threshold for clustering
+(CDRs): 40%, - size of validation subset: 10%. ```bash proteinflow generate --
+sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split
+0.1 ``` ### Splitting By default, both `proteinflow generate` and `proteinflow
 download` will also split your data into training, test and validation
 according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
 However, you can skip this step with a `--skip_splitting` flag and then perform
 it separately with the `proteinflow split` command. The following command will
 perform the splitting with a 10% validation set, a 5% test set and a 50%
 threshold for sequence identity clusters. ```bash proteinflow split --tag new -
 -valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
@@ -73,31 +104,33 @@
 are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
 array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
 `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
 coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
 `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
 known coordinates and zeros to missing values, - `'seq'`: a string of length
 `L` with residue types. In a SAbDab datasets, an additional key is added to the
-dictionary: - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are
+dictionary: - `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are
 marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
-are marked with `'-'`. Once your data is ready, you can open the files with
-`pickle`. ```python import pickle import os train_folder = "./data/
-proteinflow_new/training" for filename in os.listdir(train_folder): with open
-(os.path.join(train_folder, filename), "rb") as f: data = pickle.load(f) crd_bb
-= data["crd_bb"] seq = data["seq"] ... ``` Alternatively, you can use our
-`ProteinDataset` or `ProteinLoader` classes for convenient processing. Among
-other things, they allow for feature extraction, single chain / homomer /
-heteromer filtering and randomized sampling from sequence identity clusters.
-For example, here is how we can create a data loader that: - samples a
-different cluster representative at every epoch, - extracts dihedral angles,
-sidechain orientation and secondary structure features, - only loads pairs of
-interacting proteins (larger biounits are broken up into pairs), - has batch
-size 8. ```python from proteinflow import ProteinLoader train_loader =
-ProteinLoader.from_args( "./data/proteinflow_new/training",
-clustering_dict_path="./data/proteinflow_new/splits_dict/train.pickle",
+are marked with `'-'`. Note that the sequence information in the PDB files is
+aligned to the FASTA sequences to identify the missing residues. Once your data
+is ready, you can open the files with `pickle` directly. ```python import
+pickle import os train_folder = "./data/proteinflow_new/training" for filename
+in os.listdir(train_folder): with open(os.path.join(train_folder, filename),
+"rb") as f: data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ...
+``` Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes
+for convenient processing. Among other things, they allow for feature
+extraction, single chain / homomer / heteromer filtering and randomized
+sampling from sequence identity clusters. For example, here is how we can
+create a data loader that: - samples a different cluster representative at
+every epoch, - extracts dihedral angles, sidechain orientation and secondary
+structure features, - only loads pairs of interacting proteins (larger biounits
+are broken up into pairs), - has batch size 8. ```python from proteinflow
+import ProteinLoader train_loader = ProteinLoader.from_args( "./data/
+proteinflow_new/training", clustering_dict_path="./data/proteinflow_new/
+splits_dict/train.pickle",
 node_features_type="dihedral+sidechain_orientation+secondary_structure",
 entry_type="pair", batch_size=8, ) for batch in train_loader: crd_bb = batch
 ["X"] #(B, L, 4, 3) seq = batch["S"] #(B, L) sse = batch["secondary_structure"]
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
```

### Comparing `proteinflow-1.3.1/proteinflow/__init__.py` & `proteinflow-1.3.2/proteinflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ## Usage
 ### Downloading pre-computed datasets (stable)
 Already precomputed datasets with consensus set of parameters and can be accessed and downloaded using the `proteinflow`. package. Check the output of `proteinflow check_tags` for a list of available tags.
 ```bash
 proteinflow download --tag 20230102_stable 
 ```
 
-### Running the pipeline
+### Running the pipeline (PDB)
 You can also run `proteinflow` with your own parameters. Check the output of `proteinflow check_snapshots` for a list of available PDB snapshots (naming rule: `yyyymmdd`).
 
 For instance, let's generate a dataset with the following description:
 - resolution threshold: 5 angstrom,
 - PDB snapshot: 20190101,
 - structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
 - sequence identity threshold for clustering: 40% sequence similarity,
@@ -64,16 +64,30 @@
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
 A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
-You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
+### Running the pipeline (SAbDab)
+You can also use the `--sabdab` option in `proteinflow generate` to load files from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will download the latest up-to-date version of the SabDab dataset and cluster the antibodies based on their CDR sequence.
+Alternatively, it can be used together with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or folder. This allows you to use search and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a custom dataset by downloading the archived zip file of the structures selected. (Under Downloads section of your SabDab query).
 
+SAbDab sequences clustering is done across all 6 Complementary Determining Regions (CDRs) - CDRH1, CDRH2, CDRH3, CDRL1, CDRL2, CDRL3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic constructs are clustered together with other heavy chain CDRs. The resulting CDR clusters are split into training, test and validation in a way that ensures that every PDB file only appears in one subset.
+
+For instance, let's generate a dataset with the following description:
+- SabDab version: latest (up-to-date),
+- resolution threshold: 5 angstrom,
+- structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
+- sequence identity threshold for clustering (CDRs): 40%,
+- size of validation subset: 10%.
+
+```bash
+proteinflow generate --sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split 0.1
+```
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
 ```
@@ -122,18 +136,18 @@
     "./data/proteinflow_new/training", 
     clustering_dict_path="./data/proteinflow_new/splits_dict/train.pickle",
     node_features_type="dihedral+sidechain_orientation+secondary_structure",
     entry_type="pair",
     batch_size=8,
 )
 for batch in train_loader:
-    crd_bb = batch["X"] #(B, L, 4, 3)
-    seq = batch["S"] #(B, L)
-    sse = batch["secondary_structure"] #(B, L, 3)
-    to_predict = batch["masked_res"] #(B, L), 1 where the residues should be masked, 0 otherwise
+    crd_bb = batch["X"] # (B, L, 4, 3)
+    seq = batch["S"] # (B, L)
+    sse = batch["secondary_structure"] # (B, L, 3)
+    to_predict = batch["masked_res"] # (B, L), 1 where the residues should be masked, 0 otherwise
     ...
 ```
 
 """
 
 __pdoc__ = {"utils": False, "scripts": False}
 __docformat__ = "numpy"
@@ -315,14 +329,23 @@
     FEATURES_DICT["charge"][x],
     FEATURES_DICT["polarity"][x],
     FEATURES_DICT["acceptor"][x],
     FEATURES_DICT["donor"][x],
 ]
 CDR = {"-": 0, "H1": 1, "H2": 2, "H3": 3, "L1": 4, "L2": 5, "L3": 6}
 
+ALLOWED_AG_TYPES = {
+    "protein",
+    "protein | protein",
+    "protein | protein | protein",
+    "protein | protein | protein | protein | protein",
+    "protein | protein | protein | protein",
+    np.nan,
+}
+
 
 def _clean(pdb_id, tmp_folder):
     """
     Remove all temporary files associated with a PDB ID
     """
     for file in os.listdir(tmp_folder):
         if file.startswith(f"{pdb_id}."):
@@ -388,15 +411,15 @@
         The percentage of chains to put in the validation set (default 5%)
     out_split_dict_folder : str, default "./data/dataset_splits_dict"
         The folder where the dictionaries containing the train/validation/test splits information will be saved"
     min_seq_id : float in [0, 1], default 0.3
         minimum sequence identity for `mmseqs`
     """
 
-    sample_file = os.listdir(output_folder)[0]
+    sample_file = [x for x in os.listdir(output_folder) if x.endswith(".pickle")][0]
     ind = sample_file.split(".")[0].split("-")[1]
     sabdab = not ind.isnumeric()
 
     os.makedirs(out_split_dict_folder, exist_ok=True)
     (
         train_clusters_dict,
         train_classes_dict,
@@ -436,15 +459,14 @@
     else:
         raise e
 
 
 def _run_processing(
     tmp_folder="./data/tmp_pdb",
     output_folder="./data/pdb",
-    log_folder="./data/logs",
     min_length=30,
     max_length=10000,
     resolution_thr=3.5,
     missing_ends_thr=0.3,
     missing_middle_thr=0.1,
     filter_methods=True,
     remove_redundancies=False,
@@ -478,16 +500,14 @@
 
     Parameters
     ----------
     tmp_folder : str, default "./data/tmp_pdb"
         The folder where temporary files will be saved
     output_folder : str, default "./data/pdb"
         The folder where the output files will be saved
-    log_folder : str, default "./data/logs"
-        The folder where the log file will be saved
     min_length : int, default 30
         The minimum number of non-missing residues per chain
     max_length : int, default 10000
         The maximum number of residues per chain (set None for no threshold)
     resolution_thr : float, default 3.5
         The maximum resolution
     missing_ends_thr : float, default 0.3
@@ -541,21 +561,16 @@
     MISSING_ENDS_THR = missing_ends_thr
     MISSING_MIDDLE_THR = missing_middle_thr
 
     if not os.path.exists(TMP_FOLDER):
         os.makedirs(TMP_FOLDER)
     if not os.path.exists(OUTPUT_FOLDER):
         os.makedirs(OUTPUT_FOLDER)
-    if not os.path.exists(log_folder):
-        os.makedirs(log_folder)
 
-    i = 0
-    while os.path.exists(os.path.join(log_folder, f"log_{i}.txt")):
-        i += 1
-    LOG_FILE = os.path.join(log_folder, f"log_{i}.txt")
+    LOG_FILE = os.path.join(OUTPUT_FOLDER, f"log.txt")
     print(f"Log file: {LOG_FILE} \n")
     now = datetime.now()  # current date and time
     date_time = now.strftime("%m/%d/%Y, %H:%M:%S") + "\n\n"
     with open(LOG_FILE, "a") as f:
         f.write(date_time)
         if tag is not None:
             f.write(f"tag: {tag} \n\n")
@@ -603,51 +618,53 @@
                 _log_exception(e, LOG_FILE, pdb_id, TMP_FOLDER, chain_id=chain_id)
 
     try:
         paths, error_ids = _load_files(
             resolution_thr=RESOLUTION_THR,
             filter_methods=filter_methods,
             pdb_snapshot=pdb_snapshot,
-            log_folder=log_folder,
             n=n,
             tmp_folder=TMP_FOLDER,
             load_live=load_live,
             sabdab=sabdab,
             sabdab_data_path=sabdab_data_path,
             require_antigen=require_antigen,
         )
         for id in error_ids:
             with open(LOG_FILE, "a") as f:
                 f.write(f"<<< Could not download PDB/mmCIF file: {id} \n")
-        # for x in [("data/tmp/5ivn.pdb", "A_nan_B")]:
-        #     process_f(x, show_error=True, force=force, sabdab=True)
+        # paths = [(os.path.join(TMP_FOLDER, "6tkb.pdb"), "H_L_nan")]
         print("Filter and process...")
         _ = p_map(lambda x: process_f(x, force=force, sabdab=sabdab), paths)
         # _ = [process_f(x, force=force, sabdab=sabdab, show_error=True) for x in tqdm(paths)]
     except Exception as e:
         _raise_rcsbsearch(e)
 
     stats = get_error_summary(LOG_FILE, verbose=False)
     not_found_error = "<<< PDB / mmCIF file downloaded but not found"
-    while not_found_error in stats:
-        with open(LOG_FILE, "r") as f:
-            lines = [x for x in f.readlines() if not x.startswith(not_found_error)]
-        os.remove(LOG_FILE)
-        with open(f"{LOG_FILE}_tmp", "a") as f:
-            for line in lines:
-                f.write(line)
-        if sabdab:
-            paths = [
-                (os.path.join(TMP_FOLDER, x.split("-")[0] + ".pdb"), x.split("-")[1])
-                for x in stats[not_found_error]
-            ]
-        else:
-            paths = stats[not_found_error]
-        _ = p_map(lambda x: process_f(x, force=force, sabdab=sabdab), paths)
-        stats = get_error_summary(LOG_FILE, verbose=False)
+    if not sabdab:
+        while not_found_error in stats:
+            with open(LOG_FILE, "r") as f:
+                lines = [x for x in f.readlines() if not x.startswith(not_found_error)]
+            os.remove(LOG_FILE)
+            with open(f"{LOG_FILE}_tmp", "a") as f:
+                for line in lines:
+                    f.write(line)
+            if sabdab:
+                paths = [
+                    (
+                        os.path.join(TMP_FOLDER, x.split("-")[0] + ".pdb"),
+                        x.split("-")[1],
+                    )
+                    for x in stats[not_found_error]
+                ]
+            else:
+                paths = stats[not_found_error]
+            _ = p_map(lambda x: process_f(x, force=force, sabdab=sabdab), paths)
+            stats = get_error_summary(LOG_FILE, verbose=False)
     if os.path.exists(f"{LOG_FILE}_tmp"):
         with open(LOG_FILE, "r") as f:
             lines = [x for x in f.readlines() if not x.startswith(not_found_error)]
         os.remove(LOG_FILE)
         with open(f"{LOG_FILE}_tmp", "a") as f:
             for line in lines:
                 f.write(line)
@@ -868,15 +885,14 @@
         return self.pad_collate(batch)
 
 
 def _get_pdb_ids(
     resolution_thr=3.5,
     pdb_snapshot=None,
     filter_methods=True,
-    log_folder="data/tmp/logs",
 ):
     """
     Get PDB ids from PDB API
     """
 
     # get filtered PDB ids from PDB API
     pdb_ids = (
@@ -963,28 +979,26 @@
         return None
 
 
 def _load_pdb(
     resolution_thr=3.5,
     pdb_snapshot=None,
     filter_methods=True,
-    log_folder="data/tmp/logs",
     n=None,
     tmp_folder="data/tmp",
     load_live=False,
 ):
     """
     Download filtered PDB files and return a list of local file paths
     """
 
     ordered_folders, pdb_ids = _get_pdb_ids(
         resolution_thr=resolution_thr,
         pdb_snapshot=pdb_snapshot,
         filter_methods=filter_methods,
-        log_folder=log_folder,
     )
     with ThreadPoolExecutor(max_workers=8) as executor:
         print("Getting a file list...")
         ids = []
         for i, x in enumerate(tqdm(pdb_ids)):
             ids.append(x)
             if n is not None and i == n:
@@ -1087,14 +1101,15 @@
             os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip")
             for method in methods
         ]
     else:
         paths = [sabdab_data_path]
     ids = []
     pdb_ids = []
+    error_ids = []
     print("Moving files...")
     for path in paths:
         if not os.path.isdir(path):
             if not path.endswith(".zip"):
                 raise ValueError("SAbDab data path should be a zip file or a directory")
             dir_path = path[:-4]
             print(f"Unzipping {path}...")
@@ -1113,18 +1128,21 @@
         for file in os.listdir(dir_path):
             if file.endswith(".tsv"):
                 summary_path = os.path.join(dir_path, file)
                 break
         if summary_path is None:
             raise ValueError("Summary file not found")
         summary = pd.read_csv(summary_path, sep="\t")
+        # check antigen type
+        summary = summary[summary["antigen_type"].isin(ALLOWED_AG_TYPES)]
         # filter out structures with repeating chains
         summary = summary[summary["antigen_chain"] != summary["Hchain"]]
         summary = summary[summary["antigen_chain"] != summary["Lchain"]]
         summary = summary[summary["Lchain"] != summary["Hchain"]]
+        # optional filters
         if require_antigen:
             summary = summary[~summary["antigen_chain"].isna()]
         if pdb_snapshot is not None:
             date = pd.to_datetime(summary["date"], format="%m/%d/%Y")
             summary = summary[date <= pdb_snapshot]
         if sabdab_data_path is not None:
             summary.loc[summary["resolution"] == "NOT", "resolution"] = 0
@@ -1136,45 +1154,50 @@
                     summary["method"].isin([" ".join(m) for m in methods])
                 ]
         if n is not None:
             summary = summary.iloc[:n]
         ids_method = summary["pdb"].unique().tolist()
         for id in tqdm(ids_method):
             pdb_path = os.path.join(dir_path, "chothia", f"{id}.pdb")
-            shutil.move(pdb_path, os.path.join(tmp_folder, f"{id}.pdb"))
+            try:
+                if sabdab_data_path is None or not os.path.isdir(sabdab_data_path):
+                    shutil.move(pdb_path, os.path.join(tmp_folder, f"{id}.pdb"))
+                else:
+                    shutil.copy(pdb_path, os.path.join(tmp_folder, f"{id}.pdb"))
+            except FileNotFoundError:
+                error_ids.append(id)
         if sabdab_data_path is None or sabdab_data_path.endswith(".zip"):
             shutil.rmtree(dir_path)
         ids_full = summary.apply(
             lambda x: (x["pdb"], f"{x['Hchain']}_{x['Lchain']}_{x['antigen_chain']}"),
             axis=1,
         ).tolist()
         ids += ids_full
         pdb_ids += ids_method
     print("Downloading fasta files...")
     with ThreadPoolExecutor(max_workers=8) as executor:
+        # pdb_ids = ["6tkb"]
         future_to_key = {
             executor.submit(
                 lambda x: _download_fasta_f(x, datadir=tmp_folder), key
             ): key
             for key in pdb_ids
         }
         _ = [
             x.result()
             for x in tqdm(futures.as_completed(future_to_key), total=len(pdb_ids))
         ]
     paths = [(os.path.join(tmp_folder, f"{x[0]}.pdb"), x[1]) for x in ids]
-    error_ids = []
     return paths, error_ids
 
 
 def _load_files(
     resolution_thr=3.5,
     pdb_snapshot=None,
     filter_methods=True,
-    log_folder="data/tmp/logs",
     n=None,
     tmp_folder="data/tmp",
     load_live=False,
     sabdab=False,
     sabdab_data_path=None,
     require_antigen=False,
 ):
@@ -1196,15 +1219,14 @@
         out = _load_pdb(
             resolution_thr=resolution_thr,
             filter_methods=filter_methods,
             pdb_snapshot=pdb_snapshot,
             tmp_folder=tmp_folder,
             load_live=load_live,
             n=n,
-            log_folder=log_folder,
         )
     return out
 
 
 def download_data(tag, local_datasets_folder="./data", skip_splitting=False):
     """
     Download a pre-computed dataset with train/test/validation splits
@@ -1331,32 +1353,29 @@
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
 
     """
-    _check_mmseqs()
     filter_methods = not not_filter_methods
     remove_redundancies = not not_remove_redundancies
     tmp_id = "".join(
         random.choice(string.ascii_uppercase + string.digits) for _ in range(5)
     )
     tmp_folder = os.path.join("", "tmp", tag + tmp_id)
     output_folder = os.path.join(local_datasets_folder, f"proteinflow_{tag}")
-    log_folder = os.path.join(local_datasets_folder, "logs")
     out_split_dict_folder = os.path.join(output_folder, "splits_dict")
 
     if force and os.path.exists(output_folder):
         shutil.rmtree(output_folder)
 
     log_dict = _run_processing(
         tmp_folder=tmp_folder,
         output_folder=output_folder,
-        log_folder=log_folder,
         min_length=min_length,
         max_length=max_length,
         resolution_thr=resolution_thr,
         missing_ends_thr=missing_ends_thr,
         missing_middle_thr=missing_middle_thr,
         filter_methods=filter_methods,
         remove_redundancies=remove_redundancies,
@@ -1527,27 +1546,27 @@
             tag,
             local_datasets_folder,
             os.path.join(local_datasets_folder, "tmp"),
             exclude_chains,
             exclude_threshold,
         )
 
-    _check_mmseqs()
     tmp_folder = os.path.join(local_datasets_folder, "tmp")
     output_folder = os.path.join(local_datasets_folder, f"proteinflow_{tag}")
     out_split_dict_folder = os.path.join(output_folder, "splits_dict")
     exists = False
 
     if os.path.exists(out_split_dict_folder):
         if not ignore_existing:
             warnings.warn(
                 f"Found an existing dictionary for tag {tag}. proteinflow will load it and ignore the parameters! Run with --ignore_existing to overwrite."
             )
             exists = True
     if not exists:
+        _check_mmseqs()
         _get_split_dictionaries(
             tmp_folder=tmp_folder,
             output_folder=output_folder,
             split_tolerance=split_tolerance,
             test_split=test_split,
             valid_split=valid_split,
             out_split_dict_folder=out_split_dict_folder,
@@ -1555,14 +1574,44 @@
         )
 
     _split_data(
         output_folder, excluded_biounits, exclude_clusters, exclude_based_on_cdr
     )
 
 
+def unsplit_data(
+    tag,
+    local_datasets_folder="./data",
+):
+    """
+    Move files from train, test, validation and excluded folders back into the main folder
+
+    Parameters
+    ----------
+    tag : str
+        the name of the dataset
+    local_datasets_folder : str, default "./data"
+        the path to the folder that stores proteinflow datasets
+    """
+
+    for folder in ["excluded", "train", "test", "valid"]:
+        if not os.path.exists(
+            os.path.join(local_datasets_folder, f"proteinflow_{tag}", folder)
+        ):
+            continue
+        for file in os.listdir(
+            os.path.join(local_datasets_folder, f"proteinflow_{tag}", folder)
+        ):
+            shutil.move(
+                os.path.join(local_datasets_folder, f"proteinflow_{tag}", folder, file),
+                os.path.join(local_datasets_folder, f"proteinflow_{tag}", file),
+            )
+        shutil.rmtree(os.path.join(local_datasets_folder, f"proteinflow_{tag}", folder))
+
+
 class ProteinDataset(Dataset):
     """
     Dataset to load proteinflow data
 
     Saves the model input tensors as pickle files in `features_folder`. When `clustering_dict_path` is provided,
     at each iteration a random biounit from a cluster is sampled.
 
@@ -1588,15 +1637,15 @@
     - `'secondary_structure'`: a one-hot encoding of secondary structure ([alpha-helix, beta-sheet, coil]), `(total_L, 3)`,
     - `'sidechain_coords'`: the coordinates of the sidechain atoms (see `proteinflow.sidechain_order()` for the order), `(total_L, 10, 3)`.
 
     If the dataset contains a `'cdr'` key (if it was generated from SAbDab files), the output files will also additionally contain a `'cdr'`
     key with a CDR tensor of length `total_L`. In the array, the CDR residues are marked with the corresponding CDR type
     (H1=1, H2=2, H3=3, L1=4, L2=5, L3=6) and the rest of the residues are marked with 0s.
 
-    Use the `set_cdr` method to only iterate over biounits that contain specific CDRs.
+    Use the `set_cdr` method to only iterate over specific CDRs.
 
     In order to compute additional features, use the `feature_functions` parameter. It should be a dictionary with keys
     corresponding to the feature names and values corresponding to the functions that compute the features. The functions
     should take a chain dictionary and an integer representation of the sequence as input (the dictionary is in `proteinflow` format,
     see the docs for `generate_data` for details) and return a `numpy` array shaped as `(#residues, #features)`.
 
     """
@@ -1702,15 +1751,17 @@
         if not os.path.exists(self.features_folder):
             os.makedirs(self.features_folder)
 
         self.interpolate = interpolate
         # generate the feature files
         print("Processing files...")
         if debug_file_path is None:
-            to_process = os.listdir(dataset_folder)
+            to_process = [
+                x for x in os.listdir(dataset_folder) if x.endswith(".pickle")
+            ]
         else:
             to_process = [debug_file_path]
         if clustering_dict_path is not None and use_fraction < 1:
             with open(clustering_dict_path, "rb") as f:
                 clusters = pickle.load(f)
             keys = sorted(clusters.keys())[: int(len(clusters) * use_fraction)]
             to_process = set()
@@ -2111,15 +2162,15 @@
 
     def set_cdr(self, cdr):
         """
         Set the CDR to be iterated over (only for SAbDab datasets).
 
         Parameters
         ----------
-        cdr : str
+        cdr : {"H1", "H2", "H3", "L1", "L2", "L3"}
             The CDR to be iterated over. Set to `None` to go back to iterating over all chains.
         """
 
         if not self.sabdab:
             cdr = None
         if cdr == self.cdr:
             return
```

### Comparing `proteinflow-1.3.1/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.3.2/proteinflow/scripts/proteinflow_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from proteinflow import (
     check_download_tags,
     check_pdb_snapshots,
     download_data,
     generate_data,
     split_data,
     get_error_summary,
+    unsplit_data,
 )
 import click
 
 
 @click.group(help="A data processing pipeline for protein design ML tasks")
 def cli():
     pass
@@ -223,14 +224,31 @@
     "split",
     help="Split an existing ProteinFlow dataset into training, validation and test subset according to MMseqs clustering and homomer/heteromer/single chain proportions",
 )
 def split(**kwargs):
     split_data(**kwargs)
 
 
+@click.option(
+    "--tag",
+    help="The name of the dataset",
+)
+@click.option(
+    "--local_datasets_folder",
+    default="./data",
+    help="The folder where proteinflow datasets are stored",
+)
+@cli.command(
+    "unsplit",
+    help="Move files from train, test, validation and excluded folders back into the main folder",
+)
+def unsplit(**kwargs):
+    unsplit_data(**kwargs)
+
+
 @click.argument("log_path")
 @cli.command("get_summary", help="Get a summary of filtering reasons from a log file")
 def get_summary(log_path):
     get_error_summary(log_path)
 
 
 if __name__ == "__main__":
```

### Comparing `proteinflow-1.3.1/proteinflow/utils/async_download.py` & `proteinflow-1.3.2/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/proteinflow/utils/biotite_sse.py` & `proteinflow-1.3.2/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/proteinflow/utils/build_pdb.py` & `proteinflow-1.3.2/proteinflow/utils/build_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.3.2/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

```diff
@@ -80,15 +80,15 @@
 def _load_pdbs(dir, cdr=None):
     """
     Load biounits and group their sequences by PDB and similarity (90%)
     """
 
     seqs_dict = defaultdict(lambda: [])
 
-    for file in tqdm(os.listdir(dir)):
+    for file in tqdm([x for x in os.listdir(dir) if x.endswith(".pickle")]):
         load_path = os.path.join(dir, file)
         if os.path.isdir(load_path):
             continue
         with open(load_path, "rb") as f:
             pdb_dict = pkl.load(f)
         if cdr is None:
             seqs = [(chain, pdb_dict[chain]["seq"]) for chain in pdb_dict.keys()]
@@ -1204,18 +1204,18 @@
         )
         clusters_dict.update(c_dict)
         clusters_pdb_dict.update(c_pdb_dict)
 
     subprocess.run(["rm", "-r", os.path.join(tmp_folder, "MMSeqs2_results")])
     graph = _make_graph(clusters_pdb_dict)
 
-    import pickle
+    # import pickle
 
-    with open("graph.pickle", "wb") as f:
-        pickle.dump(graph, f)
+    # with open("graph.pickle", "wb") as f:
+    #     pickle.dump(graph, f)
 
     # perform the splitting into train, validation and tesst sets
     (
         train_clusters_dict,
         train_classes_dict,
         valid_clusters_dict,
         valid_classes_dict,
```

### Comparing `proteinflow-1.3.1/proteinflow/utils/filter_database.py` & `proteinflow-1.3.2/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.3.2/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/proteinflow/utils/process_pdb.py` & `proteinflow-1.3.2/proteinflow/utils/process_pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,27 +277,24 @@
             else:
                 p = PandasPdb().read_pdb(file_path).get_model(1)
     except FileNotFoundError:
         raise PDBError("PDB / mmCIF file downloaded but not found")
     out_dict["crd_raw"] = p.df["ATOM"]
     out_dict["seq_df"] = p.amino3to1()
 
-    # # add metadata
-    # metadata = parse_pdb_header(file_path)
-    # for key in ["structure_method"]:
-    #     out_dict[key] = metadata.get(key)
-
     # retrieve sequences that are relevant for this PDB from the fasta file
     if chain_id is None:
         chains = p.df["ATOM"]["chain_id"].unique()
     else:
-        H, L, A = chain_id.split("_")
-        chains = [H, L] + A.split(" | ")
+        h, l, a = chain_id.split("_")
+        chains = [h, l] + a.split(" | ")
         chains = [x for x in chains if x != "nan"]
     seqs_dict = {k.upper(): v for k, v in seqs_dict.items()}
+    if all([len(x) == 3 and len(set(list(x))) == 1 for x in seqs_dict.keys()]):
+        seqs_dict = {k[0]: v for k, v in seqs_dict.items()}
 
     if not set([x.split("-")[0].upper() for x in chains]).issubset(
         set(list(seqs_dict.keys()))
     ):
         raise PDBError("Some chains in the PDB do not appear in the fasta file")
 
     out_dict["fasta"] = {k: seqs_dict[k.split("-")[0].upper()] for k in chains}
```

### Comparing `proteinflow-1.3.1/proteinflow/utils/split_dataset.py` & `proteinflow-1.3.2/proteinflow/utils/split_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 
 def _biounits_in_clusters_dict(clusters_dict, excluded_files=None):
     """
     Return the list of all biounit files present in clusters_dict
     """
 
+    if len(clusters_dict) == 0:
+        return np.array([])
     if excluded_files is None:
         excluded_files = []
     return np.unique(
         [
             c[0]
             for c in list(np.concatenate(list(clusters_dict.values())))
             if c[0] not in excluded_files
```

### Comparing `proteinflow-1.3.1/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: proteinflow
-Version: 1.3.1
-Summary: Versatile pipeline for processing protein structure data for deep learning applications.
-Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
-License: BSD-3-Clause
-Keywords: bioinformatics,dataset,protein,PDB,deep learning
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
     <b> ProteinFlow - A data processing pipeline for all your protein design needs </b> <br />
 </p>
 
 <p align="center">
   <a href="https://adaptyvbio.github.io/ProteinFlow/" target="_blank">
       Docs
@@ -74,15 +63,15 @@
 ## Usage
 ### Downloading pre-computed datasets (stable)
 Already precomputed datasets with consensus set of parameters and can be accessed and downloaded using the `proteinflow`. package. Check the output of `proteinflow check_tags` for a list of available tags.
 ```bash
 proteinflow download --tag 20230102_stable 
 ```
 
-### Running the pipeline
+### Running the pipeline (PDB)
 You can also run `proteinflow` with your own parameters. Check the output of `proteinflow check_snapshots` for a list of available PDB snapshots (naming rule: `yyyymmdd`).
 
 For instance, let's generate a dataset with the following description:
 - resolution threshold: 5 angstrom,
 - PDB snapshot: 20190101,
 - structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
 - sequence identity threshold for clustering: 40% sequence similarity,
@@ -94,15 +83,32 @@
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
 A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
 
-You can also use the `--sabdab` option to load files from SAbDab and cluster them based on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip file.
+### Running the pipeline (SAbDab)
+You can also use the `--sabdab` option in `proteinflow generate` to load files from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will download the latest up-to-date version of the SabDab dataset and cluster the antibodies based on their CDR sequence.
+Alternatively, it can be used together with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or folder. This allows you to use search and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a custom dataset by downloading the archived zip file of the structures selected. (Under Downloads section of your SabDab query).
+
+SAbDab sequences clustering is done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1, L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic constructs are clustered together with other heavy chain CDRs. The resulting CDR clusters are split into training, test and validation in a way that ensures that every PDB file only appears in one subset.
+
+Individual output pickle files represent heavy chain - light chain - antigen complexes (created from SAbDab annotation, sometimes more than one per PDB entry). Each of the elements (heavy chain, light chain, antigen) can be missing in specific entries and there can be multiple antigen chains. In order to filter for at least one antigen chain, use the `--require_antigen` option.
+
+For instance, let's generate a dataset with the following description:
+- SabDab version: latest (up-to-date),
+- resolution threshold: 5 angstrom,
+- structure methods accepted: all (x-ray christolography, NRM, Cryo-EM),
+- sequence identity threshold for clustering (CDRs): 40%,
+- size of validation subset: 10%.
+
+```bash
+proteinflow generate --sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split 0.1
+```
 
 ### Splitting
 By default, both `proteinflow generate` and `proteinflow download` will also split your data into training, test and validation according to MMseqs2 clustering and homomer/heteromer/single chain proportions. However, you can skip this step with a `--skip_splitting` flag and then perform it separately with the `proteinflow split` command.
 
 The following command will perform the splitting with a 10% validation set, a 5% test set and a 50% threshold for sequence identity clusters.
 ```bash
 proteinflow split --tag new --valid_split 0.1 --test_split 0.5 --min_seq_id 0.5
@@ -115,18 +121,20 @@
 - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
 - `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check `proteinflow.sidechain_order()` for the order of atoms),
 - `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with known coordinates and
     zeros to missing values,
 - `'seq'`: a string of length `L` with residue types.
 
 In a SAbDab datasets, an additional key is added to the dictionary:
-- `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
+- `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...) 
     and non-CDR residues are marked with `'-'`.
+    
+Note that the sequence information in the PDB files is aligned to the FASTA sequences to identify the missing residues.
 
-Once your data is ready, you can open the files with `pickle`.
+Once your data is ready, you can open the files with `pickle` directly.
 
 ```python
 import pickle
 import os
 
 train_folder = "./data/proteinflow_new/training"
 for filename in os.listdir(train_folder):
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.1 Summary: Versatile
-pipeline for processing protein structure data for deep learning applications.
-Author-email: Liza Kozlova
-adaptyvbio.com>, Arthur Valentin
-adaptyvbio.com> License: BSD-3-Clause Keywords:
-bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
                                      Docs
 --- [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)]
 (https://opensource.org/licenses/BSD-3-Clause) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/
 project/proteinflow/) [![Conda](https://img.shields.io/conda/v/adaptyvbio/
@@ -43,34 +36,58 @@
 github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
 The docker image can be accessed in interactive mode with this command. ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
 ### Downloading pre-computed datasets (stable) Already precomputed datasets
 with consensus set of parameters and can be accessed and downloaded using the
 `proteinflow`. package. Check the output of `proteinflow check_tags` for a list
 of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
-Running the pipeline You can also run `proteinflow` with your own parameters.
-Check the output of `proteinflow check_snapshots` for a list of available PDB
-snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
-with the following description: - resolution threshold: 5 angstrom, - PDB
-snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
-NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
-similarity, - maximum length per sequence: 1000 residues, - minimum length per
-sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
-size of validation subset: 10%. ```bash proteinflow generate --tag new --
-resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
---max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
-See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
-generate --help`) for the full list of parameters and more information. A
-registry of all the files that are removed during the filtering as well as
-description with the reason for their removal is created automatically for each
-`generate` command. The log files are save (at `data/logs` by default) and a
-summary can be accessed running `proteinflow get_summary {log_path}`. You can
-also use the `--sabdab` option to load files from SAbDab and cluster them based
-on CDRs. Use together with `--zip_path` to process a custom SAbDab-like zip
-file. ### Splitting By default, both `proteinflow generate` and `proteinflow
+Running the pipeline (PDB) You can also run `proteinflow` with your own
+parameters. Check the output of `proteinflow check_snapshots` for a list of
+available PDB snapshots (naming rule: `yyyymmdd`). For instance, let's generate
+a dataset with the following description: - resolution threshold: 5 angstrom, -
+PDB snapshot: 20190101, - structure methods accepted: all (x-ray
+christolography, NRM, Cryo-EM), - sequence identity threshold for clustering:
+40% sequence similarity, - maximum length per sequence: 1000 residues, -
+minimum length per sequence: 5 residues, - maximum fraction of missing values
+at the ends: 10%, - size of validation subset: 10%. ```bash proteinflow
+generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --
+not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --
+missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs](https://
+adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the
+full list of parameters and more information. A registry of all the files that
+are removed during the filtering as well as description with the reason for
+their removal is created automatically for each `generate` command. The log
+files are save (at `data/logs` by default) and a summary can be accessed
+running `proteinflow get_summary {log_path}`. ### Running the pipeline (SAbDab)
+You can also use the `--sabdab` option in `proteinflow generate` to load files
+from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will
+download the latest up-to-date version of the SabDab dataset and cluster the
+antibodies based on their CDR sequence. Alternatively, it can be used together
+with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or
+folder. This allows you to use search and query tools from the [SabDab web
+interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a
+custom dataset by downloading the archived zip file of the structures selected.
+(Under Downloads section of your SabDab query). SAbDab sequences clustering is
+done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1,
+L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/
+9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic
+constructs are clustered together with other heavy chain CDRs. The resulting
+CDR clusters are split into training, test and validation in a way that ensures
+that every PDB file only appears in one subset. Individual output pickle files
+represent heavy chain - light chain - antigen complexes (created from SAbDab
+annotation, sometimes more than one per PDB entry). Each of the elements (heavy
+chain, light chain, antigen) can be missing in specific entries and there can
+be multiple antigen chains. In order to filter for at least one antigen chain,
+use the `--require_antigen` option. For instance, let's generate a dataset with
+the following description: - SabDab version: latest (up-to-date), - resolution
+threshold: 5 angstrom, - structure methods accepted: all (x-ray
+christolography, NRM, Cryo-EM), - sequence identity threshold for clustering
+(CDRs): 40%, - size of validation subset: 10%. ```bash proteinflow generate --
+sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split
+0.1 ``` ### Splitting By default, both `proteinflow generate` and `proteinflow
 download` will also split your data into training, test and validation
 according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
 However, you can skip this step with a `--skip_splitting` flag and then perform
 it separately with the `proteinflow split` command. The following command will
 perform the splitting with a 10% validation set, a 5% test set and a 50%
 threshold for sequence identity clusters. ```bash proteinflow split --tag new -
 -valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
@@ -80,31 +97,33 @@
 are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
 array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
 `'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
 coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
 `'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
 known coordinates and zeros to missing values, - `'seq'`: a string of length
 `L` with residue types. In a SAbDab datasets, an additional key is added to the
-dictionary: - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are
+dictionary: - `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are
 marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
-are marked with `'-'`. Once your data is ready, you can open the files with
-`pickle`. ```python import pickle import os train_folder = "./data/
-proteinflow_new/training" for filename in os.listdir(train_folder): with open
-(os.path.join(train_folder, filename), "rb") as f: data = pickle.load(f) crd_bb
-= data["crd_bb"] seq = data["seq"] ... ``` Alternatively, you can use our
-`ProteinDataset` or `ProteinLoader` classes for convenient processing. Among
-other things, they allow for feature extraction, single chain / homomer /
-heteromer filtering and randomized sampling from sequence identity clusters.
-For example, here is how we can create a data loader that: - samples a
-different cluster representative at every epoch, - extracts dihedral angles,
-sidechain orientation and secondary structure features, - only loads pairs of
-interacting proteins (larger biounits are broken up into pairs), - has batch
-size 8. ```python from proteinflow import ProteinLoader train_loader =
-ProteinLoader.from_args( "./data/proteinflow_new/training",
-clustering_dict_path="./data/proteinflow_new/splits_dict/train.pickle",
+are marked with `'-'`. Note that the sequence information in the PDB files is
+aligned to the FASTA sequences to identify the missing residues. Once your data
+is ready, you can open the files with `pickle` directly. ```python import
+pickle import os train_folder = "./data/proteinflow_new/training" for filename
+in os.listdir(train_folder): with open(os.path.join(train_folder, filename),
+"rb") as f: data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ...
+``` Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes
+for convenient processing. Among other things, they allow for feature
+extraction, single chain / homomer / heteromer filtering and randomized
+sampling from sequence identity clusters. For example, here is how we can
+create a data loader that: - samples a different cluster representative at
+every epoch, - extracts dihedral angles, sidechain orientation and secondary
+structure features, - only loads pairs of interacting proteins (larger biounits
+are broken up into pairs), - has batch size 8. ```python from proteinflow
+import ProteinLoader train_loader = ProteinLoader.from_args( "./data/
+proteinflow_new/training", clustering_dict_path="./data/proteinflow_new/
+splits_dict/train.pickle",
 node_features_type="dihedral+sidechain_orientation+secondary_structure",
 entry_type="pair", batch_size=8, ) for batch in train_loader: crd_bb = batch
 ["X"] #(B, L, 4, 3) seq = batch["S"] #(B, L) sse = batch["secondary_structure"]
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
```

### Comparing `proteinflow-1.3.1/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.3.2/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/pyproject.toml` & `proteinflow-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-1.3.1/tests/test_download.py` & `proteinflow-1.3.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.1/tests/test_generate.py` & `proteinflow-1.3.2/tests/test_generate.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         shutil.rmtree(folder)
     start = time()
     generate_data(tag="test", skip_splitting=True, n=50)
     end = time()
     num_files = len(os.listdir(folder))
     split_data(tag="test", valid_split=0.2, test_split=0.1, ignore_existing=True)
     assert os.path.exists(folder)
-    assert len(os.listdir(folder)) == 4
+    assert len(os.listdir(folder)) == 5
     num_files_split = 0
 
     for subset in ["train", "valid", "test"]:
         num_files_split += len(os.listdir(os.path.join(folder, subset)))
         subset_folder = os.path.join(folder, subset)
         with open(os.path.join(folder, "splits_dict", f"{subset}.pickle"), "rb") as f:
             for _ in range(2):
@@ -57,14 +57,14 @@
             classes[c] += 1
         for c in class_data:
             class_files = set()
             for chain_arr in class_data[c].values():
                 for file, _ in chain_arr:
                     class_files.add(file)
             assert classes[c] == len(class_files)
-    assert num_files == num_files_split
+    assert num_files == num_files_split + 1
     shutil.rmtree(folder)
     print(f"generation time: {end - start} sec")
 
 
 if __name__ == "__main__":
     test_generate()
```

### Comparing `proteinflow-1.3.1/tests/test_sabdab.py` & `proteinflow-1.3.2/tests/test_sabdab.py`

 * *Files identical despite different names*

