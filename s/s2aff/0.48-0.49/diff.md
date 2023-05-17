# Comparing `tmp/s2aff-0.48.tar.gz` & `tmp/s2aff-0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.48.tar", last modified: Wed May 17 02:07:59 2023, max compression
+gzip compressed data, was "s2aff-0.49.tar", last modified: Wed May 17 02:32:54 2023, max compression
```

## Comparing `s2aff-0.48.tar` & `s2aff-0.49.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:07:59.034328 s2aff-0.48/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.48/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 02:07:59.034084 s2aff-0.48/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.48/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:07:59.025274 s2aff-0.48/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.48/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.48/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.48/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:07:59.025603 s2aff-0.48/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.48/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:07:59.029112 s2aff-0.48/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11369 2023-05-17 02:04:34.000000 s2aff-0.48/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.48/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.48/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.48/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.48/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.48/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.48/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 23:30:17.000000 s2aff-0.48/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.48/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:07:59.031848 s2aff-0.48/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.48/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.48/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.48/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:07:59.031318 s2aff-0.48/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 02:07:58.000000 s2aff-0.48/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-17 02:07:58.000000 s2aff-0.48/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-17 02:07:58.000000 s2aff-0.48/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-17 02:07:58.000000 s2aff-0.48/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-17 02:07:58.000000 s2aff-0.48/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:07:59.033806 s2aff-0.48/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.48/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.48/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.48/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.48/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.48/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.48/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.48/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-17 02:07:59.034386 s2aff-0.48/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-17 01:46:16.000000 s2aff-0.48/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:32:54.411762 s2aff-0.49/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.49/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 02:32:54.411468 s2aff-0.49/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.49/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:32:54.401746 s2aff-0.49/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.49/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.49/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.49/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:32:54.402072 s2aff-0.49/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.49/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:32:54.405606 s2aff-0.49/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11210 2023-05-17 02:31:31.000000 s2aff-0.49/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.49/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.49/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.49/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.49/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.49/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.49/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 23:30:17.000000 s2aff-0.49/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.49/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:32:54.408575 s2aff-0.49/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.49/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.49/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.49/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:32:54.407509 s2aff-0.49/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-17 02:32:53.000000 s2aff-0.49/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-17 02:32:54.000000 s2aff-0.49/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-17 02:32:54.000000 s2aff-0.49/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-17 02:32:54.000000 s2aff-0.49/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-17 02:32:54.000000 s2aff-0.49/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-17 02:32:54.411026 s2aff-0.49/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.49/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.49/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.49/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.49/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.49/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.49/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.49/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-17 02:32:54.411887 s2aff-0.49/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-17 02:32:18.000000 s2aff-0.49/setup.py
```

### Comparing `s2aff-0.48/LICENSE` & `s2aff-0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/README.md` & `s2aff-0.49/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/data/combine_gold.py` & `s2aff-0.49/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/data/download_latest_ror.py` & `s2aff-0.49/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/__init__.py` & `s2aff-0.49/s2aff/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
 import multiprocess
 multiprocess.set_start_method("spawn", force=True)
 from s2aff.model import parse_ner_prediction
 from functools import partial
-import psutil
-ram = psutil.virtual_memory()
 
 logger = logging.getLogger("s2aff")
 logger.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 ch.setLevel(logging.INFO)
@@ -98,17 +96,15 @@
     ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = \
         ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_
 
 
 def reranking_multi(inputs, **kwargs):
     func = partial(process_item, **kwargs)
     with multiprocess.get_context("spawn").Pool(multiprocess.cpu_count()) as pool:
-        chunk_s = round(((ram.total/(2**30))/32)*150)  # general rule is 150 per 32 GB of RAM
-        print("CHUNK_SIZE:", chunk_s)
-        generator = pool.imap_unordered(func, inputs, chunk_s)
+        generator = pool.imap_unordered(func, inputs, min(100, inputs[-1][-1]))
         for result in generator:
             yield result
 
 
 class S2AFF:
     """
     The wrapper class that links a raw affiliation string to a ROR entry.
```

### Comparing `s2aff-0.48/s2aff/consts.py` & `s2aff-0.49/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/data.py` & `s2aff-0.49/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/features.py` & `s2aff-0.49/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/file_cache.py` & `s2aff-0.49/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/lightgbm_helpers.py` & `s2aff-0.49/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/model.py` & `s2aff-0.49/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/ror.py` & `s2aff-0.49/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/text.py` & `s2aff-0.49/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/timo/integration_test.py` & `s2aff-0.49/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff/timo/interface.py` & `s2aff-0.49/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/s2aff.egg-info/SOURCES.txt` & `s2aff-0.49/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.49/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.49/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/scripts/generate_lightgbm_training_data.py` & `s2aff-0.49/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/scripts/train_lightgbm_reranker.py` & `s2aff-0.49/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/scripts/train_ner_model.py` & `s2aff-0.49/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/scripts/update_openalex_works_counts.py` & `s2aff-0.49/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.48/setup.py` & `s2aff-0.49/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.48",
+    version="0.49",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

