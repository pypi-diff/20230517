# Comparing `tmp/neurondm-0.1.4.tar.gz` & `tmp/neurondm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurondm-0.1.4.tar", last modified: Fri Dec 23 06:38:46 2022, max compression
+gzip compressed data, was "neurondm-0.1.5.tar", last modified: Wed May 17 20:20:52 2023, max compression
```

## Comparing `neurondm-0.1.4.tar` & `neurondm-0.1.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.341932 neurondm-0.1.4/
--rw-r--r--   0 tom       (1000) tom       (1000)       35 2022-12-22 22:00:01.000000 neurondm-0.1.4/.coveragerc
--rw-r--r--   0 tom       (1000) tom       (1000)     1080 2022-12-22 22:00:01.000000 neurondm-0.1.4/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     4080 2022-12-23 06:38:46.341932 neurondm-0.1.4/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2885 2022-12-22 22:00:01.000000 neurondm-0.1.4/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.337932 neurondm-0.1.4/docs/
--rw-r--r--   0 tom       (1000) tom       (1000)    46880 2022-12-22 22:00:01.000000 neurondm-0.1.4/docs/NeuronLangExample.ipynb
--rw-r--r--   0 tom       (1000) tom       (1000)    11858 2022-12-22 22:00:01.000000 neurondm-0.1.4/docs/basic-model.org
--rw-r--r--   0 tom       (1000) tom       (1000)     1618 2022-12-22 22:00:01.000000 neurondm-0.1.4/docs/neurons_notebook.md
--rw-r--r--   0 tom       (1000) tom       (1000)     9180 2022-12-22 22:00:01.000000 neurondm-0.1.4/docs/types.org
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.338932 neurondm-0.1.4/neurondm/
--rw-r--r--   0 tom       (1000) tom       (1000)       69 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      199 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/auth-config.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    68421 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/build.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.339932 neurondm-0.1.4/neurondm/compiled/
--rw-r--r--   0 tom       (1000) tom       (1000)        5 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/compiled/.gitignore
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/compiled/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)   146440 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/core.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4459 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/example.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     6333 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/indicators.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3843 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/lang.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.340932 neurondm-0.1.4/neurondm/models/
--rw-r--r--   0 tom       (1000) tom       (1000)      642 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/__init__.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    15190 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/allen_cell_types.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12913 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/allen_type_specimen_mapping.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3638 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/apinat_npo.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6574 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/apinat_pops_more.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4389 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/basic_neurons.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     3001 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/bolew.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    28861 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/cuts.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    35426 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/huang2017.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    20675 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/keast2020.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     6991 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/ma2015.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1310 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/nerves.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4282 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/nlp.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4334 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/pcl.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4341 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/models/phenotype_direct.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    13633 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/phenotype_namespaces.py
--rw-r--r--   0 tom       (1000) tom       (1000)    29628 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/sheets.py
--rw-r--r--   0 tom       (1000) tom       (1000)    15634 2022-12-22 22:00:01.000000 neurondm-0.1.4/neurondm/simple.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.338932 neurondm-0.1.4/neurondm.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     4080 2022-12-23 06:38:46.000000 neurondm-0.1.4/neurondm.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1356 2022-12-23 06:38:46.000000 neurondm-0.1.4/neurondm.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2022-12-23 06:38:46.000000 neurondm-0.1.4/neurondm.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      168 2022-12-23 06:38:46.000000 neurondm-0.1.4/neurondm.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2022-12-23 06:38:46.000000 neurondm-0.1.4/neurondm.egg-info/top_level.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.340932 neurondm-0.1.4/resources/
--rw-r--r--   0 tom       (1000) tom       (1000)    94794 2022-12-23 01:57:43.000000 neurondm-0.1.4/resources/part-of-self.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    26996 2022-12-22 22:49:52.000000 neurondm-0.1.4/resources/phenotype-core.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    14907 2022-12-21 21:24:17.000000 neurondm-0.1.4/resources/phenotype-indicators.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    37194 2022-12-22 22:49:52.000000 neurondm-0.1.4/resources/phenotypes.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2022-12-23 06:38:46.341932 neurondm-0.1.4/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     4636 2022-12-23 02:00:24.000000 neurondm-0.1.4/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-12-23 06:38:46.341932 neurondm-0.1.4/test/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1191 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2300 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_integration.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2316 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_label.py
--rw-r--r--   0 tom       (1000) tom       (1000)      387 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_load.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2023 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_madness.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10400 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_neurons.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3399 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_simple.py
--rw-r--r--   0 tom       (1000) tom       (1000)      754 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_triples.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2022-12-22 22:00:01.000000 neurondm-0.1.4/test/test_write.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.186375 neurondm-0.1.5/
+-rw-r--r--   0 tom       (1000) tom       (1000)       35 2023-05-16 03:35:52.000000 neurondm-0.1.5/.coveragerc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1080 2023-05-16 03:35:52.000000 neurondm-0.1.5/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-05-17 20:20:52.186375 neurondm-0.1.5/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2885 2023-05-16 03:35:52.000000 neurondm-0.1.5/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.181375 neurondm-0.1.5/docs/
+-rw-r--r--   0 tom       (1000) tom       (1000)    46880 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/NeuronLangExample.ipynb
+-rw-r--r--   0 tom       (1000) tom       (1000)    11858 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/basic-model.org
+-rw-r--r--   0 tom       (1000) tom       (1000)     3267 2023-05-17 20:15:44.000000 neurondm-0.1.5/docs/composer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1618 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/neurons_notebook.md
+-rw-r--r--   0 tom       (1000) tom       (1000)     9180 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/types.org
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.182375 neurondm-0.1.5/neurondm/
+-rw-r--r--   0 tom       (1000) tom       (1000)       69 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      199 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/auth-config.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    68696 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/build.py
+-rw-r--r--   0 tom       (1000) tom       (1000)   150961 2023-05-17 20:15:44.000000 neurondm-0.1.5/neurondm/core.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4459 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/example.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     6333 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/indicators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3843 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/lang.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.184375 neurondm-0.1.5/neurondm/models/
+-rw-r--r--   0 tom       (1000) tom       (1000)      642 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/__init__.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    14860 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/allen_cell_types.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12913 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/allen_type_specimen_mapping.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3853 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/apinat_npo.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6540 2023-05-16 06:04:48.000000 neurondm-0.1.5/neurondm/models/apinat_pops_more.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4389 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/basic_neurons.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     3001 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/bolew.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    28861 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/cuts.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    35426 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/huang2017.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    20675 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/keast2020.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     6991 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/ma2015.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1310 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/nerves.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6704 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/nlp.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4334 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/pcl.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4341 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/phenotype_direct.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6624 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/orders.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    13633 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/phenotype_namespaces.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    29628 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/sheets.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    15634 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/simple.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.183375 neurondm-0.1.5/neurondm.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1364 2023-05-17 20:20:52.000000 neurondm-0.1.5/neurondm.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        9 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.185375 neurondm-0.1.5/resources/
+-rw-r--r--   0 tom       (1000) tom       (1000)   104921 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/part-of-self.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    26995 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/phenotype-core.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    14792 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/phenotype-indicators.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    37820 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/phenotypes.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2023-05-17 20:20:52.186375 neurondm-0.1.5/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4513 2023-05-16 06:44:23.000000 neurondm-0.1.5/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.186375 neurondm-0.1.5/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1202 2023-05-17 18:34:54.000000 neurondm-0.1.5/test/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      407 2023-05-17 18:34:54.000000 neurondm-0.1.5/test/test_0_fix_sys_modules.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2403 2023-05-16 05:56:35.000000 neurondm-0.1.5/test/test_integration.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2316 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_label.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      387 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_load.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2023 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_madness.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10400 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_neurons.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3399 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_simple.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      754 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_triples.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_write.py
```

### Comparing `neurondm-0.1.4/LICENSE` & `neurondm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/PKG-INFO` & `neurondm-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurondm
-Version: 0.1.4
+Version: 0.1.5
 Summary: A data model for neuron types.
 Home-page: https://github.com/tgbugs/pyontutils/tree/master/neurondm
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: neuron types NIF ontology neuroscience phenotype OWL rdf rdflib data model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `neurondm-0.1.4/README.md` & `neurondm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/docs/NeuronLangExample.ipynb` & `neurondm-0.1.5/docs/NeuronLangExample.ipynb`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/docs/basic-model.org` & `neurondm-0.1.5/docs/basic-model.org`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/docs/neurons_notebook.md` & `neurondm-0.1.5/docs/neurons_notebook.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/docs/types.org` & `neurondm-0.1.5/docs/types.org`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/build.py` & `neurondm-0.1.5/neurondm/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1377,14 +1377,16 @@
         )
         prefixes = oq.OntCuries._dict
         def _triples(self, terms=terms):
             yield from helper_triples()
             yield OntId('overlaps:').u, rdfs.label, rdflib.Literal('overlaps')
             yield ilx_partOf, rdfs.subPropertyOf, OntId('BFO:0000050').u
 
+            yield OntId('SAO:1224657022'), rdfs.subClassOf, OntId('BFO:0000040').u  # needed for cfde
+
             yield OntId('BFO:0000050').u, a, owl.ObjectProperty
             yield OntId('BFO:0000050').u, a, owl.TransitiveProperty
             yield OntId('BFO:0000050').u, owl.inverseOf, OntId('BFO:0000051').u
             yield OntId('BFO:0000050').u, rdfs.subPropertyOf, OntId('overlaps:').u
 
             yield OntId('BFO:0000051').u, a, owl.ObjectProperty
             yield OntId('BFO:0000051').u, a, owl.TransitiveProperty
@@ -1404,15 +1406,15 @@
             cortical_layer = OntTermOntologyOnly('UBERON:0002301')
             #yield from cortical_layer.triples_simple
             #yield from cortical_layer('hasPart:')
 
             if not terms:
                 raise BaseException('WHAT')
 
-            skip = 'TEMPIND', 'npokb'
+            skip = 'TEMPIND', 'npokb', 'mmset'
             while terms:
                 next_terms = []
                 for term in terms:
                     if term in done:
                         continue
 
                     done.append(term)
@@ -1463,15 +1465,17 @@
                             if ot.label:
                                 yield ot.u, rdfs.label, rdflib.Literal(ot.label)
                                 if hasattr(ot, '_graph'):
                                     ipo = str(ilx_partOf)
                                     for s, p, o in ot._graph.subjectGraphClosure(ot.u):
                                         yield s, p, o
                                         if str(p) == ipo and isinstance(o, rdflib.URIRef):
-                                            if (s, o) not in _ipo_done:
+                                            if s == o:
+                                                pass  # prevent partOf self from creeping in via scigraph
+                                            elif (s, o) not in _ipo_done:
                                                 _ipo_done.append((s, o))
                                                 yield from cmb.restriction(
                                                     BFO_partOf, o)(s)
 
                                                 no = OntTermOntologyOnly(o)
                                                 if no not in done:
                                                     next_terms.append(no)
```

### Comparing `neurondm-0.1.4/neurondm/core.py` & `neurondm-0.1.5/neurondm/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,15 +536,15 @@
         p = OntId(predicate).u
         for o in objects:
             o = OntId(o)  # FIXME the parent OntId sneaks in and sews madness :/
             yield s, p, o.u
 
     @property
     def triples_simple(self):
-        skips = 'pheno:parvalbumin',
+        skips = 'pheno:parvalbumin', 'owl:Thing', self.curie
         bads = ('TEMP', 'ilxtr', 'rdf', 'rdfs', 'owl', '_', 'prov', 'ILX', 'BFO1SNAP', 'NLXANAT',
                 'NLXCELL', 'NLXNEURNT', 'BFO', 'MBA', 'JAX', 'MMRRC', 'ilx', 'CARO', 'NLX',
                 'BIRNLEX', 'NIFEXT', 'obo', 'NIFRID', 'TEMPIND', 'npokb')
         s = self.URIRef
         if self.type is None:
             yield s, rdf.type, owl.Class  # FIXME ... IAO terms fail on this ... somehow
         else:
@@ -588,15 +588,16 @@
 
         predicates = 'partOf:', 'RO:0002433', 'ilx.partOf:' #'ilxtr:labelPartOf', 'ilxtr:isDelineatedBy', 'ilxtr:delineates'
         done = []
         for predicate in predicates:
             if self(predicate, asTerm=True):
                 for superpart in self.predicates[predicate]:
                     if (superpart.prefix in bads or
-                        superpart.prefix == 'FMA' and 'UBERON' in s):  # XXX FIXME hardcoded hack to work around bad sparc community terms cross hierarchy issues
+                        superpart.prefix == 'FMA' and 'UBERON' in s or  # XXX FIXME hardcoded hack to work around bad sparc community terms cross hierarchy issues
+                        superpart.curie == self.curie):  # prevent partOfSelf polution
                         continue
 
                     if (predicate, superpart) not in done:
                         yield from cmb.restriction(OntId(predicate).URIRef,
                                                    superpart.URIRef)(s)
 
                         # ensure that all superparts are closed for type and label
@@ -760,15 +761,16 @@
                 ):
 
         olr = auth.get_path('ontology-local-repo')  # we get this again because it might have changed
         if ttl_export_dir is not None:
             if not isinstance(ttl_export_dir, Path):
                 ttl_export_dir = Path(ttl_export_dir).resolve()
 
-            local_base = get_working_dir(ttl_export_dir)
+            _lbwd = get_working_dir(ttl_export_dir)
+            local_base = ttl_export_dir if _lbwd is None else _lbwd
             # FIXME there are cases where ttl_export_dir
             # and local_base will both be None???
             # reasonable failover?
         else:
             local_base = None
 
         if file is not None:
@@ -793,24 +795,28 @@
         self.__name = name  # TODO allow reload from owl to get the load graph? how to handle this
 
         graphBase.python_subclasses = list(subclasses(NeuronEBM)) + [Neuron, NeuronCUT]
         graphBase.knownClasses = [OntId(c.owlClass).u
                                   for c in graphBase.python_subclasses]
 
         imports = list(imports)
-        remote = OntId('NIFTTL:') if branch == 'master' else OntId(f'NIFRAW:{branch}/')
+        remote = OntId('NIFTTL:') if branch == 'master' else (
+            # XXX EVIL HARDCODED defaulting to dev/ by convention KILL IT WITH FIRE
+            # DO NOT CHANGE branch IN THIS CASE
+            OntId(f'NIFRAW:dev/') if branch is None else OntId(f'NIFRAW:{branch}/'))
         imports += [remote.iri + 'ttl/phenotype-core.ttl',
                     remote.iri + 'ttl/phenotypes.ttl',
                     remote.iri + 'ttl/phenotype-indicators.ttl']
         remote_path = ('' if local_base is None
                        else (ttl_export_dir
                              .resolve()
                              .relative_to(local_base.resolve())))
-        out_remote_base = os.path.join(remote.iri, remote_path)
+        out_remote_base = remote.iri.rstrip('/') + '/' + remote_path.as_posix()
         imports = [OntId(i) for i in imports]
+        imports = sorted(set(imports))
 
         remote_base = remote.iri.rsplit('/', 2)[0] if branch == 'master' else remote
 
         if local_base is None:
             local = olr / 'ttl'
             local_base = local.parent
         else:
@@ -905,15 +911,15 @@
             [_done.add(s) for s, o in graphBase.part_of_graph[:rdfs.subClassOf:]]
 
         log.debug(core_graph_paths)
 
         out_graph_path = (out_local_base / f'{name}.ttl')
 
         class lConfig(self.__class__):
-            iri = os.path.join(out_remote_base, f'{name}.ttl')
+            iri = out_remote_base.rstrip('/') + f'/{name}.ttl'
 
         self.__class__._subclasses.add(lConfig)
 
         kwargs = dict(remote_base = remote_base,  # leave it as raw for now?
                       local_base = local_base.as_posix(),
                       core_graph_paths = core_graph_paths,
                       out_graph_path = out_graph_path.as_posix(),
@@ -930,26 +936,57 @@
                       local_conventions = local_conventions)
 
         # don't klobber defaults set below
         if compiled_location is not None:
             compiled_location = Path(compiled_location).resolve()
             kwargs['compiled_location'] = compiled_location
 
-        for name, value in kwargs.items():
+        for _name, value in kwargs.items():
             # FIXME only works if we do this in __new__
             #@property
             def nochangepls(v=value):
                 return v
 
-            setattr(self, name, nochangepls)
+            setattr(self, _name, nochangepls)
             # FIXME need a way to make it clear that changing kwargs values
             # will only confuse you ...
-            #setattr(self, name, value)
+            #setattr(self, _name, value)
 
-        graphBase.configGraphIO(**kwargs)  # FIXME KILL IT WITH FIRE
+        try:
+            graphBase.configGraphIO(**kwargs)  # FIXME KILL IT WITH FIRE
+        except graphBase.GitRepoOnWrongBranch as e:
+            #breakpoint()
+            log.exception(e)
+            # XXX ALSO KILL THIS WITH FIRE
+            # XXX NOTE that since _lb will not be a git repo baring some insanity
+            # the path {:user-data-path}/neurondm/git-repo set above in configGraphIO
+            # will take precedence (UGH what a mess), _lb is forced to match the behavior above
+            # otherwise this will get out of sync an be even more confusing than they already are
+            _lb = cfg._pathit('{:user-data-path}/neurondm/git-repo')  # XXX isn't actually used
+            # this whole layer should never care about where a graph will be serialized, unfortunately
+            # the legacy codebase assumes that this layer does handle it, so we need a stopgap
+            sigh = Config(
+                 name =                 name,
+                 prefixes =             prefixes,
+                 imports =              imports,
+                 import_as_local =      import_as_local,
+                 load_from_local =      load_from_local,
+                 branch =               None,
+                 sources =              sources,
+                 source_file =          source_file,
+                 ignore_existing =      ignore_existing,
+                 py_export_dir=         py_export_dir,
+                 ttl_export_dir=        _lb,
+                 git_repo=              None,
+                 file =                 file,
+                 local_conventions =    local_conventions,
+                 import_no_net =        import_no_net,
+            )
+            self.__dict__ = sigh.__dict__
+            return
 
         graphBase.config = self  # a nice hack ... can do this for self.activate() too
         # temporary fix to persist graphs and neurons with a config
         # until I have time to rewrite Config so that multiple configs
         # can co-exist but only one config at a time can be operated on
         # when creating new neurons (since only CUTs can be modified)
         # the 'proper' way to move neurons from one config to another
@@ -988,15 +1025,15 @@
         return graphBase.part_of_graph
 
     def neurons(self):
         return sorted(self.existing_pes)  # FIXME stupidly slow
 
     def activate(self):
         """ set this config as the active config """
-        raise NotImplemented
+        raise NotImplementedError()
 
     def write(self):
         # FIXME per config prefixes using derived OntCuries?
         # FIXME code duplication with graphBase
         [n._sigh() for n in self.existing_pes]  # ugh
         og = cull_prefixes(self.out_graph, prefixes={**graphBase.prefixes, **uPREFIXES})
         og.filename = graphBase.ng.filename
@@ -1011,15 +1048,15 @@
         self.part_of_graph.write()
         log.debug(f'Neurons ttl file written to {path}')
 
     def write_python(self):
         # FIXME hack, will write other configs if call after graphbase has switched
         graphBase.write_python()
 
-    def load_existing(self):
+    def load_existing(self, load_graph=None):
         """ advanced usage allows loading multiple sets of neurons and using a config
             object to keep track of the different graphs """
         # bag existing
 
         try:
             next(iter(self.neurons()))
             raise self.ExistingNeuronsError('Existing neurons detected. Please '
@@ -1053,18 +1090,22 @@
             return sorted(classes, key=key)[:1]
 
         # bug is that I am not wiping graphBase.knownClasses and swapping it for each config
         # OR the bug is that self.load_graph is persisting, either way the call to type()
         # below seems to be the primary suspect for the issue
         if not graphBase.ignore_existing:
             ogp = Path(graphBase.ng.filename)  # FIXME ng.filename <-> out_graph_path property ...
-            if ogp.exists():
+            if ogp.exists() or load_graph is not None:
                 from itertools import chain
-                from rdflib import Graph  # FIXME
-                self.load_graph = Graph().parse(graphBase.ng.filename, format='turtle')
+                if load_graph is None:
+                    from rdflib import Graph  # FIXME
+                    self.load_graph = Graph().parse(graphBase.ng.filename, format='turtle')
+                else:
+                    self.load_graph = load_graph
+
                 graphBase.load_graph = self.load_graph
                 # FIXME memory inefficiency here ...
                 _ = [graphBase.in_graph.add(t) for t in graphBase.load_graph]  # FIXME use conjuctive ...
                 if len(graphBase.python_subclasses) == 2:  # FIXME magic number for Neuron and NeuronCUT
                     ebms = [type(OntId(s).suffix, (NeuronCUT,), dict(owlClass=s))
                             for s in self.load_graph[:rdfs.subClassOf:NeuronEBM.owlClass]
                             if not graphBase.knownClasses.append(s)]
@@ -1094,15 +1135,15 @@
         if not graphBase.ignore_existing:
             # FIXME ideally we want to be able to call self.compiled_location
             # but so long as THERE CAN BE ONLY ONE graphBase then we are going
             if self.compiled_location() != graphBase.compiled_location:
                 raise self.NotCurrentConifgError('This config is not the active config!')
             containing = graphBase.compiled_location.parent.as_posix()
             if containing not in sys.path:
-                sys.path.append(containing)
+                sys.path = [containing] + sys.path
             full_path = graphBase.compiled_location / graphBase.filename_python()
             module_path = graphBase.compiled_location.name + '.' + full_path.stem
             module = import_module(module_path)  # this returns the submod
 
             # for some reason out_graph and existing_pes do not stick to graphBase
             # correctly despite the fact that module.graphBase is graphBase -> True
             # this is a temporary hack fix, the correct fix is to have a single ConjunctiveGraph
@@ -1114,43 +1155,63 @@
             self.out_graph = graphBase.out_graph = module.config.out_graph
             self.existing_pes = NeuronBase.existing_pes = module.config.existing_pes
 
             #graphBase.existing_pes = module.config.existing_pes
             #self.load_graph = module.config.load_graph
             #graphBase.load_graph = self.load_graph
 
+
+class AcceptAllPreds:
+    def __getattr__(self, attr):
+        log.warning(f'fake predicate! {attr}')
+        return TEMP[attr]
+
+
+class AcceptAllKeys:
+    def __getitem__(self, key):
+        log.warning(f'fake super! {key}')
+        return tuple()
+
+
 # the monstrosity
 
 class graphBase:
     core_graph = 'ASSIGN ME AFTER IMPORT!'
     in_graph = 'ASSIGN ME AFTER IMPORT!'
     out_graph = 'ASSIGN ME AFTER IMPORT'
 
-    _predicates = 'ASSIGN ME AFTER IMPORT'
-
+    _predicates = AcceptAllPreds()
     LocalNames = {}
 
     _registered = False
 
     __import_name__ = __name__
 
+    # variables that cause errors if they are not present at the class level
+    # when trying to use graphBase before configGraphIO has been called (sigh)
+    config = None  # XXX ICK avoid AttributeError when no call to Config()
+    _predicate_supers = AcceptAllKeys()  # XXX also ick
+    _location_predicates = tuple()  # XXX SIGH
+    _location_predicate_supers = {}  # XXX SIGH
+    local_conventions = False  # XXX SIGH
+
     #_sgv = Vocabulary(cache=True)
 
     class owlClassMismatch(Exception):
         pass
 
     class GitRepoOnWrongBranch(Exception):
         """ Git repo is checked out to the wrong branch. """
 
     class ShouldNotHappenError(Exception):
         """ big oops """
 
     def __init__(self):
         if type(self.core_graph) == str:
-            raise TypeError('You must have at least a core_graph')
+            raise TypeError(f'You must have at least a core_graph: {self.core_graph!r}')
 
         if type(self.in_graph) == str:
             self.in_graph = self.core_graph
 
         if type(self.out_graph) == str:
             self.out_graph = self.in_graph
 
@@ -1270,15 +1331,15 @@
 
         if local_base is None:
             local_base = olr
         graphBase.local_base = Path(local_base).expanduser().resolve()
         graphBase.remote_base = remote_base
 
         def makeLocalRemote(suffixes):
-            remote = [os.path.join(graphBase.remote_base, branch, s)
+            remote = [(graphBase.remote_base.rstrip('/') + '/' + s)  # XXX WHY was branch passed here ?!??! HOW DID THIS EVER WORK !?
                       if '://' not in s else  # 'remote' is file:// or http[s]://
                       s for s in suffixes]
             # TODO the whole thing needs to be reworked to not use suffixes...
             local = [(graphBase.local_base / s).as_uri()
                      if '://' not in s else
                      ((graphBase.local_base / s.replace(graphBase.remote_base, '').strip('/')).as_uri()
                       if graphBase.remote_base in s else s)  # FIXME this breaks the semanics of local?
@@ -1329,15 +1390,15 @@
                 log.warning(f'Warning local base has been set manually you are on your own!')
                 try:
                     repo = Repo(graphBase.local_base.as_posix())
                 except (git.exc.InvalidGitRepositoryError, git.exc.NoSuchPathError) as e:
                     local_working_dir = get_working_dir(graphBase.local_base)
                     if local_working_dir is None:
                         log.exception(e)
-                        udp = cfg._pathit('{:user-data-path}/neurondm/git-repo')
+                        udp = cfg._pathit('{:user-data-path}/neurondm/git-repo')  # XXX hardcoded
                         trp = RepoPath(udp)
                         if not trp.exists():
                             trp.init()
 
                         graphBase.local_base = trp
                         # FIXME this is a stupid hack, and a reminder that the whole
                         # set up inside graphBase was a horrible mistake
@@ -1761,15 +1822,16 @@
     def getObjectProperty(self, phenotype):
         predicates = list(self.in_graph.objects(phenotype, self.expand('ilxtr:useObjectProperty')))  # useObjectProperty works for phenotypes we control
 
         if predicates:
             return predicates[0]
         else:
             # TODO check if falls in one of the expression categories
-            predicates = [_[1] for _ in self.in_graph.subject_predicates(phenotype) if _ in self._predicates.__dict__.values()]
+            predicates = [_[1] for _ in self.in_graph.subject_predicates(phenotype)
+                          if _ in self._predicates.__dict__.values()]
             mapping = {
                 'NCBITaxon':self._predicates.hasInstanceInTaxon,
                 'CHEBI':self._predicates.hasExpressionPhenotype,
                 'PR':self._predicates.hasExpressionPhenotype,
                 'NCBIGene':self._predicates.hasExpressionPhenotype,
                 'UBERON':self._predicates.hasSomaLocatedIn,
                 #'UBERON':self._predicates.hasLayerLocationPhenotype,  # a very short list is needed here
@@ -1779,22 +1841,24 @@
                 return mapping[prefix]
             return self.expand(PHENO_ROOT)
 
     def checkObjectProperty(self, ObjectProperty):  # FIXME this doesn't seem to work
         op = self.expand(ObjectProperty)
 
         if isinstance(self._predicates, str):
-            if not hasattr(cls, '_first_time'):
+            if not hasattr(self, '_first_time'):
                 log.warning('No reference predicates have been set, you are on your own!')
                 self._first_time = False
 
             return op
 
         if op in self._predicates.__dict__.values():
             return op
+        elif isinstance(self._predicates, AcceptAllPreds):
+            return op  # XXX possibly warn?
         else:
             raise TypeError(f'WARNING: Unknown ObjectProperty {op!r}')
             #t = OntTerm(ObjectProperty)  # will fail here?
             #if t.label:
                 #setattr(self._predicates, t.curie.replace(':', '_'), op)
             #else:
 
@@ -1848,15 +1912,21 @@
         if self.local_conventions:
             inj = {v:k for k, v in graphBase.LocalNames.items()}  # XXX very slow...
             if self in inj:
                 return inj[self]
 
         pn = self.in_graph.namespace_manager.qname(self.p)
         try:
-            resp = self._sgv.findById(pn)
+            if hasattr(self, '_sgv'):
+                resp = self._sgv.findById(pn)
+            else:
+                msg = ('no scigraph instance bound, graphBase.configGraphIO '
+                       'probably has not been called')
+                log.warning(msg)
+                resp = None
         except ConnectionError as e:
             #print(tc.red('WARNING:'), f'Could not set label for {pn}. No SciGraph was instance found at', self._sgv._basePath)
             log.info(f'Could not set label for {pn}. No SciGraph was instance found at ' + self._sgv._basePath)
             resp = None
 
         if pn.startswith('TEMPIND'):
             return next(self.in_graph[self.p:skos.hiddenLabel])
@@ -2111,15 +2181,15 @@
     local_names = {
         AND:'AND',
         OR:'OR',
     }
     def __init__(self, op, *edges):
         super().__init__()
         self.op = op  # TODO more with op
-        self.pes = tuple(sorted(edges))
+        self.pes = tuple(sorted(set(edges)))  # XXX SIGH must use set here
         _pesDict = {}
         for e in self.e:
             for pe in self.pes:
                 if pe.e == e:
                     if e in _pesDict:
                         _pesDict[e].add(pe)
                     else:
@@ -2725,25 +2795,29 @@
             # FIXME warn/error on ambiguous?
 
         t = OntTerm(object)
         t.set_next_repr('curie', 'label')
         raise AttributeError(f'{self} has no aspect with the phenotype {t!r}')  # FIXME AttributeError seems wrong
 
     def getObject(self, predicate):
-        for p in self.pes:
-            if p.e == predicate:  # FIXME probably need to munge the object
-                return p.p  # just to confuse you, the second p here is phenotype not predicate >_<
-
-        return rdf.nil  # FIXME how to indicate all values?
+        msg = 'deprecated, use .getObjects'
+        raise NotImplementedError(msg)
+        #return rdf.nil  # FIXME how to indicate all values?
         # predicate is different than object in the sense that it is possible
         # for neurons to have aspects (aka phenotype dimensions) without anyone
         # having measured those values, also handy when we don't know how to parse a value
         # but there is note attached
         #raise AttributeError(f'{self} has no phenotype for {predicate}')  # FIXME AttributeError seems wrong
 
+
+    def getObjects(self, predicate):
+        for p in self.pes:
+            if p.e == predicate:  # FIXME probably need to munge the object
+                yield p.p  # just to confuse you, the second p here is phenotype not predicate >_<
+
     def __expanded__(self):
         args = '(' + ', '.join([_.__expanded__() for _ in self.pes]) + ')'
         return '%s%s' % (self.__class__.__name__, args)
 
     def __repr__(self):  # TODO use local_names (since we will bind them in globals, but we do need a rule, and local names do need to be to pairs or full logicals? eg L2L3 issue
         inj = {v:k for k, v in graphBase.LocalNames.items()}  # XXX very slow...
         sn = self._shortname
@@ -2909,42 +2983,50 @@
         # PR ??
 
     def bagExisting(self):  # TODO intersections
         #if self.ng.qname(self.id_).startswith('TEMP'):
             #raise TypeError('TEMP id, no need to bag')
         out = set()  # prevent duplicates in cases where phenotypes are duplicated in the hierarchy
         embeddedKnownClasses = set()
+        def process_pe(pe):
+            if isinstance(pe, tuple):
+                for p in pe:
+                    if p in self.knownClasses:
+                        embeddedKnownClasses.add(p)
+
+                # strip out any known iris
+                out.update([_ for _ in pe if _ not in self.knownClasses])
+            else:
+                if pe in self.knownClasses:
+                    embeddedKnownClasses.add(pe)
+
+                out.add(pe)
 
         c = None
         # support CUT pattern  # FIXME maybe reimplement this method on NeuronCUT?
         for c in self.Class.subClassOf:
             if c.identifier in self.knownClasses:
                 embeddedKnownClasses.add(c.identifier)
+            else:
+                epe = self._unpackPheno(c, type_=EntailedPhenotype)
+                if epe:
+                    process_pe(epe)
+                else:
+                    log.error(f'hrm!? {epe}')
 
         for c in self.Class.equivalentClass:
             if isinstance(c.identifier, rdflib.URIRef):
                 # FIXME this is entailment stuff
                 # also prevents potential infinite recursion
                 self._equivalent_bags_ids.add(c.identifier)
                 continue
 
             pe = self._unpackPheno(c)
             if pe:
-                if isinstance(pe, tuple):
-                    for p in pe:
-                        if p in self.knownClasses:
-                            embeddedKnownClasses.add(p)
-
-                    # strip out any known iris
-                    out.update([_ for _ in pe if _ not in self.knownClasses])
-                else:
-                    if pe in self.knownClasses:
-                        embeddedKnownClasses.add(pe)
-
-                    out.add(pe)
+                process_pe(pe)
             else:
                 raise self.ShouldNotHappenError('bah!')
 
         if not embeddedKnownClasses:
             cf = [_ for _ in self.Class.graph[:rdf.type:owl.Ontology]
                   if 'phenotype' not in _]
             raise self.owlClassMismatch(f'\nowlClass {embeddedKnownClasses} '
@@ -3065,16 +3147,25 @@
                         log.warning(f'dangling reference {id_}')
                     else:
                         log.critical(str(pr))
                         raise BaseException('wat')
 
                 return tuple(pes)
             else:
-                log.critical('WHAT')  # FIXME something is wrong for negative phenotypes...
                 pr = putativeBooleanClass
+                if isinstance(pr, infixowl.Restriction):
+                    # entailed case is nearly always direct subClassOf restriction
+                    pes = []
+                    expand_restriction(pr, pes)
+                    if len(pes) > 1:
+                        log.error(f'unexpected multiple phenotypes for: {self.id_}\n{pes}')
+                    return pes[0]
+                else:
+                    log.critical(f'WHAT\n{list(c.graph.subjectGraph(c.identifier))!r}')  # FIXME something is wrong for negative phenotypes...
+
                 p = pr.someValuesFrom
                 e = pr.onProperty
                 if p and e:
                     return type_(p, e)
                 else:
                     log.critical(str(putativeBooleanClass))
         else:
@@ -3530,15 +3621,22 @@
 # to solve import issues
 """
 All work towards a common standard for neuron type naming conventions
 should be implemented here. This is only in the case where the underlying
 rules cannot be implemented in a consistent way in the ontology. The ultimate
 objective for any entry here should be to have it ultimately implemented as
 a rule plus operating from single standard ontology file. """
-Config(import_no_net=True)  # explicitly load the core graph TODO need a lighter weight way to do this
+if False:  # calling Config at top level breaks import for all normal users
+    Config(import_no_net=True)  # explicitly load the core graph TODO need a lighter weight way to do this
+else:
+    # note: this solves part of the problem, but mostly defers it until later
+    _g = OntConjunctiveGraph()
+    graphBase.core_graph = _g
+
+
 OntologyGlobalConventions = _ogc = injective_dict(
     Vertebrata = Phenotype('NCBITaxon:7742', 'ilxtr:hasInstanceInTaxon'),  # fix annoying labels
 
     L1 = Phenotype('UBERON:0005390', 'ilxtr:hasSomaLocatedInLayer'),
     L2 = Phenotype('UBERON:0005391', 'ilxtr:hasSomaLocatedInLayer'),
     L3 = Phenotype('UBERON:0005392', 'ilxtr:hasSomaLocatedInLayer'),
     L4 = Phenotype('UBERON:0005393', 'ilxtr:hasSomaLocatedInLayer'),
```

### Comparing `neurondm-0.1.4/neurondm/example.py` & `neurondm-0.1.5/neurondm/example.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/indicators.py` & `neurondm-0.1.5/neurondm/indicators.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/lang.py` & `neurondm-0.1.5/neurondm/lang.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/README.md` & `neurondm-0.1.5/neurondm/models/README.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/allen_cell_types.py` & `neurondm-0.1.5/neurondm/models/allen_cell_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,15 @@
     shortname = 'AllenCT'
 
 
 class AllenCellTypes:
 
     branch = auth.get('neurons-branch')
 
-    prefixes = {**{'JAX': 'http://jaxmice.jax.org/strain/',
-                   'MMRRC': 'http://www.mmrrc.org/catalog/getSDS.jsp?mmrrc_id=',
-                   'AllenTL': 'http://api.brain-map.org/api/v2/data/TransgenicLine/'},
-                **makePrefixes('definition', 'ilxtr', 'owl')}
-    prefixes['AllenTransgenicLine'] = 'http://api.brain-map.org/api/v2/data/TransgenicLine/'
-    prefixes['AIBSSPEC'] = str(AIBSSPEC)
+    prefixes = makePrefixes('definition', 'ilxtr', 'owl', 'AIBSTL', 'JAX', 'MMRRC', 'AIBSSPEC')
 
     def __init__(self, input, name):
         self.name = name
         self.ns = {k:rdflib.Namespace(v) for k, v in self.prefixes.items()}
         self.neuron_data = input
         self.tag_names = set()
         # self.sample_neuron()
@@ -149,15 +144,15 @@
                 pred = 'ilxtr:hasReporterExpressionPhenotype'
             else:
                 pred = 'ilxtr:hasExpressionPhenotype'
 
             line_names = []
             if prefix and suffix and prefix in ['AIBS', 'MMRRC', 'JAX']:
                 if prefix == 'AIBS':
-                    prefix = 'AllenTL'
+                    prefix = 'AIBSTL'
                 iri = self.ns[prefix][suffix]
                 phenotypes.append(Phenotype(iri, pred))
         return phenotypes
 
     # TODO: search if description exists
     # TODO: Create mapping for all possible types
     # TODO: Fork negatives to NegPhenotype
@@ -311,15 +306,15 @@
                 if line_type == 'driver' and 'CreERT2' in tl['name']:
                     line_type = 'inducibleDriver'
 
                 if prefix not in ['JAX', 'MMRRC', 'AIBS']:
                     print(tc.red('WARNING:'), 'unknown prefix', prefix, json.dumps(tl, indent=4))
                     continue
                 elif prefix == 'AIBS':
-                    prefix = 'AllenTL'
+                    prefix = 'AIBSTL'
 
                 _class = self.ns[prefix][str(_id)]
                 triples.append((_class, rdf.type, owl.Class))
                 triples.append((_class, rdfs.label, rdflib.Literal(tl['name'])))
                 triples.append((_class, definition, rdflib.Literal(tl['description'])))
                 triples.append((_class, rdfs.subClassOf, ilxtr.transgenicLine))
                 triples.append((_class, ilxtr.hasTransgenicType, ilxtr[line_type + 'Line']))
```

### Comparing `neurondm-0.1.4/neurondm/models/allen_type_specimen_mapping.py` & `neurondm-0.1.5/neurondm/models/allen_type_specimen_mapping.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/apinat_npo.py` & `neurondm-0.1.5/neurondm/models/apinat_npo.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         'Dendrite-Location': ilxtr.hasDendriteLocatedIn,
         #'Dendrite-Terminal-Location': ilxtr.hasDendriteSensorySubcellularElementIn,
         'Forward-Connection': ilxtr.hasForwardConnectionPhenotype,
         'Axon-Sensory-Location': ilxtr.hasAxonSensorySubcellularElementIn,
         'Equivalent-To': owl.equivalentClass,
         'Functional-Circuit-Role': ilxtr.hasFunctionalCircuitRolePhenotype,
         'entail:hasInstanceInTaxon': ilxtr.hasInstanceInTaxon,
+        'Organ-Destination': ilxtr.hasOrganTarget,
+        'Has-Phenotype': ilxtr.hasPhenotype,  # needed for aacar 7 and 8
+        'Projection-Phenotype': ilxtr.hasProjectionPhenotype,
     }[sheet_pred]
     return p
 
 
 def main():
     cs = [c() for c in sheet_classes]
     trips = [[cl] + [c.value for c in
@@ -68,15 +71,15 @@
         try:
             p = map_predicates(_p)
         except KeyError as e:
             log.error(f'sigh {s}')
             raise e
         o = OntId(_o)
 
-        if p == owl.equivalentClass:
+        if p == owl.equivalentClass or p == ilxtr.hasOrganTarget:
             to_add.append((s.u, p, o.u))
             continue
 
         try:
             if _p.startswith('entail:'):  # XXX FIXME hack
                 dd[s].append(EntailedPhenotype(o, p))
             else:
```

### Comparing `neurondm-0.1.4/neurondm/models/apinat_pops_more.py` & `neurondm-0.1.5/neurondm/models/apinat_pops_more.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,18 +157,17 @@
 #sys.modules['__main__'].__file__ = __file__
 #import linecache
 #linecache.cache[__file__] = size, mtime, lines, fullname
 config.write()
 config.write_python()
 
 # cleanup
-repo_relative_path = 'ttl/generated/neurons/apinat-pops-more.ttl'
-olr = aug.LocalPath(auth.get('ontology-local-repo')).expanduser()
-og = OntGraph(path=olr / repo_relative_path)
+ogp = config._written_graph.path  # XXX cannot trust config.out_graph_path() due to failover if path does not exist in graphBase >_< hooray
+og = OntGraph(path=ogp)
 og.parse()
 ng = OntGraph().populate_from_triples((t for t in og if 'able' not in t[1] and 'abel' not in t[1]))
 ng.namespace_manager.populate_from(og)
-ng.write(olr / repo_relative_path)
+ng.write(ogp)
 
 if False:
     pprint([(a, b, c, d) for a, b, c, d in bagged if not a])
     pprint([(d, b, c) for a, b, c, d in bagged if d])
```

### Comparing `neurondm-0.1.4/neurondm/models/basic_neurons.py` & `neurondm-0.1.5/neurondm/models/basic_neurons.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/bolew.py` & `neurondm-0.1.5/neurondm/models/bolew.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/cuts.py` & `neurondm-0.1.5/neurondm/models/cuts.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/huang2017.py` & `neurondm-0.1.5/neurondm/models/huang2017.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/keast2020.py` & `neurondm-0.1.5/neurondm/models/keast2020.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/ma2015.py` & `neurondm-0.1.5/neurondm/models/ma2015.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/nerves.py` & `neurondm-0.1.5/neurondm/models/nerves.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/nlp.py` & `neurondm-0.1.5/neurondm/models/nlp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,87 @@
 import re
 from collections import defaultdict
 import rdflib
 from pyontutils.sheets import Sheet
 from pyontutils.namespaces import ilxtr, TEMP, rdfs, skos, owl, interlex_namespace
-from neurondm.core import Config, NeuronEBM, Phenotype, log, OntId
+from neurondm.core import Config, NeuronEBM, Phenotype, NegPhenotype, log, OntId
+from neurondm import orders
+
+orders.to_rdf = orders.bind_rdflib()
 
 
 class NeuronSparcNlp(NeuronEBM):
     owlClass = ilxtr.NeuronSparcNlp
     shortname = 'sprcnlp'
 
 
 class NLP1(Sheet):
-    name = 'off-nlp'
+    name = 'off-nlp-1'
+
+
+class NLP2(Sheet):
+    name = 'off-nlp-2'
 
 
 def nlp_ns(name):
     return rdflib.Namespace(interlex_namespace(f'tgbugs/uris/readable/sparc-nlp/{name}/'))
 
 
 snames = {
-    'MM Set 1': nlp_ns('mmset1'),
-    'MM Set 2 Cranial Nerves': nlp_ns('mmset2cn'),
+    'MM Set 1': (NLP1, nlp_ns('mmset1')),
+    'MM Set 2 Cranial Nerves': (NLP1, nlp_ns('mmset2cn')),
+    'MM Set 4': (NLP2, nlp_ns('mmset4')),
 }
 
 
 sheet_classes = [
-    type(f'NLP1{sname.replace(" ", "_")}',
-         (NLP1,), dict(sheet_name=sname))
-    for sname in snames]
+    type(f'{base.__name__}{sname.replace(" ", "_")}',
+         (base,), dict(sheet_name=sname))
+    for sname, (base, ns) in snames.items()]
 
 
 def map_predicates(sheet_pred):
     p = {
         '': TEMP.BROKEN_EMPTY,
         'Soma': ilxtr.hasSomaLocatedIn,
         'Axon terminal': ilxtr.hasAxonPresynapticElementIn,
         'Axon': ilxtr.hasAxonLocatedIn,
         'Dendrite': ilxtr.hasDendriteLocatedIn,
         'Axon sensory terminal': ilxtr.hasAxonSensorySubcellularElementIn,
         'hasInstanceInTaxon': ilxtr.hasInstanceInTaxon,
         'hasPhenotype': ilxtr.hasPhenotype,
+        'hasBiologicalSex': ilxtr.hasBiologicalSex,
         'hasCircuitRolePhenotype': ilxtr.hasCircuitRolePhenotype,
+        'hasForwardConnectionPhenotype': ilxtr.hasForwardConnectionPhenotype,  # FIXME this needs to be unionOf
     }[sheet_pred]
     return p
 
 
+def ind_to_adj(ind_uri):
+    inds = sorted(set([i for i, u in ind_uri]))
+    edges = []
+    for a, b in zip(inds[:-1], inds[1:]):
+        for i, iu in ind_uri:
+            # XXX yes this is a horribly inefficient way to do this
+            # index them in a dict if it becomes an issue
+            if i == a:
+                for j, ju in ind_uri:
+                    if j == b:
+                        edge =  iu, ju
+                        edges.append(edge)
+
+    return edges
+
+
+def add_partial_orders(graph, nested):
+    for s, nst in nested.items():
+        bn = orders.to_rdf(graph, nst)
+        graph.add((s, ilxtr.neuronPartialOrder, bn))
+
+
 def main():
     cs = [c() for c in sheet_classes]
     trips = [[cl] + [c.value for c in
                      (r.id(), r.relationship(), r.identifier())]
              for cl in cs for r in cl.rows()
              if r.row_index > 0 and r.id().value
              #and (not hasattr(r, 'exclude') or not r.exclude().value)
@@ -64,79 +96,107 @@
     def asdf(s, p, rm):
         v = vl(rm)
         if v:
             # XXX watch out for non-homogenous subject types
             # (e.g. OntId vs rdflib.URIRef)
             to_add.append((s.u, p, v))
 
+    dd = defaultdict(list)
+    ec = {}
     for cl in cs:
-        nlpns = snames[cl.sheet_name]
+        _, nlpns = snames[cl.sheet_name]
         for r in cl.rows():
             if (r.row_index > 0 and
                 r.id().value and
                 r.proposed_action().value != "Don't add"):
                 # extra trips
                 #print(repr(r.id()))
                 s = OntId(nlpns[r.id().value])
                 #print(s)
                 asdf(s, ilxtr.sentenceNumber, r.sentence_number)
                 asdf(s, ilxtr.curatorNote, r.different_from_existing)
                 asdf(s, ilxtr.curatorNote, r.curation_notes)
                 asdf(s, ilxtr.reviewNote, r.review_notes)
                 asdf(s, ilxtr.reference, r.reference_pubmed_id__doi_or_text)
                 asdf(s, rdfs.label, r.neuron_population_label_a_to_b_via_c)
+                if hasattr(r, 'alert_explanation'):
+                    asdf(s, ilxtr.alertNote, r.alert_explanation)
+
+                if hasattr(r, 'explicit_complement') and r.explicit_complement().value:
+                    p = map_predicates(r.relationship().value)
+                    o = OntId(r.explicit_complement().value)
+                    ec[(s, p)] = o
+                if hasattr(r, 'axonal_course_poset') and r.axonal_course_poset().value:
+                    # s.u and OntId(...).u to avoid duplicate subjects/objects in the graph
+                    # due to type vs instance issues for rdflib.URIRef and OntId
+                    dd[s.u].append((int(r.axonal_course_poset().value), OntId(r.identifier().value).u))
+
+    sorders = {k:sorted(v) for k, v in dd.items()}
+    sadj = {k:ind_to_adj(v) for k, v in sorders.items()}
+    snst = {k:orders.adj_to_nst(v) for k, v in sadj.items()}
 
     dd = defaultdict(list)
     for c, _s, _p, _o in trips:
-        nlpns = snames[c.sheet_name]
+        _, nlpns = snames[c.sheet_name]
         for x in (_s, _p, _o):
             if re.match(r'(^[\s]+[^\s].*|.*[^\s][\s]+$)', x):
                 msg = f'leading/trailing whitespace in {c} {_s!r} {_p!r} {_o!r}'
                 log.error(msg)
                 raise ValueError(msg)
 
         s = OntId(nlpns[_s])
         try:
             p = map_predicates(_p)
         except KeyError as e:
             log.error(f'sigh {s}')
             raise e
+
+        if p == ilxtr.hasForwardConnectionPhenotype:
+            _o = nlpns[_o]
+
         o = OntId(_o)
 
         if p == owl.equivalentClass:
             to_add.append((s.u, p, o.u))
             continue
 
         try:
             dd[s].append(Phenotype(o, p))
         except TypeError as e:
             log.error(f'bad data for {c} {s} {p} {o}')
             raise e
 
+        if ec and (s, p) in ec:
+            dd[s].append(NegPhenotype(ec[(s, p)], p))
+
 
     config = Config('sparc-nlp')
 
     sigh = []
     nrns = []
     for id, phenos in dd.items():
         n = NeuronSparcNlp(*phenos, id_=id)
         if False and eff(n):
             n._sigh()  # XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX FIXME figure out why this is not getting called internally
             sigh.append(n)
 
         nrns.append(n)
 
+    Phenotype.in_graph.bind('mmset4', snames['MM Set 4'][-1])  # XXX FIXME UGH
     config.write()
     labels = (
         #ilxtr.genLabel,
         ilxtr.localLabel, ilxtr.simpleLabel,
         ilxtr.simpleLocalLabel, rdfs.label, skos.prefLabel)
     to_remove = [t for t in config._written_graph if t[1] in labels]
     [config._written_graph.remove(t) for t in to_remove]
     [config._written_graph.add(t) for t in to_add]
+    add_partial_orders(config._written_graph, snst)
+    # uncomment to debug type vs instance issues
+    #sigh = sorted(set(s for s in config._written_graph.subjects() if isinstance(s, rdflib.URIRef)))
     config._written_graph.write()
     config.write_python()
     return config,
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `neurondm-0.1.4/neurondm/models/pcl.py` & `neurondm-0.1.5/neurondm/models/pcl.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/models/phenotype_direct.py` & `neurondm-0.1.5/neurondm/models/phenotype_direct.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/phenotype_namespaces.py` & `neurondm-0.1.5/neurondm/phenotype_namespaces.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/sheets.py` & `neurondm-0.1.5/neurondm/sheets.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm/simple.py` & `neurondm-0.1.5/neurondm/simple.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/neurondm.egg-info/PKG-INFO` & `neurondm-0.1.5/neurondm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurondm
-Version: 0.1.4
+Version: 0.1.5
 Summary: A data model for neuron types.
 Home-page: https://github.com/tgbugs/pyontutils/tree/master/neurondm
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: neuron types NIF ontology neuroscience phenotype OWL rdf rdflib data model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `neurondm-0.1.4/neurondm.egg-info/SOURCES.txt` & `neurondm-0.1.5/neurondm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 .coveragerc
 LICENSE
 README.md
 setup.cfg
 setup.py
 docs/NeuronLangExample.ipynb
 docs/basic-model.org
+docs/composer.py
 docs/neurons_notebook.md
 docs/types.org
 neurondm/__init__.py
 neurondm/auth-config.py
 neurondm/build.py
 neurondm/core.py
 neurondm/example.py
 neurondm/indicators.py
 neurondm/lang.py
+neurondm/orders.py
 neurondm/phenotype_namespaces.py
 neurondm/sheets.py
 neurondm/simple.py
 neurondm.egg-info/PKG-INFO
 neurondm.egg-info/SOURCES.txt
 neurondm.egg-info/dependency_links.txt
 neurondm.egg-info/requires.txt
 neurondm.egg-info/top_level.txt
-neurondm/compiled/.gitignore
-neurondm/compiled/__init__.py
 neurondm/models/README.md
 neurondm/models/__init__.py
 neurondm/models/allen_cell_types.py
 neurondm/models/allen_type_specimen_mapping.py
 neurondm/models/apinat_npo.py
 neurondm/models/apinat_pops_more.py
 neurondm/models/basic_neurons.py
@@ -42,14 +42,15 @@
 neurondm/models/phenotype_direct.py
 resources/part-of-self.ttl
 resources/phenotype-core.ttl
 resources/phenotype-indicators.ttl
 resources/phenotypes.ttl
 test/__init__.py
 test/common.py
+test/test_0_fix_sys_modules.py
 test/test_integration.py
 test/test_label.py
 test/test_load.py
 test/test_madness.py
 test/test_neurons.py
 test/test_simple.py
 test/test_triples.py
```

### Comparing `neurondm-0.1.4/resources/part-of-self.ttl` & `neurondm-0.1.5/resources/part-of-self.ttl`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0738432 ] .
 
 ILX:0738433 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0738433 ] .
 
+ILX:0738444 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0738444 ] .
+
 ILX:0739295 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0739295 ] .
 
 ILX:0739296 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0739296 ] .
@@ -165,14 +169,22 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0739297 ] .
 
 ILX:0739299 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0739299 ] .
 
+ILX:0739303 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0739303 ] .
+
+ILX:0739304 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0739304 ] .
+
 ILX:0770759 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0770759 ] .
 
 ILX:0771089 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0771089 ] .
@@ -381,14 +393,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0790472 ] .
 
 ILX:0790482 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0790482 ] .
 
+ILX:0790497 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0790497 ] .
+
 ILX:0791062 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0791062 ] .
 
 ILX:0791105 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0791105 ] .
@@ -453,14 +469,22 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793221 ] .
 
 ILX:0793228 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793228 ] .
 
+ILX:0793335 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793335 ] .
+
+ILX:0793336 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793336 ] .
+
 ILX:0793357 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793357 ] .
 
 ILX:0793359 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793359 ] .
@@ -529,14 +553,30 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793613 ] .
 
 ILX:0793615 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793615 ] .
 
+ILX:0793617 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793617 ] .
+
+ILX:0793618 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793618 ] .
+
+ILX:0793619 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793619 ] .
+
+ILX:0793621 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793621 ] .
+
 ILX:0793626 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793626 ] .
 
 ILX:0793632 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793632 ] .
@@ -625,14 +665,178 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793680 ] .
 
 ILX:0793681 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom ILX:0793681 ] .
 
+ILX:0793697 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793697 ] .
+
+ILX:0793698 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793698 ] .
+
+ILX:0793699 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793699 ] .
+
+ILX:0793700 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793700 ] .
+
+ILX:0793701 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793701 ] .
+
+ILX:0793702 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793702 ] .
+
+ILX:0793711 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793711 ] .
+
+ILX:0793712 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793712 ] .
+
+ILX:0793713 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793713 ] .
+
+ILX:0793714 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793714 ] .
+
+ILX:0793722 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793722 ] .
+
+ILX:0793723 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793723 ] .
+
+ILX:0793735 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793735 ] .
+
+ILX:0793737 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793737 ] .
+
+ILX:0793738 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793738 ] .
+
+ILX:0793739 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793739 ] .
+
+ILX:0793800 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793800 ] .
+
+ILX:0793801 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793801 ] .
+
+ILX:0793802 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793802 ] .
+
+ILX:0793803 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793803 ] .
+
+ILX:0793804 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793804 ] .
+
+ILX:0793805 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793805 ] .
+
+ILX:0793806 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793806 ] .
+
+ILX:0793807 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793807 ] .
+
+ILX:0793808 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793808 ] .
+
+ILX:0793809 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793809 ] .
+
+ILX:0793811 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793811 ] .
+
+ILX:0793812 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793812 ] .
+
+ILX:0793813 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793813 ] .
+
+ILX:0793814 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793814 ] .
+
+ILX:0793815 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793815 ] .
+
+ILX:0793816 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793816 ] .
+
+ILX:0793817 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793817 ] .
+
+ILX:0793818 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793818 ] .
+
+ILX:0793819 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793819 ] .
+
+ILX:0793821 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793821 ] .
+
+ILX:0793822 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793822 ] .
+
+ILX:0793823 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793823 ] .
+
+ILX:0793832 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793832 ] .
+
+ILX:0793833 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793833 ] .
+
+ILX:0793834 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom ILX:0793834 ] .
+
 MBA:33 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom MBA:33 ] .
 
 MBA:41 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom MBA:41 ] .
@@ -1009,14 +1213,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000966 ] .
 
 UBERON:0000988 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0000988 ] .
 
+UBERON:0000992 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0000992 ] .
+
 UBERON:0001043 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001043 ] .
 
 UBERON:0001051 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001051 ] .
@@ -1125,14 +1333,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001607 ] .
 
 UBERON:0001629 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001629 ] .
 
+UBERON:0001643 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0001643 ] .
+
 UBERON:0001647 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001647 ] .
 
 UBERON:0001649 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001649 ] .
@@ -1173,14 +1385,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001737 ] .
 
 UBERON:0001759 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001759 ] .
 
+UBERON:0001780 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0001780 ] .
+
 UBERON:0001787 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001787 ] .
 
 UBERON:0001789 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001789 ] .
@@ -1205,14 +1421,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001817 ] .
 
 UBERON:0001818 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001818 ] .
 
+UBERON:0001826 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0001826 ] .
+
 UBERON:0001831 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001831 ] .
 
 UBERON:0001832 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0001832 ] .
@@ -1389,14 +1609,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002009 ] .
 
 UBERON:0002012 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002012 ] .
 
+UBERON:0002014 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0002014 ] .
+
 UBERON:0002019 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002019 ] .
 
 UBERON:0002022 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002022 ] .
@@ -1621,14 +1845,22 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002318 ] .
 
 UBERON:0002348 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002348 ] .
 
+UBERON:0002366 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0002366 ] .
+
+UBERON:0002370 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0002370 ] .
+
 UBERON:0002380 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002380 ] .
 
 UBERON:0002421 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002421 ] .
@@ -1645,14 +1877,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002436 ] .
 
 UBERON:0002440 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002440 ] .
 
+UBERON:0002441 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0002441 ] .
+
 UBERON:0002476 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002476 ] .
 
 UBERON:0002477 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0002477 ] .
@@ -1945,14 +2181,22 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0003715 ] .
 
 UBERON:0003716 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0003716 ] .
 
+UBERON:0003721 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0003721 ] .
+
+UBERON:0003729 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0003729 ] .
+
 UBERON:0003881 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0003881 ] .
 
 UBERON:0003882 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0003882 ] .
@@ -1997,18 +2241,26 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004679 ] .
 
 UBERON:0004681 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004681 ] .
 
+UBERON:0004713 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0004713 ] .
+
 UBERON:0004789 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004789 ] .
 
+UBERON:0004917 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0004917 ] .
+
 UBERON:0004982 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0004982 ] .
 
 UBERON:0005024 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0005024 ] .
@@ -2217,14 +2469,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006493 ] .
 
 UBERON:0006562 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006562 ] .
 
+UBERON:0006608 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0006608 ] .
+
 UBERON:0006718 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006718 ] .
 
 UBERON:0006719 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0006719 ] .
@@ -2317,14 +2573,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0008712 ] .
 
 UBERON:0008804 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0008804 ] .
 
+UBERON:0008810 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0008810 ] .
+
 UBERON:0008857 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0008857 ] .
 
 UBERON:0008862 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0008862 ] .
@@ -2417,22 +2677,34 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0010947 ] .
 
 UBERON:0010952 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0010952 ] .
 
+UBERON:0011096 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0011096 ] .
+
 UBERON:0011173 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0011173 ] .
 
 UBERON:0011176 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0011176 ] .
 
+UBERON:0011183 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0011183 ] .
+
+UBERON:0011194 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0011194 ] .
+
 UBERON:0011315 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0011315 ] .
 
 UBERON:0011316 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0011316 ] .
@@ -2605,30 +2877,50 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0016508 ] .
 
 UBERON:0016848 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0016848 ] .
 
+UBERON:0018412 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0018412 ] .
+
 UBERON:0018675 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0018675 ] .
 
 UBERON:0018680 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0018680 ] .
 
+UBERON:0018681 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0018681 ] .
+
 UBERON:0018683 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0018683 ] .
 
 UBERON:0020358 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0020358 ] .
 
+UBERON:0022278 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0022278 ] .
+
+UBERON:0022301 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0022301 ] .
+
+UBERON:0022302 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0022302 ] .
+
 UBERON:0022317 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0022317 ] .
 
 UBERON:0022318 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0022318 ] .
@@ -2713,14 +3005,18 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035642 ] .
 
 UBERON:0035647 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035647 ] .
 
+UBERON:0035772 rdfs:subClassOf [ a owl:Restriction ;
+            owl:onProperty partOf: ;
+            owl:someValuesFrom UBERON:0035772 ] .
+
 UBERON:0035971 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035971 ] .
 
 UBERON:0035973 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0035973 ] .
@@ -2729,8 +3025,8 @@
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0036216 ] .
 
 UBERON:0038727 rdfs:subClassOf [ a owl:Restriction ;
             owl:onProperty partOf: ;
             owl:someValuesFrom UBERON:0038727 ] .
 
-### Serialized using the ttlser deterministic serializer v1.2.0
+### Serialized using the ttlser deterministic serializer v1.2.1
```

### Comparing `neurondm-0.1.4/resources/phenotype-core.ttl` & `neurondm-0.1.5/resources/phenotype-core.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -442,8 +442,8 @@
     rdfs:label "Phenotype" ;
     skos:definition "A Phenotype is a binary property of a biological entity. Phenotypes are derived from measurements made on the subject of interest. While Phenotype is not currently placed within the BFO hierarchy, if we were to place it, it would fall under BFO:0000016 -> disposition, since these phenotypes are contingent on the experimental conditions under which measurements were made and are NOT qualities. For consideration: in theory this would mean that disjointness does not make sense, even for things that would seem to be obviously disjoint such as Accommodating and Non-Accommodating. However, this information can still be captured on a subject by subject basis by asserting that for this particular entity, coocurrance of phenotypes is not possible. This still leaves the question of whether the class of biological entities that correspond to the bag of phenotypes is implicitly bounded/limited only to the extrinsic and unspecified experimental conditions, some of which are not and cannot be included in a bag of phenotypes. The way to deal with this when we want to include 2 'same time' disjoint phenotypes, is to use a logical phenotype to wrap them with an auxiliary variable that we think accounts for the difference." .
 
 ### Annotations
 
 ilxtr:delineates owl:inverseOf ilxtr:isDelineatedBy .
 
-### Serialized using the ttlser deterministic serializer v1.2.0
+### Serialized using the ttlser deterministic serializer v1.2.1
```

### Comparing `neurondm-0.1.4/resources/phenotype-indicators.ttl` & `neurondm-0.1.5/resources/phenotype-indicators.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 @prefix : <file:///ERROR/EMPTY/PREFIX/BANNED/> .
-@prefix AllenTransgenicLine: <http://api.brain-map.org/api/v2/data/TransgenicLine/> .
+@prefix AIBSTL: <http://api.brain-map.org/api/v2/data/TransgenicLine/> .
 @prefix CHEBI: <http://purl.obolibrary.org/obo/CHEBI_> .
 @prefix ilxtr: <http://uri.interlex.org/tgbugs/uris/readable/> .
 @prefix JAX: <http://jaxmice.jax.org/strain/> .
 @prefix MMRRC: <http://www.mmrrc.org/catalog/getSDS.jsp?mmrrc_id=> .
 @prefix NCBIGene: <http://www.ncbi.nlm.nih.gov/gene/> .
 @prefix NIFEXT: <http://uri.neuinfo.org/nif/nifstd/nifext_> .
 @prefix NIFRID: <http://uri.neuinfo.org/nif/nifstd/readable/> .
@@ -14,15 +14,15 @@
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix SAO: <http://uri.neuinfo.org/nif/nifstd/sao> .
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix TEMPIND: <http://uri.interlex.org/temp/uris/phenotype-indicators/> .
 
 <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/neurons/ttl/phenotype-indicators.ttl> a owl:Ontology ;
     rdfs:label "Phenotype indicators" ;
-    owl:versionInfo "2022-07-18" .
+    owl:versionInfo "2023-04-27" .
 
 ### Classes
 
 ilxtr:PhenotypeIndicator a owl:Class ;
     rdfs:label "phenotype indicator" .
 
 TEMPIND:ACh a owl:Class ;
@@ -283,36 +283,30 @@
     rdfs:label "Vipr2 (indicator)" ;
     NIFRID:synonym "vasoactive intestinal peptide receptor 2" ;
     rdfs:subClassOf ilxtr:PhenotypeIndicator ;
     skos:hiddenLabel "Vipr2" .
 
 ### Annotations
 
-AllenTransgenicLine:301021674 rdfs:subClassOf TEMPIND:Oxtr .
+AIBSTL:301021674 rdfs:subClassOf TEMPIND:Oxtr .
 
-AllenTransgenicLine:543338518 rdfs:subClassOf TEMPIND:Vipr2 .
+AIBSTL:543338518 rdfs:subClassOf TEMPIND:Vipr2 .
 
 CHEBI:9937 rdfs:subClassOf TEMPIND:Avp .
 
 CHEBI:15355 rdfs:subClassOf TEMPIND:ACh .
 
 CHEBI:16015 rdfs:subClassOf TEMPIND:Glutamate .
 
 CHEBI:16865 rdfs:subClassOf TEMPIND:GABA .
 
 CHEBI:28790 rdfs:subClassOf TEMPIND:Serotonin .
 
 CHEBI:64628 rdfs:subClassOf TEMPIND:Sst .
 
-<http://www.jax.org/strain/007914> rdfs:subClassOf TEMPIND:CreDependentProteinFluorescingInSpectrumRed .
-
-<http://www.jax.org/strain/021875> rdfs:subClassOf TEMPIND:CreFlpDependentProteinFluorescingInSpectrumRed .
-
-<https://www.ncbi.nlm.nih.gov/gene/11998> rdfs:subClassOf TEMPIND:Avp .
-
 ilxtr:CCK-cre rdfs:subClassOf TEMPIND:Cck .
 
 ilxtr:GABAReceptor rdfs:subClassOf TEMPIND:GABAR .
 
 ilxtr:glutamateReceptor rdfs:subClassOf TEMPIND:GluR .
 
 ilxtr:NOS1-creER rdfs:subClassOf TEMPIND:Nos1 .
@@ -323,14 +317,16 @@
 
 ilxtr:SST-flp rdfs:subClassOf TEMPIND:Sst .
 
 ilxtr:VIP-flp rdfs:subClassOf TEMPIND:VIP .
 
 JAX:006410 rdfs:subClassOf TEMPIND:ACh .
 
+JAX:007914 rdfs:subClassOf TEMPIND:CreDependentProteinFluorescingInSpectrumRed .
+
 JAX:008069 rdfs:subClassOf TEMPIND:Pvalb .
 
 JAX:010802 rdfs:subClassOf TEMPIND:GABA .
 
 JAX:010908 rdfs:subClassOf TEMPIND:VIP .
 
 JAX:012706 rdfs:subClassOf TEMPIND:Cck .
@@ -343,28 +339,32 @@
 
 JAX:017320 rdfs:subClassOf TEMPIND:Pvalb .
 
 JAX:021189 rdfs:subClassOf TEMPIND:Pvalb .
 
 JAX:021190 rdfs:subClassOf TEMPIND:Pvalb .
 
+JAX:021875 rdfs:subClassOf TEMPIND:CreFlpDependentProteinFluorescingInSpectrumRed .
+
 JAX:022730 rdfs:subClassOf TEMPIND:Pvalb .
 
 JAX:025112 rdfs:subClassOf TEMPIND:Penk .
 
 JAX:028578 rdfs:subClassOf TEMPIND:VIP .
 
 JAX:028579 rdfs:subClassOf TEMPIND:Sst .
 
 JAX:029591 rdfs:subClassOf TEMPIND:GABA .
 
 MMRRC:036680 rdfs:subClassOf TEMPIND:Htr3a .
 
 NCBIGene:11535 rdfs:subClassOf TEMPIND:Adm .
 
+NCBIGene:11998 rdfs:subClassOf TEMPIND:Avp .
+
 NCBIGene:12307 rdfs:subClassOf TEMPIND:Calb .
 
 NCBIGene:12308 rdfs:subClassOf TEMPIND:Calb2 .
 
 NCBIGene:12310 rdfs:subClassOf TEMPIND:Calca .
 
 NCBIGene:12424 rdfs:subClassOf TEMPIND:Cck .
@@ -523,8 +523,8 @@
 
 SAO:711465902 rdfs:subClassOf TEMPIND:Serotonin .
 
 SAO:722953401 rdfs:subClassOf TEMPIND:ACh .
 
 SAO:1744435799 rdfs:subClassOf TEMPIND:Glutamate .
 
-### Serialized using the ttlser deterministic serializer v1.2.0
+### Serialized using the ttlser deterministic serializer v1.2.1
```

### Comparing `neurondm-0.1.4/resources/phenotypes.ttl` & `neurondm-0.1.5/resources/phenotypes.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 
 ilxtr:ANSPopulationPhenotype a owl:Class ;
     rdfs:label "Autonomic nervous system population phenotype" ;
     rdfs:subClassOf ilxtr:CellPhenotype ;
     rdfs:comment "used to account for populations that are part of distinct autonomic nervous system subdivisions" ;
     skos:hiddenLabel "Autonomic nervous system population" .
 
+ilxtr:AnteriorProjecting a owl:Class ;
+    rdfs:label "Anterior projecting" ;
+    rdfs:subClassOf ilxtr:ProjectionPhenotype ;
+    rdfs:comment "projects in the anterior direction of the housing structure" ;
+    ilxtr:useObjectProperty ilxtr:hasProjectionPhenotype ;
+    skos:hiddenLabel "Anterior projecting" .
+
 ilxtr:ApicalDendritePhenotype a owl:Class ;
     rdfs:label "Apical dendrite phenotype" ;
     rdfs:subClassOf ilxtr:DendritePhenotype ;
     rdfs:comment "When used directly indicates the presence or absense of an apical dendrite. Rather than subclassing directly, could be combined with general dendrite phenotypes to allow specificity." ;
     ilxtr:useObjectProperty ilxtr:hasDendriteMorphologicalPhenotype ;
     skos:hiddenLabel "Apical dendrite" .
 
@@ -650,14 +657,21 @@
 ilxtr:PetillaSustainedStutteringPhenotype a owl:Class ;
     rdfs:label "Petilla sustained stuttering phenotype" ;
     NIFRID:synonym "petilla stut" ;
     rdfs:subClassOf ilxtr:PetillaSustainedSpikingPhenotype ;
     ilxtr:useObjectProperty ilxtr:hasElectrophysiologicalPhenotype ;
     skos:hiddenLabel "Petilla sustained stuttering" .
 
+ilxtr:PosteriorProjecting a owl:Class ;
+    rdfs:label "Posterior projecting" ;
+    rdfs:subClassOf ilxtr:ProjectionPhenotype ;
+    rdfs:comment "projects in the posterior direction of the housing structure" ;
+    ilxtr:useObjectProperty ilxtr:hasProjectionPhenotype ;
+    skos:hiddenLabel "Posterior projecting" .
+
 ilxtr:PostGanglionicPhenotype a owl:Class ;
     rdfs:label "Post ganglionic phenotype" ;
     rdfs:subClassOf ilxtr:ANSPopulationPhenotype ;
     owl:disjointWith ilxtr:PreGanglionicPhenotype ;
     skos:hiddenLabel "Post ganglionic" .
 
 ilxtr:PreGanglionicPhenotype a owl:Class ;
@@ -772,22 +786,22 @@
     rdfs:label "Spiking phenotype" ;
     rdfs:subClassOf ilxtr:ElectrophysiologicalPhenotype ;
     ilxtr:useObjectProperty ilxtr:hasElectrophysiologicalPhenotype ;
     skos:hiddenLabel "Spiking" .
 
 ilxtr:SpinalCordAscendingProjectionPhenotype a owl:Class ;
     rdfs:label "Spinal cord ascending projection phenotype" ;
-    rdfs:subClassOf ilxtr:ProjectionPhenotype ;
+    rdfs:subClassOf ilxtr:AnteriorProjecting ;
     rdfs:comment "projects in the anterior direction of the spinal cord" ;
     ilxtr:useObjectProperty ilxtr:hasProjectionPhenotype ;
     skos:hiddenLabel "Spinal cord ascending projection" .
 
 ilxtr:SpinalCordDescendingProjectionPhenotype a owl:Class ;
     rdfs:label "Spinal cord descending projection phenotype" ;
-    rdfs:subClassOf ilxtr:ProjectionPhenotype ;
+    rdfs:subClassOf ilxtr:PosteriorProjecting ;
     rdfs:comment "projects in the posterior direction of the spinal cord" ;
     ilxtr:useObjectProperty ilxtr:hasProjectionPhenotype ;
     skos:hiddenLabel "Spinal cord descending projection" .
 
 ilxtr:SpinyPhenotype a owl:Class ;
     rdfs:label "Spiny phenotype" ;
     rdfs:subClassOf ilxtr:DendritePhenotype ;
@@ -868,8 +882,8 @@
 
 ilxtr:UntuftedPyramidalPhenotype a owl:Class ;
     rdfs:label "Untufted pyramidal phenotype" ;
     rdfs:subClassOf ilxtr:PyramidalPhenotype ;
     ilxtr:useObjectProperty ilxtr:hasMorphologicalPhenotype ;
     skos:hiddenLabel "Untufted pyramidal" .
 
-### Serialized using the ttlser deterministic serializer v1.2.0
+### Serialized using the ttlser deterministic serializer v1.2.1
```

### Comparing `neurondm-0.1.4/setup.py` & `neurondm-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,44 +25,41 @@
     resources = 'resources'
     relpaths = ['ttl/phenotype-core.ttl',
                 'ttl/phenotype-indicators.ttl',
                 'ttl/phenotypes.ttl',
                 'ttl/generated/part-of-self.ttl',]
     if RELEASE:
         from augpathlib import RepoPath as Path
-        ### KILL IT WITH FIRE
-        try:
-            from neurondm.core import auth  ### this is NOT ok
-        except Exception:
-            # can't catch an error that you can never import because
-            # it will be raised before you can import it ... SIGH
-            import orthauth as oa
-            from pyontutils.config import auth as pauth
-            auth = oa.configure(Path('neurondm/auth-config.py').resolve(), include=pauth)
-        ###
-
+        from neurondm.core import auth  ### this is NOT ok
+        from pyontutils.core import OntResGit
         olr = Path(auth.get_path('ontology-local-repo'))
 
         ### KILL IT WITH FIRE
         if not olr.exists():
             original = auth.get('ontology-local-repo')
             raise FileNotFoundError(f'ontology local repo does not exist: {olr}'
                                     f'path expanded from {original}')
-        elif olr.repo.active_branch.name != auth.get('neurons-branch'):
+        #elif olr.repo.active_branch.name != auth.get('neurons-branch'):
             # FIXME yes indeed having to call Config in a way that is
             # invoked at import time is REALLY REALLY BAD :/
-            raise ValueError('git is on the wrong branch! '
-                             f'{olr.repo.active_branch}')
+            #raise ValueError('git is on the wrong branch! '
+                             #f'{olr.repo.active_branch}')
         ###
 
+        ref = auth.get('neurons-branch')
         resources = Path(resources)
         resources.mkdir()  # if we add resources to git, this will error before we delete by accident
         paths = [olr / rp for rp in relpaths]
         for p in paths:
-            p.copy_to(resources / p.name)
+            org = OntResGit(p, ref=ref)
+            target = resources / p.name
+            generator = org.data
+            with open(target, 'wb') as f:
+                for chunk in generator:
+                    f.write(chunk)
 
     else:
         from pathlib import Path
         resources = Path(resources)
         paths = [Path(rp) for rp in relpaths]
 
     return resources.absolute(), [(resources / p.name).as_posix() for p in paths]
```

### Comparing `neurondm-0.1.4/test/common.py` & `neurondm-0.1.5/test/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import unittest
 from pathlib import Path
 from tempfile import gettempdir
 import pytest
 from git import Repo
 from neurondm.core import log
```

### Comparing `neurondm-0.1.4/test/test_integration.py` & `neurondm-0.1.5/test/test_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,45 +11,46 @@
     """ woo! """
 
 
 only = tuple()
 
 lasts = tuple()
 
-neurons = ('neurondm/example',
-           'neurondm/phenotype_namespaces',
-           'neurondm/models/allen_cell_types',
-           'neurondm/models/phenotype_direct',
-           'neurondm/models/basic_neurons',
-           'neurondm/models/huang2017',
-           'neurondm/models/ma2015',
-           'neurondm/models/cuts',
-           'neurondm/build',
-           'neurondm/sheets',)
+neurons = (#'neurondm/example',
+           #'neurondm/phenotype_namespaces',
+           #'neurondm/models/allen_cell_types',
+           'neurondm/models/phenotype_direct',  # needs NIF-Neuron-Defined.ttl
+           'neurondm/models/basic_neurons',  # needs swanson.ttl
+           #'neurondm/models/huang2017',
+           #'neurondm/models/ma2015',
+           #'neurondm/models/cuts',
+           #'neurondm/build',
+           #'neurondm/sheets',
+)
 
 skip = tuple()
 olr = auth.get_path('ontology-local-repo')
 if olr.exists():
     ont_repo = Repo(olr)
     # FIXME these aren't called?
     post_load = lambda : (ont_repo.remove_diff_untracked(), ont_repo.checkout_diff_tracked())
     post_main = lambda : (ont_repo.remove_diff_untracked(), ont_repo.checkout_diff_tracked())
 
     ### handle ontology branch behavior
     checkout_ok = neurondm.core.ont_checkout_ok
     print('checkout ok:', checkout_ok)
     ont_branch = ont_repo.active_branch.name
     if not checkout_ok and ont_branch != 'neurons':
-        neurons += ('neurondm/core', 'neurondm/lang',)  # FIXME these two are ok for no repo but not wrong branch?!
+        #neurons += ('neurondm/core', 'neurondm/lang',)  # FIXME these two are ok for no repo but not wrong branch?!
         skip += tuple(n.split('/')[-1] for n in neurons)
     else:
         lasts += tuple(f'neurondm/{s}.py' for s in neurons)
 
 else:
-    skip += tuple(n.split('/')[-1] for n in neurons)
+    skip += tuple(n.split('/')[-1] for n in neurons)  # should be able to run without repo ?
 
 
 ### build mains
 mains = {}  # NOTE mains run even if this is empty ? is this desired?
 
 module_parent = Path(__file__).resolve().parent.parent.as_posix()
 working_dir = get_working_dir(__file__)
```

### Comparing `neurondm-0.1.4/test/test_label.py` & `neurondm-0.1.5/test/test_label.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/test/test_madness.py` & `neurondm-0.1.5/test/test_madness.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/test/test_neurons.py` & `neurondm-0.1.5/test/test_neurons.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/test/test_simple.py` & `neurondm-0.1.5/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/test/test_triples.py` & `neurondm-0.1.5/test/test_triples.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.4/test/test_write.py` & `neurondm-0.1.5/test/test_write.py`

 * *Files identical despite different names*

