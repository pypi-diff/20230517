# Comparing `tmp/noise2read-0.0.76.tar.gz` & `tmp/noise2read-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.76.tar", last modified: Sat May 13 12:25:23 2023, max compression
+gzip compressed data, was "noise2read-0.0.81.tar", last modified: Wed May 17 05:41:07 2023, max compression
```

## Comparing `noise2read-0.0.76.tar` & `noise2read-0.0.81.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-13 12:25:23.722598 noise2read-0.0.76/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.76/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-13 12:25:23.724444 noise2read-0.0.76/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.76/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.76/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)     1000 2023-05-13 12:25:23.727464 noise2read-0.0.76/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-13 12:25:23.572083 noise2read-0.0.76/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-13 12:25:23.668244 noise2read-0.0.76/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-13 06:56:03.000000 noise2read-0.0.76/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    12784 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15992 2023-05-03 12:02:17.000000 noise2read-0.0.76/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    45703 2023-05-13 12:24:51.000000 noise2read-0.0.76/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11181 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    29580 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26366 2023-04-25 08:21:29.000000 noise2read-0.0.76/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    34369 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    12273 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.76/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-13 12:25:23.703091 noise2read-0.0.76/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-13 12:25:23.000000 noise2read-0.0.76/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-13 12:25:23.000000 noise2read-0.0.76/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-13 12:25:23.000000 noise2read-0.0.76/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-13 12:25:23.000000 noise2read-0.0.76/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.76/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      218 2023-05-13 12:25:23.000000 noise2read-0.0.76/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-13 12:25:23.000000 noise2read-0.0.76/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-13 12:25:23.717768 noise2read-0.0.76/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.76/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.76/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.76/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 05:41:07.296411 noise2read-0.0.81/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.81/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 05:41:07.310039 noise2read-0.0.81/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.81/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.81/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-17 05:41:07.328358 noise2read-0.0.81/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 05:41:06.601056 noise2read-0.0.81/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 05:41:06.984377 noise2read-0.0.81/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-17 00:22:19.000000 noise2read-0.0.81/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.81/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16457 2023-05-17 01:27:10.000000 noise2read-0.0.81/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.81/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.81/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    45704 2023-05-16 13:16:54.000000 noise2read-0.0.81/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.81/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.81/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.81/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.81/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.81/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    34335 2023-05-16 12:55:31.000000 noise2read-0.0.81/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.81/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.81/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.81/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 05:41:07.166310 noise2read-0.0.81/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 05:41:06.000000 noise2read-0.0.81/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-17 05:41:06.000000 noise2read-0.0.81/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-17 05:41:06.000000 noise2read-0.0.81/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-17 05:41:06.000000 noise2read-0.0.81/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.81/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-17 05:41:06.000000 noise2read-0.0.81/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-17 05:41:06.000000 noise2read-0.0.81/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 05:41:07.282350 noise2read-0.0.81/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.81/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.81/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.81/tests/test_utils.py
```

### Comparing `noise2read-0.0.76/LICENSE` & `noise2read-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/PKG-INFO` & `noise2read-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.76
+Version: 0.0.81
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.76/README.rst` & `noise2read-0.0.81/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/setup.cfg` & `noise2read-0.0.81/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	biopython == 1.79
 	xgboost == 1.6.1
 	Xlsxwriter == 3.0.3
 	tqdm == 4.64.0
 	scikit-learn == 1.1.1
 	networkx == 2.8.5
 	pandas == 1.4.3
-	optuna == 2.10.1
+	optuna >= 3.1.1
 	matplotlib == 3.5.2
 	mpire >= 2.5.0
 	editdistance == 0.6.0
 	imbalanced-learn == 0.9.1
 	seaborn >= 0.12.1
 
 [options.packages.find]
```

### Comparing `noise2read-0.0.76/src/noise2read/classifier.py` & `noise2read-0.0.81/src/noise2read/classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-04-07 22:31:52
+# @Last Modified time: 2023-05-16 18:27:41
 
 import optuna
+from optuna.samplers import TPESampler
 from sklearn.model_selection import train_test_split
 import os
 import xgboost as xgb
 import numpy as np
 # from imblearn.combine import SMOTEENN
 from imblearn.over_sampling import SMOTE 
 import collections
@@ -39,23 +40,30 @@
         self.logger = logger
         self.config = config
         self.study_name = study_name
         self.data = data
         self.label = label
         self.ambi_data = ambi_data
 
-        self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(self.data, self.label, test_size=self.config.test_size, shuffle=True, random_state=self.config.random_state)
+        # Shuffle the data in a deterministic way
+        np.random.seed(self.config.random_state)
+        indices = np.random.permutation(len(self.data))
+        shuffled_data = self.data[indices]
+        shuffled_labels = self.label[indices]
+        self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(shuffled_data, shuffled_labels, test_size=self.config.test_size, shuffle=False, random_state=self.config.random_state)
+
+        # self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(self.data, self.label, test_size=self.config.test_size, shuffle=True, random_state=self.config.random_state)
 
         # self.x_test, self.x_val, self.y_test, self.y_val, self.x_test_weight, self.x_val_weight = train_test_split(test_val_x, test_val_y, test_val_weight, test_size=0.50, random_state=self.config.random_state, shuffle=True)
         # self.x_test_weight, self.x_val_weight = train_test_split(test_val_weight, test_size=0.50, random_state=self.config.random_state, shuffle=False)
         # self.logger.debug(type(self.x_val_weight))
         # self.logger.debug(f'{self.x_val}, {self.y_val.shape}, {len(self.x_val_weight)}')
         self.logger.info(f'The number of negative and positive samples: {sorted(collections.Counter(self.y_train).items())}')
 
-        sm = SMOTE(random_state=0)
+        sm = SMOTE(random_state=self.config.random_state)
         self.X_resampled, self.y_resampled = sm.fit_resample(self.x_train, self.y_train)
         self.logger.info(f'After over-sampling: {sorted(collections.Counter(self.y_resampled).items())}')
 
         # rus = RandomUnderSampler(random_state=42)
         # self.X_resampled, self.y_resampled = rus.fit_resample(self.x_train, self.y_train)
         # self.logger.info(f'After under-sampling {sorted(collections.Counter(self.y_resampled).items())}')
 
@@ -122,16 +130,16 @@
         # y_count = sorted(collections.Counter(self.y_train).items())
         # _, neg_num = y_count[0]
         # _, pos_num = y_count[1]
         # xgbc = xgb.XGBClassifier(**param, pruning_callback=[pruning_callback], probability=True, scale_pos_weight= neg_num/pos_num)
         # xgbc.fit(self.x_train, self.y_train, eval_set=[(self.x_train, self.y_train),(self.x_test, self.y_test)],  verbose=True)
         # train_accuracy = xgbc.score(self.x_train, self.y_train)
 
-        xgbc = xgb.XGBClassifier(**param, pruning_callback=[pruning_callback], probability=True)
-        xgbc.fit(self.X_resampled, self.y_resampled, eval_set=[(self.X_resampled, self.y_resampled),(self.x_test, self.y_test)],  verbose=self.config.verbose_eval)
+        xgbc = xgb.XGBClassifier(**param, pruning_callback=[pruning_callback], probability=True, seed=self.config.xgboost_seed)
+        xgbc.fit(self.X_resampled, self.y_resampled, eval_set=[(self.X_resampled, self.y_resampled), (self.x_test, self.y_test)],  verbose=self.config.verbose_eval)
         
         # xgbc.fit(self.x_train, self.y_train, eval_set=[(self.x_train, self.y_train),(self.x_test, self.y_test)],  verbose=True)
         # xgbc.fit(self.x_train, self.y_train, eval_set=[(self.x_val, self.y_val)], verbose=False)
         # xgbc.fit(self.x_train, self.y_train, sample_weight = self.x_train_weight, eval_set=[(self.x_val, self.y_val)], sample_weight_eval_set = [self.x_val_weight],  verbose=False)
 
         # accuracy = xgbc.score(self.x_test, self.y_test, sample_weight=self.x_test_weight)
         # train_accuracy = xgbc.score(self.X_resampled, self.y_resampled)
@@ -172,18 +180,19 @@
             array: numpy ndarray of shape (n_samples, n_classes)
             Estimated probabilities.
         """
         # study = optuna.create_study(study_name = self.study_name,
         #     pruner=optuna.pruners.MedianPruner(n_warmup_steps=5), direction="maximize" 
         # ) #, interval_steps=10 n_startup_trials=5, 
         self.logger.info("-------------------------------------------------------------")
-        study = optuna.create_study(study_name = self.study_name, direction="maximize")
+        sampler = TPESampler(seed=self.config.optuna_seed)  # Make the sampler behave in a deterministic way.
+        study = optuna.create_study(study_name = self.study_name, direction="maximize", sampler=sampler)
         study.optimize(self.objective, n_trials, show_progress_bar=False, gc_after_trial=True)
         # print(study.best_trial)
-        
+
         self.logger.info(f'Study Name: {self.study_name}')
         self.logger.info('Number of finished trials: {}'.format(len(study.trials)))
         self.logger.info('Best trial:')
         best_trial = study.best_trial
         self.logger.info('  Test Accuracy: {}'.format(best_trial.value))
         self.logger.info('  Params: ')
         for key, value in best_trial.params.items():
```

### Comparing `noise2read-0.0.76/src/noise2read/config.py` & `noise2read-0.0.81/src/noise2read/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-19 10:56:38
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-03 22:02:17
+# @Last Modified time: 2023-05-17 11:27:10
 
 import configparser
 import os
 
 class Config(object):
     def __init__(self, config_file, logger):
         conf = configparser.ConfigParser()
@@ -105,18 +105,18 @@
                 self.kmer_freq = 3  
             if conf.has_option("EmbeddingSetup", "read_type"):
                 self.read_type = conf.get("EmbeddingSetup", "read_type")
             else:
                 self.read_type = 'DNA'
 
             # AmbiguousSetup
-            if conf.has_option("AmbiguousSetup", "ambiguous_error_node_degree"):
-                self.ambiguous_error_node_degree = conf.getint("AmbiguousSetup", "ambiguous_error_node_degree")
-            else:
-                self.ambiguous_error_node_degree = 4 # default 
+            # if conf.has_option("AmbiguousSetup", "ambiguous_error_node_degree"):
+            #     self.ambiguous_error_node_degree = conf.getint("AmbiguousSetup", "ambiguous_error_node_degree")
+            # else:
+            #     self.ambiguous_error_node_degree = 4 # default 
             if conf.has_option("AmbiguousSetup", "high_ambiguous"):
                 self.high_ambiguous = conf.getboolean("AmbiguousSetup", "high_ambiguous")
             else:
                 self.high_ambiguous = True        
             if conf.has_option("AmbiguousSetup", "proba_deviation"):
                 self.proba_deviation = conf.getfloat("AmbiguousSetup", "proba_deviation")
             else:
@@ -202,18 +202,23 @@
             
             if conf.has_option("ModelTuningSetup", "verbose_eval"):
                 self.verbose_eval = conf.getboolean("ModelTuningSetup", "verbose_eval")
             else:
                 self.verbose_eval = False
                 
             # xgboostclassifier seed
-            if conf.has_option("ModelTuningSetup", "seed"):
-                self.seed = conf.getint("ModelTuningSetup", "seed")
+            if conf.has_option("ModelTuningSetup", "xgboost_seed"):
+                self.xgboost_seed = conf.getint("ModelTuningSetup", "xgboost_seed")
+            else:
+                self.xgboost_seed = 32 # default 
+
+            if conf.has_option("ModelTuningSetup", "optuna_seed"):
+                self.optuna_seed = conf.getint("ModelTuningSetup", "optuna_seed")
             else:
-                self.seed = 32 # default 
+                self.optuna_seed = 32 # default 
 
             if conf.has_option("ModelTuningSetup", "best_accuracy"):
                 self.best_accuracy = conf.getfloat("ModelTuningSetup", "best_accuracy")
             else:
                 self.best_accuracy = 0.8 # default     
 
             # real umi
@@ -283,36 +288,37 @@
             self.top_n = 100      
             # self.over_sampling = True 
             self.negative_sample_num = 500000
             self.min_read_len = 30
 
             # GraphSetup
             self.high_freq_thre = 4
-            self.max_error_freq = 3
+            self.max_error_freq = 4
             self.save_graph = False
             self.graph_visualization = False
             self.drawing_graph_num = 50   
 
             # EmbeddingSetup
             self.entropy_kmer = 3
             self.entropy_q = 2
             self.kmer_freq = 3
             self.read_type = 'DNA'
 
             # AmbiguousSetup
             self.high_ambiguous = True 
             # high ambiguous predict probability difference
-            self.proba_deviation = 0.6      # for base editing and lncRNA quant datasets 0.75 others 0.6 
-            self.ambiguous_error_node_degree = 4   # for base editing and lncRNA quant datasets 3 others 4 
+            self.proba_deviation = 0.95      # for base editing and lncRNA quant datasets 0.75 others 0.6 
+            # self.ambiguous_error_node_degree = 4   # for base editing and lncRNA quant datasets 3 others 4 
 
             # ModelTuningSetup
-            self.n_trials = 20
+            self.n_trials = 30
             self.n_estimators = 400
-            self.test_size = 0.1 # default        
-            self.random_state = 32 # default  
+            self.test_size = 0.1 # default 
+            # random state for SMOTE and train_test_split       
+            self.random_state = 42 # default  
             self.tree_method = 'auto'
             self.learning_rate_min = 1e-3 # default     
             self.learning_rate_max = 1e-1 # default 
             self.max_depth_min = 3 # default     
             self.max_depth_max = 15 # default     
             self.max_depth_step = 1 # default 
             self.num_boost_round_min = 200 # default     
@@ -320,15 +326,16 @@
             self.num_boost_round_step = 10 # default 
             self.subsample_min = 0.8 # default     
             self.subsample_max = 1 # default     
             self.colsample_bytree_min = 0.8 # default     
             self.colsample_bytree_max = 1 # default     
             self.verbose_eval = False
             # xgboostclassifier seed
-            self.seed = 32 # default 
+            self.xgboost_seed = 42 # default 
+            self.optuna_seed = 42
             # optuna best trial accuracy
             self.best_accuracy = 0.8
 
             # real umi
             self.umi_start = 0
             self.umi_end = 12
             self.non_umi_start = 24
@@ -336,18 +343,21 @@
             #amplicon
             self.amplicon_low_freq = 50
             self.amplicon_high_freq = 1500
             self.amplicon_threshold_proba = 0.85
             self.amplicon_error_node_degree = 4
 
             # simulation
-            self.min_read_count = 30
+            self.min_freq = 4
+            self.min_read_count = 29
             self.substations = True
-            self.indels = False
-            self.error_rate = 0.001
+            self.indels = True
+            self.error_rate1 = 0.01
+            self.error_rate2 = 0.005
+            self.sim_random_state = 42
 
             # # Evaluation
             # self.delta = 1
 
             # # coverage
             # self.library_layout = 'PE'
             # self.Alignment = '--local' # '--end-to-end'
```

### Comparing `noise2read-0.0.76/src/noise2read/coverage.py` & `noise2read-0.0.81/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/src/noise2read/data_analysis.py` & `noise2read-0.0.81/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/src/noise2read/data_generation.py` & `noise2read-0.0.81/src/noise2read/data_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-13 22:24:36
+# @Last Modified time: 2023-05-16 23:16:54
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -212,15 +212,15 @@
             edges_lst = [e for e in sub_graph.edges()]
             if len(edges_lst) > 0:
                 nodes_lst = list(sub_graph.nodes)
                 for node in nodes_lst:
                     node_count = sub_graph.nodes[node]['count']
                     node_degree = sub_graph.degree[node]
                     line = []
-                    if node_degree >= 1 and node_degree <= 4 and node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']:
+                    if node_degree >= 1 and node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']: #and node_degree <= 4
                         node_neis = [n for n in sub_graph.neighbors(node)]
                         # nei2count = []
                         nei_degree_count = []
                         for nei in node_neis:
                             nei_count = sub_graph.nodes[nei]['count']
                             nei_degree = sub_graph.degree[nei]
                             # nei2count.append((nei, nei_count))
@@ -708,22 +708,22 @@
             edges_lst = [e for e in sub_graph.edges()]
             if len(edges_lst) > 0:
                 nodes_lst = list(sub_graph.nodes)
                 for node in nodes_lst:
                     node_count = sub_graph.nodes[node]['count']
                     node_degree = sub_graph.degree[node]
                     line = []
-                    if node_count <= amplicon_low_freq and not sub_graph.nodes[node]['flag'] and node_degree <= self.config.amplicon_error_node_degree:
+                    if node_count < amplicon_low_freq and not sub_graph.nodes[node]['flag']:# and node_degree <= self.config.amplicon_error_node_degree:
                         node_neis = [n for n in sub_graph.neighbors(node)]
                         # nei2count = []
                         nei_degree_count = []
                         for nei in node_neis:
                             nei_count = sub_graph.nodes[nei]['count']
                             nei_degree = sub_graph.degree[nei]
-                            if nei_count >= amplicon_high_freq:
+                            if nei_count > amplicon_high_freq:
                                 line = [nei, nei_count, nei_degree, node, node_count, node_degree]
                                 new_line = self.err_type_classification(line) 
                                 new_line.insert(0, idx) 
                                 # writer.writerow(new_line)
                                 amplicon_df.loc[len(amplicon_df)] = new_line
                         idx += 1
                         sub_graph.nodes[node]['flag'] = True
```

### Comparing `noise2read-0.0.76/src/noise2read/data_preprocessing.py` & `noise2read-0.0.81/src/noise2read/data_preprocessing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:11:05
+# @Last Modified time: 2023-05-17 10:24:07
 
 import collections
 from Bio import SeqIO
 from Bio.SeqRecord import SeqRecord
 import os
 from noise2read.utils import *
 from noise2read.data_generation import DataGneration
 from noise2read.error_orrection import ErrorCorrection
 # from noise2read.data_analysis import DataAnalysis
 import editdistance
 from tqdm import tqdm
 from Bio.Seq import Seq
 
 class DataProcessing():
-    def __init__(self, logger, num_workers, output_dir, umi_start=None, umi_end=None, non_umi_start=None):
+    # def __init__(self, logger, num_workers, output_dir, umi_start=None, umi_end=None, non_umi_start=None):
+    def __init__(self, logger, config):
         self.logger = logger
-        self.num_workers = num_workers
-        self.output_dir = output_dir
-        self.umi_start = umi_start
-        self.umi_end = umi_end
-        self.non_umi_start = non_umi_start
-        if os.path.exists(self.output_dir):
-            self.logger.info("Directory '% s' already exists" % self.output_dir)
+        self.config = config
+        
+        if os.path.exists(self.config.result_dir):
+            self.logger.info("Directory '% s' already exists" % self.config.result_dir)
         else:
-            os.makedirs(self.output_dir)
-        if os.path.exists(self.output_dir + 'raw/'):
-            self.logger.info("Directory '% s' already exists" % self.output_dir + 'raw/')
+            os.makedirs(self.config.result_dir)
+        if os.path.exists(self.config.result_dir + 'raw/'):
+            self.logger.info("Directory '% s' already exists" % self.config.result_dir + 'raw/')
         else:
-            os.makedirs(self.output_dir + 'raw/')       
-        if os.path.exists(self.output_dir + 'true/'):
-            self.logger.info("Directory '% s' already exists" % self.output_dir + 'true/')
+            os.makedirs(self.config.result_dir + 'raw/')       
+        if os.path.exists(self.config.result_dir + 'true/'):
+            self.logger.info("Directory '% s' already exists" % self.config.result_dir + 'true/')
         else:
-            os.makedirs(self.output_dir + 'true/') 
+            os.makedirs(self.config.result_dir + 'true/') 
                
     def extract_umis(self, original_data, umi_start, umi_end, non_umi_start):
         record_iterator, ff_type = parse_data(original_data) 
         self.logger.info("Read Data")
         umi_records = []
         non_umi_records = []
 
@@ -71,43 +69,46 @@
         with open(non_umi_raw_dataset, "w") as handle:
             SeqIO.write(non_umi_records, handle, ff_type) 
         self.logger.info("Split umi and non-umis completed.") 
         return umi_raw_dataset, non_umi_raw_dataset
 
     def real_umi_data(self, original_data):
         # step1: extract umis to a sperate fastq file
-        umi_raw_dataset, non_umi_raw_dataset = self.extract_umis(original_data, self.umi_start, self.umi_end, self.non_umi_start)
+        umi_raw_dataset, non_umi_raw_dataset = self.extract_umis(original_data, self.config.umi_start, self.config.umi_end, self.config.non_umi_start)
         # step2: correct umi errors
-        DG = DataGneration(
-            self.logger,
-            self.num_workers,
-            umi_raw_dataset, 
-            self.output_dir,
-            high_freq_thre = 5,
-            max_error_freq = 4,
-            save_graph = False,
-            graph_visualization = False,
-            drawing_graph_num = False,
-            high_ambiguous=False, 
-            verbose=True
-            )
+        self.config.input_file = umi_raw_dataset
+        DG = DataGneration(self.logger, self.config)
+        # DG = DataGneration(
+        #     self.logger,
+        #     self.config.num_workers,
+        #     umi_raw_dataset, 
+        #     self.config.output_dir,
+        #     high_freq_thre = self.config.high_freq_thre,
+        #     max_error_freq = self.config.max_error_freq,
+        #     save_graph = self.config.save_graph,
+        #     graph_visualization = self.config.graph_visualization,
+        #     drawing_graph_num = self.config.drawing_graph_num,
+        #     high_ambiguous=self.config.high_ambiguous, 
+        #     verbose=self.config.verbose
+        #     )
         genuine_df = DG.extract_umi_genuine_errs()
         # ##############################################################
-        EC = ErrorCorrection(
-            self.logger,
-            self.num_workers,
-            umi_raw_dataset,
-            self.output_dir,
-            read_max_len = self.umi_end - self.umi_start,
-            entropy_kmer=3, 
-            entropy_q=2, 
-            kmer_freq=3,
-            read_type="DNA",
-            iso_change_detail=False,
-            min_iters=100)
+        EC = ErrorCorrection(self.logger, self.config)
+        # EC = ErrorCorrection(
+        #     self.logger,
+        #     self.num_workers,
+        #     umi_raw_dataset,
+        #     self.output_dir,
+        #     read_max_len = self.umi_end - self.umi_start,
+        #     entropy_kmer=3, 
+        #     entropy_q=2, 
+        #     kmer_freq=3,
+        #     read_type="DNA",
+        #     iso_change_detail=False,
+        #     min_iters=100)
         corrected_file = EC.umi_correction(umi_raw_dataset, genuine_df)
 
         # base_name = umi_raw_dataset.split("/")[-1].split(".fastq")[0]
         # step3: use umi and real dataset to generate raw and true dataset
         raw_file, true_file = self.raw_true_umi(corrected_file, non_umi_raw_dataset)
         return raw_file, true_file
```

### Comparing `noise2read-0.0.76/src/noise2read/encoding.py` & `noise2read-0.0.81/src/noise2read/encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:11:17
+# @Last Modified time: 2023-05-14 11:00:24
+# The codes in this section for features construction are modified from https://github.com/Bonidia/MathFeature, if you re-use these codes or methods, please also cite the original publication of Robson P Bonidia, Douglas S Domingues, Danilo S Sanches, André C P L F de Carvalho, MathFeature: feature extraction package for DNA, RNA and protein sequences based on mathematical descriptors, Briefings in Bioinformatics, 2021; bbab434, https://doi.org/10.1093/bib/bbab434.
+
 
 import numpy as np
 import statistics
 from scipy.fftpack import fft
 import math
 
 class FourierTransform():
```

### Comparing `noise2read-0.0.76/src/noise2read/error_orrection.py` & `noise2read-0.0.81/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/src/noise2read/isolates_correction.py` & `noise2read-0.0.81/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/src/noise2read/noise2read.py` & `noise2read-0.0.81/src/noise2read/noise2read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2022-12-29 23:04:12
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-04-25 18:21:29
+# @Last Modified time: 2023-05-16 23:42:25
 
 from noise2read.config import Config
 import sys, getopt
 from noise2read.data_generation import DataGneration
 from noise2read.error_orrection import ErrorCorrection
 from noise2read.data_analysis import DataAnalysis
 import os
@@ -20,15 +20,16 @@
     argv = sys.argv[1:]
     # create logger
     logger = custom_logger("noise2read", debug_mode=False)
 
     ##############################################################
     try:
         # opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:o:l:h:", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "over_sampling", "libray_layout", "help"]) 
-        opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:l:hv", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "libray_layout", "help", "version"]) 
+        # opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:l:hv", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "libray_layout", "help", "version"]) 
+        opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:hv", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "help", "version"]) 
         script_name = sys.argv[0]
         input_commands = [script_name]
 
         for opt, arg in opts:
             input_commands.append(opt)
             if arg:
                 input_commands.append(arg)
@@ -344,21 +345,15 @@
                     if d_lst:
                         config.result_dir = opts_dict[d_lst[0]] 
                     if config.num_workers <= 0:
                         config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
                         config.num_workers = available_cpu_cores
-                    DP = DataProcessing( 
-                        logger,
-                        config.num_workers,
-                        config.result_dir,
-                        config.umi_start,
-                        config.umi_end,
-                        config.non_umi_start)
+                    DP = DataProcessing(logger, config)
                     DP.real_umi_data(config.input_file)                  
 ############################################################################################################################
                 elif module_arg == "evaluation":   
                     if i_lst and t_lst and r_lst:
                         config = Config(None, logger)  
                         config.input_file = opts_dict[i_lst[0]]
                         config.ground_truth_data = opts_dict[t_lst[0]]
```

### Comparing `noise2read-0.0.76/src/noise2read/reads2vectors.py` & `noise2read-0.0.81/src/noise2read/reads2vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-04-07 16:47:06
+# @Last Modified time: 2023-05-16 22:55:31
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
@@ -60,15 +60,15 @@
         # onehot_fea = ES.descriptors("OneHot", reads_lst1[i])
         # features.extend(onehot_fea)
         features.extend(other_features[i])
         # self.logger.debug(f'FourierTransform: {len(ft_fea)}, ChaosGame: {len(cg_fea)}, Entropy: {len(entropy_fea)}, FickettScore: {len(fs_fea)}')
         return features 
 
     def high_all_in_one_embedding(self, genuine_df, negative_df, new_negative_df, ambiguous_df):
-        self.logger.info("  Embedding genuine and high ambiguous data.")
+        self.logger.info("Embedding genuine and high ambiguous data.")
         genuine_reads_lst1 = []
         negtive_reads_lst1 = []
         ambiguous_reads_lst1 = []
 
         genuine_reads_lst2 = []
         negtive_reads_lst2 = []
         ambiguous_reads_lst2 = []
@@ -164,29 +164,29 @@
             cur_kmer1 = row['StartErrKmer']
             cur_kmer2 = row['EndErrKmer']
             cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
             cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
             cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
             negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
 
-        # # isolates negative
-        # for idx, row in negative_df.iterrows():
-        #     read = row['StartRead']
-        #     pos_reads = enumerate_ed1_seqs(read)
-        #     for read2 in pos_reads:
-        #         negtive_reads_lst1.append(read) 
-        #         negtive_reads_lst2.append(read2)  
-        #         cur_err_tye_kmers = error_type_classification(read, read2)
-        #         cur_err_tye = cur_err_tye_kmers[0]
-        #         cur_kmer1 = cur_err_tye_kmers[1]
-        #         cur_kmer2 = cur_err_tye_kmers[2]
-        #         cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
-        #         cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
-        #         cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-        #         negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
+        # isolates negative
+        for idx, row in negative_df.iterrows():
+            read = row['StartRead']
+            pos_reads = enumerate_ed1_seqs(read)
+            for read2 in pos_reads:
+                negtive_reads_lst1.append(read) 
+                negtive_reads_lst2.append(read2)  
+                cur_err_tye_kmers = error_type_classification(read, read2)
+                cur_err_tye = cur_err_tye_kmers[0]
+                cur_kmer1 = cur_err_tye_kmers[1]
+                cur_kmer2 = cur_err_tye_kmers[2]
+                cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
+                cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
+                cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
+                negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
 
         for idx, row in ambiguous_df.iterrows():
             ambiguous_reads_lst1.append(row['StartRead'])
             ambiguous_reads_lst2.append(row['EndRead'])
             cur_err_tye = row['ErrorTye']
             cur_kmer1 = row['StartErrKmer']
             cur_kmer2 = row['EndErrKmer']
@@ -214,15 +214,15 @@
         self.logger.debug(ambiguous_data.shape)
         train, ambiguous = self.scaler(train_data, ambiguous_data, high_flag=True)
         self.logger.debug(train[0])
         del train_data, ambiguous_data, genuine_fea, negative_fea, ambiguous_fea, read_features
         return train, labels, ambiguous
 
     def all_in_one_embedding(self, total_reads, genuine_df, negative_df, ambiguous_df, high_flag):
-        self.logger.info("  Embedding genuine and ambiguous data.")
+        self.logger.info("Embedding genuine and ambiguous data.")
         genuine_reads_lst1 = []
         negtive_reads_lst1 = []
         ambiguous_reads_lst1 = []
 
         genuine_reads_lst2 = []
         negtive_reads_lst2 = []
         ambiguous_reads_lst2 = []
```

### Comparing `noise2read-0.0.76/src/noise2read/simulation.py` & `noise2read-0.0.81/src/noise2read/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,281 +1,423 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
-# @Date:   2023-02-16 11:04:45
+# @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-02-16 11:11:52
+# @Last Modified time: 2023-04-07 17:22:18
 
-import collections
 from Bio import SeqIO
-# import gzip
-from Bio.SeqRecord import SeqRecord
-from Bio.Seq import Seq
-from tqdm import tqdm
+import gzip
+# from Bio.SeqRecord import SeqRecord
+# from Bio.Seq import Seq
+import logging
+from colorlog import ColoredFormatter
 import copy
 import random
-from mpire import WorkerPool
+import editdistance
 import os
-from noise2read.utils import *
-from noise2read.data_generation import DataGneration
-from noise2read.error_orrection import ErrorCorrection
-from noise2read.data_preprocessing import DataProcessing
-
-class Simulation():
-    # def __init__(self, logger, config, num_workers, f_in, error_rate, output_dir, substations, indels, seed=0):
-    def __init__(self, logger, config):
-        self.logger = logger
-        self.config = config
-        if os.path.exists(config.result_dir):
-            self.logger.info("Directory '% s' already exists" % config.result_dir)
-            # for f in os.listdir(self.config.result_dir):
-            #     os.remove(os.path.join(self.config.result_dir, f))
-        else:
-            os.makedirs(config.result_dir)
-            self.logger.info("Directory '% s' created" % config.result_dir)
-
-    def enumerate_ed1_seqs(self, read):
-        possible_ed1 = []
-        if self.config.substations:
-            possible_ed1.extend(self.seq2substitution(read))
-        if self.config.indels:
-            possible_ed1.extend(self.seq2deletion(read))
-            possible_ed1.extend(self.seq2insertion(read))
-        return list(set(possible_ed1))
-
-    def replace_char(self, seq, char, index):
-        seq[index] = char
-        return ''.join(seq)
-
-    def sub_base(self, base):
-        if base == 'A':
-            return 'TCG'
-        elif base == 'T':
-            return 'ACG'
-        elif base == 'C':
-            return 'ATG'
-        elif base == 'G':
-            return 'ACT'
-        elif base == 'N':
-            return 'N'
-            
-    def seq2substitution(self, read):
-        """
-        enumerate all the substitutions for one read 
-        Args:
-            read (str): a sequence
-        Returns:
-            set: a set contains reads
-        """
-        editdis1_list = []
-        # substitution
-        raw_seq = list(read)
-        n = len(raw_seq)
-        for i in range(n):
-            seq = copy.deepcopy(raw_seq)
-            temp_base = seq[i]
-            #print(temp_base)
-            temp_sub_base = list(self.sub_base(temp_base))
-            #print(temp_sub_base)
-            for b in temp_sub_base:
-                if b != 'N':
-                    sub_seq = self.replace_char(seq, b, i)
-                    editdis1_list.append(sub_seq)
-        return set(editdis1_list)
-
-    def seq2deletion(self, read):
-        """
-        enumerate all the deletions for one read 
-        Args:
-            read (str): a sequence
-        Returns:
-            set: a set contains reads
-        """
-        editdis1_list = []
-        seq = list(read)
-        n = len(seq)
-        # deletion
-        for i in range(n):
-            del_seq = read[:i] + read[(i+1):]
-            editdis1_list.append(del_seq)
-        return set(editdis1_list)
-
-    def seq2insertion(self, read):
-        """
-        enumerate all the insertions for one read 
-        Args:
-            read (str): a sequence
-        Returns:
-            set: a set contains reads
-        """
-        editdis1_list = []
-        seq = list(read)
-        n = len(seq)
-        # insertion
-        bases = ['A', 'G', 'C', 'T']
-        for i in range(n+1):
-            for b in bases:
-                raw_seq = copy.deepcopy(seq)
-                raw_seq.insert(i, b)
-                editdis1_list.append(''.join(raw_seq))
-        return set(editdis1_list)
-        
-    def read2err_read(self, read):
-        possible_seqs = self.enumerate_ed1_seqs(read)
-        num = len(possible_seqs)
-        # random.seed(self.config.indels)
-        random.shuffle(possible_seqs)
-        idx = random.randint(0, num-1)
-        return possible_seqs[idx]
-
-    def error_correction(self, config):
-        DG = DataGneration(self.logger, config)
-        if config.high_ambiguous:
-            isolates_file, non_isolates_file, unique_seqs, read_max_len, read_min_len, genuine_df, negative_df, ambiguous_df, high_ambiguous_df = DG.data_files(edit_dis=1)
-        else:
-            isolates_file, non_isolates_file, unique_seqs, read_max_len, read_min_len, genuine_df, negative_df, ambiguous_df = DG.data_files(edit_dis=1)      
-        config.read_max_len = read_max_len
-        ###############################################################
-        EC = ErrorCorrection(self.logger, config)
-        ## one model to predict
-        if config.high_ambiguous:
-            ##################################
-            corrected_file, new_negative_df = EC.all_in_one_correction(isolates_file, non_isolates_file, unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df)
-        else:
-            corrected_file, new_negative_df = EC.all_in_one_correction(isolates_file, non_isolates_file, unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df =None) 
-        if read_min_len > 30:
-            genuine_df2, negative_df2, ambiguous_df2, unique_seqs2 = DG.extract_ed2_errors(corrected_file)
-            correct_data = EC.all_in_one_ed2_correction(corrected_file, unique_seqs2, genuine_df2, negative_df2, ambiguous_df2)
-        else:
-            correct_data = corrected_file
-        return correct_data        
-
-    def simulation(self):
-        # step 1 correct errors using noise2read
-        corrected_data = self.error_correction(self.config)
-        # inject errors
-        raw_data, true_data = self.error_injection(corrected_data)
-        # raw_data, true_data = self.error_injection(self.config.input_file)
-        DP = DataProcessing( 
-            self.logger,
-            self.config.num_workers,
-            self.config.result_dir)
-        umi_raw_dataset, umi_true_dataset = DP.write_mimic_umis(raw_data, true_data)
-        return umi_raw_dataset, umi_true_dataset
-        
-    def error_injection(self, data_set):
-        records_dict, file_type = parse_data_dict(data_set)
-        id_lst = list(records_dict.keys())
-
-        total_seqs_lst = []
-        seq2id_dict = {}
-        for item in id_lst:
-            seq = str(records_dict[item].seq)
-            seq2id_dict.setdefault(seq, []).append(item)
-            total_seqs_lst.append(seq)
-            # total_bases += len(seq)
-            # total_reads += 1
-
-        read2counts = collections.Counter(total_seqs_lst)
-        select_id_lst = []
-        total_bases = 0
-        total_reads = 0
-        new_read2counts = {}
-        for read, count in read2counts.items():
-            if count >= 5:
-                select_id_lst.extend(seq2id_dict[read])
-            if count >= self.config.min_read_count:
-                new_read2counts[read] = count
-                
-                total_reads += count
-                total_bases += len(read) * count
+import datetime
 
-        err_reads_num = round(total_bases * self.config.error_rate)
+def custom_logger(root_name, debug_mode) -> logging.Logger: 
+    logger = logging.getLogger(root_name)    
     
-        if total_reads > err_reads_num:
-            per_num =  err_reads_num / total_reads
-        err_id_lst = []
-        for read, count in new_read2counts.items():
-            random_num = round(count * per_num)
-            name_lst = seq2id_dict[read]
-            random.shuffle(name_lst)
-            err_id_lst.extend(random.sample(name_lst, random_num))
-
-        # err_reads_num = round(total_bases * self.config.error_rate / total_reads)
-        self.logger.info(f"total bases: {total_bases}, total reads: {total_reads}, error rate: {self.config.error_rate}, calculated error reads number: {err_reads_num}, actual error reads number: {len(err_id_lst)}")
-
-        err_subdataset = self.config.result_dir + "err_subdataset" + file_type
-        err_records = []
-        shared_objects = records_dict, file_type
-        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-            for tmp_rec in pool.imap(self.mutate_seq, err_id_lst, progress_bar=self.config.verbose):
-                err_records.append(tmp_rec)
-
-        # with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-        #     with tqdm(total=len(err_id_lst), desc=self.logger.info("Generate Mutated Seqs")) as pbar:   
-        #         for tmp_rec in pool.imap(self.mutate_seq, err_id_lst):
-        #             # print(tmp_rec)
-        #             err_records.append(tmp_rec)
-        #             pbar.update() 
-        # print(type(sub_records[0]), sub_records[0])
-        with open(err_subdataset, "w") as handle:
-            SeqIO.write(err_records, handle, file_type)
-        ########################################################################################
-        err_free_subdataset = self.config.result_dir + "err_free_subdataset" + file_type
-
-        err_free_id_lst = list(set(select_id_lst) - set(err_id_lst))
-        extract_records(self.config.result_dir, err_free_id_lst, data_set, err_free_subdataset)
-
-        base = self.config.input_file.split("/")[-1]
-        file_name = base.split(file_type)[0]
-        raw_data = self.config.result_dir + "simulated_raw_" + file_name + file_type
-        os.system("cat %s %s > %s" % (err_subdataset, err_free_subdataset, raw_data))
-        ##################################################################################
-        err_free_subdataset_2 = self.config.result_dir + "err_free_subdataset2" + file_type
-        extract_records(self.config.result_dir, err_id_lst, data_set, err_free_subdataset_2)
-        true_data = self.config.result_dir + "simulated_true_" + file_name + file_type  
-        os.system("cat %s %s > %s" % (err_free_subdataset_2, err_free_subdataset, true_data))     
-        return raw_data, true_data
-
-    def mutate_seq(self, shared_objects, idx):
-        records_dict, file_type = shared_objects
-        ori_seq = str(records_dict[idx].seq)
-        mutation_seq = self.read2err_read(ori_seq)
-        if file_type == "fastq":
-            return SeqRecord(Seq(mutation_seq), id=records_dict[idx].id, description=records_dict[idx].description, letter_annotations=records_dict[idx].letter_annotations)
-        elif file_type == "fasta":
-            return SeqRecord(Seq(mutation_seq).seq, id=records_dict[idx].id, description=records_dict[idx].description)           
+    formatter = ColoredFormatter(
+        "%(green)s[%(asctime)s] %(blue)s%(name)s %(log_color)s%(levelname)-8s%(reset)s %(message)s",
+        datefmt=None,
+        reset=True,
+        log_colors={
+            'DEBUG':    'cyan',
+            'INFO':     'green',
+            'WARNING':  'yellow',
+            'ERROR':    'red',
+            'CRITICAL': 'red, bg_white',
+        },
+        secondary_log_colors={},
+        style='%'
+    )
+    if debug_mode:
+        logger.setLevel(logging.DEBUG)
+    else:
+        logger.setLevel(logging.INFO)
+    stream_handler = logging.StreamHandler()
+    stream_handler.setFormatter(formatter)
+    logger.addHandler(stream_handler)
+    
+    # Output full log
+    file_handler = logging.FileHandler( datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_") + 'noise2read.log')
+
+    file_handler.setLevel(logging.INFO)
+
+    # formatter = logging.Formatter(log_format)
+    logger.addHandler(file_handler)
+
+    # # Output warning log
+    # file_handler = logging.FileHandler('noise2read.Warning.log')
+    # file_handler.setLevel(logging.WARNING)
+    # # formatter = logging.Formatter(log_format)
+    # file_handler.setFormatter(formatter)
+    # logger.addHandler(file_handler)
+
+    # # Output error log
+    # file_handler = logging.FileHandler('noise2read.Error.log')
+    # file_handler.setLevel(logging.ERROR)
+    # # formatter = logging.Formatter(log_format)
+    # file_handler.setFormatter(formatter)
+    # logger.addHandler(file_handler)
+
+    return logger
+
+def parse_file_type(data_set):
+    items = data_set.split(".")
+    ext = items[-1]
+    if ext == 'fa' or ext == 'fasta':
+        f_type = 'fasta'
+    elif ext == 'fq' or ext == 'fastq':
+        f_type = 'fastq'
+    elif ext == 'gz':
+        f_type = items[-2] + '.' + ext
+    return f_type
+
+def parse_data(data_set):
+    file_type = parse_file_type(data_set)
+    if file_type == 'fastq.gz' or file_type == 'fq.gz' or file_type == 'fa.gz' or file_type == 'fasta.gz':
+        ff_type = file_type.split('.')[0]
+        handle = gzip.open(data_set, 'rt')
+        record_iterator = SeqIO.parse(handle, ff_type)
+        return record_iterator, ff_type
+    else:
+        record_iterator = SeqIO.parse(data_set, file_type) 
+        return record_iterator, file_type
+
+def parse_data_index(data_set):
+    file_type = parse_file_type(data_set)
+    if file_type == 'fastq.gz' or file_type == 'fq.gz' or file_type == 'fa.gz' or file_type == 'fasta.gz':
+        ff_type = file_type.split('.')[0]
+        handle = gzip.open(data_set, 'rt')
+        records = SeqIO.index(handle, ff_type)
+        return records, ff_type
+    else:
+        records = SeqIO.index(data_set, file_type)     
+        return records, file_type
+
+def parse_data_dict(data_set):
+    file_type = parse_file_type(data_set)
+    if file_type == 'fastq.gz' or file_type == 'fq.gz' or file_type == 'fa.gz' or file_type == 'fasta.gz':
+        ff_type = file_type.split('.')[0]
+        handle = gzip.open(data_set, 'rt')
+        records_dict = SeqIO.to_dict(SeqIO.parse(handle, ff_type))
+        return records_dict, ff_type
+    else:
+        records_dict = SeqIO.to_dict(SeqIO.parse(data_set, file_type))   
+        return records_dict, file_type
+'''
+def extract_seq(shared_objects, name):
+    records_dict, file_type = shared_objects
+    if file_type == "fastq":
+        return SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description, letter_annotations=records_dict[name].letter_annotations)
+    elif file_type == "fasta":
+        return SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description)
+
+def extract_seqs(num_workers, name_lst, data_set, sub_dataset, logger):
+    records_dict, file_type = parse_data_dict(data_set)
+    sub_records = []
+    shared_objects = records_dict, file_type
+    with WorkerPool(num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+        with tqdm(total=len(name_lst), desc=logger.info("Extract Seqs")) as pbar:   
+            for tmp_rec in pool.imap(extract_seq, name_lst):
+                # print(tmp_rec)
+                sub_records.append(tmp_rec)
+                pbar.update() 
+    # print(type(sub_records[0]), sub_records[0])
+    with open(sub_dataset, "w") as handle:
+        SeqIO.write(sub_records, handle, file_type)
+    return 
+'''
+def extract_records(working_dir, name_lst, data_set, sub_dataset):
+    f_name_lst = os.path.join(working_dir, 'tmp_name.lst')
+    with open(f_name_lst, "w") as outfile:
+        outfile.write("\n".join(name_lst))
+    os.system("seqtk subseq %s %s > %s" % (data_set, f_name_lst, sub_dataset))
+    os.system("rm %s" % f_name_lst)
+    # record_iterator, file_type = parse_data(data_set)
+    # records = [rec for rec in record_iterator if str(rec.id) in name_lst]
+    # SeqIO.write(records, sub_dataset, file_type)
+    return
+#####################################################################################
+def sub_base(base):
+    if base == 'A':
+        return 'TCG'
+    elif base == 'T':
+        return 'ACG'
+    elif base == 'C':
+        return 'ATG'
+    elif base == 'G':
+        return 'ACT'
+    elif base == 'N':
+        return 'N'
+
+def replace_char(seq, char, index):
+    seq[index] = char
+    return ''.join(seq)
+
+def seq2substitution(read):
+    """
+    enumerate all the substitutions for one read 
+    Args:
+        read (str): a sequence
+    Returns:
+        set: a set contains reads
+    """
+    editdis1_list = []
+    # substitution
+    raw_seq = list(read)
+    n = len(raw_seq)
+    for i in range(n):
+        seq = copy.deepcopy(raw_seq)
+        temp_base = seq[i]
+        #print(temp_base)
+        temp_sub_base = list(sub_base(temp_base))
+        #print(temp_sub_base)
+        for b in temp_sub_base:
+            if b != 'N':
+                sub_seq = replace_char(seq, b, i)
+                editdis1_list.append(sub_seq)
+    return set(editdis1_list)
+
+def seq2deletion(read):
+    """
+    enumerate all the deletions for one read 
+    Args:
+        read (str): a sequence
+    Returns:
+        set: a set contains reads
+    """
+    editdis1_list = []
+    seq = list(read)
+    n = len(seq)
+    # deletion
+    for i in range(n):
+        del_seq = read[:i] + read[(i+1):]
+        editdis1_list.append(del_seq)
+    return set(editdis1_list)
+
+def seq2insertion(read):
+    """
+    enumerate all the insertions for one read 
+    Args:
+        read (str): a sequence
+    Returns:
+        set: a set contains reads
+    """
+    editdis1_list = []
+    seq = list(read)
+    n = len(seq)
+    # insertion
+    bases = ['A', 'G', 'C', 'T']
+    for i in range(n+1):
+        for b in bases:
+            raw_seq = copy.deepcopy(seq)
+            raw_seq.insert(i, b)
+            editdis1_list.append(''.join(raw_seq))
+    return set(editdis1_list)
+
+def enumerate_ed1_seqs(read):
+    possible_ed1 = []
+    possible_ed1.extend(seq2deletion(read))
+    possible_ed1.extend(seq2substitution(read))
+    possible_ed1.extend(seq2insertion(read))
+    return set(possible_ed1)
+
+def enumerate_ed2_seqs(read):
+    # possible_ed1 = self.enumerate_ed1_seqs(read)
+    possible_ed1 = seq2substitution(read)
+    possible_ed2 = []
+    for seq in possible_ed1:
+        possible_ed2.extend(list(set(seq2substitution(seq)) - possible_ed1))
+    return set(possible_ed2)
+    
+def random_ed2_seq(read, total_reads, num):
     '''
-    def extract_seq(self, shared_objects, name):
-        records_dict, file_type = shared_objects
-        if file_type == "fastq":
-            return SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description, letter_annotations=records_dict[name].letter_annotations)
-        elif file_type == "fasta":
-            return SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description)
-
-    def extract_seqs(self, num_workers, name_lst, data_set, sub_dataset):
-        records_dict, file_type = self.parse_data_dict(data_set)
-        sub_records = []
-        shared_objects = records_dict, file_type
-        with WorkerPool(num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-            with tqdm(total=len(name_lst), desc=self.logger.info("Extract Seqs")) as pbar:   
-                for tmp_rec in pool.imap(self.extract_seq, name_lst):
-                    # print(tmp_rec)
-                    sub_records.append(tmp_rec)
-                    pbar.update() 
-        # print(type(sub_records[0]), sub_records[0])
-        with open(sub_dataset, "w") as handle:
-            SeqIO.write(sub_records, handle, file_type)
-        return 
+    return num reads that each have two bases difference from given read and these generated reads not exist in total_reads
     '''
+    editdis2_list = []
+    # substitution
+    raw_seq = list(read)
+    n = len(raw_seq)
+    pos_lst = []
+    for i in range(num):
+        pos_lst.append(random.sample(range(n), 2))
+    for item in pos_lst:
+        seq = copy.deepcopy(raw_seq)
+        i = item[0]
+        j = item[1]
+        i_base = seq[i]
+        j_base = seq[j]
+        i_sub_base = random.sample(list(sub_base(i_base)), 1)[0]    
+        j_sub_base = random.sample(list(sub_base(j_base)), 1)[0]  
+        sub_seq = replace_char(seq, i_sub_base, i)
+        sub_seq = replace_char(seq, j_sub_base, j)
+        if sub_seq not in total_reads:
+            editdis2_list.append(sub_seq)
+    return editdis2_list
+
+def error_type_classification(read1, read2):
+    f_len = len(read1)
+    s_len = len(read2)  
+    # position = -1  
+    dis = editdistance.eval(read1, read2)
+    # print(dis)
+    if dis == 1:              
+        if f_len == s_len:
+            position = -1
+            for index in range(f_len):
+                if read1[index] == read2[index]:
+                    continue
+                else:
+                    position = index
+                    # first = f_seq[index]
+                    # second = s_seq[index]
+                    break
+            first = read1[position]
+            second = read2[position]
+            if position == 0:
+                f_kmer = read1[0:2]
+                s_kmer = read2[0:2]
+            elif position == f_len:
+                f_kmer = read1[-2:] 
+                s_kmer = read2[-2:]
+            else:
+                f_kmer = read1[position-1 : position+2]
+                s_kmer = read2[position-1 : position+2]  
+
+        elif f_len < s_len:
+            position = -1
+            num = 0
+            for index in range(f_len):
+                if read1[index] == read2[index]:
+                    num = num + 1
+                else:
+                    position = index
+                    break
+            if num == f_len:
+                position = f_len
+            first = 'X'
+            second = read2[position]  
+            if position == 0:
+                f_kmer = 'X' + read1[0]
+                s_kmer = read2[0:2]
+            elif position == f_len:
+                f_kmer = read1[-1] + 'X'
+                s_kmer = read2[-2:]
+            else:
+                f_kmer = read1[position-1] + 'X' + read1[position]
+                s_kmer = read2[position-1 : position+2]                    
+        elif f_len > s_len:
+            position = -1
+            num = 0
+            for index in range(s_len):
+                if read1[index] == read2[index]:
+                    num = num + 1
+                else:
+                    position = index
+                    break
+            if num == s_len:
+                position = s_len
+            first = read1[position]
+            second = 'X'
+            if position == 0:
+                f_kmer = read1[0:2]
+                s_kmer = 'X' + read2[0]
+            elif position == s_len:
+                f_kmer = read1[-2:] 
+                s_kmer = read2[-1] + 'X'
+            else:
+                f_kmer = read1[position-1 : position+2]
+                s_kmer = read2[position-1] + 'X' + read2[position]    
+
+        errorType = first + '-' + second
+    
+        return [errorType, f_kmer, s_kmer]
+    else:
+        raise ValueError("The editdistance of two reads in the input list must equal to one!")
+
+def usage():
+    # print(" ")
+    print("noise2read Usage:")
+    print("   Mandatory:")
+    print("     -m|--module                   module selection")
+    print("   Modules: [correction, amplicon_correction, umi_correction, mimic_umi, real_umi, evaluation, simulation]")
+    # print(" ")
+    print("1. Using config file")
+    print("     noise2read -m|--module <module_name> -c <path_configuration_file>")
+    print("   Mandatory:")
+    print("     -c|--config                   input configuration file")
+    # print(" ")
+    print("2. Using command line with the default parameters")
+    print("     noise2read -m|--module <module_name> -i <path_raw_data.fastq|fasta|fa|fq>")
+    print("   Mandatory:")
+    print("     -i|--input                    input raw data to be corrected")
+    print("   Options:")
+    print("     -d|--directory                set output directory")
+    print("     -a|--high_ambiguous           predict high ambiguous errors using machine learning when set true, defaut true")
+    print("     -t|--true                     input ground truth data if you have")
+    print("     -r|--rectification            input corrected data when using module evaluation")
+    print("     -p|--parallel                 use multiple cpu cores, default total cpu cores - 2")
+    print("     -g|--tree_method              use gpu for training and prediction, default auto, (options gpu_hist, hist, auto)")
+    # print("     -o|--over_sampling            use over sampling or downsampling for negative samples, default True")
+    print("     -h|--help                     show this help")
+    # print("########################################################################################################################")
+
+#####################################################################################
+# def split_seqs(num_workers, name_set, data_set, sub_dataset_1, sub_dataset_2):
+#     records_dict, file_type = parse_data_dict(data_set)
+#     sub_records_1 = []
+#     sub_records_2 = []
+#     shared_objects = records_dict, file_type
+
+#     with WorkerPool(num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+#         with tqdm(total=len(name_lst), desc="Extract Seqs") as pbar:   
+#             for tmp_rec in pool.imap(extract_seq, name_lst):
+#                 # print(tmp_rec)
+#                 sub_records.append(tmp_rec)
+#                 pbar.update() 
+
+#     for item in record_iterator:
+#         qual = {}
+#         name = item.id
+#         if file_type == "fastq":
+#             qual['phred_quality'] = item.letter_annotations['phred_quality']
+#             tmp_rec = SeqRecord(item.seq, id=name, description=item.description, letter_annotations=qual) 
+#         elif file_type == "fasta":
+#             tmp_rec = SeqRecord(item.seq, id=name, description=item.description)    
+#         if name in name_set:             
+#             sub_records_1.append(tmp_rec)
+#         elif name in non_name_set:                        
+#             sub_records_2.append(tmp_rec)
+#     with open(sub_dataset_1, "w") as handle:
+#         SeqIO.write(sub_records_1, handle, file_type)
+#     with open(sub_dataset_2, "w") as handle:
+#         SeqIO.write(sub_records_2, handle, file_type)
+#     return 
+
+if __name__ == "__main__":
+    # input_file = '/home/pping/Data/Repo/data/noise2read_data/group1/raw/new_tcr.seq.real_SRR1543964.fastq'
     
-# if __name__ == '__main__':
-#     logger = custom_logger("simulation", debug_mode=True)
-#     input_file = "/home/pping/Data/Repo/data/noise2read_data/group3/SAS-Cov-2/noise2read_result/new_no_ml/output/umi_simulated_raw_original_sars_r1_corrected_correct.fastq"
-#     sim = Simulation(logger, 30, )
-
-#     raw_data, true_data = sim.error_injection(input_file)
-#     output_dir = "/home/pping/Data/Repo/data/noise2read_data/group3/SAS-Cov-2/"
-#     DP = DataProcessing( 
-#         logger,
-#         num_workers=30,
-#         output_dir=output_dir)
-#     umi_raw_dataset, umi_true_dataset = DP.write_mimic_umis(raw_data, true_data)
+    # records_dict, file_type = parse_data_dict(input_file)
+    # sub_records = []
+    # for name in records_dict:
+    #     if file_type == "fastq":
+    #         # qual = {}
+    #         # qual['phred_quality'] = records[name].letter_annotations["phred_quality"]
+    #         tmp_rec = SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description, letter_annotations=records_dict[name].letter_annotations) 
+    #         print(type(records_dict[name].seq))
+    #         print(type(records_dict[name].id))
+    #         print(type(records_dict[name].description))
+    #         print(type(records_dict[name].letter_annotations))
+    #     elif file_type == "fasta":
+    #         tmp_rec = SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description)      
+    #         print(records_dict[name].seq, records_dict[name].id)
+    #     break
+    num = 3
+    total_reads = ['AACGT', 'GACGT', 'CACGT', 'TACGT', 'AACGT', 'AGCGT','ACCGT', 'ATCGT', 'ACAGT', 'ACGGT', 'ACCGT', 'ACTGT', 'ACGAT']
+    read = 'AACGT'
+    seqs = random_ed2_seq(read, total_reads, num)
+    print(seqs)
```

### Comparing `noise2read-0.0.76/src/noise2read/umitest.py` & `noise2read-0.0.81/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.0.81/src/noise2read.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.76
+Version: 0.0.81
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.76/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.81/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/tests/test_data_generation.py` & `noise2read-0.0.81/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/tests/test_reads2vector.py` & `noise2read-0.0.81/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.76/tests/test_utils.py` & `noise2read-0.0.81/tests/test_utils.py`

 * *Files identical despite different names*

