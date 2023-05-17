# Comparing `tmp/deepBreaks-1.0.2.tar.gz` & `tmp/deepBreaks-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepBreaks-1.0.2.tar", last modified: Mon May 15 20:20:24 2023, max compression
+gzip compressed data, was "deepBreaks-1.1.0.tar", last modified: Wed May 17 20:37:36 2023, max compression
```

## Comparing `deepBreaks-1.0.2.tar` & `deepBreaks-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 20:20:24.051900 deepBreaks-1.0.2/
--rw-r--r--   0 root         (0) staff       (20)     1084 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/LICENSE.txt
--rw-r--r--   0 root         (0) staff       (20)    22640 2023-05-15 20:20:24.051665 deepBreaks-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    21765 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 20:20:24.049931 deepBreaks-1.0.2/deepBreaks/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9980 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/deepBreaks.py
--rw-r--r--   0 root         (0) staff       (20)    11921 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/models.py
--rw-r--r--   0 root         (0) staff       (20)    17472 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/preprocessing.py
--rw-r--r--   0 root         (0) staff       (20)    18237 2023-05-01 19:14:30.000000 deepBreaks-1.0.2/deepBreaks/visualization.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 20:20:24.051392 deepBreaks-1.0.2/deepBreaks.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    22640 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      394 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       58 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)      145 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2023-05-15 20:20:23.000000 deepBreaks-1.0.2/deepBreaks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-15 20:20:24.051972 deepBreaks-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     3001 2023-05-15 20:18:53.000000 deepBreaks-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-17 20:37:36.221151 deepBreaks-1.1.0/
+-rw-r--r--   0 root         (0) staff       (20)     1084 2022-05-16 04:21:29.000000 deepBreaks-1.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) staff       (20)    23668 2023-05-17 20:37:36.220895 deepBreaks-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    22793 2023-05-17 20:34:59.000000 deepBreaks-1.1.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-17 20:37:36.218988 deepBreaks-1.1.0/deepBreaks/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-05-16 04:21:29.000000 deepBreaks-1.1.0/deepBreaks/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    11892 2023-05-15 21:01:55.000000 deepBreaks-1.1.0/deepBreaks/deepBreaks.py
+-rw-r--r--   0 root         (0) staff       (20)    18235 2023-05-15 21:01:55.000000 deepBreaks-1.1.0/deepBreaks/models.py
+-rw-r--r--   0 root         (0) staff       (20)    23642 2023-05-04 15:17:40.000000 deepBreaks-1.1.0/deepBreaks/preprocessing.py
+-rw-r--r--   0 root         (0) staff       (20)    12522 2023-05-16 13:37:21.000000 deepBreaks-1.1.0/deepBreaks/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    12937 2023-05-15 21:01:55.000000 deepBreaks-1.1.0/deepBreaks/visualization.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-17 20:37:36.220576 deepBreaks-1.1.0/deepBreaks.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    23668 2023-05-17 20:37:36.000000 deepBreaks-1.1.0/deepBreaks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      431 2023-05-17 20:37:36.000000 deepBreaks-1.1.0/deepBreaks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-17 20:37:36.000000 deepBreaks-1.1.0/deepBreaks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       58 2023-05-17 20:37:36.000000 deepBreaks-1.1.0/deepBreaks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-16 13:45:54.000000 deepBreaks-1.1.0/deepBreaks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)      160 2023-05-17 20:37:36.000000 deepBreaks-1.1.0/deepBreaks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2023-05-17 20:37:36.000000 deepBreaks-1.1.0/deepBreaks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      159 2023-05-16 19:22:38.000000 deepBreaks-1.1.0/requirements.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-17 20:37:36.221223 deepBreaks-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3046 2023-05-16 19:23:46.000000 deepBreaks-1.1.0/setup.py
```

### Comparing `deepBreaks-1.0.2/LICENSE.txt` & `deepBreaks-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepBreaks-1.0.2/PKG-INFO` & `deepBreaks-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: deepBreaks
-Version: 1.0.2
-Summary: deepBreaks: a machine learning tool for identifying and prioritizing genotype-phenotype associations
-Home-page: http://github.com/omicsEye/deepBreaks
-Author: Mahdi Baghbanzadeh
-Author-email: mbagh@gwu.edu
-License: MIT
-Keywords: machine learning,genomics,sequencing data
-Platform: Linux
-Platform: MacOS
-Platform: Windows
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # deepBreaks #
 ![](https://github.com/omicsEye/deepbreaks/blob/master/img/fig1_overview.png?raw=True)
 ---
 
 ***deepBreaks*** , a computational method, aims to identify important
 changes in association with the phenotype of interest
 using multi-alignment sequencing data from a population.
@@ -151,15 +127,15 @@
   ```
 7) Activate the conda environment
   ```commandline
   conda activate deepBreaks_env
   ```
 8) Install packages from Conda
   ```commandline
-  conda install lightgbm
+  conda install -c conda-forge lightgbm
   pip install xgboost
   ```
 9) Finally, install *deepBreaks*:
 install with pip:
 ```commandline
 pip install deepBreaks
 ```
@@ -175,96 +151,82 @@
 
 To test if deepBreaks is installed correctly, you may run the following command in the terminal:
 
 ```#!cmd
 deepBreaks -h
 ```
 Which yields deepBreaks command line options.
+
+
+
+## Options ##
+
+```
+$ deepBreaks -h
+```
+## Input ##
 ```commandline
-usage: deepBreaks [-h] --seqfile SEQFILE --seqtype SEQTYPE --meta_data META_DATA --metavar
-                  METAVAR [--gap GAP] --anatype {reg,cl}
+usage: deepBreaks [-h] --seqfile SEQFILE --seqtype SEQTYPE --meta_data META_DATA --metavar METAVAR [--gap GAP] [--miss_gap MISS_GAP]
+                  [--ult_rare ULT_RARE] --anatype {reg,cl}
                   [--distance_metric {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}]
-                  [--fraction FRACTION] [--redundant_threshold REDUNDANT_THRESHOLD]
-                  [--distance_threshold DISTANCE_THRESHOLD] [--top_models TOP_MODELS] [--plot]
-                  [--write]
+                  [--fraction FRACTION] [--redundant_threshold REDUNDANT_THRESHOLD] [--distance_threshold DISTANCE_THRESHOLD]
+                  [--top_models TOP_MODELS] [--cv CV] [--separate_cv] [--tune] [--plot] [--write]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --seqfile SEQFILE, -sf SEQFILE
                         files contains the sequences
   --seqtype SEQTYPE, -st SEQTYPE
                         type of sequence: 'nu' for nucleotides or 'aa' for amino-acid
   --meta_data META_DATA, -md META_DATA
                         files contains the meta data
   --metavar METAVAR, -mv METAVAR
                         name of the meta var (response variable)
-  --gap GAP, -gp GAP    Threshold to drop positions that have GAPs above this proportion.
-                        Default value is 0.7 and it means that the positions that 70% or more
-                        GAPs will be dropped from the analysis.
+  --gap GAP, -gp GAP    Threshold to drop positions that have GAPs above this proportion. Default value is 0.7 and it means that the positions that
+                        70% or more GAPs will be dropped from the analysis.
+  --miss_gap MISS_GAP, -mgp MISS_GAP
+                        Threshold to impute missing values with GAP. Gapsin positions that have missing values (gaps) above this proportionare
+                        replaced with the term 'GAP'. the rest of the missing valuesare replaced by the mode of each position.
+  --ult_rare ULT_RARE, -u ULT_RARE
+                        Threshold to modify the ultra rare cases in each position.
   --anatype {reg,cl}, -a {reg,cl}
                         type of analysis
   --distance_metric {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}, -dm {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}
                         distance metric. Default is correlation.
   --fraction FRACTION, -fr FRACTION
                         fraction of main data to run
   --redundant_threshold REDUNDANT_THRESHOLD, -rt REDUNDANT_THRESHOLD
-                        threshold for the p-value of the statistical tests to drop redundant
-                        features. Defaultvalue is 0.25
+                        threshold for the p-value of the statistical tests to drop redundant features. Defaultvalue is 0.25
   --distance_threshold DISTANCE_THRESHOLD, -dth DISTANCE_THRESHOLD
-                        threshold for the distance between positions to put them in clusters.
-                        features with distances <= than the threshold will be grouped together.
-                        Default values is 0.3
+                        threshold for the distance between positions to put them in clusters. features with distances <= than the threshold will be
+                        grouped together. Default values is 0.3
   --top_models TOP_MODELS, -tm TOP_MODELS
-                        number of top models to consider for merging the results. Default value
-                        is 5
-  --plot                plot all the individual positions that are statistically
-                        significant.Depending on your data, this process may produce many
+                        number of top models to consider for merging the results. Default value is 5
+  --cv CV, -cv CV       number of folds for cross validation. Default is 10. If the given number is less than 1,
+                        then instead of CV, a train/test split approach will be used with --cv being the test size. 
+  
+  --tune                After running the 10-fold cross validations, should the top selected models be tuned and finalize, or finalized only?
+  --plot                plot all the individual positions that are statistically significant.Depending on your data, this process may produce many
                         plots.
-  --write               During reading the fasta file we delete the positions that have GAPs
-                        over a certain threshold that can be changed in the `gap_threshold`
-                        argumentin the `read_data` function. As this may change the whole FASTA
-                        file, you maywant to save the FASTA file after this cleaning step.
-```
-
-
-## Options ##
+  --write               During reading the fasta file we delete the positions that have GAPs over a certain threshold that can be changed in the
+                        `gap_threshold` argumentin the `read_data` function. As this may change the whole FASTA file, you maywant to save the FASTA
+                        file after this cleaning step.
 
 ```
-$ deepBreaks -h
-```
-## Input ##
-1. `--seqfile` or `-sf` PATH to a sequence data file
-2. `--seqtype` or `-st` sequence type, values are `amino-acid` and `nu` for nucleotides
-3. `--meta_data` or `-md` PATH to metadata file
-4. `--metavar` or `-mv` name of the meta variable
-5. `--anatype` or `-a` analysis type, options are `reg` for regression and `cl` for classification
-6. `--fraction` or `-fr` fraction of the main data (sequence positions) to run. it is optional, 
-but you can enter a value between 0 and 1 to sample from the main data set.
-7. `--redundant_threshold` or `-rt` threshold for the p-value of the statistical 
-tests to drop redundant features. Default value is 0.25.
-8. `--distance_threshold` or `-dth` threshold for the distance between positions to put them in clusters. 
-features with distances <= than the threshold will be grouped together. Default values is 0.3.
-9. `--top_models` or `-tm` number of top models to consider for merging the results. Default value is 3
-10. `--plot` plot all the individual positions that are statistically significant. 
-Depending on your data, this process may produce many plots.
-11. `--gap` or `-gp` Threshold to drop positions that have GAPs above this proportion. 
-Default value is 0.7, and it means that the positions that 70% or more GAPs will be dropped from the analysis.
-12. `--write` During reading the fasta file we delete the positions that have GAPs over a  certain threshold that can 
-be changed in the `gap_threshold` argument in the `read_data` function. As this may change the whole FASTA file,
-you may want to save the FASTA file after this cleaning step.
 
 ## Output ##  
 1. correlated positions. We group all the colinear positions together.
 2. models summary. list of models and their performance metrics.
 3. plot of the feature importance of the top models in *modelName_dpi.png* format.
 4. csv files of feature importance based on top models containing, feature, importance, relative importance, 
 group of the position (we group all the colinear positions together)
 5. plots and csv file of average of feature importance of top models.
 6. box plot (regression) or stacked bar plot (classification) for top positions of each model.
-7. pickle files of the plots
+7. pickle files of the plots and final models
+8. p-values of all the variables used in training of the final model
 
 ## Demo ##
 ```commandline
 deepBreaks -sf PATH_TO_SEQUENCE.FASTA -st aa -md PATH_TO_META_DATA.tsv -mv
  META_VARIABLE_NAME -a reg  -dth 0.15 --plot --write
 ```
 
@@ -327,97 +289,110 @@
 To get the ful list of available metrics, you can use:
 ```python
 from sklearn import metrics
 print(metrics.SCORERS.keys())
 ```
 The default search parameters for the models are:
 ```python
+import numpy as np
 params = {
-        'rf': {
-            'max_depth': [4, 6, 8],
-            'n_estimators': [500, 1000]
-        },
-        'Adaboost': {
-            'learning_rate': [0.01, 0.05],
-            'n_estimators': [50, 100]
-        },
-        'et': {
-            'max_depth': [4, 6, 8],
-            'n_estimators': [500, 1000]
-        },
-        'dt': {
-            'max_depth': [4, 6, 8]
-        },
-        'Lasso': {
-            'alpha': [0.5, 1, 3]
-        },
-        'LassoLars': {
-            'alpha': [0.5, 1, 3]
-        }
+        'rf': {'rf__max_features': ["sqrt", "log2"]},
+        'Adaboost': {'Adaboost__learning_rate': np.linspace(0.001, 0.1, num=2),
+                     'Adaboost__n_estimators': [100, 200]},
+        'gbc': {'gbc__max_depth': range(3, 6),
+                'gbc__max_features': ['sqrt', 'log2'],
+                'gbc__n_estimators': [200, 500, 800],
+                'gbc__learning_rate': np.linspace(0.001, 0.1, num=2)},
+        'et': {'et__max_depth': [4, 6, 8],
+               'et__n_estimators': [500, 1000]},
+        'dt': {'dt__max_depth': [4, 6, 8]},
+        'Lasso': {'Lasso__alpha': np.linspace(0.01, 100, num=5)},
+        'LassoLars': {'LassoLars__alpha': np.linspace(0.01, 100, num=5)}
     }
 ```
 **Attention:** The names of models in the provided `dict` are the same with the names in the `dict` provided 
 for the `params`. If the name from the models `dict` does not match, the default `sklearn` parameters for that model
-is then used.  For example, `model_compare` uses the `xgboost` with default hyperparameters.  
+is then used.  For example, `model_compare_cv` uses the `xgboost` with default hyperparameters.  
 
-To use the `deepBreaks.models.model_compare` function with default parameters:
+To use the `deepBreaks.models.model_compare_cv` function with default parameters:
 ```python
-import deepBreaks.models as ml
+from deepBreaks.models import model_compare_cv
+from deepBreaks.preprocessing import MisCare, ConstantCare, URareCare, CustomOneHotEncoder
+from deepBreaks.preprocessing import FeatureSelection, CollinearCare
+from deepBreaks.utils import get_models, get_scores, get_params, make_pipeline
+
 ana_type = 'reg'  # assume that we are running a regression analysis
-trained_models = ml.model_compare(X_train, y_train, ana_type,
-                  cv=10, select_top=5,
-                  models=None, scores=None,
-                  params=None, sort_by=None,
-                  n_positions=None,
-                  grouped_features=None,
-                  report_dir='.')
+report_dir = 'PATH/TO/A/DIRECTORY' # to save the reports
+prep_pipeline = make_pipeline(cache_dir=None,
+    steps=[
+        ('mc', MisCare(missing_threshold=0.25)),
+        ('cc', ConstantCare()),
+        ('ur', URareCare(threshold=0.05)),
+        ('cc2', ConstantCare()),
+        ('one_hot', CustomOneHotEncoder()),
+        ('feature_selection', FeatureSelection(model_type=ana_type, alpha=0.25)),
+        ('collinear_care', CollinearCare(dist_method='correlation', threshold=0.25))
+    ])
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=get_models(ana_type=ana_type),
+                               scoring=get_scores(ana_type=ana_type),
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
+
 ```
 To use a new set of `models`, `params`, or `metrics` you can define them in a `dict`:
 ```python
 import deepBreaks.models as ml
 from sklearn.ensemble import RandomForestRegressor, AdaBoostRegressor
 from sklearn.ensemble import ExtraTreesRegressor
-        
-ana_type = 'reg'  # assume that we are running a regression analysis
+from deepBreaks.models import model_compare_cv
+from deepBreaks.preprocessing import MisCare, ConstantCare, URareCare, CustomOneHotEncoder
+from deepBreaks.preprocessing import FeatureSelection, CollinearCare
+from deepBreaks.utils import get_models, get_scores, get_params, make_pipeline
 
+ana_type = 'reg'  # assume that we are running a regression analysis
+report_dir = 'PATH/TO/A/DIRECTORY' # to save the reports
 # define a new set of models
 models = {'rf': RandomForestRegressor(n_jobs=-1, random_state=123),
           'Adaboost': AdaBoostRegressor(random_state=123),
           'et': ExtraTreesRegressor(n_jobs=-1, random_state=123)
           }
 
-# define a new set of params.
-params = {
-        'rf': {
-            'max_depth': [3, 5],
-            'n_estimators': [100]
-        },
-        'Adaboost': {
-            'learning_rate': [0.01, 0.05, 0.1],
-            'n_estimators': [50]
-        }
-    }
+
+prep_pipeline = make_pipeline(cache_dir=None,
+    steps=[
+        ('mc', MisCare(missing_threshold=0.25)),
+        ('cc', ConstantCare()),
+        ('ur', URareCare(threshold=0.05)),
+        ('cc2', ConstantCare()),
+        ('one_hot', CustomOneHotEncoder()),
+        ('feature_selection', FeatureSelection(model_type=ana_type, alpha=0.25)),
+        ('collinear_care', CollinearCare(dist_method='correlation', threshold=0.25))
+    ])
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=models,
+                               scoring=get_scores(ana_type=ana_type),
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
 
 '''
 Since we do not define a set of parameters for the model "et", it will fit with
 default parameters
 '''
 # change the set of metrics
 scores = {'R2': 'r2',
           'MAE': 'neg_mean_absolute_error',
           'MSE': 'neg_mean_squared_error'
           }
 
-trained_models = ml.model_compare(X_train, y_train, ana_type,
-                  cv=10, select_top=5,
-                  models=models, scores=scores,
-                  params=params, sort_by='MAE', # sort the models by "MAE" values
-                  n_positions=None,
-                  grouped_features=None,
-                  report_dir='.')
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=models,
+                               scoring=scores,
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
 ```
 
 # Applications #
 Here we try to use the **_deepBreaks_** on different datasets and elaborate on the results.
 
 <h2 id="opsin">
 <i>deepBreaks</i> identifies amino acids associated with color sensitivity
@@ -430,30 +405,30 @@
 amino acid sequence of rod opsins because previously published mutagenesis work established mechanistic connections
 between 12 specific amino acid sites and phenotypes [Yokoyama et al. (2008)](https://doi.org/10.1073/pnas.0802426105). 
 Therefore, we hypothesized that machine learning approaches could predict known associations between amino acid sites 
 and absorbance phenotypes. We identified opsins expressed in
 rod cells of vertebrates (mainly marine fishes) with absorption spectra measurements (λmax, the wavelength with the
 highest absorption). The dataset contains 175 samples of opsin sequences. We next applied deepBreaks on this
 dataset to find the most important sites contributing to the variations of λmax. 
-This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/continuous_phenotype.ipynb) 
+This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/continuous_phenotype_light_sensitivity.ipynb) 
 illustrates the steps.
 
 
 <h2 id="hmp">
 Novel insights of niche associations in the oral microbiome
 </h2>
 
 ![hmp](https://github.com/omicsEye/deepbreaks/blob/master/img/hmp/hmp.png?raw=True)  
 Microbial species tend to adapt at the genome level to the niche in which they live. We hypothesize 
 that genes with essential functions change based on where microbial species live. Here we use microbial strain 
 representatives from stool metagenomics data of healthy adults from the
 [Human Microbiome Project](https://doi.org/10.1038/nature11234). The input for deepBreaks consists of 1) an MSA file
 with 1006 rows, each a representative strain of a specific microbial species, here Haemophilus parainfluenzae, with
 49839 lengths; and 2) labels for deepBreaks prediction are body sites from which samples were collected. 
-This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype.ipynb)
+This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype_HMP.ipynb)
 illustrates the steps.
 
 
 <h2 id="covid">
 <i>deepBreaks</i> reveals important SARS-CoV-2 regions associated with Alpha and Delta variants
 </h2>
```

### Comparing `deepBreaks-1.0.2/README.md` & `deepBreaks-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: deepBreaks
+Version: 1.1.0
+Summary: deepBreaks: a machine learning tool for identifying and prioritizing genotype-phenotype associations
+Home-page: http://github.com/omicsEye/deepBreaks
+Author: Mahdi Baghbanzadeh
+Author-email: mbagh@gwu.edu
+License: MIT
+Keywords: machine learning,genomics,sequencing data
+Platform: Linux
+Platform: MacOS
+Platform: Windows
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # deepBreaks #
 ![](https://github.com/omicsEye/deepbreaks/blob/master/img/fig1_overview.png?raw=True)
 ---
 
 ***deepBreaks*** , a computational method, aims to identify important
 changes in association with the phenotype of interest
 using multi-alignment sequencing data from a population.
@@ -127,15 +151,15 @@
   ```
 7) Activate the conda environment
   ```commandline
   conda activate deepBreaks_env
   ```
 8) Install packages from Conda
   ```commandline
-  conda install lightgbm
+  conda install -c conda-forge lightgbm
   pip install xgboost
   ```
 9) Finally, install *deepBreaks*:
 install with pip:
 ```commandline
 pip install deepBreaks
 ```
@@ -151,96 +175,82 @@
 
 To test if deepBreaks is installed correctly, you may run the following command in the terminal:
 
 ```#!cmd
 deepBreaks -h
 ```
 Which yields deepBreaks command line options.
+
+
+
+## Options ##
+
+```
+$ deepBreaks -h
+```
+## Input ##
 ```commandline
-usage: deepBreaks [-h] --seqfile SEQFILE --seqtype SEQTYPE --meta_data META_DATA --metavar
-                  METAVAR [--gap GAP] --anatype {reg,cl}
+usage: deepBreaks [-h] --seqfile SEQFILE --seqtype SEQTYPE --meta_data META_DATA --metavar METAVAR [--gap GAP] [--miss_gap MISS_GAP]
+                  [--ult_rare ULT_RARE] --anatype {reg,cl}
                   [--distance_metric {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}]
-                  [--fraction FRACTION] [--redundant_threshold REDUNDANT_THRESHOLD]
-                  [--distance_threshold DISTANCE_THRESHOLD] [--top_models TOP_MODELS] [--plot]
-                  [--write]
+                  [--fraction FRACTION] [--redundant_threshold REDUNDANT_THRESHOLD] [--distance_threshold DISTANCE_THRESHOLD]
+                  [--top_models TOP_MODELS] [--cv CV] [--separate_cv] [--tune] [--plot] [--write]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --seqfile SEQFILE, -sf SEQFILE
                         files contains the sequences
   --seqtype SEQTYPE, -st SEQTYPE
                         type of sequence: 'nu' for nucleotides or 'aa' for amino-acid
   --meta_data META_DATA, -md META_DATA
                         files contains the meta data
   --metavar METAVAR, -mv METAVAR
                         name of the meta var (response variable)
-  --gap GAP, -gp GAP    Threshold to drop positions that have GAPs above this proportion.
-                        Default value is 0.7 and it means that the positions that 70% or more
-                        GAPs will be dropped from the analysis.
+  --gap GAP, -gp GAP    Threshold to drop positions that have GAPs above this proportion. Default value is 0.7 and it means that the positions that
+                        70% or more GAPs will be dropped from the analysis.
+  --miss_gap MISS_GAP, -mgp MISS_GAP
+                        Threshold to impute missing values with GAP. Gapsin positions that have missing values (gaps) above this proportionare
+                        replaced with the term 'GAP'. the rest of the missing valuesare replaced by the mode of each position.
+  --ult_rare ULT_RARE, -u ULT_RARE
+                        Threshold to modify the ultra rare cases in each position.
   --anatype {reg,cl}, -a {reg,cl}
                         type of analysis
   --distance_metric {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}, -dm {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}
                         distance metric. Default is correlation.
   --fraction FRACTION, -fr FRACTION
                         fraction of main data to run
   --redundant_threshold REDUNDANT_THRESHOLD, -rt REDUNDANT_THRESHOLD
-                        threshold for the p-value of the statistical tests to drop redundant
-                        features. Defaultvalue is 0.25
+                        threshold for the p-value of the statistical tests to drop redundant features. Defaultvalue is 0.25
   --distance_threshold DISTANCE_THRESHOLD, -dth DISTANCE_THRESHOLD
-                        threshold for the distance between positions to put them in clusters.
-                        features with distances <= than the threshold will be grouped together.
-                        Default values is 0.3
+                        threshold for the distance between positions to put them in clusters. features with distances <= than the threshold will be
+                        grouped together. Default values is 0.3
   --top_models TOP_MODELS, -tm TOP_MODELS
-                        number of top models to consider for merging the results. Default value
-                        is 5
-  --plot                plot all the individual positions that are statistically
-                        significant.Depending on your data, this process may produce many
+                        number of top models to consider for merging the results. Default value is 5
+  --cv CV, -cv CV       number of folds for cross validation. Default is 10. If the given number is less than 1,
+                        then instead of CV, a train/test split approach will be used with --cv being the test size. 
+  
+  --tune                After running the 10-fold cross validations, should the top selected models be tuned and finalize, or finalized only?
+  --plot                plot all the individual positions that are statistically significant.Depending on your data, this process may produce many
                         plots.
-  --write               During reading the fasta file we delete the positions that have GAPs
-                        over a certain threshold that can be changed in the `gap_threshold`
-                        argumentin the `read_data` function. As this may change the whole FASTA
-                        file, you maywant to save the FASTA file after this cleaning step.
-```
-
-
-## Options ##
+  --write               During reading the fasta file we delete the positions that have GAPs over a certain threshold that can be changed in the
+                        `gap_threshold` argumentin the `read_data` function. As this may change the whole FASTA file, you maywant to save the FASTA
+                        file after this cleaning step.
 
 ```
-$ deepBreaks -h
-```
-## Input ##
-1. `--seqfile` or `-sf` PATH to a sequence data file
-2. `--seqtype` or `-st` sequence type, values are `amino-acid` and `nu` for nucleotides
-3. `--meta_data` or `-md` PATH to metadata file
-4. `--metavar` or `-mv` name of the meta variable
-5. `--anatype` or `-a` analysis type, options are `reg` for regression and `cl` for classification
-6. `--fraction` or `-fr` fraction of the main data (sequence positions) to run. it is optional, 
-but you can enter a value between 0 and 1 to sample from the main data set.
-7. `--redundant_threshold` or `-rt` threshold for the p-value of the statistical 
-tests to drop redundant features. Default value is 0.25.
-8. `--distance_threshold` or `-dth` threshold for the distance between positions to put them in clusters. 
-features with distances <= than the threshold will be grouped together. Default values is 0.3.
-9. `--top_models` or `-tm` number of top models to consider for merging the results. Default value is 3
-10. `--plot` plot all the individual positions that are statistically significant. 
-Depending on your data, this process may produce many plots.
-11. `--gap` or `-gp` Threshold to drop positions that have GAPs above this proportion. 
-Default value is 0.7, and it means that the positions that 70% or more GAPs will be dropped from the analysis.
-12. `--write` During reading the fasta file we delete the positions that have GAPs over a  certain threshold that can 
-be changed in the `gap_threshold` argument in the `read_data` function. As this may change the whole FASTA file,
-you may want to save the FASTA file after this cleaning step.
 
 ## Output ##  
 1. correlated positions. We group all the colinear positions together.
 2. models summary. list of models and their performance metrics.
 3. plot of the feature importance of the top models in *modelName_dpi.png* format.
 4. csv files of feature importance based on top models containing, feature, importance, relative importance, 
 group of the position (we group all the colinear positions together)
 5. plots and csv file of average of feature importance of top models.
 6. box plot (regression) or stacked bar plot (classification) for top positions of each model.
-7. pickle files of the plots
+7. pickle files of the plots and final models
+8. p-values of all the variables used in training of the final model
 
 ## Demo ##
 ```commandline
 deepBreaks -sf PATH_TO_SEQUENCE.FASTA -st aa -md PATH_TO_META_DATA.tsv -mv
  META_VARIABLE_NAME -a reg  -dth 0.15 --plot --write
 ```
 
@@ -303,97 +313,110 @@
 To get the ful list of available metrics, you can use:
 ```python
 from sklearn import metrics
 print(metrics.SCORERS.keys())
 ```
 The default search parameters for the models are:
 ```python
+import numpy as np
 params = {
-        'rf': {
-            'max_depth': [4, 6, 8],
-            'n_estimators': [500, 1000]
-        },
-        'Adaboost': {
-            'learning_rate': [0.01, 0.05],
-            'n_estimators': [50, 100]
-        },
-        'et': {
-            'max_depth': [4, 6, 8],
-            'n_estimators': [500, 1000]
-        },
-        'dt': {
-            'max_depth': [4, 6, 8]
-        },
-        'Lasso': {
-            'alpha': [0.5, 1, 3]
-        },
-        'LassoLars': {
-            'alpha': [0.5, 1, 3]
-        }
+        'rf': {'rf__max_features': ["sqrt", "log2"]},
+        'Adaboost': {'Adaboost__learning_rate': np.linspace(0.001, 0.1, num=2),
+                     'Adaboost__n_estimators': [100, 200]},
+        'gbc': {'gbc__max_depth': range(3, 6),
+                'gbc__max_features': ['sqrt', 'log2'],
+                'gbc__n_estimators': [200, 500, 800],
+                'gbc__learning_rate': np.linspace(0.001, 0.1, num=2)},
+        'et': {'et__max_depth': [4, 6, 8],
+               'et__n_estimators': [500, 1000]},
+        'dt': {'dt__max_depth': [4, 6, 8]},
+        'Lasso': {'Lasso__alpha': np.linspace(0.01, 100, num=5)},
+        'LassoLars': {'LassoLars__alpha': np.linspace(0.01, 100, num=5)}
     }
 ```
 **Attention:** The names of models in the provided `dict` are the same with the names in the `dict` provided 
 for the `params`. If the name from the models `dict` does not match, the default `sklearn` parameters for that model
-is then used.  For example, `model_compare` uses the `xgboost` with default hyperparameters.  
+is then used.  For example, `model_compare_cv` uses the `xgboost` with default hyperparameters.  
 
-To use the `deepBreaks.models.model_compare` function with default parameters:
+To use the `deepBreaks.models.model_compare_cv` function with default parameters:
 ```python
-import deepBreaks.models as ml
+from deepBreaks.models import model_compare_cv
+from deepBreaks.preprocessing import MisCare, ConstantCare, URareCare, CustomOneHotEncoder
+from deepBreaks.preprocessing import FeatureSelection, CollinearCare
+from deepBreaks.utils import get_models, get_scores, get_params, make_pipeline
+
 ana_type = 'reg'  # assume that we are running a regression analysis
-trained_models = ml.model_compare(X_train, y_train, ana_type,
-                  cv=10, select_top=5,
-                  models=None, scores=None,
-                  params=None, sort_by=None,
-                  n_positions=None,
-                  grouped_features=None,
-                  report_dir='.')
+report_dir = 'PATH/TO/A/DIRECTORY' # to save the reports
+prep_pipeline = make_pipeline(cache_dir=None,
+    steps=[
+        ('mc', MisCare(missing_threshold=0.25)),
+        ('cc', ConstantCare()),
+        ('ur', URareCare(threshold=0.05)),
+        ('cc2', ConstantCare()),
+        ('one_hot', CustomOneHotEncoder()),
+        ('feature_selection', FeatureSelection(model_type=ana_type, alpha=0.25)),
+        ('collinear_care', CollinearCare(dist_method='correlation', threshold=0.25))
+    ])
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=get_models(ana_type=ana_type),
+                               scoring=get_scores(ana_type=ana_type),
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
+
 ```
 To use a new set of `models`, `params`, or `metrics` you can define them in a `dict`:
 ```python
 import deepBreaks.models as ml
 from sklearn.ensemble import RandomForestRegressor, AdaBoostRegressor
 from sklearn.ensemble import ExtraTreesRegressor
-        
-ana_type = 'reg'  # assume that we are running a regression analysis
+from deepBreaks.models import model_compare_cv
+from deepBreaks.preprocessing import MisCare, ConstantCare, URareCare, CustomOneHotEncoder
+from deepBreaks.preprocessing import FeatureSelection, CollinearCare
+from deepBreaks.utils import get_models, get_scores, get_params, make_pipeline
 
+ana_type = 'reg'  # assume that we are running a regression analysis
+report_dir = 'PATH/TO/A/DIRECTORY' # to save the reports
 # define a new set of models
 models = {'rf': RandomForestRegressor(n_jobs=-1, random_state=123),
           'Adaboost': AdaBoostRegressor(random_state=123),
           'et': ExtraTreesRegressor(n_jobs=-1, random_state=123)
           }
 
-# define a new set of params.
-params = {
-        'rf': {
-            'max_depth': [3, 5],
-            'n_estimators': [100]
-        },
-        'Adaboost': {
-            'learning_rate': [0.01, 0.05, 0.1],
-            'n_estimators': [50]
-        }
-    }
+
+prep_pipeline = make_pipeline(cache_dir=None,
+    steps=[
+        ('mc', MisCare(missing_threshold=0.25)),
+        ('cc', ConstantCare()),
+        ('ur', URareCare(threshold=0.05)),
+        ('cc2', ConstantCare()),
+        ('one_hot', CustomOneHotEncoder()),
+        ('feature_selection', FeatureSelection(model_type=ana_type, alpha=0.25)),
+        ('collinear_care', CollinearCare(dist_method='correlation', threshold=0.25))
+    ])
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=models,
+                               scoring=get_scores(ana_type=ana_type),
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
 
 '''
 Since we do not define a set of parameters for the model "et", it will fit with
 default parameters
 '''
 # change the set of metrics
 scores = {'R2': 'r2',
           'MAE': 'neg_mean_absolute_error',
           'MSE': 'neg_mean_squared_error'
           }
 
-trained_models = ml.model_compare(X_train, y_train, ana_type,
-                  cv=10, select_top=5,
-                  models=models, scores=scores,
-                  params=params, sort_by='MAE', # sort the models by "MAE" values
-                  n_positions=None,
-                  grouped_features=None,
-                  report_dir='.')
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=models,
+                               scoring=scores,
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
 ```
 
 # Applications #
 Here we try to use the **_deepBreaks_** on different datasets and elaborate on the results.
 
 <h2 id="opsin">
 <i>deepBreaks</i> identifies amino acids associated with color sensitivity
@@ -406,30 +429,30 @@
 amino acid sequence of rod opsins because previously published mutagenesis work established mechanistic connections
 between 12 specific amino acid sites and phenotypes [Yokoyama et al. (2008)](https://doi.org/10.1073/pnas.0802426105). 
 Therefore, we hypothesized that machine learning approaches could predict known associations between amino acid sites 
 and absorbance phenotypes. We identified opsins expressed in
 rod cells of vertebrates (mainly marine fishes) with absorption spectra measurements (λmax, the wavelength with the
 highest absorption). The dataset contains 175 samples of opsin sequences. We next applied deepBreaks on this
 dataset to find the most important sites contributing to the variations of λmax. 
-This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/continuous_phenotype.ipynb) 
+This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/continuous_phenotype_light_sensitivity.ipynb) 
 illustrates the steps.
 
 
 <h2 id="hmp">
 Novel insights of niche associations in the oral microbiome
 </h2>
 
 ![hmp](https://github.com/omicsEye/deepbreaks/blob/master/img/hmp/hmp.png?raw=True)  
 Microbial species tend to adapt at the genome level to the niche in which they live. We hypothesize 
 that genes with essential functions change based on where microbial species live. Here we use microbial strain 
 representatives from stool metagenomics data of healthy adults from the
 [Human Microbiome Project](https://doi.org/10.1038/nature11234). The input for deepBreaks consists of 1) an MSA file
 with 1006 rows, each a representative strain of a specific microbial species, here Haemophilus parainfluenzae, with
 49839 lengths; and 2) labels for deepBreaks prediction are body sites from which samples were collected. 
-This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype.ipynb)
+This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype_HMP.ipynb)
 illustrates the steps.
 
 
 <h2 id="covid">
 <i>deepBreaks</i> reveals important SARS-CoV-2 regions associated with Alpha and Delta variants
 </h2>
```

### Comparing `deepBreaks-1.0.2/deepBreaks/deepBreaks.py` & `deepBreaks-1.1.0/deepBreaks/deepBreaks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # importing libraries
-from deepBreaks.preprocessing import *
-from deepBreaks.models import *
-from deepBreaks.visualization import *
+# from deepBreaks.preprocessing import *
+# from deepBreaks.models import *
+# from deepBreaks.visualization import *
+from deepBreaks.utils import get_models, get_scores, get_params, make_pipeline
+from deepBreaks.preprocessing import MisCare, ConstantCare, URareCare, CustomOneHotEncoder, FeatureSelection, \
+    CollinearCare
+from deepBreaks.preprocessing import read_data, check_data, write_fasta, balanced_classes
+from deepBreaks.models import model_compare_cv, finalize_top, importance_from_pipe, mean_importance, summarize_results
+from deepBreaks.visualization import plot_scatter, dp_plot, plot_imp_model, plot_imp_all
+from sklearn.preprocessing import LabelEncoder
 import os
 import datetime
 import argparse
 import warnings
 import logging
 from zipfile import ZipFile
 
@@ -22,14 +29,17 @@
                                              "GAPs will be dropped from the analysis.",
                         type=float, default=0.7)
     parser.add_argument('--miss_gap', '-mgp', help="Threshold to impute missing values with GAP. Gaps"
                                                    "in positions that have missing values (gaps) above this proportion"
                                                    "are replaced with the term 'GAP'. the rest of the missing values"
                                                    "are replaced by the mode of each position.",
                         type=float, default=0.15)
+    parser.add_argument('--ult_rare', '-u', help="Threshold to modify the ultra rare cases in each position.",
+                        type=float, default=0.025)
+
     parser.add_argument('--anatype', '-a', help="type of analysis", choices=['reg', 'cl'], type=str, required=True)
     parser.add_argument('--distance_metric', '-dm',
                         help="distance metric. Default is correlation.",
                         choices=['correlation', 'hamming', 'jaccard',
                                  'normalized_mutual_info_score',
                                  'adjusted_mutual_info_score', 'adjusted_rand_score'],
                         type=str, default='correlation')
@@ -41,15 +51,24 @@
     parser.add_argument('--distance_threshold', '-dth',
                         help="threshold for the distance between positions to put them in clusters. "
                              "features with distances <= than the threshold will be grouped together. Default "
                              "values is 0.3",
                         type=float, default=0.3)
     parser.add_argument('--top_models', '-tm',
                         help="number of top models to consider for merging the results. Default value is 5",
-                        type=int, default=5)
+                        type=int, default=3)
+    parser.add_argument('--cv', '-cv',
+                        help="number of folds for cross validation. Default is 10. If the given number is less than 1,"
+                             " then instead of CV, a train/test split approach will be used with "
+                             "cv being the test size.",
+                        type=float, default=10)
+
+    parser.add_argument("--tune", help="After running the 10-fold cross validations, should the top selected models be"
+                                       " tuned and finalize, or finalized only?",
+                        action="store_true", default=False)
     parser.add_argument("--plot", help="plot all the individual positions that are statistically significant."
                                        "Depending on your data, this process may produce many plots.",
                         action="store_true", default=False)
     parser.add_argument("--write", help="During reading the fasta file we delete the positions that have GAPs over a "
                                         "certain threshold that can be changed in the `gap_threshold` argument"
                                         "in the `read_data` function. As this may change the whole FASTA file, you may"
                                         "want to save the FASTA file after this cleaning step.",
@@ -62,29 +81,32 @@
     # Parse arguments from command line
     warnings.filterwarnings("ignore")
     warnings.simplefilter('ignore')
 
     args = parse_arguments()
     print(args)  # printing Namespace
     if args.seqtype not in ['nu', 'aa']:
-        print('For sequence data type, please enter "nu" for nucleotide or "aa" for amino-acid sequences.')
+        raise Exception('For sequence data type, please enter "nu" for nucleotide or "aa" for amino-acid sequences.')
         exit()
 
     if args.anatype not in ['reg', 'cl']:
-        print('For analysis type, please enter "reg" for regression or "cl" for classification only')
+        raise Exception('For analysis type, please enter "reg" for regression or "cl" for classification only')
+        exit()
+    if args.cv == 1:
+        raise Exception('cv can not be equal to 1')
         exit()
     # making directory
     print('directory preparation')
     dt_label = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
     seq_file_name = args.seqfile.split('.')[0]
 
     report_dir = str(seq_file_name + '_' + args.metavar + '_' + dt_label)
     os.makedirs(report_dir)
 
-    logging.basicConfig(filename=report_dir+"/log.txt", level=logging.DEBUG,
+    logging.basicConfig(filename=report_dir + "/log.txt", level=logging.DEBUG,
                         format="%(asctime)s %(message)s")
 
     logging.info("The parameters are{}".format(args))
     print('reading meta-data')
     meta_data = read_data(args.meta_data, seq_type=None, is_main=False)
     print('meta_data:', meta_data.shape)
 
@@ -93,92 +115,119 @@
 
     # importing seq data
     print('reading fasta file')
     df = read_data(args.seqfile, seq_type=args.seqtype, gap_threshold=args.gap, is_main=True)
 
     if args.write:
         print('Writing cleaned FASTA file')
-        write_fasta(dat=df, fasta_file=seq_file_name+'_clean.fasta', report_dir=report_dir)
+        write_fasta(dat=df, fasta_file=seq_file_name + '_clean.fasta', report_dir=report_dir)
 
     positions = df.shape[1]
     print('Done')
     print('Shape of data is: ', df.shape)
     logging.info("Shape of data is {}".format(df.shape))
     # selecting only more frequent classes
     if args.anatype == 'cl':
         df = balanced_classes(dat=df, meta_dat=meta_data, feature=args.metavar)
 
-    # taking care of missing data
-    print('Shape of data before missing/constant care: ', df.shape)
-    df = missing_constant_care(df, missing_threshold=args.miss_gap)
-    print('Shape of data after missing/constant care: ', df.shape)
-    logging.info("Shape of data after missing/constant care: {}".format(df.shape))
-
-    print('Shape of data before imbalanced care: ', df.shape)
-    df = imb_care(dat=df, imbalance_threshold=0.05)
-    print('Shape of data after imbalanced care: ', df.shape)
-    logging.info("Shape of data after imbalanced care care: {}".format(df.shape))
-
-    if args.fraction is not None:
-        print('number of columns of main data before: ', df.shape[1])
-        df = col_sampler(dat=df, sample_frac=args.fraction)
-        print('number of columns of main data after: ', df.shape[1])
-
-    print('Statistical tests to drop redundant features')
-    df_cleaned = redundant_drop(dat=df, meta_dat=meta_data, feature=args.metavar, model_type=args.anatype,
-                                report_dir=report_dir, threshold=args.redundant_threshold)
-    if df_cleaned is None:
-        exit()
+    df = df.merge(meta_data.loc[:, args.metavar], left_index=True, right_index=True)
+    y = df.loc[:, args.metavar].values
+    df.drop(args.metavar, axis=1, inplace=True)
 
-    print('Shape of data after dropping redundant columns: ', df_cleaned.shape)
-    logging.info("Shape of data after dropping redundant columns: {}".format(df_cleaned.shape))
+    if args.anatype == 'cl':
+        le = LabelEncoder()
+        y = le.fit_transform(y)
 
-    print('prepare dummy variables')
-    df_cleaned = get_dummies(dat=df_cleaned, drop_first=True)
-    print('correlation analysis')
-    cr = distance_calc(dat=df_cleaned, dist_method=args.distance_metric, report_dir=report_dir)
-    print('finding collinear groups')
-    dc_df = db_grouped(dat=cr, report_dir=report_dir, threshold=args.distance_threshold)
-    print('grouping features')
-    dc = group_features(dat=df_cleaned, group_dat=dc_df, report_dir=report_dir)
-    print('dropping correlated features')
-    print('Shape of data before linearity care: ', df_cleaned.shape)
-    df_cleaned = cor_remove(df_cleaned, dc)
-    print('Shape of data after linearity care: ', df_cleaned.shape)
-    logging.info("Shape of data after linearity care: {}".format(df_cleaned.shape))
-    # merge with meta data
-    df = df.merge(meta_data[args.metavar], left_index=True, right_index=True)
-    df_cleaned = df_cleaned.merge(meta_data[args.metavar], left_index=True, right_index=True)
-    logging.info("Shape of data after joining with meta_data: {}".format(df_cleaned.shape))
-
-    # model
-    print('Training the models...')
-    logging.info("Training the models...")
-    select_top = args.top_models
-    trained_models = model_compare(X_train=df_cleaned.loc[:, df_cleaned.columns != args.metavar],
-                                   y_train=df_cleaned.loc[:, args.metavar], n_positions=positions,
-                                   grouped_features=dc, report_dir=report_dir, ana_type=args.anatype,
-                                   select_top=select_top)
+    if args.cv > 1:
+        args.cv = int(args.cv)
+        print(f'Running a {args.cv}-fold cross-validation.')
+    else:
+        print(f'Performing a {args.cv*100}% train-test split.')
+
+    prep_pipeline = make_pipeline(
+        steps=[
+            ('mc', MisCare(missing_threshold=args.miss_gap)),
+            ('cc', ConstantCare()),
+            ('ur', URareCare(threshold=args.ult_rare)),
+            ('cc2', ConstantCare()),
+            ('one_hot', CustomOneHotEncoder()),
+            ('feature_selection', FeatureSelection(model_type=args.anatype, alpha=args.redundant_threshold)),
+            ('collinear_care', CollinearCare(dist_method=args.distance_metric, threshold=args.distance_threshold))
+        ])
+
+    # fit and compare models
+    report, top = model_compare_cv(X=df, y=y, preprocess_pipe=prep_pipeline,
+                                   models_dict=get_models(ana_type=args.anatype),
+                                   scoring=get_scores(ana_type=args.anatype),
+                                   report_dir=report_dir,
+                                   cv=args.cv, ana_type=args.anatype, cache_dir=None)
+
+    prep_pipeline = make_pipeline(
+        steps=[
+            ('mc', MisCare(missing_threshold=args.miss_gap)),
+            ('cc', ConstantCare()),
+            ('ur', URareCare(threshold=args.ult_rare)),
+            ('cc2', ConstantCare()),
+            ('one_hot', CustomOneHotEncoder()),
+            ('feature_selection', FeatureSelection(model_type=args.anatype,
+                                                   alpha=args.redundant_threshold, keep=True)),
+            ('collinear_care', CollinearCare(dist_method=args.distance_metric,
+                                             threshold=args.distance_threshold, keep=True))
+        ])
+
+    modified_top = []
+    for model in top:
+        modified_top.append(make_pipeline(steps=[('prep', prep_pipeline), model.steps[-1]]))
+
+    if args.tune:
+        top = finalize_top(X=df, y=y, top_models=modified_top, grid_param=get_params(),
+                           report_dir=report_dir, cv=args.cv)
+    else:
+        top = finalize_top(X=df, y=y, top_models=modified_top, grid_param={},
+                           report_dir=report_dir, cv=args.cv)
+
+    n_positions = None
+    grouped_features = None
+    p_values = None
+    corr_mat = None
+
+    sr = summarize_results(top_models=top, grouped_features=grouped_features,
+                           p_values=p_values, cor_mat=corr_mat, report_dir=report_dir)
+    mean_imp = mean_importance(top_models=top, n_positions=n_positions,
+                               grouped_features=grouped_features, report_dir=report_dir)
 
     print('Visualizing the results...')
     logging.info("Visualizing the results...")
-    for key in trained_models.keys():
-        if key == 'mean':
-            dp_plot(importance=trained_models[key], imp_col='mean', model_name=key, annotate=2, report_dir=report_dir)
-        else:
-            dp_plot(importance=trained_models[key]['importance'], imp_col='standard_value',
-                    model_name=key, annotate=2, report_dir=report_dir)
-            plot_imp_model(importance=trained_models[key]['importance'],
-                           X_train=df.loc[:, df.columns != args.metavar], y_train=df.loc[:, args.metavar],
-                           meta_var=args.metavar, model_type=args.anatype, model_name=key, report_dir=report_dir)
+
+    scatter_plot = plot_scatter(summary_result=sr, report_dir=report_dir)
+    dp_plot(importance=mean_imp, imp_col='mean', model_name='mean', report_dir=report_dir)
+
+    df = prep_pipeline[:4].fit_transform(df)
+    if args.anatype == 'cl':
+        y = le.inverse_transform(y)
+
+    for model in top:
+        model_name = model.steps[-1][0]
+        dp_plot(importance=importance_from_pipe(model=model, grouped_features=grouped_features,
+                                                n_positions=n_positions),
+                imp_col='standard_value',
+                model_name=model_name, report_dir=report_dir)
+
+        plot_imp_model(importance=importance_from_pipe(model=model, grouped_features=grouped_features,
+                                                       n_positions=n_positions),
+                       X_train=df, y_train=y, model_name=model_name,
+                       meta_var=args.metavar, model_type=args.anatype, report_dir=report_dir)
 
     if args.plot:
-        plot_imp_all(trained_models=trained_models,
-                     X_train=df.loc[:, df.columns != args.metavar], y_train=df.loc[:, args.metavar],
-                     meta_var=args.metavar, model_type=args.anatype, report_dir=report_dir, max_plots=100)
+        plot_imp_all(final_models=top,
+                     X_train=df, y_train=y,
+                     meta_var=args.metavar, model_type=args.anatype,
+                     n_positions=n_positions, grouped_features=grouped_features,
+                     report_dir=report_dir, max_plots=100,
+                     figsize=(1.85, 3))
 
     zip_obj = ZipFile(str(report_dir + '/report.zip'), 'w')
     file_names = os.listdir(report_dir)
     for file in file_names:
         if not file.endswith('.zip'):
             zip_obj.write(str(report_dir + '/' + file))
     logging.info("done!")
```

### Comparing `deepBreaks-1.0.2/deepBreaks.egg-info/PKG-INFO` & `deepBreaks-1.1.0/deepBreaks.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepBreaks
-Version: 1.0.2
+Version: 1.1.0
 Summary: deepBreaks: a machine learning tool for identifying and prioritizing genotype-phenotype associations
 Home-page: http://github.com/omicsEye/deepBreaks
 Author: Mahdi Baghbanzadeh
 Author-email: mbagh@gwu.edu
 License: MIT
 Keywords: machine learning,genomics,sequencing data
 Platform: Linux
@@ -151,15 +151,15 @@
   ```
 7) Activate the conda environment
   ```commandline
   conda activate deepBreaks_env
   ```
 8) Install packages from Conda
   ```commandline
-  conda install lightgbm
+  conda install -c conda-forge lightgbm
   pip install xgboost
   ```
 9) Finally, install *deepBreaks*:
 install with pip:
 ```commandline
 pip install deepBreaks
 ```
@@ -175,96 +175,82 @@
 
 To test if deepBreaks is installed correctly, you may run the following command in the terminal:
 
 ```#!cmd
 deepBreaks -h
 ```
 Which yields deepBreaks command line options.
+
+
+
+## Options ##
+
+```
+$ deepBreaks -h
+```
+## Input ##
 ```commandline
-usage: deepBreaks [-h] --seqfile SEQFILE --seqtype SEQTYPE --meta_data META_DATA --metavar
-                  METAVAR [--gap GAP] --anatype {reg,cl}
+usage: deepBreaks [-h] --seqfile SEQFILE --seqtype SEQTYPE --meta_data META_DATA --metavar METAVAR [--gap GAP] [--miss_gap MISS_GAP]
+                  [--ult_rare ULT_RARE] --anatype {reg,cl}
                   [--distance_metric {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}]
-                  [--fraction FRACTION] [--redundant_threshold REDUNDANT_THRESHOLD]
-                  [--distance_threshold DISTANCE_THRESHOLD] [--top_models TOP_MODELS] [--plot]
-                  [--write]
+                  [--fraction FRACTION] [--redundant_threshold REDUNDANT_THRESHOLD] [--distance_threshold DISTANCE_THRESHOLD]
+                  [--top_models TOP_MODELS] [--cv CV] [--separate_cv] [--tune] [--plot] [--write]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --seqfile SEQFILE, -sf SEQFILE
                         files contains the sequences
   --seqtype SEQTYPE, -st SEQTYPE
                         type of sequence: 'nu' for nucleotides or 'aa' for amino-acid
   --meta_data META_DATA, -md META_DATA
                         files contains the meta data
   --metavar METAVAR, -mv METAVAR
                         name of the meta var (response variable)
-  --gap GAP, -gp GAP    Threshold to drop positions that have GAPs above this proportion.
-                        Default value is 0.7 and it means that the positions that 70% or more
-                        GAPs will be dropped from the analysis.
+  --gap GAP, -gp GAP    Threshold to drop positions that have GAPs above this proportion. Default value is 0.7 and it means that the positions that
+                        70% or more GAPs will be dropped from the analysis.
+  --miss_gap MISS_GAP, -mgp MISS_GAP
+                        Threshold to impute missing values with GAP. Gapsin positions that have missing values (gaps) above this proportionare
+                        replaced with the term 'GAP'. the rest of the missing valuesare replaced by the mode of each position.
+  --ult_rare ULT_RARE, -u ULT_RARE
+                        Threshold to modify the ultra rare cases in each position.
   --anatype {reg,cl}, -a {reg,cl}
                         type of analysis
   --distance_metric {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}, -dm {correlation,hamming,jaccard,normalized_mutual_info_score,adjusted_mutual_info_score,adjusted_rand_score}
                         distance metric. Default is correlation.
   --fraction FRACTION, -fr FRACTION
                         fraction of main data to run
   --redundant_threshold REDUNDANT_THRESHOLD, -rt REDUNDANT_THRESHOLD
-                        threshold for the p-value of the statistical tests to drop redundant
-                        features. Defaultvalue is 0.25
+                        threshold for the p-value of the statistical tests to drop redundant features. Defaultvalue is 0.25
   --distance_threshold DISTANCE_THRESHOLD, -dth DISTANCE_THRESHOLD
-                        threshold for the distance between positions to put them in clusters.
-                        features with distances <= than the threshold will be grouped together.
-                        Default values is 0.3
+                        threshold for the distance between positions to put them in clusters. features with distances <= than the threshold will be
+                        grouped together. Default values is 0.3
   --top_models TOP_MODELS, -tm TOP_MODELS
-                        number of top models to consider for merging the results. Default value
-                        is 5
-  --plot                plot all the individual positions that are statistically
-                        significant.Depending on your data, this process may produce many
+                        number of top models to consider for merging the results. Default value is 5
+  --cv CV, -cv CV       number of folds for cross validation. Default is 10. If the given number is less than 1,
+                        then instead of CV, a train/test split approach will be used with --cv being the test size. 
+  
+  --tune                After running the 10-fold cross validations, should the top selected models be tuned and finalize, or finalized only?
+  --plot                plot all the individual positions that are statistically significant.Depending on your data, this process may produce many
                         plots.
-  --write               During reading the fasta file we delete the positions that have GAPs
-                        over a certain threshold that can be changed in the `gap_threshold`
-                        argumentin the `read_data` function. As this may change the whole FASTA
-                        file, you maywant to save the FASTA file after this cleaning step.
-```
-
-
-## Options ##
+  --write               During reading the fasta file we delete the positions that have GAPs over a certain threshold that can be changed in the
+                        `gap_threshold` argumentin the `read_data` function. As this may change the whole FASTA file, you maywant to save the FASTA
+                        file after this cleaning step.
 
 ```
-$ deepBreaks -h
-```
-## Input ##
-1. `--seqfile` or `-sf` PATH to a sequence data file
-2. `--seqtype` or `-st` sequence type, values are `amino-acid` and `nu` for nucleotides
-3. `--meta_data` or `-md` PATH to metadata file
-4. `--metavar` or `-mv` name of the meta variable
-5. `--anatype` or `-a` analysis type, options are `reg` for regression and `cl` for classification
-6. `--fraction` or `-fr` fraction of the main data (sequence positions) to run. it is optional, 
-but you can enter a value between 0 and 1 to sample from the main data set.
-7. `--redundant_threshold` or `-rt` threshold for the p-value of the statistical 
-tests to drop redundant features. Default value is 0.25.
-8. `--distance_threshold` or `-dth` threshold for the distance between positions to put them in clusters. 
-features with distances <= than the threshold will be grouped together. Default values is 0.3.
-9. `--top_models` or `-tm` number of top models to consider for merging the results. Default value is 3
-10. `--plot` plot all the individual positions that are statistically significant. 
-Depending on your data, this process may produce many plots.
-11. `--gap` or `-gp` Threshold to drop positions that have GAPs above this proportion. 
-Default value is 0.7, and it means that the positions that 70% or more GAPs will be dropped from the analysis.
-12. `--write` During reading the fasta file we delete the positions that have GAPs over a  certain threshold that can 
-be changed in the `gap_threshold` argument in the `read_data` function. As this may change the whole FASTA file,
-you may want to save the FASTA file after this cleaning step.
 
 ## Output ##  
 1. correlated positions. We group all the colinear positions together.
 2. models summary. list of models and their performance metrics.
 3. plot of the feature importance of the top models in *modelName_dpi.png* format.
 4. csv files of feature importance based on top models containing, feature, importance, relative importance, 
 group of the position (we group all the colinear positions together)
 5. plots and csv file of average of feature importance of top models.
 6. box plot (regression) or stacked bar plot (classification) for top positions of each model.
-7. pickle files of the plots
+7. pickle files of the plots and final models
+8. p-values of all the variables used in training of the final model
 
 ## Demo ##
 ```commandline
 deepBreaks -sf PATH_TO_SEQUENCE.FASTA -st aa -md PATH_TO_META_DATA.tsv -mv
  META_VARIABLE_NAME -a reg  -dth 0.15 --plot --write
 ```
 
@@ -327,97 +313,110 @@
 To get the ful list of available metrics, you can use:
 ```python
 from sklearn import metrics
 print(metrics.SCORERS.keys())
 ```
 The default search parameters for the models are:
 ```python
+import numpy as np
 params = {
-        'rf': {
-            'max_depth': [4, 6, 8],
-            'n_estimators': [500, 1000]
-        },
-        'Adaboost': {
-            'learning_rate': [0.01, 0.05],
-            'n_estimators': [50, 100]
-        },
-        'et': {
-            'max_depth': [4, 6, 8],
-            'n_estimators': [500, 1000]
-        },
-        'dt': {
-            'max_depth': [4, 6, 8]
-        },
-        'Lasso': {
-            'alpha': [0.5, 1, 3]
-        },
-        'LassoLars': {
-            'alpha': [0.5, 1, 3]
-        }
+        'rf': {'rf__max_features': ["sqrt", "log2"]},
+        'Adaboost': {'Adaboost__learning_rate': np.linspace(0.001, 0.1, num=2),
+                     'Adaboost__n_estimators': [100, 200]},
+        'gbc': {'gbc__max_depth': range(3, 6),
+                'gbc__max_features': ['sqrt', 'log2'],
+                'gbc__n_estimators': [200, 500, 800],
+                'gbc__learning_rate': np.linspace(0.001, 0.1, num=2)},
+        'et': {'et__max_depth': [4, 6, 8],
+               'et__n_estimators': [500, 1000]},
+        'dt': {'dt__max_depth': [4, 6, 8]},
+        'Lasso': {'Lasso__alpha': np.linspace(0.01, 100, num=5)},
+        'LassoLars': {'LassoLars__alpha': np.linspace(0.01, 100, num=5)}
     }
 ```
 **Attention:** The names of models in the provided `dict` are the same with the names in the `dict` provided 
 for the `params`. If the name from the models `dict` does not match, the default `sklearn` parameters for that model
-is then used.  For example, `model_compare` uses the `xgboost` with default hyperparameters.  
+is then used.  For example, `model_compare_cv` uses the `xgboost` with default hyperparameters.  
 
-To use the `deepBreaks.models.model_compare` function with default parameters:
+To use the `deepBreaks.models.model_compare_cv` function with default parameters:
 ```python
-import deepBreaks.models as ml
+from deepBreaks.models import model_compare_cv
+from deepBreaks.preprocessing import MisCare, ConstantCare, URareCare, CustomOneHotEncoder
+from deepBreaks.preprocessing import FeatureSelection, CollinearCare
+from deepBreaks.utils import get_models, get_scores, get_params, make_pipeline
+
 ana_type = 'reg'  # assume that we are running a regression analysis
-trained_models = ml.model_compare(X_train, y_train, ana_type,
-                  cv=10, select_top=5,
-                  models=None, scores=None,
-                  params=None, sort_by=None,
-                  n_positions=None,
-                  grouped_features=None,
-                  report_dir='.')
+report_dir = 'PATH/TO/A/DIRECTORY' # to save the reports
+prep_pipeline = make_pipeline(cache_dir=None,
+    steps=[
+        ('mc', MisCare(missing_threshold=0.25)),
+        ('cc', ConstantCare()),
+        ('ur', URareCare(threshold=0.05)),
+        ('cc2', ConstantCare()),
+        ('one_hot', CustomOneHotEncoder()),
+        ('feature_selection', FeatureSelection(model_type=ana_type, alpha=0.25)),
+        ('collinear_care', CollinearCare(dist_method='correlation', threshold=0.25))
+    ])
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=get_models(ana_type=ana_type),
+                               scoring=get_scores(ana_type=ana_type),
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
+
 ```
 To use a new set of `models`, `params`, or `metrics` you can define them in a `dict`:
 ```python
 import deepBreaks.models as ml
 from sklearn.ensemble import RandomForestRegressor, AdaBoostRegressor
 from sklearn.ensemble import ExtraTreesRegressor
-        
-ana_type = 'reg'  # assume that we are running a regression analysis
+from deepBreaks.models import model_compare_cv
+from deepBreaks.preprocessing import MisCare, ConstantCare, URareCare, CustomOneHotEncoder
+from deepBreaks.preprocessing import FeatureSelection, CollinearCare
+from deepBreaks.utils import get_models, get_scores, get_params, make_pipeline
 
+ana_type = 'reg'  # assume that we are running a regression analysis
+report_dir = 'PATH/TO/A/DIRECTORY' # to save the reports
 # define a new set of models
 models = {'rf': RandomForestRegressor(n_jobs=-1, random_state=123),
           'Adaboost': AdaBoostRegressor(random_state=123),
           'et': ExtraTreesRegressor(n_jobs=-1, random_state=123)
           }
 
-# define a new set of params.
-params = {
-        'rf': {
-            'max_depth': [3, 5],
-            'n_estimators': [100]
-        },
-        'Adaboost': {
-            'learning_rate': [0.01, 0.05, 0.1],
-            'n_estimators': [50]
-        }
-    }
+
+prep_pipeline = make_pipeline(cache_dir=None,
+    steps=[
+        ('mc', MisCare(missing_threshold=0.25)),
+        ('cc', ConstantCare()),
+        ('ur', URareCare(threshold=0.05)),
+        ('cc2', ConstantCare()),
+        ('one_hot', CustomOneHotEncoder()),
+        ('feature_selection', FeatureSelection(model_type=ana_type, alpha=0.25)),
+        ('collinear_care', CollinearCare(dist_method='correlation', threshold=0.25))
+    ])
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=models,
+                               scoring=get_scores(ana_type=ana_type),
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
 
 '''
 Since we do not define a set of parameters for the model "et", it will fit with
 default parameters
 '''
 # change the set of metrics
 scores = {'R2': 'r2',
           'MAE': 'neg_mean_absolute_error',
           'MSE': 'neg_mean_squared_error'
           }
 
-trained_models = ml.model_compare(X_train, y_train, ana_type,
-                  cv=10, select_top=5,
-                  models=models, scores=scores,
-                  params=params, sort_by='MAE', # sort the models by "MAE" values
-                  n_positions=None,
-                  grouped_features=None,
-                  report_dir='.')
+report, top = model_compare_cv(X=tr, y=y, preprocess_pipe=prep_pipeline,
+                               models_dict=models,
+                               scoring=scores,
+                               report_dir=report_dir,
+                               cv=10, ana_type=ana_type, cache_dir=None)
 ```
 
 # Applications #
 Here we try to use the **_deepBreaks_** on different datasets and elaborate on the results.
 
 <h2 id="opsin">
 <i>deepBreaks</i> identifies amino acids associated with color sensitivity
@@ -430,30 +429,30 @@
 amino acid sequence of rod opsins because previously published mutagenesis work established mechanistic connections
 between 12 specific amino acid sites and phenotypes [Yokoyama et al. (2008)](https://doi.org/10.1073/pnas.0802426105). 
 Therefore, we hypothesized that machine learning approaches could predict known associations between amino acid sites 
 and absorbance phenotypes. We identified opsins expressed in
 rod cells of vertebrates (mainly marine fishes) with absorption spectra measurements (λmax, the wavelength with the
 highest absorption). The dataset contains 175 samples of opsin sequences. We next applied deepBreaks on this
 dataset to find the most important sites contributing to the variations of λmax. 
-This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/continuous_phenotype.ipynb) 
+This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/continuous_phenotype_light_sensitivity.ipynb) 
 illustrates the steps.
 
 
 <h2 id="hmp">
 Novel insights of niche associations in the oral microbiome
 </h2>
 
 ![hmp](https://github.com/omicsEye/deepbreaks/blob/master/img/hmp/hmp.png?raw=True)  
 Microbial species tend to adapt at the genome level to the niche in which they live. We hypothesize 
 that genes with essential functions change based on where microbial species live. Here we use microbial strain 
 representatives from stool metagenomics data of healthy adults from the
 [Human Microbiome Project](https://doi.org/10.1038/nature11234). The input for deepBreaks consists of 1) an MSA file
 with 1006 rows, each a representative strain of a specific microbial species, here Haemophilus parainfluenzae, with
 49839 lengths; and 2) labels for deepBreaks prediction are body sites from which samples were collected. 
-This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype.ipynb)
+This [Jupyter Notebook](https://github.com/omicsEye/deepbreaks/blob/master/examples/discrete_phenotype_HMP.ipynb)
 illustrates the steps.
 
 
 <h2 id="covid">
 <i>deepBreaks</i> reveals important SARS-CoV-2 regions associated with Alpha and Delta variants
 </h2>
```

### Comparing `deepBreaks-1.0.2/setup.py` & `deepBreaks-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering :: Bio-Informatics"
     ]
 
-VERSION = "1.0.2"
+VERSION = "1.1.0"
 AUTHOR = "Mahdi Baghbanzadeh"
 AUTHOR_EMAIL = "mbagh@gwu.edu"
 MAINTAINER = "Mahdi Baghbanzadeh"
 MAINTAINER_EMAIL = "mbagh@gwu.edu"
 
 # try to download the bitbucket counter file to count downloads
 # this has been added since PyPI has turned off the download stats
@@ -73,15 +73,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/omicsEye/deepBreaks",
     keywords=['machine learning', 'genomics', 'sequencing data'],
     platforms=['Linux', 'MacOS', "Windows"],
     classifiers=classifiers,
     # long_description=open('readme.md').read(),
-
+    data_files=[('.', ['requirements.txt'])],
     install_requires=required,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'deepBreaks = deepBreaks.deepBreaks:main'
         ]},
     test_suite='deepBreaks.tests.deepBreaks_test',
```

