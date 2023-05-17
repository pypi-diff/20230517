# Comparing `tmp/nlp-models-1.1.0.tar.gz` & `tmp/nlp-models-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-1.1.0.tar", last modified: Wed May 17 15:22:10 2023, max compression
+gzip compressed data, was "nlp-models-1.1.1.tar", last modified: Wed May 17 16:46:53 2023, max compression
```

## Comparing `nlp-models-1.1.0.tar` & `nlp-models-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:22:10.223508 nlp-models-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-17 15:21:59.000000 nlp-models-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-17 15:22:10.223508 nlp-models-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-17 15:21:59.000000 nlp-models-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 15:21:59.000000 nlp-models-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-17 15:22:10.223508 nlp-models-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 15:21:59.000000 nlp-models-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:22:10.219508 nlp-models-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:22:10.223508 nlp-models-1.1.0/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:22:10.223508 nlp-models-1.1.0/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-17 15:21:59.000000 nlp-models-1.1.0/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:22:10.223508 nlp-models-1.1.0/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-17 15:22:10.000000 nlp-models-1.1.0/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-17 15:22:10.000000 nlp-models-1.1.0/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:22:10.000000 nlp-models-1.1.0/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 15:22:10.000000 nlp-models-1.1.0/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 15:22:10.000000 nlp-models-1.1.0/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:46:53.949756 nlp-models-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-17 16:46:40.000000 nlp-models-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-17 16:46:53.949756 nlp-models-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-17 16:46:40.000000 nlp-models-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 16:46:40.000000 nlp-models-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-17 16:46:53.949756 nlp-models-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 16:46:40.000000 nlp-models-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:46:53.945756 nlp-models-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:46:53.949756 nlp-models-1.1.1/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:46:53.949756 nlp-models-1.1.1/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-17 16:46:40.000000 nlp-models-1.1.1/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:46:53.949756 nlp-models-1.1.1/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-17 16:46:53.000000 nlp-models-1.1.1/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-17 16:46:53.000000 nlp-models-1.1.1/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:46:53.000000 nlp-models-1.1.1/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 16:46:53.000000 nlp-models-1.1.1/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 16:46:53.000000 nlp-models-1.1.1/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-1.1.0/LICENSE` & `nlp-models-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/PKG-INFO` & `nlp-models-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.1.0
+Version: 1.1.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-1.1.0/README.md` & `nlp-models-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/setup.cfg` & `nlp-models-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 1.1.0
+version = 1.1.1
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-1.1.0/src/bert_classifier/bert.py` & `nlp-models-1.1.1/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/bert_classifier/data.py` & `nlp-models-1.1.1/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/bert_classifier/io.py` & `nlp-models-1.1.1/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/bert_classifier/metrics.py` & `nlp-models-1.1.1/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/bert_classifier/predict.py` & `nlp-models-1.1.1/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/bert_classifier/train.py` & `nlp-models-1.1.1/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/multi_task_model/layers.py` & `nlp-models-1.1.1/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/multi_task_model/metrics.py` & `nlp-models-1.1.1/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/multi_task_model/mtl.py` & `nlp-models-1.1.1/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/multi_task_model/trainer.py` & `nlp-models-1.1.1/src/multi_task_model/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
             optimizer, num_warmup_steps=warmup_steps, num_training_steps=t_total)
     else:
         raise ValueError(f'Unkown scheduler {scheduler}')
 
 
 def validate(model: torch.nn.Module,
              test_dataloader: DataLoader,
+             device: torch.device = torch.device('cpu'),
              multi_label: bool = False,
              num_labels: Optional[int] = None,
              metrics = accuracy,
-             device: torch.device = torch.device('cpu'),
              average: Literal['micro', 'macro', 'weighted', 'none'] = 'macro'
              ):
     '''
     Validate module
     '''
     model.eval()
     val_targets = torch.tensor(()).to(device)
@@ -135,15 +135,15 @@
         logger.info(f'''
             Training Info: 
                 Total Time: {time.time() - t0} sec || 
                 Average Loss: {avg_train_loss} ||
                 Average Accuracy: {avg_train_acc}
             ''')
         logger.info('Evaluation in progress...')
-        avg_val_loss, avg_val_acc = validate(model, test_dataloader, multi_label, num_labels, device, average=None)
+        avg_val_loss, avg_val_acc = validate(model, test_dataloader, device, multi_label, num_labels, average=None)
         logger.info(f'''
             Validation Info:
                 Time: {time.time() - t0} ||
                 Loss: {avg_val_loss} ||
                 Accuracy: {avg_val_acc}
         ''')
         save_checkpoint(model, optimizer_obj, epoch, avg_train_loss, avg_train_acc, avg_val_loss, avg_val_acc)
```

### Comparing `nlp-models-1.1.0/src/multi_task_model/utils.py` & `nlp-models-1.1.1/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.1.0/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-1.1.1/src/nlp_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.1.0
+Version: 1.1.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-1.1.0/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-1.1.1/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

