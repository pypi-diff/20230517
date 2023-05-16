# Comparing `tmp/s2aff-0.45.tar.gz` & `tmp/s2aff-0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.45.tar", last modified: Tue May 16 20:56:30 2023, max compression
+gzip compressed data, was "s2aff-0.46.tar", last modified: Tue May 16 23:27:08 2023, max compression
```

## Comparing `s2aff-0.45.tar` & `s2aff-0.46.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.603282 s2aff-0.45/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.45/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:56:30.602981 s2aff-0.45/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.45/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.594975 s2aff-0.45/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.45/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.45/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.45/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.595311 s2aff-0.45/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.45/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.598537 s2aff-0.45/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9542 2023-05-16 20:55:45.000000 s2aff-0.45/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.45/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.45/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.45/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:43:25.000000 s2aff-0.45/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.600857 s2aff-0.45/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.45/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.600374 s2aff-0.45/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.602674 s2aff-0.45/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.45/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.45/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.45/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.45/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.45/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.45/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.45/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 20:56:30.603335 s2aff-0.45/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 20:56:18.000000 s2aff-0.45/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 23:27:08.214766 s2aff-0.46/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.46/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 23:27:08.214626 s2aff-0.46/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.46/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 23:27:08.206581 s2aff-0.46/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.46/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.46/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.46/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 23:27:08.206852 s2aff-0.46/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.46/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 23:27:08.210336 s2aff-0.46/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9771 2023-05-16 23:26:19.000000 s2aff-0.46/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.46/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.46/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.46/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.46/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.46/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.46/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34547 2023-05-16 23:25:25.000000 s2aff-0.46/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.46/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 23:27:08.212299 s2aff-0.46/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.46/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.46/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.46/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 23:27:08.211439 s2aff-0.46/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 23:27:07.000000 s2aff-0.46/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 23:27:08.000000 s2aff-0.46/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 23:27:07.000000 s2aff-0.46/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 23:27:08.000000 s2aff-0.46/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 23:27:08.000000 s2aff-0.46/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 23:27:08.214259 s2aff-0.46/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.46/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.46/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.46/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.46/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.46/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.46/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.46/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 23:27:08.214858 s2aff-0.46/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 23:26:59.000000 s2aff-0.46/setup.py
```

### Comparing `s2aff-0.45/LICENSE` & `s2aff-0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/README.md` & `s2aff-0.46/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/data/combine_gold.py` & `s2aff-0.46/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/data/download_latest_ror.py` & `s2aff-0.46/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/__init__.py` & `s2aff-0.46/s2aff/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         self.pairwise_model_delta_threshold = pairwise_model_delta_threshold
         self.no_ror_output_text = no_ror_output_text
         self.no_candidates_output_text = no_candidates_output_text
         self.number_of_top_candidates_to_return = number_of_top_candidates_to_return
         self.look_for_grid_and_isni = True
         set_s2aff_vars(self.ror_index, self.look_for_grid_and_isni, self.no_candidates_output_text, self.pairwise_model, self.top_k_first_stage, self.pairwise_model_threshold, self.no_ror_output_text, self.pairwise_model_delta_threshold, self.number_of_top_candidates_to_return)
 
-    def predict(self, raw_affiliations):
+    def predict(self, raw_affiliations, do_reranking_multiprocessing=False):
         """Predict function for raw affiliation strings
 
         :param raw_affiliations: a list of raw affiliation strings
 
         :return: a list of dictionaries with the following keys:
             "raw_affiliation": raw affiliation string
             "ner_prediction": raw NER prediction
@@ -176,8 +176,13 @@
         ner_predictions = self.ner_predictor.predict(raw_affiliations)
         print("Done")
 
         inputs_ = []
         for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions)):
             inputs_.append((counter, raw_affiliation, ner_prediction, len(raw_affiliations)))
 
-        return [process_item(input) for input in inputs_]
+        if not do_reranking_multiprocessing:
+            return [process_item(input) for input in inputs_]
+
+        with multiprocessing.get_context("spawn").Pool() as pool:
+            outputs = pool.map(process_item, inputs_)
+        return outputs
```

### Comparing `s2aff-0.45/s2aff/consts.py` & `s2aff-0.46/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/data.py` & `s2aff-0.46/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/features.py` & `s2aff-0.46/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/file_cache.py` & `s2aff-0.46/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/lightgbm_helpers.py` & `s2aff-0.46/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/model.py` & `s2aff-0.46/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/ror.py` & `s2aff-0.46/s2aff/ror.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     USE_PROB_WEIGHTS,
     WORD_MULTIPLIER,
     REINSERT_CUTOFF_FRAC,
     SCORE_BASED_EARLY_CUTOFF,
 )
 from s2aff.file_cache import cached_path
 
+from multiprocessing import set_start_method
+set_start_method("spawn")
+
 
 grid_extractor = re.compile(r"(grid\.\d{4,6}\.[0-9a-f]{1,2})")
 isni_extractor = re.compile(r"(?=(\d{4}\s{0,1}\d{4}\s{0,1}\d{4}\s{0,1}[xX\d]{4}))")
 
 
 def get_special_tokens_dict():
     special_tokens_dict = {
```

### Comparing `s2aff-0.45/s2aff/text.py` & `s2aff-0.46/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/timo/integration_test.py` & `s2aff-0.46/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff/timo/interface.py` & `s2aff-0.46/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/s2aff.egg-info/SOURCES.txt` & `s2aff-0.46/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.46/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.46/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/scripts/generate_lightgbm_training_data.py` & `s2aff-0.46/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/scripts/train_lightgbm_reranker.py` & `s2aff-0.46/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/scripts/train_ner_model.py` & `s2aff-0.46/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/scripts/update_openalex_works_counts.py` & `s2aff-0.46/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.45/setup.py` & `s2aff-0.46/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.45",
+    version="0.46",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

