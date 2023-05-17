# Comparing `tmp/nlp-models-1.0.2.tar.gz` & `tmp/nlp-models-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-1.0.2.tar", last modified: Tue May 16 13:55:13 2023, max compression
+gzip compressed data, was "nlp-models-1.0.4.tar", last modified: Tue May 16 15:20:19 2023, max compression
```

## Comparing `nlp-models-1.0.2.tar` & `nlp-models-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.491190 nlp-models-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 13:55:02.000000 nlp-models-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:55:13.491190 nlp-models-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 13:55:02.000000 nlp-models-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 13:55:02.000000 nlp-models-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 13:55:13.491190 nlp-models-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 13:55:02.000000 nlp-models-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.487190 nlp-models-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.487190 nlp-models-1.0.2/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.491190 nlp-models-1.0.2/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.491190 nlp-models-1.0.2/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:20:19.556776 nlp-models-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 15:20:02.000000 nlp-models-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 15:20:19.556776 nlp-models-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 15:20:02.000000 nlp-models-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 15:20:02.000000 nlp-models-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 15:20:19.556776 nlp-models-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 15:20:02.000000 nlp-models-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:20:19.552776 nlp-models-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:20:19.552776 nlp-models-1.0.4/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:20:19.556776 nlp-models-1.0.4/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-16 15:20:02.000000 nlp-models-1.0.4/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:20:19.556776 nlp-models-1.0.4/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 15:20:19.000000 nlp-models-1.0.4/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 15:20:19.000000 nlp-models-1.0.4/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:20:19.000000 nlp-models-1.0.4/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 15:20:19.000000 nlp-models-1.0.4/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 15:20:19.000000 nlp-models-1.0.4/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-1.0.2/LICENSE` & `nlp-models-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/PKG-INFO` & `nlp-models-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.0.2
+Version: 1.0.4
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-1.0.2/README.md` & `nlp-models-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/setup.cfg` & `nlp-models-1.0.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 1.0.2
+version = 1.0.4
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -16,14 +16,15 @@
 packages = find:
 package_dir = 
 	=src
 python_requires = 
 	>=3.6
 install_requires = 
 	torch
+	torchmetrics
 	transformers
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full =
```

### Comparing `nlp-models-1.0.2/src/bert_classifier/bert.py` & `nlp-models-1.0.4/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/bert_classifier/data.py` & `nlp-models-1.0.4/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/bert_classifier/io.py` & `nlp-models-1.0.4/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/bert_classifier/metrics.py` & `nlp-models-1.0.4/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/bert_classifier/predict.py` & `nlp-models-1.0.4/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/bert_classifier/train.py` & `nlp-models-1.0.4/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/multi_task_model/layers.py` & `nlp-models-1.0.4/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/multi_task_model/metrics.py` & `nlp-models-1.0.4/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/multi_task_model/mtl.py` & `nlp-models-1.0.4/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/multi_task_model/trainer.py` & `nlp-models-1.0.4/src/multi_task_model/trainer.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.2/src/multi_task_model/utils.py` & `nlp-models-1.0.4/src/multi_task_model/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 def batch_to_device(batch, target_device: device):
     '''
     Send a pytorch batch to a device (CPU/GPU)
     '''
     for key in batch:
         if isinstance(batch[key], Tensor):
             batch[key] = batch[key].squeeze(1).to(target_device)
+    return batch
 
 
 def get_embedding_group(label, cat_lookup, corpus):
     idx_grp = cat_lookup[label]
     corpus_embeddings, question_corpus, answer_corpus = corpus
     corpus_embeddings = corpus_embeddings[idx_grp]
     question_corpus = np.array(question_corpus)[idx_grp].tolist()
```

### Comparing `nlp-models-1.0.2/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-1.0.4/src/nlp_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.0.2
+Version: 1.0.4
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-1.0.2/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-1.0.4/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

